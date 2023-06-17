# Comparing `tmp/skulk-2.1.6-py2.py3-none-any.whl.zip` & `tmp/skulk-2.1.7-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 11391 bytes, number of entries: 12
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-15 08:38 skulk/VERSION
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 08:37 skulk/__init__.py
--rw-r--r--  2.0 unx    10677 b- defN 23-Jun-15 08:37 skulk/bumper.py
--rw-r--r--  2.0 unx     2294 b- defN 23-Jun-15 08:37 skulk/questions.py
--rw-r--r--  2.0 unx     2601 b- defN 23-Jun-15 08:37 skulk/questions_fallback.py
--rw-r--r--  2.0 unx    10237 b- defN 23-Jun-15 08:37 skulk/skulk.py
--rw-r--r--  2.0 unx     3586 b- defN 23-Jun-15 08:37 skulk/util.py
--rw-r--r--  2.0 unx      675 b- defN 23-Jun-15 08:38 skulk-2.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-15 08:38 skulk-2.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       43 b- defN 23-Jun-15 08:38 skulk-2.1.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-15 08:38 skulk-2.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      894 b- defN 23-Jun-15 08:38 skulk-2.1.6.dist-info/RECORD
-12 files, 31128 bytes uncompressed, 9907 bytes compressed:  68.2%
+Zip file size: 11358 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-17 03:54 skulk/VERSION
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-17 03:54 skulk/__init__.py
+-rw-r--r--  2.0 unx    10725 b- defN 23-Jun-17 03:54 skulk/bumper.py
+-rw-r--r--  2.0 unx     2294 b- defN 23-Jun-17 03:54 skulk/questions.py
+-rw-r--r--  2.0 unx     2601 b- defN 23-Jun-17 03:54 skulk/questions_fallback.py
+-rw-r--r--  2.0 unx    10237 b- defN 23-Jun-17 03:54 skulk/skulk.py
+-rw-r--r--  2.0 unx     3490 b- defN 23-Jun-17 03:54 skulk/util.py
+-rw-r--r--  2.0 unx      675 b- defN 23-Jun-17 03:54 skulk-2.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-17 03:54 skulk-2.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       43 b- defN 23-Jun-17 03:54 skulk-2.1.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-17 03:54 skulk-2.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      894 b- defN 23-Jun-17 03:54 skulk-2.1.7.dist-info/RECORD
+12 files, 31080 bytes uncompressed, 9874 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: skulk/skulk.py
 Comment: 
 
 Filename: skulk/util.py
 Comment: 
 
-Filename: skulk-2.1.6.dist-info/METADATA
+Filename: skulk-2.1.7.dist-info/METADATA
 Comment: 
 
-Filename: skulk-2.1.6.dist-info/WHEEL
+Filename: skulk-2.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: skulk-2.1.6.dist-info/entry_points.txt
+Filename: skulk-2.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: skulk-2.1.6.dist-info/top_level.txt
+Filename: skulk-2.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: skulk-2.1.6.dist-info/RECORD
+Filename: skulk-2.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## skulk/VERSION

```diff
@@ -1 +1 @@
-2.1.6
+2.1.7
```

## skulk/bumper.py

```diff
@@ -67,20 +67,20 @@
 
     def get_versions(self):
         """Fetch the latest tags and PyPi versions."""
         if MOCKED:
             return MOCK_VERSIONS
         else:
             return {
-                "test": self.get_pypi_versions(index=util.TEST_PYPI_INDEX),
+                "test": self.get_pypi_versions(index=TEST_PYPI_INDEX),
                 "pypi": self.get_pypi_versions(),
                 "tags": self.get_tags(),
             }
 
-    def get_pypi_versions(self, index=util.PROD_PYPI_INDEX):
+    def get_pypi_versions(self, index=PROD_PYPI_INDEX):
         """
         Return a list of all PyPi versions for the named package.
         """
         return _get_pypi_versions(self.pip_name, index=index)
 
     def get_tags(self):
         """Return a list of all tags in the repo."""
@@ -215,22 +215,26 @@
         return "0.0.1"
     return version if semver.Version.is_valid(version) else "0.0.1"
 
 
 
 def _get_pypi_versions(pip_name, index):
     url = f"{index}/{pip_name}/json"
+    print(url)
+    
     request = Request(url=url, headers={'User-Agent': 'Mozilla/5.0', "Accept": "application/json"} )
+    
     try:
         response = urlopen(request)
-    except HTTPError as e:
-        print("ERROR:", e)
+    except HTTPError as err:
+        print("ERROR:", err)
         return ["0.0.0"]
     code = response.code
     if code != 200:
+        print("code:", code)
         return  ["0.0.0"]
 
     raw_data = response.read()
     response_encoding = response.headers.get_content_charset("utf-8")
     decoded_data = raw_data.decode(response_encoding)
     data = json.loads(decoded_data)
     if "releases" not in data:
```

## skulk/util.py

```diff
@@ -1,17 +1,14 @@
 import os
 import sys
 from git import InvalidGitRepositoryError, Repo
 
 from git import Repo
 
 MOCKED = True
-PROD_PYPI_INDEX = "https://pypi.org/simple/"
-TEST_PYPI_INDEX = "https://test.pypi.org/simple/"
-
 
 def yellow(rhs):
     """Return the rhs in red."""
     return f"\033[93m{rhs}\033[0m"
 
 
 def green(rhs):
```

## Comparing `skulk-2.1.6.dist-info/METADATA` & `skulk-2.1.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skulk
-Version: 2.1.6
+Version: 2.1.7
 Summary: Streamline release for Conductor client tools and others
 Home-page: https://github.com/ConductorTechnologies/skulk
 Author: Julian Mann
 Author-email: julian@conductortech.com
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python
```

## Comparing `skulk-2.1.6.dist-info/RECORD` & `skulk-2.1.7.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-skulk/VERSION,sha256=JPUCseOr-o6i21WmLdCf175ZHUFbkfgq8M6QzXpEMGM,5
+skulk/VERSION,sha256=UWlFItN7l7WK9wepGFQZFCnWjnLxT6VWRF2wqSNBq3U,5
 skulk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-skulk/bumper.py,sha256=ojOfmd0IlMcyedAPFMIntkLgrrGcVzHH6_yjZY882TM,10677
+skulk/bumper.py,sha256=BCJZNjh73oXR2p6BkLRPiU802TG03iyzRhBgMI91hew,10725
 skulk/questions.py,sha256=ihDx7B1JNw4wQnwjox6BRHpDUM_VzTajmf867IugP-U,2294
 skulk/questions_fallback.py,sha256=aQrtgxnHr6VUlJHO4OcVvPbzJj5V8U2OwXyJ4hBwHi8,2601
 skulk/skulk.py,sha256=OfT4HjKv_1PhjNW2RRs--P6D2GUULrcFXptpQdgjDoY,10237
-skulk/util.py,sha256=uBlyNpq_8RsuD2oOKxk4cL7-2zqXotcBPjI-QHacsHo,3586
-skulk-2.1.6.dist-info/METADATA,sha256=yr4nKLguGVIi51O7OTCOdrV-KehEyQYtWrZMabClwxQ,675
-skulk-2.1.6.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-skulk-2.1.6.dist-info/entry_points.txt,sha256=8DGRFZ3C46ZQBYFsfNj4eYw5ZGq8NWW8uKe-2xC-c34,43
-skulk-2.1.6.dist-info/top_level.txt,sha256=EOnQuA1Vdf2WjOz9xLTPLCynTq2IdzLPGQ54LdhP7oY,6
-skulk-2.1.6.dist-info/RECORD,,
+skulk/util.py,sha256=qoiXmwPmAndSc-NJ7I8LUsyeM3XzdE4_R4IqHufLw_c,3490
+skulk-2.1.7.dist-info/METADATA,sha256=nWKqd_2rAjPpjNulefQjVQTLAz7juSVabR9OweBT9uo,675
+skulk-2.1.7.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+skulk-2.1.7.dist-info/entry_points.txt,sha256=8DGRFZ3C46ZQBYFsfNj4eYw5ZGq8NWW8uKe-2xC-c34,43
+skulk-2.1.7.dist-info/top_level.txt,sha256=EOnQuA1Vdf2WjOz9xLTPLCynTq2IdzLPGQ54LdhP7oY,6
+skulk-2.1.7.dist-info/RECORD,,
```

