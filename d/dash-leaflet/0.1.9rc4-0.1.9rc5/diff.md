# Comparing `tmp/dash_leaflet-0.1.9rc4.tar.gz` & `tmp/dash_leaflet-0.1.9rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dash_leaflet-0.1.9rc4.tar", last modified: Fri Nov 27 12:43:37 2020, max compression
+gzip compressed data, was "dist/dash_leaflet-0.1.9rc5.tar", last modified: Fri Nov 27 12:50:03 2020, max compression
```

## Comparing `dash_leaflet-0.1.9rc4.tar` & `dash_leaflet-0.1.9rc5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 emher     (1000) emher     (1000)        0 2020-11-27 12:43:37.591119 dash_leaflet-0.1.9rc4/
--rw-rw-r--   0 emher     (1000) emher     (1000)      169 2020-08-21 19:24:26.000000 dash_leaflet-0.1.9rc4/MANIFEST.in
--rw-rw-r--   0 emher     (1000) emher     (1000)     2525 2020-11-27 12:43:37.591119 dash_leaflet-0.1.9rc4/PKG-INFO
--rw-rw-r--   0 emher     (1000) emher     (1000)     1742 2020-09-24 11:50:44.000000 dash_leaflet-0.1.9rc4/README.md
-drwxrwxr-x   0 emher     (1000) emher     (1000)        0 2020-11-27 12:43:37.591119 dash_leaflet-0.1.9rc4/dash_leaflet/
--rw-rw-r--   0 emher     (1000) emher     (1000)     1483 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/BaseLayer.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     4482 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/Circle.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     4504 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/CircleMarker.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     3923 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/Colorbar.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     4655 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/DivMarker.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     1685 2020-09-02 16:46:05.000000 dash_leaflet-0.1.9rc4/dash_leaflet/DivOverlay.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     1798 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/EasyButton.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     1744 2020-09-22 14:11:13.000000 dash_leaflet-0.1.9rc4/dash_leaflet/FreeDraw.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     1955 2020-09-22 15:03:41.000000 dash_leaflet-0.1.9rc4/dash_leaflet/Freedraw.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     3796 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/GeoJSON.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     8161 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/GeoTIFFOverlay.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     4689 2020-09-02 16:46:05.000000 dash_leaflet-0.1.9rc4/dash_leaflet/GridLayer.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     3749 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/ImageOverlay.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     1546 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/LayerGroup.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     1590 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/LayersControl.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     2017 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/LocateControl.py
--rw-rw-r--   0 emher     (1000) emher     (1000)    13242 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/Map.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     1557 2020-09-02 16:46:05.000000 dash_leaflet-0.1.9rc4/dash_leaflet/MapLayer.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     4258 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/Marker.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     1742 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/MarkerClusterGroup.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     3441 2020-11-14 16:36:57.000000 dash_leaflet-0.1.9rc4/dash_leaflet/Measure.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     3469 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/MeasureControl.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     1472 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/Overlay.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     1740 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/Pane.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     4068 2020-09-02 16:46:05.000000 dash_leaflet-0.1.9rc4/dash_leaflet/Path.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     5000 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/Polygon.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     4970 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/Polyline.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     2801 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/PolylineDecorator.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     4123 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/Popup.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     4969 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/Rectangle.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     3256 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/SVGOverlay.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     2106 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/ScaleControl.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     3861 2020-09-02 16:46:05.000000 dash_leaflet-0.1.9rc4/dash_leaflet/SuperCluster.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     6791 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/TileLayer.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     2671 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/Tooltip.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     4350 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/VideoOverlay.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     7352 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/WMSTileLayer.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     1141 2020-08-31 20:56:59.000000 dash_leaflet-0.1.9rc4/dash_leaflet/__init__.py
--rw-rw-r--   0 emher     (1000) emher     (1000)     1529 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/_imports_.py
--rw-rw-r--   0 emher     (1000) emher     (1000)  5784139 2020-11-27 12:43:21.000000 dash_leaflet-0.1.9rc4/dash_leaflet/dash_leaflet.dev.js
--rw-rw-r--   0 emher     (1000) emher     (1000)   741415 2020-11-27 12:43:16.000000 dash_leaflet-0.1.9rc4/dash_leaflet/dash_leaflet.min.js
--rw-rw-r--   0 emher     (1000) emher     (1000)      993 2020-11-27 10:58:27.000000 dash_leaflet-0.1.9rc4/dash_leaflet/express.py
--rw-rw-r--   0 emher     (1000) emher     (1000)   131260 2020-11-27 12:43:22.000000 dash_leaflet-0.1.9rc4/dash_leaflet/metadata.json
--rw-rw-r--   0 emher     (1000) emher     (1000)     2514 2020-11-27 12:43:21.000000 dash_leaflet-0.1.9rc4/dash_leaflet/package.json
-drwxrwxr-x   0 emher     (1000) emher     (1000)        0 2020-11-27 12:43:37.591119 dash_leaflet-0.1.9rc4/dash_leaflet.egg-info/
--rw-rw-r--   0 emher     (1000) emher     (1000)     2525 2020-11-27 12:43:37.000000 dash_leaflet-0.1.9rc4/dash_leaflet.egg-info/PKG-INFO
--rw-rw-r--   0 emher     (1000) emher     (1000)     1381 2020-11-27 12:43:37.000000 dash_leaflet-0.1.9rc4/dash_leaflet.egg-info/SOURCES.txt
--rw-rw-r--   0 emher     (1000) emher     (1000)        1 2020-11-27 12:43:37.000000 dash_leaflet-0.1.9rc4/dash_leaflet.egg-info/dependency_links.txt
--rw-rw-r--   0 emher     (1000) emher     (1000)        7 2020-11-27 12:43:37.000000 dash_leaflet-0.1.9rc4/dash_leaflet.egg-info/requires.txt
--rw-rw-r--   0 emher     (1000) emher     (1000)       13 2020-11-27 12:43:37.000000 dash_leaflet-0.1.9rc4/dash_leaflet.egg-info/top_level.txt
--rw-rw-r--   0 emher     (1000) emher     (1000)       38 2020-11-27 12:43:37.591119 dash_leaflet-0.1.9rc4/setup.cfg
--rw-rw-r--   0 emher     (1000) emher     (1000)     1017 2020-09-08 14:40:00.000000 dash_leaflet-0.1.9rc4/setup.py
+drwxrwxr-x   0 emher     (1000) emher     (1000)        0 2020-11-27 12:50:03.466345 dash_leaflet-0.1.9rc5/
+-rw-rw-r--   0 emher     (1000) emher     (1000)      169 2020-08-21 19:24:26.000000 dash_leaflet-0.1.9rc5/MANIFEST.in
+-rw-rw-r--   0 emher     (1000) emher     (1000)     2525 2020-11-27 12:50:03.466345 dash_leaflet-0.1.9rc5/PKG-INFO
+-rw-rw-r--   0 emher     (1000) emher     (1000)     1742 2020-09-24 11:50:44.000000 dash_leaflet-0.1.9rc5/README.md
+drwxrwxr-x   0 emher     (1000) emher     (1000)        0 2020-11-27 12:50:03.466345 dash_leaflet-0.1.9rc5/dash_leaflet/
+-rw-rw-r--   0 emher     (1000) emher     (1000)     1483 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/BaseLayer.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     4482 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/Circle.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     4504 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/CircleMarker.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     3923 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/Colorbar.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     4655 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/DivMarker.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     1685 2020-09-02 16:46:05.000000 dash_leaflet-0.1.9rc5/dash_leaflet/DivOverlay.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     1798 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/EasyButton.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     1744 2020-09-22 14:11:13.000000 dash_leaflet-0.1.9rc5/dash_leaflet/FreeDraw.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     1955 2020-09-22 15:03:41.000000 dash_leaflet-0.1.9rc5/dash_leaflet/Freedraw.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     3796 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/GeoJSON.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     8161 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/GeoTIFFOverlay.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     4689 2020-09-02 16:46:05.000000 dash_leaflet-0.1.9rc5/dash_leaflet/GridLayer.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     3749 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/ImageOverlay.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     1546 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/LayerGroup.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     1590 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/LayersControl.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     2017 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/LocateControl.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)    13242 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/Map.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     1557 2020-09-02 16:46:05.000000 dash_leaflet-0.1.9rc5/dash_leaflet/MapLayer.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     4258 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/Marker.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     1742 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/MarkerClusterGroup.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     3441 2020-11-14 16:36:57.000000 dash_leaflet-0.1.9rc5/dash_leaflet/Measure.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     3469 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/MeasureControl.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     1472 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/Overlay.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     1740 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/Pane.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     4068 2020-09-02 16:46:05.000000 dash_leaflet-0.1.9rc5/dash_leaflet/Path.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     5000 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/Polygon.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     4970 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/Polyline.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     2801 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/PolylineDecorator.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     4123 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/Popup.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     4969 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/Rectangle.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     3256 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/SVGOverlay.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     2106 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/ScaleControl.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     3861 2020-09-02 16:46:05.000000 dash_leaflet-0.1.9rc5/dash_leaflet/SuperCluster.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     6791 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/TileLayer.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     2671 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/Tooltip.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     4350 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/VideoOverlay.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     7352 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/WMSTileLayer.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     1141 2020-08-31 20:56:59.000000 dash_leaflet-0.1.9rc5/dash_leaflet/__init__.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)     1529 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/_imports_.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)  5784139 2020-11-27 12:49:59.000000 dash_leaflet-0.1.9rc5/dash_leaflet/dash_leaflet.dev.js
+-rw-rw-r--   0 emher     (1000) emher     (1000)   741415 2020-11-27 12:49:54.000000 dash_leaflet-0.1.9rc5/dash_leaflet/dash_leaflet.min.js
+-rw-rw-r--   0 emher     (1000) emher     (1000)      935 2020-11-27 12:49:36.000000 dash_leaflet-0.1.9rc5/dash_leaflet/express.py
+-rw-rw-r--   0 emher     (1000) emher     (1000)   131260 2020-11-27 12:50:00.000000 dash_leaflet-0.1.9rc5/dash_leaflet/metadata.json
+-rw-rw-r--   0 emher     (1000) emher     (1000)     2514 2020-11-27 12:49:59.000000 dash_leaflet-0.1.9rc5/dash_leaflet/package.json
+drwxrwxr-x   0 emher     (1000) emher     (1000)        0 2020-11-27 12:50:03.466345 dash_leaflet-0.1.9rc5/dash_leaflet.egg-info/
+-rw-rw-r--   0 emher     (1000) emher     (1000)     2525 2020-11-27 12:50:03.000000 dash_leaflet-0.1.9rc5/dash_leaflet.egg-info/PKG-INFO
+-rw-rw-r--   0 emher     (1000) emher     (1000)     1381 2020-11-27 12:50:03.000000 dash_leaflet-0.1.9rc5/dash_leaflet.egg-info/SOURCES.txt
+-rw-rw-r--   0 emher     (1000) emher     (1000)        1 2020-11-27 12:50:03.000000 dash_leaflet-0.1.9rc5/dash_leaflet.egg-info/dependency_links.txt
+-rw-rw-r--   0 emher     (1000) emher     (1000)        7 2020-11-27 12:50:03.000000 dash_leaflet-0.1.9rc5/dash_leaflet.egg-info/requires.txt
+-rw-rw-r--   0 emher     (1000) emher     (1000)       13 2020-11-27 12:50:03.000000 dash_leaflet-0.1.9rc5/dash_leaflet.egg-info/top_level.txt
+-rw-rw-r--   0 emher     (1000) emher     (1000)       38 2020-11-27 12:50:03.466345 dash_leaflet-0.1.9rc5/setup.cfg
+-rw-rw-r--   0 emher     (1000) emher     (1000)     1017 2020-09-08 14:40:00.000000 dash_leaflet-0.1.9rc5/setup.py
```

### Comparing `dash_leaflet-0.1.9rc4/PKG-INFO` & `dash_leaflet-0.1.9rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash_leaflet
-Version: 0.1.9rc4
+Version: 0.1.9rc5
 Summary: Leaflet component for Dash
 Home-page: https://github.com/thedirtyfew/dash-leaflet
 Author: Emil Haldrup Eriksen
 Author-email: emil.h.eriksen@gmail.com
 License: MIT
 Description: Dash Leaflet is a light wrapper around React-Leaflet. The syntax is similar to other Dash components, with naming conventions following the React-Leaflet API.
```

### Comparing `dash_leaflet-0.1.9rc4/README.md` & `dash_leaflet-0.1.9rc5/README.md`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/BaseLayer.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/BaseLayer.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/Circle.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/Circle.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/CircleMarker.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/CircleMarker.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/Colorbar.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/Colorbar.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/DivMarker.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/DivMarker.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/DivOverlay.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/DivOverlay.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/EasyButton.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/EasyButton.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/FreeDraw.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/FreeDraw.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/Freedraw.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/Freedraw.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/GeoJSON.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/GeoJSON.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/GeoTIFFOverlay.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/GeoTIFFOverlay.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/GridLayer.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/GridLayer.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/ImageOverlay.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/ImageOverlay.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/LayerGroup.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/LayerGroup.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/LayersControl.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/LayersControl.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/LocateControl.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/LocateControl.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/Map.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/Map.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/MapLayer.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/MapLayer.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/Marker.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/Marker.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/MarkerClusterGroup.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/MarkerClusterGroup.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/Measure.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/Measure.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/MeasureControl.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/MeasureControl.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/Overlay.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/Overlay.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/Pane.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/Pane.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/Path.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/Path.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/Polygon.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/Polygon.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/Polyline.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/Polyline.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/PolylineDecorator.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/PolylineDecorator.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/Popup.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/Popup.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/Rectangle.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/Rectangle.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/SVGOverlay.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/SVGOverlay.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/ScaleControl.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/ScaleControl.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/SuperCluster.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/SuperCluster.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/TileLayer.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/TileLayer.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/Tooltip.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/Tooltip.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/VideoOverlay.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/VideoOverlay.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/WMSTileLayer.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/WMSTileLayer.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/__init__.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/_imports_.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/_imports_.py`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/dash_leaflet.dev.js` & `dash_leaflet-0.1.9rc5/dash_leaflet/dash_leaflet.dev.js`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/dash_leaflet.min.js` & `dash_leaflet-0.1.9rc5/dash_leaflet/dash_leaflet.min.js`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/express.py` & `dash_leaflet-0.1.9rc5/dash_leaflet/express.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import geobuf
 import dash_leaflet as dl
 import base64
 
-from dash_extensions.snippets import JavaScriptNamespace
-
 
 def categorical_colorbar(*args, categories, colorscale, **kwargs):
     indices = list(range(len(categories) + 1))
     return dl.Colorbar(*args, min=0, max=len(categories), classes=indices, colorscale=colorscale, tooltip=False,
                        tickValues=[item + 0.5 for item in indices[:-1]], tickText=categories, **kwargs)
```

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/metadata.json` & `dash_leaflet-0.1.9rc5/dash_leaflet/metadata.json`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet/package.json` & `dash_leaflet-0.1.9rc5/dash_leaflet/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'0.1.9rc5'"}*

```diff
@@ -72,9 +72,9 @@
         "build:js-dev": "webpack --mode development",
         "build:py": "dash-generate-components ./src/lib/components dash_leaflet",
         "build:py-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py)",
         "prepublish": "npm run validate-init",
         "start": "webpack-serve ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.1.9rc4"
+    "version": "0.1.9rc5"
 }
```

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet.egg-info/PKG-INFO` & `dash_leaflet-0.1.9rc5/dash_leaflet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-leaflet
-Version: 0.1.9rc4
+Version: 0.1.9rc5
 Summary: Leaflet component for Dash
 Home-page: https://github.com/thedirtyfew/dash-leaflet
 Author: Emil Haldrup Eriksen
 Author-email: emil.h.eriksen@gmail.com
 License: MIT
 Description: Dash Leaflet is a light wrapper around React-Leaflet. The syntax is similar to other Dash components, with naming conventions following the React-Leaflet API.
```

### Comparing `dash_leaflet-0.1.9rc4/dash_leaflet.egg-info/SOURCES.txt` & `dash_leaflet-0.1.9rc5/dash_leaflet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash_leaflet-0.1.9rc4/setup.py` & `dash_leaflet-0.1.9rc5/setup.py`

 * *Files identical despite different names*

