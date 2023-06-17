# Comparing `tmp/TabularDataInvestigation-0.0.5.tar.gz` & `tmp/TabularDataInvestigation-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TabularDataInvestigation-0.0.5.tar", last modified: Sat Jun 17 06:42:29 2023, max compression
+gzip compressed data, was "TabularDataInvestigation-0.0.6.tar", last modified: Sat Jun 17 06:46:21 2023, max compression
```

## Comparing `TabularDataInvestigation-0.0.5.tar` & `TabularDataInvestigation-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 06:42:29.314095 TabularDataInvestigation-0.0.5/
--rw-rw-rw-   0        0        0     1088 2023-06-16 11:32:51.000000 TabularDataInvestigation-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      913 2023-06-17 06:42:29.315097 TabularDataInvestigation-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-16 11:30:47.000000 TabularDataInvestigation-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 06:42:29.299094 TabularDataInvestigation-0.0.5/TabularDataInvestigation/
--rw-rw-rw-   0        0        0        0 2023-06-16 11:29:46.000000 TabularDataInvestigation-0.0.5/TabularDataInvestigation/__init__.py
--rw-rw-rw-   0        0        0     5774 2023-06-17 06:40:15.000000 TabularDataInvestigation-0.0.5/TabularDataInvestigation/tdi.py
-drwxrwxrwx   0        0        0        0 2023-06-17 06:42:29.313097 TabularDataInvestigation-0.0.5/TabularDataInvestigation.egg-info/
--rw-rw-rw-   0        0        0      913 2023-06-17 06:42:29.000000 TabularDataInvestigation-0.0.5/TabularDataInvestigation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-06-17 06:42:29.000000 TabularDataInvestigation-0.0.5/TabularDataInvestigation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 06:42:29.000000 TabularDataInvestigation-0.0.5/TabularDataInvestigation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-17 06:42:29.000000 TabularDataInvestigation-0.0.5/TabularDataInvestigation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-17 06:42:29.000000 TabularDataInvestigation-0.0.5/TabularDataInvestigation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-17 06:42:29.317095 TabularDataInvestigation-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1260 2023-06-17 06:42:22.000000 TabularDataInvestigation-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 06:46:21.559647 TabularDataInvestigation-0.0.6/
+-rw-rw-rw-   0        0        0     1088 2023-06-16 11:32:51.000000 TabularDataInvestigation-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      913 2023-06-17 06:46:21.560652 TabularDataInvestigation-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-16 11:30:47.000000 TabularDataInvestigation-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 06:46:21.536649 TabularDataInvestigation-0.0.6/TabularDataInvestigation/
+-rw-rw-rw-   0        0        0        0 2023-06-16 11:29:46.000000 TabularDataInvestigation-0.0.6/TabularDataInvestigation/__init__.py
+-rw-rw-rw-   0        0        0     5777 2023-06-17 06:45:43.000000 TabularDataInvestigation-0.0.6/TabularDataInvestigation/tdi.py
+drwxrwxrwx   0        0        0        0 2023-06-17 06:46:21.558649 TabularDataInvestigation-0.0.6/TabularDataInvestigation.egg-info/
+-rw-rw-rw-   0        0        0      913 2023-06-17 06:46:21.000000 TabularDataInvestigation-0.0.6/TabularDataInvestigation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-06-17 06:46:21.000000 TabularDataInvestigation-0.0.6/TabularDataInvestigation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 06:46:21.000000 TabularDataInvestigation-0.0.6/TabularDataInvestigation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-17 06:46:21.000000 TabularDataInvestigation-0.0.6/TabularDataInvestigation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-17 06:46:21.000000 TabularDataInvestigation-0.0.6/TabularDataInvestigation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-17 06:46:21.562648 TabularDataInvestigation-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1260 2023-06-17 06:46:04.000000 TabularDataInvestigation-0.0.6/setup.py
```

### Comparing `TabularDataInvestigation-0.0.5/LICENSE.txt` & `TabularDataInvestigation-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `TabularDataInvestigation-0.0.5/PKG-INFO` & `TabularDataInvestigation-0.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: TabularDataInvestigation
-Version: 0.0.5
+Version: 0.0.6
 Summary: This package provide a fast tabular data investigation and it will eligible for ML model building and also helps to developers in their projects when needed 
 Home-page: https://github.com/Tanvir223/TabularDataInvestigation
-Download-URL: https://github.com/Tanvir223/TabularDataInvestigation/archive/refs/tags/0.0.5.tar.gz
+Download-URL: https://github.com/Tanvir223/TabularDataInvestigation/archive/refs/tags/0.0.6.tar.gz
 Author: Tanvir Islam
 Author-email: islamtanvir659@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Tanvir223/TabularDataInvestigation/issues
 Keywords: pypi,TabularDataInvestigation,TabularData,Data-Manupulation,Data-Preprocessing,Data Cleaning,Machine Learning,Artificial Intelligence,Industry Data,Data Science
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `TabularDataInvestigation-0.0.5/TabularDataInvestigation/tdi.py` & `TabularDataInvestigation-0.0.6/TabularDataInvestigation/tdi.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         response.reset_index(drop=True, inplace=True)
         return response
     else:
         return 'invalid return type'
     
 def find_special_char_index(df, return_type = 'dataframe'):
     # define a regular expression pattern that matches any special character
-    pattern = r'[^a-zA-Z0-9]'
+    pattern = r'[^a-zA-Z0-9\s.]'
     response = pd.DataFrame(columns = ['columns', 'has_special_char_at'])
 
     for col in df.columns:
         # apply the regular expression to each cell in the dataframe
         matches = df[col].astype(str).str.contains(pattern).reset_index()
         indexes_spacial_char = matches[matches[col] == True]['index'].values.tolist()
         response.loc[col] = [col, indexes_spacial_char]
```

### Comparing `TabularDataInvestigation-0.0.5/TabularDataInvestigation.egg-info/PKG-INFO` & `TabularDataInvestigation-0.0.6/TabularDataInvestigation.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: TabularDataInvestigation
-Version: 0.0.5
+Version: 0.0.6
 Summary: This package provide a fast tabular data investigation and it will eligible for ML model building and also helps to developers in their projects when needed 
 Home-page: https://github.com/Tanvir223/TabularDataInvestigation
-Download-URL: https://github.com/Tanvir223/TabularDataInvestigation/archive/refs/tags/0.0.5.tar.gz
+Download-URL: https://github.com/Tanvir223/TabularDataInvestigation/archive/refs/tags/0.0.6.tar.gz
 Author: Tanvir Islam
 Author-email: islamtanvir659@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Tanvir223/TabularDataInvestigation/issues
 Keywords: pypi,TabularDataInvestigation,TabularData,Data-Manupulation,Data-Preprocessing,Data Cleaning,Machine Learning,Artificial Intelligence,Industry Data,Data Science
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `TabularDataInvestigation-0.0.5/setup.py` & `TabularDataInvestigation-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='TabularDataInvestigation',
     packages=['TabularDataInvestigation'],
-    version='0.0.5',
+    version='0.0.6',
     license='MIT',
     description='This package provide a fast tabular data investigation and it will eligible for ML model building and also helps to developers in their projects when needed ',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Tanvir Islam',
     author_email='islamtanvir659@gmail.com',
     url='https://github.com/Tanvir223/TabularDataInvestigation',
     project_urls = {
         "Bug Tracker": "https://github.com/Tanvir223/TabularDataInvestigation/issues"
     },
     install_requires=['requests'],
 
-    download_url="https://github.com/Tanvir223/TabularDataInvestigation/archive/refs/tags/0.0.5.tar.gz",
+    download_url="https://github.com/Tanvir223/TabularDataInvestigation/archive/refs/tags/0.0.6.tar.gz",
     keywords=["pypi", "TabularDataInvestigation", "TabularData", "Data-Manupulation", "Data-Preprocessing", "Data Cleaning","Machine Learning", "Artificial Intelligence", "Industry Data" , "Data Science"],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.10'
     ]
 )
```

