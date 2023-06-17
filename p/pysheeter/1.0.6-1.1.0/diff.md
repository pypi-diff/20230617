# Comparing `tmp/pysheeter-1.0.6.tar.gz` & `tmp/pysheeter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pysheeter-1.0.6.tar", last modified: Mon Nov 23 17:03:08 2020, max compression
+gzip compressed data, was "pysheeter-1.1.0.tar", last modified: Sat Jun 17 12:04:55 2023, max compression
```

## Comparing `pysheeter-1.0.6.tar` & `pysheeter-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2020-11-23 17:03:08.000000 pysheeter-1.0.6/
--rw-r--r--   0 victor    (1000) victor    (1000)     4129 2020-11-23 17:03:08.000000 pysheeter-1.0.6/PKG-INFO
--rw-r--r--   0 victor    (1000) victor    (1000)     2990 2020-11-23 16:48:48.000000 pysheeter-1.0.6/README.md
-drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2020-11-23 17:03:08.000000 pysheeter-1.0.6/pysheeter/
--rw-r--r--   0 victor    (1000) victor    (1000)     1719 2020-11-23 16:48:42.000000 pysheeter-1.0.6/pysheeter/PySheeter.py
--rw-r--r--   0 victor    (1000) victor    (1000)        0 2020-11-23 17:02:03.000000 pysheeter-1.0.6/pysheeter/__init__.py
-drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2020-11-23 17:03:08.000000 pysheeter-1.0.6/pysheeter.egg-info/
--rw-r--r--   0 victor    (1000) victor    (1000)     4129 2020-11-23 17:03:08.000000 pysheeter-1.0.6/pysheeter.egg-info/PKG-INFO
--rw-r--r--   0 victor    (1000) victor    (1000)      227 2020-11-23 17:03:08.000000 pysheeter-1.0.6/pysheeter.egg-info/SOURCES.txt
--rw-r--r--   0 victor    (1000) victor    (1000)        1 2020-11-23 17:03:08.000000 pysheeter-1.0.6/pysheeter.egg-info/dependency_links.txt
--rw-r--r--   0 victor    (1000) victor    (1000)        7 2020-11-23 17:03:08.000000 pysheeter-1.0.6/pysheeter.egg-info/requires.txt
--rw-r--r--   0 victor    (1000) victor    (1000)       10 2020-11-23 17:03:08.000000 pysheeter-1.0.6/pysheeter.egg-info/top_level.txt
--rw-r--r--   0 victor    (1000) victor    (1000)       38 2020-11-23 17:03:08.000000 pysheeter-1.0.6/setup.cfg
--rw-r--r--   0 victor    (1000) victor    (1000)      770 2020-11-23 17:02:27.000000 pysheeter-1.0.6/setup.py
+drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2023-06-17 12:04:55.727462 pysheeter-1.1.0/
+-rw-r--r--   0 victor    (1000) victor    (1000)      316 2023-06-17 12:04:55.727462 pysheeter-1.1.0/PKG-INFO
+-rw-r--r--   0 victor    (1000) victor    (1000)     3284 2023-06-17 10:34:43.000000 pysheeter-1.1.0/README.md
+drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2023-06-17 12:04:55.724462 pysheeter-1.1.0/pysheeter/
+-rw-r--r--   0 victor    (1000) victor    (1000)        0 2023-06-17 10:38:23.000000 pysheeter-1.1.0/pysheeter/__init__.py
+-rw-r--r--   0 victor    (1000) victor    (1000)     1759 2023-06-17 11:52:23.000000 pysheeter-1.1.0/pysheeter/pysheeter.py
+drwxr-xr-x   0 victor    (1000) victor    (1000)        0 2023-06-17 12:04:55.726462 pysheeter-1.1.0/pysheeter.egg-info/
+-rw-r--r--   0 victor    (1000) victor    (1000)      316 2023-06-17 12:04:55.000000 pysheeter-1.1.0/pysheeter.egg-info/PKG-INFO
+-rw-r--r--   0 victor    (1000) victor    (1000)      227 2023-06-17 12:04:55.000000 pysheeter-1.1.0/pysheeter.egg-info/SOURCES.txt
+-rw-r--r--   0 victor    (1000) victor    (1000)        1 2023-06-17 12:04:55.000000 pysheeter-1.1.0/pysheeter.egg-info/dependency_links.txt
+-rw-r--r--   0 victor    (1000) victor    (1000)        7 2023-06-17 12:04:55.000000 pysheeter-1.1.0/pysheeter.egg-info/requires.txt
+-rw-r--r--   0 victor    (1000) victor    (1000)       10 2023-06-17 12:04:55.000000 pysheeter-1.1.0/pysheeter.egg-info/top_level.txt
+-rw-r--r--   0 victor    (1000) victor    (1000)       38 2023-06-17 12:04:55.727462 pysheeter-1.1.0/setup.cfg
+-rw-r--r--   0 victor    (1000) victor    (1000)      474 2023-06-17 12:04:12.000000 pysheeter-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pysheeter-1.0.6/README.md` & `pysheeter-1.1.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,89 +1,93 @@
-# PySheeter
-Lightweight Pillow Python-script to create and scale sprite sheets from PNGs in folders or individually
-
-## Get started / Basic usage
-1. Download and install [Python 3](https://www.python.org/downloads/) for your architecture
-2. Install the latest version of PySheeter with [`pip3`](https://pypi.org/project/pysheeter-VicW/)
-```bash
-$ pip3 install pysheeter-VicW
-```
-### Sprite sheet from folder
-1. Import `Sheet` from `pysheeter`
-```python
-from pysheeter import Sheet
-```
-2. Initialize the class with a path to your PNG-folder
-```python
-spritesheet = pysheeter.Sheet("example/")
-```
-3. Create a sprite sheet with `put()`
-```python
-spritesheet.put("example_v1616.png",(16,16)) 
-# Creates a vertical spritesheet named 'example_v1616.png' with the dimensions 16x16px (scaled automatically)
-```
-
-__Example usage:__
-```python
-# from 'example.py'
-from pysheeter import PySheeter
-
-# Load sprites from 'example/'
-spritesheet = PySheeter.Sheet("example")
-
-# Create a vertical spritesheet with the dimensions 16x16
-spritesheet.put("example_v1616.png",(16,16))
-
-# Create a horizontal spritesheet with the dimensions 16x32
-spritesheet.put("example_h1632.png",(16,32),False)
-```
-![Example 1](https://storage.googleapis.com/public.victorwesterlund.com/github/VictorWesterlund/pysheeter/1example_v1616.png)
-![Example 2](https://storage.googleapis.com/public.victorwesterlund.com/github/VictorWesterlund/pysheeter/1example_h1632.png)
-### Sprite sheet from individual PNG-images
-1. Import `Sheet` from `pysheeter`
-```python
-from pysheeter import Sheet
-```
-2. Initialize the class without any arguments
-```python
-spritesheet = pysheeter.Sheet()
-```
-3. Add PNG-images with `add()`
-```python
-spritesheet.add("example/1.png")
-spritesheet.add("example/2.png")
-spritesheet.add("example/3.png")
-...
-```
-4. Remove PNG-images with `remove()`
-```python
-spritesheet.remove("example/2.png")
-```
-5. Create a sprite sheet with `put()`
-```python
-spritesheet.put("example_v1616.png",(16,16)) 
-# Creates a vertical spritesheet named 'example_v1616.png' with the dimensions 16x16px (scaled automatically)
-```
-
-__Example usage:__
-```python
-from pysheeter import PySheeter
-
-# Load sprites from 'example/'
-spritesheet = PySheeter.Sheet()
-
-# Add PNG-images
-spritesheet.add("example/1.png")
-spritesheet.add("example/2.png")
-spritesheet.add("example/3.png")
-spritesheet.add("example/7.png")
-spritesheet.add("example/5.png")
-spritesheet.add("example/9.png")
-
-# Create a vertical spritesheet with the dimensions 16x16
-spritesheet.put("example_v1616.png",(16,16))
-
-# Create a horizontal spritesheet with the dimensions 16x32
-spritesheet.put("example_h1632.png",(16,32),False)
-```
-![Example 1](https://storage.googleapis.com/public.victorwesterlund.com/github/VictorWesterlund/pysheeter/2example_v1616.png)
-![Example 2](https://storage.googleapis.com/public.victorwesterlund.com/github/VictorWesterlund/pysheeter/2example_h1632.png)
+# PySheeter
+![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/VictorWesterlund/pysheeter?include_prereleases)
+![GitHub last commit](https://img.shields.io/github/last-commit/VictorWesterlund/pysheeter)
+![Maintenance](https://img.shields.io/maintenance/yes/2020)
+
+Lightweight Pillow Python package to create and scale sprite sheets from individual PNGs or whole folders
+
+## Get started / Basic usage
+1. Download and install the latest version of [Python 3](https://www.python.org/downloads/) for your architecture
+2. Install the latest build of PySheeter with [`pip3`](https://pypi.org/project/pysheeter/)
+```bash
+$ python3 -m pip install pysheeter
+```
+### Sprite sheet from folder
+1. Import `Sheet` from `pysheeter`
+```python
+from pysheeter import PySheeter
+```
+2. Initialize the class with a path to your PNG-folder
+```python
+spritesheet = PySheeter.Sheet("example/")
+```
+3. Create a sprite sheet with `put()`
+```python
+spritesheet.put("example_v1616.png",(16,16)) 
+# Creates a vertical spritesheet named 'example_v1616.png' with the dimensions 16x16px (scaled automatically)
+```
+
+__Example usage:__
+```python
+# from 'example.py'
+from pysheeter import PySheeter
+
+# Load sprites from './files/' (all sprites are 64x64)
+spritesheet = PySheeter.Sheet("example")
+
+# Create a vertical spritesheet with the dimensions 16x16 (scaled)
+spritesheet.put("example_v1616.png",(16,16))
+
+# Create a horizontal spritesheet with the dimensions 16x32 (scaled & stretched)
+spritesheet.put("example_h1632.png",(16,32),False)
+```
+![Example 1](https://storage.googleapis.com/public.victorwesterlund.com/github/VictorWesterlund/pysheeter/1example_v1616.png)
+![Example 2](https://storage.googleapis.com/public.victorwesterlund.com/github/VictorWesterlund/pysheeter/1example_h1632.png)
+### Sprite sheet from individual PNG-images
+1. Import `Sheet` from `pysheeter`
+```python
+from pysheeter import PySheeter
+```
+2. Initialize the class without any arguments
+```python
+spritesheet = PySheeter.Sheet()
+```
+3. Add PNG-images with `add()`
+```python
+spritesheet.add("example/1.png")
+spritesheet.add("example/2.png")
+spritesheet.add("example/3.png")
+...
+```
+4. Remove PNG-images with `remove()`
+```python
+spritesheet.remove("example/2.png")
+```
+5. Create a sprite sheet with `put()`
+```python
+spritesheet.put("example_v1616.png",(16,16)) 
+# Creates a vertical spritesheet named 'example_v1616.png' with the dimensions 16x16px (scaled automatically)
+```
+
+__Example usage:__
+```python
+from pysheeter import PySheeter
+
+# Load sprites from 'example/'
+spritesheet = PySheeter.Sheet()
+
+# Add PNG-images
+spritesheet.add("example/1.png")
+spritesheet.add("example/2.png")
+spritesheet.add("example/3.png")
+spritesheet.add("example/7.png")
+spritesheet.add("example/5.png")
+spritesheet.add("example/9.png")
+
+# Create a vertical spritesheet with the dimensions 16x16
+spritesheet.put("example_v1616.png",(16,16))
+
+# Create a horizontal spritesheet with the dimensions 16x32
+spritesheet.put("example_h1632.png",(16,32),False)
+```
+![Example 1](https://storage.googleapis.com/public.victorwesterlund.com/github/VictorWesterlund/pysheeter/2example_v1616.png)
+![Example 2](https://storage.googleapis.com/public.victorwesterlund.com/github/VictorWesterlund/pysheeter/2example_h1632.png)
```

