# Comparing `tmp/kp_compression-0.2.5.tar.gz` & `tmp/kp_compression-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kp_compression-0.2.5.tar", last modified: Wed Feb 22 17:50:34 2023, max compression
+gzip compressed data, was "kp_compression-0.2.6.tar", last modified: Sat Jun 17 17:55:13 2023, max compression
```

## Comparing `kp_compression-0.2.5.tar` & `kp_compression-0.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 varun     (1001) varun     (1001)        0 2023-02-22 17:50:34.222053 kp_compression-0.2.5/
--rw-rw-r--   0 varun     (1001) varun     (1001)      248 2023-02-22 17:50:34.222053 kp_compression-0.2.5/PKG-INFO
--rw-rw-r--   0 varun     (1001) varun     (1001)        0 2022-09-10 09:39:29.000000 kp_compression-0.2.5/README.md
-drwxrwxr-x   0 varun     (1001) varun     (1001)        0 2023-02-22 17:50:34.222053 kp_compression-0.2.5/kp_compression/
--rw-rw-r--   0 varun     (1001) varun     (1001)       65 2022-09-12 12:01:01.000000 kp_compression-0.2.5/kp_compression/__init__.py
--rw-rw-r--   0 varun     (1001) varun     (1001)     9358 2023-02-22 17:42:28.000000 kp_compression-0.2.5/kp_compression/myfunctions.py
-drwxrwxr-x   0 varun     (1001) varun     (1001)        0 2023-02-22 17:50:34.222053 kp_compression-0.2.5/kp_compression.egg-info/
--rw-rw-r--   0 varun     (1001) varun     (1001)      248 2023-02-22 17:50:34.000000 kp_compression-0.2.5/kp_compression.egg-info/PKG-INFO
--rw-rw-r--   0 varun     (1001) varun     (1001)      264 2023-02-22 17:50:34.000000 kp_compression-0.2.5/kp_compression.egg-info/SOURCES.txt
--rw-rw-r--   0 varun     (1001) varun     (1001)        1 2023-02-22 17:50:34.000000 kp_compression-0.2.5/kp_compression.egg-info/dependency_links.txt
--rw-rw-r--   0 varun     (1001) varun     (1001)       12 2023-02-22 17:50:34.000000 kp_compression-0.2.5/kp_compression.egg-info/requires.txt
--rw-rw-r--   0 varun     (1001) varun     (1001)       15 2023-02-22 17:50:34.000000 kp_compression-0.2.5/kp_compression.egg-info/top_level.txt
--rw-rw-r--   0 varun     (1001) varun     (1001)       38 2023-02-22 17:50:34.222053 kp_compression-0.2.5/setup.cfg
--rw-rw-r--   0 varun     (1001) varun     (1001)      349 2023-02-22 17:50:07.000000 kp_compression-0.2.5/setup.py
+drwxrwxr-x   0 varun     (1001) varun     (1001)        0 2023-06-17 17:55:13.884858 kp_compression-0.2.6/
+-rw-rw-r--   0 varun     (1001) varun     (1001)      248 2023-06-17 17:55:13.884858 kp_compression-0.2.6/PKG-INFO
+-rw-rw-r--   0 varun     (1001) varun     (1001)        0 2022-09-10 09:39:29.000000 kp_compression-0.2.6/README.md
+drwxrwxr-x   0 varun     (1001) varun     (1001)        0 2023-06-17 17:55:13.880858 kp_compression-0.2.6/kp_compression/
+-rw-rw-r--   0 varun     (1001) varun     (1001)       65 2022-09-12 12:01:01.000000 kp_compression-0.2.6/kp_compression/__init__.py
+-rw-rw-r--   0 varun     (1001) varun     (1001)     9375 2023-06-17 17:51:22.000000 kp_compression-0.2.6/kp_compression/myfunctions.py
+drwxrwxr-x   0 varun     (1001) varun     (1001)        0 2023-06-17 17:55:13.884858 kp_compression-0.2.6/kp_compression.egg-info/
+-rw-rw-r--   0 varun     (1001) varun     (1001)      248 2023-06-17 17:55:13.000000 kp_compression-0.2.6/kp_compression.egg-info/PKG-INFO
+-rw-rw-r--   0 varun     (1001) varun     (1001)      264 2023-06-17 17:55:13.000000 kp_compression-0.2.6/kp_compression.egg-info/SOURCES.txt
+-rw-rw-r--   0 varun     (1001) varun     (1001)        1 2023-06-17 17:55:13.000000 kp_compression-0.2.6/kp_compression.egg-info/dependency_links.txt
+-rw-rw-r--   0 varun     (1001) varun     (1001)       12 2023-06-17 17:55:13.000000 kp_compression-0.2.6/kp_compression.egg-info/requires.txt
+-rw-rw-r--   0 varun     (1001) varun     (1001)       15 2023-06-17 17:55:13.000000 kp_compression-0.2.6/kp_compression.egg-info/top_level.txt
+-rw-rw-r--   0 varun     (1001) varun     (1001)       38 2023-06-17 17:55:13.884858 kp_compression-0.2.6/setup.cfg
+-rw-rw-r--   0 varun     (1001) varun     (1001)      349 2023-06-17 17:51:34.000000 kp_compression-0.2.6/setup.py
```

### Comparing `kp_compression-0.2.5/kp_compression/myfunctions.py` & `kp_compression-0.2.6/kp_compression/myfunctions.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
       Atilde = np.vstack([block.ravel() for blockcol in blocks
                                         for block in blockcol])
       #print("~")
       U, s, V = np.linalg.svd(Atilde)
       #print("2")
       Cshape = A.shape[0] // Bshape[0], A.shape[1] // Bshape[1]
       idx = np.argmax(s)
-      B = np.sqrt(s[idx]) * U[:,idx].reshape(Bshape)
+      B = np.sqrt(s[idx]) * U[:,idx].reshape((Bshape[1],Bshape[0])).T
       C = np.sqrt(s[idx]) * V[idx,:].reshape(Cshape)
       return B, C
 
     def init_weights(self,om, input_sz, hidden_sz, factor):
       for i in range(self.layer):
         x = getattr(om,'weight_ih_l{}'.format(i))
         x = x.detach().cpu().numpy()
```

