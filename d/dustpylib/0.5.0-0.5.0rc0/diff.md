# Comparing `tmp/dustpylib-0.5.0.tar.gz` & `tmp/dustpylib-0.5.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dustpylib-0.5.0.tar", last modified: Sat Jun 17 19:30:05 2023, max compression
+gzip compressed data, was "dustpylib-0.5.0rc0.tar", last modified: Fri Jun 16 15:57:00 2023, max compression
```

## Comparing `dustpylib-0.5.0.tar` & `dustpylib-0.5.0rc0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:30:07.131848 dustpylib-0.5.0/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1505 2023-04-19 09:53:48.000000 dustpylib-0.5.0/LICENSE
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      256 2023-05-21 09:32:44.000000 dustpylib-0.5.0/MANIFEST.in
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3068 2023-06-17 19:30:07.123885 dustpylib-0.5.0/PKG-INFO
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1925 2023-05-21 09:52:26.000000 dustpylib-0.5.0/README.md
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:30:04.392512 dustpylib-0.5.0/docs/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      637 2023-04-27 14:03:17.000000 dustpylib-0.5.0/docs/Makefile
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      763 2023-04-27 14:02:49.000000 dustpylib-0.5.0/docs/make.bat
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      166 2023-04-27 17:33:15.000000 dustpylib-0.5.0/docs/requirements.txt
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:30:05.717868 dustpylib-0.5.0/docs/source/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2802 2023-05-22 12:20:13.000000 dustpylib-0.5.0/docs/source/A_contrib_bug_feature.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      798 2023-06-16 15:38:45.000000 dustpylib-0.5.0/docs/source/api.rst
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)   276682 2023-06-16 15:32:31.000000 dustpylib-0.5.0/docs/source/backreaction.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1962 2023-05-03 15:14:00.000000 dustpylib-0.5.0/docs/source/conf.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      174 2023-06-16 15:36:43.000000 dustpylib-0.5.0/docs/source/dynamics.rst
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      150 2023-04-29 20:41:23.000000 dustpylib-0.5.0/docs/source/grid.rst
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)   180984 2023-05-21 09:31:06.000000 dustpylib-0.5.0/docs/source/grid_refinement.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      888 2023-06-16 15:37:41.000000 dustpylib-0.5.0/docs/source/index.rst
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)   254062 2023-05-21 09:54:36.000000 dustpylib-0.5.0/docs/source/planetary_gaps.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    25402 2023-05-21 09:56:51.000000 dustpylib-0.5.0/docs/source/planetesimal_formation.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      224 2023-04-29 17:08:50.000000 dustpylib-0.5.0/docs/source/planetesimals.rst
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)  1957524 2023-06-16 14:10:43.000000 dustpylib-0.5.0/docs/source/radmc3d.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      369 2023-04-29 17:09:25.000000 dustpylib-0.5.0/docs/source/radtrans.rst
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      204 2023-04-29 20:40:49.000000 dustpylib-0.5.0/docs/source/substructures.rst
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:30:05.766844 dustpylib-0.5.0/dustpylib/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      402 2023-06-17 19:24:23.000000 dustpylib-0.5.0/dustpylib/__init__.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:30:06.072844 dustpylib-0.5.0/dustpylib/dynamics/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      146 2023-06-16 14:33:41.000000 dustpylib-0.5.0/dustpylib/dynamics/__init__.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:30:06.410844 dustpylib-0.5.0/dustpylib/dynamics/backreaction/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      902 2023-06-16 14:36:16.000000 dustpylib-0.5.0/dustpylib/dynamics/backreaction/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     7830 2023-06-16 14:35:39.000000 dustpylib-0.5.0/dustpylib/dynamics/backreaction/functions_backreaction.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2623 2023-06-16 14:42:34.000000 dustpylib-0.5.0/dustpylib/dynamics/backreaction/setup_backreaction.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:30:06.454844 dustpylib-0.5.0/dustpylib/grid/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      134 2023-05-20 14:49:24.000000 dustpylib-0.5.0/dustpylib/grid/__init__.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:30:06.580844 dustpylib-0.5.0/dustpylib/grid/refinement/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      170 2023-05-20 14:50:16.000000 dustpylib-0.5.0/dustpylib/grid/refinement/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1235 2023-05-20 14:50:52.000000 dustpylib-0.5.0/dustpylib/grid/refinement/refinement.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:30:06.619844 dustpylib-0.5.0/dustpylib/planetesimals/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      138 2023-05-20 14:53:28.000000 dustpylib-0.5.0/dustpylib/planetesimals/__init__.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:30:06.737847 dustpylib-0.5.0/dustpylib/planetesimals/formation/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      362 2023-05-20 14:53:35.000000 dustpylib-0.5.0/dustpylib/planetesimals/formation/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3827 2023-05-20 14:56:23.000000 dustpylib-0.5.0/dustpylib/planetesimals/formation/formation.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:30:06.773843 dustpylib-0.5.0/dustpylib/radtrans/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      163 2023-05-20 14:56:48.000000 dustpylib-0.5.0/dustpylib/radtrans/__init__.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:30:06.895848 dustpylib-0.5.0/dustpylib/radtrans/radmc3d/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      418 2023-05-20 15:04:37.000000 dustpylib-0.5.0/dustpylib/radtrans/radmc3d/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    33639 2023-06-16 13:59:08.000000 dustpylib-0.5.0/dustpylib/radtrans/radmc3d/radmc3d.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:30:06.943886 dustpylib-0.5.0/dustpylib/substructures/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      158 2023-05-20 15:04:54.000000 dustpylib-0.5.0/dustpylib/substructures/__init__.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:30:07.057845 dustpylib-0.5.0/dustpylib/substructures/gaps/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      249 2023-05-20 15:05:01.000000 dustpylib-0.5.0/dustpylib/substructures/gaps/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2192 2023-05-20 15:05:33.000000 dustpylib-0.5.0/dustpylib/substructures/gaps/gaps.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:30:06.020846 dustpylib-0.5.0/dustpylib.egg-info/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3068 2023-06-17 19:30:02.000000 dustpylib-0.5.0/dustpylib.egg-info/PKG-INFO
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1365 2023-06-17 19:30:03.000000 dustpylib-0.5.0/dustpylib.egg-info/SOURCES.txt
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2023-06-17 19:30:02.000000 dustpylib-0.5.0/dustpylib.egg-info/dependency_links.txt
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2023-04-27 15:54:48.000000 dustpylib-0.5.0/dustpylib.egg-info/not-zip-safe
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)       59 2023-06-17 19:30:02.000000 dustpylib-0.5.0/dustpylib.egg-info/requires.txt
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)       16 2023-06-17 19:30:02.000000 dustpylib-0.5.0/dustpylib.egg-info/top_level.txt
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)       38 2023-06-17 19:30:07.134851 dustpylib-0.5.0/setup.cfg
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2149 2023-06-17 19:25:04.000000 dustpylib-0.5.0/setup.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:30:07.091848 dustpylib-0.5.0/tests/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-19 17:36:43.000000 dustpylib-0.5.0/tests/__init__.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-16 15:57:01.746990 dustpylib-0.5.0rc0/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1505 2023-04-19 09:53:48.000000 dustpylib-0.5.0rc0/LICENSE
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      256 2023-05-21 09:32:44.000000 dustpylib-0.5.0rc0/MANIFEST.in
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3055 2023-06-16 15:57:01.743993 dustpylib-0.5.0rc0/PKG-INFO
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1925 2023-05-21 09:52:26.000000 dustpylib-0.5.0rc0/README.md
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-16 15:57:00.279778 dustpylib-0.5.0rc0/docs/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      637 2023-04-27 14:03:17.000000 dustpylib-0.5.0rc0/docs/Makefile
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      763 2023-04-27 14:02:49.000000 dustpylib-0.5.0rc0/docs/make.bat
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      166 2023-04-27 17:33:15.000000 dustpylib-0.5.0rc0/docs/requirements.txt
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-16 15:57:00.855989 dustpylib-0.5.0rc0/docs/source/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2802 2023-05-22 12:20:13.000000 dustpylib-0.5.0rc0/docs/source/A_contrib_bug_feature.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      798 2023-06-16 15:38:45.000000 dustpylib-0.5.0rc0/docs/source/api.rst
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)   276682 2023-06-16 15:32:31.000000 dustpylib-0.5.0rc0/docs/source/backreaction.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1962 2023-05-03 15:14:00.000000 dustpylib-0.5.0rc0/docs/source/conf.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      174 2023-06-16 15:36:43.000000 dustpylib-0.5.0rc0/docs/source/dynamics.rst
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      150 2023-04-29 20:41:23.000000 dustpylib-0.5.0rc0/docs/source/grid.rst
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)   180984 2023-05-21 09:31:06.000000 dustpylib-0.5.0rc0/docs/source/grid_refinement.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      888 2023-06-16 15:37:41.000000 dustpylib-0.5.0rc0/docs/source/index.rst
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)   254062 2023-05-21 09:54:36.000000 dustpylib-0.5.0rc0/docs/source/planetary_gaps.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    25402 2023-05-21 09:56:51.000000 dustpylib-0.5.0rc0/docs/source/planetesimal_formation.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      224 2023-04-29 17:08:50.000000 dustpylib-0.5.0rc0/docs/source/planetesimals.rst
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)  1957524 2023-06-16 14:10:43.000000 dustpylib-0.5.0rc0/docs/source/radmc3d.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      369 2023-04-29 17:09:25.000000 dustpylib-0.5.0rc0/docs/source/radtrans.rst
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      204 2023-04-29 20:40:49.000000 dustpylib-0.5.0rc0/docs/source/substructures.rst
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-16 15:57:00.881989 dustpylib-0.5.0rc0/dustpylib/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      405 2023-06-16 15:56:51.000000 dustpylib-0.5.0rc0/dustpylib/__init__.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-16 15:57:01.068987 dustpylib-0.5.0rc0/dustpylib/dynamics/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      146 2023-06-16 14:33:41.000000 dustpylib-0.5.0rc0/dustpylib/dynamics/__init__.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-16 15:57:01.215989 dustpylib-0.5.0rc0/dustpylib/dynamics/backreaction/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      902 2023-06-16 14:36:16.000000 dustpylib-0.5.0rc0/dustpylib/dynamics/backreaction/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     7830 2023-06-16 14:35:39.000000 dustpylib-0.5.0rc0/dustpylib/dynamics/backreaction/functions_backreaction.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2623 2023-06-16 14:42:34.000000 dustpylib-0.5.0rc0/dustpylib/dynamics/backreaction/setup_backreaction.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-16 15:57:01.250987 dustpylib-0.5.0rc0/dustpylib/grid/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      134 2023-05-20 14:49:24.000000 dustpylib-0.5.0rc0/dustpylib/grid/__init__.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-16 15:57:01.332986 dustpylib-0.5.0rc0/dustpylib/grid/refinement/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      170 2023-05-20 14:50:16.000000 dustpylib-0.5.0rc0/dustpylib/grid/refinement/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1235 2023-05-20 14:50:52.000000 dustpylib-0.5.0rc0/dustpylib/grid/refinement/refinement.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-16 15:57:01.371990 dustpylib-0.5.0rc0/dustpylib/planetesimals/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      138 2023-05-20 14:53:28.000000 dustpylib-0.5.0rc0/dustpylib/planetesimals/__init__.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-16 15:57:01.450987 dustpylib-0.5.0rc0/dustpylib/planetesimals/formation/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      362 2023-05-20 14:53:35.000000 dustpylib-0.5.0rc0/dustpylib/planetesimals/formation/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3827 2023-05-20 14:56:23.000000 dustpylib-0.5.0rc0/dustpylib/planetesimals/formation/formation.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-16 15:57:01.486988 dustpylib-0.5.0rc0/dustpylib/radtrans/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      163 2023-05-20 14:56:48.000000 dustpylib-0.5.0rc0/dustpylib/radtrans/__init__.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-16 15:57:01.565988 dustpylib-0.5.0rc0/dustpylib/radtrans/radmc3d/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      418 2023-05-20 15:04:37.000000 dustpylib-0.5.0rc0/dustpylib/radtrans/radmc3d/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    33639 2023-06-16 13:59:08.000000 dustpylib-0.5.0rc0/dustpylib/radtrans/radmc3d/radmc3d.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-16 15:57:01.603991 dustpylib-0.5.0rc0/dustpylib/substructures/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      158 2023-05-20 15:04:54.000000 dustpylib-0.5.0rc0/dustpylib/substructures/__init__.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-16 15:57:01.686991 dustpylib-0.5.0rc0/dustpylib/substructures/gaps/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      249 2023-05-20 15:05:01.000000 dustpylib-0.5.0rc0/dustpylib/substructures/gaps/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2192 2023-05-20 15:05:33.000000 dustpylib-0.5.0rc0/dustpylib/substructures/gaps/gaps.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-16 15:57:01.045987 dustpylib-0.5.0rc0/dustpylib.egg-info/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3055 2023-06-16 15:56:59.000000 dustpylib-0.5.0rc0/dustpylib.egg-info/PKG-INFO
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1365 2023-06-16 15:56:59.000000 dustpylib-0.5.0rc0/dustpylib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2023-06-16 15:56:59.000000 dustpylib-0.5.0rc0/dustpylib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2023-04-27 15:54:48.000000 dustpylib-0.5.0rc0/dustpylib.egg-info/not-zip-safe
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)       59 2023-06-16 15:56:59.000000 dustpylib-0.5.0rc0/dustpylib.egg-info/requires.txt
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)       16 2023-06-16 15:56:59.000000 dustpylib-0.5.0rc0/dustpylib.egg-info/top_level.txt
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)       38 2023-06-16 15:57:01.747988 dustpylib-0.5.0rc0/setup.cfg
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2133 2023-04-27 17:33:26.000000 dustpylib-0.5.0rc0/setup.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-16 15:57:01.717988 dustpylib-0.5.0rc0/tests/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-05-19 17:36:43.000000 dustpylib-0.5.0rc0/tests/__init__.py
```

### Comparing `dustpylib-0.5.0/LICENSE` & `dustpylib-0.5.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dustpylib-0.5.0/PKG-INFO` & `dustpylib-0.5.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dustpylib
-Version: 0.5.0
+Version: 0.5.0rc0
 Home-page: https://github.com/stammler/dustpylib/
-Author: Sebastian Stammler, Matias, Garate, Tilman Birnstiel
+Author: Sebastian Stammler, Tilman Birnstiel
 Author-email: sebastian.stammler@gmail.com
 Maintainer: Sebastian Stammler
 License: BSD
 Project-URL: Source Code, https://github.com/stammler/dustpylib/
 Project-URL: Documentation, https://dustpylib.rtfd.io/
 Keywords: science physics mathematics visualization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dustpylib-0.5.0/README.md` & `dustpylib-0.5.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `dustpylib-0.5.0/docs/Makefile` & `dustpylib-0.5.0rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dustpylib-0.5.0/docs/make.bat` & `dustpylib-0.5.0rc0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dustpylib-0.5.0/docs/source/A_contrib_bug_feature.ipynb` & `dustpylib-0.5.0rc0/docs/source/A_contrib_bug_feature.ipynb`

 * *Files identical despite different names*

### Comparing `dustpylib-0.5.0/docs/source/api.rst` & `dustpylib-0.5.0rc0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `dustpylib-0.5.0/docs/source/backreaction.ipynb` & `dustpylib-0.5.0rc0/docs/source/backreaction.ipynb`

 * *Files identical despite different names*

### Comparing `dustpylib-0.5.0/docs/source/conf.py` & `dustpylib-0.5.0rc0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dustpylib-0.5.0/docs/source/grid_refinement.ipynb` & `dustpylib-0.5.0rc0/docs/source/grid_refinement.ipynb`

 * *Files identical despite different names*

### Comparing `dustpylib-0.5.0/docs/source/index.rst` & `dustpylib-0.5.0rc0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `dustpylib-0.5.0/docs/source/planetary_gaps.ipynb` & `dustpylib-0.5.0rc0/docs/source/planetary_gaps.ipynb`

 * *Files identical despite different names*

### Comparing `dustpylib-0.5.0/docs/source/planetesimal_formation.ipynb` & `dustpylib-0.5.0rc0/docs/source/planetesimal_formation.ipynb`

 * *Files identical despite different names*

### Comparing `dustpylib-0.5.0/docs/source/radmc3d.ipynb` & `dustpylib-0.5.0rc0/docs/source/radmc3d.ipynb`

 * *Files identical despite different names*

### Comparing `dustpylib-0.5.0/dustpylib/dynamics/backreaction/__init__.py` & `dustpylib-0.5.0rc0/dustpylib/dynamics/backreaction/__init__.py`

 * *Files identical despite different names*

### Comparing `dustpylib-0.5.0/dustpylib/dynamics/backreaction/functions_backreaction.py` & `dustpylib-0.5.0rc0/dustpylib/dynamics/backreaction/functions_backreaction.py`

 * *Files identical despite different names*

### Comparing `dustpylib-0.5.0/dustpylib/dynamics/backreaction/setup_backreaction.py` & `dustpylib-0.5.0rc0/dustpylib/dynamics/backreaction/setup_backreaction.py`

 * *Files identical despite different names*

### Comparing `dustpylib-0.5.0/dustpylib/grid/refinement/refinement.py` & `dustpylib-0.5.0rc0/dustpylib/grid/refinement/refinement.py`

 * *Files identical despite different names*

### Comparing `dustpylib-0.5.0/dustpylib/planetesimals/formation/formation.py` & `dustpylib-0.5.0rc0/dustpylib/planetesimals/formation/formation.py`

 * *Files identical despite different names*

### Comparing `dustpylib-0.5.0/dustpylib/radtrans/radmc3d/radmc3d.py` & `dustpylib-0.5.0rc0/dustpylib/radtrans/radmc3d/radmc3d.py`

 * *Files identical despite different names*

### Comparing `dustpylib-0.5.0/dustpylib/substructures/gaps/gaps.py` & `dustpylib-0.5.0rc0/dustpylib/substructures/gaps/gaps.py`

 * *Files identical despite different names*

### Comparing `dustpylib-0.5.0/dustpylib.egg-info/PKG-INFO` & `dustpylib-0.5.0rc0/dustpylib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dustpylib
-Version: 0.5.0
+Version: 0.5.0rc0
 Home-page: https://github.com/stammler/dustpylib/
-Author: Sebastian Stammler, Matias, Garate, Tilman Birnstiel
+Author: Sebastian Stammler, Tilman Birnstiel
 Author-email: sebastian.stammler@gmail.com
 Maintainer: Sebastian Stammler
 License: BSD
 Project-URL: Source Code, https://github.com/stammler/dustpylib/
 Project-URL: Documentation, https://dustpylib.rtfd.io/
 Keywords: science physics mathematics visualization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dustpylib-0.5.0/dustpylib.egg-info/SOURCES.txt` & `dustpylib-0.5.0rc0/dustpylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dustpylib-0.5.0/setup.py` & `dustpylib-0.5.0rc0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     keywords="science physics mathematics visualization",
 
     url="https://github.com/stammler/dustpylib/",
     project_urls={"Source Code": "https://github.com/stammler/dustpylib/",
                   "Documentation": "https://dustpylib.rtfd.io/"
                   },
 
-    author="Sebastian Stammler, Matias, Garate, Tilman Birnstiel",
+    author="Sebastian Stammler, Tilman Birnstiel",
     author_email="sebastian.stammler@gmail.com",
     maintainer="Sebastian Stammler",
 
     version=read_version(),
     license="BSD",
 
     classifiers=["Development Status :: 4 - Beta",
```

