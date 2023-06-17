# Comparing `tmp/AshCrypt-1.0.tar.gz` & `tmp/AshCrypt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AshCrypt-1.0.tar", last modified: Sat Jun 17 02:45:30 2023, max compression
+gzip compressed data, was "AshCrypt-1.0.1.tar", last modified: Sat Jun 17 13:01:27 2023, max compression
```

## Comparing `AshCrypt-1.0.tar` & `AshCrypt-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 02:45:30.820248 AshCrypt-1.0/
-drwxrwxrwx   0        0        0        0 2023-06-17 02:45:30.774901 AshCrypt-1.0/AshCrypt.egg-info/
--rw-rw-rw-   0        0        0    14982 2023-06-17 02:45:30.000000 AshCrypt-1.0/AshCrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-06-17 02:45:30.000000 AshCrypt-1.0/AshCrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 02:45:30.000000 AshCrypt-1.0/AshCrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-06-17 02:45:30.000000 AshCrypt-1.0/AshCrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-17 02:45:30.000000 AshCrypt-1.0/AshCrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-05-28 20:09:20.000000 AshCrypt-1.0/LICENSE
--rw-rw-rw-   0        0        0    14982 2023-06-17 02:45:30.818728 AshCrypt-1.0/PKG-INFO
--rw-rw-rw-   0        0        0    16201 2023-06-17 02:36:27.000000 AshCrypt-1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-17 02:45:30.820248 AshCrypt-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1553 2023-06-17 02:45:21.000000 AshCrypt-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 02:45:30.806705 AshCrypt-1.0/src/
--rw-rw-rw-   0        0        0     5157 2023-06-16 19:49:28.000000 AshCrypt-1.0/src/Ash.py
--rw-rw-rw-   0        0        0     4378 2023-06-16 19:49:28.000000 AshCrypt-1.0/src/AshCryptGUI.py
--rw-rw-rw-   0        0        0     7922 2023-06-16 19:49:28.000000 AshCrypt-1.0/src/AshDatabase.py
--rw-rw-rw-   0        0        0     2987 2023-06-16 19:49:28.000000 AshCrypt-1.0/src/AshFileCrypt.py
--rw-rw-rw-   0        0        0     2060 2023-06-16 19:49:28.000000 AshCrypt-1.0/src/AshTextCrypt.py
--rw-rw-rw-   0        0        0     5973 2023-06-16 19:49:28.000000 AshCrypt-1.0/src/CliCrypt.py
--rw-rw-rw-   0        0        0    14065 2023-06-17 02:43:04.000000 AshCrypt-1.0/src/README.md
--rw-rw-rw-   0        0        0       98 2023-06-16 19:49:28.000000 AshCrypt-1.0/src/__init__.py
--rw-rw-rw-   0        0        0     1045 2023-06-16 19:49:28.000000 AshCrypt-1.0/src/qr.py
-drwxrwxrwx   0        0        0        0 2023-06-17 02:45:30.814667 AshCrypt-1.0/unittests/
--rw-rw-rw-   0        0        0       25 2023-06-16 19:49:28.000000 AshCrypt-1.0/unittests/__init__.py
--rw-rw-rw-   0        0        0     3397 2023-06-16 19:49:28.000000 AshCrypt-1.0/unittests/unittestAsh.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:01:27.253232 AshCrypt-1.0.1/
+drwxrwxrwx   0        0        0        0 2023-06-17 13:01:27.183137 AshCrypt-1.0.1/AshCrypt.egg-info/
+-rw-rw-rw-   0        0        0    15322 2023-06-17 13:01:26.000000 AshCrypt-1.0.1/AshCrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-06-17 13:01:26.000000 AshCrypt-1.0.1/AshCrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 13:01:26.000000 AshCrypt-1.0.1/AshCrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-06-17 13:01:26.000000 AshCrypt-1.0.1/AshCrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-17 13:01:26.000000 AshCrypt-1.0.1/AshCrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-05-28 20:09:20.000000 AshCrypt-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    15322 2023-06-17 13:01:27.251216 AshCrypt-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    16621 2023-06-17 03:46:03.000000 AshCrypt-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-17 13:01:27.253232 AshCrypt-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1555 2023-06-17 13:00:41.000000 AshCrypt-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:01:27.232287 AshCrypt-1.0.1/src/
+-rw-rw-rw-   0        0        0     5157 2023-06-16 19:49:28.000000 AshCrypt-1.0.1/src/Ash.py
+-rw-rw-rw-   0        0        0     4378 2023-06-16 19:49:28.000000 AshCrypt-1.0.1/src/AshCryptGUI.py
+-rw-rw-rw-   0        0        0     7922 2023-06-16 19:49:28.000000 AshCrypt-1.0.1/src/AshDatabase.py
+-rw-rw-rw-   0        0        0     2987 2023-06-16 19:49:28.000000 AshCrypt-1.0.1/src/AshFileCrypt.py
+-rw-rw-rw-   0        0        0     2060 2023-06-16 19:49:28.000000 AshCrypt-1.0.1/src/AshTextCrypt.py
+-rw-rw-rw-   0        0        0     5972 2023-06-17 12:59:06.000000 AshCrypt-1.0.1/src/CliCrypt.py
+-rw-rw-rw-   0        0        0    14403 2023-06-17 12:58:00.000000 AshCrypt-1.0.1/src/README.md
+-rw-rw-rw-   0        0        0       98 2023-06-16 19:49:28.000000 AshCrypt-1.0.1/src/__init__.py
+-rw-rw-rw-   0        0        0     1045 2023-06-16 19:49:28.000000 AshCrypt-1.0.1/src/qr.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:01:27.245172 AshCrypt-1.0.1/unittests/
+-rw-rw-rw-   0        0        0       25 2023-06-16 19:49:28.000000 AshCrypt-1.0.1/unittests/__init__.py
+-rw-rw-rw-   0        0        0     3397 2023-06-16 19:49:28.000000 AshCrypt-1.0.1/unittests/unittestAsh.py
```

### Comparing `AshCrypt-1.0/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-1.0.1/AshCrypt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.0
+Version: 1.0.1
 Summary: Comprehensive AES-256 Cryptography library equipped with a file handling module along with a text module w/ a user-friendly GUI and a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography,AES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -19,45 +19,46 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Cryptography w/ AES-256
 ##  Objective ## 
 #### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256.
 ## Overview ## 
-**Visit [GitHub](https://github.com/AshGw/AES-256/tree/main)**
-<br>The project incorporates a library I made called **Ash.py** : 
+**Visit The [GitHub](https://github.com/AshGw/AES-256/tree/main) Repository**
+<br>The library incorporates a base cryptography mdoule called **Ash** 
 
-<br>A simple, secure, and developer-oriented library for
+<br>A simple, secure, and developer-oriented module for
 encryption and decryption with AES-256 (CBC) . It offers an intuitive
 interface, seamless integration with precompiled 
 functions, and robust security measures to safeguard
 sensitive data,  providing a hassle-free experience when dealing with cryptographic libraries.
 <br>View **Features** Header for more details.
 
 
 
-The project uses that same module to ensure secure data encryption and decryption for Files and Texts while keeping it very easy and simple to use .
+The library uses that same module to ensure secure data encryption and decryption for Files and Texts while keeping it very easy and simple to use .
 view the headers for **AshFileCrypt**  and **AshTextCrypt** learn more.
 
 It also includes a simple graphical user interface (GUI) for easy interaction with the **AshTextCrypt** module.
 <br>If you're trying to either encrypt or decrypt some messages on the go ( 200 characters max ) you can use this GUI.
 <br>It also has a qr module associated with it to display the message.
 <br>check **GUI**  for more info.
 
+While The **GUI** is limited to 200 characters of text, if you want to be free over how much data or type of data you want to include, then u can use `CliCrypt.py` which is an innovative command line interface (CLI) designed to provide encryption and decryption capabilities for both text and file data with no constraints
 
 It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
 safe and simple manner, you can use whichever you see fit.
 
 <br>The module has a simple straight forward apporach for dealing with sqlite3 databases, even if youre not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check **AshDatabase** header to learn more.
 
-## Ash Library ##
-The `Ash.py` library is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring the utmost security and 
+## Ash Module ##
+The `Ash.py` module is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring the utmost security and 
 confidentiality.
 
-<br>It uses primitives from the `cryptography.py` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers. 
+<br>It uses primitives from the `cryptography` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers. 
 
 <br>You can check **Features** tag below to learn more about the security features.
 
 ### Usage ##
 1) Generate a key if you don't have one already
 ```python
 mainkey = Enc.genMainkey()
```

### Comparing `AshCrypt-1.0/LICENSE` & `AshCrypt-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.0/PKG-INFO` & `AshCrypt-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.0
+Version: 1.0.1
 Summary: Comprehensive AES-256 Cryptography library equipped with a file handling module along with a text module w/ a user-friendly GUI and a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography,AES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -19,45 +19,46 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Cryptography w/ AES-256
 ##  Objective ## 
 #### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256.
 ## Overview ## 
-**Visit [GitHub](https://github.com/AshGw/AES-256/tree/main)**
-<br>The project incorporates a library I made called **Ash.py** : 
+**Visit The [GitHub](https://github.com/AshGw/AES-256/tree/main) Repository**
+<br>The library incorporates a base cryptography mdoule called **Ash** 
 
-<br>A simple, secure, and developer-oriented library for
+<br>A simple, secure, and developer-oriented module for
 encryption and decryption with AES-256 (CBC) . It offers an intuitive
 interface, seamless integration with precompiled 
 functions, and robust security measures to safeguard
 sensitive data,  providing a hassle-free experience when dealing with cryptographic libraries.
 <br>View **Features** Header for more details.
 
 
 
-The project uses that same module to ensure secure data encryption and decryption for Files and Texts while keeping it very easy and simple to use .
+The library uses that same module to ensure secure data encryption and decryption for Files and Texts while keeping it very easy and simple to use .
 view the headers for **AshFileCrypt**  and **AshTextCrypt** learn more.
 
 It also includes a simple graphical user interface (GUI) for easy interaction with the **AshTextCrypt** module.
 <br>If you're trying to either encrypt or decrypt some messages on the go ( 200 characters max ) you can use this GUI.
 <br>It also has a qr module associated with it to display the message.
 <br>check **GUI**  for more info.
 
+While The **GUI** is limited to 200 characters of text, if you want to be free over how much data or type of data you want to include, then u can use `CliCrypt.py` which is an innovative command line interface (CLI) designed to provide encryption and decryption capabilities for both text and file data with no constraints
 
 It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
 safe and simple manner, you can use whichever you see fit.
 
 <br>The module has a simple straight forward apporach for dealing with sqlite3 databases, even if youre not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check **AshDatabase** header to learn more.
 
-## Ash Library ##
-The `Ash.py` library is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring the utmost security and 
+## Ash Module ##
+The `Ash.py` module is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring the utmost security and 
 confidentiality.
 
-<br>It uses primitives from the `cryptography.py` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers. 
+<br>It uses primitives from the `cryptography` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers. 
 
 <br>You can check **Features** tag below to learn more about the security features.
 
 ### Usage ##
 1) Generate a key if you don't have one already
 ```python
 mainkey = Enc.genMainkey()
```

### Comparing `AshCrypt-1.0/README.md` & `AshCrypt-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ## Reason Behind It
 In a world where control, surveillance, and privacy violations are increasingly prevalent, the protection of individual freedom becomes crucial. 
 
 As a firm believer in **Freedom** , I have developed a set of tools in Python that leverages the AES-256 algorithm to make it easier for undividuals to safeguard their data without blindly relying on third parties to do it tor them  . 
 
 My aim here is to make these tools accessible and user-friendly, even for individuals with limited programming knowledge. By providing these resources, I hope to contribute to the preservation of privacy and enable individuals to take control of their own data security, so feel free to explore these tools.
 ## Overview ## 
-The project incorporates a library I made called [Ash.py](https://github.com/AshGw/AES-256#ash-library) : 
+The project incorporates a library I made called **[AshCrypt](https://github.com/AshGw/AES-256/tree/main/src)** : 
 
 <br>A simple, secure, and developer-oriented library for
 encryption and decryption with AES-256 (CBC) . It offers an intuitive
 interface, seamless integration with precompiled 
 functions, and robust security measures to safeguard
 sensitive data,  providing a hassle-free experience when dealing with cryptographic libraries.
 <br>View [Features](https://github.com/AshGw/AES-256#features) Header for more details.
@@ -30,22 +30,35 @@
 
 It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
 safe and simple manner, you can use whichever you see fit.
 
 <br>The module has a simple straight forward apporach for dealing with sqlite3 databases, even if youre not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check [AshDatabase](https://github.com/AshGw/CryptographyAES-256#ashdatabase) header to learn more.
 
 ## Installation ##
-No need to clone or configure anything manually.
+You can simply use **pip**
+```
+pip install AshCrypt
+```
+This will install the latest version of `AshCrypt`.
+
+<br>If you want to get the whole repo without manual configurations
 <br>Run this command in the Terminal
 ```bash
 curl -sSfL https://raw.githubusercontent.com/AshGw/AES-256/main/important/setup.sh | bash
 ```
 This will run the commands in [setup.sh](important/setup.sh).
 <br>It will clone & install all the dependencies needed on your machine inside the directory you're currently at.
-<br>The GUI will pop off automatically and you can start using it right away.
+<br>The `CliCrypt` will pop off automatically and you can start using it right away.
+
+<br>If you're testing how this works on a Debian based Docker container you can run this command to automatically set the environment before you run the command above
+```bash
+curl -sSfL https://github.com/AshGw/AES-256/blob/main/docker-build/env-setup.sh
+```
+
+
 <details>
 <summary>Got Errors ?</summary>
 
 <h5>For Debian based systems</h5>
 
 1) Install `curl` if you don't have it already 
 ```bash
@@ -59,19 +72,19 @@
 3) If you're running `python 3.6` or older then you might need to install `dataclasses`
 ```
 pip install dataclasses
 ```
 <br>Now if none of this works you might just use the docker image for this purpose, so check this [directory](docker-build)
 </details>
 
-## Ash Library ##
-The Ash.py library is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring the utmost security and 
+## Ash Module ##
+The `Ash.py` Module is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring the utmost security and 
 confidentiality.
 
-<br>It uses primitives from the cryptography.py library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers. 
+<br>It uses primitives from the `cryptography.py` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers. 
 
 <br>You can check [Features](https://github.com/AshGw/AES-256#features) tag below to learn more about the security features.
 <br>You can check the [unittesting file](unittests/unittestAsh.py) to verify how it works.
 
 ### Usage ##
 1) Generate a key if you don't have one already
 ```python
```

### Comparing `AshCrypt-1.0/setup.py` & `AshCrypt-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('src/README.md','r') as f :
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='1.0',
+    version='1.0.1',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography library equipped with a file handling module along with"
                 " a text module w/ a user-friendly GUI and a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

### Comparing `AshCrypt-1.0/src/Ash.py` & `AshCrypt-1.0.1/src/Ash.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.0/src/AshCryptGUI.py` & `AshCrypt-1.0.1/src/AshCryptGUI.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.0/src/AshDatabase.py` & `AshCrypt-1.0.1/src/AshDatabase.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.0/src/AshFileCrypt.py` & `AshCrypt-1.0.1/src/AshFileCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.0/src/AshTextCrypt.py` & `AshCrypt-1.0.1/src/AshTextCrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.0/src/CliCrypt.py` & `AshCrypt-1.0.1/src/CliCrypt.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             return None
 def intro():
     intro = True
     while intro:
         print('Program started running..')
         print('Press c to view commands : ')
         while True:
-            n = input("Press : \n")
+            n = input("Press..\n")
             inputWrap(n)
 def keysetup():
     outer = True
     inner = True
     while outer :
         global key
         key = ''
```

### Comparing `AshCrypt-1.0/src/README.md` & `AshCrypt-1.0.1/src/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 # Cryptography w/ AES-256
 ##  Objective ## 
 #### Enhanced Security, Simplicity & Ease of use For Everyone And Anyone Willing To Use AES 256.
 ## Overview ## 
-**Visit [GitHub](https://github.com/AshGw/AES-256/tree/main)**
-<br>The project incorporates a library I made called **Ash.py** : 
+**Visit The [GitHub](https://github.com/AshGw/AES-256/tree/main) Repository**
+<br>The library incorporates a base cryptography mdoule called **Ash** 
 
-<br>A simple, secure, and developer-oriented library for
+<br>A simple, secure, and developer-oriented module for
 encryption and decryption with AES-256 (CBC) . It offers an intuitive
 interface, seamless integration with precompiled 
 functions, and robust security measures to safeguard
 sensitive data,  providing a hassle-free experience when dealing with cryptographic libraries.
 <br>View **Features** Header for more details.
 
 
 
-The project uses that same module to ensure secure data encryption and decryption for Files and Texts while keeping it very easy and simple to use .
+The library uses that same module to ensure secure data encryption and decryption for Files and Texts while keeping it very easy and simple to use .
 view the headers for **AshFileCrypt**  and **AshTextCrypt** learn more.
 
 It also includes a simple graphical user interface (GUI) for easy interaction with the **AshTextCrypt** module.
 <br>If you're trying to either encrypt or decrypt some messages on the go ( 200 characters max ) you can use this GUI.
 <br>It also has a qr module associated with it to display the message.
 <br>check **GUI**  for more info.
 
+While The **GUI** is limited to 200 characters of text, if you want to be free over how much data or type of data you want to include, then u can use `CliCrypt.py` which is an innovative command line interface (CLI) designed to provide encryption and decryption capabilities for both text and file data with no constraints
 
 It also incorporates a database module that serve the same purpose which is allowing for the management and storage of classified content in a secure, 
 safe and simple manner, you can use whichever you see fit.
 
 <br>The module has a simple straight forward apporach for dealing with sqlite3 databases, even if youre not familiar with Python itself you can still use this module to run SQL queries and built in functions to perform various operations on a given database.<br>Check **AshDatabase** header to learn more.
 
-## Ash Library ##
-The `Ash.py` library is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring the utmost security and 
+## Ash Module ##
+The `Ash.py` module is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring the utmost security and 
 confidentiality.
 
-<br>It uses primitives from the `cryptography.py` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers. 
+<br>It uses primitives from the `cryptography` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers. 
 
 <br>You can check **Features** tag below to learn more about the security features.
 
 ### Usage ##
 1) Generate a key if you don't have one already
 ```python
 mainkey = Enc.genMainkey()
```

### Comparing `AshCrypt-1.0/src/qr.py` & `AshCrypt-1.0.1/src/qr.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.0/unittests/unittestAsh.py` & `AshCrypt-1.0.1/unittests/unittestAsh.py`

 * *Files identical despite different names*

