# Comparing `tmp/sppersist-1.1.6.tar.gz` & `tmp/sppersist-1.1.7.tar.gz`

## Comparing `sppersist-1.1.6.tar` & `sppersist-1.1.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 sppersist-1.1.6/src/spPersist/DTM_filtrations.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sppersist-1.1.6/src/spPersist/__init__.py
--rw-r--r--   0        0        0     9259 2020-02-02 00:00:00.000000 sppersist-1.1.6/src/spPersist/dp.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sppersist-1.1.6/src/spPersist/hc.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 sppersist-1.1.6/src/spPersist/persistence_statistics.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 sppersist-1.1.6/src/spPersist/ph.py
--rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 sppersist-1.1.6/src/spPersist/pp.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-1.1.6/LICENSE
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sppersist-1.1.6/README.md
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 sppersist-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sppersist-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 sppersist-1.1.7/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sppersist-1.1.7/src/spPersist/__init__.py
+-rw-r--r--   0        0        0     9259 2020-02-02 00:00:00.000000 sppersist-1.1.7/src/spPersist/dp.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sppersist-1.1.7/src/spPersist/hc.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 sppersist-1.1.7/src/spPersist/persistence_statistics.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 sppersist-1.1.7/src/spPersist/ph.py
+-rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 sppersist-1.1.7/src/spPersist/pp.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-1.1.7/LICENSE
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sppersist-1.1.7/README.md
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 sppersist-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sppersist-1.1.7/PKG-INFO
```

### Comparing `sppersist-1.1.6/src/spPersist/DTM_filtrations.py` & `sppersist-1.1.7/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.6/src/spPersist/dp.py` & `sppersist-1.1.7/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.6/src/spPersist/hc.py` & `sppersist-1.1.7/src/spPersist/hc.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.6/src/spPersist/persistence_statistics.py` & `sppersist-1.1.7/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.6/src/spPersist/ph.py` & `sppersist-1.1.7/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.6/src/spPersist/pp.py` & `sppersist-1.1.7/src/spPersist/pp.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,22 +131,15 @@
   '''
   extract_reference_data takes a single-cell reference data adata_ref
   as annotated data object, and returns the estimated reference expression
   as a pandas dataframe.
   '''
 
   # prepare anndata for the regression model
-  cell2location.models.RegressionModel.setup_anndata(adata=adata_ref, 
-                          # 10X reaction / sample / batch
-                          batch_key='Sample', 
-                          # cell type, covariate used for constructing signatures
-                          labels_key='Subset', 
-                          # multiplicative technical effects (platform, 3' vs 5', donor effect)
-                          categorical_covariate_keys=['Method']
-                        )
+  cell2location.models.RegressionModel.setup_anndata(adata=adata_ref)
   
   from cell2location.models import RegressionModel
   mod = RegressionModel(adata_ref) 
 
   mod.train(max_epochs=250, use_gpu=True)
 
   adata_ref = mod.export_posterior(
```

### Comparing `sppersist-1.1.6/LICENSE` & `sppersist-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.6/README.md` & `sppersist-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.6/pyproject.toml` & `sppersist-1.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spPersist"
-version = "1.1.6"
+version = "1.1.7"
 authors = [
   { name="Lirong Yang", email="lirong.yang@outlook.com" },
 ]
 description = "Spatial transcriptomics with Persistent Homology"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sppersist-1.1.6/PKG-INFO` & `sppersist-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 1.1.6
+Version: 1.1.7
 Summary: Spatial transcriptomics with Persistent Homology
 Author-email: Lirong Yang <lirong.yang@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

