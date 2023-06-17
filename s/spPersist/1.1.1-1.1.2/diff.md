# Comparing `tmp/sppersist-1.1.1.tar.gz` & `tmp/sppersist-1.1.2.tar.gz`

## Comparing `sppersist-1.1.1.tar` & `sppersist-1.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 sppersist-1.1.1/src/spPersist/DTM_filtrations.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sppersist-1.1.1/src/spPersist/__init__.py
--rw-r--r--   0        0        0     9073 2020-02-02 00:00:00.000000 sppersist-1.1.1/src/spPersist/dp.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sppersist-1.1.1/src/spPersist/hc.py
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 sppersist-1.1.1/src/spPersist/persistence_statistics.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 sppersist-1.1.1/src/spPersist/ph.py
--rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 sppersist-1.1.1/src/spPersist/pp.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-1.1.1/LICENSE
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sppersist-1.1.1/README.md
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 sppersist-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sppersist-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 sppersist-1.1.2/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sppersist-1.1.2/src/spPersist/__init__.py
+-rw-r--r--   0        0        0     9244 2020-02-02 00:00:00.000000 sppersist-1.1.2/src/spPersist/dp.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sppersist-1.1.2/src/spPersist/hc.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 sppersist-1.1.2/src/spPersist/persistence_statistics.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 sppersist-1.1.2/src/spPersist/ph.py
+-rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 sppersist-1.1.2/src/spPersist/pp.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-1.1.2/LICENSE
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sppersist-1.1.2/README.md
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 sppersist-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sppersist-1.1.2/PKG-INFO
```

### Comparing `sppersist-1.1.1/src/spPersist/DTM_filtrations.py` & `sppersist-1.1.2/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.1/src/spPersist/dp.py` & `sppersist-1.1.2/src/spPersist/dp.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,14 +101,16 @@
 def visium(gex: str, pos: str):
   '''
   visium takes cell by gene count file name gex and tissue position lists pos, 
   and return an annotated data object with spatial coordinates in obsm.
   Note that gex and pos should be formatted as Spance Ranger outputs.
   '''
   ad = sc.read_10x_h5(gex)
+  ad.var_names_make_unique()
+  ad.var["mt"] = ad.var_names.str.startswith("MT-")
   coords = pd.read_csv(pos,index_col=0)
   coords.columns = ["in_tissue", "array_row", "array_col", "pxl_col_in_fullres", "pxl_row_in_fullres"]
   ad.obs = pd.merge(ad.obs, coords, how="left", left_index=True, right_index=True)
   ad.obsm['spatial'] = ad.obs[["pxl_row_in_fullres", "pxl_col_in_fullres"]].values
   ad.obs.drop(columns=["pxl_row_in_fullres", "pxl_col_in_fullres"], inplace=True)
   return ad
 
@@ -116,15 +118,16 @@
   '''
   merfish takes cell by gene count file name gex and
   metadata file pos that contains spatial coordinates, 
   and return an annotated data object with spatial coordinates in obsm.
   Note that gex and pos should be formatted as Vizgen outputs.
   '''
   adata = anndata.AnnData(pd.read_csv(gex, header=0, index_col=0))
-  
+  adata.var_names_make_unique()
+  adata.var["mt"] = adata.var_names.str.startswith("MT-")
 
   coords = pd.read_csv(pos, header=0, index_col=0)
   coords.columns = ["fov", "volume", "center_x", "center_y", "min_x", "max_x", "min_y", "max_y"]
 
   adata.obs = pd.merge(adata.obs, coords, how="left", left_index=True, right_index=True)
   adata.obsm['spatial'] = adata.obs[["center_x", "center_y"]].values
   adata.obs.drop(columns=["center_x", "center_y"], inplace=True)
```

### Comparing `sppersist-1.1.1/src/spPersist/hc.py` & `sppersist-1.1.2/src/spPersist/hc.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.1/src/spPersist/persistence_statistics.py` & `sppersist-1.1.2/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.1/src/spPersist/ph.py` & `sppersist-1.1.2/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.1/src/spPersist/pp.py` & `sppersist-1.1.2/src/spPersist/pp.py`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.1/LICENSE` & `sppersist-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.1/README.md` & `sppersist-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sppersist-1.1.1/pyproject.toml` & `sppersist-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "spPersist"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="Lirong Yang", email="lirong.yang@outlook.com" },
 ]
 description = "Spatial transcriptomics with Persistent Homology"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sppersist-1.1.1/PKG-INFO` & `sppersist-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 1.1.1
+Version: 1.1.2
 Summary: Spatial transcriptomics with Persistent Homology
 Author-email: Lirong Yang <lirong.yang@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

