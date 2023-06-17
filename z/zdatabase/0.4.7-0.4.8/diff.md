# Comparing `tmp/zdatabase-0.4.7.tar.gz` & `tmp/zdatabase-0.4.8.tar.gz`

## Comparing `zdatabase-0.4.7.tar` & `zdatabase-0.4.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 zdatabase-0.4.7/src/zdatabase/__init__.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 zdatabase-0.4.7/src/zdatabase/model.py
--rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 zdatabase-0.4.7/src/zdatabase/utility.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 zdatabase-0.4.7/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zdatabase-0.4.7/LICENSE
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zdatabase-0.4.7/README.md
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 zdatabase-0.4.7/pyproject.toml
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 zdatabase-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 zdatabase-0.4.8/src/zdatabase/__init__.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 zdatabase-0.4.8/src/zdatabase/model.py
+-rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 zdatabase-0.4.8/src/zdatabase/utility.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 zdatabase-0.4.8/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zdatabase-0.4.8/LICENSE
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zdatabase-0.4.8/README.md
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 zdatabase-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 zdatabase-0.4.8/PKG-INFO
```

### Comparing `zdatabase-0.4.7/src/zdatabase/__init__.py` & `zdatabase-0.4.8/src/zdatabase/__init__.py`

 * *Files identical despite different names*

### Comparing `zdatabase-0.4.7/src/zdatabase/model.py` & `zdatabase-0.4.8/src/zdatabase/model.py`

 * *Files identical despite different names*

### Comparing `zdatabase-0.4.7/src/zdatabase/utility.py` & `zdatabase-0.4.8/src/zdatabase/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from zdatabase import session
+from zdatabase import db
 from jsonschema import validate
 
 
 class DatabaseUtility:
     @staticmethod
     def flush():
-        session.flush()
+        db.session.flush()
 
     @staticmethod
     def commit():
-        session.commit()
+        db.session.commit()
 
     @staticmethod
     def query_(*args, **kwargs):
-        return session.query(*args, **kwargs)
+        return db.session.query(*args, **kwargs)
 
     @staticmethod
     def add_all(items):
-        session.add_all(items)
-        session.commit()
+        db.session.add_all(items)
+        db.session.commit()
         return items
 
 
 class QueryUtility:
     @classmethod
     def select(cls, params, conds):
         """ 筛选(模糊匹配）
```

### Comparing `zdatabase-0.4.7/LICENSE` & `zdatabase-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `zdatabase-0.4.7/pyproject.toml` & `zdatabase-0.4.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zdatabase"
-version = "0.4.7"
+version = "0.4.8"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen database library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `zdatabase-0.4.7/PKG-INFO` & `zdatabase-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zdatabase
-Version: 0.4.7
+Version: 0.4.8
 Summary: zen database library
 Project-URL: Homepage, https://github.com/inspirare6/zdatabase
 Project-URL: Bug Tracker, https://github.com/inspirare6/zdatabase/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

