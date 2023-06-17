# Comparing `tmp/TabularDataInvestigation-0.0.6.tar.gz` & `tmp/TabularDataInvestigation-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TabularDataInvestigation-0.0.6.tar", last modified: Sat Jun 17 06:46:21 2023, max compression
+gzip compressed data, was "TabularDataInvestigation-0.0.7.tar", last modified: Sat Jun 17 08:02:02 2023, max compression
```

## Comparing `TabularDataInvestigation-0.0.6.tar` & `TabularDataInvestigation-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 06:46:21.559647 TabularDataInvestigation-0.0.6/
--rw-rw-rw-   0        0        0     1088 2023-06-16 11:32:51.000000 TabularDataInvestigation-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0      913 2023-06-17 06:46:21.560652 TabularDataInvestigation-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-16 11:30:47.000000 TabularDataInvestigation-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 06:46:21.536649 TabularDataInvestigation-0.0.6/TabularDataInvestigation/
--rw-rw-rw-   0        0        0        0 2023-06-16 11:29:46.000000 TabularDataInvestigation-0.0.6/TabularDataInvestigation/__init__.py
--rw-rw-rw-   0        0        0     5777 2023-06-17 06:45:43.000000 TabularDataInvestigation-0.0.6/TabularDataInvestigation/tdi.py
-drwxrwxrwx   0        0        0        0 2023-06-17 06:46:21.558649 TabularDataInvestigation-0.0.6/TabularDataInvestigation.egg-info/
--rw-rw-rw-   0        0        0      913 2023-06-17 06:46:21.000000 TabularDataInvestigation-0.0.6/TabularDataInvestigation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-06-17 06:46:21.000000 TabularDataInvestigation-0.0.6/TabularDataInvestigation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 06:46:21.000000 TabularDataInvestigation-0.0.6/TabularDataInvestigation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-17 06:46:21.000000 TabularDataInvestigation-0.0.6/TabularDataInvestigation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-17 06:46:21.000000 TabularDataInvestigation-0.0.6/TabularDataInvestigation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-17 06:46:21.562648 TabularDataInvestigation-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1260 2023-06-17 06:46:04.000000 TabularDataInvestigation-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 08:02:02.712310 TabularDataInvestigation-0.0.7/
+-rw-rw-rw-   0        0        0     1088 2023-06-16 11:32:51.000000 TabularDataInvestigation-0.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0    14894 2023-06-17 08:02:02.713310 TabularDataInvestigation-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0    13979 2023-06-17 08:01:56.000000 TabularDataInvestigation-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 08:02:02.682311 TabularDataInvestigation-0.0.7/TabularDataInvestigation/
+-rw-rw-rw-   0        0        0        0 2023-06-16 11:29:46.000000 TabularDataInvestigation-0.0.7/TabularDataInvestigation/__init__.py
+-rw-rw-rw-   0        0        0     5794 2023-06-17 07:59:46.000000 TabularDataInvestigation-0.0.7/TabularDataInvestigation/tdi.py
+drwxrwxrwx   0        0        0        0 2023-06-17 08:02:02.711316 TabularDataInvestigation-0.0.7/TabularDataInvestigation.egg-info/
+-rw-rw-rw-   0        0        0    14894 2023-06-17 08:02:02.000000 TabularDataInvestigation-0.0.7/TabularDataInvestigation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-06-17 08:02:02.000000 TabularDataInvestigation-0.0.7/TabularDataInvestigation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 08:02:02.000000 TabularDataInvestigation-0.0.7/TabularDataInvestigation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-17 08:02:02.000000 TabularDataInvestigation-0.0.7/TabularDataInvestigation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-17 08:02:02.000000 TabularDataInvestigation-0.0.7/TabularDataInvestigation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-17 08:02:02.715311 TabularDataInvestigation-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1260 2023-06-17 07:59:30.000000 TabularDataInvestigation-0.0.7/setup.py
```

### Comparing `TabularDataInvestigation-0.0.6/LICENSE.txt` & `TabularDataInvestigation-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `TabularDataInvestigation-0.0.6/TabularDataInvestigation/tdi.py` & `TabularDataInvestigation-0.0.7/TabularDataInvestigation/tdi.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     #if the row have same value then both of them will return True
     dublicate_checked_df = pd.DataFrame(temp.duplicated(keep=False)).reset_index()
     #return a list of column name which are duplicate
     return list(dublicate_checked_df[dublicate_checked_df[0]==True]['index'])
 
 def correlated_columns(df, return_type='dataframe'):
     risk_variable_df = pd.DataFrame()
-    correalated_df = df.corr()
+    correalated_df = df.corr(numeric_only=True)
     correalated_df.reset_index(inplace=True)
     lst_leakage_cols = []
     lst_leakage_value = []
     for col in correalated_df.columns[1:]:
         
         j = np.where((correalated_df[col] > 0.9) & (col != correalated_df['index']), correalated_df['index'] , 0)
         j = j[np.where(j!=0)]
```

### Comparing `TabularDataInvestigation-0.0.6/setup.py` & `TabularDataInvestigation-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='TabularDataInvestigation',
     packages=['TabularDataInvestigation'],
-    version='0.0.6',
+    version='0.0.7',
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
 
-    download_url="https://github.com/Tanvir223/TabularDataInvestigation/archive/refs/tags/0.0.6.tar.gz",
+    download_url="https://github.com/Tanvir223/TabularDataInvestigation/archive/refs/tags/0.0.7.tar.gz",
     keywords=["pypi", "TabularDataInvestigation", "TabularData", "Data-Manupulation", "Data-Preprocessing", "Data Cleaning","Machine Learning", "Artificial Intelligence", "Industry Data" , "Data Science"],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.10'
     ]
 )
```

