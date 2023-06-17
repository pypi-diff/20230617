# Comparing `tmp/spectrochempy-0.6.5.tar.gz` & `tmp/spectrochempy-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrochempy-0.6.5.tar", last modified: Mon Jun  5 21:34:28 2023, max compression
+gzip compressed data, was "spectrochempy-0.6.6.tar", last modified: Sat Jun 17 10:08:33 2023, max compression
```

## Comparing `spectrochempy-0.6.5.tar` & `spectrochempy-0.6.6.tar`

### file list

```diff
@@ -1,284 +1,360 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.175764 spectrochempy-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/.codeclimate.yml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/.codespellrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.139763 spectrochempy-0.6.5/.conda/
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/.conda/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18144 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    21393 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.139763 spectrochempy-0.6.5/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/LICENSES/NMRGLUE_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/LICENSES/NNMF_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/LICENSES/PACKAGING_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/LICENSES/PANDAS_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/LICENSES/TRAITTYPES_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-05 21:34:28.175764 spectrochempy-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/environment_dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/environment_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.139763 spectrochempy-0.6.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/requirements/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/requirements/requirements_test.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.139763 spectrochempy-0.6.5/scp_data/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.139763 spectrochempy-0.6.5/scp_data/databases/
--rw-r--r--   0 runner    (1001) docker     (123)    26810 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/databases/isotopes.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.147763 spectrochempy-0.6.5/scp_data/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    38040 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/Felipa-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/Humor-Sans.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/LICENSE_felipa.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/LICENSE_victormono.txt
--rw-r--r--   0 runner    (1001) docker     (123)   157048 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   197120 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   164392 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-BoldOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150324 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   184764 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   156852 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-ExtraLightOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188172 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150888 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188268 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   157596 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-LightOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   153808 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   194336 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161360 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-MediumOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   158228 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-Oblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   151576 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   155276 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   193176 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161200 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-SemiBoldOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150284 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188288 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-ThinItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   157184 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/VictorMono-ThinOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105316 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/fonts/comic-sans-ms.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.147763 spectrochempy-0.6.5/scp_data/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/stylesheets/grayscale.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/stylesheets/notebook.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/stylesheets/paper.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/stylesheets/poster.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/stylesheets/sans.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/stylesheets/scpy.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/stylesheets/serif.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scp_data/stylesheets/talk.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.151764 spectrochempy-0.6.5/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scripts/checkindex.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/scripts/validate_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-05 21:34:28.175764 spectrochempy-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.151764 spectrochempy-0.6.5/spectrochempy/
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.151764 spectrochempy-0.6.5/spectrochempy/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71573 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/efa.py
--rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/fast_ica.py
--rw-r--r--   0 runner    (1001) docker     (123)    35188 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/iris.py
--rw-r--r--   0 runner    (1001) docker     (123)    59491 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/kinetic_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/linearregression.py
--rw-r--r--   0 runner    (1001) docker     (123)    49016 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/mcrals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/nmf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.155763 spectrochempy-0.6.5/spectrochempy/analysis/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/optimize/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9926 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/optimize/_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/optimize/_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    36669 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/optimize/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    22461 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/pca.py
--rw-r--r--   0 runner    (1001) docker     (123)    13470 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/peakfinding.py
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/pls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21106 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/simplisma.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/analysis/svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.155763 spectrochempy-0.6.5/spectrochempy/application/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/application/_check_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    32639 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/application/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/application/datadir.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/application/general_preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/application/metaconfigurable.py
--rw-r--r--   0 runner    (1001) docker     (123)    47043 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/application/plot_preferences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.155763 spectrochempy-0.6.5/spectrochempy/core/
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.155763 spectrochempy-0.6.5/spectrochempy/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/common/dialogs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.155763 spectrochempy-0.6.5/spectrochempy/core/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.155763 spectrochempy-0.6.5/spectrochempy/core/dataset/arraymixins/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/arraymixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15122 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/arraymixins/ndio.py
--rw-r--r--   0 runner    (1001) docker     (123)   119937 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/arraymixins/ndmath.py
--rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/arraymixins/ndplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/arraymixins/npy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.159764 spectrochempy-0.6.5/spectrochempy/core/dataset/baseobjects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/baseobjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/baseobjects/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    74571 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/baseobjects/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)    22940 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/baseobjects/ndcomplex.py
--rw-r--r--   0 runner    (1001) docker     (123)    30120 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/coord.py
--rw-r--r--   0 runner    (1001) docker     (123)    37757 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/coordset.py
--rw-r--r--   0 runner    (1001) docker     (123)    53489 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/dataset/nddataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.159764 spectrochempy-0.6.5/spectrochempy/core/plotters/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/plotters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/plotters/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/plotters/multiplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    19702 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/plotters/plot1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    26223 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/plotters/plot2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/plotters/plot3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/plotters/plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.159764 spectrochempy-0.6.5/spectrochempy/core/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15766 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/align.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/autosub.py
--rw-r--r--   0 runner    (1001) docker     (123)    28400 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (123)    19381 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/phasing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/processors/zero_filling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.159764 spectrochempy-0.6.5/spectrochempy/core/project/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/project/abstractproject.py
--rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/project/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.163764 spectrochempy-0.6.5/spectrochempy/core/readers/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    29889 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_carroucell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_jcamp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_labspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_matlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    39297 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_omnic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_opus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_quadera.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_soc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_spc.py
--rw-r--r--   0 runner    (1001) docker     (123)    45418 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_topspin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/readers/read_zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.163764 spectrochempy-0.6.5/spectrochempy/core/script/
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.163764 spectrochempy-0.6.5/spectrochempy/core/units/
--rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/units/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.163764 spectrochempy-0.6.5/spectrochempy/core/writers/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/writers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/writers/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/writers/write_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/writers/write_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/writers/write_jcamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/core/writers/write_matlab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.163764 spectrochempy-0.6.5/spectrochempy/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.167764 spectrochempy-0.6.5/spectrochempy/examples/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_efa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_efa_keller_massart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_fast_ica.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_iris.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_mcrals_chrom1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_mcrals_kinetics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_nmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_pca_iris.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_pca_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_pls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_simplisma.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/analysis/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.167764 spectrochempy-0.6.5/spectrochempy/examples/fitting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/fitting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/fitting/plot_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/fitting/plot_lstsq_single_equation.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/fitting/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.167764 spectrochempy-0.6.5/spectrochempy/examples/nddataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/nddataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/nddataset/plot_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/nddataset/plot_create_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/nddataset/plot_units.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/nddataset/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.167764 spectrochempy-0.6.5/spectrochempy/examples/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/plotting/plot_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/plotting/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.167764 spectrochempy-0.6.5/spectrochempy/examples/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/processing/plot_baseline_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/processing/plot_proc_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/processing/plot_proc_sp.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/processing/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.171764 spectrochempy-0.6.5/spectrochempy/examples/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/project/plot_project.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/project/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.171764 spectrochempy-0.6.5/spectrochempy/examples/read/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/read/plot_generic_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/read/plot_read_IR_from_omnic.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/read/plot_read_IR_from_opus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/read/plot_read_nmr_from_bruker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/read/plot_read_raman_from_labspec.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/read/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/examples/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.171764 spectrochempy-0.6.5/spectrochempy/extern/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/extern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64415 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/extern/nmrglue.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/extern/traittypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/extern/traittypes_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.171764 spectrochempy-0.6.5/spectrochempy/ipython/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/ipython/magics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.175764 spectrochempy-0.6.5/spectrochempy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/citation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/coordrange.py
--rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/decorators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14176 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/fake.py
--rw-r--r--   0 runner    (1001) docker     (123)    23757 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/jsonutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/numutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/optional.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/orderedset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/print.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3422 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)    33071 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    16115 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/utils/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.175764 spectrochempy-0.6.5/spectrochempy/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/widgets/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/widgets/baselinecorrector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-06-05 21:34:09.000000 spectrochempy-0.6.5/spectrochempy/widgets/fileselector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 21:34:28.151764 spectrochempy-0.6.5/spectrochempy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-05 21:34:27.000000 spectrochempy-0.6.5/spectrochempy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-06-05 21:34:28.000000 spectrochempy-0.6.5/spectrochempy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:34:27.000000 spectrochempy-0.6.5/spectrochempy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 21:34:27.000000 spectrochempy-0.6.5/spectrochempy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-05 21:34:27.000000 spectrochempy-0.6.5/spectrochempy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-05 21:34:27.000000 spectrochempy-0.6.5/spectrochempy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.265452 spectrochempy-0.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/.codeclimate.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/.codespellrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.217447 spectrochempy-0.6.6/.conda/
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/.conda/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18144 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    21393 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.221448 spectrochempy-0.6.6/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/LICENSES/NMRGLUE_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/LICENSES/NNMF_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/LICENSES/PACKAGING_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/LICENSES/PANDAS_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/LICENSES/TRAITTYPES_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/LICENSES/WHITTAKER_SMOOTH_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-17 10:08:33.265452 spectrochempy-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/environment_dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/environment_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.221448 spectrochempy-0.6.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/requirements/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/requirements/requirements_test.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.221448 spectrochempy-0.6.6/scp_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.221448 spectrochempy-0.6.6/scp_data/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)    26810 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/databases/isotopes.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.229449 spectrochempy-0.6.6/scp_data/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    38040 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/Felipa-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/Humor-Sans.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/LICENSE_felipa.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/LICENSE_victormono.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   157048 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   197120 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   164392 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-BoldOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150324 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   184764 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   156852 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-ExtraLightOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188172 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150888 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188268 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   157596 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-LightOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   153808 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   194336 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161360 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-MediumOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   158228 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   151576 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155276 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   193176 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161200 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-SemiBoldOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150284 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188288 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-ThinItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   157184 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/VictorMono-ThinOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105316 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/fonts/comic-sans-ms.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.229449 spectrochempy-0.6.6/scp_data/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/stylesheets/grayscale.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/stylesheets/notebook.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/stylesheets/paper.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/stylesheets/poster.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/stylesheets/sans.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/stylesheets/scpy.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/stylesheets/serif.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scp_data/stylesheets/talk.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.229449 spectrochempy-0.6.6/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scripts/checkindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/scripts/validate_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-17 10:08:33.265452 spectrochempy-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.229449 spectrochempy-0.6.6/spectrochempy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.233449 spectrochempy-0.6.6/spectrochempy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.233449 spectrochempy-0.6.6/spectrochempy/analysis/_base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53764 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/_base/_analysisbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.233449 spectrochempy-0.6.6/spectrochempy/analysis/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/baseline/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39539 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/baseline/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/baseline/baseline_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/baseline/baselineutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.233449 spectrochempy-0.6.6/spectrochempy/analysis/crossdecomposition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/crossdecomposition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/crossdecomposition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/crossdecomposition/pls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.233449 spectrochempy-0.6.6/spectrochempy/analysis/curvefitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/curvefitting/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9926 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/curvefitting/_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/curvefitting/_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/curvefitting/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/curvefitting/linearregression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36742 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/curvefitting/optimize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.237450 spectrochempy-0.6.6/spectrochempy/analysis/decomposition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/decomposition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/decomposition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8268 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/decomposition/efa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11441 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/decomposition/fast_ica.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35222 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/decomposition/iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49037 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/decomposition/mcrals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9303 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/decomposition/nmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22562 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/decomposition/pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21127 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/decomposition/simplisma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/decomposition/svd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.237450 spectrochempy-0.6.6/spectrochempy/analysis/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/integration/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/integration/integrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.237450 spectrochempy-0.6.6/spectrochempy/analysis/kinetic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/kinetic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/kinetic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59505 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/kinetic/kineticutilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.237450 spectrochempy-0.6.6/spectrochempy/analysis/peakfinding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/peakfinding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/peakfinding/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13470 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/peakfinding/peakfinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/analysis/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.237450 spectrochempy-0.6.6/spectrochempy/application/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/application/_check_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32609 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/application/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/application/datadir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/application/general_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47037 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/application/plot_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/application/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.237450 spectrochempy-0.6.6/spectrochempy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.237450 spectrochempy-0.6.6/spectrochempy/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/common/dialogs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.241450 spectrochempy-0.6.6/spectrochempy/core/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.241450 spectrochempy-0.6.6/spectrochempy/core/dataset/arraymixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/arraymixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15237 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/arraymixins/ndio.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119944 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/arraymixins/ndmath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27604 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/arraymixins/ndplot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.241450 spectrochempy-0.6.6/spectrochempy/core/dataset/baseobjects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/baseobjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/baseobjects/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75007 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/baseobjects/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22940 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/baseobjects/ndcomplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30311 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/coord.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37757 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/coordset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53490 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/dataset/nddataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.241450 spectrochempy-0.6.6/spectrochempy/core/plotters/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/plotters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/plotters/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/plotters/multiplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21204 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/plotters/plot1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26223 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/plotters/plot2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/plotters/plot3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/plotters/plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.241450 spectrochempy-0.6.6/spectrochempy/core/project/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/project/abstractproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/project/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.245450 spectrochempy-0.6.6/spectrochempy/core/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29953 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_carroucell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11381 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_jcamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_labspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_matlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39331 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_omnic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_opus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_quadera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_soc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17013 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_spc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45425 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_topspin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/readers/read_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.245450 spectrochempy-0.6.6/spectrochempy/core/script/
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.245450 spectrochempy-0.6.6/spectrochempy/core/units/
+-rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.245450 spectrochempy-0.6.6/spectrochempy/core/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/writers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/writers/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/writers/write_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/writers/write_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/writers/write_jcamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/core/writers/write_matlab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.245450 spectrochempy-0.6.6/spectrochempy/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.245450 spectrochempy-0.6.6/spectrochempy/examples/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.249451 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_efa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_efa_keller_massart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_fast_ica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_mcrals_chrom1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_mcrals_kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_nmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_pca_iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_pca_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_simplisma.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.249451 spectrochempy-0.6.6/spectrochempy/examples/analysis/b_crossdecomposition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/b_crossdecomposition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/b_crossdecomposition/plot_pls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/b_crossdecomposition/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.249451 spectrochempy-0.6.6/spectrochempy/examples/analysis/c_curvefitting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/c_curvefitting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/c_curvefitting/plot_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/c_curvefitting/plot_lstsq_single_equation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/c_curvefitting/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.249451 spectrochempy-0.6.6/spectrochempy/examples/analysis/d_baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/d_baseline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/d_baseline/plot_baseline_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/d_baseline/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/analysis/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.249451 spectrochempy-0.6.6/spectrochempy/examples/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.249451 spectrochempy-0.6.6/spectrochempy/examples/core/a_nddataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/a_nddataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/a_nddataset/plot_a_create_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/a_nddataset/plot_b_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/a_nddataset/plot_c_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/a_nddataset/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.249451 spectrochempy-0.6.6/spectrochempy/examples/core/b_units/
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/b_units/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.253451 spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/plot_generic_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/plot_read_IR_from_omnic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/plot_read_IR_from_opus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/plot_read_nmr_from_bruker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/plot_read_raman_from_labspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.253451 spectrochempy-0.6.6/spectrochempy/examples/core/d_plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/d_plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/d_plotting/plot_plot_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/d_plotting/plot_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/d_plotting/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.253451 spectrochempy-0.6.6/spectrochempy/examples/core/e_project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/e_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/e_project/plot_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/e_project/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/core/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.253451 spectrochempy-0.6.6/spectrochempy/examples/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.253451 spectrochempy-0.6.6/spectrochempy/examples/processing/apodization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/apodization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/apodization/plot_proc_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/apodization/plot_proc_sp.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/apodization/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.253451 spectrochempy-0.6.6/spectrochempy/examples/processing/denoising/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/denoising/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/denoising/plot_denoising.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/denoising/plot_despike.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/denoising/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.253451 spectrochempy-0.6.6/spectrochempy/examples/processing/filtering/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/filtering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/filtering/plot_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/filtering/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.257452 spectrochempy-0.6.6/spectrochempy/examples/processing/raman/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/raman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/raman/plot_raman_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/raman/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/examples/processing/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.257452 spectrochempy-0.6.6/spectrochempy/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/extern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64415 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/extern/nmrglue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/extern/traittypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/extern/traittypes_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/extern/whittaker_smooth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.257452 spectrochempy-0.6.6/spectrochempy/ipython/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/ipython/magics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.257452 spectrochempy-0.6.6/spectrochempy/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.257452 spectrochempy-0.6.6/spectrochempy/processing/_base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/_base/_processingbase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.257452 spectrochempy-0.6.6/spectrochempy/processing/alignement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/alignement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15773 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/alignement/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/alignement/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.257452 spectrochempy-0.6.6/spectrochempy/processing/fft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/fft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/fft/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24702 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/fft/apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19382 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/fft/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23167 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/fft/phasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/fft/shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/fft/zero_filling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.257452 spectrochempy-0.6.6/spectrochempy/processing/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/filter/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/filter/denoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/filter/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.261452 spectrochempy-0.6.6/spectrochempy/processing/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/interpolation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/interpolation/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/interpolation/interpolate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.261452 spectrochempy-0.6.6/spectrochempy/processing/transformation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/transformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/transformation/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/transformation/autosub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/transformation/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/processing/transformation/npy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/structure.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.265452 spectrochempy-0.6.6/spectrochempy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14466 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/baseconfigurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/citation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/coordrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18013 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/decorators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14507 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8977 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23764 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/jsonutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/metaconfigurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/numutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/optional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/orderedset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/print.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3422 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33071 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/timeutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16115 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/utils/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.265452 spectrochempy-0.6.6/spectrochempy/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/widgets/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/widgets/baselinecorrector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-06-17 10:08:11.000000 spectrochempy-0.6.6/spectrochempy/widgets/fileselector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:08:33.233449 spectrochempy-0.6.6/spectrochempy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-17 10:08:32.000000 spectrochempy-0.6.6/spectrochempy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-06-17 10:08:33.000000 spectrochempy-0.6.6/spectrochempy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 10:08:32.000000 spectrochempy-0.6.6/spectrochempy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 10:08:32.000000 spectrochempy-0.6.6/spectrochempy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-17 10:08:32.000000 spectrochempy-0.6.6/spectrochempy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-17 10:08:32.000000 spectrochempy-0.6.6/spectrochempy.egg-info/top_level.txt
```

### Comparing `spectrochempy-0.6.5/.codeclimate.yml` & `spectrochempy-0.6.6/.codeclimate.yml`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/.conda/meta.yaml` & `spectrochempy-0.6.6/.conda/meta.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -28,30 +28,30 @@
     - python >=3.8
     - setuptools
     - setuptools_scm
   run:
     - python
 
     # specific dependencies
-    - quadprog
     - brukeropusreader
+    - quadprog
     - quaternion
 
     # dependencies for the core package
     - cffconvert
     - colorama
     - dill
     - docrep
     - ipython
     - jinja2
     - matplotlib
     - numba
     - numpy
     - numpydoc>=1.2
-    - pint
+    - pint>=0.20
     - pytz
     - requests
     - scipy
     - tqdm
     - traitlets
     - scikit-learn
     - xlrd
@@ -59,20 +59,25 @@
 
     # dependencies needed mainly for install and a bit more ...
     - setuptools
     - setuptools_scm
     - git
 
     # Jupyter lab
+    - ipywidgets=8.0.4
+    - ipympl
     - jupyterlab
+    - jupyterlab_widgets=3.0.5
+    - jupyter_server=1.23.6
     - nodejs
-    - ipywidgets=8.0.4
     - widgetsnbextension=4.0.5
-    - jupyterlab_widgets=3.0.5
-    - ipympl
+
+    # voila
+    - voila
+    - voila-material
 
 
   test:
     - python  {{ python }}
 
 test:
   script_env:
```

### Comparing `spectrochempy-0.6.5/.gitignore` & `spectrochempy-0.6.6/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 .cache/
 /.pytest_cache/
 
 # Sphinx documentation
 docs/reference/generated
 docs/reference/api.rst
 build/
-docs/gallery/
+gallery/
 docs/savefig/
 dist/
 build/
 
 # tests
 tests/figures
 /tests_extern_packages/
```

### Comparing `spectrochempy-0.6.5/.pre-commit-config.yaml` & `spectrochempy-0.6.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/.pylintrc` & `spectrochempy-0.6.6/.pylintrc`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/.zenodo.json` & `spectrochempy-0.6.6/.zenodo.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'publication_date'": "'2023-06-17'", "'version'": "'0.6.6'"}*

```diff
@@ -50,12 +50,12 @@
         "raman",
         "raman-spectra",
         "raman-spectroscopy",
         "spectroscopy",
         "uv-vis"
     ],
     "license": "CECILL-B",
-    "publication_date": "2023-06-05",
+    "publication_date": "2023-06-17",
     "title": "SpectroChemPy",
     "upload_type": "software",
-    "version": "0.6.5"
+    "version": "0.6.6"
 }
```

### Comparing `spectrochempy-0.6.5/CITATION.cff` & `spectrochempy-0.6.6/CITATION.cff`

 * *Files 9% similar despite different names*

```diff
@@ -11,20 +11,20 @@
   orcid: https://orcid.org/0000-0002-9579-8910
 - affiliation: "ENSICAEN, Universit\xE9 de Caen, CNRS (Laboratoire Catalyse et Spectrochimie)"
   email: christian.fernandez@ensicaen.fr
   family-names: Fernandez
   given-names: Christian
   orcid: https://orcid.org/0000-0002-5476-3148
 cff-version: 1.2.0
-date-released: '2023-06-05'
+date-released: '2023-06-17'
 identifiers:
 - description: Persistent identifier for all versions of SpectroChemPy
   type: doi
   value: 10.5281/zenodo.3823841
 license: CECILL-B
 message: If you use this software, please cite it using the metadata from this file.
 repository-code: https://github.com/spectrochempy/spectrochempy
 title: SpectroChemPy, a framework for processing, analyzing and modeling spectroscopic
   data for chemistry with Python
 type: software
 url: https://www.spectrochempy.fr
-version: 0.6.5
+version: 0.6.6
```

### Comparing `spectrochempy-0.6.5/Dockerfile` & `spectrochempy-0.6.6/Dockerfile`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/LICENSE` & `spectrochempy-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/LICENSES/NMRGLUE_LICENSE.rst` & `spectrochempy-0.6.6/LICENSES/NMRGLUE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/LICENSES/NNMF_LICENSE.rst` & `spectrochempy-0.6.6/LICENSES/NNMF_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/LICENSES/PACKAGING_LICENSE.rst` & `spectrochempy-0.6.6/LICENSES/PACKAGING_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/LICENSES/PANDAS_LICENSE.rst` & `spectrochempy-0.6.6/LICENSES/PANDAS_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/LICENSES/TRAITTYPES_LICENSE.rst` & `spectrochempy-0.6.6/LICENSES/TRAITTYPES_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/PKG-INFO` & `spectrochempy-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrochempy
-Version: 0.6.5
+Version: 0.6.6
 Summary: Processing, analysis and modelling Spectroscopic data for Chemistry with Python
 Home-page: https://www.spectrochempy.fr
 Author: Arnaud Travert & Christian Fernandez
 Author-email: contact@spectrochempy.fr
 Maintainer: C. Fernandez
 Maintainer-email: christian.fernandez@ensicaen.fr
 License: CECILL-B
```

### Comparing `spectrochempy-0.6.5/README.md` & `spectrochempy-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/environment.yml` & `spectrochempy-0.6.6/environment.yml`

 * *Files 9% similar despite different names*

```diff
@@ -17,30 +17,30 @@
 channels:
     - conda-forge
     - spectrocat
     - defaults
 
 dependencies:
     # specific dependencies
-    - quadprog
     - brukeropusreader
+    - quadprog
     - quaternion
 
     # dependencies for the core package
     - cffconvert
     - colorama
     - dill
     - docrep
     - ipython
     - jinja2
     - matplotlib
     - numba
     - numpy
     - numpydoc>=1.2
-    - pint
+    - pint>=0.20
     - pytz
     - requests
     - scipy
     - tqdm
     - traitlets
     - scikit-learn
     - xlrd
@@ -48,13 +48,18 @@
 
     # dependencies needed mainly for install and a bit more ...
     - setuptools
     - setuptools_scm
     - git
 
     # Jupyter lab
+    - ipywidgets=8.0.4
+    - ipympl
     - jupyterlab
+    - jupyterlab_widgets=3.0.5
+    - jupyter_server=1.23.6
     - nodejs
-    - ipywidgets=8.0.4
     - widgetsnbextension=4.0.5
-    - jupyterlab_widgets=3.0.5
-    - ipympl
+
+    # voila
+    - voila
+    - voila-material
```

### Comparing `spectrochempy-0.6.5/environment_dev.yml` & `spectrochempy-0.6.6/environment_dev.yml`

 * *Files 10% similar despite different names*

```diff
@@ -17,30 +17,30 @@
 channels:
     - conda-forge
     - spectrocat
     - defaults
 
 dependencies:
     # specific dependencies
-    - quadprog
     - brukeropusreader
+    - quadprog
     - quaternion
 
     # dependencies for the core package
     - cffconvert
     - colorama
     - dill
     - docrep
     - ipython
     - jinja2
     - matplotlib
     - numba
     - numpy
     - numpydoc>=1.2
-    - pint
+    - pint>=0.20
     - pytz
     - requests
     - scipy
     - tqdm
     - traitlets
     - scikit-learn
     - xlrd
@@ -48,20 +48,25 @@
 
     # dependencies needed mainly for install and a bit more ...
     - setuptools
     - setuptools_scm
     - git
 
     # Jupyter lab
+    - ipywidgets=8.0.4
+    - ipympl
     - jupyterlab
+    - jupyterlab_widgets=3.0.5
+    - jupyter_server=1.23.6
     - nodejs
-    - ipywidgets=8.0.4
     - widgetsnbextension=4.0.5
-    - jupyterlab_widgets=3.0.5
-    - ipympl
+
+    # voila
+    - voila
+    - voila-material
 
     # TEST dependencies
     # ----------------
     - coverage
     - pytest
     - pytest-doctestplus
     - pytest-flake8
@@ -70,26 +75,29 @@
     - pep8-naming
     - xarray
 
     # DEV dependencies
     # ----------------
     # From here, the dependencies are essentially for development.
     # They should not be necessary for the user of  spectrochempy.
-    - scikit-image
+    - anaconda-client
     - black
-    - pre-commit
-    - mamba
+    - boa
+    - conda-build
+    - conda-verify
+    - isort
+    - json5
     - jupytext
-    - sphinx=5.3
-    - sphinx_rtd_theme=1.2
-    - autodocsumm
-    - sphinx-gallery
-    - nbsphinx
     - jupyter_sphinx
-    - json5
+    - mamba
+    - nbconvert=7.4.0
+    - nbsphinx
+    - numpydoc>=1.2
+    - pandoc=2.19
+    - pypandoc
+    - pre-commit
+    - scikit-image
+    - sphinx=5.3
     - sphinx-copybutton
+    - sphinx-gallery=0.13
+    - sphinx_rtd_theme=1.2
     - sphinxcontrib-bibtex
-    - pandoc=2.19
-    - conda-build
-    - conda-verify
-    - anaconda-client
-    - numpydoc>=1.2
```

### Comparing `spectrochempy-0.6.5/environment_test.yml` & `spectrochempy-0.6.6/environment_test.yml`

 * *Files 14% similar despite different names*

```diff
@@ -17,30 +17,30 @@
 channels:
     - conda-forge
     - spectrocat
     - defaults
 
 dependencies:
     # specific dependencies
-    - quadprog
     - brukeropusreader
+    - quadprog
     - quaternion
 
     # dependencies for the core package
     - cffconvert
     - colorama
     - dill
     - docrep
     - ipython
     - jinja2
     - matplotlib
     - numba
     - numpy
     - numpydoc>=1.2
-    - pint
+    - pint>=0.20
     - pytz
     - requests
     - scipy
     - tqdm
     - traitlets
     - scikit-learn
     - xlrd
@@ -48,20 +48,25 @@
 
     # dependencies needed mainly for install and a bit more ...
     - setuptools
     - setuptools_scm
     - git
 
     # Jupyter lab
+    - ipywidgets=8.0.4
+    - ipympl
     - jupyterlab
+    - jupyterlab_widgets=3.0.5
+    - jupyter_server=1.23.6
     - nodejs
-    - ipywidgets=8.0.4
     - widgetsnbextension=4.0.5
-    - jupyterlab_widgets=3.0.5
-    - ipympl
+
+    # voila
+    - voila
+    - voila-material
 
     # TEST dependencies
     # ----------------
     - coverage
     - pytest
     - pytest-doctestplus
     - pytest-flake8
```

### Comparing `spectrochempy-0.6.5/requirements/requirements.txt` & `spectrochempy-0.6.6/requirements/requirements.txt`

 * *Files 17% similar despite different names*

```diff
@@ -3,38 +3,41 @@
 # This file is auto-generated from environment.yml file.
 #
 # !!! DO NOT MODIFY !!!
 #
 # See in `environment.yml` for more information.
 #
 # ======================================================================================
-quadprog
 brukeropusreader
+quadprog
 numpy-quaternion
 cffconvert
 colorama
 dill
 docrep
 ipython
 jinja2
 matplotlib
 numba
 numpy
 numpydoc>=1.2
-pint
+pint>=0.20
 pytz
 requests
 scipy
 tqdm
 traitlets
 scikit-learn
 xlrd
 pyyaml
 setuptools
 setuptools_scm
 gitpython
+ipywidgets==8.0.4
+ipympl
 jupyterlab
+jupyterlab_widgets==3.0.5
+jupyter_server==1.23.6
 nodejs
-ipywidgets==8.0.4
 widgetsnbextension==4.0.5
-jupyterlab_widgets==3.0.5
-ipympl
+voila
+voila-material
```

### Comparing `spectrochempy-0.6.5/requirements/requirements_dev.txt` & `spectrochempy-0.6.6/requirements/requirements_dev.txt`

 * *Files 18% similar despite different names*

```diff
@@ -3,62 +3,68 @@
 # This file is auto-generated from environment_dev.yml file.
 #
 # !!! DO NOT MODIFY !!!
 #
 # See in `environment_dev.yml` for more information.
 #
 # ======================================================================================
-quadprog
 brukeropusreader
+quadprog
 numpy-quaternion
 cffconvert
 colorama
 dill
 docrep
 ipython
 jinja2
 matplotlib
 numba
 numpy
 numpydoc>=1.2
-pint
+pint>=0.20
 pytz
 requests
 scipy
 tqdm
 traitlets
 scikit-learn
 xlrd
 pyyaml
 setuptools
 setuptools_scm
 gitpython
+ipywidgets==8.0.4
+ipympl
 jupyterlab
+jupyterlab_widgets==3.0.5
+jupyter_server==1.23.6
 nodejs
-ipywidgets==8.0.4
 widgetsnbextension==4.0.5
-jupyterlab_widgets==3.0.5
-ipympl
+voila
+voila-material
 coverage
 pytest
 pytest-doctestplus
 pytest-flake8
 pytest-mock
 pyfakefs
 pep8-naming
 xarray
-scikit-image
 black
-pre-commit
-mamba
+boa
+isort
+json5
 jupytext
-sphinx==5.3
-sphinx_rtd_theme==1.2
-autodocsumm
-sphinx-gallery
-nbsphinx
 jupyter_sphinx
-json5
+mamba
+nbconvert==7.4.0
+nbsphinx
+numpydoc>=1.2
+pandoc==2.19
+pypandoc
+pre-commit
+scikit-image
+sphinx==5.3
 sphinx-copybutton
+sphinx-gallery==0.13
+sphinx_rtd_theme==1.2
 sphinxcontrib-bibtex
-pandoc==2.19
-numpydoc>=1.2
```

### Comparing `spectrochempy-0.6.5/scp_data/databases/isotopes.csv` & `spectrochempy-0.6.6/scp_data/databases/isotopes.csv`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/Felipa-Regular.ttf` & `spectrochempy-0.6.6/scp_data/fonts/Felipa-Regular.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/Humor-Sans.ttf` & `spectrochempy-0.6.6/scp_data/fonts/Humor-Sans.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/LICENSE_felipa.txt` & `spectrochempy-0.6.6/scp_data/fonts/LICENSE_felipa.txt`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/LICENSE_victormono.txt` & `spectrochempy-0.6.6/scp_data/fonts/LICENSE_victormono.txt`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/VictorMono-Bold.ttf` & `spectrochempy-0.6.6/scp_data/fonts/VictorMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/VictorMono-BoldItalic.ttf` & `spectrochempy-0.6.6/scp_data/fonts/VictorMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/VictorMono-BoldOblique.ttf` & `spectrochempy-0.6.6/scp_data/fonts/VictorMono-BoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/VictorMono-ExtraLight.ttf` & `spectrochempy-0.6.6/scp_data/fonts/VictorMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/VictorMono-ExtraLightItalic.ttf` & `spectrochempy-0.6.6/scp_data/fonts/VictorMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/VictorMono-ExtraLightOblique.ttf` & `spectrochempy-0.6.6/scp_data/fonts/VictorMono-ExtraLightOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/VictorMono-Italic.ttf` & `spectrochempy-0.6.6/scp_data/fonts/VictorMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/VictorMono-Light.ttf` & `spectrochempy-0.6.6/scp_data/fonts/VictorMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/VictorMono-LightItalic.ttf` & `spectrochempy-0.6.6/scp_data/fonts/VictorMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/VictorMono-LightOblique.ttf` & `spectrochempy-0.6.6/scp_data/fonts/VictorMono-LightOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/VictorMono-Medium.ttf` & `spectrochempy-0.6.6/scp_data/fonts/VictorMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/VictorMono-MediumItalic.ttf` & `spectrochempy-0.6.6/scp_data/fonts/VictorMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/VictorMono-MediumOblique.ttf` & `spectrochempy-0.6.6/scp_data/fonts/VictorMono-MediumOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/VictorMono-Oblique.ttf` & `spectrochempy-0.6.6/scp_data/fonts/VictorMono-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/VictorMono-Regular.ttf` & `spectrochempy-0.6.6/scp_data/fonts/VictorMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/VictorMono-SemiBold.ttf` & `spectrochempy-0.6.6/scp_data/fonts/VictorMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/VictorMono-SemiBoldItalic.ttf` & `spectrochempy-0.6.6/scp_data/fonts/VictorMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/VictorMono-SemiBoldOblique.ttf` & `spectrochempy-0.6.6/scp_data/fonts/VictorMono-SemiBoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/VictorMono-Thin.ttf` & `spectrochempy-0.6.6/scp_data/fonts/VictorMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/VictorMono-ThinItalic.ttf` & `spectrochempy-0.6.6/scp_data/fonts/VictorMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/VictorMono-ThinOblique.ttf` & `spectrochempy-0.6.6/scp_data/fonts/VictorMono-ThinOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/fonts/comic-sans-ms.ttf` & `spectrochempy-0.6.6/scp_data/fonts/comic-sans-ms.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/stylesheets/grayscale.mplstyle` & `spectrochempy-0.6.6/scp_data/stylesheets/grayscale.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/stylesheets/notebook.mplstyle` & `spectrochempy-0.6.6/scp_data/stylesheets/notebook.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/stylesheets/sans.mplstyle` & `spectrochempy-0.6.6/scp_data/stylesheets/sans.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/stylesheets/scpy.mplstyle` & `spectrochempy-0.6.6/scp_data/stylesheets/scpy.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scp_data/stylesheets/serif.mplstyle` & `spectrochempy-0.6.6/scp_data/stylesheets/serif.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scripts/checkindex.py` & `spectrochempy-0.6.6/scripts/checkindex.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/scripts/validate_docstrings.py` & `spectrochempy-0.6.6/scripts/validate_docstrings.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/setup.cfg` & `spectrochempy-0.6.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/setup.py` & `spectrochempy-0.6.6/setup.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/__init__.py` & `spectrochempy-0.6.6/spectrochempy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,19 +64,18 @@
 warnings.filterwarnings(action="ignore", module="jupyter")  # , category=UserWarning)
 warnings.filterwarnings(action="ignore", module="pykwalify")  # , category=UserWarning)
 warnings.filterwarnings(action="ignore", module="matplotlib")
 warnings.filterwarnings(action="ignore", category=FutureWarning)
 
 from spectrochempy import api
 from spectrochempy.api import *
-from spectrochempy.core.dataset.coord import Coord
-from spectrochempy.core.dataset.coordset import CoordSet
-from spectrochempy.core.dataset.nddataset import NDDataset
 
 __all__ = api.__all__
 
 
 def __getattr__(name):
     # NDDataset method accessible from the API
+    from spectrochempy.core.dataset.nddataset import NDDataset
+
     if hasattr(NDDataset, name):
         return getattr(NDDataset, name)
     raise AttributeError
```

### Comparing `spectrochempy-0.6.5/spectrochempy/analysis/_base.py` & `spectrochempy-0.6.6/spectrochempy/analysis/_base/_analysisbase.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,272 +4,47 @@
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
 This module implements the base abstract classes to define estimators such as PCA, ...
 """
 
-import inspect
 import logging
 import warnings
-from copy import copy
-from functools import partial, update_wrapper
 
 import matplotlib.pyplot as plt
 import numpy as np
 import traitlets as tr
 from sklearn import linear_model
 
-from spectrochempy.application.metaconfigurable import MetaConfigurable
-from spectrochempy.core import app, set_loglevel
+from spectrochempy.application import app
 from spectrochempy.core.dataset.baseobjects.ndarray import NDArray
-from spectrochempy.core.dataset.coordset import CoordSet
 from spectrochempy.core.dataset.nddataset import NDDataset
 from spectrochempy.extern.traittypes import Array
-from spectrochempy.utils import exceptions
-from spectrochempy.utils.constants import MASKED, NOMASK
-from spectrochempy.utils.decorators import deprecated, preserve_signature
+from spectrochempy.utils.baseconfigurable import BaseConfigurable
+from spectrochempy.utils.decorators import _wrap_ndarray_output_to_nddataset, deprecated
 from spectrochempy.utils.docstrings import _docstring
+from spectrochempy.utils.exceptions import NotFittedError
 from spectrochempy.utils.plots import NBlue, NGreen, NRed
 from spectrochempy.utils.traits import NDDatasetType
 
 
 # ======================================================================================
-# Exceptions for analysis models
-# ======================================================================================
-class NotFittedError(exceptions.SpectroChemPyError):
-    """
-    Exception raised when an analysis estimator is not fitted
-    but one use one of its method.
-
-    Parameters
-    ----------
-    attr : method, optional
-        The method from which the error was issued. In general it is determined
-        automatically.
-    """
-
-    def __init__(self, attr=None):
-        frame = inspect.currentframe().f_back
-        caller = frame.f_code.co_name if attr is None else attr
-        model = frame.f_locals["self"].name
-        message = (
-            f"To use `{caller}` ,  the method `fit` of model `{model}`"
-            f" should be executed first"
-        )
-        super().__init__(message)
-
-
-# ======================================================================================
-# A decorator to transform np.ndarray output from models to NDDataset
-# according to the X (default) and/or Y input
-# ======================================================================================
-class _set_output(object):
-    def __init__(
-        self,
-        method,
-        *args,
-        meta_from="_X",  # the attribute or tuple of attributes from which meta data are taken
-        units="keep",
-        title="keep",
-        typex=None,
-        typey=None,
-        typesingle=None,
-    ):
-        self.method = method
-        update_wrapper(self, method)
-        self.meta_from = meta_from
-        self.units = units
-        self.title = title
-        self.typex = typex
-        self.typey = typey
-        self.typesingle = typesingle
-
-    @preserve_signature
-    def __get__(self, obj, objtype):
-        """Support instance methods."""
-        newfunc = partial(self.__call__, obj)
-        update_wrapper(newfunc, self.method)
-        return newfunc
-
-    def __call__(self, obj, *args, **kwargs):
-
-        from spectrochempy.core.dataset.coord import Coord
-        from spectrochempy.core.dataset.nddataset import NDDataset
-
-        # HACK to be able to used deprecated alias of the method, without error
-        # because if not this modification obj appears two times
-        if args and type(args[0]) == type(obj):
-            args = args[1:]
-
-        # get the method output - one or two arrays depending on the method and *args
-        output = self.method(obj, *args, **kwargs)
-
-        # restore eventually masked rows and columns
-        axis = "both"
-        if self.typex is not None and self.typex != "features":
-            axis = 0
-        elif self.typey is not None:
-            axis = 1
-
-        # if a single array was returned...
-        if not isinstance(output, tuple):
-            # ... make a tuple of 1 array:
-            data_tuple = (output,)
-            # ... and a tuple of 1 from_meta element:
-            if not isinstance(self.meta_from, tuple):
-                meta_from_tuple = (self.meta_from,)
-            else:
-                # ensure that the first one
-                meta_from_tuple = (self.meta_from[0],)
-        else:
-            data_tuple = output
-            meta_from_tuple = self.meta_from
-
-        out = []
-        for data, meta_from in zip(data_tuple, meta_from_tuple):
-            X_transf = NDDataset(data)
-
-            # Now set the NDDataset attributes from the original X
-
-            # determine the input X dataset
-            X = getattr(obj, meta_from)
-
-            if self.units is not None:
-                if self.units == "keep":
-                    X_transf.units = X.units
-                else:
-                    X_transf.units = self.units
-            X_transf.name = f"{X.name}_{obj.name}.{self.method.__name__}"
-            X_transf.history = f"Created using method {obj.name}.{self.method.__name__}"
-            if self.title is not None:
-                if self.title == "keep":
-                    X_transf.title = X.title
-                else:
-                    X_transf.title = self.title
-            # make coordset
-            M, N = X.shape
-            if X_transf.shape == X.shape and self.typex is None and self.typey is None:
-                X_transf.set_coordset(y=X.coord(0), x=X.coord(1))
-            else:
-                if self.typey == "components":
-                    X_transf.set_coordset(
-                        y=Coord(
-                            None,
-                            labels=["#%d" % (i) for i in range(X_transf.shape[0])],
-                            title="components",
-                        ),
-                        x=X.coord(-1).copy() if X.coord(-1) is not None else None,
-                    )
-                if self.typex == "components":
-                    X_transf.set_coordset(
-                        y=X.coord(0).copy() if X.coord(0) is not None else None,
-                        # cannot use X.y in case of transposed X
-                        x=Coord(
-                            None,
-                            labels=["#%d" % (i) for i in range(X_transf.shape[-1])],
-                            title="components",
-                        ),
-                    )
-                if self.typex == "features":
-                    X_transf.set_coordset(
-                        y=Coord(
-                            None,
-                            labels=["#%d" % (i) for i in range(X_transf.shape[-1])],
-                            title="components",
-                        ),
-                        x=X.coord(1).copy() if X.coord(1) is not None else None,
-                    )
-                if self.typey == "features":
-                    X_transf.set_coordset(
-                        y=X.coord(1).copy() if X.coord(1) is not None else None,
-                        x=Coord(
-                            None,
-                            labels=["#%d" % (i) for i in range(X_transf.shape[-1])],
-                            title="components",
-                        ),
-                    )
-                if self.typesingle == "components":
-                    # occurs when the data are 1D such as ev_ratio...
-                    X_transf.set_coordset(
-                        x=Coord(
-                            None,
-                            labels=["#%d" % (i) for i in range(X_transf.shape[-1])],
-                            title="components",
-                        ),
-                    )
-                if self.typesingle == "targets":
-                    # occurs when the data are 1D such as PLSRegression intercept...
-                    if X.coordset[0].labels is not None:
-                        labels = X.coordset[0].labels
-                    else:
-                        labels = ["#%d" % (i + 1) for i in range(X.shape[-1])]
-                    X_transf.set_coordset(
-                        x=Coord(
-                            None,
-                            labels=labels,
-                            title="targets",
-                        ),
-                    )
-
-            # eventually restore masks
-            X_transf = obj._restore_masked_data(X_transf, axis=axis)
-            out.append(X_transf.squeeze())
-
-        if len(out) == 1:
-            return out[0]
-        else:
-            return tuple(out)
-
-
-def _wrap_ndarray_output_to_nddataset(
-    method=None,
-    meta_from="_X",
-    units="keep",
-    title="keep",
-    typex=None,
-    typey=None,
-    typesingle=None,
-):
-    # wrap _set_output to allow for deferred calling
-    if method:
-        # case of the decorator without argument
-        out = _set_output(method)
-    else:
-        # and with argument
-        def wrapper(method):
-            return _set_output(
-                method,
-                meta_from=meta_from,
-                units=units,
-                title=title,
-                typex=typex,
-                typey=typey,
-                typesingle=typesingle,
-            )
-
-        out = wrapper
-    return out
-
-
-# ======================================================================================
 # Base class AnalysisConfigurable
 # ======================================================================================
-class AnalysisConfigurable(MetaConfigurable):
-
+class AnalysisConfigurable(BaseConfigurable):
     __doc__ = _docstring.dedent(
         r"""
     Abstract class to write analysis model estimators.
 
     Analysis model class must subclass this to get a minimal structure
 
     Parameters
     ----------
-    log_level : any of [``"INFO"``\ , ``"DEBUG"``\ , ``"WARNING"``\ , ``"ERROR"``\ ], optional, default: ``"WARNING"``
-        The log level at startup.
+    %(BaseConfigurable.parameters.log_level)s
     warm_start : `bool`\ , optional, default: `False`
         When fitting repeatedly on the same dataset, but for multiple
         parameter values (such as to find the value maximizing performance),
         it may be possible to reuse previous model learned from the previous parameter
         value, saving time.
 
         When `warm_start` is `True`\ , the existing fitted model attributes is used to
@@ -280,29 +55,15 @@
     # Get doc sections for reuse in subclass
     _docstring.get_sections(__doc__, base="AnalysisConfigurable")
 
     # ----------------------------------------------------------------------------------
     # Runtime Parameters
     # ----------------------------------------------------------------------------------
     _fitted = tr.Bool(False, help="False if the model was not yet fitted")
-    _masked_rc = tr.Tuple(allow_none=True, help="List of masked rows and columns")
-    _X = NDDatasetType(allow_none=True, help="Data to fit a model")
-    _X_mask = Array(allow_none=True, help="Mask information of the input X data")
-    _X_preprocessed = Array(help="Preprocessed inital input X data")
-    _X_shape = tr.Tuple(
-        help="Original shape of the input X data, " "before any transformation"
-    )
-    _X_coordset = tr.Instance(CoordSet, allow_none=True)
-    _is_dataset = tr.Bool(help="True if the input X data is a NDDataset")
     _outfit = tr.Any(help="the output of the _fit method - generally a tuple")
-    _output_type = tr.Enum(
-        ["NDDataset", "ndarray"],
-        default_value="NDDataset",
-        help="Whether the output is a NDDataset or a ndarray",
-    )
 
     # ----------------------------------------------------------------------------------
     # Configuration parameters (mostly defined in subclass
     # as they depend on the model estimator)
     # ----------------------------------------------------------------------------------
 
     # Write here traits like e.g.,
@@ -315,260 +76,43 @@
         self,
         *,
         log_level=logging.WARNING,
         warm_start=False,
         **kwargs,
     ):
         """ """
-        # An empty __doc__ is placed here, else Configurable.__doc__
-        # will appear when there is no __init___.doc in subclass
-
-        # Reset default configuration if not warm_start
-        reset = not warm_start
+        self._warm_start = warm_start
 
-        # Call the super class (MetaConfigurable) for initialisation
-        super().__init__(parent=app, reset=reset)
-
-        # Set log_level of the console report (accessible using the log property)
-        set_loglevel(log_level)
-
-        # Initial configuration
-        # ---------------------
-        # Reset all config parameters to default, if not warm_start
-        defaults = self.parameters(default=True)
-        configkw = {} if warm_start else defaults
-
-        # Eventually take parameters from kwargs
-        configkw.update(kwargs)
-
-        # Now update all configuration parameters
-        # if an item k is not in the config parameters, an error is raised.
-        for k, v in configkw.items():
-            if hasattr(self, k) and k in defaults:
-                if getattr(self, k) != v:
-                    setattr(self, k, v)
-            else:
-                raise KeyError(
-                    f"'{k}' is not a valid configuration parameters. "
-                    f"Use the method `parameters()` to check the current "
-                    f"allowed parameters and their current value."
-                )
+        super().__init__(log_level=log_level, **kwargs)
 
-        # If warm start we can use the previous fit as starting profiles.
-        # so the flag _fitted is not set.
         if not warm_start:
             # We should not be able to use any methods requiring fit results
             # until the fit method has been executed
             self._fitted = False
 
     # ----------------------------------------------------------------------------------
-    # Private methods
-    # ----------------------------------------------------------------------------------
-    def _make_dataset(self, d):
-        # Transform an array-like object to NDDataset
-        # or a list of array-like to a list of NDQataset
-        if d is None:
-            return
-        if isinstance(d, (tuple, list)):
-            d = [self._make_dataset(item) for item in d]
-        elif not isinstance(d, NDDataset):
-            d = NDDataset(d, copy=True)
-        else:
-            d = d.copy()
-        return d
-
-    def _make_unsqueezed_dataset(self, d):
-        # add a dimension to 1D Dataset
-        if d.ndim == 1:
-            coordset = d.coordset
-            d._data = d._data[np.newaxis]
-            if np.any(d.mask):
-                d._mask = d._mask[np.newaxis]
-            d.dims = ["y", "x"]  # "y" is the new dimension
-            coordx = coordset[0] if coordset is not None else None
-            d.set_coordset(x=coordx, y=None)
-        return d
-
-    def _get_masked_rc(self, mask):
-        # Get the mask by row and columns.
-        # -------------------------------
-        # When a single element in the array is
-        # masked, the whole row and columns for this element is masked as well as the
-        # corresponding columns.
-        if np.any(mask):
-            masked_columns = np.all(mask, axis=-2)  # if mask.ndim == 2 else None
-            masked_rows = np.all(mask, axis=-1)
-        else:
-            masked_columns = np.zeros(self._X_shape[-1], dtype=bool)
-            masked_rows = np.zeros(self._X_shape[-2], dtype=bool)
-        return masked_rows, masked_columns
-
-    def _remove_masked_data(self, X):
-        # Retains only valid rows and columns
-        # -----------------------------------
-        # unfortunately, the implementation of linalg library
-        # doesn't support numpy masked arrays as input. So we will have to
-        # remove the masked values ourselves
-
-        # the following however assumes that entire rows or columns are masked,
-        # not only some individual data (if this is what you wanted, this
-        # will fail)
-        if not hasattr(X, "mask") or not np.any(X._mask):
-            return X
-
-        # remove masked rows and columns
-        masked_rows, masked_columns = self._get_masked_rc(X._mask)
-
-        Xc = X[:, ~masked_columns]
-        Xrc = Xc[~masked_rows]
-
-        # destroy the mask
-        Xrc._mask = NOMASK
-
-        # return the modified X dataset
-        return Xrc
-
-    def _restore_masked_data(self, D, axis=-1):
-        # by default, we restore columns, put axis=0 to restore rows instead
-        # Note that it is very important to use here the ma version of zeros
-        # array constructor or both if both axis should be restored
-        if not np.any(self._X_mask):
-            # return it inchanged as wa had no mask originally
-            return D
-
-        rowsize, colsize = self._X_shape
-        masked_rows, masked_columns = self._get_masked_rc(self._X_mask)
-
-        if D.ndim == 2:
-            # Put back masked columns in D
-            # ----------------------------
-            M, N = D.shape
-            if axis == "both":  # and D.shape[0] == rowsize:
-                if np.any(masked_columns) or np.any(masked_rows):
-                    Dtemp = np.ma.zeros((rowsize, colsize))  # note np.ma, not np.
-                    Dtemp[~self._X_mask] = D.data.flatten()
-                    Dtemp[self._X_mask] = MASKED
-                    D.data = Dtemp
-                    try:
-                        D.coordset[D.dims[-1]] = self._X_coordset[D.dims[-1]]
-                        D.coordset[D.dims[-2]] = self._X_coordset[D.dims[-2]]
-                    except TypeError:
-                        # probably no coordset
-                        pass
-            elif axis == -1 or axis == 1:
-                if np.any(masked_columns):
-                    Dtemp = np.ma.zeros((M, colsize))  # note np.ma, not np.
-                    Dtemp[:, ~masked_columns] = D
-                    Dtemp[:, masked_columns] = MASKED
-                    D.data = Dtemp
-                    try:
-                        D.coordset[D.dims[-1]] = self._X_coordset[D.dims[-1]]
-                    except TypeError:
-                        # probably no coordset
-                        pass
-
-            # Put back masked rows in D
-            # -------------------------
-            elif axis == -2 or axis == 0:
-                if np.any(masked_rows):
-                    Dtemp = np.ma.zeros((rowsize, N))
-                    Dtemp[~masked_rows] = D
-                    Dtemp[masked_rows] = MASKED
-                    D.data = Dtemp
-                    try:
-                        D.coordset[D.dims[-2]] = self._X_coordset[D.dims[-2]]
-                    except TypeError:
-                        # probably no coordset
-                        pass
-        elif D.ndim == 1:
-            # we assume here that the only case it happens is for array as explained
-            # variance so that we deal with masked rows
-            if np.any(masked_rows):
-                Dtemp = np.ma.zeros((rowsize,))  # note np.ma, not np.
-                Dtemp[~masked_rows] = D
-                Dtemp[masked_rows] = MASKED
-                D.data = Dtemp
-
-        elif D.ndim == 3:
-            # CASE of IRIS for instance
-
-            # Put back masked columns in D
-            # ----------------------------
-            J, M, N = D.shape
-            if axis == -1 or axis == 2:
-                if np.any(masked_columns):
-                    Dtemp = np.ma.zeros((J, M, colsize))  # note np.ma, not np.
-                    Dtemp[..., ~masked_columns] = D
-                    Dtemp[..., masked_columns] = MASKED
-                    D.data = Dtemp
-                    try:
-                        D.coordset[D.dims[-1]] = self._X_coordset[D.dims[-1]]
-                    except TypeError:
-                        # probably no coordset
-                        pass
-
-        # return the D array with restored masked data
-        return D
-
-    # ----------------------------------------------------------------------------------
     # Private validation and default getter methods
     # ----------------------------------------------------------------------------------
     @tr.default("_X")
     def _X_default(self):
         raise NotFittedError
 
-    @tr.validate("_X")
-    def _X_validate(self, proposal):
-        # validation fired when self._X is assigned
-        X = proposal.value
-
-        # for the following we need X with two dimensions
-        # So let's generate the un-squeezed X
-        X = self._make_unsqueezed_dataset(X)
-
-        # as in fit methods we often use np.linalg library, we cannot handle directly
-        # masked data (so we remove them here and they will be restored at the end of
-        # the process during transform or inverse transform methods
-        # store the original shape as it will be eventually modified as welle- as the
-        # original coordset
-        self._X_shape = X.shape
-
-        # store the mask because it may be destroyed
-        self._X_mask = X._mask.copy()
-
-        # and the original coordset
-        self._X_coordset = copy(X._coordset)
-
-        # remove masked data and return modified dataset
-        X = self._remove_masked_data(X)
-        return X
-
     @property
     def _X_is_missing(self):
         # check whether X has been already defined
         try:
             if self._X is None:
                 return True
         except NotFittedError:
             return True
         return False
 
     # ----------------------------------------------------------------------------------
     # Private methods that should be, most of the time, overloaded in subclass
     # ----------------------------------------------------------------------------------
-    @tr.observe("_X")
-    def _preprocess_as_X_changed(self, change):
-        # to be optionally replaced by user defined function (with the same name)
-        X = change.new
-        # .... preprocessing as scaling, centering, ... must return a ndarray with
-        #  same shape a X.data
-
-        # Set a X.data by default
-        self._X_preprocessed = X.data
-
     def _fit(self, X, Y=None):  # pragma: no cover
         #  Intended to be replaced in the subclasses by user defined function
         #  (with the same name)
         raise NotImplementedError("fit method has not yet been implemented")
 
     # ----------------------------------------------------------------------------------
     # Public methods and property
@@ -1210,15 +754,14 @@
             Whether to also apply the dimensionality reduction to Y when neither X nor Y are provided.
         %(kwargs)s
 
         Returns
         -------
         x_score, y_score: `NDDataset` or tuple of `NDDataset`
             Datasets with shape (:term:`n_observations`\ , :term:`n_components`\ ).
-
         """
         if not self._fitted:
             raise NotFittedError()
 
         # Fire the validation and preprocessing
         self._X = X if X is not None else self.X
         self._Y = Y if Y is not None else self.Y
@@ -1521,15 +1064,14 @@
     _docstring.get_sections(_docstring.dedent(parityplot.__doc__), base="parityplot")
 
 
 # ======================================================================================
 # Base class LinearRegressionAnalysis
 # ======================================================================================
 class LinearRegressionAnalysis(AnalysisConfigurable):
-
     # ----------------------------------------------------------------------------------
     # Configuration parameters (mostly defined in subclass
     # as they depend on the model estimator)
     # ----------------------------------------------------------------------------------
     fit_intercept = tr.Bool(
         default_value=True,
         help="Whether to calculate the `intercept` for this model. If set to `False`, "
@@ -1555,15 +1097,14 @@
     def __init__(
         self,
         *,
         log_level="WARNING",
         warm_start=False,
         **kwargs,
     ):
-
         # call the super class for initialisation of the configuration parameters
         # to do before anything else!
         super().__init__(
             log_level=log_level,
             warm_start=warm_start,
             **kwargs,
         )
@@ -1717,15 +1258,14 @@
         if self._linear_regression.coef_.size == 1:
             # this is the result of the single equation, so only one value
             # should be returned
             A = float(self._linear_regression.coef_)
             if self._is_dataset and self._Y.has_units and self._X.has_units:
                 A = A * self._Y.units / self._X.units
         elif self._is_dataset:
-
             unitsX = self._X.units if self._X.units is not None else 1.0
             unitsY = self._Y.units if self._Y.units is not None else 1.0
             if unitsX != 1 or unitsY != 1:
                 units = self._Y.units / self._X.units
             else:
                 units = None
```

### Comparing `spectrochempy-0.6.5/spectrochempy/analysis/api.py` & `spectrochempy-0.6.6/spectrochempy/analysis/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/analysis/efa.py` & `spectrochempy-0.6.6/spectrochempy/analysis/decomposition/efa.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,21 @@
 # ======================================================================================
 """
 This module implement the EFA (Evolving Factor Analysis) class.
 """
 import numpy as np
 import traitlets as tr
 
-from spectrochempy.analysis._base import (
-    DecompositionAnalysis,
+from spectrochempy.analysis._base._analysisbase import DecompositionAnalysis
+from spectrochempy.application import info_
+from spectrochempy.utils.decorators import (
     _wrap_ndarray_output_to_nddataset,
+    deprecated,
+    signature_has_configurable_traits,
 )
-from spectrochempy.core import info_
-from spectrochempy.utils.decorators import deprecated, signature_has_configurable_traits
 from spectrochempy.utils.docstrings import _docstring
 
 __all__ = ["EFA"]
 __configurables__ = ["EFA"]
 
 
 @signature_has_configurable_traits
```

### Comparing `spectrochempy-0.6.5/spectrochempy/analysis/fast_ica.py` & `spectrochempy-0.6.6/spectrochempy/analysis/decomposition/fast_ica.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 Implementation of FastICA model (using scikit-learn library)
 """
 
 import traitlets as tr
 from numpy.random import RandomState
 from sklearn import decomposition
 
-from spectrochempy.analysis._base import (
+from spectrochempy.analysis._base._analysisbase import (
     DecompositionAnalysis,
     _wrap_ndarray_output_to_nddataset,
 )
 from spectrochempy.utils.decorators import signature_has_configurable_traits
 from spectrochempy.utils.docstrings import _docstring
 from spectrochempy.utils.traits import NDDatasetType
```

### Comparing `spectrochempy-0.6.5/spectrochempy/analysis/iris.py` & `spectrochempy-0.6.6/spectrochempy/analysis/decomposition/iris.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,19 @@
 
 import numpy as np
 import quadprog
 import traitlets as tr
 from matplotlib import pyplot as plt
 from scipy import optimize
 
-from spectrochempy.analysis._base import DecompositionAnalysis, NotFittedError
-from spectrochempy.core import info_, warning_
+from spectrochempy.analysis._base._analysisbase import (
+    DecompositionAnalysis,
+    NotFittedError,
+)
+from spectrochempy.application import info_, warning_
 from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.core.dataset.coordset import CoordSet
 from spectrochempy.core.dataset.nddataset import NDDataset
 from spectrochempy.extern.traittypes import Array
 from spectrochempy.utils.constants import EPSILON
 from spectrochempy.utils.decorators import signature_has_configurable_traits
 from spectrochempy.utils.docstrings import _docstring
```

### Comparing `spectrochempy-0.6.5/spectrochempy/analysis/kinetic_utilities.py` & `spectrochempy-0.6.6/spectrochempy/analysis/kinetic/kineticutilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from functools import partial
 
 import numpy as np
 import traitlets as tr
 from scipy.integrate import solve_ivp
 from scipy.optimize import differential_evolution, least_squares, minimize
 
-from spectrochempy.core import error_
+from spectrochempy.application import error_
 from spectrochempy.core.dataset.nddataset import Coord, NDDataset
 from spectrochempy.core.units import Quantity
 from spectrochempy.extern.traittypes import Array
 from spectrochempy.utils.exceptions import SpectroChemPyError
 from spectrochempy.utils.optional import import_optional_dependency
 
 __all__ = [
@@ -612,15 +612,15 @@
                 jac=jac,
             )
 
             # uncomment for debugging and optimization
             # t2 = time.time()
 
         # uncomment for debugging (warning: debug_() multiply the exec time by 4...)
-        # from from spectrochempy.core import debug_
+        # from from spectrochempy.application import debug_
         # debug_(bunch.message)
         # t4 = time.time()
 
         if bunch.status != 0:
             raise SolverError(bunch.message)
 
         C = (left_op @ bunch.y).T if left_op is not None else bunch.y.T
```

### Comparing `spectrochempy-0.6.5/spectrochempy/analysis/linearregression.py` & `spectrochempy-0.6.6/spectrochempy/analysis/curvefitting/linearregression.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
 Implementation of least squares Linear Regression.
 """
 import traitlets as tr
 
-from spectrochempy.analysis._base import LinearRegressionAnalysis
+from spectrochempy.analysis._base._analysisbase import LinearRegressionAnalysis
 from spectrochempy.utils.decorators import signature_has_configurable_traits
 from spectrochempy.utils.docstrings import _docstring
 
 __all__ = ["LSTSQ", "NNLS"]
 __configurables__ = ["LSTSQ", "NNLS"]
```

### Comparing `spectrochempy-0.6.5/spectrochempy/analysis/mcrals.py` & `spectrochempy-0.6.6/spectrochempy/analysis/decomposition/mcrals.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 
 import dill
 import numpy as np
 import scipy
 import traitlets as tr
 from sklearn import decomposition
 
-from spectrochempy.analysis._base import (
+from spectrochempy.analysis._base._analysisbase import (
     DecompositionAnalysis,
     NotFittedError,
     _wrap_ndarray_output_to_nddataset,
 )
-from spectrochempy.core import info_
+from spectrochempy.application import info_
 from spectrochempy.extern.traittypes import Array
 from spectrochempy.utils.decorators import deprecated, signature_has_configurable_traits
 from spectrochempy.utils.docstrings import _docstring
 
 
 # DEVNOTE:
 # the following decorator allow to correct signature and docs of traitlets.HasTraits
```

### Comparing `spectrochempy-0.6.5/spectrochempy/analysis/nmf.py` & `spectrochempy-0.6.6/spectrochempy/analysis/decomposition/nmf.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 import logging
 
 import traitlets as tr
 from numpy.random import RandomState
 from sklearn import decomposition
 
-from spectrochempy.analysis._base import DecompositionAnalysis
+from spectrochempy.analysis._base._analysisbase import DecompositionAnalysis
 from spectrochempy.utils.decorators import deprecated, signature_has_configurable_traits
 from spectrochempy.utils.docstrings import _docstring
 
 __all__ = ["NMF"]
 __configurables__ = ["NMF"]
```

### Comparing `spectrochempy-0.6.5/spectrochempy/analysis/optimize/_models.py` & `spectrochempy-0.6.6/spectrochempy/analysis/curvefitting/_models.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/analysis/optimize/_parameters.py` & `spectrochempy-0.6.6/spectrochempy/analysis/curvefitting/_parameters.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/analysis/optimize/optimize.py` & `spectrochempy-0.6.6/spectrochempy/analysis/curvefitting/optimize.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
+__all__ = ["Optimize"]
+__configurables__ = __all__
 
 import re
 import sys
 
 import numpy as np
 import scipy.optimize
 import traitlets as tr
 from IPython import display
 
-from spectrochempy.analysis._base import DecompositionAnalysis
-from spectrochempy.analysis.optimize import _models as models_
-from spectrochempy.analysis.optimize._parameters import FitParameters
+from spectrochempy.analysis._base._analysisbase import DecompositionAnalysis
+from spectrochempy.analysis.curvefitting import _models as models_
+from spectrochempy.analysis.curvefitting._parameters import FitParameters
 from spectrochempy.application import info_, warning_
 from spectrochempy.extern.traittypes import Array
 from spectrochempy.utils.decorators import signature_has_configurable_traits
 from spectrochempy.utils.docstrings import _docstring
 
 
 # ======================================================================================
```

### Comparing `spectrochempy-0.6.5/spectrochempy/analysis/pca.py` & `spectrochempy-0.6.6/spectrochempy/analysis/decomposition/pca.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import traitlets as tr
 from matplotlib.ticker import MaxNLocator, ScalarFormatter
 from numpy.random import RandomState
 from sklearn import decomposition
 
-from spectrochempy.analysis._base import (
+from spectrochempy.analysis._base._analysisbase import (
     DecompositionAnalysis,
     NotFittedError,
     _wrap_ndarray_output_to_nddataset,
 )
 from spectrochempy.utils.decorators import deprecated, signature_has_configurable_traits
 from spectrochempy.utils.docstrings import _docstring
 from spectrochempy.utils.plots import NBlue, NRed
@@ -276,14 +276,16 @@
     def _transform(self, X):
         return self._pca.transform(X)
 
     def _inverse_transform(self, X_transform):
         # we need to  set self._pca.components_ to a compatible size but without
         # destroying the full matrix:
         store_components_ = self._pca.components_
+        if X_transform.ndim == 1:
+            X_transform = X_transform.reshape(-1, 1)
         self._pca.components_ = self._pca.components_[: X_transform.shape[1]]
         X = self._pca.inverse_transform(X_transform)
         # restore
         self._pca.components_ = store_components_
         return X
 
     def _get_components(self):
```

### Comparing `spectrochempy-0.6.5/spectrochempy/analysis/peakfinding.py` & `spectrochempy-0.6.6/spectrochempy/analysis/peakfinding/peakfinding.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/analysis/pls.py` & `spectrochempy-0.6.6/spectrochempy/analysis/crossdecomposition/pls.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 Implementation of Partial Least Square regression (using scikit-learn library)
 """
 
 import traitlets as tr
 from sklearn import cross_decomposition
 
-from spectrochempy.analysis._base import (
+from spectrochempy.analysis._base._analysisbase import (
     CrossDecompositionAnalysis,
     _wrap_ndarray_output_to_nddataset,
 )
 from spectrochempy.core.dataset.nddataset import NDDataset
 from spectrochempy.utils.decorators import signature_has_configurable_traits
 from spectrochempy.utils.docstrings import _docstring
 
@@ -271,18 +271,10 @@
     def intercept(self):
         return self._intercept
 
     @property
     def n_iter(self):
         return self._n_iter_
 
-    # ----------------------------------------------------------------------------------
-    # Reporting specific to PCA
-    # ----------------------------------------------------------------------------------
-
-    # ----------------------------------------------------------------------------------
-    # Plot methods specific to PLSRegression
-    # ----------------------------------------------------------------------------------
-
 
 if __name__ == "__main__":
     pass
```

### Comparing `spectrochempy-0.6.5/spectrochempy/analysis/readme.rst` & `spectrochempy-0.6.6/spectrochempy/analysis/readme.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/analysis/simplisma.py` & `spectrochempy-0.6.6/spectrochempy/analysis/decomposition/simplisma.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 __configurables__ = ["SIMPLISMA"]
 
 from warnings import warn
 
 import numpy as np
 import traitlets as tr
 
-from spectrochempy.analysis._base import DecompositionAnalysis
-from spectrochempy.core import info_
+from spectrochempy.analysis._base._analysisbase import DecompositionAnalysis
+from spectrochempy.application import info_
 from spectrochempy.utils import exceptions
 from spectrochempy.utils.decorators import deprecated, signature_has_configurable_traits
 from spectrochempy.utils.docstrings import _docstring
 
 
 # ======================================================================================
 # class SIMPLISMA
```

### Comparing `spectrochempy-0.6.5/spectrochempy/analysis/svd.py` & `spectrochempy-0.6.6/spectrochempy/analysis/decomposition/svd.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # ======================================================================================
 """
 This module implements the Singular Value Decomposition (SVD) class.
 """
 import numpy as np
 import traitlets as tr
 
-from spectrochempy.analysis._base import (
+from spectrochempy.analysis._base._analysisbase import (
     DecompositionAnalysis,
     _wrap_ndarray_output_to_nddataset,
 )
 from spectrochempy.utils.docstrings import _docstring
 
 __all__ = ["SVD"]
 __configurables__ = ["SVD"]
```

### Comparing `spectrochempy-0.6.5/spectrochempy/api.py` & `spectrochempy-0.6.6/spectrochempy/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/application/_check_update.py` & `spectrochempy-0.6.6/spectrochempy/application/_check_update.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/application/application.py` & `spectrochempy-0.6.6/spectrochempy/application/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,15 +457,15 @@
     _from_warning_ = tr.Bool(False)
 
     # ----------------------------------------------------------------------------------
     # Initialisation of the application
     # ----------------------------------------------------------------------------------
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.debug_("*" * 40)
+
         self.initialize()
 
     # ----------------------------------------------------------------------------------
     # Error/warning capture
     # ----------------------------------------------------------------------------------
     def _ipython_catch_exceptions(self, shell, etype, evalue, tb, tb_offset=None):
         # output the full traceback only in DEBUG mode or when under pytest
@@ -602,15 +602,14 @@
         Initialisation function for the API applications.
 
         Parameters
         ----------
         argv :  List, [optional].
             List of configuration parameters.
         """
-
         # parse the argv
         # --------------------------------------------------------------------
         # if we are running this under ipython and jupyter notebooks
         # deactivate potential command line arguments
         # (such that those from jupyter which cause problems here)
 
         ipy = get_ipython() if InteractiveShell.initialized() else None
@@ -767,15 +766,15 @@
             emessage = str(args[0])
         elif len(args) == 2:
             etype = args[0] if args else kwargs.get("type", None)
             emessage = (
                 args[1] if args and len(args) > 1 else kwargs.get("message", None)
             )
         else:
-            raise KeyError("wrong argiments have been passed to error_")
+            raise KeyError("wrong arguments have been passed to error_")
         self._catch_exceptions(etype, emessage, None)
 
     def warning_(self, msg, *args, **kwargs):
         """
         Formatted warning message.
         """
         self._from_warning_ = True
```

### Comparing `spectrochempy-0.6.5/spectrochempy/application/datadir.py` & `spectrochempy-0.6.6/spectrochempy/application/datadir.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/application/general_preferences.py` & `spectrochempy-0.6.6/spectrochempy/application/general_preferences.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import logging
 import warnings
 from os import environ
 from pathlib import Path
 
 import traitlets as tr
 
-from spectrochempy.application.metaconfigurable import MetaConfigurable
 from spectrochempy.utils.file import pathclean
+from spectrochempy.utils.metaconfigurable import MetaConfigurable
 
 
 # ======================================================================================
 # General Preferences
 # ======================================================================================
 class GeneralPreferences(MetaConfigurable):
     """
```

### Comparing `spectrochempy-0.6.5/spectrochempy/application/metaconfigurable.py` & `spectrochempy-0.6.6/spectrochempy/utils/metaconfigurable.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
+# -*- coding: utf-8 -*-
+# ======================================================================================
+# Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
+# CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
+# See full LICENSE agreement in the root directory.
+# ======================================================================================
+"""
+This module implements the base class for all configurables.
+"""
+
 from pathlib import Path
 
 import numpy as np
 import traitlets as tr
 from matplotlib import cycler
 from traitlets.config import Config
 from traitlets.config.configurable import Configurable
 from traitlets.config.loader import LazyConfigValue
 
+from spectrochempy.utils.decorators import deprecated
+from spectrochempy.utils.docstrings import _docstring
 from spectrochempy.utils.objects import Adict
 
 
 class MetaConfigurable(Configurable):
     """
     A subclass of Configurable that stores configuration changes in a json file.
 
@@ -55,25 +67,26 @@
         """
         d = {}
         for k, v in self.traits(config=True).items():
             d[k] = v.default_value
         return d
 
     def trait_defaults(self, *names, **metadata):
-        # override traitlets trait default to take into accound changes in the config file
+        # override traitlets trait default to take into accound changes in the config
+        # file
         defaults = super().trait_defaults(*names, **metadata)
         # modify with the loaded external config
         if not names:  # full dictionary
             config = self.config[self.name]
             if "shape" in config and isinstance(config["shape"], LazyConfigValue):
                 del config["shape"]  # remove the lazy configurable object
             defaults.update(config)
         return defaults
 
-    def parameters(self, default=False):
+    def params(self, default=False):
         """
         Current or default configuration values.
 
         Parameters
         ----------
         default : `bool`, optional, default: `False`
             If `default` is `True`, the default parameters are returned,
@@ -87,64 +100,73 @@
         d = Adict()
         if not default:
             d.update(self.trait_values(config=True))
         else:
             d.update(self.trait_defaults(config=True))
         return d
 
+    _docstring.get_docstring(params.__doc__, base="MetaConfigurable.parameters_doc")
+
+    @deprecated(replace="params", removed="0.7.1")
+    def parameters(self, default=False):
+        """
+        Alias for `params` method.
+        """
+        return self.params(default=default)
+
     def reset(self):
         """
         Reset configuration parameters to their default values
         """
         # for this we need to remove the section corresponding
         # to the current configurable (i.e., self.name)
         if self.name in self.config:
             # remove this entry in config
             del self.config[self.name]
             # also delete the current JSON config file
             f = (Path(self.cfg.config_dir) / self.name).with_suffix(".json")
             f.unlink(missing_ok=True)
 
         # then set the default parameters
-        for k, v in self.parameters(default=True).items():
+        for k, v in self.params(default=True).items():
             if getattr(self, k) != v:
                 setattr(self, k, v)
 
     @tr.observe(tr.All)
     def _anytrait_changed(self, change):
         # update configuration after any change
 
         if not hasattr(self, "cfg"):
             # not yet initialized
             return
 
         if change.name in self.trait_names(config=True):
-
             value = change.new
 
             # Serialization of callable functions
             # (avoid recursive functions, though!)
             # for this we use the dill library
             # (see
-            # https://medium.com/@greyboi/serialising-all-the-functions-in-python-cd880a63b591)
+            # https://medium.com/@greyboi/
+            # serialising-all-the-functions-in-python-cd880a63b591)
             if callable(value):
                 import dill
 
                 value = dill.dumps(value)
                 # bytes are however not JSON serialisable: make an encoded string
                 import base64
 
                 value = base64.b64encode(value).decode()
 
             # replace other serializable value by an equivalent
             elif isinstance(value, (type(cycler), Path)):
                 value = str(value)
             if isinstance(value, np.ndarray):
-                # we need to transform it to a list of elements, bUT with python built-in
-                # types, which is not the case e.g., for int64
+                # we need to transform it to a list of elements, bUT with python
+                # built-in types, which is not the case e.g., for int64
                 value = value.tolist()
 
             self.cfg.update(
                 self.name,
                 {
                     self.__class__.__name__: {
                         change.name: value,
```

### Comparing `spectrochempy-0.6.5/spectrochempy/application/plot_preferences.py` & `spectrochempy-0.6.6/spectrochempy/application/plot_preferences.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Tuple,
     Unicode,
     Union,
     default,
     observe,
 )
 
-from spectrochempy.application.metaconfigurable import MetaConfigurable
+from spectrochempy.utils.metaconfigurable import MetaConfigurable
 
 # from spectrochempy.core import warning_
 
 
 # --------------------------------------------------------------------------------------
 # available matplotlib styles (equivalent of plt.style.available)
 # --------------------------------------------------------------------------------------
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/__init__.py` & `spectrochempy-0.6.6/spectrochempy/core/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,45 +11,21 @@
 
 isort:skip_file
 """
 # flake8: noqa
 
 __all__ = []  # modified below
 
-from os import environ
-import sys
-
-from time import perf_counter
-
-
-class timeit:
-    def __init__(self, msg):
-        self.msg = msg
-
-    def __enter__(self):
-        self.time = perf_counter()
-        return self
-
-    def __exit__(self, type, value, traceback):
-        self.time = perf_counter() - self.time
-        self.readout = f"Elapsed Time for {self.msg}: {self.time:.6f} seconds\n"
-        if "pytest" in sys.argv[0] or "py.test" in sys.argv[0]:
-            print(self.readout)
-
+from spectrochempy.utils.timeutils import timeit
 
 # ======================================================================================
 # loading module libraries
 # here we also construct the __all__ list automatically
 # ======================================================================================
 
-with timeit("app"):
-    from spectrochempy.application import app  # noqa: E402
-
-    __all__ += ["app"]
-
 with timeit("application"):
     from spectrochempy.application import (
         version,
         release,
         copyright,
         license,
         release_date,
@@ -70,16 +46,14 @@
         description,
         long_description,
         config_dir,
         config_manager,
         reset_preferences,
     )  # noqa: E402
 
-    # datadir = app.datadir
-
     def set_loglevel(level=WARNING):
         if isinstance(level, str):
             import logging
 
             level = getattr(logging, level)
         preferences.log_level = level
 
@@ -113,14 +87,42 @@
         "release_date",
         "authors",
         "contributors",
         "description",
         "long_description",
     ]
 
+
+# constants
+# ---------
+with timeit("constants"):
+    from spectrochempy.utils.plots import show
+    from spectrochempy.utils.constants import (
+        MASKED,
+        NOMASK,
+        EPSILON,
+        INPLACE,
+    )  # noqa: E402
+    from spectrochempy.utils.print_versions import show_versions  # noqa: E402
+
+    __all__ += ["show", "MASKED", "NOMASK", "EPSILON", "INPLACE", "show_versions"]
+
+# units
+# -----
+with timeit("units"):
+    from spectrochempy.core.units import *  # noqa: E402,F403,F401
+
+    __all__ += [
+        "Unit",
+        "Quantity",
+        "ur",
+        "set_nmr_context",
+        "DimensionalityError",
+    ]
+
 # dataset
 # -------
 with timeit("dataset"):
     from spectrochempy.core.dataset import api  # noqa: E402
     from spectrochempy.core.dataset.api import *  # noqa: E402,F403,F401
 
     __all__ += api.__all__
@@ -129,22 +131,14 @@
 # --------
 with timeit("plotter"):
     from spectrochempy.core.plotters import api  # noqa: E402
     from spectrochempy.core.plotters.api import *  # noqa: E402,F403,F401
 
     __all__ += api.__all__
 
-# processors
-# ----------
-with timeit("processor"):
-    from spectrochempy.core.processors import api  # noqa: E402
-    from spectrochempy.core.processors.api import *  # noqa: E402,F403,F401
-
-    __all__ += api.__all__
-
 # readers
 # -------
 with timeit("readers"):
     from spectrochempy.core.readers import api  # noqa: E402
     from spectrochempy.core.readers.api import *  # noqa: E402,F403,F401
 
     __all__ += api.__all__
@@ -184,38 +178,21 @@
 # --------
 with timeit("analysis"):
     from spectrochempy.analysis import api  # noqa: E402
     from spectrochempy.analysis.api import *  # noqa: E402,F403,F401
 
     __all__ += api.__all__
 
-with timeit("constants"):
-
-    # constants
-    # ---------
-    from spectrochempy.utils.plots import show
-    from spectrochempy.utils.constants import (
-        MASKED,
-        NOMASK,
-        EPSILON,
-        INPLACE,
-    )
-    from spectrochempy.utils.print_versions import show_versions
-
-    __all__ += ["show", "MASKED", "NOMASK", "EPSILON", "INPLACE", "show_versions"]
-
-# units
-# -----
-with timeit("units"):
-    from spectrochempy.core.units import *  # noqa: E402,F403,F401
+# processing
+# ----------
+with timeit("processing"):
+    from spectrochempy.processing import api  # noqa: E402
+    from spectrochempy.processing.api import *  # noqa: E402,F403,F401
 
-    __all__ += [
-        "Unit",
-        "Quantity",
-        "ur",
-        "set_nmr_context",
-        "DimensionalityError",
-    ]
+    __all__ += api.__all__
 
 # START THE app
+# -------------
 with timeit("start app"):
+    from spectrochempy.application import app
+
     _started = app.start()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/common/dialogs.py` & `spectrochempy-0.6.6/spectrochempy/core/common/dialogs.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 # ======================================================================================
 """
 This module implement File I/O Dialogs
 """
 
 from os import environ
 
-from spectrochempy.core import error_, preferences
+from spectrochempy.application import error_
+from spectrochempy.core import preferences
 from spectrochempy.utils.optional import import_optional_dependency
 
 __all__ = ["open_dialog", "save_dialog"]
 
 # Set flags
 USE_QT = preferences.use_qt or environ.get("SCPY_GUI", None) == "RUNNING"
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/dataset/api.py` & `spectrochempy-0.6.6/spectrochempy/core/dataset/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/core/dataset/arraymixins/__init__.py` & `spectrochempy-0.6.6/spectrochempy/core/dataset/arraymixins/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/core/dataset/arraymixins/ndio.py` & `spectrochempy-0.6.6/spectrochempy/core/dataset/arraymixins/ndio.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,28 +10,30 @@
 """
 
 __all__ = ["load"]
 
 import io
 import json
 import pathlib
-from warnings import warn
 
 import numpy as np
 from numpy.lib.npyio import zipfile_factory
 from traitlets import HasTraits, Instance, Unicode, Union
 
 from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.core.dataset.coordset import CoordSet
 from spectrochempy.utils import exceptions
 from spectrochempy.utils.file import check_filename_to_save, pathclean
 from spectrochempy.utils.jsonutils import json_serialiser
 from spectrochempy.utils.misc import TYPE_BOOL
 from spectrochempy.utils.zip import ScpFile
 
+# from warnings import warn
+
+
 SCPY_SUFFIX = {"NDDataset": ".scp", "Project": ".pscp"}
 
 
 # --------------------------------------------------------------------------------------
 # Utilities
 # --------------------------------------------------------------------------------------
 # ======================================================================================
@@ -61,15 +63,18 @@
 
     @property
     def filename(self):
         """
         Current filename for this dataset.
         """
         if self._filename:
-            return self._filename.stem + self.suffix
+            try:
+                return self._filename.relative_to(self.preferences.datadir)
+            except ValueError:
+                return self._filename
         else:
             return None
 
     @filename.setter
     def filename(self, val):
         self._filename = pathclean(val)
 
@@ -435,18 +440,18 @@
         """
 
         # Stage data in a temporary file on disk, before writing to zip.
         import tempfile
         import zipfile
 
         # prepare the json data
-        try:
-            js = self.dumps(encoding="base64")
-        except Exception as e:
-            warn(str(e))
+        # try:
+        js = self.dumps(encoding="base64")
+        # except Exception as e:
+        #     warn(str(e))
 
         # write in a temp file
         _, tmpfile = tempfile.mkstemp(suffix="-spectrochempy")
         tmpfile = pathclean(tmpfile)
         tmpfile.write_bytes(js.encode("utf-8"))
 
         # compress and write zip file
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/dataset/arraymixins/ndmath.py` & `spectrochempy-0.6.6/spectrochempy/core/dataset/arraymixins/ndmath.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import re
 import sys
 from warnings import catch_warnings
 
 import numpy as np
 from quaternion import as_float_array
 
-from spectrochempy.core import error_, warning_
+from spectrochempy.application import error_, warning_
 from spectrochempy.core.units import DimensionalityError, Quantity, ur
 from spectrochempy.utils.constants import NOMASK
 from spectrochempy.utils.exceptions import CoordinatesMismatchError
 from spectrochempy.utils.misc import TYPE_COMPLEX, as_quaternion, quat_as_complex_array
 from spectrochempy.utils.orderedset import OrderedSet
 from spectrochempy.utils.testing import assert_coord_almost_equal
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/dataset/arraymixins/ndplot.py` & `spectrochempy-0.6.6/spectrochempy/core/dataset/arraymixins/ndplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 import matplotlib as mpl
 from cycler import cycler
 from matplotlib import pyplot as plt
 from matplotlib.colors import to_rgba
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from traitlets import Dict, HasTraits, Instance, TraitError, Union, default
 
-from spectrochempy.core import error_, plot_preferences, preferences
+from spectrochempy.application import error_, plot_preferences
+from spectrochempy.core import preferences
 from spectrochempy.core.dataset.baseobjects.meta import Meta
 from spectrochempy.core.plotters.plot1d import plot_1D
 from spectrochempy.core.plotters.plot2d import plot_2D
 from spectrochempy.core.plotters.plot3d import plot_3D
 from spectrochempy.utils.file import pathclean
 from spectrochempy.utils.optional import import_optional_dependency
 from spectrochempy.utils.plots import _Axes, _Axes3D, get_figure
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/dataset/arraymixins/npy.py` & `spectrochempy-0.6.6/spectrochempy/processing/transformation/npy.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/core/dataset/baseobjects/meta.py` & `spectrochempy-0.6.6/spectrochempy/core/dataset/baseobjects/meta.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/core/dataset/baseobjects/ndarray.py` & `spectrochempy-0.6.6/spectrochempy/core/dataset/baseobjects/ndarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     List,
     Unicode,
     Union,
     default,
     validate,
 )
 
-from spectrochempy.core import error_, info_
+from spectrochempy.application import error_, info_
 from spectrochempy.core.dataset.baseobjects.meta import Meta
 from spectrochempy.core.units import (
     DimensionalityError,
     Quantity,
     Unit,
     set_nmr_context,
     ur,
@@ -366,15 +366,26 @@
         # choose, if we keep the same or create new object
         inplace = False
         if isinstance(items, tuple) and np.any(str(items[-1]) == INPLACE):
             items = items[:-1]
             inplace = True
 
         # Eventually get a better representation of the indexes
-        keys = self._make_index(items)
+        try:
+            keys = self._make_index(items)
+        except IndexError as e:
+            if "Could not find this location" in str(e) and self._squeeze_ndim == 1:
+                # Try to use the next dimension if items is not already a tuple
+                if not isinstance(items, tuple):
+                    new_items = (slice(None), items)
+                    keys = self._make_index(new_items)
+                else:
+                    raise e
+            else:
+                raise e
 
         # init returned object
         if inplace:
             new = self
         else:
             new = self.copy()
 
@@ -1189,15 +1200,14 @@
         if not keepname:
             new.name = ""  # default
 
         return new
 
     @property
     @_docstring.get_docstring(base="data")
-    @_docstring.dedent
     def data(self):
         """
         Data array (`~numpy.ndarray`).
 
         If there is no data but labels, then the labels are returned instead of data.
         """
         return self._data
@@ -1962,31 +1972,29 @@
         transpose: Permute the dimensions of an array.
         """
         return self.transpose()
 
     @property
     def title(self):
         """
-        An user friendly title (str).
+        An user-friendly title (str).
 
         When the title is provided, it can be used for labeling the object,
         e.g., axe title in a matplotlib plot.
         """
         if self._title:
             return self._title
         else:
             return "<untitled>"
 
     @title.setter
     def title(self, title):
         if title:
             self._title = title
 
-    @_docstring.get_docstring(base="to")
-    @_docstring.dedent
     def to(self, other, inplace=False, force=False):
         """
         Return the object with data rescaled to different units.
 
         Parameters
         ----------
         other : `Quantity` or str
@@ -2154,14 +2162,16 @@
             self._units = new._units
             self._title = new._title
             self._roi = new._roi
 
         else:
             return new
 
+    _docstring.get_docstring(to.__doc__, base="to")
+
     def to_base_units(self, inplace=False):
         """
         Return an array rescaled to base units.
 
         Parameters
         ----------
         inplace : bool
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/dataset/baseobjects/ndcomplex.py` & `spectrochempy-0.6.6/spectrochempy/core/dataset/baseobjects/ndcomplex.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/core/dataset/coord.py` & `spectrochempy-0.6.6/spectrochempy/core/dataset/coord.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 __all__ = ["Coord"]
 
 import textwrap
 
 import numpy as np
 import traitlets as tr
 
-from spectrochempy.core import error_
+from spectrochempy.application import error_
 from spectrochempy.core.dataset.arraymixins.ndmath import NDMath, _set_operators
 from spectrochempy.core.dataset.baseobjects.ndarray import NDArray
 from spectrochempy.core.units import Quantity, ur
 from spectrochempy.utils.compare import is_iterable, is_number
 from spectrochempy.utils.constants import INPLACE, NOMASK
 from spectrochempy.utils.decorators import deprecated
 from spectrochempy.utils.docstrings import _docstring
@@ -492,15 +492,15 @@
     @property
     def is_1d(self):
         return True
 
     # ----------------------------------------------------------------------------------
     # public methods
     # ----------------------------------------------------------------------------------
-    def loc2index(self, loc):
+    def loc2index(self, loc, return_error=False):
         """
         Return the index corresponding to a given location.
 
         Parameters
         ----------
         loc : float.
             Value corresponding to a given location on the coordinates axis.
@@ -513,15 +513,21 @@
         Examples
         --------
 
         >>> dataset = scp.read("irdata/nh4y-activation.spg")
         >>> dataset.x.loc2index(1644.0)
         4517
         """
-        return self._loc2index(loc)
+        res = self._loc2index(loc)
+        if isinstance(res, tuple):
+            if return_error:
+                return res
+            else:
+                return res[0]
+        return res
 
     # TODO: new method to replace the old loc2index
     # def loc2index(self, *loc):
     #     """
     #     Return the index(es) corresponding to given location(s).
     #
     #     Parameters
@@ -850,15 +856,15 @@
             # we set the number with their full precision
             # rounding will be made if necessary when reading the data property
             nd = get_n_decimals(np.diff(self._data).max(), self._sigdigits)
             data = np.around(data, nd)
             self._data = np.linspace(data[0], data[-1], data.size)
             self._linear = True
         else:
-            # from spectrochempy.core import debug_
+            # from spectrochempy.application import debug_
             # debug_(
             #      "The coordinates spacing is not enough uniform to allow linearization."
             #  )
             self._linear = False
 
     @property
     def sigdigits(self):
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/dataset/coordset.py` & `spectrochempy-0.6.6/spectrochempy/core/dataset/coordset.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/core/dataset/nddataset.py` & `spectrochempy-0.6.6/spectrochempy/core/dataset/nddataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import textwrap
 from datetime import datetime, tzinfo
 
 import numpy as np
 import pytz  # TODO: for py>=3.9, we could use builtin zoneinfo library instead of pyt
 import traitlets as tr
 
-from spectrochempy.core import error_, warning_
+from spectrochempy.application import error_, warning_
 from spectrochempy.core.dataset.arraymixins.ndio import NDIO
 from spectrochempy.core.dataset.arraymixins.ndmath import NDMath  # _set_ufuncs,
 from spectrochempy.core.dataset.arraymixins.ndmath import _set_operators
 from spectrochempy.core.dataset.arraymixins.ndplot import NDPlot
 from spectrochempy.core.dataset.baseobjects.ndarray import DEFAULT_DIM_NAME, NDArray
 from spectrochempy.core.dataset.baseobjects.ndcomplex import NDComplexArray
 from spectrochempy.core.dataset.coord import Coord
@@ -197,15 +197,15 @@
 
     # baseline data (for GUI)
     # _baselinedata = Array(Float(), allow_none=True)
 
     # reference data (for GUI)
     # _referencedata = Array(Float(), allow_none=True)
 
-    # region ranges
+    # ranges
     # _ranges = Instance(Meta)
 
     # history
     _history = tr.List(tr.Tuple(), allow_none=True)
 
     # Dates
     # _acquisition_date = Instance(datetime, allow_none=True)
@@ -1540,15 +1540,15 @@
 ]
 
 for funcname in api_funcs:
     setattr(thismodule, funcname, getattr(NDDataset, funcname))
     __all__.append(funcname)
 
 # import also npy functions  # TODO: this will be changed with __array_functions__
-from spectrochempy.core.dataset.arraymixins.npy import dot
+from spectrochempy.processing.transformation.npy import dot
 
 NDDataset.dot = dot
 
 # ======================================================================================
 # Set the operators
 # ======================================================================================
 _set_operators(NDDataset, priority=100000)
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/plotters/multiplot.py` & `spectrochempy-0.6.6/spectrochempy/core/plotters/multiplot.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/core/plotters/plot1d.py` & `spectrochempy-0.6.6/spectrochempy/core/plotters/plot1d.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,51 +138,81 @@
     """
     Plot a 1D dataset with bars.
 
     Alias of plot (with `method` argument set to `bar` .
     """
 
 
-def plot_multiple(datasets, method="scatter", pen=True, labels=None, **kwargs):
+def plot_multiple(
+    datasets,
+    method="scatter",
+    pen=True,
+    labels=None,
+    marker="AUTO",
+    color="AUTO",
+    ls="AUTO",
+    lw=1,
+    shift=0,
+    **kwargs,
+):
     """
     Plot a series of 1D datasets as a scatter plot with optional lines between markers.
 
     Parameters
     ----------
-    datasets : a list of ndatasets
-    method : str among [scatter, pen]
+    datasets : `list` of 1D `NDDataset`
+        NDdatasets to plot.
+    method : `str` among [scatter, pen]
+        Method to use for plotting.
     pen : bool, optional, default: True
         If method is scatter, this flag tells to draw also the lines
         between the marks.
-    labels : a list of str, optional
-        Labels used for the legend.
+    labels : a `list` of `str`, optional
+        Labels used for the legend. The length of the list must be equal to the number
+        of datasets to plot.
+    marker : `str`, list` os `str` or `AUTO`, optional, default: 'AUTO'
+        Marker type for scatter plot. If marker is not provided then the scatter type
+        of plot is chosen automatically.
+    color : `str`, list` os `str` or `AUTO`, optional, default: 'AUTO'
+        Color of the lines. If color is not provided then the color of the lines is
+        chosen automatically.
+    ls: `str`, `list` os `str` or `AUTO`, optional, default: 'AUTO'
+        Line style definition. If ls is not provided then the line style is chosen
+        automatically.
+    lw: `float`, `list`of  `floats`, optional, default: 1.0
+        Line width. If lw is not provided then the line width is chosen automatically.
+    shift: `float`, `list`of  `floats`, optional, default: 0.0
+        Vertical shift of the lines.
     **kwargs
         Other parameters that will be passed to the plot1D function.
 
-    Other Parameters
-    ----------------
-    {0}
-
     See Also
     --------
     plot_1D
     plot_pen
     plot_scatter
     plot_bar
     plot_scatter_pen
     """
     if not is_sequence(datasets):
         # we need a sequence. Else it is a single plot.
         return datasets.plot(**kwargs)
 
-    if not is_sequence(labels) or len(labels) != len(datasets):
-        # we need a sequence of labels of same length as datasets
-        raise ValueError(
-            "the list of labels must be of same length " "as the datasets list"
-        )
+    def _valid(x, desc):
+        if is_sequence(x) and len(x) != len(datasets):
+            raise ValueError(
+                f"list of {desc} must be of same length as the datasets list"
+            )
+        if not is_sequence(x) and x != "AUTO":
+            x = [x] * len(datasets)
+            return x
+
+        return x
+
+    labels = _valid(labels, "labels")
 
     for dataset in datasets:
         if dataset._squeeze_ndim > 1:
             raise NotImplementedError(
                 "plot multiple is designed to work on "
                 "1D dataset only. you may achieved "
                 "several plots with "
@@ -200,37 +230,46 @@
     kwargs["commands"] = []
     clear = kwargs.pop("clear", True)
     legend = kwargs.pop(
         "legend", None
     )  # remove 'legend' from kwargs before calling plot
     # else it will generate a conflict
 
-    for s in datasets:  # , colors, markers):
-
-        ax = s.plot(
+    marker = _valid(marker, "marker")
+    color = _valid(color, "color")
+    ls = _valid(ls, "ls")
+    lw = _valid(lw, "lw")
+    shift = _valid(shift, "shift")
+
+    # now we can plot
+    sh = 0
+    for i, s in enumerate(datasets):  # , colors, markers):
+        ax = (s + shift[i] + sh).plot(
             method=method,
             pen=pen,
-            marker="AUTO",
-            color="AUTO",
-            ls="AUTO",
+            marker=(marker[i] if marker != "AUTO" else marker),
+            color=color[i] if color != "AUTO" else color,
+            ls=ls[i] if ls != "AUTO" else ls,
+            lw=lw[i] if lw != "AUTO" else lw,
             clear=clear,
-            **kwargs
+            **kwargs,
         )
+        sh += shift[i]
         clear = False  # clear=False is necessary for the next plot to say
         # that we will plot on the same figure
 
     # scale all plots
     if legend is not None:
         _ = ax.legend(
             ax.lines,
             labels,
             shadow=True,
             loc=legend,
             frameon=True,
-            facecolor="lightyellow",
+            fontsize="small",
         )
 
     # now we can output the final figure
     kw = {"output": output, "commands": commands}
     datasets[0]._plot_resume(datasets[-1], **kw)
 
     return ax
@@ -549,15 +588,14 @@
         xlabel = make_label(x, new.dims[-1])
     ax.set_xlabel(xlabel)
 
     # x tick labels
 
     uselabel = kwargs.get("uselabel", False)
     if x and x.is_labeled and (uselabel or not np.any(x.data)):
-
         if x.data is not None:
             xt = ax.get_xticks()
             ticklabels = x.labels[x._loc2index(xt), 0]
             ax.set_xticks(ax.get_xticks(), labels=ticklabels, rotation=90.0)
         else:
             ax.set_xticks(xdata)
             ax.set_xticklabels(x.labels)
@@ -590,15 +628,14 @@
     elif kwargs.get("plottitle", False):
         ax.set_title(new.name)
 
     new._plot_resume(dataset, **kwargs)
 
     # masks
     if kwargs.get("show_mask", False):
-
         ax.fill_between(
             xdata,
             zdata.min() - 1.0,
             zdata.max() + 1,
             where=new.mask,
             facecolor="#FFEEEE",
             alpha=0.3,
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/plotters/plot2d.py` & `spectrochempy-0.6.6/spectrochempy/core/plotters/plot2d.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/core/plotters/plot3d.py` & `spectrochempy-0.6.6/spectrochempy/core/plotters/plot3d.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/core/plotters/plotly.py` & `spectrochempy-0.6.6/spectrochempy/core/plotters/plotly.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/core/processors/align.py` & `spectrochempy-0.6.6/spectrochempy/processing/alignement/align.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 __all__ = ["align"]
 __dataset_methods__ = __all__
 
 # import scipy.interpolate
 import numpy as np
 
-from spectrochempy.core import error_, warning_
+from spectrochempy.application import error_, warning_
 from spectrochempy.utils import exceptions
 from spectrochempy.utils.constants import MASKED
 from spectrochempy.utils.misc import get_n_decimals
 
 
 def can_merge_or_align(coord1, coord2):
     """
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/processors/apodization.py` & `spectrochempy-0.6.6/spectrochempy/processing/fft/apodization.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 __dataset_methods__ = __all__
 
 import functools
 
 import numpy as np
 from scipy.signal import windows
 
-from spectrochempy.core import error_
+from spectrochempy.application import error_
 from spectrochempy.core.units import Quantity
 from spectrochempy.utils.constants import EPSILON
 
 pi = np.pi
 
 
 # ======================================================================================
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/processors/autosub.py` & `spectrochempy-0.6.6/spectrochempy/processing/transformation/autosub.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         The subtracted dataset.
     coefs : `~numpy.ndarray` .
         The table of subtraction coefficients
         (only if `return_coefs` is set to `True` ).
 
     See Also
     --------
-    BaselineCorrection : Manual baseline corrections.
+    Baseline : Manual baseline corrections.
     abc : Automatic baseline corrections.
 
     Examples
     ---------
 
     >>> path_A = 'irdata/nh4y-activation.spg'
     >>> A = scp.read(path_A, protocol='omnic')
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/processors/baseline.py` & `spectrochempy-0.6.6/spectrochempy/core/readers/importer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,850 +1,869 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
-This module implements the `BaselineCorrection` class for baseline corrections.
+This module define a generic class to import directories, files and contents.
 """
-__all__ = ["BaselineCorrection", "ab", "abc", "dc", "basc"]
+__all__ = ["read", "read_dir"]  # , "read_remote"]
+__dataset_methods__ = __all__
 
-__dataset_methods__ = ["ab", "abc", "dc", "basc"]
+import io
+import re
+from warnings import warn
+from zipfile import ZipFile
+
+import requests
+import yaml
+from traitlets import Dict, HasTraits, List, Type, Unicode
+
+from spectrochempy.application import info_, warning_
+from spectrochempy.utils.docstrings import _docstring
+from spectrochempy.utils.exceptions import DimensionsCompatibilityError, ProtocolError
+from spectrochempy.utils.file import (
+    check_filename_to_open,
+    get_directory_name,
+    get_filenames,
+    pathclean,
+)
+
+FILETYPES = [
+    ("scp", "SpectroChemPy files (*.scp)"),
+    ("omnic", "Nicolet OMNIC files and series (*.spa *.spg *.srs)"),
+    ("soc", "Surface Optics Corp. (*.ddr *.hdr *.sdr)"),
+    ("labspec", "LABSPEC exported files (*.txt)"),
+    ("opus", "Bruker OPUS files (*.[0-9]*)"),
+    (
+        "topspin",
+        "Bruker TOPSPIN fid or series or processed data files "
+        "(fid ser 1[r|i] 2[r|i]* 3[r|i]*)",
+    ),
+    ("matlab", "MATLAB files (*.mat)"),
+    ("dso", "Data Set Object files (*.dso)"),
+    ("jcamp", "JCAMP-DX files (*.jdx *.dx)"),
+    ("csv", "CSV files (*.csv)"),
+    ("excel", "Microsoft Excel files (*.xls)"),
+    ("zip", "Compressed folder of data files (*.zip)"),
+    ("quadera", "Quadera ascii files (*.asc)"),
+    ("carroucell", "Carroucell files (*spa)"),
+    ("galactic", "GRAMS/Thermo Galactic files (*.spc)")
+    #  ('all', 'All files (*.*)')
+]
+ALIAS = [
+    ("spg", "omnic"),
+    ("spa", "omnic"),
+    ("ddr", "soc"),
+    ("hdr", "soc"),
+    ("sdr", "soc"),
+    ("spc", "galactic"),
+    ("srs", "omnic"),
+    ("mat", "matlab"),
+    ("txt", "labspec"),
+    ("jdx", "jcamp"),
+    ("dx", "jcamp"),
+    ("xls", "excel"),
+    ("asc", "quadera"),
+]
+
+
+# --------------------------------------------------------------------------------------
+class Importer(HasTraits):
+    # Private Importer class
+
+    objtype = Type()
+    datasets = List()
+    files = Dict()
+    default_key = Unicode()
+    protocol = Unicode()
+
+    protocols = Dict()
+    filetypes = Dict()
+
+    def __init__(self):
+
+        super().__init__()
+
+        self.filetypes = dict(FILETYPES)
+        temp = list(zip(*FILETYPES))
+        temp.reverse()
+        self.protocols = dict(zip(*temp))
+
+        #  add alias
+
+        self.alias = dict(ALIAS)
+
+    def __call__(self, *args, **kwargs):
+
+        self.datasets = []
+        self.default_key = kwargs.pop("default_key", ".scp")
+
+        if "merge" not in kwargs.keys():
+            # if merge is not specified, but the args are provided as a single list,
+            # then will are supposed to merge the datasets. If merge is specified then
+            # it has priority.
+            # This is not useful for the 1D datasets, as if they are compatible they
+            # are merged automatically
+            if args and len(args) == 1 and isinstance(args[0], (list, tuple)):
+                kwargs["merge"] = True
+
+        args, kwargs = self._setup_objtype(*args, **kwargs)
+        res = check_filename_to_open(*args, **kwargs)
+        if res:
+            # Normal return
+            self.files = res
+        else:
+            # Cancel in dialog!
+            return None
+
+        for key in self.files.keys():
+
+            if key == "" and kwargs.get("protocol") == ["carroucell"]:
+                key = ".carroucell"
+                self.files = {".carroucell": self.files[""]}
+
+            if key == "frombytes":
+                # here we need to read contents
+                for filename, content in self.files[key].items():
+                    files_ = check_filename_to_open(filename)
+                    kwargs["content"] = content
+                    key_ = list(files_.keys())[0]
+                    self._switch_protocol(key_, files_, **kwargs)
+                if len(self.datasets) > 1:
+                    self.datasets = self._do_merge(self.datasets, **kwargs)
+
+            elif key and key[1:] not in list(zip(*FILETYPES))[0] + list(zip(*ALIAS))[0]:
+                raise TypeError(f"Filetype `{key}` is unknown in spectrochempy")
+            else:
+                # here files are read / or remotely from the disk using filenames
+                self._switch_protocol(key, self.files, **kwargs)
+
+        # now we will reset preference for this newly loaded datasets
+        if len(self.datasets) > 0:
+
+            if all(self.datasets) is None:
+                return None
+
+            try:
+                prefs = self.datasets[0].preferences
+                prefs.reset()
+            except (FileNotFoundError, AttributeError):
+                pass
+        else:
+            return None
+
+        if len(self.datasets) == 1:
+            nd = self.datasets[0]  # a single dataset is returned
+            name = kwargs.pop("name", None)
+            if name:
+                nd.name = name
+            return nd
+
+        else:
+            nds = self.datasets
+            names = kwargs.pop("names", None)
+            if names and len(names) == len(nds):
+                for nd, name in zip(nds, names):
+                    nd.name = name
+            elif names and len(names) != len(nds):
+                warn(
+                    "length of the `names` list and of the list of datasets mismatch - names not applied"
+                )
+            return sorted(
+                nds, key=str
+            )  # return a sorted list (sorted according to their string representation)
+
+    def _setup_objtype(self, *args, **kwargs):
+        # check if the first argument is an instance of NDDataset or Project
+
+        args = list(args)
+        if (
+            args
+            and hasattr(args[0], "_implements")
+            and args[0]._implements() in ["NDDataset"]
+        ):
+            # the first arg is an instance of NDDataset
+            object = args.pop(0)
+            self.objtype = type(object)
+
+        else:
+            # by default returned objtype is NDDataset (import here to avoid circular import)
+            from spectrochempy.core.dataset.nddataset import NDDataset
+
+            self.objtype = kwargs.pop("objtype", NDDataset)
+
+        return args, kwargs
 
-import matplotlib.pyplot as plt
-import numpy as np
-import scipy.interpolate
-from matplotlib.widgets import SpanSelector
-from traitlets import Enum, Float, HasTraits, Int, List, Tuple, Unicode
-
-from spectrochempy.core import debug_, warning_
-from spectrochempy.core.plotters.multiplot import multiplot
-from spectrochempy.core.processors.smooth import smooth
-from spectrochempy.core.processors.utils import _units_agnostic_method
-from spectrochempy.utils.coordrange import trim_ranges
-from spectrochempy.utils.decorators import signature_has_configurable_traits
-from spectrochempy.utils.misc import TYPE_FLOAT, TYPE_INTEGER
-from spectrochempy.utils.traits import NDDatasetType
-
-
-@signature_has_configurable_traits
-# Note: with this decorator
-# Configurable traits are added to the signature as keywords if they are not yet present.
-class BaselineCorrection(HasTraits):
+    def _switch_protocol(self, key, files, **kwargs):
+
+        protocol = kwargs.get("protocol", None)
+        if protocol is not None and protocol != "ALL":
+            if not isinstance(protocol, list):
+                protocol = [protocol]
+            if key and key[1:] not in protocol and self.alias[key[1:]] not in protocol:
+                return
+
+        datasets = []
+        for filename in files[key]:
+
+            read_ = getattr(self, f"_read_{key[1:]}")
+
+            dataset = None
+            try:
+                # read locally or using url if filename is an url
+                dataset = read_(self.objtype(), filename, **kwargs)
+
+            except (FileNotFoundError, OSError) as exc:
+                # file was not found.
+                # it is an url we raise an error
+                local_only = kwargs.get("local_only", False)
+                if _is_url(filename) or local_only:
+                    raise (FileNotFoundError) from exc
+
+                # else, we try on github
+                try:
+                    # Try to get the file from github
+                    kwargs["read_method"] = read_
+                    info_(
+                        "File/directory not found locally: Attempt to download it from "
+                        "the GitHub repository `spectrochempy_data`..."
+                    )
+                    dataset = _read_remote(self.objtype(), filename, **kwargs)
+
+                except (FileNotFoundError) as exc:
+                    raise (FileNotFoundError) from exc
+
+                except Exception as e:
+                    warning_(str(e))
+
+            except Exception as e:
+                warning_(str(e))
+
+            if dataset is not None:
+                if not isinstance(dataset, list):
+                    datasets.append(dataset)
+                else:
+                    datasets.extend(dataset)
+
+        if len(datasets) > 1:
+            datasets = self._do_merge(datasets, **kwargs)
+            if kwargs.get("merge", False):
+                datasets[0].name = pathclean(filename).stem
+                datasets[0].filename = pathclean(filename)
+
+        self.datasets.extend(datasets)
+
+    def _do_merge(self, datasets, **kwargs):
+
+        # several datasets returned (only if several files have been passed) and the `merge` keyword argument is False
+        merged = kwargs.get("merge", False)
+        shapes = list({nd.shape if hasattr(nd, "shape") else None for nd in datasets})
+        if len(shapes) == 1 and None not in shapes:
+            # homogeneous set of files
+            # we can merge them if they are 1D spectra
+            if len(shapes[0]) == 1 or shapes[0][0] == 1:
+                merged = kwargs.get("merge", True)  # priority to the keyword setting
+        else:
+            # not homogeneous
+            merged = kwargs.get("merge", False)
+
+        if merged:
+            # Try to stack the dataset into a single one
+            try:
+                dataset = self.objtype.concatenate(datasets, axis=0)
+                if dataset.coordset is not None and kwargs.pop("sortbydate", True):
+                    dataset.sort(dim="y", inplace=True)
+                    dataset.history = "Sorted by date"
+                datasets = [dataset]
+
+            except DimensionsCompatibilityError as e:
+                warn(str(e))  # return only the list
+
+        return datasets
+
+
+def _importer_method(func):
+    # Decorator to define a given read function as belonging to Importer
+    setattr(Importer, func.__name__, staticmethod(func))
+    return func
+
+
+# --------------------------------------------------------------------------------------
+# Public Generic Read function
+# --------------------------------------------------------------------------------------
+
+_docstring.get_sections(
     """
-    Baseline Correction processor.
+See Also
+--------
+read : Generic reader inferring protocol from the filename extension.
+read_zip : Read Zip archives (containing spectrochempy readable files)
+read_dir : Read an entire directory.
+read_opus : Read OPUS spectra.
+read_labspec : Read Raman LABSPEC spectra (:file:`.txt`\ ).
+read_omnic : Read Omnic spectra (:file:`.spa`\ , :file:`.spg`\ , :file:`.srs`\ ).
+read_soc : Read Surface Optics Corps. files (:file:`.ddr` , :file:`.hdr` or :file:`.sdr`\ ).
+read_galactic : Read Galactic files (:file:`.spc`\ ).
+read_quadera : Read a Pfeiffer Vacuum's QUADERA mass spectrometer software file.
+read_topspin : Read TopSpin Bruker NMR spectra.
+read_csv : Read CSV files (:file:`.csv`\ ).
+read_jcamp : Read Infrared JCAMP-DX files (:file:`.jdx`\ , :file:`.dx`\ ).
+read_matlab : Read Matlab files (:file:`.mat`\ , :file:`.dso`\ ).
+read_carroucell : Read files in a directory after a carroucell experiment.
+""",
+    sections=["See Also"],
+    base="Importer",
+)
 
-    Two methods are proposed :
+_docstring.delete_params("Importer.see_also", "read")
 
-    - ``'sequential'`` (default) = classical polynom fit or spline
-      interpolation with separate fitting of each row (spectrum)
-    - ``'multivariate'`` = SVD modeling of baseline, polynomial fit of PC's
-      and calculation of the modeled baseline spectra.
 
-    Interactive mode is proposed using the interactive method `run` .
+@_docstring.dedent
+def read(*paths, **kwargs):
+    """
+    Generic read method.
+
+    This method is generally able to load experimental files based on extensions.
 
     Parameters
     ----------
-    dataset : `NDDataset`
-        The dataset to be transformed.
+    *paths : `str`, `~pathlib.Path` object objects or valid urls, optional
+        The data source(s) can be specified by the name or a list of name for the
+        file(s) to be loaded:
 
-    See Also
-    --------
-    abc : Automatic baseline correction.
-    BaselineCorrector : A helper widget to use in Jupyter notebooks
+        * *e.g.,* ( filename1, filename2, ...,  \*\*kwargs )*
 
-    Examples
-    --------
-    .. plot::
-        :include-source:
+        If the list of filenames are enclosed into brackets:
 
-        from spectrochempy import *
-        nd = NDDataset.read_omnic('irdata/nh4y-activation.spg')
-        ndp = nd[:, 1291.0:5999.0]
-        bc = BaselineCorrection(ndp)
-        ranges=[[5996., 5998.], [1290., 1300.],
-                [2205., 2301.], [5380., 5979.],
-                [3736., 5125.]]
-        span = bc.compute(*ranges,method='multivariate',
-                          interpolation='pchip', npc=8)
-        _ = bc.corrected.plot_stack()
-        show()
-    """
+        * *e.g.,* ( **[** *filename1, filename2, ...* **]**, \*\*kwargs *)*
 
-    dataset = NDDatasetType()
+        The returned datasets are merged to form a single dataset,
+        except if ``merge`` is set to `False`.
 
-    # hidden parameters (not passed in the constructor)
-    corrected = NDDatasetType()
-    method = Enum(
-        ["sequential", "multivariate"],
-        default_value="sequential",
-        help="Method used for baseline resolution.",
-    ).tag(config=True)
-    interpolation = Unicode(
-        "polynomial",
-    )
-    axis = Int(-1)
-    dim = Unicode("")
-    ranges = List(List(minlen=2, maxlen=2))
-    order = Int(1, min=1, allow_none=True)
-    npc = Int(5, min=1, allow_none=True)
-    zoompreview = Float(1.0)
-    figsize = Tuple((7, 5))
-    sps = List()
-
-    def __init__(self, dataset, **kwargs):
-
-        super().__init__(**kwargs)
-
-        self.dataset = dataset
-
-        self.corrected = self.dataset.copy()
-        if kwargs:
-            warning_(
-                "DEPRECATION WARNING: Pass all arguments such range, and method definition in the "
-                "`compute` method, not during the initialisation of the BaselineCorrection instance.\n"
-                "Here they are ignored."
-            )
-
-    def _extendranges(self, *ranges, **kwargs):
-        if not ranges:
-            # look in the kwargs
-            ranges = kwargs.pop("ranges", ())
-        if isinstance(ranges, tuple) and len(ranges) == 1:
-            ranges = ranges[0]  # probably passed with no start to the compute function
-        if not isinstance(ranges, (list, tuple)):
-            ranges = list(ranges)
-        if not ranges:
-            return
-
-        if len(ranges) == 2:
-            if isinstance(ranges[0], TYPE_INTEGER + TYPE_FLOAT) and isinstance(
-                ranges[1], TYPE_INTEGER + TYPE_FLOAT
-            ):
-                # a pair a values, we interpret this as a single range
-                ranges = [[ranges[0], ranges[1]]]
-        # find the single values
-        for item in ranges:
-            if isinstance(item, TYPE_INTEGER + TYPE_FLOAT):
-                # a single numerical value: interpret this as a single range
-                item = [item, item]
-            self.ranges.append(item)
-
-    def _setup(self, **kwargs):
-
-        self.method = kwargs.get("method", self.method)
-        self.interpolation = kwargs.get("interpolation", self.interpolation)
-        if self.interpolation == "polynomial":
-            self.order = int(kwargs.get("order", self.order))
-        if self.method == "multivariate":
-            self.npc = int(kwargs.get("npc", self.npc))
-        self.zoompreview = kwargs.get("zoompreview", self.zoompreview)
-        self.figsize = kwargs.get("figsize", self.figsize)
-
-    def __call__(self, *ranges, **kwargs):
-
-        return self.compute(*ranges, **kwargs)
-
-    def compute(self, *ranges, **kwargs):
-        """
-        Base function for dataset baseline correction.
-
-        Parameters
-        ----------
-        *ranges : a variable number of pair-tuples
-            The regions taken into account for the manual baseline correction.
-        **kwargs
-            Optional keyword parameters (see Other Parameters).
-
-        Other Parameters
-        ----------------
-        dim : str or int, keyword parameter, optional, default='x'.
-            Specify on which dimension to apply the apodization method.
-            If `dim` is specified as an integer
-            it is equivalent  to the usual `axis` numpy parameter.
-        method : str, keyword parameter, optional, default='sequential'
-            Correction method among ['multivariate','sequential']
-        interpolation : string, keyword parameter, optional, default='polynomial'
-            Interpolation method for the computation of the baseline,
-            among ['polynomial','pchip']
-        order : int, keyword parameter, optional, default=1
-            If the correction method polynomial,
-            this give the polynomial order to use.
-        npc : int, keyword parameter, optional, default=5
-            Number of components to keep for the `multivariate` method
-        zoompreview : float, keyword parameter, optional, default=1.0
-            The zoom factor for the preview in interactive mode
-        figsize : tuple, keyword parameter, optional, default=(8, 6)
-            Size of the figure to display in inch
-        """
-
-        self._setup(**kwargs)
-
-        # output dataset
-        new = self.corrected
-
-        # we assume that the last dimension
-        # if always the dimension to which we want to subtract the baseline.
-        # Swap the axes to be sure to be in this situation
-        axis, dim = new.get_axis(**kwargs, negative_axis=True)
-
-        swapped = False
-        if axis != -1:
-            new.swapdims(axis, -1, inplace=True)
-            swapped = True
-
-        lastcoord = new.coordset[dim]
-
-        # most of the time we need sorted axis, so let's do it now
-        is_descendant = False
-        if lastcoord.is_descendant:
-            new.sort(dim=dim, inplace=True, descend=False)
-            is_descendant = True
-            lastcoord = new.coordset[dim]
-
-        x = lastcoord.data
-        self.ranges = [[x[0], x[2]], [x[-3], x[-1]]]
-        self._extendranges(*ranges, **kwargs)
-        self.ranges = ranges = trim_ranges(*self.ranges)
-
-        baseline = np.zeros_like(new)
-
-        # Extract: Sbase: the matrix of data corresponding to ranges
-        #          xbase: the xaxis values corresponding to ranges
-
-        s = []
-        for pair in ranges:
-            # determine the slices
-
-            sl = slice(*pair)
-            sect = new[..., sl]
-            if sect is None:
-                continue
-
-            s.append(sect)
-
-        from spectrochempy.core.dataset.nddataset import NDDataset
-
-        sbase = NDDataset.concatenate(s, axis=-1)
-        # TODO: probably we could use masked data instead of concatenating - could be faster
-        xbase = sbase.coordset(dim)
-
-        if self.method == "sequential":
-
-            if self.interpolation == "polynomial":
-                # # bad fit when NaN values => are replaced by 0      # NO reason we have Nan -> suppressed
-                # if np.any(np.isnan(sbase)):
-                #     sbase[np.isnan(sbase)] = 0
+        If a source is not provided (*i.e.,* no ``paths`` , nor ``content``\ ),
+        a dialog box will be opened to select files.
+    %(kwargs)s
 
-                polycoef = np.polynomial.polynomial.polyfit(
-                    xbase.data, sbase.data.T, deg=self.order, rcond=None, full=False
-                )
-                baseline = np.polynomial.polynomial.polyval(x, polycoef)
+    Returns
+    -------
+    object : `NDDataset` or list of `NDDataset`
+        The returned dataset(s).
 
-            elif self.interpolation == "pchip":
-                for i in range(new.shape[0]):
-                    interp = scipy.interpolate.PchipInterpolator(
-                        xbase.data, sbase.data[i]
-                    )
-                    baseline[i] = interp(x)
+    Other Parameters
+    ----------------
+    protocol : `str`\ , optional
+        ``Protocol`` used for reading. It can be one of {``'scp'``\ , ``'omnic'``\ ,
+        ``'opus'``\ , ``'topspin'``\ , ``'matlab'``\ , ``'jcamp'``\ , ``'csv'``\ ,
+        ``'excel'``\ }. If not provided, the correct protocol
+        is inferred (whenever it is possible) from the filename extension.
+    directory : `~pathlib.Path` object objects or valid urls, optional
+        From where to read the files.
+    merge : `bool`\ , optional, default: `False`
+        If `True` and several filenames or a ``directory`` have been provided as
+        arguments, then a single `NDDataset` with merged (stacked along the first
+        dimension) is returned.
+    sortbydate : `bool`, optional, default: `True`
+        Sort multiple filename by acquisition date.
+    description : `str`, optional
+        A Custom description.
+    origin : one of {``'omnic'``\ , ``'tga'``\ }, optional
+        Used when reading with the CSV protocol. In order to properly interpret CSV file
+        it can be necessary to set the origin of the spectra.
+        Up to now only ``'omnic'`` and ``'tga'`` have been implemented.
+    csv_delimiter : `str`\ , optional, default: `~spectrochempy.preferences.csv_delimiter`
+        Set the column delimiter in CSV file.
+    content : `bytes` object, optional
+        Instead of passing a filename for further reading, a bytes content can be
+        directly provided as bytes objects.
+        The most convenient way is to use a dictionary. This feature is particularly
+        useful for a GUI Dash application to handle drag and drop of files into a
+        Browser.
+    iterdir : `bool`\ , optional, default: `True`
+        If `True` and no filename was provided, all files present in the provided
+        ``directory`` are returned (and merged if ``merge`` is `True`\ .
+        It is assumed that all the files correspond to current reading protocol.
+
+        .. versionchanged:: 0.6.2
+
+            ``iterdir`` replace the deprecated ``listdir`` argument.
+
+    recursive : `bool`, optional, default: `False`
+        Read also in subfolders.
+    replace_existing: `bool`, optional, default: `False`
+        Used only when url are specified. By default, existing files are not replaced
+        so not downloaded.
+    download_only: `bool`, optional, default: `False`
+        Used only when url are specified.  If True, only downloading and saving of the
+        files is performed, with no attempt to read their content.
+    read_only: `bool`, optional, default: `True`
+        Used only when url are specified.  If True, saving of the
+        files is performed in the current directory, or in the directory specified by
+        the directory parameter.
 
-        elif self.method == "multivariate":
+    See Also
+    --------
+    %(Importer.see_also.no_read)s
 
-            # SVD of Sbase
-            U, s, Vt = np.linalg.svd(sbase.data, full_matrices=False, compute_uv=True)
+    Examples
+    ---------
+    Reading a single OPUS file  (providing a windows type filename relative
+    to the default `~spectrochempy.preferences.datadir` )
 
-            # npc cannot be higher than the size of s
-            npc = min(self.npc, s.shape[0])
+    >>> scp.read('irdata\\\\OPUS\\\\test.0000')
+    NDDataset: [float64] a.u. (shape: (y:1, x:2567))
 
-            # select npc loadings & compute scores
-            Pt = Vt[0:npc]
-            T = np.dot(U[:, 0:npc], np.diag(s)[0:npc, 0:npc])
+    Reading a single OPUS file  (providing a unix/python type filename relative
+    to the default ``datadir`` )
+    Note that here read_opus is called as a classmethod of the NDDataset class
 
-            baseline_loadings = np.zeros((npc, new.shape[-1]))
+    >>> scp.read('irdata/OPUS/test.0000')
+    NDDataset: [float64] a.u. (shape: (y:1, x:2567))
 
-            if self.interpolation == "pchip":
-                for i in range(npc):
-                    interp = scipy.interpolate.PchipInterpolator(xbase.data, Pt[i])
-                    baseline_loadings[i] = interp(x)
+    Single file specified with pathlib.Path object
 
-            elif self.interpolation == "polynomial":
-                polycoef = np.polynomial.polynomial.polyfit(
-                    xbase.data, Pt.T, deg=self.order, rcond=None, full=False
-                )
+    >>> from pathlib import Path
+    >>> folder = Path('irdata/OPUS')
+    >>> p = folder / 'test.0000'
+    >>> scp.read(p)
+    NDDataset: [float64] a.u. (shape: (y:1, x:2567))
 
-                baseline_loadings = np.polynomial.polynomial.polyval(x, polycoef)
+    Multiple files not merged (return a list of datasets).
+    Note that a directory is specified
 
-            baseline = np.dot(T, baseline_loadings)
+    >>> le = scp.read('test.0000', 'test.0001', 'test.0002', directory='irdata/OPUS')
+    >>> len(le)
+    3
+    >>> le[0]
+    NDDataset: [float64] a.u. (shape: (y:1, x:2567))
 
-        new.data = new.data - baseline
+    Multiple files merged as the `merge` keyword is set to true
 
-        # eventually sort back to the original order
-        if is_descendant:
-            new.sort(axis=-1, inplace=True, descend=True)
+    >>> scp.read('test.0000', 'test.0001', 'test.0002', directory='irdata/OPUS', merge=True)
+    NDDataset: [float64] a.u. (shape: (y:3, x:2567))
 
-        new.history = "Baseline correction." + " Method: "
-        if self.method == "Multivariate":
-            new.history = "Multivariate (" + str(self.npc) + " PCs)."
-        else:
-            new.history = "Sequential."
+    Multiple files to merge : they are passed as a list instead of using the keyword
+    `merge`
 
-        if self.interpolation == "polynomial":
-            new.history = "Interpolation: Polynomial, order=" + str(self.order) + ".\n"
-        else:
-            new.history = "Interpolation: Pchip. \n"
+    >>> scp.read(['test.0000', 'test.0001', 'test.0002'], directory='irdata/OPUS')
+    NDDataset: [float64] a.u. (shape: (y:3, x:2567))
 
-        if swapped:
-            new = new.swapdims(axis, -1)
+    Multiple files not merged : they are passed as a list but `merge` is set to false
 
-        self.corrected = new
-        return new
+    >>> le = scp.read(['test.0000', 'test.0001', 'test.0002'], directory='irdata/OPUS', merge=False)
+    >>> len(le)
+    3
 
-    def show_regions(self, ax):
-        if self.sps:
-            for sp in self.sps:
-                sp.remove()
-        self.sps = []
-        self.ranges = list(trim_ranges(*self.ranges))
-        for x in self.ranges:
-            x.sort()
-            sp = ax.axvspan(x[0], x[1], facecolor="#2ca02c", alpha=0.5)
-            self.sps.append(sp)
-
-    def run(self, *ranges, **kwargs):
-        """
-        Interactive version of the baseline correction.
-
-        Parameters
-        ----------
-        *ranges : a variable number of pair-tuples
-            The regions taken into account for the manual baseline correction.
-        **kwargs
-            See other parameter of method compute.
-        """
-        self._setup(**kwargs)
-        self.sps = []
-
-        # output dataset
-        new = self.corrected
-        origin = self.dataset.copy()
-
-        # we assume that the last dimension if always the dimension to which we want to subtract the baseline.
-        # Swap the axes to be sure to be in this situation
-        axis, dim = new.get_axis(**kwargs, negative_axis=True)
-
-        # swapped = False
-        if axis != -1:
-            new.swapdims(axis, -1, inplace=True)
-            origin.swapdims(axis, -1, inplace=True)
-            # swapped = True
-
-        lastcoord = new.coordset[dim]
-
-        # most of the time we need sorted axis, so let's do it now
-
-        if lastcoord.reversed:
-            new.sort(dim=dim, inplace=True, descend=False)
-            lastcoord = new.coordset[dim]
-
-        x = lastcoord.data
-        self.ranges = [[x[0], x[2]], [x[-3], x[-1]]]
-        self._extendranges(*ranges, **kwargs)
-        self.ranges = ranges = trim_ranges(*self.ranges)
-
-        new = self.compute(*ranges, **kwargs)
-
-        # display
-        datasets = [origin, new]
-        labels = [
-            "Click on left button & Span to set regions. Click on right button on a region to remove it.",
-            "Baseline corrected dataset preview",
-        ]
-        axes = multiplot(
-            datasets,
-            labels,
-            method="stack",
-            sharex=True,
-            nrow=2,
-            ncol=1,
-            figsize=self.figsize,
-            suptitle="INTERACTIVE BASELINE CORRECTION",
-        )
+    Read without a filename. This has the effect of opening a dialog for file(s)
+    selection
 
-        fig = plt.gcf()
-        fig.canvas.draw()
+    >>> nd = scp.read()
 
-        ax1 = axes["axe11"]
-        ax2 = axes["axe21"]
+    Read in a directory (assume that only OPUS files are present in the directory
+    (else we must use the generic `read` function instead)
 
-        self.show_regions(ax1)
+    >>> le = scp.read(directory='irdata/OPUS')
+    >>> len(le)
+    2
 
-        def show_basecor(ax2):
-
-            corrected = self.compute(*ranges, **kwargs)
-
-            ax2.clear()
-            ax2.set_title(
-                "Baseline corrected dataset preview", fontweight="bold", fontsize=8
-            )
-            if self.zoompreview > 1:
-                zb = 1.0  # self.zoompreview
-                zlim = [corrected.data.min() / zb, corrected.data.max() / zb]
-                _ = corrected.plot_stack(ax=ax2, colorbar=False, zlim=zlim, clear=False)
-            else:
-                _ = corrected.plot_stack(ax=ax2, colorbar=False, clear=False)
+    Again we can use merge to stack all 4 spectra if thet have compatible dimensions.
+
+    >>> scp.read(directory='irdata/OPUS', merge=True)
+    [NDDataset: [float64] a.u. (shape: (y:1, x:5549)), NDDataset: [float64] a.u. (shape: (y:4, x:2567))]
+    """
 
-        show_basecor(ax2)
+    importer = Importer()
 
-        def onselect(xmin, xmax):
-            self.ranges.append([xmin, xmax])
-            self.show_regions(ax1)
-            show_basecor(ax2)
-            fig.canvas.draw()
-
-        def onclick(event):
-            if event.button == 3:
-                for i, r in enumerate(self.ranges):
-                    if r[0] > event.xdata or r[1] < event.xdata:
-                        continue
-                    else:
-                        self.ranges.remove(r)
-                        self.show_regions(ax1)
-                        show_basecor(ax2)
-                        fig.canvas.draw()  # _idle
-
-        _ = fig.canvas.mpl_connect("button_press_event", onclick)
-
-        _ = SpanSelector(
-            ax1,
-            onselect,
-            "horizontal",
-            minspan=5,
-            button=[1],
-            useblit=True,
-            props=dict(alpha=0.5, facecolor="blue"),
+    protocol = kwargs.get("protocol", None)
+    available_protocols = list(importer.protocols.values())
+    available_protocols.extend(
+        list(importer.alias.keys())
+    )  # to handle variants of protocols
+    if protocol is None:
+        kwargs["filetypes"] = list(importer.filetypes.values())
+        kwargs["protocol"] = "ALL"
+        default_filter = kwargs.get("default_filter", None)
+        if default_filter is not None:
+            kwargs["default_filter"] = importer.filetypes[default_filter]
+    else:
+        try:
+            kwargs["filetypes"] = [importer.filetypes[protocol]]
+        except KeyError:
+            raise ProtocolError(protocol, list(importer.protocols.values()))
+        except TypeError as e:
+            print(e)
+
+    # deprecated kwargs
+    listdir = kwargs.pop("listdir", True)
+    if "listdir" in kwargs and "iterdir" not in kwargs:
+        kwargs["iterdir"] = listdir
+        warning_(
+            "argument `listdir` is deprecated, use ìterdir` instead",
+            category=DeprecationWarning,
         )
 
-        fig.canvas.draw()
+    return importer(*paths, **kwargs)
 
-        return
 
+# for some reasons the doctring.getsection modify the signature of the function
+# when used as a decorator, so we use it as a function
+_docstring.get_sections(
+    read.__doc__,
+    sections=["Parameters", "Other Parameters", "Returns"],
+    base="Importer",
+)
+
+_docstring.delete_params("Importer.see_also", "read_dir")
 
-def basc(dataset, *ranges, **kwargs):
+
+@_docstring.dedent
+def read_dir(directory=None, **kwargs):
     """
-    Compute a baseline correction using the BaselineCorrection processor.
+    Read an entire directory.
 
-    2 methods are proposed :
+    Open a list of readable files in a and store data/metadata in a dataset or a list of
+    datasets according to the following rules :
 
-    * `sequential` (default) = classical polynom fit or spline
-      interpolation with separate fitting of each row (spectrum)
-    * `multivariate` = SVD modeling of baseline, polynomial fit of PC's
-      and calculation of the modelled baseline spectra.
+    * 2D spectroscopic data (e.g. valid .spg files or matlab arrays, etc...) from
+      distinct files are stored in distinct `NDdataset`\ s.
+    * 1D spectroscopic data (e.g., :file:`.spa` files) in a given directory are merged
+      into single `NDDataset`\ , providing their unique dimension are compatible.
+      If not, an error is generated.
+    * non-readable files are ignored
 
     Parameters
     ----------
-    dataset : a [NDDataset| instance
-        The dataset where to calculate the baseline.
-    \*ranges : a variable number of pair-tuples
-        The regions taken into account for the manual baseline correction.
-    **kwargs
-        Optional keyword parameters (see Other Parameters).
+    directory : str or pathlib
+        Folder where are located the files to read.
 
-    Other Parameters
-    ----------------
-    dim : str or int, keyword parameter, optional, default: 'x'.
-        Specify on which dimension to apply the apodization method.
-        If `dim` is specified as an integer
-        it is equivalent  to the usual `axis` numpy parameter.
-    method : str, keyword parameter, optional, default: 'sequential'
-        Correction method among ['multivariate','sequential']
-    interpolation : string, keyword parameter, optional, default='polynomial'
-        Interpolation method for the computation of the baseline,
-        among ['polynomial','pchip']
-    order : int, keyword parameter, optional, default: 6
-        If the correction method polynomial, this give the polynomial order to use.
-    npc : int, keyword parameter, optional, default: 5
-        Number of components to keep for the `multivariate` method
+    Returns
+    --------
+    %(Importer.returns)s
+        Depending on the python version, the order of the datasets in the list
+        may change.
 
     See Also
     --------
-    BaselineCorrection : Manual baseline corrections.
-    abc : Automatic baseline correction.
+    %(Importer.see_also.no_read_dir)s
+
+    Examples
+    --------
 
-    Notes
-    -----
-    For more flexibility and functionality, it is advised to use the BaselineCorrection
-    processor instead.
+    >>> scp.preferences.csv_delimiter = ','
+    >>> A = scp.read_dir('irdata')
+    >>> len(A)
+    4
+
+    >>> B = scp.read_dir()
     """
-    blc = BaselineCorrection(dataset)
-    if not ranges and dataset.meta.regions is not None:
-        # use the range stored in metadata
-        ranges = dataset.meta.regions["baseline"]
-    return blc.compute(*ranges, **kwargs)
+    kwargs["iterdir"] = True
+    importer = Importer()
+    return importer(directory, **kwargs)
 
 
+# _docstring.delete_params("Importer.see_also", "read_remote")
+# @_docstring.dedent
+# def read_remote(file_or_dir, **kwargs):
+#     """
+#     Download and read files or an entire directory from any url
+#
+#     The first usage in spectrochempy is the loading of test files in the
+#     `spectrochempy_data repository <https://github.com/spectrochempy/spectrochempy_data>`__\ .
+#     This is done only if the data are not yet
+#     downloaded and present in the `~spectrochempy.preferences.datadir` directory.
+#
+#     It can also be used to download and read file or directory from any url.
+#
+#     Parameters
+#     ----------
+#     path : `str`, `~pathlib.Path` object or an url.
+#         When a file or folder is specified, it must be written as if it were present
+#         locally exactly as for the `read` function. The correponding file or directory
+#         is downloaded from the ``github spectrochemp_data`` repository.
+#         Otherwise it should be a full and valid url.
+#     %(kwargs)s
+#
+#     Returns
+#     --------
+#     %(Importer.returns)s
+#
+#     Other Parameters
+#     ----------------
+#     %(Importer.other_parameters)s
+#
+#     See Also
+#     --------
+#     %(Importer.see_also.no_read_remote)s
+#
+#     Examples
+#     --------
+#
+#     >>> A = scp.read_remote('irdata/subdir')
+#     """
+#     kwargs["remote"] = True
+#     importer = Importer()
+#     return importer(file_or_dir, **kwargs)
+#
+
 # ======================================================================================
-# abc # TODO: some work to perform on this
+# Private read functions
 # ======================================================================================
-def abc(dataset, dim=-1, **kwargs):
-    """
-    Automatic baseline correction.
+@_importer_method
+def _read_dir(*args, **kwargs):
+    _, directory = args
+    directory = get_directory_name(directory)
+    files = get_filenames(directory, **kwargs)
+    datasets = []
+    valid_extensions = list(zip(*FILETYPES))[0] + list(zip(*ALIAS))[0]
+    for key in [key for key in files.keys() if key[1:] in valid_extensions]:
+        if key:
+            importer = Importer()
+            nd = importer(files[key], **kwargs)
+            if nd is not None:
+                if not isinstance(nd, list):
+                    nd = [nd]
+                datasets.extend(nd)
+    return datasets
+
+
+@_importer_method
+def _read_scp(*args, **kwargs):
+    dataset, filename = args
+    return dataset.load(filename, **kwargs)
+
+
+@_importer_method
+def _read_(*args, **kwargs):
+    dataset, filename = args
+
+    if kwargs.pop("remote", False):
+        return Importer._read_remote(*args, **kwargs)
+    elif not filename or filename.is_dir():
+        return Importer._read_dir(*args, **kwargs)
+    else:
+        raise FileNotFoundError
 
-    Various algorithms are provided to calculate the baseline automatically.
+    # protocol = kwargs.get("protocol", None)
+    # if protocol and ".scp" in protocol:
+    #     return dataset.load(filename, **kwargs)
+    #
+    # elif filename and filename.name in ("fid", "ser", "1r", "2rr", "3rrr"):
+    #     # probably an Topspin NMR file
+    #     return dataset.read_topspin(filename, **kwargs)
+    # elif filename:
+    #     # try scp format
+    #     try:
+    #         return dataset.load(filename, **kwargs)
+    #     except Exception:
+    #         # lets try some common format
+    #         for key in ["omnic", "opus", "topspin", "labspec", "matlab", "jdx"]:
+    #             try:
+    #                 _read = getattr(dataset, f"read_{key}")
+    #                 f = f"{filename}.{key}"
+    #                 return _read(f, **kwargs)
+    #             except Exception:
+    #                 pass
+    #         raise NotImplementedError
 
-    Parameters
-    ----------
-    dataset : a [NDDataset| instance
-        The dataset where to calculate the baseline.
-    dim : str or int, optional
-        The dataset dimentsion where to calculate the baseline. Default is -1.
-    **kwargs
-        Optional keyword parameters (see Other Parameters).
 
-    Returns
-    -------
-    baseline_corrected
-        A baseline corrected dataset.
-    baseline_only
-        Only the baseline (apply must be set to False).
-    baseline_points
-        Points where the baseline is calculated (return_points must be set to True).
+# ======================================================================================
+# Private functions
+# ======================================================================================
+def _is_url(filename):
+    return (
+        isinstance(filename, str)
+        and re.match(r"http[s]?:[\/]{2}", filename) is not None
+    )
 
-    Other Parameters
-    ----------------
-    basetype : string, optional, default: 'linear'
-        See notes - available = linear, basf, ...
-    window : float/int, optional, default is 0.05
-        If float <1 then the corresponding percentage of the axis size is taken as window.
-    nbzone : int, optional, default is 32
-        Number of zones. We will divide the size of the last axis by this number
-        to determine the number of points in each zone (nw).
-    mult : int
-        A multiplicator. determine the number of point for the database calculation (nw*mult<n base points).
-    nstd : int, optional, default is 2 times the standard error
-        Another multiplicator. Multiply the standard error to determine the region in which points are from the
-        baseline.
-    polynom : bool, optional, default is True
-        If True a polynom is computed for the base line, else an interpolation is achieved betwwen points.
-    porder : int, default is 6
-        Order of the polynom to fit on the baseline points
-    return_points : bool, optional, default is False
-        If True, the points abscissa used to determine the baseline are returned.
-    apply : bool, optional, default is True
-        If apply is False, the data are not modified only the baseline is returned.
-    return_pts : bool, optional, default is False
-        If True, the baseline reference points are returned.
 
-    See Also
-    --------
-    BaselineCorrection : Manual baseline corrections.
-    basc : Manual baseline correction.
+def _openfid(filename, mode="rb", **kwargs):
+    # Return a file ID
 
-    Notes
-    -----
-    #TODO: description of these algorithms
-    * linear -
-    * basf -
+    # Check if Content has been passed?
+    content = kwargs.get("content", False)
 
-    Examples
-    --------
-    To be done
-    """
-    # # options evaluation
-    # parser = argparse.ArgumentParser(description='BC processing.', usage="""
-    # ab [-h] [--mode {linear,poly, svd}] [--dryrun]
-    #                        [--window WINDOW] [--step STEP] [--nbzone NBZONE]
-    #                        [--mult MULT] [--order ORDER] [--verbose]
-    # """)
-    # # positional arguments
-    # parser.add_argument('--mode', '-mo', default='linear',
-    #                      choices=['linear', 'poly', 'svd'], help="mode of correction")
-    # parser.add_argument('--dryrun', action='store_true', help='dry flag')
-    #
-    # parser.add_argument('--window', '-wi', default=0.05, type=float, help='selected window for linear and svd bc')
-    # parser.add_argument('--step', '-st', default=5, type=int, help='step for svd bc')
-    # parser.add_argument('--nbzone', '-nz', default=32, type=int, help='number of zone for poly')
-    # parser.add_argument('--mult', '-mt', default=4, type=int, help='multiplicator of zone for poly')
-    # parser.add_argument('--order', '-or', default=5, type=int, help='polynom order for poly')
-    #
-    # parser.add_argument('--verbose', action='store_true', help='verbose flag')
-    # args = parser.parse_args(options.split())
-    #
-    # source.history.append('baseline correction mode:%s' % args.mode)
+    # default encoding
+    encoding = "utf-8"
 
-    inplace = kwargs.pop("inplace", False)
-    dryrun = kwargs.pop("dryrun", False)
+    if _is_url(filename):
+        # by default we set the read_only flag to True when reading remote url
+        kwargs["read_only"] = kwargs.get("read_only", True)
+
+        # use request to read the remote content
+        r = requests.get(filename, allow_redirects=True)
+        r.raise_for_status()
+        content = r.content
+        encoding = r.encoding
 
-    # output dataset inplace or not
-    if not inplace or dryrun:  # default
-        new = dataset.copy()
     else:
-        new = dataset
-
-    axis, dim = new.get_axis(dim, negative_axis=True)
-    swapped = False
-    if axis != -1:
-        new.swapdims(axis, -1, inplace=True)  # must be done in  place
-        swapped = True
-
-    base = _basecor(new.data.real, **kwargs)
+        # Transform filename to a Path object is not yet the case
+        filename = pathclean(filename)
 
-    if not dryrun:
-        new.data -= base  # return the corrected spectra
+    # Create the file ID
+    if content:
+        # if a content has been passed, then it has priority
+        fid = (
+            io.BytesIO(content)
+            if mode == "rb"
+            else io.StringIO(content.decode(encoding))
+        )
     else:
-        new.data = base  # return the baseline
+        fid = open(filename, mode=mode)
 
-    # restore original data order if it was swapped
-    if swapped:
-        new.swapdims(axis, -1, inplace=True)  # must be done inplace
+    return fid, kwargs
 
-    new.history = "`abc` Baseline correction applied."
-    return new
 
+def _write_downloaded_file(content, dst):
+    if not dst.parent.exists():
+        # create the eventually missing subdirectory
+        dst.parent.mkdir(parents=True, exist_ok=True)
+    dst.write_bytes(content)
+    info_(f"{dst.name} has been downloaded and written in {dst.parent}")
 
-def ab(dataset, dim=-1, **kwargs):
-    """
-    Alias of `abc` .
-    """
-    return abs(dataset, dim, **kwargs)
 
+def _get_url_content_and_save(url, dst, replace, read_only=False):
 
-@_units_agnostic_method
-def dc(dataset, **kwargs):
-    """
-    Time domain baseline correction.
+    if not replace and dst.exists():
+        return
 
-    Parameters
-    ----------
-    dataset : nddataset
-        The time domain daatset to be corrected.
-    kwargs : dict, optional
-        Additional parameters.
+    try:
+        r = requests.get(url, allow_redirects=True)
 
-    Returns
-    -------
-    dc
-        DC corrected array.
+        r.raise_for_status()
 
-    Other Parameters
-    ----------------
-    len : float, optional
-        Proportion in percent of the data at the end of the dataset to take into account. By default, 25%.
-    """
+        # write downloaded file
+        if not read_only:
+            _write_downloaded_file(r.content, dst)
 
-    len = int(kwargs.pop("len", 0.25) * dataset.shape[-1])
-    dc = np.mean(np.atleast_2d(dataset)[..., -len:])
-    dataset -= dc
+        # in all case return the content
+        return r.content
 
-    return dataset
+    except OSError:
+        raise FileNotFoundError(f"Not found locally or at url:{url}")
 
 
-# ======================================================================================
-# private functions
-# ======================================================================================
-def _basecor(data, **kwargs):
-    mode = kwargs.pop("mode", "linear")
+def _download_full_testdata_directory():
+    from spectrochempy.core import preferences as prefs
 
-    if mode == "linear":
-        return _linearbase(data, **kwargs)
+    datadir = prefs.datadir
 
-    if mode == "svd":
-        return _svdbase(data, **kwargs)
+    url = "https://github.com/spectrochempy/spectrochempy_data/archive/refs/heads/master.zip"
 
-    if mode == "poly":
-        return _polybase(data, **kwargs)
-    else:
-        raise ValueError(f"`ab` mode = `{mode}`  not known")
+    resp = requests.get(url)
+    zipfile = ZipFile(io.BytesIO(resp.content))
+    files = [zipfile.open(file_name) for file_name in zipfile.namelist()]
 
+    for file in files:
+        name = file.name
+        if name.endswith("/") or "testdata/" not in name:  # dir
+            continue
+        uncompressed = zipfile.read(name)
+        p = list(pathclean(name).parts)[2:]
+        dst = datadir.joinpath("/".join(p))
+        _write_downloaded_file(uncompressed, dst)
 
-#
-# _linear mode
-#
-def _linearbase(data, **kwargs):
-    # Apply a linear baseline correction
-    # Very simple and naive procedure that compute a straight baseline from side to the other
-    # (averging on a window given by the window parameters : 5% of the total width on each side by default)
-
-    window = kwargs.pop("window", 0.05)
-
-    if window <= 1.0:
-        # percent
-        window = int(data.shape[-1] * window)
-
-    if len(data.shape) == 1:
-        npts = float(data.shape[-1])
-        a = (data[-window:].mean() - data[:window].mean()) / (npts - 1.0)
-        b = data[:window].mean()
-        baseline = a * np.arange(npts) + b
 
-    else:
-        npts = float(data.shape[-1])
-        a = (data[:, -window:].mean(axis=-1) - data[:, :window].mean(axis=-1)) / (
-            npts - 1.0
-        )
-        b = data[:, :window].mean(axis=-1)
-        baseline = (((np.ones_like(data).T * a).T * np.arange(float(npts))).T + b).T
+def _download_from_github(path, dst, replace=False):
+    # download on github (always save the downloaded files)
+    relative_path = str(pathclean(path).as_posix())
+    path = (
+        f"https://github.com/spectrochempy/spectrochempy_data/raw/master/"
+        f"testdata/{relative_path}"
+    )
 
-    return baseline
+    # first determine if it is a directory
+    r = requests.get(path + "/__index__", allow_redirects=True)
+    index = None
+    if r.status_code == 200:
+        index = yaml.load(r.content, Loader=yaml.CLoader)
 
+    if index is None:
+        return _get_url_content_and_save(path, dst, replace)
 
-def _planeFit(points):
-    # p, n = planeFit(points)  # copied from https://stackoverflow.com/a/18968498
-    #
-    # Fit an multi-dimensional plane to the points.
-    # Return a point on the plane and the normal.
-    #
-    # Parameters
-    # ----------
-    # points :
-    #
-    # Notes
-    # -----
-    #     Replace the nonlinear optimization with an SVD.
-    #     The following creates the moment of inertia tensor, M, and then
-    #     SVD's it to get the normal to the plane.
-    #     This should be a close approximation to the least-squares fit
-    #     and be much faster and more predictable.
-    #     It returns the point-cloud center and the normal.
-
-    from numpy.linalg import svd
-
-    npts = points.shape[0]
-    points = np.reshape(points, (npts, -1))
-    assert points.shape[0] < points.shape[1]
-    ctr = points.mean(axis=1)
-    x = points - ctr[:, None]
-    M = np.dot(x, x.T)
-    return ctr, svd(M)[0][:, -1]
-
-
-def _svdbase(data, args=None, retw=False):
-    # Apply a planar baseline correction to 2D data
-    import pandas as pd  # TODO: suppress this need
-
-    if not args:
-        window = 0.05
-        step = 5
     else:
-        window = args.window
-        step = args.step
-
-    if window <= 1.0:
-        # percent
-        window = int(data.shape[-1] * window)
-
-    data = pd.DataFrame(
-        data
-    )  # TODO: facilitate the manipulation (but to think about further)
-    a = pd.concat([data.iloc[:window], data.iloc[-window:]])
-    b = pd.concat(
-        [data.iloc[window:-window, :window], data.iloc[window:-window, -window:]],
-        axis=1,
+        # download folder
+        for filename in index["files"]:
+            _get_url_content_and_save(f"{path}/{filename}", dst / filename, replace)
+        for folder in index["folders"]:
+            _download_from_github(f"{relative_path}/{folder}", dst / folder)
+
+
+def _is_relative_to(path, base):
+    # try to emulate the pathlib is_relative_to method which does not work on python
+    # 3.7 (needed for Colab!)
+    # TODO: replace as Colab is updated to 3.9
+    pparts = path.parts
+    bparts = base.parts
+    if bparts[-1] in pparts:
+        idx = pparts.index(bparts[-1])
+        pparts_base = pparts[: idx + 1]
+        return pparts_base == bparts
+    return False
+
+
+def _relative_to(path, base):
+    pparts = path.parts
+    bparts = base.parts
+    if bparts[-1] in pparts:
+        idx = pparts.index(bparts[-1])
+        return pathclean("/".join(pparts[idx + 1 :]))
+    raise ValueError(
+        f"'{path}' is not in the subpath of '{base}' OR one path is "
+        f"relative and the other absolute."
     )
-    bs = pd.concat([a, b])
-    bs = bs.stack()
-    bs.sort()
-    x = []
-    y = []
-    z = []
-    for item in bs.index[::step]:
-        x.append(item[0])
-        y.append(item[1])
-        z.append(bs[item].real)
-
-    norm = np.max(np.abs(z))
-    z = np.array(z)
-    z = z / norm
-    XYZ = np.array((x, y, z))
-    p, n = _planeFit(XYZ)
-    d = np.dot(p, n)
-
-    col = data.columns
-    row = data.index
-    X, Y = np.meshgrid(col, row)
-    Z = -norm * (n[0] * X + n[1] * Y - d) / n[2]
-
-    if retw:
-        return Z, None  # TODO: return something
-    return Z
-
-
-def _polybase(data, **kwargs):
-    # Automatic baseline correction
-
-    if data.ndim == 1:
-        dat = np.array(
-            [
-                data,
-            ]
-        )
 
-    nbzone = kwargs.pop("nbzone", 64)
-    mult = kwargs.pop("mult", 4)
-    order = kwargs.pop("order", 6)
-
-    npts = data.shape[-1]
-    w = np.arange(npts)
-
-    baseline = np.ma.masked_array(dat, mask=True)
-    sigma = 1.0e6
-    nw = int(npts / nbzone)
-
-    # print (nw)
-    # unmask extremities of the baseline
-    baseline[:, :nw].mask = False
-    baseline[:, -nw:].mask = False
-
-    for j in range(nbzone):
-        s = dat[:, nw * j : min(nw * (j + 1), npts + 1)]
-        sigma = min(s.std(), sigma)
-
-    nw = nw * 2  # bigger window
-    nw2 = int(nw / 2)
-
-    found = False
-    nb = 0
-    nstd = 2.0
-    while (not found) or (nb < nw * mult):
-        nb = 0
-        for i in range(nw2, npts - nw2 + 1, 1):
-            s1 = dat[:, max(i - 1 - nw2, 0) : min(i - 1 + nw2, npts + 1)]
-            s2 = dat[:, max(i - nw2, 0) : min(i + nw2, npts + 1)]
-            s3 = dat[:, max(i + 1 - nw2, 0) : min(i + 1 + nw2, npts + 1)]
-            mi1, mi2, mi3 = s1.min(), s2.min(), s3.min()
-            ma1, ma2, ma3 = s1.max(), s2.max(), s3.max()
-
-            if (
-                abs(ma1 - mi1) < float(nstd) * sigma
-                and abs(ma2 - mi2) < float(nstd) * sigma
-                and abs(ma3 - mi3) < float(nstd) * sigma
-            ):
-                found = True
-                nb += 1
-                baseline[:1, i].mask = False  # baseline points
-
-        # increase nstd
-        nstd = nstd * 1.1
-    debug_("basf optimized nstd: %.2F mult: %.2f" % (nstd, mult))
-
-    wm = np.array(list(zip(*np.argwhere(~baseline[:1].mask)))[1])
-    bm = baseline[:, wm]
-    if data.ndim > 1:
-        bm = smooth(bm.T, max(int(dat.shape[0] / 10), 3)).T
-    bm = smooth(bm, max(int(dat.shape[-1] / 10), 3))
-
-    # if not polynom:
-    #    sr = pchip(wm, bm.real)
-    #    si = pchip(wm, bm.imag)
-    #    baseline = sr(w) + si(w) * 1.0j
-    #    baseline = smooth(baseline, window_len=int(nw / 4))
-    # else:
-    # fit a polynom
-    pf = np.polyfit(wm, bm.T, order).T
-    for i, row in enumerate(pf[:]):
-        poly = np.poly1d(row)
-        baseline[i] = poly(w)
 
-    if data.ndim == 1:
-        baseline = baseline[0]
+@_importer_method
+def _read_remote(*args, **kwargs):
+    from spectrochempy.core import preferences as prefs
+
+    datadir = prefs.datadir
+    dataset, path = args
+    kwargs["merge"] = kwargs.get("merge", False)  # by default, no attempt to merge
+    read_method = kwargs.pop("read_method", read)
+    download_only = kwargs.pop("download_only", False)
+    replace = kwargs.pop(
+        "replace_existing", False
+    )  # by default we download only if needed.
+
+    # downloaded file
+    # we try to download the github testdata
+    path = pathclean(path)
+
+    # we need to download additional files for topspin
+    topspin = True if "topspin" in read_method.__name__ else False
+    # we have to treat a special case: topspin, where the parent directory need
+    # to be downloaded with the required file
+    if topspin:
+        savedpath = path
+        m = re.match(r"(.*)(\/pdata\/\d+\/\d+[r|i]{1,2}|ser|fid)", str(path))
+        if m is not None:
+            path = pathclean(m[1])
+
+    if _is_relative_to(path, datadir):
+        # try to make it relative for remote downloading on github
+        relative_path = _relative_to(path, datadir)
+    else:
+        # assume it is already relative
+        relative_path = path
+
+    # Try to download it
+    dst = datadir / relative_path
+    if dst.name == "testdata":
+        # we are going to download the whole testdata directory
+        # -> use a faster method
+        _download_full_testdata_directory()
+        return
+    else:
+        content = _download_from_github(relative_path, dst, replace)
 
-    return baseline
+    if not download_only:
+        if content is None:
+            if topspin:
+                return read_method(
+                    dataset, dst / _relative_to(savedpath, dst), **kwargs
+                )
+            else:
+                return read_method(dataset, dst, **kwargs)
+        else:
+            return read_method(dataset, dst, content=content, **kwargs)
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/processors/concatenate.py` & `spectrochempy-0.6.6/spectrochempy/processing/transformation/concatenate.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/core/processors/fft.py` & `spectrochempy-0.6.6/spectrochempy/processing/fft/fft.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 import re
 
 import numpy as np
 from quaternion import as_float_array
 from scipy.signal import hilbert
 
-from spectrochempy.core import error_
+from spectrochempy.application import error_
 from spectrochempy.core.dataset.coord import Coord
-from spectrochempy.core.processors.utils import _units_agnostic_method
-from spectrochempy.core.processors.zero_filling import zf_size
 from spectrochempy.core.units import ur
+from spectrochempy.processing.fft.zero_filling import zf_size
+from spectrochempy.utils.decorators import _units_agnostic_method
 from spectrochempy.utils.misc import (
     as_quaternion,
     get_component,
     largest_power_of_2,
     typequaternion,
 )
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/processors/integrate.py` & `spectrochempy-0.6.6/spectrochempy/analysis/integration/integrate.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/core/processors/interpolate.py` & `spectrochempy-0.6.6/spectrochempy/processing/interpolation/interpolate.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 
 
 # import scipy.interpolate
 # import numpy as np
 
 # from ...utils import NOMASK, MASKED, UnitsCompatibilityError
 # from spectrochempy.extern.orderedset import OrderedSet
-# from spectrochempy.core import warning_, error_
+# from spectrochempy.application import warning_, error_
 
 
 def interpolate(dataset, axis=0, size=None):
     # TODO: a simple interpolator of the data (either to reduce
     #      or increase number of points in every dimension)
     raise NotImplementedError("Not yet implemented")
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/processors/phasing.py` & `spectrochempy-0.6.6/spectrochempy/processing/fft/phasing.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 __all__ = ["pk", "pk_exp"]
 __dataset_methods__ = __all__
 
 import functools
 
 import numpy as np
 
-from spectrochempy.core import error_
+from spectrochempy.application import error_
 from spectrochempy.core.units import Quantity, ur
 
 pi = np.pi
 
 
 # ======================================================================================
 # Decorators
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/processors/shift.py` & `spectrochempy-0.6.6/spectrochempy/processing/fft/shift.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 """
 A collection of NMR spectral processing functions which operate on the last
 dimension (1) of 2D arrays.
 
 Adapted from NMRGLUE proc_base (New BSD License)
 """
 
-__all__ = ["rs", "ls", "roll", "cs", "fsh", "fsh2"]
+__all__ = ["rs", "ls", "roll", "cs", "fsh", "fsh2", "dc"]
 __dataset_methods__ = __all__
 
 import numpy as np
 
-from spectrochempy.core.processors.utils import _units_agnostic_method
+from spectrochempy.utils.decorators import _units_agnostic_method
 
 pi = np.pi
 
 
 # ======================================================================================
 # Public methods
 # ======================================================================================
@@ -208,15 +208,15 @@
     inplace : bool, keyword parameter, optional, default=False
         True if we make the transform inplace.  If False, the function return a new dataset.
 
     See Also
     --------
     ls, rs, cs, roll, fsh2
     """
-    from spectrochempy.core.processors.fft import _fft, _ifft
+    from spectrochempy.processing.fft.fft import _fft, _ifft
 
     s = float(dataset.shape[-1])
 
     data = _ifft(dataset)
     data = np.exp(-2.0j * pi * pts * np.arange(s) / s) * data
     data = _fft(data)
 
@@ -253,16 +253,46 @@
         True if we make the transform inplace.  If False, the function return a new dataset.
 
     See Also
     --------
     ls, rs, cs, roll, fsh2
     """
 
-    from spectrochempy.core.processors.fft import _fft_positive, _ifft_positive
+    from spectrochempy.processing.fft.fft import _fft_positive, _ifft_positive
 
     s = float(dataset.shape[-1])
 
     data = _ifft_positive(dataset)
     data = np.exp(2.0j * pi * pts * np.arange(s) / s) * data
     data = _fft_positive(data)
 
     return data
+
+
+@_units_agnostic_method
+def dc(dataset, **kwargs):
+    """
+    Time domain baseline correction.
+
+    Parameters
+    ----------
+    dataset : nddataset
+        The time domain daatset to be corrected.
+    kwargs : dict, optional
+        Additional parameters.
+
+    Returns
+    -------
+    dc
+        DC corrected array.
+
+    Other Parameters
+    ----------------
+    len : float, optional
+        Proportion in percent of the data at the end of the dataset to take into account. By default, 25%.
+    """
+
+    len = int(kwargs.pop("len", 0.25) * dataset.shape[-1])
+    dc = np.mean(np.atleast_2d(dataset)[..., -len:])
+    dataset -= dc
+
+    return dataset
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/processors/zero_filling.py` & `spectrochempy-0.6.6/spectrochempy/processing/fft/zero_filling.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 __dataset_methods__ = __all__
 
 import functools
 
 import numpy as np
 
-from spectrochempy.core import error_
+from spectrochempy.application import error_
 from spectrochempy.utils.misc import largest_power_of_2
 
 
 # ======================================================================================
 # Decorators
 # ======================================================================================
 def _zf_method(method):
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/project/abstractproject.py` & `spectrochempy-0.6.6/spectrochempy/core/project/abstractproject.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/core/project/project.py` & `spectrochempy-0.6.6/spectrochempy/core/project/project.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/core/readers/download.py` & `spectrochempy-0.6.6/spectrochempy/core/readers/download.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,118 +4,66 @@
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
 In this module, methods are provided to download external datasets
 from public database.
 """
-__all__ = ["download_iris", "download_nist_ir"]
+__all__ = ["load_iris", "download_nist_ir"]
 __dataset_methods__ = __all__
 
-from io import StringIO
 from pathlib import Path
 
-import numpy as np
 import requests
 
-from spectrochempy.core import error_, info_
+from spectrochempy.application import error_, info_
 from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.core.dataset.nddataset import NDDataset
 from spectrochempy.core.readers.read_jcamp import read_jcamp
 from spectrochempy.utils.misc import is_iterable
-from spectrochempy.utils.optional import import_optional_dependency
 
 
-def download_iris():
+def load_iris():
     """
     Upload the classical "iris" dataset.
 
-    The "IRIS" dataset is a classical example for machine learning.It is downloaded from
-    the
-    [UCI distant repository](https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data)
+    The "IRIS" dataset is a classical example for machine learning.
+    It is read from the `scikit-learn` package.
 
     Returns
     -------
     dataset
         The `IRIS` dataset.
 
     See Also
     --------
     read : Read data from experimental data.
     """
-    url = "https://archive.ics.uci.edu/ml/machine-learning-databases/iris/iris.data"
+    from sklearn.datasets import load_iris as sklearn_iris
 
-    try:
-        connection = True
-        response = requests.get(url, stream=True, timeout=10)
-    except OSError:
-        error_(OSError, "Cannot connect to the UCI repository. Try Scikit-Learn")
-        connection = False
-
-    if connection:  # Download data
-        txtdata = ""
-        for rd in response.iter_content():
-            txtdata += rd.decode("utf8")
-
-        fil = StringIO(txtdata)
-        try:
-            data = np.loadtxt(fil, delimiter=",", usecols=range(4))
-            fil.seek(0)
-            labels = np.loadtxt(fil, delimiter=",", usecols=(4,), dtype="|S")
-            labels = list((lab.decode("utf8") for lab in labels))
-        except Exception:
-            raise OSError("can't read JCAMP file")
-
-        coordx = Coord(
-            labels=["sepal_length", "sepal width", "petal_length", "petal_width"],
-            title="features",
-        )
-        coordy = Coord(labels=labels, title="samples")
-
-        new = NDDataset(
-            data,
-            coordset=[coordy, coordx],
-            title="size",
-            name="`IRIS` Dataset",
-            units="cm",
-        )
-
-        new.history = "Loaded from UC Irvine machine learning repository"
-
-        return new
-
-    else:
-        # Cannot download - use the scikit-learn dataset (if scikit-learn is installed)
-
-        sklearn = import_optional_dependency("sklearn", errors="ignore")
-        if sklearn is None:
-            raise OSError("Failed in uploading the `IRIS` dataset!")
-        else:
-            from sklearn import datasets
-
-        data = datasets.load_iris()
+    data = sklearn_iris()
 
-        coordx = Coord(
-            labels=["sepal_length", "sepal width", "petal_length", "petal_width"],
-            title="features",
-        )
-        labels = [data.target_names[i] for i in data.target]
-        coordy = Coord(labels=labels, title="samples")
-
-        new = NDDataset(
-            data.data,
-            coordset=[coordy, coordx],
-            title="size",
-            name="`IRIS` Dataset",
-            units="cm",
-        )
+    coordx = Coord(
+        labels=["sepal_length", "sepal width", "petal_length", "petal_width"],
+        title="features",
+    )
+    labels = [data.target_names[i] for i in data.target]
+    coordy = Coord(labels=labels, title="samples")
+
+    new = NDDataset(
+        data.data,
+        coordset=[coordy, coordx],
+        title="size",
+        name="`IRIS` Dataset",
+        units="cm",
+    )
 
-        new.history = "Loaded from scikit-learn datasets"
+    new.history = "Loaded from scikit-learn datasets"
 
-        return new
+    return new
 
 
 def download_nist_ir(CAS, index="all"):
     """
     Upload IR spectra from NIST webbook
 
     Parameters
@@ -152,16 +100,15 @@
                 response = requests.get(url, timeout=10)
                 if b"Spectrum not found" in response.content[:30]:
                     break
                 else:
                     index.append(i)
                     i += 1
             except OSError:
-                error_("OSError: could not connect to NIST")
-                return None
+                raise OSError("Cannot connect to the NIST server... ")
 
         if len(index) == 0:
             error_(IOError, "NIST IR: no spectrum found")
             return
         elif len(index) == 1:
             info_("NIST IR: 1 spectrum found")
         else:
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/readers/importer.py` & `spectrochempy-0.6.6/spectrochempy/utils/testing.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,869 +1,971 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
-"""
-This module define a generic class to import directories, files and contents.
-"""
-__all__ = ["read", "read_dir"]  # , "read_remote"]
-__dataset_methods__ = __all__
-
-import io
-import re
-from warnings import warn
-from zipfile import ZipFile
-
-import requests
-import yaml
-from traitlets import Dict, HasTraits, List, Type, Unicode
-
-from spectrochempy.core import info_, warning_
-from spectrochempy.utils.docstrings import _docstring
-from spectrochempy.utils.exceptions import DimensionsCompatibilityError, ProtocolError
-from spectrochempy.utils.file import (
-    check_filename_to_open,
-    get_directory_name,
-    get_filenames,
-    pathclean,
+
+import contextlib
+import functools
+import operator
+import os
+import warnings
+
+import numpy as np
+
+# import matplotlib.pyplot as plt
+# from matplotlib.testing.compare import calculate_rms, ImageAssertionError
+from numpy.testing import (  # noqa
+    assert_approx_equal,
+    assert_array_almost_equal,
+    assert_array_compare,
+    assert_array_equal,
+    assert_equal,
+    assert_raises,
 )
 
-FILETYPES = [
-    ("scp", "SpectroChemPy files (*.scp)"),
-    ("omnic", "Nicolet OMNIC files and series (*.spa *.spg *.srs)"),
-    ("soc", "Surface Optics Corp. (*.ddr *.hdr *.sdr)"),
-    ("labspec", "LABSPEC exported files (*.txt)"),
-    ("opus", "Bruker OPUS files (*.[0-9]*)"),
-    (
-        "topspin",
-        "Bruker TOPSPIN fid or series or processed data files "
-        "(fid ser 1[r|i] 2[r|i]* 3[r|i]*)",
-    ),
-    ("matlab", "MATLAB files (*.mat)"),
-    ("dso", "Data Set Object files (*.dso)"),
-    ("jcamp", "JCAMP-DX files (*.jdx *.dx)"),
-    ("csv", "CSV files (*.csv)"),
-    ("excel", "Microsoft Excel files (*.xls)"),
-    ("zip", "Compressed folder of data files (*.zip)"),
-    ("quadera", "Quadera ascii files (*.asc)"),
-    ("carroucell", "Carroucell files (*spa)"),
-    ("galactic", "GRAMS/Thermo Galactic files (*.spc)")
-    #  ('all', 'All files (*.*)')
-]
-ALIAS = [
-    ("spg", "omnic"),
-    ("spa", "omnic"),
-    ("ddr", "soc"),
-    ("hdr", "soc"),
-    ("sdr", "soc"),
-    ("spc", "galactic"),
-    ("srs", "omnic"),
-    ("mat", "matlab"),
-    ("txt", "labspec"),
-    ("jdx", "jcamp"),
-    ("dx", "jcamp"),
-    ("xls", "excel"),
-    ("asc", "quadera"),
-]
 
+@contextlib.contextmanager
+def set_env(**environ):
+    """
+    Temporarily set the process environment variables.
 
-# --------------------------------------------------------------------------------------
-class Importer(HasTraits):
-    # Private Importer class
+    Parameters
+    ----------
+    environ : dict(str)
+        Environment variables to set
 
-    objtype = Type()
-    datasets = List()
-    files = Dict()
-    default_key = Unicode()
-    protocol = Unicode()
-
-    protocols = Dict()
-    filetypes = Dict()
-
-    def __init__(self):
-
-        super().__init__()
-
-        self.filetypes = dict(FILETYPES)
-        temp = list(zip(*FILETYPES))
-        temp.reverse()
-        self.protocols = dict(zip(*temp))
-
-        #  add alias
-
-        self.alias = dict(ALIAS)
-
-    def __call__(self, *args, **kwargs):
-
-        self.datasets = []
-        self.default_key = kwargs.pop("default_key", ".scp")
-
-        if "merge" not in kwargs.keys():
-            # if merge is not specified, but the args are provided as a single list,
-            # then will are supposed to merge the datasets. If merge is specified then
-            # it has priority.
-            # This is not useful for the 1D datasets, as if they are compatible they
-            # are merged automatically
-            if args and len(args) == 1 and isinstance(args[0], (list, tuple)):
-                kwargs["merge"] = True
-
-        args, kwargs = self._setup_objtype(*args, **kwargs)
-        res = check_filename_to_open(*args, **kwargs)
-        if res:
-            # Normal return
-            self.files = res
-        else:
-            # Cancel in dialog!
-            return None
+    Examples
+    --------
+    >>> import os
+    >>> from spectrochempy.utils.testing import set_env
+    >>> with set_env(PLUGINS_DIR=u'test/plugins'):
+    ...     "PLUGINS_DIR" in os.environ
+    True
 
-        for key in self.files.keys():
+    >>> "PLUGINS_DIR" in os.environ
+    False
 
-            if key == "" and kwargs.get("protocol") == ["carroucell"]:
-                key = ".carroucell"
-                self.files = {".carroucell": self.files[""]}
-
-            if key == "frombytes":
-                # here we need to read contents
-                for filename, content in self.files[key].items():
-                    files_ = check_filename_to_open(filename)
-                    kwargs["content"] = content
-                    key_ = list(files_.keys())[0]
-                    self._switch_protocol(key_, files_, **kwargs)
-                if len(self.datasets) > 1:
-                    self.datasets = self._do_merge(self.datasets, **kwargs)
+    """
+    # https://stackoverflow.com/questions/2059482/
+    # python-temporarily-modify-the-current-processs-environment/51754362
+    old_environ = dict(os.environ)
+    os.environ.update(environ)
+    try:
+        yield
+    finally:
+        os.environ.clear()
+        os.environ.update(old_environ)
 
-            elif key and key[1:] not in list(zip(*FILETYPES))[0] + list(zip(*ALIAS))[0]:
-                raise TypeError(f"Filetype `{key}` is unknown in spectrochempy")
-            else:
-                # here files are read / or remotely from the disk using filenames
-                self._switch_protocol(key, self.files, **kwargs)
 
-        # now we will reset preference for this newly loaded datasets
-        if len(self.datasets) > 0:
+# ======================================================================================
+# NDDataset comparison
+# ======================================================================================
+def gisinf(x):
+    # copied from numpy.testing._private.utils
+    from numpy.core import errstate, isinf
+
+    with errstate(invalid="ignore"):
+        st = isinf(x)
+        if isinstance(st, type(NotImplemented)):
+            raise TypeError("isinf not supported for this type")
+    return st
+
+
+def _compare(x, y, decimal):
+    # copied from numpy.testing._private.utils
+    from numpy.core import array, float_, number, result_type
+    from numpy.core.fromnumeric import any as npany
+    from numpy.core.numerictypes import issubdtype
 
-            if all(self.datasets) is None:
-                return None
+    try:
+        if npany(gisinf(x)) or npany(gisinf(y)):
+            xinfid = gisinf(x)
+            yinfid = gisinf(y)
+            if not (xinfid == yinfid).all():
+                return False
+            # if one item, x and y is +- inf
+            if x.size == y.size == 1:
+                return x == y
+            x = x[~xinfid]
+            y = y[~yinfid]
+    except (TypeError, NotImplementedError):
+        pass
+
+    # make sure y is an inexact type to avoid abs(MIN_INT); will cause
+    # casting of x later.
+    dtype = result_type(y, 1.0)
+    y = array(y, dtype=dtype, copy=False, subok=True)
+    z = abs(x - y)
+
+    if not issubdtype(z.dtype, number):
+        z = z.astype(float_)  # handle object arrays
+
+    return z < 1.5 * 10.0 ** (-decimal)
+
+
+def compare_ndarrays(this, other, approx=False, decimal=6, data_only=False):
+
+    # Comparison based on attributes:
+    #        data, dims, mask, labels, units, meta
+
+    from spectrochempy.core.units import ur
+
+    def compare(x, y):
+        return _compare(x, y, decimal)
+
+    eq = True
+    thistype = this._implements()
+
+    if other.data is None and this.data is None and data_only:
+        attrs = ["labels"]
+    elif data_only:
+        attrs = ["data"]
+    else:
+        attrs = (
+            "data",
+            "dims",
+            "mask",
+            "labels",
+            "units",
+            "meta",
+        )
 
-            try:
-                prefs = self.datasets[0].preferences
-                prefs.reset()
-            except (FileNotFoundError, AttributeError):
-                pass
+    for attr in attrs:
+        if attr != "units":
+            sattr = getattr(this, f"_{attr}")
+            if hasattr(other, f"_{attr}"):
+                oattr = getattr(other, f"_{attr}")
+                if sattr is None and oattr is not None:
+                    raise AssertionError(f"`{attr}` of {this} is None.")
+                if oattr is None and sattr is not None:
+                    raise AssertionError(f"{attr} of {other} is None.")
+                if (
+                    hasattr(oattr, "size")
+                    and hasattr(sattr, "size")
+                    and oattr.size != sattr.size
+                ):
+                    # particular case of mask
+                    if attr != "mask":
+                        raise AssertionError(f"{thistype}.{attr} sizes are different.")
+                    else:
+                        assert_array_equal(
+                            other.mask,
+                            this.mask,
+                            f"{this} and {other} masks are different.",
+                        )
+                if attr in ["data", "mask"]:
+                    if approx:
+                        assert_array_compare(
+                            compare,
+                            sattr,
+                            oattr,
+                            header=(
+                                f"{thistype}.{attr} attributes ar"
+                                f"e not almost equal to %d decimals" % decimal
+                            ),
+                            precision=decimal,
+                        )
+                    else:
+                        assert_array_compare(
+                            operator.__eq__,
+                            sattr,
+                            oattr,
+                            header=f"{thistype}.{attr} "
+                            f"attributes are not "
+                            f"equal",
+                        )
+                else:
+                    eq &= np.all(sattr == oattr)
+                if not eq:
+                    raise AssertionError(
+                        f"The {attr} attributes of {this} and {other} are "
+                        f"different."
+                    )
+            else:
+                return False
         else:
-            return None
+            # unitless and dimensionless are supposed equal units
+            sattr = this._units
+            if sattr is None:
+                sattr = ur.dimensionless
+            if hasattr(other, "_units"):
+                oattr = other._units
+                if oattr is None:
+                    oattr = ur.dimensionless
+
+                eq &= np.all(sattr == oattr)
+                if not eq:
+                    raise AssertionError(
+                        f"attributes `{attr}` are not equals or one is "
+                        f"missing: \n{sattr} != {oattr}"
+                    )
+            else:
+                raise AssertionError(f"{other} has no units")
 
-        if len(self.datasets) == 1:
-            nd = self.datasets[0]  # a single dataset is returned
-            name = kwargs.pop("name", None)
-            if name:
-                nd.name = name
-            return nd
+    return True
 
-        else:
-            nds = self.datasets
-            names = kwargs.pop("names", None)
-            if names and len(names) == len(nds):
-                for nd, name in zip(nds, names):
-                    nd.name = name
-            elif names and len(names) != len(nds):
-                warn(
-                    "length of the `names` list and of the list of datasets mismatch - names not applied"
-                )
-            return sorted(
-                nds, key=str
-            )  # return a sorted list (sorted according to their string representation)
-
-    def _setup_objtype(self, *args, **kwargs):
-        # check if the first argument is an instance of NDDataset or Project
-
-        args = list(args)
-        if (
-            args
-            and hasattr(args[0], "_implements")
-            and args[0]._implements() in ["NDDataset"]
-        ):
-            # the first arg is an instance of NDDataset
-            object = args.pop(0)
-            self.objtype = type(object)
 
-        else:
-            # by default returned objtype is NDDataset (import here to avoid circular import)
-            from spectrochempy.core.dataset.nddataset import NDDataset
+def compare_coords(this, other, approx=False, decimal=3, data_only=False):
+
+    # TODO: compare base on signficant digit for coordinate instead of decimals
+    #  (that may not work for very small coordinates numbers)
+    from spectrochempy.core.units import ur
+
+    def compare(x, y):
+        return _compare(x, y, decimal)
 
-            self.objtype = kwargs.pop("objtype", NDDataset)
+    eq = True
+    thistype = this._implements()
 
-        return args, kwargs
+    if other.data is None and this.data is None and data_only:
+        attrs = ["labels"]
+    elif data_only:
+        attrs = ["data"]
+    else:
+        attrs = ["data", "labels", "units", "meta", "title"]
+        # if 'title' in attrs:  #    attrs.remove('title')
+        # #TODO: should we use title for comparison?
+
+    for attr in attrs:
+        if attr != "units":
+            sattr = getattr(this, f"_{attr}")
+            if hasattr(other, f"_{attr}"):
+                oattr = getattr(other, f"_{attr}")
+                # to avoid deprecation warning issue for unequal array
+                if sattr is None and oattr is not None:
+                    raise AssertionError(f"`{attr}` of {this} is None.")
+                if oattr is None and sattr is not None:
+                    raise AssertionError(f"{attr} of {other} is None.")
+                if (
+                    hasattr(oattr, "size")
+                    and hasattr(sattr, "size")
+                    and oattr.size != sattr.size
+                ):
+                    raise AssertionError(f"{thistype}.{attr} sizes are different.")
+
+                if attr == "data":
+                    if approx:
+                        assert_array_compare(
+                            compare,
+                            sattr,
+                            oattr,
+                            header=(
+                                f"{thistype}.{attr} attributes ar"
+                                f"e not almost equal to %d decimals" % decimal
+                            ),
+                            precision=decimal,
+                        )
+                    else:
+                        assert_array_compare(
+                            operator.__eq__,
+                            sattr,
+                            oattr,
+                            header=f"{thistype}.{attr} "
+                            f"attributes are not "
+                            f"equal",
+                        )
 
-    def _switch_protocol(self, key, files, **kwargs):
+                else:
+                    eq &= np.all(sattr == oattr)
 
-        protocol = kwargs.get("protocol", None)
-        if protocol is not None and protocol != "ALL":
-            if not isinstance(protocol, list):
-                protocol = [protocol]
-            if key and key[1:] not in protocol and self.alias[key[1:]] not in protocol:
-                return
-
-        datasets = []
-        for filename in files[key]:
-
-            read_ = getattr(self, f"_read_{key[1:]}")
-
-            dataset = None
-            try:
-                # read locally or using url if filename is an url
-                dataset = read_(self.objtype(), filename, **kwargs)
-
-            except (FileNotFoundError, OSError) as exc:
-                # file was not found.
-                # it is an url we raise an error
-                local_only = kwargs.get("local_only", False)
-                if _is_url(filename) or local_only:
-                    raise (FileNotFoundError) from exc
-
-                # else, we try on github
-                try:
-                    # Try to get the file from github
-                    kwargs["read_method"] = read_
-                    info_(
-                        "File/directory not found locally: Attempt to download it from "
-                        "the GitHub repository `spectrochempy_data`..."
+                if not eq:
+                    raise AssertionError(
+                        f"The {attr} attributes of {this} and {other} are "
+                        f"different."
                     )
-                    dataset = _read_remote(self.objtype(), filename, **kwargs)
+            else:
+                return False
+        else:
+            # unitless and dimensionless are supposed equals
+            sattr = this._units
+            if sattr is None:
+                sattr = ur.dimensionless
+            if hasattr(other, "_units"):
+                oattr = other._units
+                if oattr is None:
+                    oattr = ur.dimensionless
+
+                eq &= np.all(sattr == oattr)
+                if not eq:
+                    raise AssertionError(
+                        f"attributes `{attr}` are not equals or one is "
+                        f"missing: \n{sattr} != {oattr}"
+                    )
+            else:
+                raise AssertionError(f"{other} has no units")
 
-                except (FileNotFoundError) as exc:
-                    raise (FileNotFoundError) from exc
+    return True
 
-                except Exception as e:
-                    warning_(str(e))
 
-            except Exception as e:
-                warning_(str(e))
+def compare_datasets(this, other, approx=False, decimal=6, data_only=False):
+    from spectrochempy.core.units import ur
 
-            if dataset is not None:
-                if not isinstance(dataset, list):
-                    datasets.append(dataset)
+    def compare(x, y):
+        return _compare(x, y, decimal)
+
+    eq = True
+
+    # if not isinstance(other, NDArray):
+    #     # try to make some assumption to make useful comparison.
+    #     if isinstance(other, Quantity):
+    #         otherdata = other.magnitude
+    #         otherunits = other.units
+    #     elif isinstance(other, (float, int, np.ndarray)):
+    #         otherdata = other
+    #         otherunits = False
+    #     else:
+    #         raise AssertionError(
+    #             f"{this} and {other} objects are too different to be " f"compared."
+    #         )
+    #
+    #     if not this.has_units and not otherunits:
+    #         eq = np.all(this._data == otherdata)
+    #     elif this.has_units and otherunits:
+    #         eq = np.all(this._data * this._units == otherdata * otherunits)
+    #     else:
+    #         raise AssertionError(
+    #         f"units of {this} and {other} objects does not match")
+    #     return eq
+
+    thistype = this._implements()
+
+    if other.data is None and this.data is None and data_only:
+        attrs = ["labels"]
+    elif data_only:
+        attrs = ["data"]
+    else:
+        attrs = this.__dir__()
+        exclude = (
+            "filename",
+            "preferences",
+            "description",
+            "history",
+            "created",
+            "modified",
+            "origin",
+            "roi",
+            "size",
+            "name",
+            "modeldata",
+            "processeddata",
+            "baselinedata",
+            "referencedata",
+            "state",
+        )
+        for attr in exclude:
+            # these attributes are not used for comparison (comparison based on
+            # data and units!)
+            if attr in attrs:
+                if attr in attrs:
+                    attrs.remove(attr)
+
+        # if 'title' in attrs:  #    attrs.remove('title')
+        # #TODO: should we use title for comparison?
+
+    for attr in attrs:
+        if attr != "units":
+            sattr = getattr(this, f"_{attr}")
+            if hasattr(other, f"_{attr}"):
+                oattr = getattr(other, f"_{attr}")
+                if sattr is None and oattr is not None:
+                    raise AssertionError(f"`{attr}` of {this} is None.")
+                if oattr is None and sattr is not None:
+                    raise AssertionError(f"{attr} of {other} is None.")
+                if (
+                    hasattr(oattr, "size")
+                    and hasattr(sattr, "size")
+                    and oattr.size != sattr.size
+                ):
+                    # particular case of mask
+                    if attr != "mask":
+                        raise AssertionError(f"{thistype}.{attr} sizes are different.")
+                    else:
+                        assert_array_equal(
+                            other.mask,
+                            this.mask,
+                            f"{this} and {other} masks are different.",
+                        )
+                if attr in ["data"]:
+                    # we must compare masked array
+                    sattr = this.masked_data
+                    oattr = other.masked_data
+                    if approx:
+                        assert_array_compare(
+                            compare,
+                            sattr,
+                            oattr,
+                            header=(
+                                f"{thistype}.{attr} attributes ar"
+                                f"e not almost equal to %d decimals" % decimal
+                            ),
+                            precision=decimal,
+                        )
+                    else:
+                        assert_array_compare(
+                            operator.__eq__,
+                            sattr,
+                            oattr,
+                            header=f"{thistype}.{attr} "
+                            f"attributes are not "
+                            f"equal",
+                        )
+
+                elif attr in ["coordset"]:
+                    if (sattr is None and oattr is not None) or (
+                        oattr is None and sattr is not None
+                    ):
+                        raise AssertionError("One of the coordset is None")
+                    elif sattr is None and oattr is None:
+                        pass
+                    else:
+                        for item in zip(sattr, oattr):
+                            res = compare_coords(*item, approx=True, decimal=3)
+                            if not res:
+                                raise AssertionError(f"coords differs:\n{res}")
                 else:
-                    datasets.extend(dataset)
-
-        if len(datasets) > 1:
-            datasets = self._do_merge(datasets, **kwargs)
-            if kwargs.get("merge", False):
-                datasets[0].name = pathclean(filename).stem
-                datasets[0].filename = pathclean(filename)
-
-        self.datasets.extend(datasets)
-
-    def _do_merge(self, datasets, **kwargs):
-
-        # several datasets returned (only if several files have been passed) and the `merge` keyword argument is False
-        merged = kwargs.get("merge", False)
-        shapes = {nd.shape if hasattr(nd, "shape") else None for nd in datasets}
-        if len(shapes) == 1 and None not in shapes:
-            # homogeneous set of files
-            dim0 = shapes.pop()[0]
-            if dim0 == 1:
-                merged = kwargs.get("merge", True)  # priority to the keyword setting
+                    eq &= np.all(sattr == oattr)
+                if not eq:
+                    raise AssertionError(
+                        f"The {attr} attributes of {this} and {other} are "
+                        f"different."
+                    )
+            else:
+                return False
         else:
-            # not homogeneous
-            merged = kwargs.get("merge", False)
+            # unitlesss and dimensionless are supposed equals
+            sattr = this._units
+            if sattr is None:
+                sattr = ur.dimensionless
+            if hasattr(other, "_units"):
+                oattr = other._units
+                if oattr is None:
+                    oattr = ur.dimensionless
+
+                eq &= np.all(sattr == oattr)
+                if not eq:
+                    raise AssertionError(
+                        f"attributes `{attr}` are not equals or one is "
+                        f"missing: \n{sattr} != {oattr}"
+                    )
+            else:
+                raise AssertionError(f"{other} has no units")
 
-        if merged:
-            # Try to stack the dataset into a single one
-            try:
-                dataset = self.objtype.concatenate(datasets, axis=0)
-                if dataset.coordset is not None and kwargs.pop("sortbydate", True):
-                    dataset.sort(dim="y", inplace=True)
-                    dataset.history = "Sorted by date"
-                datasets = [dataset]
-
-            except DimensionsCompatibilityError as e:
-                warn(str(e))  # return only the list
-
-        return datasets
-
-
-def _importer_method(func):
-    # Decorator to define a given read function as belonging to Importer
-    setattr(Importer, func.__name__, staticmethod(func))
-    return func
+    return True
 
 
-# --------------------------------------------------------------------------------------
-# Public Generic Read function
-# --------------------------------------------------------------------------------------
+def assert_dataset_equal(nd1, nd2, **kwargs):
+    kwargs["approx"] = False
+    assert_dataset_almost_equal(nd1, nd2, **kwargs)
+    return True
 
-_docstring.get_sections(
-    """
-See Also
---------
-read : Generic reader inferring protocol from the filename extension.
-read_zip : Read Zip archives (containing spectrochempy readable files)
-read_dir : Read an entire directory.
-read_opus : Read OPUS spectra.
-read_labspec : Read Raman LABSPEC spectra (:file:`.txt`\ ).
-read_omnic : Read Omnic spectra (:file:`.spa`\ , :file:`.spg`\ , :file:`.srs`\ ).
-read_soc : Read Surface Optics Corps. files (:file:`.ddr` , :file:`.hdr` or :file:`.sdr`\ ).
-read_galactic : Read Galactic files (:file:`.spc`\ ).
-read_quadera : Read a Pfeiffer Vacuum's QUADERA mass spectrometer software file.
-read_topspin : Read TopSpin Bruker NMR spectra.
-read_csv : Read CSV files (:file:`.csv`\ ).
-read_jcamp : Read Infrared JCAMP-DX files (:file:`.jdx`\ , :file:`.dx`\ ).
-read_matlab : Read Matlab files (:file:`.mat`\ , :file:`.dso`\ ).
-read_carroucell : Read files in a directory after a carroucell experiment.
-""",
-    sections=["See Also"],
-    base="Importer",
-)
 
-_docstring.delete_params("Importer.see_also", "read")
+def assert_dataset_almost_equal(nd1, nd2, **kwargs):
+    decimal = kwargs.get("decimal", 3)
+    approx = kwargs.get("approx", True)
+    # if data_only is True, compare only based on data (not labels and so on)
+    # except if dataset is label only!.
+    data_only = kwargs.get("data_only", False)
+    compare_datasets(nd1, nd2, approx=approx, decimal=decimal, data_only=data_only)
+    return True
 
 
-@_docstring.dedent
-def read(*paths, **kwargs):
-    """
-    Generic read method.
-
-    This method is generally able to load experimental files based on extensions.
+def assert_coord_equal(nd1, nd2, **kwargs):
+    kwargs["approx"] = False
+    assert_coord_almost_equal(nd1, nd2, **kwargs)
+    return True
 
-    Parameters
-    ----------
-    *paths : `str`, `~pathlib.Path` object objects or valid urls, optional
-        The data source(s) can be specified by the name or a list of name for the
-        file(s) to be loaded:
-
-        * *e.g.,* ( filename1, filename2, ...,  \*\*kwargs )*
-
-        If the list of filenames are enclosed into brackets:
-
-        * *e.g.,* ( **[** *filename1, filename2, ...* **]**, \*\*kwargs *)*
-
-        The returned datasets are merged to form a single dataset,
-        except if ``merge`` is set to `False`.
-
-        If a source is not provided (*i.e.,* no ``paths`` , nor ``content``\ ),
-        a dialog box will be opened to select files.
-    %(kwargs)s
-
-    Returns
-    -------
-    object : `NDDataset` or list of `NDDataset`
-        The returned dataset(s).
-
-    Other Parameters
-    ----------------
-    protocol : `str`\ , optional
-        ``Protocol`` used for reading. It can be one of {``'scp'``\ , ``'omnic'``\ ,
-        ``'opus'``\ , ``'topspin'``\ , ``'matlab'``\ , ``'jcamp'``\ , ``'csv'``\ ,
-        ``'excel'``\ }. If not provided, the correct protocol
-        is inferred (whenever it is possible) from the filename extension.
-    directory : `~pathlib.Path` object objects or valid urls, optional
-        From where to read the files.
-    merge : `bool`\ , optional, default: `False`
-        If `True` and several filenames or a ``directory`` have been provided as
-        arguments, then a single `NDDataset` with merged (stacked along the first
-        dimension) is returned.
-    sortbydate : `bool`, optional, default: `True`
-        Sort multiple filename by acquisition date.
-    description : `str`, optional
-        A Custom description.
-    origin : one of {``'omnic'``\ , ``'tga'``\ }, optional
-        Used when reading with the CSV protocol. In order to properly interpret CSV file
-        it can be necessary to set the origin of the spectra.
-        Up to now only ``'omnic'`` and ``'tga'`` have been implemented.
-    csv_delimiter : `str`\ , optional, default: `~spectrochempy.preferences.csv_delimiter`
-        Set the column delimiter in CSV file.
-    content : `bytes` object, optional
-        Instead of passing a filename for further reading, a bytes content can be
-        directly provided as bytes objects.
-        The most convenient way is to use a dictionary. This feature is particularly
-        useful for a GUI Dash application to handle drag and drop of files into a
-        Browser.
-    iterdir : `bool`\ , optional, default: `True`
-        If `True` and no filename was provided, all files present in the provided
-        ``directory`` are returned (and merged if ``merge`` is `True`\ .
-        It is assumed that all the files correspond to current reading protocol.
-
-        .. versionchanged:: 0.6.2
-
-            ``iterdir`` replace the deprecated ``listdir`` argument.
-
-    recursive : `bool`, optional, default: `False`
-        Read also in subfolders.
-    replace_existing: `bool`, optional, default: `False`
-        Used only when url are specified. By default, existing files are not replaced
-        so not downloaded.
-    download_only: `bool`, optional, default: `False`
-        Used only when url are specified.  If True, only downloading and saving of the
-        files is performed, with no attempt to read their content.
-    read_only: `bool`, optional, default: `True`
-        Used only when url are specified.  If True, saving of the
-        files is performed in the current directory, or in the directory specified by
-        the directory parameter.
 
-    See Also
-    --------
-    %(Importer.see_also.no_read)s
+def assert_coord_almost_equal(nd1, nd2, **kwargs):
+    decimal = kwargs.get("decimal", 6)
+    approx = kwargs.get("approx", True)
+    # if data_only is True, compare only based on data (not labels and so on)
+    # except if coord is label only!.
+    data_only = kwargs.get("data_only", False)
+    compare_coords(nd1, nd2, approx=approx, decimal=decimal, data_only=data_only)
+    return True
 
-    Examples
-    ---------
-    Reading a single OPUS file  (providing a windows type filename relative
-    to the default `~spectrochempy.preferences.datadir` )
 
-    >>> scp.read('irdata\\\\OPUS\\\\test.0000')
-    NDDataset: [float64] a.u. (shape: (y:1, x:2567))
+def assert_ndarray_equal(nd1, nd2, **kwargs):
+    kwargs["approx"] = False
+    assert_ndarray_almost_equal(nd1, nd2, **kwargs)
+    return True
 
-    Reading a single OPUS file  (providing a unix/python type filename relative
-    to the default ``datadir`` )
-    Note that here read_opus is called as a classmethod of the NDDataset class
 
-    >>> scp.read('irdata/OPUS/test.0000')
-    NDDataset: [float64] a.u. (shape: (y:1, x:2567))
+def assert_ndarray_almost_equal(nd1, nd2, **kwargs):
+    decimal = kwargs.get("decimal", 6)
+    approx = kwargs.get("approx", True)
+    # if data_only is True, compare only based on data (not labels and so on)
+    # except if ndarray is label only!.
+    data_only = kwargs.get("data_only", False)
+    compare_ndarrays(nd1, nd2, approx=approx, decimal=decimal, data_only=data_only)
+    return True
 
-    Single file specified with pathlib.Path object
 
-    >>> from pathlib import Path
-    >>> folder = Path('irdata/OPUS')
-    >>> p = folder / 'test.0000'
-    >>> scp.read(p)
-    NDDataset: [float64] a.u. (shape: (y:1, x:2567))
+def assert_project_equal(proj1, proj2, **kwargs):
+    assert_project_almost_equal(proj1, proj2, approx=False)
+    return True
 
-    Multiple files not merged (return a list of datasets).
-    Note that a directory is specified
 
-    >>> le = scp.read('test.0000', 'test.0001', 'test.0002', directory='irdata/OPUS')
-    >>> len(le)
-    3
-    >>> le[0]
-    NDDataset: [float64] a.u. (shape: (y:1, x:2567))
+def assert_project_almost_equal(proj1, proj2, **kwargs):
+    assert len(proj1.datasets) == len(proj2.datasets)
+    for nd1, nd2 in zip(proj1.datasets, proj2.datasets):
+        compare_datasets(nd1, nd2, **kwargs)
 
-    Multiple files merged as the `merge` keyword is set to true
+    assert len(proj1.projects) == len(proj2.projects)
+    for pr1, pr2 in zip(proj1.projects, proj2.projects):
+        assert_project_almost_equal(pr1, pr2, **kwargs)
 
-    >>> scp.read('test.0000', 'test.0001', 'test.0002', directory='irdata/OPUS', merge=True)
-    NDDataset: [float64] a.u. (shape: (y:3, x:2567))
+    assert len(proj1.scripts) == len(proj2.scripts)
+    for sc1, sc2 in zip(proj1.scripts, proj2.scripts):
+        assert_script_equal(sc1, sc2, **kwargs)
 
-    Multiple files to merge : they are passed as a list instead of using the keyword
-    `merge`
+    return True
 
-    >>> scp.read(['test.0000', 'test.0001', 'test.0002'], directory='irdata/OPUS')
-    NDDataset: [float64] a.u. (shape: (y:3, x:2567))
 
-    Multiple files not merged : they are passed as a list but `merge` is set to false
+def assert_script_equal(sc1, sc2, **kwargs):
+    if sc1 != sc2:
+        raise AssertionError(f"Scripts are different: {sc1.content} != {sc2.content}")
 
-    >>> le = scp.read(['test.0000', 'test.0001', 'test.0002'], directory='irdata/OPUS', merge=False)
-    >>> len(le)
-    3
 
-    Read without a filename. This has the effect of opening a dialog for file(s)
-    selection
+# ======================================================================================
+# RandomSeedContext
+# ======================================================================================
+class RandomSeedContext(object):
+    """
+    A context manager (for use with the `with` statement) that will seed the
+    numpy random number generator (RNG) to a specific value, and then restore
+    the RNG state back to whatever it was before.
 
-    >>> nd = scp.read()
+    (Copied from Astropy, licence BSD-3).
 
-    Read in a directory (assume that only OPUS files are present in the directory
-    (else we must use the generic `read` function instead)
+    Parameters
+    ----------
+    seed : int
+        The value to use to seed the numpy RNG
 
-    >>> le = scp.read(directory='irdata/OPUS')
-    >>> len(le)
-    2
+    Examples
+    --------
+    A typical use case might be::
 
-    Again we can use merge to stack all 4 spectra if thet have compatible dimensions.
+        with RandomSeedContext(<some seed value you pick>):
+            from numpy import random
 
-    >>> scp.read(directory='irdata/OPUS', merge=True)
-    [NDDataset: [float64] a.u. (shape: (y:1, x:5549)), NDDataset: [float64] a.u. (shape: (y:4, x:2567))]
+            randarr = random.randn(100)
+            ... run your test using `randarr` ...
     """
 
-    importer = Importer()
-
-    protocol = kwargs.get("protocol", None)
-    available_protocols = list(importer.protocols.values())
-    available_protocols.extend(
-        list(importer.alias.keys())
-    )  # to handle variants of protocols
-    if protocol is None:
-        kwargs["filetypes"] = list(importer.filetypes.values())
-        kwargs["protocol"] = "ALL"
-        default_filter = kwargs.get("default_filter", None)
-        if default_filter is not None:
-            kwargs["default_filter"] = importer.filetypes[default_filter]
-    else:
-        try:
-            kwargs["filetypes"] = [importer.filetypes[protocol]]
-        except KeyError:
-            raise ProtocolError(protocol, list(importer.protocols.values()))
-        except TypeError as e:
-            print(e)
-
-    # deprecated kwargs
-    listdir = kwargs.pop("listdir", True)
-    if "listdir" in kwargs and "iterdir" not in kwargs:
-        kwargs["iterdir"] = listdir
-        warning_(
-            "argument `listdir` is deprecated, use ìterdir` instead",
-            category=DeprecationWarning,
-        )
+    def __init__(self, seed):
+        self.seed = seed
 
-    return importer(*paths, **kwargs)
+    def __enter__(self):
+        from numpy import random
 
+        self.startstate = random.get_state()
+        random.seed(self.seed)
 
-# for some reasons the doctring.getsection modify the signature of the function
-# when used as a decorator, so we use it as a function
-_docstring.get_sections(
-    read.__doc__,
-    sections=["Parameters", "Other Parameters", "Returns"],
-    base="Importer",
-)
+    def __exit__(self, exc_type, exc_value, traceback):
+        from numpy import random
 
-_docstring.delete_params("Importer.see_also", "read_dir")
+        random.set_state(self.startstate)
 
 
-@_docstring.dedent
-def read_dir(directory=None, **kwargs):
+# ======================================================================================
+# raises and assertions (mostly copied from astropy)
+# ======================================================================================
+def assert_equal_units(unit1, unit2, strict=False):
     """
-    Read an entire directory.
-
-    Open a list of readable files in a and store data/metadata in a dataset or a list of
-    datasets according to the following rules :
-
-    * 2D spectroscopic data (e.g. valid .spg files or matlab arrays, etc...) from
-      distinct files are stored in distinct `NDdataset`\ s.
-    * 1D spectroscopic data (e.g., :file:`.spa` files) in a given directory are merged
-      into single `NDDataset`\ , providing their unique dimension are compatible.
-      If not, an error is generated.
-    * non-readable files are ignored
+    Compare units.
 
     Parameters
     ----------
-    directory : str or pathlib
-        Folder where are located the files to read.
-
-    Returns
-    --------
-    %(Importer.returns)s
-        Depending on the python version, the order of the datasets in the list
-        may change.
-
-    See Also
-    --------
-    %(Importer.see_also.no_read_dir)s
-
-    Examples
-    --------
-
-    >>> scp.preferences.csv_delimiter = ','
-    >>> A = scp.read_dir('irdata')
-    >>> len(A)
-    4
-
-    >>> B = scp.read_dir()
+    unit1 : units
+        Units to be compared.
+    unit2 : units
+        Other units to be compared
+    strict :  bool, optional, default: False
+        If True, units should be exactly the same: `km` != `mm` .
     """
-    kwargs["iterdir"] = True
-    importer = Importer()
-    return importer(directory, **kwargs)
+    from pint import DimensionalityError
 
+    try:
+        x = (1.0 * unit1).to_base_units() / (1.0 * unit2).to_base_units()
+    except DimensionalityError:
+        raise AssertionError
 
-# _docstring.delete_params("Importer.see_also", "read_remote")
-# @_docstring.dedent
-# def read_remote(file_or_dir, **kwargs):
-#     """
-#     Download and read files or an entire directory from any url
-#
-#     The first usage in spectrochempy is the loading of test files in the
-#     `spectrochempy_data repository <https://github.com/spectrochempy/spectrochempy_data>`__\ .
-#     This is done only if the data are not yet
-#     downloaded and present in the `~spectrochempy.preferences.datadir` directory.
-#
-#     It can also be used to download and read file or directory from any url.
-#
-#     Parameters
-#     ----------
-#     path : `str`, `~pathlib.Path` object or an url.
-#         When a file or folder is specified, it must be written as if it were present
-#         locally exactly as for the `read` function. The correponding file or directory
-#         is downloaded from the ``github spectrochemp_data`` repository.
-#         Otherwise it should be a full and valid url.
-#     %(kwargs)s
-#
-#     Returns
-#     --------
-#     %(Importer.returns)s
-#
-#     Other Parameters
-#     ----------------
-#     %(Importer.other_parameters)s
-#
-#     See Also
-#     --------
-#     %(Importer.see_also.no_read_remote)s
-#
-#     Examples
-#     --------
-#
-#     >>> A = scp.read_remote('irdata/subdir')
-#     """
-#     kwargs["remote"] = True
-#     importer = Importer()
-#     return importer(file_or_dir, **kwargs)
-#
+    if x.dimensionless and (x == 1.0 or not strict):
+        _check_absorbance_related_units(unit1, unit2)
+        return True
 
-# ======================================================================================
-# Private read functions
-# ======================================================================================
-@_importer_method
-def _read_dir(*args, **kwargs):
-    _, directory = args
-    directory = get_directory_name(directory)
-    files = get_filenames(directory, **kwargs)
-    datasets = []
-    valid_extensions = list(zip(*FILETYPES))[0] + list(zip(*ALIAS))[0]
-    for key in [key for key in files.keys() if key[1:] in valid_extensions]:
-        if key:
-            importer = Importer()
-            nd = importer(files[key], **kwargs)
-            if nd is not None:
-                if not isinstance(nd, list):
-                    nd = [nd]
-                datasets.extend(nd)
-    return datasets
-
-
-@_importer_method
-def _read_scp(*args, **kwargs):
-    dataset, filename = args
-    return dataset.load(filename, **kwargs)
-
-
-@_importer_method
-def _read_(*args, **kwargs):
-    dataset, filename = args
-
-    if kwargs.pop("remote", False):
-        return Importer._read_remote(*args, **kwargs)
-    elif not filename or filename.is_dir():
-        return Importer._read_dir(*args, **kwargs)
-    else:
-        raise FileNotFoundError
+    raise AssertionError
 
-    # protocol = kwargs.get("protocol", None)
-    # if protocol and ".scp" in protocol:
-    #     return dataset.load(filename, **kwargs)
-    #
-    # elif filename and filename.name in ("fid", "ser", "1r", "2rr", "3rrr"):
-    #     # probably an Topspin NMR file
-    #     return dataset.read_topspin(filename, **kwargs)
-    # elif filename:
-    #     # try scp format
-    #     try:
-    #         return dataset.load(filename, **kwargs)
-    #     except Exception:
-    #         # lets try some common format
-    #         for key in ["omnic", "opus", "topspin", "labspec", "matlab", "jdx"]:
-    #             try:
-    #                 _read = getattr(dataset, f"read_{key}")
-    #                 f = f"{filename}.{key}"
-    #                 return _read(f, **kwargs)
-    #             except Exception:
-    #                 pass
-    #         raise NotImplementedError
 
+def _check_absorbance_related_units(unit1, unit2):
+    # particular case of absorbance, transmittance and absolute_transmitttance units
+    lunit = ["absorbance", "transmittance", "absolute_transmittance"]
+    if f"{unit1:P}" in lunit and f"{unit2:P}" in lunit:
+        if f"{unit1:P}" != f"{unit2:P}":
+            raise AssertionError
+    return True
 
-# ======================================================================================
-# Private functions
-# ======================================================================================
-def _is_url(filename):
-    return (
-        isinstance(filename, str)
-        and re.match(r"http[s]?:[\/]{2}", filename) is not None
-    )
-
-
-def _openfid(filename, mode="rb", **kwargs):
-    # Return a file ID
-
-    # Check if Content has been passed?
-    content = kwargs.get("content", False)
-
-    # default encoding
-    encoding = "utf-8"
-
-    if _is_url(filename):
-        # by default we set the read_only flag to True when reading remote url
-        kwargs["read_only"] = kwargs.get("read_only", True)
-
-        # use request to read the remote content
-        r = requests.get(filename, allow_redirects=True)
-        r.raise_for_status()
-        content = r.content
-        encoding = r.encoding
 
-    else:
-        # Transform filename to a Path object is not yet the case
-        filename = pathclean(filename)
+class raises(object):
+    """
+    A decorator to mark that a test should raise a given exception.
+    Use as follows::
 
-    # Create the file ID
-    if content:
-        # if a content has been passed, then it has priority
-        fid = (
-            io.BytesIO(content)
-            if mode == "rb"
-            else io.StringIO(content.decode(encoding))
-        )
-    else:
-        fid = open(filename, mode=mode)
+        @raises(ZeroDivisionError)
+        def test_foo():
+            x = 1/0
+
+    This can also be used a context manager, in which case it is just
+    an alias for the `pytest.raises` context manager (because the
+    two have the same name this help avoid confusion by being
+    flexible).
 
-    return fid, kwargs
+    (Copied from Astropy, licence BSD-3)
+    """
 
+    # pep-8 naming exception -- this is a decorator class
+    def __init__(self, exc):
+        self._exc = exc
+        self._ctx = None
 
-def _write_downloaded_file(content, dst):
-    if not dst.parent.exists():
-        # create the eventually missing subdirectory
-        dst.parent.mkdir(parents=True, exist_ok=True)
-    dst.write_bytes(content)
-    info_(f"{dst.name} has been downloaded and written in {dst.parent}")
+    def __call__(self, func):
+        @functools.wraps(func)
+        def run_raises_test(*args, **kwargs):
+            import pytest
 
+            pytest.raises(self._exc, func, *args, **kwargs)
 
-def _get_url_content_and_save(url, dst, replace, read_only=False):
+        return run_raises_test
 
-    if not replace and dst.exists():
-        return
+    def __enter__(self):
+        import pytest
 
-    try:
-        r = requests.get(url, allow_redirects=True)
+        self._ctx = pytest.raises(self._exc)
+        return self._ctx.__enter__()
 
-        r.raise_for_status()
+    def __exit__(self, *exc_info):
+        return self._ctx.__exit__(*exc_info)
 
-        # write downloaded file
-        if not read_only:
-            _write_downloaded_file(r.content, dst)
 
-        # in all case return the content
-        return r.content
+class catch_warnings(warnings.catch_warnings):
+    """
+    A high-powered version of warnings.catch_warnings to use for testing
+    and to make sure that there is no dependence on the order in which
+    the tests are run.
 
-    except OSError:
-        raise FileNotFoundError(f"Not found locally or at url:{url}")
+    This completely blitzes any memory of any warnings that have
+    appeared before so that all warnings will be caught and displayed.
 
+    `*args` is a set of warning classes to collect.  If no arguments are
+    provided, all warnings are collected.
 
-def _download_full_testdata_directory():
-    from spectrochempy.core import preferences as prefs
+    Use as follows::
 
-    datadir = prefs.datadir
+        with catch_warnings(MyCustomWarning) as w :
+            do.something.bad()
+        assert len(w) > 0
 
-    url = "https://github.com/spectrochempy/spectrochempy_data/archive/refs/heads/master.zip"
+    (Copied from Astropy, licence BSD-3)
+    """
 
-    resp = requests.get(url)
-    zipfile = ZipFile(io.BytesIO(resp.content))
-    files = [zipfile.open(file_name) for file_name in zipfile.namelist()]
+    def __init__(self, *classes):
+        super(catch_warnings, self).__init__(record=True)
+        self.classes = classes
+
+    def __enter__(self):
+        warning_list = super(catch_warnings, self).__enter__()
+        if len(self.classes) == 0:
+            warnings.simplefilter("always")
+        else:
+            warnings.simplefilter("ignore")
+            for cls in self.classes:
+                warnings.simplefilter("always", cls)
+        return warning_list
 
-    for file in files:
-        name = file.name
-        if name.endswith("/") or "testdata/" not in name:  # dir
-            continue
-        uncompressed = zipfile.read(name)
-        p = list(pathclean(name).parts)[2:]
-        dst = datadir.joinpath("/".join(p))
-        _write_downloaded_file(uncompressed, dst)
+    def __exit__(self, type, value, traceback):
+        pass
 
 
-def _download_from_github(path, dst, replace=False):
-    # download on github (always save the downloaded files)
-    relative_path = str(pathclean(path).as_posix())
-    path = (
-        f"https://github.com/spectrochempy/spectrochempy_data/raw/master/"
-        f"testdata/{relative_path}"
-    )
+# TODO: work on this
+# #
+# --------------------------------------------------------------------------------------
+# # Matplotlib testing utilities
+# #
+# --------------------------------------------------------------------------------------
+#
+# figures_dir = os.path.join(os.path.expanduser("~"), ".spectrochempy",
+# "figures")
+# os.makedirs(figures_dir, exist_ok=True)
+#
+#
+# #
 
-    # first determine if it is a directory
-    r = requests.get(path + "/__index__", allow_redirects=True)
-    index = None
-    if r.status_code == 200:
-        index = yaml.load(r.content, Loader=yaml.CLoader)
+# def _compute_rms(x, y):
+#     return calculate_rms(x, y)
+#
+#
+# #
 
-    if index is None:
-        return _get_url_content_and_save(path, dst, replace)
+# def _image_compare(imgpath1, imgpath2, REDO_ON_TYPEERROR):
+#     # compare two images saved in files imgpath1 and imgpath2
+#
+#     from matplotlib.pyplot import imread
+#     from skimage.measure import compare_ssim as ssim
+#
+#     # read image
+#     try:
+#         img1 = imread(imgpath1)
+#     except IOError:
+#         img1 = imread(imgpath1 + '.png')
+#     try:
+#         img2 = imread(imgpath2)
+#     except IOError:
+#         img2 = imread(imgpath2 + '.png')
+#
+#     try:
+#         sim = ssim(img1, img2,
+#                    data_range=img1.max() - img2.min(),
+#                    multichannel=True) * 100.
+#         rms = _compute_rms(img1, img2)
+#
+#     except ValueError:
+#         rms = sim = -1
+#
+#     except TypeError as e:
+#         # this happen sometimes and erratically during testing using
+#         # pytest-xdist (parallele testing). This is work-around the problem
+#         if e.args[0] == "unsupported operand type(s) " \
+#                         "for - : 'PngImageFile' and 'int'" and not
+#                         REDO_ON_TYPEERROR:
+#             REDO_ON_TYPEERROR = True
+#             rms = sim = -1
+#         else:
+#             raise
+#
+#     return (sim, rms, REDO_ON_TYPEERROR)
+#
+#
+# #
 
-    else:
-        # download folder
-        for filename in index["files"]:
-            _get_url_content_and_save(f"{path}/{filename}", dst / filename, replace)
-        for folder in index["folders"]:
-            _download_from_github(f"{relative_path}/{folder}", dst / folder)
-
-
-def _is_relative_to(path, base):
-    # try to emulate the pathlib is_relative_to method which does not work on python
-    # 3.7 (needed for Colab!)
-    # TODO: replace as Colab is updated to 3.9
-    pparts = path.parts
-    bparts = base.parts
-    if bparts[-1] in pparts:
-        idx = pparts.index(bparts[-1])
-        pparts_base = pparts[: idx + 1]
-        return pparts_base == bparts
-    return False
-
-
-def _relative_to(path, base):
-    pparts = path.parts
-    bparts = base.parts
-    if bparts[-1] in pparts:
-        idx = pparts.index(bparts[-1])
-        return pathclean("/".join(pparts[idx + 1 :]))
-    raise ValueError(
-        f"'{path}' is not in the subpath of '{base}' OR one path is "
-        f"relative and the other absolute."
-    )
-
-
-@_importer_method
-def _read_remote(*args, **kwargs):
-    from spectrochempy.core import preferences as prefs
-
-    datadir = prefs.datadir
-    dataset, path = args
-    kwargs["merge"] = kwargs.get("merge", False)  # by default, no attempt to merge
-    read_method = kwargs.pop("read_method", read)
-    download_only = kwargs.pop("download_only", False)
-    replace = kwargs.pop(
-        "replace_existing", False
-    )  # by default we download only if needed.
-
-    # downloaded file
-    # we try to download the github testdata
-    path = pathclean(path)
-
-    # we need to download additional files for topspin
-    topspin = True if "topspin" in read_method.__name__ else False
-    # we have to treat a special case: topspin, where the parent directory need
-    # to be downloaded with the required file
-    if topspin:
-        savedpath = path
-        m = re.match(r"(.*)(\/pdata\/\d+\/\d+[r|i]{1,2}|ser|fid)", str(path))
-        if m is not None:
-            path = pathclean(m[1])
-
-    if _is_relative_to(path, datadir):
-        # try to make it relative for remote downloading on github
-        relative_path = _relative_to(path, datadir)
-    else:
-        # assume it is already relative
-        relative_path = path
+# def compare_images(imgpath1, imgpath2,
+#                    max_rms=None,
+#                    min_similarity=None, ):
+#     sim, rms, _ = _image_compare(imgpath1, imgpath2, False)
+#
+#     EPSILON = np.finfo(float).eps
+#     CHECKSIM = (min_similarity is not None)
+#     SIM = min_similarity if CHECKSIM else 100. - EPSILON
+#     MESSSIM = "(similarity : {:.2f}%)".format(sim)
+#     CHECKRMS = (max_rms is not None and not CHECKSIM)
+#     RMS = max_rms if CHECKRMS else EPSILON
+#     MESSRMS = "(rms : {:.2f})".format(rms)
+#
+#     if sim < 0 or rms < 0:
+#         message = "Sizes of the images are different"
+#     elif CHECKRMS and rms <= RMS:
+#         message = "identical images {}".format(MESSRMS)
+#     elif (CHECKSIM or not CHECKRMS) and sim >= SIM:
+#         message = "identical/similar images {}".format(MESSSIM)
+#     else:
+#         message = "different images {}".format(MESSSIM)
+#
+#     return message
+#
+#
+# #
 
-    # Try to download it
-    dst = datadir / relative_path
-    if dst.name == "testdata":
-        # we are going to download the whole testdata directory
-        # -> use a faster method
-        _download_full_testdata_directory()
-        return
-    else:
-        content = _download_from_github(relative_path, dst, replace)
+# def same_images(imgpath1, imgpath2):
+#     if compare_images(imgpath1, imgpath2).startswith('identical'):
+#         return True
+#
+#
+# #
 
-    if not download_only:
-        if content is None:
-            if topspin:
-                return read_method(
-                    dataset, dst / _relative_to(savedpath, dst), **kwargs
-                )
-            else:
-                return read_method(dataset, dst, **kwargs)
-        else:
-            return read_method(dataset, dst, content=content, **kwargs)
+# def image_comparison(reference=None,
+#                      extension=None,
+#                      max_rms=None,
+#                      min_similarity=None,
+#                      force_creation=False,
+#                      savedpi=150):
+#     """
+#     image file comparison decorator.
+#
+#     Performs a comparison of the images generated by the decorated function.
+#     If none of min_similarity and max_rms if set,
+#     automatic similarity check is done :
+#
+#     Parameters
+#     ----------
+#     reference : list of image filename for the references
+#
+#         List the image filenames of the reference figures
+#         (located in ` .spectrochempy/figures` ) which correspond in
+#         the same order to
+#         the various figures created in the decorated function. if
+#         these files doesn't exist an error is generated, except if the
+#         force_creation argument is True. This should allow the creation
+#         of a reference figures, the first time the corresponding figures are
+#         created.
+#
+#     extension : str, optional, default=`png`
+#
+#         Extension to be used to save figure, among
+#         (eps, jpeg, jpg, pdf, pgf, png, ps, raw, rgba, svg, svgz, tif, tiff)
+#
+#     force_creation : `bool` , optional, default=`False` .
+#
+#         if this flag is True, the figures created in the decorated
+#         function are
+#         saved in the reference figures directory (
+#         ` .spectrocchempy/figures` )
+#
+#     min_similarity : float (percent).
+#
+#         If set, then it will be used to decide if an image is the same (
+#         similar)
+#         or not. In this case max_rms is not used.
+#
+#     max_rms : float
+#
+#         rms stands for `Root Mean Square` . If set, then it will
+#         be used to decide if an image is the same
+#         (less than the acceptable rms). Not used if min_similarity also set.
+#
+#     savedpi : int, optional, default=150
+#
+#         dot per inch of the generated figures
+#
+#     """
+#     from spectrochempy.utils import is_sequence
+#
+#     if not reference:
+#         raise ValueError('no reference image provided. Stopped')
+#
+#     if not extension:
+#         extension = 'png'
+#
+#     if not is_sequence(reference):
+#         reference = list(reference)
+#
+#     def make_image_comparison(func):
+#
+#         @functools.wraps(func)
+#         def wrapper(*args, **kwargs):
+#
+#             # check the existence of the file if force creation is False
+#             for ref in reference:
+#                 filename = os.path.join(figures_dir,
+#                                         '{}.{}'.format(ref, extension))
+#                 if not os.path.exists(filename) and not force_creation:
+#                     raise ValueError(
+#                             'One or more reference file do not exist.\n'
+#                             'Creation can be forced from the generated '
+#                             'figure, by setting force_creation flag to True')
+#
+#             # get the nums of the already existing figures
+#             # that, obviously,should not considered in
+#             # this comparison
+#             fignums = plt.get_fignums()
+#
+#             # execute the function generating the figures
+#             # rest style to basic 'lcs' style
+#             _ = func(*args, **kwargs)
+#
+#             # get the new fignums if any
+#             curfignums = plt.get_fignums()
+#             for x in fignums:
+#                 # remove not newly created
+#                 curfignums.remove(x)
+#
+#             if not curfignums:
+#                 # no figure where generated
+#                 raise RuntimeError(f'No figure was generated by the "{
+#                 func.__name__}" function. Stopped')
+#
+#             if len(reference) != len(curfignums):
+#                 raise ValueError("number of reference figures provided
+#                 doesn't match the number of generated
+#                 figures.")
+#
+#             # Comparison
+#             REDO_ON_TYPEERROR = False
+#
+#             while True:
+#                 errors = ""
+#                 for fignum, ref in zip(curfignums, reference):
+#                     referfile = os.path.join(figures_dir,
+#                                              '{}.{}'.format(ref, extension))
+#
+#                     fig = plt.figure(fignum)  # work around to set
+#                     # the correct style: we
+#                     # we have saved the rcParams
+#                     # in the figure attributes
+#                     plt.rcParams.update(fig.rcParams)
+#                     fig = plt.figure(fignum)
+#
+#                     if force_creation:
+#                         # make the figure for reference and bypass
+#                         # the rest of the test
+#                         tmpfile = referfile
+#                     else:
+#                         # else we create a temporary file to save the figure
+#                         fd, tmpfile = tempfile.mkstemp(
+#                                 prefix='temp{}-'.format(fignum),
+#                                 suffix='.{}'.format(extension), text=True)
+#                         os.close(fd)
+#
+#                     fig.savefig(tmpfile, dpi=savedpi)
+#
+#                     sim, rms = 100.0, 0.0
+#                     if not force_creation:
+#                         # we do not need to loose time
+#                         # if we have just created the figure
+#                         sim, rms, REDO_ON_TYPEERROR = _image_compare(
+#                         referfile,
+#                                                                      tmpfile,
+#                                                                      REDO_ON_TYPEERROR)
+#                     EPSILON = np.finfo(float).eps
+#                     CHECKSIM = (min_similarity is not None)
+#                     SIM = min_similarity if CHECKSIM else 100. - EPSILON
+#                     MESSSIM = "(similarity : {:.2f}%)".format(sim)
+#                     CHECKRMS = (max_rms is not None and not CHECKSIM)
+#                     RMS = max_rms if CHECKRMS else EPSILON
+#                     MESSRMS = "(rms : {:.2f})".format(rms)
+#
+#                     if sim < 0 or rms < 0:
+#                         message = "Sizes of the images are different"
+#                     elif CHECKRMS and rms <= RMS:
+#                         message = "identical images {}".format(MESSRMS)
+#                     elif (CHECKSIM or not CHECKRMS) and sim >= SIM:
+#                         message = "identical/similar images {}".format(
+#                         MESSSIM)
+#                     else:
+#                         message = "different images {}".format(MESSSIM)
+#
+#                     message += "\n\t reference : {}".format(
+#                             os.path.basename(referfile))
+#                     message += "\n\t generated : {}\n".format(
+#                             tmpfile)
+#
+#                     if not message.startswith("identical"):
+#                         errors += message
+#                     else:
+#                         print(message)
+#
+#                 if errors and not REDO_ON_TYPEERROR:
+#                     # raise an error if one of the image is different from
+#                     the
+#                     # reference image
+#                     raise ImageAssertionError("\n" + errors)
+#
+#                 if not REDO_ON_TYPEERROR:
+#                     break
+#
+#             return
+#
+#         return wrapper
+#
+#     return make_image_comparison
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/readers/read_carroucell.py` & `spectrochempy-0.6.6/spectrochempy/core/readers/read_carroucell.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import re
 import warnings
 
 import numpy as np
 import scipy.interpolate
 import xlrd
 
-from spectrochempy.core import info_
+from spectrochempy.application import info_
 from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.core.readers.importer import Importer, _importer_method
 from spectrochempy.core.readers.read_omnic import read_omnic
 from spectrochempy.utils.docstrings import _docstring
 from spectrochempy.utils.file import get_directory_name, get_filenames
 
 _docstring.delete_params("Importer.see_also", "read_carroucell")
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/readers/read_csv.py` & `spectrochempy-0.6.6/spectrochempy/core/readers/read_csv.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/core/readers/read_jcamp.py` & `spectrochempy-0.6.6/spectrochempy/core/readers/read_jcamp.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,14 +273,16 @@
     else:
         axisname = ""
         axisunit = ""
     fid.close()
 
     dataset.data = data
     dataset.name = jdx_title
+    dataset.filename = filename
+
     if yunits[0].strip() == "ABSORBANCE":
         dataset.units = "absorbance"
         dataset.title = "absorbance"
     elif yunits[0].strip() == "TRANSMITTANCE":
         # TODO: This units not in pint. Add this
         dataset.title = "transmittance"
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/readers/read_labspec.py` & `spectrochempy-0.6.6/spectrochempy/core/readers/read_labspec.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,15 @@
 
     # set dataset metadata
     dataset.data = data
     dataset.set_coordset(y=_y, x=_x)
     dataset.title = "Counts"
     dataset.units = None
     dataset.name = filename.stem
+    dataset.filename = filename
     dataset.meta = meta
 
     # date_acq is Acquisition date at start (first moment of acquisition)
     dataset.description = "Spectrum acquisition : " + str(date_acq)
 
     # Set origin, description and history
     dataset.history = f"Imported from LabSpec6 text file {filename}"
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/readers/read_matlab.py` & `spectrochempy-0.6.6/spectrochempy/core/readers/read_matlab.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,15 @@
             np.dtype("uint32"),
             np.dtype("uint64"),
         ]:
 
             # this is an array of numbers
             dataset.data = data
             dataset.name = name
+            dataset.filename = filename
             dataset.history = "Imported from .mat file"
             # TODO: reshape from fortran/Matlab order to C opder
             # for 3D or higher datasets ?
             datasets.append(dataset)
 
         elif data.dtype.char == "U":
             # this is an array of string
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/readers/read_omnic.py` & `spectrochempy-0.6.6/spectrochempy/core/readers/read_omnic.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import io
 import re
 import struct
 from datetime import datetime, timedelta, timezone
 
 import numpy as np
 
-from spectrochempy.core import info_
+from spectrochempy.application import info_
 from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.core.dataset.nddataset import NDDataset
 from spectrochempy.core.readers.importer import Importer, _importer_method, _openfid
 from spectrochempy.core.units import ur
 from spectrochempy.utils.docstrings import _docstring
 
 # ======================================================================================
@@ -682,15 +682,15 @@
             len(intensities),
             title="data points",
             units=None,
         )
 
     dataset.set_coordset(y=_y, x=_x)
     dataset.name = spa_name  # to be consistent with omnic behaviour
-    dataset.filename = str(filename)
+    dataset.filename = filename
 
     # Set origin, description, history, date
     # Omnic spg file don't have specific "origin" field stating the oirigin of the data
 
     dataset.description = kwargs.get("description", default_description) + "\n"
     if len(spa_comments) > 1:
         dataset.description += "# Comments from Omnic:\n"
@@ -836,14 +836,15 @@
 
     # in case part of the spectra/ifg has been blanked:
     dataset.mask = np.isnan(dataset.data)
 
     dataset.units = info["units"]
     dataset.title = info["title"]
     dataset.origin = "omnic"
+    dataset.filename = filename
 
     # now add coordinates
     _x = Coord.linspace(
         info["firstx"],
         info["lastx"],
         int(info["nx"]),
         title=info["xtitle"],
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/readers/read_opus.py` & `spectrochempy-0.6.6/spectrochempy/core/readers/read_opus.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 __dataset_methods__ = __all__
 
 from datetime import datetime, timedelta, timezone
 
 import numpy as np
 from brukeropusreader.opus_parser import parse_data, parse_meta
 
-from spectrochempy.core import debug_
+from spectrochempy.application import debug_
 from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.core.readers.importer import Importer, _importer_method, _openfid
 from spectrochempy.utils.docstrings import _docstring
 
 # ======================================================================================
 # Public functions
 # ======================================================================================
@@ -186,14 +186,15 @@
     # set dataset's Coordset
     dataset.set_coordset(y=yaxis, x=xaxis)
     dataset.units = "absorbance"
     dataset.title = "absorbance"
 
     # Set name, origin, description and history
     dataset.name = filename.name
+    dataset.filename = filename
     dataset.origin = "opus"
     dataset.description = "Dataset from opus files. \n"
     dataset.history = str(datetime.now(timezone.utc)) + ": import from opus files \n"
 
     # reset modification date to cretion date
     dataset._modified = dataset._created
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/readers/read_quadera.py` & `spectrochempy-0.6.6/spectrochempy/core/readers/read_quadera.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,15 @@
                 times[j][k] += 3600 * 12
             reltimes[j][k] = data[1 + 3 * k].replace(",", ".")
             ioncurrent[j][k] = data[2 + 3 * k].replace(",", ".")
         prev_timestamp = times[j][k]
 
     dataset = NDDataset(ioncurrent)
     dataset.name = filename.stem
+    dataset.filename = filename
     dataset.title = "ion current"
     dataset.units = "amp"
 
     if timestamp:
         _y = Coord(times[:, 0], title="acquisition timestamp (UTC)", units="s")
     else:
         _y = Coord(times[:, 0] - times[0, 0], title="Time", units="s")
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/readers/read_soc.py` & `spectrochempy-0.6.6/spectrochempy/core/readers/read_soc.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/core/readers/read_spc.py` & `spectrochempy-0.6.6/spectrochempy/core/readers/read_spc.py`

 * *Files 1% similar despite different names*

```diff
@@ -469,14 +469,15 @@
         )
 
         logtxt = str(content[Flogoff + Logtxto : len(content)].decode("utf-8"))
 
     # Create NDDataset Object for the series
     dataset = NDDataset(np.expand_dims(floatY, axis=0))
     dataset.name = str(filename)
+    dataset.filename = filename
     dataset.units = y_unit
     dataset.title = y_title
     dataset.origin = "thermo galactic"
 
     # now add coordinates
     _y = Coord(
         [timestamp],
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/readers/read_topspin.py` & `spectrochempy-0.6.6/spectrochempy/core/readers/read_topspin.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 __dataset_methods__ = __all__
 
 import re
 
 import numpy as np
 from quaternion import as_quat_array
 
-from spectrochempy.core import debug_
+from spectrochempy.application import debug_
 from spectrochempy.core.dataset.baseobjects.meta import Meta
 from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.core.readers.importer import Importer, _importer_method
 from spectrochempy.core.units import ur
 from spectrochempy.extern.nmrglue import read_fid, read_pdata
 from spectrochempy.utils.docstrings import _docstring
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/readers/read_zip.py` & `spectrochempy-0.6.6/spectrochempy/core/readers/read_zip.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/core/script/__init__.py` & `spectrochempy-0.6.6/spectrochempy/core/script/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Instance,
     TraitError,
     Unicode,
     signature_has_traits,
     validate,
 )
 
-from spectrochempy.core import error_
+from spectrochempy.application import error_
 from spectrochempy.core.project.abstractproject import AbstractProject
 
 __all__ = ["Script", "run_script", "run_all_scripts"]
 
 
 @signature_has_traits
 class Script(HasTraits):
```

### Comparing `spectrochempy-0.6.5/spectrochempy/core/units/__init__.py` & `spectrochempy-0.6.6/spectrochempy/core/units/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/core/writers/exporter.py` & `spectrochempy-0.6.6/spectrochempy/core/writers/exporter.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/core/writers/write_csv.py` & `spectrochempy-0.6.6/spectrochempy/core/writers/write_csv.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/core/writers/write_excel.py` & `spectrochempy-0.6.6/spectrochempy/core/writers/write_excel.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/core/writers/write_jcamp.py` & `spectrochempy-0.6.6/spectrochempy/core/writers/write_jcamp.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/core/writers/write_matlab.py` & `spectrochempy-0.6.6/spectrochempy/core/writers/write_matlab.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_efa.py` & `spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_efa.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,12 +89,10 @@
 
 # %%
 LT = pca.loadings
 LT.plot(title="PCA components", legend=LT.y.labels)
 
 # %%
 # This ends the example ! The following line can be uncommented if no plot shows when
-# running the .py script
-
-# %%
+# running the .py script with python
 
 # scp.show()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_efa_keller_massart.py` & `spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_efa_keller_massart.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,12 +92,10 @@
 # Get the abstract concentration profile based on the FIFO EFA analysis
 #
 C = efa.transform()
 C.T.plot(title="EFA concentration")
 
 # %%
 # This ends the example ! The following line can be uncommented if no plot shows when
-# running the .py script
-
-# %%
+# running the .py script with python
 
 # scp.show()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_fast_ica.py` & `spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_fast_ica.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,12 +77,10 @@
 
 # %%
 # Finally, the quality of the reconstriction can be checked by `plotmerit()`
 _ = ica.plotmerit(nb_traces=15)
 
 # %%
 # This ends the example ! The following line can be uncommented if no plot shows when
-# running the .py script
-
-# %%
+# running the .py script with python
 
 # scp.show()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_iris.py` & `spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_iris.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,12 +153,10 @@
 # sphinx_gallery_thumbnail_number = 11
 
 iris3.plotdistribution(-2)
 _ = iris3.plotmerit(-2)
 
 # %%
 # This ends the example ! The following line can be uncommented if no plot shows when
-# running the .py script
-
-# %%
+# running the .py script with python
 
 # scp.show()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_mcrals_chrom1.py` & `spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_mcrals_chrom1.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,12 +94,10 @@
 # (:math:`X`\ ) as well as the residuals (:math:`E`\ ) for few spectra.
 #
 # The fit is good and comparable to the original paper (:cite:t:`jaumot:2005`).
 _ = mcr.plotmerit(nb_traces=5)
 
 # %%
 # This ends the example ! The following line can be uncommented if no plot shows when
-# running the .py script
-
-# %%
+# running the .py script with python
 
 # scp.show()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_mcrals_kinetics.py` & `spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_mcrals_kinetics.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,12 +120,10 @@
 # Finally, let\'s plot some of the pure spectra profiles St, and the
 #  reconstructed dataset  (X_hat = C St) vs original dataset (X) and residuals.
 _ = mcr_2.St.plot()
 _ = mcr_2.plotmerit(nb_traces=10)
 
 # %%
 # This ends the example ! The following line can be uncommented if no plot shows when
-# running the .py script
-
-# %%
+# running the .py script with python
 
 # scp.show()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_nmf.py` & `spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_nmf.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,12 +72,10 @@
 for i in range(St.shape[0]):
     St.data[i] -= i * m / 2
 ax = St.plot(title="Components", colormap=None, legend=St.y.labels)
 ax.set_yticks([])
 
 # %%
 # This ends the example ! The following line can be uncommented if no plot shows when
-# running the .py script
-
-# %%
+# running the .py script with python
 
 # scp.show()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_pca_iris.py` & `spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_pca_iris.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,22 +14,17 @@
 
 """
 # %%
 # First we laod the spectrochempy API package
 import spectrochempy as scp
 
 # %%
-# Upload a dataset form a distant server
-try:
-    dataset = scp.download_iris()
-except (IOError, OSError):
-    print("Could not load The `IRIS` dataset. Finishing here.")
-    import sys
+# load a dataset from scikit-learn
+dataset = scp.load_iris()
 
-    sys.exit(0)
 # %%
 # Create a PCA object
 # Here, the number of components  wich is used by the model is automatically determined
 # using `n_components="mle"`\. Warning: `mle` cannot be used when
 # n_observations < n_features.
 pca = scp.PCA(n_components="mle")
 # %%
@@ -86,12 +81,10 @@
 # The second one - in 3D for the 3 first PC's - indicates that a thid PC won't allow
 # better distinguishing versicolor from viginica.
 ax = pca.scoreplot(scores, 1, 2, 3, color_mapping="labels")
 ax.view_init(10, 75)
 
 # %%
 # This ends the example ! The following line can be uncommented if no plot shows when
-# running the .py script
-
-# %%
+# running the .py script with python
 
 # scp.show()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_pca_spec.py` & `spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_pca_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,16 @@
 _ = pca.loadings.plot(legend=True)
 
 # %%
 # Let's plot the scores
 scores = pca.transform()
 _ = pca.scoreplot(scores, 1, 2)
 
-# %% labeling scoreplot with spectra labels
+# %%
+# Labeling scoreplot with spectra labels
 # Our dataset has already two columns of labels for the spectra but there are little
 # too long for display on plots.
 scores.y.labels
 
 # %%
 # So we define some short labels for each component, and add them as a third column:
 labels = [lab[:6] for lab in dataset.y.labels[:, 1]]
@@ -95,12 +96,10 @@
 
 # %%
 # now display thse
 _ = pca.scoreplot(scores, 1, 2, show_labels=True, labels_column=2)
 
 # %%
 # This ends the example ! The following line can be uncommented if no plot shows when
-# running the .py script
-
-# %%
+# running the .py script with python
 
 # scp.show()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_pls.py` & `spectrochempy-0.6.6/spectrochempy/examples/analysis/b_crossdecomposition/plot_pls.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,12 +65,10 @@
 _ = pls.parityplot(
     y_test, pls.predict(X_test), s=150, c="red", label="validation", clear=False
 )
 _ = ax.legend(loc="lower right")
 
 # %%
 # This ends the example ! The following line can be uncommented if no plot shows when
-# running the .py script
-
-# %%
+# running the .py script with python
 
 # scp.show()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/analysis/plot_simplisma.py` & `spectrochempy-0.6.6/spectrochempy/examples/analysis/a_decomposition/plot_simplisma.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,12 +56,10 @@
 # %%
 # Show the plot of merit
 # after reconstruction oto the original data space
 simpl.plotmerit(offset=0, nb_traces=5)
 
 # %%
 # This ends the example ! The following line can be uncommented if no plot shows when
-# running the .py script
-
-# %%
+# running the .py script with python
 
 # scp.show()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/fitting/plot_fit.py` & `spectrochempy-0.6.6/spectrochempy/examples/analysis/c_curvefitting/plot_fit.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,12 +105,11 @@
 ax.autoscale(enable=True, axis="y")
 
 # plotmerit
 som = f1.inverse_transform()
 f1.plotmerit(ndOH, som, method="scatter", markevery=5, markersize=2)
 
 # %%
-# This ends the example ! The following line can be uncommented if no plot shows when running
-# the .py script
+# This ends the example ! The following line can be uncommented if no plot shows when
+# running the .py script with python
 
-# %%
 # scp.show()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/fitting/plot_lstsq_single_equation.py` & `spectrochempy-0.6.6/spectrochempy/examples/analysis/c_curvefitting/plot_lstsq_single_equation.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,12 +113,11 @@
     label="Original data",
     title=f"Least-square regression, $r^2={rsquare:.3f}$",
 )
 distance_fitted3 = lstsq.predict()
 distance_fitted3.plot_pen(clear=False, color="g", label="Fitted line", legend=True)
 
 # %%
-# This ends the example ! The following line can be uncommented if no plot shows when running
-# the .py script
+# This ends the example ! The following line can be uncommented if no plot shows when
+# running the .py script with python
 
-# %%
 # scp.show()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/nddataset/plot_coordinates.py` & `spectrochempy-0.6.6/spectrochempy/examples/core/a_nddataset/plot_b_coordinates.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,12 +133,11 @@
 c_wavelength = row10.x.to("nanometer")
 print(c_wavenumber, c_wavelength)
 row10.x = [c_wavenumber, c_wavelength]
 row10.x.select(2)
 _ = row10.plot()
 
 # %%
-# This ends the example ! The following line can be uncommented if no plot shows when running
-# the .py script
+# This ends the example ! The following line can be uncommented if no plot shows when
+# running the .py script with python
 
-# %%
 # scp.show()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/nddataset/plot_create_dataset.py` & `spectrochempy-0.6.6/spectrochempy/examples/core/a_nddataset/plot_a_create_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 # axis and the array of data
 import numpy as np
 
 # %%
 # As usual, we start by loading the spectrochempy library
 import spectrochempy as scp
 
+# %%
+# We create the data for the coordinates axis and the array of data
 c0 = np.linspace(200.0, 300.0, 3)
 c1 = np.linspace(0.0, 60.0, 100)
 c2 = np.linspace(4000.0, 1000.0, 100)
 nd_data = np.array(
     [
         np.array([np.sin(2.0 * np.pi * c2 / 4000.0) * np.exp(-y / 60) for y in c1]) * t
         for t in c0
@@ -92,12 +94,11 @@
 new.plot(method="stack")
 
 # %%
 # Note that the scp allows one to use this syntax too:
 scp.plot_stack(new)
 
 # %%
-# This ends the example ! The following line can be uncommented if no plot shows when running
-# the .py script
+# This ends the example ! The following line can be uncommented if no plot shows when
+# running the .py script with python
 
-# %%
 # scp.show()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/nddataset/plot_units.py` & `spectrochempy-0.6.6/spectrochempy/examples/core/a_nddataset/plot_c_units.py`

 * *Files 9% similar despite different names*

```diff
@@ -111,12 +111,11 @@
 
 ""
 ds.ito("absorbance")
 ds.x.ito("cm^-1")
 _ = ds.plot()
 
 # %%
-# This ends the example ! The following line can be uncommented if no plot shows when running
-# the .py script
+# This ends the example ! The following line can be uncommented if no plot shows when
+# running the .py script with python
 
-# %%
 # scp.show()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/plotting/plot_plotting.py` & `spectrochempy-0.6.6/spectrochempy/examples/core/d_plotting/plot_plotting.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,12 +56,11 @@
 )
 
 # %%
 # check that style reinit to default
 _ = scp.plot_multiple(method="scatter", datasets=datasets, labels=labels, legend="best")
 
 # %%
-# This ends the example ! The following line can be uncommented if no plot shows when running
-# the .py script
+# This ends the example ! The following line can be uncommented if no plot shows when
+# running the .py script with python
 
-# %%
 # scp.show()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/processing/plot_proc_em.py` & `spectrochempy-0.6.6/spectrochempy/examples/processing/apodization/plot_proc_em.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,21 +41,22 @@
 new2, curve2 = dataset1D.copy().em(
     lb=100 * Hz, shifted=10000 * us, retapod=True, inplace=False
 )
 
 # %%
 # Plotting
 
-p = dataset1D.plot(zlim=(-2, 2), color="k")
+_ = dataset1D.plot(zlim=(-2, 2), color="k")
 
-curve1.plot(color="r")
-new1.plot(color="r", clear=False, label=" em = 20 hz")
+_ = curve1.plot(color="r")
+_ = new1.plot(color="r", clear=False, label=" em = 20 hz")
 
-curve2.plot(color="b", clear=False)
-new2.plot(dcolor="b", clear=False, label=" em = 30 HZ, shifted = ")
+_ = curve2.plot(color="b", clear=False)
+_ = new2.plot(dcolor="b", clear=False, label=" em = 30 HZ, shifted = ")
 
 # %%
-# This ends the example ! The following line can be uncommented if no plot shows when running
-# the .py script
+# This ends the example ! The following line can be uncommented if no plot shows when
+# running the .py script with python
 
-# %%
 # scp.show()
+
+# sphinx_gallery_thumbnail_number = -1
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/processing/plot_proc_sp.py` & `spectrochempy-0.6.6/spectrochempy/examples/processing/apodization/plot_proc_sp.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,12 +87,13 @@
     ls="--",
     clear=False,
     label=" sinm with ssb= 8",
     legend="best",
 )
 
 # %%
-# This ends the example ! The following line can be uncommented if no plot shows when running
-# the .py script
+# This ends the example ! The following line can be uncommented if no plot shows when
+# running the .py script with python
 
-# %%
 # scp.show()
+
+# sphinx_gallery_thumbnail_number = -1
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/project/plot_project.py` & `spectrochempy-0.6.6/spectrochempy/examples/core/e_project/plot_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,12 +103,11 @@
 #show()
 """
 proj["tgscatter"] = scp.Script("tgscatter", script_source_2)
 
 proj.tgscatter()
 
 # %%
-# This ends the example ! The following line can be uncommented if no plot shows when running
-# the .py script
+# This ends the example ! The following line can be uncommented if no plot shows when
+# running the .py script with python
 
-# %%
 # scp.show()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/read/plot_generic_read.py` & `spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/plot_generic_read.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,12 +75,11 @@
 )
 _ = dataset_list[-1].plot()
 _ = dataset_list[-2].plot()
 _ = dataset_list[-3].plot()
 _ = dataset_list[-4].plot()
 
 # %%
-# This ends the example ! The following line can be uncommented if no plot shows when running
-# the .py script
+# This ends the example ! The following line can be uncommented if no plot shows when
+# running the .py script with python
 
-# %%
 # scp.show()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/read/plot_read_IR_from_omnic.py` & `spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/plot_read_IR_from_omnic.py`

 * *Files 23% similar despite different names*

```diff
@@ -31,12 +31,11 @@
 dataset.y.to("hour")
 dataset.y -= dataset.y[0]
 dataset.y.title = "acquisition time"
 
 _ = dataset.plot_stack()
 
 # %%
-# This ends the example ! The following line can be uncommented if no plot shows when running
-# the .py script
+# This ends the example ! The following line can be uncommented if no plot shows when
+# running the .py script with python
 
-# %%
 # scp.show()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/read/plot_read_IR_from_opus.py` & `spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/plot_read_IR_from_opus.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,12 +23,11 @@
 
 # %%
 # plot it
 
 _ = Z.plot()
 
 # %%
-# This ends the example ! The following line can be uncommented if no plot shows when running
-# the .py script
+# This ends the example ! The following line can be uncommented if no plot shows when
+# running the .py script with python
 
-# %%
 # scp.show()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/read/plot_read_nmr_from_bruker.py` & `spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/plot_read_nmr_from_bruker.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,12 +36,11 @@
 # Now load a 2D  dataset
 
 path = datadir / "nmrdata" / "bruker" / "tests" / "nmr" / "topspin_2d"
 ndd = scp.read_topspin(path, expno=1, remove_digital_filter=True)
 _ = scp.plot(ndd)
 
 # %%
-# This ends the example ! The following line can be uncommented if no plot shows when running
-# the .py script
+# This ends the example ! The following line can be uncommented if no plot shows when
+# running the .py script with python
 
-# %%
 # scp.show()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/examples/read/plot_read_raman_from_labspec.py` & `spectrochempy-0.6.6/spectrochempy/examples/core/c_importer/plot_read_raman_from_labspec.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,12 +41,11 @@
 
 # %%
 # this pack all spectra of the subdir directory (without dialog - look at the difference above)
 B = scp.read_labspec(ramandir / "subdir")
 _ = B.plot()
 
 # %%
-# This ends the example ! The following line can be uncommented if no plot shows when running
-# the .py script
+# This ends the example ! The following line can be uncommented if no plot shows when
+# running the .py script with python
 
-# %%
 # scp.show()
```

### Comparing `spectrochempy-0.6.5/spectrochempy/extern/nmrglue.py` & `spectrochempy-0.6.6/spectrochempy/extern/nmrglue.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/extern/traittypes.py` & `spectrochempy-0.6.6/spectrochempy/extern/traittypes.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/extern/traittypes_utils.py` & `spectrochempy-0.6.6/spectrochempy/extern/traittypes_utils.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/ipython/magics.py` & `spectrochempy-0.6.6/spectrochempy/ipython/magics.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/__init__.py` & `spectrochempy-0.6.6/spectrochempy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/citation.py` & `spectrochempy-0.6.6/spectrochempy/utils/citation.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         """
         self._js["publication_date"] = date.today().isoformat()
 
     def update_version(self, version=None):
         """
         Update the version string metadata
         """
-        from spectrochempy.core import version as scpversion
+        from spectrochempy.application import version as scpversion
 
         if version is None:
             version = scpversion
         self._js["version"] = ".".join(version.split(".")[:3])
 
     def __str__(self):
         return json.dumps(self._js, indent=2)
@@ -134,12 +134,12 @@
         """
         self._citation.cffobj["date-released"] = date.today().isoformat()
 
     def update_version(self, version=None):
         """
         Update the version metadata.
         """
-        from spectrochempy.core import version as scpversion
+        from spectrochempy.application import version as scpversion
 
         if version is None:
             version = scpversion
         self._citation.cffobj["version"] = ".".join(version.split(".")[:3])
```

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/compare.py` & `spectrochempy-0.6.6/spectrochempy/utils/compare.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/constants.py` & `spectrochempy-0.6.6/spectrochempy/utils/constants.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/coordrange.py` & `spectrochempy-0.6.6/spectrochempy/utils/coordrange.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,23 +71,23 @@
         if self.reversed:
             for range in self.ranges:
                 range.reverse()
             self.ranges.reverse()
 
 
 def trim_ranges(*ranges, reversed=False):
-    """
-    Set of ordered, non intersecting intervals.
+    r"""
+    Set of ordered, non-intersecting intervals.
 
     An ordered set of ranges is constructed from the inputs and returned.
     *e.g.,* [[a, b], [c, d]] with a < b < c < d or a > b > c > d.
 
     Parameters
     -----------
-    \*ranges :  iterable
+    *ranges :  iterable
         An interval or a set of intervals.
         set of  intervals. If none is given, the range will be a set of an empty
         interval [[]]. The interval
         limits do not need to be ordered, and the intervals do not need to be distincts.
     reversed : bool, optional
         The intervals are ranked by decreasing order if True or increasing order if
         False.
```

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/docstrings.py` & `spectrochempy-0.6.6/spectrochempy/utils/docstrings.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,19 +47,31 @@
     "EX03": "flake8 error: {error_code} {error_message}{times_happening}",
     "EX04": "Do not import {imported_library}, as it is imported "
     "automatically for the examples (numpy as np, spectrochempy as scp)",
 }
 
 
 _common_doc = """
+out : `object`
+    Input object or a newly allocated object, depending on the `inplace` flag.
+new : `object`
+    Newly allocated object.
 copy : `bool`, optional, default: `True`
     Perform a copy of the passed object.
 inplace : `bool`, optional, default: `False`
     By default, the method returns a newly allocated object.
     If `inplace` is set to `True`, the input object is returned.
+dataset : `NDDataset` or :term:`array-like` of shape (:term:`n_observations`\ , :term:`n_features`\ )
+    Input data, where :term:`n_observations` is the number of observations
+    and :term:`n_features` is the number of features.
+dim : `int` or `str`, optional, default: -1,
+    Dimension along which the method is applied.
+    By default, the method is applied to the last dimension.
+    If `dim` is specified as an integer it is equivalent to the usual `axis` numpy
+    parameter.
 **kwargs : keyword parameters, optional
     See Other Parameters.
 """
 
 
 class DocstringProcessor(docrep.DocstringProcessor):
 
@@ -72,22 +84,14 @@
         regex = re.compile(r"(?=^[*]{0,2}\b\w+\b\s?:?\s?)", re.MULTILINE | re.DOTALL)
         plist = regex.split(_common_doc.strip())[1:]
         params = {
             k.strip("*"): f"{k.strip()} : {v.strip()}"
             for k, v in (re.split(r"\s?:\s?", p, maxsplit=1) for p in plist)
         }
         self.params.update(params)
-        self.params.update(
-            {
-                "out": "`object`\n"
-                "    Input object or a newly allocated object\n"
-                "    depending on the `inplace` flag.",
-                "new": "`object`\n" "    Newly allocated object.",
-            }
-        )
 
     def dedent(self, s, stacklevel=3):
         s_ = s
         start = ""
         end = ""
         string = True
         if not isinstance(s, str) and hasattr(s, "__doc__"):
```

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/exceptions.py` & `spectrochempy-0.6.6/spectrochempy/utils/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
 SpectroChemPy specific exceptions
 """
+import inspect
 from contextlib import contextmanager
 
 import pint
 import pytz
 
 
 # ======================================================================================
@@ -56,14 +57,66 @@
 
     def __init__(self, message):
         self.message = message
 
         super().__init__(message)
 
 
+# ======================================================================================
+# Exceptions for configurable models
+# ======================================================================================
+class NotTransformedError(SpectroChemPyError):
+    """
+    Exception raised when a model has not yet been applied to a dataset,
+    but one use one of its method.
+
+    Parameters
+    ----------
+    attr : method, optional
+        The method from which the error was issued. In general, it is determined
+        automatically.
+    """
+
+    def __init__(self, attr=None, message=None):
+        if message is not None:
+            super().__init__(message)
+            return
+        frame = inspect.currentframe().f_back
+        caller = frame.f_code.co_name if attr is None else attr
+        model = frame.f_locals["self"].name
+        message = (
+            f"To use `{caller}` ,  the method `apply` of model `{model}`"
+            f" should be executed first"
+        )
+        super().__init__(message)
+
+
+class NotFittedError(NotTransformedError):
+    """
+    Exception raised when an analysis estimator is not fitted
+    but one use one of its method.
+
+    Parameters
+    ----------
+    attr : method, optional
+        The method from which the error was issued. In general, it is determined
+        automatically.
+    """
+
+    def __init__(self, attr=None, message=None):
+        frame = inspect.currentframe().f_back
+        caller = frame.f_code.co_name if attr is None else attr
+        model = frame.f_locals["self"].name
+        message = (
+            f"To use `{caller}` ,  the method `fit` of model `{model}`"
+            f" should be executed first"
+        )
+        super().__init__(message=message)
+
+
 class CastingError(SpectroChemPyError):
     """
     Exception raised when an array cannot be cast to the required data type
     """
 
     def __init__(self, dtype, message):
         message = f" Assigned value has type {dtype} but {message}"
@@ -82,21 +135,14 @@
     """
 
     def __init__(self, shape, message):
         message = f" Assigned value has shape {shape} but {message}"
         super().__init__(message)
 
 
-# Analysis method errors
-class NotFittedError(SpectroChemPyError):
-    """
-    Exception raised when an analysis estimtor is not fitted before use.
-    """
-
-
 class MissingDataError(SpectroChemPyError):
     """
     Exception raised when no data is present in an object.
     """
 
 
 class NDDatasetAttributeError(SpectroChemPyError):
```

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/fake.py` & `spectrochempy-0.6.6/spectrochempy/utils/fake.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 
 
 # --------------------------------------------------------------------------------------
 # Create fake data to be used by analysis routine for testing
 # --------------------------------------------------------------------------------------
 def _make_spectra_matrix(modelname, ampl, pos, width, ratio=None, asym=None):
-    from spectrochempy.analysis.optimize import _models
+    from spectrochempy.analysis.curvefitting import _models
     from spectrochempy.core.dataset.coord import Coord
     from spectrochempy.core.dataset.nddataset import NDDataset
 
     x = Coord(np.linspace(6000.0, 1000.0, 4000), units="cm^-1", title="wavenumbers")
     s = []
     for arg in zip(modelname, ampl, pos, width, ratio, asym):
         model = getattr(_models, arg[0] + "model")()
@@ -55,16 +55,16 @@
     -------
     datasets:
         2D spectra, individual spectra and concentrations
     """
 
     # define properties of the spectra and concentration profiles
     # ----------------------------------------------------------------------------------
-    from spectrochempy.analysis.optimize import _models
-    from spectrochempy.core.dataset.arraymixins.npy import dot
+    from spectrochempy.analysis.curvefitting import _models
+    from spectrochempy.processing.transformation.npy import dot
 
     # data for four peaks (one very broad)
     POS = (6000.0, 4000.0, 2000.0, 2500.0)
     WIDTH = (6000.0, 1000.0, 250.0, 800.0)
     AMPL = (100.0, 70.0, 10.0, 50.0)
     RATIO = (0.1, 0.5, 0.2, 1.0)
     ASYM = (0.0, 0.0, 0, 4)
```

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/file.py` & `spectrochempy-0.6.6/spectrochempy/utils/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -625,15 +625,15 @@
 
 
 def check_filename_to_save(
     dataset, filename=None, save_as=False, confirm=True, **kwargs
 ):
 
     from spectrochempy import NO_DIALOG
-    from spectrochempy.core import info_
+    from spectrochempy.application import info_
 
     NODIAL = (NO_DIALOG or "DOC_BUILDING" in environ) and "KEEP_DIALOGS" not in environ
 
     if filename and pathclean(filename).parent.resolve() == Path.cwd():
         filename = Path.cwd() / filename
 
     if not filename or save_as or filename.exists():
```

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/jsonutils.py` & `spectrochempy-0.6.6/spectrochempy/utils/jsonutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,28 +141,28 @@
             }
         else:
             return {
                 "base64": base64.b64encode(pickle.dumps(byte_obj)).decode(),
                 "__class__": "NUMPY_ARRAY",
             }
 
-    elif isinstance(byte_obj, pathlib.PosixPath):
+    elif isinstance(byte_obj, (pathlib.PosixPath, pathlib.WindowsPath)):
         return {"str": str(byte_obj), "__class__": "PATH"}
 
     elif isinstance(byte_obj, Unit):
         strunits = f"{byte_obj:D}"
         return {"str": strunits, "__class__": "UNIT"}
 
     elif isinstance(byte_obj, Quantity):
         return {
             "tuple": json_serialiser(byte_obj.to_tuple(), encoding=encoding),
             "__class__": "QUANTITY",
         }
 
-    elif isinstance(byte_obj, (np.complex128, np.complex64, np.complex)):
+    elif isinstance(byte_obj, (np.complex128, np.complex64, complex)):
         if encoding is None:
             return {
                 "tolist": json_serialiser(
                     [byte_obj.real, byte_obj.imag], encoding=encoding
                 ),
                 "dtype": str(byte_obj.dtype),
                 "__class__": "COMPLEX",
```

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/misc.py` & `spectrochempy-0.6.6/spectrochempy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/numutils.py` & `spectrochempy-0.6.6/spectrochempy/utils/numutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,19 +89,20 @@
     Returns
     -------
     pw : int
         Power of 2.
     """
     return int(pow(2, np.ceil(np.log(value) / np.log(2))))
 
+    #
+    #
+    # def make_func_from(func, first=None):
+    # """
+
 
-#
-#
-# def make_func_from(func, first=None):
-#     """
 #     Create a new func with its arguments from another func and a new signature.
 #     """
 #     code_obj = func.__code__
 #     new_varnames = list(code_obj.co_varnames)
 #     if first:
 #         new_varnames[0] = first
 #     new_varnames = tuple(new_varnames)
```

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/objects.py` & `spectrochempy-0.6.6/spectrochempy/utils/objects.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/optional.py` & `spectrochempy-0.6.6/spectrochempy/utils/optional.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/orderedset.py` & `spectrochempy-0.6.6/spectrochempy/utils/orderedset.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/packages.py` & `spectrochempy-0.6.6/spectrochempy/utils/packages.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/plots.py` & `spectrochempy-0.6.6/spectrochempy/utils/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -451,14 +451,16 @@
     n = plt.get_fignums()
 
     clear = kwargs.get("clear", True)
 
     if not n or clear:
         # create a figure
         prefs = kwargs.pop("preferences", None)
+        if prefs is None:
+            return None
 
         figsize = kwargs.get("figsize", prefs.figure_figsize)
         dpi = kwargs.get("dpi", prefs.figure_dpi)
         facecolor = kwargs.get("facecolor", prefs.figure_facecolor)
         edgecolor = kwargs.get("edgecolor", prefs.figure_edgecolor)
         frameon = kwargs.get("frameon", prefs.figure_frameon)
         tight_layout = kwargs.get("autolayout", prefs.figure_autolayout)
```

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/print.py` & `spectrochempy-0.6.6/spectrochempy/utils/print.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/print_versions.py` & `spectrochempy-0.6.6/spectrochempy/utils/print_versions.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/system.py` & `spectrochempy-0.6.6/spectrochempy/utils/system.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/traits.py` & `spectrochempy-0.6.6/spectrochempy/utils/traits.py`

 * *Files 22% similar despite different names*

```diff
@@ -94,7 +94,43 @@
     def __init__(self, default_value=Empty, allow_none=False, dtype=None, **kwargs):
         if "klass" not in kwargs and self.klass is None:
             from spectrochempy.core.dataset.coord import Coord
 
             kwargs["klass"] = Coord
         super().__init__(default_value=default_value, allow_none=allow_none, **kwargs)
         self.metadata.update({"dtype": dtype})
+
+
+class PositiveInteger(tr.Integer):
+    """
+    A trait for positive integer values.
+    """
+
+    info_text = "a positive integer"
+    default_value = 0
+
+    def validate(self, obj, value):
+        if value is None and not self.allow_none:
+            self.error(obj, value)
+        if value is None or value is tr.Undefined:
+            return super().validate(obj, value)
+        if value < 0:
+            self.error(obj, value)
+        return super().validate(obj, value)
+
+
+class PositiveOddInteger(tr.Integer):
+    """
+    A trait for positive odd integer values.
+    """
+
+    info_text = "a positive odd integer"
+    default_value = 1
+
+    def validate(self, obj, value):
+        if value is None and not self.allow_none:
+            self.error(obj, value)
+        if value is None or value is tr.Undefined:
+            return super().validate(obj, value)
+        if value < 0 or value % 2 == 0:
+            self.error(obj, value)
+        return super().validate(obj, value)
```

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/version.py` & `spectrochempy-0.6.6/spectrochempy/utils/version.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/warnings.py` & `spectrochempy-0.6.6/spectrochempy/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/utils/zip.py` & `spectrochempy-0.6.6/spectrochempy/utils/zip.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy/widgets/baselinecorrector.py` & `spectrochempy-0.6.6/spectrochempy/widgets/baselinecorrector.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,19 @@
 # ======================================================================================
 import re
 from functools import partial
 
 from IPython.display import display
 from ipywidgets import Layout, widgets
 
-from spectrochempy.core import info_, warning_
+from spectrochempy.analysis.baseline.baseline import Baseline
+from spectrochempy.application import info_, warning_
 from spectrochempy.core.dataset.nddataset import NDDataset
 from spectrochempy.core.plotters.multiplot import multiplot
-from spectrochempy.core.processors.baseline import BaselineCorrection
-from spectrochempy.core.processors.concatenate import concatenate
 from spectrochempy.core.readers.importer import read
-from spectrochempy.utils.plots import show
 
 __all__ = ["BaselineCorrector"]
 
 
 class BaselineCorrector:
     """
     Launch a GUI for baseline corrections.
@@ -28,16 +26,17 @@
     Wrapper of BaselineCorrection(X), with widgets for dataset slicing,
     input parameters and graphical output.
     Should be run in jupyter notebook (does not always run properly in jupyter lab)
     with the widget backend (magic `%matplotlib widget` ).
 
     Parameters
     ----------
-    X : `NDDataset`\, default: None
-        The NDDataset to process. If None, an upload button can be used to load data.
+    X : `NDDataset`\ , default: `None`
+        The `NDDataset` to process. If `None`, an upload button can be used to load
+        data.
     initial_ranges : list, optional, default: None
         The initial regions where to compute the baseline. If not given, 5% on each
         side of the spectra will be taken as a starting range's list.
 
     Attributes
     ----------
     original : `NDDataset`
@@ -88,31 +87,35 @@
     """
 
     def __init__(self, X=None, initial_ranges=None):
 
         if not isinstance(X, (NDDataset, type(None))):
             raise ValueError("X must be None or a valid NDDataset")
 
+        self.blc = Baseline()
+
         self._X = X
         self._fig = None
         self._initial_ranges = initial_ranges
         self._done = False
 
         # I/O and processing widgets
         self._load_button = widgets.Button(description="Upload", icon="upload")
         self._load_button.on_click(self._load_clicked)
         self._process_button = widgets.Button(description="Process", icon="play")
         self._process_button.on_click(self._process_clicked)
         self._save_button = widgets.Button(description="Save as", icon="save")
         self._save_button.on_click(self._save_clicked)
 
         # Parameters widgets
-        self._npc_slider = widgets.IntSlider(description="N pc", value=1, min=1, max=5)
+        self._npc_slider = widgets.IntSlider(
+            description="N components", value=1, min=1, max=5
+        )
         self._order_slider = widgets.IntSlider(
-            description="Order", layout=Layout(width="350px"), value=1, min=1, max=6
+            description="Order", layout=Layout(width="350px"), value=1, min=1, max=10
         )
 
         self._method_selector = widgets.Dropdown(
             description="Method",
             options=["sequential", "multivariate"],
             value="sequential",
         )
@@ -140,16 +143,14 @@
         self._input = widgets.HBox(children=[self._io, self._controls])
         self._output = widgets.Output()
         display(self._input)
         display(self._output)
 
         # init attributes
         self.original = NDDataset()
-        self.corrected = NDDataset()
-        self.baseline = NDDataset()
 
         # events
         for control in [
             "x_limits_control",
             "y_limits_control",
             "ranges_control",
             "npc_slider",
@@ -224,47 +225,60 @@
             new_ranges, changed = _update_ranges(
                 _str_to_ranges(self._ranges_control.value), self.original.x.data
             )
             if changed:
                 ranges = _round_ranges(new_ranges)
                 self._ranges_control.value = _ranges_to_str(ranges)
 
-            blc = BaselineCorrection(self.original)
-            self.corrected = blc.compute(
-                *ranges,
-                interpolation=self._interpolation_selector.value,
-                order=self._order_slider.value,
-                method=self._method_selector.value,
-                npc=self._npc_slider.value,
+            self.blc.ranges = list(ranges)
+            self.blc.model = "polynomial"
+            interpolation = self._interpolation_selector.value
+            self.blc.order = (
+                self._order_slider.value if interpolation == "polynomial" else "pchip"
             )
-            self.baseline = self.original - self.corrected
+            self.blc.multivariate = self._method_selector.value == "multivariate"
+            self.blc.n_components = self._npc_slider.value
+
+            self.blc.fit(self.original)
 
             self._output.clear_output(True)
             with self._output:
                 axes = multiplot(
                     [
-                        concatenate(self.original, self.baseline, dims="y"),
-                        self.corrected,
+                        self.original,
+                        self.blc.corrected,
                     ],
-                    labels=["Original", "Corrected"],
+                    labels=["Original", "Baseline corrected"],
                     sharex=True,
                     nrow=2,
                     ncol=1,
                     fig=self._fig,
                     figsize=(8, 6),
                     dpi=96,
                     left=0.12,
                     mpl_event=False,
                 )
                 axes["axe11"].get_xaxis().set_visible(False)
-                blc.show_regions(axes["axe21"])
-                self._fig = axes["axe21"].figure
-                show()
+                self.blc.show_regions(axes["axe11"])
+                self._fig = axes["axe11"].figure
+
+                ylim = axes["axe11"].get_ylim()
+                self.blc.baseline.plot(ax=axes["axe11"], cmap="copper")
+                axes["axe11"].set_ylim(ylim)
+
             self._done = True
 
+    @property
+    def corrected(self):
+        return self.blc.corrected
+
+    @property
+    def baseline(self):
+        return self.blc.baseline
+
     def _load_clicked(self, b=None):
         # read data and reset defaults
         ds = read()
         if ds is not None:
             if isinstance(ds, NDDataset):
                 self._X = ds
                 self._method_selector.value = "sequential"
@@ -304,16 +318,16 @@
             self._y_limits_control.value = _y_slice_to_str(slice(0, len(self._X.y), 1))
             # ... and baseline correct with defaults
 
         self._blcorrect_and_plot()
         self._process_button.disabled = True
 
     def _save_clicked(self, b=None):
-        if self.corrected is not None:
-            return self.corrected.write()
+        if self.blc.corrected is not None:
+            return self.blc.corrected.write()
 
 
 # Utility functions
 def _x_slice_to_str(slice, dataset, decimals=2):
     return (
         f"[{round(dataset.x.data[slice.start], decimals)} : "
         f"{round(dataset.x.data[slice.stop - 1], decimals)} : {slice.step}]"
```

### Comparing `spectrochempy-0.6.5/spectrochempy/widgets/fileselector.py` & `spectrochempy-0.6.6/spectrochempy/widgets/fileselector.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.5/spectrochempy.egg-info/PKG-INFO` & `spectrochempy-0.6.6/spectrochempy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrochempy
-Version: 0.6.5
+Version: 0.6.6
 Summary: Processing, analysis and modelling Spectroscopic data for Chemistry with Python
 Home-page: https://www.spectrochempy.fr
 Author: Arnaud Travert & Christian Fernandez
 Author-email: contact@spectrochempy.fr
 Maintainer: C. Fernandez
 Maintainer-email: christian.fernandez@ensicaen.fr
 License: CECILL-B
```

