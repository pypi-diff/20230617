# Comparing `tmp/datamatic-0.1.5.tar.gz` & `tmp/datamatic-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamatic-0.1.5.tar", max compression
+gzip compressed data, was "datamatic-0.1.6.tar", max compression
```

## Comparing `datamatic-0.1.5.tar` & `datamatic-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datamatic-0.1.5/LICENSE
--rw-r--r--   0        0        0     2449 2023-06-17 03:08:37.619789 datamatic-0.1.5/datamatic/__init__.py
--rw-r--r--   0        0        0      338 2023-06-16 12:59:32.220890 datamatic-0.1.5/datamatic/exceptions.py
--rw-r--r--   0        0        0      464 2023-06-17 03:10:00.404176 datamatic-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      318 1970-01-01 00:00:00.000000 datamatic-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datamatic-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2625 2023-06-17 03:43:27.391323 datamatic-0.1.6/datamatic/__init__.py
+-rw-r--r--   0        0        0      338 2023-06-16 12:59:32.220890 datamatic-0.1.6/datamatic/exceptions.py
+-rw-r--r--   0        0        0      464 2023-06-17 03:28:12.383150 datamatic-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      318 1970-01-01 00:00:00.000000 datamatic-0.1.6/PKG-INFO
```

### Comparing `datamatic-0.1.5/LICENSE` & `datamatic-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `datamatic-0.1.5/datamatic/__init__.py` & `datamatic-0.1.6/datamatic/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     load_dotenv()
     self.api_base = api_base if api_base else os.getenv("DATAMATIC_API_BASE")
     self.api_key = api_key if api_key else os.getenv("DATAMATIC_API_KEY")
     
   @retry(exceptions=(RequestException, DataMaticInternalError), tries=3, delay=2)
   def sql(self, query, dataframes, error=None, code=False, num_retries=0):
     if not (type(dataframes) is dict): raise Exception("dataframes needs to be a dictionary with key being dataframe name and value being the dataframe.")
-    if num_retries > 3: raise DataMaticInternalError()
+    if num_retries > 3: raise Exception("We couldn't translate your query. :(")
 
     data = {
       "dataframe": "\n".join([f"{idx+1}. Dataframe named {key} with columns {value.columns.tolist()}" for idx, (key, value) in enumerate(dataframes.items())]),
       "sql": query,
       "error": error
     }
 
@@ -49,19 +49,20 @@
     locals["pd"] = pd
     try:
       exec(python_code, {}, locals) # ;return_df=return_df.reset_index(drop=True)
       if isinstance(locals["return_df"], pd.DataFrame):
         return_df=locals["return_df"].reset_index(drop=True)
       else:
         num_retries += 1
-        data["error"] = "Not a pandas dataframe. Please return dataframe."
+        data["error"] = "Is not a pandas dataframe. Please return dataframe."
         return_df = self.sql(query, dataframes, error=data["error"], code=code, num_retries=num_retries)
     except Exception as e:
-      print(e)
-      pass
+      num_retries += 1
+      data["error"] = f"Threw exception: `{e}`"
+      return_df = self.sql(query, dataframes, error=data["error"], code=code, num_retries=num_retries)
     
     return return_df
   
     # try:
     #   import pandas as pd
     #   locals = dataframes.copy()
     #   locals["pd"] = pd
```

