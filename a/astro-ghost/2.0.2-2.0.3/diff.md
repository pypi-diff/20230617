# Comparing `tmp/astro_ghost-2.0.2.tar.gz` & `tmp/astro_ghost-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_ghost-2.0.2.tar", last modified: Tue Jun  6 15:53:20 2023, max compression
+gzip compressed data, was "astro_ghost-2.0.3.tar", last modified: Sat Jun 17 15:54:06 2023, max compression
```

## Comparing `astro_ghost-2.0.2.tar` & `astro_ghost-2.0.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-06 15:53:20.060965 astro_ghost-2.0.2/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-06 15:53:19.986346 astro_ghost-2.0.2/.github/
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-06 15:53:19.993622 astro_ghost-2.0.2/.github/workflows/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-2.0.2/.github/workflows/docs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      587 2023-05-24 04:50:38.000000 astro_ghost-2.0.2/.github/workflows/tests.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-2.0.2/.gitignore
--rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-2.0.2/.readthedocs.yml
--rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-2.0.2/MANIFEST.in
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-06 15:53:20.061173 astro_ghost-2.0.2/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     3674 2023-05-24 04:49:23.000000 astro_ghost-2.0.2/README.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-06 15:53:20.041456 astro_ghost-2.0.2/astro_ghost/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    21836 2023-06-04 03:47:53.000000 astro_ghost-2.0.2/astro_ghost/DLR.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4668 2023-05-22 16:28:50.000000 astro_ghost-2.0.2/astro_ghost/NEDQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    38694 2023-06-06 15:46:00.000000 astro_ghost-2.0.2/astro_ghost/PS1QueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-2.0.2/astro_ghost/SimbadQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-2.0.2/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2023-05-11 05:34:31.000000 astro_ghost-2.0.2/astro_ghost/TNSQueryFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-2.0.2/astro_ghost/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-06-06 15:51:38.000000 astro_ghost-2.0.2/astro_ghost/_version.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-2.0.2/astro_ghost/conftest.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    39826 2023-05-23 03:25:58.000000 astro_ghost-2.0.2/astro_ghost/ghostHelperFunctions.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    32887 2023-06-04 03:48:08.000000 astro_ghost-2.0.2/astro_ghost/gradientAscent.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-2.0.2/astro_ghost/hostMatching.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)    17727 2023-05-22 03:39:53.000000 astro_ghost-2.0.2/astro_ghost/photoz_helper.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     9853 2023-05-22 16:28:44.000000 astro_ghost-2.0.2/astro_ghost/sourceCleaning.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     7737 2023-05-24 04:44:13.000000 astro_ghost-2.0.2/astro_ghost/starSeparation.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4610 2023-05-24 04:43:14.000000 astro_ghost-2.0.2/astro_ghost/stellarLocus.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-2.0.2/astro_ghost/tonry_ps1_locus.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-06 15:53:20.044081 astro_ghost-2.0.2/astro_ghost.egg-info/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-06 15:53:19.000000 astro_ghost-2.0.2/astro_ghost.egg-info/PKG-INFO
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1318 2023-06-06 15:53:19.000000 astro_ghost-2.0.2/astro_ghost.egg-info/SOURCES.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-06 15:53:19.000000 astro_ghost-2.0.2/astro_ghost.egg-info/dependency_links.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-06 15:53:19.000000 astro_ghost-2.0.2/astro_ghost.egg-info/not-zip-safe
--rw-r--r--   0 alexgagliano   (501) staff       (20)      368 2023-06-06 15:53:19.000000 astro_ghost-2.0.2/astro_ghost.egg-info/requires.txt
--rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-06-06 15:53:19.000000 astro_ghost-2.0.2/astro_ghost.egg-info/top_level.txt
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-06 15:53:20.047686 astro_ghost-2.0.2/docs/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-2.0.2/docs/Makefile
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-2.0.2/docs/conf.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-2.0.2/docs/index.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-2.0.2/docs/make.bat
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-06 15:53:20.055021 astro_ghost-2.0.2/docs/source/
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-2.0.2/docs/source/associationmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)     2479 2023-05-22 07:06:49.000000 astro_ghost-2.0.2/docs/source/basicusage.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-2.0.2/docs/source/catalogmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-2.0.2/docs/source/detailedtutorials.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      670 2023-05-10 20:33:11.000000 astro_ghost-2.0.2/docs/source/installation.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-2.0.2/docs/source/preprocessingmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-2.0.2/docs/source/supplementalmodules.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-2.0.2/docs/source/wrappermodules.rst
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-06 15:53:20.057484 astro_ghost-2.0.2/licenses/
--rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-2.0.2/licenses/LICENSE.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-2.0.2/licenses/README.rst
--rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-2.0.2/pyproject.toml
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1519 2023-06-06 15:53:20.062137 astro_ghost-2.0.2/setup.cfg
--rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1834 2023-06-06 15:51:48.000000 astro_ghost-2.0.2/setup.py
-drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-06 15:53:20.060125 astro_ghost-2.0.2/tests/
--rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-2.0.2/tests/__init__.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)      648 2023-05-22 03:39:53.000000 astro_ghost-2.0.2/tests/debug.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)        0 2023-05-10 21:17:11.000000 astro_ghost-2.0.2/tests/pytest.ini
--rw-r--r--   0 alexgagliano   (501) staff       (20)     4213 2023-05-22 05:37:16.000000 astro_ghost-2.0.2/tests/test_tutorial.py
--rw-r--r--   0 alexgagliano   (501) staff       (20)     1391 2023-05-24 04:36:02.000000 astro_ghost-2.0.2/tox.ini
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 15:54:06.088340 astro_ghost-2.0.3/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 15:54:05.976252 astro_ghost-2.0.3/.github/
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 15:54:05.984296 astro_ghost-2.0.3/.github/workflows/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      377 2022-08-10 18:18:27.000000 astro_ghost-2.0.3/.github/workflows/docs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      587 2023-05-24 04:50:38.000000 astro_ghost-2.0.3/.github/workflows/tests.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      769 2022-08-10 18:18:27.000000 astro_ghost-2.0.3/.gitignore
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      170 2022-08-10 18:18:27.000000 astro_ghost-2.0.3/.readthedocs.yml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      341 2022-08-10 18:18:27.000000 astro_ghost-2.0.3/MANIFEST.in
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-17 15:54:06.088682 astro_ghost-2.0.3/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     3674 2023-05-24 04:49:23.000000 astro_ghost-2.0.3/README.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 15:54:06.062436 astro_ghost-2.0.3/astro_ghost/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    23314 2023-06-17 15:51:41.000000 astro_ghost-2.0.3/astro_ghost/DLR.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4668 2023-05-22 16:28:50.000000 astro_ghost-2.0.3/astro_ghost/NEDQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    38694 2023-06-06 15:46:00.000000 astro_ghost-2.0.3/astro_ghost/PS1QueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1296 2023-05-10 22:09:14.000000 astro_ghost-2.0.3/astro_ghost/SimbadQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20) 13643353 2023-05-08 18:43:43.000000 astro_ghost-2.0.3/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1475 2023-05-11 05:34:31.000000 astro_ghost-2.0.3/astro_ghost/TNSQueryFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      112 2023-02-17 00:45:54.000000 astro_ghost-2.0.3/astro_ghost/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       22 2023-06-17 15:52:22.000000 astro_ghost-2.0.3/astro_ghost/_version.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1957 2023-02-17 00:45:54.000000 astro_ghost-2.0.3/astro_ghost/conftest.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    42487 2023-06-17 15:47:53.000000 astro_ghost-2.0.3/astro_ghost/ghostHelperFunctions.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    32887 2023-06-04 03:48:08.000000 astro_ghost-2.0.3/astro_ghost/gradientAscent.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2838 2023-05-09 20:46:38.000000 astro_ghost-2.0.3/astro_ghost/hostMatching.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    17727 2023-05-22 03:39:53.000000 astro_ghost-2.0.3/astro_ghost/photoz_helper.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     9853 2023-06-06 16:38:06.000000 astro_ghost-2.0.3/astro_ghost/sourceCleaning.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     7737 2023-05-24 04:44:13.000000 astro_ghost-2.0.3/astro_ghost/starSeparation.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4610 2023-05-24 04:43:14.000000 astro_ghost-2.0.3/astro_ghost/stellarLocus.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      302 2023-02-17 00:45:54.000000 astro_ghost-2.0.3/astro_ghost/tonry_ps1_locus.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 15:54:06.066524 astro_ghost-2.0.3/astro_ghost.egg-info/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4275 2023-06-17 15:54:05.000000 astro_ghost-2.0.3/astro_ghost.egg-info/PKG-INFO
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1318 2023-06-17 15:54:05.000000 astro_ghost-2.0.3/astro_ghost.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-17 15:54:05.000000 astro_ghost-2.0.3/astro_ghost.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        1 2023-06-17 15:54:05.000000 astro_ghost-2.0.3/astro_ghost.egg-info/not-zip-safe
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      368 2023-06-17 15:54:05.000000 astro_ghost-2.0.3/astro_ghost.egg-info/requires.txt
+-rw-r--r--   0 alexgagliano   (501) staff       (20)       18 2023-06-17 15:54:05.000000 astro_ghost-2.0.3/astro_ghost.egg-info/top_level.txt
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 15:54:06.069974 astro_ghost-2.0.3/docs/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      634 2022-08-10 18:18:27.000000 astro_ghost-2.0.3/docs/Makefile
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2545 2023-05-10 05:04:18.000000 astro_ghost-2.0.3/docs/conf.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2641 2023-05-10 20:40:49.000000 astro_ghost-2.0.3/docs/index.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      760 2022-08-10 18:18:27.000000 astro_ghost-2.0.3/docs/make.bat
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 15:54:06.079793 astro_ghost-2.0.3/docs/source/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1402 2023-05-10 20:31:16.000000 astro_ghost-2.0.3/docs/source/associationmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     2479 2023-05-22 07:06:49.000000 astro_ghost-2.0.3/docs/source/basicusage.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      819 2023-05-10 20:30:40.000000 astro_ghost-2.0.3/docs/source/catalogmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      124 2023-05-10 20:18:30.000000 astro_ghost-2.0.3/docs/source/detailedtutorials.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      670 2023-05-10 20:33:11.000000 astro_ghost-2.0.3/docs/source/installation.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      844 2023-05-10 20:31:25.000000 astro_ghost-2.0.3/docs/source/preprocessingmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      320 2023-05-10 20:31:41.000000 astro_ghost-2.0.3/docs/source/supplementalmodules.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      268 2023-05-10 20:38:08.000000 astro_ghost-2.0.3/docs/source/wrappermodules.rst
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 15:54:06.083418 astro_ghost-2.0.3/licenses/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)    37573 2022-08-10 18:18:27.000000 astro_ghost-2.0.3/licenses/LICENSE.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      372 2022-08-10 18:18:27.000000 astro_ghost-2.0.3/licenses/README.rst
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      134 2022-08-10 18:18:27.000000 astro_ghost-2.0.3/pyproject.toml
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1519 2023-06-17 15:54:06.090345 astro_ghost-2.0.3/setup.cfg
+-rwxr-xr-x   0 alexgagliano   (501) staff       (20)     1834 2023-06-17 15:52:29.000000 astro_ghost-2.0.3/setup.py
+drwxr-xr-x   0 alexgagliano   (501) staff       (20)        0 2023-06-17 15:54:06.087161 astro_ghost-2.0.3/tests/
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      108 2023-02-16 19:42:21.000000 astro_ghost-2.0.3/tests/__init__.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)      648 2023-05-22 03:39:53.000000 astro_ghost-2.0.3/tests/debug.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)        0 2023-05-10 21:17:11.000000 astro_ghost-2.0.3/tests/pytest.ini
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     4213 2023-05-22 05:37:16.000000 astro_ghost-2.0.3/tests/test_tutorial.py
+-rw-r--r--   0 alexgagliano   (501) staff       (20)     1391 2023-05-24 04:36:02.000000 astro_ghost-2.0.3/tox.ini
```

### Comparing `astro_ghost-2.0.2/.github/workflows/tests.yml` & `astro_ghost-2.0.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/.gitignore` & `astro_ghost-2.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/PKG-INFO` & `astro_ghost-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_ghost
-Version: 2.0.2
+Version: 2.0.3
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-2.0.2/README.rst` & `astro_ghost-2.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/astro_ghost/DLR.py` & `astro_ghost-2.0.3/astro_ghost/DLR.py`

 * *Files 7% similar despite different names*

```diff
@@ -372,16 +372,15 @@
         with open('../dictionaries/DLR_rankOrdered_hosts.p', 'wb') as fp:
             pickle.dump(dict_mod, fp, protocol=pickle.HIGHEST_PROTOCOL)
         hosts.to_csv("../tables/DLR_rankOrdered_hosts.csv")
         return
     elif todo =="r":
         return hosts, dict_mod, noHosts, GA_SN
 
-#new method - beta!
-def chooseByGladeDLR(path, fn, snDF, todo='r'):
+def chooseByGladeDLR(path, fn, snDF, verbose=False, todo='r'):
     """The wrapper function for selecting hosts by the DLR method (Gupta et al., 2013).
 
     Here, candidate hosts are taken from the GLADE (Dalya et al., 2021; arXiv:2110.06184) catalog.
 
     :param path: Filepath where to write out the results of the DLR algorithm.
     :type path: str
     :param fn: Filename to write the results of the associations (useful for debugging).
@@ -412,20 +411,47 @@
         ra_SN = float(row['RA'])
         dec_SN = float(row['DEC'])
         class_SN = str(row['Obj. Type'])
 
         #query the glade catalog
         result = Vizier.query_region(SkyCoord(ra=ra_SN, dec=dec_SN,unit=(u.deg, u.deg),frame='icrs'),width="1d",catalog=["VII/275/glade1"])
         hosts = result[0].to_pandas()
+        
+        #NEW (06/14) - query NED for GLADE sources and get their radius
+        GLADE_rad = hosts.dropna(subset=['a_b', 'maj', 'min'])
+        GLADE_norad = hosts[~hosts.index.isin(GLADE_rad.index)]
+
+        from astroquery.ipac.ned import Ned
+        badRadCount = 0
+        for idx, row in GLADE_norad.iterrows():
+            try:
+                result_table = Ned.query_region(SkyCoord(ra=row.RAJ2000*u.degree, dec=row.DEJ2000*u.degree, frame='icrs'), radius=(2/3600)*u.deg, equinox='J2000.0')
+                diameters = Ned.get_table(result_table.to_pandas()['Object Name'].values[0], table='diameters')
+                tempDF = diameters.to_pandas()
+                tempMaj_arcsec = np.nanmedian(tempDF.loc[(tempDF['Major Axis Unit'] == 'arcsec') & (tempDF['Major Axis Flag'] == '(a)'), 'Major Axis'])
+                AxisRatio = np.nanmedian(tempDF.loc[(tempDF['Axis Ratio Flag'] == '(b/a)'), 'Axis Ratio'])
+                tempMin_arcsec = tempMaj_arcsec*AxisRatio
+
+                GLADE_norad.loc[GLADE_norad.index == idx, 'maj'] = tempMaj_arcsec*2./60
+                GLADE_norad.loc[GLADE_norad.index == idx, 'min'] = tempMin_arcsec*2./60
+                GLADE_norad.loc[GLADE_norad.index == idx, 'a_b'] = 1/AxisRatio  
+            except:
+                badRadCount +=1
+
+        #recombine
+        if verbose:
+            print("No NED radius found for %i GLADE galaxies."%badRadCount)
+        hosts = pd.concat([GLADE_rad, GLADE_norad], ignore_index=True)
+
         hosts.dropna(subset=['a_b', 'maj', 'min'], inplace=True)
         if len(hosts)<1:
             noGladeHosts.append(name)
             continue
-        hosts['MajorRad'] = hosts['maj']*60/2 #in arcsec, to radius
-        hosts['MinorRad'] = hosts['min']*60/2 #in arcsec, to radius
+        hosts['MajorRad'] = hosts['maj']*60./2 #in arcsec, to radius
+        hosts['MinorRad'] = hosts['min']*60./2 #in arcsec, to radius
 
         #get names for the galaxies that match
         hosts.rename(columns={'RAJ2000':'raMean','DEJ2000':'decMean'}, inplace=True)
         hosts = getNEDInfo(hosts)
 
         R_dict = {}
         ra_dict = {}
```

### Comparing `astro_ghost-2.0.2/astro_ghost/NEDQueryFunctions.py` & `astro_ghost-2.0.3/astro_ghost/NEDQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/astro_ghost/PS1QueryFunctions.py` & `astro_ghost-2.0.3/astro_ghost/PS1QueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/astro_ghost/SimbadQueryFunctions.py` & `astro_ghost-2.0.3/astro_ghost/SimbadQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav` & `astro_ghost-2.0.3/astro_ghost/Star_Galaxy_RealisticModel_GHOST_PS1ClassLabels.sav`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/astro_ghost/TNSQueryFunctions.py` & `astro_ghost-2.0.3/astro_ghost/TNSQueryFunctions.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/astro_ghost/conftest.py` & `astro_ghost-2.0.3/astro_ghost/conftest.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/astro_ghost/ghostHelperFunctions.py` & `astro_ghost-2.0.3/astro_ghost/ghostHelperFunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from astro_ghost.gradientAscent import gradientAscent
 from astro_ghost.starSeparation import separateStars_STRM, separateStars_South
 from astro_ghost.sourceCleaning import clean_dict, removePS1Duplicates, getColors, makeCuts
 from astro_ghost.stellarLocus import calc_7DCD
 from astro_ghost.DLR import chooseByDLR, chooseByGladeDLR
 import requests
 import pickle
+import pyvo
 import glob
 from datetime import datetime
 from joblib import dump, load
 import pandas as pd
 
 #we do a lot of copies, sub-selects and rewrites - no need to warn about everything!
 pd.options.mode.chained_assignment = None  # default='warn'
@@ -203,14 +204,64 @@
     :type prefix: str
     :return: The input text, with prefix removed.
     :rtype: str
     """
 
     return text[text.startswith(prefix) and len(prefix):]
 
+def checkSimbadHierarchy(df, verbose=False):
+    """Throw a warning if the source has a parent in simbad!
+
+    :param df: The final associated data frame containing host and transient features.
+    :type df: Pandas DataFrame
+    :return: The dataframe, after correcting for SIMBAD hierarchical information.
+    :rtype: Pandas DataFrame
+    """
+    host_DF = df.copy()
+    HierarchicalHostedSNe = []
+    parents = []
+    for idx, row in host_DF.iterrows():
+        # cone search of the best-fit host in SIMBAD - if it gets it right,
+        #replace the info with the parent information!
+        tap_simbad = pyvo.dal.TAPService("https://simbad.u-strasbg.fr/simbad/sim-tap")
+        query = """SELECT main_id, otype, basic.ra, basic.dec,
+        DISTANCE( POINT('ICRS', ra, dec), POINT('ICRS', {0}, {1})) AS dist,
+        h_link.membership, cluster.id AS cluster
+        FROM (SELECT oid, id FROM basic JOIN ident ON oidref = oid WHERE
+        CONTAINS(POINT('ICRS',ra,dec),CIRCLE('ICRS',{0},{1},0.000556))=1 ) AS cluster, basic
+        JOIN h_link ON basic.oid = h_link.parent WHERE h_link.child = cluster.oid ORDER BY dist ASC;
+        """.format(row.raMean, row.decMean)
+        result = tap_simbad.search(query)
+        tap_pandas = result.to_table().to_pandas().reset_index(drop=True)
+        if ((not tap_pandas.empty) and (tap_pandas.loc[0, 'membership'] > 50)):
+            if verbose:
+                print("Warning! Host of %s is the hierarchical child of another object in Simbad, choosing parent as host instead..." % row.TransientName)
+            tap_pandas.drop_duplicates(subset=['main_id'], inplace=True)
+
+            # query PS1 for correct host
+            a = ps1cone(tap_pandas.loc[0, 'ra'], tap_pandas.loc[0, 'dec'], 10./3600)
+            if a:
+                a = ascii.read(a)
+                a = a.to_pandas()
+                parent = a.iloc[[0]]
+                parent['TransientName'] = row.TransientName
+                parent['TransientClass'] = row.TransientClass
+                parent['TransientRA'] = row.TransientRA
+                parent['TransientDEC'] = row.TransientDEC
+                parent = getNEDInfo(parent)
+                HierarchicalHostedSNe.append(row.TransientName)
+                parents.append(parent)
+    if len(parents)>0:
+        parentDF = pd.concat(parents)
+    else:
+        parentDF = pd.DataFrame({})
+    finalHosts_traditional = host_DF.loc[~host_DF['TransientName'].isin(HierarchicalHostedSNe)]
+    host_DF = pd.concat([finalHosts_traditional, parentDF], ignore_index=True)
+    return host_DF
+
 def getDBHostFromTransientCoords(transientCoords, GHOSTpath=''):
     """Gets the host of a GHOST transient by position.
 
     :param transientCoords: A list of astropy SkyCoord coordinates of transients.
     :type transientCoords: array-like
     :param GHOSTpath: The path to the saved GHOST database.
     :type GHOSTpath: str
@@ -229,15 +280,15 @@
     #a little wrapper so that this function can take lists of coords in addition to one coord
     for transientCoord in transientCoords:
         smallTable = fullTable[np.abs(fullTable['TransientRA'] - transientCoord.ra.degree)<0.1]
         smallTable = smallTable[np.abs(smallTable['TransientDEC'] - transientCoord.dec.degree)<0.1]
         if len(smallTable) < 1:
             notFound.append(transientCoord)
             continue
-        c2 = SkyCoord(smallTable['TransientRA']*u.deg, smallTable['TransientDEC']*u.deg, frame='icrs')
+        c2 = SkyCoord(smallTable['TransientRA'].values*u.deg, smallTable['TransientDEC'].values*u.deg, frame='icrs')
         sep = np.array(transientCoord.separation(c2).arcsec)
         if np.nanmin(sep) <= 1:
             host_idx = np.where(sep == np.nanmin(sep))[0][0]
             host = smallTable.iloc[[host_idx]]
             hostList.append(host)
         else:
             notFound.append(transientCoord)
@@ -699,15 +750,15 @@
 
     #create temp dataframe with RA and DEC corresponding to the transient
     snDF = pd.DataFrame({'Name':transientName_arr, 'RA':snRA_arr, 'DEC':snDEC_arr, 'HostName':['']*len(snDEC_arr), 'Obj. Type':snClass_arr})
     snDF.to_csv(path+fn_transients, index=False)
 
     #new low-z method (beta) - before we do anything else, find and associate with GLADE
     fn_glade = "gladeDLR.txt"
-    foundGladeHosts, noGladeHosts = chooseByGladeDLR(path, fn_glade, snDF, todo="r")
+    foundGladeHosts, noGladeHosts = chooseByGladeDLR(path, fn_glade, snDF, verbose=verbose, todo="r")
 
     #open transients df and drop the transients already found in GLADE. We'll add these back in at the end
     snDF = snDF[snDF['Name'].isin(noGladeHosts)]
     fn_transients_preGLADE = fn_transients
     fn_transients = 'transients_%s_postGlade.csv' % dateStr
     snDF.to_csv(path+fn_transients, index=False)
 
@@ -869,14 +920,16 @@
 
             #combine
             host_DF = pd.concat([host_DF, foundGladeHosts], ignore_index=True)
 
         with open(path+"/dictionaries/" + "Final_Dictionary.p", 'wb') as fp:
                dump(final_dict, fp)
 
+    host_DF = checkSimbadHierarchy(host_DF, verbose=verbose)
+
     #a few final cleaning steps
     host_DF.drop_duplicates(subset=['TransientName'], inplace=True)
     host_DF = host_DF[host_DF['TransientName'] != ""]
     host_DF.reset_index(inplace=True, drop=True)
     host_DF['TransientName'] = [x.replace(" ", "") for x in host_DF['TransientName']]
 
     allTransients = pd.read_csv(path+fn_transients_preGLADE)
```

### Comparing `astro_ghost-2.0.2/astro_ghost/gradientAscent.py` & `astro_ghost-2.0.3/astro_ghost/gradientAscent.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/astro_ghost/hostMatching.py` & `astro_ghost-2.0.3/astro_ghost/hostMatching.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/astro_ghost/photoz_helper.py` & `astro_ghost-2.0.3/astro_ghost/photoz_helper.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/astro_ghost/sourceCleaning.py` & `astro_ghost-2.0.3/astro_ghost/sourceCleaning.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/astro_ghost/starSeparation.py` & `astro_ghost-2.0.3/astro_ghost/starSeparation.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/astro_ghost/stellarLocus.py` & `astro_ghost-2.0.3/astro_ghost/stellarLocus.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/astro_ghost.egg-info/PKG-INFO` & `astro_ghost-2.0.3/astro_ghost.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-ghost
-Version: 2.0.2
+Version: 2.0.3
 Summary: A package to associate transients with host galaxies, and a database of 16k SNe-host galaxies in PS1.
 Home-page: https://github.com/pypa/sampleproject
 Author: Alex Gagliano
 Author-email: gaglian2@illinois.edu
 License: GNU GPL v3+
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `astro_ghost-2.0.2/astro_ghost.egg-info/SOURCES.txt` & `astro_ghost-2.0.3/astro_ghost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/docs/Makefile` & `astro_ghost-2.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/docs/conf.py` & `astro_ghost-2.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/docs/index.rst` & `astro_ghost-2.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/docs/make.bat` & `astro_ghost-2.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/docs/source/associationmodules.rst` & `astro_ghost-2.0.3/docs/source/associationmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/docs/source/basicusage.rst` & `astro_ghost-2.0.3/docs/source/basicusage.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/docs/source/catalogmodules.rst` & `astro_ghost-2.0.3/docs/source/catalogmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/docs/source/installation.rst` & `astro_ghost-2.0.3/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/docs/source/preprocessingmodules.rst` & `astro_ghost-2.0.3/docs/source/preprocessingmodules.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/licenses/LICENSE.rst` & `astro_ghost-2.0.3/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/setup.cfg` & `astro_ghost-2.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/setup.py` & `astro_ghost-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 
 import os
 
 from setuptools import setup
 
-version = "2.0.2"
+version = "2.0.3"
 
 VERSION_TEMPLATE = """
  Note that we need to fall back to the hard-coded version if either
  setuptools_scm can't be imported or setuptools_scm can't determine the
  version, so we catch the generic 'Exception'.
 __version__ = '{version}'
 """.lstrip()
```

### Comparing `astro_ghost-2.0.2/tests/debug.py` & `astro_ghost-2.0.3/tests/debug.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/tests/test_tutorial.py` & `astro_ghost-2.0.3/tests/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `astro_ghost-2.0.2/tox.ini` & `astro_ghost-2.0.3/tox.ini`

 * *Files identical despite different names*

