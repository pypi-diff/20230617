# Comparing `tmp/Rest-OC-1.2.3.tar.gz` & `tmp/Rest-OC-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Rest-OC-1.2.3.tar", last modified: Fri Jun  2 10:58:52 2023, max compression
+gzip compressed data, was "Rest-OC-1.2.4.tar", last modified: Sat Jun 17 19:16:53 2023, max compression
```

## Comparing `Rest-OC-1.2.3.tar` & `Rest-OC-1.2.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-06-02 10:58:52.183926 Rest-OC-1.2.3/
--rw-rw-r--   0 bast      (1002) bast      (1002)     1073 2023-03-03 20:50:56.000000 Rest-OC-1.2.3/LICENSE
--rw-rw-r--   0 bast      (1002) bast      (1002)      856 2023-06-02 10:58:52.183926 Rest-OC-1.2.3/PKG-INFO
--rw-rw-r--   0 bast      (1002) bast      (1002)      217 2023-03-20 17:38:57.000000 Rest-OC-1.2.3/README.md
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-06-02 10:58:52.179926 Rest-OC-1.2.3/RestOC/
--rw-rw-r--   0 bast      (1002) bast      (1002)     2524 2023-01-10 16:46:53.000000 Rest-OC-1.2.3/RestOC/CLI.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     3857 2023-01-10 16:46:53.000000 Rest-OC-1.2.3/RestOC/Conf.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     5041 2023-01-10 16:46:53.000000 Rest-OC-1.2.3/RestOC/DateTimeHelper.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     5631 2023-01-27 13:06:17.000000 Rest-OC-1.2.3/RestOC/DictHelper.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     3326 2023-03-03 20:50:56.000000 Rest-OC-1.2.3/RestOC/EMail.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     1037 2023-01-10 16:46:53.000000 Rest-OC-1.2.3/RestOC/Environment.py
--rw-rw-r--   0 bast      (1002) bast      (1002)      381 2023-03-20 18:18:38.000000 Rest-OC-1.2.3/RestOC/Errors.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     5526 2023-03-20 17:38:57.000000 Rest-OC-1.2.3/RestOC/Image.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     2946 2023-01-10 16:46:53.000000 Rest-OC-1.2.3/RestOC/JSON.py
--rw-rw-r--   0 bast      (1002) bast      (1002)    15049 2023-05-26 11:06:24.000000 Rest-OC-1.2.3/RestOC/REST.py
--rw-rw-r--   0 bast      (1002) bast      (1002)    23650 2023-02-13 23:13:11.000000 Rest-OC-1.2.3/RestOC/Record_Base.py
--rw-rw-r--   0 bast      (1002) bast      (1002)    66432 2023-03-11 14:44:28.000000 Rest-OC-1.2.3/RestOC/Record_MySQL.py
--rw-rw-r--   0 bast      (1002) bast      (1002)    47196 2023-01-27 13:06:17.000000 Rest-OC-1.2.3/RestOC/Record_ReDB.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     2738 2023-01-10 16:46:53.000000 Rest-OC-1.2.3/RestOC/Resize.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     7092 2023-01-10 16:46:53.000000 Rest-OC-1.2.3/RestOC/SMTP.py
--rw-rw-r--   0 bast      (1002) bast      (1002)    19557 2023-03-26 13:12:06.000000 Rest-OC-1.2.3/RestOC/Services.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     4502 2023-01-10 16:46:53.000000 Rest-OC-1.2.3/RestOC/Session.py
--rw-rw-r--   0 bast      (1002) bast      (1002)    18147 2023-01-10 16:46:53.000000 Rest-OC-1.2.3/RestOC/StrHelper.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     1653 2023-01-10 16:46:53.000000 Rest-OC-1.2.3/RestOC/Templates.py
--rw-r--r--   0 bast      (1002) bast      (1002)        0 2021-06-08 11:58:01.000000 Rest-OC-1.2.3/RestOC/__init__.py
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-06-02 10:58:52.183926 Rest-OC-1.2.3/Rest_OC.egg-info/
--rw-rw-r--   0 bast      (1002) bast      (1002)      856 2023-06-02 10:58:52.000000 Rest-OC-1.2.3/Rest_OC.egg-info/PKG-INFO
--rw-rw-r--   0 bast      (1002) bast      (1002)      587 2023-06-02 10:58:52.000000 Rest-OC-1.2.3/Rest_OC.egg-info/SOURCES.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)        1 2023-06-02 10:58:52.000000 Rest-OC-1.2.3/Rest_OC.egg-info/dependency_links.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)      267 2023-06-02 10:58:52.000000 Rest-OC-1.2.3/Rest_OC.egg-info/requires.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)        7 2023-06-02 10:58:52.000000 Rest-OC-1.2.3/Rest_OC.egg-info/top_level.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)        1 2022-06-23 11:30:41.000000 Rest-OC-1.2.3/Rest_OC.egg-info/zip-safe
--rw-r--r--   0 bast      (1002) bast      (1002)       79 2023-06-02 10:58:52.183926 Rest-OC-1.2.3/setup.cfg
--rw-rw-r--   0 bast      (1002) bast      (1002)     1142 2023-06-02 10:58:42.000000 Rest-OC-1.2.3/setup.py
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2023-06-17 19:16:53.009205 Rest-OC-1.2.4/
+-rw-rw-r--   0 bast      (1000) bast      (1000)     1073 2023-03-03 20:50:56.000000 Rest-OC-1.2.4/LICENSE
+-rw-rw-r--   0 bast      (1000) bast      (1000)      856 2023-06-17 19:16:53.009205 Rest-OC-1.2.4/PKG-INFO
+-rw-rw-r--   0 bast      (1000) bast      (1000)      217 2023-03-20 17:38:57.000000 Rest-OC-1.2.4/README.md
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2023-06-17 19:16:53.009205 Rest-OC-1.2.4/RestOC/
+-rw-rw-r--   0 bast      (1000) bast      (1000)     2524 2023-01-10 16:46:53.000000 Rest-OC-1.2.4/RestOC/CLI.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     3857 2023-01-10 16:46:53.000000 Rest-OC-1.2.4/RestOC/Conf.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     5041 2023-01-10 16:46:53.000000 Rest-OC-1.2.4/RestOC/DateTimeHelper.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     5631 2023-01-27 13:06:17.000000 Rest-OC-1.2.4/RestOC/DictHelper.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     3326 2023-03-03 20:50:56.000000 Rest-OC-1.2.4/RestOC/EMail.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     1037 2023-01-10 16:46:53.000000 Rest-OC-1.2.4/RestOC/Environment.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)      381 2023-03-20 18:18:38.000000 Rest-OC-1.2.4/RestOC/Errors.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     5526 2023-03-20 17:38:57.000000 Rest-OC-1.2.4/RestOC/Image.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     2946 2023-01-10 16:46:53.000000 Rest-OC-1.2.4/RestOC/JSON.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)    15049 2023-05-26 11:06:24.000000 Rest-OC-1.2.4/RestOC/REST.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)    23672 2023-06-17 19:14:01.000000 Rest-OC-1.2.4/RestOC/Record_Base.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)    66432 2023-03-11 14:44:28.000000 Rest-OC-1.2.4/RestOC/Record_MySQL.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)    47196 2023-01-27 13:06:17.000000 Rest-OC-1.2.4/RestOC/Record_ReDB.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     2738 2023-01-10 16:46:53.000000 Rest-OC-1.2.4/RestOC/Resize.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     7092 2023-01-10 16:46:53.000000 Rest-OC-1.2.4/RestOC/SMTP.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)    19557 2023-03-26 13:12:06.000000 Rest-OC-1.2.4/RestOC/Services.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     4502 2023-01-10 16:46:53.000000 Rest-OC-1.2.4/RestOC/Session.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)    18147 2023-01-10 16:46:53.000000 Rest-OC-1.2.4/RestOC/StrHelper.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     1653 2023-01-10 16:46:53.000000 Rest-OC-1.2.4/RestOC/Templates.py
+-rw-r--r--   0 bast      (1000) bast      (1000)        0 2021-06-08 11:58:01.000000 Rest-OC-1.2.4/RestOC/__init__.py
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2023-06-17 19:16:53.009205 Rest-OC-1.2.4/Rest_OC.egg-info/
+-rw-rw-r--   0 bast      (1000) bast      (1000)      856 2023-06-17 19:16:53.000000 Rest-OC-1.2.4/Rest_OC.egg-info/PKG-INFO
+-rw-rw-r--   0 bast      (1000) bast      (1000)      587 2023-06-17 19:16:53.000000 Rest-OC-1.2.4/Rest_OC.egg-info/SOURCES.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)        1 2023-06-17 19:16:53.000000 Rest-OC-1.2.4/Rest_OC.egg-info/dependency_links.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)      267 2023-06-17 19:16:53.000000 Rest-OC-1.2.4/Rest_OC.egg-info/requires.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)        7 2023-06-17 19:16:53.000000 Rest-OC-1.2.4/Rest_OC.egg-info/top_level.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)        1 2022-06-23 11:30:41.000000 Rest-OC-1.2.4/Rest_OC.egg-info/zip-safe
+-rw-r--r--   0 bast      (1000) bast      (1000)       79 2023-06-17 19:16:53.009205 Rest-OC-1.2.4/setup.cfg
+-rw-rw-r--   0 bast      (1000) bast      (1000)     1142 2023-06-17 19:14:01.000000 Rest-OC-1.2.4/setup.py
```

### Comparing `Rest-OC-1.2.3/LICENSE` & `Rest-OC-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.3/PKG-INFO` & `Rest-OC-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Rest-OC
-Version: 1.2.3
+Version: 1.2.4
 Summary: Rest-OC is a library of python 3 modules for rapidly setting up REST microservices.
 Home-page: https://ouroboroscoding.com/rest-oc/
 Author: Chris Nasr - Ouroboros Coding Inc.
 Author-email: chris@ouroboroscoding.com
 License: MIT
 Project-URL: Documentation, https://ouroboroscoding.com/rest-oc/
 Project-URL: Source, https://github.com/ouroboroscoding/rest-oc-python
```

### Comparing `Rest-OC-1.2.3/RestOC/CLI.py` & `Rest-OC-1.2.4/RestOC/CLI.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.3/RestOC/Conf.py` & `Rest-OC-1.2.4/RestOC/Conf.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.3/RestOC/DateTimeHelper.py` & `Rest-OC-1.2.4/RestOC/DateTimeHelper.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.3/RestOC/DictHelper.py` & `Rest-OC-1.2.4/RestOC/DictHelper.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.3/RestOC/EMail.py` & `Rest-OC-1.2.4/RestOC/EMail.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.3/RestOC/Environment.py` & `Rest-OC-1.2.4/RestOC/Environment.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.3/RestOC/Image.py` & `Rest-OC-1.2.4/RestOC/Image.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.3/RestOC/JSON.py` & `Rest-OC-1.2.4/RestOC/JSON.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.3/RestOC/REST.py` & `Rest-OC-1.2.4/RestOC/REST.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.3/RestOC/Record_Base.py` & `Rest-OC-1.2.4/RestOC/Record_Base.py`

 * *Files 0% similar despite different names*

```diff
@@ -816,15 +816,15 @@
 
 		# If no specific fields requested
 		if not fields:
 			dRet = DictHelper.clone(self._dRecord)
 
 		# Else, get each requested field and return
 		else:
-			dRet = {f:self._dRecord[f] for f in fields}
+			dRet = {f:self._dRecord[f] for f in fields if f in self._dRecord}
 
 		# Clone the results and return
 		return DictHelper.clone(dRet)
 
 	@abc.abstractclassmethod
 	def remove(cls, _id, array, index, custom={}):
 		"""Remove
```

### Comparing `Rest-OC-1.2.3/RestOC/Record_MySQL.py` & `Rest-OC-1.2.4/RestOC/Record_MySQL.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.3/RestOC/Record_ReDB.py` & `Rest-OC-1.2.4/RestOC/Record_ReDB.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.3/RestOC/Resize.py` & `Rest-OC-1.2.4/RestOC/Resize.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.3/RestOC/SMTP.py` & `Rest-OC-1.2.4/RestOC/SMTP.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.3/RestOC/Services.py` & `Rest-OC-1.2.4/RestOC/Services.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.3/RestOC/Session.py` & `Rest-OC-1.2.4/RestOC/Session.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.3/RestOC/StrHelper.py` & `Rest-OC-1.2.4/RestOC/StrHelper.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.3/RestOC/Templates.py` & `Rest-OC-1.2.4/RestOC/Templates.py`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.3/Rest_OC.egg-info/PKG-INFO` & `Rest-OC-1.2.4/Rest_OC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Rest-OC
-Version: 1.2.3
+Version: 1.2.4
 Summary: Rest-OC is a library of python 3 modules for rapidly setting up REST microservices.
 Home-page: https://ouroboroscoding.com/rest-oc/
 Author: Chris Nasr - Ouroboros Coding Inc.
 Author-email: chris@ouroboroscoding.com
 License: MIT
 Project-URL: Documentation, https://ouroboroscoding.com/rest-oc/
 Project-URL: Source, https://github.com/ouroboroscoding/rest-oc-python
```

### Comparing `Rest-OC-1.2.3/Rest_OC.egg-info/SOURCES.txt` & `Rest-OC-1.2.4/Rest_OC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Rest-OC-1.2.3/setup.py` & `Rest-OC-1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as oF:
 	long_description=oF.read()
 
 setup(
 	name='Rest-OC',
-	version='1.2.3',
+	version='1.2.4',
 	description='Rest-OC is a library of python 3 modules for rapidly setting up REST microservices.',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	url='https://ouroboroscoding.com/rest-oc/',
 	project_urls={
 		'Documentation': 'https://ouroboroscoding.com/rest-oc/',
 		'Source': 'https://github.com/ouroboroscoding/rest-oc-python',
```

