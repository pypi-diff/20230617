# Comparing `tmp/carpy-0.0.1.tar.gz` & `tmp/carpy-0.0.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carpy-0.0.1.tar", last modified: Sat Jun 17 11:03:14 2023, max compression
+gzip compressed data, was "carpy-0.0.1.post1.tar", last modified: Sat Jun 17 11:48:43 2023, max compression
```

## Comparing `carpy-0.0.1.tar` & `carpy-0.0.1.post1.tar`

### file list

```diff
@@ -1,63 +1,75 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 11:03:14.605145 carpy-0.0.1/
--rw-rw-rw-   0        0        0    35823 2023-06-17 10:48:43.000000 carpy-0.0.1/LICENSE
--rw-rw-rw-   0        0        0    35821 2023-06-17 10:48:43.000000 carpy-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0       69 2023-06-17 10:48:43.000000 carpy-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0    46703 2023-06-17 11:03:14.606543 carpy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4848 2023-06-17 10:48:43.000000 carpy-0.0.1/README.md
--rw-rw-rw-   0        0        0     1116 2023-06-17 10:55:36.000000 carpy-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      237 2023-06-17 10:48:43.000000 carpy-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0      199 2023-06-17 11:03:14.618543 carpy-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      147 2023-06-17 10:48:43.000000 carpy-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 11:03:14.246213 carpy-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-17 11:03:14.265170 carpy-0.0.1/src/carpy/
--rw-rw-rw-   0        0        0     2117 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 11:03:14.325942 carpy-0.0.1/src/carpy/aerodynamics/
--rw-rw-rw-   0        0        0      121 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/aerodynamics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 11:03:14.330066 carpy-0.0.1/src/carpy/aerodynamics/aerofoil/
--rw-rw-rw-   0        0        0      103 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/aerodynamics/aerofoil/__init__.py
--rw-rw-rw-   0        0        0    27735 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/aerodynamics/aerofoil/_profiles.py
-drwxrwxrwx   0        0        0        0 2023-06-17 11:03:14.332478 carpy-0.0.1/src/carpy/aerodynamics/fuselage/
--rw-rw-rw-   0        0        0       75 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/aerodynamics/fuselage/__init__.py
--rw-rw-rw-   0        0        0     1113 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/aerodynamics/fuselage/_geometry3d.py
-drwxrwxrwx   0        0        0        0 2023-06-17 11:03:14.338293 carpy-0.0.1/src/carpy/aerodynamics/wing/
--rw-rw-rw-   0        0        0      136 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/aerodynamics/wing/__init__.py
--rw-rw-rw-   0        0        0     7366 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/aerodynamics/wing/_geometry3d.py
--rw-rw-rw-   0        0        0    22688 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/aerodynamics/wing/_planforms.py
-drwxrwxrwx   0        0        0        0 2023-06-17 11:03:14.357395 carpy-0.0.1/src/carpy/environment/
--rw-rw-rw-   0        0        0      133 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/environment/__init__.py
--rw-rw-rw-   0        0        0    24925 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/environment/_atmospheres.py
--rw-rw-rw-   0        0        0     4104 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/environment/_weather.py
-drwxrwxrwx   0        0        0        0 2023-06-17 11:03:14.455681 carpy-0.0.1/src/carpy/gaskinetics/
--rw-rw-rw-   0        0        0      149 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/gaskinetics/__init__.py
--rw-rw-rw-   0        0        0    12264 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/gaskinetics/_chemistry_elements.py
--rw-rw-rw-   0        0        0    27557 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/gaskinetics/_chemistry_molecules.py
--rw-rw-rw-   0        0        0    39190 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/gaskinetics/_dynamics_ideal.py
--rw-rw-rw-   0        0        0    17672 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/gaskinetics/_equations_of_state.py
-drwxrwxrwx   0        0        0        0 2023-06-17 11:03:14.471075 carpy-0.0.1/src/carpy/propulsion/
--rw-rw-rw-   0        0        0        0 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/propulsion/__init__.py
--rw-rw-rw-   0        0        0     1863 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/propulsion/_network.py
-drwxrwxrwx   0        0        0        0 2023-06-17 11:03:14.477746 carpy-0.0.1/src/carpy/propulsion/components/
--rw-rw-rw-   0        0        0        0 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/propulsion/components/__init__.py
--rw-rw-rw-   0        0        0     7691 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/propulsion/components/_common.py
--rw-rw-rw-   0        0        0      920 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/propulsion/components/_power_raise.py
-drwxrwxrwx   0        0        0        0 2023-06-17 11:03:14.590588 carpy-0.0.1/src/carpy/utility/
--rw-rw-rw-   0        0        0      221 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/utility/__init__.py
--rw-rw-rw-   0        0        0    16027 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/utility/_constants.py
--rw-rw-rw-   0        0        0     9813 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/utility/_graphtheory.py
--rw-rw-rw-   0        0        0     3203 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/utility/_maths.py
--rw-rw-rw-   0        0        0     6132 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/utility/_miscellaneous.py
--rw-rw-rw-   0        0        0    25752 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/utility/_unitconversion.py
--rw-rw-rw-   0        0        0     6375 2023-06-17 10:48:43.000000 carpy-0.0.1/src/carpy/utility/_vanity.py
-drwxrwxrwx   0        0        0        0 2023-06-17 11:03:14.311757 carpy-0.0.1/src/carpy.egg-info/
--rw-rw-rw-   0        0        0    46703 2023-06-17 11:03:14.000000 carpy-0.0.1/src/carpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1567 2023-06-17 11:03:14.000000 carpy-0.0.1/src/carpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 11:03:14.000000 carpy-0.0.1/src/carpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      150 2023-06-17 11:03:14.000000 carpy-0.0.1/src/carpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-17 11:03:14.000000 carpy-0.0.1/src/carpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-17 11:03:14.604123 carpy-0.0.1/tests/
--rw-rw-rw-   0        0        0     2970 2023-06-17 10:55:36.000000 carpy-0.0.1/tests/test_aerodynamics_wing.py
--rw-rw-rw-   0        0        0     1643 2023-06-17 10:55:36.000000 carpy-0.0.1/tests/test_environment_atmospheres.py
--rw-rw-rw-   0        0        0      412 2023-06-17 10:55:36.000000 carpy-0.0.1/tests/test_environment_weather.py
--rw-rw-rw-   0        0        0     4122 2023-06-17 10:55:36.000000 carpy-0.0.1/tests/test_utility_miscellaneous.py
--rw-rw-rw-   0        0        0     2275 2023-06-17 10:55:36.000000 carpy-0.0.1/tests/test_utility_unitconversion.py
--rw-rw-rw-   0        0        0     1027 2023-06-17 10:55:36.000000 carpy-0.0.1/tests/test_utility_vanity.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:48:43.627377 carpy-0.0.1.post1/
+-rw-rw-rw-   0        0        0    35823 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/LICENSE
+-rw-rw-rw-   0        0        0    35821 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/LICENSE.md
+-rw-rw-rw-   0        0        0       69 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/MANIFEST.in
+-rw-rw-rw-   0        0        0    46709 2023-06-17 11:48:43.629972 carpy-0.0.1.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     4848 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/README.md
+-rw-rw-rw-   0        0        0     1239 2023-06-17 11:37:36.000000 carpy-0.0.1.post1/pyproject.toml
+-rw-rw-rw-   0        0        0      237 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/requirements.txt
+-rw-rw-rw-   0        0        0      199 2023-06-17 11:48:43.639040 carpy-0.0.1.post1/setup.cfg
+-rw-rw-rw-   0        0        0      147 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:48:43.508975 carpy-0.0.1.post1/src/
+drwxrwxrwx   0        0        0        0 2023-06-17 11:48:43.526367 carpy-0.0.1.post1/src/carpy/
+-rw-rw-rw-   0        0        0     2119 2023-06-17 11:48:19.000000 carpy-0.0.1.post1/src/carpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:48:43.565160 carpy-0.0.1.post1/src/carpy/aerodynamics/
+-rw-rw-rw-   0        0        0      121 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/aerodynamics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:48:43.568044 carpy-0.0.1.post1/src/carpy/aerodynamics/aerofoil/
+-rw-rw-rw-   0        0        0      103 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/aerodynamics/aerofoil/__init__.py
+-rw-rw-rw-   0        0        0    27735 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/aerodynamics/aerofoil/_profiles.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:48:43.570515 carpy-0.0.1.post1/src/carpy/aerodynamics/fuselage/
+-rw-rw-rw-   0        0        0       75 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/aerodynamics/fuselage/__init__.py
+-rw-rw-rw-   0        0        0     1113 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/aerodynamics/fuselage/_geometry3d.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:48:43.574217 carpy-0.0.1.post1/src/carpy/aerodynamics/wing/
+-rw-rw-rw-   0        0        0      136 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/aerodynamics/wing/__init__.py
+-rw-rw-rw-   0        0        0     7366 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/aerodynamics/wing/_geometry3d.py
+-rw-rw-rw-   0        0        0    22688 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/aerodynamics/wing/_planforms.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:48:43.578983 carpy-0.0.1.post1/src/carpy/environment/
+-rw-rw-rw-   0        0        0      133 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/environment/__init__.py
+-rw-rw-rw-   0        0        0    24925 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/environment/_atmospheres.py
+-rw-rw-rw-   0        0        0     4104 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/environment/_weather.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:48:43.584321 carpy-0.0.1.post1/src/carpy/environment/data/
+-rw-rw-rw-   0        0        0     8901 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/environment/data/1954-ICAO.xlsx
+-rw-rw-rw-   0        0        0    14794 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/environment/data/1976-US_standard.xlsx
+-rw-rw-rw-   0        0        0     8702 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/environment/data/ISO-2533-1975.xlsx
+-rw-rw-rw-   0        0        0    59087 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/environment/data/MIL-HDBK-310_profiles.xlsx
+drwxrwxrwx   0        0        0        0 2023-06-17 11:48:43.590494 carpy-0.0.1.post1/src/carpy/gaskinetics/
+-rw-rw-rw-   0        0        0      149 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/gaskinetics/__init__.py
+-rw-rw-rw-   0        0        0    12264 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/gaskinetics/_chemistry_elements.py
+-rw-rw-rw-   0        0        0    27557 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/gaskinetics/_chemistry_molecules.py
+-rw-rw-rw-   0        0        0    39190 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/gaskinetics/_dynamics_ideal.py
+-rw-rw-rw-   0        0        0    17672 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/gaskinetics/_equations_of_state.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:48:43.596699 carpy-0.0.1.post1/src/carpy/gaskinetics/data/
+-rw-rw-rw-   0        0        0      772 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/gaskinetics/data/bond_forceconstants.yaml
+-rw-rw-rw-   0        0        0     2131 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/gaskinetics/data/bond_lengths.yaml
+-rw-rw-rw-   0        0        0     2098 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/gaskinetics/data/bond_strengths.yaml
+-rw-rw-rw-   0        0        0    11509 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/gaskinetics/data/molecule_criticalpoints.xlsx
+drwxrwxrwx   0        0        0        0 2023-06-17 11:48:43.599208 carpy-0.0.1.post1/src/carpy/propulsion/
+-rw-rw-rw-   0        0        0        0 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/propulsion/__init__.py
+-rw-rw-rw-   0        0        0     1863 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/propulsion/_network.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:48:43.602208 carpy-0.0.1.post1/src/carpy/propulsion/components/
+-rw-rw-rw-   0        0        0        0 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/propulsion/components/__init__.py
+-rw-rw-rw-   0        0        0     7691 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/propulsion/components/_common.py
+-rw-rw-rw-   0        0        0      920 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/propulsion/components/_power_raise.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:48:43.614155 carpy-0.0.1.post1/src/carpy/utility/
+-rw-rw-rw-   0        0        0      221 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/utility/__init__.py
+-rw-rw-rw-   0        0        0    16027 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/utility/_constants.py
+-rw-rw-rw-   0        0        0     9813 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/utility/_graphtheory.py
+-rw-rw-rw-   0        0        0     3203 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/utility/_maths.py
+-rw-rw-rw-   0        0        0     6132 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/utility/_miscellaneous.py
+-rw-rw-rw-   0        0        0    25752 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/utility/_unitconversion.py
+-rw-rw-rw-   0        0        0     6375 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/utility/_vanity.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:48:43.615663 carpy-0.0.1.post1/src/carpy/utility/data/
+-rw-rw-rw-   0        0        0    22170 2023-06-17 10:48:43.000000 carpy-0.0.1.post1/src/carpy/utility/data/quantities.xlsx
+drwxrwxrwx   0        0        0        0 2023-06-17 11:48:43.563659 carpy-0.0.1.post1/src/carpy.egg-info/
+-rw-rw-rw-   0        0        0    46709 2023-06-17 11:48:43.000000 carpy-0.0.1.post1/src/carpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1997 2023-06-17 11:48:43.000000 carpy-0.0.1.post1/src/carpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 11:48:43.000000 carpy-0.0.1.post1/src/carpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      150 2023-06-17 11:48:43.000000 carpy-0.0.1.post1/src/carpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-17 11:48:43.000000 carpy-0.0.1.post1/src/carpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 11:48:43.625877 carpy-0.0.1.post1/tests/
+-rw-rw-rw-   0        0        0     2970 2023-06-17 10:55:36.000000 carpy-0.0.1.post1/tests/test_aerodynamics_wing.py
+-rw-rw-rw-   0        0        0     1643 2023-06-17 10:55:36.000000 carpy-0.0.1.post1/tests/test_environment_atmospheres.py
+-rw-rw-rw-   0        0        0      412 2023-06-17 10:55:36.000000 carpy-0.0.1.post1/tests/test_environment_weather.py
+-rw-rw-rw-   0        0        0     4122 2023-06-17 10:55:36.000000 carpy-0.0.1.post1/tests/test_utility_miscellaneous.py
+-rw-rw-rw-   0        0        0     2275 2023-06-17 10:55:36.000000 carpy-0.0.1.post1/tests/test_utility_unitconversion.py
+-rw-rw-rw-   0        0        0     1027 2023-06-17 10:55:36.000000 carpy-0.0.1.post1/tests/test_utility_vanity.py
```

### Comparing `carpy-0.0.1/LICENSE` & `carpy-0.0.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/LICENSE.md` & `carpy-0.0.1.post1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/PKG-INFO` & `carpy-0.0.1.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carpy
-Version: 0.0.1
+Version: 0.0.1.post1
 Summary: Consolidated aircraft recipes in Python.
 Author-email: Yaseen Reza <yaseen605@gmail.com>, Luana Defourny <luanadefourny@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `carpy-0.0.1/README.md` & `carpy-0.0.1.post1/README.md`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/pyproject.toml` & `carpy-0.0.1.post1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -40,7 +40,13 @@
 
 [project.urls]
 homepage = "https://github.com/yaseen157/carpy"
 documentation = "https://pypi.org/project/carpy/"
 
 [tool.setuptools.dynamic]
 version = {attr = "carpy.__version__"}
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
+[tool.setuptools.package-data]
+"*" = ["*.csv", "*.xlsx", "*.yaml"]
```

### Comparing `carpy-0.0.1/src/carpy/__init__.py` & `carpy-0.0.1.post1/src/carpy/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 information, examples, and tutorials on usage.
 
 carpy is distributed under the GNU GPLv3 License. A full copy of the license
 should be present alongside the source code on GitHub.
 """
 # The version number of the "entire" package is specified here (for now).
 # In future, the idea would be this is tied to the git release (somehow).
-__version__ = "0.0.1"
+__version__ = "0.0.1-1"
 
 # ============================================================================ #
 # -------------------------------- LICENSING --------------------------------- #
 # ============================================================================ #
 __license__ = "GNU GPLv3"
 # Console interaction copyright notice
 __copyright__ = (
```

### Comparing `carpy-0.0.1/src/carpy/aerodynamics/aerofoil/_profiles.py` & `carpy-0.0.1.post1/src/carpy/aerodynamics/aerofoil/_profiles.py`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/src/carpy/aerodynamics/fuselage/_geometry3d.py` & `carpy-0.0.1.post1/src/carpy/aerodynamics/fuselage/_geometry3d.py`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/src/carpy/aerodynamics/wing/_geometry3d.py` & `carpy-0.0.1.post1/src/carpy/aerodynamics/wing/_geometry3d.py`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/src/carpy/aerodynamics/wing/_planforms.py` & `carpy-0.0.1.post1/src/carpy/aerodynamics/wing/_planforms.py`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/src/carpy/environment/_atmospheres.py` & `carpy-0.0.1.post1/src/carpy/environment/_atmospheres.py`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/src/carpy/environment/_weather.py` & `carpy-0.0.1.post1/src/carpy/environment/_weather.py`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/src/carpy/gaskinetics/_chemistry_elements.py` & `carpy-0.0.1.post1/src/carpy/gaskinetics/_chemistry_elements.py`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/src/carpy/gaskinetics/_chemistry_molecules.py` & `carpy-0.0.1.post1/src/carpy/gaskinetics/_chemistry_molecules.py`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/src/carpy/gaskinetics/_dynamics_ideal.py` & `carpy-0.0.1.post1/src/carpy/gaskinetics/_dynamics_ideal.py`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/src/carpy/gaskinetics/_equations_of_state.py` & `carpy-0.0.1.post1/src/carpy/gaskinetics/_equations_of_state.py`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/src/carpy/propulsion/_network.py` & `carpy-0.0.1.post1/src/carpy/propulsion/_network.py`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/src/carpy/propulsion/components/_common.py` & `carpy-0.0.1.post1/src/carpy/propulsion/components/_common.py`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/src/carpy/propulsion/components/_power_raise.py` & `carpy-0.0.1.post1/src/carpy/propulsion/components/_power_raise.py`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/src/carpy/utility/_constants.py` & `carpy-0.0.1.post1/src/carpy/utility/_constants.py`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/src/carpy/utility/_graphtheory.py` & `carpy-0.0.1.post1/src/carpy/utility/_graphtheory.py`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/src/carpy/utility/_maths.py` & `carpy-0.0.1.post1/src/carpy/utility/_maths.py`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/src/carpy/utility/_miscellaneous.py` & `carpy-0.0.1.post1/src/carpy/utility/_miscellaneous.py`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/src/carpy/utility/_unitconversion.py` & `carpy-0.0.1.post1/src/carpy/utility/_unitconversion.py`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/src/carpy/utility/_vanity.py` & `carpy-0.0.1.post1/src/carpy/utility/_vanity.py`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/src/carpy.egg-info/PKG-INFO` & `carpy-0.0.1.post1/src/carpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carpy
-Version: 0.0.1
+Version: 0.0.1.post1
 Summary: Consolidated aircraft recipes in Python.
 Author-email: Yaseen Reza <yaseen605@gmail.com>, Luana Defourny <luanadefourny@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `carpy-0.0.1/tests/test_aerodynamics_wing.py` & `carpy-0.0.1.post1/tests/test_aerodynamics_wing.py`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/tests/test_environment_atmospheres.py` & `carpy-0.0.1.post1/tests/test_environment_atmospheres.py`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/tests/test_utility_miscellaneous.py` & `carpy-0.0.1.post1/tests/test_utility_miscellaneous.py`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/tests/test_utility_unitconversion.py` & `carpy-0.0.1.post1/tests/test_utility_unitconversion.py`

 * *Files identical despite different names*

### Comparing `carpy-0.0.1/tests/test_utility_vanity.py` & `carpy-0.0.1.post1/tests/test_utility_vanity.py`

 * *Files identical despite different names*

