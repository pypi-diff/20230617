# Comparing `tmp/AshCrypt-1.1.2.tar.gz` & `tmp/AshCrypt-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AshCrypt-1.1.2.tar", last modified: Sat Jun 17 15:02:07 2023, max compression
+gzip compressed data, was "AshCrypt-1.1.3.tar", last modified: Sat Jun 17 15:36:16 2023, max compression
```

## Comparing `AshCrypt-1.1.2.tar` & `AshCrypt-1.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 15:02:07.183426 AshCrypt-1.1.2/
-drwxrwxrwx   0        0        0        0 2023-06-17 15:02:07.145801 AshCrypt-1.1.2/AshCrypt/
--rw-rw-rw-   0        0        0     5157 2023-06-16 19:49:28.000000 AshCrypt-1.1.2/AshCrypt/Ash.py
--rw-rw-rw-   0        0        0     4378 2023-06-16 19:49:28.000000 AshCrypt-1.1.2/AshCrypt/AshCryptGUI.py
--rw-rw-rw-   0        0        0     7922 2023-06-16 19:49:28.000000 AshCrypt-1.1.2/AshCrypt/AshDatabase.py
--rw-rw-rw-   0        0        0     2987 2023-06-17 14:40:01.000000 AshCrypt-1.1.2/AshCrypt/AshFileCrypt.py
--rw-rw-rw-   0        0        0     2060 2023-06-16 19:49:28.000000 AshCrypt-1.1.2/AshCrypt/AshTextCrypt.py
--rw-rw-rw-   0        0        0     5972 2023-06-17 14:40:15.000000 AshCrypt-1.1.2/AshCrypt/CliCrypt.py
--rw-rw-rw-   0        0        0    14403 2023-06-17 13:08:51.000000 AshCrypt-1.1.2/AshCrypt/README.md
--rw-rw-rw-   0        0        0       91 2023-06-17 14:34:20.000000 AshCrypt-1.1.2/AshCrypt/__init__.py
--rw-rw-rw-   0        0        0     1045 2023-06-16 19:49:28.000000 AshCrypt-1.1.2/AshCrypt/qr.py
-drwxrwxrwx   0        0        0        0 2023-06-17 15:02:07.163098 AshCrypt-1.1.2/AshCrypt.egg-info/
--rw-rw-rw-   0        0        0    15322 2023-06-17 15:02:06.000000 AshCrypt-1.1.2/AshCrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      422 2023-06-17 15:02:06.000000 AshCrypt-1.1.2/AshCrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 15:02:06.000000 AshCrypt-1.1.2/AshCrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-06-17 15:02:06.000000 AshCrypt-1.1.2/AshCrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-17 15:02:06.000000 AshCrypt-1.1.2/AshCrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-05-28 20:09:20.000000 AshCrypt-1.1.2/LICENSE
--rw-rw-rw-   0        0        0    15322 2023-06-17 15:02:07.182422 AshCrypt-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    17338 2023-06-17 14:27:43.000000 AshCrypt-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-17 15:02:07.183426 AshCrypt-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1548 2023-06-17 14:56:35.000000 AshCrypt-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 15:02:07.177427 AshCrypt-1.1.2/unittests/
--rw-rw-rw-   0        0        0       25 2023-06-16 19:49:28.000000 AshCrypt-1.1.2/unittests/__init__.py
--rw-rw-rw-   0        0        0     3397 2023-06-16 19:49:28.000000 AshCrypt-1.1.2/unittests/unittestAsh.py
+drwxrwxrwx   0        0        0        0 2023-06-17 15:36:16.907180 AshCrypt-1.1.3/
+drwxrwxrwx   0        0        0        0 2023-06-17 15:36:16.844533 AshCrypt-1.1.3/AshCrypt/
+-rw-rw-rw-   0        0        0     5157 2023-06-17 15:23:25.000000 AshCrypt-1.1.3/AshCrypt/Ash.py
+-rw-rw-rw-   0        0        0     4387 2023-06-17 15:35:28.000000 AshCrypt-1.1.3/AshCrypt/AshCryptGUI.py
+-rw-rw-rw-   0        0        0     7922 2023-06-17 15:23:25.000000 AshCrypt-1.1.3/AshCrypt/AshDatabase.py
+-rw-rw-rw-   0        0        0     3001 2023-06-17 15:32:26.000000 AshCrypt-1.1.3/AshCrypt/AshFileCrypt.py
+-rw-rw-rw-   0        0        0     2074 2023-06-17 15:32:26.000000 AshCrypt-1.1.3/AshCrypt/AshTextCrypt.py
+-rw-rw-rw-   0        0        0     6000 2023-06-17 15:32:26.000000 AshCrypt-1.1.3/AshCrypt/CliCrypt.py
+-rw-rw-rw-   0        0        0    14403 2023-06-17 15:23:25.000000 AshCrypt-1.1.3/AshCrypt/README.md
+-rw-rw-rw-   0        0        0       91 2023-06-17 15:23:25.000000 AshCrypt-1.1.3/AshCrypt/__init__.py
+-rw-rw-rw-   0        0        0     1045 2023-06-17 15:23:25.000000 AshCrypt-1.1.3/AshCrypt/qr.py
+drwxrwxrwx   0        0        0        0 2023-06-17 15:36:16.866887 AshCrypt-1.1.3/AshCrypt.egg-info/
+-rw-rw-rw-   0        0        0    15322 2023-06-17 15:36:16.000000 AshCrypt-1.1.3/AshCrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-06-17 15:36:16.000000 AshCrypt-1.1.3/AshCrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 15:36:16.000000 AshCrypt-1.1.3/AshCrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-06-17 15:36:16.000000 AshCrypt-1.1.3/AshCrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-17 15:36:16.000000 AshCrypt-1.1.3/AshCrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-06-17 15:23:25.000000 AshCrypt-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0    15322 2023-06-17 15:36:16.905178 AshCrypt-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    17338 2023-06-17 15:23:25.000000 AshCrypt-1.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-17 15:36:16.908176 AshCrypt-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1544 2023-06-17 15:24:14.000000 AshCrypt-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 15:36:16.874327 AshCrypt-1.1.3/unittests/
+-rw-rw-rw-   0        0        0       25 2023-06-17 15:23:25.000000 AshCrypt-1.1.3/unittests/__init__.py
+-rw-rw-rw-   0        0        0     3397 2023-06-17 15:23:25.000000 AshCrypt-1.1.3/unittests/unittestAsh.py
```

### Comparing `AshCrypt-1.1.2/AshCrypt/Ash.py` & `AshCrypt-1.1.3/AshCrypt/Ash.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.2/AshCrypt/AshCryptGUI.py` & `AshCrypt-1.1.3/AshCrypt/AshCryptGUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import ttkbootstrap as tk
-from AshTextCrypt import *
+from AshCrypt.AshTextCrypt import *
 import qr
 
 key = 'c3066e464350e68a144d6be3e35c879eac1b9f360139443ee3d9e1960725d6a4d3379af0a35b6a07d083ecc29c4ba03767ad6d48b8e9c20d319dd459da52a91a'
 
 def encryption():
     m = inputfield1_1.get()
     if len(m) > 200 :
```

### Comparing `AshCrypt-1.1.2/AshCrypt/AshDatabase.py` & `AshCrypt-1.1.3/AshCrypt/AshDatabase.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.2/AshCrypt/AshFileCrypt.py` & `AshCrypt-1.1.3/AshCrypt/AshFileCrypt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import Ash
+from AshCrypt import Ash
 import os
 
 class KeyError(Exception):
     def __init__(self):
         self.display = 'Key must be 512 Bit long !'
         super().__init__(self.display)
```

### Comparing `AshCrypt-1.1.2/AshCrypt/AshTextCrypt.py` & `AshCrypt-1.1.3/AshCrypt/AshTextCrypt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Union
-import Ash
+from AshCrypt import Ash
 
 
 class KeyError(Exception):
     def __init__(self):
         self.display = 'Key must be 512 Bit long !'
         super().__init__(self.display)
```

### Comparing `AshCrypt-1.1.2/AshCrypt/CliCrypt.py` & `AshCrypt-1.1.3/AshCrypt/CliCrypt.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import AshFileCrypt as AF
-import AshTextCrypt as A
+from AshCrypt import AshFileCrypt as AF
+from AshCrypt import AshTextCrypt as A
 import sys
 
 
 print('Welcome to the CLI')
 
 commands = 'Commands : \n\tq: to quit the program \n\tc : view commands\n\te: for encryption\n\td : for decryption\n' \
            '\tef : to encrypt a file\n\tdf : to decrypt a file\n'
```

### Comparing `AshCrypt-1.1.2/AshCrypt/README.md` & `AshCrypt-1.1.3/AshCrypt/README.md`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.2/AshCrypt/qr.py` & `AshCrypt-1.1.3/AshCrypt/qr.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.2/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-1.1.3/AshCrypt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.1.2
+Version: 1.1.3
 Summary: Comprehensive AES-256 Cryptography library equipped with a file handling module along with a text module w/ a user-friendly GUI and a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography,AES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `AshCrypt-1.1.2/LICENSE` & `AshCrypt-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.2/PKG-INFO` & `AshCrypt-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.1.2
+Version: 1.1.3
 Summary: Comprehensive AES-256 Cryptography library equipped with a file handling module along with a text module w/ a user-friendly GUI and a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography,AES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `AshCrypt-1.1.2/README.md` & `AshCrypt-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.1.2/setup.py` & `AshCrypt-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('AshCrypt/README.md','r') as f :
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='1.1.2',
+    version='1.1.3',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography library equipped with a file handling module along with"
                 " a text module w/ a user-friendly GUI and a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
@@ -40,9 +40,8 @@
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     keywords=[
         'Cryptography',
         'AES-256',
     ],
-
-)
+)
```

### Comparing `AshCrypt-1.1.2/unittests/unittestAsh.py` & `AshCrypt-1.1.3/unittests/unittestAsh.py`

 * *Files identical despite different names*

