# Comparing `tmp/rocketsolver-0.3.0.tar.gz` & `tmp/rocketsolver-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocketsolver-0.3.0.tar", last modified: Fri Sep 23 16:20:52 2022, max compression
+gzip compressed data, was "rocketsolver-0.5.0.tar", last modified: Sat Jun 17 20:21:53 2023, max compression
```

## Comparing `rocketsolver-0.3.0.tar` & `rocketsolver-0.5.0.tar`

### file list

```diff
@@ -1,95 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.445993 rocketsolver-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)    41887 2022-09-23 16:20:52.445993 rocketsolver-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.441993 rocketsolver-0.3.0/rocketsolver/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.441993 rocketsolver-0.3.0/rocketsolver/analytics/
--rw-r--r--   0 runner    (1001) docker     (121)      811 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/analytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.441993 rocketsolver-0.3.0/rocketsolver/analytics/srm/
--rw-r--r--   0 runner    (1001) docker     (121)    10172 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/analytics/srm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.441993 rocketsolver-0.3.0/rocketsolver/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.441993 rocketsolver-0.3.0/rocketsolver/models/atmosphere/
--rw-r--r--   0 runner    (1001) docker     (121)     1982 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/atmosphere/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.441993 rocketsolver-0.3.0/rocketsolver/models/fuselage/
--rw-r--r--   0 runner    (1001) docker     (121)     3472 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/fuselage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.441993 rocketsolver-0.3.0/rocketsolver/models/fuselage/components/
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/fuselage/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.441993 rocketsolver-0.3.0/rocketsolver/models/fuselage/components/body/
--rw-r--r--   0 runner    (1001) docker     (121)     2753 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/fuselage/components/body/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.441993 rocketsolver-0.3.0/rocketsolver/models/fuselage/components/fins/
--rw-r--r--   0 runner    (1001) docker     (121)      863 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/fuselage/components/fins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2169 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/fuselage/components/fins/trapezoidal.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.441993 rocketsolver-0.3.0/rocketsolver/models/fuselage/components/nosecones/
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/fuselage/components/nosecones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2365 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/fuselage/components/nosecones/haack.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.441993 rocketsolver-0.3.0/rocketsolver/models/materials/
--rw-r--r--   0 runner    (1001) docker     (121)     1198 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/materials/composites.py
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/materials/elastics.py
--rw-r--r--   0 runner    (1001) docker     (121)     1413 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/materials/metals.py
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/materials/plastics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.441993 rocketsolver-0.3.0/rocketsolver/models/propellants/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/propellants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2958 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/propellants/solid.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.441993 rocketsolver-0.3.0/rocketsolver/models/propulsion/
--rw-r--r--   0 runner    (1001) docker     (121)    11061 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/propulsion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.445993 rocketsolver-0.3.0/rocketsolver/models/propulsion/grain/
--rw-r--r--   0 runner    (1001) docker     (121)     3877 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/propulsion/grain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3529 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/propulsion/grain/bates.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.445993 rocketsolver-0.3.0/rocketsolver/models/propulsion/propellant/
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/propulsion/propellant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3148 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/propulsion/propellant/solid.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.445993 rocketsolver-0.3.0/rocketsolver/models/propulsion/structure/
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/propulsion/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7840 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/propulsion/structure/chamber.py
--rw-r--r--   0 runner    (1001) docker     (121)     2361 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/propulsion/structure/nozzle.py
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/propulsion/thermals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.445993 rocketsolver-0.3.0/rocketsolver/models/recovery/
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/recovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2058 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/recovery/events.py
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/recovery/parachutes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.445993 rocketsolver-0.3.0/rocketsolver/models/rocket/
--rw-r--r--   0 runner    (1001) docker     (121)     2052 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/models/rocket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.445993 rocketsolver-0.3.0/rocketsolver/montecarlo/
--rw-r--r--   0 runner    (1001) docker     (121)     7937 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/montecarlo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3140 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/montecarlo/random.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.445993 rocketsolver-0.3.0/rocketsolver/operations/
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/operations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.445993 rocketsolver-0.3.0/rocketsolver/operations/ballistics/
--rw-r--r--   0 runner    (1001) docker     (121)     6024 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/operations/ballistics/_1dof.py
--rw-r--r--   0 runner    (1001) docker     (121)    15714 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/operations/ballistics/_6dof.py
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/operations/ballistics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.445993 rocketsolver-0.3.0/rocketsolver/operations/internal_ballistics/
--rw-r--r--   0 runner    (1001) docker     (121)    12766 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/operations/internal_ballistics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.445993 rocketsolver-0.3.0/rocketsolver/simulations/
--rw-r--r--   0 runner    (1001) docker     (121)     2171 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/simulations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3640 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/simulations/ballistics.py
--rw-r--r--   0 runner    (1001) docker     (121)     4023 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/simulations/ballistics_6dof.py
--rw-r--r--   0 runner    (1001) docker     (121)     4597 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/simulations/internal_balistics_coupled.py
--rw-r--r--   0 runner    (1001) docker     (121)     2403 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/simulations/internal_ballistics.py
--rw-r--r--   0 runner    (1001) docker     (121)     4171 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/simulations/structural.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.445993 rocketsolver-0.3.0/rocketsolver/solvers/
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1537 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/solvers/ballistics_1d.py
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/solvers/ballistics_6d.py
--rw-r--r--   0 runner    (1001) docker     (121)     2639 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/solvers/srm_internal_ballistics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.445993 rocketsolver-0.3.0/rocketsolver/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/utils/classes.py
--rw-r--r--   0 runner    (1001) docker     (121)      765 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/utils/geometric.py
--rw-r--r--   0 runner    (1001) docker     (121)     8476 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/utils/isentropic_flow.py
--rw-r--r--   0 runner    (1001) docker     (121)     1420 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (121)     2990 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/utils/odes.py
--rw-r--r--   0 runner    (1001) docker     (121)     8847 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/utils/plots.py
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/utils/strings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/utils/units.py
--rw-r--r--   0 runner    (1001) docker     (121)     4364 2022-09-23 16:20:40.000000 rocketsolver-0.3.0/rocketsolver/utils/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 16:20:52.441993 rocketsolver-0.3.0/rocketsolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    41887 2022-09-23 16:20:52.000000 rocketsolver-0.3.0/rocketsolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2683 2022-09-23 16:20:52.000000 rocketsolver-0.3.0/rocketsolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-23 16:20:52.000000 rocketsolver-0.3.0/rocketsolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-09-23 16:20:52.000000 rocketsolver-0.3.0/rocketsolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-09-23 16:20:52.000000 rocketsolver-0.3.0/rocketsolver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-23 16:20:52.445993 rocketsolver-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:21:53.591512 rocketsolver-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    41802 2023-06-17 20:21:53.591512 rocketsolver-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34502 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:21:53.583512 rocketsolver-0.5.0/rocketsolver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:21:53.583512 rocketsolver-0.5.0/rocketsolver/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:21:53.583512 rocketsolver-0.5.0/rocketsolver/models/atmosphere/
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/atmosphere/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:21:53.583512 rocketsolver-0.5.0/rocketsolver/models/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/materials/composites.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/materials/elastics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/materials/metals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/materials/plastics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:21:53.583512 rocketsolver-0.5.0/rocketsolver/models/propulsion/
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/propulsion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:21:53.583512 rocketsolver-0.5.0/rocketsolver/models/propulsion/grain/
+-rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/propulsion/grain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:21:53.587512 rocketsolver-0.5.0/rocketsolver/models/propulsion/grain/fmm/
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/propulsion/grain/fmm/_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/propulsion/grain/fmm/_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/propulsion/grain/fmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/propulsion/grain/fmm/stl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:21:53.587512 rocketsolver-0.5.0/rocketsolver/models/propulsion/grain/geometries/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/propulsion/grain/geometries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/propulsion/grain/geometries/bates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/propulsion/grain/geometries/conical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/propulsion/grain/geometries/d_grain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/propulsion/grain/geometries/multi_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/propulsion/grain/geometries/rod_and_tube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/propulsion/grain/geometries/star.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/propulsion/grain/geometries/wagon_wheel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:21:53.587512 rocketsolver-0.5.0/rocketsolver/models/propulsion/propellants/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/propulsion/propellants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/propulsion/propellants/solid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:21:53.587512 rocketsolver-0.5.0/rocketsolver/models/propulsion/structure/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/propulsion/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/propulsion/structure/chamber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/propulsion/structure/nozzle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/propulsion/thermals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:21:53.587512 rocketsolver-0.5.0/rocketsolver/models/recovery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/recovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/recovery/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/recovery/parachutes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:21:53.587512 rocketsolver-0.5.0/rocketsolver/models/rocket/
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/rocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/models/rocket/fuselage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:21:53.587512 rocketsolver-0.5.0/rocketsolver/montecarlo/
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/montecarlo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/montecarlo/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:21:53.587512 rocketsolver-0.5.0/rocketsolver/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/operations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:21:53.587512 rocketsolver-0.5.0/rocketsolver/operations/ballistics/
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/operations/ballistics/_1dof.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/operations/ballistics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:21:53.587512 rocketsolver-0.5.0/rocketsolver/operations/internal_ballistics/
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/operations/internal_ballistics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:21:53.587512 rocketsolver-0.5.0/rocketsolver/services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:21:53.587512 rocketsolver-0.5.0/rocketsolver/services/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/services/common/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/services/common/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/services/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/services/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/services/equations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/services/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/services/isentropic_flow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:21:53.591512 rocketsolver-0.5.0/rocketsolver/services/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/services/math/geometric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:21:53.591512 rocketsolver-0.5.0/rocketsolver/simulations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/simulations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/simulations/ballistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/simulations/internal_balistics_coupled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/simulations/internal_ballistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:21:53.591512 rocketsolver-0.5.0/rocketsolver/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-17 20:21:43.000000 rocketsolver-0.5.0/rocketsolver/solvers/odes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:21:53.583512 rocketsolver-0.5.0/rocketsolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41802 2023-06-17 20:21:53.000000 rocketsolver-0.5.0/rocketsolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-17 20:21:53.000000 rocketsolver-0.5.0/rocketsolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 20:21:53.000000 rocketsolver-0.5.0/rocketsolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-17 20:21:53.000000 rocketsolver-0.5.0/rocketsolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-17 20:21:53.000000 rocketsolver-0.5.0/rocketsolver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 20:21:53.591512 rocketsolver-0.5.0/setup.cfg
```

### Comparing `rocketsolver-0.3.0/PKG-INFO` & `rocketsolver-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocketsolver
-Version: 0.3.0
+Version: 0.5.0
 Summary: Rocket simulator
 Author-email: Felipe Bogaerts de Mattos <me@felipebm.com>
 License: GNU GENERAL PUBLIC LICENSE
            Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
         Everyone is permitted to copy and distribute verbatim copies
@@ -728,11 +728,7 @@
 ## a015140
 
 Correction factors.
 
 ## Hans Seidel's Chamber Pressure article
 
 Chamber Pressure equation.
-
-## 6DOF Trajectory Simulator
-
-http://pee.ufrj.br/teses/textocompleto/2007062901.pdf
```

### Comparing `rocketsolver-0.3.0/README.md` & `rocketsolver-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -38,11 +38,7 @@
 ## a015140
 
 Correction factors.
 
 ## Hans Seidel's Chamber Pressure article
 
 Chamber Pressure equation.
-
-## 6DOF Trajectory Simulator
-
-http://pee.ufrj.br/teses/textocompleto/2007062901.pdf
```

### Comparing `rocketsolver-0.3.0/pyproject.toml` & `rocketsolver-0.5.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rocketsolver"
-version = "0.3.0"
+version = "0.5.0"
 description = "Rocket simulator"
 readme = "README.md"
 authors = [{ name = "Felipe Bogaerts de Mattos", email = "me@felipebm.com" }]
 license = { file = "license.txt" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: Unix",
@@ -32,16 +32,16 @@
 [project.optional-dependencies]
 dev = ["black", "pytest", "bumpver"]
 
 [project.urls]
 Homepage = "https://github.com/felipebogaertsm/rocket-solver"
 
 [tool.bumpver]
-current_version = "0.3.0"
+current_version = "0.5.0"
 version_pattern = "MAJOR.MINOR.PATCH"
-commit_message  = "Testing CI"
+commit_message  = "Refactored many modules of the library"
 commit          = true
 tag             = true
 push            = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
```

### Comparing `rocketsolver-0.3.0/rocketsolver/models/fuselage/components/body/__init__.py` & `rocketsolver-0.5.0/rocketsolver/models/propulsion/grain/geometries/bates.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,102 +1,69 @@
-# -*- coding: utf-8 -*-
-# Author: Felipe Bogaerts de Mattos
-# Contact me at felipe.bogaerts@engenharia.ufjf.br.
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, version 3.
-
-from typing import Optional
-
 import numpy as np
 
-from ..fins import Fins
-from rocketsolver.models.materials import Material
-from rocketsolver.models.fuselage.components import FuselageComponent
-
+from rocketsolver.services.math.geometric import (
+    get_circle_area,
+    get_cylinder_surface_area,
+)
 
-class BodySegment(FuselageComponent):
-    pass
+from .. import GrainSegment2D, GrainGeometryError
+from rocketsolver.services.decorators import validate_assertions
 
 
-class CylindricalBody(BodySegment):
+class BatesSegment(GrainSegment2D):
     def __init__(
         self,
-        material: Material,
-        center_of_gravity: float,
-        mass: float,
-        length: float,
         outer_diameter: float,
-        rugosity: float,
-        constant_K: float,
-        fins: Optional[Fins] = None,
+        core_diameter: float,
+        length: float,
+        spacing: float,
     ) -> None:
-        self.length = length
-        self.outer_diameter = outer_diameter
-        self.rugosity = rugosity
-        self.constant_K = constant_K
-        self.fins = fins
+        self.core_diameter = core_diameter
 
         super().__init__(
-            material=material, center_of_gravity=center_of_gravity, mass=mass
+            length=length,
+            outer_diameter=outer_diameter,
+            spacing=spacing,
+            inhibited_ends=0,
         )
 
-    @property
-    def frontal_area(self) -> float:
-        return np.pi * self.outer_diameter**2 / 4
-
-    @property
-    def outer_surface_area(self) -> float:
-        return self.length * np.pi * (self.outer_diameter)
-
-    @property
-    def is_valid(self) -> None:
-        assert self.rugosity < 1e-3
-        assert self.frontal_area > 0
-        assert self.outer_surface_area > 0
-
-    def get_cd_body(
-        self, total_vehicle_length: float, nose_cone_length: float
-    ) -> float:
-        """
-        Not tested.
-        """
-        return (
-            1
-            + 60 / ((total_vehicle_length / self.outer_diameter) ** 3)
-            + 0.0025
-            * (self.length / self.outer_diameter)
-            * (
-                2.7 * (nose_cone_length / self.outer_diameter)
-                + 4 * (self.length / self.outer_diameter)
-            )
+    @validate_assertions(exception=GrainGeometryError)
+    def validate(self) -> None:
+        super().validate()
+
+        assert self.outer_diameter > self.core_diameter
+        assert self.core_diameter > 0
+
+    def get_core_diameter(self, web_distance: float) -> float:
+        return self.core_diameter + 2 * web_distance
+
+    def get_port_area(self, web_distance: float) -> float:
+        return get_circle_area(diameter=self.get_core_diameter(web_distance))
+
+    def get_core_area(self, web_distance: float) -> float:
+        length = self.get_length(web_distance=web_distance)
+        core_diameter = self.core_diameter + 2 * web_distance
+        return get_cylinder_surface_area(length, core_diameter)
+
+    def get_face_area(self, web_distance: float) -> float:
+        core_diameter = self.get_core_diameter(web_distance)
+        return np.pi * (
+            ((self.outer_diameter ** 2) - (core_diameter) ** 2) / 4
         )
 
-    def get_cd_base(self) -> float:
+    def get_web_thickness(self) -> float:
         """
-        Not tested.
+        More details on the web thickness of BATES grains can be found in:
+        https://www.nakka-rocketry.net/design1.html
         """
-        return 0.029 / np.sqrt(
-            self.get_cd_body(total_vehicle_length=0, nose_cone_length=0)
-        )
+        return 0.5 * (self.outer_diameter - self.core_diameter)
 
-    def get_drag_coefficient(
-        self,
-        total_vehicle_length: float,
-        nose_cone_length: float,
-    ) -> float:
+    def get_optimal_length(self) -> float:
         """
-        Not tested.
-        """
-        return (
-            self.get_cd_body(
-                total_vehicle_length=total_vehicle_length,
-                nose_cone_length=nose_cone_length,
-            )
-            + self.get_cd_base()
-        )
+        Returns the optimal length for BATES segment.
+        More details on the calculation:
+        https://www.nakka-rocketry.net/th_grain.html
 
-    def get_lift_coefficient(self) -> float:
-        """
-        Not tested.
+        :return: Optimal length for neutral burn of BATES segment
+        :rtype: float
         """
-        return self.constant_K * self.outer_surface_area / self.frontal_area
+        return 1e3 * 0.5 * (3 * self.outer_diameter + self.core_diameter)
```

### Comparing `rocketsolver-0.3.0/rocketsolver/models/fuselage/components/nosecones/haack.py` & `rocketsolver-0.5.0/rocketsolver/models/propulsion/grain/fmm/stl.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,86 +1,71 @@
-# -*- coding: utf-8 -*-
-# Author: Felipe Bogaerts de Mattos
-# Contact me at felipe.bogaerts@engenharia.ufjf.br.
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, version 3.
+from abc import ABC
+from typing import Optional
 
 import numpy as np
+import trimesh
+from trimesh import load_mesh
+from trimesh.voxel import creation
 
-from . import NoseCone
-from rocketsolver.models.materials import Material
+from ._3d import FMMGrainSegment3D
+from .. import GrainGeometryError
+from rocketsolver.services.decorators import validate_assertions
 
 
-class HaackSeriesNoseCone(NoseCone):
+class FMMSTLGrainSegment(FMMGrainSegment3D, ABC):
     """
-    Reference:
-    THE DESCRIPTIVE GEOMETRY OF NOSE CONES, Gary Crowell, 1996
-    http://servidor.demec.ufpr.br/CFD/bibliografia/aerodinamica/Crowell_1996.pdf
-    Accessed September 17, 2022 at 2:01 pm EST.
+    Fast Marching Method (FMM) implementation for a grain segment obtained
+    from an STL file.
     """
 
     def __init__(
         self,
-        material: Material,
-        center_of_gravity: float,
-        mass: float,
+        file_path: str,
+        outer_diameter: float,
         length: float,
-        base_diameter: float,
-        C: float,
+        spacing: float,
+        inhibited_ends: Optional[int] = 0,
+        map_dim: Optional[int] = 50,
     ) -> None:
-        self.C = C
+
+        self.file_path = file_path
+        self.outer_diameter = outer_diameter
+        self.length = length
+
+        # "Cache" variables:
+        self.face_area_interp_func = None
 
         super().__init__(
-            material=material,
-            center_of_gravity=center_of_gravity,
-            mass=mass,
             length=length,
-            base_diameter=base_diameter,
-            surface_area=None,
+            outer_diameter=outer_diameter,
+            spacing=spacing,
+            inhibited_ends=inhibited_ends,
+            map_dim=map_dim,
         )
 
-    def get_theta(self, x: float) -> float:
-        """
-        Theta is used to calculate the Von Karman profile along the main nose
-        cone axis.
-        """
-        return np.arccos(1 - 2 * x / self.length)
+    @validate_assertions(exception=GrainGeometryError)
+    def validate(self) -> None:
+        assert self.map_dim >= 20
 
-    def get_y_from_x(self, x: float) -> float:
-        """
-        Calculates the y coordinate of the Von Karman profile along the x
-        axis.
+    def get_voxel_size(self) -> float:
         """
-        theta = self.get_theta(x)
+        NOTE: Only returns correct voxel size if map_dim is an odd number.
 
-        return (
-            self.base_diameter
-            / np.sqrt(np.pi)
-            * np.sqrt(
-                theta - np.sin(2 * theta) / 2 + self.C * (np.sin(theta) ** 3)
-            )
-        )
-
-    @property
-    def is_valid(self) -> None:
-        assert self.C <= 4 / 3
-
-    @property
-    def surface_area(self) -> float:
-        """
-        Calculates the surface area of the Haack Series nose cone.
+        :return: the voxel edge size.
+        :rtype: float
         """
-        iterations = 1000
-        area = 0  # initial value, to be incremented
+        return self.outer_diameter / int(self.map_dim - 1)
 
-        for x in np.linspace(0, self.length, iterations):
-            y = self.get_y_from_x(x)
-            area += 2 * np.pi * y * self.length / iterations
+    def get_initial_face_map(self) -> tuple[np.ndarray, np.ndarray]:
+        """
+        Generate a map by voxelizing an STL file. Uses trimesh library.
 
-        return area
+        NOTE: Still needs to convert boolean matrix to masked array.
+        """
+        mesh = load_mesh(self.file_path)
+        assert mesh.is_watertight
 
-    def get_drag_coefficient(self, *args, **kwargs) -> float:
-        return 0
+        volume = mesh.voxelized(pitch=self.get_voxel_size()).fill()
+        map = volume.matrix.view(np.ndarray).transpose() * 1
 
-    def get_lift_coefficient(self, *args, **kwargs) -> float:
-        return 2
+        assert map.shape == self.get_maps()[0].shape
+        return map
```

### Comparing `rocketsolver-0.3.0/rocketsolver/models/materials/metals.py` & `rocketsolver-0.5.0/rocketsolver/models/materials/plastics.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,35 @@
-# -*- coding: utf-8 -*-
-# Author: Felipe Bogaerts de Mattos
-# Contact me at felipe.bogaerts@engenharia.ufjf.br.
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, version 3.
+from . import Material
 
-from . import NozzleMaterial
 
-
-class Steel(NozzleMaterial):
-    """
-    Data obtained from:
-    https://www.thyssenkrupp-materials.co.uk/stainless-steel-304-14301.html
+class EpoxiResin(Material):
     """
+    EpoxiResin material class derived from the Material base class.
 
-    def __init__(self) -> None:
-        super().__init__(
-            density=8000,
-            yield_strength=210e6,
-            ultimate_strength=520e6,
-            C1=0.00506,
-            C2=0.0,
-        )
+    This class represents a specific type of material, EpoxiResin, which
+    inherits properties from the Material base class. It provides default
+    values for the density, yield strength, and ultimate strength specific to
+    EpoxiResin.
 
+    Inherits:
+        Material: Base class representing a generic material.
 
-class Al6063T5(NozzleMaterial):
-    """
-    Data obtained from:
-    https://www.makeitfrom.com/material-properties/6063-T5-Aluminum
+    Attributes:
+        None
     """
 
     def __init__(self) -> None:
-        super().__init__(
-            density=2700,
-            yield_strength=170e6,
-            ultimate_strength=180e6,
-            C1=0.00506,
-            C2=0.0,
-        )
+        """
+        Initialize an EpoxiResin object.
 
+        This constructor sets the default values for the density, yield
+        strength, and ultimate strength of EpoxiResin.
 
-class Al6061T6(NozzleMaterial):
-    """
-    Data obtained from:
-    https://matweb.com/search/DataSheet.aspx?MatGUID=b8d536e0b9b54bd7b69e4124d8f1d20a&ckck=1
-    """
+        Args:
+            None
 
-    def __init__(self) -> None:
+        Returns:
+            None
+        """
         super().__init__(
-            density=2700,
-            yield_strength=262e6,
-            ultimate_strength=290e6,
-            C1=0.00506,
-            C2=0.0,
+            density=1100, yield_strength=60e6, ultimate_strength=60e6
         )
```

### Comparing `rocketsolver-0.3.0/rocketsolver/models/propulsion/structure/chamber.py` & `rocketsolver-0.5.0/rocketsolver/models/propulsion/structure/chamber.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,16 @@
-# -*- coding: utf-8 -*-
-# Author: Felipe Bogaerts de Mattos
-# Contact me at felipe.bogaerts@engenharia.ufjf.br.
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, version 3.
-
 """
 Stores MotorStructure class and methods.
 """
 
 import numpy as np
 
 from rocketsolver.models.materials import Material
 from rocketsolver.models.propulsion.thermals import ThermalLiner
-from rocketsolver.utils.geometric import get_cylinder_volume
+from rocketsolver.services.math.geometric import get_cylinder_volume
 
 
 class CombustionChamber:
     def __init__(
         self,
         casing_inner_diameter: float,
         outer_diameter: float,
@@ -45,61 +38,66 @@
     def outer_radius(self) -> float:
         return self.outer_diameter / 2
 
     @property
     def casing_inner_radius(self) -> float:
         return self.casing_inner_diameter / 2
 
+    @property
+    def chamber_length(
+        self,
+        grain_length: float,
+        grain_count: int,
+        grain_spacing: float,
+    ) -> float:
+        """
+        Returns the chamber length of the SRM, given the grain parameters.
+        """
+        return np.sum(grain_length) + (grain_count - 1) * grain_spacing
+
+    @property
+    def empty_volume(self) -> None:
+        return get_cylinder_volume(self.inner_diameter, self.length)
+
     def get_bulkhead_thickness(
         self, chamber_pressure: np.ndarray, safety_factor: float
     ) -> float:
         """
         Returns the thickness of a planar bulkhead pressure vessel.
         """
         return self.inner_diameter * (
             np.sqrt(
                 (0.75 * chamber_pressure)
                 / (self.bulkhead_material.yield_strength / safety_factor)
             )
         )
 
-    def get_chamber_length(
-        self,
-        grain_length: float,
-        grain_count: int,
-        grain_spacing: float,
-    ) -> float:
-        """
-        Returns the chamber length of the SRM, given the grain parameters.
-        """
-        return np.sum(grain_length) + (grain_count - 1) * grain_spacing
-
     def get_casing_stress_theta(self, chamber_pressure: float) -> float:
         return (
-            (chamber_pressure * self.casing_inner_radius**2)
-            / (self.outer_radius**2 - self.casing_inner_radius**2)
+            (chamber_pressure * self.casing_inner_radius ** 2)
+            / (self.outer_radius ** 2 - self.casing_inner_radius ** 2)
             * (
                 1
-                + ((self.outer_radius**2) / (self.casing_inner_radius**2))
+                + ((self.outer_radius ** 2) / (self.casing_inner_radius ** 2))
             )
         )
 
     def get_casing_stress_radius(self, chamber_pressure: float) -> float:
         return (
-            (chamber_pressure * self.casing_inner_radius**2)
-            / (self.outer_radius**2 - self.casing_inner_radius**2)
+            (chamber_pressure * self.casing_inner_radius ** 2)
+            / (self.outer_radius ** 2 - self.casing_inner_radius ** 2)
             * (1 - ((self.outer_radius) / (self.casing_inner_radius)) ** 2)
         )
 
     def get_casing_stress_z(self, chamber_pressure: float) -> float:
         return (
             2
             * chamber_pressure
-            * self.casing_inner_radius**2
-            / (self.outer_radius**2 - self.casing_inner_radius**2)
+            * self.casing_inner_radius ** 2
+            / (self.outer_radius ** 2 - self.casing_inner_radius ** 2)
         )
 
     def get_casing_safety_factor(self, chamber_pressure: np.ndarray) -> float:
         """
         Returns the thickness for a cylindrical pressure vessel, using
         Von Misses criteria.
         """
@@ -115,17 +113,14 @@
                 (gama_z - gama_r) ** 2
                 + (gama_r - gama_theta) ** 2
                 + (gama_theta - gama_z) ** 2
             )
             / 2
         )
 
-    def get_empty_volume(self) -> None:
-        return get_cylinder_volume(self.inner_diameter, self.length)
-
 
 class BoltedCombustionChamber(CombustionChamber):
     def __init__(
         self,
         casing_inner_diameter: float,
         outer_diameter: float,
         liner: ThermalLiner,
@@ -147,33 +142,33 @@
         )
         self.screw_material = screw_material
         self.max_screw_count = max_screw_count
         self.screw_clearance_diameter = screw_clearance_diameter
         self.screw_diameter = screw_diameter
 
     def get_shear_area(self) -> float:
-        return (self.screw_diameter**2) * np.pi * 0.25
+        return (self.screw_diameter ** 2) * np.pi * 0.25
 
     def get_tear_area(self, screw_count: int) -> float:
         """
         Calculates tear area for screw section.
         """
         return (
             (
                 np.pi
                 * 0.25
-                * ((self.outer_diameter**2) - (self.inner_diameter**2))
+                * ((self.outer_diameter ** 2) - (self.inner_diameter ** 2))
             )
             / screw_count
         ) - (
             np.arcsin(
                 (self.screw_clearance_diameter / 2) / (self.inner_diameter / 2)
             )
         ) * 0.25 * (
-            (self.outer_diameter**2) - (self.inner_diameter**2)
+            (self.outer_diameter ** 2) - (self.inner_diameter ** 2)
         )
 
     def get_compression_area(self) -> float:
         return (
             ((self.outer_diameter - self.inner_diameter))
             * self.screw_clearance_diameter
             / 2
```

### Comparing `rocketsolver-0.3.0/rocketsolver/models/propulsion/structure/nozzle.py` & `rocketsolver-0.5.0/rocketsolver/models/propulsion/structure/nozzle.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,18 @@
-# -*- coding: utf-8 -*-
-# Author: Felipe Bogaerts de Mattos
-# Contact me at felipe.bogaerts@engenharia.ufjf.br.
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, version 3.
-
 """
 Stores MotorStructure class and methods.
 """
 
 import numpy as np
 
 from .chamber import CombustionChamber
-from rocketsolver.utils.geometric import get_circle_area
-from rocketsolver.utils.isentropic_flow import get_divergent_correction_factor
+from rocketsolver.services.math.geometric import get_circle_area
+from rocketsolver.services.isentropic_flow import (
+    get_divergent_correction_factor,
+)
 
 
 class Nozzle:
     def __init__(
         self,
         throat_diameter,
         divergent_angle,
```

### Comparing `rocketsolver-0.3.0/rocketsolver/models/rocket/__init__.py` & `rocketsolver-0.5.0/rocketsolver/models/rocket/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,74 +1,91 @@
-# -*- coding: utf-8 -*-
-# Author: Felipe Bogaerts de Mattos
-# Contact me at felipe.bogaerts@engenharia.ufjf.br.
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, version 3.
-
 from abc import ABC, abstractmethod
-
-from rocketsolver.models.fuselage import Fuselage, Fuselage3D
+from rocketsolver.models.rocket.fuselage import Fuselage
 from rocketsolver.models.propulsion import Motor
 from rocketsolver.models.recovery import Recovery
 
 
 class RocketBaseClass(ABC):
     """
     Base class for a Rocket.
     """
 
     def __init__(
         self,
         propulsion: Motor,
         recovery: Recovery,
-        fuselage: Fuselage | Fuselage3D,
+        fuselage: Fuselage,
     ) -> None:
+        """
+        Initializes a RocketBaseClass object.
+
+        Args:
+            propulsion (Motor): The motor or propulsion system of the rocket.
+            recovery (Recovery): The recovery system of the rocket.
+            fuselage (Fuselage): The fuselage or body of the rocket.
+        """
         self.propulsion = propulsion
         self.recovery = recovery
         self.fuselage = fuselage
 
     @abstractmethod
     def get_launch_mass(self) -> float:
+        """
+        Calculates the total mass of the rocket at launch.
+
+        Returns:
+            float: The total mass of the rocket at launch, in kg.
+        """
         pass
 
     @abstractmethod
     def get_dry_mass(self) -> float:
+        """
+        Calculates the dry mass of the rocket.
+
+        Returns:
+            float: The dry mass of the rocket, in kg.
+        """
         pass
 
 
 class Rocket(RocketBaseClass):
     def __init__(
         self,
         propulsion: Motor,
         recovery: Recovery,
         fuselage: Fuselage,
         mass_without_motor: float,
     ) -> None:
+        """
+        Initializes a Rocket object.
+
+        Args:
+            propulsion (Motor): The motor or propulsion system of the rocket.
+            recovery (Recovery): The recovery system of the rocket.
+            fuselage (Fuselage): The fuselage or body of the rocket.
+            mass_without_motor (float): The mass of the rocket without the motor, in kg.
+        """
         super().__init__(
             propulsion=propulsion,
             recovery=recovery,
             fuselage=fuselage,
         )
-
         self.mass_without_motor = mass_without_motor
 
     def get_launch_mass(self) -> float:
+        """
+        Calculates the total mass of the rocket at launch.
+
+        Returns:
+            float: The total mass of the rocket at launch, in kg.
+        """
         return self.mass_without_motor + self.propulsion.get_launch_mass()
 
     def get_dry_mass(self) -> float:
-        return self.mass_without_motor + self.propulsion.get_dry_mass()
+        """
+        Calculates the dry mass of the rocket.
 
-
-class Rocket3D(RocketBaseClass):
-    def __init__(
-        self, propulsion: Motor, recovery: Recovery, fuselage: Fuselage3D
-    ) -> None:
-        super().__init__(
-            propulsion=propulsion, recovery=recovery, fuselage=fuselage
-        )
-
-    def get_launch_mass(self) -> float:
-        return self.propulsion.get_launch_mass() + self.fuselage.get_mass()
-
-    def get_dry_mass(self) -> float:
-        return self.propulsion.get_dry_mass() + self.fuselage.get_mass()
+        Returns:
+            float: The dry mass of the rocket, in kg.
+        """
+        return self.mass_without_motor + self.propulsion.get_dry_mass()
```

### Comparing `rocketsolver-0.3.0/rocketsolver/montecarlo/__init__.py` & `rocketsolver-0.5.0/rocketsolver/montecarlo/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,35 @@
-# -*- coding: utf-8 -*-
-# Author: Felipe Bogaerts de Mattos
-# Contact me at felipe.bogaerts@engenharia.ufjf.br.
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, version 3.
-
 from copy import deepcopy
 from dataclasses import dataclass
-from typing import Any, Optional
+from typing import Any, List, Optional
 
 import numpy as np
 import plotly.graph_objects as go
 
 from rocketsolver.montecarlo.random import get_random_generator
 from rocketsolver.operations import Operation
 from rocketsolver.simulations import Simulation
-from rocketsolver.utils.utilities import obtain_attributes_from_object
+from rocketsolver.services.common.utilities import (
+    obtain_attributes_from_object,
+)
 
 
 @dataclass
 class MonteCarloParameter:
     """
     Stores a Monte Carlo parameter alongside its upper/lower bound.
 
-    :param value: Parameter main value
-    :param lower_tolerance: Lower bound of the parameter
-    :param upper_tolerance: Upper bound of the parameter
-    :param tolerance: Tolerance of the parameter
-    :param probability_distribution: Probability distribution of the random
-        values. It can be set to 'uniform', 'normal' or any other distribution
-        supported by the numpy.random module.
-    :rtype: None
+    Args:
+        value: Parameter main value
+        lower_tolerance: Lower bound of the parameter
+        upper_tolerance: Upper bound of the parameter
+        tolerance: Tolerance of the parameter
+        probability_distribution: Probability distribution of the random
+            values. It can be set to 'uniform', 'normal' or any other
+            distribution supported by the numpy.random module.
     """
 
     value: float | int
     lower_tolerance: Optional[float | int] = 0
     upper_tolerance: Optional[float | int] = 0
     tolerance: Optional[float | int] = 0
     probability_distribution: str = "normal"
@@ -49,16 +44,16 @@
         )
 
     def get_random_value(self) -> float:
         """
         Generates a random value for the parameter, according to the
         probability distribution and tolerances.
 
-        :return: Random value
-        :rtype: float
+        Returns:
+            Random value
         """
         return self.probability_distribution_class.get_value()
 
     def __lt__(self, other: Any) -> bool:
         return self.value < other
 
     def __gt__(self, other: Any) -> bool:
@@ -98,67 +93,62 @@
     - Stores data for a Monte Carlo simulation
     - Executes the simulation
     - Presents distribution of results
     """
 
     def __init__(
         self,
-        parameters: list[Any],
+        parameters: List[Any],
         number_of_scenarios: int,
         simulation: Simulation,
     ) -> None:
         """
-        :param parameters: List with the input parameters for a simulation
-            class instance.
-        :param number_of_scenarios: Number of scenarios to be simulated.
-        :param simulation: Simulation class instance.
-        :rtype: None
-        """
+        Initializes a MonteCarloSimulation object.
 
+        Args:
+            parameters: List with the input parameters for a simulation
+                class instance.
+            number_of_scenarios: Number of scenarios to be simulated.
+            simulation: Simulation class instance.
+        """
         self.parameters = parameters
         self.number_of_scenarios = number_of_scenarios
         self.simulation = simulation
 
-        self.scenarios: list[list[float | int]] = []
-
-        # "results" gets populates when the "run" method is called. It gets
-        # filled with a list of simulation outputs.
-        self.results: list[list[Operation]] = []
+        self.scenarios: List[List[float | int]] = []
+        self.results: List[List[Operation]] = []
 
-    def generate_scenario(
-        self,
-    ) -> list[float | int]:
+    def generate_scenario(self) -> List[float | int]:
         """
-        Generates a monte carlo scenario in the form of a list of parameters.
+        Generates a Monte Carlo scenario in the form of a list of parameters.
 
         These parameters are randomly generated within the tolerance bounds,
-        set in the MontrCarloParameter class. The random numbers follow a
-        gaussian distribution.
+        set in the MonteCarloParameter class. The random numbers follow a
+        Gaussian distribution.
 
-        :return: Monte Carlo scenario
-        :rtype: list[float | int]
+        Returns:
+            Monte Carlo scenario
         """
-
         new_scenario = []
         parameters = deepcopy(self.parameters)
 
         for parameter in parameters:
             if isinstance(parameter, MonteCarloParameter):
                 parameter = parameter.get_random_value()
             else:
                 search_tree = {
                     parameter: obtain_attributes_from_object(parameter)
                 }
                 i = 0
 
                 while True:
-                    new_search_tree = {}  # search tree for the next iteration
+                    new_search_tree = {}
 
                     if len(search_tree) == 0:
-                        break  # skip iteration if there are no sub params
+                        break
 
                     for param, sub_params in search_tree.items():
                         for name, attr in sub_params.items():
                             if isinstance(attr, MonteCarloParameter):
                                 setattr(param, name, attr.get_random_value())
                             elif isinstance(attr, list):
                                 for item in attr:
@@ -188,51 +178,67 @@
 
             new_scenario.append(parameter)
 
         self.scenarios.append(new_scenario)
         return new_scenario
 
     def run(self) -> None:
+        """
+        Executes the Monte Carlo simulation.
+        """
         self.results = []
 
         for _ in range(self.number_of_scenarios):
             scenario = self.generate_scenario()
             self.results.append(self.simulation(*scenario).run())
 
-        return self.results
-
     def retrieve_values_from_result(
         self,
         operation_index: int,
         property: str,
     ) -> np.ndarray:
+        """
+        Retrieves a specific property from the simulation results.
+
+        Args:
+            operation_index: Index of the operation/result to retrieve the
+                property from.
+            property: Name of the property or the attribute of the operation
+                to retrieve.
+
+        Returns:
+            Numpy array containing the values of the specified property.
+        """
         return np.array(
             [
                 getattr(result[operation_index], property)
                 for result in self.results
             ]
         )
 
     def plot_histogram(
         self,
         operation_index: int,
         property: str,
         x_axes_title: Optional[str] = None,
         *args,
-        **kwargs
+        **kwargs,
     ) -> None:
         """
         Plots a histogram given a result index and the property name.
 
-        :param operation_index: Index of the operation/result to plot
-        :param property: Name of the property or the attribute of the
-            operation to plot.
-        :param x_axes_title: Title of the x axes. By default, the property
-            name is used.
-        :rtype: None
+        Args:
+            operation_index: Index of the operation/result to plot.
+            property: Name of the property or the attribute of the operation
+                to plot.
+            x_axes_title: Title of the x axes. By default, the property name
+                is used.
+            *args: Additional arguments to pass to the histogram plot.
+            **kwargs: Additional keyword arguments to pass to the histogram
+                plot.
         """
         values = self.retrieve_values_from_result(
             operation_index=operation_index, property=property
         )
 
         fig = go.Figure()
         fig.add_trace(go.Histogram(x=values, *args, **kwargs))
```

### Comparing `rocketsolver-0.3.0/rocketsolver/operations/ballistics/_1dof.py` & `rocketsolver-0.5.0/rocketsolver/operations/ballistics/_1dof.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,47 @@
-# -*- coding: utf-8 -*-
-# Author: Felipe Bogaerts de Mattos
-# Contact me at felipe.bogaerts@engenharia.ufjf.br.
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, version 3.
-
 from typing import Optional
 
 import numpy as np
 
 from . import BallisticOperation
 from rocketsolver.models.atmosphere import Atmosphere
 from rocketsolver.models.rocket import Rocket
-from rocketsolver.solvers.ballistics_1d import Ballistics1D
+from rocketsolver.services.equations import ballistics_ode
+from rocketsolver.solvers.odes import rk4th_ode_solver
 
 
 class Ballistic1DOperation(BallisticOperation):
-    """
-    Stores and processes a ballistics operation (aka flight).
-    """
+    """Stores and processes a ballistics operation (aka flight)."""
 
     def __init__(
         self,
         rocket: Rocket,
         atmosphere: Atmosphere,
         rail_length: float,
         motor_dry_mass: float,
         initial_vehicle_mass: float,
         initial_elevation_amsl: Optional[float] = 0,
     ) -> None:
         """
-        Initializes attributes for the operation.
+        Initialize the attributes for the ballistics operation.
+
+        Args:
+            rocket (Rocket): The rocket used for the operation.
+            atmosphere (Atmosphere): The atmospheric conditions.
+            rail_length (float): The length of the rail for launch.
+            motor_dry_mass (float): The dry mass of the motor.
+            initial_vehicle_mass (float): The initial mass of the vehicle.
+            initial_elevation_amsl (float, optional): The initial elevation above mean sea level (AMSL). Defaults to 0.
         """
         self.rocket = rocket
         self.atmosphere = atmosphere
         self.rail_length = rail_length
         self.motor_dry_mass = motor_dry_mass
         self.initial_elevation_amsl = initial_elevation_amsl
 
-        self.ballistics_solver = Ballistics1D()
-
         self.t = np.array([0])  # time vector
 
         self.P_ext = np.array(
             [self.atmosphere.get_pressure(initial_elevation_amsl)]
         )  # external pressure
         self.rho_air = np.array(
             [self.atmosphere.get_density(initial_elevation_amsl)]
@@ -55,52 +53,52 @@
             [initial_vehicle_mass]
         )  # total mass of the vehicle
 
         # Spacial params:
         self.y = np.array([0])  # altitude, AGL
         self.v = np.array([0])  # velocity
         self.acceleration = np.array([0])  # acceleration
-        self.mach_no = np.array([0])  # mach number
+        self.mach_no = np.array([0])  # Mach number
 
         self.velocity_out_of_rail = None
 
     @property
     def apogee(self) -> float:
-        """
-        Returns the apogee of the operation.
-        """
+        """Get the apogee of the operation."""
         return np.max(self.y)
 
     @property
     def apogee_time(self) -> float:
-        """
-        Returns the time of the apogee.
-        """
+        """Get the time of the apogee."""
         return self.t[np.argmax(self.y)]
 
     @property
     def max_velocity(self) -> float:
-        """
-        Returns the maximum velocity of the operation.
-        """
+        """Get the maximum velocity of the operation."""
         return np.max(self.v)
 
     @property
     def max_velocity_time(self) -> float:
-        """
-        Returns the time of the maximum velocity.
-        """
+        """Get the time of the maximum velocity."""
         return self.t[np.argmax(self.v)]
 
     def iterate(
         self,
         propellant_mass: float,
         thrust: float,
         d_t: float,
     ) -> None:
+        """
+        Perform an iteration of the ballistics operation.
+
+        Args:
+            propellant_mass (float): The mass of the propellant.
+            thrust (float): The thrust force.
+            d_t (float): The time step.
+        """
         self.t = np.append(self.t, self.t[-1] + d_t)  # append new time value
 
         self.rho_air = np.append(
             self.rho_air,
             self.atmosphere.get_density(
                 y_amsl=(self.y[-1] + self.initial_elevation_amsl)
             ),
@@ -109,15 +107,15 @@
             self.g,
             self.atmosphere.get_gravity(
                 self.initial_elevation_amsl + self.y[-1]
             ),
         )
 
         # Appending the current vehicle mass, consisting of the motor
-        # structural mass, mass without the motor and propellant mass.
+        # structural mass, mass without the motor, and propellant mass.
         self.vehicle_mass = np.append(
             self.vehicle_mass, propellant_mass + self.rocket.get_dry_mass()
         )
 
         # Drag properties:
         fuselage_area = self.rocket.fuselage.frontal_area
         fuselage_drag_coeff = self.rocket.fuselage.get_drag_coefficient()
@@ -136,22 +134,22 @@
                 fuselage_area * fuselage_drag_coeff
                 + recovery_area * recovery_drag_coeff
             )
             * self.rho_air[-1]
             * 0.5
         )
 
-        ballistics_results = self.ballistics_solver.solve(
-            self.y[-1],
-            self.v[-1],
-            thrust,
-            D,
-            self.vehicle_mass[-1],
-            self.g[-1],
-            d_t,
+        ballistics_results = rk4th_ode_solver(
+            variables={"y": self.y[-1], "v": self.v[-1]},
+            equation=ballistics_ode,
+            d_t=d_t,
+            T=thrust,
+            D=D,
+            M=self.vehicle_mass[-1],
+            g=self.g[-1],
         )
 
         height = ballistics_results[0]
         velocity = ballistics_results[1]
         acceleration = ballistics_results[2]
 
         if height < 0 and len(self.y[self.y > 0]) == 0:
@@ -179,15 +177,15 @@
         )
 
         if self.velocity_out_of_rail is None and self.y[-1] > self.rail_length:
             self.velocity_out_of_rail = self.v[-2]
 
     def print_results(self) -> None:
         """
-        Prints the results of the operation.
+        Print the results of the ballistics operation.
         """
         print("\nROCKET BALLISTICS")
 
         print(f" Apogee: {np.max(self.y):.2f} m")
         print(f" Max. velocity: {np.max(self.v):.2f} m/s")
         print(f" Max. Mach number: {np.max(self.mach_no):.3f}")
         print(f" Max. acceleration: {np.max(self.acceleration) / 9.81:.2f} gs")
```

### Comparing `rocketsolver-0.3.0/rocketsolver/operations/internal_ballistics/__init__.py` & `rocketsolver-0.5.0/rocketsolver/operations/internal_ballistics/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,25 @@
-# -*- coding: utf-8 -*-
-# Author: Felipe Bogaerts de Mattos
-# Contact me at felipe.bogaerts@engenharia.ufjf.br.
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, version 3.
-
 from abc import abstractmethod
 from typing import Optional
 
 import numpy as np
 
 from rocketsolver.operations import Operation
-from rocketsolver.solvers.srm_internal_ballistics import (
-    SRMInternalBallisticsSolver,
-)
+from rocketsolver.solvers.odes import rk4th_ode_solver
+from rocketsolver.services.equations import solve_cp_seidel
 from rocketsolver.models.propulsion import Motor, SolidMotor
-from rocketsolver.utils.isentropic_flow import (
+from rocketsolver.services.isentropic_flow import (
     get_critical_pressure_ratio,
-    get_opt_expansion_ratio,
     get_exit_pressure,
     get_operational_correction_factors,
     get_thrust_coefficients,
     get_thrust_from_cf,
     is_flow_choked,
 )
-from rocketsolver.utils.units import (
+from rocketsolver.services.conversions import (
     convert_pa_to_psi,
     convert_mass_flux_metric_to_imperial,
 )
 
 
 class MotorOperation(Operation):
     """
@@ -47,17 +38,16 @@
         Each motor category will contain a particular set of attributes.
         """
         self.motor = motor
 
         self.t = np.array([0])  # time vector
 
         self.V_0 = np.array(
-            [motor.structure.chamber.get_empty_volume()]
+            [motor.structure.chamber.empty_volume]
         )  # empty chamber volume
-        self.optimal_expansion_ratio = np.array([1])  # optimal expansion ratio
         self.m_prop = np.array(
             [motor.initial_propellant_mass]
         )  # propellant mass
         self.P_0 = np.array([initial_pressure])  # chamber stagnation pressure
         self.P_exit = np.array([initial_atmospheric_pressure])  # exit pressure
 
         # Thrust coefficients and thrust:
@@ -95,56 +85,54 @@
         Prints results obtained during simulation/operation.
         """
         pass
 
     @property
     def initial_propellant_mass(self) -> float:
         """
-        :return: Initial propellant mass.
+        Get the initial propellant mass.
+
+        Returns:
+            float: The initial propellant mass.
         """
         return self.motor.initial_propellant_mass
 
 
 class SRMOperation(MotorOperation):
     """
     Operation for a Solid Rocket Motor.
 
-    The variable names correspond to what they are commonly reffered to in
+    The variable names correspond to what they are commonly referred to in
     books and papers related to Solid Rocket Propulsion.
 
     Therefore, PEP8's snake_case will not be followed rigorously.
     """
 
     def __init__(
         self,
         motor: SolidMotor,
         initial_pressure: float,
         initial_atmospheric_pressure: float,
-        ib_solver: Optional[
-            SRMInternalBallisticsSolver
-        ] = SRMInternalBallisticsSolver(),
     ) -> None:
         """
         Initial parameters for a SRM operation.
         """
-        self.ib_solver = ib_solver
-
         super().__init__(
             motor=motor,
             initial_pressure=initial_pressure,
             initial_atmospheric_pressure=initial_atmospheric_pressure,
         )
 
         # Grain and propellant parameters:
         self.web = np.array([0])  # instant web thickness
         self.burn_area = np.array(
             [self.motor.grain.get_burn_area(self.web[0])]
         )
         self.propellant_volume = np.array(
-            [self.motor.grain.get_burn_area(self.web[0])]
+            [self.motor.grain.get_propellant_volume(self.web[0])]
         )
         self.burn_rate = np.array([0])  # burn rate
 
         # Correction factors:
         self.n_kin = np.array([0])  # kinetics correction factor
         self.n_bl = np.array([0])  # boundary layer correction factor
         self.n_tp = np.array([0])  # two-phase flow correction factor
@@ -152,18 +140,22 @@
 
     def iterate(
         self,
         d_t: float,
         P_ext: float,
     ) -> None:
         """
-        The function uses the Runge-Kutta 4th order numerical method for
-        solving the differential equations.
+        Iterate the motor operation by calculating and storing operational
+        parameters in the corresponding vectors.
+
+        Args:
+            d_t (float): The time increment.
+            P_ext (float): The external pressure.
         """
-        if self.end_thrust is False:
+        if not self.end_thrust:
             self.t = np.append(
                 self.t, self.t[-1] + d_t
             )  # append new time value
 
             self.burn_area = np.append(
                 self.burn_area, self.motor.grain.get_burn_area(self.web[-1])
             )
@@ -190,34 +182,28 @@
             )
 
             d_x = d_t * self.burn_rate[-1]
             self.web = np.append(self.web, self.web[-1] + d_x)
 
             self.P_0 = np.append(
                 self.P_0,
-                self.ib_solver.solve(
-                    self.P_0[-1],
-                    P_ext,
-                    self.burn_area[-1],
-                    self.V_0[-1],
-                    self.motor.structure.nozzle.get_throat_area(),
-                    self.motor.propellant.density,
-                    self.motor.propellant.k_mix_ch,
-                    self.motor.propellant.R_ch,
-                    self.motor.propellant.T0,
-                    self.burn_rate[-1],
-                    d_t,
-                ),
-            )
-
-            self.optimal_expansion_ratio = np.append(
-                self.optimal_expansion_ratio,
-                get_opt_expansion_ratio(
-                    self.motor.propellant.k_2ph_ex, self.P_0[-1], P_ext
-                ),
+                rk4th_ode_solver(
+                    variables={"P0": self.P_0[-1]},
+                    equation=solve_cp_seidel,
+                    d_t=d_t,
+                    Pe=P_ext,
+                    Ab=self.burn_area[-1],
+                    V0=self.V_0[-1],
+                    At=self.motor.structure.nozzle.get_throat_area(),
+                    pp=self.motor.propellant.density,
+                    k=self.motor.propellant.k_mix_ch,
+                    R=self.motor.propellant.R_ch,
+                    T0=self.motor.propellant.T0,
+                    r=self.burn_rate[-1],
+                )[0],
             )
 
             self.P_exit = np.append(
                 self.P_exit,
                 get_exit_pressure(
                     self.motor.propellant.k_2ph_ex,
                     self.motor.structure.nozzle.expansion_ratio,
@@ -270,29 +256,32 @@
                 get_thrust_from_cf(
                     self.C_f[-1],
                     self.P_0[-1],
                     self.motor.structure.nozzle.get_throat_area(),
                 ),
             )  # thrust calculation
 
-            if self.m_prop[-1] == 0 and self.end_burn is False:
+            if self.m_prop[-1] == 0 and not self.end_burn:
                 self.burn_time = self.t[-1]
                 self.end_burn = True
 
             # This if statement changes 'end_thrust' to True if supersonic
             # flow is not achieved anymore.
             if is_flow_choked(
                 self.P_0[-1],
                 P_ext,
                 get_critical_pressure_ratio(self.motor.propellant.k_mix_ch),
             ):
                 self.thrust_time = self.t[-1]
                 self.end_thrust = True
 
     def print_results(self) -> None:
+        """
+        Prints the results obtained during the SRM operation.
+        """
         print("\nBURN REGRESSION")
         if self.m_prop[0] > 1:
             print(f" Propellant initial mass {self.m_prop[0]:.3f} kg")
         else:
             print(f" Propellant initial mass {self.m_prop[0] * 1e3:.3f} g")
         print(" Mean Kn: %.2f" % np.mean(self.klemmung))
         print(" Max Kn: %.2f" % np.max(self.klemmung))
@@ -325,56 +314,105 @@
         )
 
         print("\nNOZZLE DESIGN")
         print(f" Average nozzle efficiency: {np.mean(self.n_cf):.3%}")
 
     @property
     def klemmung(self) -> np.ndarray:
+        """
+        Get the klemmung values.
+
+        Returns:
+            np.ndarray: The klemmung values.
+        """
         return (
             self.burn_area[self.burn_area > 0]
             / self.motor.structure.nozzle.get_throat_area()
         )
 
     @property
     def initial_to_final_klemmung_ratio(self) -> float:
+        """
+        Get the ratio of the initial to final klemmung.
+
+        Returns:
+            float: The ratio of the initial to final klemmung.
+        """
         return self.klemmung[0] / self.klemmung[-1]
 
     @property
     def volumetric_efficiency(self) -> float:
+        """
+        Get the volumetric efficiency.
+
+        Returns:
+            float: The volumetric efficiency.
+        """
         return (
             self.propellant_volume[0]
-            / self.motor.structure.chamber.get_empty_volume()
+            / self.motor.structure.chamber.empty_volume
         )
 
     @property
     def burn_profile(self, deviancy: Optional[float] = 0.02) -> str:
         """
-        Returns string with burn profile.
+        Get the burn profile.
+
+        Args:
+            deviancy (float, optional): The deviancy threshold for determining the burn profile.
+                Defaults to 0.02.
+
+        Returns:
+            str: The burn profile ("regressive", "progressive", or "neutral").
         """
         burn_area = self.burn_area[self.burn_area > 0]
 
         if burn_area[0] / burn_area[-1] > 1 + deviancy:
             return "regressive"
         elif burn_area[0] / burn_area[-1] < 1 - deviancy:
             return "progressive"
         else:
             return "neutral"
 
     @property
     def max_mass_flux(self) -> float:
+        """
+        Get the maximum mass flux.
+
+        Returns:
+            float: The maximum mass flux.
+        """
         return np.max(self.grain_mass_flux)
 
     @property
     def grain_mass_flux(self) -> np.ndarray:
+        """
+        Get the grain mass flux.
+
+        Returns:
+            np.ndarray: The grain mass flux.
+        """
         return self.motor.grain.get_mass_flux_per_segment(
             self.burn_rate,
             self.motor.propellant.density,
             self.web,
         )
 
     @property
     def total_impulse(self) -> float:
+        """
+        Get the total impulse.
+
+        Returns:
+            float: The total impulse.
+        """
         return np.mean(self.thrust) * self.t[-1]
 
     @property
     def specific_impulse(self) -> float:
+        """
+        Get the specific impulse.
+
+        Returns:
+            float: The specific impulse.
+        """
         return self.total_impulse / self.m_prop[0] / 9.81
```

### Comparing `rocketsolver-0.3.0/rocketsolver/simulations/__init__.py` & `rocketsolver-0.5.0/rocketsolver/simulations/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,69 @@
-# -*- coding: utf-8 -*-
-# Author: Felipe Bogaerts de Mattos
-# Contact me at felipe.bogaerts@engenharia.ufjf.br.
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, version 3.
-
 from abc import ABC, abstractmethod
 
 from rocketsolver.operations import Operation
 
 
 class SimulationParameters(ABC):
     """
-    Class that stores simulation parameters and that should always be passed
-    to the corresponding simulation. Every Simulation class should also have
-    a SimulationParameters class associated with it.
+    Abstract class that stores simulation parameters and should be subclassed
+    for specific simulations.
 
     Examples of simulation parameters:
-    - time step for an time-based iterative simulation
-    - initial elevation, in case of a rocket launch
-    - igniter pressure, in case of an internal ballistic simulation
+    - time step for a time-based iterative simulation
+    - initial elevation in the case of a rocket launch
+    - igniter pressure in the case of an internal ballistic simulation
     """
 
     pass
 
 
 class Simulation(ABC):
     """
-    The Simulation class stores simulation parameters, arguments and runs the
-    main loop of an iterative simulation.
+    Abstract class that represents a simulation. Subclasses of Simulation
+    implement specific simulation logic.
+
+    NOTE: Instances of this class should not store any simulation state.
+    Storing and analyzing simulation data should be done only by the Operation
+    class.
+
+    Attributes:
+        params (SimulationParameters): Object containing simulation parameters.
 
-    NOTE: Instances of this class shall not store any simulation state.
-    Storing and analyzing simulation data should be done only by the
-    Operation class.
     """
 
     def __init__(self, params: SimulationParameters) -> None:
         """
-        :param SimulationParameters params: Object containing every parameter
-            needed for a certain simulation to execute. Example:
-            A Rocket launch needs to know the initial elevation of the launch
-            base in order to determine the air density.
-        :returns: None
-        :rtype: None
+        Initializes the Simulation instance with the provided parameters.
+
+        Args:
+            params (SimulationParameters): Object containing simulation
+                parameters.
+
         """
         self.params = params
 
     @abstractmethod
     def run(self) -> list[Operation]:
         """
-        Runs the simulation. In most cases, contains a loop that iterates over
-        time or distance.
+        Runs the simulation. This method should be implemented by subclasses.
+        It typically contains a loop that iterates over time or distance.
+
+        Returns:
+            list[Operation]: A list of Operation instances representing the
+            operations performed during the simulation.
 
-        :returns: A list of instances of the Operation class.
-        :rtype: list[Operation]
         """
         pass
 
     @abstractmethod
     def print_results(self, *args, **kwargs):
         """
-        Prints the results of the simulation, by calling the print_results
-        method inside the Operation class instances of the simulation.
+        Prints the results of the simulation by calling the print_results
+        method on the Operation instances of the simulation.
+
+        Args:
+            *args: Additional positional arguments.
+            **kwargs: Additional keyword arguments.
+
         """
         pass
```

### Comparing `rocketsolver-0.3.0/rocketsolver/simulations/ballistics.py` & `rocketsolver-0.5.0/rocketsolver/simulations/ballistics.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,30 @@
-# -*- coding: utf-8 -*-
-# Author: Felipe Bogaerts de Mattos
-# Contact me at felipe.bogaerts@engenharia.ufjf.br.
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, version 3.
-
 import numpy as np
 
 from rocketsolver.models.atmosphere import Atmosphere
 from rocketsolver.models.recovery import Recovery
 from rocketsolver.models.rocket import Rocket
 from rocketsolver.operations.ballistics._1dof import Ballistic1DOperation
 from rocketsolver.simulations import Simulation, SimulationParameters
 
 
 class BallisticSimulationParameters(SimulationParameters):
+    """
+    Parameters for a ballistic simulation.
+
+    Attributes:
+        thrust (np.ndarray): Array of thrust values.
+        motor_dry_mass (float): Dry mass of the motor.
+        initial_propellant_mass (float): Initial mass of the propellant.
+        time (np.ndarray): Array of time values.
+        d_t (float): Time step.
+        initial_elevation_amsl (float): Initial elevation above mean sea level.
+        rail_length (float): Length of the launch rail.
+    """
+
     def __init__(
         self,
         thrust: np.ndarray,
         motor_dry_mass: float,
         initial_propellant_mass: float,
         time: np.ndarray,
         d_t: float,
@@ -31,80 +37,109 @@
         self.time = time
         self.d_t = d_t
         self.initial_elevation_amsl = initial_elevation_amsl
         self.rail_length = rail_length
 
 
 class BallisticSimulation(Simulation):
+    """
+    Ballistic simulation class.
+
+    Attributes:
+        rocket (Rocket): The rocket object.
+        atmosphere (Atmosphere): The atmosphere object.
+        params (BallisticSimulationParameters): The simulation parameters.
+        t (np.ndarray): Array of time values.
+        ballistic_operation (Ballistic1DOperation): The ballistic operation
+            object.
+    """
+
     def __init__(
         self,
         rocket: Rocket,
         atmosphere: Atmosphere,
         params: BallisticSimulationParameters,
     ) -> None:
-        super().__init__(params=params)
+        """
+        Initializes the BallisticSimulation instance.
 
+        Args:
+            rocket (Rocket): The rocket object.
+            atmosphere (Atmosphere): The atmosphere object.
+            params (BallisticSimulationParameters): The simulation parameters.
+        """
+        super().__init__(params=params)
         self.rocket = rocket
         self.atmosphere = atmosphere
-
         self.t = np.array([0])
+        self.ballistic_operation = None
 
     def get_propellant_mass(self) -> np.ndarray:
+        """
+        Computes the propellant mass at each time step.
+
+        Returns:
+            np.ndarray: Array of propellant mass values.
+        """
         initial_propellant_mass = self.params.initial_propellant_mass
         prop_mass = np.array([])
         time = self.params.time
 
-        for t in self.time:
+        for t in time:
             prop_mass = np.append(
                 prop_mass, initial_propellant_mass * (time[-1] - t) / time[-1]
             )
 
         return prop_mass
 
     def run(self) -> tuple[np.array, Ballistic1DOperation]:
         """
-        Runs the main loop of the simulation, returning all the internal and
-        external ballistics parameters.
+        Runs the main loop of the simulation, returning the time array and
+        the ballistic operation object.
+
+        Returns:
+            tuple[np.array, Ballistic1DOperation]: A tuple containing the time
+            array and the ballistic operation object.
         """
         self.ballistic_operation = Ballistic1DOperation(
             self.rocket,
             self.atmosphere,
-            rail_length=self.rail_length,
-            motor_dry_mass=self.params.motor_dry_mass,
-            initial_vehicle_mass=self.rocket.structure.mass_without_motor
-            + self.params.motor_dry_mass
-            + self.params.initial_propellant_mass,
+            rail_length=self.params.rail_length,
+            motor_dry_mass=self.rocket.propulsion.get_dry_mass(),
+            initial_vehicle_mass=self.rocket.get_launch_mass(),
             initial_elevation_amsl=self.params.initial_elevation_amsl,
         )
 
         propellant_mass = self.get_propellant_mass()
 
         i = 0
 
         while self.ballistic_operation.y[i] >= 0:
-            self.t = np.append(self.t, self.t[i] + self.d_t)  # new time value
+            self.t = np.append(
+                self.t, self.t[i] + self.params.d_t
+            )  # new time value
 
             thrust = np.interp(
                 self.t[-1],
-                self.time,
-                self.thrust,
+                self.params.time,
+                self.params.thrust,
                 left=0,
                 right=0,
             )  # interpolating thrust with new time value
 
             self.ballistic_operation.iterate(
                 np.interp(
                     self.t[-1],
-                    self.time,
+                    self.params.time,
                     propellant_mass,
                     left=0,
                     right=0,
                 ),  # interpolating propellant mass with new time value
                 thrust,
-                self.d_t,
+                self.params.d_t,
             )
 
             i += 1
 
         return (self.t, self.ballistic_operation)
 
     def print_results(self):
```

### Comparing `rocketsolver-0.3.0/rocketsolver/simulations/internal_balistics_coupled.py` & `rocketsolver-0.5.0/rocketsolver/simulations/internal_balistics_coupled.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-# -*- coding: utf-8 -*-
-# Author: Felipe Bogaerts de Mattos
-# Contact me at felipe.bogaerts@engenharia.ufjf.br.
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, version 3.
-
 """
 The coupled internal ballistics simulation calculates both internal and 
 external ballistics parameters simulatneously. 
 
 The main advantage of this strategy is that, while some environmental 
 attributes change during flight, they also serve as inputs for the internal 
 ballistic of the motor. The main attribute that changes during flight is the 
@@ -18,69 +11,104 @@
 import numpy as np
 
 from rocketsolver.models.atmosphere import Atmosphere
 from rocketsolver.models.rocket import Rocket
 from rocketsolver.operations.ballistics._1dof import Ballistic1DOperation
 from rocketsolver.operations.internal_ballistics import MotorOperation
 from rocketsolver.simulations import Simulation, SimulationParameters
-from rocketsolver.utils.classes import get_motor_operation_class
+from rocketsolver.services.factories import get_motor_operation_class
 
 
 class InternalBallisticsCoupledParams(SimulationParameters):
+    """
+    Parameters for a coupled internal ballistics simulation.
+
+    Attributes:
+        atmosphere (Atmosphere): The atmosphere object.
+        d_t (float): Time step for the ballistic simulation.
+        dd_t (float): Time step factor for the motor simulation.
+        initial_elevation_amsl (float): Initial elevation above mean sea level.
+        igniter_pressure (float): Igniter pressure.
+        rail_length (float): Length of the launch rail.
+    """
+
     def __init__(
         self,
         atmosphere: Atmosphere,
         d_t: float,
         dd_t: float,
         initial_elevation_amsl: float,
         igniter_pressure: float,
         rail_length: float,
     ) -> None:
         super().__init__()
-
         self.atmosphere = atmosphere
         self.d_t = d_t
         self.dd_t = dd_t
         self.initial_elevation_amsl = initial_elevation_amsl
         self.igniter_pressure = igniter_pressure
         self.rail_length = rail_length
 
 
 class InternalBallisticsCoupled(Simulation):
+    """
+    Coupled internal ballistics simulation class.
+
+    Attributes:
+        rocket (Rocket): The rocket object.
+        params (InternalBallisticsCoupledParams): The simulation parameters.
+        t (np.ndarray): Array of time values.
+        motor_operation (MotorOperation): The motor operation object.
+        ballistic_operation (Ballistic1DOperation): The ballistic operation object.
+    """
+
     def __init__(
         self,
         rocket: Rocket,
         params: InternalBallisticsCoupledParams,
     ) -> None:
-        super().__init__(params=params)
+        """
+        Initializes the InternalBallisticsCoupled instance.
 
+        Args:
+            rocket (Rocket): The rocket object.
+            params (InternalBallisticsCoupledParams): The simulation parameters.
+        """
+        super().__init__(params=params)
         self.rocket = rocket
-
         self.t = np.array([0])
+        self.motor_operation = None
+        self.ballistic_operation = None
 
     def get_motor_operation(self) -> MotorOperation:
         """
-        Will depend on the type of the motor (SR, HRE or LRE).
+        Returns the motor operation object based on the type of the motor.
+
+        Returns:
+            MotorOperation: The motor operation object.
         """
         motor_operation_class = get_motor_operation_class(
             self.rocket.propulsion
         )
-
         return motor_operation_class(
             motor=self.rocket.propulsion,
             initial_pressure=self.params.igniter_pressure,
             initial_atmospheric_pressure=self.params.atmosphere.get_pressure(
                 self.params.initial_elevation_amsl
             ),
         )
 
     def run(self) -> tuple[MotorOperation, Ballistic1DOperation]:
         """
-        Runs the main loop of the simulation, returning all the internal and
-        external ballistics parameters.
+        Runs the main loop of the simulation, returning the motor operation
+        and ballistic operation objects.
+
+        Returns:
+            tuple[MotorOperation, Ballistic1DOperation]: A tuple containing
+            the motor operation object and the ballistic operation object.
         """
         self.motor_operation = self.get_motor_operation()
         self.ballistic_operation = Ballistic1DOperation(
             self.rocket,
             self.params.atmosphere,
             rail_length=self.params.rail_length,
             motor_dry_mass=self.rocket.propulsion.get_dry_mass(),
```

### Comparing `rocketsolver-0.3.0/rocketsolver/simulations/internal_ballistics.py` & `rocketsolver-0.5.0/rocketsolver/simulations/internal_ballistics.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,87 @@
-# -*- coding: utf-8 -*-
-# Author: Felipe Bogaerts de Mattos
-# Contact me at felipe.bogaerts@engenharia.ufjf.br.
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, version 3.
-
 import numpy as np
 
 from rocketsolver.models.propulsion import Motor
 from rocketsolver.operations.internal_ballistics import MotorOperation
 from rocketsolver.simulations import Simulation, SimulationParameters
-from rocketsolver.utils.classes import get_motor_operation_class
+from rocketsolver.services.factories import get_motor_operation_class
 
 
 class InternalBallisticsParams(SimulationParameters):
+    """
+    Parameters for an internal ballistics simulation.
+
+    Attributes:
+        d_t (float): Time step.
+        igniter_pressure (float): Igniter pressure.
+        external_pressure (float): External pressure.
+    """
+
     def __init__(
         self,
         d_t: float,
         igniter_pressure: float,
         external_pressure: float,
     ) -> None:
         super().__init__()
-
         self.d_t = d_t
         self.igniter_pressure = igniter_pressure
         self.external_pressure = external_pressure
 
 
 class InternalBallistics(Simulation):
+    """
+    Internal ballistics simulation class.
+
+    Attributes:
+        motor (Motor): The motor object.
+        params (InternalBallisticsParams): The simulation parameters.
+        t (np.ndarray): Array of time values.
+        motor_operation (MotorOperation): The motor operation object.
+    """
+
     def __init__(
         self,
         motor: Motor,
         params: InternalBallisticsParams,
     ) -> None:
-        super().__init__(params=params)
+        """
+        Initializes the InternalBallistics instance.
 
+        Args:
+            motor (Motor): The motor object.
+            params (InternalBallisticsParams): The simulation parameters.
+        """
+        super().__init__(params=params)
         self.motor = motor
-
         self.t = np.array([0])
+        self.motor_operation = None
 
     def get_motor_operation(self) -> MotorOperation:
         """
-        Will depend on the type of the motor (SR, HRE or LRE).
+        Returns the motor operation object based on the type of the motor.
+
+        Returns:
+            MotorOperation: The motor operation object.
         """
         motor_operation_class = get_motor_operation_class(self.motor)
-
         return motor_operation_class(
             motor=self.motor,
             initial_pressure=self.params.igniter_pressure,
             initial_atmospheric_pressure=self.params.external_pressure,
         )
 
     def run(self):
         """
-        Runs the main loop of the simulation, returning all the internal and
-        external ballistics parameters.
+        Runs the main loop of the simulation, returning the motor operation
+        object.
+
+        Returns:
+            tuple[np.ndarray, MotorOperation]: A tuple containing the time
+                array and the motor operation object.
         """
         self.motor_operation = self.get_motor_operation()
 
         i = 0
 
         while not self.motor_operation.end_thrust:
             self.t = np.append(
```

### Comparing `rocketsolver-0.3.0/rocketsolver/utils/plots.py` & `rocketsolver-0.5.0/rocketsolver/services/common/plots.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-# -*- coding: utf-8 -*-
-# Author: Felipe Bogaerts de Mattos
-# Contact me at felipe.bogaerts@engenharia.ufjf.br.
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, version 3.
-
-"""
-Plotting functions.
-"""
-
 import matplotlib.gridspec as gs
 import matplotlib.pyplot as plt
 import numpy as np
 import plotly.graph_objects as go
 import plotly.subplots
 
 
@@ -55,14 +44,31 @@
     figure.update_yaxes(
         title_text="<b>Pressure</b> (MPa)", secondary_y=True, color="#008141"
     )
 
     return figure
 
 
+def mass_flux_plot(mass_flux: np.ndarray, t: np.ndarray) -> go.Figure:
+    figure = go.Figure()
+
+    for i in range(len(mass_flux)):
+        figure.add_trace(
+            go.Scatter(
+                x=t,
+                y=mass_flux[i, :],
+                name="Segment " + str(i + 1),
+            )
+        )
+
+    figure.update_layout(title="Segment Mass Flux")
+
+    return figure
+
+
 def ballistics_plots(t, a, v, y, g):
     fig1 = plt.figure()
 
     plt.subplot(3, 1, 1)
     plt.ylabel("Height (m)")
     plt.grid(linestyle="-.")
     plt.plot(t, y, color="b")
@@ -285,25 +291,7 @@
     ax4.set_xlim(0, t[-1])
     ax4.grid(linestyle="-", linewidth=".4")
     ax4.plot(t[: len(m_prop)], m_prop, color="r", linewidth="1.5")
 
     main_figure.set_size_inches(12, 8, forward=True)
     main_figure.savefig("output/MotorPlots.png", dpi=300)
     return main_figure
-
-
-def mass_flux_plot(t, grain_mass_flux, t_burnout):
-    """Plots and saves figure of the mass flux for all the grain segments"""
-    t = t[t <= t_burnout]
-    t = np.append(t, t[-1])
-    grain_mass_flux = grain_mass_flux
-    N, index = grain_mass_flux.shape
-    mass_flux_figure = plt.figure()
-    for i in range(N):
-        plt.plot(t[: len(grain_mass_flux[i])], grain_mass_flux[i] * 1.42233e-3)
-    plt.ylabel("Mass Flux [lb/s-in-in]")
-    plt.xlabel("Time [s]")
-    plt.ylim(0, np.max(grain_mass_flux) * 1.42233e-3 * 1.05)
-    plt.xlim(0, t[-1])
-    plt.grid(linestyle="-", linewidth=".4")
-    mass_flux_figure.savefig("output/GrainMassFlux.png", dpi=300)
-    return mass_flux_figure
```

### Comparing `rocketsolver-0.3.0/rocketsolver/utils/utilities.py` & `rocketsolver-0.5.0/rocketsolver/services/common/utilities.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-# -*- coding: utf-8 -*-
-# Author: Felipe Bogaerts de Mattos
-# Contact me at felipe.bogaerts@engenharia.ufjf.br.
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, version 3.
-
-"""
-Stores utility functions, used in various locations throughtout the 
-application.
-"""
-
 from pathlib import Path
 
 import numpy as np
 
 
 def generate_eng(
     time: np.ndarray,
```

### Comparing `rocketsolver-0.3.0/rocketsolver.egg-info/PKG-INFO` & `rocketsolver-0.5.0/rocketsolver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocketsolver
-Version: 0.3.0
+Version: 0.5.0
 Summary: Rocket simulator
 Author-email: Felipe Bogaerts de Mattos <me@felipebm.com>
 License: GNU GENERAL PUBLIC LICENSE
            Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
         Everyone is permitted to copy and distribute verbatim copies
@@ -728,11 +728,7 @@
 ## a015140
 
 Correction factors.
 
 ## Hans Seidel's Chamber Pressure article
 
 Chamber Pressure equation.
-
-## 6DOF Trajectory Simulator
-
-http://pee.ufrj.br/teses/textocompleto/2007062901.pdf
```

### Comparing `rocketsolver-0.3.0/rocketsolver.egg-info/SOURCES.txt` & `rocketsolver-0.5.0/rocketsolver.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,58 @@
 README.md
+license.txt
 pyproject.toml
-rocketsolver/__init__.py
 rocketsolver.egg-info/PKG-INFO
 rocketsolver.egg-info/SOURCES.txt
 rocketsolver.egg-info/dependency_links.txt
 rocketsolver.egg-info/requires.txt
 rocketsolver.egg-info/top_level.txt
-rocketsolver/analytics/__init__.py
-rocketsolver/analytics/srm/__init__.py
-rocketsolver/models/__init__.py
 rocketsolver/models/atmosphere/__init__.py
-rocketsolver/models/fuselage/__init__.py
-rocketsolver/models/fuselage/components/__init__.py
-rocketsolver/models/fuselage/components/body/__init__.py
-rocketsolver/models/fuselage/components/fins/__init__.py
-rocketsolver/models/fuselage/components/fins/trapezoidal.py
-rocketsolver/models/fuselage/components/nosecones/__init__.py
-rocketsolver/models/fuselage/components/nosecones/haack.py
 rocketsolver/models/materials/__init__.py
 rocketsolver/models/materials/composites.py
 rocketsolver/models/materials/elastics.py
 rocketsolver/models/materials/metals.py
 rocketsolver/models/materials/plastics.py
-rocketsolver/models/propellants/__init__.py
-rocketsolver/models/propellants/solid.py
 rocketsolver/models/propulsion/__init__.py
 rocketsolver/models/propulsion/thermals.py
 rocketsolver/models/propulsion/grain/__init__.py
-rocketsolver/models/propulsion/grain/bates.py
-rocketsolver/models/propulsion/propellant/__init__.py
-rocketsolver/models/propulsion/propellant/solid.py
+rocketsolver/models/propulsion/grain/fmm/_2d.py
+rocketsolver/models/propulsion/grain/fmm/_3d.py
+rocketsolver/models/propulsion/grain/fmm/__init__.py
+rocketsolver/models/propulsion/grain/fmm/stl.py
+rocketsolver/models/propulsion/grain/geometries/__init__.py
+rocketsolver/models/propulsion/grain/geometries/bates.py
+rocketsolver/models/propulsion/grain/geometries/conical.py
+rocketsolver/models/propulsion/grain/geometries/d_grain.py
+rocketsolver/models/propulsion/grain/geometries/multi_port.py
+rocketsolver/models/propulsion/grain/geometries/rod_and_tube.py
+rocketsolver/models/propulsion/grain/geometries/star.py
+rocketsolver/models/propulsion/grain/geometries/wagon_wheel.py
+rocketsolver/models/propulsion/propellants/__init__.py
+rocketsolver/models/propulsion/propellants/solid.py
 rocketsolver/models/propulsion/structure/__init__.py
 rocketsolver/models/propulsion/structure/chamber.py
 rocketsolver/models/propulsion/structure/nozzle.py
 rocketsolver/models/recovery/__init__.py
 rocketsolver/models/recovery/events.py
 rocketsolver/models/recovery/parachutes.py
 rocketsolver/models/rocket/__init__.py
+rocketsolver/models/rocket/fuselage.py
 rocketsolver/montecarlo/__init__.py
 rocketsolver/montecarlo/random.py
 rocketsolver/operations/__init__.py
 rocketsolver/operations/ballistics/_1dof.py
-rocketsolver/operations/ballistics/_6dof.py
 rocketsolver/operations/ballistics/__init__.py
 rocketsolver/operations/internal_ballistics/__init__.py
+rocketsolver/services/conversions.py
+rocketsolver/services/decorators.py
+rocketsolver/services/equations.py
+rocketsolver/services/factories.py
+rocketsolver/services/isentropic_flow.py
+rocketsolver/services/common/plots.py
+rocketsolver/services/common/utilities.py
+rocketsolver/services/math/geometric.py
 rocketsolver/simulations/__init__.py
 rocketsolver/simulations/ballistics.py
-rocketsolver/simulations/ballistics_6dof.py
 rocketsolver/simulations/internal_balistics_coupled.py
 rocketsolver/simulations/internal_ballistics.py
-rocketsolver/simulations/structural.py
-rocketsolver/solvers/__init__.py
-rocketsolver/solvers/ballistics_1d.py
-rocketsolver/solvers/ballistics_6d.py
-rocketsolver/solvers/srm_internal_ballistics.py
-rocketsolver/utils/__init__.py
-rocketsolver/utils/classes.py
-rocketsolver/utils/geometric.py
-rocketsolver/utils/isentropic_flow.py
-rocketsolver/utils/math.py
-rocketsolver/utils/odes.py
-rocketsolver/utils/plots.py
-rocketsolver/utils/strings.py
-rocketsolver/utils/units.py
-rocketsolver/utils/utilities.py
+rocketsolver/solvers/odes.py
```

