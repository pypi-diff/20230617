# Comparing `tmp/datamatic-0.1.3.tar.gz` & `tmp/datamatic-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamatic-0.1.3.tar", max compression
+gzip compressed data, was "datamatic-0.1.4.tar", max compression
```

## Comparing `datamatic-0.1.3.tar` & `datamatic-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datamatic-0.1.3/LICENSE
--rw-r--r--   0        0        0     1688 2023-06-16 20:08:59.450621 datamatic-0.1.3/datamatic/__init__.py
--rw-r--r--   0        0        0      338 2023-06-16 12:59:32.220890 datamatic-0.1.3/datamatic/exceptions.py
--rw-r--r--   0        0        0      463 2023-06-16 20:12:04.378169 datamatic-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 datamatic-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datamatic-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2008 2023-06-16 22:50:48.792403 datamatic-0.1.4/datamatic/__init__.py
+-rw-r--r--   0        0        0      338 2023-06-16 12:59:32.220890 datamatic-0.1.4/datamatic/exceptions.py
+-rw-r--r--   0        0        0      464 2023-06-16 22:49:44.850459 datamatic-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      318 1970-01-01 00:00:00.000000 datamatic-0.1.4/PKG-INFO
```

### Comparing `datamatic-0.1.3/LICENSE` & `datamatic-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datamatic-0.1.3/datamatic/__init__.py` & `datamatic-0.1.4/datamatic/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     self, 
     api_base="https://datamatic-z9aq.vercel.app/api",
     api_key=None
   ):
     load_dotenv()
     self.api_base = api_base if api_base else os.getenv("DATAMATIC_API_BASE")
     self.api_key = api_key if api_key else os.getenv("DATAMATIC_API_KEY")
-    print(self.api_key)
     
   @retry(exceptions=(RequestException, DataMaticInternalError), tries=3, delay=2)
   def sql(self, query, dataframes, code=False):
     if not (type(dataframes) is dict): raise Exception("dataframes needs to be a dictionary with key being dataframe name and value being the dataframe.")
 
     data = {
       "dataframe": "\n".join([f"{idx+1}. Dataframe named {key} with columns {value.columns.tolist()}" for idx, (key, value) in enumerate(dataframes.items())]),
@@ -47,8 +46,17 @@
     locals = dataframes.copy()
     locals["pd"] = pd
     try:
       exec(python_code + ";return_df=return_df.reset_index(drop=True)", {}, locals)
     except Exception as e:
       pass
     
-    return locals["return_df"]
+    return locals["return_df"]
+  
+    # try:
+    #   import pandas as pd
+    #   locals = dataframes.copy()
+    #   locals["pd"] = pd
+    #   exec(python_code + ";return_df=return_df.reset_index(drop=True)", {}, locals)
+    #   return locals["return_df"]
+    # except Exception as e:
+    #   raise DataMaticInternalError("Could not convert the query to a pandas dataframe.")
```

