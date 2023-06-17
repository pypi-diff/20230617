# Comparing `tmp/tf2-utilities-2.0.5.tar.gz` & `tmp/tf2-utilities-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf2-utilities-2.0.5.tar", last modified: Thu Jan 12 09:06:54 2023, max compression
+gzip compressed data, was "tf2-utilities-2.1.0.tar", last modified: Sat Jun 17 07:26:40 2023, max compression
```

## Comparing `tf2-utilities-2.0.5.tar` & `tf2-utilities-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dixonlokeshengheng   (501) staff       (20)        0 2023-01-12 09:06:54.410483 tf2-utilities-2.0.5/
--rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)     1069 2022-05-19 15:29:26.000000 tf2-utilities-2.0.5/LICENSE
--rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)     2116 2023-01-12 09:06:54.410324 tf2-utilities-2.0.5/PKG-INFO
--rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)     1586 2022-08-05 09:37:00.000000 tf2-utilities-2.0.5/README.md
--rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)       38 2023-01-12 09:06:54.410535 tf2-utilities-2.0.5/setup.cfg
--rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)      941 2023-01-12 09:05:21.000000 tf2-utilities-2.0.5/setup.py
-drwxr-xr-x   0 dixonlokeshengheng   (501) staff       (20)        0 2023-01-12 09:06:54.408917 tf2-utilities-2.0.5/tf2_utilities.egg-info/
--rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)     2116 2023-01-12 09:06:54.000000 tf2-utilities-2.0.5/tf2_utilities.egg-info/PKG-INFO
--rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)      322 2023-01-12 09:06:54.000000 tf2-utilities-2.0.5/tf2_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)        1 2023-01-12 09:06:54.000000 tf2-utilities-2.0.5/tf2_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)       13 2023-01-12 09:06:54.000000 tf2-utilities-2.0.5/tf2_utilities.egg-info/requires.txt
--rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)       13 2023-01-12 09:06:54.000000 tf2-utilities-2.0.5/tf2_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 dixonlokeshengheng   (501) staff       (20)        0 2023-01-12 09:06:54.410083 tf2-utilities-2.0.5/tf2utilities/
--rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)        0 2022-05-19 07:01:37.000000 tf2-utilities-2.0.5/tf2utilities/__init__.py
--rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)     3279 2022-08-05 06:49:07.000000 tf2-utilities-2.0.5/tf2utilities/main.py
--rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)    53979 2023-01-10 04:01:45.000000 tf2-utilities-2.0.5/tf2utilities/schema.py
--rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)     7398 2022-06-28 08:39:47.000000 tf2-utilities-2.0.5/tf2utilities/sku.py
--rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)      563 2022-05-18 13:06:58.000000 tf2-utilities-2.0.5/tf2utilities/webapi.py
+drwxr-xr-x   0 dixonlokeshengheng   (501) staff       (20)        0 2023-06-17 07:26:40.903499 tf2-utilities-2.1.0/
+-rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)     1069 2022-05-19 15:29:26.000000 tf2-utilities-2.1.0/LICENSE
+-rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)     2218 2023-06-17 07:26:40.903345 tf2-utilities-2.1.0/PKG-INFO
+-rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)     1586 2022-08-05 09:37:00.000000 tf2-utilities-2.1.0/README.md
+-rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)       38 2023-06-17 07:26:40.903554 tf2-utilities-2.1.0/setup.cfg
+-rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)     1041 2023-06-17 07:21:25.000000 tf2-utilities-2.1.0/setup.py
+drwxr-xr-x   0 dixonlokeshengheng   (501) staff       (20)        0 2023-06-17 07:26:40.902396 tf2-utilities-2.1.0/tf2_utilities.egg-info/
+-rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)     2218 2023-06-17 07:26:40.000000 tf2-utilities-2.1.0/tf2_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)      322 2023-06-17 07:26:40.000000 tf2-utilities-2.1.0/tf2_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)        1 2023-06-17 07:26:40.000000 tf2-utilities-2.1.0/tf2_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)       13 2023-06-17 07:26:40.000000 tf2-utilities-2.1.0/tf2_utilities.egg-info/requires.txt
+-rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)       13 2023-06-17 07:26:40.000000 tf2-utilities-2.1.0/tf2_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 dixonlokeshengheng   (501) staff       (20)        0 2023-06-17 07:26:40.903128 tf2-utilities-2.1.0/tf2utilities/
+-rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)        0 2022-05-19 07:01:37.000000 tf2-utilities-2.1.0/tf2utilities/__init__.py
+-rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)     3279 2022-08-05 06:49:07.000000 tf2-utilities-2.1.0/tf2utilities/main.py
+-rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)    54078 2023-06-17 07:02:24.000000 tf2-utilities-2.1.0/tf2utilities/schema.py
+-rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)     7398 2022-06-28 08:39:47.000000 tf2-utilities-2.1.0/tf2utilities/sku.py
+-rw-r--r--   0 dixonlokeshengheng   (501) staff       (20)      563 2022-05-18 13:06:58.000000 tf2-utilities-2.1.0/tf2utilities/webapi.py
```

### Comparing `tf2-utilities-2.0.5/LICENSE` & `tf2-utilities-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tf2-utilities-2.0.5/PKG-INFO` & `tf2-utilities-2.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: tf2-utilities
-Version: 2.0.5
+Version: 2.1.0
 Summary: Get information about TF2 items, effects, skins and more
 Home-page: https://github.com/j0hnnyblack/python-tf2-utilities
 Author: Johnny Black
 Author-email: lokedixon@hotmail.my
 License: MIT
 Keywords: tf2,teamfortress2,steam,trade,trading
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-tf2-utilities
 Get information about TF2 items, effects, skins and more. 
 Inspired by [TF2autobot's node-tf2-schema](https://github.com/TF2Autobot/node-tf2-schema) and [TF2autobot's node-tf2-sku](https://github.com/TF2Autobot/node-tf2-sku).
```

### Comparing `tf2-utilities-2.0.5/README.md` & `tf2-utilities-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tf2-utilities-2.0.5/setup.py` & `tf2-utilities-2.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="tf2-utilities",
-    version="2.0.5",
+    version="2.1.0",
     description="Get information about TF2 items, effects, skins and more",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/j0hnnyblack/python-tf2-utilities",
     author="Johnny Black",
     author_email="lokedixon@hotmail.my",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     packages=["tf2utilities"],
     include_package_data=True,
     install_requires=['requests', 'vdf'],
     keywords=["tf2", "teamfortress2", "steam", "trade", "trading"]
 )
```

### Comparing `tf2-utilities-2.0.5/tf2_utilities.egg-info/PKG-INFO` & `tf2-utilities-2.1.0/tf2_utilities.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: tf2-utilities
-Version: 2.0.5
+Version: 2.1.0
 Summary: Get information about TF2 items, effects, skins and more
 Home-page: https://github.com/j0hnnyblack/python-tf2-utilities
 Author: Johnny Black
 Author-email: lokedixon@hotmail.my
 License: MIT
 Keywords: tf2,teamfortress2,steam,trade,trading
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # python-tf2-utilities
 Get information about TF2 items, effects, skins and more. 
 Inspired by [TF2autobot's node-tf2-schema](https://github.com/TF2Autobot/node-tf2-schema) and [TF2autobot's node-tf2-sku](https://github.com/TF2Autobot/node-tf2-sku).
```

### Comparing `tf2-utilities-2.0.5/tf2utilities/main.py` & `tf2-utilities-2.1.0/tf2utilities/main.py`

 * *Files identical despite different names*

### Comparing `tf2-utilities-2.0.5/tf2utilities/schema.py` & `tf2-utilities-2.1.0/tf2utilities/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,15 +408,17 @@
             'haunted phantasm jr',
             'haunted phantasm',
             'haunted metal scrap',
             'haunted hat',
             'unusual cap',
             'vintage tyrolean',
             'vintage merryweather',
-            'haunted kraken'
+            'haunted kraken',
+            'haunted forever!',
+            'frostbite bonnet'
         ]
 
         qualitySearch = name
         for ex in exception:
             if ex in name: 
                 qualitySearch = name.replace(ex, "").strip()
                 break
@@ -525,15 +527,15 @@
                                 item["quality"] = 15
                         elif item.get("quality") == 5 and item.get("quality5") is None:
                             item["quality"] == 15
                     if not item.get("quality"):
                         item["quality"] = 15
                     break
 
-            if "war paint" not in name:
+            if "war paint" not in name and "paintkit" in item:
                 oldDefindex = item["defindex"]
                 if 'pistol' in name and str(item['paintkit']) in self.getWeaponSkinsList["pistolSkins"]:
                     item['defindex'] = self.getWeaponSkinsList["pistolSkins"][str(item['paintkit'])]
                 elif 'rocket launcher' in name and str(item['paintkit']) in self.getWeaponSkinsList["rocketLauncherSkins"]:
                     item['defindex'] = self.getWeaponSkinsList["rocketLauncherSkins"][str(item['paintkit'])]
                 elif 'medi gun' in name and str(item['paintkit']) in self.getWeaponSkinsList["medicgunSkins"]:
                     item['defindex'] = self.getWeaponSkinsList["medicgunSkins"][str(item['paintkit'])]
@@ -672,29 +674,29 @@
                 number = name[len(withoutNumber) + 1:].strip()
                 name = name.split('#')[0].strip()
 
             if name in retiredKeysNames:
                 for retiredKey in retiredKeys:
                     if retiredKey['name'].lower() == name:
                         item["defindex"] = retiredKey["defindex"]
-                        item["quality"] = item.get["quality"] or 6
+                        item["quality"] = item.get("quality") or 6
                         return item
 
             schemaItem = self.getItemByNameWithThe(name)
             if not schemaItem: return item
             item["defindex"] = schemaItem["defindex"]
             item["quality"] = item.get("quality") or schemaItem.get("item_quality") # default quality
 
             # Fix defindex for Exclusive Genuine items
             if item["quality"] == 1:
                 if item["defindex"] in exclusiveGenuine:
                     item["defindex"] = exclusiveGenuine[item['defindex']]
 
             if schemaItem["item_class"] == "supply_crate":
-                item["crateseries"] = self.crateSeriesList[str(item["defindex"])]
+                item["crateseries"] = self.crateSeriesList.get(str(item["defindex"])) or None
             
             elif schemaItem["item_class"] != "supply_crate" and number is not None:
                 item["craftnumber"] = number
 
         return item
```

### Comparing `tf2-utilities-2.0.5/tf2utilities/sku.py` & `tf2-utilities-2.1.0/tf2utilities/sku.py`

 * *Files identical despite different names*

### Comparing `tf2-utilities-2.0.5/tf2utilities/webapi.py` & `tf2-utilities-2.1.0/tf2utilities/webapi.py`

 * *Files identical despite different names*

