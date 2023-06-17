# Comparing `tmp/utnamgeo-0.0.1.tar.gz` & `tmp/utnamgeo-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utnamgeo-0.0.1.tar", last modified: Fri Jun 16 15:03:39 2023, max compression
+gzip compressed data, was "utnamgeo-0.0.2.tar", last modified: Sat Jun 17 06:11:15 2023, max compression
```

## Comparing `utnamgeo-0.0.1.tar` & `utnamgeo-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwx------   0 kali     (10549) kali     (10549)        0 2023-06-16 15:03:39.339638 utnamgeo-0.0.1/
--rw-------   0 kali     (10549) kali     (10549)       76 2023-06-16 11:23:11.000000 utnamgeo-0.0.1/CHANGELOG.txt
--rw-------   0 kali     (10549) kali     (10549)     1052 2023-06-06 10:53:43.000000 utnamgeo-0.0.1/LICENCE.txt
--rw-------   0 kali     (10549) kali     (10549)       30 2023-06-16 14:20:50.000000 utnamgeo-0.0.1/MANIFEST.in
--rw-------   0 kali     (10549) kali     (10549)     2334 2023-06-16 15:03:39.339638 utnamgeo-0.0.1/PKG-INFO
--rw-------   0 kali     (10549) kali     (10549)     1580 2023-06-16 15:03:32.000000 utnamgeo-0.0.1/README.md
--rw-------   0 kali     (10549) kali     (10549)       15 2023-06-16 11:20:25.000000 utnamgeo-0.0.1/requirements.txt
--rw-------   0 kali     (10549) kali     (10549)       38 2023-06-16 15:03:39.339638 utnamgeo-0.0.1/setup.cfg
--rw-------   0 kali     (10549) kali     (10549)      879 2023-06-16 15:02:28.000000 utnamgeo-0.0.1/setup.py
-drwx------   0 kali     (10549) kali     (10549)        0 2023-06-16 15:03:39.303638 utnamgeo-0.0.1/utnamgeo/
--rw-------   0 kali     (10549) kali     (10549)    30612 2023-06-16 13:10:07.000000 utnamgeo-0.0.1/utnamgeo/__init__.py
-drwx------   0 kali     (10549) kali     (10549)        0 2023-06-16 15:03:39.327638 utnamgeo-0.0.1/utnamgeo.egg-info/
--rw-------   0 kali     (10549) kali     (10549)     2334 2023-06-16 15:03:38.000000 utnamgeo-0.0.1/utnamgeo.egg-info/PKG-INFO
--rw-------   0 kali     (10549) kali     (10549)      222 2023-06-16 15:03:38.000000 utnamgeo-0.0.1/utnamgeo.egg-info/SOURCES.txt
--rw-------   0 kali     (10549) kali     (10549)        1 2023-06-16 15:03:38.000000 utnamgeo-0.0.1/utnamgeo.egg-info/dependency_links.txt
--rw-------   0 kali     (10549) kali     (10549)        9 2023-06-16 15:03:38.000000 utnamgeo-0.0.1/utnamgeo.egg-info/top_level.txt
+drwx------   0 kali     (10549) kali     (10549)        0 2023-06-17 06:11:15.473799 utnamgeo-0.0.2/
+-rw-------   0 kali     (10549) kali     (10549)      139 2023-06-17 06:00:59.000000 utnamgeo-0.0.2/CHANGELOG.txt
+-rw-------   0 kali     (10549) kali     (10549)     1052 2023-06-06 10:53:43.000000 utnamgeo-0.0.2/LICENCE.txt
+-rw-------   0 kali     (10549) kali     (10549)       30 2023-06-16 14:20:50.000000 utnamgeo-0.0.2/MANIFEST.in
+-rw-------   0 kali     (10549) kali     (10549)     6352 2023-06-17 06:11:15.469799 utnamgeo-0.0.2/PKG-INFO
+-rw-------   0 kali     (10549) kali     (10549)     5532 2023-06-17 06:10:26.000000 utnamgeo-0.0.2/README.md
+-rw-------   0 kali     (10549) kali     (10549)       15 2023-06-16 11:20:25.000000 utnamgeo-0.0.2/requirements.txt
+-rw-------   0 kali     (10549) kali     (10549)       38 2023-06-17 06:11:15.473799 utnamgeo-0.0.2/setup.cfg
+-rw-------   0 kali     (10549) kali     (10549)      882 2023-06-16 15:23:25.000000 utnamgeo-0.0.2/setup.py
+drwx------   0 kali     (10549) kali     (10549)        0 2023-06-17 06:11:15.437799 utnamgeo-0.0.2/utnamgeo/
+-rw-------   0 kali     (10549) kali     (10549)    30642 2023-06-17 05:59:33.000000 utnamgeo-0.0.2/utnamgeo/__init__.py
+drwx------   0 kali     (10549) kali     (10549)        0 2023-06-17 06:11:15.465799 utnamgeo-0.0.2/utnamgeo.egg-info/
+-rw-------   0 kali     (10549) kali     (10549)     6352 2023-06-17 06:11:14.000000 utnamgeo-0.0.2/utnamgeo.egg-info/PKG-INFO
+-rw-------   0 kali     (10549) kali     (10549)      222 2023-06-17 06:11:15.000000 utnamgeo-0.0.2/utnamgeo.egg-info/SOURCES.txt
+-rw-------   0 kali     (10549) kali     (10549)        1 2023-06-17 06:11:14.000000 utnamgeo-0.0.2/utnamgeo.egg-info/dependency_links.txt
+-rw-------   0 kali     (10549) kali     (10549)        9 2023-06-17 06:11:14.000000 utnamgeo-0.0.2/utnamgeo.egg-info/top_level.txt
```

### Comparing `utnamgeo-0.0.1/LICENCE.txt` & `utnamgeo-0.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `utnamgeo-0.0.1/setup.py` & `utnamgeo-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 2.7',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='utnamgeo',
-    version='0.0.1',
+    version='0.0.2',
     description='Python library for 2d/3d coordinate geometry',
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
     long_description_content_type ='text/markdown',
-    url='https://github.com/utkarsh-naman/cogeo',
+    url='https://github.com/utkarsh-naman/utnamgeo',
     author='Utkarsh Naman',
     author_email='its.utnam@gmail.com',
     license='MIT',
     classifiers=classifiers,
     keywords='cogeo geometry coordinate-geometry math evaluate calculate',
     packages=find_packages(),
     install_requires=['']
```

### Comparing `utnamgeo-0.0.1/utnamgeo/__init__.py` & `utnamgeo-0.0.2/utnamgeo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,17 @@
     y2 = eval(tte(y2))
     y3 = eval(tte(y3))
 
     z1 = eval(tte(z1))
     z2 = eval(tte(z2))
     z3 = eval(tte(z3))
 
-    if x1 * (y2 * z3 - y3 * z2) - y1 * (x2 * z3 - x3 * z2) + z1 * (x2 * y3 - x3 * y2) == 0:
+    if (x1-x2)*(y2-y3) == (x2-x3)*(y1-y2) and (y1-y2)*(z2-z3) == (y2-y3)*(z1-z2) and (x1-x2)*(z2-z3) == (x2-x3)*(z1-z2):
         return True
+
     else:
         return False
 
 
 def iscollinear(x1, x2, x3, y1, y2, y3):
     x1 = eval(tte(x1))
     x2 = eval(tte(x2))
```

