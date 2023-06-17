# Comparing `tmp/authomize-rest-api-client-4.2.6.tar.gz` & `tmp/authomize-rest-api-client-4.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-4.2.6.tar", last modified: Mon Jun 12 11:24:29 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-4.2.7.tar", last modified: Sat Jun 17 05:35:26 2023, max compression
```

## Comparing `authomize-rest-api-client-4.2.6.tar` & `authomize-rest-api-client-4.2.7.tar`

### file list

```diff
@@ -1,44 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2194 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10358 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    13027 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76002 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37380 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   190165 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89370 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-06-12 11:24:29.000000 authomize-rest-api-client-4.2.6/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1377 2023-06-12 11:24:29.000000 authomize-rest-api-client-4.2.6/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 11:24:29.000000 authomize-rest-api-client-4.2.6/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      214 2023-06-12 11:24:29.000000 authomize-rest-api-client-4.2.6/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-12 11:24:29.000000 authomize-rest-api-client-4.2.6/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-06-12 11:24:29.528043 authomize-rest-api-client-4.2.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1161 2023-06-12 11:24:28.000000 authomize-rest-api-client-4.2.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:24:29.524043 authomize-rest-api-client-4.2.6/tests/
--rw-r--r--   0 root         (0) root         (0)      205 2023-06-12 11:24:05.000000 authomize-rest-api-client-4.2.6/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 05:35:26.156314 authomize-rest-api-client-4.2.7/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-06-17 05:35:05.000000 authomize-rest-api-client-4.2.7/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-06-17 05:35:05.000000 authomize-rest-api-client-4.2.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-06-17 05:35:26.156314 authomize-rest-api-client-4.2.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2194 2023-06-17 05:35:05.000000 authomize-rest-api-client-4.2.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 05:35:26.152314 authomize-rest-api-client-4.2.7/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 05:35:26.156314 authomize-rest-api-client-4.2.7/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-06-17 05:35:05.000000 authomize-rest-api-client-4.2.7/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 05:35:26.156314 authomize-rest-api-client-4.2.7/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-17 05:35:05.000000 authomize-rest-api-client-4.2.7/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-06-17 05:35:05.000000 authomize-rest-api-client-4.2.7/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10358 2023-06-17 05:35:05.000000 authomize-rest-api-client-4.2.7/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    13027 2023-06-17 05:35:05.000000 authomize-rest-api-client-4.2.7/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-06-17 05:35:05.000000 authomize-rest-api-client-4.2.7/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 05:35:26.156314 authomize-rest-api-client-4.2.7/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-17 05:35:05.000000 authomize-rest-api-client-4.2.7/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-06-17 05:35:05.000000 authomize-rest-api-client-4.2.7/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 05:35:26.156314 authomize-rest-api-client-4.2.7/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-17 05:35:05.000000 authomize-rest-api-client-4.2.7/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 05:35:26.156314 authomize-rest-api-client-4.2.7/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-17 05:35:05.000000 authomize-rest-api-client-4.2.7/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76002 2023-06-17 05:35:05.000000 authomize-rest-api-client-4.2.7/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 05:35:26.156314 authomize-rest-api-client-4.2.7/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-17 05:35:05.000000 authomize-rest-api-client-4.2.7/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37380 2023-06-17 05:35:05.000000 authomize-rest-api-client-4.2.7/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 05:35:26.156314 authomize-rest-api-client-4.2.7/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-17 05:35:05.000000 authomize-rest-api-client-4.2.7/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 05:35:26.156314 authomize-rest-api-client-4.2.7/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-17 05:35:05.000000 authomize-rest-api-client-4.2.7/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   190165 2023-06-17 05:35:05.000000 authomize-rest-api-client-4.2.7/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 05:35:26.156314 authomize-rest-api-client-4.2.7/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-17 05:35:05.000000 authomize-rest-api-client-4.2.7/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89370 2023-06-17 05:35:05.000000 authomize-rest-api-client-4.2.7/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-17 05:35:05.000000 authomize-rest-api-client-4.2.7/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 05:35:26.156314 authomize-rest-api-client-4.2.7/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-06-17 05:35:26.000000 authomize-rest-api-client-4.2.7/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-06-17 05:35:26.000000 authomize-rest-api-client-4.2.7/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 05:35:26.000000 authomize-rest-api-client-4.2.7/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      206 2023-06-17 05:35:26.000000 authomize-rest-api-client-4.2.7/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-17 05:35:26.000000 authomize-rest-api-client-4.2.7/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-06-17 05:35:26.156314 authomize-rest-api-client-4.2.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-06-17 05:35:08.000000 authomize-rest-api-client-4.2.7/setup.py
```

### Comparing `authomize-rest-api-client-4.2.6/LICENSE.txt` & `authomize-rest-api-client-4.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.2.6/README.md` & `authomize-rest-api-client-4.2.7/README.md`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.2.6/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-4.2.7/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.2.6/authomize/rest_api_client/client/base_client.py` & `authomize-rest-api-client-4.2.7/authomize/rest_api_client/client/base_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.2.6/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-4.2.7/authomize/rest_api_client/client/client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.2.6/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-4.2.7/authomize/rest_api_client/client/connectors_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.2.6/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-4.2.7/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.2.6/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-4.2.7/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.2.6/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-4.2.7/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.2.6/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-4.2.7/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.2.6/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-4.2.7/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.2.6/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-4.2.7/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
 authomize/rest_api_client/openapi/external_rest_api/__init__.py
 authomize/rest_api_client/openapi/external_rest_api/openapi.json
 authomize_rest_api_client.egg-info/PKG-INFO
 authomize_rest_api_client.egg-info/SOURCES.txt
 authomize_rest_api_client.egg-info/dependency_links.txt
 authomize_rest_api_client.egg-info/requires.txt
-authomize_rest_api_client.egg-info/top_level.txt
-tests/test_import.py
+authomize_rest_api_client.egg-info/top_level.txt
```

### Comparing `authomize-rest-api-client-4.2.6/setup.py` & `authomize-rest-api-client-4.2.7/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='4.2.6',
+        version='4.2.7',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
             'authomize.rest_api_client': [
                 'openapi/connectors_rest_api/*.json',
                 'openapi/external_rest_api/*.json',
                 'py.typed',
             ],
         },
         install_requires=[
-            'requests~=2.28',
+            'requests~=2.31',
             'api-client-pydantic~=1.2',
         ],
         extras_require={
             'test': [
                 'coverage~=5.2',
                 'flake8~=4.0',
                 'flake8-isort~=4.0',
                 'mypy~=0.910',
                 'pyhamcrest~=2.0',
                 'pytest~=6.2',
                 'pytest-html~=2.1',
-                'types-requests~=2.28.7',
+                'types-requests',
             ],
             'codegen': [
                 'datamodel-code-generator~=0.11',
             ],
         },
     )
```

