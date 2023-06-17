# Comparing `tmp/dtorch-0.0.5.tar.gz` & `tmp/dtorch-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtorch-0.0.5.tar", last modified: Wed Jun 14 14:58:47 2023, max compression
+gzip compressed data, was "dtorch-0.0.6.tar", last modified: Sat Jun 17 17:19:37 2023, max compression
```

## Comparing `dtorch-0.0.5.tar` & `dtorch-0.0.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-14 14:58:47.026172 dtorch-0.0.5/
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     1067 2023-06-06 07:48:12.000000 dtorch-0.0.5/LICENSE
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2642 2023-06-14 14:58:47.026172 dtorch-0.0.5/PKG-INFO
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2134 2023-06-07 09:47:40.000000 dtorch-0.0.5/README.md
-drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-14 14:58:47.026172 dtorch-0.0.5/dtorch/
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      225 2023-06-14 14:55:00.000000 dtorch-0.0.5/dtorch/__init__.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     1146 2023-06-06 10:00:04.000000 dtorch-0.0.5/dtorch/dataset.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    17758 2023-06-14 14:55:00.000000 dtorch-0.0.5/dtorch/derivatives.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2096 2023-06-12 11:58:25.000000 dtorch-0.0.5/dtorch/einops.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    17143 2023-06-13 17:43:40.000000 dtorch-0.0.5/dtorch/functionnal.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    12424 2023-06-12 11:58:25.000000 dtorch-0.0.5/dtorch/jtensors.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2679 2023-06-12 11:58:25.000000 dtorch-0.0.5/dtorch/loss.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    16153 2023-06-14 14:55:00.000000 dtorch-0.0.5/dtorch/nn.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      218 2023-06-08 10:17:42.000000 dtorch-0.0.5/dtorch/operation_class.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      940 2023-06-06 10:00:04.000000 dtorch-0.0.5/dtorch/operations.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     7914 2023-06-12 11:58:25.000000 dtorch-0.0.5/dtorch/optim.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     1606 2023-06-12 11:58:25.000000 dtorch-0.0.5/dtorch/typing.py
-drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-14 14:58:47.026172 dtorch-0.0.5/dtorch.egg-info/
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2642 2023-06-14 14:58:47.000000 dtorch-0.0.5/dtorch.egg-info/PKG-INFO
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      498 2023-06-14 14:58:47.000000 dtorch-0.0.5/dtorch.egg-info/SOURCES.txt
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)        1 2023-06-14 14:58:47.000000 dtorch-0.0.5/dtorch.egg-info/dependency_links.txt
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)       15 2023-06-14 14:58:47.000000 dtorch-0.0.5/dtorch.egg-info/requires.txt
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)       31 2023-06-14 14:58:47.000000 dtorch-0.0.5/dtorch.egg-info/top_level.txt
-drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-14 14:58:47.026172 dtorch-0.0.5/dtorchtext/
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-14 14:55:00.000000 dtorch-0.0.5/dtorchtext/datasets.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-14 14:55:00.000000 dtorch-0.0.5/dtorchtext/models.py
-drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-14 14:58:47.026172 dtorch-0.0.5/dtorchvision/
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     4690 2023-06-14 14:55:00.000000 dtorch-0.0.5/dtorchvision/datasets.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2994 2023-06-14 14:55:00.000000 dtorch-0.0.5/dtorchvision/models.py
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      689 2023-06-14 14:57:56.000000 dtorch-0.0.5/pyproject.toml
--rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)       38 2023-06-14 14:58:47.026172 dtorch-0.0.5/setup.cfg
+drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-17 17:19:37.620059 dtorch-0.0.6/
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     1067 2023-06-06 07:48:12.000000 dtorch-0.0.6/LICENSE
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2801 2023-06-17 17:19:37.620059 dtorch-0.0.6/PKG-INFO
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2293 2023-06-17 17:18:46.000000 dtorch-0.0.6/README.md
+drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-17 17:19:37.620059 dtorch-0.0.6/dtorch/
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      225 2023-06-14 14:55:00.000000 dtorch-0.0.6/dtorch/__init__.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2312 2023-06-17 17:18:46.000000 dtorch-0.0.6/dtorch/dataset.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    17758 2023-06-14 14:55:00.000000 dtorch-0.0.6/dtorch/derivatives.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2096 2023-06-12 11:58:25.000000 dtorch-0.0.6/dtorch/einops.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    17008 2023-06-17 17:18:46.000000 dtorch-0.0.6/dtorch/functionnal.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    12424 2023-06-12 11:58:25.000000 dtorch-0.0.6/dtorch/jtensors.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2679 2023-06-12 11:58:25.000000 dtorch-0.0.6/dtorch/loss.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)    17143 2023-06-17 17:18:46.000000 dtorch-0.0.6/dtorch/nn.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      218 2023-06-08 10:17:42.000000 dtorch-0.0.6/dtorch/operation_class.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      940 2023-06-06 10:00:04.000000 dtorch-0.0.6/dtorch/operations.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     7914 2023-06-12 11:58:25.000000 dtorch-0.0.6/dtorch/optim.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     1606 2023-06-12 11:58:25.000000 dtorch-0.0.6/dtorch/typing.py
+drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-17 17:19:37.620059 dtorch-0.0.6/dtorch.egg-info/
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2801 2023-06-17 17:19:37.000000 dtorch-0.0.6/dtorch.egg-info/PKG-INFO
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      498 2023-06-17 17:19:37.000000 dtorch-0.0.6/dtorch.egg-info/SOURCES.txt
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)        1 2023-06-17 17:19:37.000000 dtorch-0.0.6/dtorch.egg-info/dependency_links.txt
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)       15 2023-06-17 17:19:37.000000 dtorch-0.0.6/dtorch.egg-info/requires.txt
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)       31 2023-06-17 17:19:37.000000 dtorch-0.0.6/dtorch.egg-info/top_level.txt
+drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-17 17:19:37.620059 dtorch-0.0.6/dtorchtext/
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-14 14:55:00.000000 dtorch-0.0.6/dtorchtext/datasets.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-14 14:55:00.000000 dtorch-0.0.6/dtorchtext/models.py
+drwxr-xr-x   0 ostentatoire  (1000) ostentatoire  (1001)        0 2023-06-17 17:19:37.620059 dtorch-0.0.6/dtorchvision/
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     3687 2023-06-17 17:18:46.000000 dtorch-0.0.6/dtorchvision/datasets.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)     2113 2023-06-17 17:18:46.000000 dtorch-0.0.6/dtorchvision/models.py
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)      689 2023-06-17 17:19:08.000000 dtorch-0.0.6/pyproject.toml
+-rw-r--r--   0 ostentatoire  (1000) ostentatoire  (1001)       38 2023-06-17 17:19:37.620059 dtorch-0.0.6/setup.cfg
```

### Comparing `dtorch-0.0.5/LICENSE` & `dtorch-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.5/PKG-INFO` & `dtorch-0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtorch
-Version: 0.0.5
+Version: 0.0.6
 Summary: A scientific package made a fellow student
 Author-email: Just1truc <hyppoduc@gmail.com>
 Project-URL: Homepage, https://github.com/Just1truc/dtorch
 Project-URL: Bug Tracker, https://github.com/Just1truc/dtorch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -40,11 +40,13 @@
 | dtorch | the base module where other are regrouped|
 | functionnal | a gather of all the functions that can be used on jtensors|
 | jtensors | a simple module containing the JTensors declaration |
 | loss | loss classes for model implementation |
 | nn | a neural network layer system and its multiple layers (see doc for more details).|
 | einops | a basic reproduction of some einops library methods that support autograd |
 | optim | A library contaning the optimizers that can be used on the networks parameters. |
+| dtorchvision | A lib containing visual datasets and models (pretrained too) |
+| dtorchtext | A lib containing textual datasets and models (pretrained too) |
 
 ### About Autograd
 
 The implementation in this library may not be the most effective computationnaly but the goal was to make it simple and make it work effectively by relying on numpy matrices operations for computation speed concerns.
```

### Comparing `dtorch-0.0.5/README.md` & `dtorch-0.0.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -26,11 +26,13 @@
 | dtorch | the base module where other are regrouped|
 | functionnal | a gather of all the functions that can be used on jtensors|
 | jtensors | a simple module containing the JTensors declaration |
 | loss | loss classes for model implementation |
 | nn | a neural network layer system and its multiple layers (see doc for more details).|
 | einops | a basic reproduction of some einops library methods that support autograd |
 | optim | A library contaning the optimizers that can be used on the networks parameters. |
+| dtorchvision | A lib containing visual datasets and models (pretrained too) |
+| dtorchtext | A lib containing textual datasets and models (pretrained too) |
 
 ### About Autograd
 
 The implementation in this library may not be the most effective computationnaly but the goal was to make it simple and make it work effectively by relying on numpy matrices operations for computation speed concerns.
```

### Comparing `dtorch-0.0.5/dtorch/derivatives.py` & `dtorch-0.0.6/dtorch/derivatives.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.5/dtorch/einops.py` & `dtorch-0.0.6/dtorch/einops.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.5/dtorch/functionnal.py` & `dtorch-0.0.6/dtorch/functionnal.py`

 * *Files 1% similar despite different names*

```diff
@@ -434,17 +434,14 @@
     Returns:
         JTensors: the created tensor
     """
 
     return dtorch.jtensors.JTensors(np.arange(start, end, step))
 
 
-@types(list = (list, np.ndarray), require_grads = bool,
-       dtype = (type, np.dtype),
-        return_type=dtorch.jtensors.JTensors)
 def tensor(list : list | np.ndarray, require_grads : bool = False, dtype : type | np.dtype = np.float64) -> dtorch.jtensors.JTensors:
 
     """create a tensor from a list or a numpy array
 
     Args:
         list (list | np.ndarray): the list or numpy array to create the tensor from
     """
```

### Comparing `dtorch-0.0.5/dtorch/jtensors.py` & `dtorch-0.0.6/dtorch/jtensors.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.5/dtorch/loss.py` & `dtorch-0.0.6/dtorch/loss.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.5/dtorch/nn.py` & `dtorch-0.0.6/dtorch/nn.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,49 @@
 """ imports """
 from typing import Any, Optional
 import dtorch
 import functools
 from math import sqrt
 import pickle
+from abc import ABC
+import os
+import requests
 
 # gabriel destr
 
+class JPretrainedModel(ABC):
+
+    def __init__(self,
+                 model_name : str,
+                 type : str,
+                 root : str = '.models') -> None:
+        """Pretrained model interface
+
+        Args:
+            model_name (str): model name
+            root (str, optional): where the model should be found. Defaults to '.models'.
+        """
+
+        self.__model_url : str = 'https://raw.githubusercontent.com/Just1truc/dtorch/main/pretrained_model/' + type + '/' + model_name + '.jt'
+        self.__model_path : str = os.path.join(root, f'{model_name}.jt')
+        self.__root : str = root
+
+        if not(os.path.isdir(root)):
+            os.makedirs(self.__root)
+        
+        if not(os.path.exists(self.__model_path)):
+            with open(self.__model_path, 'wb') as bf:
+                bf.write(requests.get(self.__model_url).content)
+
+
+    @property
+    def model_path(self):
+        return self.__model_path
+
+
 class Parameter:
 
     def __init__(self, tensor : dtorch.jtensors.JTensors, name : str = "") -> None:
         
         self.__tensor : dtorch.jtensors.JTensors = tensor
         self.__tensor.require_grads = True
         if (name != ""):
```

### Comparing `dtorch-0.0.5/dtorch/operations.py` & `dtorch-0.0.6/dtorch/operations.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.5/dtorch/optim.py` & `dtorch-0.0.6/dtorch/optim.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.5/dtorch/typing.py` & `dtorch-0.0.6/dtorch/typing.py`

 * *Files identical despite different names*

### Comparing `dtorch-0.0.5/dtorch.egg-info/PKG-INFO` & `dtorch-0.0.6/dtorch.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtorch
-Version: 0.0.5
+Version: 0.0.6
 Summary: A scientific package made a fellow student
 Author-email: Just1truc <hyppoduc@gmail.com>
 Project-URL: Homepage, https://github.com/Just1truc/dtorch
 Project-URL: Bug Tracker, https://github.com/Just1truc/dtorch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -40,11 +40,13 @@
 | dtorch | the base module where other are regrouped|
 | functionnal | a gather of all the functions that can be used on jtensors|
 | jtensors | a simple module containing the JTensors declaration |
 | loss | loss classes for model implementation |
 | nn | a neural network layer system and its multiple layers (see doc for more details).|
 | einops | a basic reproduction of some einops library methods that support autograd |
 | optim | A library contaning the optimizers that can be used on the networks parameters. |
+| dtorchvision | A lib containing visual datasets and models (pretrained too) |
+| dtorchtext | A lib containing textual datasets and models (pretrained too) |
 
 ### About Autograd
 
 The implementation in this library may not be the most effective computationnaly but the goal was to make it simple and make it work effectively by relying on numpy matrices operations for computation speed concerns.
```

### Comparing `dtorch-0.0.5/dtorchvision/models.py` & `dtorch-0.0.6/dtorchvision/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,25 @@
 """ imports """
 from typing import Any
 import dtorch as dt
 from abc import ABC
 import os
 import requests
-
-# PRETRAINED MODELs
-
-class JPretrainedModel(ABC):
-
-    def __init__(self,
-                 model_name : str,
-                 root : str = '.models') -> None:
-        """Pretrained model interface
-
-        Args:
-            model_name (str): model name
-            root (str, optional): where the model should be found. Defaults to '.models'.
-        """
-
-        self.__model_url : str = 'https://raw.githubusercontent.com/Just1truc/dtorch/main/pretrained_model/dtorchvision/' + model_name + '.jt'
-        self.__model_path : str = os.path.join(root, f'{model_name}.jt')
-        self.__root : str = root
-
-        if not(os.path.isdir(root)):
-            os.makedirs(self.__root)
-        
-        if not(os.path.exists(self.__model_path)):
-            with open(self.__model_path, 'wb') as bf:
-                bf.write(requests.get(self.__model_url).content)
-
-
-    @property
-    def model_path(self):
-        return self.__model_path
-
+from dtorch.nn import JPretrainedModel
 
 class MNISTAutoEncoder_128_32(JPretrainedModel):
 
     def __init__(self, root : str = './models') -> None:
         """MNIST Autoencoder (1070 loss (MSE mean) on 60000 images)
 
         Args:
             root (str, optional): root of model folder. Defaults to '.models'.
         """
 
-        super().__init__('mnist_128_32', root=root)
+        super().__init__('mnist_128_32', 'dtorchvision', root=root)
 
         self.__model = AutoEncoder(784, [128, 32])
         self.__model.load(self.model_path)
         self.__model.eval()
 
     
     def forward(self, *args, **kwargs):
```

### Comparing `dtorch-0.0.5/pyproject.toml` & `dtorch-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [project]
 dependencies = [
   'requests',
   'numpy'
 ]
 name = "dtorch"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Just1truc", email="hyppoduc@gmail.com" },
 ]
 description = "A scientific package made a fellow student"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

