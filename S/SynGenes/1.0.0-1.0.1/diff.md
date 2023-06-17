# Comparing `tmp/SynGenes-1.0.0.tar.gz` & `tmp/SynGenes-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SynGenes-1.0.0.tar", last modified: Sat Jun 17 19:16:55 2023, max compression
+gzip compressed data, was "SynGenes-1.0.1.tar", last modified: Sat Jun 17 19:59:13 2023, max compression
```

## Comparing `SynGenes-1.0.0.tar` & `SynGenes-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 19:16:55.947713 SynGenes-1.0.0/
--rw-rw-rw-   0        0        0     1068 2023-06-16 23:34:08.000000 SynGenes-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     9538 2023-06-17 19:16:55.946715 SynGenes-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     8448 2023-06-17 18:55:17.000000 SynGenes-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 19:16:55.926549 SynGenes-1.0.0/SynGenes/
--rw-rw-rw-   0        0        0    10790 2023-06-16 23:35:55.000000 SynGenes-1.0.0/SynGenes/SynGenes.py
--rw-rw-rw-   0        0        0       30 2023-06-16 23:29:37.000000 SynGenes-1.0.0/SynGenes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 19:16:55.945711 SynGenes-1.0.0/SynGenes.egg-info/
--rw-rw-rw-   0        0        0     9538 2023-06-17 19:16:55.000000 SynGenes-1.0.0/SynGenes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-06-17 19:16:55.000000 SynGenes-1.0.0/SynGenes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 19:16:55.000000 SynGenes-1.0.0/SynGenes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-17 19:16:55.000000 SynGenes-1.0.0/SynGenes.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-17 19:16:55.000000 SynGenes-1.0.0/SynGenes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 19:16:55.947713 SynGenes-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1373 2023-06-17 19:16:37.000000 SynGenes-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 19:59:13.306262 SynGenes-1.0.1/
+-rw-rw-rw-   0        0        0     1068 2023-06-16 23:34:08.000000 SynGenes-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     9593 2023-06-17 19:59:13.306262 SynGenes-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8503 2023-06-17 19:55:28.000000 SynGenes-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 19:59:13.284320 SynGenes-1.0.1/SynGenes/
+-rw-rw-rw-   0        0        0    11373 2023-06-17 19:58:28.000000 SynGenes-1.0.1/SynGenes/SynGenes.py
+-rw-rw-rw-   0        0        0       30 2023-06-16 23:29:37.000000 SynGenes-1.0.1/SynGenes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 19:59:13.304262 SynGenes-1.0.1/SynGenes.egg-info/
+-rw-rw-rw-   0        0        0     9593 2023-06-17 19:59:13.000000 SynGenes-1.0.1/SynGenes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-17 19:59:13.000000 SynGenes-1.0.1/SynGenes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 19:59:13.000000 SynGenes-1.0.1/SynGenes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-17 19:59:13.000000 SynGenes-1.0.1/SynGenes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-17 19:59:13.000000 SynGenes-1.0.1/SynGenes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 19:59:13.306262 SynGenes-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1373 2023-06-17 19:55:38.000000 SynGenes-1.0.1/setup.py
```

### Comparing `SynGenes-1.0.0/LICENSE` & `SynGenes-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SynGenes-1.0.0/PKG-INFO` & `SynGenes-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SynGenes
-Version: 1.0.0
+Version: 1.0.1
 Summary: SynGenes is a Python class for standardizing gene nomenclatures, this class is capable of recognizing and converting the different nomenclature variations into a standardized form.
 Home-page: https://github.com/luanrabelo/SynGenes
 Download-URL: https://github.com/luanrabelo/SynGenes
 Author: Luan Rabelo
 Author-email: luanrabelo@outlook.com
 Maintainer: Luan Rabelo
 Maintainer-email: luanrabelo@outlook.com
@@ -18,85 +18,90 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<p style="text-align: center;"><img src="https://raw.githubusercontent.com/luanrabelo/SynGenes/stable/docs/assets/SynGenes.png" alt="SynGenes" width="50%"></p>
-<h1 style="text-align: center;"><b>Syn</b><i>Genes</i></h1>
+<p align="center">
+<img src="https://raw.githubusercontent.com/luanrabelo/SynGenes/stable/docs/assets/SynGenes.png" alt="SynGenes" width="50%">
+</p>
+<h1 align="center">
+<b>Syn</b><i>Genes</i>
+</h1>
+
+<h1 align="center">
+Welcome to <b>Syn</b><i>Genes</i> documentation!
+</h1>
 
-<h2 style="text-align: center;"> Welcome to <b>Syn</b><i>Genes</i> documentation!</h2>
-
-<p style="text-align: center;">
+<p align="center">
 <img src="https://img.shields.io/github/license/luanrabelo/SynGenes?style=for-the-badge&label=License&labelColor=191919&color=647E68" alt="License"/>
 <img src="https://img.shields.io/github/v/release/luanrabelo/SynGenes?style=for-the-badge&label=Release&labelColor=191919&color=647E68" alt="Release"/>
+<img src="https://img.shields.io/pypi/v/SynGenes?style=for-the-badge&label=pypi&labelColor=191919&color=647E68" alt="Release"/>
 <img src="https://img.shields.io/github/stars/luanrabelo/SynGenes?style=for-the-badge&label=Stars&labelColor=191919&color=647E68" alt="Stars"/>
 <img src="https://img.shields.io/github/forks/luanrabelo/SynGenes?style=for-the-badge&label=Forks&labelColor=191919&color=647E68" alt="Forks"/>
 <img src="https://img.shields.io/github/downloads/luanrabelo/SynGenes/total?style=for-the-badge&label=Downloads&labelColor=191919&color=647E68" alt="Releases"/>
 <img src="https://img.shields.io/github/languages/top/luanrabelo/SynGenes?style=for-the-badge&label=Python&labelColor=191919&color=647E68" alt="Language"/>
 <img src="https://img.shields.io/github/commit-activity/t/luanrabelo/SynGenes?style=for-the-badge&label=Commits&labelColor=191919&color=647E68" alt="Commits"/>
 <img src="https://img.shields.io/endpoint?url=https://hits.dwyl.com/luanrabelo/SynGenes.json?&labelColor=191919&color=647E68&style=for-the-badge&label=Users" alt="Users"/>
 </p>  
   
 
-### **SynGenes** is a Python class for standardizing gene nomenclatures, this class is capable of recognizing and converting the different nomenclature variations into a standardized form.
-# Getting Started
-***
-
-## 1. Install **SynGenes**
-***
-### Before installing **SynGenes**, you need to make sure that you have the following prerequisites installed:
-* #### Python Environment
-    * ##### [Python 3.6 or higher](https://www.python.org/downloads/) *
-    * ##### [conda](https://www.anaconda.com/download)
-* #### Dependencies
+<h2 align="left"> <b>Syn</b><i>Genes</i> is a Python class for standardizing gene nomenclatures, this class is capable of recognizing and converting the different nomenclature variations into a standardized form.
+</h2>
+
+<h1>Getting Started</h1>
+
+# 1. Install **SynGenes**
+## Before installing **SynGenes**, you need to make sure that you have the following prerequisites installed:
+* ### Python Environment
+    * #### [Python 3.6 or higher](https://www.python.org/downloads/) *
+    * #### [conda](https://www.anaconda.com/download)
+* ### Dependencies
     * **requests** *
     * **pandas** *
     * **openpyxl** *
  
 > #### These dependencies are automaticatically installed using the pip commands below.
-##### * obrigatory
-***
-### There are **three** ways to install **SynGenes**:    
+### * obrigatory
+## There are **three** ways to install **SynGenes**:    
 
-#### 1.1. **Through pip**: You can install **SynGenes** directly through pip using the following command:
+### 1.1. **Through pip**: You can install **SynGenes** directly through pip using the following command:
 ```bash
 pip install SynGenes
 ```
-###### This will install **SynGenes** and its dependencies in your Python environment.  
-#### 1.2. **By cloning the source code from GitHub**: You can clone the source code of **SynGenes** from GitHub using the following command:
+##### This will install **SynGenes** and its dependencies in your Python environment.  
+### 1.2. **By cloning the source code from GitHub**: You can clone the source code of **SynGenes** from GitHub using the following command:
 ```bash
 git clone https://github.com/luanrabelo/SynGenes.git
 ```
-###### This will clone the repository to your local machine. You can then navigate to the cloned directory and install **SynGenes** and its dependencies using pip:
+##### This will clone the repository to your local machine. You can then navigate to the cloned directory and install **SynGenes** and its dependencies using pip:
 ```bash
 cd SynGenes
 pip install -r requirements.txt
 ```
 
-#### 1.3. **Through conda**: You can install **SynGenes** through conda using the following command:
+### 1.3. **Through conda**: You can install **SynGenes** through conda using the following command:
 ```bash
 conda create -n SynGenes -c conda-forge -c bioconda SynGenes
 conda activate SynGenes
 ```
-###### This will install **SynGenes** and its dependencies in your conda environment.
-***
-## Usage
+##### This will install **SynGenes** and its dependencies in your conda environment.
+# 2. Usage
 ```python
 from SynGenes import SynGenes
 geneNames = SynGenes()
 ```
-#### To update **SynGenes** database in your computer, run:
+## To update **SynGenes** database in your computer, run:
 ```python
 geneNames.updateSynGenes()
 ```
-###### This command will delete the database from your computer and download a new one from the **SynGenes** repository.
+##### This command will delete the database from your computer and download a new one from the **SynGenes** repository.
 
-#### Basic Example
+## Basic Example
 ```python
 # Mitochondrial
 # Convert nomenclature 'cytochrome oxidase subunit I' to 'COI'
 # Convert nomenclature 'cytochrome c oxidase subunit I' to 'COI'
 FullGeneName1 = "cytochrome oxidase subunit I"
 FullGeneName1 = geneNames.FixGeneName(geneName=FullGeneName1, type='mt')
 FullGeneName2 = "cytochrome c oxidase subunit I"
@@ -117,16 +122,16 @@
 FullGeneName2 = geneNames.FixGeneName(geneName=FullGeneName2, type='cp')
 print(FullGeneName1)
 print(FullGeneName2)
 # output
 atpA
 atpA
 ```
-###### Here, the user needs to provide the **geneName** parameter (**str**) and the **type** parameter (**str**), where **type='mt'** for **mitochondrial genes** and **type='cp'** for **chloroplast genes**.
-### Usage Example with Biopython
+##### Here, the user needs to provide the **geneName** parameter (**str**) and the **type** parameter (**str**), where **type='mt'** for **mitochondrial genes** and **type='cp'** for **chloroplast genes**.
+## Usage Example with Biopython
 ```python
 from SynGenes import SynGenes
 from Bio import SeqIO
 
 # Start SynGenes class
 geneNames = SynGenes()
 # Update SynGenes database 
@@ -208,21 +213,17 @@
         NADH-3
         NADH-4L
         NADH-5
         NADH-6
         CYTB
 ```
 
-#### Through an example with two genomes, it is possible to observe that they have different nomenclatures for genes. However, by using SynGenes, it is possible to standardize these nomenclatures. This allows, for example, writing the standardized forms in fasta files or in input files of other tools such as CREx. This way, it is possible to ensure the consistency and compatibility of genomic data when performing subsequent analyzes.
+##### Through an example with two genomes, it is possible to observe that they have different nomenclatures for genes. However, by using SynGenes, it is possible to standardize these nomenclatures. This allows, for example, writing the standardized forms in fasta files or in input files of other tools such as CREx. This way, it is possible to ensure the consistency and compatibility of genomic data when performing subsequent analyzes.
+
+# 3. Web Form
+## We also created a web form (https://luanrabelo.github.io/SynGenes) to researchers who wish to perform individual searches using different names associated with the same gene. This web form generates a command that incorporates multiple names, enabling precise searches on the National Center for Biotechnology Information (NCBI) - GenBank platform.
 
-***
-## 2. Web Form
-### We also created a web form (https://luanrabelo.github.io/SynGenes) to researchers who wish to perform individual searches using different names associated with the same gene. This web form generates a command that incorporates multiple names, enabling precise searches on the National Center for Biotechnology Information (NCBI) - GenBank platform.
-
-***
-## Authors
-##### Developers
+# Developers
 * [Luan Rabelo](https://twitter.com/lprabelo)
 * [Marcelo Vallinoto](https://twitter.com/mvallinoto01)
-***
-## Citation
+# Citation
 > Rabelo et al.
```

### Comparing `SynGenes-1.0.0/README.md` & `SynGenes-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,78 +1,83 @@
-<p style="text-align: center;"><img src="https://raw.githubusercontent.com/luanrabelo/SynGenes/stable/docs/assets/SynGenes.png" alt="SynGenes" width="50%"></p>
-<h1 style="text-align: center;"><b>Syn</b><i>Genes</i></h1>
+<p align="center">
+<img src="https://raw.githubusercontent.com/luanrabelo/SynGenes/stable/docs/assets/SynGenes.png" alt="SynGenes" width="50%">
+</p>
+<h1 align="center">
+<b>Syn</b><i>Genes</i>
+</h1>
+
+<h1 align="center">
+Welcome to <b>Syn</b><i>Genes</i> documentation!
+</h1>
 
-<h2 style="text-align: center;"> Welcome to <b>Syn</b><i>Genes</i> documentation!</h2>
-
-<p style="text-align: center;">
+<p align="center">
 <img src="https://img.shields.io/github/license/luanrabelo/SynGenes?style=for-the-badge&label=License&labelColor=191919&color=647E68" alt="License"/>
 <img src="https://img.shields.io/github/v/release/luanrabelo/SynGenes?style=for-the-badge&label=Release&labelColor=191919&color=647E68" alt="Release"/>
+<img src="https://img.shields.io/pypi/v/SynGenes?style=for-the-badge&label=pypi&labelColor=191919&color=647E68" alt="Release"/>
 <img src="https://img.shields.io/github/stars/luanrabelo/SynGenes?style=for-the-badge&label=Stars&labelColor=191919&color=647E68" alt="Stars"/>
 <img src="https://img.shields.io/github/forks/luanrabelo/SynGenes?style=for-the-badge&label=Forks&labelColor=191919&color=647E68" alt="Forks"/>
 <img src="https://img.shields.io/github/downloads/luanrabelo/SynGenes/total?style=for-the-badge&label=Downloads&labelColor=191919&color=647E68" alt="Releases"/>
 <img src="https://img.shields.io/github/languages/top/luanrabelo/SynGenes?style=for-the-badge&label=Python&labelColor=191919&color=647E68" alt="Language"/>
 <img src="https://img.shields.io/github/commit-activity/t/luanrabelo/SynGenes?style=for-the-badge&label=Commits&labelColor=191919&color=647E68" alt="Commits"/>
 <img src="https://img.shields.io/endpoint?url=https://hits.dwyl.com/luanrabelo/SynGenes.json?&labelColor=191919&color=647E68&style=for-the-badge&label=Users" alt="Users"/>
 </p>  
   
 
-### **SynGenes** is a Python class for standardizing gene nomenclatures, this class is capable of recognizing and converting the different nomenclature variations into a standardized form.
-# Getting Started
-***
-
-## 1. Install **SynGenes**
-***
-### Before installing **SynGenes**, you need to make sure that you have the following prerequisites installed:
-* #### Python Environment
-    * ##### [Python 3.6 or higher](https://www.python.org/downloads/) *
-    * ##### [conda](https://www.anaconda.com/download)
-* #### Dependencies
+<h2 align="left"> <b>Syn</b><i>Genes</i> is a Python class for standardizing gene nomenclatures, this class is capable of recognizing and converting the different nomenclature variations into a standardized form.
+</h2>
+
+<h1>Getting Started</h1>
+
+# 1. Install **SynGenes**
+## Before installing **SynGenes**, you need to make sure that you have the following prerequisites installed:
+* ### Python Environment
+    * #### [Python 3.6 or higher](https://www.python.org/downloads/) *
+    * #### [conda](https://www.anaconda.com/download)
+* ### Dependencies
     * **requests** *
     * **pandas** *
     * **openpyxl** *
  
 > #### These dependencies are automaticatically installed using the pip commands below.
-##### * obrigatory
-***
-### There are **three** ways to install **SynGenes**:    
+### * obrigatory
+## There are **three** ways to install **SynGenes**:    
 
-#### 1.1. **Through pip**: You can install **SynGenes** directly through pip using the following command:
+### 1.1. **Through pip**: You can install **SynGenes** directly through pip using the following command:
 ```bash
 pip install SynGenes
 ```
-###### This will install **SynGenes** and its dependencies in your Python environment.  
-#### 1.2. **By cloning the source code from GitHub**: You can clone the source code of **SynGenes** from GitHub using the following command:
+##### This will install **SynGenes** and its dependencies in your Python environment.  
+### 1.2. **By cloning the source code from GitHub**: You can clone the source code of **SynGenes** from GitHub using the following command:
 ```bash
 git clone https://github.com/luanrabelo/SynGenes.git
 ```
-###### This will clone the repository to your local machine. You can then navigate to the cloned directory and install **SynGenes** and its dependencies using pip:
+##### This will clone the repository to your local machine. You can then navigate to the cloned directory and install **SynGenes** and its dependencies using pip:
 ```bash
 cd SynGenes
 pip install -r requirements.txt
 ```
 
-#### 1.3. **Through conda**: You can install **SynGenes** through conda using the following command:
+### 1.3. **Through conda**: You can install **SynGenes** through conda using the following command:
 ```bash
 conda create -n SynGenes -c conda-forge -c bioconda SynGenes
 conda activate SynGenes
 ```
-###### This will install **SynGenes** and its dependencies in your conda environment.
-***
-## Usage
+##### This will install **SynGenes** and its dependencies in your conda environment.
+# 2. Usage
 ```python
 from SynGenes import SynGenes
 geneNames = SynGenes()
 ```
-#### To update **SynGenes** database in your computer, run:
+## To update **SynGenes** database in your computer, run:
 ```python
 geneNames.updateSynGenes()
 ```
-###### This command will delete the database from your computer and download a new one from the **SynGenes** repository.
+##### This command will delete the database from your computer and download a new one from the **SynGenes** repository.
 
-#### Basic Example
+## Basic Example
 ```python
 # Mitochondrial
 # Convert nomenclature 'cytochrome oxidase subunit I' to 'COI'
 # Convert nomenclature 'cytochrome c oxidase subunit I' to 'COI'
 FullGeneName1 = "cytochrome oxidase subunit I"
 FullGeneName1 = geneNames.FixGeneName(geneName=FullGeneName1, type='mt')
 FullGeneName2 = "cytochrome c oxidase subunit I"
@@ -93,16 +98,16 @@
 FullGeneName2 = geneNames.FixGeneName(geneName=FullGeneName2, type='cp')
 print(FullGeneName1)
 print(FullGeneName2)
 # output
 atpA
 atpA
 ```
-###### Here, the user needs to provide the **geneName** parameter (**str**) and the **type** parameter (**str**), where **type='mt'** for **mitochondrial genes** and **type='cp'** for **chloroplast genes**.
-### Usage Example with Biopython
+##### Here, the user needs to provide the **geneName** parameter (**str**) and the **type** parameter (**str**), where **type='mt'** for **mitochondrial genes** and **type='cp'** for **chloroplast genes**.
+## Usage Example with Biopython
 ```python
 from SynGenes import SynGenes
 from Bio import SeqIO
 
 # Start SynGenes class
 geneNames = SynGenes()
 # Update SynGenes database 
@@ -184,21 +189,17 @@
         NADH-3
         NADH-4L
         NADH-5
         NADH-6
         CYTB
 ```
 
-#### Through an example with two genomes, it is possible to observe that they have different nomenclatures for genes. However, by using SynGenes, it is possible to standardize these nomenclatures. This allows, for example, writing the standardized forms in fasta files or in input files of other tools such as CREx. This way, it is possible to ensure the consistency and compatibility of genomic data when performing subsequent analyzes.
+##### Through an example with two genomes, it is possible to observe that they have different nomenclatures for genes. However, by using SynGenes, it is possible to standardize these nomenclatures. This allows, for example, writing the standardized forms in fasta files or in input files of other tools such as CREx. This way, it is possible to ensure the consistency and compatibility of genomic data when performing subsequent analyzes.
+
+# 3. Web Form
+## We also created a web form (https://luanrabelo.github.io/SynGenes) to researchers who wish to perform individual searches using different names associated with the same gene. This web form generates a command that incorporates multiple names, enabling precise searches on the National Center for Biotechnology Information (NCBI) - GenBank platform.
 
-***
-## 2. Web Form
-### We also created a web form (https://luanrabelo.github.io/SynGenes) to researchers who wish to perform individual searches using different names associated with the same gene. This web form generates a command that incorporates multiple names, enabling precise searches on the National Center for Biotechnology Information (NCBI) - GenBank platform.
-
-***
-## Authors
-##### Developers
+# Developers
 * [Luan Rabelo](https://twitter.com/lprabelo)
 * [Marcelo Vallinoto](https://twitter.com/mvallinoto01)
-***
-## Citation
+# Citation
 > Rabelo et al.
```

### Comparing `SynGenes-1.0.0/SynGenes/SynGenes.py` & `SynGenes-1.0.1/SynGenes/SynGenes.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,19 +62,19 @@
             Fail        = '\033[91m'
             End         = '\033[0m'
             Bold        = '\033[1m'
             Underline   = '\033[4m'
     
     def __init__(self):
         """
-        SynGenes: A Python class to download and update SynGenes database.
-
-        Parameters
-        ----------
+        SynGenes: Python class for standardizing gene nomenclatures.
 
+        Functions:
+        updateSynGenes(): Download SynGenes database from GitHub repository (stable branch).
+        FixGeneName(): Fix gene name according to the SynGenes database.
         """
         
         if not os.path.exists(f'{SynGenes.cwdPath}/SynGenes/SynGenes.xlsx') or not os.path.isfile(f'{SynGenes.cwdPath}/SynGenes/SynGenes.xlsx'):
             print(f"{SynGenes.TerminalColors.Warning}{SynGenes.TerminalColors.Bold}SynGenes database not found in {SynGenes.cwdPath}{SynGenes.TerminalColors.End}!\n")
             print(f"{SynGenes.TerminalColors.Warning}{SynGenes.TerminalColors.Bold}Creating folder 'SynGenes' in {SynGenes.cwdPath}{SynGenes.TerminalColors.End}")
             try:
                 os.makedirs(f'{SynGenes.cwdPath}/SynGenes', exist_ok=True, mode=0o777)
@@ -94,14 +94,23 @@
                             os.fsync(f.fileno())
                 print(f'{SynGenes.TerminalColors.Green}{SynGenes.TerminalColors.Bold}Downloaded SynGenes database successfully ({time.strftime("%Y/%m/%d - %H:%M:%S")})!\n{SynGenes.TerminalColors.End}')
             else:
                 print(f'{SynGenes.TerminalColors.Fail}{SynGenes.TerminalColors.Bold}Download SynGenes database failed: status code {download.status_code} - {download.text}{SynGenes.TerminalColors.End}')
                 sys.exit()
 
     def updateSynGenes(self):
+        """
+        Download SynGenes database from GitHub repository (stable branch).
+
+        Parameters:
+        None
+
+        Returns:
+        None
+        """
         if os.path.exists(f'{SynGenes.cwdPath}/SynGenes/SynGenes.xlsx') or os.path.isfile(f'{SynGenes.cwdPath}/SynGenes/SynGenes.xlsx'):
             print(f"{SynGenes.TerminalColors.Warning}{SynGenes.TerminalColors.Bold}SynGenes database found in {SynGenes.cwdPath}{SynGenes.TerminalColors.End}!\n")
             print(f"{SynGenes.TerminalColors.Warning}{SynGenes.TerminalColors.Bold}Removing old SynGenes database...{SynGenes.TerminalColors.End}")
             try:
                 os.remove(f'{SynGenes.cwdPath}/SynGenes/SynGenes.xlsx')
                 print(f"{SynGenes.TerminalColors.Green}{SynGenes.TerminalColors.Bold}Old SynGenes database removed successfully!\n{SynGenes.TerminalColors.End}")
             except:
@@ -128,14 +137,24 @@
                         os.fsync(f.fileno())
             print(f'{SynGenes.TerminalColors.Green}{SynGenes.TerminalColors.Bold}Downloaded SynGenes database successfully ({time.strftime("%Y/%m/%d - %H:%M:%S")})!\n{SynGenes.TerminalColors.End}')
         else:
             print(f'{SynGenes.TerminalColors.Fail}{SynGenes.TerminalColors.Bold}Download SynGenes database failed: status code {download.status_code} - {download.text}{SynGenes.TerminalColors.End}')
             sys.exit()
 
     def FixGeneName(self, **kwargs):
+        """
+        Fix gene name to search in SynGenes database.
+
+        Parameters:
+        geneName (str): Gene name to search in SynGenes database.
+        type (str): Organelle type (mt or cp).
+
+        Returns:
+        str: Fixed gene name.
+        """
         GeneList = []
         GeneList.clear()
         FullName  = str(kwargs['geneName'])
         Organelle = str(kwargs['type'])
         if Organelle == 'mt':
             df = pd.DataFrame(pd.read_excel(f'{SynGenes.cwdPath}/SynGenes/SynGenes.xlsx', sheet_name="Mitochondrial", dtype=str)).reset_index()
         elif Organelle == 'cp':
```

### Comparing `SynGenes-1.0.0/SynGenes.egg-info/PKG-INFO` & `SynGenes-1.0.1/SynGenes.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SynGenes
-Version: 1.0.0
+Version: 1.0.1
 Summary: SynGenes is a Python class for standardizing gene nomenclatures, this class is capable of recognizing and converting the different nomenclature variations into a standardized form.
 Home-page: https://github.com/luanrabelo/SynGenes
 Download-URL: https://github.com/luanrabelo/SynGenes
 Author: Luan Rabelo
 Author-email: luanrabelo@outlook.com
 Maintainer: Luan Rabelo
 Maintainer-email: luanrabelo@outlook.com
@@ -18,85 +18,90 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<p style="text-align: center;"><img src="https://raw.githubusercontent.com/luanrabelo/SynGenes/stable/docs/assets/SynGenes.png" alt="SynGenes" width="50%"></p>
-<h1 style="text-align: center;"><b>Syn</b><i>Genes</i></h1>
+<p align="center">
+<img src="https://raw.githubusercontent.com/luanrabelo/SynGenes/stable/docs/assets/SynGenes.png" alt="SynGenes" width="50%">
+</p>
+<h1 align="center">
+<b>Syn</b><i>Genes</i>
+</h1>
+
+<h1 align="center">
+Welcome to <b>Syn</b><i>Genes</i> documentation!
+</h1>
 
-<h2 style="text-align: center;"> Welcome to <b>Syn</b><i>Genes</i> documentation!</h2>
-
-<p style="text-align: center;">
+<p align="center">
 <img src="https://img.shields.io/github/license/luanrabelo/SynGenes?style=for-the-badge&label=License&labelColor=191919&color=647E68" alt="License"/>
 <img src="https://img.shields.io/github/v/release/luanrabelo/SynGenes?style=for-the-badge&label=Release&labelColor=191919&color=647E68" alt="Release"/>
+<img src="https://img.shields.io/pypi/v/SynGenes?style=for-the-badge&label=pypi&labelColor=191919&color=647E68" alt="Release"/>
 <img src="https://img.shields.io/github/stars/luanrabelo/SynGenes?style=for-the-badge&label=Stars&labelColor=191919&color=647E68" alt="Stars"/>
 <img src="https://img.shields.io/github/forks/luanrabelo/SynGenes?style=for-the-badge&label=Forks&labelColor=191919&color=647E68" alt="Forks"/>
 <img src="https://img.shields.io/github/downloads/luanrabelo/SynGenes/total?style=for-the-badge&label=Downloads&labelColor=191919&color=647E68" alt="Releases"/>
 <img src="https://img.shields.io/github/languages/top/luanrabelo/SynGenes?style=for-the-badge&label=Python&labelColor=191919&color=647E68" alt="Language"/>
 <img src="https://img.shields.io/github/commit-activity/t/luanrabelo/SynGenes?style=for-the-badge&label=Commits&labelColor=191919&color=647E68" alt="Commits"/>
 <img src="https://img.shields.io/endpoint?url=https://hits.dwyl.com/luanrabelo/SynGenes.json?&labelColor=191919&color=647E68&style=for-the-badge&label=Users" alt="Users"/>
 </p>  
   
 
-### **SynGenes** is a Python class for standardizing gene nomenclatures, this class is capable of recognizing and converting the different nomenclature variations into a standardized form.
-# Getting Started
-***
-
-## 1. Install **SynGenes**
-***
-### Before installing **SynGenes**, you need to make sure that you have the following prerequisites installed:
-* #### Python Environment
-    * ##### [Python 3.6 or higher](https://www.python.org/downloads/) *
-    * ##### [conda](https://www.anaconda.com/download)
-* #### Dependencies
+<h2 align="left"> <b>Syn</b><i>Genes</i> is a Python class for standardizing gene nomenclatures, this class is capable of recognizing and converting the different nomenclature variations into a standardized form.
+</h2>
+
+<h1>Getting Started</h1>
+
+# 1. Install **SynGenes**
+## Before installing **SynGenes**, you need to make sure that you have the following prerequisites installed:
+* ### Python Environment
+    * #### [Python 3.6 or higher](https://www.python.org/downloads/) *
+    * #### [conda](https://www.anaconda.com/download)
+* ### Dependencies
     * **requests** *
     * **pandas** *
     * **openpyxl** *
  
 > #### These dependencies are automaticatically installed using the pip commands below.
-##### * obrigatory
-***
-### There are **three** ways to install **SynGenes**:    
+### * obrigatory
+## There are **three** ways to install **SynGenes**:    
 
-#### 1.1. **Through pip**: You can install **SynGenes** directly through pip using the following command:
+### 1.1. **Through pip**: You can install **SynGenes** directly through pip using the following command:
 ```bash
 pip install SynGenes
 ```
-###### This will install **SynGenes** and its dependencies in your Python environment.  
-#### 1.2. **By cloning the source code from GitHub**: You can clone the source code of **SynGenes** from GitHub using the following command:
+##### This will install **SynGenes** and its dependencies in your Python environment.  
+### 1.2. **By cloning the source code from GitHub**: You can clone the source code of **SynGenes** from GitHub using the following command:
 ```bash
 git clone https://github.com/luanrabelo/SynGenes.git
 ```
-###### This will clone the repository to your local machine. You can then navigate to the cloned directory and install **SynGenes** and its dependencies using pip:
+##### This will clone the repository to your local machine. You can then navigate to the cloned directory and install **SynGenes** and its dependencies using pip:
 ```bash
 cd SynGenes
 pip install -r requirements.txt
 ```
 
-#### 1.3. **Through conda**: You can install **SynGenes** through conda using the following command:
+### 1.3. **Through conda**: You can install **SynGenes** through conda using the following command:
 ```bash
 conda create -n SynGenes -c conda-forge -c bioconda SynGenes
 conda activate SynGenes
 ```
-###### This will install **SynGenes** and its dependencies in your conda environment.
-***
-## Usage
+##### This will install **SynGenes** and its dependencies in your conda environment.
+# 2. Usage
 ```python
 from SynGenes import SynGenes
 geneNames = SynGenes()
 ```
-#### To update **SynGenes** database in your computer, run:
+## To update **SynGenes** database in your computer, run:
 ```python
 geneNames.updateSynGenes()
 ```
-###### This command will delete the database from your computer and download a new one from the **SynGenes** repository.
+##### This command will delete the database from your computer and download a new one from the **SynGenes** repository.
 
-#### Basic Example
+## Basic Example
 ```python
 # Mitochondrial
 # Convert nomenclature 'cytochrome oxidase subunit I' to 'COI'
 # Convert nomenclature 'cytochrome c oxidase subunit I' to 'COI'
 FullGeneName1 = "cytochrome oxidase subunit I"
 FullGeneName1 = geneNames.FixGeneName(geneName=FullGeneName1, type='mt')
 FullGeneName2 = "cytochrome c oxidase subunit I"
@@ -117,16 +122,16 @@
 FullGeneName2 = geneNames.FixGeneName(geneName=FullGeneName2, type='cp')
 print(FullGeneName1)
 print(FullGeneName2)
 # output
 atpA
 atpA
 ```
-###### Here, the user needs to provide the **geneName** parameter (**str**) and the **type** parameter (**str**), where **type='mt'** for **mitochondrial genes** and **type='cp'** for **chloroplast genes**.
-### Usage Example with Biopython
+##### Here, the user needs to provide the **geneName** parameter (**str**) and the **type** parameter (**str**), where **type='mt'** for **mitochondrial genes** and **type='cp'** for **chloroplast genes**.
+## Usage Example with Biopython
 ```python
 from SynGenes import SynGenes
 from Bio import SeqIO
 
 # Start SynGenes class
 geneNames = SynGenes()
 # Update SynGenes database 
@@ -208,21 +213,17 @@
         NADH-3
         NADH-4L
         NADH-5
         NADH-6
         CYTB
 ```
 
-#### Through an example with two genomes, it is possible to observe that they have different nomenclatures for genes. However, by using SynGenes, it is possible to standardize these nomenclatures. This allows, for example, writing the standardized forms in fasta files or in input files of other tools such as CREx. This way, it is possible to ensure the consistency and compatibility of genomic data when performing subsequent analyzes.
+##### Through an example with two genomes, it is possible to observe that they have different nomenclatures for genes. However, by using SynGenes, it is possible to standardize these nomenclatures. This allows, for example, writing the standardized forms in fasta files or in input files of other tools such as CREx. This way, it is possible to ensure the consistency and compatibility of genomic data when performing subsequent analyzes.
+
+# 3. Web Form
+## We also created a web form (https://luanrabelo.github.io/SynGenes) to researchers who wish to perform individual searches using different names associated with the same gene. This web form generates a command that incorporates multiple names, enabling precise searches on the National Center for Biotechnology Information (NCBI) - GenBank platform.
 
-***
-## 2. Web Form
-### We also created a web form (https://luanrabelo.github.io/SynGenes) to researchers who wish to perform individual searches using different names associated with the same gene. This web form generates a command that incorporates multiple names, enabling precise searches on the National Center for Biotechnology Information (NCBI) - GenBank platform.
-
-***
-## Authors
-##### Developers
+# Developers
 * [Luan Rabelo](https://twitter.com/lprabelo)
 * [Marcelo Vallinoto](https://twitter.com/mvallinoto01)
-***
-## Citation
+# Citation
 > Rabelo et al.
```

### Comparing `SynGenes-1.0.0/setup.py` & `SynGenes-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     Readme = fh.read()
 
 setup(
     name = 'SynGenes',
-    version = '1.0.0',
+    version = '1.0.1',
     description = 'SynGenes is a Python class for standardizing gene nomenclatures, this class is capable of recognizing and converting the different nomenclature variations into a standardized form.',
     long_description = Readme,
     long_description_content_type="text/markdown",
     author = 'Luan Rabelo',
     author_email = 'luanrabelo@outlook.com',
     maintainer = 'Luan Rabelo',
     maintainer_email = 'luanrabelo@outlook.com',
```

