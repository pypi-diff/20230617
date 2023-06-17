# Comparing `tmp/expert_intelligence_toolbox-0.0.5.tar.gz` & `tmp/expert_intelligence_toolbox-0.0.6.tar.gz`

## Comparing `expert_intelligence_toolbox-0.0.5.tar` & `expert_intelligence_toolbox-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.5/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.5/src/expert_intelligence_toolbox/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.5/src/expert_intelligence_toolbox/example.py
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.5/src/expert_intelligence_toolbox/snowflake_connector.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.5/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.5/LICENSE
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.5/README.md
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.6/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.6/src/expert_intelligence_toolbox/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.6/src/expert_intelligence_toolbox/example.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.6/src/expert_intelligence_toolbox/snowflake_connector.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.6/README.md
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 expert_intelligence_toolbox-0.0.6/PKG-INFO
```

### Comparing `expert_intelligence_toolbox-0.0.5/src/expert_intelligence_toolbox/snowflake_connector.py` & `expert_intelligence_toolbox-0.0.6/src/expert_intelligence_toolbox/snowflake_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,12 +74,7 @@
     }
     session = Session.builder.configs(snowflake_conn_prop).create()
     # Load data into Pandas dataframe
     data_obj = session.sql(query)
     df = data_obj.toPandas()
 
     return df
-
-
-def test_test():
-
-    print("hehehehheee")
```

### Comparing `expert_intelligence_toolbox-0.0.5/LICENSE` & `expert_intelligence_toolbox-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `expert_intelligence_toolbox-0.0.5/README.md` & `expert_intelligence_toolbox-0.0.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -14,27 +14,36 @@
 - LICENSE: This file includes the license under which your package is distributed. It is important to choose and include the appropriate license file, as we discussed in the previous response.
 
 - requirements.txt or pyproject.toml: These files are used to specify the dependencies required by your package. requirements.txt is a common format that lists the package names and versions, while pyproject.toml is used in the context of projects using the Poetry dependency manager.
 
 
 # How to get the package ready.
 
+**For Unix/MacOS**: see this https://packaging.python.org/en/latest/tutorials/packaging-projects/
+
 1 - Make a 'wheel' and source distribution file (you pack the source code as binary and tar file)
 `py -m pip install --upgrade build`
 `py -m build`
 
 2 - go to https://test.pypi.org/account/register/ and complete the steps on that page. Verify your email address.
 
 3 - To securely upload your project, you’ll need a PyPI API token. Create one at https://test.pypi.org/manage/account/#api-tokens, setting the “Scope” to “Entire account”. Don’t close the page until you have copied and saved the token — you won’t see that token again.
 
 4 - Upload to PyPI test index
 `py -m pip install --upgrade twine`
 `py -m twine upload --repository testpypi dist/*`
 Username: __token__
 PW: enter your token here (WARNING - CTRL-V WILL NOT WORK. IN VSCODE: Edit --> Paste)
+**Note**: 
+- Be carefull to check whether you're using the `pypi` or `test.pypi` to access the package.
+This tutorial is for `test.pypi`, so if you're using `pypi`, please change from `--repository testpypi` into `--repository pypi`
+- If you can't not get to the package using `API key`, using (not recommend, may cause leak private information)
+```bash
+twine upload -u YOUR-USERNAME -p YOUR-PASSWORD --repository testpypi dist/*
+```
 
 5 - you can pull your own package from 
 py -m pip install --index-url https://test.pypi.org/simple/ --no-deps expert_intelligence_toolbox
 
 6 - make a real package
 delete `dist` directory
 `py -m build`
```

### Comparing `expert_intelligence_toolbox-0.0.5/pyproject.toml` & `expert_intelligence_toolbox-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "expert_intelligence_toolbox"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Arnold Kuersteiner", email="arnold.kuersteiner@expert-intelligence.com" },
 ]
 description = "This is (for now) a test."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

