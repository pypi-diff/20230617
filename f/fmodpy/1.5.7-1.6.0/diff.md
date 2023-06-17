# Comparing `tmp/fmodpy-1.5.7.tar.gz` & `tmp/fmodpy-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmodpy-1.5.7.tar", last modified: Thu Apr  6 15:07:53 2023, max compression
+gzip compressed data, was "fmodpy-1.6.0.tar", last modified: Sat Jun 17 16:37:49 2023, max compression
```

## Comparing `fmodpy-1.5.7.tar` & `fmodpy-1.6.0.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-04-06 15:07:53.180402 fmodpy-1.5.7/
--rw-r--r--   0 thomaslux   (501) staff       (20)     1072 2022-03-18 19:21:33.000000 fmodpy-1.5.7/LICENSE.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)       27 2022-07-26 13:43:21.000000 fmodpy-1.5.7/MANIFEST.in
--rw-r--r--   0 thomaslux   (501) staff       (20)      753 2023-04-06 15:07:53.180470 fmodpy-1.5.7/PKG-INFO
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-04-06 15:07:53.166226 fmodpy-1.5.7/fmodpy/
--rw-r--r--   0 thomaslux   (501) staff       (20)      658 2022-07-18 14:21:02.000000 fmodpy-1.5.7/fmodpy/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     1148 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/__main__.py
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-04-06 15:07:53.168401 fmodpy-1.5.7/fmodpy/about/
--rw-r--r--   0 thomaslux   (501) staff       (20)       47 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/about/author.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)      607 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/about/classifiers.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)       72 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/about/description.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)       31 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/about/keywords.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)        5 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/about/on_pypi.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)       12 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/about/requirements.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)        6 2023-03-28 04:51:29.000000 fmodpy-1.5.7/fmodpy/about/version.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)     4697 2023-04-06 15:07:50.000000 fmodpy-1.5.7/fmodpy/about/version_history.md
--rw-r--r--   0 thomaslux   (501) staff       (20)    12285 2023-03-28 04:47:43.000000 fmodpy-1.5.7/fmodpy/config.py
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-04-06 15:07:53.168955 fmodpy-1.5.7/fmodpy/development/
--rw-r--r--   0 thomaslux   (501) staff       (20)     1136 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/development/strange_type_example.f90
--rw-r--r--   0 thomaslux   (501) staff       (20)     5060 2022-04-09 14:56:15.000000 fmodpy-1.5.7/fmodpy/development/todo.py
--rw-r--r--   0 thomaslux   (501) staff       (20)      874 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/development/type.py
--rw-r--r--   0 thomaslux   (501) staff       (20)      522 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/exceptions.py
--rw-r--r--   0 thomaslux   (501) staff       (20)    34638 2023-03-28 04:40:43.000000 fmodpy-1.5.7/fmodpy/fmodpy.py
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-04-06 15:07:53.172901 fmodpy-1.5.7/fmodpy/parsing/
--rw-r--r--   0 thomaslux   (501) staff       (20)    10880 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/parsing/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     2926 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/parsing/_old_code.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)    39247 2023-04-06 04:56:58.000000 fmodpy-1.5.7/fmodpy/parsing/argument.py
--rw-r--r--   0 thomaslux   (501) staff       (20)      817 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/parsing/character.py
--rw-r--r--   0 thomaslux   (501) staff       (20)    13228 2023-03-28 04:21:48.000000 fmodpy-1.5.7/fmodpy/parsing/code.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     1600 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/parsing/complex.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     5153 2022-07-20 06:18:28.000000 fmodpy-1.5.7/fmodpy/parsing/file.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     2853 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/parsing/function.py
--rw-r--r--   0 thomaslux   (501) staff       (20)        0 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/parsing/implicit_none.py
--rw-r--r--   0 thomaslux   (501) staff       (20)      162 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/parsing/integer.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     1563 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/parsing/interface.py
--rw-r--r--   0 thomaslux   (501) staff       (20)      950 2023-04-06 04:56:34.000000 fmodpy-1.5.7/fmodpy/parsing/logical.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     7602 2023-03-15 16:08:22.000000 fmodpy-1.5.7/fmodpy/parsing/module.py
--rw-r--r--   0 thomaslux   (501) staff       (20)      118 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/parsing/procedure.py
--rw-r--r--   0 thomaslux   (501) staff       (20)      160 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/parsing/real.py
--rw-r--r--   0 thomaslux   (501) staff       (20)    20947 2023-03-27 01:44:22.000000 fmodpy-1.5.7/fmodpy/parsing/subroutine.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     6315 2022-05-10 02:34:01.000000 fmodpy-1.5.7/fmodpy/parsing/type.py
--rw-r--r--   0 thomaslux   (501) staff       (20)        0 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/parsing/use.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     6810 2023-03-27 01:31:38.000000 fmodpy-1.5.7/fmodpy/parsing/util.py
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-04-06 15:07:53.173423 fmodpy-1.5.7/fmodpy/test/
--rw-r--r--   0 thomaslux   (501) staff       (20)    53248 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/.coverage
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-04-06 15:07:53.173852 fmodpy-1.5.7/fmodpy/test/character/
--rw-r--r--   0 thomaslux   (501) staff       (20)     1410 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/character/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)      607 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/character/test_character.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-04-06 15:07:53.174252 fmodpy-1.5.7/fmodpy/test/complex128/
--rw-r--r--   0 thomaslux   (501) staff       (20)     2311 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/complex128/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     3655 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/complex128/test_complex128.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-04-06 15:07:53.174575 fmodpy-1.5.7/fmodpy/test/complex256/
--rw-r--r--   0 thomaslux   (501) staff       (20)     2377 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/complex256/__init__.py
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-04-06 15:07:53.174908 fmodpy-1.5.7/fmodpy/test/complex256/test_complex256/
--rw-r--r--   0 thomaslux   (501) staff       (20)     7751 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/complex256/test_complex256/test_complex256_c_wrapper.f90
--rw-r--r--   0 thomaslux   (501) staff       (20)    13250 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/complex256/test_complex256/test_complex256_python_wrapper.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     3978 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/complex256/test_complex256.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-04-06 15:07:53.175214 fmodpy-1.5.7/fmodpy/test/complex64/
--rw-r--r--   0 thomaslux   (501) staff       (20)     2309 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/complex64/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     3655 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/complex64/test_complex64.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-04-06 15:07:53.175522 fmodpy-1.5.7/fmodpy/test/double_precision/
--rw-r--r--   0 thomaslux   (501) staff       (20)     2252 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/double_precision/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     3626 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/double_precision/test_double_precision.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-04-06 15:07:53.175841 fmodpy-1.5.7/fmodpy/test/int32/
--rw-r--r--   0 thomaslux   (501) staff       (20)     2256 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/int32/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     3411 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/int32/test_int32.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-04-06 15:07:53.176273 fmodpy-1.5.7/fmodpy/test/int64/
--rw-r--r--   0 thomaslux   (501) staff       (20)     2427 2022-08-27 16:58:36.000000 fmodpy-1.5.7/fmodpy/test/int64/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     4008 2022-08-27 16:57:13.000000 fmodpy-1.5.7/fmodpy/test/int64/test_int64.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-04-06 15:07:53.176850 fmodpy-1.5.7/fmodpy/test/logical/
--rw-r--r--   0 thomaslux   (501) staff       (20)     1435 2022-03-27 18:02:26.000000 fmodpy-1.5.7/fmodpy/test/logical/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)      663 2022-03-27 17:59:28.000000 fmodpy-1.5.7/fmodpy/test/logical/test_logical.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-04-06 15:07:53.177615 fmodpy-1.5.7/fmodpy/test/misc/
--rw-r--r--   0 thomaslux   (501) staff       (20)      932 2022-05-10 02:37:20.000000 fmodpy-1.5.7/fmodpy/test/misc/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)      212 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/misc/implicit_shape.f90
--rw-r--r--   0 thomaslux   (501) staff       (20)      271 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/misc/simple.f03
--rw-r--r--   0 thomaslux   (501) staff       (20)      307 2022-05-10 02:24:48.000000 fmodpy-1.5.7/fmodpy/test/misc/subroutine_with_type.f90
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-04-06 15:07:53.178189 fmodpy-1.5.7/fmodpy/test/module/
--rw-r--r--   0 thomaslux   (501) staff       (20)     3173 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/module/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)      173 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/module/extra_module.f03
--rw-r--r--   0 thomaslux   (501) staff       (20)     1364 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/module/test_module.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-04-06 15:07:53.178507 fmodpy-1.5.7/fmodpy/test/procedure/
--rw-r--r--   0 thomaslux   (501) staff       (20)     1134 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/procedure/__init__.py
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-04-06 15:07:53.179001 fmodpy-1.5.7/fmodpy/test/procedure/og_procedure/
--rw-r--r--   0 thomaslux   (501) staff       (20)     1253 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/procedure/og_procedure/procedure.f03
--rw-r--r--   0 thomaslux   (501) staff       (20)     1624 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/procedure/og_procedure/procedure.pyx
--rw-r--r--   0 thomaslux   (501) staff       (20)     2078 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/procedure/og_procedure/procedure_c_to_f.f90
--rw-r--r--   0 thomaslux   (501) staff       (20)     1253 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/procedure/procedure.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-04-06 15:07:53.179335 fmodpy-1.5.7/fmodpy/test/real32/
--rw-r--r--   0 thomaslux   (501) staff       (20)     2261 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/real32/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     3368 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/real32/test_real32.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-04-06 15:07:53.179658 fmodpy-1.5.7/fmodpy/test/real64/
--rw-r--r--   0 thomaslux   (501) staff       (20)     2252 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/real64/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     3574 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/real64/test_real64.f03
--rw-r--r--   0 thomaslux   (501) staff       (20)     3690 2022-05-10 02:36:49.000000 fmodpy-1.5.7/fmodpy/test/test.py
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-04-06 15:07:53.180251 fmodpy-1.5.7/fmodpy/test/type/
--rw-r--r--   0 thomaslux   (501) staff       (20)     2934 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/type/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     1373 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/type/derived_type_error.f03
--rw-r--r--   0 thomaslux   (501) staff       (20)     4376 2022-03-18 19:21:33.000000 fmodpy-1.5.7/fmodpy/test/type/test_type.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-04-06 15:07:53.167335 fmodpy-1.5.7/fmodpy.egg-info/
--rw-r--r--   0 thomaslux   (501) staff       (20)      753 2023-04-06 15:07:53.000000 fmodpy-1.5.7/fmodpy.egg-info/PKG-INFO
--rw-r--r--   0 thomaslux   (501) staff       (20)     2571 2023-04-06 15:07:53.000000 fmodpy-1.5.7/fmodpy.egg-info/SOURCES.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)        1 2023-04-06 15:07:53.000000 fmodpy-1.5.7/fmodpy.egg-info/dependency_links.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)       12 2023-04-06 15:07:53.000000 fmodpy-1.5.7/fmodpy.egg-info/requires.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)        7 2023-04-06 15:07:53.000000 fmodpy-1.5.7/fmodpy.egg-info/top_level.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)      108 2023-04-06 15:07:53.180712 fmodpy-1.5.7/setup.cfg
--rw-r--r--   0 thomaslux   (501) staff       (20)     2652 2022-03-18 19:21:33.000000 fmodpy-1.5.7/setup.py
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-06-17 16:37:49.906573 fmodpy-1.6.0/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1072 2022-03-18 19:21:33.000000 fmodpy-1.6.0/LICENSE.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)       27 2022-07-26 13:43:21.000000 fmodpy-1.6.0/MANIFEST.in
+-rw-r--r--   0 thomaslux   (501) staff       (20)      753 2023-06-17 16:37:49.906638 fmodpy-1.6.0/PKG-INFO
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-06-17 16:37:49.893644 fmodpy-1.6.0/fmodpy/
+-rw-r--r--   0 thomaslux   (501) staff       (20)      658 2022-07-18 14:21:02.000000 fmodpy-1.6.0/fmodpy/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1148 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/__main__.py
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-06-17 16:37:49.895880 fmodpy-1.6.0/fmodpy/about/
+-rw-r--r--   0 thomaslux   (501) staff       (20)       47 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/about/author.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)      607 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/about/classifiers.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)       72 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/about/description.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)       31 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/about/keywords.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)        5 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/about/on_pypi.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)       12 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/about/requirements.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)        6 2023-06-17 16:37:35.000000 fmodpy-1.6.0/fmodpy/about/version.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)     4913 2023-06-17 16:37:47.000000 fmodpy-1.6.0/fmodpy/about/version_history.md
+-rw-r--r--   0 thomaslux   (501) staff       (20)    12323 2023-06-16 04:39:57.000000 fmodpy-1.6.0/fmodpy/config.py
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-06-17 16:37:49.896631 fmodpy-1.6.0/fmodpy/development/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1136 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/development/strange_type_example.f90
+-rw-r--r--   0 thomaslux   (501) staff       (20)     5060 2022-04-09 14:56:15.000000 fmodpy-1.6.0/fmodpy/development/todo.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)      874 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/development/type.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)      522 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/exceptions.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)    34638 2023-03-28 04:40:43.000000 fmodpy-1.6.0/fmodpy/fmodpy.py
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-06-17 16:37:49.900311 fmodpy-1.6.0/fmodpy/parsing/
+-rw-r--r--   0 thomaslux   (501) staff       (20)    10880 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/parsing/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2926 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/parsing/_old_code.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)    42722 2023-06-17 16:31:59.000000 fmodpy-1.6.0/fmodpy/parsing/argument.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1033 2023-06-17 15:43:32.000000 fmodpy-1.6.0/fmodpy/parsing/character.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)    13721 2023-06-17 15:13:11.000000 fmodpy-1.6.0/fmodpy/parsing/code.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1600 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/parsing/complex.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     6087 2023-06-11 23:32:55.000000 fmodpy-1.6.0/fmodpy/parsing/file.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2853 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/parsing/function.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)        0 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/parsing/implicit_none.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)      162 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/parsing/integer.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1563 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/parsing/interface.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)      950 2023-04-06 04:56:34.000000 fmodpy-1.6.0/fmodpy/parsing/logical.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     7614 2023-06-17 03:34:05.000000 fmodpy-1.6.0/fmodpy/parsing/module.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)      118 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/parsing/procedure.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)      160 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/parsing/real.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)    21105 2023-06-17 01:11:29.000000 fmodpy-1.6.0/fmodpy/parsing/subroutine.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     6315 2022-05-10 02:34:01.000000 fmodpy-1.6.0/fmodpy/parsing/type.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)        0 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/parsing/use.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     6810 2023-03-27 01:31:38.000000 fmodpy-1.6.0/fmodpy/parsing/util.py
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-06-17 16:37:49.900833 fmodpy-1.6.0/fmodpy/test/
+-rw-r--r--   0 thomaslux   (501) staff       (20)    53248 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/.coverage
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-06-17 16:37:49.901094 fmodpy-1.6.0/fmodpy/test/character/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1522 2023-06-17 16:32:35.000000 fmodpy-1.6.0/fmodpy/test/character/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)      807 2023-06-17 16:32:32.000000 fmodpy-1.6.0/fmodpy/test/character/test_character.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-06-17 16:37:49.901380 fmodpy-1.6.0/fmodpy/test/complex128/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2311 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/complex128/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     3655 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/complex128/test_complex128.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-06-17 16:37:49.901661 fmodpy-1.6.0/fmodpy/test/complex256/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2377 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/complex256/__init__.py
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-06-17 16:37:49.901954 fmodpy-1.6.0/fmodpy/test/complex256/test_complex256/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     7751 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/complex256/test_complex256/test_complex256_c_wrapper.f90
+-rw-r--r--   0 thomaslux   (501) staff       (20)    13250 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/complex256/test_complex256/test_complex256_python_wrapper.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     3978 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/complex256/test_complex256.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-06-17 16:37:49.902246 fmodpy-1.6.0/fmodpy/test/complex64/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2309 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/complex64/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     3655 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/complex64/test_complex64.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-06-17 16:37:49.902526 fmodpy-1.6.0/fmodpy/test/double_precision/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2252 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/double_precision/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     3626 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/double_precision/test_double_precision.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-06-17 16:37:49.902824 fmodpy-1.6.0/fmodpy/test/int32/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2256 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/int32/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     3411 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/int32/test_int32.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-06-17 16:37:49.903198 fmodpy-1.6.0/fmodpy/test/int64/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2427 2022-08-27 16:58:36.000000 fmodpy-1.6.0/fmodpy/test/int64/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     4008 2022-08-27 16:57:13.000000 fmodpy-1.6.0/fmodpy/test/int64/test_int64.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-06-17 16:37:49.903582 fmodpy-1.6.0/fmodpy/test/logical/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1435 2022-03-27 18:02:26.000000 fmodpy-1.6.0/fmodpy/test/logical/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)      663 2022-03-27 17:59:28.000000 fmodpy-1.6.0/fmodpy/test/logical/test_logical.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-06-17 16:37:49.904246 fmodpy-1.6.0/fmodpy/test/misc/
+-rw-r--r--   0 thomaslux   (501) staff       (20)      932 2022-05-10 02:37:20.000000 fmodpy-1.6.0/fmodpy/test/misc/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)      212 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/misc/implicit_shape.f90
+-rw-r--r--   0 thomaslux   (501) staff       (20)      271 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/misc/simple.f03
+-rw-r--r--   0 thomaslux   (501) staff       (20)      307 2022-05-10 02:24:48.000000 fmodpy-1.6.0/fmodpy/test/misc/subroutine_with_type.f90
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-06-17 16:37:49.904638 fmodpy-1.6.0/fmodpy/test/module/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     3173 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/module/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)      173 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/module/extra_module.f03
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1364 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/module/test_module.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-06-17 16:37:49.904929 fmodpy-1.6.0/fmodpy/test/procedure/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1134 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/procedure/__init__.py
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-06-17 16:37:49.905414 fmodpy-1.6.0/fmodpy/test/procedure/og_procedure/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1253 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/procedure/og_procedure/procedure.f03
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1624 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/procedure/og_procedure/procedure.pyx
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2078 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/procedure/og_procedure/procedure_c_to_f.f90
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1253 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/procedure/procedure.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-06-17 16:37:49.905737 fmodpy-1.6.0/fmodpy/test/real32/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2261 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/real32/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     3368 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/real32/test_real32.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-06-17 16:37:49.906034 fmodpy-1.6.0/fmodpy/test/real64/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2252 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/real64/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     3574 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/real64/test_real64.f03
+-rw-r--r--   0 thomaslux   (501) staff       (20)     3690 2022-05-10 02:36:49.000000 fmodpy-1.6.0/fmodpy/test/test.py
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-06-17 16:37:49.906444 fmodpy-1.6.0/fmodpy/test/type/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2934 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/type/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1373 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/type/derived_type_error.f03
+-rw-r--r--   0 thomaslux   (501) staff       (20)     4376 2022-03-18 19:21:33.000000 fmodpy-1.6.0/fmodpy/test/type/test_type.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2023-06-17 16:37:49.894611 fmodpy-1.6.0/fmodpy.egg-info/
+-rw-r--r--   0 thomaslux   (501) staff       (20)      753 2023-06-17 16:37:49.000000 fmodpy-1.6.0/fmodpy.egg-info/PKG-INFO
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2571 2023-06-17 16:37:49.000000 fmodpy-1.6.0/fmodpy.egg-info/SOURCES.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)        1 2023-06-17 16:37:49.000000 fmodpy-1.6.0/fmodpy.egg-info/dependency_links.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)       12 2023-06-17 16:37:49.000000 fmodpy-1.6.0/fmodpy.egg-info/requires.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)        7 2023-06-17 16:37:49.000000 fmodpy-1.6.0/fmodpy.egg-info/top_level.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)      108 2023-06-17 16:37:49.906953 fmodpy-1.6.0/setup.cfg
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2652 2022-03-18 19:21:33.000000 fmodpy-1.6.0/setup.py
```

### Comparing `fmodpy-1.5.7/LICENSE.txt` & `fmodpy-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/PKG-INFO` & `fmodpy-1.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fmodpy
-Version: 1.5.7
+Version: 1.6.0
 Summary: A lightweight, efficient, highly automated, fortran wrapper for python.
 Home-page: https://github.com/tchlux/fmodpy
-Download-URL: https://github.com/tchlux/fmodpy/archive/1.5.7.tar.gz
+Download-URL: https://github.com/tchlux/fmodpy/archive/1.6.0.tar.gz
 Author: Thomas C.H. Lux
 Author-email: thomas.ch.lux@gmail.com
 License: MIT
 Keywords: python,python3,fortran,wrapper
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `fmodpy-1.5.7/fmodpy/__init__.py` & `fmodpy-1.6.0/fmodpy/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/__main__.py` & `fmodpy-1.6.0/fmodpy/__main__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/about/classifiers.txt` & `fmodpy-1.6.0/fmodpy/about/classifiers.txt`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/about/version_history.md` & `fmodpy-1.6.0/fmodpy/about/version_history.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,7 +22,8 @@
 | 1.5.2<br>July 2022 | Added some additional standard library search paths <br> and renamed 'delete_destination' as 'overwrite'. <br> Also changed default configurations that were <br> strings being split into proper Python lists. |
 | 1.5.3<br>March 2023 | Minor update. Changed some logic in fimport to more <br> correctly support different system configurations. <br> Added comments drescribing most configurable <br> settings. Added support for TARGET and POINTER <br> types. |
 | 1.5.4<br>March 2023 | Added support for '$' as a line continuation <br> character in the fifth column of fixed format files. <br> Switched 'LOGICAL' types to be 'C_BOOL' |
 | 1.5.5<br>March 2023 | Updated error message for unnamed END statements to <br> include configuration suggestion. Made fixed format <br> Fortran files set 'end_is_named=False' by default. |
 | 1.5.6<br>March 2023 | Making some 'os.remove' operations safer by checking <br> for path existence. Refactored 'f_compiler_args' <br> into two more parts, 'optimization_level' and <br> 'shared_object_args', so that the typical '-fPIC <br> -shared' do not need to be included when adding <br> custom compilation arguments. |
 | 1.5.6<br>March 2023 | Making some 'os.remove' operations safer by checking <br> for path existence. Refactored 'f_compiler_args' <br> into two more parts, 'optimization_level' and <br> 'shared_object_args', so that the typical '-fPIC <br> -shared' do not need to be included when adding <br> custom compilation arguments. |
 | 1.5.7<br>April 2023 | Delayed warning message about LOGICAL arrays until <br> those arguments actually have a python interface <br> generated. This is to prevent parsed-but-unused <br> subroutine arguments from creating noise. |
+| 1.6.0<br>June 2023 | Added support for Fortran strings. Updated the <br> generated codes to automatically check for source <br> code modifications when loading and recompile if the <br> source code was modified. |
```

### Comparing `fmodpy-1.5.7/fmodpy/config.py` & `fmodpy-1.6.0/fmodpy/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 # File related maniplation arguments
 PY_EXT = ".py"
 FORT_EXT = ".f90"
 PYTHON_WRAPPER_EXT = "_python_wrapper"
 FORT_WRAPPER_EXT = "_c_wrapper"+FORT_EXT
 GET_SIZE_PROG_FILE = "fmodpy_get_size"+FORT_EXT
 GET_SIZE_EXEC_FILE = "fmodpy_get_size"
+GET_SIZE_VARIABLE_PREFIX = "SIZE_OF_"
 # --------------------------------------------------------------------
 
 # Automatically handle printing for status updates.
 #   WARNING: Do not use this function for warnings. Use `warnings.warn`.
 #   WARNING: Do not use this function for errors. Use `raise(...)`.
 # 
 # Custom print function (allows for line numbers to be automatically
```

### Comparing `fmodpy-1.5.7/fmodpy/development/strange_type_example.f90` & `fmodpy-1.6.0/fmodpy/development/strange_type_example.f90`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/development/todo.py` & `fmodpy-1.6.0/fmodpy/development/todo.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/development/type.py` & `fmodpy-1.6.0/fmodpy/development/type.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/exceptions.py` & `fmodpy-1.6.0/fmodpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/fmodpy.py` & `fmodpy-1.6.0/fmodpy/fmodpy.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/parsing/__init__.py` & `fmodpy-1.6.0/fmodpy/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/parsing/_old_code.txt` & `fmodpy-1.6.0/fmodpy/parsing/_old_code.txt`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/parsing/argument.py` & `fmodpy-1.6.0/fmodpy/parsing/argument.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,16 @@
     #          Fortran call will have an exact 1-1 mapping of arguments.
     def fort_call_name(self):
         name = self.name
         if (self.allocatable):
             name += "_LOCAL"
         elif (self.parent is not None) and (self.parent.name == self.name):
             name += "_RESULT"
+        elif ((self.type == "CHARACTER") and self.kind_prefix.startswith("LEN")):
+            name += "_STRING"
         return name
 
     # Names of arguments that will be given to the Fortran wrapper.
     def fort_input(self):
         names = []
         # Add a boolean "_PRESENT" for this variable if optional.
         if (self.optional):
@@ -120,23 +122,40 @@
         # If this is allocatable, it will be returned as an INT64 memory address.
         if self.allocatable:
             temp_arg.dimension = None
             temp_arg.intent = "OUT"
             temp_arg.show_intent = True
             temp_arg.type = "INTEGER"
             temp_arg.kind = "INT64"
+        # Make sure characters are passed as arrays.
+        if ((self.type == "CHARACTER") and self.kind_prefix.startswith("LEN")):
+            lines.append(f"INTEGER :: {self.name}_COPY_COUNTER")
+            lines.append(f"CHARACTER(LEN={self.name}_DIM_1) :: {self.name}_STRING")
+            temp_arg.kind_prefix = "KIND="
+            temp_arg.kind = ""
         # Add the actual definition of this argument.
         lines.append(str(temp_arg))
         # Reset the dimension, if it had one beforehand.
         if (self.dimension is not None): self.dimension = og_dimension
         # Return the lines of declaration.
         return lines
 
     # Lines of Fortran code that must be executed before the call.
-    def fort_prepare(self): return []
+    def fort_prepare(self):
+        lines = []
+        # Copy strings in to local variables from arrays.
+        is_input = ("IN" in self.intent) or (self.intent == "")
+        if ((self.type == "CHARACTER")
+            and self.kind_prefix.startswith("LEN")
+            and (is_input)
+        ):
+            lines.append(f"DO {self.name}_COPY_COUNTER = 1, SIZE({self.name},1)")
+            lines.append(f"  {self.name}_STRING({self.name}_COPY_COUNTER:{self.name}_COPY_COUNTER) = {self.name}({self.name}_COPY_COUNTER)")
+            lines.append(f"END DO")
+        return lines
 
     # Lines of Fortran code that must be executed after the call.
     def fort_after(self, present=True):
         lines = []
         is_output = ("OUT" in self.intent) or (self.intent == "")
         # Copy over the size of the output allocatable array if it was not known.
         if (is_output and self.allocatable):
@@ -145,14 +164,19 @@
                 if present: size = f"SIZE({self.function_safe_name()},{i})"
                 else:       size = "0"
                 lines.append(f"{self.name}_DIM_{i} = {size}")
             # Copy the allocatable address only when it is present.
             if present:
                 first_pos = ",".join(["1"]*len(self.dimension))
                 lines.append(f"{self.fort_input()[-1]} = LOC({self.function_safe_name()}({first_pos}))")
+        # Copy strings out back into character arrays.
+        if (is_output and (self.type == "CHARACTER") and self.kind_prefix.startswith("LEN")):
+            lines.append(f"DO {self.name}_COPY_COUNTER = 1, SIZE({self.name},1)")
+            lines.append(f"  {self.name}({self.name}_COPY_COUNTER) = {self.name}_STRING({self.name}_COPY_COUNTER:{self.name}_COPY_COUNTER)")
+            lines.append(f"END DO")
         # Return the list of lines.
         return lines
 
     # ----------------------------------------------------------------
     #                  Generating Python Wrapper
 
     # The names of arguments as seen in the Python function declaration.
@@ -219,14 +243,19 @@
             if self._is_optional(): p, s = f"el", "  "
             lines += [f"{p}if ((not issubclass(type({py_name}), numpy.ndarray)) or",
                       f"{s}    (not numpy.asarray({py_name}).flags.f_contiguous) or",
                       f"{s}    (not ({py_name}.dtype == numpy.dtype({self.c_type_array})))):",
                        "    import warnings",
                       f"    warnings.warn(\"The provided argument '{py_name}' was not an f_contiguous NumPy array of type '{self.c_type_array}' (or equivalent). Automatically converting (probably creating a full copy).\")",
                       f"    {py_name} = numpy.asarray({py_name}, dtype={self.c_type_array}, order='F')",]
+            # If this is a dimensioned CHARACTER, then remove the warning and ensure `.shape[0]` exists.
+            if (self.type == "CHARACTER"):
+                lines.pop(-2)
+                lines.pop(-2)
+                lines[-1] += ".reshape(-1)"
         # If this is an output-only allocatable, declare a local pointer.
         elif ((not self.optional) and self._is_output() and self.allocatable):
             lines.append(f"{py_name} = ctypes.c_void_p()")
         # Otherwise this an output immutable type, declare it locally.
         elif (not self._allowed_input()):
             lines.append(f"{py_name} = {self.c_type}()")
         # This is a singleton input, convert to appropraite C type.
@@ -277,16 +306,23 @@
             names[-1] = "ctypes.byref(" + names[-1] + ")"
         # Return the list of names.
         return names
 
     # The lines of Python code that must be executed after the Fortran call.
     def py_after(self):
         lines = []
+        py_name = self.name.lower()
+        # Handle characters with "LEN" by assuming it's one string.
+        if ((self.type == "CHARACTER")
+            and self.kind_prefix.startswith("LEN")
+            and self._is_output()
+        ):
+            lines += [f"{py_name} = ''.join({py_name}.astype(str))"]
+        # Handle allocatable arrays.
         if self.allocatable and self._is_output():
-            py_name = self.name.lower()
             # This must be an array argument and it must be 'INTENT(OUT)'.
             if (self.dimension is None): raise(NotImplementedError)
             # Get the pointer to the first index.
             local_dims = [f"{py_name}_dim_{i+1}.value" for i in range(len(self.dimension))]
             # Compute the size of the (flattened) array.
             lines += [f"{py_name}_size = ({') * ('.join(local_dims)})"]
             shape = ','.join(local_dims[::-1])
@@ -474,14 +510,17 @@
         else:
             first_pos = ",".join(["1"]*len(self.dimension))
             lines.append(f"{temp.name} = LOC({self.name}({first_pos}))")
         # Add indentation to all lints.
         lines = ["  "+l for l in lines]
         # Add the subroutine line (with all arguments).
         lines.insert(0, f"SUBROUTINE {self.parent.name}_GET_{self.name}({', '.join(args)}) BIND(C)")
+        # Assume that all needed types are in the parent.
+        if (self.type == "TYPE"):
+            lines.insert(1, f"  USE {self.parent.name}, ONLY: {self.kind}")
         # Add the end of the subroutine declaration line.
         lines.append(f"END SUBROUTINE {self.parent.name}_GET_{self.name}")
         return lines
 
     # Define the FORTRAN BIND(C) subroutine for setting the value
     # of this module attribute.
     def fort_setter(self):
@@ -512,14 +551,18 @@
             shape_str = ','.join([f'1:{name}' for name in temp.dimension])
             lines += [f'ALLOCATE({self.name}({shape_str}))']
         lines += [f"{self.name} = {temp.name}"]
         # Add indentation to all lints.
         lines = ["  "+l for l in lines]
         # Add the subroutine line (with all arguments).
         lines.insert(0, f"SUBROUTINE {self.parent.name}_SET_{self.name}({', '.join(args)}) BIND(C)")
+        # Assume that all needed types are in the parent.
+        if (self.type == "TYPE"):
+            lines.insert(1, f"  USE {self.parent.name}, ONLY: {self.kind}")
+        # Make sure self is used from parent too.
         lines.insert(1, f"  USE {self.parent.name}, ONLY: {self.name}")
         # Add the end of the subroutine declaration line.
         lines.append(f"END SUBROUTINE {self.parent.name}_SET_{self.name}")
         return lines
 
 
     # ----------------------------------------------------------------
@@ -572,14 +615,31 @@
     # from the assumed size of the object in Fortran.
     def _default_size(self):
         if (len(self._dimension_args()) != 0): raise(NotImplementedError)
         import re # <- use regular expressions to capture SIZE(...) syntax.
         sizes = []
         for size in self.dimension:
             size = size.lower().replace(" ","")
+            # Replace all occurrences of "LEN(<argument>)"
+            #  with a Python NumPy equivelent.
+            while "len(" in size:
+                start_index = size.index("len(") + len("len(")
+                before_call = size[:start_index-len("len(")]
+                parens = 1
+                for index in range(start_index, len(size)):
+                    if size[index] == "(": parens += 1
+                    elif size[index] == ")": parens -= 1
+                    if parens <= 0: break
+                argument = size[start_index:index]
+                after_call = size[index+len(")"):]
+                # Now "argument" contains whatever was inside the parenthesis
+                #  and passed into the `LEN(...)` function in Fortran.
+                argument = argument.strip()
+                # Replacement.
+                size = before_call + argument + ".shape[0]" + after_call
             # Replace all occurrences of "SIZE(<argument>)"
             #   with a Python NumPy equivalent array syntax.
             while "size(" in size:
                 start_index = size.index("size(") + len("size(")
                 before_call = size[:start_index-len("size(")]
                 parens = 1
                 for index in range(start_index, len(size)):
@@ -672,20 +732,26 @@
         if (line.pop(0) != self.type): raise(NotImplementedError)
         # Set the parent.
         self.parent = parent
         # If the line is empty now, then we're done (use defaults).
         if (len(line) == 0): return
         # Parse the remainder of the declaration line.
         # 
-        # Get the KIND declaration, if it was given.
+        # Get the KIND or LEN declaration, if it was given.
         group, line = pop_group(line)
         if (len(group) > 0):
-            if (tuple(group[:2]) == ("KIND","=")):
+            if (tuple(group[:2]) == ("LEN", "=")):
                 group = group[2:]
-            self.kind = " ".join(group)
+                self.kind_prefix = "LEN="
+                self.kind = " ".join(group)
+            else:
+                if (tuple(group[:2]) == ("KIND","=")):
+                    group = group[2:]
+                self.kind = " ".join(group)
+    
         # The rest can come in any order, so loop over possibilities.
         while (len(line) > 0):
             # Skip commas.
             if (line[0] == ","):
                 line.pop(0)
                 continue
             # The following happen if the ":: names" has not been stripped.
```

### Comparing `fmodpy-1.5.7/fmodpy/parsing/character.py` & `fmodpy-1.6.0/fmodpy/parsing/logical.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from .argument import Argument
 
-class Character(Argument):
-    type = "CHARACTER"
-    c_types = {"1":"ctypes.c_char"}
+class Logical(Argument):
+    type = "LOGICAL"
+    c_types = {"4":"ctypes.c_int", "1":"ctypes.c_bool"}
     default_singleton = "0"
 
-    # Add a warning about logical arrays.
+    # For array inputs of logicals, change the C-type to be an "int".
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         if (self.dimension is not None):
-            # TODO: Change the C-type of this character be a "uint8" for arrays.
-            # self.c_types = self.c_types.copy()
-            # self.c_types["1"] = "ctypes.c_char" # Needs to be uint8 in numpy.
-            # Show a warning to the user.
+            self.c_types = self.c_types.copy()
+            self.c_types["4"] = "ctypes.c_int"
+
+    # Add a warning about logical arrays.
+    def py_declare(self):
+        # Show a warning to the user for passing in logical array types.
+        if ((self.dimension is not None) and (self._allowed_input())):
             from fmodpy.config import show_warnings
             if show_warnings:
                 import warnings
-                warnings.warn("Fortran CHARACTER arrays are not supported yet. Raise an issue with an example to encourage development.")
+                warnings.warn("Fortran LOGICAL arrays must be given as 32-bit integers.")
+        # Return the usual function.
+        return super().py_declare()
+
```

### Comparing `fmodpy-1.5.7/fmodpy/parsing/code.py` & `fmodpy-1.6.0/fmodpy/parsing/code.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,54 +176,62 @@
             for instance in getattr(self, name):
                 if (hasattr(instance, "eval_sizes")):
                     instance.eval_sizes(build_dir)
         # After evaluating the sizes for all children, if this code object
         # has arguments inside of it, evaluate their sizes.
         if hasattr(self, "arguments"):
             # Evaluate the size of all arguments for this routine.
-            size_prog =  "PROGRAM GET_SIZE\n"
+            size_prog =  "PROGRAM GET_SIZE\n  USE ISO_C_BINDING, ONLY: C_SIZEOF\n"
             # Add a use line for the module this is in (if it is inside one).
             if (self.parent is not None):
                 # If the parent is a module, assume access to it with a USE.
                 if (self.parent.type == "MODULE"):
                     size_prog += f"  USE {self.parent.name}\n"
                 # Add any used modules by the parent (because this has access to those).
                 if (hasattr(self.parent, "uses")):
                     for line in self.parent.uses: size_prog += f"  {line}\n"
+            # If this is module, we might need to USE it to get PARAMETER values.
+            if (self.type == "MODULE"):
+                size_prog += f"  USE {self.name}\n"
 
             # # If this is a TYPE, then add the type declaration.
             # if (self.type == "TYPE"):
             #     size_prog += "\n".join(["  " + l for l in str(self).split("\n")]) + "\n"
 
             # If this is not a TYPE, then it might have USES statements.
             if hasattr(self, "uses"):
-                for line in sorted(self.uses): size_prog += line+"\n"
+                for line in sorted(self.uses): size_prog += f"  {line}\n"
             # Get the unique argument type:kind pairs, all arguments as values.
             unique_types_and_kinds = {}
             for arg in self.arguments:
                 # Skip "TYPE" arguments, their sizes are evaluated separately.
                 if (arg.type == "TYPE"): continue
-                # Append a unique identifier to "RESULT" for functions.
-                if (hasattr(self, "result") and (arg.name == self.name)):
-                    arg.name += "_result"
+                # Character arguments with "LEN" are size = 1.
+                if ((arg.type == "CHARACTER") and (arg.kind_prefix.startswith("LEN"))):
+                    arg.size = "1"
+                    continue
+                # Generate a unique lookup for this argument type and kind.
                 key = (arg.type,arg.kind)
                 unique_types_and_kinds[key] = unique_types_and_kinds.get(key,[]) + [arg]
+
+            from fmodpy.config import GET_SIZE_VARIABLE_PREFIX
             # Add all unique (type,kind) arguments to the size check program.
             for (t,k) in sorted(unique_types_and_kinds):
                 # Create a singleton argument of the same type to measure size.
                 arg = unique_types_and_kinds[(t,k)][0]
                 temp_arg = type(arg)([arg.type])
-                temp_arg.name = arg.function_safe_name()
+                temp_arg.name = GET_SIZE_VARIABLE_PREFIX + arg.function_safe_name()
+                temp_arg.kind_prefix = arg.kind_prefix
                 temp_arg.kind = arg.kind
                 temp_arg.show_intent = False
                 size_prog += f"  {temp_arg}\n"
             # Add print statements (printing the sizes).
             for k in sorted(unique_types_and_kinds):
-                name = unique_types_and_kinds[k][0].name
-                size_prog += f"  WRITE (*,*) SIZEOF({name})\n"
+                name = GET_SIZE_VARIABLE_PREFIX + unique_types_and_kinds[k][0].name
+                size_prog += f"  WRITE (*,*) C_SIZEOF({name})\n"
             # End the program file.
             size_prog += "END PROGRAM GET_SIZE\n"
             # Take the size program string and make sure all lines 
             #  fit within the expected character width.
             from fmodpy.parsing.util import wrap_long_lines
             size_prog = "\n".join(wrap_long_lines(size_prog.split("\n")))
             # Import some necessary configurations to make the SIZEOF program.
```

### Comparing `fmodpy-1.5.7/fmodpy/parsing/complex.py` & `fmodpy-1.6.0/fmodpy/parsing/complex.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/parsing/file.py` & `fmodpy-1.6.0/fmodpy/parsing/file.py`

 * *Files 13% similar despite different names*

```diff
@@ -77,14 +77,25 @@
                  '#               AUTO-COMPILING',
                  '#',
                  '# Try to import the prerequisite symbols for the compiled code.',
                  'for _ in _symbol_files:',
                  '    _ = ctypes.CDLL(os.path.join(_this_directory, _), mode=ctypes.RTLD_GLOBAL)',
                  '# Try to import the existing object. If that fails, recompile and then try.',
                  'try:',
+                 '    # Check to see if the source files have been modified and a recompilation is needed.',
+                 '    if (max(max([0]+[os.path.getmtime(os.path.realpath(os.path.join(_this_directory,_))) for _ in _symbol_files]),',
+                 '            max([0]+[os.path.getmtime(os.path.realpath(os.path.join(_this_directory,_))) for _ in _ordered_dependencies]))',
+                 '        > os.path.getmtime(_path_to_lib)):',
+                 '        print()',
+                 '        print("WARNING: Recompiling because the modification time of a source file is newer than the library.", flush=True)',
+                 '        print()',
+                 '        if os.path.exists(_path_to_lib):',
+                 '            os.remove(_path_to_lib)',
+                 '        raise NotImplementedError(f"The newest library code has not been compiled.")',
+                 '    # Import the library.',
                  '    clib = ctypes.CDLL(_path_to_lib)',
                  'except:',
                  '    # Remove the shared object if it exists, because it is faulty.',
                  '    if os.path.exists(_shared_object_name):',
                  '        os.remove(_shared_object_name)',
                  '    # Compile a new shared object.',
                  '    _command = " ".join([_fort_compiler] + _compile_options + ["-o", _shared_object_name] + _ordered_dependencies)',
```

### Comparing `fmodpy-1.5.7/fmodpy/parsing/function.py` & `fmodpy-1.6.0/fmodpy/parsing/function.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/parsing/interface.py` & `fmodpy-1.6.0/fmodpy/parsing/interface.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/parsing/module.py` & `fmodpy-1.6.0/fmodpy/parsing/module.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
                 for i in reversed(to_remove): codes.pop(i)
                 if (len(to_remove) > 0):
                     from fmodpy.config import fmodpy_print as print
                     print(f"  removed {len(to_remove)} from '{attr}' declared PRIVATE..")
         # Remove any things not declared public if this MODULE is private.
         if (self.status == "PRIVATE"):
             public = set(self.public)
-            for attr in ("interfaces","types","subroutines","functions"):
+            for attr in ("interfaces","types","subroutines","functions","arguments"):
                 codes = getattr(self,attr)
                 to_remove = [i for (i,c) in enumerate(codes) if (c.name not in public)]
                 for i in reversed(to_remove): codes.pop(i)
                 if (len(to_remove) > 0):
                     from fmodpy.config import fmodpy_print as print
                     print(f"  removed {len(to_remove)} from '{attr}' because this MODULE is PRIVATE..")
         # Make sure all "arguments" don't show intent.
```

### Comparing `fmodpy-1.5.7/fmodpy/parsing/subroutine.py` & `fmodpy-1.6.0/fmodpy/parsing/subroutine.py`

 * *Files identical despite different names*

```diff
@@ -174,14 +174,17 @@
         if any((a.allocatable and a._is_output()) for a in self.arguments):
             lines += ["  USE ISO_FORTRAN_ENV, ONLY: INT64"]
         if any(a._is_optional() for a in self.arguments):
             lines += ["  USE ISO_C_BINDING, ONLY: C_BOOL"]
         # Check if this is in a module.
         in_module = (self.parent is not None) and (self.parent.type == "MODULE")
         if (in_module): lines += [f"  USE {self.parent.name}, ONLY: {self.name}"]
+        # If this is module, we might need to USE it to get PARAMETER values.
+        if (self.type == "MODULE"):
+            lines += [f"  USE {self.name}"]
         # Add any type definitions from parents that are used here.
         known_types = {t.name for t in self.types}
         for l in self.uses:
             if (":" not in l): continue
             known_types |= {n.strip() for n in l.split(":")[-1].split(",")}
         needed_types = set()
         for a in self.arguments:
```

### Comparing `fmodpy-1.5.7/fmodpy/parsing/type.py` & `fmodpy-1.6.0/fmodpy/parsing/type.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/parsing/util.py` & `fmodpy-1.6.0/fmodpy/parsing/util.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/.coverage` & `fmodpy-1.6.0/fmodpy/test/.coverage`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/character/__init__.py` & `fmodpy-1.6.0/fmodpy/test/character/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,19 @@
     # Check for successful copy.
     result = fort.test_simple_character(a, b=out, c=ord('1'))
     assert(all(result.view('uint8') == a.view('uint8')))
     # Check for successful overwrite.
     result = fort.test_simple_character(a, b=out, c=ord('0'))
     assert(all(result.view('uint8') == [1, 2, 0, 1, 2, 0, 1, 2]))
 
+    # Check for string copy in and out correctly.
+    a = "abc"
+    b = fort.test_string(a)
+    assert(a == b)
+
     # End specific testing code.
     # ---------------------------------------------------------------
     print("passed", flush=True)
     import shutil
     shutil.rmtree(os.path.join(dir_name,f"test_{test_name}"))
 
 if __name__ == "__main__":
```

### Comparing `fmodpy-1.5.7/fmodpy/test/character/test_character.f03` & `fmodpy-1.6.0/fmodpy/test/character/test_character.f03`

 * *Files 20% similar despite different names*

```diff
@@ -11,9 +11,20 @@
         B(I) = A(I)
      ELSE
         B(I) = CHAR(MOD(I,3))
      END IF
   END DO
 END SUBROUTINE TEST_SIMPLE_CHARACTER
 
+
+SUBROUTINE TEST_STRING(A,B)
+  CHARACTER(LEN=*), INTENT(IN) :: A
+  CHARACTER(LEN=LEN(A)), INTENT(OUT) :: B
+  INTEGER :: I
+  DO I = 1, LEN(A)
+     B(I:I) = A(I:I)
+  END DO
+END SUBROUTINE TEST_STRING
+
+
 ! python3 -c "import fmodpy as f; f.fimport('simple_character.f03', build_dir='.', verbose=True)"
 ! python3 -c "import og_fmodpy as f; f.wrap('simple_character.f03', working_directory='og_fmodpy', verbose=True)"
```

### Comparing `fmodpy-1.5.7/fmodpy/test/complex128/__init__.py` & `fmodpy-1.6.0/fmodpy/test/complex128/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/complex128/test_complex128.f03` & `fmodpy-1.6.0/fmodpy/test/complex128/test_complex128.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/complex256/__init__.py` & `fmodpy-1.6.0/fmodpy/test/complex256/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/complex256/test_complex256/test_complex256_c_wrapper.f90` & `fmodpy-1.6.0/fmodpy/test/complex256/test_complex256/test_complex256_c_wrapper.f90`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/complex256/test_complex256/test_complex256_python_wrapper.py` & `fmodpy-1.6.0/fmodpy/test/complex256/test_complex256/test_complex256_python_wrapper.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/complex256/test_complex256.f03` & `fmodpy-1.6.0/fmodpy/test/complex256/test_complex256.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/complex64/__init__.py` & `fmodpy-1.6.0/fmodpy/test/complex64/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/complex64/test_complex64.f03` & `fmodpy-1.6.0/fmodpy/test/complex64/test_complex64.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/double_precision/__init__.py` & `fmodpy-1.6.0/fmodpy/test/double_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/double_precision/test_double_precision.f03` & `fmodpy-1.6.0/fmodpy/test/double_precision/test_double_precision.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/int32/__init__.py` & `fmodpy-1.6.0/fmodpy/test/int32/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/int32/test_int32.f03` & `fmodpy-1.6.0/fmodpy/test/int32/test_int32.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/int64/__init__.py` & `fmodpy-1.6.0/fmodpy/test/int64/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/int64/test_int64.f03` & `fmodpy-1.6.0/fmodpy/test/int64/test_int64.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/logical/__init__.py` & `fmodpy-1.6.0/fmodpy/test/logical/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/logical/test_logical.f03` & `fmodpy-1.6.0/fmodpy/test/logical/test_logical.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/misc/__init__.py` & `fmodpy-1.6.0/fmodpy/test/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/module/__init__.py` & `fmodpy-1.6.0/fmodpy/test/module/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/module/test_module.f03` & `fmodpy-1.6.0/fmodpy/test/module/test_module.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/procedure/__init__.py` & `fmodpy-1.6.0/fmodpy/test/procedure/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/procedure/og_procedure/procedure.f03` & `fmodpy-1.6.0/fmodpy/test/procedure/og_procedure/procedure.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/procedure/og_procedure/procedure.pyx` & `fmodpy-1.6.0/fmodpy/test/procedure/og_procedure/procedure.pyx`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/procedure/og_procedure/procedure_c_to_f.f90` & `fmodpy-1.6.0/fmodpy/test/procedure/og_procedure/procedure_c_to_f.f90`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/procedure/procedure.f03` & `fmodpy-1.6.0/fmodpy/test/procedure/procedure.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/real32/__init__.py` & `fmodpy-1.6.0/fmodpy/test/real32/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/real32/test_real32.f03` & `fmodpy-1.6.0/fmodpy/test/real32/test_real32.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/real64/__init__.py` & `fmodpy-1.6.0/fmodpy/test/real64/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/real64/test_real64.f03` & `fmodpy-1.6.0/fmodpy/test/real64/test_real64.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/test.py` & `fmodpy-1.6.0/fmodpy/test/test.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/type/__init__.py` & `fmodpy-1.6.0/fmodpy/test/type/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/type/derived_type_error.f03` & `fmodpy-1.6.0/fmodpy/test/type/derived_type_error.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy/test/type/test_type.f03` & `fmodpy-1.6.0/fmodpy/test/type/test_type.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/fmodpy.egg-info/PKG-INFO` & `fmodpy-1.6.0/fmodpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fmodpy
-Version: 1.5.7
+Version: 1.6.0
 Summary: A lightweight, efficient, highly automated, fortran wrapper for python.
 Home-page: https://github.com/tchlux/fmodpy
-Download-URL: https://github.com/tchlux/fmodpy/archive/1.5.7.tar.gz
+Download-URL: https://github.com/tchlux/fmodpy/archive/1.6.0.tar.gz
 Author: Thomas C.H. Lux
 Author-email: thomas.ch.lux@gmail.com
 License: MIT
 Keywords: python,python3,fortran,wrapper
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `fmodpy-1.5.7/fmodpy.egg-info/SOURCES.txt` & `fmodpy-1.6.0/fmodpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fmodpy-1.5.7/setup.py` & `fmodpy-1.6.0/setup.py`

 * *Files identical despite different names*

