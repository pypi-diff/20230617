# Comparing `tmp/hylite-1.21.tar.gz` & `tmp/hylite-1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hylite-1.21.tar", last modified: Fri Aug  5 20:47:18 2022, max compression
+gzip compressed data, was "hylite-1.23.tar", last modified: Sat Jun 17 06:54:28 2023, max compression
```

## Comparing `hylite-1.21.tar` & `hylite-1.23.tar`

### file list

```diff
@@ -1,124 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 20:47:18.752070 hylite-1.21/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-08-05 20:47:04.000000 hylite-1.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      938 2022-08-05 20:47:18.752070 hylite-1.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6356 2022-08-05 20:47:04.000000 hylite-1.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 20:47:18.732070 hylite-1.21/hylite/
--rw-r--r--   0 runner    (1001) docker     (121)     4421 2022-08-05 20:47:04.000000 hylite-1.21/hylite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 20:47:18.732070 hylite-1.21/hylite/analyse/
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-08-05 20:47:04.000000 hylite-1.21/hylite/analyse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1728 2022-08-05 20:47:04.000000 hylite-1.21/hylite/analyse/dtree.py
--rw-r--r--   0 runner    (1001) docker     (121)     4876 2022-08-05 20:47:04.000000 hylite-1.21/hylite/analyse/indices.py
--rw-r--r--   0 runner    (1001) docker     (121)    47134 2022-08-05 20:47:04.000000 hylite-1.21/hylite/analyse/mwl.py
--rw-r--r--   0 runner    (1001) docker     (121)     2218 2022-08-05 20:47:04.000000 hylite-1.21/hylite/analyse/sam.py
--rw-r--r--   0 runner    (1001) docker     (121)     4135 2022-08-05 20:47:04.000000 hylite-1.21/hylite/analyse/supervised.py
--rw-r--r--   0 runner    (1001) docker     (121)     2065 2022-08-05 20:47:04.000000 hylite-1.21/hylite/analyse/unsupervised.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 20:47:18.732070 hylite-1.21/hylite/correct/
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-08-05 20:47:04.000000 hylite-1.21/hylite/correct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4146 2022-08-05 20:47:04.000000 hylite-1.21/hylite/correct/detrend.py
--rw-r--r--   0 runner    (1001) docker     (121)     3220 2022-08-05 20:47:04.000000 hylite-1.21/hylite/correct/equalize.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 20:47:18.732070 hylite-1.21/hylite/correct/illumination/
--rw-r--r--   0 runner    (1001) docker     (121)    27868 2022-08-05 20:47:04.000000 hylite-1.21/hylite/correct/illumination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1627 2022-08-05 20:47:04.000000 hylite-1.21/hylite/correct/illumination/occlusion.py
--rw-r--r--   0 runner    (1001) docker     (121)     4573 2022-08-05 20:47:04.000000 hylite-1.21/hylite/correct/illumination/path.py
--rw-r--r--   0 runner    (1001) docker     (121)     4335 2022-08-05 20:47:04.000000 hylite-1.21/hylite/correct/illumination/reflection.py
--rw-r--r--   0 runner    (1001) docker     (121)    19645 2022-08-05 20:47:04.000000 hylite-1.21/hylite/correct/panel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 20:47:18.732070 hylite-1.21/hylite/filter/
--rw-r--r--   0 runner    (1001) docker     (121)     1599 2022-08-05 20:47:04.000000 hylite-1.21/hylite/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2785 2022-08-05 20:47:04.000000 hylite-1.21/hylite/filter/combine.py
--rw-r--r--   0 runner    (1001) docker     (121)     9863 2022-08-05 20:47:04.000000 hylite-1.21/hylite/filter/dimension_reduction.py
--rw-r--r--   0 runner    (1001) docker     (121)     5517 2022-08-05 20:47:04.000000 hylite-1.21/hylite/filter/sample.py
--rw-r--r--   0 runner    (1001) docker     (121)    25600 2022-08-05 20:47:04.000000 hylite-1.21/hylite/filter/segment.py
--rw-r--r--   0 runner    (1001) docker     (121)    10873 2022-08-05 20:47:04.000000 hylite-1.21/hylite/filter/tpt.py
--rw-r--r--   0 runner    (1001) docker     (121)    33567 2022-08-05 20:47:04.000000 hylite-1.21/hylite/hycloud.py
--rw-r--r--   0 runner    (1001) docker     (121)    15632 2022-08-05 20:47:04.000000 hylite-1.21/hylite/hycollection.py
--rw-r--r--   0 runner    (1001) docker     (121)    38953 2022-08-05 20:47:04.000000 hylite-1.21/hylite/hydata.py
--rw-r--r--   0 runner    (1001) docker     (121)    12504 2022-08-05 20:47:04.000000 hylite-1.21/hylite/hyfeature.py
--rw-r--r--   0 runner    (1001) docker     (121)    18321 2022-08-05 20:47:04.000000 hylite-1.21/hylite/hyheader.py
--rw-r--r--   0 runner    (1001) docker     (121)    35957 2022-08-05 20:47:04.000000 hylite-1.21/hylite/hyimage.py
--rw-r--r--   0 runner    (1001) docker     (121)    23458 2022-08-05 20:47:04.000000 hylite-1.21/hylite/hylibrary.py
--rw-r--r--   0 runner    (1001) docker     (121)    38362 2022-08-05 20:47:04.000000 hylite-1.21/hylite/hyscene.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 20:47:18.736070 hylite-1.21/hylite/io/
--rw-r--r--   0 runner    (1001) docker     (121)     7957 2022-08-05 20:47:04.000000 hylite-1.21/hylite/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2963 2022-08-05 20:47:04.000000 hylite-1.21/hylite/io/cameras.py
--rw-r--r--   0 runner    (1001) docker     (121)    15931 2022-08-05 20:47:04.000000 hylite-1.21/hylite/io/clouds.py
--rw-r--r--   0 runner    (1001) docker     (121)     7721 2022-08-05 20:47:04.000000 hylite-1.21/hylite/io/headers.py
--rw-r--r--   0 runner    (1001) docker     (121)    10437 2022-08-05 20:47:04.000000 hylite-1.21/hylite/io/images.py
--rw-r--r--   0 runner    (1001) docker     (121)    10894 2022-08-05 20:47:04.000000 hylite-1.21/hylite/io/libraries.py
--rw-r--r--   0 runner    (1001) docker     (121)     1800 2022-08-05 20:47:04.000000 hylite-1.21/hylite/io/pmaps.py
--rw-r--r--   0 runner    (1001) docker     (121)    10576 2022-08-05 20:47:04.000000 hylite-1.21/hylite/multiprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 20:47:18.736070 hylite-1.21/hylite/project/
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-08-05 20:47:04.000000 hylite-1.21/hylite/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24738 2022-08-05 20:47:04.000000 hylite-1.21/hylite/project/align.py
--rw-r--r--   0 runner    (1001) docker     (121)    16501 2022-08-05 20:47:04.000000 hylite-1.21/hylite/project/basic.py
--rw-r--r--   0 runner    (1001) docker     (121)     3248 2022-08-05 20:47:04.000000 hylite-1.21/hylite/project/camera.py
--rw-r--r--   0 runner    (1001) docker     (121)    34768 2022-08-05 20:47:04.000000 hylite-1.21/hylite/project/pmap.py
--rw-r--r--   0 runner    (1001) docker     (121)    29673 2022-08-05 20:47:04.000000 hylite-1.21/hylite/project/pushbroom.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 20:47:18.736070 hylite-1.21/hylite/reference/
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-08-05 20:47:04.000000 hylite-1.21/hylite/reference/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 20:47:18.736070 hylite-1.21/hylite/reference/features/
--rw-r--r--   0 runner    (1001) docker     (121)     6480 2022-08-05 20:47:04.000000 hylite-1.21/hylite/reference/features/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 20:47:18.736070 hylite-1.21/hylite/reference/spectra/
--rw-r--r--   0 runner    (1001) docker     (121)     3730 2022-08-05 20:47:04.000000 hylite-1.21/hylite/reference/spectra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 20:47:18.736070 hylite-1.21/hylite/reference/spectra/custom/
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-08-05 20:47:04.000000 hylite-1.21/hylite/reference/spectra/custom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 20:47:18.736070 hylite-1.21/hylite/reference/spectra/pvc/
--rw-r--r--   0 runner    (1001) docker     (121)    20987 2022-08-05 20:47:04.000000 hylite-1.21/hylite/reference/spectra/pvc/PVC_Black.txt
--rw-r--r--   0 runner    (1001) docker     (121)    20987 2022-08-05 20:47:04.000000 hylite-1.21/hylite/reference/spectra/pvc/PVC_Grey.txt
--rw-r--r--   0 runner    (1001) docker     (121)    20987 2022-08-05 20:47:04.000000 hylite-1.21/hylite/reference/spectra/pvc/PVC_Red.txt
--rw-r--r--   0 runner    (1001) docker     (121)    20987 2022-08-05 20:47:04.000000 hylite-1.21/hylite/reference/spectra/pvc/PVC_White.txt
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-08-05 20:47:04.000000 hylite-1.21/hylite/reference/spectra/pvc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 20:47:18.736070 hylite-1.21/hylite/reference/spectra/spectralon/
--rw-r--r--   0 runner    (1001) docker     (121)    45471 2022-08-05 20:47:04.000000 hylite-1.21/hylite/reference/spectra/spectralon/R50.txt
--rw-r--r--   0 runner    (1001) docker     (121)    47694 2022-08-05 20:47:04.000000 hylite-1.21/hylite/reference/spectra/spectralon/R55_SiSu.txt
--rw-r--r--   0 runner    (1001) docker     (121)    45471 2022-08-05 20:47:04.000000 hylite-1.21/hylite/reference/spectra/spectralon/R6.txt
--rw-r--r--   0 runner    (1001) docker     (121)    45492 2022-08-05 20:47:04.000000 hylite-1.21/hylite/reference/spectra/spectralon/R90.txt
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-08-05 20:47:04.000000 hylite-1.21/hylite/reference/spectra/spectralon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 20:47:18.740070 hylite-1.21/hylite/sensors/
--rw-r--r--   0 runner    (1001) docker     (121)     4095 2022-08-05 20:47:04.000000 hylite-1.21/hylite/sensors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 20:47:18.740070 hylite-1.21/hylite/sensors/calibration_data/
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-05 20:47:04.000000 hylite-1.21/hylite/sensors/calibration_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 20:47:18.740070 hylite-1.21/hylite/sensors/calibration_data/fenix/
--rw-r--r--   0 runner    (1001) docker     (121)   958464 2022-08-05 20:47:04.000000 hylite-1.21/hylite/sensors/calibration_data/fenix/Radiometric_2x2_1x1.dat
--rw-r--r--   0 runner    (1001) docker     (121)    10164 2022-08-05 20:47:04.000000 hylite-1.21/hylite/sensors/calibration_data/fenix/Radiometric_2x2_1x1.hdr
--rw-r--r--   0 runner    (1001) docker     (121)   691200 2022-08-05 20:47:04.000000 hylite-1.21/hylite/sensors/calibration_data/fenix/Radiometric_4x2_1x1.dat
--rw-r--r--   0 runner    (1001) docker     (121)     7777 2022-08-05 20:47:04.000000 hylite-1.21/hylite/sensors/calibration_data/fenix/Radiometric_4x2_1x1.hdr
--rw-r--r--   0 runner    (1001) docker     (121)   557568 2022-08-05 20:47:04.000000 hylite-1.21/hylite/sensors/calibration_data/fenix/Radiometric_8x2_1x1.dat
--rw-r--r--   0 runner    (1001) docker     (121)     6573 2022-08-05 20:47:04.000000 hylite-1.21/hylite/sensors/calibration_data/fenix/Radiometric_8x2_1x1.hdr
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-05 20:47:04.000000 hylite-1.21/hylite/sensors/calibration_data/fenix/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 20:47:18.748070 hylite-1.21/hylite/sensors/calibration_data/fenix1k/
--rwxr-xr-x   0 runner    (1001) docker     (121)  2449408 2022-08-05 20:47:04.000000 hylite-1.21/hylite/sensors/calibration_data/fenix1k/Radiometric_2x2_1x1.dat
--rwxr-xr-x   0 runner    (1001) docker     (121)     9738 2022-08-05 20:47:04.000000 hylite-1.21/hylite/sensors/calibration_data/fenix1k/Radiometric_2x2_1x1.hdr
--rwxr-xr-x   0 runner    (1001) docker     (121)  1728512 2022-08-05 20:47:04.000000 hylite-1.21/hylite/sensors/calibration_data/fenix1k/Radiometric_4x2_1x1.dat
--rwxr-xr-x   0 runner    (1001) docker     (121)     7339 2022-08-05 20:47:04.000000 hylite-1.21/hylite/sensors/calibration_data/fenix1k/Radiometric_4x2_1x1.hdr
--rwxr-xr-x   0 runner    (1001) docker     (121)  1368064 2022-08-05 20:47:04.000000 hylite-1.21/hylite/sensors/calibration_data/fenix1k/Radiometric_8x2_1x1.dat
--rwxr-xr-x   0 runner    (1001) docker     (121)     6124 2022-08-05 20:47:04.000000 hylite-1.21/hylite/sensors/calibration_data/fenix1k/Radiometric_8x2_1x1.hdr
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-08-05 20:47:04.000000 hylite-1.21/hylite/sensors/calibration_data/fenix1k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    66214 2022-08-05 20:47:04.000000 hylite-1.21/hylite/sensors/fenix.py
--rw-r--r--   0 runner    (1001) docker     (121)    10472 2022-08-05 20:47:04.000000 hylite-1.21/hylite/sensors/fx.py
--rw-r--r--   0 runner    (1001) docker     (121)     6974 2022-08-05 20:47:04.000000 hylite-1.21/hylite/sensors/owl.py
--rw-r--r--   0 runner    (1001) docker     (121)    27347 2022-08-05 20:47:04.000000 hylite-1.21/hylite/sensors/rikola.py
--rw-r--r--   0 runner    (1001) docker     (121)     4784 2022-08-05 20:47:04.000000 hylite-1.21/hylite/sensors/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 20:47:18.732070 hylite-1.21/hylite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      938 2022-08-05 20:47:18.000000 hylite-1.21/hylite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3238 2022-08-05 20:47:18.000000 hylite-1.21/hylite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-05 20:47:18.000000 hylite-1.21/hylite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-08-05 20:47:18.000000 hylite-1.21/hylite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-05 20:47:18.000000 hylite-1.21/hylite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-05 20:47:18.752070 hylite-1.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2095 2022-08-05 20:47:04.000000 hylite-1.21/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 20:47:18.752070 hylite-1.21/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1468 2022-08-05 20:47:04.000000 hylite-1.21/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2444 2022-08-05 20:47:04.000000 hylite-1.21/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (121)      852 2022-08-05 20:47:04.000000 hylite-1.21/tests/test_atmospheric.py
--rw-r--r--   0 runner    (1001) docker     (121)     1241 2022-08-05 20:47:04.000000 hylite-1.21/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2201 2022-08-05 20:47:04.000000 hylite-1.21/tests/test_hycloud.py
--rw-r--r--   0 runner    (1001) docker     (121)     4032 2022-08-05 20:47:04.000000 hylite-1.21/tests/test_hycollection.py
--rw-r--r--   0 runner    (1001) docker     (121)     6668 2022-08-05 20:47:04.000000 hylite-1.21/tests/test_hydata.py
--rw-r--r--   0 runner    (1001) docker     (121)      950 2022-08-05 20:47:04.000000 hylite-1.21/tests/test_hyfeature.py
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-08-05 20:47:04.000000 hylite-1.21/tests/test_hyimage.py
--rw-r--r--   0 runner    (1001) docker     (121)     3455 2022-08-05 20:47:04.000000 hylite-1.21/tests/test_hylibrary.py
--rw-r--r--   0 runner    (1001) docker     (121)     3394 2022-08-05 20:47:04.000000 hylite-1.21/tests/test_hyscene.py
--rw-r--r--   0 runner    (1001) docker     (121)    10706 2022-08-05 20:47:04.000000 hylite-1.21/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     6265 2022-08-05 20:47:04.000000 hylite-1.21/tests/test_mwl.py
--rw-r--r--   0 runner    (1001) docker     (121)     3771 2022-08-05 20:47:04.000000 hylite-1.21/tests/test_pmap.py
--rw-r--r--   0 runner    (1001) docker     (121)     1646 2022-08-05 20:47:04.000000 hylite-1.21/tests/test_sensors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:54:28.067696 hylite-1.23/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-17 06:54:18.000000 hylite-1.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-17 06:54:28.067696 hylite-1.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-06-17 06:54:18.000000 hylite-1.23/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:54:28.047696 hylite-1.23/hylite/
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-06-17 06:54:18.000000 hylite-1.23/hylite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:54:28.047696 hylite-1.23/hylite/analyse/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-17 06:54:18.000000 hylite-1.23/hylite/analyse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-06-17 06:54:18.000000 hylite-1.23/hylite/analyse/dtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-06-17 06:54:18.000000 hylite-1.23/hylite/analyse/indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48093 2023-06-17 06:54:18.000000 hylite-1.23/hylite/analyse/mwl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-17 06:54:18.000000 hylite-1.23/hylite/analyse/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-17 06:54:18.000000 hylite-1.23/hylite/analyse/supervised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-17 06:54:18.000000 hylite-1.23/hylite/analyse/unsupervised.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:54:28.051696 hylite-1.23/hylite/correct/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-17 06:54:18.000000 hylite-1.23/hylite/correct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-06-17 06:54:18.000000 hylite-1.23/hylite/correct/detrend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-17 06:54:18.000000 hylite-1.23/hylite/correct/equalize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:54:28.051696 hylite-1.23/hylite/correct/illumination/
+-rw-r--r--   0 runner    (1001) docker     (123)    27868 2023-06-17 06:54:18.000000 hylite-1.23/hylite/correct/illumination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-17 06:54:18.000000 hylite-1.23/hylite/correct/illumination/occlusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-17 06:54:18.000000 hylite-1.23/hylite/correct/illumination/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-17 06:54:18.000000 hylite-1.23/hylite/correct/illumination/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19888 2023-06-17 06:54:18.000000 hylite-1.23/hylite/correct/panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:54:28.051696 hylite-1.23/hylite/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-17 06:54:18.000000 hylite-1.23/hylite/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-17 06:54:18.000000 hylite-1.23/hylite/filter/combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11037 2023-06-17 06:54:18.000000 hylite-1.23/hylite/filter/dimension_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-06-17 06:54:18.000000 hylite-1.23/hylite/filter/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27000 2023-06-17 06:54:18.000000 hylite-1.23/hylite/filter/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-06-17 06:54:18.000000 hylite-1.23/hylite/filter/tpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33549 2023-06-17 06:54:18.000000 hylite-1.23/hylite/hycloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23755 2023-06-17 06:54:18.000000 hylite-1.23/hylite/hycollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40425 2023-06-17 06:54:18.000000 hylite-1.23/hylite/hydata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-06-17 06:54:18.000000 hylite-1.23/hylite/hyfeature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18352 2023-06-17 06:54:18.000000 hylite-1.23/hylite/hyheader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37339 2023-06-17 06:54:18.000000 hylite-1.23/hylite/hyimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23458 2023-06-17 06:54:18.000000 hylite-1.23/hylite/hylibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38362 2023-06-17 06:54:18.000000 hylite-1.23/hylite/hyscene.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:54:28.051696 hylite-1.23/hylite/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     9178 2023-06-17 06:54:18.000000 hylite-1.23/hylite/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-17 06:54:18.000000 hylite-1.23/hylite/io/cameras.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15925 2023-06-17 06:54:18.000000 hylite-1.23/hylite/io/clouds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-06-17 06:54:18.000000 hylite-1.23/hylite/io/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-06-17 06:54:18.000000 hylite-1.23/hylite/io/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-06-17 06:54:18.000000 hylite-1.23/hylite/io/libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-17 06:54:18.000000 hylite-1.23/hylite/io/pmaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-06-17 06:54:18.000000 hylite-1.23/hylite/multiprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:54:28.051696 hylite-1.23/hylite/project/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-17 06:54:18.000000 hylite-1.23/hylite/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24735 2023-06-17 06:54:18.000000 hylite-1.23/hylite/project/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16495 2023-06-17 06:54:18.000000 hylite-1.23/hylite/project/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-17 06:54:18.000000 hylite-1.23/hylite/project/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34765 2023-06-17 06:54:18.000000 hylite-1.23/hylite/project/pmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29673 2023-06-17 06:54:18.000000 hylite-1.23/hylite/project/pushbroom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:54:28.051696 hylite-1.23/hylite/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-17 06:54:18.000000 hylite-1.23/hylite/reference/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:54:28.051696 hylite-1.23/hylite/reference/features/
+-rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-06-17 06:54:18.000000 hylite-1.23/hylite/reference/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-17 06:54:18.000000 hylite-1.23/hylite/reference/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:54:28.051696 hylite-1.23/hylite/reference/spectra/
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-17 06:54:18.000000 hylite-1.23/hylite/reference/spectra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:54:28.051696 hylite-1.23/hylite/reference/spectra/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-17 06:54:18.000000 hylite-1.23/hylite/reference/spectra/custom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:54:28.055696 hylite-1.23/hylite/reference/spectra/pvc/
+-rw-r--r--   0 runner    (1001) docker     (123)    20987 2023-06-17 06:54:18.000000 hylite-1.23/hylite/reference/spectra/pvc/PVC_Black.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20987 2023-06-17 06:54:18.000000 hylite-1.23/hylite/reference/spectra/pvc/PVC_Grey.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20987 2023-06-17 06:54:18.000000 hylite-1.23/hylite/reference/spectra/pvc/PVC_Red.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20987 2023-06-17 06:54:18.000000 hylite-1.23/hylite/reference/spectra/pvc/PVC_White.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-17 06:54:18.000000 hylite-1.23/hylite/reference/spectra/pvc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:54:28.055696 hylite-1.23/hylite/reference/spectra/spectralon/
+-rw-r--r--   0 runner    (1001) docker     (123)    45471 2023-06-17 06:54:18.000000 hylite-1.23/hylite/reference/spectra/spectralon/R50.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    47694 2023-06-17 06:54:18.000000 hylite-1.23/hylite/reference/spectra/spectralon/R55_SiSu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    45471 2023-06-17 06:54:18.000000 hylite-1.23/hylite/reference/spectra/spectralon/R6.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    45492 2023-06-17 06:54:18.000000 hylite-1.23/hylite/reference/spectra/spectralon/R90.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-17 06:54:18.000000 hylite-1.23/hylite/reference/spectra/spectralon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:54:28.055696 hylite-1.23/hylite/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-06-17 06:54:18.000000 hylite-1.23/hylite/sensors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:54:28.055696 hylite-1.23/hylite/sensors/calibration_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 06:54:18.000000 hylite-1.23/hylite/sensors/calibration_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:54:28.059696 hylite-1.23/hylite/sensors/calibration_data/fenix/
+-rw-r--r--   0 runner    (1001) docker     (123)   958464 2023-06-17 06:54:18.000000 hylite-1.23/hylite/sensors/calibration_data/fenix/Radiometric_2x2_1x1.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-06-17 06:54:18.000000 hylite-1.23/hylite/sensors/calibration_data/fenix/Radiometric_2x2_1x1.hdr
+-rw-r--r--   0 runner    (1001) docker     (123)   691200 2023-06-17 06:54:18.000000 hylite-1.23/hylite/sensors/calibration_data/fenix/Radiometric_4x2_1x1.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-17 06:54:18.000000 hylite-1.23/hylite/sensors/calibration_data/fenix/Radiometric_4x2_1x1.hdr
+-rw-r--r--   0 runner    (1001) docker     (123)   557568 2023-06-17 06:54:18.000000 hylite-1.23/hylite/sensors/calibration_data/fenix/Radiometric_8x2_1x1.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     6573 2023-06-17 06:54:18.000000 hylite-1.23/hylite/sensors/calibration_data/fenix/Radiometric_8x2_1x1.hdr
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-17 06:54:18.000000 hylite-1.23/hylite/sensors/calibration_data/fenix/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:54:28.063696 hylite-1.23/hylite/sensors/calibration_data/fenix1k/
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2449408 2023-06-17 06:54:18.000000 hylite-1.23/hylite/sensors/calibration_data/fenix1k/Radiometric_2x2_1x1.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9738 2023-06-17 06:54:18.000000 hylite-1.23/hylite/sensors/calibration_data/fenix1k/Radiometric_2x2_1x1.hdr
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1728512 2023-06-17 06:54:18.000000 hylite-1.23/hylite/sensors/calibration_data/fenix1k/Radiometric_4x2_1x1.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7339 2023-06-17 06:54:18.000000 hylite-1.23/hylite/sensors/calibration_data/fenix1k/Radiometric_4x2_1x1.hdr
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1368064 2023-06-17 06:54:18.000000 hylite-1.23/hylite/sensors/calibration_data/fenix1k/Radiometric_8x2_1x1.dat
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6124 2023-06-17 06:54:18.000000 hylite-1.23/hylite/sensors/calibration_data/fenix1k/Radiometric_8x2_1x1.hdr
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-17 06:54:18.000000 hylite-1.23/hylite/sensors/calibration_data/fenix1k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67041 2023-06-17 06:54:18.000000 hylite-1.23/hylite/sensors/fenix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-06-17 06:54:18.000000 hylite-1.23/hylite/sensors/fx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-06-17 06:54:18.000000 hylite-1.23/hylite/sensors/owl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27350 2023-06-17 06:54:18.000000 hylite-1.23/hylite/sensors/rikola.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4784 2023-06-17 06:54:18.000000 hylite-1.23/hylite/sensors/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:54:28.047696 hylite-1.23/hylite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-17 06:54:28.000000 hylite-1.23/hylite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-17 06:54:28.000000 hylite-1.23/hylite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 06:54:28.000000 hylite-1.23/hylite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-17 06:54:28.000000 hylite-1.23/hylite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-17 06:54:28.000000 hylite-1.23/hylite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-17 06:54:28.067696 hylite-1.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-17 06:54:18.000000 hylite-1.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:54:28.067696 hylite-1.23/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-17 06:54:18.000000 hylite-1.23/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-17 06:54:18.000000 hylite-1.23/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-17 06:54:18.000000 hylite-1.23/tests/test_atmospheric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-17 06:54:18.000000 hylite-1.23/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-17 06:54:18.000000 hylite-1.23/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-17 06:54:18.000000 hylite-1.23/tests/test_hycloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-06-17 06:54:18.000000 hylite-1.23/tests/test_hycollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-06-17 06:54:18.000000 hylite-1.23/tests/test_hydata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-17 06:54:18.000000 hylite-1.23/tests/test_hyfeature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-17 06:54:18.000000 hylite-1.23/tests/test_hyimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-17 06:54:18.000000 hylite-1.23/tests/test_hylibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-17 06:54:18.000000 hylite-1.23/tests/test_hyscene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-17 06:54:18.000000 hylite-1.23/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-06-17 06:54:18.000000 hylite-1.23/tests/test_mwl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-06-17 06:54:18.000000 hylite-1.23/tests/test_pmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-17 06:54:18.000000 hylite-1.23/tests/test_sensors.py
```

### Comparing `hylite-1.21/LICENSE` & `hylite-1.23/LICENSE`

 * *Files identical despite different names*

### Comparing `hylite-1.21/PKG-INFO` & `hylite-1.23/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hylite
-Version: 1.21
+Version: 1.23
 Summary: Open-source toolbox for hyperspectral geology.
 Home-page: https://github.com/samthiele/hylite
 Author: Helmholtz Institute Freiberg
 Author-email: s.thiele@hzdr.de
 Project-URL: Source, https://github.com/samthiele/hylite
 Project-URL: Documentation, https://hifexplo.github.io/hylite/hylite.html
 Keywords: hyperspectral data analysis hypercloud geology mineral mapping
```

### Comparing `hylite-1.21/README.md` & `hylite-1.23/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 dimensionality reduction and spectral angle mapping. Reference spectra from spectral libraries, ground or laboratory measurements
 can also be integrated and used to perform supervised classifications using machine learning techniques.
 
 --------
 
 #### Tutorial:
 
-Try *hylite* here! These example notebooks can alse be [downloaded](https://github.com/samthiele/hylite_demo2).
+Try *hylite* [here](https://mybinder.org/v2/gh/samthiele/hylite_demo2/HEAD)! These example notebooks can alse be [downloaded](https://github.com/samthiele/hylite_demo2).
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/samthiele/hylite_demo2/HEAD)
 
 #### Documentation:
 
-Detailed documentation for *hylite* can be found here: https://hifexplo.github.io/hylite/hylite.html
+Detailed documentation for *hylite* can be found at: https://hifexplo.github.io/hylite/hylite.html
 
 --------
 
 A key design feature of *hylite* is polymorphism between different spectral data types, such that spectral libraries,
 images and point clouds can be easily analysed and integrated. Pre-processing workflows for each of these
 data types have also been implemented.
 
@@ -179,13 +179,8 @@
 Contributing to  hylite
 -------------------------
 
 Cool additions are welcomed!
 Please feel free to submit pull requests through GitHub or get in touch with us directly if
 you have any questions. Bug reports are also welcomed (though do try to be specific).
 
-Documentation
----------------
-
-For more information on how to use *hylite*, please refer to https://hylite.readthedocs.io/en/latest/index.html.
-
 ---------------
```

### Comparing `hylite-1.21/hylite/__init__.py` & `hylite-1.23/hylite/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,24 +58,25 @@
 import os
 os.environ["OMP_NUM_THREADS"] = "1"
 os.environ["OPENBLAS_NUM_THREADS"] = "1"
 os.environ["MKL_NUM_THREADS"] = "1"
 os.environ["VECLIB_MAXIMUM_THREADS"] = "1"
 os.environ["NUMEXPR_NUM_THREADS"] = "1"
 
-import numpy as np
-import warnings
-
 #disable annoying warnings
-np.warnings.filterwarnings('ignore')
-warnings.filterwarnings("ignore", category=DeprecationWarning)
+#np.warnings.filterwarnings('ignore')
+#warnings.filterwarnings("ignore", category=DeprecationWarning)
 # ignore all warnings
-def _warn(*args, **kwargs):
-    pass
-warnings.warn = _warn
+#def _warn(*args, **kwargs):
+#    pass
+#warnings.warn = _warn
+
+import warnings
+warnings.filterwarnings('ignore')
+warnings.filterwarnings("ignore", category=DeprecationWarning)
 
 ###########################################
 ## Define useful preset band combinations
 ###########################################
 RGB = (680.0,550.0,505.0)
 """
 Wavelengths for red [680.0], green [550.0] and blue [505.0]- useful for plotting.
```

### Comparing `hylite-1.21/hylite/analyse/dtree.py` & `hylite-1.23/hylite/analyse/dtree.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                 None to skip branches for certain labels (e.g. True -> None -> False will ignore the second layer of
                 the decision tree for this label).
 
     Returns:
          an output labels array of the sampe shape as each layer array but containing 0 ... n class labels.
     """
 
-    out = np.zeros( layers[0].shape, dtype=np.int )
+    out = np.zeros( layers[0].shape, dtype=int )
     names = ["Unknown"]
     for k in labels.items():
         key, value = k
         if not value in names:
             names.append(value)
         msk = np.full( layers[0].shape, True )
         for n,l in enumerate(layers):
```

### Comparing `hylite-1.21/hylite/analyse/indices.py` & `hylite-1.23/hylite/analyse/indices.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/analyse/mwl.py` & `hylite-1.23/hylite/analyse/mwl.py`

 * *Files 3% similar despite different names*

```diff
@@ -691,42 +691,45 @@
     mwld.data = out.reshape(data.data.shape[:-1] + (out.shape[-1],))
 
     # setup mwl collection and return
     mwl = MWL('M', '')
     mwl.bind( mwld, n, x=hc.get_wavelengths(), sym=sym, X=hc )
     return mwl
 
+
 class mwl_legend(object):
     """
     A utility class storing data needed to create a legend for mwl plots.
     """
 
-    def __init__(self, minh, maxh, minc, maxc, mode='val', **kwds):
+    def __init__(self, minh, maxh, minc, maxc, mode='val', cmap='rainbow', **kwds):
         """
         Create an mwl_legend instance.
 
         Args:
             minh: the value (wavelength) mapped to hue of 0
             maxh: the value (wavelength) mapped to a hue of 1
             minc: the value (typically depth/strength) mapped to brightness/saturation of 0.
             maxc: the value (typically depth/strength) mapped to brightness/saturation fo 1.
             mode: specifies if minc and maxc refer to brightness ('val', default) or saturation ('sat').
+            cmap: the colormapping to use to determine hue.
             **kwds: Keywords can include:
 
                 - xlab = a custom name for the hue (x) label. Default is 'Wavelength (nm)'
                 - ylab = a custom name for the second axis. Default is 'Strength'.
         """
 
         self.minh = minh
         self.maxh = maxh
         self.minc = minc
         self.maxc = maxc
         self.xlab = kwds.get("xlab", 'Wavelength (nm)')
         self.ylab = kwds.get("ylab", 'Strength')
         self.mode = mode
+        self.cmap = cmap
 
     def plot(self, ax, pos='top left', s=(0.3, 0.2)):
         """
         Add this legend to the specified figure.
 
         Args:
             ax: the axes to overlay the legend on.
@@ -771,16 +774,16 @@
             ax.yaxis.tick_right()
             ax.yaxis.set_label_position("right")
         if not tickBottom:
             ax.xaxis.tick_top()
             ax.xaxis.set_label_position("top")
 
         # fill axes using imshow
-        if 'swir' in str(self.minh): # again - this is dirty dirty hack... todo - write proper stop-based colour map
-            extent =( 2150.0, 2380.0, self.minc, self.maxc)
+        if 'swir' in str(self.cmap):  # again - this is dirty dirty hack...
+            extent = (2150.0, 2380.0, self.minc, self.maxc)
 
             # calculate hue
             h = np.linspace(2150., 2380., num=int(2000 * s[0]))
             _x = np.array([0, 2150,
                            2175, 2190, 2220,  # white mica
                            2245, 2254, 2261,  # chlorite/biotite/epidote
                            2325, 2330, 2345,  # carbonate
@@ -789,23 +792,29 @@
             _y = np.array([0.1, 0.1,
                            0.15, 0.3, 0.44,  # white mica
                            0.48, 0.5, 0.54,  # chlorite/biotite/epidote
                            0.82, 0.85, 0.94,  # carbonate
                            1.0, 1.0])
             wav = np.linspace(2150.0, 2380.0, 255)
             lookup = np.interp(wav, _x, 1 - _y)
-            idx = (((h - 2150.0) / (2380.0 - 2150.0)) * lookup.shape[0]).astype(np.int)
+            idx = (((h - 2150.0) / (2380.0 - 2150.0)) * lookup.shape[0]).astype(int)
             idx[idx < 0] = 0
             idx[idx > 254] = 254
             x = lookup[idx]
-
+        elif 'rainbow' in self.cmap:
+            extent = (self.minh, self.maxh, self.minc, self.maxc)
+            x = np.linspace(0, 1, num=int(2000 * s[0]))
         else:
             extent = (self.minh, self.maxh, self.minc, self.maxc)
             x = np.linspace(0, 1, num=int(2000 * s[0]))
+            cm = mpl.cm.get_cmap(self.cmap)
+            rgba = cm(x)  # compute color from cmap
+            x = mpl.colors.rgb_to_hsv(rgba[:, :3])[:, 0]  # update hue value accordingly
 
+        # build image grid
         y = np.linspace(0, 1, num=int(2000 * s[1]))
         xx, yy = np.meshgrid(x, y)
         zz = np.full(xx.shape, 0.8)
         if 'val' in self.mode.lower():
             ax.imshow(matplotlib.colors.hsv_to_rgb(np.dstack([xx, zz, yy])),
                       origin=origin, aspect='auto', extent=extent)
         else:
@@ -814,63 +823,68 @@
                       origin=origin, aspect='auto', extent=extent)
 
         ax.set_xlabel(self.xlab)
         ax.set_ylabel(self.ylab)
         ax.set_yticks([])
         return ax
 
-def colourise_mwl(mwl, mode='p-d', **kwds):
+
+def colourise_mwl(mwl, mode='p-d', cmap='rainbow', **kwds):
     """
     Takes a HyData instance containing minimum wavelength bands (pos, depth, width and strength) and creates
     a RGB composite such that hue ~ pos, sat ~ width and val ~ strength or depth.
 
     Args:
         mwl: the HyData instance containing minimum wavelength data.
         mode: the mapping from position (p), width (w) and depth and (d) to hsv. Default is 'pwd', though other options
               are 'p-d' (constant saturation of 80%), 'pdw' and 'pd-' (constant brightness of 85%).
+        cmap: the colour mapping to use. Default is to map position to hue ('rainbow'), but any matplotlib
+              colormap string can be provided here. Note that colours output by this colormap will be scaled in brightness
+              and saturation according to the mode argument. Alternatively use 'swir' for customised
+              rainbow-like colour stretch optimised for clay, mica and chlorite absorbtion features in the SWIR.
         **kwds: Keywords can include:
 
               - hue_map = Wavelengths (xxx.x, yyy.y) or percentiles (x,y) to use when converting wavelength to hue.
-                            Default is (0,100). Alternatively use 'SWIR' for customised colour stretch optimised for
-                            clay, mica and chlorite absorbtion features.
+                            Default is (0,100).
               - sat_map = Widths (xxx.x, yyy.y) or percentiles (x,y) to use when converting width to saturation.
                             Default is (0,100).
               - val_map = Strengths/depths (xxx.x, yyy.y) or percentiles (x,y) to use when converting strength to brightness.
                             Default is (0,75), as these tend to be dominated by low/zero values.
 
     Returns:
         A tuple containing:
 
         - either an RGB HyImage object (if mwl is an image) or the original HyCloud with defined rgb bands.
         - cmap = a mwl_legend instance for plotting colour maps.
     """
 
     # extract data
-    assert (mwl.band_count() == 4) or (mwl.band_count() == 3), "Error - HyData instance does not contain minimum wavelength data?"
+    assert (mwl.band_count() == 4) or (
+                mwl.band_count() == 3), "Error - HyData instance does not contain minimum wavelength data?"
 
-    h = mwl.get_raveled()[..., 1].copy()  # pos
-    s = mwl.get_raveled()[..., 2].copy()  # width
-    v = mwl.get_raveled()[..., 0].copy()  # depth
+    h = mwl.X()[..., 1].copy()  # pos
+    s = mwl.X()[..., 2].copy()  # width
+    v = mwl.X()[..., 0].copy()  # depth
 
     # normalise to range 0 - 1
     stretch = ['hue_map', 'sat_map', 'val_map']
     ranges = []  # store data ranges for colour map
     for i, b in enumerate([h, s, v]):
         if 'swir' in str(kwds.get(stretch[i], '')).lower():
             ranges.append((2150.0, 2380.0))
             continue
 
         mn, mx = kwds.get(stretch[i], (0, 100))
         if i == 2:  # use different default stretch for value (as these tend to be heavily skewed)
             mn, mx = kwds.get(stretch[i], (0, 75))
+
         if isinstance(mn, int):  # convert percentiles to values
             mn = np.nanpercentile(b, mn)
         if isinstance(mx, int):  # convert percentiles to values
             mx = np.nanpercentile(b, mx)
-
         ranges.append((mn, mx))  # store data ranges for colour map
 
         # apply stretch
         b -= mn
         b /= (mx - mn)
         b[b < 0] = 0
         b[b > 1] = 1
@@ -884,54 +898,61 @@
 
     # remove nans
     mask = np.logical_not(np.isfinite(h) & np.isfinite(s) & np.isfinite(v))
     h[mask] = 0
     v[mask] = 0
     s[mask] = 0
 
-    # map wavelength using custom map if specified
-    # N.B. this is a filthy hack.... todo - write proper stop-based colour map sometime?
-    if 'swir' in str(kwds.get('hue_map', '')).lower():
+    # calculate hue value from colormap
+    if 'rainbow' in cmap.lower():
+        h = h  # no change to hue
+    elif 'swir' in cmap.lower():  # use SWIR customised colormap
         _x = np.array([0, 2150,
                        2175, 2190, 2220,  # white mica
                        2245, 2254, 2261,  # chlorite/biotite/epidote
                        2325, 2330, 2345,  # carbonate
                        2360, 3000])
 
         _y = np.array([0.1, 0.1,
                        0.15, 0.3, 0.44,  # white mica
                        0.48, 0.5, 0.54,  # chlorite/biotite/epidote
                        0.82, 0.85, 0.94,  # carbonate
                        1.0, 1.0])
         wav = np.linspace(2150.0, 2380.0, 255)
         lookup = np.interp(wav, _x, 1 - _y)
-        idx = (((h - 2150.0) / (2380.0 - 2150.0)) * lookup.shape[0]).astype(np.int)
+        idx = (((h - 2150.0) / (2380.0 - 2150.0)) * lookup.shape[0]).astype(int)
         idx[idx < 0] = 0
         idx[idx > 254] = 254
         h = lookup[idx]
+    else:  # use matplotlib colormap
+        cm = mpl.cm.get_cmap(cmap)
+        rgba = cm(h)
+        h = mpl.colors.rgb_to_hsv(rgba[:, :3])[:, 0]  # update hue value accordingly
 
     # convert to rgb based on mapping mode
     if 'pwd' in mode.lower():  # pos, width, depth (default)
         rgb = matplotlib.colors.hsv_to_rgb(np.array([h, s, v]).T)
     elif 'pdw' in mode.lower():  # pos, depth, width
         s[mask] = 0.5
         rgb = matplotlib.colors.hsv_to_rgb(np.array([h, v, s]).T)
     elif 'p-d' in mode.lower():  # pos, const, depth
         rgb = matplotlib.colors.hsv_to_rgb(np.array([h, np.full(len(h), 0.8), v]).T)
     elif 'pd-' in mode.lower():  # pos, depth, const
         rgb = matplotlib.colors.hsv_to_rgb(np.array([h, v, np.full(len(h), 0.8)]).T)
 
     # add nans back in
-    rgb[ mask, : ] = np.nan
+    rgb[mask, :] = np.nan
 
     # create a colourbar object
     if 'pdw' in mode.lower() or 'pd-' in mode.lower():
-        cbar = mwl_legend(ranges[0][0], ranges[0][1], ranges[2][0], ranges[2][1], mode='sat')
+        cbar = mwl_legend(ranges[0][0], ranges[0][1],
+                          ranges[2][0], ranges[2][1], mode='sat', cmap=cmap)
     else:
-        cbar = mwl_legend(ranges[0][0], ranges[0][1], ranges[2][0], ranges[2][1], mode='val')
+        cbar = mwl_legend(ranges[0][0], ranges[0][1],
+                          ranges[2][0], ranges[2][1], mode='val', cmap=cmap)
     if 'swir' in str(kwds.get('hue_map', '')).lower():
         cbar.minh = 'swir'
         cbar.maxh = 'swir'
 
     if mwl.is_image():
         out = mwl.copy(data=False)
         out.data = rgb.reshape((mwl.data.shape[0], mwl.data.shape[1], 3))
```

### Comparing `hylite-1.21/hylite/analyse/sam.py` & `hylite-1.23/hylite/analyse/sam.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/analyse/supervised.py` & `hylite-1.23/hylite/analyse/supervised.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     # reshape image data
     data = data.get_raveled()
 
     # get features
     F = []
     c = []
     for i, lab in enumerate(labels):
-        mask = lab.reshape(data.shape[0]).astype(np.bool)
+        mask = lab.reshape(data.shape[0]).astype(bool)
         F.append(data[mask])
         c.append(np.sum(mask))
 
     return F, c
 
 
 def balance( F, n=1.0):
```

### Comparing `hylite-1.21/hylite/analyse/unsupervised.py` & `hylite-1.23/hylite/analyse/unsupervised.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/correct/detrend.py` & `hylite-1.23/hylite/correct/detrend.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,25 +36,26 @@
     elif 'sub' in method.lower():
         y -= t
         y += np.min(y) #map to positive
 
     return y.reshape(data.shape), t.reshape(data.shape)
 
 
-def get_hull_corrected(data, band_range=None, method='div', vb=True):
+def get_hull_corrected(data, band_range=None, method='div', hull='upper', vb=True):
     """
     Apply a hull correction to an entire HyData instance (HyImage, HyCloud or HyLibrary). Returns a corrected copy of
     the input dataset. Note that noise can greatly effect hull corrections, so you should consider denoising first (see
     HyData.smooth_median(...) and HyData.smooth_savgol(...).
 
     Args:
         data: a numpy array or HyData instance to detrend.
         band_range: Tuple containing the (min,max) band indices or wavelengths to run the correction between. If None
                      (default) then the correction is run of the entire range. Only works if data is a HyData instance.
         method: Trend removal method: 'divide' or 'subtract'. Default is 'divide'.
+        hull: 'upper' if a hull should be fitted to the top of the data (default), or 'lower' if it should be fit to the bottom of the data.
         vb: True if this should print output.
 
     Returns:
         A hull corrected dataset.
     """
 
     if isinstance(data, HyData):
@@ -89,15 +90,20 @@
     #valid = (np.isfinite(D) & (D != nan)).all(axis=1)  # drop nans/no-data values
     D = np.nan_to_num(D, nan=0, posinf=0, neginf=0) # ensure all values are finite (and do not effect hul)
     valid = (D != D[:, 0][:, None]).any(axis=1)  # drop flat spectra (e.g. all zeros)
     if len(valid) == 0:
         return corrected  # quick exit for empty images
 
     # do hull correction
-    X = remove_hull( D[valid],upper=True, div=('div' in method), vb=vb)
+    if 'upper' in hull.lower():
+        X = remove_hull( D[valid],upper=True, div=('div' in method), vb=vb)
+    elif 'lower' in hull.lower():
+        X = remove_hull(np.max(D[valid]) - D[valid], upper=True, div=('div' in method), vb=vb)
+    else:
+        assert False, "Error = 'hull' should be 'upper' or 'lower', not %s." % hull
     D[valid] = X  # copy data back into original array
 
     # do housekeeping and return
     if isinstance(data, HyData):
         if isinstance(corrected, HyLibrary):
             corrected.upper = None # reset upper and lower limits as these will now be incorrect
             corrected.lower = None # reset upper and lower limits as these will now be incorrect
```

### Comparing `hylite-1.21/hylite/correct/equalize.py` & `hylite-1.23/hylite/correct/equalize.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/correct/illumination/__init__.py` & `hylite-1.23/hylite/correct/illumination/__init__.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/correct/illumination/occlusion.py` & `hylite-1.23/hylite/correct/illumination/occlusion.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/correct/illumination/path.py` & `hylite-1.23/hylite/correct/illumination/path.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/correct/illumination/reflection.py` & `hylite-1.23/hylite/correct/illumination/reflection.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/correct/panel.py` & `hylite-1.23/hylite/correct/panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,22 +19,24 @@
 class Panel( HyData ):
     """
     A class for identifying calibration reference in images and storing
     the observed pixel radiances and known target reflectance values. This is used
     by, e.g., empirical line calibration procedures.
     """
 
-    def __init__(self, material, radiance, **kwds):
+    def __init__(self, material, radiance, strict=True, **kwds):
         """
         Generic constructor. Can be of the following forms:
 
         Args:
             material: a hylite.reference.Target instance containing target reflectance data for this panel.
             radiance: either a HyImage object (which contains some reference pixels) or a
                         NxM numpy array containing radiance values for N pixels across M bands.
+            strict: True if measured radiance wavelengths must be entirely within the range of the reference material
+                    spectra. Default is True. Use with care!
             **kwds: Keywords can include the following:
 
                  - wavelengths = wavelengths corresponding to the radiance values (if radiance is an array rather than a HyImage
                                  object).
                  - method = 'manual' (default) to manually pick reference in image (using an interactive plot). Can also be
                              'sobel' or 'laplace' to use the corresponding edge detectors to automatically identify the
                              calibration target (using OpenCV contouring).
@@ -189,22 +191,23 @@
         if self.data.shape[0] > 30:
             brightness = np.nanmean(self.data, axis=1)
             mask = brightness > np.nanpercentile(brightness, 50)
             self.data = self.data[mask, :]
 
         # extract reflectance data from target
         target_bands = material.get_wavelengths()
-        assert np.nanmin(target_bands) <= np.nanmin(
-            self.get_wavelengths()), "Error - calibration range does not cover pixel range. " \
-                                     "Radiance data starts at %.1f nm but calibration data starts %.1f nm." % (
-                                         np.nanmin(self.get_wavelengths()), np.nanmin(target_bands))
-        assert np.nanmax(target_bands) >= np.nanmax(
-            self.get_wavelengths()), "Error - calibration range does not cover pixel range. " \
-                                     "Radiance data ends at %.1f nm but calibration data ends %.1f nm." % (
-                                         np.nanmax(self.get_wavelengths()), np.nanmax(target_bands))
+        if strict:
+            assert np.nanmin(target_bands) <= np.nanmin(
+                self.get_wavelengths()), "Error - calibration range does not cover pixel range. " \
+                                         "Radiance data starts at %.1f nm but calibration data starts %.1f nm." % (
+                                             np.nanmin(self.get_wavelengths()), np.nanmin(target_bands))
+            assert np.nanmax(target_bands) >= np.nanmax(
+                self.get_wavelengths()), "Error - calibration range does not cover pixel range. " \
+                                         "Radiance data ends at %.1f nm but calibration data ends %.1f nm." % (
+                                             np.nanmax(self.get_wavelengths()), np.nanmax(target_bands))
         idx = [np.argmin(np.abs(target_bands - w)) for w in self.get_wavelengths()]  # matching wavelengths
         self.reflectance = material.get_reflectance()[idx]
         self.material = material
 
     def set_outline(self, coords ):
         """
         Define a panel outline (for e.g., estimating orientation) based on a known camera pose.
```

### Comparing `hylite-1.21/hylite/filter/__init__.py` & `hylite-1.23/hylite/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/filter/combine.py` & `hylite-1.23/hylite/filter/combine.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/filter/dimension_reduction.py` & `hylite-1.23/hylite/filter/dimension_reduction.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 PCA and MNF methods for dimensionality reduction.
 """
 
 import numpy as np
+
 import spectral
 from hylite import HyData
 
 def PCA(hydata, bands=20, band_range=None, step=5):
     """
     Apply a PCA dimensionality reduction to the hyperspectral dataset using singular vector decomposition (SVD).
 
@@ -19,16 +20,19 @@
                     if image is a hyImage object.
         step: subsample the dataset during SVD for performance reason. step = 1 will include all pixels in the calculation,
               step = n includes every nth pixel only. Default is 5 (as most images contain more than enough pixels to
               accurately estimate variance etc.).
     Returns:
         A tuple containing:
 
-        - bands = Bands transformed into PCA space, ordered from highest to lowest variance.
+        - bands = A HyData instance containing the PCA components, ordered from highest to lowest variance.
         - factors = the factors (vector) each band is multiplied with to give the corresponding PCA band.
+
+        Additional info (including loadings and the per-band means) are stored in the header file of the returned HyData
+        instance.
     """
 
     # get numpy array
     wav = None
     decomp = False
     if isinstance(hydata, HyData):
         wav = hydata.get_wavelengths()
@@ -65,53 +69,59 @@
     X = X - mean[None, :]
 
     # calculate covariance
     cov = np.dot(X.T, X) / (X.shape[0] - 1)
 
     # and eigens (sorted from biggest to smallest)
     eigval, eigvec = np.linalg.eig(cov)
-    idx = np.argsort(eigval)[::-1]
+    idx = np.argsort(np.abs(eigval))[::-1]
     eigvec = eigvec[:, idx]
     eigval = np.abs(eigval[idx])
 
     # project data
     data = data[..., minb:maxb] - mean
     out = np.zeros_like(data)
     for b in range(min(bands, data.shape[-1])):
         out[..., b] = np.dot(data, eigvec[:, b])
 
     # compute variance percentage of each eigenvalue
     eigval /= np.sum(eigval)  # sum to 1
 
-    # filter wavelengths for return
-    if not wav is None:
-        wav = wav[minb:maxb]
     # compress?
     if decomp:
         hydata.compress()
 
     # prepare output
-    outobj = hydata.copy(data=False)
-    outobj.header.drop_all_bands()  # drop band specific attributes
-    outobj.data = out[..., 0:bands]
+    bands = min(bands, out.shape[-1])
+    if isinstance(hydata, HyData):
+        outobj = hydata.copy(data=False)
+        outobj.data = out[..., 0:bands]
+    else:
+        outobj = HyData( out[..., 0:bands] )
     outobj.set_wavelengths(np.cumsum(eigval[0:bands]))  # wavelengths are % of explained variance
-    outobj.push_to_header()
+    outobj.header['mean'] = mean
+    for n in range(bands):
+        outobj.header['L_%d'%n] = eigvec[:, n]
     return outobj, eigvec[:, :bands ].T
 
-def MNF(hydata, bands=20, band_range=None, denoise=False):
+
+def MNF(hydata, bands=20, band_range=None, noise=None, denoise=False):
     """
     Apply a minimum noise filter to a hyperspectral image.
 
     Args:
         hydata: A HyData instance containing the source dataset (e.g. image or point cloud).
         bands: the number of bands to keep after MNF for dimensionality reduction or denoising. Default is 20.
         band_range: the spectral range to perform the MNF over. If (int,int) is passed then the values are treated as
                     min/max band IDs, if (float,float) is passed then values are treated as wavelenghts (in nm). If None is
                     passed (default) then the MNF is computed using all bands. Note that wavelengths can only be passed
                     if image is a hyImage object.
+        noise: The noise model to use. If None (default) then the 'band noise' parameter will be retrieved from the headerinfo,
+                and if this does not exist then, this it is crudely estimated by comparing adjacent pixels / points.
+                This estimation can be forced by setting noise to 'diff'.
         denoise: True if a MNF denoised image should be returned (rather than the MNF bands). Default is False.
     Returns:
         A tuple containing:
 
         - mnf = a HyData instance containing the MNF bands or denoised image.
         - factors = A 2D numpy array containing the factors applied to the input datset. Useful
                      for plotting/interpreting the regions each MNF band is sensitive too.
@@ -156,34 +166,39 @@
     X = X[:, np.isfinite(np.sum(X, axis=0))]  # drop columns containing nans
     X = X[:, np.sum(X, axis=0) > 0 ] #drop columns containing all zeros
     mean = np.mean(X, axis = 1)
     cov = np.cov(X)
     n = X.shape[1]
     signal = spectral.GaussianStats(mean, cov, n)
 
-    # calculate noise as per spectral.noise_from_diffs (but allowing for nans)
-    if len(data.shape) == 3:  # estimate noise by subtracting adjacent pixels
-        if data.shape[0] == 1:  # special case - 1-D image
-            deltas = data[:, :-1, :] - data[:, 1:, :]
-        elif data.shape[1] == 1:
-            deltas = data[:-1, :, :] - data[1:, :, :]
-        else:
-            deltas = data[:-1, :-1, :] - data[1:, 1:, :]
-    elif len(data.shape) == 2:  # point cloud data. N.B. this assumes that adjacent points are close in space!
-        deltas = data[:-1, :] - data[1:, :]
-
-    X = deltas.reshape(-1, deltas.shape[-1]).T
-    X = X[:, np.isfinite(np.sum(X, axis=0))]  # drop columns containing nans
-    X = X[:, np.sum(X, axis=0) > 0]  # drop columns containing all zeros
-    X = X[:, np.sum(X, axis=0) < np.nanpercentile( np.sum(X,axis=0), 50) ] #drop high noise data (these relate to edges)
-    mean = np.mean(X, axis=1)
-    cov = np.cov(X)
-    n = X.shape[1]
+    if (noise is None) and 'band noise' in hydata.header:  # get noise from header?
+        noise = np.array( hydata.header.get_list('band noise') )
+    if (noise is not None) and (noise != 'diff'): # we have noise info - use it
+        assert noise.shape[0] == hydata.band_count(), "Error - noise provided for %d bands but data has %d" % (noise.shape[0], hydata.band_count())
+        mean = noise[valid_bands] # easy
+        cov = np.full( (mean.shape[0], mean.shape[0]), 0. ) # assume noise is de-corellated
+    else: # we need to guesstimate the noise model from the data
+        if len(data.shape) == 3:  # estimate noise by subtracting adjacent pixels
+            if data.shape[0] == 1:  # special case - 1-D image
+                deltas = data[:, :-1, :] - data[:, 1:, :]
+            elif data.shape[1] == 1:
+                deltas = data[:-1, :, :] - data[1:, :, :]
+            else:
+                deltas = data[:-1, :-1, :] - data[1:, 1:, :]
+        elif len(data.shape) == 2:  # point cloud data. N.B. this assumes that adjacent points are close in space!
+            deltas = data[:-1, :] - data[1:, :]
+
+        X = deltas.reshape(-1, deltas.shape[-1]).T
+        X = X[:, np.isfinite(np.sum(X, axis=0))]  # drop columns containing nans
+        X = X[:, np.sum(X, axis=0) > 0]  # drop columns containing all zeros
+        X = X[:, np.sum(X, axis=0) < np.nanpercentile( np.sum(X,axis=0), 50) ] # drop high noise data (these relate to edges)
+        mean = np.mean(X, axis=1)
+        cov = np.cov(X)
+        #n = X.shape[1]
     noise = spectral.GaussianStats(mean, cov, n)
-
     mnfr = spectral.mnf(signal, noise)
 
     # reduce bands
     reduced = mnfr.reduce(data, num=bands)
 
     #apply sign correction so there are less positive pixels than negative ones (sign is aribrary, helps maintain
     #consistency for plotting etc. by having low-valued background with some high-value regions (<50%)
@@ -212,39 +227,43 @@
     # put factors in the header
     for i in range(factors.shape[0]):
         out.header['mnf weights %d' % i] = factors[i, :]
 
     return out, factors
 
 
-def from_loadings(data, L):
+def from_loadings(data, L, m=None):
     """
-    Transform a dataset using a precomputed loading vector.  This allows PCA or MNF
+    Transform a dataset using a precomputed loading vector.  This allows PCA
     transforms to be computed on one dataset and then applied to another.
 
     Args:
        data: A dataset (HyData instance or numpy array) with b bands in the last axis.
        L: the loadings vector of shape (k,b), such that data is projected into a
                  k-dimensional space.
-
+       m: the mean of each dimension. Default is None ( do not apply mean offset ).
     Returns:
        a hydata instance or numpy array containing the transformed data.
     """
     # get relevant data
     if isinstance(data, HyData):
         X = data.X()
-        outshape = data.data.shape[:-1] + (L.shape[0],)
+        outshape = data.data.shape[:-1] + (L.shape[1],)
     else:
         X = data.reshape((-1, data.shape[-1]))
-        outshape = data.shape[:-1] + (L.shape[0],)
+        outshape = data.shape[:-1] + (L.shape[1],)
 
     # project data
-    out = np.zeros((X.shape[0], L.shape[0]))
-    for b in range(L.shape[0]):
-        out[..., b] = np.dot(X, L[b, :])
+    out = np.dot(X, L)
+
+    # add mean
+    if m is not None:
+        out += m
+
+    # reshape
     out = out.reshape(outshape)
 
     # return HyData or numpy array
     if isinstance(data, HyData):
         O = data.copy(data=False)
         O.data = out
         return O
```

### Comparing `hylite-1.21/hylite/filter/sample.py` & `hylite-1.23/hylite/filter/sample.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/filter/segment.py` & `hylite-1.23/hylite/filter/segment.py`

 * *Files 4% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     if erode > 0:
         kernel = np.ones((3, 3), np.uint8)
         mask = cv2.erode(mask.astype(np.uint8), kernel, iterations=1)
         mask = mask == 1
 
     # extract contours and create label mask
     contours,_ = cv2.findContours(mask.astype(np.uint8) * 255, cv2.RETR_TREE, cv2.CHAIN_APPROX_SIMPLE)
-    labels = np.zeros(mask.shape, dtype=np.int)
+    labels = np.zeros(mask.shape, dtype=int)
     xx, yy = np.meshgrid(np.arange(mask.shape[0]), np.arange(mask.shape[1]))
     xx = xx.flatten()
     yy = yy.flatten()
     points = np.vstack([xx, yy]).T  # coordinates of each pixel
     for cnt in contours:
 
         # convert to matplotlib path
@@ -195,65 +195,96 @@
     # create classification file
     cls = hylite.HyImage(labels[:, :, None])
     cls.header["file type"] = "ENVI Classification"
 
     n = int(np.max(fg))
     cls.header['classes'] = n
     names = image.header.get_class_names()
-    if len(names) == 0:
+    if names is not None and len(names) == 0:
         names = [str(i) for i in range(1, n + 1)]
-    cls.header['class names'] = ['background'] + names
+        cls.header['class names'] = ['background'] + names
     cmap = mpl.cm.get_cmap('viridis')
     cls.header['class lookup'] = (np.array([cmap(i)[:3] for i in np.linspace(0, 1, n)]).ravel() * 255).astype(np.uint8)
 
     return cls
 
-def extract_tiles( image, labels ):
+
+# do extraction
+def extract_tiles(image, labels, connected=False, ids=None, erode=0):
     """
     Extract tiles that each contain a single contiguous block based on the specified classification. Useful for
     extracting individual samples from core-scanner imagery.
 
     Args:
         image: the hyperspectral image to extract blocks from
-        labels: a HyImage instance with different samples labelled as non-0 values.
+        labels: a HyImage instance or numpy array with different samples labelled as non-0 values.
+        connected: True if separate groups of pixels with the same label should be split
+                   into different tiles using cv2.connectedComponents. Default is True.
+        ids: a list of label ids to extract. If None (default), all non-zero classes will
+             be extracted.
+        erode: number of pixels to erode from mask before extracting tiles. Default is 0.
     """
 
-    # extract connected components
-    components = cv2.connectedComponents( (labels.data[:,:,0] != 0).astype(np.uint8) )
+    # get labels array
+    if isinstance(labels, hylite.HyImage):
+        labels = labels.data[..., 0]
+
+    # get ids
+    if ids is None:
+        ids = np.unique(labels)
+        ids = ids[ids != 0]  # remove zero
 
     # extract tiles
     tiles = []
     sampleID = []
-    for i in range(1, components[0]): # loop through connected components
-        # extract bounding box of this sample
-        mask = components[1] == i
-        bounds = cv2.boundingRect(mask.astype(np.uint8))
-
-        # extract tile and remove pixels not related to this sample
-        data = image.data[bounds[1]:(bounds[1] + bounds[3]),
-               bounds[0]:(bounds[0] + bounds[2]), :].copy()
-        mask = mask[bounds[1]:(bounds[1] + bounds[3]),
-               bounds[0]:(bounds[0] + bounds[2])].copy()
-        label = np.nanmax(labels.data[bounds[1]:(bounds[1] + bounds[3]),
-                          bounds[0]:(bounds[0] + bounds[2]), :])
-
-        # remove pixels not related to this tile
-        if image.is_float():
-            data[np.logical_not(mask)] = np.nan
-        else:
-            data[np.logical_not(mask)] = 0
+    for i in ids:  # loop through labels
 
-        t = hylite.HyImage(data)
-        if image.has_wavelengths():
-            t.set_wavelengths(image.get_wavelengths())
-        if image.has_band_names():
-            t.set_wavelengths(image.get_wavelengths())
-
-        tiles.append( t )
-        sampleID.append(label)
+        # get mask
+        mask = labels == i
+        if not mask.any():
+            continue  # can be the case if erode removed entire labels
+
+        if erode > 0:
+            mask = cv2.erode(mask.astype(np.uint8), np.ones((erode, erode,))) == 1
+
+        if not connected:
+            # easy - don't bother to separate
+            pixels = np.argwhere(mask)  # get valid pixels
+            local = pixels - np.min(pixels, axis=0)[None, :]  # translate to get pixels in tile
+
+            tile = hylite.HyImage(np.full((np.max(local[:, 0] + 1),
+                                           np.max(local[:, 1] + 1), image.band_count()), np.nan))
+            tile[local[:, 0], local[:, 1], :] = image.data[pixels[:, 0], pixels[:, 1], :]
+            tile.set_wavelengths(image.get_wavelengths())
+
+            # store label and tile
+            sampleID.append(i)
+            tiles.append(tile)
+        else:
+            # check connected components first
+            nc, cl = cv2.connectedComponents(mask.astype(np.uint8))
+            for n in range(nc):  # loop through components
+                comp_mask = cl == n
+                if not mask[comp_mask].all():
+                    continue  # this component is background
+
+                mask2 = mask & comp_mask
+
+                # extact pixels
+                pixels = np.argwhere(mask2)  # get valid pixels
+                local = pixels - np.min(pixels, axis=0)[None, :]  # translate to get pixels in tile
+
+                tile = hylite.HyImage(np.full((np.max(local[:, 0] + 1),
+                                               np.max(local[:, 1] + 1), image.band_count()), np.nan))
+                tile[local[:, 0], local[:, 1], :] = image.data[pixels[:, 0], pixels[:, 1], :]
+                tile.set_wavelengths(image.get_wavelengths())
+
+                # store label and tile
+                sampleID.append(i)
+                tiles.append(tile)
 
     return tiles, sampleID
 
 def group_tiles( tiles, groups, ids=None, rotate=True, ignore=[] ):
     """
     Group a list of image tiles based on corresponding group IDs.
```

### Comparing `hylite-1.21/hylite/filter/tpt.py` & `hylite-1.23/hylite/filter/tpt.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/hycloud.py` & `hylite-1.23/hylite/hycloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,15 +204,15 @@
         if isinstance(val, tuple) or isinstance(val, list):
             assert len(val) == 2, "Error - filter range (val) must have length 2."
             if trim:
                 msk = np.logical_or(self.data[..., b] <= val[0], self.data[..., b] >= val[1])
             else:
                 msk = np.logical_and(self.data[..., b] >= val[0], self.data[..., b] <= val[1])
         elif isinstance(val, np.ndarray):
-            assert val.dtype == np.bool, "Error - only boolean arrays can be used as point masks."
+            assert val.dtype == bool, "Error - only boolean arrays can be used as point masks."
             msk = val
         else:
             msk = self.data[..., b] == val
 
         # convert to indices
         msk = np.argwhere(msk)
 
@@ -607,15 +607,15 @@
         assert len(bands) == 3, "Error - bands must have length three. No more. No less. Three."
 
         # convert to band indexes
         bands = list(bands)
         for i, b in enumerate(bands):
             bands[i] = self.get_band_index(b)
 
-        self.rgb = self.data[:, bands].astype(np.float)
+        self.rgb = self.data[:, bands].astype(float)
 
         # normalise bands
         for i, b in enumerate(bands):
             if 'data ignore value' in self.header:  # deal with data ignore values for integer arrays...
                 self.rgb[self.rgb[:, i] == int(self.header['data ignore value'])] = np.nan  # make nans
 
             # calculate stretch values for normalisation
@@ -735,18 +735,18 @@
 
             # rasterise to make depth map
             _vals, _d = rasterize(pp, vis, self.xyz, _image.data.shape, 1)
 
             # mask occluded points
             if occ_tol != 0:  # occlusion is enabled
                 vis[vis == True] = np.abs(
-                    _d[pp[vis, 0].astype(np.int), pp[vis, 1].astype(np.int)] - pp[vis, 2]) <= occ_tol
+                    _d[pp[vis, 0].astype(int), pp[vis, 1].astype(int)] - pp[vis, 2]) <= occ_tol
 
             # extract pixels
-            pixels = _image.data[pp[vis, 0].astype(np.int), pp[vis, 1].astype(np.int)][:, bid]
+            pixels = _image.data[pp[vis, 0].astype(int), pp[vis, 1].astype(int)][:, bid]
             valid = np.zeros(pixels.shape, dtype=count.dtype) + 1  # valid pixels
 
             #deal with nans/missing data
             for nanpixels in [np.isnan(pixels), pixels == nan ]: #nan == 0 for integer data...
                 valid[nanpixels] = 0
                 pixels[nanpixels] = 0
```

### Comparing `hylite-1.21/hylite/hydata.py` & `hylite-1.23/hylite/hydata.py`

 * *Files 4% similar despite different names*

```diff
@@ -252,15 +252,15 @@
 
         # wrap individual integers or floats in a list
         if isinstance(bands, int) or isinstance(bands, float):
             bands = [bands]  # wrap in list
 
         # calculate bands to remove
         mask = np.full( self.band_count(), True )
-        if isinstance(bands, np.ndarray) and bands.dtype == np.bool:
+        if isinstance(bands, np.ndarray) and bands.dtype == bool:
             # mask is a numpy array containing True for bands to keep, so flip it to get bands to remove.
             mask = np.logical_not(bands)
         elif isinstance(bands, tuple) and len(bands) == 2:
             # get indices of bands to keep and flag these as False in mask.
             if bands[0] == -1: bands = (0, bands[1])
             if bands[1] == -1: bands = (bands[0], self.band_count())
             mn = self.get_band_index(bands[0])
@@ -432,33 +432,57 @@
 
         Returns:
             pixels (ndarray): an array such that pixel[n][band] gives the spectra of the nth pixel.
         """
 
         return self.data.reshape(-1, self.data.shape[-1])
 
-    def X(self):
+    def X(self, onlyFinite = False):
         """
         A shorthand way of writing get_raveled(), as X is conventionally used for a vector of spectra.
+
+        Args:
+            onlyFinite (bool): True if data points containing nan bands should be removed from the feature vector. Default is False.
         """
-        return self.get_raveled()
+        X = self.get_raveled()
+        if onlyFinite:
+            return X[ np.isfinite(X).all(axis=-1) ]
+        else:
+            return X
 
-    def set_raveled(self, pix, shape=None):
+    def set_raveled(self, pix, shape=None, onlyFinite = False, strict=True ):
         """
         Fills the image/dataset from a list of pixels of the format returned by get_pixel_list(...). Note that this does not
         copy the list, but simply stores a view of it in this image.
 
         Args:
             pix (list, ndarray): a list such that pixel[n][band] gives the spectra of the nth pixel.
             shape (tuple): the reshaped data dimensions. Defaults to the shape of the current dataset, except with auto-shape for the last dimension.
+            onlyFinite (bool): True if pix contains only pixel values corresponding to non-nan pixels in self.data (as returned by self.X( True ) ).
+            strict (bool): True if set_raveled should not change the number of bands in this image. Default is True.
         """
         if shape is None:
             shape = list( self.data.shape )
             shape[-1] = -1
-        self.data = pix.reshape(shape)
+
+        if strict: # number of bands cannot change
+            assert self.data.shape[-1] == pix.shape[-1], \
+                "Error: image and pix array have different number of bands. To allow changes to band count please specify strict=False."
+            if onlyFinite:
+                self.data[ np.isfinite(self.data).all(axis=-1), : ] = pix
+            else:
+                self.data = pix.reshape(shape)
+        else:
+            newdata = np.full( self.data.shape[:-1] + (pix.shape[-1],), np.nan, )
+            if onlyFinite:
+                if onlyFinite:
+                    newdata[np.isfinite(self.data).all(axis=-1), :] = pix
+                else:
+                    newdata = pix.reshape( self.data.shape[:-1] + (pix.shape[-1],) )
+            self.data = newdata
 
     def get_band_index(self, w, **kwds):
         """
         Get the band index that corresponds with the given wavelength or band name.
 
         Args:
             w (float, int, str): the wavelength, index or band name search for. Note that if w is an integer it is treated
@@ -659,16 +683,16 @@
 
         assert isinstance(window, int), "Error - running window size must be integer."
 
         # extract contiguous chunks
         if chunk:
             C, w = self.contiguous_chunks(min_size=window)
         else:
-            C = [self.data]
-            w = [self.get_wavelengths()]
+            C = [self.data.copy()]
+            w = [self.get_wavelengths().copy()]
 
         # do smoothing
         kwds['window_length'] = window
         kwds['polyorder'] = poly
         kwds['axis'] = -1
         for X in C:
             mask = np.isfinite(X).all(axis=-1)  # remove nans
@@ -912,17 +936,20 @@
 
         # calculate percentile thresholds
         if per_band:
             minv, maxv = np.nanpercentile(self.data, (minv, maxv), tuple(np.arange(len(self.data.shape) - 1)))
         else:
             minv, maxv = np.nanpercentile(self.data, (minv, maxv))
 
+        # ensure dtype is a float
+        if np.issubdtype(self.data.dtype, np.integer):
+            self.data = self.data.astype(np.float32)
+
         # apply normalisation
-        self.data -= minv
-        self.data /= maxv
+        self.data = (self.data - minv) / (maxv-minv)
 
         # apply clipping
         if clip:
             self.data = np.clip( self.data, 0, 1 )
 
         return minv, maxv
```

### Comparing `hylite-1.21/hylite/hyfeature.py` & `hylite-1.23/hylite/hyfeature.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/hyheader.py` & `hylite-1.23/hylite/hyheader.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         """
         return 'band names' in self
 
     def has_wavelengths(self):
         """
         Return true if wavelengths are defined.
         """
-        return 'wavelength' in self
+        return ('wavelength' in self)
 
     def has_fwhm(self):
         """
         Return true if FWHM are defined.
         """
         return 'fwhm' in self
 
@@ -61,16 +61,19 @@
         assert 'band names' in self, "Error - header file has no band names."
         return self.get_list('band names', str)
 
     def get_wavelengths(self):
         """
         Get list of band wavelengths from header file.
         """
-        assert 'wavelength' in self, "Error - header file has no wavelength information."
-        return self['wavelength'].copy()
+        if 'wavelength' in self:
+            return self['wavelength'].copy()
+        else:
+            assert False, "Error - header file has no wavelength information."
+
 
     def get_bbl(self):
         """
         Get the list of bad bands from header file. This will return an
         array scored True if a band is good and False if it is bad.
         """
         assert 'bbl' in self, "Error - header file has no bad band information."
@@ -105,29 +108,29 @@
             wavelengths (list, ndarray): a list or numpy array of wavelengths.
         """
         if wavelengths is None:
             if 'wavelength' in self:
                 del self['wavelength']
         else:
             assert isinstance(wavelengths, list) or isinstance(wavelengths, np.ndarray) or isinstance(wavelengths, tuple), "Error - wavelengths must be list, tuple or numpy array."
-            self['wavelength'] = np.array(wavelengths).astype(np.float)
+            self['wavelength'] = np.array(wavelengths).astype(float)
 
     def set_fwhm(self, fwhm):
         """
         Set list of band wavelengths from header file.
 
         Args:
             fwhm (list, ndarray): a list or numpy array of band widths.
         """
         if fwhm is None:
             if 'fwhm' in self:
                 del self['fwhm']
         else:
             assert isinstance(fwhm, list) or isinstance(fwhm, np.ndarray), "Error - fwhm must be list or numpy array."
-            self['fwhm'] = np.array(fwhm).astype(np.float)
+            self['fwhm'] = np.array(fwhm).astype(float)
 
     def set_bbl(self, bbl):
         """
         Set list of bad bands.
 
         Args:
             bbl (list, ndarray): a list or numpy array scored True for good bads and False for bad ones, or None to remove bbl.
@@ -148,15 +151,15 @@
             mask (list, ndarray): either a list of band indices to remove or a boolean numpy array with True for bands that should remove.
         """
         # how many bands are there?
         nbands = self.band_count()
 
         # create boolean mask
         mask = np.array(mask)
-        if mask.dtype == np.bool:
+        if mask.dtype == bool:
             keep = np.logical_not(mask)  # flip so we have array with True for bands to keep
         elif issubclass(mask.dtype, np.integer):
             keep = np.full(nbands, True)
             keep[mask] = False  # drop bands
         else:
             "Error - unrecognised data type %s." % mask.dtype
 
@@ -237,15 +240,15 @@
         for key, value in self.items():
             s = str(value).strip()
             print("%s = { %s } " % (key, s))
 
     ############################################################
     ## Functions related to other data we store in header files
     ############################################################
-    def get_list(self, name, dtype=np.float):
+    def get_list(self, name, dtype=float):
         """
         Get generic list data from the header as a numpy array.
 
         Args:
             name (str): the header key used to access the list.
             dtype (str): the numpy data type that should be returned. Default is float.
```

### Comparing `hylite-1.21/hylite/hyimage.py` & `hylite-1.23/hylite/hyimage.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import scipy as sp
 from scipy import ndimage
 import hylite
 from hylite.hydata import HyData
 from hylite.hylibrary import HyLibrary
 
 
+
 class HyImage( HyData ):
     """
     A class for hyperspectral image data. These can be individual scenes or hyperspectral orthoimages.
     """
 
     def __init__(self, data, **kwds):
         """
@@ -37,16 +38,18 @@
 
         #call constructor for HyData
         super().__init__(data, **kwds)
 
         # special case - if dataset only has oneband, slice it so it still has
         # the format data[x,y,b].
         if not self.data is None:
+            if len(self.data.shape) == 1:
+                self.data = self.data[None, None, :] # single pixel image
             if len(self.data.shape) == 2:
-                self.data = self.data[:, :, np.newaxis]
+                self.data = self.data[:, :, None] # single band iamge
 
         #load any additional project information (specific to images)
         self.set_projection(kwds.get("projection",None))
         self.affine = kwds.get("affine",[0,1,0,0,0,1])
 
         #special header formatting
         self.header['file type'] = 'ENVI Standard'
@@ -62,14 +65,20 @@
             a new HyImage instance.
         """
         if not data:
             return HyImage(None, header=self.header.copy(), projection=self.projection, affine=self.affine)
         else:
             return HyImage( self.data.copy(), header=self.header.copy(), projection=self.projection, affine=self.affine)
 
+    def T(self):
+        """
+        Return a transposed view of the data matrix (corresponding with the [y,x] indexing used by matplotlib, opencv etc.
+        """
+        return np.transpose(self.data, (1,0,2))
+
     def xdim(self):
         """
         Return number of pixels in x (first dimension of data array)
         """
         return self.data.shape[0]
 
     def ydim(self):
@@ -503,15 +512,15 @@
     def quick_plot(self, band=0, ax=None, bfac=0.0, cfac=0.0, samples=False, tscale=False, rot=False, flipX=False, flipY=False,
                    **kwds):
         """
         Plot a band using matplotlib.imshow(...).
 
         Args:
             band (str,int,float,tuple): the band name (string), index (integer) or wavelength (float) to plot. Default is 0. If a tuple is passed then
-                  each band in the tuple (string or index) will be mapped to rgb.
+                  each band in the tuple (string or index) will be mapped to rgb. Bands with negative wavelengths or indices will be inverted before plotting.
             ax: an axis object to plot to. If none, plt.imshow( ... ) is used.
             bfac (float): a brightness adjustment to apply to RGB mappings (-1 to 1)
             cfac (float): a contrast adjustment to apply to RGB mappings (-1 to 1)
             samples (bool): True if sample points (defined in the header file) should be plotted. Default is False. Otherwise, a list of
                      [ (x,y), ... ] points can be passed.
             tscale (bool): True if each band (for ternary images) should be scaled independently. Default is False.
                     When using scaling, vmin and vmax can be used to set the clipping percentiles (integers) or
@@ -542,56 +551,77 @@
         if not kwds.pop('ticks', False ):
             ax.set_xticks([])
             ax.set_yticks([])
 
         #map individual band using colourmap
         if isinstance(band, str) or isinstance(band, int) or isinstance(band, float):
             #get band
-            data = self.data[:, :, self.get_band_index(band)]
+            if isinstance(band, str):
+                data = self.data[:, :, self.get_band_index(band)]
+            else:
+                data = self.data[:, :, self.get_band_index(np.abs(band))]
+            if not isinstance(band, str) and band < 0:
+                data = np.nanmax(data) - data # flip
+
+            # convert integer vmin and vmax values to percentiles
+            if 'vmin' in kwds:
+                if isinstance(kwds['vmin'], int):
+                    kwds['vmin'] = np.nanpercentile( data, kwds['vmin'] )
+            if 'vmax' in kwds:
+                if isinstance(kwds['vmax'], int):
+                    kwds['vmax'] = np.nanpercentile( data, kwds['vmax'] )
 
             #mask nans (and apply custom mask)
             mask = np.isnan(data)
             if not np.isnan(self.header.get_data_ignore_value()):
                 mask = mask + data == self.header.get_data_ignore_value()
             if 'mask' in kwds:
                 mask = mask + kwds.get('mask')
                 del kwds['mask']
             data = np.ma.array(data, mask = mask > 0 )
 
-            # convert integer vmin and vmax values to percentiles
-            if 'vmin' in kwds:
-                if isinstance(kwds['vmin'], int):
-                    kwds['vmin'] = np.nanpercentile( data, kwds['vmin'] )
-            if 'vmax' in kwds:
-                if isinstance(kwds['vmax'], int):
-                    kwds['vmax'] = np.nanpercentile( data, kwds['vmax'] )
-
             # apply rotations and flipping
             if rot:
                 data = data.T
             if flipX:
                 data = data[::-1, :]
             if flipY:
                 data = data[:, ::-1]
 
-            ax.cbar = ax.imshow(data.T, interpolation=kwds.pop('interpolation', 'none'), **kwds)
+            # save?
+            if 'path' in kwds:
+                path = kwds.pop('path')
+                from matplotlib.pyplot import imsave
+                if not os.path.exists(os.path.dirname(path)):
+                    os.makedirs(os.path.dirname(path)) # ensure output directory exists
+                imsave(path, data.T, **kwds)  # save the image
+
+            ax.cbar = ax.imshow(data.T, interpolation=kwds.pop('interpolation', 'none'), **kwds) # change default interpolation to None
 
         #map 3 bands to RGB
         elif isinstance(band, tuple) or isinstance(band, list):
             #get band indices and range
             rgb = []
             for b in band:
-                rgb.append( self.get_band_index( b ) )
+                if isinstance(b, str):
+                    rgb.append(self.get_band_index(b))
+                else:
+                    rgb.append(self.get_band_index(np.abs(b)))
 
             #slice image (as copy) and map to 0 - 1
             img = np.array(self.data[:, :, rgb]).copy()
             if np.isnan(img).all():
                 print("Warning - image contains no data.")
                 return ax.get_figure(), ax
 
+            # invert if needed
+            for i,b in enumerate(band):
+                if not isinstance(b, str) and (b < 0):
+                    img[..., i] = np.nanmax(img[..., i]) - img[..., i]
+
             # do scaling
             if tscale: # scale bands independently
                 for b in range(3):
                     mn = kwds.get("vmin", float(np.nanmin(img)))
                     mx = kwds.get("vmax", float(np.nanmax(img)))
                     if isinstance (mn, int):
                         assert mn >= 0 and mn <= 100, "Error - integer vmin values must be a percentile."
```

### Comparing `hylite-1.21/hylite/hylibrary.py` & `hylite-1.23/hylite/hylibrary.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/hyscene.py` & `hylite-1.23/hylite/hyscene.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/io/__init__.py` & `hylite-1.23/hylite/io/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .pmaps import *
 from .cameras import saveCameraTXT, loadCameraTXT
 
 from hylite import HyImage, HyCloud, HyLibrary, HyCollection, HyScene, HyData
 from hylite.project import PMap, Camera, Pushbroom
 from hylite.analyse.mwl import MWL
 from distutils.dir_util import copy_tree
+import os
 
 # check if gdal is installed
 try:
     from osgeo import gdal
     usegdal = True
 except ModuleNotFoundError:
     usegdal = False
@@ -38,23 +39,33 @@
 
     if isinstance(data, HyImage):
 
         # special case - save ternary image to png or jpg or bmp
         ext = os.path.splitext(path)[1].lower()
         if 'jpg' in ext or 'bmp' in ext or 'png' in ext or 'pdf' in ext:
             if data.band_count() == 1 or data.band_count() == 3 or data.band_count == 4:
-                from matplotlib.pyplot import imsave
                 rgb = np.transpose( data.data, (1,0,2) )
                 if not ((data.is_int() and np.max(rgb) <= 255)): # handle normalisation
                     vmin = kwds.get("vmin", np.nanpercentile(rgb, 1 ) )
                     vmax = kwds.get("vmax", np.nanpercentile(rgb, 99) )
                     rgb = (rgb - vmin) / (vmax-vmin)
                     rgb = (np.clip(rgb, 0, 1) * 255).astype(np.uint8) # convert to 8 bit image
-                imsave( path, rgb ) # save the image
+                #from matplotlib.pyplot import imsave
+                # imsave( path, rgb )
+                from skimage import io as skio
+                skio.imsave( path, rgb ) # save the image
                 return
+        elif ((data.band_count() == 3) or (data.band_count() == 4)) and (data.data.dtype == np.uint8):
+            # save 3 and 4 band uint8 arrays as png files
+            # from matplotlib.pyplot import imsave
+            # imsave( os.path.splitext(path)[0]+".png", data.data)  # save the image
+            from skimage import io as skio
+            skio.imsave(os.path.splitext(path)[0]+".png", np.transpose( data.data, (1,0,2) ))  # save the image
+            save( os.path.splitext(path)[0] + ".hdr", data.header ) # save header
+            return
         else: # save hyperspectral image
             if usegdal:
                 from osgeo import gdal  # is gdal installed?
                 save_func = saveWithGDAL
             else:  # no gdal, use SPy
                 save_func = saveWithSPy
             if 'lib' in ext: # special case - we are actually saving a HyLibrary (as an image)
@@ -79,35 +90,38 @@
     elif isinstance(data, Pushbroom):
         save_func = saveCameraTXT
         ext = 'brm'
     elif isinstance(data, HyCollection):
         save_func = _saveCollection
         ext = data.ext[1:]
         outdir = os.path.join(data.root, os.path.splitext(data.name)[0])
+        os.makedirs( os.path.splitext(path)[0] +"."+ ext, exist_ok=True ) # make output directory (even if empty)
         if os.path.splitext(path)[0] != outdir:
             if os.path.exists( outdir+"."+ext): # if it exists...
                 #if sys.version_info[1] >= 8: # python 3.8 or greater
                 #    shutil.copytree( outdir+"."+ext, os.path.splitext(path)[0]+"."+ext, dirs_exist_ok=True)
                 #else:
                 #    shutil.copytree( outdir+"."+ext, os.path.splitext(path)[0]+"."+ext ) # will fail if directory already exists unfortunately.
                 copy_tree(outdir+"."+ext, os.path.splitext(path)[0]+"."+ext)
 
-    elif isinstance(data, np.ndarray):
+
+    elif isinstance(data, np.ndarray) or isinstance(data, list):
         save_func = np.save
         ext = 'npy'
     else:
         assert False, "Error - data type %s is unsupported by hylite.io.save." % type(data)
 
     # check path file extension
     if 'hdr' in os.path.splitext(path)[1]: # auto strip .hdr extensions if provided
         path = os.path.splitext(path)[0]
     if ext not in os.path.splitext(path)[1]: # add type-specific extension if needed
         path += '.%s'%ext
 
     # save!
+    os.makedirs( os.path.dirname(path), exist_ok=True)  # make output directory
     save_func( path, data )
 
 def load(path):
     """
     A generic function for loading hyperspectral images, point clouds and libraries. The appropriate load function
     will be chosen based on the file extension.
 
@@ -124,15 +138,15 @@
     if 'npz' in os.path.splitext( path )[1].lower():
         return loadPMap(path)
     elif 'npy' in os.path.splitext( path )[1].lower():
         return np.load( path ) # load numpy
 
     # file (should/could) have header - look for it
     header, data = matchHeader( path )
-    assert os.path.exists(data), "Error - data file %s does not exist." % path
+    assert os.path.exists(str(data)), "Error - data file %s does not exist." % path
     ext = os.path.splitext(data)[1].lower()
     if ext == '':
         assert os.path.isfile(data), "Error - %s is a directory not a file." % data
 
     # load other file types
     if 'ply' in ext: # point or hypercloud
         out = loadCloudPLY(path) # load dataset
@@ -150,16 +164,23 @@
         out = _loadCollection(path)
     elif 'cam' in ext or 'brm' in ext: # load pushbroom and normal cameras
         out = loadCameraTXT(path)
     else: # image
         # load conventional images with PIL
         if 'png' in ext or 'jpg' in ext or 'bmp' in ext:
             # load image with matplotlib
-            from matplotlib.pyplot import imread
-            out = HyImage(np.transpose(imread(path), (1, 0, 2)))
+            #from matplotlib.pyplot import imread
+            #im = imread(path)
+            from skimage import io as skio
+            im = skio.imread(data)
+            if len(im.shape) == 2:
+                im = im[:,:,None] # add last dimension if greyscale image is loaded
+            out = HyImage(np.transpose(im, (1, 0, 2)))
+            if header is not None:
+                out.header = loadHeader(header)
         else:
             if usegdal:
                 from osgeo import gdal # is gdal installed?
                 out = loadWithGDAL(path)
             else: # no gdal, use SPy
                 out = loadWithSPy(path)
 
@@ -172,17 +193,17 @@
 ## save and load data collections
 ##############################################
 # save collection
 def _saveCollection(path, collection):
     # generate file paths
     dirmap = collection.get_file_dictionary(root=os.path.dirname(path),
                                             name=os.path.splitext(os.path.basename(path))[0])
-    # save files
+    # print(dirmap)
     for p, o in dirmap.items():
-        os.makedirs(os.path.dirname(p), exist_ok=True)
+        os.makedirs(os.path.dirname(p), exist_ok=True) # make output directory if needed
         save(p, o)  # save each path and item [ n.b. this includes the header file! :-) ]
 
 def _loadCollection(path):
     # load header and find directory path
     header, directory = matchHeader(path)
 
     # parse name and root
@@ -192,10 +213,10 @@
     if 'hyc' in os.path.splitext(directory)[1]:
         C = HyCollection(name, root, header=loadHeader(header))
     elif 'hys' in os.path.splitext(directory)[1]:
         C = HyScene(name, root, header=loadHeader(header))
     elif 'mwl' in os.path.splitext(directory)[1]:
         C = MWL(name, root, header=loadHeader(header))
     else:
-        print(header, directory )
+        # print(header, directory )
         assert False, "Error - %s is an invalid collection." % directory
     return C
```

### Comparing `hylite-1.21/hylite/io/cameras.py` & `hylite-1.23/hylite/io/cameras.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,20 +58,20 @@
         #trim comments
         lines = [l.split('#')[0].strip() for l in lines]
         if 'camera' in lines[0].lower():
             pos = np.fromstring( lines[1], sep=',')
             ori = np.fromstring( lines[2], sep=',')
             proj = lines[3]
             fov = float(lines[4])
-            dims = tuple( np.fromstring( lines[5], sep=',').astype(np.int))
+            dims = tuple( np.fromstring( lines[5], sep=',').astype(int))
             step  = None
             if len(lines) > 6:
                 step = float( lines[6] )
             return Camera(pos, ori, proj, fov, dims, step)
         elif 'pushbroom' in lines[0].lower():
 
             xfov, lfov = np.fromstring( lines[1], sep=',')
-            dims = tuple( np.fromstring( lines[2], sep=',').astype(np.int))
+            dims = tuple( np.fromstring( lines[2], sep=',').astype(int))
             cp = np.array([ np.fromstring(lines[3+i], sep=',') for i in range(3)]).T
             co = np.array([ np.fromstring(lines[6+i], sep=',') for i in range(3)]).T
 
             return Pushbroom( cp, co,  xfov, lfov, dims )
```

### Comparing `hylite-1.21/hylite/io/clouds.py` & `hylite-1.23/hylite/io/clouds.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 
     #add rgb (as integers)
     if cloud.has_rgb():
         header += '%sr%sg%sb' % (d, d, d)
         format += ['%d', '%d', '%d']
         if cloud.rgb.dtype == np.uint8:
             data.append(cloud.rgb)
-        elif cloud.rgb.dtype == np.float or cloud.rgb.dtype == np.float32:
-            data.append((cloud.rgb * 255).astype(np.int))
+        elif cloud.rgb.dtype == np.float64 or cloud.rgb.dtype == np.float32:
+            data.append((cloud.rgb * 255).astype(int))
         else:
             print("Warning - unknown data type for RGB colours (%s)" % cloud.rgb.dtype)
 
     #add normals
     if cloud.has_normals():
         header += '%sNx%sNy%sNz' % (d, d, d)
         format += [fmt, fmt, fmt]
@@ -186,18 +186,18 @@
 
     # export point colours
     if cloud.has_rgb():
         if cloud.rgb.dtype == np.uint8: #RGB is 0-255
             outfile.red = cloud.rgb[:, 0]
             outfile.green = cloud.rgb[:, 1]
             outfile.blue = cloud.rgb[:, 2]
-        elif cloud.rgb.dtype is np.float or cloud.rgb.dtype is np.float32: #RGB is 0-1
-            outfile.red = (cloud.rgb[:, 0] * 255).astype(np.int)
-            outfile.green = (cloud.rgb[:, 1] * 255).astype(np.int)
-            outfile.blue = (cloud.rgb[:, 2] * 255).astype(np.int)
+        elif cloud.rgb.dtype is np.float64 or cloud.rgb.dtype is np.float32: #RGB is 0-1
+            outfile.red = (cloud.rgb[:, 0] * 255).astype(int)
+            outfile.green = (cloud.rgb[:, 1] * 255).astype(int)
+            outfile.blue = (cloud.rgb[:, 2] * 255).astype(int)
         else:
             print("Warning - unknown data type for RGB colours (%s)" % cloud.rgb.dtype)
 
     outfile.close()
 
     #write header file
     if not cloud.header is None:
@@ -326,15 +326,15 @@
                 data = cloud.data  # no need to do any mapping :)
             else:
                 cloud.compress()
                 data = cloud.data
         elif 'f4' in sfmt.lower():
             if cloud.data.dtype == np.float32:
                 data = cloud.data  # no need to do any mapping :)
-            elif cloud.data.dtype == np.float:
+            elif cloud.data.dtype == np.float64:
                 data = cloud.data.astype(np.float32)
             else:
                 cloud.decompress()
                 data = cloud.data.astype(np.float32)
         else:
             assert False, "Error - %s is an invalid data format." % sfmt
         # build data arrays
```

### Comparing `hylite-1.21/hylite/io/headers.py` & `hylite-1.23/hylite/io/headers.py`

 * *Files 7% similar despite different names*

```diff
@@ -79,26 +79,28 @@
     # store path
     header['path'] = path
 
     inblock = False
     try:
         hdrfile = open(path, "r")
     except:
-        print("Could not open hdr file %s" % str(path))
-        return
+        if path is not None: # no header file exists. This is not necessarily an issue.
+            print("Could not open hdr file %s" % str(path))
+        return None
 
     # Read line, split it on equals, strip whitespace from resulting strings and add key/value pair to output
     currentline = hdrfile.readline()
     while (currentline != ""):
         # ENVI headers accept blocks bracketed by curly braces - check for these
         if not inblock:
             # Split line on first equals sign
             if (re.search("=", currentline) is not None):
                 linesplit = re.split("=", currentline, 1)
-                key = str.lower(linesplit[0].strip())
+                # key = str.lower(linesplit[0].strip())
+                key = linesplit[0].strip()
                 value = linesplit[1].strip()
 
                 # If value starts with an open brace, it's the start of a block - strip the brace off and read the rest of the block
                 if (re.match("{", value) is not None):
                     inblock = True
                     value = re.sub("^{", "", value, 1)
                     # If value ends with a close brace it's the end of the block as well - strip the brace off
@@ -117,14 +119,17 @@
                 value = value.strip()
             header[key] = header[key] + value
         currentline = hdrfile.readline()
     hdrfile.close()
 
     #convert default things like wavelength data to numeric form
     #N.B. wavelength should ALWAYS be stored as nanometres
+    if 'Wavelength' in header: # drop upper case wavelength for some files
+        header['wavelength'] = header['Wavelength']
+        del header['Wavelength']
     if "wavelength" in header:
         units = header.get("wavelength units", "nm").lower()
         if "nm" in units or "nano" in units: #units in nanometers
             header['wavelength'] = np.fromstring(header['wavelength'], sep=',')
         elif "um" in units or "micro" in units:
             header['wavelength'] = np.fromstring(header['wavelength'], sep=',') * 1000.0
         elif "mm" in units or "milli" in units:
@@ -190,15 +195,17 @@
                     and not "txt" in str.lower(os.path.splitext(m)[1]) \
                     and not "xml" in str.lower(os.path.splitext(m)[1]) \
                     and not "cam" in str.lower(os.path.splitext(m)[1]) \
                     and not "brm" in str.lower(os.path.splitext(m)[1]):
 
                 image = m  # store matching image file
                 break
-
+            elif (os.path.splitext(m)[0] == path) and (image is None):
+                image = m # .png files can be valid, but should be lower priority, so store but continue looking
+                          # in case there is e.g., a .dat file also.
     # we have an image file, find associated header file
     else:
         image = path + ext
         for m in match:
             if ".hdr" in str.lower(m) and os.path.splitext(m)[0] == path:
                 header = m
                 break
```

### Comparing `hylite-1.21/hylite/io/images.py` & `hylite-1.23/hylite/io/images.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Read common image formats, including ENVI format hyperspectral data.
 """
 
 import sys, os
 import numpy as np
 import spectral
-from hylite.hyimage import HyImage
+from hylite.hyimage import HyImage, HyData
 from .headers import matchHeader, makeDirs, loadHeader, saveHeader
 
 # spectral python throws depreciation warnings - ignore these!
 import warnings
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 
 def loadWithGDAL(path, dtype=np.float32, mask_zero = True):
@@ -58,15 +58,15 @@
 
     #create image object
     assert data is not None, "Error - GDAL could not retrieve valid image data from %s" % path
     pj = raster.GetProjection()
     gt = raster.GetGeoTransform()
     img = HyImage(data, projection=pj, affine=gt, header=header, dtype=dtype)
 
-    if mask_zero and img.dtype == np.float:
+    if mask_zero and (img.dtype == np.float32 or img.dtype == np.float64):
             img.data[img.data == 0] = np.nan #note to self: np.nan is float...
 
     return img
 
 def loadWithSPy( path, dtype=np.float32, mask_zero = True):
     """
     Load an image using spectral python. This works for most envi images, but doesn not load
@@ -113,15 +113,15 @@
     # create image object
     assert data is not None, "Error - GDAL could not retrieve valid image data from %s" % path
     img = HyImage(data, projection=None, affine=None, header=header, dtype=dtype)
 
     # spectral python automatically applies reflectance scale factor, so we must set this to 1.0 to avoid future nightmares...
     img.header['reflectance scale factor'] = 1.0
 
-    if mask_zero and img.dtype == np.float:
+    if mask_zero and img.dtype == float:
         img.data[img.data == 0] = np.nan  # note to self: np.nan is float...
 
     return img
 
 def loadSubset( path, *, bands=None, pixels=None, dtype=np.float32, mask_zero=True):
     """
     Load either specific bands (bands!=None) or pixels (pixels != None) from an ENVI file using spy to facilitate e.g. out-of-core
@@ -154,24 +154,24 @@
         # load image with SPy
         assert os.path.exists(image), "Error - %s does not exist." % image
         try:  # try loading envi file first
             img = spectral.envi.open(header, image)  # this must be an envi file
         except:
             img = spectral.open_image(header)  # load unknown image type
 
-
         if bands is not None:  # get bands and put in HyImage
             data = np.dstack( [ img.read_band( b ).T for b in bands ] )
             out = HyImage( data, projection=None, affine=None, header=imageheader, dtype=dtype)
             out.set_wavelengths( imageheader.get_wavelengths()[bands] )
             if out.has_band_names():
                 out.set_band_names( imageheader.get_band_names()[bands])
         if pixels is not None:  # get pixels and put in HyCloud
-            assert False, "Error - this has not yet been implemented."
-            data = np.array( [ img.read_pixel( *p ) for p in pixels ] )
+            data = np.array( [ img.read_pixel( *p[::-1] ) for p in pixels ] )
+            out = HyData( data )
+            out.header=imageheader
         return out
 
 
 
 
 
 # noinspection PyUnusedLocal
@@ -215,15 +215,15 @@
         image.header['byte order'] = 1
 
     #parse data type from image array
     data = image.data
     dtype = gdal.GDT_Float32
     image.header["data type"] = 4
     image.header["interleave"] = str.lower(interleave)
-    if image.data.dtype == np.int or image.data.dtype == np.int32:
+    if image.data.dtype == np.intc or image.data.dtype == np.int32:
         dtype = gdal.GDT_Int32
         image.header["data type"] = 3
     if image.data.dtype == np.int16:
         dtype = gdal.GDT_Int16
         image.header["data type"] = 2
     if image.data.dtype == np.uint8:
         data = np.array(image.data, np.dtype('b'))
@@ -277,9 +277,9 @@
         byteorder = 0
     else:
         image.header['byte order'] = 1
         byteorder = 1
 
     image.push_to_header()
     spectral.envi.save_image( path + ".hdr", np.transpose(image.data,(1,0,2)),
-                                dtype=image.data.dtype, force=True,
-                                ext=ext, byteorder=byteorder, metadata=image.header)
+                                    dtype=image.data.dtype, force=True,
+                                    ext=ext, byteorder=byteorder, metadata=image.header)
```

### Comparing `hylite-1.21/hylite/io/libraries.py` & `hylite-1.23/hylite/io/libraries.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,24 +178,24 @@
         for i,n in enumerate(library.get_sample_names()):
             f.write( str(n) + ", " + str(list( library.data[i,0,:] ))[1:-1] + '\n' )
     f.close()
 
 def loadLibraryCSV(path):
     with open(path, 'r') as f:
         header = f.readline()
-        wav = np.array( header.split(",")[1:], dtype=np.float)
+        wav = np.array( header.split(",")[1:], dtype=float)
 
         # parse spectra
         names = []
         refl = []
         l = f.readline()
         while l:
             l = l.split(",")
             names.append( l[0] )
-            refl.append( np.array(l[1:],dtype=np.float) )
+            refl.append( np.array(l[1:],dtype=float) )
             l = f.readline()
     return HyLibrary( np.array(refl), names, wav=wav )
 
 
 def loadLibraryTXT(path):
     """
     Load an ENVI text format library. This should have the following structure:
```

### Comparing `hylite-1.21/hylite/io/pmaps.py` & `hylite-1.23/hylite/io/pmaps.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/multiprocessing.py` & `hylite-1.23/hylite/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/project/align.py` & `hylite-1.23/hylite/project/align.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     assert len(points) >= 4, "Error - at least four pixel/point pairs are needed to solve PnP problem."
 
     # get world coordinate array
     points = np.array(points).astype(np.uint)
     kxyz = cloud.xyz[ points, : ]
 
     # get pixel coordinates array
-    kxy = np.array( pixels ).astype(np.float) - 0.5 # must be float for OpenCV. - 0.5 transforms to pixel centers.
+    kxy = np.array( pixels ).astype(float) - 0.5 # must be float for OpenCV. - 0.5 transforms to pixel centers.
 
     # solve pnp problem
     if 'pano' in cam.proj.lower():
         kxy_pp = pano_to_persp(kxy[:,0], kxy[:, 1], cam.fov, cam.step, cam.dims)
         p_est, r_est, inl = pnp(kxyz, kxy_pp, cam.fov, cam.dims, ransac=True, **kwds)
     else:
         p_est, r_est, inl = pnp(kxyz, kxy, cam.fov, cam.dims, ransac=True, **kwds)
```

### Comparing `hylite-1.21/hylite/project/basic.py` & `hylite-1.23/hylite/project/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         - vis = a (n,) array scored with True if the corresponding point is visible from the camera.
     """
 
     #transform origin to camera position
     xyz = xyz - C[None,:]
 
     # backface culling
-    vis = np.full(xyz.shape[0],True,dtype=np.bool)
+    vis = np.full(xyz.shape[0],True,dtype=bool)
     if not normals is None:
         ndv = np.einsum('ij, ij->i', normals, xyz) #calculate dot product between each normal and vector from camera to point
                                                    #(which is the point position vector in this coordinate system)
         vis = ndv < 0 #normal is pointing towards the camera (in opposite direction to view)
 
     #apply camera rotation to get to coordinate system
     #  where y is camera up and z distance along the view axis
@@ -81,15 +81,15 @@
         - vis = a (n,) array scored with True if the corresponding point is visible from the camera.
     """
 
     # transform origin to camera position
     xyz = xyz - C[None, :]
 
     # backface culling
-    vis = np.full(xyz.shape[0], True, dtype=np.bool)
+    vis = np.full(xyz.shape[0], True, dtype=bool)
     if not normals is None:
         ndv = np.einsum('ij, ij->i', normals,
                         xyz)  # calculate dot product between each normal and vector from camera to point
         # (which is the point position vector in this coordinate system)
         vis = ndv < 0  # normal is pointing towards the camera (in opposite direction to view)
 
     # apply camera rotation to get to coordinate system
```

### Comparing `hylite-1.21/hylite/project/camera.py` & `hylite-1.23/hylite/project/camera.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/project/pmap.py` & `hylite-1.23/hylite/project/pmap.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
             vis: point visibilities, as returned by e.g. proj_pano.
         """
         # convert to indices
         pid = np.argwhere(vis)[:, 0]
         pp = pp[vis]
 
         # convert pixel indices to flat indices
-        pix = np.ravel_multi_index(pp[:,[0,1]].astype(np.int).T, dims=(self.xdim, self.ydim), order='F')
+        pix = np.ravel_multi_index(pp[:,[0,1]].astype(int).T, dims=(self.xdim, self.ydim), order='F')
 
         # set data values
         self.set_flat( pid, pix, pp[:,2] )
 
     def size(self):
         """
         How many relationships are stored in this?
```

### Comparing `hylite-1.21/hylite/project/pushbroom.py` & `hylite-1.23/hylite/project/pushbroom.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/reference/features/__init__.py` & `hylite-1.23/hylite/reference/features/__init__.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/reference/spectra/__init__.py` & `hylite-1.23/hylite/reference/spectra/__init__.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/reference/spectra/pvc/PVC_Black.txt` & `hylite-1.23/hylite/reference/spectra/pvc/PVC_Black.txt`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/reference/spectra/pvc/PVC_Grey.txt` & `hylite-1.23/hylite/reference/spectra/pvc/PVC_Grey.txt`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/reference/spectra/pvc/PVC_Red.txt` & `hylite-1.23/hylite/reference/spectra/pvc/PVC_Red.txt`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/reference/spectra/pvc/PVC_White.txt` & `hylite-1.23/hylite/reference/spectra/pvc/PVC_White.txt`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/reference/spectra/spectralon/R50.txt` & `hylite-1.23/hylite/reference/spectra/spectralon/R50.txt`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/reference/spectra/spectralon/R55_SiSu.txt` & `hylite-1.23/hylite/reference/spectra/spectralon/R55_SiSu.txt`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/reference/spectra/spectralon/R6.txt` & `hylite-1.23/hylite/reference/spectra/spectralon/R6.txt`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/reference/spectra/spectralon/R90.txt` & `hylite-1.23/hylite/reference/spectra/spectralon/R90.txt`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/sensors/__init__.py` & `hylite-1.23/hylite/sensors/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         image (hylite.HyImage): the image containing data from the sensor..
         method (str): "LDPE" for SWIR using reference LDPE foil, "FT" for VNIR using fluorescence tube.
         dim (int): dimensionality of the evaluation (0 = overall average, 1 = row-wise, 2 = full frame).
         fit (str): method for peak fitting. For details, check hylite.analyse.mapping.minimum_wavelength( ... ).
         checklines (list): define custom features to check for (list of ints or floats).
     """
 
-    image.data = image.data.astype(np.float)
+    image.data = image.data.astype(np.float32)
 
     # define indicative feature lines
     if method == "FT":
         checklines = [404.66, 435.83, 546.08, 611.08]
         image.data = np.nanmax(image.data) - image.data
     elif method == "LDPE":
         checklines = [1728., 1764., 2310., 2350.]
```

### Comparing `hylite-1.21/hylite/sensors/calibration_data/fenix/Radiometric_2x2_1x1.dat` & `hylite-1.23/hylite/sensors/calibration_data/fenix/Radiometric_2x2_1x1.dat`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/sensors/calibration_data/fenix/Radiometric_2x2_1x1.hdr` & `hylite-1.23/hylite/sensors/calibration_data/fenix/Radiometric_2x2_1x1.hdr`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/sensors/calibration_data/fenix/Radiometric_4x2_1x1.dat` & `hylite-1.23/hylite/sensors/calibration_data/fenix/Radiometric_4x2_1x1.dat`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/sensors/calibration_data/fenix/Radiometric_4x2_1x1.hdr` & `hylite-1.23/hylite/sensors/calibration_data/fenix/Radiometric_4x2_1x1.hdr`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/sensors/calibration_data/fenix/Radiometric_8x2_1x1.dat` & `hylite-1.23/hylite/sensors/calibration_data/fenix/Radiometric_8x2_1x1.dat`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/sensors/calibration_data/fenix/Radiometric_8x2_1x1.hdr` & `hylite-1.23/hylite/sensors/calibration_data/fenix/Radiometric_8x2_1x1.hdr`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/sensors/calibration_data/fenix1k/Radiometric_2x2_1x1.dat` & `hylite-1.23/hylite/sensors/calibration_data/fenix1k/Radiometric_2x2_1x1.dat`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/sensors/calibration_data/fenix1k/Radiometric_2x2_1x1.hdr` & `hylite-1.23/hylite/sensors/calibration_data/fenix1k/Radiometric_2x2_1x1.hdr`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/sensors/calibration_data/fenix1k/Radiometric_4x2_1x1.dat` & `hylite-1.23/hylite/sensors/calibration_data/fenix1k/Radiometric_4x2_1x1.dat`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/sensors/calibration_data/fenix1k/Radiometric_4x2_1x1.hdr` & `hylite-1.23/hylite/sensors/calibration_data/fenix1k/Radiometric_4x2_1x1.hdr`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/sensors/calibration_data/fenix1k/Radiometric_8x2_1x1.dat` & `hylite-1.23/hylite/sensors/calibration_data/fenix1k/Radiometric_8x2_1x1.dat`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/sensors/calibration_data/fenix1k/Radiometric_8x2_1x1.hdr` & `hylite-1.23/hylite/sensors/calibration_data/fenix1k/Radiometric_8x2_1x1.hdr`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite/sensors/fenix.py` & `hylite-1.23/hylite/sensors/fenix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 from pathlib import Path
 import cv2
 import numpy.ma as ma
+import hylite
 import hylite.io as io
 from .sensor import Sensor
 
 class Fenix(Sensor):
     """
     Implementation of sensor corrections for the Fenix sensor.
     """
@@ -56,30 +57,30 @@
         Apply sensor corrections to an image.
 
         Args:
             image (hylite.HyImage): a hyImage instance of an image captured using this sensor.
             verbose (bool): true if updates/progress should be printed to the console. Default is False.
             **kwds: Optional arguments include:
 
-                 - rad = true if image should be converted to radiance by applying dark reference. Default is True.
+                 - rad = true if image should be converted to reflectance by applying white and dark reference. Default is True.
                  - bpr = replace bad pixels (only for raw data). Default is True.
                  - shift = shift bands to account for time-delay between their acquisitions.
                            Only use for near-field sensing (e.g. drill-core scans). Default is False.
                  - flip = true if image should be flipped before applying lens correction (if camera mounted backwards in core
                           scanner). Default is False.
                  - lens = apply GLTX lens correction to remove lens distortion. Default is True.
 
         """
 
         # get kwds
         rad = kwds.get("rad", True)
         bpr = kwds.get("bpr", True)
         shift = kwds.get("shift", False)
         lens = kwds.get("lens", True)
-
+        noise = kwds.get("noise", False) # true if noise info should be calculated and returned.
         if rad:
             if verbose: print("Converting to radiance... ", end="", flush="True")
 
             # convert from int to float
             image.data = image.data.astype(np.float32)
 
             # find saturation and store in mask
@@ -154,39 +155,49 @@
             image.data[..., :r] /= exp_vnir
             image.data[..., r:] /= exp_swir
 
             # apply white reference (if specified)
             if not cls.white is None:
 
                 # calculate white reference radiance
-                white = np.nanmean(cls.white.data.astype(np.float32),
-                                   axis=1) - dref  # average each line and subtract dark reference
-                white *= cal  # apply laboratory calibration to white reference
+                white = cls.white.data.astype(np.float32) - dref[:,None,:]  # subtract dark current
+                white *= cal[:,None,:]  # apply laboratory calibration to white reference
 
                 # extract white (or grey) reference reflectance
                 if cls.white_spectra is None:
-                    refl = np.zeros(white.shape[1]) + 1.0  # assume pure white
+                    refl = np.zeros(white.shape[-1]) + 1.0  # assume pure white
                 else:
                     # get known target spectra
                     refl = cls.white_spectra.get_reflectance()
 
                     # match bands with this image
                     idx = [np.argmin(cls.white_spectra.get_wavelengths() < w) for w in image.get_wavelengths()]
                     refl = refl[idx]
 
                 # divide by exposure (in ms)
                 exp_vnir = float(cls.white.header.get('tint1', 1.0))
                 exp_swir = float(cls.white.header.get('tint2', 1.0))
                 white[..., :r ]  /= exp_vnir
                 white[..., r: ] /= exp_swir
 
-                # apply white reference
-                cfac = refl[None, :] / white
+                # divide by white value to get reflectance
+                cfac = refl[None, :] / np.nanmean( white, axis=1 )
                 image.data[:, :, :] *= cfac[:, None, :]
 
+                # also compute noise model (as this can come in handy during analyses)
+                if noise:
+                    X = hylite.HyImage(white*cfac[:,None,:]).X(onlyFinite=True)
+                    mean = np.mean(X, axis=0)
+                    X = X - mean[None, :]
+
+                    # calculate covariance
+                    noise_std = np.std(X, axis=0 )
+                    noise_cov = np.cov(X.T)
+                    image.header['band noise'] = noise_std
+
             if verbose: print("DONE.")
 
         ##############################################################
         # replace bad pixels with an average of the surrounding ones
         ##############################################################
         if bpr:
             if verbose: print("Filtering bad pixels... ", end="", flush="True")
@@ -317,14 +328,17 @@
 
             image.data = remap
             if verbose: print("DONE.")
 
         # rotate image so that scanning direction is horizontal rather than vertical)
         image.data = np.rot90(image.data)  # np.transpose(remap, (1, 0, 2))
         image.data = np.flip(image.data, axis=1)
+        image.set_band_names(None) # delete band names as they get super annoying
+        if noise:
+            return noise_std, noise_cov
 
     @classmethod
     def correct_folder(cls, path, **kwds):
 
         """
         Many sensors use simple/common data structures to store data/headers/dark reference etc. Hence it is often easiest
         to pass an output folder to the sensor for correction.
@@ -354,22 +368,25 @@
             del imgs[imgs.index(w)]
         for r in refl:
             del imgs[imgs.index(r)]
 
         if len(imgs) > 1 or len(
             dark) > 1: assert False, "Error - multiple scenes found in folder. Double check file path..."
         if len(imgs) == 0 or len(
-            dark) == 0: assert False, "Error - no image or dark calibration found in folder. Double check file path... %s" % path
+            dark) == 0: assert False, ("Error - no image or dark calibration found in folder. Double check file path... %s"%path)
 
         if verbose: print('\nLoading image %s' % imgs[0])
 
         # load image
         image = io.load(imgs[0])
         Fenix.set_dark_ref(dark[0])
         if len(white) > 0:  # white reference exists
             Fenix.set_white_ref(white[0])
 
         # correct
-        Fenix.correct_image(image, **kwds)
+        noise = Fenix.correct_image(image, **kwds)
 
         # return corrected image
-        return image
+        if noise is not None:
+            return image, noise[0], noise[1]
+        else:
+            return image
```

### Comparing `hylite-1.21/hylite/sensors/fx.py` & `hylite-1.23/hylite/sensors/fx.py`

 * *Files 3% similar despite different names*

```diff
@@ -224,28 +224,30 @@
             else:
                 dref = np.nanmean(cls.dark.data, axis=1)  # calculate dark reference
                 image.data[:, :, :] -= dref[:, None, :]  # apply dark calibration
 
             # apply white reference (if specified)
             if not cls.white is None:
                 # calculate white reference radiance
-                white = np.nanmean(cls.white.data.astype(np.float32),
-                                   axis=1) - dref  # average each line and subtract dark reference
-
-                refl = np.ones(white.shape[1])  # assume pure white
+                white = cls.white.data.astype(np.float32) - dref[:,None,:]  # average each line and subtract dark reference
+                refl = np.ones(white.shape[-1])  # assume white panel is pure white
 
                 # apply white reference
-                cfac = refl[None, :] / white
+                cfac = refl[None, :] / np.nanmean( white, axis=1 )
                 image.data[:, :, :] *= cfac[:, None, :]
 
+                # also estimate noise per-band (useful for eg., MNFs)
+                noise = np.nanstd(white * cfac[:, None, :], axis=(0, 1))
+                image.header['band noise'] = noise
+
             if verbose: print("DONE.")
 
-        ##############################################################
-        # replace bad pixels with an average of the surrounding ones
-        ##############################################################
+        ###################################################################
+        # replace bad (nan) pixels with an average of the surrounding ones
+        ###################################################################
         if bpr:
             if verbose: print("Filtering bad pixels... ", end="", flush="True")
             invalids = np.argwhere(np.isnan(image.data) | np.isinf(image.data))  # search for bad pixels
             for px, py, band in invalids:
                 n = 0
                 sum = 0
                 for xx in range(px - 1, px + 2):
@@ -260,14 +262,15 @@
                 if n > 0: sum /= n  # do averaging
                 image.data[px][py][band] = sum
             if verbose: print("DONE.")
 
         # rotate image so that scanning direction is horizontal rather than vertical)
         image.data = np.rot90(image.data)  # np.transpose(remap, (1, 0, 2))
         image.data = np.flip(image.data, axis=1)
+        image.set_band_names(None)  # delete band names as they get super annoying
 
     @classmethod
     def correct_folder(cls, path, **kwds):
 
         """
         Many sensors use simple/common data structures to store data/headers/dark reference etc. Hence it is often easiest
         to pass an output folder to the sensor for correction.
```

### Comparing `hylite-1.21/hylite/sensors/owl.py` & `hylite-1.23/hylite/sensors/owl.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,28 +85,28 @@
             else:
                 dref = np.nanmean(cls.dark.data, axis=1)  # calculate dark reference
                 image.data[:, :, :] -= dref[:, None, :lim]  # apply dark calibration
 
             # apply white reference (if specified)
             if not cls.white is None:
                 # calculate white reference radiance
-                white = np.nanmean(cls.white.data.astype(np.float32),
-                                   axis=1) - dref  # average each line and subtract dark reference
-
-                refl = np.ones(white.shape[1])  # assume pure white
+                white = cls.white.data.astype(np.float32) - dref[:, None, :]
+                refl = np.ones(white.shape[-1])  # assume pure white
 
                 # apply white reference
-                cfac = refl[None, :] / white
+                cfac = refl[None, :] / np.nanmean( white, axis=1 )
                 image.data[:, :, :] *= cfac[:, None, :lim]
+                white = white[:,:,:lim] * cfac[:, None, :lim]
+
 
             if verbose: print("DONE.")
 
-        ##############################################################
-        # replace bad pixels with an average of the surrounding ones
-        ##############################################################
+        ####################################################################
+        # replace bad (nan) pixels with an average of the surrounding ones
+        ####################################################################
         if bpr:
             if verbose: print("Filtering bad pixels... ", end="", flush="True")
             invalids = np.argwhere(np.isnan(image.data) | np.isinf(image.data))  # search for bad pixels
             for px, py, band in invalids:
                 n = 0
                 sum = 0
                 for xx in range(px - 1, px + 2):
@@ -120,18 +120,24 @@
                         sum += image.data[xx][yy][band]
                 if n > 0: sum /= n  # do averaging
                 image.data[px][py][band] = sum
             if verbose: print("DONE.")
 
         # Denoise LWIR along sensor plane
         image.data = median_filter(image.data, size=(3, 1, 3), mode="mirror")
+        white = median_filter(white, size=(3,1,3), mode='mirror') # also apply to white panel for noise estimation
+
+        # also estimate noise per-band (useful for eg., MNFs)
+        noise = np.nanstd(white, axis=(0, 1))
+        image.header['band noise'] = noise
 
         # rotate image so that scanning direction is horizontal rather than vertical)
         image.data = np.rot90(image.data)  # np.transpose(remap, (1, 0, 2))
         image.data = np.flip(image.data, axis=1)
+        image.set_band_names(None)  # delete band names as they get super annoying
 
     @classmethod
     def correct_folder(cls, path, **kwds):
 
         """
         Many sensors use simple/common data structures to store data/headers/dark reference etc. Hence it is often easiest
         to pass an output folder to the sensor for correction.
```

### Comparing `hylite-1.21/hylite/sensors/rikola.py` & `hylite-1.23/hylite/sensors/rikola.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,21 +419,21 @@
         for file in filelist:
 
             # read 3 bands (RGB) as PIL image
             raster = gdal.Open(file)
             band1 = raster.GetRasterBand(23).ReadAsArray()
             band2 = raster.GetRasterBand(7).ReadAsArray()
             band3 = raster.GetRasterBand(1).ReadAsArray()
-            arr1 = band1.astype(np.float)
+            arr1 = band1.astype(np.float32)
             maxim = np.nanmax(band1)
             band1_255 = np.uint8(arr1 / maxim * 255)
-            arr1 = band2.astype(np.float)
+            arr1 = band2.astype(np.float32)
             maxim = np.nanmax(arr1)
             band2_255 = np.uint8(arr1 / maxim * 255)
-            arr1 = band3.astype(np.float)
+            arr1 = band3.astype(np.float32)
             maxim = np.nanmax(arr1)
             band3_255 = np.uint8(arr1 / maxim * 255)
 
             # find and extract file-relevant info from taskfile
             rawfilename = os.path.split(file)[1].replace('_CORRECTED.dat', '.DAT')[6:]
             filenumber = np.where(taskfile[:, 0] == rawfilename)
             test = taskfile[filenumber, 16].tolist()
@@ -462,15 +462,15 @@
                              3: WE,  # Longituteref
                              4: ((int(long), 1), (int(100 * (long - int(long))), 1),
                                  (int((100 * (long - int(long)) - int(100 * (long - int(long)))) * 6000), 100)),
                              # longitude
                              6: (abs(int(altitude * 100)), 100),  # Altitude
                              7: (
                              (int((time.split(' ')[2]).split(':')[0]), 1), (int((time.split(' ')[2]).split(':')[1]), 1),
-                             (int((np.float((time.split(' ')[2]).split(':')[2])) * 100), 10)),
+                             (int((float((time.split(' ')[2]).split(':')[2])) * 100), 10)),
                              29: date},  # timestamp
                          'Interop': {},
                          'thumbnail': None}
             exif_bytes = piexif.dump(exif_dict)
             plt.imsave(out,np.dstack((band1_255, band2_255, band3_255)))
             piexif.insert(exif_bytes, out)
```

### Comparing `hylite-1.21/hylite/sensors/sensor.py` & `hylite-1.23/hylite/sensors/sensor.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/hylite.egg-info/PKG-INFO` & `hylite-1.23/hylite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hylite
-Version: 1.21
+Version: 1.23
 Summary: Open-source toolbox for hyperspectral geology.
 Home-page: https://github.com/samthiele/hylite
 Author: Helmholtz Institute Freiberg
 Author-email: s.thiele@hzdr.de
 Project-URL: Source, https://github.com/samthiele/hylite
 Project-URL: Documentation, https://hifexplo.github.io/hylite/hylite.html
 Keywords: hyperspectral data analysis hypercloud geology mineral mapping
```

### Comparing `hylite-1.21/hylite.egg-info/SOURCES.txt` & `hylite-1.23/hylite.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 hylite/project/__init__.py
 hylite/project/align.py
 hylite/project/basic.py
 hylite/project/camera.py
 hylite/project/pmap.py
 hylite/project/pushbroom.py
 hylite/reference/__init__.py
+hylite/reference/generate.py
 hylite/reference/features/__init__.py
 hylite/reference/spectra/__init__.py
 hylite/reference/spectra/custom/__init__.py
 hylite/reference/spectra/pvc/PVC_Black.txt
 hylite/reference/spectra/pvc/PVC_Grey.txt
 hylite/reference/spectra/pvc/PVC_Red.txt
 hylite/reference/spectra/pvc/PVC_White.txt
@@ -86,14 +87,15 @@
 hylite/sensors/calibration_data/fenix1k/Radiometric_8x2_1x1.dat
 hylite/sensors/calibration_data/fenix1k/Radiometric_8x2_1x1.hdr
 hylite/sensors/calibration_data/fenix1k/__init__.py
 tests/__init__.py
 tests/test_align.py
 tests/test_atmospheric.py
 tests/test_filters.py
+tests/test_generate.py
 tests/test_hycloud.py
 tests/test_hycollection.py
 tests/test_hydata.py
 tests/test_hyfeature.py
 tests/test_hyimage.py
 tests/test_hylibrary.py
 tests/test_hyscene.py
```

### Comparing `hylite-1.21/setup.py` & `hylite-1.23/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hylite",
-    version="1.21",
+    version="1.23",
     author="Helmholtz Institute Freiberg",
     author_email="s.thiele@hzdr.de",
     description="Open-source toolbox for hyperspectral geology.",
     long_description="A python package for loading, correcting, projecting and analysing hyperspectral datasets, with particular emphasis on geological applications.",
     long_description_content_type="text/markdown",
     url="https://github.com/samthiele/hylite",
     #package_dir={'': 'hylite'},
@@ -22,16 +22,16 @@
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering"
     ],
     keywords='hyperspectral data analysis hypercloud geology mineral mapping',
     python_requires='>=3.6',
     install_requires=["scipy>=1.4", "matplotlib>=3", "numpy",
                       "imageio","opencv-python>=4.5", "opencv-contrib-python>=4.5",
-                      "scikit-image", "tqdm", "roipoly", "spectral", "utm",
-                      "laspy","plyfile","astral","piexif","gfit","numba"],
+                      "scikit-image", "tqdm", "roipoly", "spectral", "utm","pytz",
+                      "laspy","plyfile","astral","piexif","gfit","numba","natsort"],
 
     # List additional URLs that are relevant to your project as a dict.
     #
     # This field corresponds to the "Project-URL" metadata fields:
     # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
     #
     # Examples listed include a pattern for specifying where the package tracks
```

### Comparing `hylite-1.21/tests/__init__.py` & `hylite-1.23/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/tests/test_align.py` & `hylite-1.23/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/tests/test_atmospheric.py` & `hylite-1.23/tests/test_atmospheric.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/tests/test_filters.py` & `hylite-1.23/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/tests/test_hycloud.py` & `hylite-1.23/tests/test_hycloud.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/tests/test_hydata.py` & `hylite-1.23/tests/test_hydata.py`

 * *Files 18% similar despite different names*

```diff
@@ -139,9 +139,23 @@
             # test fill holes
             data.data = np.nan_to_num(data.data, posinf=0, neginf=0) # remove any stray nans
             self.assertTrue(np.isfinite(data.data).all())
             data.data[...,5] = np.nan # add some nans
             data.fill_gaps() # remove them again!
             self.assertTrue(np.isfinite(data.data).all() ) # check they were removed
 
+            # test reshaping to feature vectors
+            data.data[..., 5] = np.nan  # add some nans
+            self.assertSequenceEqual( data.X().shape, np.reshape(data.data, (-1, data.band_count())).shape ) # check shape is unchanged
+            self.assertNotEquals(data.X(True).shape[0], np.reshape(data.data, (-1, data.band_count())).shape[0] ) # check nans are removed
+            self.assertTrue( np.isfinite( data.X(True).all()) )
+
+            data.set_raveled( np.zeros_like( data.X(True)), onlyFinite=True ) # set with nan-mask
+            self.assertFalse( np.isfinite(data.data ).all() ) # check nans persist
+
+            data.set_raveled(np.zeros_like(data.X()), onlyFinite=False)  # set without nan-mask
+            self.assertTrue(np.isfinite(data.data).all())  # check nans are gone
+
+            # N.B. data.data is now all zero!
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `hylite-1.21/tests/test_hyfeature.py` & `hylite-1.23/tests/test_hyfeature.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/tests/test_hyimage.py` & `hylite-1.23/tests/test_hyimage.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/tests/test_hylibrary.py` & `hylite-1.23/tests/test_hylibrary.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,19 +37,20 @@
         # test building library and plotting functions
         from hylite.hylibrary import from_classification
         for sample in [50, (50,),'all', (5,50,95)]:
             lib = from_classification( image, cls, ignore=[0], subsample=sample )
             lib.quick_plot(color=['r','g','b'], clip=(0,50,100))
             lib.quick_plot(color=['r', 'g', 'b'], clip=50)
 
-        # test copy
+        # test copy functions (well... run them)
         lib2 = lib.copy(data=False)
         lib2 = lib.copy(data=True)
 
-        # test access
+        # test merging / splitting
+        lib.set_sample_names(['A','B','C'])
         lib2 = lib[['A','A','B']] # check merging of names
         self.assertEqual( lib2.data.shape[0], 2 )
         self.assertEqual(lib2.data.shape[1], 6)
         lib2 = lib[[1, 'A', 'B']] # check indices and names merge seamlessly
         self.assertEqual(lib2.data.shape[0], 2)
         self.assertEqual(lib2.data.shape[1], 6)
```

### Comparing `hylite-1.21/tests/test_hyscene.py` & `hylite-1.23/tests/test_hyscene.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/tests/test_io.py` & `hylite-1.23/tests/test_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,26 @@
                         # save with SPy
                         io.saveWithSPy(os.path.join(pth, "data2.hdr"), data )
                         self.assertEqual(os.path.exists(os.path.join(pth, "data2.hdr")), True)
                         data2 = io.load(os.path.join(pth, "data2.hdr")) # reload it
                         self.assertAlmostEquals(np.nanmax(np.abs(data.data - data2.data)), 0,
                                                 6)  # check values are the same
 
+                # test saving 3-band images to png files
+                rgb = self.img.export_bands(hylite.RGB) # get 3-band image
+                rgb.percent_clip(1,99,per_band=True,clip=True) # scale to range 0 - 1
+                rgb.data = (rgb.data * 255).astype(np.uint8) # convert to uint8
+                io.save(os.path.join(pth, "rgb.hdr"), rgb )
+                print(os.listdir(pth))
+                self.assertTrue(os.path.exists(os.path.join(pth,'rgb.png')))
+
+                # test loading png image from header file
+                img = io.load(os.path.join(pth,'rgb.hdr'))
+                self.assertTrue( img is not None)
+
                 # test saving camera objects
                 cam = Camera( np.ones(3), np.ones(3), 'pano', 32.2, (100,100), step=0.1 ) # build test camera
                 track = Pushbroom( np.ones((1000,3)), np.ones((1000,3)), 0.05, 30.04, (100,1000)) # test pushbroom camera
 
                 # test saving camera
                 data = cam
                 io.save(os.path.join(pth, "camera"), data )
```

### Comparing `hylite-1.21/tests/test_mwl.py` & `hylite-1.23/tests/test_mwl.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,37 +102,39 @@
                                    ftol=0.1, minima=False)
             M.sortByDepth()
             self.assertGreater(np.nanmax(M[0,'depth']), 0 ) # check there are some valid features
 
     def testIO(self):
         image = io.load(os.path.join(os.path.join(str(Path(__file__).parent.parent), "test_data"),"image.hdr"))
         M = minimum_wavelength(image, minw=2100., maxw=2400., sym=False, method='gauss', n=2, vb=True)
-
         pth = mkdtemp()
 
         # do save and load
         eq0,eq1 = False,False
         df = np.inf
         try:
             io.save(pth+'/test', M)
+            print("MWL: ", os.path.exists('/Users/thiele67/Documents/Python/public/hylite/tests/M.mwl'))
             eq0 = os.path.exists(os.path.join(pth,'test.mwl')) # save worked?
             M2 = io.load(os.path.join(pth,'test.hdr'))
 
             # check identical
             eq1 = (M2.x == M.x).all()
             df = np.nanmax( M.model.data - M2.model.data ) # max difference
 
         except:
             shutil.rmtree(pth)  # delete temp directory
             self.assertFalse(True, "Error..." )
+
         shutil.rmtree(pth)  # delete temp directory
 
         self.assertTrue(eq0) # fail here if something went wrong
         self.assertTrue(eq1)
         self.assertTrue(df < 1e-2) # difference should be very small
+
     def test_TPT(self):
         from hylite.filter import TPT
         image = io.load(os.path.join(os.path.join(str(Path(__file__).parent.parent), "test_data"),"image.hdr"))
         tpt,p,d = TPT(image, sigma=10., window=7, thresh=0, vb=False)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `hylite-1.21/tests/test_pmap.py` & `hylite-1.23/tests/test_pmap.py`

 * *Files identical despite different names*

### Comparing `hylite-1.21/tests/test_sensors.py` & `hylite-1.23/tests/test_sensors.py`

 * *Files identical despite different names*

