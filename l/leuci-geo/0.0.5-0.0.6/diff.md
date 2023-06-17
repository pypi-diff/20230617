# Comparing `tmp/leuci-geo-0.0.5.tar.gz` & `tmp/leuci-geo-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leuci-geo-0.0.5.tar", last modified: Sat Jun 17 16:06:26 2023, max compression
+gzip compressed data, was "leuci-geo-0.0.6.tar", last modified: Sat Jun 17 19:02:33 2023, max compression
```

## Comparing `leuci-geo-0.0.5.tar` & `leuci-geo-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-17 16:06:26.350780 leuci-geo-0.0.5/
--rw-r--r--   0 rachel    (1000) rachel    (1000)    35149 2023-05-25 20:00:31.000000 leuci-geo-0.0.5/LICENSE
--rw-r--r--   0 rachel    (1000) rachel    (1000)      553 2023-06-17 16:06:26.360780 leuci-geo-0.0.5/PKG-INFO
--rw-r--r--   0 rachel    (1000) rachel    (1000)       22 2023-05-25 20:00:31.000000 leuci-geo-0.0.5/README.md
--rw-r--r--   0 rachel    (1000) rachel    (1000)      104 2023-02-09 09:20:26.000000 leuci-geo-0.0.5/pyproject.toml
--rw-r--r--   0 rachel    (1000) rachel    (1000)      656 2023-06-17 16:06:26.380780 leuci-geo-0.0.5/setup.cfg
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-17 16:06:26.160780 leuci-geo-0.0.5/src/
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-17 16:06:26.300780 leuci-geo-0.0.5/src/leuci_geo/
--rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2023-02-09 09:20:26.000000 leuci-geo-0.0.5/src/leuci_geo/__init__.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)     2963 2023-05-29 13:51:47.000000 leuci-geo-0.0.5/src/leuci_geo/geocalculator.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)    27123 2023-06-04 18:16:10.000000 leuci-geo-0.0.5/src/leuci_geo/pdbgeometry.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)     2844 2023-05-29 13:40:46.000000 leuci-geo-0.0.5/src/leuci_geo/pdbloader.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)     9405 2023-06-04 13:05:42.000000 leuci-geo-0.0.5/src/leuci_geo/pdbobject.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2023-05-29 10:54:24.000000 leuci-geo-0.0.5/src/leuci_geo/pdbspace.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)    21739 2023-06-17 16:02:55.000000 leuci-geo-0.0.5/src/leuci_geo/reportmaker.py
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-17 16:06:26.340780 leuci-geo-0.0.5/src/leuci_geo.egg-info/
--rw-r--r--   0 rachel    (1000) rachel    (1000)      553 2023-06-17 16:06:25.000000 leuci-geo-0.0.5/src/leuci_geo.egg-info/PKG-INFO
--rw-r--r--   0 rachel    (1000) rachel    (1000)      385 2023-06-17 16:06:26.000000 leuci-geo-0.0.5/src/leuci_geo.egg-info/SOURCES.txt
--rw-r--r--   0 rachel    (1000) rachel    (1000)        1 2023-06-17 16:06:25.000000 leuci-geo-0.0.5/src/leuci_geo.egg-info/dependency_links.txt
--rw-r--r--   0 rachel    (1000) rachel    (1000)       10 2023-06-17 16:06:25.000000 leuci-geo-0.0.5/src/leuci_geo.egg-info/top_level.txt
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-17 19:02:33.295976 leuci-geo-0.0.6/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)    35149 2023-05-25 20:00:31.000000 leuci-geo-0.0.6/LICENSE
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      553 2023-06-17 19:02:33.295976 leuci-geo-0.0.6/PKG-INFO
+-rw-r--r--   0 rachel    (1000) rachel    (1000)       22 2023-05-25 20:00:31.000000 leuci-geo-0.0.6/README.md
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      104 2023-02-09 09:20:26.000000 leuci-geo-0.0.6/pyproject.toml
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      656 2023-06-17 19:02:33.295976 leuci-geo-0.0.6/setup.cfg
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-17 19:02:33.285976 leuci-geo-0.0.6/src/
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-17 19:02:33.295976 leuci-geo-0.0.6/src/leuci_geo/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2023-02-09 09:20:26.000000 leuci-geo-0.0.6/src/leuci_geo/__init__.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)     2963 2023-05-29 13:51:47.000000 leuci-geo-0.0.6/src/leuci_geo/geocalculator.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)    27123 2023-06-04 18:16:10.000000 leuci-geo-0.0.6/src/leuci_geo/pdbgeometry.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)     2844 2023-05-29 13:40:46.000000 leuci-geo-0.0.6/src/leuci_geo/pdbloader.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)     9405 2023-06-04 13:05:42.000000 leuci-geo-0.0.6/src/leuci_geo/pdbobject.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2023-05-29 10:54:24.000000 leuci-geo-0.0.6/src/leuci_geo/pdbspace.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)    22513 2023-06-17 19:01:30.000000 leuci-geo-0.0.6/src/leuci_geo/reportmaker.py
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-17 19:02:33.295976 leuci-geo-0.0.6/src/leuci_geo.egg-info/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      553 2023-06-17 19:02:33.000000 leuci-geo-0.0.6/src/leuci_geo.egg-info/PKG-INFO
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      385 2023-06-17 19:02:33.000000 leuci-geo-0.0.6/src/leuci_geo.egg-info/SOURCES.txt
+-rw-r--r--   0 rachel    (1000) rachel    (1000)        1 2023-06-17 19:02:33.000000 leuci-geo-0.0.6/src/leuci_geo.egg-info/dependency_links.txt
+-rw-r--r--   0 rachel    (1000) rachel    (1000)       10 2023-06-17 19:02:33.000000 leuci-geo-0.0.6/src/leuci_geo.egg-info/top_level.txt
```

### Comparing `leuci-geo-0.0.5/LICENSE` & `leuci-geo-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `leuci-geo-0.0.5/PKG-INFO` & `leuci-geo-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leuci-geo
-Version: 0.0.5
+Version: 0.0.6
 Summary: geometric paramaters and searches of protein structures
 Home-page: https://github.com/pypa/sampleproject
 Author: Rachel Alcraft
 Author-email: rachelalcraft@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `leuci-geo-0.0.5/setup.cfg` & `leuci-geo-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = leuci-geo
-version = 0.0.5
+version = 0.0.6
 author = Rachel Alcraft
 author_email = rachelalcraft@gmail.com
 description = geometric paramaters and searches of protein structures
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `leuci-geo-0.0.5/src/leuci_geo/geocalculator.py` & `leuci-geo-0.0.6/src/leuci_geo/geocalculator.py`

 * *Files identical despite different names*

### Comparing `leuci-geo-0.0.5/src/leuci_geo/pdbgeometry.py` & `leuci-geo-0.0.6/src/leuci_geo/pdbgeometry.py`

 * *Files identical despite different names*

### Comparing `leuci-geo-0.0.5/src/leuci_geo/pdbloader.py` & `leuci-geo-0.0.6/src/leuci_geo/pdbloader.py`

 * *Files identical despite different names*

### Comparing `leuci-geo-0.0.5/src/leuci_geo/pdbobject.py` & `leuci-geo-0.0.6/src/leuci_geo/pdbobject.py`

 * *Files identical despite different names*

### Comparing `leuci-geo-0.0.5/src/leuci_geo/reportmaker.py` & `leuci-geo-0.0.6/src/leuci_geo/reportmaker.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,33 @@
         #Having plotted we now need to get the image data from the plt
         if not overlay:
             encoded = self.getPlotImage(self.fig, self.ax)
             htmlstring = '<img src="data:image/png;base64, {}">'.format(encoded.decode('utf-8')) + '\n'
             self.HTMLIncrement()
             self.html_string += '<td width=' + str(int(100/self.cols)) + '%>' + htmlstring + '</td>\n'
 
+    def addPoints2d(self,points,hue="yellow",overlay=False):
+        self.incrementOverlay(overlay)        
+        self.ax.set_axisbelow(True)
+        xs = []
+        ys = []
+        for p in points:
+            xs.append(p[0])
+            ys.append(p[1])
+        g = self.ax.scatter(xs, ys, edgecolor='silver', linewidth=0.5, s=20,c=hue)
+        cb = plt.colorbar(g)
+        #Having plotted we now need to get the image data from the plt
+        if not overlay:
+            encoded = self.getPlotImage(self.fig, self.ax)
+            htmlstring = '<img src="data:image/png;base64, {}">'.format(encoded.decode('utf-8')) + '\n'
+            self.HTMLIncrement()
+            self.html_string += '<td width=' + str(int(100/self.cols)) + '%>' + htmlstring + '</td>\n'
+
+        
+
     def addPlotOnly(self,fig,ax):
         encoded = self.getPlotImage(fig,ax)
         htmlstring = '<img src="data:image/png;base64, {}">'.format(encoded.decode('utf-8')) + '\n'
         self.HTMLIncrement()
         self.html_string += '<td width=' + str(int(100 / self.cols)) + '%>' + htmlstring + '</td>\n'
 
     def addPlot1d(self, data,plottype, geo_x,hue='',title='',palette='crimson',overlay=False,alpha=1,xrange=[None,None],cumulative=False,density=False,bins=20):
```

### Comparing `leuci-geo-0.0.5/src/leuci_geo.egg-info/PKG-INFO` & `leuci-geo-0.0.6/src/leuci_geo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leuci-geo
-Version: 0.0.5
+Version: 0.0.6
 Summary: geometric paramaters and searches of protein structures
 Home-page: https://github.com/pypa/sampleproject
 Author: Rachel Alcraft
 Author-email: rachelalcraft@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

