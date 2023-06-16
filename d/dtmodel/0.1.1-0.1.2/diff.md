# Comparing `tmp/dtmodel-0.1.1.tar.gz` & `tmp/dtmodel-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtmodel-0.1.1.tar", max compression
+gzip compressed data, was "dtmodel-0.1.2.tar", max compression
```

## Comparing `dtmodel-0.1.1.tar` & `dtmodel-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1324 2023-06-02 17:19:45.034575 dtmodel-0.1.1/dtmodel/.env
--rw-r--r--   0        0        0       88 2023-06-12 04:49:16.374284 dtmodel-0.1.1/dtmodel/__init__.py
--rw-r--r--   0        0        0      115 2023-06-12 21:18:03.013541 dtmodel-0.1.1/dtmodel/bases/__init__.py
--rw-r--r--   0        0        0      304 2023-06-12 21:29:50.059622 dtmodel-0.1.1/dtmodel/bases/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3560 2023-06-13 04:27:28.265842 dtmodel-0.1.1/dtmodel/bases/__pycache__/facility.cpython-39.pyc
--rw-r--r--   0        0        0     4604 2023-06-13 17:43:08.968458 dtmodel-0.1.1/dtmodel/bases/__pycache__/general.cpython-39.pyc
--rw-r--r--   0        0        0     1577 2023-06-13 17:57:46.852879 dtmodel-0.1.1/dtmodel/bases/__pycache__/medical.cpython-39.pyc
--rw-r--r--   0        0        0     5821 2023-06-13 17:43:08.960204 dtmodel-0.1.1/dtmodel/bases/__pycache__/people.cpython-39.pyc
--rw-r--r--   0        0        0      582 2023-06-13 17:43:07.063185 dtmodel-0.1.1/dtmodel/bases/__pycache__/self_key.cpython-39.pyc
--rw-r--r--   0        0        0     2568 2023-06-13 04:27:28.038908 dtmodel-0.1.1/dtmodel/bases/facility.py
--rw-r--r--   0        0        0     2673 2023-06-13 17:43:06.932755 dtmodel-0.1.1/dtmodel/bases/general.py
--rw-r--r--   0        0        0      977 2023-06-13 17:57:46.452606 dtmodel-0.1.1/dtmodel/bases/medical.py
--rw-r--r--   0        0        0     3631 2023-06-13 16:24:06.049956 dtmodel-0.1.1/dtmodel/bases/people.py
--rw-r--r--   0        0        0      221 2023-06-13 16:24:06.045510 dtmodel-0.1.1/dtmodel/bases/self_key.py
--rw-r--r--   0        0        0       68 2023-06-13 17:57:46.458805 dtmodel-0.1.1/dtmodel/enums/__init__.py
--rw-r--r--   0        0        0      265 2023-06-13 17:57:46.843945 dtmodel-0.1.1/dtmodel/enums/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1198 2023-06-13 03:10:22.624703 dtmodel-0.1.1/dtmodel/enums/__pycache__/facility.cpython-39.pyc
--rw-r--r--   0        0        0      581 2023-06-13 22:55:38.876455 dtmodel-0.1.1/dtmodel/enums/__pycache__/medical.cpython-39.pyc
--rw-r--r--   0        0        0      724 2023-06-13 17:43:08.962350 dtmodel-0.1.1/dtmodel/enums/__pycache__/person.cpython-39.pyc
--rw-r--r--   0        0        0      774 2023-06-13 03:10:22.295967 dtmodel-0.1.1/dtmodel/enums/facility.py
--rw-r--r--   0        0        0      263 2023-06-13 18:31:48.621060 dtmodel-0.1.1/dtmodel/enums/medical.py
--rw-r--r--   0        0        0      313 2023-06-13 16:24:06.058052 dtmodel-0.1.1/dtmodel/enums/person.py
--rw-r--r--   0        0        0     1224 2023-06-12 19:51:27.475674 dtmodel-0.1.1/dtmodel/functions.py
--rw-r--r--   0        0        0       70 2023-06-12 03:19:07.376538 dtmodel-0.1.1/dtmodel/models/__init__.py
--rw-r--r--   0        0        0      266 2023-06-12 03:25:45.653987 dtmodel-0.1.1/dtmodel/models/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1910 2023-06-13 04:03:41.579393 dtmodel-0.1.1/dtmodel/models/__pycache__/facility.cpython-39.pyc
--rw-r--r--   0        0        0     2121 2023-06-13 18:00:19.662916 dtmodel-0.1.1/dtmodel/models/__pycache__/medical.cpython-39.pyc
--rw-r--r--   0        0        0     3236 2023-06-13 17:43:08.977809 dtmodel-0.1.1/dtmodel/models/__pycache__/people.cpython-39.pyc
--rw-r--r--   0        0        0     1233 2023-06-13 04:03:41.210118 dtmodel-0.1.1/dtmodel/models/facility.py
--rw-r--r--   0        0        0     2079 2023-06-13 18:00:19.392445 dtmodel-0.1.1/dtmodel/models/medical.py
--rw-r--r--   0        0        0     2078 2023-06-13 15:52:50.120362 dtmodel-0.1.1/dtmodel/models/people.py
--rw-r--r--   0        0        0      319 2023-06-14 00:47:05.610171 dtmodel-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      659 2023-06-14 00:47:10.432590 dtmodel-0.1.1/setup.py
--rw-r--r--   0        0        0      371 2023-06-14 00:47:10.432879 dtmodel-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1324 2023-06-02 17:19:45.034575 dtmodel-0.1.2/dtmodel/.env
+-rw-r--r--   0        0        0       88 2023-06-12 04:49:16.374284 dtmodel-0.1.2/dtmodel/__init__.py
+-rw-r--r--   0        0        0      115 2023-06-12 21:18:03.013541 dtmodel-0.1.2/dtmodel/bases/__init__.py
+-rw-r--r--   0        0        0      304 2023-06-12 21:29:50.059622 dtmodel-0.1.2/dtmodel/bases/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3560 2023-06-13 04:27:28.265842 dtmodel-0.1.2/dtmodel/bases/__pycache__/facility.cpython-39.pyc
+-rw-r--r--   0        0        0     4604 2023-06-13 17:43:08.968458 dtmodel-0.1.2/dtmodel/bases/__pycache__/general.cpython-39.pyc
+-rw-r--r--   0        0        0     1577 2023-06-13 17:57:46.852879 dtmodel-0.1.2/dtmodel/bases/__pycache__/medical.cpython-39.pyc
+-rw-r--r--   0        0        0     5821 2023-06-13 17:43:08.960204 dtmodel-0.1.2/dtmodel/bases/__pycache__/people.cpython-39.pyc
+-rw-r--r--   0        0        0      582 2023-06-13 17:43:07.063185 dtmodel-0.1.2/dtmodel/bases/__pycache__/self_key.cpython-39.pyc
+-rw-r--r--   0        0        0     2568 2023-06-13 04:27:28.038908 dtmodel-0.1.2/dtmodel/bases/facility.py
+-rw-r--r--   0        0        0     2673 2023-06-13 17:43:06.932755 dtmodel-0.1.2/dtmodel/bases/general.py
+-rw-r--r--   0        0        0      977 2023-06-13 17:57:46.452606 dtmodel-0.1.2/dtmodel/bases/medical.py
+-rw-r--r--   0        0        0     3631 2023-06-13 16:24:06.049956 dtmodel-0.1.2/dtmodel/bases/people.py
+-rw-r--r--   0        0        0      221 2023-06-13 16:24:06.045510 dtmodel-0.1.2/dtmodel/bases/self_key.py
+-rw-r--r--   0        0        0       68 2023-06-13 17:57:46.458805 dtmodel-0.1.2/dtmodel/enums/__init__.py
+-rw-r--r--   0        0        0      265 2023-06-13 17:57:46.843945 dtmodel-0.1.2/dtmodel/enums/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1198 2023-06-13 03:10:22.624703 dtmodel-0.1.2/dtmodel/enums/__pycache__/facility.cpython-39.pyc
+-rw-r--r--   0        0        0      581 2023-06-13 22:55:38.876455 dtmodel-0.1.2/dtmodel/enums/__pycache__/medical.cpython-39.pyc
+-rw-r--r--   0        0        0      724 2023-06-13 17:43:08.962350 dtmodel-0.1.2/dtmodel/enums/__pycache__/person.cpython-39.pyc
+-rw-r--r--   0        0        0      774 2023-06-13 03:10:22.295967 dtmodel-0.1.2/dtmodel/enums/facility.py
+-rw-r--r--   0        0        0      263 2023-06-13 18:31:48.621060 dtmodel-0.1.2/dtmodel/enums/medical.py
+-rw-r--r--   0        0        0      313 2023-06-13 16:24:06.058052 dtmodel-0.1.2/dtmodel/enums/person.py
+-rw-r--r--   0        0        0     1224 2023-06-12 19:51:27.475674 dtmodel-0.1.2/dtmodel/functions.py
+-rw-r--r--   0        0        0       70 2023-06-12 03:19:07.376538 dtmodel-0.1.2/dtmodel/models/__init__.py
+-rw-r--r--   0        0        0      266 2023-06-12 03:25:45.653987 dtmodel-0.1.2/dtmodel/models/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1910 2023-06-13 04:03:41.579393 dtmodel-0.1.2/dtmodel/models/__pycache__/facility.cpython-39.pyc
+-rw-r--r--   0        0        0     2121 2023-06-13 18:00:19.662916 dtmodel-0.1.2/dtmodel/models/__pycache__/medical.cpython-39.pyc
+-rw-r--r--   0        0        0     3236 2023-06-13 17:43:08.977809 dtmodel-0.1.2/dtmodel/models/__pycache__/people.cpython-39.pyc
+-rw-r--r--   0        0        0     1233 2023-06-13 04:03:41.210118 dtmodel-0.1.2/dtmodel/models/facility.py
+-rw-r--r--   0        0        0     2079 2023-06-13 18:00:19.392445 dtmodel-0.1.2/dtmodel/models/medical.py
+-rw-r--r--   0        0        0     2078 2023-06-13 15:52:50.120362 dtmodel-0.1.2/dtmodel/models/people.py
+-rw-r--r--   0        0        0      319 2023-06-16 23:48:37.241621 dtmodel-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      659 2023-06-16 23:48:42.132641 dtmodel-0.1.2/setup.py
+-rw-r--r--   0        0        0      371 2023-06-16 23:48:42.132848 dtmodel-0.1.2/PKG-INFO
```

### Comparing `dtmodel-0.1.1/dtmodel/.env` & `dtmodel-0.1.2/dtmodel/.env`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.1/dtmodel/bases/__pycache__/facility.cpython-39.pyc` & `dtmodel-0.1.2/dtmodel/bases/__pycache__/facility.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.1/dtmodel/bases/__pycache__/general.cpython-39.pyc` & `dtmodel-0.1.2/dtmodel/bases/__pycache__/general.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.1/dtmodel/bases/__pycache__/medical.cpython-39.pyc` & `dtmodel-0.1.2/dtmodel/bases/__pycache__/medical.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.1/dtmodel/bases/__pycache__/people.cpython-39.pyc` & `dtmodel-0.1.2/dtmodel/bases/__pycache__/people.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.1/dtmodel/bases/__pycache__/self_key.cpython-39.pyc` & `dtmodel-0.1.2/dtmodel/bases/__pycache__/self_key.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.1/dtmodel/bases/facility.py` & `dtmodel-0.1.2/dtmodel/bases/facility.py`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.1/dtmodel/bases/general.py` & `dtmodel-0.1.2/dtmodel/bases/general.py`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.1/dtmodel/bases/medical.py` & `dtmodel-0.1.2/dtmodel/bases/medical.py`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.1/dtmodel/bases/people.py` & `dtmodel-0.1.2/dtmodel/bases/people.py`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.1/dtmodel/enums/__pycache__/facility.cpython-39.pyc` & `dtmodel-0.1.2/dtmodel/enums/__pycache__/facility.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.1/dtmodel/enums/__pycache__/medical.cpython-39.pyc` & `dtmodel-0.1.2/dtmodel/enums/__pycache__/medical.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.1/dtmodel/enums/__pycache__/person.cpython-39.pyc` & `dtmodel-0.1.2/dtmodel/enums/__pycache__/person.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.1/dtmodel/enums/facility.py` & `dtmodel-0.1.2/dtmodel/enums/facility.py`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.1/dtmodel/functions.py` & `dtmodel-0.1.2/dtmodel/functions.py`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.1/dtmodel/models/__pycache__/facility.cpython-39.pyc` & `dtmodel-0.1.2/dtmodel/models/__pycache__/facility.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.1/dtmodel/models/__pycache__/medical.cpython-39.pyc` & `dtmodel-0.1.2/dtmodel/models/__pycache__/medical.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.1/dtmodel/models/__pycache__/people.cpython-39.pyc` & `dtmodel-0.1.2/dtmodel/models/__pycache__/people.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.1/dtmodel/models/facility.py` & `dtmodel-0.1.2/dtmodel/models/facility.py`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.1/dtmodel/models/medical.py` & `dtmodel-0.1.2/dtmodel/models/medical.py`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.1/dtmodel/models/people.py` & `dtmodel-0.1.2/dtmodel/models/people.py`

 * *Files identical despite different names*

### Comparing `dtmodel-0.1.1/setup.py` & `dtmodel-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['dtmodel', 'dtmodel.bases', 'dtmodel.enums', 'dtmodel.models']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['bcrypt>=4.0.1,<5.0.0', 'dtfield>=0.2.0,<0.3.0']
+['bcrypt>=4.0.1,<5.0.0', 'dtfield>=0.2.1,<0.3.0']
 
 setup_kwargs = {
     'name': 'dtmodel',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': '',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

