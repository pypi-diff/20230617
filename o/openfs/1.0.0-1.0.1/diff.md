# Comparing `tmp/openfs-1.0.0-py3-none-any.whl.zip` & `tmp/openfs-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 9175 bytes, number of entries: 15
--rw-r--r--  2.0 unx      118 b- defN 23-Jun-17 02:16 openfs/__init__.py
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-16 06:23 openfs/_version.py
+Zip file size: 9893 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      118 b- defN 23-Jun-17 03:28 openfs/__init__.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-17 03:34 openfs/_version.py
 -rw-r--r--  2.0 unx       29 b- defN 23-Jun-16 06:15 openfs/boosters/__init__.py
 -rw-r--r--  2.0 unx     8575 b- defN 23-Jun-17 02:41 openfs/boosters/boosters.py
 -rw-r--r--  2.0 unx       21 b- defN 23-Jun-16 06:15 openfs/client/__init__.py
 -rw-r--r--  2.0 unx     2001 b- defN 23-Jun-16 06:45 openfs/client/client.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-17 02:16 openfs/gui/__init__.py
--rw-r--r--  2.0 unx     2996 b- defN 23-Jun-16 06:15 openfs/gui/gui.py
+-rw-r--r--  2.0 unx     3167 b- defN 23-Jun-17 03:40 openfs/gui/gui.py
 -rw-r--r--  2.0 unx       21 b- defN 23-Jun-16 06:15 openfs/stores/__init__.py
 -rw-r--r--  2.0 unx     3427 b- defN 23-Jun-17 02:41 openfs/stores/stores.py
--rw-r--r--  2.0 unx     1074 b- defN 23-Jun-17 02:42 openfs-1.0.0.dist-info/LICENCE
--rw-r--r--  2.0 unx     2991 b- defN 23-Jun-17 02:42 openfs-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-17 02:42 openfs-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jun-17 02:42 openfs-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1163 b- defN 23-Jun-17 02:42 openfs-1.0.0.dist-info/RECORD
-15 files, 22537 bytes uncompressed, 7255 bytes compressed:  67.8%
+-rw-r--r--  2.0 unx     1074 b- defN 23-Jun-17 03:42 openfs-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4263 b- defN 23-Jun-17 03:42 openfs-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-17 03:42 openfs-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-17 03:42 openfs-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1163 b- defN 23-Jun-17 03:42 openfs-1.0.1.dist-info/RECORD
+15 files, 23980 bytes uncompressed, 7973 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: openfs/stores/__init__.py
 Comment: 
 
 Filename: openfs/stores/stores.py
 Comment: 
 
-Filename: openfs-1.0.0.dist-info/LICENCE
+Filename: openfs-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: openfs-1.0.0.dist-info/METADATA
+Filename: openfs-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: openfs-1.0.0.dist-info/WHEEL
+Filename: openfs-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: openfs-1.0.0.dist-info/top_level.txt
+Filename: openfs-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: openfs-1.0.0.dist-info/RECORD
+Filename: openfs-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openfs/__init__.py

 * *Ordering differences only*

```diff
@@ -1,5 +1,5 @@
 from .client import Client
-from .gui.gui import gui_add_features
 from ._version import __version__
+from .gui.gui import gui_add_features
 
 client = Client()
```

## openfs/_version.py

```diff
@@ -1,2 +1,2 @@
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
```

## openfs/gui/gui.py

```diff
@@ -1,12 +1,18 @@
-import ipywidgets as widgets
 import time
-from ipywidgets import interactive
-from IPython.display import display, Code
-
+try:
+    import ipywidgets as widgets
+    from IPython.display import display, Code
+    from ipywidgets import interactive
+except ImportError:
+    print(
+        ("Optional dependencies are available. Use `pip install openfs[gui]`"
+        "to use the gui."
+        )
+        )
 
 def _gui_add(table_name, booster, metadata):
 
     # Use table_name to get the actual table from metadata
     table = next(
         (i for i in metadata["files"] if i["filename"] == table_name), None)
     if table is None:
```

## Comparing `openfs-1.0.0.dist-info/LICENCE` & `openfs-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `openfs-1.0.0.dist-info/RECORD` & `openfs-1.0.1.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-openfs/__init__.py,sha256=d1nEZl583L3HWrXUq9FtY5_5Mn7Vt-a57E4Z_cyoSPM,118
-openfs/_version.py,sha256=LwM61MmSdL4jyVluWPY8dHjusagjFagDKe9r3jDSWzo,22
+openfs/__init__.py,sha256=1BOiebMAMBG65xqSAUc-jPbdg0I8YOFjxmamE4AbiBA,118
+openfs/_version.py,sha256=gHQLL_1_UbHnOqTXuNHj0nJgl9mmypw_voEFhaHx75c,22
 openfs/boosters/__init__.py,sha256=ML6R2qmYi7HvDqb0JU_4Rg3PAvG9tLDvj7tttsxlzVA,29
 openfs/boosters/boosters.py,sha256=yVQuWw1CEeTcTkkbnraIGtTQna4Z-fLZ1pG7swljvTQ,8575
 openfs/client/__init__.py,sha256=tiVfgKlswRPaDMEy0gA7u8rveqEYZTA_kyB9lJ3J6Sc,21
 openfs/client/client.py,sha256=uVONFDuxCAalDvKQSjGhsufjOF7_JyFUYose3UOMXho,2001
 openfs/gui/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-openfs/gui/gui.py,sha256=C2WWR4OJR6r2BwwLMdP-dsk3zhX8Eszczx_sGgOzG8E,2996
+openfs/gui/gui.py,sha256=DGB0twGMHcezODI8qXxE9AOvrSUch5ZhoWB2HKAVMQc,3167
 openfs/stores/__init__.py,sha256=qWLyV6w6mUxUvo81mx9oOWZcNnPzi60rC2-sAmEwjt8,21
 openfs/stores/stores.py,sha256=wjiTd1l2IVWZVmtySjxRfbKIeeNssf1wplVegIwrcQw,3427
-openfs-1.0.0.dist-info/LICENCE,sha256=Sox9decnXsMjRIki7_sAwfVjfaNpJpqpiPbShfWe3sw,1074
-openfs-1.0.0.dist-info/METADATA,sha256=q70vQURjFOrKMLQTaUy1cUahJHs1zbfH4RLJXBQY4_w,2991
-openfs-1.0.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-openfs-1.0.0.dist-info/top_level.txt,sha256=fjXHUnBOPTosjMbrHtRq824mrq7ZBJXqTrPmRupIops,7
-openfs-1.0.0.dist-info/RECORD,,
+openfs-1.0.1.dist-info/LICENSE,sha256=Sox9decnXsMjRIki7_sAwfVjfaNpJpqpiPbShfWe3sw,1074
+openfs-1.0.1.dist-info/METADATA,sha256=UV2pbN0mnxqhMW7YLAi13Un6JbxTqGPtTI6gaubLDI0,4263
+openfs-1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+openfs-1.0.1.dist-info/top_level.txt,sha256=fjXHUnBOPTosjMbrHtRq824mrq7ZBJXqTrPmRupIops,7
+openfs-1.0.1.dist-info/RECORD,,
```

