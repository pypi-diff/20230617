# Comparing `tmp/lammps_step-2023.6.16.tar.gz` & `tmp/lammps_step-2023.6.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lammps_step-2023.6.16.tar", last modified: Fri Jun 16 17:31:31 2023, max compression
+gzip compressed data, was "lammps_step-2023.6.17.tar", last modified: Sat Jun 17 02:12:51 2023, max compression
```

## Comparing `lammps_step-2023.6.16.tar` & `lammps_step-2023.6.17.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.918614 lammps_step-2023.6.16/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-06-16 17:31:31.918614 lammps_step-2023.6.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.890614 lammps_step-2023.6.16/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.890614 lammps_step-2023.6.16/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.890614 lammps_step-2023.6.16/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9562 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.894614 lammps_step-2023.6.16/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.902614 lammps_step-2023.6.16/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)  2437613 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/getting_started/density.png
--rw-r--r--   0 runner    (1001) docker     (123)   175972 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/getting_started/edit_forcefield.png
--rw-r--r--   0 runner    (1001) docker     (123)   312162 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/getting_started/edit_initialization.png
--rw-r--r--   0 runner    (1001) docker     (123)   877297 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/getting_started/edit_npt.png
--rw-r--r--   0 runner    (1001) docker     (123)   575423 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/getting_started/edit_packmol.png
--rw-r--r--   0 runner    (1001) docker     (123)   408930 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/getting_started/flowchart.png
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)   220257 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/getting_started/lammps_flowchart.png
--rw-r--r--   0 runner    (1001) docker     (123)   148973 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/getting_started/nist.png
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.902614 lammps_step-2023.6.16/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.922614 lammps_step-2023.6.16/lammps_step/
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      492 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-16 17:31:31.922614 lammps_step-2023.6.16/lammps_step/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/custom_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/custom_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.918614 lammps_step-2023.6.16/lammps_step/data/
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/data/configuration.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/data/properties.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/data/seamm-lammps.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/energy_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/energy_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    18198 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/heat_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/heat_flux_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/heat_flux_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    22441 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/initialization_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/initialization_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    24239 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)    91984 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/lammps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/lammps_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/lammps_units.py
--rw-r--r--   0 runner    (1001) docker     (123)    11638 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/minimization.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/minimization_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    23933 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/npt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/npt_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/npt_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    16217 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/nve.py
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/nve_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/nve_step.py
--rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/nvt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/nvt_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/nvt_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/tk_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/tk_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/tk_heat_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/tk_initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/tk_lammps.py
--rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/tk_minimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    30919 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/tk_npt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/tk_nve.py
--rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/tk_nvt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/tk_velocities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/velocities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/velocities_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/lammps_step/velocities_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.918614 lammps_step-2023.6.16/lammps_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-06-16 17:31:31.000000 lammps_step-2023.6.16/lammps_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-16 17:31:31.000000 lammps_step-2023.6.16/lammps_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:31:31.000000 lammps_step-2023.6.16/lammps_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-16 17:31:31.000000 lammps_step-2023.6.16/lammps_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-16 17:31:31.000000 lammps_step-2023.6.16/lammps_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 17:31:31.000000 lammps_step-2023.6.16/lammps_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:31:19.000000 lammps_step-2023.6.16/lammps_step.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-16 17:31:31.922614 lammps_step-2023.6.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.918614 lammps_step-2023.6.16/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:31:31.918614 lammps_step-2023.6.16/tests/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14459 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/tests/data/Ar_xtal_energy.flow
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/tests/test_lammps_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/tests/test_lammps_units.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-16 17:31:16.000000 lammps_step-2023.6.16/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:12:51.539282 lammps_step-2023.6.17/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-06-17 02:12:51.539282 lammps_step-2023.6.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:12:51.511282 lammps_step-2023.6.17/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:12:51.515282 lammps_step-2023.6.17/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:12:51.515282 lammps_step-2023.6.17/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9562 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:12:51.515282 lammps_step-2023.6.17/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:12:51.523282 lammps_step-2023.6.17/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)  2437613 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/getting_started/density.png
+-rw-r--r--   0 runner    (1001) docker     (123)   175972 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/getting_started/edit_forcefield.png
+-rw-r--r--   0 runner    (1001) docker     (123)   312162 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/getting_started/edit_initialization.png
+-rw-r--r--   0 runner    (1001) docker     (123)   877297 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/getting_started/edit_npt.png
+-rw-r--r--   0 runner    (1001) docker     (123)   575423 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/getting_started/edit_packmol.png
+-rw-r--r--   0 runner    (1001) docker     (123)   408930 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/getting_started/flowchart.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   220257 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/getting_started/lammps_flowchart.png
+-rw-r--r--   0 runner    (1001) docker     (123)   148973 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/getting_started/nist.png
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:12:51.523282 lammps_step-2023.6.17/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:12:51.539282 lammps_step-2023.6.17/lammps_step/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      492 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-17 02:12:51.539282 lammps_step-2023.6.17/lammps_step/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/custom_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/custom_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:12:51.535282 lammps_step-2023.6.17/lammps_step/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/data/configuration.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/data/properties.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/data/seamm-lammps.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/energy_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/energy_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18551 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/heat_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/heat_flux_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/heat_flux_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22441 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/initialization_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/initialization_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24239 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91984 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/lammps_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/lammps_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11638 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/minimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/minimization_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23933 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/npt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/npt_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/npt_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/nve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/nve_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/nve_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/nvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/nvt_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/nvt_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/tk_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/tk_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/tk_heat_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/tk_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/tk_lammps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/tk_minimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30919 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/tk_npt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/tk_nve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/tk_nvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/tk_velocities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/velocities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/velocities_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/lammps_step/velocities_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:12:51.535282 lammps_step-2023.6.17/lammps_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-06-17 02:12:51.000000 lammps_step-2023.6.17/lammps_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-17 02:12:51.000000 lammps_step-2023.6.17/lammps_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 02:12:51.000000 lammps_step-2023.6.17/lammps_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-17 02:12:51.000000 lammps_step-2023.6.17/lammps_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-17 02:12:51.000000 lammps_step-2023.6.17/lammps_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-17 02:12:51.000000 lammps_step-2023.6.17/lammps_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 02:12:31.000000 lammps_step-2023.6.17/lammps_step.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-17 02:12:51.539282 lammps_step-2023.6.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:12:51.535282 lammps_step-2023.6.17/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:12:51.535282 lammps_step-2023.6.17/tests/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14459 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/tests/data/Ar_xtal_energy.flow
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/tests/test_lammps_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/tests/test_lammps_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-17 02:12:27.000000 lammps_step-2023.6.17/versioneer.py
```

### Comparing `lammps_step-2023.6.16/CONTRIBUTING.rst` & `lammps_step-2023.6.17/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/HISTORY.rst` & `lammps_step-2023.6.17/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 =======
 History
 =======
+2023.6.17 -- Bugfix: more centroid/stress/atom issues
+   * Avoided using centroid/stress/atom for heat flux in standard NVE, NVT, ... dynamics
+     with Class 2 forcefield.
+   * Added option to not use centroid/stress/atom for any forcefield.
 2023.6.16 -- Heat flux with PCFF
    * centroid/stress/atom does not work with Class 2 forcefields, so don't use for PCFF.
 2023.5.29 -- Self diffusion and other improvements
    * Added trajectory panel to support diffusion, viscosity and simple thermal
      conductivity.
    * Added support for separate GPU versions of LAMMPS.
    * Added support for command-line arguments to LAMMPS, mainly used for accelerators.
```

### Comparing `lammps_step-2023.6.16/LICENSE` & `lammps_step-2023.6.17/LICENSE`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/PKG-INFO` & `lammps_step-2023.6.17/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lammps_step
-Version: 2023.6.16
+Version: 2023.6.17
 Summary: A SEAMM plug-in for LAMMPS, a forcefield-based molecular dynamics code.
 Home-page: https://github.com/molssi-seamm/lammps_step
 Author: MolSSI @ Virginia Tech
 Author-email: seamm@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,forcefield,EAM,OpenKIM,molecular dynamics,atomistic,MD
 Platform: Linux
@@ -109,14 +109,18 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2023.6.17 -- Bugfix: more centroid/stress/atom issues
+   * Avoided using centroid/stress/atom for heat flux in standard NVE, NVT, ... dynamics
+     with Class 2 forcefield.
+   * Added option to not use centroid/stress/atom for any forcefield.
 2023.6.16 -- Heat flux with PCFF
    * centroid/stress/atom does not work with Class 2 forcefields, so don't use for PCFF.
 2023.5.29 -- Self diffusion and other improvements
    * Added trajectory panel to support diffusion, viscosity and simple thermal
      conductivity.
    * Added support for separate GPU versions of LAMMPS.
    * Added support for command-line arguments to LAMMPS, mainly used for accelerators.
```

### Comparing `lammps_step-2023.6.16/README.rst` & `lammps_step-2023.6.17/README.rst`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/docs/Makefile` & `lammps_step-2023.6.17/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/docs/_static/SEAMM inverted.png` & `lammps_step-2023.6.17/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/docs/_static/SEAMM logo.png` & `lammps_step-2023.6.17/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/docs/_static/molssi_main_logo.png` & `lammps_step-2023.6.17/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/docs/_static/molssi_main_logo_inverted_white.png` & `lammps_step-2023.6.17/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/docs/_static/molssi_square.png` & `lammps_step-2023.6.17/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/docs/_static/nsf.png` & `lammps_step-2023.6.17/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/docs/conf.py` & `lammps_step-2023.6.17/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/docs/developer_guide/installation.rst` & `lammps_step-2023.6.17/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/docs/getting_started/density.png` & `lammps_step-2023.6.17/docs/getting_started/density.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/docs/getting_started/edit_forcefield.png` & `lammps_step-2023.6.17/docs/getting_started/edit_forcefield.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/docs/getting_started/edit_initialization.png` & `lammps_step-2023.6.17/docs/getting_started/edit_initialization.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/docs/getting_started/edit_npt.png` & `lammps_step-2023.6.17/docs/getting_started/edit_npt.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/docs/getting_started/edit_packmol.png` & `lammps_step-2023.6.17/docs/getting_started/edit_packmol.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/docs/getting_started/flowchart.png` & `lammps_step-2023.6.17/docs/getting_started/flowchart.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/docs/getting_started/index.rst` & `lammps_step-2023.6.17/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/docs/getting_started/lammps_flowchart.png` & `lammps_step-2023.6.17/docs/getting_started/lammps_flowchart.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/docs/getting_started/nist.png` & `lammps_step-2023.6.17/docs/getting_started/nist.png`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/docs/index.rst` & `lammps_step-2023.6.17/docs/index.rst`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/docs/make.bat` & `lammps_step-2023.6.17/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/__init__.py` & `lammps_step-2023.6.17/lammps_step/__init__.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/custom.py` & `lammps_step-2023.6.17/lammps_step/custom.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/custom_parameters.py` & `lammps_step-2023.6.17/lammps_step/custom_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/custom_step.py` & `lammps_step-2023.6.17/lammps_step/custom_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/data/configuration.txt` & `lammps_step-2023.6.17/lammps_step/data/configuration.txt`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/data/properties.csv` & `lammps_step-2023.6.17/lammps_step/data/properties.csv`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/data/references.bib` & `lammps_step-2023.6.17/lammps_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/energy.py` & `lammps_step-2023.6.17/lammps_step/energy.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/energy_parameters.py` & `lammps_step-2023.6.17/lammps_step/energy_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/energy_step.py` & `lammps_step-2023.6.17/lammps_step/energy_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/heat_flux.py` & `lammps_step-2023.6.17/lammps_step/heat_flux.py`

 * *Files 3% similar despite different names*

```diff
@@ -537,40 +537,41 @@
 
 variable            factor delete
 variable            Jx delete
 variable            Jy delete
 variable            Jz delete
 unfix               summary
 unfix               J_filter
-unfix               S_b0
 unfix               S_p0
 unfix               PE0
-unfix               S_b_ave
 unfix               S_p_ave
 unfix               PE_ave
 unfix               dynamics
-uncompute           flux_b
-uncompute           flux_p
-uncompute           S_b
-uncompute           S_p
-uncompute           PE
-uncompute           KE
-
 """
         ]
         for compute in computes:
             post_lines.append(f"uncompute           {compute}")
         for fix in fixes:
             post_lines.append(f"unfix               {fix}")
         for n in range(1, nfixes + 1):
             post_lines.append(f"unfix               {n}")
         for n in range(1, ncomputes + 1):
             post_lines.append(f"uncompute           {n}")
         for n in range(1, ndumps + 1):
             post_lines.append(f"undump              {n}")
+        if P["heat flux"] != "never":
+            if "cff" not in ffname:
+                post_lines.append("uncompute           flux_b")
+                post_lines.append("uncompute           S_b")
+                post_lines.append("unfix               S_b0")
+                post_lines.append("unfix               S_b_ave")
+            post_lines.append("uncompute           flux_p")
+            post_lines.append("uncompute           S_p")
+            post_lines.append("uncompute           PE")
+            post_lines.append("uncompute           KE")
 
         if "cff" in ffname:
             return {
                 "script": lines,
                 "postscript": post_lines,
                 "use python": True,
                 "python script": script2,
```

### Comparing `lammps_step-2023.6.16/lammps_step/heat_flux_parameters.py` & `lammps_step-2023.6.17/lammps_step/heat_flux_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/heat_flux_step.py` & `lammps_step-2023.6.17/lammps_step/heat_flux_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/initialization.py` & `lammps_step-2023.6.17/lammps_step/initialization.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/initialization_parameters.py` & `lammps_step-2023.6.17/lammps_step/initialization_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/initialization_step.py` & `lammps_step-2023.6.17/lammps_step/initialization_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/installer.py` & `lammps_step-2023.6.17/lammps_step/installer.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/lammps.py` & `lammps_step-2023.6.17/lammps_step/lammps.py`

 * *Files 0% similar despite different names*

```diff
@@ -916,15 +916,15 @@
             new_input_data.append("run                 0")
             new_input_data.append(
                 f"write_dump         all custom  {dump} id xu yu zu "
                 "modify flush yes sort id"
             )
             new_input_data.append("")
             new_input_data.append("")
-            new_input_data.append("info               computes fixes dumps log out")
+            new_input_data.append("info               computes fixes dumps out log")
 
         files["input"]["data"] += new_input_data
 
         files["input"]["filename"] = input_file
         files["input"]["data"] = "\n".join(files["input"]["data"])
         self.logger.debug(files["input"]["filename"] + ":\n" + files["input"]["data"])
 
@@ -932,15 +932,15 @@
             postscript.append("reset_timestep      0")
             postscript.append("run                 0")
             postscript.append(
                 f"write_dump          all custom  {dump} id xu yu zu "
                 "modify flush yes sort id"
             )
             postscript.append("")
-            postscript.append("info               computes fixes dumps log out")
+            postscript.append("info               computes fixes dumps out log")
             files["postscript"] = {
                 "data": "\n".join(postscript),
                 "filename": "lammps_post.dat",
             }
         if python_script is not None:
             files["python script"] = {
                 "data": python_script,
```

### Comparing `lammps_step-2023.6.16/lammps_step/lammps_step.py` & `lammps_step-2023.6.17/lammps_step/lammps_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/lammps_units.py` & `lammps_step-2023.6.17/lammps_step/lammps_units.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/metadata.py` & `lammps_step-2023.6.17/lammps_step/metadata.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/minimization.py` & `lammps_step-2023.6.17/lammps_step/minimization.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/minimization_step.py` & `lammps_step-2023.6.17/lammps_step/minimization_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/npt.py` & `lammps_step-2023.6.17/lammps_step/npt.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/npt_parameters.py` & `lammps_step-2023.6.17/lammps_step/npt_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/npt_step.py` & `lammps_step-2023.6.17/lammps_step/npt_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/nve.py` & `lammps_step-2023.6.17/lammps_step/nve.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,21 @@
         )
 
         return self.header + "\n" + __(text, **P, indent=4 * " ").__str__()
 
     def get_input(self, extras=None):
         """Get the input for an NVE dynamics run in LAMMPS"""
 
+        # See what type of forcefield we have and handle it
+        ff = self.get_variable("_forcefield")
+        if ff == "OpenKIM":
+            ffname = ""
+        else:
+            ffname = ff.current_forcefield
+
         self.description = []
         self.description.append(__(self.header, indent=3 * " "))
 
         P = self.parameters.current_values_to_dict(
             context=seamm.flowchart_variables._data
         )
 
@@ -120,16 +127,37 @@
             if lammps_step.get_lammps_unit_system() == "metal":
                 factor = Q_("eV/Å^2/ps")
             else:
                 factor = (
                     Q_("kcal/Å^2/fs/mol") / Q_("kcal/mol") * Q_("kcal/mol").to("kJ")
                 )
             factor = factor.m_as("W/m^2")
-            lines.append(
-                f"""
+            if "cff" in ffname or not P["use centroid stress"]:
+                # Centroid/stress/atom does not handle class2 ff ... cross-terms?
+                lines.append(
+                    f"""
+compute             KE all ke/atom
+compute             PE all pe/atom
+
+#          centroid doesn't work with kspace, so split into pair and non-pair parts
+
+compute             S_p all stress/atom NULL virial
+compute             flux_p all heat/flux KE PE S_p
+
+#          Conversion from kcal/Å^2/fs/mol to W/m^2")
+
+variable            factor equal {factor}
+variable            Jx equal v_factor*c_flux_p[1]/vol
+variable            Jy equal v_factor*c_flux_p[2]/vol
+variable            Jz equal v_factor*c_flux_p[3]/vol
+"""
+                )
+            else:
+                lines.append(
+                    f"""
 compute             KE all ke/atom
 compute             PE all pe/atom
 
 #          centroid doesn't work with kspace, so split into pair and non-pair parts
 
 compute             S_p all stress/atom NULL pair kspace
 compute             S_b all centroid/stress/atom NULL bond angle dihedral improper
@@ -139,15 +167,15 @@
 #          Conversion from kcal/Å^2/fs/mol to W/m^2")
 
 variable            factor equal {factor}
 variable            Jx equal v_factor*(c_flux_p[1]+c_flux_b[1])/vol
 variable            Jy equal v_factor*(c_flux_p[2]+c_flux_b[2])/vol
 variable            Jz equal v_factor*(c_flux_p[3]+c_flux_b[3])/vol
 """
-            )
+                )
 
         # summary output written 10 times during run so we can see progress
         nevery = 10
         nfreq = int(nsteps / 10)
         nrepeat = int(nfreq / nevery)
         nfreq = nevery * nrepeat
         nfixes += 1
@@ -224,14 +252,26 @@
 
         for i in range(1, ncomputes + 1):
             lines.append(f"uncompute           {i}")
         for i in range(1, ndumps + 1):
             lines.append(f"undump              {i}")
         for i in range(1, nfixes + 1):
             lines.append(f"unfix               {i}")
+        if P["heat flux"] != "never":
+            if "cff" not in ffname and P["use centroid stress"]:
+                lines.append("uncompute           flux_b")
+                lines.append("uncompute           S_b")
+            lines.append("uncompute           flux_p")
+            lines.append("uncompute           S_p")
+            lines.append("uncompute           PE")
+            lines.append("uncompute           KE")
+            lines.append("variable            factor delete")
+            lines.append("variable            Jx delete")
+            lines.append("variable            Jy delete")
+            lines.append("variable            Jz delete")
         lines.append("")
 
         return {
             "script": lines,
             "postscript": None,
             "use python": False,
         }
```

### Comparing `lammps_step-2023.6.16/lammps_step/nve_parameters.py` & `lammps_step-2023.6.17/lammps_step/nve_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,23 @@
             "description": "Sample the heat flux:",
             "help_text": (
                 "How often to sample the heat flux, usually used for thermal "
                 "conductivity calculations. However, it is recommended to use the "
                 "heat-flux step instead of using this."
             ),
         },
+        "use centroid stress": {
+            "default": "yes",
+            "kind": "boolean",
+            "default_units": None,
+            "enumeration": ("yes", "no"),
+            "format_string": "",
+            "description": "Use centroid/stress/atom:",
+            "help_text": "Whether to use centroid/stress/atom",
+        },
         "shear stress": {
             "default": "never",
             "kind": "float",
             "default_units": "fs",
             "enumeration": ("never",),
             "format_string": ".1f",
             "description": "Sample the shear stress:",
```

### Comparing `lammps_step-2023.6.16/lammps_step/nve_step.py` & `lammps_step-2023.6.17/lammps_step/nve_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/nvt.py` & `lammps_step-2023.6.17/lammps_step/nvt.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/nvt_parameters.py` & `lammps_step-2023.6.17/lammps_step/nvt_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/nvt_step.py` & `lammps_step-2023.6.17/lammps_step/nvt_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/tk_custom.py` & `lammps_step-2023.6.17/lammps_step/tk_custom.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/tk_energy.py` & `lammps_step-2023.6.17/lammps_step/tk_energy.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/tk_heat_flux.py` & `lammps_step-2023.6.17/lammps_step/tk_heat_flux.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
         frame = super().create_dialog(title="Heat Flux")
 
         # Shortcut for parameters
         P = self.node.parameters
 
         # Then create the widgets
-        for key in ("time", "timestep", "heat flux", "sampling"):
+        for key in ("time", "timestep", "heat flux", "use centroid stress", "sampling"):
             self[key] = P[key].widget(frame)
 
         # and lay them out
         self.reset_dialog()
 
     def reset_dialog(self, widget=None):
         """Layout the widgets in the dialog.
@@ -151,15 +151,15 @@
         # Shortcut for parameters
         P = self.node.parameters
 
         # keep track of the row in a variable, so that the layout is flexible
         # if e.g. rows are skipped to control such as "method" here
         row = 0
         widgets = []
-        for key in ("time", "timestep", "heat flux", "sampling"):
+        for key in ("time", "timestep", "heat flux", "use centroid stress", "sampling"):
             self[key].grid(row=row, column=0, sticky=tk.EW)
             widgets.append(self[key])
             row += 1
 
         # Align the labels
         sw.align_labels(widgets, sticky=tk.E)
```

### Comparing `lammps_step-2023.6.16/lammps_step/tk_initialization.py` & `lammps_step-2023.6.17/lammps_step/tk_initialization.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/tk_lammps.py` & `lammps_step-2023.6.17/lammps_step/tk_lammps.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/tk_minimization.py` & `lammps_step-2023.6.17/lammps_step/tk_minimization.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/tk_npt.py` & `lammps_step-2023.6.17/lammps_step/tk_npt.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/tk_nve.py` & `lammps_step-2023.6.17/lammps_step/tk_nve.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         notebook.insert(
             self["results frame"], tframe, text="Trajectories", sticky=tk.NSEW
         )
 
         row = 0
         widgets = []
         for key in lammps_step.NVE_Parameters.trajectories:
-            if title == "Heat Flux" and key == "heat flux":
+            if title == "Heat Flux" and (key == "heat flux" or "centroid" in key):
                 continue
             self[key] = P[key].widget(tframe)
             self[key].grid(row=row, column=0)
             row += 1
             widgets.append(self[key])
         sw.align_labels(widgets, sticky=tk.E)
```

### Comparing `lammps_step-2023.6.16/lammps_step/tk_nvt.py` & `lammps_step-2023.6.17/lammps_step/tk_nvt.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/tk_velocities.py` & `lammps_step-2023.6.17/lammps_step/tk_velocities.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/velocities.py` & `lammps_step-2023.6.17/lammps_step/velocities.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/velocities_parameters.py` & `lammps_step-2023.6.17/lammps_step/velocities_parameters.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step/velocities_step.py` & `lammps_step-2023.6.17/lammps_step/velocities_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step.egg-info/PKG-INFO` & `lammps_step-2023.6.17/lammps_step.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lammps-step
-Version: 2023.6.16
+Version: 2023.6.17
 Summary: A SEAMM plug-in for LAMMPS, a forcefield-based molecular dynamics code.
 Home-page: https://github.com/molssi-seamm/lammps_step
 Author: MolSSI @ Virginia Tech
 Author-email: seamm@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,forcefield,EAM,OpenKIM,molecular dynamics,atomistic,MD
 Platform: Linux
@@ -109,14 +109,18 @@
 .. _MolSSI: https://www.molssi.org
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
+2023.6.17 -- Bugfix: more centroid/stress/atom issues
+   * Avoided using centroid/stress/atom for heat flux in standard NVE, NVT, ... dynamics
+     with Class 2 forcefield.
+   * Added option to not use centroid/stress/atom for any forcefield.
 2023.6.16 -- Heat flux with PCFF
    * centroid/stress/atom does not work with Class 2 forcefields, so don't use for PCFF.
 2023.5.29 -- Self diffusion and other improvements
    * Added trajectory panel to support diffusion, viscosity and simple thermal
      conductivity.
    * Added support for separate GPU versions of LAMMPS.
    * Added support for command-line arguments to LAMMPS, mainly used for accelerators.
```

### Comparing `lammps_step-2023.6.16/lammps_step.egg-info/SOURCES.txt` & `lammps_step-2023.6.17/lammps_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/lammps_step.egg-info/entry_points.txt` & `lammps_step-2023.6.17/lammps_step.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/setup.py` & `lammps_step-2023.6.17/setup.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/tests/data/Ar_xtal_energy.flow` & `lammps_step-2023.6.17/tests/data/Ar_xtal_energy.flow`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/tests/test_lammps_step.py` & `lammps_step-2023.6.17/tests/test_lammps_step.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/tests/test_lammps_units.py` & `lammps_step-2023.6.17/tests/test_lammps_units.py`

 * *Files identical despite different names*

### Comparing `lammps_step-2023.6.16/versioneer.py` & `lammps_step-2023.6.17/versioneer.py`

 * *Files identical despite different names*

