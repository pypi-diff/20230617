# Comparing `tmp/spark_quality_rules_tools-0.2.7.tar.gz` & `tmp/spark_quality_rules_tools-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_quality_rules_tools-0.2.7.tar", last modified: Wed Jun 14 15:30:04 2023, max compression
+gzip compressed data, was "spark_quality_rules_tools-0.2.8.tar", last modified: Sat Jun 17 21:30:52 2023, max compression
```

## Comparing `spark_quality_rules_tools-0.2.7.tar` & `spark_quality_rules_tools-0.2.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 15:30:04.475709 spark_quality_rules_tools-0.2.7/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.7/LICENSE
--rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0     4041 2023-06-14 15:30:04.475709 spark_quality_rules_tools-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.2.7/README.md
--rw-rw-rw-   0        0        0      643 2023-06-14 13:22:39.000000 spark_quality_rules_tools-0.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-06-14 15:30:04.476709 spark_quality_rules_tools-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-06-14 15:29:55.000000 spark_quality_rules_tools-0.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:30:04.455705 spark_quality_rules_tools-0.2.7/spark_quality_rules_tools/
--rw-rw-rw-   0        0        0     1477 2023-06-14 13:37:36.000000 spark_quality_rules_tools-0.2.7/spark_quality_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:30:04.471708 spark_quality_rules_tools-0.2.7/spark_quality_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.7/spark_quality_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    20640 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.2.7/spark_quality_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:30:04.473708 spark_quality_rules_tools-0.2.7/spark_quality_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.7/spark_quality_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.2.7/spark_quality_rules_tools/utils/color.py
--rw-rw-rw-   0        0        0     2113 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.7/spark_quality_rules_tools/utils/resolve.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:30:04.474709 spark_quality_rules_tools-0.2.7/spark_quality_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0      716 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.7/spark_quality_rules_tools/utils/resource/resolve.conf
--rw-rw-rw-   0        0        0    25817 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.2.7/spark_quality_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0     3344 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.2.7/spark_quality_rules_tools/utils/rules.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:30:04.469707 spark_quality_rules_tools-0.2.7/spark_quality_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     4041 2023-06-14 15:30:04.000000 spark_quality_rules_tools-0.2.7/spark_quality_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      717 2023-06-14 15:30:04.000000 spark_quality_rules_tools-0.2.7/spark_quality_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 15:30:04.000000 spark_quality_rules_tools-0.2.7/spark_quality_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      173 2023-06-14 15:30:04.000000 spark_quality_rules_tools-0.2.7/spark_quality_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-06-14 15:30:04.000000 spark_quality_rules_tools-0.2.7/spark_quality_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 21:30:52.376355 spark_quality_rules_tools-0.2.8/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.2.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     4041 2023-06-17 21:30:52.376355 spark_quality_rules_tools-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.2.8/README.md
+-rw-rw-rw-   0        0        0      643 2023-06-14 13:22:39.000000 spark_quality_rules_tools-0.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-06-17 21:30:52.380355 spark_quality_rules_tools-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-06-17 21:29:22.000000 spark_quality_rules_tools-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 21:30:52.360351 spark_quality_rules_tools-0.2.8/spark_quality_rules_tools/
+-rw-rw-rw-   0        0        0     1477 2023-06-14 13:37:36.000000 spark_quality_rules_tools-0.2.8/spark_quality_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 21:30:52.372353 spark_quality_rules_tools-0.2.8/spark_quality_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.8/spark_quality_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    21148 2023-06-17 21:29:22.000000 spark_quality_rules_tools-0.2.8/spark_quality_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-06-17 21:30:52.374354 spark_quality_rules_tools-0.2.8/spark_quality_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.8/spark_quality_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.2.8/spark_quality_rules_tools/utils/color.py
+-rw-rw-rw-   0        0        0     2113 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.8/spark_quality_rules_tools/utils/resolve.py
+drwxrwxrwx   0        0        0        0 2023-06-17 21:30:52.375354 spark_quality_rules_tools-0.2.8/spark_quality_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0      716 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.2.8/spark_quality_rules_tools/utils/resource/resolve.conf
+-rw-rw-rw-   0        0        0    25817 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.2.8/spark_quality_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0     3344 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.2.8/spark_quality_rules_tools/utils/rules.py
+drwxrwxrwx   0        0        0        0 2023-06-17 21:30:52.371354 spark_quality_rules_tools-0.2.8/spark_quality_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     4041 2023-06-17 21:30:52.000000 spark_quality_rules_tools-0.2.8/spark_quality_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      717 2023-06-17 21:30:52.000000 spark_quality_rules_tools-0.2.8/spark_quality_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 21:30:52.000000 spark_quality_rules_tools-0.2.8/spark_quality_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2023-06-17 21:30:52.000000 spark_quality_rules_tools-0.2.8/spark_quality_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-06-17 21:30:52.000000 spark_quality_rules_tools-0.2.8/spark_quality_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_quality_rules_tools-0.2.7/LICENSE` & `spark_quality_rules_tools-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.7/PKG-INFO` & `spark_quality_rules_tools-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_quality_rules_tools
-Version: 0.2.7
+Version: 0.2.8
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.2.7/README.md` & `spark_quality_rules_tools-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.7/pyproject.toml` & `spark_quality_rules_tools-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.7/setup.py` & `spark_quality_rules_tools-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_quality_rules_tools',
     packages=find_packages(),
-    version='0.2.7',
+    version='0.2.8',
     description='spark_quality_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_quality_rules_tools/',
     download_url='https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip',
```

### Comparing `spark_quality_rules_tools-0.2.7/spark_quality_rules_tools/__init__.py` & `spark_quality_rules_tools-0.2.8/spark_quality_rules_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.7/spark_quality_rules_tools/functions/generator.py` & `spark_quality_rules_tools-0.2.8/spark_quality_rules_tools/functions/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,16 @@
 
     with open(dir_confs_filename) as f:
         hammurabi_conf = f.read()
 
     variables_1 = sorted(list(set(re.findall(r'{([a-zA-Z_.-]+)}', hammurabi_conf))))
     variables_2 = sorted(list(set(re.findall(r'{?([a-zA-Z_.-]+)}', hammurabi_conf))))
     variables_list = list(set(variables_1 + variables_2))
-    variables_dict = {variables: "" for variables in variables_list}
+    variables_dict = {variables: "" for variables in variables_list if
+                      variables not in ("ARTIFACTORY_UNIQUE_CACHE", "SCHEMAS_REPOSITORY")}
 
     parameter_dict = dict()
     parameter_dict[uuaa_name] = list()
     parameter_dict[uuaa_name].append({"table": url_conf_name,
                                       "conf_name": url_conf_extension,
                                       "parameters": variables_dict})
 
@@ -249,15 +250,16 @@
     print(f"{get_color('parameters:')} {get_color_b(params)}")
     print(f"{get_color('=================================')} ")
 
 
 def dq_run_sandbox(spark=None,
                    sc=None,
                    parameter_conf_list=None,
-                   url_conf=None):
+                   url_conf=None,
+                   is_prod=True):
     import json
     import sys
     import os
     from datetime import datetime
     from tqdm import tqdm
     from pyhocon import ConfigFactory
     from pyhocon.converter import HOCONConverter
@@ -322,21 +324,29 @@
     validate_compare_parameters = (sorted(validate_parameter_keys) == sorted(validate_parameter_conf_keys))
     if not validate_compare_parameters:
         raise Exception(f'Need more variables the parameters: parameter_conf_list')
 
     cutoff_date = ""
     with open(dir_confs_filename) as f:
         txt_conf = f.read()
+
+    txt_conf = txt_conf.replace(f'"/artifactory/"', "/artifactory/")
+    txt_conf = txt_conf.replace(f'${{ARTIFACTORY_UNIQUE_CACHE}}',
+                                "http://artifactory-gdt.central-02.nextgen.igrupobbva")
+    if is_prod:
+        txt_conf = txt_conf.replace(f'${{SCHEMAS_REPOSITORY}}', "gl-datio-da-generic-local")
+    else:
+        txt_conf = txt_conf.replace(f'${{SCHEMAS_REPOSITORY}}', "gl-datio-da-generic-dev-local")
+
     for params_parameter_conf in tqdm(parameter_conf_list):
         for k, v in params_parameter_conf.items():
             if str(k).upper() in ("ODATE", "ODATE_DATE", "CUTOFF_DATE"):
                 cutoff_date = str(v).replace("-", "").strip()
             txt_conf = txt_conf.replace(f'${{{k}}}', v)
             txt_conf = txt_conf.replace(f'${{?{k}}}', v)
-    txt_conf = txt_conf.replace(f'"/artifactory/"', "/artifactory/")
     dir_reports_name_filename = os.path.join(dir_reports_name, uuaa_name,
                                              f"{url_conf_name}_{current_datetime_str}_{cutoff_date}.csv")
     if is_windows:
         dir_reports_name_filename = dir_reports_name_filename.replace("\\", "/")
     os.makedirs(os.path.dirname(dir_reports_name_filename), exist_ok=True)
 
     conf_file = ConfigFactory.parse_string(txt_conf)
```

### Comparing `spark_quality_rules_tools-0.2.7/spark_quality_rules_tools/utils/resolve.py` & `spark_quality_rules_tools-0.2.8/spark_quality_rules_tools/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.7/spark_quality_rules_tools/utils/resource/resolve.conf` & `spark_quality_rules_tools-0.2.8/spark_quality_rules_tools/utils/resource/resolve.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.7/spark_quality_rules_tools/utils/resource/rules.json` & `spark_quality_rules_tools-0.2.8/spark_quality_rules_tools/utils/resource/rules.json`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.7/spark_quality_rules_tools/utils/rules.py` & `spark_quality_rules_tools-0.2.8/spark_quality_rules_tools/utils/rules.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.2.7/spark_quality_rules_tools.egg-info/PKG-INFO` & `spark_quality_rules_tools-0.2.8/spark_quality_rules_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-quality-rules-tools
-Version: 0.2.7
+Version: 0.2.8
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.2.7/spark_quality_rules_tools.egg-info/SOURCES.txt` & `spark_quality_rules_tools-0.2.8/spark_quality_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

