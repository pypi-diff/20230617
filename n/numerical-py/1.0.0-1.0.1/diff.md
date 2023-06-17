# Comparing `tmp/numerical_py-1.0.0.tar.gz` & `tmp/numerical_py-1.0.1.linux-x86_64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numerical_py-1.0.0.tar", last modified: Thu Jun 15 23:24:55 2023, max compression
+gzip compressed data, was "numerical_py-1.0.1.linux-x86_64.tar", last modified: Sat Jun 17 09:06:38 2023, max compression
```

## Comparing `numerical_py-1.0.0.tar` & `numerical_py-1.0.1.linux-x86_64.tar`

### file list

```diff
@@ -1,18 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 23:24:55.410183 numerical_py-1.0.0/
--rw-rw-rw-   0        0        0      144 2023-06-15 23:24:55.399184 numerical_py-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 23:24:55.392184 numerical_py-1.0.0/numerical_py/
--rw-rw-rw-   0        0        0      277 2023-06-15 23:19:21.000000 numerical_py-1.0.0/numerical_py/__init__.py
--rw-rw-rw-   0        0        0     1426 2023-06-15 21:14:08.000000 numerical_py-1.0.0/numerical_py/derivative.py
--rw-rw-rw-   0        0        0     1126 2023-06-15 21:13:57.000000 numerical_py-1.0.0/numerical_py/differentional.py
--rw-rw-rw-   0        0        0     1533 2023-06-15 21:59:45.000000 numerical_py-1.0.0/numerical_py/eigenvals.py
--rw-rw-rw-   0        0        0     5994 2023-06-15 23:23:32.000000 numerical_py-1.0.0/numerical_py/equations.py
--rw-rw-rw-   0        0        0     3763 2023-06-15 21:59:48.000000 numerical_py-1.0.0/numerical_py/integrals.py
--rw-rw-rw-   0        0        0     1589 2023-06-15 22:35:42.000000 numerical_py-1.0.0/numerical_py/interpolation.py
--rw-rw-rw-   0        0        0        0 2023-06-15 13:55:38.000000 numerical_py-1.0.0/numerical_py/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-15 23:24:55.399184 numerical_py-1.0.0/numerical_py.egg-info/
--rw-rw-rw-   0        0        0      144 2023-06-15 23:24:55.000000 numerical_py-1.0.0/numerical_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2023-06-15 23:24:55.000000 numerical_py-1.0.0/numerical_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 23:24:55.000000 numerical_py-1.0.0/numerical_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-15 23:24:55.000000 numerical_py-1.0.0/numerical_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 23:24:55.411185 numerical_py-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      240 2023-06-15 23:24:44.000000 numerical_py-1.0.0/setup.py
+drwxr-xr-x   0 ivannewest  (1000) ivannewest  (1000)        0 2023-06-17 09:06:37.018392 ./
+drwxr-xr-x   0 ivannewest  (1000) ivannewest  (1000)        0 2023-06-17 09:06:37.022392 ./home/
+drwxr-xr-x   0 ivannewest  (1000) ivannewest  (1000)        0 2023-06-17 09:06:37.022392 ./home/ivannewest/
+drwxr-xr-x   0 ivannewest  (1000) ivannewest  (1000)        0 2023-06-17 09:06:37.022392 ./home/ivannewest/anaconda3/
+drwxr-xr-x   0 ivannewest  (1000) ivannewest  (1000)        0 2023-06-17 09:06:37.022392 ./home/ivannewest/anaconda3/lib/
+drwxr-xr-x   0 ivannewest  (1000) ivannewest  (1000)        0 2023-06-17 09:06:37.022392 ./home/ivannewest/anaconda3/lib/python3.10/
+drwxr-xr-x   0 ivannewest  (1000) ivannewest  (1000)        0 2023-06-17 09:06:37.814396 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/
+drwxr-xr-x   0 ivannewest  (1000) ivannewest  (1000)        0 2023-06-17 09:06:37.030392 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py/
+-rw-r--r--   0 ivannewest  (1000) ivannewest  (1000)      271 2023-06-17 09:00:32.000000 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py/__init__.py
+drwxr-xr-x   0 ivannewest  (1000) ivannewest  (1000)        0 2023-06-17 09:06:37.034392 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py/__pycache__/
+-rw-r--r--   0 ivannewest  (1000) ivannewest  (1000)      522 2023-06-17 09:06:37.034392 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 ivannewest  (1000) ivannewest  (1000)     2364 2023-06-17 09:06:37.034392 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py/__pycache__/derivative.cpython-310.pyc
+-rw-r--r--   0 ivannewest  (1000) ivannewest  (1000)     1948 2023-06-17 09:06:37.034392 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py/__pycache__/differentional.cpython-310.pyc
+-rw-r--r--   0 ivannewest  (1000) ivannewest  (1000)     1836 2023-06-17 09:06:37.034392 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py/__pycache__/eigenvals.cpython-310.pyc
+-rw-r--r--   0 ivannewest  (1000) ivannewest  (1000)     5864 2023-06-17 09:06:37.030392 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py/__pycache__/equations.cpython-310.pyc
+-rw-r--r--   0 ivannewest  (1000) ivannewest  (1000)     3680 2023-06-17 09:06:37.030392 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py/__pycache__/integrals.cpython-310.pyc
+-rw-r--r--   0 ivannewest  (1000) ivannewest  (1000)     2498 2023-06-17 09:06:37.034392 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py/__pycache__/interpolation.cpython-310.pyc
+-rw-r--r--   0 ivannewest  (1000) ivannewest  (1000)      170 2023-06-17 09:06:37.030392 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 ivannewest  (1000) ivannewest  (1000)     1384 2023-06-17 09:00:32.000000 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py/derivative.py
+-rw-r--r--   0 ivannewest  (1000) ivannewest  (1000)     1520 2023-06-17 09:01:18.000000 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py/differentional.py
+-rw-r--r--   0 ivannewest  (1000) ivannewest  (1000)     1487 2023-06-17 09:00:32.000000 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py/eigenvals.py
+-rw-r--r--   0 ivannewest  (1000) ivannewest  (1000)     5833 2023-06-17 09:00:32.000000 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py/equations.py
+-rw-r--r--   0 ivannewest  (1000) ivannewest  (1000)     3646 2023-06-17 09:00:32.000000 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py/integrals.py
+-rw-r--r--   0 ivannewest  (1000) ivannewest  (1000)     1541 2023-06-17 09:00:32.000000 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py/interpolation.py
+-rw-r--r--   0 ivannewest  (1000) ivannewest  (1000)        0 2023-06-17 09:00:32.000000 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py/utils.py
+drwxr-xr-x   0 ivannewest  (1000) ivannewest  (1000)        0 2023-06-17 09:06:37.818396 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py-1.0.1-py3.10.egg-info/
+-rw-r--r--   0 ivannewest  (1000) ivannewest  (1000)      138 2023-06-17 09:06:37.778396 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py-1.0.1-py3.10.egg-info/PKG-INFO
+-rw-r--r--   0 ivannewest  (1000) ivannewest  (1000)      365 2023-06-17 09:06:37.814396 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py-1.0.1-py3.10.egg-info/SOURCES.txt
+-rw-r--r--   0 ivannewest  (1000) ivannewest  (1000)        1 2023-06-17 09:06:37.778396 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py-1.0.1-py3.10.egg-info/dependency_links.txt
+-rw-r--r--   0 ivannewest  (1000) ivannewest  (1000)       13 2023-06-17 09:06:37.782396 ./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py-1.0.1-py3.10.egg-info/top_level.txt
```

### Comparing `numerical_py-1.0.0/numerical_py/derivative.py` & `./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py/derivative.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import numpy as np
-import sympy as sp
-
-from .interpolation import Interpolate
-
-
-class Derivative:
-    def __init__(
-        self, x_values: np.ndarray, f_x_values: np.ndarray, h_val: float = 0.02
-    ) -> None:
-        self.x_values = x_values
-        self.f_x_values = f_x_values
-        self.h_val = h_val
-
-    def deriv_by_nodes(self, num_nodes: int = 4) -> float:
-        def sub_q(L):
-            x = sp.Symbol("x")
-            x0 = sp.Symbol("x0")
-            x_nodes = sp.symbols(" ".join([f"x{i}" for i in range(1, num_nodes)]))
-            h, q = sp.symbols("h q")
-            subs_dict = {
-                k: v for k, v in zip(x_nodes, [x0 + i * h for i in range(1, num_nodes)])
-            }
-            subs_dict[x] = x0 + h * q
-            return L.subs(subs_dict)
-
-        q = sp.Symbol("q")
-        h = sp.Symbol("h")
-        x0 = sp.Symbol("x0")
-        L = Interpolate(self.x_values, self.f_x_values).lagrange_polynom()
-        Ldiff = 1 / h * sub_q(L).diff(q)
-        Ldiff2 = 1 / h * Ldiff.diff(q)
-        return {
-            "first_deriv": [
-                Ldiff.subs({x0: self.x_values[0], h: self.h_val, q: i})
-                for i in range(len(self.f_x_values))
-            ],
-            "second_deriv": [
-                Ldiff2.subs({x0: self.x_values[0], h: self.h_val, q: i})
-                for i in range(len(self.f_x_values))
-            ],
-        }
+import numpy as np
+import sympy as sp
+
+from .interpolation import Interpolate
+
+
+class Derivative:
+    def __init__(
+        self, x_values: np.ndarray, f_x_values: np.ndarray, h_val: float = 0.02
+    ) -> None:
+        self.x_values = x_values
+        self.f_x_values = f_x_values
+        self.h_val = h_val
+
+    def deriv_by_nodes(self, num_nodes: int = 4) -> float:
+        def sub_q(L):
+            x = sp.Symbol("x")
+            x0 = sp.Symbol("x0")
+            x_nodes = sp.symbols(" ".join([f"x{i}" for i in range(1, num_nodes)]))
+            h, q = sp.symbols("h q")
+            subs_dict = {
+                k: v for k, v in zip(x_nodes, [x0 + i * h for i in range(1, num_nodes)])
+            }
+            subs_dict[x] = x0 + h * q
+            return L.subs(subs_dict)
+
+        q = sp.Symbol("q")
+        h = sp.Symbol("h")
+        x0 = sp.Symbol("x0")
+        L = Interpolate(self.x_values, self.f_x_values).lagrange_polynom()
+        Ldiff = 1 / h * sub_q(L).diff(q)
+        Ldiff2 = 1 / h * Ldiff.diff(q)
+        return {
+            "first_deriv": [
+                Ldiff.subs({x0: self.x_values[0], h: self.h_val, q: i})
+                for i in range(len(self.f_x_values))
+            ],
+            "second_deriv": [
+                Ldiff2.subs({x0: self.x_values[0], h: self.h_val, q: i})
+                for i in range(len(self.f_x_values))
+            ],
+        }
```

### Comparing `numerical_py-1.0.0/numerical_py/eigenvals.py` & `./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py/eigenvals.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-import numpy as np
-import sympy as sp
-from typing import Dict, List
-
-
-class Eigenvals:
-    def __init__(self, matrix: sp.Matrix) -> None:
-        assert isinstance(matrix, sp.Matrix), "Matrix must be sympy"
-        self.matrix = matrix
-
-    def direct_deployment_method(self) -> Dict[str, List[Dict[str, int]]]:
-        lam = sp.symbols("lam")
-        n = self.matrix.shape[0]
-        E = np.eye(n)
-        det = sp.det(self.matrix - lam * E)
-        lambda_ = sp.solve(det, lam)
-
-        eigenitems = []
-
-        for l in lambda_:
-            print(f"λ = {round(l, 5)} is an eigenvalue of A")
-            x = sp.Matrix(sp.symbols(f"x:{self.matrix.shape[0]}"))
-            sol = sp.solve((self.matrix - l * sp.eye(self.matrix.shape[0])) * x, x)
-            print(f"eigenvector: {sol}\n")
-            eigenitems.append({"value": l, "vector": sol})
-
-        return {"items": eigenitems}
-
-    def iteration_method(
-        self, eps: float, x0: np.matrix = np.matrix([1, 1, 1]).T
-    ) -> Dict[str, List[Dict[str, int]]]:
-        x = self.matrix @ x0
-        lambda_ = x[0, 0] / x0[0, 0]
-        k = 1
-        while True:
-            x_new = self.matrix @ x
-            lambda_new = x_new[0, 0] / x[0, 0]
-            print(f"iteration {k}: λ = {round(lambda_new, 5)}")
-            if abs(lambda_new - lambda_) < eps:
-                break
-
-            lambda_ = lambda_new
-            x = x_new
-            k += 1
-
-        return {"items": [{"value": lambda_new, "vector": x / x[0, 0]}]}
+import numpy as np
+import sympy as sp
+from typing import Dict, List
+
+
+class Eigenvals:
+    def __init__(self, matrix: sp.Matrix) -> None:
+        assert isinstance(matrix, sp.Matrix), "Matrix must be sympy"
+        self.matrix = matrix
+
+    def direct_deployment_method(self) -> Dict[str, List[Dict[str, int]]]:
+        lam = sp.symbols("lam")
+        n = self.matrix.shape[0]
+        E = np.eye(n)
+        det = sp.det(self.matrix - lam * E)
+        lambda_ = sp.solve(det, lam)
+
+        eigenitems = []
+
+        for l in lambda_:
+            print(f"λ = {round(l, 5)} is an eigenvalue of A")
+            x = sp.Matrix(sp.symbols(f"x:{self.matrix.shape[0]}"))
+            sol = sp.solve((self.matrix - l * sp.eye(self.matrix.shape[0])) * x, x)
+            print(f"eigenvector: {sol}\n")
+            eigenitems.append({"value": l, "vector": sol})
+
+        return {"items": eigenitems}
+
+    def iteration_method(
+        self, eps: float, x0: np.matrix = np.matrix([1, 1, 1]).T
+    ) -> Dict[str, List[Dict[str, int]]]:
+        x = self.matrix @ x0
+        lambda_ = x[0, 0] / x0[0, 0]
+        k = 1
+        while True:
+            x_new = self.matrix @ x
+            lambda_new = x_new[0, 0] / x[0, 0]
+            print(f"iteration {k}: λ = {round(lambda_new, 5)}")
+            if abs(lambda_new - lambda_) < eps:
+                break
+
+            lambda_ = lambda_new
+            x = x_new
+            k += 1
+
+        return {"items": [{"value": lambda_new, "vector": x / x[0, 0]}]}
```

### Comparing `numerical_py-1.0.0/numerical_py/integrals.py` & `./home/ivannewest/anaconda3/lib/python3.10/site-packages/numerical_py/integrals.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-from typing import Callable, Optional
-import sympy as sp
-import numpy as np
-
-
-class Integrate:
-    def __init__(
-        self, f: Callable, a: float, b: float, n: int, h: Optional[float] = None
-    ) -> None:
-        self.f = f
-        self.a = a
-        self.b = b
-        self.n = n
-        self.h = h
-        if h is None:
-            self.h = (self.b - self.a) / self.n
-
-    def trapezoidal_rule(self) -> float:
-        s = (self.f(self.a) + self.f(self.b)) / 2
-        for i in range(1, self.n):
-            s += self.f(self.a + i * self.h)
-        return self.h * s
-
-    def three_eights_rule(self) -> float:
-        s = self.f(self.a) + self.f(self.b)
-        for i in range(1, self.n):
-            x = self.a + i * self.h
-            if i % 3 == 0:
-                s += 2 * self.f(x)
-            else:
-                s += 3 * self.f(x)
-        return (3 * self.h / 8) * s
-
-    @staticmethod
-    def cotes_coef(i: int, m: int):
-        a, b = sp.symbols("a b")
-        formulas_dict = {
-            1: {
-                0: (b - a) / 2,
-            },
-            2: {
-                0: (b - a) / 6,
-                1: 4 * (b - a) / 6,
-            },
-            3: {
-                0: (b - a) / 8,
-                1: 3 * (b - a) / 8,
-            },
-            4: {
-                0: 7 * (b - a) / 90,
-                1: 16 * (b - a) / 45,
-                2: 2 * (b - a) / 15,
-            },
-            5: {
-                0: 19 * (b - a) / 288,
-                1: 25 * (b - a) / 96,
-                2: 25 * (b - a) / 144,
-            },
-            6: {
-                0: 41 * (b - a) / 840,
-                1: 9 * (b - a) / 35,
-                2: 9 * (b - a) / 280,
-                3: 34 * (b - a) / 105,
-            },
-        }
-        if i > m / 2:
-            return Integrate.cotes_coef(m - i, m)
-        return formulas_dict[m][i]
-
-    def cotes_rule(self, x_values: np.ndarray, f_x_values: np.ndarray) -> float:
-        a, b = sp.symbols("a b")
-        L5_integr = np.sum(
-            [
-                Integrate.cotes_coef(i, len(x_values)) * f_x_values[i]
-                for i in range(len(x_values))
-            ]
-        )
-        return L5_integr.subs({a: x_values[0], b: x_values[-1]})
-
-    def simpson_rule(self) -> float:
-        simpson_integral = 0
-
-        for step in range(self.n):
-            x1 = self.a + step * self.h
-            x2 = self.a + (step + 1) * self.h
-
-            simpson_integral += (
-                (x2 - x1)
-                / 6.0
-                * (self.f(x1) + 4.0 * self.f(0.5 * (x1 + x2)) + self.f(x2))
-            )
-
-        return simpson_integral
-
-    def rectangles_rule(self, rect_type="middle") -> float:
-        rectangles_integral = 0
-        if rect_type == "left":
-            for i in range(0, self.n):
-                x_i_plus_1 = self.a + (i + 1) * self.h
-                x_i = self.a + i * self.h
-                f_x = self.f(x_i)
-                rectangles_integral += f_x * (x_i_plus_1 - x_i)
-        elif rect_type == "right":
-            for i in range(1, self.n + 1):
-                x_i = self.a + i * self.h
-                x_i_minus_1 = self.a + (i - 1) * self.h
-                f_x = self.f(x_i)
-                rectangles_integral += f_x * (x_i - x_i_minus_1)
-        elif rect_type == "middle":
-            for i in range(0, self.n):
-                x_i = self.a + (i * self.h)
-                x_i_plus_1 = self.a + ((i + 1) * self.h)
-                f_x = self.f((x_i + x_i_plus_1) / 2)
-                rectangles_integral += f_x * (x_i_plus_1 - x_i)
-        else:
-            print("Correct options:\nleft\nright\nmiddle")
-        return rectangles_integral
+from typing import Callable, Optional
+import sympy as sp
+import numpy as np
+
+
+class Integrate:
+    def __init__(
+        self, f: Callable, a: float, b: float, n: int, h: Optional[float] = None
+    ) -> None:
+        self.f = f
+        self.a = a
+        self.b = b
+        self.n = n
+        self.h = h
+        if h is None:
+            self.h = (self.b - self.a) / self.n
+
+    def trapezoidal_rule(self) -> float:
+        s = (self.f(self.a) + self.f(self.b)) / 2
+        for i in range(1, self.n):
+            s += self.f(self.a + i * self.h)
+        return self.h * s
+
+    def three_eights_rule(self) -> float:
+        s = self.f(self.a) + self.f(self.b)
+        for i in range(1, self.n):
+            x = self.a + i * self.h
+            if i % 3 == 0:
+                s += 2 * self.f(x)
+            else:
+                s += 3 * self.f(x)
+        return (3 * self.h / 8) * s
+
+    @staticmethod
+    def cotes_coef(i: int, m: int):
+        a, b = sp.symbols("a b")
+        formulas_dict = {
+            1: {
+                0: (b - a) / 2,
+            },
+            2: {
+                0: (b - a) / 6,
+                1: 4 * (b - a) / 6,
+            },
+            3: {
+                0: (b - a) / 8,
+                1: 3 * (b - a) / 8,
+            },
+            4: {
+                0: 7 * (b - a) / 90,
+                1: 16 * (b - a) / 45,
+                2: 2 * (b - a) / 15,
+            },
+            5: {
+                0: 19 * (b - a) / 288,
+                1: 25 * (b - a) / 96,
+                2: 25 * (b - a) / 144,
+            },
+            6: {
+                0: 41 * (b - a) / 840,
+                1: 9 * (b - a) / 35,
+                2: 9 * (b - a) / 280,
+                3: 34 * (b - a) / 105,
+            },
+        }
+        if i > m / 2:
+            return Integrate.cotes_coef(m - i, m)
+        return formulas_dict[m][i]
+
+    def cotes_rule(self, x_values: np.ndarray, f_x_values: np.ndarray) -> float:
+        a, b = sp.symbols("a b")
+        L5_integr = np.sum(
+            [
+                Integrate.cotes_coef(i, len(x_values)) * f_x_values[i]
+                for i in range(len(x_values))
+            ]
+        )
+        return L5_integr.subs({a: x_values[0], b: x_values[-1]})
+
+    def simpson_rule(self) -> float:
+        simpson_integral = 0
+
+        for step in range(self.n):
+            x1 = self.a + step * self.h
+            x2 = self.a + (step + 1) * self.h
+
+            simpson_integral += (
+                (x2 - x1)
+                / 6.0
+                * (self.f(x1) + 4.0 * self.f(0.5 * (x1 + x2)) + self.f(x2))
+            )
+
+        return simpson_integral
+
+    def rectangles_rule(self, rect_type="middle") -> float:
+        rectangles_integral = 0
+        if rect_type == "left":
+            for i in range(0, self.n):
+                x_i_plus_1 = self.a + (i + 1) * self.h
+                x_i = self.a + i * self.h
+                f_x = self.f(x_i)
+                rectangles_integral += f_x * (x_i_plus_1 - x_i)
+        elif rect_type == "right":
+            for i in range(1, self.n + 1):
+                x_i = self.a + i * self.h
+                x_i_minus_1 = self.a + (i - 1) * self.h
+                f_x = self.f(x_i)
+                rectangles_integral += f_x * (x_i - x_i_minus_1)
+        elif rect_type == "middle":
+            for i in range(0, self.n):
+                x_i = self.a + (i * self.h)
+                x_i_plus_1 = self.a + ((i + 1) * self.h)
+                f_x = self.f((x_i + x_i_plus_1) / 2)
+                rectangles_integral += f_x * (x_i_plus_1 - x_i)
+        else:
+            print("Correct options:\nleft\nright\nmiddle")
+        return rectangles_integral
```

