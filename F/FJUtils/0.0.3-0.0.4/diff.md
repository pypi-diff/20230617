# Comparing `tmp/FJUtils-0.0.3.tar.gz` & `tmp/FJUtils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FJUtils-0.0.3.tar", last modified: Mon Jun  5 08:36:48 2023, max compression
+gzip compressed data, was "FJUtils-0.0.4.tar", last modified: Sat Jun 17 07:38:35 2023, max compression
```

## Comparing `FJUtils-0.0.3.tar` & `FJUtils-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-05 08:36:48.474817 FJUtils-0.0.3/
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-05 08:36:48.470817 FJUtils-0.0.3/FJUtils.egg-info/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3670 2023-06-05 08:36:48.000000 FJUtils-0.0.3/FJUtils.egg-info/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      313 2023-06-05 08:36:48.000000 FJUtils-0.0.3/FJUtils.egg-info/SOURCES.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-06-05 08:36:48.000000 FJUtils-0.0.3/FJUtils.egg-info/dependency_links.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      121 2023-06-05 08:36:48.000000 FJUtils-0.0.3/FJUtils.egg-info/requires.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-06-05 08:36:48.000000 FJUtils-0.0.3/FJUtils.egg-info/top_level.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-05-31 06:53:13.000000 FJUtils-0.0.3/LICENSE
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3670 2023-06-05 08:36:48.470817 FJUtils-0.0.3/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2911 2023-06-05 08:34:56.000000 FJUtils-0.0.3/README.md
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-05 08:36:48.470817 FJUtils-0.0.3/fjutils/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      708 2023-05-31 08:45:55.000000 FJUtils-0.0.3/fjutils/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     8245 2023-05-31 15:57:33.000000 FJUtils-0.0.3/fjutils/checkpointing.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     9903 2023-05-31 08:28:39.000000 FJUtils-0.0.3/fjutils/easylm.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1800 2023-05-31 08:45:55.000000 FJUtils-0.0.3/fjutils/load.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     6882 2023-06-05 08:30:43.000000 FJUtils-0.0.3/fjutils/optimizers.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3757 2023-06-05 08:19:58.000000 FJUtils-0.0.3/fjutils/utils.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      533 2023-05-31 08:31:14.000000 FJUtils-0.0.3/pyproject.toml
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-06-05 08:36:48.474817 FJUtils-0.0.3/setup.cfg
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1214 2023-06-05 08:36:45.000000 FJUtils-0.0.3/setup.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-17 07:38:35.353042 FJUtils-0.0.4/
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-17 07:38:35.353042 FJUtils-0.0.4/FJUtils.egg-info/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3670 2023-06-17 07:38:35.000000 FJUtils-0.0.4/FJUtils.egg-info/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      313 2023-06-17 07:38:35.000000 FJUtils-0.0.4/FJUtils.egg-info/SOURCES.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-06-17 07:38:35.000000 FJUtils-0.0.4/FJUtils.egg-info/dependency_links.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      108 2023-06-17 07:38:35.000000 FJUtils-0.0.4/FJUtils.egg-info/requires.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-06-17 07:38:35.000000 FJUtils-0.0.4/FJUtils.egg-info/top_level.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    11357 2023-06-06 11:02:09.000000 FJUtils-0.0.4/LICENSE
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3670 2023-06-17 07:38:35.353042 FJUtils-0.0.4/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2911 2023-06-06 11:02:09.000000 FJUtils-0.0.4/README.md
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-06-17 07:38:35.353042 FJUtils-0.0.4/fjutils/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      708 2023-06-06 11:02:09.000000 FJUtils-0.0.4/fjutils/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     8245 2023-06-06 11:02:09.000000 FJUtils-0.0.4/fjutils/checkpointing.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9932 2023-06-17 07:11:27.000000 FJUtils-0.0.4/fjutils/easylm.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1800 2023-06-06 11:02:09.000000 FJUtils-0.0.4/fjutils/load.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     9494 2023-06-17 07:36:45.000000 FJUtils-0.0.4/fjutils/optimizers.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     7287 2023-06-17 07:27:33.000000 FJUtils-0.0.4/fjutils/utils.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      533 2023-06-06 11:02:09.000000 FJUtils-0.0.4/pyproject.toml
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-06-17 07:38:35.353042 FJUtils-0.0.4/setup.cfg
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1191 2023-06-17 07:38:01.000000 FJUtils-0.0.4/setup.py
```

### Comparing `FJUtils-0.0.3/FJUtils.egg-info/PKG-INFO` & `FJUtils-0.0.4/FJUtils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FJUtils
-Version: 0.0.3
+Version: 0.0.4
 Summary: UNKNOWN
 Home-page: https://github.com/erfanzar/
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@yahoo.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `FJUtils-0.0.3/LICENSE` & `FJUtils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.3/PKG-INFO` & `FJUtils-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FJUtils
-Version: 0.0.3
+Version: 0.0.4
 Summary: UNKNOWN
 Home-page: https://github.com/erfanzar/
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@yahoo.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `FJUtils-0.0.3/README.md` & `FJUtils-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.3/fjutils/__init__.py` & `FJUtils-0.0.4/fjutils/__init__.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.3/fjutils/checkpointing.py` & `FJUtils-0.0.4/fjutils/checkpointing.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.3/fjutils/easylm.py` & `FJUtils-0.0.4/fjutils/easylm.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,19 @@
         partition specs.
     """
     float_dtypes = (jnp.bfloat16, jnp.float16, jnp.float32, jnp.float64)
 
     def make_to_dtype_fn(dtype_spec):
         def to_dtype(tensor):
             if dtype_specs in float_dtypes and getattr(tensor, 'dtype', None) in float_dtypes:
-                # Convert all float tensors to the same dtype
-                return tensor.astype(dtype_specs)
+                # force np array to jax numpy array
+                return jnp.asarray(tensor).astype(dtype_specs)
             elif hasattr(dtype_spec, 'dtype') and hasattr(tensor, 'dtype'):
-                return tensor.astype(dtype_spec.dtype)
-            return tensor
+                return jnp.asarray(tensor).astype(dtype_spec.dtype)
+            return jnp.asarray(tensor)
 
         return to_dtype
 
     def make_shard_fn(partition_spec, dtype_spec=None):
         jax_shard_function = pjit(
             make_to_dtype_fn(dtype_spec),
             in_shardings=None,
```

### Comparing `FJUtils-0.0.3/fjutils/load.py` & `FJUtils-0.0.4/fjutils/load.py`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.3/pyproject.toml` & `FJUtils-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `FJUtils-0.0.3/setup.py` & `FJUtils-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,30 +3,29 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="FJUtils",
-    version='0.0.3',
+    version='0.0.4',
     author="Erfan Zare Chavoshi",
     author_email="erfanzare82@yahoo.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/erfanzar/",
     packages=setuptools.find_packages(),
     install_requires=[
         'jax~=0.4.7',
-        'transformers~=4.29.2',
+        'transformers~=4.30.2',
         'typing~=3.7.4.3',
         'numpy~=1.24.3',
         'flax~=0.6.4',
         'msgpack~=1.0.5',
         'setuptools~=59.6.0',
-        'mlxu~=0.1.11'
     ],
     python_requires=">=3.7, <3.11",
     license='Apache License 2.0',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

