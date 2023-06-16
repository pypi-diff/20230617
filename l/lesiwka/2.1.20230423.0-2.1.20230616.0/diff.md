# Comparing `tmp/lesiwka-2.1.20230423.0.tar.gz` & `tmp/lesiwka-2.1.20230616.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lesiwka-2.1.20230423.0.tar", last modified: Fri Apr 21 13:34:38 2023, max compression
+gzip compressed data, was "lesiwka-2.1.20230616.0.tar", last modified: Fri Jun 16 23:07:51 2023, max compression
```

## Comparing `lesiwka-2.1.20230423.0.tar` & `lesiwka-2.1.20230616.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:34:38.555656 lesiwka-2.1.20230423.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-21 13:34:38.555656 lesiwka-2.1.20230423.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:34:38.551656 lesiwka-2.1.20230423.0/lesiwka/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:34:38.555656 lesiwka-2.1.20230423.0/lesiwka/_decode/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18985 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/rule_1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/rule_1_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/rule_1_3.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/rule_1_4.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/rule_1_5.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/rule_1_6.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/rule_1_7.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/rule_2_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/rule_3_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/rule_3_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_decode/rule_3_4.py
--rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/ascii.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/diacritics.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/punctuation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/lesiwka/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:34:38.551656 lesiwka-2.1.20230423.0/lesiwka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-21 13:34:38.000000 lesiwka-2.1.20230423.0/lesiwka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-21 13:34:38.000000 lesiwka-2.1.20230423.0/lesiwka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:34:38.000000 lesiwka-2.1.20230423.0/lesiwka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-21 13:34:38.000000 lesiwka-2.1.20230423.0/lesiwka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 13:34:38.000000 lesiwka-2.1.20230423.0/lesiwka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-21 13:34:38.555656 lesiwka-2.1.20230423.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 13:34:26.000000 lesiwka-2.1.20230423.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:07:51.143426 lesiwka-2.1.20230616.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 23:07:51.143426 lesiwka-2.1.20230616.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:07:51.139426 lesiwka-2.1.20230616.0/lesiwka/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:07:51.143426 lesiwka-2.1.20230616.0/lesiwka/_decode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18985 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/rule_1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/rule_1_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/rule_1_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/rule_1_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/rule_1_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/rule_1_6.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/rule_1_7.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/rule_2_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/rule_3_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/rule_3_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_decode/rule_3_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12444 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/ascii.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/diacritics.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/punctuation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/lesiwka/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:07:51.139426 lesiwka-2.1.20230616.0/lesiwka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-16 23:07:51.000000 lesiwka-2.1.20230616.0/lesiwka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-16 23:07:51.000000 lesiwka-2.1.20230616.0/lesiwka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 23:07:51.000000 lesiwka-2.1.20230616.0/lesiwka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 23:07:51.000000 lesiwka-2.1.20230616.0/lesiwka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 23:07:51.000000 lesiwka-2.1.20230616.0/lesiwka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-16 23:07:51.143426 lesiwka-2.1.20230616.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 23:07:42.000000 lesiwka-2.1.20230616.0/setup.py
```

### Comparing `lesiwka-2.1.20230423.0/LICENSE` & `lesiwka-2.1.20230616.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lesiwka-2.1.20230423.0/PKG-INFO` & `lesiwka-2.1.20230616.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lesiwka
-Version: 2.1.20230423.0
+Version: 2.1.20230616.0
 Summary: Python library to convert to/from Lesivka
 Author: Oleksandr Tishyn
 Author-email: 1079805+Mystic-Mirage@users.noreply.github.com
 License: CC0 1.0 Universal
 Project-URL: Source Code, https://github.com/lesiwka/python-lesiwka
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `lesiwka-2.1.20230423.0/lesiwka/__main__.py` & `lesiwka-2.1.20230616.0/lesiwka/__main__.py`

 * *Files identical despite different names*

### Comparing `lesiwka-2.1.20230423.0/lesiwka/_decode/__init__.py` & `lesiwka-2.1.20230616.0/lesiwka/_decode/__init__.py`

 * *Files identical despite different names*

### Comparing `lesiwka-2.1.20230423.0/lesiwka/_decode/postprocess.py` & `lesiwka-2.1.20230616.0/lesiwka/_decode/postprocess.py`

 * *Files identical despite different names*

### Comparing `lesiwka-2.1.20230423.0/lesiwka/_decode/preprocess.py` & `lesiwka-2.1.20230616.0/lesiwka/_decode/preprocess.py`

 * *Files identical despite different names*

### Comparing `lesiwka-2.1.20230423.0/lesiwka/_decode/rule_2_2.py` & `lesiwka-2.1.20230616.0/lesiwka/_decode/rule_2_2.py`

 * *Files identical despite different names*

### Comparing `lesiwka-2.1.20230423.0/lesiwka/_encode.py` & `lesiwka-2.1.20230616.0/lesiwka/_encode.py`

 * *Files 10% similar despite different names*

```diff
@@ -238,14 +238,75 @@
     ("ЮУАЕС", "JuUAES"),
     ("ЮФ", "JuF"),
     ("ЯМР", "JaMR"),
     ("еВ", "eV"),
     ("вт", "vt"),
     ("Вт", "Vt"),
     ("ВТ", "VT"),
+    ("АВК", "AVK"),
+    ("АВН", "AVN"),
+    ("АВС", "AVS"),
+    ("АСУВ", "ASUV"),
+    ("БДЖ", "BĐŽ"),
+    ("БЄК", "BJeK"),
+    ("ВЯВ", "VJaV"),
+    ("ДЗЗСЄ", "DZZSJe"),
+    ("Дз", "Dz"),
+    ("дз", "dz"),
+    ("ДПРОВТ", "DPROVT"),
+    ("ДРЖ", "ĐRŽ"),
+    ("ЕВП", "EVP"),
+    ("ЄАІС", "JeAIS"),
+    ("ЄАМЗ", "JeAMZ"),
+    ("ЄАСЗ", "JeASZ"),
+    ("ЄАСК", "JeASK"),
+    ("ЄАСУ", "JeASU"),
+    ("ЄБК", "JeBK"),
+    ("ЄКНС", "JeKNS"),
+    ("ЄСВОН", "JeSVON"),
+    ("ЄСКБ", "JeSKB"),
+    ("ЄСКС", "JeSKS"),
+    ("ЄССЗ", "JeCCZ"),
+    ("ЄСУБ", "JeSUB"),
+    ("ЗАВЗ", "ZAVZ"),
+    ("ЗВОВС", "ZVOVS"),
+    ("ЗВЯЗ", "ZVJaZ"),
+    ("ЗЕРАВ", "ZERAV"),
+    ("ІВ", "IV"),
+    ("КЗАУВ", "KZAUV"),
+    ("КІВ", "KIV"),
+    ("МСЯС", "MSJaS"),
+    ("ОВ", "OV"),
+    ("ОВСТ", "OVST"),
+    ("ОСУВ", "OSUV"),
+    ("ОУВ", "OUV"),
+    ("ОЯП", "OJaP"),
+    ("ПСЯБ", "PSJaB"),
+    ("ПУВ", "PUV"),
+    ("РЯЗ", "RJaZ"),
+    ("РЯН", "RJaN"),
+    ("РЯО", "RJaO"),
+    ("СУВ", "SUV"),
+    ("СЯС", "SJaS"),
+    ("УВ", "UV"),
+    ("УВС", "UVS"),
+    ("УВФ", "UVF"),
+    ("ХДС", "XĐS"),
+    ("ЯБВ", "JaBV"),
+    ("ЯБП", "JaBP"),
+    ("ЯБЧ", "JaBČ"),
+    ("ЯВ", "JaV"),
+    ("ЯЕУ", "JaEU"),
+    ("ЯЗ", "JaZ"),
+    ("ЯЗК", "JaZK"),
+    ("ЯМ", "JaM"),
+    ("ЯРМД", "JaRMD"),
+    ("ЯРР", "JaRR"),
+    ("ЯРСД", "JaRSD"),
+    ("ЯФ", "JaF"),
 )
 abbr_dot_pattern = (
     r"(?i:(?<=\b)|(?<=\b(г|з|і|к|с))|(?<=\b(ди|за|ін|по|св))|"
     r"(?<=\b(про|сло))|(?<=\b(буль|пере|родо))){0}(?=\.)"
 )
 
 w_pattern = (
@@ -281,14 +342,15 @@
         r"(?i:((?<=\bбу)|(?<=\bзагоро)|(?<=\bме)|(?<=\bпро)|(?<=\bсту)))"
         r"{0}(?i:(?=заг[іо]н))"
     ),
     r"(?i:((?<=\bвищеві)|(?<=\bкінові)|(?<=\bлітві)|(?<=\bра)|(?<=\bспецві)))"
     r"{0}(?i:(?=зна[кч]))",
     r"(?i:(?<=епі)){0}(?i:(?=зах[іо]д))",
     r"(?i:(?<=пі)){0}(?i:(?=жи[вw]))",
+    r"(?<=\b){0}(?i:(?=зо[cт]))",
 )
 affricate_pattern_1 = r"(?i:(?<=\bпере)){0}(?i:з)(?i:(?=вен|він|вон|ижч))"
 affricate_pattern_2 = (
     r"(?i:(?!(?<=\bві)|(?<=\bна)|(?<=\bо)|(?<=\bпере)|(?<=\bпі)|(?<=\bпона)|"
     r"(?<=\bпопі)|(?<=\bпре)|(?<=\bсере)|(?<=\bневі)|(?<=\bнепі)|(?<=\bнапере)"
     r"|(?<=\bопі))){0}"
 )
```

### Comparing `lesiwka-2.1.20230423.0/lesiwka/ascii.py` & `lesiwka-2.1.20230616.0/lesiwka/ascii.py`

 * *Files identical despite different names*

### Comparing `lesiwka-2.1.20230423.0/lesiwka/utils.py` & `lesiwka-2.1.20230616.0/lesiwka/utils.py`

 * *Files identical despite different names*

### Comparing `lesiwka-2.1.20230423.0/lesiwka.egg-info/PKG-INFO` & `lesiwka-2.1.20230616.0/lesiwka.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lesiwka
-Version: 2.1.20230423.0
+Version: 2.1.20230616.0
 Summary: Python library to convert to/from Lesivka
 Author: Oleksandr Tishyn
 Author-email: 1079805+Mystic-Mirage@users.noreply.github.com
 License: CC0 1.0 Universal
 Project-URL: Source Code, https://github.com/lesiwka/python-lesiwka
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `lesiwka-2.1.20230423.0/lesiwka.egg-info/SOURCES.txt` & `lesiwka-2.1.20230616.0/lesiwka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lesiwka-2.1.20230423.0/setup.cfg` & `lesiwka-2.1.20230616.0/setup.cfg`

 * *Files identical despite different names*

