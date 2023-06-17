# Comparing `tmp/AshCrypt-1.0.1.tar.gz` & `tmp/AshCrypt-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AshCrypt-1.0.1.tar", last modified: Sat Jun 17 13:01:27 2023, max compression
+gzip compressed data, was "AshCrypt-1.1.1.tar", last modified: Sat Jun 17 14:17:55 2023, max compression
```

## Comparing `AshCrypt-1.0.1.tar` & `AshCrypt-1.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 13:01:27.253232 AshCrypt-1.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-17 13:01:27.183137 AshCrypt-1.0.1/AshCrypt.egg-info/
--rw-rw-rw-   0        0        0    15322 2023-06-17 13:01:26.000000 AshCrypt-1.0.1/AshCrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-06-17 13:01:26.000000 AshCrypt-1.0.1/AshCrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 13:01:26.000000 AshCrypt-1.0.1/AshCrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-06-17 13:01:26.000000 AshCrypt-1.0.1/AshCrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-17 13:01:26.000000 AshCrypt-1.0.1/AshCrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-05-28 20:09:20.000000 AshCrypt-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    15322 2023-06-17 13:01:27.251216 AshCrypt-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    16621 2023-06-17 03:46:03.000000 AshCrypt-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-17 13:01:27.253232 AshCrypt-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1555 2023-06-17 13:00:41.000000 AshCrypt-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 13:01:27.232287 AshCrypt-1.0.1/src/
--rw-rw-rw-   0        0        0     5157 2023-06-16 19:49:28.000000 AshCrypt-1.0.1/src/Ash.py
--rw-rw-rw-   0        0        0     4378 2023-06-16 19:49:28.000000 AshCrypt-1.0.1/src/AshCryptGUI.py
--rw-rw-rw-   0        0        0     7922 2023-06-16 19:49:28.000000 AshCrypt-1.0.1/src/AshDatabase.py
--rw-rw-rw-   0        0        0     2987 2023-06-16 19:49:28.000000 AshCrypt-1.0.1/src/AshFileCrypt.py
--rw-rw-rw-   0        0        0     2060 2023-06-16 19:49:28.000000 AshCrypt-1.0.1/src/AshTextCrypt.py
--rw-rw-rw-   0        0        0     5972 2023-06-17 12:59:06.000000 AshCrypt-1.0.1/src/CliCrypt.py
--rw-rw-rw-   0        0        0    14403 2023-06-17 12:58:00.000000 AshCrypt-1.0.1/src/README.md
--rw-rw-rw-   0        0        0       98 2023-06-16 19:49:28.000000 AshCrypt-1.0.1/src/__init__.py
--rw-rw-rw-   0        0        0     1045 2023-06-16 19:49:28.000000 AshCrypt-1.0.1/src/qr.py
-drwxrwxrwx   0        0        0        0 2023-06-17 13:01:27.245172 AshCrypt-1.0.1/unittests/
--rw-rw-rw-   0        0        0       25 2023-06-16 19:49:28.000000 AshCrypt-1.0.1/unittests/__init__.py
--rw-rw-rw-   0        0        0     3397 2023-06-16 19:49:28.000000 AshCrypt-1.0.1/unittests/unittestAsh.py
+drwxrwxrwx   0        0        0        0 2023-06-17 14:17:55.479616 AshCrypt-1.1.1/
+drwxrwxrwx   0        0        0        0 2023-06-17 14:17:55.449792 AshCrypt-1.1.1/AshCrypt/
+-rw-rw-rw-   0        0        0     5157 2023-06-16 19:49:28.000000 AshCrypt-1.1.1/AshCrypt/Ash.py
+-rw-rw-rw-   0        0        0     4378 2023-06-16 19:49:28.000000 AshCrypt-1.1.1/AshCrypt/AshCryptGUI.py
+-rw-rw-rw-   0        0        0     7922 2023-06-16 19:49:28.000000 AshCrypt-1.1.1/AshCrypt/AshDatabase.py
+-rw-rw-rw-   0        0        0     2987 2023-06-16 19:49:28.000000 AshCrypt-1.1.1/AshCrypt/AshFileCrypt.py
+-rw-rw-rw-   0        0        0     2060 2023-06-16 19:49:28.000000 AshCrypt-1.1.1/AshCrypt/AshTextCrypt.py
+-rw-rw-rw-   0        0        0     5972 2023-06-17 13:08:51.000000 AshCrypt-1.1.1/AshCrypt/CliCrypt.py
+-rw-rw-rw-   0        0        0    14403 2023-06-17 13:08:51.000000 AshCrypt-1.1.1/AshCrypt/README.md
+-rw-rw-rw-   0        0        0       98 2023-06-16 19:49:28.000000 AshCrypt-1.1.1/AshCrypt/__init__.py
+-rw-rw-rw-   0        0        0     1045 2023-06-16 19:49:28.000000 AshCrypt-1.1.1/AshCrypt/qr.py
+drwxrwxrwx   0        0        0        0 2023-06-17 14:17:55.465719 AshCrypt-1.1.1/AshCrypt.egg-info/
+-rw-rw-rw-   0        0        0    15322 2023-06-17 14:17:54.000000 AshCrypt-1.1.1/AshCrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-06-17 14:17:54.000000 AshCrypt-1.1.1/AshCrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 14:17:54.000000 AshCrypt-1.1.1/AshCrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-06-17 14:17:54.000000 AshCrypt-1.1.1/AshCrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-17 14:17:54.000000 AshCrypt-1.1.1/AshCrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-05-28 20:09:20.000000 AshCrypt-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0    15322 2023-06-17 14:17:55.477699 AshCrypt-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    17198 2023-06-17 13:32:00.000000 AshCrypt-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-17 14:17:55.480659 AshCrypt-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1548 2023-06-17 14:17:42.000000 AshCrypt-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 14:17:55.473099 AshCrypt-1.1.1/unittests/
+-rw-rw-rw-   0        0        0       25 2023-06-16 19:49:28.000000 AshCrypt-1.1.1/unittests/__init__.py
+-rw-rw-rw-   0        0        0     3397 2023-06-16 19:49:28.000000 AshCrypt-1.1.1/unittests/unittestAsh.py
```

### Comparing `AshCrypt-1.0.1/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-1.1.1/AshCrypt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.0.1
+Version: 1.1.1
 Summary: Comprehensive AES-256 Cryptography library equipped with a file handling module along with a text module w/ a user-friendly GUI and a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography,AES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `AshCrypt-1.0.1/LICENSE` & `AshCrypt-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.0.1/PKG-INFO` & `AshCrypt-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.0.1
+Version: 1.1.1
 Summary: Comprehensive AES-256 Cryptography library equipped with a file handling module along with a text module w/ a user-friendly GUI and a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography,AES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `AshCrypt-1.0.1/README.md` & `AshCrypt-1.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 As a firm believer in **Freedom** , I have developed a set of tools in Python that leverages the AES-256 algorithm to make it easier for undividuals to safeguard their data without blindly relying on third parties to do it tor them  . 
 
 My aim here is to make these tools accessible and user-friendly, even for individuals with limited programming knowledge. By providing these resources, I hope to contribute to the preservation of privacy and enable individuals to take control of their own data security, so feel free to explore these tools.
 ## Overview ## 
 The project incorporates a library I made called **[AshCrypt](https://github.com/AshGw/AES-256/tree/main/src)** : 
 
 <br>A simple, secure, and developer-oriented library for
-encryption and decryption with AES-256 (CBC) . It offers an intuitive
-interface, seamless integration with precompiled 
+encryption and decryption with AES-256 (CBC) . 
+<br>The core of the library is the module `Ash`
+It offers an intuitive interface, seamless integration with precompiled 
 functions, and robust security measures to safeguard
 sensitive data,  providing a hassle-free experience when dealing with cryptographic libraries.
 <br>View [Features](https://github.com/AshGw/AES-256#features) Header for more details.
 
 
 
 The project uses that same module to ensure secure data encryption and decryption for Files and Texts while keeping it very easy and simple to use .
@@ -24,40 +25,51 @@
 
 It also includes a simple graphical user interface (GUI) for easy interaction with the AshTextCrypt module.
 <br>If you're trying to either encrypt or decrypt some messages on the go ( 200 characters max ) you can use this GUI.
 <br>It also has a qr module associated with it to display the message.
 <br>check [GUI](https://github.com/AshGw/AES-256/src#ashcryptgui) header for more info.
 
 
+While The **GUI** is limited to 200 characters of text, if you want to be free over how much data or type of data you want to include, then u can use `CliCrypt.py` which is an innovative command line interface (CLI) designed to provide encryption and decryption capabilities for both text and file data with no constraints.
+
+
 It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
 safe and simple manner, you can use whichever you see fit.
 
 <br>The module has a simple straight forward apporach for dealing with sqlite3 databases, even if youre not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check [AshDatabase](https://github.com/AshGw/CryptographyAES-256#ashdatabase) header to learn more.
 
 ## Installation ##
 You can simply use **pip**
+<br>First upgrade the package installer 
+```bash
+pip install --upgrade pip 
 ```
+Then install the Library 
+```bash
 pip install AshCrypt
 ```
 This will install the latest version of `AshCrypt`.
-
-<br>If you want to get the whole repo without manual configurations
+<br>That's it.
+<br>Now if you want to get the whole repo without manual configurations
 <br>Run this command in the Terminal
 ```bash
 curl -sSfL https://raw.githubusercontent.com/AshGw/AES-256/main/important/setup.sh | bash
 ```
 This will run the commands in [setup.sh](important/setup.sh).
 <br>It will clone & install all the dependencies needed on your machine inside the directory you're currently at.
 <br>The `CliCrypt` will pop off automatically and you can start using it right away.
 
 <br>If you're testing how this works on a Debian based Docker container you can run this command to automatically set the environment before you run the command above
 ```bash
-curl -sSfL https://github.com/AshGw/AES-256/blob/main/docker-build/env-setup.sh
+curl -sSfL https://raw.githubusercontent.com/AshGw/AES-256/Apex/docker-build/env-setup.sh | bash
+```
+Then run 
+```bash
+source vvv/bin/activate
 ```
-
 
 <details>
 <summary>Got Errors ?</summary>
 
 <h5>For Debian based systems</h5>
 
 1) Install `curl` if you don't have it already
```

### Comparing `AshCrypt-1.0.1/setup.py` & `AshCrypt-1.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from setuptools import setup , find_packages
 
 
-with open('src/README.md','r') as f :
+with open('AshCrypt/README.md','r') as f :
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='1.0.1',
+    version='1.1.1',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography library equipped with a file handling module along with"
                 " a text module w/ a user-friendly GUI and a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
     url='https://github.com/AshGw/AES-256.git',
     packages=find_packages(exclude=['important', 'docker-build']),
     package_data={
-        '': ['LICENSE', 'README.md'],
-        'src': ['*'],
-        'unittest': ['*'],
+        'AshCrypt': ['*'],
+        'unittestsAC': ['*'],
     },
     exclude_package_data={
-        '': ['.gitignore'],
+        '': ['.gitignore','LICENSE','README'],
     },
     install_requires=[
         'bcrypt==4.0.1',
         'cryptography==40.0.2',
         'qrcode==7.4.2',
         'ttkbootstrap==1.10.1',
     ],
```

### Comparing `AshCrypt-1.0.1/src/Ash.py` & `AshCrypt-1.1.1/AshCrypt/Ash.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.0.1/src/AshCryptGUI.py` & `AshCrypt-1.1.1/AshCrypt/AshCryptGUI.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.0.1/src/AshDatabase.py` & `AshCrypt-1.1.1/AshCrypt/AshDatabase.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.0.1/src/AshFileCrypt.py` & `AshCrypt-1.1.1/AshCrypt/AshFileCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.0.1/src/AshTextCrypt.py` & `AshCrypt-1.1.1/AshCrypt/AshTextCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.0.1/src/CliCrypt.py` & `AshCrypt-1.1.1/AshCrypt/CliCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.0.1/src/README.md` & `AshCrypt-1.1.1/AshCrypt/README.md`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.0.1/src/qr.py` & `AshCrypt-1.1.1/AshCrypt/qr.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.0.1/unittests/unittestAsh.py` & `AshCrypt-1.1.1/unittests/unittestAsh.py`

 * *Files identical despite different names*

