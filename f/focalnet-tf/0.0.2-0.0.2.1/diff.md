# Comparing `tmp/focalnet-tf-0.0.2.tar.gz` & `tmp/focalnet-tf-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\focalnet-tf-0.0.2.tar", last modified: Wed Jun 14 23:50:24 2023, max compression
+gzip compressed data, was "dist\focalnet-tf-0.0.2.1.tar", last modified: Fri Jun 16 23:49:16 2023, max compression
```

## Comparing `focalnet-tf-0.0.2.tar` & `focalnet-tf-0.0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 23:50:24.000000 focalnet-tf-0.0.2/
--rw-rw-rw-   0        0        0     1086 2023-06-11 19:49:16.000000 focalnet-tf-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     4288 2023-06-14 23:50:24.000000 focalnet-tf-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3727 2023-06-11 20:34:38.000000 focalnet-tf-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 23:50:24.000000 focalnet-tf-0.0.2/focalnet/
--rw-rw-rw-   0        0        0      195 2023-06-11 13:35:42.000000 focalnet-tf-0.0.2/focalnet/__init__.py
--rw-rw-rw-   0        0        0     1667 2023-06-11 22:12:59.000000 focalnet-tf-0.0.2/focalnet/download_weights.py
--rw-rw-rw-   0        0        0     1680 2023-06-04 22:28:23.000000 focalnet-tf-0.0.2/focalnet/drop.py
--rw-rw-rw-   0        0        0    23191 2023-06-14 23:09:34.000000 focalnet-tf-0.0.2/focalnet/focalnet.py
--rw-rw-rw-   0        0        0     5289 2023-06-14 23:48:00.000000 focalnet-tf-0.0.2/focalnet/focalnet_utils.py
--rw-rw-rw-   0        0        0    35363 2023-06-09 22:50:12.000000 focalnet-tf-0.0.2/focalnet/imagenet-1k.json
--rw-rw-rw-   0        0        0   872487 2023-06-10 00:38:09.000000 focalnet-tf-0.0.2/focalnet/imagenet-21k.json
--rw-rw-rw-   0        0        0   773963 2023-06-10 00:38:09.000000 focalnet-tf-0.0.2/focalnet/imagenet-22k-reorder.json
-drwxrwxrwx   0        0        0        0 2023-06-14 23:50:24.000000 focalnet-tf-0.0.2/focalnet_tf.egg-info/
--rw-rw-rw-   0        0        0     4288 2023-06-14 23:50:23.000000 focalnet-tf-0.0.2/focalnet_tf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-06-14 23:50:23.000000 focalnet-tf-0.0.2/focalnet_tf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 23:50:23.000000 focalnet-tf-0.0.2/focalnet_tf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-14 23:50:23.000000 focalnet-tf-0.0.2/focalnet_tf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 23:50:23.000000 focalnet-tf-0.0.2/focalnet_tf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 23:50:24.000000 focalnet-tf-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1105 2023-06-14 23:49:06.000000 focalnet-tf-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 23:50:24.000000 focalnet-tf-0.0.2/tests/
--rw-rw-rw-   0        0        0     7608 2023-06-11 20:50:45.000000 focalnet-tf-0.0.2/tests/test_focalnet.py
--rw-rw-rw-   0        0        0    15498 2023-06-11 20:50:53.000000 focalnet-tf-0.0.2/tests/test_reproductible.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:49:16.000000 focalnet-tf-0.0.2.1/
+-rw-rw-rw-   0        0        0     1086 2023-06-11 19:49:16.000000 focalnet-tf-0.0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4290 2023-06-16 23:49:16.000000 focalnet-tf-0.0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3727 2023-06-11 20:34:38.000000 focalnet-tf-0.0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 23:49:16.000000 focalnet-tf-0.0.2.1/focalnet/
+-rw-rw-rw-   0        0        0      195 2023-06-11 13:35:42.000000 focalnet-tf-0.0.2.1/focalnet/__init__.py
+-rw-rw-rw-   0        0        0     1667 2023-06-11 22:12:59.000000 focalnet-tf-0.0.2.1/focalnet/download_weights.py
+-rw-rw-rw-   0        0        0     1740 2023-06-16 23:39:20.000000 focalnet-tf-0.0.2.1/focalnet/drop.py
+-rw-rw-rw-   0        0        0    23191 2023-06-14 23:09:34.000000 focalnet-tf-0.0.2.1/focalnet/focalnet.py
+-rw-rw-rw-   0        0        0     5289 2023-06-14 23:48:00.000000 focalnet-tf-0.0.2.1/focalnet/focalnet_utils.py
+-rw-rw-rw-   0        0        0    35363 2023-06-09 22:50:12.000000 focalnet-tf-0.0.2.1/focalnet/imagenet-1k.json
+-rw-rw-rw-   0        0        0   872487 2023-06-10 00:38:09.000000 focalnet-tf-0.0.2.1/focalnet/imagenet-21k.json
+-rw-rw-rw-   0        0        0   773963 2023-06-10 00:38:09.000000 focalnet-tf-0.0.2.1/focalnet/imagenet-22k-reorder.json
+drwxrwxrwx   0        0        0        0 2023-06-16 23:49:16.000000 focalnet-tf-0.0.2.1/focalnet_tf.egg-info/
+-rw-rw-rw-   0        0        0     4290 2023-06-16 23:49:16.000000 focalnet-tf-0.0.2.1/focalnet_tf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-06-16 23:49:16.000000 focalnet-tf-0.0.2.1/focalnet_tf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 23:49:16.000000 focalnet-tf-0.0.2.1/focalnet_tf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-16 23:49:16.000000 focalnet-tf-0.0.2.1/focalnet_tf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-16 23:49:16.000000 focalnet-tf-0.0.2.1/focalnet_tf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 23:49:16.000000 focalnet-tf-0.0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1105 2023-06-16 23:49:12.000000 focalnet-tf-0.0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:49:16.000000 focalnet-tf-0.0.2.1/tests/
+-rw-rw-rw-   0        0        0     7608 2023-06-11 20:50:45.000000 focalnet-tf-0.0.2.1/tests/test_focalnet.py
+-rw-rw-rw-   0        0        0    15498 2023-06-11 20:50:53.000000 focalnet-tf-0.0.2.1/tests/test_reproductible.py
```

### Comparing `focalnet-tf-0.0.2/LICENSE` & `focalnet-tf-0.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.2/PKG-INFO` & `focalnet-tf-0.0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: focalnet-tf
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: Re-implementation of FocalNet for tensorflow 2.X
 Home-page: https://github.com/Shiro-LK/focalnet-tf
 Download-URL: https://github.com/Shiro-LK/focalnet-tf.git
 Author: Shiro-LK
 Author-email: shirosaki94@gmail.com
 License: MIT License
 Keywords: focalnet,tensorflow
```

### Comparing `focalnet-tf-0.0.2/README.md` & `focalnet-tf-0.0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.2/focalnet/download_weights.py` & `focalnet-tf-0.0.2.1/focalnet/download_weights.py`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.2/focalnet/drop.py` & `focalnet-tf-0.0.2.1/focalnet/drop.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,20 @@
     'survival rate' as the argument.
 
     """
     if drop_prob == 0. or not training:
         return x
     keep_prob = 1 - drop_prob
     shape = (x.shape[0],) + (1,) * (len(tf.shape(x)) - 1)  # work with diff dim tensors, not just 2D ConvNets
-    random_tensor =  tfp.distributions.Bernoulli(keep_prob).sample(shape)
+    random_tensor =  tf.cast(tfp.distributions.Bernoulli(keep_prob).sample(shape), dtype=x.dtype)
+    
     if keep_prob > 0.0 and scale_by_keep:
         random_tensor = random_tensor / keep_prob
-    return x * random_tensor
+    
+    return x * tf.cast(random_tensor, dtype=x.dtype)
 
 
 class DropPath(tf.keras.layers.Layer):
     """Drop paths (Stochastic Depth) per sample  (when applied in main path of residual blocks).
     """
     def __init__(self, drop_prob: float = 0., scale_by_keep: bool = True):
         super(DropPath, self).__init__()
```

### Comparing `focalnet-tf-0.0.2/focalnet/focalnet.py` & `focalnet-tf-0.0.2.1/focalnet/focalnet.py`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.2/focalnet/focalnet_utils.py` & `focalnet-tf-0.0.2.1/focalnet/focalnet_utils.py`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.2/focalnet/imagenet-1k.json` & `focalnet-tf-0.0.2.1/focalnet/imagenet-1k.json`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.2/focalnet/imagenet-21k.json` & `focalnet-tf-0.0.2.1/focalnet/imagenet-21k.json`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.2/focalnet/imagenet-22k-reorder.json` & `focalnet-tf-0.0.2.1/focalnet/imagenet-22k-reorder.json`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.2/focalnet_tf.egg-info/PKG-INFO` & `focalnet-tf-0.0.2.1/focalnet_tf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: focalnet-tf
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: Re-implementation of FocalNet for tensorflow 2.X
 Home-page: https://github.com/Shiro-LK/focalnet-tf
 Download-URL: https://github.com/Shiro-LK/focalnet-tf.git
 Author: Shiro-LK
 Author-email: shirosaki94@gmail.com
 License: MIT License
 Keywords: focalnet,tensorflow
```

### Comparing `focalnet-tf-0.0.2/setup.py` & `focalnet-tf-0.0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open('README.md', encoding="utf-8-sig") as f:
         README = f.read()
     return README
 
 
 setup(
     name='focalnet-tf',
-    version='0.0.2',    
+    version='0.0.2.1',    
     description='Re-implementation of FocalNet for tensorflow 2.X',
     author='Shiro-LK',
     author_email='shirosaki94@gmail.com',
     license='MIT License',
     packages=['focalnet'],
     package_data={'focalnet': ['imagenet-1k.json', 'imagenet-21k.json', 'imagenet-22k-reorder.json']},
     long_description=readme(),
@@ -26,8 +26,8 @@
     download_url='https://github.com/Shiro-LK/focalnet-tf.git',
     keywords=["focalnet", "tensorflow"],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
-)
+)
```

### Comparing `focalnet-tf-0.0.2/tests/test_focalnet.py` & `focalnet-tf-0.0.2.1/tests/test_focalnet.py`

 * *Files identical despite different names*

### Comparing `focalnet-tf-0.0.2/tests/test_reproductible.py` & `focalnet-tf-0.0.2.1/tests/test_reproductible.py`

 * *Files identical despite different names*

