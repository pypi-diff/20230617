# Comparing `tmp/astro_ghost-2.0.3.tar.gz` & `tmp/astro_ghost-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_ghost-2.0.3.tar", last modified: Sat Jun 17 15:54:06 2023, max compression
+gzip compressed data, was "astro_ghost-2.0.5.tar", last modified: Sat Jun 17 16:36:09 2023, max compression
```

## Comparing `astro_ghost-2.0.3.tar` & `astro_ghost-2.0.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 15:54:06.088340 astro_ghost-2.0.3/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 15:54:05.976252 astro_ghost-2.0.3/.github/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 15:54:05.984296 astro_ghost-2.0.3/.github/workflows/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-2.0.3/.github/workflows/docs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      587 2023-05-24 04:50:38.000000 astro_ghost-2.0.3/.github/workflows/tests.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-2.0.3/.gitignore
--rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-2.0.3/.readthedocs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-2.0.3/MANIFEST.in
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-17 15:54:06.088682 astro_ghost-2.0.3/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     3674 2023-05-24 04:49:23.000000 astro_ghost-2.0.3/README.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 15:54:06.062436 astro_ghost-2.0.3/astro_ghost/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    23314 2023-06-17 15:51:41.000000 astro_ghost-2.0.3/astro_ghost/DLR.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4668 2023-05-22 16:28:50.000000 astro_ghost-2.0.3/astro_ghost/NEDQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    38694 2023-06-06 15:46:00.000000 astro_ghost-2.0.3/astro_ghost/PS1QueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-2.0.3/astro_ghost/SimbadQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-2.0.3/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2023-05-11 05:34:31.000000 astro_ghost-2.0.3/astro_ghost/TNSQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-2.0.3/astro_ghost/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-06-17 15:52:22.000000 astro_ghost-2.0.3/astro_ghost/_version.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-2.0.3/astro_ghost/conftest.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    42487 2023-06-17 15:47:53.000000 astro_ghost-2.0.3/astro_ghost/ghostHelperFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    32887 2023-06-04 03:48:08.000000 astro_ghost-2.0.3/astro_ghost/gradientAscent.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-2.0.3/astro_ghost/hostMatching.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    17727 2023-05-22 03:39:53.000000 astro_ghost-2.0.3/astro_ghost/photoz_helper.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     9853 2023-06-06 16:38:06.000000 astro_ghost-2.0.3/astro_ghost/sourceCleaning.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     7737 2023-05-24 04:44:13.000000 astro_ghost-2.0.3/astro_ghost/starSeparation.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4610 2023-05-24 04:43:14.000000 astro_ghost-2.0.3/astro_ghost/stellarLocus.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-2.0.3/astro_ghost/tonry_ps1_locus.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 15:54:06.066524 astro_ghost-2.0.3/astro_ghost.egg-info/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-17 15:54:05.000000 astro_ghost-2.0.3/astro_ghost.egg-info/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1318 2023-06-17 15:54:05.000000 astro_ghost-2.0.3/astro_ghost.egg-info/SOURCES.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-17 15:54:05.000000 astro_ghost-2.0.3/astro_ghost.egg-info/dependency_links.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-17 15:54:05.000000 astro_ghost-2.0.3/astro_ghost.egg-info/not-zip-safe
--rw-r--r--   0 alexgagliano   (501) staff       (20)      368 2023-06-17 15:54:05.000000 astro_ghost-2.0.3/astro_ghost.egg-info/requires.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-06-17 15:54:05.000000 astro_ghost-2.0.3/astro_ghost.egg-info/top_level.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 15:54:06.069974 astro_ghost-2.0.3/docs/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-2.0.3/docs/Makefile
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-2.0.3/docs/conf.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-2.0.3/docs/index.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-2.0.3/docs/make.bat
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 15:54:06.079793 astro_ghost-2.0.3/docs/source/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-2.0.3/docs/source/associationmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2479 2023-05-22 07:06:49.000000 astro_ghost-2.0.3/docs/source/basicusage.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-2.0.3/docs/source/catalogmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-2.0.3/docs/source/detailedtutorials.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      670 2023-05-10 20:33:11.000000 astro_ghost-2.0.3/docs/source/installation.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-2.0.3/docs/source/preprocessingmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-2.0.3/docs/source/supplementalmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-2.0.3/docs/source/wrappermodules.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 15:54:06.083418 astro_ghost-2.0.3/licenses/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-2.0.3/licenses/LICENSE.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-2.0.3/licenses/README.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-2.0.3/pyproject.toml
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1519 2023-06-17 15:54:06.090345 astro_ghost-2.0.3/setup.cfg
--rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1834 2023-06-17 15:52:29.000000 astro_ghost-2.0.3/setup.py
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 15:54:06.087161 astro_ghost-2.0.3/tests/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-2.0.3/tests/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      648 2023-05-22 03:39:53.000000 astro_ghost-2.0.3/tests/debug.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)        0 2023-05-10 21:17:11.000000 astro_ghost-2.0.3/tests/pytest.ini
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4213 2023-05-22 05:37:16.000000 astro_ghost-2.0.3/tests/test_tutorial.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1391 2023-05-24 04:36:02.000000 astro_ghost-2.0.3/tox.ini
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 16:36:09.578470 astro_ghost-2.0.5/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 16:36:09.449455 astro_ghost-2.0.5/.github/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 16:36:09.455364 astro_ghost-2.0.5/.github/workflows/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-2.0.5/.github/workflows/docs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      587 2023-05-24 04:50:38.000000 astro_ghost-2.0.5/.github/workflows/tests.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-2.0.5/.gitignore
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-2.0.5/.readthedocs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-2.0.5/MANIFEST.in
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-17 16:36:09.579382 astro_ghost-2.0.5/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     3674 2023-05-24 04:49:23.000000 astro_ghost-2.0.5/README.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 16:36:09.532190 astro_ghost-2.0.5/astro_ghost/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    23337 2023-06-17 16:33:29.000000 astro_ghost-2.0.5/astro_ghost/DLR.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4668 2023-05-22 16:28:50.000000 astro_ghost-2.0.5/astro_ghost/NEDQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    38694 2023-06-06 15:46:00.000000 astro_ghost-2.0.5/astro_ghost/PS1QueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-2.0.5/astro_ghost/SimbadQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-2.0.5/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2023-05-11 05:34:31.000000 astro_ghost-2.0.5/astro_ghost/TNSQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-2.0.5/astro_ghost/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-06-17 16:33:58.000000 astro_ghost-2.0.5/astro_ghost/_version.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-2.0.5/astro_ghost/conftest.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    42487 2023-06-17 15:47:53.000000 astro_ghost-2.0.5/astro_ghost/ghostHelperFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    32887 2023-06-04 03:48:08.000000 astro_ghost-2.0.5/astro_ghost/gradientAscent.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-2.0.5/astro_ghost/hostMatching.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    17727 2023-05-22 03:39:53.000000 astro_ghost-2.0.5/astro_ghost/photoz_helper.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     9853 2023-06-06 16:38:06.000000 astro_ghost-2.0.5/astro_ghost/sourceCleaning.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     7737 2023-05-24 04:44:13.000000 astro_ghost-2.0.5/astro_ghost/starSeparation.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4610 2023-05-24 04:43:14.000000 astro_ghost-2.0.5/astro_ghost/stellarLocus.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-2.0.5/astro_ghost/tonry_ps1_locus.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 16:36:09.537737 astro_ghost-2.0.5/astro_ghost.egg-info/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-17 16:36:09.000000 astro_ghost-2.0.5/astro_ghost.egg-info/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1318 2023-06-17 16:36:09.000000 astro_ghost-2.0.5/astro_ghost.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-17 16:36:09.000000 astro_ghost-2.0.5/astro_ghost.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-17 16:36:09.000000 astro_ghost-2.0.5/astro_ghost.egg-info/not-zip-safe
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      368 2023-06-17 16:36:09.000000 astro_ghost-2.0.5/astro_ghost.egg-info/requires.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-06-17 16:36:09.000000 astro_ghost-2.0.5/astro_ghost.egg-info/top_level.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 16:36:09.543011 astro_ghost-2.0.5/docs/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-2.0.5/docs/Makefile
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-2.0.5/docs/conf.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-2.0.5/docs/index.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-2.0.5/docs/make.bat
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 16:36:09.560068 astro_ghost-2.0.5/docs/source/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-2.0.5/docs/source/associationmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2479 2023-05-22 07:06:49.000000 astro_ghost-2.0.5/docs/source/basicusage.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-2.0.5/docs/source/catalogmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-2.0.5/docs/source/detailedtutorials.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      670 2023-05-10 20:33:11.000000 astro_ghost-2.0.5/docs/source/installation.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-2.0.5/docs/source/preprocessingmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-2.0.5/docs/source/supplementalmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-2.0.5/docs/source/wrappermodules.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 16:36:09.568095 astro_ghost-2.0.5/licenses/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-2.0.5/licenses/LICENSE.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-2.0.5/licenses/README.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-2.0.5/pyproject.toml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1519 2023-06-17 16:36:09.581253 astro_ghost-2.0.5/setup.cfg
+-rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1834 2023-06-17 16:34:38.000000 astro_ghost-2.0.5/setup.py
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 16:36:09.575468 astro_ghost-2.0.5/tests/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-2.0.5/tests/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      648 2023-05-22 03:39:53.000000 astro_ghost-2.0.5/tests/debug.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        0 2023-05-10 21:17:11.000000 astro_ghost-2.0.5/tests/pytest.ini
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4213 2023-05-22 05:37:16.000000 astro_ghost-2.0.5/tests/test_tutorial.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1391 2023-05-24 04:36:02.000000 astro_ghost-2.0.5/tox.ini
```

### Comparing `astro_ghost-2.0.3/.github/workflows/tests.yml` & `astro_ghost-2.0.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/.gitignore` & `astro_ghost-2.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/PKG-INFO` & `astro_ghost-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_ghost
-Version: 2.0.3
+Version: 2.0.5
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-2.0.3/README.rst` & `astro_ghost-2.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/astro_ghost/DLR.py` & `astro_ghost-2.0.5/astro_ghost/DLR.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,15 +410,16 @@
         name = str(row['Name'])
         ra_SN = float(row['RA'])
         dec_SN = float(row['DEC'])
         class_SN = str(row['Obj. Type'])
 
         #query the glade catalog
         result = Vizier.query_region(SkyCoord(ra=ra_SN, dec=dec_SN,unit=(u.deg, u.deg),frame='icrs'),width="1d",catalog=["VII/275/glade1"])
-        hosts = result[0].to_pandas()
+        if result:
+            hosts = result[0].to_pandas()
         
         #NEW (06/14) - query NED for GLADE sources and get their radius
         GLADE_rad = hosts.dropna(subset=['a_b', 'maj', 'min'])
         GLADE_norad = hosts[~hosts.index.isin(GLADE_rad.index)]
 
         from astroquery.ipac.ned import Ned
         badRadCount = 0
```

### Comparing `astro_ghost-2.0.3/astro_ghost/NEDQueryFunctions.py` & `astro_ghost-2.0.5/astro_ghost/NEDQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/astro_ghost/PS1QueryFunctions.py` & `astro_ghost-2.0.5/astro_ghost/PS1QueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/astro_ghost/SimbadQueryFunctions.py` & `astro_ghost-2.0.5/astro_ghost/SimbadQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav` & `astro_ghost-2.0.5/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/astro_ghost/TNSQueryFunctions.py` & `astro_ghost-2.0.5/astro_ghost/TNSQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/astro_ghost/conftest.py` & `astro_ghost-2.0.5/astro_ghost/conftest.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/astro_ghost/ghostHelperFunctions.py` & `astro_ghost-2.0.5/astro_ghost/ghostHelperFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/astro_ghost/gradientAscent.py` & `astro_ghost-2.0.5/astro_ghost/gradientAscent.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/astro_ghost/hostMatching.py` & `astro_ghost-2.0.5/astro_ghost/hostMatching.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/astro_ghost/photoz_helper.py` & `astro_ghost-2.0.5/astro_ghost/photoz_helper.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/astro_ghost/sourceCleaning.py` & `astro_ghost-2.0.5/astro_ghost/sourceCleaning.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/astro_ghost/starSeparation.py` & `astro_ghost-2.0.5/astro_ghost/starSeparation.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/astro_ghost/stellarLocus.py` & `astro_ghost-2.0.5/astro_ghost/stellarLocus.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/astro_ghost.egg-info/PKG-INFO` & `astro_ghost-2.0.5/astro_ghost.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-ghost
-Version: 2.0.3
+Version: 2.0.5
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-2.0.3/astro_ghost.egg-info/SOURCES.txt` & `astro_ghost-2.0.5/astro_ghost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/docs/Makefile` & `astro_ghost-2.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/docs/conf.py` & `astro_ghost-2.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/docs/index.rst` & `astro_ghost-2.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/docs/make.bat` & `astro_ghost-2.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/docs/source/associationmodules.rst` & `astro_ghost-2.0.5/docs/source/associationmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/docs/source/basicusage.rst` & `astro_ghost-2.0.5/docs/source/basicusage.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/docs/source/catalogmodules.rst` & `astro_ghost-2.0.5/docs/source/catalogmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/docs/source/installation.rst` & `astro_ghost-2.0.5/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/docs/source/preprocessingmodules.rst` & `astro_ghost-2.0.5/docs/source/preprocessingmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/licenses/LICENSE.rst` & `astro_ghost-2.0.5/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/setup.cfg` & `astro_ghost-2.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/setup.py` & `astro_ghost-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import os
 
 from setuptools import setup
 
-version = "2.0.3"
+version = "2.0.5"
 
 VERSION_TEMPLATE = """
  Note that we need to fall back to the hard-coded version if either
  setuptools_scm can't be imported or setuptools_scm can't determine the
  version, so we catch the generic 'Exception'.
 __version__ = '{version}'
 """.lstrip()
```

### Comparing `astro_ghost-2.0.3/tests/debug.py` & `astro_ghost-2.0.5/tests/debug.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/tests/test_tutorial.py` & `astro_ghost-2.0.5/tests/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.3/tox.ini` & `astro_ghost-2.0.5/tox.ini`

 * *Files identical despite different names*

