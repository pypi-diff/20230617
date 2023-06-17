# Comparing `tmp/sppersist-1.1.4.tar.gz` & `tmp/sppersist-1.1.5.tar.gz`

## Comparing `sppersist-1.1.4.tar` & `sppersist-1.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 sppersist-1.1.4/src/spPersist/DTM_filtrations.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sppersist-1.1.4/src/spPersist/__init__.py
--rw-r--r--   0        0        0     9238 2020-02-02 00:00:00.000000 sppersist-1.1.4/src/spPersist/dp.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sppersist-1.1.4/src/spPersist/hc.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 sppersist-1.1.4/src/spPersist/persistence_statistics.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 sppersist-1.1.4/src/spPersist/ph.py
--rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 sppersist-1.1.4/src/spPersist/pp.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-1.1.4/LICENSE
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sppersist-1.1.4/README.md
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 sppersist-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sppersist-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 sppersist-1.1.5/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sppersist-1.1.5/src/spPersist/__init__.py
+-rw-r--r--   0        0        0     9279 2020-02-02 00:00:00.000000 sppersist-1.1.5/src/spPersist/dp.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sppersist-1.1.5/src/spPersist/hc.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 sppersist-1.1.5/src/spPersist/persistence_statistics.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 sppersist-1.1.5/src/spPersist/ph.py
+-rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 sppersist-1.1.5/src/spPersist/pp.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-1.1.5/LICENSE
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sppersist-1.1.5/README.md
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 sppersist-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sppersist-1.1.5/PKG-INFO
```

### Comparing `sppersist-1.1.4/src/spPersist/DTM_filtrations.py` & `sppersist-1.1.5/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.4/src/spPersist/dp.py` & `sppersist-1.1.5/src/spPersist/dp.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 def Visium_FFPE_Mouse_Brain():
   '''
   Returns annotated data object of the Adult Mouse Brain (FFPE) dataset from 
   Visium, 10x Genomics.
   '''
 
   gex = 'Visium_FFPE_Mouse_Brain_filtered_feature_bc_matrix.h5'
+  pos = 'Visium_FFPE_Mouse_Brain_spatial.tar.gz'
   url_gex = 'https://cf.10xgenomics.com/samples/spatial-exp/1.3.0/Visium_FFPE_Mouse_Brain/Visium_FFPE_Mouse_Brain_filtered_feature_bc_matrix.h5'
   url_pos = 'https://cf.10xgenomics.com/samples/spatial-exp/1.3.0/Visium_FFPE_Mouse_Brain/Visium_FFPE_Mouse_Brain_spatial.tar.gz'
   os.system('wget '+url_gex)
-  os.system('wget '+url_pos+' -o spatial.tar')
+  os.system('wget '+url_pos)
 
-  tar = tarfile.open('spatial.tar')
+  tar = tarfile.open(pos)
   posfile = tar.getmembers()[1] # 1 is the index of the coordinate file.
   tar.extract(posfile)
 
   adata = visium(gex, posfile.name)
 
   shutil.rmtree('spatial/')
   os.remove(gex)
@@ -35,20 +36,21 @@
 def V1_Adult_Mouse_Brain():
   '''
   Returns annotated data object of the Mouse Brain Section (Coronal) dataset
   from Visium, 10x Genomics.
   '''
 
   gex = 'V1_Adult_Mouse_Brain_filtered_feature_bc_matrix.h5'
+  pos = 'V1_Adult_Mouse_Brain_spatial.tar.gz'
   url_gex = 'https://cf.10xgenomics.com/samples/spatial-exp/1.0.0/V1_Adult_Mouse_Brain/V1_Adult_Mouse_Brain_filtered_feature_bc_matrix.h5'
   url_pos = 'https://cf.10xgenomics.com/samples/spatial-exp/1.0.0/V1_Adult_Mouse_Brain/V1_Adult_Mouse_Brain_spatial.tar.gz'
   os.system('wget '+url_gex)
-  os.system('wget '+url_pos+' -o spatial.tar')
+  os.system('wget '+url_pos)
 
-  tar = tarfile.open('spatial.tar')
+  tar = tarfile.open(pos)
   posfile = tar.getmembers()[3] # 3 is the index of the coordinate file.
   tar.extract(posfile)
 
   adata = visium(gex, posfile.name)
 
   shutil.rmtree('spatial/')
   os.remove(gex)
```

### Comparing `sppersist-1.1.4/src/spPersist/hc.py` & `sppersist-1.1.5/src/spPersist/hc.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.4/src/spPersist/persistence_statistics.py` & `sppersist-1.1.5/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.4/src/spPersist/ph.py` & `sppersist-1.1.5/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.4/src/spPersist/pp.py` & `sppersist-1.1.5/src/spPersist/pp.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.4/LICENSE` & `sppersist-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.4/README.md` & `sppersist-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.4/pyproject.toml` & `sppersist-1.1.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spPersist"
-version = "1.1.4"
+version = "1.1.5"
 authors = [
   { name="Lirong Yang", email="lirong.yang@outlook.com" },
 ]
 description = "Spatial transcriptomics with Persistent Homology"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sppersist-1.1.4/PKG-INFO` & `sppersist-1.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 1.1.4
+Version: 1.1.5
 Summary: Spatial transcriptomics with Persistent Homology
 Author-email: Lirong Yang <lirong.yang@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

