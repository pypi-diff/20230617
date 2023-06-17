# Comparing `tmp/gascompressibility-0.1.0.tar.gz` & `tmp/gascompressibility-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gascompressibility-0.1.0.tar", last modified: Sun Jun 11 20:32:19 2023, max compression
+gzip compressed data, was "gascompressibility-0.1.1.tar", last modified: Sat Jun 17 04:36:11 2023, max compression
```

## Comparing `gascompressibility-0.1.0.tar` & `gascompressibility-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 20:32:19.744045 gascompressibility-0.1.0/
--rw-rw-rw-   0        0        0     1095 2023-05-23 14:19:22.000000 gascompressibility-0.1.0/LICENSE
--rw-rw-rw-   0        0        0    11089 2023-06-11 20:32:19.743045 gascompressibility-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    10113 2023-06-11 01:23:44.000000 gascompressibility-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 20:32:19.720999 gascompressibility-0.1.0/gascompressibility/
--rw-rw-rw-   0        0        0      220 2023-06-10 23:57:14.000000 gascompressibility-0.1.0/gascompressibility/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 20:32:19.734998 gascompressibility-0.1.0/gascompressibility/pseudocritical/
--rw-rw-rw-   0        0        0        0 2023-05-31 21:11:20.000000 gascompressibility-0.1.0/gascompressibility/pseudocritical/__init__.py
--rw-rw-rw-   0        0        0    14812 2023-06-11 01:43:49.000000 gascompressibility-0.1.0/gascompressibility/pseudocritical/piper.py
--rw-rw-rw-   0        0        0    16380 2023-06-11 01:47:21.000000 gascompressibility-0.1.0/gascompressibility/pseudocritical/sutton.py
-drwxrwxrwx   0        0        0        0 2023-06-11 20:32:19.736998 gascompressibility-0.1.0/gascompressibility/utilities/
--rw-rw-rw-   0        0        0        0 2023-05-31 21:10:39.000000 gascompressibility-0.1.0/gascompressibility/utilities/__init__.py
--rw-rw-rw-   0        0        0      162 2023-06-06 18:54:16.000000 gascompressibility-0.1.0/gascompressibility/utilities/utilities.py
-drwxrwxrwx   0        0        0        0 2023-06-11 20:32:19.741043 gascompressibility-0.1.0/gascompressibility/z_correlation/
--rw-rw-rw-   0        0        0     1088 2023-06-11 02:01:39.000000 gascompressibility-0.1.0/gascompressibility/z_correlation/DAK.py
--rw-rw-rw-   0        0        0        0 2023-06-10 02:22:58.000000 gascompressibility-0.1.0/gascompressibility/z_correlation/__init__.py
--rw-rw-rw-   0        0        0      746 2023-06-11 02:05:15.000000 gascompressibility-0.1.0/gascompressibility/z_correlation/hall_yarborough.py
--rw-rw-rw-   0        0        0     1871 2023-06-11 04:54:16.000000 gascompressibility-0.1.0/gascompressibility/z_correlation/kareem.py
--rw-rw-rw-   0        0        0     1195 2023-06-11 03:43:15.000000 gascompressibility-0.1.0/gascompressibility/z_correlation/londono.py
--rw-rw-rw-   0        0        0     1463 2023-06-11 05:13:08.000000 gascompressibility-0.1.0/gascompressibility/z_correlation/z_helper.py
--rw-rw-rw-   0        0        0    24973 2023-05-31 14:14:57.000000 gascompressibility-0.1.0/gascompressibility/zfactor.py
-drwxrwxrwx   0        0        0        0 2023-06-11 20:32:19.732999 gascompressibility-0.1.0/gascompressibility.egg-info/
--rw-rw-rw-   0        0        0    11089 2023-06-11 20:32:19.000000 gascompressibility-0.1.0/gascompressibility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      821 2023-06-11 20:32:19.000000 gascompressibility-0.1.0/gascompressibility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 20:32:19.000000 gascompressibility-0.1.0/gascompressibility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-11 20:32:19.000000 gascompressibility-0.1.0/gascompressibility.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-11 20:32:19.000000 gascompressibility-0.1.0/gascompressibility.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 20:32:19.744045 gascompressibility-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1418 2023-06-11 20:32:09.000000 gascompressibility-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 20:32:19.743045 gascompressibility-0.1.0/tests/
--rw-rw-rw-   0        0        0      137 2023-06-10 01:30:30.000000 gascompressibility-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0    32341 2023-06-11 05:14:37.000000 gascompressibility-0.1.0/tests/test_gascomp.py
+drwxrwxrwx   0        0        0        0 2023-06-17 04:36:11.097356 gascompressibility-0.1.1/
+-rw-rw-rw-   0        0        0     1095 2023-05-23 14:19:22.000000 gascompressibility-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0    11101 2023-06-17 04:36:11.097356 gascompressibility-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10123 2023-06-11 23:32:19.000000 gascompressibility-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 04:36:11.042840 gascompressibility-0.1.1/gascompressibility/
+-rw-rw-rw-   0        0        0      220 2023-06-10 23:57:14.000000 gascompressibility-0.1.1/gascompressibility/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 04:36:11.065356 gascompressibility-0.1.1/gascompressibility/pseudocritical/
+-rw-rw-rw-   0        0        0        0 2023-05-31 21:11:20.000000 gascompressibility-0.1.1/gascompressibility/pseudocritical/__init__.py
+-rw-rw-rw-   0        0        0    14942 2023-06-17 04:32:50.000000 gascompressibility-0.1.1/gascompressibility/pseudocritical/piper.py
+-rw-rw-rw-   0        0        0    16503 2023-06-17 04:32:50.000000 gascompressibility-0.1.1/gascompressibility/pseudocritical/sutton.py
+drwxrwxrwx   0        0        0        0 2023-06-17 04:36:11.066357 gascompressibility-0.1.1/gascompressibility/utilities/
+-rw-rw-rw-   0        0        0        0 2023-05-31 21:10:39.000000 gascompressibility-0.1.1/gascompressibility/utilities/__init__.py
+-rw-rw-rw-   0        0        0      317 2023-06-17 04:32:50.000000 gascompressibility-0.1.1/gascompressibility/utilities/utilities.py
+drwxrwxrwx   0        0        0        0 2023-06-17 04:36:11.094356 gascompressibility-0.1.1/gascompressibility/z_correlation/
+-rw-rw-rw-   0        0        0     1088 2023-06-11 02:01:39.000000 gascompressibility-0.1.1/gascompressibility/z_correlation/DAK.py
+-rw-rw-rw-   0        0        0        0 2023-06-10 02:22:58.000000 gascompressibility-0.1.1/gascompressibility/z_correlation/__init__.py
+-rw-rw-rw-   0        0        0      746 2023-06-11 02:05:15.000000 gascompressibility-0.1.1/gascompressibility/z_correlation/hall_yarborough.py
+-rw-rw-rw-   0        0        0     1871 2023-06-11 04:54:16.000000 gascompressibility-0.1.1/gascompressibility/z_correlation/kareem.py
+-rw-rw-rw-   0        0        0     1195 2023-06-11 03:43:15.000000 gascompressibility-0.1.1/gascompressibility/z_correlation/londono.py
+-rw-rw-rw-   0        0        0     1463 2023-06-11 05:13:08.000000 gascompressibility-0.1.1/gascompressibility/z_correlation/z_helper.py
+-rw-rw-rw-   0        0        0    24973 2023-05-31 14:14:57.000000 gascompressibility-0.1.1/gascompressibility/zfactor.py
+drwxrwxrwx   0        0        0        0 2023-06-17 04:36:11.062358 gascompressibility-0.1.1/gascompressibility.egg-info/
+-rw-rw-rw-   0        0        0    11101 2023-06-17 04:36:10.000000 gascompressibility-0.1.1/gascompressibility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      821 2023-06-17 04:36:10.000000 gascompressibility-0.1.1/gascompressibility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 04:36:10.000000 gascompressibility-0.1.1/gascompressibility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-17 04:36:10.000000 gascompressibility-0.1.1/gascompressibility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-17 04:36:10.000000 gascompressibility-0.1.1/gascompressibility.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 04:36:11.098356 gascompressibility-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1428 2023-06-17 04:36:08.000000 gascompressibility-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 04:36:11.096356 gascompressibility-0.1.1/tests/
+-rw-rw-rw-   0        0        0      137 2023-06-10 01:30:30.000000 gascompressibility-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0    32379 2023-06-17 04:35:39.000000 gascompressibility-0.1.1/tests/test_gascomp.py
```

### Comparing `gascompressibility-0.1.0/LICENSE` & `gascompressibility-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.0/PKG-INFO` & `gascompressibility-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gascompressibility
-Version: 0.1.0
+Version: 0.1.1
 Summary: GasCompressibility-py is a Python library for calculating the gas compressibility factor, Z, based on real gas law.
 Home-page: https://github.com/aegis4048/GasCompressibiltiy-py/tree/main
 Author: Eric Kim
 Author-email: aegis4048@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -100,15 +100,15 @@
 Tr            = 1.5005661019949397
 ```
 
 ### 4.2. Calculation modes
 
 The package currently supports 2 ways to compute pseudo-critical properties:
 
-* `zfactor(mode='sutton)` : Sutton's gas specific gravity correlation<sup>[[1]](#ref-1)</sup> and DAK correction for $`H_{2}S`$ and $`CO_{2}`$ fractions<sup>[[2]](#ref-2)</sup> (default mode)
+* `zfactor(mode='sutton)` : Sutton's gas specific gravity correlation<sup>[[1]](#ref-1)</sup> and Wichert-Aziz correction for $`H_{2}S`$ and $`CO_{2}`$ fractions<sup>[[2]](#ref-2)</sup> (default mode)
 
 * `zfactor(mode='piper')` : Piper's gas specific gravity correlation for naturally occuring petroleum gases with  $`H_{2}S`$, $`CO_{2}`$ and $`N_{2}`$ fractions<sup>[[3]](#ref-3)</sup>
 
 These two modes can be specified with the keyward argument `mode=` when instantiating the class object `zfactor()`.
 
 ```python
 z_obj_sutton = gascomp.zfactor('sutton')  # mode='sutton', default
@@ -219,7 +219,8 @@
 8. Congrats! Installation is finished
 9. Type `(base) C:\Users\EricKim>Jupyter Notebook` and try the package on Jupyter Notebook.
 
 # Work in Progress
 Currently working on
 * Making documentations
 * Theory exlanations
+d
```

### Comparing `gascompressibility-0.1.0/README.md` & `gascompressibility-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 Tr            = 1.5005661019949397
 ```
 
 ### 4.2. Calculation modes
 
 The package currently supports 2 ways to compute pseudo-critical properties:
 
-* `zfactor(mode='sutton)` : Sutton's gas specific gravity correlation<sup>[[1]](#ref-1)</sup> and DAK correction for $`H_{2}S`$ and $`CO_{2}`$ fractions<sup>[[2]](#ref-2)</sup> (default mode)
+* `zfactor(mode='sutton)` : Sutton's gas specific gravity correlation<sup>[[1]](#ref-1)</sup> and Wichert-Aziz correction for $`H_{2}S`$ and $`CO_{2}`$ fractions<sup>[[2]](#ref-2)</sup> (default mode)
 
 * `zfactor(mode='piper')` : Piper's gas specific gravity correlation for naturally occuring petroleum gases with  $`H_{2}S`$, $`CO_{2}`$ and $`N_{2}`$ fractions<sup>[[3]](#ref-3)</sup>
 
 These two modes can be specified with the keyward argument `mode=` when instantiating the class object `zfactor()`.
 
 ```python
 z_obj_sutton = gascomp.zfactor('sutton')  # mode='sutton', default
@@ -197,7 +197,8 @@
 8. Congrats! Installation is finished
 9. Type `(base) C:\Users\EricKim>Jupyter Notebook` and try the package on Jupyter Notebook.
 
 # Work in Progress
 Currently working on
 * Making documentations
 * Theory exlanations
+d
```

### Comparing `gascompressibility-0.1.0/gascompressibility/pseudocritical/piper.py` & `gascompressibility-0.1.1/gascompressibility/pseudocritical/piper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 from scipy import optimize
 import matplotlib.pyplot as plt
 import inspect
 
 from gascompressibility.utilities.utilities import calc_Fahrenheit_to_Rankine
+from gascompressibility.utilities.utilities import calc_psig_to_psia
 from gascompressibility.z_correlation.z_helper import get_z_model
 
 
 class piper(object):
     def __init__(
             self,
             Pc_H2S=1306,
@@ -199,23 +200,24 @@
                                 "Either both Tpc and Ppc must be inputted, or only sg needs to be inputted. "
                                 "Both Tpc and Ppc can be computed from sg")
         else:
             self.sg = sg
 
     def _initialize_P(self, P):
         if P is None:
-            raise TypeError("Missing a required argument, P (gas pressure, psia)")
+            raise TypeError("Missing a required argument, P (gas pressure, psig)")
         else:
-            self.P = P
+            self.P_a = P  # psia
+            self.P = calc_psig_to_psia(P)
 
     def _initialize_T(self, T):
         if T is None:
             raise TypeError("Missing a required argument, T (gas temperature, °F)")
         else:
-            self.T_f = T
+            self.T_f = T  # °F
             self.T = calc_Fahrenheit_to_Rankine(T)
 
     def _initialize_H2S(self, H2S):
         if H2S is None:
             self.H2S = 0
         else:
             self.H2S = H2S
```

### Comparing `gascompressibility-0.1.0/gascompressibility/pseudocritical/sutton.py` & `gascompressibility-0.1.1/gascompressibility/pseudocritical/sutton.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 from scipy import optimize
 import matplotlib.pyplot as plt
 import inspect
 
 from gascompressibility.utilities.utilities import calc_Fahrenheit_to_Rankine
+from gascompressibility.utilities.utilities import calc_psig_to_psia
 from gascompressibility.z_correlation.z_helper import get_z_model
 
 
 class sutton:
     def __init__(self):
         self.mode = 'sutton'
         self._check_invalid_mode(self.mode)  # prevent user modification of self.mode
@@ -200,17 +201,18 @@
                                 "Either both Tpc and Ppc must be inputted, or only sg needs to be inputted. "
                                 "Both Tpc and Ppc can be computed from sg")
         else:
             self.sg = sg
 
     def _initialize_P(self, P):
         if P is None:
-            raise TypeError("Missing a required argument, P (gas pressure, psia)")
+            raise TypeError("Missing a required argument, P (gas pressure, psig)")
         else:
-            self.P = P
+            self.P_a = P  # psia
+            self.P = calc_psig_to_psia(P)
 
     def _initialize_T(self, T):
         if T is None:
             raise TypeError("Missing a required argument, T (gas temperature, °F)")
         else:
             self.T_f = T
             self.T = calc_Fahrenheit_to_Rankine(T)
```

### Comparing `gascompressibility-0.1.0/gascompressibility/z_correlation/DAK.py` & `gascompressibility-0.1.1/gascompressibility/z_correlation/DAK.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.0/gascompressibility/z_correlation/hall_yarborough.py` & `gascompressibility-0.1.1/gascompressibility/z_correlation/hall_yarborough.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.0/gascompressibility/z_correlation/kareem.py` & `gascompressibility-0.1.1/gascompressibility/z_correlation/kareem.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.0/gascompressibility/z_correlation/londono.py` & `gascompressibility-0.1.1/gascompressibility/z_correlation/londono.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.0/gascompressibility/z_correlation/z_helper.py` & `gascompressibility-0.1.1/gascompressibility/z_correlation/z_helper.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.0/gascompressibility/zfactor.py` & `gascompressibility-0.1.1/gascompressibility/zfactor.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.0/gascompressibility.egg-info/PKG-INFO` & `gascompressibility-0.1.1/gascompressibility.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gascompressibility
-Version: 0.1.0
+Version: 0.1.1
 Summary: GasCompressibility-py is a Python library for calculating the gas compressibility factor, Z, based on real gas law.
 Home-page: https://github.com/aegis4048/GasCompressibiltiy-py/tree/main
 Author: Eric Kim
 Author-email: aegis4048@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -100,15 +100,15 @@
 Tr            = 1.5005661019949397
 ```
 
 ### 4.2. Calculation modes
 
 The package currently supports 2 ways to compute pseudo-critical properties:
 
-* `zfactor(mode='sutton)` : Sutton's gas specific gravity correlation<sup>[[1]](#ref-1)</sup> and DAK correction for $`H_{2}S`$ and $`CO_{2}`$ fractions<sup>[[2]](#ref-2)</sup> (default mode)
+* `zfactor(mode='sutton)` : Sutton's gas specific gravity correlation<sup>[[1]](#ref-1)</sup> and Wichert-Aziz correction for $`H_{2}S`$ and $`CO_{2}`$ fractions<sup>[[2]](#ref-2)</sup> (default mode)
 
 * `zfactor(mode='piper')` : Piper's gas specific gravity correlation for naturally occuring petroleum gases with  $`H_{2}S`$, $`CO_{2}`$ and $`N_{2}`$ fractions<sup>[[3]](#ref-3)</sup>
 
 These two modes can be specified with the keyward argument `mode=` when instantiating the class object `zfactor()`.
 
 ```python
 z_obj_sutton = gascomp.zfactor('sutton')  # mode='sutton', default
@@ -219,7 +219,8 @@
 8. Congrats! Installation is finished
 9. Type `(base) C:\Users\EricKim>Jupyter Notebook` and try the package on Jupyter Notebook.
 
 # Work in Progress
 Currently working on
 * Making documentations
 * Theory exlanations
+d
```

### Comparing `gascompressibility-0.1.0/gascompressibility.egg-info/SOURCES.txt` & `gascompressibility-0.1.1/gascompressibility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.1.0/setup.py` & `gascompressibility-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def classifiers():
     with open('classifiers.txt') as f:
         return f.read().strip().split('\n')
 
 
 setup(
     name='gascompressibility',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(exclude=[
         "tutorials",
         "LICENSE",
         ".gitignore",
         "README.md",
         "misc",
         ".travis.yml",
@@ -47,10 +47,10 @@
         'matplotlib>=3.5.1',
     ],
     url='https://github.com/aegis4048/GasCompressibiltiy-py/tree/main',
 )
 
 
 # python setup.py sdist bdist_wheel
-# twine upload --skip-existing dist/*
+# python -m twine upload --skip-existing dist/*
 
 # python -m twine upload --skip-existing --repository testpypi dist/*
```

### Comparing `gascompressibility-0.1.0/tests/test_gascomp.py` & `gascompressibility-0.1.1/tests/test_gascomp.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 import sys
 
 sys.path.append('.')
 from gascompressibility import sutton
 from gascompressibility import piper
 from gascompressibility import calc_Z
 
+# Documents\GasCompressibiltiyFactor-py>python -m unittest tests.test_gascomp
+# python -m unittest discover .
+
 """ Test print script
 def tround(a, n):
     if a is not None:
         return round(a, n)
     return None  
 n = 4
 
@@ -418,117 +421,117 @@
         self.assertAlmostEqual(instance.T, 534.67, places=3)
         self.assertAlmostEqual(instance.Tr, 1.4311, places=3)
 
         print('calc_Tr passed (mode="piper")')
 
     def test_calc_Pr(self):
         instance = sutton()
-        result = instance.calc_Pr(sg=0.7, P=2010, H2S=0.07, CO2=0.1)
+        result = instance.calc_Pr(sg=0.7, P=1995.3, H2S=0.07, CO2=0.1)
         self.assertEqual(instance.sg, 0.7)
         self.assertEqual(instance.P, 2010)
         self.assertEqual(instance.H2S, 0.07)
         self.assertEqual(instance.CO2, 0.1)
         self.assertAlmostEqual(result, 3.1995, places=3)
         self.assertAlmostEqual(instance.P, 2010, places=3)
         self.assertAlmostEqual(instance.e_correction, 21.2778, places=3)
         self.assertAlmostEqual(instance.Ppc_corrected, 628.2143, places=3)
         self.assertAlmostEqual(instance.Tpc_corrected, 356.3122, places=3)
         self.assertAlmostEqual(instance.Ppc, 663.287, places=3)
         self.assertAlmostEqual(instance.Tpc, 377.59, places=3)
         self.assertAlmostEqual(instance.Pr, 3.1995, places=3)
 
         instance = sutton()
-        result = instance.calc_Pr(Ppc=663.29, Tpc=377.59, P=2010, H2S=0.07, CO2=0.1)
+        result = instance.calc_Pr(Ppc=663.29, Tpc=377.59, P=1995.3, H2S=0.07, CO2=0.1)
         self.assertEqual(instance.Ppc, 663.29)
         self.assertEqual(instance.Tpc, 377.59)
         self.assertEqual(instance.P, 2010)
         self.assertEqual(instance.H2S, 0.07)
         self.assertEqual(instance.CO2, 0.1)
         self.assertAlmostEqual(result, 3.1995, places=3)
         self.assertAlmostEqual(instance.P, 2010, places=3)
         self.assertAlmostEqual(instance.e_correction, 21.2778, places=3)
         self.assertAlmostEqual(instance.Ppc_corrected, 628.2171, places=3)
         self.assertAlmostEqual(instance.Tpc_corrected, 356.3122, places=3)
         self.assertAlmostEqual(instance.Pr, 3.1995, places=3)
 
         instance = sutton()
-        result = instance.calc_Pr(Ppc_corrected=628.21, P=2010)
+        result = instance.calc_Pr(Ppc_corrected=628.21, P=1995.3)
         self.assertEqual(instance.Ppc_corrected, 628.21)
         self.assertEqual(instance.P, 2010)
         self.assertAlmostEqual(result, 3.1995, places=3)
         self.assertAlmostEqual(instance.Pr, 3.1996, places=3)
 
         instance = sutton()
-        result = instance.calc_Pr(Ppc=663.29, P=2010, e_correction=21.278, H2S=0.07, Tpc=377.59, ignore_conflict=True)
+        result = instance.calc_Pr(Ppc=663.29, P=1995.3, e_correction=21.278, H2S=0.07, Tpc=377.59, ignore_conflict=True)
         self.assertEqual(instance.Ppc, 663.29)
         self.assertEqual(instance.P, 2010)
         self.assertEqual(instance.e_correction, 21.278)
         self.assertEqual(instance.H2S, 0.07)
         self.assertEqual(instance.Tpc, 377.59)
         self.assertAlmostEqual(result, 3.1995, places=3)
         self.assertAlmostEqual(instance.Ppc_corrected, 628.2168, places=3)
         self.assertAlmostEqual(instance.Tpc_corrected, 356.312, places=3)
         self.assertAlmostEqual(instance.Pr, 3.1995, places=3)
 
         print('calc_Pr passed (mode="sutton")')
 
         instance = piper()
-        result = instance.calc_Pr(Tpc=373.6, sg=0.7, P=2010, H2S=0.07, CO2=0.1)
+        result = instance.calc_Pr(Tpc=373.6, sg=0.7, P=1995.3, H2S=0.07, CO2=0.1)
         self.assertEqual(instance.Tpc, 373.6)
         self.assertEqual(instance.sg, 0.7)
         self.assertEqual(instance.P, 2010)
         self.assertEqual(instance.H2S, 0.07)
         self.assertEqual(instance.CO2, 0.1)
         self.assertAlmostEqual(result, 2.6874, places=3)
         self.assertAlmostEqual(instance.J, 0.4995, places=3)
         self.assertAlmostEqual(instance.Ppc, 747.9162, places=3)
         self.assertAlmostEqual(instance.Pr, 2.6875, places=3)
 
         instance = piper()
-        result = instance.calc_Pr(Ppc=747.9, P=2010)
+        result = instance.calc_Pr(Ppc=747.9, P=1995.3)
         self.assertEqual(instance.Ppc, 747.9)
         self.assertEqual(instance.P, 2010)
         self.assertAlmostEqual(result, 2.6875, places=3)
         self.assertAlmostEqual(instance.Pr, 2.6875, places=3)
 
         instance = piper()
-        result = instance.calc_Pr(P=2010, K=4, J=2)
+        result = instance.calc_Pr(P=1995.3, K=4, J=2)
         self.assertEqual(instance.K, 4)
         self.assertEqual(instance.J, 2)
         self.assertEqual(instance.P, 2010)
         self.assertAlmostEqual(result, 502.5, places=1)
         self.assertAlmostEqual(instance.Ppc, 4.0, places=3)
         self.assertAlmostEqual(instance.Tpc, 8.0, places=3)
         self.assertAlmostEqual(instance.Pr, 502.5, places=3)
 
         instance = piper()
-        result = instance.calc_Pr(P=2010, sg=2)
+        result = instance.calc_Pr(P=1995.3, sg=2)
         self.assertEqual(instance.sg, 2)
         self.assertEqual(instance.P, 2010)
         self.assertAlmostEqual(result, 3.8686, places=3)
         self.assertAlmostEqual(instance.J, 1.1328, places=3)
         self.assertAlmostEqual(instance.K, 25.8212, places=3)
         self.assertAlmostEqual(instance.Ppc, 519.5617, places=3)
         self.assertAlmostEqual(instance.Tpc, 588.5658, places=3)
         self.assertAlmostEqual(instance.Pr, 3.8686, places=3)
 
         instance = piper()
-        result = instance.calc_Pr(P=2010, Tpc=373.6, J=0.4995)
+        result = instance.calc_Pr(P=1995.3, Tpc=373.6, J=0.4995)
         self.assertEqual(instance.Tpc, 373.6)
         self.assertEqual(instance.J, 0.4995)
         self.assertEqual(instance.P, 2010)
         self.assertAlmostEqual(result, 2.6873, places=3)
         self.assertAlmostEqual(instance.Ppc, 747.9479, places=3)
         self.assertAlmostEqual(instance.Pr, 2.6874, places=3)
 
         print('calc_Pr passed (mode="piper")')
 
     def test_calc_Z(self):
         instance = sutton()
-        result = instance.calc_Z(P=2010, T=75, CO2=0.1, H2S=0.07, sg=0.7)
+        result = instance.calc_Z(P=1995.3, T=75, CO2=0.1, H2S=0.07, sg=0.7)
         self.assertEqual(instance.P, 2010)
         self.assertEqual(instance.T_f, 75)
         self.assertEqual(instance.CO2, 0.1)
         self.assertEqual(instance.H2S, 0.07)
         self.assertEqual(instance.sg, 0.7)
         self.assertAlmostEqual(result, 0.7730, places=3)
         self.assertAlmostEqual(instance.T, 534.67, places=3)
@@ -538,15 +541,15 @@
         self.assertAlmostEqual(instance.Ppc, 663.287, places=3)
         self.assertAlmostEqual(instance.Tpc, 377.59, places=3)
         self.assertAlmostEqual(instance.Pr, 3.1995, places=3)
         self.assertAlmostEqual(instance.Tr, 1.5006, places=3)
         self.assertAlmostEqual(instance.Z, 0.7731, places=3)
 
         instance = sutton()
-        result = instance.calc_Z(P=2010, T=75, Ppc=747.9, Tpc=373.6)
+        result = instance.calc_Z(P=1995.3, T=75, Ppc=747.9, Tpc=373.6)
         self.assertEqual(instance.P, 2010)
         self.assertEqual(instance.T_f, 75)
         self.assertEqual(instance.Ppc, 747.9)
         self.assertEqual(instance.Tpc, 373.6)
         self.assertAlmostEqual(result, 0.7418, places=3)
         self.assertAlmostEqual(instance.T, 534.67, places=3)
         self.assertAlmostEqual(instance.e_correction, 0.0, places=3)
@@ -565,15 +568,15 @@
         self.assertAlmostEqual(result, 0.7730, places=3)
         self.assertAlmostEqual(instance.T, 534.67, places=3)
         self.assertAlmostEqual(instance.Tpc_corrected, 356.312, places=3)
         self.assertAlmostEqual(instance.Tr, 1.5006, places=3)
         self.assertAlmostEqual(instance.Z, 0.7731, places=3)
 
         instance = sutton()
-        result = instance.calc_Z(Tpc_corrected=356.31, sg=0.7, P=2010, T=75, H2S=0.07, CO2=0.1, ignore_conflict=True)
+        result = instance.calc_Z(Tpc_corrected=356.31, sg=0.7, P=1995.3, T=75, H2S=0.07, CO2=0.1, ignore_conflict=True)
         self.assertEqual(instance.P, 2010)
         self.assertEqual(instance.T_f, 75)
         self.assertEqual(instance.H2S, 0.07)
         self.assertEqual(instance.CO2, 0.1)
         self.assertEqual(instance.Tpc_corrected, 356.31)
         self.assertAlmostEqual(result, 0.7730, places=3)
         self.assertAlmostEqual(instance.T, 534.67, places=3)
@@ -584,15 +587,15 @@
         self.assertAlmostEqual(instance.Pr, 3.1996, places=3)
         self.assertAlmostEqual(instance.Tr, 1.5006, places=3)
         self.assertAlmostEqual(instance.Z, 0.7731, places=3)
 
         print('calc_Z passed (mode="sutton")')
 
         instance = piper()
-        result = instance.calc_Z(P=2010, T=75, sg=0.7, H2S=0.07, CO2=0.1, N2=0)
+        result = instance.calc_Z(P=1995.3, T=75, sg=0.7, H2S=0.07, CO2=0.1, N2=0)
         self.assertEqual(instance.P, 2010)
         self.assertEqual(instance.T_f, 75)
         self.assertEqual(instance.sg, 0.7)
         self.assertEqual(instance.H2S, 0.07)
         self.assertEqual(instance.CO2, 0.1)
         self.assertEqual(instance.N2, 0.0)
         self.assertAlmostEqual(result, 0.7418, places=3)
@@ -602,15 +605,15 @@
         self.assertAlmostEqual(instance.Ppc, 747.9468, places=3)
         self.assertAlmostEqual(instance.Tpc, 373.6153, places=3)
         self.assertAlmostEqual(instance.Pr, 2.6874, places=3)
         self.assertAlmostEqual(instance.Tr, 1.4311, places=3)
         self.assertAlmostEqual(instance.Z, 0.7418, places=3)
 
         instance = piper()
-        result = instance.calc_Z(P=2010, T=75, sg=0.7, H2S=0.07, CO2=0.1, N2=0.1)
+        result = instance.calc_Z(P=1995.3, T=75, sg=0.7, H2S=0.07, CO2=0.1, N2=0.1)
         self.assertEqual(instance.P, 2010)
         self.assertEqual(instance.T_f, 75)
         self.assertEqual(instance.sg, 0.7)
         self.assertEqual(instance.H2S, 0.07)
         self.assertEqual(instance.CO2, 0.1)
         self.assertEqual(instance.N2, 0.1)
         self.assertAlmostEqual(result, 0.8093, places=3)
@@ -620,29 +623,29 @@
         self.assertAlmostEqual(instance.Ppc, 736.2064, places=3)
         self.assertAlmostEqual(instance.Tpc, 345.3259, places=3)
         self.assertAlmostEqual(instance.Pr, 2.7302, places=3)
         self.assertAlmostEqual(instance.Tr, 1.5483, places=3)
         self.assertAlmostEqual(instance.Z, 0.8093, places=3)
 
         instance = piper()
-        result = instance.calc_Z(P=2010, T=75, K=13.661, J=0.4995)
+        result = instance.calc_Z(P=1995.3, T=75, K=13.661, J=0.4995)
         self.assertEqual(instance.P, 2010)
         self.assertEqual(instance.T_f, 75)
         self.assertEqual(instance.K, 13.661)
         self.assertEqual(instance.J, 0.4995)
         self.assertAlmostEqual(result, 0.7418, places=3)
         self.assertAlmostEqual(instance.T, 534.67, places=3)
         self.assertAlmostEqual(instance.Ppc, 747.9869, places=3)
         self.assertAlmostEqual(instance.Tpc, 373.6195, places=3)
         self.assertAlmostEqual(instance.Pr, 2.6872, places=3)
         self.assertAlmostEqual(instance.Tr, 1.4311, places=3)
         self.assertAlmostEqual(instance.Z, 0.7418, places=3)
 
         instance = piper()
-        result = instance.calc_Z(P=2010, T=75, Tpc=373.6, J=0.4995, ignore_conflict=True)
+        result = instance.calc_Z(P=1995.3, T=75, Tpc=373.6, J=0.4995, ignore_conflict=True)
         self.assertEqual(instance.P, 2010)
         self.assertEqual(instance.T_f, 75)
         self.assertEqual(instance.Tpc, 373.6)
         self.assertEqual(instance.J, 0.4995)
         self.assertAlmostEqual(result, 0.7418, places=3)
         self.assertAlmostEqual(instance.Ppc, 747.9479, places=3)
         self.assertAlmostEqual(instance.Pr, 2.6874, places=3)
@@ -658,15 +661,15 @@
         self.assertAlmostEqual(result, 0.7418, places=3)
         self.assertAlmostEqual(instance.T, 534.67, places=3)
         self.assertAlmostEqual(instance.Tpc, 373.6195, places=3)
         self.assertAlmostEqual(instance.Tr, 1.4311, places=3)
         self.assertAlmostEqual(instance.Z, 0.7418, places=3)
 
         instance = piper()
-        result = instance.calc_Z(P=2010, T=75, Ppc=663.28, Tpc=377.59, ignore_conflict=True)
+        result = instance.calc_Z(P=1995.3, T=75, Ppc=663.28, Tpc=377.59, ignore_conflict=True)
         self.assertEqual(instance.P, 2010)
         self.assertEqual(instance.T_f, 75)
         self.assertEqual(instance.Ppc, 663.28)
         self.assertEqual(instance.Tpc, 377.59)
         self.assertAlmostEqual(result, 0.7207, places=3)
         self.assertAlmostEqual(instance.T, 534.67, places=3)
         self.assertAlmostEqual(instance.Pr, 3.0304, places=3)
@@ -696,9 +699,8 @@
 
         print('calc_Z_models passed (model="kareem")')
 
 
 if __name__ == '__main__':
     unittest.main()
 
-# Documents\GasCompressibiltiyFactor-py>python -m unittest tests.test_gascomp
-# python -m unittest discover .
+
```

