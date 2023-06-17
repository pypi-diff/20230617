# Comparing `tmp/Pyara-0.1.26.tar.gz` & `tmp/Pyara-0.1.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Pyara-0.1.26.tar", last modified: Fri Jun 16 11:06:03 2023, max compression
+gzip compressed data, was "dist\Pyara-0.1.27.tar", last modified: Sat Jun 17 15:00:33 2023, max compression
```

## Comparing `Pyara-0.1.26.tar` & `Pyara-0.1.27.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 11:06:03.000000 Pyara-0.1.26/
--rw-rw-rw-   0        0        0     1098 2023-06-05 08:31:19.000000 Pyara-0.1.26/LICENSE
--rw-rw-rw-   0        0        0       73 2023-06-16 10:56:25.000000 Pyara-0.1.26/MANIFEST.in
--rw-rw-rw-   0        0        0      539 2023-06-16 11:06:03.000000 Pyara-0.1.26/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-16 11:06:03.000000 Pyara-0.1.26/Pyara.egg-info/
--rw-rw-rw-   0        0        0      539 2023-06-16 11:06:03.000000 Pyara-0.1.26/Pyara.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      492 2023-06-16 11:06:03.000000 Pyara-0.1.26/Pyara.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 11:06:03.000000 Pyara-0.1.26/Pyara.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-21 09:07:37.000000 Pyara-0.1.26/Pyara.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       33 2023-06-16 11:06:03.000000 Pyara-0.1.26/Pyara.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 11:06:03.000000 Pyara-0.1.26/Pyara.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       48 2023-04-10 18:25:02.000000 Pyara-0.1.26/README.md
--rw-rw-rw-   0        0        0      950 2023-06-11 12:54:48.000000 Pyara-0.1.26/instruct.txt
--rw-rw-rw-   0        0        0    92204 2023-03-28 18:31:37.000000 Pyara-0.1.26/mozila11_1.wav
--rw-rw-rw-   0        0        0   164396 2023-03-28 18:37:21.000000 Pyara-0.1.26/mozila11_2.wav
-drwxrwxrwx   0        0        0        0 2023-06-16 11:06:03.000000 Pyara-0.1.26/pyara/
-drwxrwxrwx   0        0        0        0 2023-06-16 11:06:03.000000 Pyara-0.1.26/pyara/Model/
--rw-rw-rw-   0        0        0        0 2023-06-11 12:49:19.000000 Pyara-0.1.26/pyara/Model/__init__.py
--rw-rw-rw-   0        0        0     3983 2023-06-16 11:06:00.000000 Pyara-0.1.26/pyara/Model/model.py
--rw-rw-rw-   0        0        0  1075221 2023-04-03 12:30:41.000000 Pyara-0.1.26/pyara/Model_weights.bin
--rw-rw-rw-   0        0        0      350 2023-06-14 09:04:25.000000 Pyara-0.1.26/pyara/__init__.py
--rw-rw-rw-   0        0        0     6412 2023-06-14 08:53:51.000000 Pyara-0.1.26/pyara/audio_prepare.py
--rw-rw-rw-   0        0        0     1029 2023-05-21 08:36:42.000000 Pyara-0.1.26/pyara/config.py
--rw-rw-rw-   0        0        0      836 2023-06-14 08:53:51.000000 Pyara-0.1.26/pyara/main.py
--rw-rw-rw-   0        0        0   184364 2023-03-28 18:31:37.000000 Pyara-0.1.26/pyara/mozila11_0.wav
--rw-rw-rw-   0        0        0       28 2023-06-14 09:11:56.000000 Pyara-0.1.26/pyara/some.txt
--rw-rw-rw-   0        0        0      108 2023-06-05 08:20:17.000000 Pyara-0.1.26/pyproject.toml
--rw-rw-rw-   0        0        0      276 2023-05-28 20:41:04.000000 Pyara-0.1.26/requirements.txt
--rw-rw-rw-   0        0        0      131 2023-05-30 08:51:00.000000 Pyara-0.1.26/requirements_dev.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 11:06:03.000000 Pyara-0.1.26/setup.cfg
--rw-rw-rw-   0        0        0     1116 2023-06-16 11:06:00.000000 Pyara-0.1.26/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 15:00:33.000000 Pyara-0.1.27/
+-rw-rw-rw-   0        0        0     1098 2023-06-05 08:31:19.000000 Pyara-0.1.27/LICENSE
+-rw-rw-rw-   0        0        0       73 2023-06-16 10:56:25.000000 Pyara-0.1.27/MANIFEST.in
+-rw-rw-rw-   0        0        0      539 2023-06-17 15:00:33.000000 Pyara-0.1.27/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-17 15:00:33.000000 Pyara-0.1.27/Pyara.egg-info/
+-rw-rw-rw-   0        0        0      539 2023-06-17 15:00:33.000000 Pyara-0.1.27/Pyara.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2023-06-17 15:00:33.000000 Pyara-0.1.27/Pyara.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 15:00:33.000000 Pyara-0.1.27/Pyara.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-21 09:07:37.000000 Pyara-0.1.27/Pyara.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       54 2023-06-17 15:00:33.000000 Pyara-0.1.27/Pyara.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-17 15:00:33.000000 Pyara-0.1.27/Pyara.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       48 2023-04-10 18:25:02.000000 Pyara-0.1.27/README.md
+-rw-rw-rw-   0        0        0      950 2023-06-11 12:54:48.000000 Pyara-0.1.27/instruct.txt
+-rw-rw-rw-   0        0        0    92204 2023-03-28 18:31:37.000000 Pyara-0.1.27/mozila11_1.wav
+-rw-rw-rw-   0        0        0   164396 2023-03-28 18:37:21.000000 Pyara-0.1.27/mozila11_2.wav
+drwxrwxrwx   0        0        0        0 2023-06-17 15:00:33.000000 Pyara-0.1.27/pyara/
+drwxrwxrwx   0        0        0        0 2023-06-17 15:00:33.000000 Pyara-0.1.27/pyara/Model/
+-rw-rw-rw-   0        0        0  1075221 2023-04-03 12:30:41.000000 Pyara-0.1.27/pyara/Model/Model_weights.bin
+-rw-rw-rw-   0        0        0        0 2023-06-11 12:49:19.000000 Pyara-0.1.27/pyara/Model/__init__.py
+-rw-rw-rw-   0        0        0     4177 2023-06-17 15:00:11.000000 Pyara-0.1.27/pyara/Model/model.py
+-rw-rw-rw-   0        0        0      350 2023-06-14 09:04:25.000000 Pyara-0.1.27/pyara/__init__.py
+-rw-rw-rw-   0        0        0     6412 2023-06-14 08:53:51.000000 Pyara-0.1.27/pyara/audio_prepare.py
+-rw-rw-rw-   0        0        0     1029 2023-05-21 08:36:42.000000 Pyara-0.1.27/pyara/config.py
+-rw-rw-rw-   0        0        0      836 2023-06-14 08:53:51.000000 Pyara-0.1.27/pyara/main.py
+-rw-rw-rw-   0        0        0   184364 2023-03-28 18:31:37.000000 Pyara-0.1.27/pyara/mozila11_0.wav
+-rw-rw-rw-   0        0        0       28 2023-06-14 09:11:56.000000 Pyara-0.1.27/pyara/some.txt
+-rw-rw-rw-   0        0        0      108 2023-06-05 08:20:17.000000 Pyara-0.1.27/pyproject.toml
+-rw-rw-rw-   0        0        0      276 2023-05-28 20:41:04.000000 Pyara-0.1.27/requirements.txt
+-rw-rw-rw-   0        0        0      131 2023-05-30 08:51:00.000000 Pyara-0.1.27/requirements_dev.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 15:00:33.000000 Pyara-0.1.27/setup.cfg
+-rw-rw-rw-   0        0        0     1177 2023-06-17 15:00:11.000000 Pyara-0.1.27/setup.py
```

### Comparing `Pyara-0.1.26/LICENSE` & `Pyara-0.1.27/LICENSE`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.26/PKG-INFO` & `Pyara-0.1.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyara
-Version: 0.1.26
+Version: 0.1.27
 Summary: Library for audio classification
 Home-page: https://github.com/Millcool/Pyara.git
 Author: Ilya Mironov
 Author-email: ilyamironov210202@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Pyara-0.1.26/Pyara.egg-info/PKG-INFO` & `Pyara-0.1.27/Pyara.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pyara
-Version: 0.1.26
+Version: 0.1.27
 Summary: Library for audio classification
 Home-page: https://github.com/Millcool/Pyara.git
 Author: Ilya Mironov
 Author-email: ilyamironov210202@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `Pyara-0.1.26/instruct.txt` & `Pyara-0.1.27/instruct.txt`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.26/mozila11_1.wav` & `Pyara-0.1.27/mozila11_1.wav`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.26/mozila11_2.wav` & `Pyara-0.1.27/mozila11_2.wav`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.26/pyara/Model/model.py` & `Pyara-0.1.27/pyara/Model/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Module for where models described
 """
 import torch
 from torch import nn
-
+import os
 from pyara.config import CFG
 
 
 class ResNetBlock(nn.Module):
     """Class for ResNet Block description"""
 
     def __init__(self, in_depth, depth, first=False):
@@ -111,13 +111,18 @@
         return out
 
 
 def model_eval():
     """Function for model Evaluation"""
 
     model = MFCCModel()
-    model.load_state_dict(torch.load('Model_weights.bin',
+    import os
+
+    module_path = os.path.dirname(__file__)  # Путь к текущему модулю (mylibrary.py)
+    weights_path = os.path.join(module_path,  'Model_weights.bin')
+
+    model.load_state_dict(torch.load(weights_path,
                                      map_location=torch.device('cpu')))
     model.eval()
     model.to(CFG.device)
     print(' Model Evaluated ! DONE !')
     return model
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Pyara-0.1.26/pyara/Model_weights.bin` & `Pyara-0.1.27/pyara/Model/Model_weights.bin`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.26/pyara/audio_prepare.py` & `Pyara-0.1.27/pyara/audio_prepare.py`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.26/pyara/config.py` & `Pyara-0.1.27/pyara/config.py`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.26/pyara/main.py` & `Pyara-0.1.27/pyara/main.py`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.26/pyara/mozila11_0.wav` & `Pyara-0.1.27/pyara/mozila11_0.wav`

 * *Files identical despite different names*

### Comparing `Pyara-0.1.26/setup.py` & `Pyara-0.1.27/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Metadata of package"""
 from setuptools import setup, find_packages   # ,  pkg_resources
 
 requirements = ['torch>=1.13.1',
-                'torchaudio>=0.13.1'
+                'torchaudio>=0.13.1',
+                'soundfile==0.12.1',
+                'os'
                 ]
 
 # Создаст библиотеку для загрузки на PyPI
 setup(name='Pyara',
-      version='0.1.26',
+      version='0.1.27',
       url='https://github.com/Millcool/Pyara.git',
       license='MIT',
       author='Ilya Mironov',
       author_email='ilyamironov210202@gmail.com',
       description='Library for audio classification',
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

