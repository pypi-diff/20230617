# Comparing `tmp/datamatic-0.1.6.tar.gz` & `tmp/datamatic-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamatic-0.1.6.tar", max compression
+gzip compressed data, was "datamatic-0.1.7.tar", max compression
```

## Comparing `datamatic-0.1.6.tar` & `datamatic-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datamatic-0.1.6/LICENSE
--rw-r--r--   0        0        0     2625 2023-06-17 03:43:27.391323 datamatic-0.1.6/datamatic/__init__.py
--rw-r--r--   0        0        0      338 2023-06-16 12:59:32.220890 datamatic-0.1.6/datamatic/exceptions.py
--rw-r--r--   0        0        0      464 2023-06-17 03:28:12.383150 datamatic-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      318 1970-01-01 00:00:00.000000 datamatic-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-16 12:22:48.812559 datamatic-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2245 2023-06-17 11:23:17.132802 datamatic-0.1.7/datamatic/__init__.py
+-rw-r--r--   0        0        0      338 2023-06-16 12:59:32.220890 datamatic-0.1.7/datamatic/exceptions.py
+-rw-r--r--   0        0        0      464 2023-06-17 11:23:20.765494 datamatic-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      318 1970-01-01 00:00:00.000000 datamatic-0.1.7/PKG-INFO
```

### Comparing `datamatic-0.1.6/LICENSE` & `datamatic-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `datamatic-0.1.6/datamatic/__init__.py` & `datamatic-0.1.7/datamatic/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,32 +41,23 @@
     if (response.status_code == 400): raise AuthorizationError()
     if (response.status_code >= 500): raise DataMaticInternalError()
 
     python_code = response.json()
     if code: return python_code
     
     import pandas as pd
+    globals = { "pd": pd }
     locals = dataframes.copy()
-    locals["pd"] = pd
     try:
-      exec(python_code, {}, locals) # ;return_df=return_df.reset_index(drop=True)
+      exec(python_code, globals, locals)
       if isinstance(locals["return_df"], pd.DataFrame):
         return_df=locals["return_df"].reset_index(drop=True)
       else:
         num_retries += 1
         data["error"] = "Is not a pandas dataframe. Please return dataframe."
         return_df = self.sql(query, dataframes, error=data["error"], code=code, num_retries=num_retries)
     except Exception as e:
       num_retries += 1
       data["error"] = f"Threw exception: `{e}`"
       return_df = self.sql(query, dataframes, error=data["error"], code=code, num_retries=num_retries)
     
-    return return_df
-  
-    # try:
-    #   import pandas as pd
-    #   locals = dataframes.copy()
-    #   locals["pd"] = pd
-    #   exec(python_code + ";return_df=return_df.reset_index(drop=True)", {}, locals)
-    #   return locals["return_df"]
-    # except Exception as e:
-    #   raise DataMaticInternalError("Could not convert the query to a pandas dataframe.")
+    return return_df
```

