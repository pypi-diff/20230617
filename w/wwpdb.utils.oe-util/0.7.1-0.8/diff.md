# Comparing `tmp/wwpdb.utils.oe_util-0.7.1.tar.gz` & `tmp/wwpdb.utils.oe_util-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.oe_util-0.7.1.tar", last modified: Sun Jun  5 23:28:28 2022, max compression
+gzip compressed data, was "wwpdb.utils.oe_util-0.8.tar", last modified: Sat Jun 17 11:32:17 2023, max compression
```

## Comparing `wwpdb.utils.oe_util-0.7.1.tar` & `wwpdb.utils.oe_util-0.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-05 23:28:28.891689 wwpdb.utils.oe_util-0.7.1/
--rw-r--r--   0 vsts      (1001) docker     (121)      732 2022-06-05 23:28:28.891689 wwpdb.utils.oe_util-0.7.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1222 2022-06-05 23:27:15.000000 wwpdb.utils.oe_util-0.7.1/README.md
--rw-r--r--   0 vsts      (1001) docker     (121)      108 2022-06-05 23:28:28.891689 wwpdb.utils.oe_util-0.7.1/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (121)     2397 2022-06-05 23:27:15.000000 wwpdb.utils.oe_util-0.7.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-05 23:28:28.887689 wwpdb.utils.oe_util-0.7.1/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (121)       65 2022-06-05 23:27:15.000000 wwpdb.utils.oe_util-0.7.1/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-05 23:28:28.887689 wwpdb.utils.oe_util-0.7.1/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (121)       65 2022-06-05 23:27:15.000000 wwpdb.utils.oe_util-0.7.1/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-05 23:28:28.887689 wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/
--rw-r--r--   0 vsts      (1001) docker     (121)      151 2022-06-05 23:27:15.000000 wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-05 23:28:28.887689 wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/build/
--rw-r--r--   0 vsts      (1001) docker     (121)    10746 2022-06-05 23:27:15.000000 wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/build/OeBuildModelMol.py
--rw-r--r--   0 vsts      (1001) docker     (121)    19744 2022-06-05 23:27:15.000000 wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/build/OeBuildMol.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3824 2022-06-05 23:27:15.000000 wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/build/OeChemCompIoUtils.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1366 2022-06-05 23:27:15.000000 wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/build/OeDescriptorUtils.py
--rw-r--r--   0 vsts      (1001) docker     (121)    16791 2022-06-05 23:27:15.000000 wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/build/OePersist.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14062 2022-06-05 23:27:15.000000 wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/build/PdbxBuildChemComp.py
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-05 23:27:15.000000 wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/build/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-05 23:28:28.891689 wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/oedepict/
--rw-r--r--   0 vsts      (1001) docker     (121)    28515 2022-06-05 23:27:15.000000 wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/oedepict/OeAlignDepict.py
--rw-r--r--   0 vsts      (1001) docker     (121)    45990 2022-06-05 23:27:15.000000 wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/oedepict/OeAlignDepictUtils.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     9099 2022-06-05 23:27:15.000000 wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/oedepict/OeDepict.py
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-05 23:27:15.000000 wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/oedepict/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2719 2022-06-05 23:27:15.000000 wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/oedepict/modMCSAlign.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3373 2022-06-05 23:27:15.000000 wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/oedepict/simple-example.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-05 23:28:28.887689 wwpdb.utils.oe_util-0.7.1/wwpdb.utils.oe_util.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)      732 2022-06-05 23:28:28.000000 wwpdb.utils.oe_util-0.7.1/wwpdb.utils.oe_util.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)      931 2022-06-05 23:28:28.000000 wwpdb.utils.oe_util-0.7.1/wwpdb.utils.oe_util.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-06-05 23:28:28.000000 wwpdb.utils.oe_util-0.7.1/wwpdb.utils.oe_util.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-06-05 23:27:40.000000 wwpdb.utils.oe_util-0.7.1/wwpdb.utils.oe_util.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (121)      233 2022-06-05 23:28:28.000000 wwpdb.utils.oe_util-0.7.1/wwpdb.utils.oe_util.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        6 2022-06-05 23:28:28.000000 wwpdb.utils.oe_util-0.7.1/wwpdb.utils.oe_util.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-17 11:32:17.397557 wwpdb.utils.oe_util-0.8/
+-rw-r--r--   0 vsts      (1001) docker     (123)      730 2023-06-17 11:32:17.397557 wwpdb.utils.oe_util-0.8/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1222 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-17 11:32:17.397557 wwpdb.utils.oe_util-0.8/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2397 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-17 11:32:17.393557 wwpdb.utils.oe_util-0.8/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-17 11:32:17.393557 wwpdb.utils.oe_util-0.8/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-17 11:32:17.393557 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/
+-rw-r--r--   0 vsts      (1001) docker     (123)      149 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-17 11:32:17.397557 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/
+-rw-r--r--   0 vsts      (1001) docker     (123)    10746 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/OeBuildModelMol.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19744 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/OeBuildMol.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4150 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/OeChemCompIoUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1366 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/OeDescriptorUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16791 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/OePersist.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14062 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/PdbxBuildChemComp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-17 11:32:17.397557 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/
+-rw-r--r--   0 vsts      (1001) docker     (123)    28515 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/OeAlignDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    45990 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/OeAlignDepictUtils.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     9099 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/OeDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2719 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/modMCSAlign.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3373 2023-06-17 11:31:11.000000 wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/simple-example.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-17 11:32:17.393557 wwpdb.utils.oe_util-0.8/wwpdb.utils.oe_util.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      730 2023-06-17 11:32:17.000000 wwpdb.utils.oe_util-0.8/wwpdb.utils.oe_util.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      931 2023-06-17 11:32:17.000000 wwpdb.utils.oe_util-0.8/wwpdb.utils.oe_util.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-17 11:32:17.000000 wwpdb.utils.oe_util-0.8/wwpdb.utils.oe_util.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-17 11:31:45.000000 wwpdb.utils.oe_util-0.8/wwpdb.utils.oe_util.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-06-17 11:32:17.000000 wwpdb.utils.oe_util-0.8/wwpdb.utils.oe_util.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-17 11:32:17.000000 wwpdb.utils.oe_util-0.8/wwpdb.utils.oe_util.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.oe_util-0.7.1/PKG-INFO` & `wwpdb.utils.oe_util-0.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.oe_util
-Version: 0.7.1
+Version: 0.8
 Summary: wwPDB workflow engine utils
 Home-page: https://github.com/rcsb/py-wwpdb_apps_wf_engine_utils
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.oe_util-0.7.1/README.md` & `wwpdb.utils.oe_util-0.8/README.md`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.7.1/setup.py` & `wwpdb.utils.oe_util-0.8/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/build/OeBuildModelMol.py` & `wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/OeBuildModelMol.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/build/OeBuildMol.py` & `wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/OeBuildMol.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/build/OeChemCompIoUtils.py` & `wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/OeChemCompIoUtils.py`

 * *Files 14% similar despite different names*

```diff
@@ -86,11 +86,23 @@
             if len(ide) < 1:
                 continue
             idU = str(ide).upper()
             if idU.startswith("PRDCC_"):
                 hashd = idU[-1]
                 pth = os.path.join(self.__topCachePath, hashd, idU + '.cif')
             else:
-                hashd = idU[0]
+                hashd = self.__getCcdHash(idU)
                 pth = os.path.join(self.__topCachePath, hashd, idU, idU + '.cif')
             pathList.append(pth)
         return self.getFromPathList(pathList, use3D=use3D, coordType=coordType, setTitle=setTitle)
+
+    def __getCcdHash(self, idCode):
+        """Returns the hash code for a CCD id.  Currently first letter"""
+        if not idCode:
+            return None
+
+        if len(idCode) > 3:
+            hash_key = idCode.upper()[-2:]
+        else:
+            hash_key = idCode.upper()[0]
+
+        return hash_key
```

### Comparing `wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/build/OeDescriptorUtils.py` & `wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/OeDescriptorUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/build/OePersist.py` & `wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/OePersist.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/build/PdbxBuildChemComp.py` & `wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/build/PdbxBuildChemComp.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/oedepict/OeAlignDepict.py` & `wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/OeAlignDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/oedepict/OeAlignDepictUtils.py` & `wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/OeAlignDepictUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/oedepict/OeDepict.py` & `wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/OeDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/oedepict/modMCSAlign.py` & `wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/modMCSAlign.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.7.1/wwpdb/utils/oe_util/oedepict/simple-example.py` & `wwpdb.utils.oe_util-0.8/wwpdb/utils/oe_util/oedepict/simple-example.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.oe_util-0.7.1/wwpdb.utils.oe_util.egg-info/PKG-INFO` & `wwpdb.utils.oe_util-0.8/wwpdb.utils.oe_util.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.oe-util
-Version: 0.7.1
+Version: 0.8
 Summary: wwPDB workflow engine utils
 Home-page: https://github.com/rcsb/py-wwpdb_apps_wf_engine_utils
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.oe_util-0.7.1/wwpdb.utils.oe_util.egg-info/SOURCES.txt` & `wwpdb.utils.oe_util-0.8/wwpdb.utils.oe_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

