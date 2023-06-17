# Comparing `tmp/skmetpy-0.0.4.tar.gz` & `tmp/skmetpy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skmetpy-0.0.4.tar", last modified: Sat Jun 17 16:06:09 2023, max compression
+gzip compressed data, was "skmetpy-0.0.5.tar", last modified: Sat Jun 17 16:12:29 2023, max compression
```

## Comparing `skmetpy-0.0.4.tar` & `skmetpy-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 16:06:09.680738 skmetpy-0.0.4/
--rw-rw-rw-   0        0        0      259 2023-06-17 16:06:09.679737 skmetpy-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-17 16:06:09.674133 skmetpy-0.0.4/nunpy/
--rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.0.4/nunpy/__init__.py
--rw-rw-rw-   0        0        0    19073 2023-06-17 16:03:26.000000 skmetpy-0.0.4/nunpy/rechape.py
--rw-rw-rw-   0        0        0       42 2023-06-17 16:06:09.680738 skmetpy-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      324 2023-06-17 16:06:07.000000 skmetpy-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 16:06:09.678735 skmetpy-0.0.4/skmetpy.egg-info/
--rw-rw-rw-   0        0        0      259 2023-06-17 16:06:09.000000 skmetpy-0.0.4/skmetpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-06-17 16:06:09.000000 skmetpy-0.0.4/skmetpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 16:06:09.000000 skmetpy-0.0.4/skmetpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-17 16:06:09.000000 skmetpy-0.0.4/skmetpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 16:12:29.227377 skmetpy-0.0.5/
+-rw-rw-rw-   0        0        0      259 2023-06-17 16:12:29.226705 skmetpy-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-17 16:12:29.220699 skmetpy-0.0.5/nunpy/
+-rw-rw-rw-   0        0        0       24 2023-06-17 16:06:02.000000 skmetpy-0.0.5/nunpy/__init__.py
+-rw-rw-rw-   0        0        0    19070 2023-06-17 16:12:21.000000 skmetpy-0.0.5/nunpy/rechape.py
+-rw-rw-rw-   0        0        0       42 2023-06-17 16:12:29.227377 skmetpy-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      324 2023-06-17 16:12:27.000000 skmetpy-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 16:12:29.224704 skmetpy-0.0.5/skmetpy.egg-info/
+-rw-rw-rw-   0        0        0      259 2023-06-17 16:12:29.000000 skmetpy-0.0.5/skmetpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-06-17 16:12:29.000000 skmetpy-0.0.5/skmetpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 16:12:29.000000 skmetpy-0.0.5/skmetpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-17 16:12:29.000000 skmetpy-0.0.5/skmetpy.egg-info/top_level.txt
```

### Comparing `skmetpy-0.0.4/nunpy/rechape.py` & `skmetpy-0.0.5/nunpy/rechape.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,57 +21,57 @@
           f"20 - fmin2()\n"
           f"21 - recom2()\n"
           f"22 - simi2()\n"
           f"23 - km2()\n"
           f"24 - checkG2()\n")
 
 
-def list_1():
+def list1():
     print(f"1 - pasos_1()\n"
           f"2 - carga1()\n"
           f"3 - hold1()\n"
           f"4 - norm1()\n"
           f"5 - ini1()\n"
           f"6 - fordw1()\n"
           f"7 - cost1()\n"
           f"8 - grad1()\n"
           f"9 - fmin1()\n"
           f"10 - unroll1()\n"
           f"11 - pred1()\n"
           )
 
 
-def list_2():
+def list2():
     print(f"1 - pasos_2()\n"
           f"2 - carga2()\n"
           f"3 - rank2()\n"
           f"4 - cost2()\n"
           f"5 - grad2()\n"
           f"6 - fmin2()\n"
           f"7 - recom2()\n"
           f"8 - simi2()\n"
           f"9 - km2()\n"
           f"10 - checkG2()\n")
 
 
-def pasos_1():
+def pasos1():
     print("1 - Carga de datos\n"
           "2 - Holdout\n"
           "3 - Normaliza\n"
           "4 - Inicializa las thetas (pesos)\n"
           "5 - Forward\n"
           "6 - Coste\n"
           "7 - Gradiente\n"
           "8 - Fmin\n"
           "9 - Desenrolla el fmin\n"
           "10 - Normaliza X-test\n"
           "11 - Predice\n")
 
 
-def pasos_2():
+def pasos2():
     print("1 - Carga de datos\n"
           "2 - Ranking de peliculas\n"
           "3 - Coste\n"
           "4 - Gradiente\n"
           "5 - Fmin\n"
           "6 - Recomendacion usuario\n"
           "7 - Peliculas similares\n"
@@ -156,15 +156,15 @@
                   W = np.random.rand(capa_salida, capa_entrada) * 2 * epsilon_init - epsilon_init
                   return W
       '''
 
     print(string)
 
 
-def forwd():
+def forwd1():
     string = '''
             def forward(theta1, theta2, theta3, X):
                 #Variables necesarias
                 m = len(X)
                 ones = np.ones((m, 1))
 
                 #Calculamos las activaciones añadiendole la bias después
```

