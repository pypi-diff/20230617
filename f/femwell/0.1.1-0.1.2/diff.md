# Comparing `tmp/femwell-0.1.1.tar.gz` & `tmp/femwell-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "femwell-0.1.1.tar", max compression
+gzip compressed data, was "femwell-0.1.2.tar", max compression
```

## Comparing `femwell-0.1.1.tar` & `femwell-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    35149 2023-06-16 21:17:55.657797 femwell-0.1.1/LICENSE
--rw-r--r--   0        0        0     2480 2023-06-16 21:17:55.657797 femwell-0.1.1/README.md
--rw-r--r--   0        0        0      255 2023-06-16 21:17:55.657797 femwell-0.1.1/femwell/__init__.py
--rw-r--r--   0        0        0     3080 2023-06-16 21:17:55.657797 femwell-0.1.1/femwell/culomb.py
--rw-r--r--   0        0        0    10175 2023-06-16 21:17:55.657797 femwell-0.1.1/femwell/eme.py.bak
--rw-r--r--   0        0        0        0 2023-06-16 21:17:55.657797 femwell-0.1.1/femwell/examples/__init__.py
--rw-r--r--   0        0        0     4820 2023-06-16 21:17:55.657797 femwell-0.1.1/femwell/examples/coplanar_waveguide.py
--rw-r--r--   0        0        0     5762 2023-06-16 21:17:55.657797 femwell-0.1.1/femwell/fefd.py
--rw-r--r--   0        0        0     1304 2023-06-16 21:17:55.657797 femwell-0.1.1/femwell/fiber.py
--rw-r--r--   0        0        0     1782 2023-06-16 21:17:55.657797 femwell-0.1.1/femwell/laplace.py
--rw-r--r--   0        0        0    17327 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/maxwell/waveguide.py
--rw-r--r--   0        0        0      224 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/mesh/__init__.py
--rw-r--r--   0        0        0    26893 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/mesh/mesh.py
--rw-r--r--   0        0        0     7713 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/mesh/meshtracker.py
--rw-r--r--   0        0        0     9318 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/mesh/slice.py
--rw-r--r--   0        0        0    21359 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/mesh.py
--rw-r--r--   0        0        0     1033 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/mode_solver_1d.py
--rw-r--r--   0        0        0     2922 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/mode_solver_2d_periodic.py
--rw-r--r--   0        0        0     6950 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/mode_solver_2d_periodic_quadratic.py
--rw-r--r--   0        0        0     4224 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/mode_solver_inplane.py
--rw-r--r--   0        0        0     1243 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/mode_solver_schrodinger.py
--rw-r--r--   0        0        0     8799 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/pn_analytical.py
--rw-r--r--   0        0        0     6453 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/solver.py
--rw-r--r--   0        0        0     5897 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/tcad.py
--rw-r--r--   0        0        0     2820 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/tests/test_mesh.py
--rw-r--r--   0        0        0     5880 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/thermal.py
--rw-r--r--   0        0        0     8803 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/thermal_transient.py
--rw-r--r--   0        0        0     2655 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/utils.py
--rw-r--r--   0        0        0     1123 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/visualization.py
--rw-r--r--   0        0        0     2089 2023-06-16 21:17:55.661797 femwell-0.1.1/femwell/waveguide.py
--rw-r--r--   0        0        0      974 2023-06-16 21:18:06.821815 femwell-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3482 1970-01-01 00:00:00.000000 femwell-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-17 06:40:05.912416 femwell-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2480 2023-06-17 06:40:05.912416 femwell-0.1.2/README.md
+-rw-r--r--   0        0        0      255 2023-06-17 06:40:05.916416 femwell-0.1.2/femwell/__init__.py
+-rw-r--r--   0        0        0     3080 2023-06-17 06:40:05.916416 femwell-0.1.2/femwell/culomb.py
+-rw-r--r--   0        0        0    10175 2023-06-17 06:40:05.916416 femwell-0.1.2/femwell/eme.py.bak
+-rw-r--r--   0        0        0        0 2023-06-17 06:40:05.916416 femwell-0.1.2/femwell/examples/__init__.py
+-rw-r--r--   0        0        0     4820 2023-06-17 06:40:05.916416 femwell-0.1.2/femwell/examples/coplanar_waveguide.py
+-rw-r--r--   0        0        0     5762 2023-06-17 06:40:05.916416 femwell-0.1.2/femwell/fefd.py
+-rw-r--r--   0        0        0     1304 2023-06-17 06:40:05.916416 femwell-0.1.2/femwell/fiber.py
+-rw-r--r--   0        0        0     1782 2023-06-17 06:40:05.916416 femwell-0.1.2/femwell/laplace.py
+-rw-r--r--   0        0        0    17333 2023-06-17 06:40:05.916416 femwell-0.1.2/femwell/maxwell/waveguide.py
+-rw-r--r--   0        0        0      224 2023-06-17 06:40:05.916416 femwell-0.1.2/femwell/mesh/__init__.py
+-rw-r--r--   0        0        0    26893 2023-06-17 06:40:05.916416 femwell-0.1.2/femwell/mesh/mesh.py
+-rw-r--r--   0        0        0     7713 2023-06-17 06:40:05.916416 femwell-0.1.2/femwell/mesh/meshtracker.py
+-rw-r--r--   0        0        0     9318 2023-06-17 06:40:05.916416 femwell-0.1.2/femwell/mesh/slice.py
+-rw-r--r--   0        0        0    21359 2023-06-17 06:40:05.916416 femwell-0.1.2/femwell/mesh.py
+-rw-r--r--   0        0        0     1033 2023-06-17 06:40:05.916416 femwell-0.1.2/femwell/mode_solver_1d.py
+-rw-r--r--   0        0        0     2922 2023-06-17 06:40:05.916416 femwell-0.1.2/femwell/mode_solver_2d_periodic.py
+-rw-r--r--   0        0        0     6950 2023-06-17 06:40:05.916416 femwell-0.1.2/femwell/mode_solver_2d_periodic_quadratic.py
+-rw-r--r--   0        0        0     4224 2023-06-17 06:40:05.920416 femwell-0.1.2/femwell/mode_solver_inplane.py
+-rw-r--r--   0        0        0     1243 2023-06-17 06:40:05.920416 femwell-0.1.2/femwell/mode_solver_schrodinger.py
+-rw-r--r--   0        0        0     8799 2023-06-17 06:40:05.920416 femwell-0.1.2/femwell/pn_analytical.py
+-rw-r--r--   0        0        0     6453 2023-06-17 06:40:05.920416 femwell-0.1.2/femwell/solver.py
+-rw-r--r--   0        0        0     5897 2023-06-17 06:40:05.920416 femwell-0.1.2/femwell/tcad.py
+-rw-r--r--   0        0        0     2820 2023-06-17 06:40:05.920416 femwell-0.1.2/femwell/tests/test_mesh.py
+-rw-r--r--   0        0        0     5880 2023-06-17 06:40:05.920416 femwell-0.1.2/femwell/thermal.py
+-rw-r--r--   0        0        0     8803 2023-06-17 06:40:05.920416 femwell-0.1.2/femwell/thermal_transient.py
+-rw-r--r--   0        0        0     2655 2023-06-17 06:40:05.920416 femwell-0.1.2/femwell/utils.py
+-rw-r--r--   0        0        0     1123 2023-06-17 06:40:05.920416 femwell-0.1.2/femwell/visualization.py
+-rw-r--r--   0        0        0     2089 2023-06-17 06:40:05.920416 femwell-0.1.2/femwell/waveguide.py
+-rw-r--r--   0        0        0      974 2023-06-17 06:40:26.396478 femwell-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3482 1970-01-01 00:00:00.000000 femwell-0.1.2/PKG-INFO
```

### Comparing `femwell-0.1.1/LICENSE` & `femwell-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/README.md` & `femwell-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/culomb.py` & `femwell-0.1.2/femwell/culomb.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/eme.py.bak` & `femwell-0.1.2/femwell/eme.py.bak`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/examples/coplanar_waveguide.py` & `femwell-0.1.2/femwell/examples/coplanar_waveguide.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/fefd.py` & `femwell-0.1.2/femwell/fefd.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/fiber.py` & `femwell-0.1.2/femwell/fiber.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/laplace.py` & `femwell-0.1.2/femwell/laplace.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/maxwell/waveguide.py` & `femwell-0.1.2/femwell/maxwell/waveguide.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
 
     A = aform.assemble(basis, epsilon=basis_epsilon_r.interpolate(epsilon_r))
     B = bform.assemble(basis, epsilon=basis_epsilon_r.interpolate(epsilon_r))
 
     if n_guess:
         sigma = sigma = k0**2 * n_guess**2
     else:
-        sigma = sigma = k0**2 * np.max(epsilon_r)
+        sigma = sigma = k0**2 * np.max(epsilon_r) * 1.1
 
     if metallic_boundaries:
         lams, xs = solve(
             *condense(
                 -A,
                 -B,
                 D=basis.get_dofs(None if metallic_boundaries is True else metallic_boundaries),
```

### Comparing `femwell-0.1.1/femwell/mesh/mesh.py` & `femwell-0.1.2/femwell/mesh/mesh.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/mesh/meshtracker.py` & `femwell-0.1.2/femwell/mesh/meshtracker.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/mesh/slice.py` & `femwell-0.1.2/femwell/mesh/slice.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/mesh.py` & `femwell-0.1.2/femwell/mesh.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/mode_solver_1d.py` & `femwell-0.1.2/femwell/mode_solver_1d.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/mode_solver_2d_periodic.py` & `femwell-0.1.2/femwell/mode_solver_2d_periodic.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/mode_solver_2d_periodic_quadratic.py` & `femwell-0.1.2/femwell/mode_solver_2d_periodic_quadratic.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/mode_solver_inplane.py` & `femwell-0.1.2/femwell/mode_solver_inplane.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/mode_solver_schrodinger.py` & `femwell-0.1.2/femwell/mode_solver_schrodinger.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/pn_analytical.py` & `femwell-0.1.2/femwell/pn_analytical.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/solver.py` & `femwell-0.1.2/femwell/solver.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/tcad.py` & `femwell-0.1.2/femwell/tcad.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/tests/test_mesh.py` & `femwell-0.1.2/femwell/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/thermal.py` & `femwell-0.1.2/femwell/thermal.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/thermal_transient.py` & `femwell-0.1.2/femwell/thermal_transient.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/utils.py` & `femwell-0.1.2/femwell/utils.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/visualization.py` & `femwell-0.1.2/femwell/visualization.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/femwell/waveguide.py` & `femwell-0.1.2/femwell/waveguide.py`

 * *Files identical despite different names*

### Comparing `femwell-0.1.1/pyproject.toml` & `femwell-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "femwell"
-version = "0.1.1"
+version = "0.1.2"
 authors = ["Helge Gehring"]
 description = "Mode solver for photonic and electric waveguides based on FEM"
 homepage = "https://github.com/HelgeGehring/femwell"
 keywords = [
     "integrated photonics",
     "silicon photonics",
     "mode solving",
```

### Comparing `femwell-0.1.1/PKG-INFO` & `femwell-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: femwell
-Version: 0.1.1
+Version: 0.1.2
 Summary: Mode solver for photonic and electric waveguides based on FEM
 Home-page: https://github.com/HelgeGehring/femwell
 License: GPLv3
 Keywords: integrated photonics,silicon photonics,mode solving,finite element analysis
 Author: Helge Gehring
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
```

