# Comparing `tmp/polar_diagrams-1.0.4.tar.gz` & `tmp/polar_diagrams-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polar_diagrams-1.0.4.tar", last modified: Fri Feb 10 14:01:09 2023, max compression
+gzip compressed data, was "polar_diagrams-1.0.5.tar", last modified: Sat Jun 17 17:04:07 2023, max compression
```

## Comparing `polar_diagrams-1.0.4.tar` & `polar_diagrams-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:01:09.989564 polar_diagrams-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-10 14:00:58.000000 polar_diagrams-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-02-10 14:01:09.989564 polar_diagrams-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-02-10 14:00:58.000000 polar_diagrams-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-10 14:00:58.000000 polar_diagrams-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-02-10 14:01:09.993564 polar_diagrams-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:01:09.989564 polar_diagrams-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:01:09.989564 polar_diagrams-1.0.4/src/polar_diagrams/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-02-10 14:00:58.000000 polar_diagrams-1.0.4/src/polar_diagrams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63051 2023-02-10 14:00:58.000000 polar_diagrams-1.0.4/src/polar_diagrams/polar_diagrams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:01:09.989564 polar_diagrams-1.0.4/src/polar_diagrams.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-02-10 14:01:09.000000 polar_diagrams-1.0.4/src/polar_diagrams.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-02-10 14:01:09.000000 polar_diagrams-1.0.4/src/polar_diagrams.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 14:01:09.000000 polar_diagrams-1.0.4/src/polar_diagrams.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-10 14:01:09.000000 polar_diagrams-1.0.4/src/polar_diagrams.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-10 14:01:09.000000 polar_diagrams-1.0.4/src/polar_diagrams.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:01:09.989564 polar_diagrams-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-02-10 14:00:58.000000 polar_diagrams-1.0.4/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:04:07.353727 polar_diagrams-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-17 17:03:57.000000 polar_diagrams-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-06-17 17:04:07.353727 polar_diagrams-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-06-17 17:03:57.000000 polar_diagrams-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-17 17:03:57.000000 polar_diagrams-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-17 17:04:07.353727 polar_diagrams-1.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:04:07.349727 polar_diagrams-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:04:07.349727 polar_diagrams-1.0.5/src/polar_diagrams/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-17 17:03:57.000000 polar_diagrams-1.0.5/src/polar_diagrams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63198 2023-06-17 17:03:57.000000 polar_diagrams-1.0.5/src/polar_diagrams/polar_diagrams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:04:07.349727 polar_diagrams-1.0.5/src/polar_diagrams.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-06-17 17:04:07.000000 polar_diagrams-1.0.5/src/polar_diagrams.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-17 17:04:07.000000 polar_diagrams-1.0.5/src/polar_diagrams.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 17:04:07.000000 polar_diagrams-1.0.5/src/polar_diagrams.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-17 17:04:07.000000 polar_diagrams-1.0.5/src/polar_diagrams.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-17 17:04:07.000000 polar_diagrams-1.0.5/src/polar_diagrams.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:04:07.349727 polar_diagrams-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-06-17 17:03:57.000000 polar_diagrams-1.0.5/tests/test.py
```

### Comparing `polar_diagrams-1.0.4/LICENSE` & `polar_diagrams-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `polar_diagrams-1.0.4/PKG-INFO` & `polar_diagrams-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polar_diagrams
-Version: 1.0.4
+Version: 1.0.5
 Summary: Interactive Polar Diagrams for Model Comparison
 Author: Aleksandar Anžel
 Author-email: aleksandar.anzel@uni-marburg.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -29,14 +29,16 @@
 
 ![GitHub Test Status](https://img.shields.io/github/actions/workflow/status/AAnzel/Polar-Diagrams-for-Model-Comparison/python-package.yml?label=test&style=flat-square)
 ![GitHub Build Status](https://img.shields.io/github/actions/workflow/status/AAnzel/Polar-Diagrams-for-Model-Comparison/python-package.yml?label=build&style=flat-square)
 ![GitHub Publish](https://img.shields.io/github/actions/workflow/status/AAnzel/Polar-Diagrams-for-Model-Comparison/python-publish.yml?label=publish&style=flat-square)
 ![GitHub Issues](https://img.shields.io/github/issues-raw/AAnzel/Polar-Diagrams-for-Model-Comparison?style=flat-square)
 ![PyPI - License](https://img.shields.io/pypi/l/polar-diagrams?style=flat-square)
 ![PyPI](https://img.shields.io/pypi/v/polar-diagrams?style=flat-square)
+![PyPI - Status](https://img.shields.io/pypi/status/polar-diagrams?style=flat-square)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/polar-diagrams?style=flat-square)
 
 ## Manuscript
 
 This library is created for the following paper:
 
 ***"Interactive Polar Diagrams for Model Comparison"*** by Aleksandar Anžel, Dominik Heider, and Georges Hattab
```

### Comparing `polar_diagrams-1.0.4/README.md` & `polar_diagrams-1.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 ![GitHub Test Status](https://img.shields.io/github/actions/workflow/status/AAnzel/Polar-Diagrams-for-Model-Comparison/python-package.yml?label=test&style=flat-square)
 ![GitHub Build Status](https://img.shields.io/github/actions/workflow/status/AAnzel/Polar-Diagrams-for-Model-Comparison/python-package.yml?label=build&style=flat-square)
 ![GitHub Publish](https://img.shields.io/github/actions/workflow/status/AAnzel/Polar-Diagrams-for-Model-Comparison/python-publish.yml?label=publish&style=flat-square)
 ![GitHub Issues](https://img.shields.io/github/issues-raw/AAnzel/Polar-Diagrams-for-Model-Comparison?style=flat-square)
 ![PyPI - License](https://img.shields.io/pypi/l/polar-diagrams?style=flat-square)
 ![PyPI](https://img.shields.io/pypi/v/polar-diagrams?style=flat-square)
+![PyPI - Status](https://img.shields.io/pypi/status/polar-diagrams?style=flat-square)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/polar-diagrams?style=flat-square)
 
 ## Manuscript
 
 This library is created for the following paper:
 
 ***"Interactive Polar Diagrams for Model Comparison"*** by Aleksandar Anžel, Dominik Heider, and Georges Hattab
```

### Comparing `polar_diagrams-1.0.4/setup.cfg` & `polar_diagrams-1.0.5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = polar_diagrams
-version = 1.0.4
+version = 1.0.5
 author = Aleksandar Anžel
 author_email = aleksandar.anzel@uni-marburg.de
 description = Interactive Polar Diagrams for Model Comparison
 long_description = file: README.md, LICENCE
 long_description_content_type = text/markdown
 Source = https://github.com/AAnzel/Polar-Diagrams-for-Model-Comparison
 Tracker = https://github.com/AAnzel/Polar-Diagrams-for-Model-Comparison/issues
```

### Comparing `polar_diagrams-1.0.4/src/polar_diagrams/__init__.py` & `polar_diagrams-1.0.5/src/polar_diagrams/__init__.py`

 * *Files identical despite different names*

### Comparing `polar_diagrams-1.0.4/src/polar_diagrams/polar_diagrams.py` & `polar_diagrams-1.0.5/src/polar_diagrams/polar_diagrams.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,35 +100,37 @@
             df_input[string_reference_model].corr(
                 df_input[string_one_model], method=string_corr_method))
 
         # Calculate arccos of Pearson's correlation
         dict_result[string_one_model].append(math.degrees(
             math.acos(dict_result[string_one_model][-1])))
 
-        # Calculating RMS
+    for string_one_model in list_all_features:
+        # Calculating CRMS
         dict_result[string_one_model].append(
-            mean_squared_error(
+            math.sqrt(mean_squared_error(
                 df_input[string_reference_model],
-                df_input[string_one_model], squared=False))
+                df_input[string_one_model], squared=True) -
+                      (np.mean(df_input[string_reference_model]) -
+                       np.mean(df_input[string_one_model]))**2))
 
-    for string_one_model in list_all_features:
-        # Normalizing the RMS as in the paper
+        # Normalizing the CRMS as in the paper
         dict_result[string_one_model].append(
             dict_result[string_one_model][3] /
             dict_result[string_reference_model][0])
 
         # Calculating normalized standard deviation
         dict_result[string_one_model].append(
             dict_result[string_one_model][0] / dict_result[
                 string_reference_model][0])
 
     df_result = pd.DataFrame().from_dict(
         dict_result, orient='index',
-        columns=['Standard Deviation', 'Correlation', 'Angle', 'RMS',
-                 'Normalized RMS', 'Normalized Standard Deviation'])
+        columns=['Standard Deviation', 'Correlation', 'Angle', 'CRMS',
+                 'Normalized CRMS', 'Normalized Standard Deviation'])
 
     df_result = df_result.reset_index().rename(columns={'index': 'Model'})
 
     return df_result
 
 
 def _float_calculate_discrete_entropy(list_labels, int_base=2):
@@ -740,15 +742,15 @@
             string_radial_column = 'Normalized Standard Deviation'
         else:
             string_radial_column = 'Standard Deviation'
         string_angular_column = 'Angle'
         string_angular_column_label = 'Correlation'
         string_tooltip_label_1 = string_radial_column
         string_tooltip_label_2 = string_angular_column_label
-        string_tooltip_label_3 = 'RMS'
+        string_tooltip_label_3 = 'CRMS'
         bool_only_half = True if (
             list_df_input[0][string_angular_column] <= 90).all() else False
         int_subplot_column_number = 1
         np_angular_labels = np_tmp if bool_only_half else np.concatenate(
             (-np_tmp[:0:-1], np_tmp))
         np_angular_ticks = np.degrees(np.arccos(np_angular_labels))
```

### Comparing `polar_diagrams-1.0.4/src/polar_diagrams.egg-info/PKG-INFO` & `polar_diagrams-1.0.5/src/polar_diagrams.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polar-diagrams
-Version: 1.0.4
+Version: 1.0.5
 Summary: Interactive Polar Diagrams for Model Comparison
 Author: Aleksandar Anžel
 Author-email: aleksandar.anzel@uni-marburg.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -29,14 +29,16 @@
 
 ![GitHub Test Status](https://img.shields.io/github/actions/workflow/status/AAnzel/Polar-Diagrams-for-Model-Comparison/python-package.yml?label=test&style=flat-square)
 ![GitHub Build Status](https://img.shields.io/github/actions/workflow/status/AAnzel/Polar-Diagrams-for-Model-Comparison/python-package.yml?label=build&style=flat-square)
 ![GitHub Publish](https://img.shields.io/github/actions/workflow/status/AAnzel/Polar-Diagrams-for-Model-Comparison/python-publish.yml?label=publish&style=flat-square)
 ![GitHub Issues](https://img.shields.io/github/issues-raw/AAnzel/Polar-Diagrams-for-Model-Comparison?style=flat-square)
 ![PyPI - License](https://img.shields.io/pypi/l/polar-diagrams?style=flat-square)
 ![PyPI](https://img.shields.io/pypi/v/polar-diagrams?style=flat-square)
+![PyPI - Status](https://img.shields.io/pypi/status/polar-diagrams?style=flat-square)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/polar-diagrams?style=flat-square)
 
 ## Manuscript
 
 This library is created for the following paper:
 
 ***"Interactive Polar Diagrams for Model Comparison"*** by Aleksandar Anžel, Dominik Heider, and Georges Hattab
```

### Comparing `polar_diagrams-1.0.4/tests/test.py` & `polar_diagrams-1.0.5/tests/test.py`

 * *Files identical despite different names*

