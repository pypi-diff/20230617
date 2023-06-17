# Comparing `tmp/nsdpy-0.3.5b0.tar.gz` & `tmp/nsdpy-0.3.6b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsdpy-0.3.5b0.tar", max compression
+gzip compressed data, was "nsdpy-0.3.6b0.tar", max compression
```

## Comparing `nsdpy-0.3.5b0.tar` & `nsdpy-0.3.6b0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2023-05-29 18:26:14.471852 nsdpy-0.3.5b0/LICENSE
--rw-r--r--   0        0        0     2720 2023-05-29 18:26:14.472080 nsdpy-0.3.5b0/README.md
--rw-r--r--   0        0        0    35941 2023-06-04 14:52:45.584025 nsdpy-0.3.5b0/functions.py
--rw-r--r--   0        0        0    13024 2023-06-04 14:53:26.111581 nsdpy-0.3.5b0/nsdpy.py
--rw-r--r--   0        0        0      841 2023-06-04 14:53:27.677228 nsdpy-0.3.5b0/pyproject.toml
--rw-r--r--   0        0        0     3730 1970-01-01 00:00:00.000000 nsdpy-0.3.5b0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-29 18:26:14.471852 nsdpy-0.3.6b0/LICENSE
+-rw-r--r--   0        0        0     2720 2023-05-29 18:26:14.472080 nsdpy-0.3.6b0/README.md
+-rw-r--r--   0        0        0    37320 2023-06-17 14:13:34.144899 nsdpy-0.3.6b0/functions.py
+-rw-r--r--   0        0        0    13273 2023-06-17 14:15:00.690285 nsdpy-0.3.6b0/nsdpy.py
+-rw-r--r--   0        0        0      841 2023-06-17 14:15:20.968769 nsdpy-0.3.6b0/pyproject.toml
+-rw-r--r--   0        0        0     3730 1970-01-01 00:00:00.000000 nsdpy-0.3.6b0/PKG-INFO
```

### Comparing `nsdpy-0.3.5b0/LICENSE` & `nsdpy-0.3.6b0/LICENSE`

 * *Files identical despite different names*

### Comparing `nsdpy-0.3.5b0/README.md` & `nsdpy-0.3.6b0/README.md`

 * *Files identical despite different names*

### Comparing `nsdpy-0.3.5b0/functions.py` & `nsdpy-0.3.6b0/functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -189,34 +189,43 @@
 
 def dispatch(lineage, classif):
     """
         take the lineage of a sequence and the classification option and return the base name of the file to store 
         the sequence.
 
         INPUTS: dispatch(lineage, classif) 
-            lineage: LIST
-            classif: INT or LIST
+            lineage: List or Dict
+            classif: Int or List
     """
     ## no option selected
     if classif == 2:
         return "sequences"
+    
+    ## user gave list of taxonomic levels (option -l --levels)
+    if isinstance(classif, str):
+        ## type checking
+        if not isinstance(lineage, dict):
+            return "OTHERS"
+    
     ## user gave list of taxonomic levels (option -l --levels)
     if isinstance(classif, list):
         try:
             other = [rank for rank in lineage if rank in classif][0]
         except IndexError:
             other = "OTHERS"
         return other
+    
     ## phylums
     if classif == 0:
         try:
             Phylum = [phy for phy in lineage if phy in METAZOA or phy in FUNGI or phy in PLANTAE][0]
         except IndexError:
             Phylum = 'OTHERS'
         return Phylum
+    
     ## kingdoms
     if classif == 1:
         if 'METAZOA' in lineage or len(list(set(lineage) & set(METAZOA))) > 0:
             kingdom = "METAZOA"
         elif "ViridiPLANTAE" in lineage or len(list(set(lineage) & set(PLANTAE))) > 0:
             kingdom = "PLANTAE" 
         elif "FUNGI" in  lineage or len(list(set(lineage) & set(FUNGI))) > 0:
@@ -297,44 +306,36 @@
                 _, Name = Name.split('<ScientificName>', 1)    
             except ValueError:
                 Name = 'not found'
             dicttemp['Name'] = Name
 
             try:
                 Lineage , _ = seq.split('</Lineage>', 1)
-                _, Lineage = Lineage.split('<Lineage>', 1)    
+                _, Lineage = Lineage.split('<Lineage>', 1)  
             except ValueError:
                 Lineage = 'not found'
             lineage = Lineage.split('; ')
             dicttemp['Lineage'] = lineage
 
             ## dispatch
-            dicttemp['dispatch'] = dispatch(lineage, classif)
+            if isinstance(classif, str):
+                lineage = parseClassifXML(seq)
+                if classif in lineage.keys():
+                    dicttemp['dispatch'] = lineage[classif].replace(' ', '_')
+                else: 
+                    dicttemp['dispatch'] = 'OTHERS'
+            else:
+                dicttemp['dispatch'] = dispatch(lineage, classif)
 
             data[TaxId] = dicttemp
 
     # comments
     if verb and verb > 0:
         print(f'number of taxids:\t{len(data.keys())}')
 
-    if verb and verb > 0:
-        dup = {}
-        duplicate = 0
-        for TaxId in data.keys():
-            if data[TaxId]['dispatch'] in dup.keys():
-                duplicate = duplicate + 1
-                dup[data[TaxId]['dispatch']] = dup[data[TaxId]['dispatch']] + [TaxId]
-            else: 
-                dup[data[TaxId]['dispatch']] = [TaxId]
-        print('--------------- DUPLICATES ---------------')
-        print(f'Number of taxa for which more than one TaxId has been found: {duplicate}')
-        for key in dup.keys():
-            if len(dup[key]) > 1:
-                print(f'{key}: {dup[key]}')
-        print('------------------------------------------')
     return data
 
 
 ## Download the CDS fasta files by batch of 'retmax' for the seq access found by an esearch request returning a querykey and a webenv variable
 def cds_fasta(path, dict_ids, dict_taxo, QUERY, list_of_ids, OPTIONS=None):
 
     if OPTIONS is None:
@@ -971,11 +972,53 @@
         if information:
             writer.writerow([name, seqid, taxid, lineage, len(dna), dna])
         else:
             writer.writerow([seqid, taxid, len(dna), dna])
 
     return
 
+"""
+    takes a string and parse it as xml format to extract the available taxonomy
+    
+
+    INPUTS: parseClassifXML(xml) 
+        xml: string
+    OUTPUTS:
+        classif: dict
+"""
+def parseClassifXML(xml):
+    classif = {}
+
+    if "</ScientificName>" in xml and "<ScientificName>" in xml:
+        scientificName, newXml = xml.split('</ScientificName>', 1)
+        _, scientificName = scientificName.split('<ScientificName>', 1)
+        classif['ScientificName'] = scientificName
+
+    if "</LineageEx>" in xml and "<LineageEx>" in xml:
+        lineageInfo, _ = xml.split("</LineageEx>", 1)
+        _, lineageInfo = lineageInfo.split("<LineageEx>", 1)
+        taxons = lineageInfo.split("</Taxon>")
+        
+        for taxon in taxons:
+            keys = classif.keys()
+            if "</ScientificName>" in taxon and "<ScientificName>" in taxon and "<Rank>" in taxon and "</Rank>" in taxon:
+                name, _ = taxon.split("</ScientificName>", 1)
+                _, name = name.split("<ScientificName>", 1)
+                name = re.sub(r"\s+", '_', name)
+                rank, _ = taxon.split("</Rank>", 1)
+                _, rank= rank.split("<Rank>", 1)
+                rank = re.sub(r"\s+", '_', rank)
+                if rank == 'clade':
+                    if rank not in keys: 
+                        classif['clade'] = [name]
+                    else:
+                        classif['clade'].append(name)
+                else:
+                    classif[rank] = name
+                    
+    return classif
+
+
 if __name__=="_main_":
     countDown()
     download()
     dispatch()
```

### Comparing `nsdpy-0.3.5b0/nsdpy.py` & `nsdpy-0.3.6b0/nsdpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.3.5-beta'
+__version__ = '0.3.6-beta'
 __author__ = "Raphael Hebert, Emese Meglecz"
 __email__ = "raphaelhebert18@gmail.com, emese.meglecz@imbe.fr"
 __license__ = "MIT"
 
 import sys
 import os
 import argparse                     #parsing command line arguments
@@ -49,14 +49,17 @@
     group3 = parser.add_mutually_exclusive_group()
     group3.add_argument("-k", "--kingdom", help="output four different text files file: Plantae and Fungi, Metazoa and  Others", action="store_true" )
     group3.add_argument("-p", "--phylum", help="output one file text per phylum", action="store_true" )
     group3.add_argument("-l", "--levels", help="find only the taxon given by user", nargs="+")
     group3.add_argument("-s", "--species",\
         help="classify the results in different text file one for each (specie + n) level found, exp: -s correspond to lowest levels, -ss 2nd lowest, -sssss 5th lowest and so on",\
         action="count", default=2)
+    group3.add_argument("-x", "--custom",\
+        help="classify the result for the given taxonomic level",\
+        nargs="+")
 
     # information line
     parser.add_argument("-i", "--information", help="just add the taxonomic information in the information line of the output file(s)", action="store_true" )
 
     args = parser.parse_args()
 
     #################################################
@@ -113,14 +116,17 @@
     elif args.phylum:
         classif = 0
         options_report.append("--phylum (-p)")
     elif args.levels:
         # here isinstance(classif, list) == true
         classif = args.levels
         options_report.append(f"--levels (-l) {args.levels[0]}")
+    elif args.custom[0]:
+        classif = args.custom[0]
+        options_report.append(f"--custom (-x) {args.custom}")
     elif args.species:
         classif = args.species
         if args.species != 2:
             options_report.append("--species (-" + "s" * ( args.species - 2 ) + ")")
     else:
         classif = 2
```

### Comparing `nsdpy-0.3.5b0/pyproject.toml` & `nsdpy-0.3.6b0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsdpy"
-version = "0.3.5-beta"
+version = "0.3.6-beta"
 description = "Automatize the download of DNA sequences from NCBI, sort them according to their taxonomy and filter them with a gene name (provided as a regular expression)"
 authors = ["RaphaelHebert <raphaelhebert18@gmail.com>", "Emese Meglecz <emese.meglecz@imbe.fr>"]
 include = ["functions.py"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/RaphaelHebert/nsdpy"
 homepage = "https://github.com/RaphaelHebert/nsdpy"
```

### Comparing `nsdpy-0.3.5b0/PKG-INFO` & `nsdpy-0.3.6b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsdpy
-Version: 0.3.5b0
+Version: 0.3.6b0
 Summary: Automatize the download of DNA sequences from NCBI, sort them according to their taxonomy and filter them with a gene name (provided as a regular expression)
 Home-page: https://github.com/RaphaelHebert/nsdpy
 License: MIT
 Keywords: NCBI,Taxonomy,DNA
 Author: RaphaelHebert
 Author-email: raphaelhebert18@gmail.com
 Requires-Python: >=3.8,<4.0
```

