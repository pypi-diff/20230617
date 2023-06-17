# Comparing `tmp/litebird_sim-0.8.0.tar.gz` & `tmp/litebird_sim-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litebird_sim-0.8.0.tar", max compression
+gzip compressed data, was "litebird_sim-0.9.0.tar", max compression
```

## Comparing `litebird_sim-0.8.0.tar` & `litebird_sim-0.9.0.tar`

### file list

```diff
@@ -1,59 +1,64 @@
--rw-r--r--   0        0        0    35149 2020-06-13 06:21:02.049495 litebird_sim-0.8.0/LICENSE
--rw-r--r--   0        0        0     5194 2021-03-18 16:37:16.377270 litebird_sim-0.8.0/README.md
--rw-r--r--   0        0        0    23889 2021-03-18 16:37:16.393270 litebird_sim-0.8.0/images/logo.png
--rw-r--r--   0        0        0     5095 2022-10-10 13:50:55.832629 litebird_sim-0.8.0/litebird_sim/__init__.py
--rw-r--r--   0        0        0     1142 2022-02-17 13:21:24.317119 litebird_sim-0.8.0/litebird_sim/compress.py
--rw-r--r--   0        0        0     3895 2022-09-20 07:27:39.595224 litebird_sim-0.8.0/litebird_sim/coordinates.py
--rw-r--r--   0        0        0   135360 2021-03-18 16:37:16.393270 litebird_sim-0.8.0/litebird_sim/datautils/Cls_Planck2018_for_PTEP_2020_r0.fits
--rw-r--r--   0        0        0   135360 2021-03-18 16:37:16.397270 litebird_sim-0.8.0/litebird_sim/datautils/Cls_Planck2018_for_PTEP_2020_tensor_r1.fits
--rw-r--r--   0        0        0    11784 2022-09-20 07:27:39.595224 litebird_sim-0.8.0/litebird_sim/destriper/__init__.py
--rw-r--r--   0        0        0    13569 2022-10-10 13:50:52.109321 litebird_sim-0.8.0/litebird_sim/detectors.py
--rw-r--r--   0        0        0    10268 2022-09-20 07:27:39.595224 litebird_sim-0.8.0/litebird_sim/dipole.py
--rw-r--r--   0        0        0     7572 2022-02-17 13:21:24.317119 litebird_sim-0.8.0/litebird_sim/distribute.py
--rw-r--r--   0        0        0    11533 2021-10-15 13:21:49.580539 litebird_sim-0.8.0/litebird_sim/healpix.py
--rw-r--r--   0        0        0     3072 2022-09-20 07:27:39.598557 litebird_sim-0.8.0/litebird_sim/hwp.py
--rw-r--r--   0        0        0       26 2021-11-08 17:18:54.303976 litebird_sim-0.8.0/litebird_sim/hwp_sys/__init__.py
--rw-r--r--   0        0        0   260976 2022-09-20 07:27:39.601891 litebird_sim-0.8.0/litebird_sim/hwp_sys/examples/simple_scan.ipynb
--rw-r--r--   0        0        0    19712 2022-09-20 07:27:39.601891 litebird_sim-0.8.0/litebird_sim/hwp_sys/hwp_sys.py
--rw-r--r--   0        0        0      305 2020-07-31 10:13:35.050263 litebird_sim-0.8.0/litebird_sim/imo/__init__.py
--rw-r--r--   0        0        0    12577 2022-09-20 07:27:39.601891 litebird_sim-0.8.0/litebird_sim/imo/flatfile.py
--rw-r--r--   0        0        0     6001 2021-09-24 08:36:33.117012 litebird_sim-0.8.0/litebird_sim/imo/imo.py
--rw-r--r--   0        0        0     7950 2020-12-02 18:14:00.941717 litebird_sim-0.8.0/litebird_sim/imo/objects.py
--rw-r--r--   0        0        0    10341 2021-10-15 13:21:49.580539 litebird_sim-0.8.0/litebird_sim/imobrowser.py
--rw-r--r--   0        0        0     6561 2020-12-02 18:14:00.941717 litebird_sim-0.8.0/litebird_sim/install_imo.py
--rw-r--r--   0        0        0    23444 2022-02-17 13:21:24.317119 litebird_sim-0.8.0/litebird_sim/io.py
--rw-r--r--   0        0        0     8372 2022-09-20 07:27:39.601891 litebird_sim-0.8.0/litebird_sim/madam.py
--rw-r--r--   0        0        0     9841 2022-09-20 07:27:39.601891 litebird_sim-0.8.0/litebird_sim/mapping.py
--rw-r--r--   0        0        0       94 2021-09-24 08:36:33.120345 litebird_sim-0.8.0/litebird_sim/mbs/__init__.py
--rw-r--r--   0        0        0      520 2021-03-18 16:37:16.397270 litebird_sim-0.8.0/litebird_sim/mbs/fg_models/pysm_ame_1.cfg
--rw-r--r--   0        0        0      405 2021-03-18 16:37:16.401270 litebird_sim-0.8.0/litebird_sim/mbs/fg_models/pysm_dust_0.cfg
--rw-r--r--   0        0        0      446 2021-03-18 16:37:16.401270 litebird_sim-0.8.0/litebird_sim/mbs/fg_models/pysm_dust_1.cfg
--rw-r--r--   0        0        0      950 2021-03-18 16:37:16.401270 litebird_sim-0.8.0/litebird_sim/mbs/fg_models/pysm_dust_4.cfg
--rw-r--r--   0        0        0      612 2021-03-18 16:37:16.401270 litebird_sim-0.8.0/litebird_sim/mbs/fg_models/pysm_dust_5.cfg
--rw-r--r--   0        0        0      624 2021-03-18 16:37:16.401270 litebird_sim-0.8.0/litebird_sim/mbs/fg_models/pysm_dust_7.cfg
--rw-r--r--   0        0        0      630 2021-03-18 16:37:16.401270 litebird_sim-0.8.0/litebird_sim/mbs/fg_models/pysm_dust_8.cfg
--rw-r--r--   0        0        0      200 2021-03-18 16:37:16.401270 litebird_sim-0.8.0/litebird_sim/mbs/fg_models/pysm_freefree_1.cfg
--rw-r--r--   0        0        0      325 2021-03-18 16:37:16.401270 litebird_sim-0.8.0/litebird_sim/mbs/fg_models/pysm_synch_0.cfg
--rw-r--r--   0        0        0      348 2021-03-18 16:37:16.401270 litebird_sim-0.8.0/litebird_sim/mbs/fg_models/pysm_synch_1.cfg
--rw-r--r--   0        0        0    31705 2022-09-20 07:27:39.601891 litebird_sim-0.8.0/litebird_sim/mbs/mbs.py
--rw-r--r--   0        0        0     1830 2020-08-12 07:25:02.669845 litebird_sim-0.8.0/litebird_sim/mpi.py
--rw-r--r--   0        0        0     6799 2022-09-20 07:27:39.601891 litebird_sim-0.8.0/litebird_sim/noise.py
--rw-r--r--   0        0        0    24821 2022-09-20 07:27:39.605224 litebird_sim-0.8.0/litebird_sim/observations.py
--rw-r--r--   0        0        0     6911 2022-10-10 13:50:55.832629 litebird_sim-0.8.0/litebird_sim/pointings.py
--rw-r--r--   0        0        0    10728 2022-08-29 18:25:48.544384 litebird_sim-0.8.0/litebird_sim/quaternions.py
--rw-r--r--   0        0        0     5573 2022-09-20 07:27:39.605224 litebird_sim-0.8.0/litebird_sim/scan_map.py
--rw-r--r--   0        0        0    34886 2022-09-20 07:27:39.605224 litebird_sim-0.8.0/litebird_sim/scanning.py
--rw-r--r--   0        0        0    30479 2022-09-20 07:27:39.605224 litebird_sim-0.8.0/litebird_sim/simulations.py
--rw-r--r--   0        0        0    16500 2022-09-20 07:27:39.605224 litebird_sim-0.8.0/litebird_sim/spacecraft.py
--rw-r--r--   0        0        0       93 2022-10-10 14:18:55.281200 litebird_sim-0.8.0/litebird_sim/version.py
--rw-r--r--   0        0        0      647 2020-10-28 13:38:21.952197 litebird_sim-0.8.0/misc/pandoc-filter.lua
--rw-r--r--   0        0        0     1937 2022-10-10 14:19:19.904928 litebird_sim-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1396 2020-06-13 06:21:02.059495 litebird_sim-0.8.0/static/report_template.html
--rw-r--r--   0        0        0     3353 2020-06-13 06:21:02.059495 litebird_sim-0.8.0/static/sakura.css
--rw-r--r--   0        0        0      925 2022-09-20 07:27:39.631891 litebird_sim-0.8.0/templates/madam_parameter_file.txt
--rw-r--r--   0        0        0      709 2022-09-20 07:27:39.631891 litebird_sim-0.8.0/templates/madam_simulation_file.txt
--rw-r--r--   0        0        0     1786 2021-03-18 16:37:16.405270 litebird_sim-0.8.0/templates/report_appendix.md
--rw-r--r--   0        0        0      183 2020-09-16 07:37:16.917508 litebird_sim-0.8.0/templates/report_generate_pointings.md
--rw-r--r--   0        0        0      155 2020-09-16 07:37:16.917508 litebird_sim-0.8.0/templates/report_header.md
--rw-r--r--   0        0        0     7141 2022-10-10 14:21:18.874107 litebird_sim-0.8.0/setup.py
--rw-r--r--   0        0        0     7081 2022-10-10 14:21:18.874579 litebird_sim-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2020-06-13 06:21:02.049495 litebird_sim-0.9.0/LICENSE
+-rw-r--r--   0        0        0     5327 2023-02-28 10:54:21.105615 litebird_sim-0.9.0/README.md
+-rw-r--r--   0        0        0    23889 2021-03-18 16:37:16.393270 litebird_sim-0.9.0/images/logo.png
+-rw-r--r--   0        0        0     5331 2023-02-16 11:32:44.272208 litebird_sim-0.9.0/litebird_sim/__init__.py
+-rw-r--r--   0        0        0    11394 2022-11-01 05:29:59.788830 litebird_sim-0.9.0/litebird_sim/bandpasses.py
+-rw-r--r--   0        0        0     1142 2022-02-17 13:21:24.317119 litebird_sim-0.9.0/litebird_sim/compress.py
+-rw-r--r--   0        0        0     8486 2023-02-28 10:54:25.572281 litebird_sim-0.9.0/litebird_sim/coordinates.py
+-rw-r--r--   0        0        0   135360 2021-03-18 16:37:16.393270 litebird_sim-0.9.0/litebird_sim/datautils/Cls_Planck2018_for_PTEP_2020_r0.fits
+-rw-r--r--   0        0        0   135360 2021-03-18 16:37:16.397270 litebird_sim-0.9.0/litebird_sim/datautils/Cls_Planck2018_for_PTEP_2020_tensor_r1.fits
+-rw-r--r--   0        0        0    11784 2022-09-20 07:27:39.595224 litebird_sim-0.9.0/litebird_sim/destriper/__init__.py
+-rw-r--r--   0        0        0    14579 2022-12-20 09:51:55.463903 litebird_sim-0.9.0/litebird_sim/detectors.py
+-rw-r--r--   0        0        0    10800 2022-11-17 17:45:02.496730 litebird_sim-0.9.0/litebird_sim/dipole.py
+-rw-r--r--   0        0        0     7572 2022-02-17 13:21:24.317119 litebird_sim-0.9.0/litebird_sim/distribute.py
+-rw-r--r--   0        0        0    11533 2021-10-15 13:21:49.580539 litebird_sim-0.9.0/litebird_sim/healpix.py
+-rw-r--r--   0        0        0     3404 2023-01-09 09:23:03.614503 litebird_sim-0.9.0/litebird_sim/hwp.py
+-rw-r--r--   0        0        0       26 2021-11-08 17:18:54.303976 litebird_sim-0.9.0/litebird_sim/hwp_sys/__init__.py
+-rw-r--r--   0        0        0   260944 2023-01-09 09:23:03.617836 litebird_sim-0.9.0/litebird_sim/hwp_sys/examples/simple_scan.ipynb
+-rw-r--r--   0        0        0    19712 2022-09-20 07:27:39.601891 litebird_sim-0.9.0/litebird_sim/hwp_sys/hwp_sys.py
+-rw-r--r--   0        0        0      305 2020-07-31 10:13:35.050263 litebird_sim-0.9.0/litebird_sim/imo/__init__.py
+-rw-r--r--   0        0        0    12577 2022-09-20 07:27:39.601891 litebird_sim-0.9.0/litebird_sim/imo/flatfile.py
+-rw-r--r--   0        0        0     6001 2021-09-24 08:36:33.117012 litebird_sim-0.9.0/litebird_sim/imo/imo.py
+-rw-r--r--   0        0        0     7950 2020-12-02 18:14:00.941717 litebird_sim-0.9.0/litebird_sim/imo/objects.py
+-rw-r--r--   0        0        0    10341 2021-10-15 13:21:49.580539 litebird_sim-0.9.0/litebird_sim/imobrowser.py
+-rw-r--r--   0        0        0     6561 2020-12-02 18:14:00.941717 litebird_sim-0.9.0/litebird_sim/install_imo.py
+-rw-r--r--   0        0        0    24170 2023-01-12 10:28:32.032009 litebird_sim-0.9.0/litebird_sim/io.py
+-rw-r--r--   0        0        0    18262 2023-02-16 11:32:44.272208 litebird_sim-0.9.0/litebird_sim/madam.py
+-rw-r--r--   0        0        0    10621 2022-11-24 12:18:18.784410 litebird_sim-0.9.0/litebird_sim/mapping.py
+-rw-r--r--   0        0        0       94 2021-09-24 08:36:33.120345 litebird_sim-0.9.0/litebird_sim/mbs/__init__.py
+-rw-r--r--   0        0        0      520 2021-03-18 16:37:16.397270 litebird_sim-0.9.0/litebird_sim/mbs/fg_models/pysm_ame_1.cfg
+-rw-r--r--   0        0        0      405 2021-03-18 16:37:16.401270 litebird_sim-0.9.0/litebird_sim/mbs/fg_models/pysm_dust_0.cfg
+-rw-r--r--   0        0        0      446 2021-03-18 16:37:16.401270 litebird_sim-0.9.0/litebird_sim/mbs/fg_models/pysm_dust_1.cfg
+-rw-r--r--   0        0        0      950 2021-03-18 16:37:16.401270 litebird_sim-0.9.0/litebird_sim/mbs/fg_models/pysm_dust_4.cfg
+-rw-r--r--   0        0        0      612 2021-03-18 16:37:16.401270 litebird_sim-0.9.0/litebird_sim/mbs/fg_models/pysm_dust_5.cfg
+-rw-r--r--   0        0        0      624 2021-03-18 16:37:16.401270 litebird_sim-0.9.0/litebird_sim/mbs/fg_models/pysm_dust_7.cfg
+-rw-r--r--   0        0        0      630 2021-03-18 16:37:16.401270 litebird_sim-0.9.0/litebird_sim/mbs/fg_models/pysm_dust_8.cfg
+-rw-r--r--   0        0        0      200 2021-03-18 16:37:16.401270 litebird_sim-0.9.0/litebird_sim/mbs/fg_models/pysm_freefree_1.cfg
+-rw-r--r--   0        0        0      325 2021-03-18 16:37:16.401270 litebird_sim-0.9.0/litebird_sim/mbs/fg_models/pysm_synch_0.cfg
+-rw-r--r--   0        0        0      348 2021-03-18 16:37:16.401270 litebird_sim-0.9.0/litebird_sim/mbs/fg_models/pysm_synch_1.cfg
+-rw-r--r--   0        0        0    31987 2023-02-28 10:54:21.112281 litebird_sim-0.9.0/litebird_sim/mbs/mbs.py
+-rw-r--r--   0        0        0     1830 2020-08-12 07:25:02.669845 litebird_sim-0.9.0/litebird_sim/mpi.py
+-rw-r--r--   0        0        0     7393 2023-02-28 10:54:25.572281 litebird_sim-0.9.0/litebird_sim/noise.py
+-rw-r--r--   0        0        0    24821 2023-02-16 11:32:44.272208 litebird_sim-0.9.0/litebird_sim/observations.py
+-rw-r--r--   0        0        0     7100 2023-02-24 16:39:50.992554 litebird_sim-0.9.0/litebird_sim/pointings.py
+-rw-r--r--   0        0        0    10728 2022-08-29 18:25:48.544384 litebird_sim-0.9.0/litebird_sim/quaternions.py
+-rw-r--r--   0        0        0     6622 2023-02-28 10:54:21.112281 litebird_sim-0.9.0/litebird_sim/scan_map.py
+-rw-r--r--   0        0        0    34886 2022-12-28 11:43:55.723816 litebird_sim-0.9.0/litebird_sim/scanning.py
+-rw-r--r--   0        0        0    48181 2023-02-28 10:54:21.112281 litebird_sim-0.9.0/litebird_sim/simulations.py
+-rw-r--r--   0        0        0    16500 2022-09-20 07:27:39.605224 litebird_sim-0.9.0/litebird_sim/spacecraft.py
+-rw-r--r--   0        0        0       93 2023-02-28 11:20:46.118853 litebird_sim-0.9.0/litebird_sim/version.py
+-rw-r--r--   0        0        0      647 2020-10-28 13:38:21.952197 litebird_sim-0.9.0/misc/pandoc-filter.lua
+-rw-r--r--   0        0        0     2092 2023-02-28 11:20:10.635522 litebird_sim-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1396 2020-06-13 06:21:02.059495 litebird_sim-0.9.0/static/report_template.html
+-rw-r--r--   0        0        0     3353 2020-06-13 06:21:02.059495 litebird_sim-0.9.0/static/sakura.css
+-rw-r--r--   0        0        0     1127 2022-11-17 17:45:02.503396 litebird_sim-0.9.0/templates/madam_parameter_file.txt
+-rw-r--r--   0        0        0      893 2022-11-17 17:45:02.503396 litebird_sim-0.9.0/templates/madam_simulation_file.txt
+-rw-r--r--   0        0        0     2110 2022-11-28 16:47:45.977947 litebird_sim-0.9.0/templates/report_appendix.md
+-rw-r--r--   0        0        0      268 2023-02-28 10:54:21.135614 litebird_sim-0.9.0/templates/report_dipole.md
+-rw-r--r--   0        0        0      155 2020-09-16 07:37:16.917508 litebird_sim-0.9.0/templates/report_header.md
+-rw-r--r--   0        0        0       84 2023-02-28 10:54:21.135614 litebird_sim-0.9.0/templates/report_noise.md
+-rw-r--r--   0        0        0      291 2023-01-09 09:23:03.654503 litebird_sim-0.9.0/templates/report_pointings.md
+-rw-r--r--   0        0        0      200 2023-01-09 09:23:03.654503 litebird_sim-0.9.0/templates/report_quaternions.md
+-rw-r--r--   0        0        0      200 2023-02-28 10:54:21.135614 litebird_sim-0.9.0/templates/report_scan_map.md
+-rw-r--r--   0        0        0     7314 1970-01-01 00:00:00.000000 litebird_sim-0.9.0/setup.py
+-rw-r--r--   0        0        0     7260 1970-01-01 00:00:00.000000 litebird_sim-0.9.0/PKG-INFO
```

### Comparing `litebird_sim-0.8.0/LICENSE` & `litebird_sim-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/README.md` & `litebird_sim-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -91,14 +91,16 @@
 to learn how to install the LiteBIRD simulation framework on your
 computer or on a HPC cluster.
 
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
+An example notebook is avalable [here](https://github.com/litebird/litebird_sim/blob/master/notebooks/litebird_sim_example.ipynb). 
+
 The documentation is available online at
 [litebird-sim.readthedocs.io/en/master/](https://litebird-sim.readthedocs.io/en/master/).
 
 To create a local copy of the documentation, make sure you ran
 `poetry` with the flag `--extras=docs`, then run the following
 command:
```

#### html2text {}

```diff
@@ -23,24 +23,26 @@
 (https://www.python.org) - [Poetry](https://python-poetry.org/) - [NumPy]
 (https://numpy.org) - [Astropy](https://www.astropy.org) - [Healpix](https://
 healpix.jpl.nasa.gov) - [Sphinx](https://www.sphinx-doc.org/en/master/) -
 [Numba](https://numba.pydata.org/) - [ducc](https://github.com/litebird/ducc)
 ## Getting Started Refer to the [documentation](https://litebird-
 sim.readthedocs.io/en/master/installation.html) to learn how to install the
 LiteBIRD simulation framework on your computer or on a HPC cluster.  ## Usage
-The documentation is available online at [litebird-sim.readthedocs.io/en/
-master/](https://litebird-sim.readthedocs.io/en/master/). To create a local
-copy of the documentation, make sure you ran `poetry` with the flag `--
-extras=docs`, then run the following command: - Linux or Mac OS X: ``` ./
-refresh_docs.sh ``` - Windows: ``` poetry shell cd docs make.bat html ```  ##
-Roadmap See the [open issues](https://github.com/litebird/litebird_sim/issues)
-for a list of proposed features (and known issues).  ## Contributing If you are
-part of the LiteBIRD collaboration and have something that might fit in this
-framework, you're encouraged to contact us! Any contributions you make are
-**greatly appreciated**. 1. Read [CONTRIBUTING.md](https://github.com/litebird/
+An example notebook is avalable [here](https://github.com/litebird/
+litebird_sim/blob/master/notebooks/litebird_sim_example.ipynb). The
+documentation is available online at [litebird-sim.readthedocs.io/en/master/]
+(https://litebird-sim.readthedocs.io/en/master/). To create a local copy of the
+documentation, make sure you ran `poetry` with the flag `--extras=docs`, then
+run the following command: - Linux or Mac OS X: ``` ./refresh_docs.sh ``` -
+Windows: ``` poetry shell cd docs make.bat html ```  ## Roadmap See the [open
+issues](https://github.com/litebird/litebird_sim/issues) for a list of proposed
+features (and known issues).  ## Contributing If you are part of the LiteBIRD
+collaboration and have something that might fit in this framework, you're
+encouraged to contact us! Any contributions you make are **greatly
+appreciated**. 1. Read [CONTRIBUTING.md](https://github.com/litebird/
 litebird_sim/blob/master/CONTRIBUTING.md) 2. Fork the project 3. Create your
 feature branch (`git checkout -b feature/AmazingFeature`) 4. Commit your
 changes (`git commit -m 'Add some AmazingFeature'`) 5. Push to the Branch (`git
 push origin feature/AmazingFeature`) 6. Open a Pull Request  ## License
 Distributed under the [GPL3 License][license-url].  ## Contact LiteBIRD
 Simulation Team - litebird_pipe@db.ipmu.jp Project Link: [https://github.com/
 litebird/litebird_sim](https://github.com/litebird/litebird_sim)  ## How to
```

### Comparing `litebird_sim-0.8.0/images/logo.png` & `litebird_sim-0.9.0/images/logo.png`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/litebird_sim/__init__.py` & `litebird_sim-0.9.0/litebird_sim/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .distribute import distribute_evenly, distribute_optimally
 from .detectors import (
     DetectorInfo,
     FreqChannelInfo,
     InstrumentInfo,
     detector_list_from_parameters,
 )
+from .bandpasses import BandPassInfo
 from .healpix import (
     nside_to_npix,
     npix_to_nside,
     is_npix_ok,
     map_type,
     get_pixel_format,
     write_healpix_map_to_hdu,
@@ -69,15 +70,20 @@
     ScanningStrategy,
     SpinningScanningStrategy,
     get_det2ecl_quaternions,
     get_ecl2det_quaternions,
 )
 from .mapping import DestriperParameters, DestriperResult, make_bin_map
 from .destriper import destripe
-from .simulations import Simulation
+from .simulations import (
+    Simulation,
+    MpiObservationDescr,
+    MpiProcessDescr,
+    MpiDistributionDescr,
+)
 from .noise import (
     add_white_noise,
     add_one_over_f_noise,
     add_noise,
     add_noise_to_observations,
 )
 from .scan_map import scan_map, scan_map_in_observations
@@ -106,14 +112,16 @@
 
 __all__ = [
     "__author__",
     "__version__",
     # compress.py
     "rle_compress",
     "rle_decompress",
+    # bandpasses.py
+    "BandPassInfo",
     # healpix.py
     "nside_to_npix",
     "npix_to_nside",
     "is_npix_ok",
     "map_type",
     "get_pixel_format",
     "write_healpix_map_to_hdu",
@@ -184,14 +192,17 @@
     "make_bin_map",
     # destripe.py
     "DestriperParameters",
     "DestriperResult",
     "destripe",
     # simulations.py
     "Simulation",
+    "MpiObservationDescr",
+    "MpiProcessDescr",
+    "MpiDistributionDescr",
     # noise.py
     "add_white_noise",
     "add_one_over_f_noise",
     "add_noise",
     "add_noise_to_observations",
     # scan_map.py
     "scan_map",
```

### Comparing `litebird_sim-0.8.0/litebird_sim/compress.py` & `litebird_sim-0.9.0/litebird_sim/compress.py`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/litebird_sim/datautils/Cls_Planck2018_for_PTEP_2020_r0.fits` & `litebird_sim-0.9.0/litebird_sim/datautils/Cls_Planck2018_for_PTEP_2020_r0.fits`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/litebird_sim/datautils/Cls_Planck2018_for_PTEP_2020_tensor_r1.fits` & `litebird_sim-0.9.0/litebird_sim/datautils/Cls_Planck2018_for_PTEP_2020_tensor_r1.fits`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/litebird_sim/destriper/__init__.py` & `litebird_sim-0.9.0/litebird_sim/destriper/__init__.py`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/litebird_sim/detectors.py` & `litebird_sim-0.9.0/litebird_sim/detectors.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 from uuid import UUID
 import numpy as np
 
 from .imo import Imo
 from .quaternions import quat_rotation_y, quat_rotation_z, quat_left_multiply
 
+from .bandpasses import BandPassInfo
+
 
 @dataclass
 class DetectorInfo:
     """A class wrapping the basic information about a detector.
 
     This is a data class that encodes the basic properties of a
     LiteBIRD detector. It can be initialized in three ways:
@@ -44,21 +46,15 @@
         - pixtype (Union[str, None]): The type of the pixel, e.g.,
              ``HP1``, ``LP3``, etc. The default is None
 
         - channel (Union[str, None]): The channel. The default is None
 
         - sampling_rate_hz (float): The sampling rate of the ADC
              associated with this detector. The default is 0.0
-
-        - bandwidth_ghz (float): The bandwidth of the channel, in GHz
-
-        - bandcenter_ghz (float): The central frequency of the
-             channel, in GHz
-
-        - fwhm_arcmin: float): The Full Width Half Maximum of the
+        - fwhm_arcmin: (float): The Full Width Half Maximum of the
              radiation pattern associated with the detector, in
              arcminutes. The default is 0.0
 
         - ellipticity (float): The ellipticity of the radiation
              pattern associated with the detector. The default is 0.0
 
         - net_ukrts (float): The noise equivalent temperature of the
@@ -70,14 +66,19 @@
 
         - bandcenter_ghz (float): The center frequency of the
              detector, in GHz. The default is 0.0
 
         - bandwidth_ghz (float): The bandwidth of the detector, in
              GHz. The default is 0.0
 
+        - band_freqs_ghz (float array): band sampled frequencies, in GHz.
+             The default is None
+
+        - band_weights (float array): band profile. The default is None
+
         - fknee_mhz (float): The knee frequency between the 1/f and
              the white noise components in nominal conditions, in mHz.
              The default is 0.0
 
         - fmin_hz (float): The minimum frequency of the noise when
              producing synthetic noise, in Hz. The default is 0.0
 
@@ -104,14 +105,16 @@
     pixtype: Union[str, None] = None
     channel: Union[str, None] = None
     sampling_rate_hz: float = 0.0
     fwhm_arcmin: float = 0.0
     ellipticity: float = 0.0
     bandcenter_ghz: float = 0.0
     bandwidth_ghz: float = 0.0
+    band_freqs_ghz: Union[None, np.ndarray] = None
+    band_weights: Union[None, np.ndarray] = None
     net_ukrts: float = 0.0
     pol_sensitivity_ukarcmin: float = 0.0
     fknee_mhz: float = 0.0
     fmin_hz: float = 0.0
     alpha: float = 0.0
     bandcenter_ghz: float = 0.0
     bandwidth_ghz: float = 0.0
@@ -124,28 +127,33 @@
 
         # Ensure that the quaternion is a NumPy array
         self.quat = np.array([float(x) for x in self.quat])
 
         # Normalize the quaternion
         self.quat /= np.sqrt(self.quat.dot(self.quat))
 
+        if type(self.band_freqs_ghz) == np.ndarray:
+            assert len(self.band_freqs_ghz) == len(self.band_weights)
+
     @staticmethod
     def from_dict(dictionary: Dict[str, Any]):
         """Create a detector from the contents of a dictionary
 
         The parameter `dictionary` must contain one key for each of
         the fields in this dataclass:
 
         - ``name``
         - ``wafer``
         - ``pixel``
         - ``pixtype``
         - ``channel``
         - ``bandcenter_ghz``
         - ``bandwidth_ghz``
+        - ``band_freqs_ghz``
+        - ``band_weights``
         - ``sampling_rate_hz``
         - ``fwhm_arcmin``
         - ``ellipticity``
         - ``net_ukrts``
         - ``pol_sensitivity_ukarcmin``
         - ``fknee_mhz``
         - ``fmin_hz``
@@ -156,14 +164,21 @@
 
         """
         result = DetectorInfo()
         for param in fields(DetectorInfo):
             if param.name in dictionary:
                 setattr(result, param.name, dictionary[param.name])
 
+        if type(result.band_freqs_ghz) != np.ndarray:
+            result.band = BandPassInfo(result.bandcenter_ghz, result.bandwidth_ghz)
+            result.band_freqs_ghz, result.band_weights = [
+                result.band.freqs_ghz,
+                result.band.weights,
+            ]
+
         # Force initializers to be called again
         result.__post_init__()
         return result
 
     @staticmethod
     def from_imo(imo: Imo, url: Union[UUID, str]):
         """Create a `DetectorInfo` object from a definition in the IMO
@@ -186,14 +201,16 @@
 
 
 @dataclass
 class FreqChannelInfo:
     bandcenter_ghz: float
     channel: Union[str, None] = None
     bandwidth_ghz: float = 0.0
+    band_freqs_ghz: Union[None, np.ndarray] = None
+    band_weights: Union[None, np.ndarray] = None
     net_detector_ukrts: float = 0.0
     net_channel_ukrts: float = 0.0
     pol_sensitivity_channel_ukarcmin: float = 0.0
     sampling_rate_hz: float = 0.0
     fwhm_arcmin: float = 0.0
     fknee_mhz: float = 0.0
     fmin_hz: float = 1e-5
@@ -251,14 +268,21 @@
     @staticmethod
     def from_dict(dictionary: Dict[str, Any]):
         result = FreqChannelInfo(bandcenter_ghz=0.0)
         for param in fields(FreqChannelInfo):
             if param.name in dictionary:
                 setattr(result, param.name, dictionary[param.name])
 
+        if type(result.band_freqs_ghz) != np.ndarray:
+            result.band = BandPassInfo(result.bandcenter_ghz, result.bandwidth_ghz)
+            result.band_freqs_ghz, result.band_weights = [
+                result.band.freqs_ghz,
+                result.band.weights,
+            ]
+
         # Force initializers in __post_init__ to be called
         result.__post_init__()
         return result
 
     @staticmethod
     def from_imo(imo: Imo, url: Union[UUID, str]):
         obj = imo.query(url)
```

### Comparing `litebird_sim-0.8.0/litebird_sim/dipole.py` & `litebird_sim-0.9.0/litebird_sim/dipole.py`

 * *Files 3% similar despite different names*

```diff
@@ -236,20 +236,32 @@
     pos_and_vel: SpacecraftPositionAndVelocity,
     pointings: Union[np.ndarray, List[np.ndarray], None] = None,
     t_cmb_k: float = 2.72548,  # Fixsen 2009 http://arxiv.org/abs/0911.1955
     dipole_type: DipoleType = DipoleType.TOTAL_FROM_LIN_T,
     frequency_ghz: Union[
         np.ndarray, None
     ] = None,  # e.g. central frequency of channel from
+    component: str = "tod",
 ):
     """Add the CMB dipole to some time-ordered data
 
     This is a wrapper around the :func:`.add_dipole` function that applies to the TOD
     stored in `obs`, which can either be one :class:`.Observation` instance or a list
     of observations.
+
+    By default, the TOD is added to ``Observation.tod``. If you want to add it to some
+    other field of the :class:`.Observation` class, use `component`::
+
+        for cur_obs in sim.observations:
+            # Allocate a new TOD for the dipole alone
+            cur_obs.dipole_tod = np.zeros_like(cur_obs.tod)
+
+        # Ask `add_dipole_to_observations` to store the dipole
+        # in `obs.dipole_tod`
+        add_dipole_to_observations(sim.observations, component="dipole_tod")
     """
 
     if pointings is None:
         if isinstance(obs, Observation):
             obs_list = [obs]
             ptg_list = [obs.pointings]
         else:
@@ -272,29 +284,31 @@
                 f"The list of observations has {len(obs)} elements, but "
                 + f"the list of pointings has {len(pointings)} elements"
             )
             obs_list = obs
             ptg_list = [point[:, :, 0:2] for point in pointings]
 
     for cur_obs, cur_ptg in zip(obs_list, ptg_list):
+        tod = getattr(cur_obs, component)
+
         # Alas, this allocates memory for the velocity vector! At the moment it is the
         # simplest implementation, but in the future we might want to inline the
         # interpolation code within "add_dipole" to save memory
         velocity = pos_and_vel.compute_velocities(
             time0=cur_obs.start_time,
             delta_time_s=cur_obs.get_delta_time().value,
-            num_of_samples=cur_obs.tod.shape[1],
+            num_of_samples=tod.shape[1],
         )
 
         if frequency_ghz is None:
             frequency_ghz = cur_obs.bandcenter_ghz
         else:
-            frequency_ghz = np.repeat(frequency_ghz, cur_obs.tod.shape[0])
+            frequency_ghz = np.repeat(frequency_ghz, tod.shape[0])
 
         add_dipole(
-            tod=cur_obs.tod,
+            tod=tod,
             pointings=cur_ptg,
             velocity=velocity,
             t_cmb_k=t_cmb_k,
             frequency_ghz=frequency_ghz,
             dipole_type=dipole_type,
         )
```

### Comparing `litebird_sim-0.8.0/litebird_sim/distribute.py` & `litebird_sim-0.9.0/litebird_sim/distribute.py`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/litebird_sim/healpix.py` & `litebird_sim-0.9.0/litebird_sim/healpix.py`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/litebird_sim/hwp.py` & `litebird_sim-0.9.0/litebird_sim/hwp.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,14 +31,19 @@
         that you should already have converted any AstroPy time to a plain scalar
         before calling this method.
         """
         raise NotImplementedError(
             "You should not use the HWP class in your code, use IdealHWP instead"
         )
 
+    def __str__(self):
+        raise NotImplementedError(
+            "You should not use the HWP class in your code, use IdealHWP instead"
+        )
+
 
 @njit
 def _add_ideal_hwp_angle(
     pointing_buffer, start_time_s, delta_time_s, start_angle_rad, ang_speed_radpsec
 ):
     detectors, samples, _ = pointing_buffer.shape
     for det_idx in range(detectors):
@@ -75,7 +80,13 @@
         _add_ideal_hwp_angle(
             pointing_buffer=pointing_buffer,
             start_time_s=start_time_s,
             delta_time_s=delta_time_s,
             start_angle_rad=self.start_angle_rad,
             ang_speed_radpsec=self.ang_speed_radpsec,
         )
+
+    def __str__(self):
+        return (
+            f"Ideal HWP, with rotating speed {self.ang_speed_radpsec} rad/sec "
+            f"and θ₀ = {self.start_angle_rad}"
+        )
```

### Comparing `litebird_sim-0.8.0/litebird_sim/hwp_sys/examples/simple_scan.ipynb` & `litebird_sim-0.9.0/litebird_sim/hwp_sys/examples/simple_scan.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998629385964912%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(1, "*

 * *            '\'sim.set_scanning_strategy(imo_url="/releases/v1.0/satellite/scanning_parameters/")\\n\')], '*

 * *            'delete: [3, 2, 1]}}}'}*

```diff
@@ -47,17 +47,15 @@
             "cell_type": "code",
             "execution_count": 4,
             "id": "ab20c691",
             "metadata": {},
             "outputs": [],
             "source": [
                 "mft_file = sim.imo.query(\"/releases/v1.0/satellite/\" + instrument + \"/instrument_info\")\n",
-                "sim.generate_spin2ecl_quaternions(\n",
-                "    imo_url=\"/releases/v1.0/satellite/scanning_parameters/\"\n",
-                ")\n",
+                "sim.set_scanning_strategy(imo_url=\"/releases/v1.0/satellite/scanning_parameters/\")\n",
                 "instrumentinfo = lbs.InstrumentInfo(\n",
                 "    name=instrument,\n",
                 "    boresight_rotangle_rad=np.deg2rad(mft_file.metadata[\"boresight_rotangle_deg\"]),\n",
                 "    spin_boresight_angle_rad=np.deg2rad(mft_file.metadata[\"spin_boresight_angle_deg\"]),\n",
                 "    spin_rotangle_rad=np.deg2rad(mft_file.metadata[\"spin_rotangle_deg\"]),\n",
                 ")\n",
                 "channelinfo = lbs.FreqChannelInfo.from_imo(\n",
```

### Comparing `litebird_sim-0.8.0/litebird_sim/hwp_sys/hwp_sys.py` & `litebird_sim-0.9.0/litebird_sim/hwp_sys/hwp_sys.py`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/litebird_sim/imo/flatfile.py` & `litebird_sim-0.9.0/litebird_sim/imo/flatfile.py`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/litebird_sim/imo/imo.py` & `litebird_sim-0.9.0/litebird_sim/imo/imo.py`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/litebird_sim/imo/objects.py` & `litebird_sim-0.9.0/litebird_sim/imo/objects.py`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/litebird_sim/imobrowser.py` & `litebird_sim-0.9.0/litebird_sim/imobrowser.py`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/litebird_sim/install_imo.py` & `litebird_sim-0.9.0/litebird_sim/install_imo.py`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/litebird_sim/io.py` & `litebird_sim-0.9.0/litebird_sim/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     output_file: h5py.File,
     obs: Observation,
     tod_dtype,
     pointings_dtype,
     global_index: int,
     local_index: int,
     tod_fields: List[str] = ["tod"],
+    gzip_compression: bool = False,
 ):
     """Write one :class:`Observation` object in a HDF5 file.
 
     This is a low-level function that stores a TOD in a HDF5 file. You should usually
     use more high-level functions that are able to write several observations at once,
     like :func:`.write_list_of_observations` and :func:`.write_observations`.
 
@@ -61,14 +62,16 @@
     use for writing TODs and pointings is specified in the `tod_dtype` and
     `pointings_dtype` (it can either be a NumPy type like ``numpy.float64`` or a
     string). The `global_index` and `local_index` parameters are two integers that are
     used by high-level functions like :func:`.write_observations` to understand how to
     read several HDF5 files at once; if you do not need them, you can pass 0 to both.
     """
 
+    compression = "gzip" if gzip_compression else None
+
     # This code assumes that the parameter `detectors` passed to Observation
     # was either an integer or a list of `DetectorInfo` objects, i.e., we
     # neglect the possibility that it was a list of dictionaries passing
     # custom keys that have no parallel in DetectorInfo, as it would
     # be too bothersome to understand which keys should be saved here.
 
     det_info = []
@@ -106,15 +109,18 @@
 
     # Now encode `det_info` in a JSON string that will be saved later as an attribute
     detectors_json = json.dumps(det_info)
 
     # Write all the TOD timelines in the HDF5 file, in separate datasets
     for field_name in tod_fields:
         cur_dataset = output_file.create_dataset(
-            field_name, data=obs.__getattribute__(field_name), dtype=tod_dtype
+            field_name,
+            data=obs.__getattribute__(field_name),
+            dtype=tod_dtype,
+            compression=compression,
         )
         if isinstance(obs.start_time, astropy.time.Time):
             cur_dataset.attrs["start_time"] = obs.start_time.to_value(
                 format="mjd", subfmt="bytes"
             )
             cur_dataset.attrs["mjd_time"] = True
         else:
@@ -123,47 +129,59 @@
 
         cur_dataset.attrs["sampling_rate_hz"] = obs.sampling_rate_hz
         cur_dataset.attrs["detectors"] = detectors_json
 
     # Save pointing information only if it is available
     try:
         output_file.create_dataset(
-            "pointings", data=obs.__getattribute__("pointings"), dtype=pointings_dtype
+            "pointings",
+            data=obs.__getattribute__("pointings"),
+            dtype=pointings_dtype,
+            compression=compression,
         )
     except (AttributeError, TypeError):
         pass
 
     try:
-        output_file.create_dataset("pixel_index", data=obs.__getattribute__("pixel"))
+        output_file.create_dataset(
+            "pixel_index", data=obs.__getattribute__("pixel"), compression=compression
+        )
     except (AttributeError, TypeError):
         pass
 
     try:
         output_file.create_dataset(
-            "psi", data=obs.__getattribute__("psi"), dtype=pointings_dtype
+            "psi",
+            data=obs.__getattribute__("psi"),
+            dtype=pointings_dtype,
+            compression=compression,
         )
     except (AttributeError, TypeError):
         pass
 
     try:
         output_file.create_dataset(
             "global_flags",
             data=rle_compress(obs.__getattribute__("global_flags")),
+            compression=compression,
         )
     except (AttributeError, TypeError):
         pass
 
     try:
         # We must separate the flags belonging to different detectors because they
         # might have different shapes
         for det_idx in range(obs.local_flags.shape[0]):
             flags = obs.__getattribute__("local_flags")
             compressed_flags = rle_compress(flags[det_idx, :])
             output_file.create_dataset(
-                f"flags_{det_idx:04d}", data=compressed_flags, dtype=flags.dtype
+                f"flags_{det_idx:04d}",
+                data=compressed_flags,
+                dtype=flags.dtype,
+                compression=compression,
             )
     except (AttributeError, TypeError):
         pass
 
     output_file.attrs["mpi_rank"] = MPI_COMM_WORLD.rank
     output_file.attrs["mpi_size"] = MPI_COMM_WORLD.size
     output_file.attrs["global_index"] = global_index
@@ -189,14 +207,15 @@
     tod_dtype=np.float32,
     pointings_dtype=np.float32,
     file_name_mask: str = __OBSERVATION_FILE_NAME_MASK,
     custom_placeholders: Optional[List[Dict[str, Any]]] = None,
     start_index: int = 0,
     collective_mpi_call: bool = True,
     tod_fields: List[str] = ["tod"],
+    gzip_compression: bool = False,
 ) -> List[Path]:
     """
     Save a list of observations in a set of HDF5 files
 
     This function takes one or more observations and saves the TODs in several
     HDF5 (each observation leads to *one* file), using `tod_dtype` and
     `pointings_dtype` as the default datatypes for the samples and the pointing
@@ -261,14 +280,18 @@
     `start_index`.
 
     If observations contain more than one timeline in separate fields
     (e.g., foregrounds, dipole, noise…), you can specify the names of the
     fields using the parameter ``tod_fields`` (list of strings), which by
     default will only save `Observation.tod`.
 
+    To save disk space, you can choose to apply GZip compression to the
+    data frames in each HDF5 file (the file will still be a valid .h5
+    file) or to save quaternions instead of full pointings.
+
     """
     try:
         obs[0]
     except TypeError:
         obs = [obs]
     except IndexError:
         # Empty list
@@ -312,14 +335,15 @@
                 output_file=output_file,
                 obs=cur_obs,
                 tod_dtype=tod_dtype,
                 pointings_dtype=pointings_dtype,
                 global_index=params["global_index"],
                 local_index=params["local_index"],
                 tod_fields=tod_fields,
+                gzip_compression=gzip_compression,
             )
 
         file_list.append(file_name)
 
     return file_list
```

### Comparing `litebird_sim-0.8.0/litebird_sim/mapping.py` & `litebird_sim-0.9.0/litebird_sim/mapping.py`

 * *Files 10% similar despite different names*

```diff
@@ -110,33 +110,36 @@
     npp: Any = None
     invnpp: Any = None
     rcond: Any = None
     coordinate_system: CoordinateSystem = CoordinateSystem.Ecliptic
 
 
 @njit
-def _accumulate_map_and_info(tod, pix, psi, weights, info):
+def _accumulate_map_and_info(tod, pix, psi, weights, info, additional_component: bool):
     # Fill the upper triangle of the information matrix and use the lower
     # triangle for the RHS of the map-making equation
     assert tod.shape == pix.shape == psi.shape
 
     ndets = tod.shape[0]
 
     for idet in range(ndets):
         for d, p, a in zip(tod[idet], pix[idet], psi[idet]):
             one = 1.0 / np.sqrt(weights[idet])
             cos = np.cos(2 * a) / np.sqrt(weights[idet])
             sin = np.sin(2 * a) / np.sqrt(weights[idet])
             info_pix = info[p]
-            info_pix[0, 0] += one * one
-            info_pix[0, 1] += one * cos
-            info_pix[0, 2] += one * sin
-            info_pix[1, 1] += cos * cos
-            info_pix[1, 2] += sin * cos
-            info_pix[2, 2] += sin * sin
+
+            if not additional_component:
+                info_pix[0, 0] += one * one
+                info_pix[0, 1] += one * cos
+                info_pix[0, 2] += one * sin
+                info_pix[1, 1] += cos * cos
+                info_pix[1, 2] += sin * cos
+                info_pix[2, 2] += sin * sin
+
             info_pix[1, 0] += d * one * one
             info_pix[2, 0] += d * cos * one
             info_pix[2, 1] += d * sin * one
 
 
 def _extract_map_and_fill_info(info):
     # Extract the RHS of the mapmaking equation from the lower triangle of info
@@ -150,27 +153,29 @@
 
 def make_bin_map(
     obs: Union[Observation, List[Observation]],
     nside: int,
     pointings: Union[np.ndarray, List[np.ndarray], None] = None,
     do_covariance: bool = False,
     output_map_in_galactic: bool = True,
+    components: List[str] = ["tod"],
 ):
     """Bin Map-maker
 
     Map a list of observations
 
     Args:
         obss (list of :class:`Observations`): observations to be mapped. They
             are required to have the following attributes as arrays
 
-            * `tod`: the time-ordered data to be mapped
             * `pointings`: the pointing information (in radians) for each tod
                sample
             * `psi`: the polarization angle (in radians) for each tod sample
+            * any attribute listed in `components` (by default, `tod`) and
+              containing the TOD(s) to be binned together
 
             If the observations are distributed over some communicator(s), they
             must share the same group processes.
             If pointings and psi are not included in the observations, they can
             be provided through an array (or a list of arrays) of dimension
             (Ndetectors x Nsamples x 3), containing theta, phi and psi
         nside (int): HEALPix nside of the output map
@@ -229,31 +234,46 @@
 
     for cur_obs, cur_ptg, cur_psi in zip(obs_list, ptg_list, psi_list):
         try:
             weights = cur_obs.sampling_rate_hz * cur_obs.net_ukrts**2
         except AttributeError:
             weights = np.ones(cur_obs.n_detectors)
 
-        ndets = cur_obs.tod.shape[0]
-        pixidx_all = np.empty_like(cur_obs.tod, dtype=int)
-        polang_all = np.empty_like(cur_obs.tod)
+        first_component = getattr(cur_obs, components[0])
+        ndets = first_component.shape[0]
+        pixidx_all = np.empty_like(first_component, dtype=int)
+        polang_all = np.empty_like(first_component)
 
         for idet in range(ndets):
             if output_map_in_galactic:
                 curr_pointings_det, curr_pol_angle_det = rotate_coordinates_e2g(
                     cur_ptg[idet, :, :], cur_psi[idet, :]
                 )
             else:
                 curr_pointings_det = cur_ptg[idet, :, :]
                 curr_pol_angle_det = cur_psi[idet, :]
 
             pixidx_all[idet] = hpx.ang2pix(curr_pointings_det)
             polang_all[idet] = curr_pol_angle_det
 
-        _accumulate_map_and_info(cur_obs.tod, pixidx_all, polang_all, weights, info)
+        for idx, cur_component_name in enumerate(components):
+            cur_component = getattr(cur_obs, cur_component_name)
+            assert (
+                cur_component.shape == first_component.shape
+            ), 'The two TODs "{}" and "{}" do not have a matching shape'.format(
+                components[0], cur_component_name
+            )
+            _accumulate_map_and_info(
+                cur_component,
+                pixidx_all,
+                polang_all,
+                weights,
+                info,
+                additional_component=idx > 0,
+            )
 
     if all([obs.comm is None for obs in obs_list]) or not mpi.MPI_ENABLED:
         # Serial call
         pass
     elif all(
         [
             mpi.MPI.Comm.Compare(obs_list[i].comm, obs_list[i + 1].comm) < 2
```

### Comparing `litebird_sim-0.8.0/litebird_sim/mbs/fg_models/pysm_ame_1.cfg` & `litebird_sim-0.9.0/litebird_sim/mbs/fg_models/pysm_ame_1.cfg`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/litebird_sim/mbs/fg_models/pysm_dust_4.cfg` & `litebird_sim-0.9.0/litebird_sim/mbs/fg_models/pysm_dust_4.cfg`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/litebird_sim/mbs/fg_models/pysm_dust_5.cfg` & `litebird_sim-0.9.0/litebird_sim/mbs/fg_models/pysm_dust_5.cfg`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/litebird_sim/mbs/fg_models/pysm_dust_7.cfg` & `litebird_sim-0.9.0/litebird_sim/mbs/fg_models/pysm_dust_7.cfg`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/litebird_sim/mbs/fg_models/pysm_dust_8.cfg` & `litebird_sim-0.9.0/litebird_sim/mbs/fg_models/pysm_dust_8.cfg`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/litebird_sim/mbs/mbs.py` & `litebird_sim-0.9.0/litebird_sim/mbs/mbs.py`

 * *Files 1% similar despite different names*

```diff
@@ -858,10 +858,17 @@
                 tot_dict = {}
                 for nch, chnl in enumerate(channels):
                     if self.params.maps_in_ecliptic:
                         tot[nch] = r.rotate_map_alms(
                             tot[nch], lmax=4 * self.params.nside
                         )
                     tot_dict[chnl] = tot[nch]
+                if self.params.maps_in_ecliptic:
+                    tot_dict["Coordinates"] = lbs.CoordinateSystem.Ecliptic
+                else:
+                    tot_dict["Coordinates"] = lbs.CoordinateSystem.Galactic
+
+                tot_dict["Mbs_parameters"] = self.params
+
                 return (tot_dict, saved_maps)
 
         return (None, saved_maps)
```

### Comparing `litebird_sim-0.8.0/litebird_sim/mpi.py` & `litebird_sim-0.9.0/litebird_sim/mpi.py`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/litebird_sim/noise.py` & `litebird_sim-0.9.0/litebird_sim/noise.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from numbers import Number
 from typing import List, Union
 
 import numpy as np
 import scipy as sp
 from numba import njit
 
-from litebird_sim import Observation
+from .observations import Observation
 
 
 def nearest_pow2(data):
     """returns the next largest power of 2 that will encompass the full data set
 
     data: 1-D numpy array
     """
@@ -85,24 +85,24 @@
         random = np.random.default_rng()
 
     noiselen = nearest_pow2(data)
 
     # makes a white noise timestream with unit variance
     noise = random.normal(0, 1, noiselen)
 
-    ft = sp.fft.fft(noise, n=noiselen)
-    freqs = sp.fft.fftfreq(noiselen, d=1 / (2 * sampling_rate_hz))
+    noise = sp.fft.rfft(noise, overwrite_x=True)
+    freqs = sp.fft.rfftfreq(noiselen, d=1 / (2 * sampling_rate_hz))
 
     # filters the white noise in the frequency domain with the 1/f filter
-    build_one_over_f_model(ft, freqs, fknee_mhz, fmin_hz, alpha, sigma)
+    build_one_over_f_model(noise, freqs, fknee_mhz, fmin_hz, alpha, sigma)
 
     # transforms the data back to the time domain
-    ifft = sp.fft.ifft(ft)
+    noise = sp.fft.irfft(noise, overwrite_x=True)
 
-    data += np.real(ifft[: len(data)])
+    data += noise[: len(data)]
 
 
 def rescale_noise(net_ukrts: float, sampling_rate_hz: float, scale: float):
     return net_ukrts * np.sqrt(sampling_rate_hz) * scale / 1e6
 
 
 def add_noise(
@@ -189,40 +189,52 @@
 
 
 def add_noise_to_observations(
     obs: Union[Observation, List[Observation]],
     noise_type: str,
     scale: float = 1.0,
     random: Union[np.random.Generator, None] = None,
+    component: str = "tod",
 ):
     """Add noise of the defined type to the observations in obs
 
     This class provides an interface to the low-level function :func:`.add_noise`.
     The parameter `obs` can either be one :class:`.Observation` instance or a list
     of observations, which are typically taken from the field `observations` of a
     :class:`.Simulation` object. Unlike :func:`.add_noise`, it is not needed to
     pass the noise parameters here, as they are taken from the characteristics of
     the detectors saved in `obs`.
 
+    By default, the noise is added to ``Observation.tod``. If you want to add it to some
+    other field of the :class:`.Observation` class, use `component`::
+
+        for cur_obs in sim.observations:
+            # Allocate a new TOD for the noise alone
+            cur_obs.noise_tod = np.zeros_like(cur_obs.tod)
+
+        # Ask `add_noise_to_observations` to store the noise
+        # in `obs.noise_tod`
+        add_noise_to_observations(sim.observations, …, component="noise_tod")
+
     See :func:`.add_noise` for more information.
     """
     if noise_type not in ["white", "one_over_f"]:
         raise ValueError("Unknown noise type " + noise_type)
 
     if isinstance(obs, Observation):
         obs_list = [obs]
     else:
         obs_list = obs
 
     # iterate through each observation
-    for i, ob in enumerate(obs_list):
+    for i, cur_obs in enumerate(obs_list):
         add_noise(
-            tod=ob.tod,
+            tod=getattr(cur_obs, component),
             noise_type=noise_type,
-            sampling_rate_hz=ob.sampling_rate_hz,
-            net_ukrts=ob.net_ukrts,
-            fknee_mhz=ob.fknee_mhz,
-            fmin_hz=ob.fmin_hz,
-            alpha=ob.alpha,
+            sampling_rate_hz=cur_obs.sampling_rate_hz,
+            net_ukrts=cur_obs.net_ukrts,
+            fknee_mhz=cur_obs.fknee_mhz,
+            fmin_hz=cur_obs.fmin_hz,
+            alpha=cur_obs.alpha,
             scale=scale,
             random=random,
         )
```

### Comparing `litebird_sim-0.8.0/litebird_sim/observations.py` & `litebird_sim-0.9.0/litebird_sim/observations.py`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/litebird_sim/pointings.py` & `litebird_sim-0.9.0/litebird_sim/pointings.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     detector to the boresight reference frame, compute a set of
     pointings for the detector that encompasses the time span
     covered by observation `obs` (i.e., starting from
     `obs.start_time` and including `obs.n_samples` pointings).
     The parameter `spin2ecliptic_quats` can be easily retrieved by
     the field `spin2ecliptic_quats` in a object of
     :class:`.Simulation` object, once the method
-    :meth:`.Simulation.generate_spin2ecl_quaternions` is called.
+    :meth:`.Simulation.set_scanning_strategy` is called.
 
     The parameter `bore2spin_quat` is calculated through the class
     :class:`.Instrument`, which has the field ``bore2spin_quat``.
     If all you have is the angle β between the boresight and the
     spin axis, just pass ``quat_rotation_y(β)`` here.
 
     The parameter `detector_quats` is optional. By default is ``None``,
@@ -127,36 +127,39 @@
     if detector_quats is None:
         assert "quat" in dir(obs), (
             "No detector quaternions found, have you passed "
             + '"detectors=" to Simulation.create_observations?'
         )
         detector_quats = obs.quat
 
-    det2ecliptic_quats = get_det2ecl_quaternions(
-        obs,
-        spin2ecliptic_quats,
-        detector_quats,
-        bore2spin_quat,
-        quaternion_buffer=quaternion_buffer,
-        dtype=dtype_quaternion,
-    )
-
     bufshape = get_pointing_buffer_shape(obs)
     if pointing_buffer is None:
         pointing_buffer = np.empty(bufshape, dtype=dtype_pointing)
     else:
         assert (
             pointing_buffer.shape == bufshape
         ), f"error, wrong pointing buffer size: {pointing_buffer.size} != {bufshape}"
 
-    # Compute the pointing direction for each sample
-    all_compute_pointing_and_polangle(
-        result_matrix=pointing_buffer,
-        quat_matrix=det2ecliptic_quats,
-    )
+    for idx, cur_quat in enumerate(detector_quats):
+        det2ecliptic_quats = get_det2ecl_quaternions(
+            obs,
+            spin2ecliptic_quats,
+            cur_quat.reshape((1, 4)),
+            bore2spin_quat,
+            quaternion_buffer=quaternion_buffer,
+            dtype=dtype_quaternion,
+        )
+
+        # Compute the pointing direction for each sample
+        all_compute_pointing_and_polangle(
+            result_matrix=pointing_buffer[idx, :, :].reshape(
+                (1, pointing_buffer.shape[1], 3)
+            ),
+            quat_matrix=det2ecliptic_quats,
+        )
 
     if hwp:
         apply_hwp_to_obs(obs=obs, hwp=hwp, pointing_matrix=pointing_buffer)
 
     if store_pointings_in_obs:
         obs.pointings = pointing_buffer[:, :, 0:2]
         obs.psi = pointing_buffer[:, :, 2]
```

### Comparing `litebird_sim-0.8.0/litebird_sim/quaternions.py` & `litebird_sim-0.9.0/litebird_sim/quaternions.py`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/litebird_sim/scan_map.py` & `litebird_sim-0.9.0/litebird_sim/scan_map.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 from .observations import Observation
 
 from .coordinates import rotate_coordinates_e2g, CoordinateSystem
 
 from .healpix import npix_to_nside
 
+import logging
+
 
 @njit
 def compute_signal_for_one_sample(T, Q, U, co, si):
     """Bolometric equation"""
     return T + co * Q + si * U
 
 
@@ -87,22 +89,35 @@
 
 
 def scan_map_in_observations(
     obs: Union[Observation, List[Observation]],
     maps: Dict[str, np.ndarray],
     pointings: Union[np.ndarray, List[np.ndarray], None] = None,
     input_map_in_galactic: bool = True,
+    component: str = "tod",
 ):
     """Scan a map filling time-ordered data
 
     This is a wrapper around the :func:`.scan_map` function that applies to the TOD
     stored in `obs` and the pointings stored in `pointings`. The two types can either
     bed a :class:`.Observation` instance and a NumPy matrix, or a list
     of observations and a list of NumPy matrices; in the latter case, they must have
     the same number of elements.
+
+    By default, the signal is added to ``Observation.tod``. If you want to add it to
+    some other field of the :class:`.Observation` class, use `component`::
+
+        for cur_obs in sim.observations:
+            # Allocate a new TOD for the sky signal alone
+            cur_obs.sky_tod = np.zeros_like(cur_obs.tod)
+
+        # Ask `add_noise_to_observations` to store the noise
+        # in `obs.sky_tod`
+        scan_map_in_observations(sim.observations, …, component="sky_tod")
+
     """
 
     if pointings is None:
         if isinstance(obs, Observation):
             obs_list = [obs]
             ptg_list = [obs.pointings]
             psi_list = [obs.psi]
@@ -140,22 +155,32 @@
             elif all(item in maps.keys() for item in cur_obs.channel):
                 input_names = cur_obs.channel
             else:
                 raise ValueError(
                     "The dictionary maps does not contain all the relevant"
                     + "keys, please check the list of detectors and channels"
                 )
+            if "Coordinates" in maps.keys():
+                dict_input_map_in_galactic = (
+                    maps["Coordinates"] is CoordinateSystem.Galactic
+                )
+                if dict_input_map_in_galactic != input_map_in_galactic:
+                    logging.warning(
+                        "input_map_in_galactic variable in scan_map_in_observations"
+                        + " overwritten!"
+                    )
+                input_map_in_galactic = dict_input_map_in_galactic
         else:
             assert isinstance(maps, np.ndarray), (
                 "maps must either a dictionary contaning keys for all the"
                 + "channels/detectors, or be a numpy array of dim (3 x Npix)"
             )
             input_names = None
 
         scan_map(
-            tod=cur_obs.tod,
+            tod=getattr(cur_obs, component),
             pointings=cur_ptg,
             pol_angle=cur_psi,
             maps=maps,
             input_names=input_names,
             input_map_in_galactic=input_map_in_galactic,
         )
```

### Comparing `litebird_sim-0.8.0/litebird_sim/scanning.py` & `litebird_sim-0.9.0/litebird_sim/scanning.py`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/litebird_sim/simulations.py` & `litebird_sim-0.9.0/litebird_sim/simulations.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,54 @@
 # -*- encoding: utf-8 -*-
 
 import codecs
 from collections import namedtuple
-from dataclasses import asdict
+from dataclasses import asdict, dataclass
 from datetime import datetime
+from deprecation import deprecated
 import logging as log
 import os
 import subprocess
-from typing import List, Tuple, Union, Dict, Any
+from typing import List, Tuple, Union, Dict, Any, Optional
 from pathlib import Path
 from shutil import copyfile, copytree, SameFileError
 
-from .detectors import DetectorInfo
+import litebird_sim
+from . import HWP
+from .detectors import DetectorInfo, InstrumentInfo
 from .distribute import distribute_evenly, distribute_optimally
-from .healpix import write_healpix_map_to_file
+from .healpix import write_healpix_map_to_file, npix_to_nside
 from .imo.imo import Imo
 from .mpi import MPI_COMM_WORLD
 from .observations import Observation
+from .pointings import get_pointings
 from .version import (
     __version__ as litebird_sim_version,
     __author__ as litebird_sim_author,
 )
 
+from .dipole import DipoleType, add_dipole_to_observations
+from .scan_map import scan_map_in_observations
+from .spacecraft import SpacecraftOrbit, spacecraft_pos_and_vel
+from .noise import add_noise_to_observations
+
 import astropy.time
 import astropy.units
 import markdown
 import numpy as np
 import jinja2
 import tomlkit
 
 from markdown_katex import KatexExtension
 
 from .scanning import ScanningStrategy, SpinningScanningStrategy
 
 
+DEFAULT_BASE_IMO_URL = "https://litebirdimo.ssdc.asi.it"
+
 OutputFileRecord = namedtuple("OutputFileRecord", ["path", "description"])
 
 
 def _tomlkit_to_popo(d):
     from datetime import date, time, datetime
 
     # This is a fix to issue
@@ -93,14 +104,113 @@
     Given a filename (e.g., ``report_header.md``), this function
     returns a full, absolute path to the file within the ``templates``
     folder of the ``litebird_sim`` source code.
     """
     return Path(__file__).parent / ".." / "templates" / filename
 
 
+@dataclass
+class MpiObservationDescr:
+    """
+    This class is used within :class:`.MpiProcessDescr`. It describes the
+    kind and size of the data held by a :class:`.Observation` object.
+
+    Its fields are:
+
+    - `det_names` (list of ``str``): names of the detectors handled by
+      this observation
+    - `tod_names` (list of ``str``): names of the fields containing the TODs
+      (e.g., ``tod``, ``cmb_tod``, ``dipole_tod``, …)
+    - `tod_shape` (tuples of ``int``): shape of each TOD held by the observation.
+      This is *not* a list, because all the TODs are assumed to have the same shape
+    - `tod_dtype` (list of ``str``): string representing the NumPy data type of each
+      TODs, in the same order as in the field `tod_name`
+    - `start_time` (either a ``float`` or a ``astropy.time.Time``): start date
+      of the observation
+    - `duration_s` (``float``): duration of the TOD in seconds
+    - `num_of_samples` (``int``): number of samples held by this TOD
+    - `num_of_detectors` (``int``): number of detectors held by this TOD. It's
+      the length of the field `det_names` (see above)
+    """
+
+    det_names: List[str]
+    tod_names: List[str]
+    tod_shape: Optional[Tuple[int, int]]
+    tod_dtype: List[str]
+    start_time: Union[float, astropy.time.Time]
+    duration_s: float
+    num_of_samples: int
+    num_of_detectors: int
+
+
+@dataclass
+class MpiProcessDescr:
+    """
+    Description of the kind of data held by a MPI process
+
+    This class is used within :class:`MpiDistributionDescr`. Its fields are:
+
+    - `mpi_rank`: rank of the MPI process described by this instance
+    - `observations`: list of :class:`.MpiObservationDescr` objects, each
+      describing one observation managed by the MPI process with rank
+      `mpi_rank`.
+
+    """
+
+    mpi_rank: int
+    observations: List[MpiObservationDescr]
+
+
+@dataclass
+class MpiDistributionDescr:
+    """A class that describes how observations are distributed among MPI processes
+
+    The fields defined in this dataclass are the following:
+
+    - `num_of_observations` (int): overall number of observations in *all* the
+      MPI processes
+    - `detectors` (list of :class:`.DetectorInfo` objects): list of *all* the
+      detectors used in the observations
+    - `mpi_processes`: list of :class:`.MpiProcessDescr` instances, describing
+      the kind of data that each MPI process is currently holding
+
+    Use :meth:`.Simulation.describe_mpi_distribution` to get an instance of this
+    object."""
+
+    num_of_observations: int
+    detectors: List[DetectorInfo]
+    mpi_processes: List[MpiProcessDescr]
+
+    def __repr__(self):
+        result = ""
+        for cur_mpi_proc in self.mpi_processes:
+            result += f"# MPI rank #{cur_mpi_proc.mpi_rank + 1}\n\n"
+            for cur_obs_idx, cur_obs in enumerate(cur_mpi_proc.observations):
+                result += """## Observation #{obs_idx}
+- Start time: {start_time}
+- Duration: {duration_s} s
+- {num_of_detectors} detector(s) ({det_names})
+- TOD(s): {tod_names}
+- TOD shape: {tod_shape}
+- Type of the TODs: {tod_dtype}
+
+""".format(
+                    obs_idx=cur_obs_idx,
+                    start_time=cur_obs.start_time,
+                    duration_s=cur_obs.duration_s,
+                    num_of_detectors=len(cur_obs.det_names),
+                    det_names=",".join(cur_obs.det_names),
+                    tod_names=", ".join(cur_obs.tod_names),
+                    tod_shape="×".join([str(x) for x in cur_obs.tod_shape]),
+                    tod_dtype=", ".join(cur_obs.tod_dtype),
+                )
+
+        return result
+
+
 class Simulation:
     """A container object for running simulations
 
     This is the most important class in the Litebird_sim framework. It
     initializes an output directory that will contain all the products
     of a simulation and will handle the generation of reports and
     writing of output files.
@@ -125,15 +235,15 @@
     of the form ``(path, description)``, where ``path`` is a
     ``pathlib.Path`` object and ``description`` is a `str` object::
 
         for curpath, curdescr in sim.list_of_outputs:
             print(f"{curpath}: {curdescr}")
 
     When pointing information is needed, you can call the method
-    :meth:`.Simulation.generate_spin2ecl_quaternions`, which
+    :meth:`.Simulation.set_scanning_strategy`, which
     initializes the members `pointing_freq_hz` and
     `spin2ecliptic_quats`; these members are used by functions like
     :func:`.get_pointings`.
 
     Args:
 
         base_path (str or `pathlib.Path`): the folder that will
@@ -187,14 +297,18 @@
         self.name = name
 
         self.observations = []
 
         self.start_time = start_time
         self.duration_s = duration_s
 
+        self.detectors = []  # type: List[DetectorInfo]
+        self.instrument = None  # type: Optional[InstrumentInfo]
+        self.hwp = None  # type: Optional[HWP]
+
         self.spin2ecliptic_quats = None
 
         self.description = description
 
         self.random = None
 
         if imo:
@@ -480,15 +594,17 @@
         for curfig, curfilename in figures:
             curpath = self.base_path / curfilename
             curfig.savefig(curpath)
             self.list_of_outputs.append(
                 OutputFileRecord(path=curpath, description="Figure")
             )
 
-    def _fill_dictionary_with_imo_information(self, dictionary: Dict[str, Any]):
+    def _fill_dictionary_with_imo_information(
+        self, dictionary: Dict[str, Any], base_imo_url: str
+    ):
         # Fill the variable "dictionary" with information about the
         # objects retrieved from the IMO. This is used when producing
         # the final report for a simulation
         if not self.imo:
             return
 
         entities = [
@@ -519,14 +635,15 @@
         if (not entities) and (not quantities) and (not data_files):
             return
 
         dictionary["entities"] = entities
         dictionary["quantities"] = quantities
         dictionary["data_files"] = data_files
         dictionary["warnings"] = warnings
+        dictionary["base_imo_url"] = base_imo_url
 
     def _fill_dictionary_with_code_status(self, dictionary, include_git_diff):
         # Fill the variable "dictionary" with information about the
         # status of the "litebird_sim" code (which version is it? was
         # it patched? etc.) It is used when producing the final report
         # for a simulation
         dictionary["litebird_sim_version"] = litebird_sim_version
@@ -570,27 +687,29 @@
             # Git is not installed, so ignore the error and continue
             pass
         except Exception as e:
             log.warning(
                 f"unable to save information about latest git commit in the report: {e}"
             )
 
-    def flush(self, include_git_diff=True):
+    def flush(self, include_git_diff=True, base_imo_url: str = DEFAULT_BASE_IMO_URL):
         """Terminate a simulation.
 
         This function must be called when a simulation is complete. It
         will save pending data to the output directory.
 
         It returns a `Path` object pointing to the HTML file that has
         been saved in the directory pointed by ``self.base_path``.
 
         """
 
         dictionary = {"datetime": datetime.now().strftime("%Y-%m-%d %H:%M:%S")}
-        self._fill_dictionary_with_imo_information(dictionary)
+        self._fill_dictionary_with_imo_information(
+            dictionary, base_imo_url=base_imo_url
+        )
         self._fill_dictionary_with_code_status(dictionary, include_git_diff)
 
         template_file_path = get_template_file_path("report_appendix.md")
         with template_file_path.open("rt") as inpf:
             markdown_template = "".join(inpf.readlines())
         self.append_to_report(markdown_template, **dictionary)
 
@@ -687,28 +806,35 @@
             self.start_time is not None
         ), "you must set start_time when creating the Simulation object"
 
         assert isinstance(
             self.duration_s, (float, int)
         ), "you must set duration_s when creating the Simulation object"
 
+        if not detectors:
+            detectors = self.detectors
+
+        # if a single detector is passed, make it a list
+        if isinstance(detectors, DetectorInfo):
+            detectors = [detectors]
+
         observations = []
 
         duration_s = self.duration_s  # Cache the value to a local variable
         sampfreq_hz = detectors[0].sampling_rate_hz
-        detectors = [asdict(d) for d in detectors]
+        self.detectors = detectors
         num_of_samples = int(sampfreq_hz * duration_s)
         samples_per_obs = distribute_evenly(num_of_samples, num_of_obs_per_detector)
 
         cur_time = self.start_time
 
         for cur_obs_idx in range(num_of_obs_per_detector):
             nsamples = samples_per_obs[cur_obs_idx].num_of_elements
             cur_obs = Observation(
-                detectors=detectors,
+                detectors=[asdict(d) for d in detectors],
                 start_time_global=cur_time,
                 sampling_rate_hz=sampfreq_hz,
                 n_samples_global=nsamples,
                 n_blocks_det=n_blocks_det,
                 n_blocks_time=n_blocks_time,
                 comm=(None if split_list_over_processes else self.mpi_comm),
                 root=0,
@@ -741,20 +867,104 @@
             weight_fn=lambda obs: obs.n_samples_global,
         )[cur_rank]
 
         self.observations = observations[
             span.start_idx : (span.start_idx + span.num_of_elements)
         ]
 
-    def generate_spin2ecl_quaternions(
+    def describe_mpi_distribution(
+        self, tod_names: List[str] = ["tod"]
+    ) -> Optional[MpiDistributionDescr]:
+        """Return a :class:`.MpiDistributionDescr` object describing observations
+
+        This method returns a :class:`.MpiDistributionDescr` that describes the data
+        stored in each MPI process running concurrently. It is a great debugging tool
+        when you are using MPI, and it can be used for tasks where you have to carefully
+        orchestrate they way different MPI processes run together.
+
+        The method registers the amount of memory required by each TOD; by default, only
+        the ``tod`` field of each observation is considered, but you can pass more than
+        one of them through the parameter ``tod_names`` (a list of strings).
+
+        If this method is called before :meth:`.Simulation.create_observations`, it will
+        return ``None``.
+
+        This method should be called by *all* the MPI processes. It can be executed in a
+        serial environment (i.e., without MPI) and will still return meaningful values.
+
+        The typical usage for this method is to call it once you have called
+        :meth:`.Simulation.create_observations` to check that the TODs have been
+        laid in memory in the way you expect::
+
+            sim.create_observations(…)
+            distr = sim.describe_mpi_distribution()
+            if litebird_sim.MPI_COMM_WORLD.rank == 0:
+                print(distr)
+
+        """
+
+        if not self.observations:
+            return None
+
+        observation_descr = []  # type: List[MpiObservationDescr]
+        for obs in self.observations:
+            cur_det_names = list(obs.name)
+
+            shapes = [tuple(getattr(obs, name).shape) for name in tod_names]
+            # Check that all the TODs have the same shape
+            if shapes:
+                for i in range(1, len(shapes)):
+                    assert shapes[0] == shapes[i], (
+                        f"TOD {tod_names[0]} and {tod_names[i]} have different shapes: "
+                        + f"{shapes[0]} vs {shapes[i]}"
+                    )
+
+            observation_descr.append(
+                MpiObservationDescr(
+                    det_names=cur_det_names,
+                    tod_names=tod_names,
+                    tod_shape=shapes[0] if shapes else None,
+                    tod_dtype=[getattr(obs, name).dtype.name for name in tod_names],
+                    start_time=obs.start_time,
+                    duration_s=obs.n_samples / obs.sampling_rate_hz,
+                    num_of_samples=obs.n_samples,
+                    num_of_detectors=obs.n_detectors,
+                )
+            )
+
+        num_of_observations = len(self.observations)
+
+        if self.mpi_comm and litebird_sim.MPI_ENABLED:
+            observation_descr_all = MPI_COMM_WORLD.allgather(observation_descr)
+            num_of_observations_all = MPI_COMM_WORLD.allgather(num_of_observations)
+        else:
+            observation_descr_all = [observation_descr]
+            num_of_observations_all = [num_of_observations]
+
+        mpi_processes = []  # type: List[MpiProcessDescr]
+        for i in range(MPI_COMM_WORLD.size):
+            mpi_processes.append(
+                MpiProcessDescr(
+                    mpi_rank=i,
+                    observations=observation_descr_all[i],
+                )
+            )
+
+        return MpiDistributionDescr(
+            num_of_observations=sum(num_of_observations_all),
+            detectors=self.detectors,
+            mpi_processes=mpi_processes,
+        )
+
+    def set_scanning_strategy(
         self,
         scanning_strategy: Union[None, ScanningStrategy] = None,
         imo_url: Union[None, str] = None,
         delta_time_s: float = 60.0,
-        append_to_report=True,
+        append_to_report: bool = True,
     ):
         """Simulate the motion of the spacecraft in free space
 
         This method computes the quaternions that encode the evolution
         of the spacecraft's orientation in time, assuming the scanning
         strategy described in the parameter `scanning_strategy` (an
         object of a class derived by :class:`.ScanningStrategy`; most
@@ -770,25 +980,26 @@
         ``/releases/v1.0/satellite/scanning_parameters/``) describing
         the parameters of the scanning strategy will be loaded. In
         this case, a :class:`SpinningScanningStrategy` object will be
         created automatically.
 
         The parameter `delta_time_s` specifies how often should
         quaternions be computed; see
-        :meth:`.ScanningStrategy.generate_spin2ecl_quaternions` for
+        :meth:`.ScanningStrategy.set_scanning_strategy` for
         more information.
 
         If the parameter `append_to_report` is set to ``True`` (the
         default), some information about the pointings will be included
-        in the report saved by the :class:`.Simulation` object.
+        in the report saved by the :class:`.Simulation` object. This will
+        be done only if the process has rank #0.
 
         """
         assert not (scanning_strategy and imo_url), (
             "you must either specify scanning_strategy or imo_url (but not"
-            "the two together) when calling Simulation.generate_spin2ecl_quaternions"
+            "the two together) when calling Simulation.set_scanning_strategy"
         )
 
         if not scanning_strategy:
             if not imo_url:
                 imo_url = "/releases/v1.0/satellite/scanning_parameters/"
 
             scanning_strategy = SpinningScanningStrategy.from_imo(
@@ -799,16 +1010,266 @@
         self.spin2ecliptic_quats = scanning_strategy.generate_spin2ecl_quaternions(
             start_time=self.start_time,
             time_span_s=self.duration_s,
             delta_time_s=delta_time_s,
         )
         quat_memory_size_bytes = self.spin2ecliptic_quats.nbytes()
 
-        template_file_path = get_template_file_path("report_generate_pointings.md")
-        with template_file_path.open("rt") as inpf:
-            markdown_template = "".join(inpf.readlines())
-        self.append_to_report(
-            markdown_template,
-            num_of_obs=len(self.observations),
+        num_of_obs = len(self.observations)
+        if append_to_report and litebird_sim.MPI_ENABLED:
+            num_of_obs = MPI_COMM_WORLD.allreduce(num_of_obs)
+
+        if append_to_report and MPI_COMM_WORLD.rank == 0:
+            template_file_path = get_template_file_path("report_quaternions.md")
+            with template_file_path.open("rt") as inpf:
+                markdown_template = "".join(inpf.readlines())
+            self.append_to_report(
+                markdown_template,
+                num_of_obs=num_of_obs,
+                num_of_mpi_processes=MPI_COMM_WORLD.size,
+                delta_time_s=delta_time_s,
+                quat_memory_size_bytes=quat_memory_size_bytes,
+            )
+
+    @deprecated(
+        deprecated_in="0.9",
+        current_version=litebird_sim_version,
+        details="Use set_scanning_strategy",
+    )
+    def generate_spin2ecl_quaternions(
+        self,
+        scanning_strategy: Union[None, ScanningStrategy] = None,
+        imo_url: Union[None, str] = None,
+        delta_time_s: float = 60.0,
+        append_to_report=True,
+    ):
+        self.set_scanning_strategy(
+            scanning_strategy=scanning_strategy,
+            imo_url=imo_url,
             delta_time_s=delta_time_s,
-            quat_memory_size_bytes=quat_memory_size_bytes,
+            append_to_report=append_to_report,
         )
+
+    def set_instrument(self, instrument: InstrumentInfo):
+        """Set the instrument to be used in the simulation.
+
+        This function sets the ``self.instrument`` field to the instance
+        of the class :class:`.InstrumentInfo` that has been passed as
+        argument. The purpose of the instrument is to provide the reference
+        frame for the direction of each detector.
+
+        Note that you should not simulate more than one instrument in the same
+        simulation. This is enforced by the fact that if you call `set_instrument`
+        twice, the second call will overwrite the instrument that was formerly
+        set.
+        """
+        self.instrument = instrument
+
+    def set_hwp(self, hwp: HWP):
+        """Set the HWP to be used in the simulation
+
+        The argument must be a class derived from :class:`.HWP`, for instance
+        :class:`.IdealHWP`.
+        """
+        self.hwp = hwp
+
+    def compute_pointings(
+        self,
+        append_to_report: bool = True,
+        dtype_quaternion=np.float64,
+        dtype_pointing=np.float32,
+    ):
+        """Trigger the computation of pointings.
+
+        This method must be called after having set the scanning strategy, the
+        instrument, and the list of detectors to simulate through calls to
+        :meth:`.set_instrument` and :meth:`.add_detector`. It combines the
+        quaternions of the spacecraft, of the instrument, and of the detectors
+        and sets the fields ``pointings``, ``psi``, and ``pointing_coords`` in
+        each observation owned by the simulation.
+        """
+        assert self.detectors, (
+            "You must call Simulation.create_observations() "
+            "before calling Simulation.compute_pointings"
+        )
+        assert self.instrument
+        assert self.spin2ecliptic_quats
+
+        memory_occupation = 0
+        num_of_obs = 0
+        for cur_obs in self.observations:
+            get_pointings(
+                cur_obs,
+                self.spin2ecliptic_quats,
+                detector_quats=cur_obs.quat,
+                bore2spin_quat=self.instrument.bore2spin_quat,
+                hwp=self.hwp,
+                dtype_quaternion=dtype_quaternion,
+                dtype_pointing=dtype_pointing,
+                store_pointings_in_obs=True,
+            )
+            memory_occupation += cur_obs.pointings.nbytes + cur_obs.psi.nbytes
+            num_of_obs += 1
+
+        if append_to_report and litebird_sim.MPI_ENABLED:
+            memory_occupation = MPI_COMM_WORLD.allreduce(memory_occupation)
+            num_of_obs = MPI_COMM_WORLD.allreduce(num_of_obs)
+
+        if append_to_report and MPI_COMM_WORLD.rank == 0:
+            template_file_path = get_template_file_path("report_pointings.md")
+            with template_file_path.open("rt") as inpf:
+                markdown_template = "".join(inpf.readlines())
+            self.append_to_report(
+                markdown_template,
+                num_of_obs=num_of_obs,
+                hwp_description=str(self.hwp) if self.hwp else "No HWP",
+                num_of_mpi_processes=MPI_COMM_WORLD.size,
+                memory_occupation=memory_occupation,
+            )
+
+    def compute_pos_and_vel(
+        self,
+        delta_time_s=86400.0,
+        solar_velocity_km_s: float = 369.8160,
+        solar_velocity_gal_lat_rad: float = 0.842_173_724,
+        solar_velocity_gal_lon_rad: float = 4.608_035_744_4,
+    ):
+        """Computes the position and the velocity of the spacescraft for computing
+        the dipole.
+        It wraps the :class:`.SpacecraftOrbit` and calls :meth:`.SpacecraftOrbit`.
+        The parameters that can be modified are the sampling of position and velocity
+        and the direction and amplitude of the solar dipole.
+        Default values for solar dipole from Planck 2018 Solar dipole (see arxiv:
+        1807.06207)
+        """
+
+        orbit = SpacecraftOrbit(
+            self.start_time,
+            solar_velocity_km_s=solar_velocity_km_s,
+            solar_velocity_gal_lat_rad=solar_velocity_gal_lat_rad,
+            solar_velocity_gal_lon_rad=solar_velocity_gal_lon_rad,
+        )
+
+        self.pos_and_vel = spacecraft_pos_and_vel(
+            orbit=orbit, obs=self.observations, delta_time_s=delta_time_s
+        )
+
+    def fill_tods(
+        self,
+        maps: Dict[str, np.ndarray],
+        append_to_report: bool = True,
+    ):
+        """Fills the TODs, scanning a map.
+
+        This method must be called after having set the scanning strategy, the
+        instrument, the list of detectors to simulate through calls to
+        :meth:`.set_instrument` and :meth:`.add_detector`, and the methond
+        compute_pointings. maps is assumed to be produced by :class:`.Mbs`
+        """
+
+        scan_map_in_observations(
+            self.observations,
+            maps=maps,
+        )
+
+        if append_to_report and MPI_COMM_WORLD.rank == 0:
+            template_file_path = get_template_file_path("report_scan_map.md")
+            with template_file_path.open("rt") as inpf:
+                markdown_template = "".join(inpf.readlines())
+            if type(maps) is dict:
+                if "Mbs_parameters" in maps.keys():
+
+                    if maps["Mbs_parameters"].make_fg:
+                        fg_model = maps["Mbs_parameters"].fg_models
+                    else:
+                        fg_model = "N/A"
+
+                    self.append_to_report(
+                        markdown_template,
+                        nside=maps["Mbs_parameters"].nside,
+                        has_cmb=maps["Mbs_parameters"].make_cmb,
+                        has_fg=maps["Mbs_parameters"].make_fg,
+                        fg_model=fg_model,
+                    )
+            else:
+                nside = npix_to_nside(len(maps[0]))
+                self.append_to_report(
+                    markdown_template,
+                    nside=nside,
+                    has_cmb="N/A",
+                    has_fg="N/A",
+                    fg_model="N/A",
+                )
+
+    def add_dipole(
+        self,
+        t_cmb_k: float = 2.72548,  # Fixsen 2009 http://arxiv.org/abs/0911.1955
+        dipole_type: DipoleType = DipoleType.TOTAL_FROM_LIN_T,
+        append_to_report: bool = True,
+    ):
+        """Fills the tod with dipole.
+
+        This method must be called after having set the scanning strategy, the
+        instrument, the list of detectors to simulate through calls to
+        :meth:`.set_instrument` and :meth:`.add_detector`, and the pointing
+        through :meth:`.compute_pointings`.
+        """
+
+        if not hasattr(self, "pos_and_vel"):
+            self.compute_pos_and_vel()
+
+        add_dipole_to_observations(
+            obs=self.observations,
+            pos_and_vel=self.pos_and_vel,
+            t_cmb_k=t_cmb_k,
+            dipole_type=dipole_type,
+        )
+
+        if append_to_report and MPI_COMM_WORLD.rank == 0:
+            template_file_path = get_template_file_path("report_dipole.md")
+
+            dip_lat_deg = np.rad2deg(self.pos_and_vel.orbit.solar_velocity_gal_lat_rad)
+            dip_lon_deg = np.rad2deg(self.pos_and_vel.orbit.solar_velocity_gal_lon_rad)
+            dip_velocity = self.pos_and_vel.orbit.solar_velocity_km_s
+
+            with template_file_path.open("rt") as inpf:
+                markdown_template = "".join(inpf.readlines())
+            self.append_to_report(
+                markdown_template,
+                t_cmb_k=t_cmb_k,
+                dipole_type=dipole_type,
+                dip_lat_deg=dip_lat_deg,
+                dip_lon_deg=dip_lon_deg,
+                dip_velocity=dip_velocity,
+            )
+
+    def add_noise(
+        self,
+        noise_type: str = "one_over_f",
+        random: Union[np.random.Generator, None] = None,
+        append_to_report: bool = True,
+    ):
+
+        """Adds noise to tods.
+
+        This method must be called after having set the instrument,
+        the list of detectors to simulate through calls to
+        :meth:`.set_instrument` and :meth:`.add_detector`.
+        """
+
+        if random is None:
+            random = self.random
+
+        add_noise_to_observations(
+            obs=self.observations,
+            noise_type=noise_type,
+            random=random,
+        )
+
+        if append_to_report and MPI_COMM_WORLD.rank == 0:
+            template_file_path = get_template_file_path("report_noise.md")
+            with template_file_path.open("rt") as inpf:
+                markdown_template = "".join(inpf.readlines())
+            self.append_to_report(
+                markdown_template,
+                noise_type="white + 1/f " if noise_type == "one_over_f" else "white",
+            )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `litebird_sim-0.8.0/litebird_sim/spacecraft.py` & `litebird_sim-0.9.0/litebird_sim/spacecraft.py`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/misc/pandoc-filter.lua` & `litebird_sim-0.9.0/misc/pandoc-filter.lua`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/pyproject.toml` & `litebird_sim-0.9.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -10,25 +10,28 @@
   | dist
   | docs
 )/
 '''
 
 [tool.poetry]
 name = "litebird_sim"
-version = "0.8.0"
+version = "0.9.0"
 description = "Simulation tools for the LiteBIRD experiment"
 authors = [
 	"The LiteBIRD Simulation Team",
 	"Ranajoy Banerji <ranajoy.cosmo@gmail.com>",
+	"Marco Bortolami <marco.bortolami@unife.it>",
 	"Mathew Galloway <mathew.galloway@astro.uio.no>",
 	"Martina Gerbino <gerbinom@fe.infn.it>",
 	"Serena Giardiello <serena.giardiello@unife.it>",
 	"Nicoletta Krachmalnicoff <nkrach@sissa.it>",
 	"Luca Pagano <luca.pagano@unife.it>",
 	"Davide Poletti <davide.poletti@sissa.it>",
+	"Giuseppe Puglisi <giuspugl@roma2.infn.it>",
+	"Nicolò Raffuzzi <rffnll@unife.it>",
 	"Martin Reinecke <martin@mpa-garching.mpg.de>",
 	"Maurizio Tomasi <maurizio.tomasi@unimi.it>",
 ]
 readme = "README.md"
 license = "GPL3"
 include = [
 	"images/logo.png",
@@ -75,14 +78,15 @@
 ducc0 = "^0.25.0"
 pysm3 = "^3.3.0"
 asciimatics = "^1.12.0"
 pyperclip = "^1.8.1"
 pre-commit = "^2.15.0"
 h5py = "3.4"
 toast-cmb = "^2.3.14"
+deprecation = "^2.1.0"
 
 [tool.poetry.extras]
 mpi = ["mpi4py"]
 jupyter = ["jupyter"]
 
 [build-system]
 requires = ["poetry_core>=1.0"]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `litebird_sim-0.8.0/static/report_template.html` & `litebird_sim-0.9.0/static/report_template.html`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/static/sakura.css` & `litebird_sim-0.9.0/static/sakura.css`

 * *Files identical despite different names*

### Comparing `litebird_sim-0.8.0/templates/madam_simulation_file.txt` & `litebird_sim-0.9.0/templates/madam_simulation_file.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 # Simulation file for Madam
 # Created by litebird_sim on {{ current_date }}
 
 fsample = {{ sampling_rate_hz }}
 nofiles = {{ number_of_files }}
-label_start = 0
-label_end = {{ number_of_files - 1 }}
 
-tod_info = 1 1.0 tod
+{% for cur_component in components_to_save %}
+tod_info = {{ loop.index }} 1.0 {{ cur_component }}
+{% endfor %}
 
 #
 # Detectors
 
 {% for det in detectors %}
 detector_info = {{ "%5d" | format(loop.index) }} 0.0 T {{ det.net_ukrts }} {{ det.slope }} {{ det.fknee_hz }} {{ det.fmin_hz }} {{ loop.index }} {{ det.name }}
 {% endfor %}
 
 #
 # Pointings
 
 path_point = {{ pointings_path }}
 
 {% for pnt in pointing_files %}
-file_point = {{ pnt.det_id }} {{ pnt.file_name }}
+file_point = {{ pnt.det_id }} {{ pnt.file_name }}[1]
 {% endfor %}
 
 #
 # TOD
 
-path_tod = 1 {{ tod_path }}
+{% for cur_component in components_to_save %}
+path_tod = {{ loop.index }} {{ tod_path }}
 
+{% set outer_index = loop.index %}
 {% for tod in tod_files %}
-file_tod = 1 {{ tod.det_id }} {{ tod.file_name }}
+file_tod = {{ outer_index }} {{ tod.det_id }} {{ tod.file_name }}[{{ outer_index }}]
+{% endfor %}
+
 {% endfor %}
```

### Comparing `litebird_sim-0.8.0/templates/report_appendix.md` & `litebird_sim-0.9.0/templates/report_appendix.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,59 +1,55 @@
 ## Instrument model objects
 
-{% if entities -%}
-
+{% if entities %}
 ### Entities
 
 Name                 | UUID
 -------------------- | --------------------------------------------------
 {% for obj in entities -%}
-{{"%-20s"|format(obj.name)}} | {{ obj.uuid }}
+{{ obj.name }} | [{{ obj.uuid|string|truncate(9) }}]({{ base_imo_url }}/browse/entities/{{ obj.uuid }}/)
 {% endfor -%}
 {% endif -%}
 
-{% if quantities -%}
-
+{% if quantities %}
 ### Quantities
 
 Name                 | UUID
 -------------------- | --------------------------------------------------
 {% for obj in quantities -%}
-{{"%-20s"|format(obj.name)}} | {{ obj.uuid }}
+{{ obj.name }} | [{{ obj.uuid|string|truncate(9) }}]({{ base_imo_url }}/browse/quantities/{{ obj.uuid }}/)
 {% endfor -%}
 {% endif -%}
 
-{% if data_files -%}
-
+{% if data_files %}
 ### Data Files
 
 Name                 | UUID                                 | Upload date
 -------------------- | ------------------------------------ | ------------
 {% for obj in data_files -%}
-{{"%-20s"|format(obj.name)}} | {{ obj.uuid }} | {{ obj.upload_date }}
+{{ obj.name }} | [{{ obj.uuid|string|truncate(9) }}]({{ base_imo_url }}/browse/data_files/{{ obj.uuid }}/) | {{ obj.upload_date }}
 {% endfor -%}
 {% endif -%}
 
-{% if warnings -%}
-
+{% if warnings %}
 ### Warnings
 
 {% for w in warnings -%}
--   {{ w[0].uuid|string|truncate(9) }} ({{ w[0].upload_date }}) has been
-    superseded by {{ w[1].uuid }} ({{ w[1].upload_date }})
+-   [{{ w[0].uuid|string|truncate(9) }}]({{ base_imo_url }}/browse/data_files/{{ w[0].uuid }}/) ({{ w[0].upload_date }}) has been
+    superseded by [{{ w[1].uuid|string|truncate(9) }}]({{ base_imo_url }}/browse/data_files/{{ w[1].uuid }}/) ({{ w[1].upload_date }})
 {% endfor -%}
 {% endif %}
 
 ## Source code used in the simulation
 
 -   Main repository: [github.com/litebird/litebird_sim](https://github.com/litebird/litebird_sim)
 -   Version: {{ litebird_sim_version }}, by {{ litebird_sim_author }}
 {% if short_commit_hash -%}
--   Commit hash: [{{ short_commit_hash }}](https://github.com/litebird/litebird_sim/commit/{commit_hash})
-    (_{{ commit_message }}_, by {{ author }})
+-   Commit hash: [{{ short_commit_hash }}](https://github.com/litebird/litebird_sim/commit/{{commit_hash}})
+    (commit comment: *{{ commit_message }}*, by {{ author }})
 {% endif %}
 
 {% if skip_code_diff %}
 The command `git diff` was skipped. Use `include_git_diff = True` when
 calling `Simulation.flush()` to enable it.
 {% else %}
 {% if code_diff -%}
```

### Comparing `litebird_sim-0.8.0/setup.py` & `litebird_sim-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
  'litebird_sim.mbs': ['fg_models/*']}
 
 install_requires = \
 ['PyGithub>=1.53,<2.0',
  'asciimatics>=1.12.0,<2.0.0',
  'astropy>=4.3,<5.0',
  'black>=22.3,<23.0',
+ 'deprecation>=2.1.0,<3.0.0',
  'ducc0>=0.25.0,<0.26.0',
  'flake8>=3.7,<4.0',
  'h5py==3.4',
  'healpy>=1.15.0,<2.0.0',
  'jinja2>=3.0,<4.0',
  'jplephem>=2.14,<3.0',
  'katex>=0.0.4,<0.0.5',
@@ -48,22 +49,22 @@
  'tomlkit>=0.11.2,<0.12.0']
 
 extras_require = \
 {'jupyter': ['jupyter>=1.0,<2.0'], 'mpi': ['mpi4py>=3.0,<4.0']}
 
 setup_kwargs = {
     'name': 'litebird-sim',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Simulation tools for the LiteBIRD experiment',
-    'long_description': '<!--\nTemplate taken from https://github.com/othneildrew/Best-README-Template\n\n*** To avoid retyping too much info. Do a search and replace for the following:\n*** github_username, repo, twitter_handle, email\n-->\n\n\n<!-- PROJECT SHIELDS -->\n<!--\n*** I\'m using markdown "reference style" links for readability.\n*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).\n*** See the bottom of this document for the declaration of the reference variables\n*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.\n*** https://www.markdownguide.org/basic-syntax/#reference-style-links\n-->\n[![Stable](https://img.shields.io/badge/docs-stable-blue.svg)](https://litebird-sim.readthedocs.io/en/master/)\n[![Tests](https://github.com/litebird/litebird_sim/workflows/Tests/badge.svg?branch=master&event=push)](https://github.com/litebird/litebird_sim/actions?query=workflow%3ATests+branch%3Amaster)\n[![Build Status](https://ci.appveyor.com/api/projects/status/github/litebird/litebird-sim?svg=true)](https://ci.appveyor.com/project/litebird/litebird-sim)\n[![Issues][issues-shield]][issues-url]\n[![GPL3 License][license-shield]][license-url]\n\n\n<!-- PROJECT LOGO -->\n<br />\n<p align="center">\n  <a href="https://github.com/litebird/litebird_sim">\n    <img src="images/logo.png" alt="Logo" width="80" height="80">\n  </a>\n\n  <h3 align="center">LiteBIRD Simulation Framework</h3>\n\n  <p align="center">\n    Main repository of the LiteBIRD Simulation Framework, a set of Python modules to simulate the instruments onboard the LiteBIRD spacecraft.\n    <br />\n    <a href="https://litebird-sim.readthedocs.io/en/master/"><strong>Explore the docs »</strong></a>\n    <br />\n    <br />\n    <a href="https://litebird-sim.readthedocs.io/en/master/tutorial.html">View Demo</a>\n    ·\n    <a href="https://github.com/litebird/litebird_sim/issues">Report Bug</a>\n    ·\n    <a href="https://github.com/litebird/litebird_sim/issues">Request Feature</a>\n  </p>\n</p>\n\n\n\n<!-- TABLE OF CONTENTS -->\n## Table of Contents\n\n* [About the Project](#about-the-project)\n  * [Built With](#built-with)\n* [Getting Started](#getting-started)\n  * [Prerequisites](#prerequisites)\n  * [Installation](#installation)\n* [Usage](#usage)\n* [Roadmap](#roadmap)\n* [Contributing](#contributing)\n* [License](#license)\n* [Contact](#contact)\n* [Acknowledgements](#acknowledgements)\n\n\n\n<!-- ABOUT THE PROJECT -->\n## About The Project\n\nThe LiteBIRD Simulation Framework is being developed for the\n[LiteBIRD collaboration](http://litebird.jp/eng/).\n\n\n### Built With\n\n-   Love!\n-   [Python 3](https://www.python.org)\n-   [Poetry](https://python-poetry.org/)\n-   [NumPy](https://numpy.org)\n-   [Astropy](https://www.astropy.org)\n-   [Healpix](https://healpix.jpl.nasa.gov)\n-   [Sphinx](https://www.sphinx-doc.org/en/master/)\n-   [Numba](https://numba.pydata.org/)\n-   [ducc](https://github.com/litebird/ducc)\n\n\n<!-- GETTING STARTED -->\n## Getting Started\n\nRefer to the\n[documentation](https://litebird-sim.readthedocs.io/en/master/installation.html)\nto learn how to install the LiteBIRD simulation framework on your\ncomputer or on a HPC cluster.\n\n\n<!-- USAGE EXAMPLES -->\n## Usage\n\nThe documentation is available online at\n[litebird-sim.readthedocs.io/en/master/](https://litebird-sim.readthedocs.io/en/master/).\n\nTo create a local copy of the documentation, make sure you ran\n`poetry` with the flag `--extras=docs`, then run the following\ncommand:\n\n-   Linux or Mac OS X:\n    ```\n    ./refresh_docs.sh\n    ```\n\n-   Windows:\n    ```\n    poetry shell\n    cd docs\n    make.bat html\n    ```\n\n\n<!-- ROADMAP -->\n## Roadmap\n\nSee the [open issues](https://github.com/litebird/litebird_sim/issues)\nfor a list of proposed features (and known issues).\n\n\n<!-- CONTRIBUTING -->\n## Contributing\n\nIf you are part of the LiteBIRD collaboration and have something that\nmight fit in this framework, you\'re encouraged to contact us! Any\ncontributions you make are **greatly appreciated**.\n\n1.  Read [CONTRIBUTING.md](https://github.com/litebird/litebird_sim/blob/master/CONTRIBUTING.md)\n2.  Fork the project\n3.  Create your feature branch (`git checkout -b feature/AmazingFeature`)\n4.  Commit your changes (`git commit -m \'Add some AmazingFeature\'`)\n5.  Push to the Branch (`git push origin feature/AmazingFeature`)\n6.  Open a Pull Request\n\n\n<!-- LICENSE -->\n## License\n\nDistributed under the [GPL3 License][license-url].\n\n\n<!-- CONTACT -->\n## Contact\n\nLiteBIRD Simulation Team - litebird_pipe@db.ipmu.jp\n\nProject Link: [https://github.com/litebird/litebird_sim](https://github.com/litebird/litebird_sim)\n\n\n\n<!-- ACKNOWLEDGEMENTS -->\n## How to cite this code\n\nTODO!\n\n\n<!-- MARKDOWN LINKS & IMAGES -->\n<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->\n[issues-shield]: https://img.shields.io/github/issues/litebird/litebird_sim?style=flat-square\n[issues-url]: https://github.com/litebird/litebird_sim/issues\n[license-shield]: https://img.shields.io/github/license/litebird/litebird_sim.svg?style=flat-square\n[license-url]: https://github.com/litebird/litebird_sim/blob/master/LICENSE\n\n<!-- Once we have some nice screenshot, let\'s put a link to it here! -->\n[product-screenshot]: images/screenshot.png\n',
+    'long_description': '<!--\nTemplate taken from https://github.com/othneildrew/Best-README-Template\n\n*** To avoid retyping too much info. Do a search and replace for the following:\n*** github_username, repo, twitter_handle, email\n-->\n\n\n<!-- PROJECT SHIELDS -->\n<!--\n*** I\'m using markdown "reference style" links for readability.\n*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).\n*** See the bottom of this document for the declaration of the reference variables\n*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.\n*** https://www.markdownguide.org/basic-syntax/#reference-style-links\n-->\n[![Stable](https://img.shields.io/badge/docs-stable-blue.svg)](https://litebird-sim.readthedocs.io/en/master/)\n[![Tests](https://github.com/litebird/litebird_sim/workflows/Tests/badge.svg?branch=master&event=push)](https://github.com/litebird/litebird_sim/actions?query=workflow%3ATests+branch%3Amaster)\n[![Build Status](https://ci.appveyor.com/api/projects/status/github/litebird/litebird-sim?svg=true)](https://ci.appveyor.com/project/litebird/litebird-sim)\n[![Issues][issues-shield]][issues-url]\n[![GPL3 License][license-shield]][license-url]\n\n\n<!-- PROJECT LOGO -->\n<br />\n<p align="center">\n  <a href="https://github.com/litebird/litebird_sim">\n    <img src="images/logo.png" alt="Logo" width="80" height="80">\n  </a>\n\n  <h3 align="center">LiteBIRD Simulation Framework</h3>\n\n  <p align="center">\n    Main repository of the LiteBIRD Simulation Framework, a set of Python modules to simulate the instruments onboard the LiteBIRD spacecraft.\n    <br />\n    <a href="https://litebird-sim.readthedocs.io/en/master/"><strong>Explore the docs »</strong></a>\n    <br />\n    <br />\n    <a href="https://litebird-sim.readthedocs.io/en/master/tutorial.html">View Demo</a>\n    ·\n    <a href="https://github.com/litebird/litebird_sim/issues">Report Bug</a>\n    ·\n    <a href="https://github.com/litebird/litebird_sim/issues">Request Feature</a>\n  </p>\n</p>\n\n\n\n<!-- TABLE OF CONTENTS -->\n## Table of Contents\n\n* [About the Project](#about-the-project)\n  * [Built With](#built-with)\n* [Getting Started](#getting-started)\n  * [Prerequisites](#prerequisites)\n  * [Installation](#installation)\n* [Usage](#usage)\n* [Roadmap](#roadmap)\n* [Contributing](#contributing)\n* [License](#license)\n* [Contact](#contact)\n* [Acknowledgements](#acknowledgements)\n\n\n\n<!-- ABOUT THE PROJECT -->\n## About The Project\n\nThe LiteBIRD Simulation Framework is being developed for the\n[LiteBIRD collaboration](http://litebird.jp/eng/).\n\n\n### Built With\n\n-   Love!\n-   [Python 3](https://www.python.org)\n-   [Poetry](https://python-poetry.org/)\n-   [NumPy](https://numpy.org)\n-   [Astropy](https://www.astropy.org)\n-   [Healpix](https://healpix.jpl.nasa.gov)\n-   [Sphinx](https://www.sphinx-doc.org/en/master/)\n-   [Numba](https://numba.pydata.org/)\n-   [ducc](https://github.com/litebird/ducc)\n\n\n<!-- GETTING STARTED -->\n## Getting Started\n\nRefer to the\n[documentation](https://litebird-sim.readthedocs.io/en/master/installation.html)\nto learn how to install the LiteBIRD simulation framework on your\ncomputer or on a HPC cluster.\n\n\n<!-- USAGE EXAMPLES -->\n## Usage\n\nAn example notebook is avalable [here](https://github.com/litebird/litebird_sim/blob/master/notebooks/litebird_sim_example.ipynb). \n\nThe documentation is available online at\n[litebird-sim.readthedocs.io/en/master/](https://litebird-sim.readthedocs.io/en/master/).\n\nTo create a local copy of the documentation, make sure you ran\n`poetry` with the flag `--extras=docs`, then run the following\ncommand:\n\n-   Linux or Mac OS X:\n    ```\n    ./refresh_docs.sh\n    ```\n\n-   Windows:\n    ```\n    poetry shell\n    cd docs\n    make.bat html\n    ```\n\n\n<!-- ROADMAP -->\n## Roadmap\n\nSee the [open issues](https://github.com/litebird/litebird_sim/issues)\nfor a list of proposed features (and known issues).\n\n\n<!-- CONTRIBUTING -->\n## Contributing\n\nIf you are part of the LiteBIRD collaboration and have something that\nmight fit in this framework, you\'re encouraged to contact us! Any\ncontributions you make are **greatly appreciated**.\n\n1.  Read [CONTRIBUTING.md](https://github.com/litebird/litebird_sim/blob/master/CONTRIBUTING.md)\n2.  Fork the project\n3.  Create your feature branch (`git checkout -b feature/AmazingFeature`)\n4.  Commit your changes (`git commit -m \'Add some AmazingFeature\'`)\n5.  Push to the Branch (`git push origin feature/AmazingFeature`)\n6.  Open a Pull Request\n\n\n<!-- LICENSE -->\n## License\n\nDistributed under the [GPL3 License][license-url].\n\n\n<!-- CONTACT -->\n## Contact\n\nLiteBIRD Simulation Team - litebird_pipe@db.ipmu.jp\n\nProject Link: [https://github.com/litebird/litebird_sim](https://github.com/litebird/litebird_sim)\n\n\n\n<!-- ACKNOWLEDGEMENTS -->\n## How to cite this code\n\nTODO!\n\n\n<!-- MARKDOWN LINKS & IMAGES -->\n<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->\n[issues-shield]: https://img.shields.io/github/issues/litebird/litebird_sim?style=flat-square\n[issues-url]: https://github.com/litebird/litebird_sim/issues\n[license-shield]: https://img.shields.io/github/license/litebird/litebird_sim.svg?style=flat-square\n[license-url]: https://github.com/litebird/litebird_sim/blob/master/LICENSE\n\n<!-- Once we have some nice screenshot, let\'s put a link to it here! -->\n[product-screenshot]: images/screenshot.png\n',
     'author': 'The LiteBIRD Simulation Team',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'author_email': 'None',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'python_requires': '>=3.7.1,<3.10',
 }
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['litebird_sim', 'litebird_sim.destriper', 'litebird_sim.hwp_sys',
 'litebird_sim.imo', 'litebird_sim.mbs'] package_data = \ {'': ['*'],
 'litebird_sim': ['datautils/*'], 'litebird_sim.hwp_sys': ['examples/*'],
 'litebird_sim.mbs': ['fg_models/*']} install_requires = \
 ['PyGithub>=1.53,<2.0', 'asciimatics>=1.12.0,<2.0.0', 'astropy>=4.3,<5.0',
-'black>=22.3,<23.0', 'ducc0>=0.25.0,<0.26.0', 'flake8>=3.7,<4.0', 'h5py==3.4',
-'healpy>=1.15.0,<2.0.0', 'jinja2>=3.0,<4.0', 'jplephem>=2.14,<3.0',
-'katex>=0.0.4,<0.0.5', 'markdown-katex>=202006.1021,<202007.0',
-'markdown>=3.2,<4.0', 'matplotlib>=3.1,<4.0', 'numba>=0.55,<0.56',
-'numpy>=1.21,<2.0', 'pre-commit>=2.15.0,<3.0.0', 'pybind11>=2.5.0,<3.0.0',
-'pyperclip>=1.8.1,<2.0.0', 'pysm3>=3.3.0,<4.0.0', 'pytest>=5.3,<6.0',
-'pyyaml>=5.3.1,<6.0.0', 'requests>=2.24.0,<3.0.0', 'rich>=11.0.0,<12.0.0',
-'sphinx>=5.1,<6.0', 'sphinx_rtd_theme>=1.0.0,<2.0.0', 'sphinxcontrib-
-bibtex>=2.5.0,<3.0.0', 'sphinxcontrib-contentui>=0.2.5,<0.3.0',
+'black>=22.3,<23.0', 'deprecation>=2.1.0,<3.0.0', 'ducc0>=0.25.0,<0.26.0',
+'flake8>=3.7,<4.0', 'h5py==3.4', 'healpy>=1.15.0,<2.0.0', 'jinja2>=3.0,<4.0',
+'jplephem>=2.14,<3.0', 'katex>=0.0.4,<0.0.5', 'markdown-
+katex>=202006.1021,<202007.0', 'markdown>=3.2,<4.0', 'matplotlib>=3.1,<4.0',
+'numba>=0.55,<0.56', 'numpy>=1.21,<2.0', 'pre-commit>=2.15.0,<3.0.0',
+'pybind11>=2.5.0,<3.0.0', 'pyperclip>=1.8.1,<2.0.0', 'pysm3>=3.3.0,<4.0.0',
+'pytest>=5.3,<6.0', 'pyyaml>=5.3.1,<6.0.0', 'requests>=2.24.0,<3.0.0',
+'rich>=11.0.0,<12.0.0', 'sphinx>=5.1,<6.0', 'sphinx_rtd_theme>=1.0.0,<2.0.0',
+'sphinxcontrib-bibtex>=2.5.0,<3.0.0', 'sphinxcontrib-contentui>=0.2.5,<0.3.0',
 'sphinxcontrib.asciinema>=0.3.4,<0.4.0', 'toast-cmb>=2.3.14,<3.0.0',
 'tomlkit>=0.11.2,<0.12.0'] extras_require = \ {'jupyter':
 ['jupyter>=1.0,<2.0'], 'mpi': ['mpi4py>=3.0,<4.0']} setup_kwargs = { 'name':
-'litebird-sim', 'version': '0.8.0', 'description': 'Simulation tools for the
+'litebird-sim', 'version': '0.9.0', 'description': 'Simulation tools for the
 LiteBIRD experiment', 'long_description': '\n\n\n\n\n[![Stable](https://
 img.shields.io/badge/docs-stable-blue.svg)](https://litebird-
 sim.readthedocs.io/en/master/)\n[![Tests](https://github.com/litebird/
 litebird_sim/workflows/Tests/badge.svg?branch=master&event=push)](https://
 github.com/litebird/litebird_sim/
 actions?query=workflow%3ATests+branch%3Amaster)\n[![Build Status](https://
 ci.appveyor.com/api/projects/status/github/litebird/litebird-sim?svg=true)]
@@ -47,15 +47,17 @@
 www.python.org)\n- [Poetry](https://python-poetry.org/)\n- [NumPy](https://
 numpy.org)\n- [Astropy](https://www.astropy.org)\n- [Healpix](https://
 healpix.jpl.nasa.gov)\n- [Sphinx](https://www.sphinx-doc.org/en/master/)\n-
 [Numba](https://numba.pydata.org/)\n- [ducc](https://github.com/litebird/
 ducc)\n\n\n\n## Getting Started\n\nRefer to the\n[documentation](https://
 litebird-sim.readthedocs.io/en/master/installation.html)\nto learn how to
 install the LiteBIRD simulation framework on your\ncomputer or on a HPC
-cluster.\n\n\n\n## Usage\n\nThe documentation is available online at\n
+cluster.\n\n\n\n## Usage\n\nAn example notebook is avalable [here](https://
+github.com/litebird/litebird_sim/blob/master/notebooks/
+litebird_sim_example.ipynb). \n\nThe documentation is available online at\n
 [litebird-sim.readthedocs.io/en/master/](https://litebird-sim.readthedocs.io/
 en/master/).\n\nTo create a local copy of the documentation, make sure you
 ran\n`poetry` with the flag `--extras=docs`, then run the following\ncommand:
 \n\n- Linux or Mac OS X:\n ```\n ./refresh_docs.sh\n ```\n\n- Windows:\n ```\n
 poetry shell\n cd docs\n make.bat html\n ```\n\n\n\n## Roadmap\n\nSee the [open
 issues](https://github.com/litebird/litebird_sim/issues)\nfor a list of
 proposed features (and known issues).\n\n\n\n## Contributing\n\nIf you are part
@@ -72,11 +74,12 @@
 litebird_sim](https://github.com/litebird/litebird_sim)\n\n\n\n\n## How to cite
 this code\n\nTODO!\n\n\n\n\n[issues-shield]: https://img.shields.io/github/
 issues/litebird/litebird_sim?style=flat-square\n[issues-url]: https://
 github.com/litebird/litebird_sim/issues\n[license-shield]: https://
 img.shields.io/github/license/litebird/litebird_sim.svg?style=flat-square\n
 [license-url]: https://github.com/litebird/litebird_sim/blob/master/
 LICENSE\n\n\n[product-screenshot]: images/screenshot.png\n', 'author': 'The
-LiteBIRD Simulation Team', 'author_email': None, 'maintainer': None,
-'maintainer_email': None, 'url': None, 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'extras_require':
-extras_require, 'python_requires': '>=3.7.1,<3.10', } setup(**setup_kwargs)
+LiteBIRD Simulation Team', 'author_email': 'None', 'maintainer': 'None',
+'maintainer_email': 'None', 'url': 'None', 'packages': packages,
+'package_data': package_data, 'install_requires': install_requires,
+'extras_require': extras_require, 'python_requires': '>=3.7.1,<3.10', } setup
+(**setup_kwargs)
```

### Comparing `litebird_sim-0.8.0/PKG-INFO` & `litebird_sim-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: litebird-sim
-Version: 0.8.0
+Version: 0.9.0
 Summary: Simulation tools for the LiteBIRD experiment
 License: GPL3
 Author: The LiteBIRD Simulation Team
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: jupyter
 Provides-Extra: mpi
 Requires-Dist: PyGithub (>=1.53,<2.0)
 Requires-Dist: asciimatics (>=1.12.0,<2.0.0)
 Requires-Dist: astropy (>=4.3,<5.0)
 Requires-Dist: black (>=22.3,<23.0)
+Requires-Dist: deprecation (>=2.1.0,<3.0.0)
 Requires-Dist: ducc0 (>=0.25.0,<0.26.0)
 Requires-Dist: flake8 (>=3.7,<4.0)
 Requires-Dist: h5py (==3.4)
 Requires-Dist: healpy (>=1.15.0,<2.0.0)
 Requires-Dist: jinja2 (>=3.0,<4.0)
 Requires-Dist: jplephem (>=2.14,<3.0)
-Requires-Dist: jupyter (>=1.0,<2.0); extra == "jupyter"
+Requires-Dist: jupyter (>=1.0,<2.0) ; extra == "jupyter"
 Requires-Dist: jupyterlab (>=1.2,<2.0)
 Requires-Dist: katex (>=0.0.4,<0.0.5)
 Requires-Dist: markdown (>=3.2,<4.0)
 Requires-Dist: markdown-katex (>=202006.1021,<202007.0)
 Requires-Dist: matplotlib (>=3.1,<4.0)
-Requires-Dist: mpi4py (>=3.0,<4.0); extra == "mpi"
+Requires-Dist: mpi4py (>=3.0,<4.0) ; extra == "mpi"
 Requires-Dist: numba (>=0.55,<0.56)
 Requires-Dist: numpy (>=1.21,<2.0)
 Requires-Dist: pre-commit (>=2.15.0,<3.0.0)
 Requires-Dist: pybind11 (>=2.5.0,<3.0.0)
 Requires-Dist: pyperclip (>=1.8.1,<2.0.0)
 Requires-Dist: pysm3 (>=3.3.0,<4.0.0)
 Requires-Dist: pytest (>=5.3,<6.0)
@@ -140,14 +141,16 @@
 to learn how to install the LiteBIRD simulation framework on your
 computer or on a HPC cluster.
 
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
+An example notebook is avalable [here](https://github.com/litebird/litebird_sim/blob/master/notebooks/litebird_sim_example.ipynb). 
+
 The documentation is available online at
 [litebird-sim.readthedocs.io/en/master/](https://litebird-sim.readthedocs.io/en/master/).
 
 To create a local copy of the documentation, make sure you ran
 `poetry` with the flag `--extras=docs`, then run the following
 command:
```

#### html2text {}

```diff
@@ -1,36 +1,37 @@
-Metadata-Version: 2.1 Name: litebird-sim Version: 0.8.0 Summary: Simulation
+Metadata-Version: 2.1 Name: litebird-sim Version: 0.9.0 Summary: Simulation
 tools for the LiteBIRD experiment License: GPL3 Author: The LiteBIRD Simulation
 Team Requires-Python: >=3.7.1,<3.10 Classifier: License :: Other/Proprietary
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: jupyter Provides-Extra: mpi Requires-Dist: PyGithub
 (>=1.53,<2.0) Requires-Dist: asciimatics (>=1.12.0,<2.0.0) Requires-Dist:
-astropy (>=4.3,<5.0) Requires-Dist: black (>=22.3,<23.0) Requires-Dist: ducc0
-(>=0.25.0,<0.26.0) Requires-Dist: flake8 (>=3.7,<4.0) Requires-Dist: h5py
-(==3.4) Requires-Dist: healpy (>=1.15.0,<2.0.0) Requires-Dist: jinja2
-(>=3.0,<4.0) Requires-Dist: jplephem (>=2.14,<3.0) Requires-Dist: jupyter
-(>=1.0,<2.0); extra == "jupyter" Requires-Dist: jupyterlab (>=1.2,<2.0)
-Requires-Dist: katex (>=0.0.4,<0.0.5) Requires-Dist: markdown (>=3.2,<4.0)
-Requires-Dist: markdown-katex (>=202006.1021,<202007.0) Requires-Dist:
-matplotlib (>=3.1,<4.0) Requires-Dist: mpi4py (>=3.0,<4.0); extra == "mpi"
-Requires-Dist: numba (>=0.55,<0.56) Requires-Dist: numpy (>=1.21,<2.0)
-Requires-Dist: pre-commit (>=2.15.0,<3.0.0) Requires-Dist: pybind11
-(>=2.5.0,<3.0.0) Requires-Dist: pyperclip (>=1.8.1,<2.0.0) Requires-Dist: pysm3
-(>=3.3.0,<4.0.0) Requires-Dist: pytest (>=5.3,<6.0) Requires-Dist: pyyaml
-(>=5.3.1,<6.0.0) Requires-Dist: requests (>=2.24.0,<3.0.0) Requires-Dist: rich
-(>=11.0.0,<12.0.0) Requires-Dist: sphinx (>=5.1,<6.0) Requires-Dist:
-sphinx_rtd_theme (>=1.0.0,<2.0.0) Requires-Dist: sphinxcontrib-bibtex
-(>=2.5.0,<3.0.0) Requires-Dist: sphinxcontrib-contentui (>=0.2.5,<0.3.0)
-Requires-Dist: sphinxcontrib.asciinema (>=0.3.4,<0.4.0) Requires-Dist: toast-
-cmb (>=2.3.14,<3.0.0) Requires-Dist: tomlkit (>=0.11.2,<0.12.0) Description-
-Content-Type: text/markdown    [![Stable](https://img.shields.io/badge/docs-
-stable-blue.svg)](https://litebird-sim.readthedocs.io/en/master/) [![Tests]
-(https://github.com/litebird/litebird_sim/workflows/Tests/
-badge.svg?branch=master&event=push)](https://github.com/litebird/litebird_sim/
+astropy (>=4.3,<5.0) Requires-Dist: black (>=22.3,<23.0) Requires-Dist:
+deprecation (>=2.1.0,<3.0.0) Requires-Dist: ducc0 (>=0.25.0,<0.26.0) Requires-
+Dist: flake8 (>=3.7,<4.0) Requires-Dist: h5py (==3.4) Requires-Dist: healpy
+(>=1.15.0,<2.0.0) Requires-Dist: jinja2 (>=3.0,<4.0) Requires-Dist: jplephem
+(>=2.14,<3.0) Requires-Dist: jupyter (>=1.0,<2.0) ; extra == "jupyter"
+Requires-Dist: jupyterlab (>=1.2,<2.0) Requires-Dist: katex (>=0.0.4,<0.0.5)
+Requires-Dist: markdown (>=3.2,<4.0) Requires-Dist: markdown-katex
+(>=202006.1021,<202007.0) Requires-Dist: matplotlib (>=3.1,<4.0) Requires-Dist:
+mpi4py (>=3.0,<4.0) ; extra == "mpi" Requires-Dist: numba (>=0.55,<0.56)
+Requires-Dist: numpy (>=1.21,<2.0) Requires-Dist: pre-commit (>=2.15.0,<3.0.0)
+Requires-Dist: pybind11 (>=2.5.0,<3.0.0) Requires-Dist: pyperclip
+(>=1.8.1,<2.0.0) Requires-Dist: pysm3 (>=3.3.0,<4.0.0) Requires-Dist: pytest
+(>=5.3,<6.0) Requires-Dist: pyyaml (>=5.3.1,<6.0.0) Requires-Dist: requests
+(>=2.24.0,<3.0.0) Requires-Dist: rich (>=11.0.0,<12.0.0) Requires-Dist: sphinx
+(>=5.1,<6.0) Requires-Dist: sphinx_rtd_theme (>=1.0.0,<2.0.0) Requires-Dist:
+sphinxcontrib-bibtex (>=2.5.0,<3.0.0) Requires-Dist: sphinxcontrib-contentui
+(>=0.2.5,<0.3.0) Requires-Dist: sphinxcontrib.asciinema (>=0.3.4,<0.4.0)
+Requires-Dist: toast-cmb (>=2.3.14,<3.0.0) Requires-Dist: tomlkit
+(>=0.11.2,<0.12.0) Description-Content-Type: text/markdown    [![Stable](https:
+//img.shields.io/badge/docs-stable-blue.svg)](https://litebird-
+sim.readthedocs.io/en/master/) [![Tests](https://github.com/litebird/
+litebird_sim/workflows/Tests/badge.svg?branch=master&event=push)](https://
+github.com/litebird/litebird_sim/
 actions?query=workflow%3ATests+branch%3Amaster) [![Build Status](https://
 ci.appveyor.com/api/projects/status/github/litebird/litebird-sim?svg=true)]
 (https://ci.appveyor.com/project/litebird/litebird-sim) [![Issues][issues-
 shield]][issues-url] [![GPL3 License][license-shield]][license-url]
                                     [Logo]
                     **** LiteBIRD Simulation Framework ****
  Main repository of the LiteBIRD Simulation Framework, a set of Python modules
@@ -48,24 +49,26 @@
 (https://www.python.org) - [Poetry](https://python-poetry.org/) - [NumPy]
 (https://numpy.org) - [Astropy](https://www.astropy.org) - [Healpix](https://
 healpix.jpl.nasa.gov) - [Sphinx](https://www.sphinx-doc.org/en/master/) -
 [Numba](https://numba.pydata.org/) - [ducc](https://github.com/litebird/ducc)
 ## Getting Started Refer to the [documentation](https://litebird-
 sim.readthedocs.io/en/master/installation.html) to learn how to install the
 LiteBIRD simulation framework on your computer or on a HPC cluster.  ## Usage
-The documentation is available online at [litebird-sim.readthedocs.io/en/
-master/](https://litebird-sim.readthedocs.io/en/master/). To create a local
-copy of the documentation, make sure you ran `poetry` with the flag `--
-extras=docs`, then run the following command: - Linux or Mac OS X: ``` ./
-refresh_docs.sh ``` - Windows: ``` poetry shell cd docs make.bat html ```  ##
-Roadmap See the [open issues](https://github.com/litebird/litebird_sim/issues)
-for a list of proposed features (and known issues).  ## Contributing If you are
-part of the LiteBIRD collaboration and have something that might fit in this
-framework, you're encouraged to contact us! Any contributions you make are
-**greatly appreciated**. 1. Read [CONTRIBUTING.md](https://github.com/litebird/
+An example notebook is avalable [here](https://github.com/litebird/
+litebird_sim/blob/master/notebooks/litebird_sim_example.ipynb). The
+documentation is available online at [litebird-sim.readthedocs.io/en/master/]
+(https://litebird-sim.readthedocs.io/en/master/). To create a local copy of the
+documentation, make sure you ran `poetry` with the flag `--extras=docs`, then
+run the following command: - Linux or Mac OS X: ``` ./refresh_docs.sh ``` -
+Windows: ``` poetry shell cd docs make.bat html ```  ## Roadmap See the [open
+issues](https://github.com/litebird/litebird_sim/issues) for a list of proposed
+features (and known issues).  ## Contributing If you are part of the LiteBIRD
+collaboration and have something that might fit in this framework, you're
+encouraged to contact us! Any contributions you make are **greatly
+appreciated**. 1. Read [CONTRIBUTING.md](https://github.com/litebird/
 litebird_sim/blob/master/CONTRIBUTING.md) 2. Fork the project 3. Create your
 feature branch (`git checkout -b feature/AmazingFeature`) 4. Commit your
 changes (`git commit -m 'Add some AmazingFeature'`) 5. Push to the Branch (`git
 push origin feature/AmazingFeature`) 6. Open a Pull Request  ## License
 Distributed under the [GPL3 License][license-url].  ## Contact LiteBIRD
 Simulation Team - litebird_pipe@db.ipmu.jp Project Link: [https://github.com/
 litebird/litebird_sim](https://github.com/litebird/litebird_sim)  ## How to
```

