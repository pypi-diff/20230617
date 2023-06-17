# Comparing `tmp/dustpy-1.0.4.tar.gz` & `tmp/dustpy-1.0.4rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dustpy-1.0.4.tar", last modified: Sat Jun 17 19:21:34 2023, max compression
+gzip compressed data, was "dustpy-1.0.4rc0.tar", last modified: Tue Jun 13 14:31:23 2023, max compression
```

## Comparing `dustpy-1.0.4.tar` & `dustpy-1.0.4rc0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:21:35.697560 dustpy-1.0.4/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    35149 2022-01-27 17:44:02.000000 dustpy-1.0.4/LICENSE
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      201 2022-07-01 12:14:11.000000 dustpy-1.0.4/MANIFEST.in
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     5178 2023-06-17 19:21:35.694559 dustpy-1.0.4/PKG-INFO
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     4000 2023-06-13 14:26:41.000000 dustpy-1.0.4/README.md
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:21:33.816451 dustpy-1.0.4/docs_source/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      816 2022-07-21 12:19:05.000000 dustpy-1.0.4/docs_source/Makefile
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      133 2023-06-13 14:26:44.000000 dustpy-1.0.4/docs_source/requirements.txt
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:21:33.906448 dustpy-1.0.4/docs_source/source/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      631 2022-01-27 17:44:05.000000 dustpy-1.0.4/docs_source/source/api.rst
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2053 2023-06-13 14:26:44.000000 dustpy-1.0.4/docs_source/source/conf.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1783 2023-06-13 14:26:44.000000 dustpy-1.0.4/docs_source/source/index.rst
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:21:33.957447 dustpy-1.0.4/dustpy/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1140 2023-06-17 19:21:19.000000 dustpy-1.0.4/dustpy/__init__.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:21:34.137476 dustpy-1.0.4/dustpy/constants/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1359 2022-01-27 17:44:05.000000 dustpy-1.0.4/dustpy/constants/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      692 2022-01-27 17:44:05.000000 dustpy-1.0.4/dustpy/constants/constants.f90
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:21:34.209485 dustpy-1.0.4/dustpy/plot/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      220 2022-01-27 17:44:05.000000 dustpy-1.0.4/dustpy/plot/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    21633 2023-02-07 12:39:58.000000 dustpy-1.0.4/dustpy/plot/plot.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    41733 2022-07-01 12:14:13.000000 dustpy-1.0.4/dustpy/simulation.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:21:34.499571 dustpy-1.0.4/dustpy/std/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      311 2022-01-27 17:44:05.000000 dustpy-1.0.4/dustpy/std/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    46670 2023-02-07 11:21:35.000000 dustpy-1.0.4/dustpy/std/dust.f90
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    26871 2023-02-07 11:21:35.000000 dustpy-1.0.4/dustpy/std/dust.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    18012 2023-06-13 14:26:44.000000 dustpy-1.0.4/dustpy/std/gas.f90
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    14014 2023-02-07 11:21:35.000000 dustpy-1.0.4/dustpy/std/gas.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      386 2022-01-27 17:44:05.000000 dustpy-1.0.4/dustpy/std/grid.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2076 2022-01-27 17:44:05.000000 dustpy-1.0.4/dustpy/std/sim.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      392 2022-01-27 17:44:05.000000 dustpy-1.0.4/dustpy/std/star.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:21:34.647572 dustpy-1.0.4/dustpy/utils/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      303 2022-01-27 17:44:05.000000 dustpy-1.0.4/dustpy/utils/__init__.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     4977 2022-01-27 17:44:05.000000 dustpy-1.0.4/dustpy/utils/boundary.py
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)      981 2022-01-27 17:44:05.000000 dustpy-1.0.4/dustpy/utils/interpolation.f90
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1276 2022-01-27 17:44:05.000000 dustpy-1.0.4/dustpy/utils/version.py
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:21:34.081443 dustpy-1.0.4/dustpy.egg-info/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     5178 2023-06-17 19:21:32.000000 dustpy-1.0.4/dustpy.egg-info/PKG-INFO
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1360 2023-06-17 19:21:33.000000 dustpy-1.0.4/dustpy.egg-info/SOURCES.txt
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2023-06-17 19:21:32.000000 dustpy-1.0.4/dustpy.egg-info/dependency_links.txt
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2022-07-01 12:33:16.000000 dustpy-1.0.4/dustpy.egg-info/not-zip-safe
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)       42 2023-06-17 19:21:33.000000 dustpy-1.0.4/dustpy.egg-info/requires.txt
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)        7 2023-06-17 19:21:33.000000 dustpy-1.0.4/dustpy.egg-info/top_level.txt
-drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-17 19:21:35.649558 dustpy-1.0.4/examples/
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)   500829 2023-06-13 14:26:44.000000 dustpy-1.0.4/examples/1_basics.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)   171323 2023-06-13 14:26:44.000000 dustpy-1.0.4/examples/2_simple_customization.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)   370912 2023-06-13 14:26:44.000000 dustpy-1.0.4/examples/3_advanced_customization.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)   108039 2023-06-13 14:26:44.000000 dustpy-1.0.4/examples/4_standard_model.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    32657 2023-06-13 14:26:44.000000 dustpy-1.0.4/examples/5_dust_coagulation.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    49744 2023-06-13 14:26:44.000000 dustpy-1.0.4/examples/6_dust_evolution.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)    31706 2023-06-13 14:26:44.000000 dustpy-1.0.4/examples/7_gas_evolution.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1944 2022-11-18 12:28:14.000000 dustpy-1.0.4/examples/A_citation.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     9143 2023-06-13 14:26:44.000000 dustpy-1.0.4/examples/B_publications.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2318 2022-07-21 12:19:06.000000 dustpy-1.0.4/examples/C_contrib_bug_feature.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1072 2022-07-21 12:19:06.000000 dustpy-1.0.4/examples/D_discussions.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     5123 2023-06-17 19:21:19.000000 dustpy-1.0.4/examples/E_changelog.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1085 2023-06-13 14:26:44.000000 dustpy-1.0.4/examples/dustpylib.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)   239326 2023-06-13 14:26:44.000000 dustpy-1.0.4/examples/example_ice_lines.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)   345145 2023-06-13 14:26:45.000000 dustpy-1.0.4/examples/example_planetary_gaps.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)   294442 2023-06-13 14:26:45.000000 dustpy-1.0.4/examples/example_planetesimal_formation.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)   621870 2023-06-13 14:26:45.000000 dustpy-1.0.4/examples/test_analytical_coagulation_kernels.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)   665624 2023-06-13 14:26:45.000000 dustpy-1.0.4/examples/test_gas_evolution.ipynb
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)       38 2023-06-17 19:21:35.698557 dustpy-1.0.4/setup.cfg
--rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3185 2022-01-27 17:44:05.000000 dustpy-1.0.4/setup.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-13 14:31:23.531147 dustpy-1.0.4rc0/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    35149 2022-01-27 17:44:02.000000 dustpy-1.0.4rc0/LICENSE
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      201 2022-07-01 12:14:11.000000 dustpy-1.0.4rc0/MANIFEST.in
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     5181 2023-06-13 14:31:23.525138 dustpy-1.0.4rc0/PKG-INFO
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     4000 2023-06-13 14:26:41.000000 dustpy-1.0.4rc0/README.md
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-13 14:31:21.295041 dustpy-1.0.4rc0/docs_source/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      816 2022-07-21 12:19:05.000000 dustpy-1.0.4rc0/docs_source/Makefile
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      133 2023-06-13 14:26:44.000000 dustpy-1.0.4rc0/docs_source/requirements.txt
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-13 14:31:21.430032 dustpy-1.0.4rc0/docs_source/source/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      631 2022-01-27 17:44:05.000000 dustpy-1.0.4rc0/docs_source/source/api.rst
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2053 2023-06-13 14:26:44.000000 dustpy-1.0.4rc0/docs_source/source/conf.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1783 2023-06-13 14:26:44.000000 dustpy-1.0.4rc0/docs_source/source/index.rst
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-13 14:31:21.515038 dustpy-1.0.4rc0/dustpy/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1143 2023-06-13 14:29:29.000000 dustpy-1.0.4rc0/dustpy/__init__.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-13 14:31:21.867045 dustpy-1.0.4rc0/dustpy/constants/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1359 2022-01-27 17:44:05.000000 dustpy-1.0.4rc0/dustpy/constants/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      692 2022-01-27 17:44:05.000000 dustpy-1.0.4rc0/dustpy/constants/constants.f90
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-13 14:31:21.965036 dustpy-1.0.4rc0/dustpy/plot/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      220 2022-01-27 17:44:05.000000 dustpy-1.0.4rc0/dustpy/plot/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    21633 2023-02-07 12:39:58.000000 dustpy-1.0.4rc0/dustpy/plot/plot.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    41733 2022-07-01 12:14:13.000000 dustpy-1.0.4rc0/dustpy/simulation.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-13 14:31:22.422883 dustpy-1.0.4rc0/dustpy/std/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      311 2022-01-27 17:44:05.000000 dustpy-1.0.4rc0/dustpy/std/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    46670 2023-02-07 11:21:35.000000 dustpy-1.0.4rc0/dustpy/std/dust.f90
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    26871 2023-02-07 11:21:35.000000 dustpy-1.0.4rc0/dustpy/std/dust.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    18012 2023-06-13 14:26:44.000000 dustpy-1.0.4rc0/dustpy/std/gas.f90
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    14014 2023-02-07 11:21:35.000000 dustpy-1.0.4rc0/dustpy/std/gas.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      386 2022-01-27 17:44:05.000000 dustpy-1.0.4rc0/dustpy/std/grid.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2076 2022-01-27 17:44:05.000000 dustpy-1.0.4rc0/dustpy/std/sim.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      392 2022-01-27 17:44:05.000000 dustpy-1.0.4rc0/dustpy/std/star.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-13 14:31:22.676142 dustpy-1.0.4rc0/dustpy/utils/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      303 2022-01-27 17:44:05.000000 dustpy-1.0.4rc0/dustpy/utils/__init__.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     4977 2022-01-27 17:44:05.000000 dustpy-1.0.4rc0/dustpy/utils/boundary.py
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)      981 2022-01-27 17:44:05.000000 dustpy-1.0.4rc0/dustpy/utils/interpolation.f90
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1276 2022-01-27 17:44:05.000000 dustpy-1.0.4rc0/dustpy/utils/version.py
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-13 14:31:21.785040 dustpy-1.0.4rc0/dustpy.egg-info/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     5181 2023-06-13 14:31:19.000000 dustpy-1.0.4rc0/dustpy.egg-info/PKG-INFO
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1360 2023-06-13 14:31:20.000000 dustpy-1.0.4rc0/dustpy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2023-06-13 14:31:19.000000 dustpy-1.0.4rc0/dustpy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)        1 2022-07-01 12:33:16.000000 dustpy-1.0.4rc0/dustpy.egg-info/not-zip-safe
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)       42 2023-06-13 14:31:19.000000 dustpy-1.0.4rc0/dustpy.egg-info/requires.txt
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)        7 2023-06-13 14:31:19.000000 dustpy-1.0.4rc0/dustpy.egg-info/top_level.txt
+drwxrwxrwx   0 stammler  (1000) stammler  (1000)        0 2023-06-13 14:31:23.446140 dustpy-1.0.4rc0/examples/
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)   500829 2023-06-13 14:26:44.000000 dustpy-1.0.4rc0/examples/1_basics.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)   171323 2023-06-13 14:26:44.000000 dustpy-1.0.4rc0/examples/2_simple_customization.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)   370912 2023-06-13 14:26:44.000000 dustpy-1.0.4rc0/examples/3_advanced_customization.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)   108039 2023-06-13 14:26:44.000000 dustpy-1.0.4rc0/examples/4_standard_model.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    32657 2023-06-13 14:26:44.000000 dustpy-1.0.4rc0/examples/5_dust_coagulation.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    49744 2023-06-13 14:26:44.000000 dustpy-1.0.4rc0/examples/6_dust_evolution.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)    31706 2023-06-13 14:26:44.000000 dustpy-1.0.4rc0/examples/7_gas_evolution.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1944 2022-11-18 12:28:14.000000 dustpy-1.0.4rc0/examples/A_citation.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     9143 2023-06-13 14:26:44.000000 dustpy-1.0.4rc0/examples/B_publications.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     2318 2022-07-21 12:19:06.000000 dustpy-1.0.4rc0/examples/C_contrib_bug_feature.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1072 2022-07-21 12:19:06.000000 dustpy-1.0.4rc0/examples/D_discussions.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     4636 2023-06-13 14:26:44.000000 dustpy-1.0.4rc0/examples/E_changelog.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     1085 2023-06-13 14:26:44.000000 dustpy-1.0.4rc0/examples/dustpylib.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)   239326 2023-06-13 14:26:44.000000 dustpy-1.0.4rc0/examples/example_ice_lines.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)   345145 2023-06-13 14:26:45.000000 dustpy-1.0.4rc0/examples/example_planetary_gaps.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)   294442 2023-06-13 14:26:45.000000 dustpy-1.0.4rc0/examples/example_planetesimal_formation.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)   621870 2023-06-13 14:26:45.000000 dustpy-1.0.4rc0/examples/test_analytical_coagulation_kernels.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)   665624 2023-06-13 14:26:45.000000 dustpy-1.0.4rc0/examples/test_gas_evolution.ipynb
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)       38 2023-06-13 14:31:23.533137 dustpy-1.0.4rc0/setup.cfg
+-rwxrwxrwx   0 stammler  (1000) stammler  (1000)     3185 2022-01-27 17:44:05.000000 dustpy-1.0.4rc0/setup.py
```

### Comparing `dustpy-1.0.4/LICENSE` & `dustpy-1.0.4rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/PKG-INFO` & `dustpy-1.0.4rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dustpy
-Version: 1.0.4
+Version: 1.0.4rc0
 Summary: Dust evolution in protoplanetary disks
 Home-page: https://github.com/stammler/dustpy
 Author: Sebastian Stammler, Til Birnstiel
 Author-email: sebastian.stammler@gmail.com, til.birnstiel@lmu.de
 Maintainer: Sebastian Stammler
 License: GPLv3
 Project-URL: Source Code, https://github.com/stammler/dustpy/
```

### Comparing `dustpy-1.0.4/README.md` & `dustpy-1.0.4rc0/README.md`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/docs_source/Makefile` & `dustpy-1.0.4rc0/docs_source/Makefile`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/docs_source/source/api.rst` & `dustpy-1.0.4rc0/docs_source/source/api.rst`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/docs_source/source/conf.py` & `dustpy-1.0.4rc0/docs_source/source/conf.py`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/docs_source/source/index.rst` & `dustpy-1.0.4rc0/docs_source/source/index.rst`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/dustpy/__init__.py` & `dustpy-1.0.4rc0/dustpy/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from dustpy import constants
 from dustpy import utils
 from dustpy.utils import hdf5writer
 
 from simframe.io.dump import readdump
 
 __name__ = "dustpy"
-__version__ = "1.0.4"
+__version__ = "1.0.4rc0"
 
 Simulation.__version__ = __version__
 plot.__version__ = __version__
 utils.__version__ = __version__
 
 __all__ = ["constants", "hdf5writer", "plot", "readdump", "Simulation"]
```

### Comparing `dustpy-1.0.4/dustpy/constants/__init__.py` & `dustpy-1.0.4rc0/dustpy/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/dustpy/constants/constants.f90` & `dustpy-1.0.4rc0/dustpy/constants/constants.f90`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/dustpy/plot/plot.py` & `dustpy-1.0.4rc0/dustpy/plot/plot.py`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/dustpy/simulation.py` & `dustpy-1.0.4rc0/dustpy/simulation.py`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/dustpy/std/dust.f90` & `dustpy-1.0.4rc0/dustpy/std/dust.f90`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/dustpy/std/dust.py` & `dustpy-1.0.4rc0/dustpy/std/dust.py`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/dustpy/std/gas.f90` & `dustpy-1.0.4rc0/dustpy/std/gas.f90`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/dustpy/std/gas.py` & `dustpy-1.0.4rc0/dustpy/std/gas.py`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/dustpy/std/sim.py` & `dustpy-1.0.4rc0/dustpy/std/sim.py`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/dustpy/utils/boundary.py` & `dustpy-1.0.4rc0/dustpy/utils/boundary.py`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/dustpy/utils/interpolation.f90` & `dustpy-1.0.4rc0/dustpy/utils/interpolation.f90`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/dustpy/utils/version.py` & `dustpy-1.0.4rc0/dustpy/utils/version.py`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/dustpy.egg-info/PKG-INFO` & `dustpy-1.0.4rc0/dustpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dustpy
-Version: 1.0.4
+Version: 1.0.4rc0
 Summary: Dust evolution in protoplanetary disks
 Home-page: https://github.com/stammler/dustpy
 Author: Sebastian Stammler, Til Birnstiel
 Author-email: sebastian.stammler@gmail.com, til.birnstiel@lmu.de
 Maintainer: Sebastian Stammler
 License: GPLv3
 Project-URL: Source Code, https://github.com/stammler/dustpy/
```

### Comparing `dustpy-1.0.4/dustpy.egg-info/SOURCES.txt` & `dustpy-1.0.4rc0/dustpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/examples/1_basics.ipynb` & `dustpy-1.0.4rc0/examples/1_basics.ipynb`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/examples/2_simple_customization.ipynb` & `dustpy-1.0.4rc0/examples/2_simple_customization.ipynb`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/examples/3_advanced_customization.ipynb` & `dustpy-1.0.4rc0/examples/3_advanced_customization.ipynb`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/examples/4_standard_model.ipynb` & `dustpy-1.0.4rc0/examples/4_standard_model.ipynb`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/examples/5_dust_coagulation.ipynb` & `dustpy-1.0.4rc0/examples/5_dust_coagulation.ipynb`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/examples/6_dust_evolution.ipynb` & `dustpy-1.0.4rc0/examples/6_dust_evolution.ipynb`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/examples/7_gas_evolution.ipynb` & `dustpy-1.0.4rc0/examples/7_gas_evolution.ipynb`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/examples/A_citation.ipynb` & `dustpy-1.0.4rc0/examples/A_citation.ipynb`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/examples/B_publications.ipynb` & `dustpy-1.0.4rc0/examples/B_publications.ipynb`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/examples/C_contrib_bug_feature.ipynb` & `dustpy-1.0.4rc0/examples/C_contrib_bug_feature.ipynb`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/examples/D_discussions.ipynb` & `dustpy-1.0.4rc0/examples/D_discussions.ipynb`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/examples/E_changelog.ipynb` & `dustpy-1.0.4rc0/examples/E_changelog.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9799107142857143%*

 * *Differences: {"'cells'": '{delete: [2]}', "'metadata'": "{'language_info': {'version': '3.10.11'}}"}*

```diff
@@ -14,27 +14,14 @@
             "metadata": {},
             "source": [
                 "This is a list of changes made to `DustPy` since version `v1.0.0` including discussions of their influence on the simulations."
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "9395dfc3-8a57-4382-a997-6aedc776963c",
-            "metadata": {},
-            "source": [
-                "### **v1.0.4**\n",
-                "**Release date: 17th June 2023**\n",
-                "\n",
-                "#### Bugfix to boundary conditions\n",
-                "\n",
-                "A bug prevented the boundaries to be set correctly for the boundary conditions `\"val\"`, `\"grad\"`, and `\"pow\"`. The boundary conditions `\"const_val\"`, `\"const_grad\"`, and `\"const_pow\"` were not affected by this bug."
-            ]
-        },
-        {
-            "cell_type": "markdown",
             "id": "c28673a5-03a9-4865-8d86-092a4cfca918",
             "metadata": {},
             "source": [
                 "### **v1.0.3**\n",
                 "**Release date: 7th February 2023**\n",
                 "\n",
                 "#### Correction to inital particle size distribution\n",
@@ -105,13 +92,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.3"
+            "version": "3.10.11"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `dustpy-1.0.4/examples/dustpylib.ipynb` & `dustpy-1.0.4rc0/examples/dustpylib.ipynb`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/examples/example_ice_lines.ipynb` & `dustpy-1.0.4rc0/examples/example_ice_lines.ipynb`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/examples/example_planetary_gaps.ipynb` & `dustpy-1.0.4rc0/examples/example_planetary_gaps.ipynb`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/examples/example_planetesimal_formation.ipynb` & `dustpy-1.0.4rc0/examples/example_planetesimal_formation.ipynb`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/examples/test_analytical_coagulation_kernels.ipynb` & `dustpy-1.0.4rc0/examples/test_analytical_coagulation_kernels.ipynb`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/examples/test_gas_evolution.ipynb` & `dustpy-1.0.4rc0/examples/test_gas_evolution.ipynb`

 * *Files identical despite different names*

### Comparing `dustpy-1.0.4/setup.py` & `dustpy-1.0.4rc0/setup.py`

 * *Files identical despite different names*

