# Comparing `tmp/pylibffm-0.3.0.tar.gz` & `tmp/pylibffm-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibffm-0.3.0.tar", last modified: Tue Jun 13 09:23:06 2023, max compression
+gzip compressed data, was "pylibffm-0.3.1.tar", last modified: Fri Jun 16 18:41:19 2023, max compression
```

## Comparing `pylibffm-0.3.0.tar` & `pylibffm-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-13 09:23:06.658867 pylibffm-0.3.0/
--rw-rw-r--   0 julien    (1003) julien    (1003)       28 2023-06-02 12:46:04.000000 pylibffm-0.3.0/MANIFEST.in
--rw-rw-r--   0 julien    (1003) julien    (1003)     1632 2023-06-13 09:23:06.658867 pylibffm-0.3.0/PKG-INFO
--rw-rw-r--   0 julien    (1003) julien    (1003)      849 2023-06-02 14:05:43.000000 pylibffm-0.3.0/README.md
-drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-13 09:23:06.658867 pylibffm-0.3.0/pylibffm/
--rw-rw-r--   0 julien    (1003) julien    (1003)       19 2023-06-02 06:22:22.000000 pylibffm-0.3.0/pylibffm/__init__.py
--rw-rw-r--   0 julien    (1003) julien    (1003)     6212 2023-06-13 09:21:26.000000 pylibffm-0.3.0/pylibffm/api.py
--rwxrwxr-x   0 julien    (1003) julien    (1003)   325896 2023-06-02 13:45:27.000000 pylibffm-0.3.0/pylibffm/wrapper.cpython-310-x86_64-linux-gnu.so
--rwxrwxr-x   0 julien    (1003) julien    (1003)   330280 2023-06-02 13:45:32.000000 pylibffm-0.3.0/pylibffm/wrapper.cpython-311-x86_64-linux-gnu.so
--rwxrwxr-x   0 julien    (1003) julien    (1003)   325856 2023-06-02 13:45:13.000000 pylibffm-0.3.0/pylibffm/wrapper.cpython-37m-x86_64-linux-gnu.so
--rwxrwxr-x   0 julien    (1003) julien    (1003)   325760 2023-06-02 13:45:18.000000 pylibffm-0.3.0/pylibffm/wrapper.cpython-38-x86_64-linux-gnu.so
--rwxrwxr-x   0 julien    (1003) julien    (1003)   326104 2023-06-02 13:45:23.000000 pylibffm-0.3.0/pylibffm/wrapper.cpython-39-x86_64-linux-gnu.so
-drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-13 09:23:06.658867 pylibffm-0.3.0/pylibffm.egg-info/
--rw-rw-r--   0 julien    (1003) julien    (1003)     1632 2023-06-13 09:23:06.000000 pylibffm-0.3.0/pylibffm.egg-info/PKG-INFO
--rw-rw-r--   0 julien    (1003) julien    (1003)      469 2023-06-13 09:23:06.000000 pylibffm-0.3.0/pylibffm.egg-info/SOURCES.txt
--rw-rw-r--   0 julien    (1003) julien    (1003)        1 2023-06-13 09:23:06.000000 pylibffm-0.3.0/pylibffm.egg-info/dependency_links.txt
--rw-rw-r--   0 julien    (1003) julien    (1003)       12 2023-06-13 09:23:06.000000 pylibffm-0.3.0/pylibffm.egg-info/requires.txt
--rw-rw-r--   0 julien    (1003) julien    (1003)        9 2023-06-13 09:23:06.000000 pylibffm-0.3.0/pylibffm.egg-info/top_level.txt
--rw-rw-r--   0 julien    (1003) julien    (1003)       38 2023-06-13 09:23:06.658867 pylibffm-0.3.0/setup.cfg
--rw-rw-r--   0 julien    (1003) julien    (1003)     1523 2023-06-13 09:23:04.000000 pylibffm-0.3.0/setup.py
+drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-16 18:41:19.792472 pylibffm-0.3.1/
+-rw-rw-r--   0 julien    (1003) julien    (1003)       28 2023-06-02 12:46:04.000000 pylibffm-0.3.1/MANIFEST.in
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1653 2023-06-16 18:41:19.792472 pylibffm-0.3.1/PKG-INFO
+-rw-rw-r--   0 julien    (1003) julien    (1003)      870 2023-06-13 09:33:56.000000 pylibffm-0.3.1/README.md
+drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-16 18:41:19.792472 pylibffm-0.3.1/pylibffm/
+-rw-rw-r--   0 julien    (1003) julien    (1003)       19 2023-06-02 06:22:22.000000 pylibffm-0.3.1/pylibffm/__init__.py
+-rw-rw-r--   0 julien    (1003) julien    (1003)     6265 2023-06-16 18:40:21.000000 pylibffm-0.3.1/pylibffm/api.py
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   325896 2023-06-02 13:45:27.000000 pylibffm-0.3.1/pylibffm/wrapper.cpython-310-x86_64-linux-gnu.so
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   330280 2023-06-02 13:45:32.000000 pylibffm-0.3.1/pylibffm/wrapper.cpython-311-x86_64-linux-gnu.so
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   325856 2023-06-02 13:45:13.000000 pylibffm-0.3.1/pylibffm/wrapper.cpython-37m-x86_64-linux-gnu.so
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   325760 2023-06-02 13:45:18.000000 pylibffm-0.3.1/pylibffm/wrapper.cpython-38-x86_64-linux-gnu.so
+-rwxrwxr-x   0 julien    (1003) julien    (1003)   326104 2023-06-02 13:45:23.000000 pylibffm-0.3.1/pylibffm/wrapper.cpython-39-x86_64-linux-gnu.so
+drwxrwxr-x   0 julien    (1003) julien    (1003)        0 2023-06-16 18:41:19.792472 pylibffm-0.3.1/pylibffm.egg-info/
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1653 2023-06-16 18:41:19.000000 pylibffm-0.3.1/pylibffm.egg-info/PKG-INFO
+-rw-rw-r--   0 julien    (1003) julien    (1003)      469 2023-06-16 18:41:19.000000 pylibffm-0.3.1/pylibffm.egg-info/SOURCES.txt
+-rw-rw-r--   0 julien    (1003) julien    (1003)        1 2023-06-16 18:41:19.000000 pylibffm-0.3.1/pylibffm.egg-info/dependency_links.txt
+-rw-rw-r--   0 julien    (1003) julien    (1003)       12 2023-06-16 18:41:19.000000 pylibffm-0.3.1/pylibffm.egg-info/requires.txt
+-rw-rw-r--   0 julien    (1003) julien    (1003)        9 2023-06-16 18:41:19.000000 pylibffm-0.3.1/pylibffm.egg-info/top_level.txt
+-rw-rw-r--   0 julien    (1003) julien    (1003)       38 2023-06-16 18:41:19.792472 pylibffm-0.3.1/setup.cfg
+-rw-rw-r--   0 julien    (1003) julien    (1003)     1523 2023-06-16 18:41:16.000000 pylibffm-0.3.1/setup.py
```

### Comparing `pylibffm-0.3.0/PKG-INFO` & `pylibffm-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibffm
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library wrapping libffm
 Home-page: https://github.com/Sinacam/pylibffm
 Author: ntumlgroup
 License: MIT License
 Description: # pylibffm
         
         pylibffm is a wrapper around libffm to allow using scipy and numpy arrays as input.
@@ -13,15 +13,15 @@
         ## Installing
         If you're running python 3.7~3.11 on linux
         ```bash
         pip install pylibffm
         ```
         Otherwise
         ```bash
-        git clone https://github.com/Sinacam/pylibffm
+        git clone --recurse-submodules https://github.com/Sinacam/pylibffm
         cd pylibffm
         make
         pip install .
         ```
         Currently, the distribution is incredibly hacky and cannot be pip installed from source.
         Windows build support is lacking, but code should be correct.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_8is1zq55_/tmplvb8nztv_TarContainer/0/2", line 52, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_8is1zq55_/tmplvb8nztv_TarContainer/0/2", line 52, column 0: CDATA terminal not found*

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: pylibffm Version: 0.3.0 Summary: A library wrapping
+Metadata-Version: 2.1 Name: pylibffm Version: 0.3.1 Summary: A library wrapping
 libffm Home-page: https://github.com/Sinacam/pylibffm Author: ntumlgroup
 License: MIT License Description: # pylibffm pylibffm is a wrapper around
 libffm to allow using scipy and numpy arrays as input. pylibffm requires SSE
 and openmp. ## Installing If you're running python 3.7~3.11 on linux ```bash
-pip install pylibffm ``` Otherwise ```bash git clone https://github.com/
-Sinacam/pylibffm cd pylibffm make pip install . ``` Currently, the distribution
-is incredibly hacky and cannot be pip installed from source. Windows build
-support is lacking, but code should be correct. ## Documentation The API only
-consists of + `train` + `load` + `Model` + `Model.save` + `Model.predict` Use
-`help` or read their docstring for their usage. ## Diff with libffm To be
-deterministic, set openmp threads to 1. For pylibffm, do ```bash
-OMP_NUM_THREADS=1 python
+pip install pylibffm ``` Otherwise ```bash git clone --recurse-submodules
+https://github.com/Sinacam/pylibffm cd pylibffm make pip install . ```
+Currently, the distribution is incredibly hacky and cannot be pip installed
+from source. Windows build support is lacking, but code should be correct. ##
+Documentation The API only consists of + `train` + `load` + `Model` +
+`Model.save` + `Model.predict` Use `help` or read their docstring for their
+usage. ## Diff with libffm To be deterministic, set openmp threads to 1. For
+pylibffm, do ```bash OMP_NUM_THREADS=1 python
```

### Comparing `pylibffm-0.3.0/README.md` & `pylibffm-0.3.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ## Installing
 If you're running python 3.7~3.11 on linux
 ```bash
 pip install pylibffm
 ```
 Otherwise
 ```bash
-git clone https://github.com/Sinacam/pylibffm
+git clone --recurse-submodules https://github.com/Sinacam/pylibffm
 cd pylibffm
 make
 pip install .
 ```
 Currently, the distribution is incredibly hacky and cannot be pip installed from source.
 Windows build support is lacking, but code should be correct.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_8is1zq55_/tmplvb8nztv_TarContainer/0/3.md", line 37, column 78: CDATA terminal not found*

 * *File "/tmp/diffoscope_8is1zq55_/tmplvb8nztv_TarContainer/0/3.md", line 37, column 78: CDATA terminal not found*

```diff
@@ -1,10 +1,10 @@
 # pylibffm pylibffm is a wrapper around libffm to allow using scipy and numpy
 arrays as input. pylibffm requires SSE and openmp. ## Installing If you're
 running python 3.7~3.11 on linux ```bash pip install pylibffm ``` Otherwise
-```bash git clone https://github.com/Sinacam/pylibffm cd pylibffm make pip
-install . ``` Currently, the distribution is incredibly hacky and cannot be pip
-installed from source. Windows build support is lacking, but code should be
-correct. ## Documentation The API only consists of + `train` + `load` + `Model`
-+ `Model.save` + `Model.predict` Use `help` or read their docstring for their
-usage. ## Diff with libffm To be deterministic, set openmp threads to 1. For
-pylibffm, do ```bash OMP_NUM_THREADS=1 python
+```bash git clone --recurse-submodules https://github.com/Sinacam/pylibffm cd
+pylibffm make pip install . ``` Currently, the distribution is incredibly hacky
+and cannot be pip installed from source. Windows build support is lacking, but
+code should be correct. ## Documentation The API only consists of + `train` +
+`load` + `Model` + `Model.save` + `Model.predict` Use `help` or read their
+docstring for their usage. ## Diff with libffm To be deterministic, set openmp
+threads to 1. For pylibffm, do ```bash OMP_NUM_THREADS=1 python
```

### Comparing `pylibffm-0.3.0/pylibffm/api.py` & `pylibffm-0.3.1/pylibffm/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
         Returns:
             np.ndarray: An array with dimension number of instances.
         """
         if x.shape[1] != fields.shape[0]:
             raise ValueError("input matrix shapes do not match")
 
+        fields = fields.astype(np.int32, copy=False)
         return wrapper.predict(
             self.n,
             self.m,
             self.k,
             self.W,
             self.normalization,
             x.shape[0],
```

### Comparing `pylibffm-0.3.0/pylibffm/wrapper.cpython-310-x86_64-linux-gnu.so` & `pylibffm-0.3.1/pylibffm/wrapper.cpython-310-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pylibffm-0.3.0/pylibffm/wrapper.cpython-311-x86_64-linux-gnu.so` & `pylibffm-0.3.1/pylibffm/wrapper.cpython-311-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pylibffm-0.3.0/pylibffm/wrapper.cpython-37m-x86_64-linux-gnu.so` & `pylibffm-0.3.1/pylibffm/wrapper.cpython-37m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pylibffm-0.3.0/pylibffm/wrapper.cpython-38-x86_64-linux-gnu.so` & `pylibffm-0.3.1/pylibffm/wrapper.cpython-38-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pylibffm-0.3.0/pylibffm/wrapper.cpython-39-x86_64-linux-gnu.so` & `pylibffm-0.3.1/pylibffm/wrapper.cpython-39-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pylibffm-0.3.0/pylibffm.egg-info/PKG-INFO` & `pylibffm-0.3.1/pylibffm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibffm
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library wrapping libffm
 Home-page: https://github.com/Sinacam/pylibffm
 Author: ntumlgroup
 License: MIT License
 Description: # pylibffm
         
         pylibffm is a wrapper around libffm to allow using scipy and numpy arrays as input.
@@ -13,15 +13,15 @@
         ## Installing
         If you're running python 3.7~3.11 on linux
         ```bash
         pip install pylibffm
         ```
         Otherwise
         ```bash
-        git clone https://github.com/Sinacam/pylibffm
+        git clone --recurse-submodules https://github.com/Sinacam/pylibffm
         cd pylibffm
         make
         pip install .
         ```
         Currently, the distribution is incredibly hacky and cannot be pip installed from source.
         Windows build support is lacking, but code should be correct.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_8is1zq55_/tmplvb8nztv_TarContainer/0/13", line 52, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_8is1zq55_/tmplvb8nztv_TarContainer/0/13", line 52, column 0: CDATA terminal not found*

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: pylibffm Version: 0.3.0 Summary: A library wrapping
+Metadata-Version: 2.1 Name: pylibffm Version: 0.3.1 Summary: A library wrapping
 libffm Home-page: https://github.com/Sinacam/pylibffm Author: ntumlgroup
 License: MIT License Description: # pylibffm pylibffm is a wrapper around
 libffm to allow using scipy and numpy arrays as input. pylibffm requires SSE
 and openmp. ## Installing If you're running python 3.7~3.11 on linux ```bash
-pip install pylibffm ``` Otherwise ```bash git clone https://github.com/
-Sinacam/pylibffm cd pylibffm make pip install . ``` Currently, the distribution
-is incredibly hacky and cannot be pip installed from source. Windows build
-support is lacking, but code should be correct. ## Documentation The API only
-consists of + `train` + `load` + `Model` + `Model.save` + `Model.predict` Use
-`help` or read their docstring for their usage. ## Diff with libffm To be
-deterministic, set openmp threads to 1. For pylibffm, do ```bash
-OMP_NUM_THREADS=1 python
+pip install pylibffm ``` Otherwise ```bash git clone --recurse-submodules
+https://github.com/Sinacam/pylibffm cd pylibffm make pip install . ```
+Currently, the distribution is incredibly hacky and cannot be pip installed
+from source. Windows build support is lacking, but code should be correct. ##
+Documentation The API only consists of + `train` + `load` + `Model` +
+`Model.save` + `Model.predict` Use `help` or read their docstring for their
+usage. ## Diff with libffm To be deterministic, set openmp threads to 1. For
+pylibffm, do ```bash OMP_NUM_THREADS=1 python
```

### Comparing `pylibffm-0.3.0/setup.py` & `pylibffm-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pathlib
 import setuptools
 
 name = "pylibffm"
-version = "0.3.0"
+version = "0.3.1"
 author = "ntumlgroup"
 license = "MIT License"
 license_file = "LICENSE"
 description = "A library wrapping libffm"
 long_description = (pathlib.Path(__file__).parent / "README.md").read_text()
 long_description_content_type = "text/markdown"
 url = "https://github.com/Sinacam/pylibffm"
```

