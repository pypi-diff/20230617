# Comparing `tmp/AshCrypt-1.1.1.tar.gz` & `tmp/AshCrypt-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AshCrypt-1.1.1.tar", last modified: Sat Jun 17 14:17:55 2023, max compression
+gzip compressed data, was "AshCrypt-1.1.2.tar", last modified: Sat Jun 17 15:02:07 2023, max compression
```

## Comparing `AshCrypt-1.1.1.tar` & `AshCrypt-1.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 14:17:55.479616 AshCrypt-1.1.1/
-drwxrwxrwx   0        0        0        0 2023-06-17 14:17:55.449792 AshCrypt-1.1.1/AshCrypt/
--rw-rw-rw-   0        0        0     5157 2023-06-16 19:49:28.000000 AshCrypt-1.1.1/AshCrypt/Ash.py
--rw-rw-rw-   0        0        0     4378 2023-06-16 19:49:28.000000 AshCrypt-1.1.1/AshCrypt/AshCryptGUI.py
--rw-rw-rw-   0        0        0     7922 2023-06-16 19:49:28.000000 AshCrypt-1.1.1/AshCrypt/AshDatabase.py
--rw-rw-rw-   0        0        0     2987 2023-06-16 19:49:28.000000 AshCrypt-1.1.1/AshCrypt/AshFileCrypt.py
--rw-rw-rw-   0        0        0     2060 2023-06-16 19:49:28.000000 AshCrypt-1.1.1/AshCrypt/AshTextCrypt.py
--rw-rw-rw-   0        0        0     5972 2023-06-17 13:08:51.000000 AshCrypt-1.1.1/AshCrypt/CliCrypt.py
--rw-rw-rw-   0        0        0    14403 2023-06-17 13:08:51.000000 AshCrypt-1.1.1/AshCrypt/README.md
--rw-rw-rw-   0        0        0       98 2023-06-16 19:49:28.000000 AshCrypt-1.1.1/AshCrypt/__init__.py
--rw-rw-rw-   0        0        0     1045 2023-06-16 19:49:28.000000 AshCrypt-1.1.1/AshCrypt/qr.py
-drwxrwxrwx   0        0        0        0 2023-06-17 14:17:55.465719 AshCrypt-1.1.1/AshCrypt.egg-info/
--rw-rw-rw-   0        0        0    15322 2023-06-17 14:17:54.000000 AshCrypt-1.1.1/AshCrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      422 2023-06-17 14:17:54.000000 AshCrypt-1.1.1/AshCrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 14:17:54.000000 AshCrypt-1.1.1/AshCrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-06-17 14:17:54.000000 AshCrypt-1.1.1/AshCrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-17 14:17:54.000000 AshCrypt-1.1.1/AshCrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-05-28 20:09:20.000000 AshCrypt-1.1.1/LICENSE
--rw-rw-rw-   0        0        0    15322 2023-06-17 14:17:55.477699 AshCrypt-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    17198 2023-06-17 13:32:00.000000 AshCrypt-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-17 14:17:55.480659 AshCrypt-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1548 2023-06-17 14:17:42.000000 AshCrypt-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 14:17:55.473099 AshCrypt-1.1.1/unittests/
--rw-rw-rw-   0        0        0       25 2023-06-16 19:49:28.000000 AshCrypt-1.1.1/unittests/__init__.py
--rw-rw-rw-   0        0        0     3397 2023-06-16 19:49:28.000000 AshCrypt-1.1.1/unittests/unittestAsh.py
+drwxrwxrwx   0        0        0        0 2023-06-17 15:02:07.183426 AshCrypt-1.1.2/
+drwxrwxrwx   0        0        0        0 2023-06-17 15:02:07.145801 AshCrypt-1.1.2/AshCrypt/
+-rw-rw-rw-   0        0        0     5157 2023-06-16 19:49:28.000000 AshCrypt-1.1.2/AshCrypt/Ash.py
+-rw-rw-rw-   0        0        0     4378 2023-06-16 19:49:28.000000 AshCrypt-1.1.2/AshCrypt/AshCryptGUI.py
+-rw-rw-rw-   0        0        0     7922 2023-06-16 19:49:28.000000 AshCrypt-1.1.2/AshCrypt/AshDatabase.py
+-rw-rw-rw-   0        0        0     2987 2023-06-17 14:40:01.000000 AshCrypt-1.1.2/AshCrypt/AshFileCrypt.py
+-rw-rw-rw-   0        0        0     2060 2023-06-16 19:49:28.000000 AshCrypt-1.1.2/AshCrypt/AshTextCrypt.py
+-rw-rw-rw-   0        0        0     5972 2023-06-17 14:40:15.000000 AshCrypt-1.1.2/AshCrypt/CliCrypt.py
+-rw-rw-rw-   0        0        0    14403 2023-06-17 13:08:51.000000 AshCrypt-1.1.2/AshCrypt/README.md
+-rw-rw-rw-   0        0        0       91 2023-06-17 14:34:20.000000 AshCrypt-1.1.2/AshCrypt/__init__.py
+-rw-rw-rw-   0        0        0     1045 2023-06-16 19:49:28.000000 AshCrypt-1.1.2/AshCrypt/qr.py
+drwxrwxrwx   0        0        0        0 2023-06-17 15:02:07.163098 AshCrypt-1.1.2/AshCrypt.egg-info/
+-rw-rw-rw-   0        0        0    15322 2023-06-17 15:02:06.000000 AshCrypt-1.1.2/AshCrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-06-17 15:02:06.000000 AshCrypt-1.1.2/AshCrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 15:02:06.000000 AshCrypt-1.1.2/AshCrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-06-17 15:02:06.000000 AshCrypt-1.1.2/AshCrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-17 15:02:06.000000 AshCrypt-1.1.2/AshCrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-05-28 20:09:20.000000 AshCrypt-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0    15322 2023-06-17 15:02:07.182422 AshCrypt-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    17338 2023-06-17 14:27:43.000000 AshCrypt-1.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-17 15:02:07.183426 AshCrypt-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1548 2023-06-17 14:56:35.000000 AshCrypt-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 15:02:07.177427 AshCrypt-1.1.2/unittests/
+-rw-rw-rw-   0        0        0       25 2023-06-16 19:49:28.000000 AshCrypt-1.1.2/unittests/__init__.py
+-rw-rw-rw-   0        0        0     3397 2023-06-16 19:49:28.000000 AshCrypt-1.1.2/unittests/unittestAsh.py
```

### Comparing `AshCrypt-1.1.1/AshCrypt/Ash.py` & `AshCrypt-1.1.2/AshCrypt/Ash.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.1/AshCrypt/AshCryptGUI.py` & `AshCrypt-1.1.2/AshCrypt/AshCryptGUI.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.1/AshCrypt/AshDatabase.py` & `AshCrypt-1.1.2/AshCrypt/AshDatabase.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.1/AshCrypt/AshFileCrypt.py` & `AshCrypt-1.1.2/AshCrypt/AshFileCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.1/AshCrypt/AshTextCrypt.py` & `AshCrypt-1.1.2/AshCrypt/AshTextCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.1/AshCrypt/CliCrypt.py` & `AshCrypt-1.1.2/AshCrypt/CliCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.1/AshCrypt/README.md` & `AshCrypt-1.1.2/AshCrypt/README.md`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.1/AshCrypt/qr.py` & `AshCrypt-1.1.2/AshCrypt/qr.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.1/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-1.1.2/AshCrypt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.1.1
+Version: 1.1.2
 Summary: Comprehensive AES-256 Cryptography library equipped with a file handling module along with a text module w/ a user-friendly GUI and a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography,AES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `AshCrypt-1.1.1/LICENSE` & `AshCrypt-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.1/PKG-INFO` & `AshCrypt-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.1.1
+Version: 1.1.2
 Summary: Comprehensive AES-256 Cryptography library equipped with a file handling module along with a text module w/ a user-friendly GUI and a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography,AES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `AshCrypt-1.1.1/README.md` & `AshCrypt-1.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,19 @@
 pip install --upgrade pip 
 ```
 Then install the Library 
 ```bash
 pip install AshCrypt
 ```
 This will install the latest version of `AshCrypt`.
+You can start using it in your code by importing its modules : 
+```python
+from AshCrypt.
+from AshCrypt.Ash import Enc.genMainkey()
+```
 <br>That's it.
 <br>Now if you want to get the whole repo without manual configurations
 <br>Run this command in the Terminal
 ```bash
 curl -sSfL https://raw.githubusercontent.com/AshGw/AES-256/main/important/setup.sh | bash
 ```
 This will run the commands in [setup.sh](important/setup.sh).
```

### Comparing `AshCrypt-1.1.1/setup.py` & `AshCrypt-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('AshCrypt/README.md','r') as f :
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='1.1.1',
+    version='1.1.2',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography library equipped with a file handling module along with"
                 " a text module w/ a user-friendly GUI and a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

### Comparing `AshCrypt-1.1.1/unittests/unittestAsh.py` & `AshCrypt-1.1.2/unittests/unittestAsh.py`

 * *Files identical despite different names*

