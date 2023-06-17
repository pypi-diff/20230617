# Comparing `tmp/pk4adi-0.1.0.tar.gz` & `tmp/pk4adi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pk4adi-0.1.0.tar", last modified: Sat Jun 17 07:24:33 2023, max compression
+gzip compressed data, was "pk4adi-0.1.1.tar", last modified: Sat Jun 17 08:25:35 2023, max compression
```

## Comparing `pk4adi-0.1.0.tar` & `pk4adi-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 07:24:33.214684 pk4adi-0.1.0/
--rw-rw-rw-   0        0        0     1088 2023-01-04 20:12:34.000000 pk4adi-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     7471 2023-06-17 07:24:33.213150 pk4adi-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     6551 2023-06-17 07:17:09.000000 pk4adi-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 07:24:33.179894 pk4adi-0.1.0/pk4adi/
--rw-rw-rw-   0        0        0      458 2023-06-16 10:10:12.000000 pk4adi-0.1.0/pk4adi/__init__.py
--rw-rw-rw-   0        0        0     9771 2023-06-17 06:56:44.000000 pk4adi-0.1.0/pk4adi/pk.py
--rw-rw-rw-   0        0        0     7997 2023-06-17 06:56:08.000000 pk4adi-0.1.0/pk4adi/pkc.py
--rw-rw-rw-   0        0        0     1143 2023-06-17 06:56:55.000000 pk4adi-0.1.0/pk4adi/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-17 07:24:33.211672 pk4adi-0.1.0/pk4adi.egg-info/
--rw-rw-rw-   0        0        0     7471 2023-06-17 07:24:33.000000 pk4adi-0.1.0/pk4adi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-17 07:24:33.000000 pk4adi-0.1.0/pk4adi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 07:24:33.000000 pk4adi-0.1.0/pk4adi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-17 07:24:33.000000 pk4adi-0.1.0/pk4adi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-17 07:24:33.000000 pk4adi-0.1.0/pk4adi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 07:24:33.214684 pk4adi-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2017 2023-06-17 07:14:57.000000 pk4adi-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 08:25:35.152740 pk4adi-0.1.1/
+-rw-rw-rw-   0        0        0     1088 2023-01-04 20:12:34.000000 pk4adi-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     8227 2023-06-17 08:25:35.152244 pk4adi-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7545 2023-06-17 08:02:23.000000 pk4adi-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 08:25:35.122940 pk4adi-0.1.1/pk4adi/
+-rw-rw-rw-   0        0        0      282 2023-06-17 08:01:07.000000 pk4adi-0.1.1/pk4adi/__init__.py
+-rw-rw-rw-   0        0        0     9589 2023-06-17 08:00:07.000000 pk4adi-0.1.1/pk4adi/pk.py
+-rw-rw-rw-   0        0        0     7821 2023-06-17 08:00:17.000000 pk4adi-0.1.1/pk4adi/pkc.py
+-rw-rw-rw-   0        0        0      968 2023-06-17 08:00:25.000000 pk4adi-0.1.1/pk4adi/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-17 08:25:35.150753 pk4adi-0.1.1/pk4adi.egg-info/
+-rw-rw-rw-   0        0        0     8227 2023-06-17 08:25:35.000000 pk4adi-0.1.1/pk4adi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-17 08:25:35.000000 pk4adi-0.1.1/pk4adi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 08:25:35.000000 pk4adi-0.1.1/pk4adi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-17 08:25:35.000000 pk4adi-0.1.1/pk4adi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-17 08:25:35.000000 pk4adi-0.1.1/pk4adi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 08:25:35.152740 pk4adi-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1841 2023-06-17 08:00:35.000000 pk4adi-0.1.1/setup.py
```

### Comparing `pk4adi-0.1.0/LICENSE` & `pk4adi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pk4adi-0.1.0/PKG-INFO` & `pk4adi-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pk4adi
-Version: 0.1.0
+Version: 0.1.1
 Summary: Using PK to Measure the Performance of Anesthetic Depth Indicators.
 Home-page: https://github.com/xfz329/pk.git
 Author: silencejiang
 Author-email: silencejiang@zju.edu.cn
 License: MIT License
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,15 @@
 
 # pk4adi
 
 ## Project Information
 
 The package's name pk4adi is short for "PK for anesthetic depth indicators". The PK (Prediction probability) was firstly proposed by [Docor Warren D. Smith](https://www.csus.edu/faculty/s/smithwd/) in the paper [Measuring the Performance of Anesthetic Depth Indicators](https://pubs.asahq.org/anesthesiology/article/84/1/38/35261/Measuring-the-Performance-of-Anesthetic-Depth) in 1996. Docor Warren D. Smith and his team provide a tool to calculate PK writen using the xls macro language.
 
-Our team provide a reimplementation of the PK tools developed using the Python language with easy using apis in this package. The project is fully open source in the [github](https://github.com/xfz329/pk). The lastest version 0.1.0 released on June 17, 2023. 
+Our team provide a reimplementation of the PK tools developed using the Python language with easy using apis in this package. The project is fully open source in the [github](https://github.com/xfz329/pk). The lastest version released could be found [here](https://github.com/xfz329/pk/releases). 
 
 Please feel free to contact us(silencejiang@zju.edu.cn). Any kind of feedbacks is welcomed. You could report any bugs or issues when using pk4adi in the github [project](https://github.com/xfz329/pk/issues).
 
 Specially, a gui version of pk4adi is under development. We will also open source the gui version project.
 
 ## Changelogs
 
@@ -152,17 +152,19 @@
 ### 1. calculate PK
 
 ```python
 from pk4adi.pk import calculate_pk
 
 x = [ 0, 0, 0, 0, 0, 0]
 y = [ 1, 1, 1, 1, 1, 2]
+calculate_pk(x, y)
 
-pk = PK()
-pk.calculate_pk(x_in=x, y_in=y)
+x = [0, 0, 0, 0, 0, 0, 1, 1, 2]
+y = [1, 1, 1, 1, 1, 2, 3, 3, 4]
+calculate_pk(x, y)
 ```
 You will get the following output.
 ```
 ==============
 PK calculation
 ==============
 
@@ -236,14 +238,27 @@
 =================
 
   PKDJ    SEDJ    DF     TD    P value  Comment
 ------  ------  ----  -----  ---------  ---------
  0.030   0.066    23  0.453      0.327  P > 0.05
 ```
 
+### 3. more details
+You could get the all the matrix and variables in the returned dicts of the function calculate_pk() and compare_pks().
+```python
+print(pk1.keys())
+print(ans.keys())
+```
+You will get the following output.
+```
+dict_keys(['type', 'A', 'S', 'C', 'D', 'T', 'SA', 'CA', 'DA', 'TA', 'jack_ok', 'n_case', 'n', 'Qc', 'Qd', 'Qtx', 'Qcdt', 'dyx', 'PK', 'Qcc', 'Qdd', 'Qcd', 'Term1', 'Term2', 'Term3', 'SE1', 'SE0', 'PKm', 'SPKm', 'SSPKm', 'PKj', 'SEj'])
+dict_keys(['type', 'n_case', 'PKD', 'SED', 'ZD', 'ZP', 'ZJ', 'PKmD', 'SumD', 'SSD', 'DF', 'PKDJ', 'SEDJ', 'TD', 'TP', 'TJ'])
+```
+Then just get the value with the key of the dict!
+
 # Development
 
 ## Contribute
 
 Please feel free to contact us(silencejiang@zju.edu.cn). Any kind of feedbacks is welcomed and appreciated.
 - Check out the wiki for development info (coming soon!).
 - Fork us from @xfz329's [main](https://github.com/xfz329/pk).
```

### Comparing `pk4adi-0.1.0/pk4adi/pk.py` & `pk4adi-0.1.1/pk4adi/pk.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 """
 @File    :   pk.py
 @Contact :   Jiang Feng(silencejiang@zju.edu.cn)
 @License :   (C)Copyright 2004-2020, Zhejiang University
-
-@Modify Time        @Author       @Version    @Desciption
-------------        -------       --------    -----------
-2023/6/13 20:56   silencejiang      0.1.0         None
 """
 
 import math
 import pandas as pd
 import numpy as np
 from pk4adi.utils import print_table
 
@@ -308,9 +304,9 @@
 
     x = [ 0, 0, 0, 0, 0, 0]
     y = [ 1, 1, 1, 1, 1, 2]
     calculate_pk(x, y)
 
     x = [0, 0, 0, 0, 0, 0, 1, 1, 2]
     y = [1, 1, 1, 1, 1, 2, 3, 3, 4]
-    ans = calculate_pk(x, y)
+    calculate_pk(x, y)
```

### Comparing `pk4adi-0.1.0/pk4adi/pkc.py` & `pk4adi-0.1.1/pk4adi/pkc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 """
 @File    :   pkc.py
 @Contact :   Jiang Feng(silencejiang@zju.edu.cn)
 @License :   (C)Copyright 2004-2020, Zhejiang University
-
-@Modify Time        @Author       @Version    @Desciption
-------------        -------       --------    -----------
-2023/6/13 16:20   silencejiang      0.1.0         None
 """
 
 import math
 import pandas as pd
 from scipy.stats import norm, t
 from pk4adi.utils import print_table
 from pk4adi.pk import calculate_pk
```

### Comparing `pk4adi-0.1.0/pk4adi/utils.py` & `pk4adi-0.1.1/pk4adi/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 """
 @File    :   utils.py    
 @Contact :   Jiang Feng(silencejiang@zju.edu.cn)
 @License :   (C)Copyright 2004-2020, Zhejiang University
-
-@Modify Time        @Author       @Version    @Desciption
-------------        -------       --------    -----------
-2023/6/16 1:03   silencejiang      0.1.0         None
 """
 
 
 from tabulate import tabulate
 
 __all__ = ["print_table"]
```

### Comparing `pk4adi-0.1.0/pk4adi.egg-info/PKG-INFO` & `pk4adi-0.1.1/pk4adi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pk4adi
-Version: 0.1.0
+Version: 0.1.1
 Summary: Using PK to Measure the Performance of Anesthetic Depth Indicators.
 Home-page: https://github.com/xfz329/pk.git
 Author: silencejiang
 Author-email: silencejiang@zju.edu.cn
 License: MIT License
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,15 @@
 
 # pk4adi
 
 ## Project Information
 
 The package's name pk4adi is short for "PK for anesthetic depth indicators". The PK (Prediction probability) was firstly proposed by [Docor Warren D. Smith](https://www.csus.edu/faculty/s/smithwd/) in the paper [Measuring the Performance of Anesthetic Depth Indicators](https://pubs.asahq.org/anesthesiology/article/84/1/38/35261/Measuring-the-Performance-of-Anesthetic-Depth) in 1996. Docor Warren D. Smith and his team provide a tool to calculate PK writen using the xls macro language.
 
-Our team provide a reimplementation of the PK tools developed using the Python language with easy using apis in this package. The project is fully open source in the [github](https://github.com/xfz329/pk). The lastest version 0.1.0 released on June 17, 2023. 
+Our team provide a reimplementation of the PK tools developed using the Python language with easy using apis in this package. The project is fully open source in the [github](https://github.com/xfz329/pk). The lastest version released could be found [here](https://github.com/xfz329/pk/releases). 
 
 Please feel free to contact us(silencejiang@zju.edu.cn). Any kind of feedbacks is welcomed. You could report any bugs or issues when using pk4adi in the github [project](https://github.com/xfz329/pk/issues).
 
 Specially, a gui version of pk4adi is under development. We will also open source the gui version project.
 
 ## Changelogs
 
@@ -152,17 +152,19 @@
 ### 1. calculate PK
 
 ```python
 from pk4adi.pk import calculate_pk
 
 x = [ 0, 0, 0, 0, 0, 0]
 y = [ 1, 1, 1, 1, 1, 2]
+calculate_pk(x, y)
 
-pk = PK()
-pk.calculate_pk(x_in=x, y_in=y)
+x = [0, 0, 0, 0, 0, 0, 1, 1, 2]
+y = [1, 1, 1, 1, 1, 2, 3, 3, 4]
+calculate_pk(x, y)
 ```
 You will get the following output.
 ```
 ==============
 PK calculation
 ==============
 
@@ -236,14 +238,27 @@
 =================
 
   PKDJ    SEDJ    DF     TD    P value  Comment
 ------  ------  ----  -----  ---------  ---------
  0.030   0.066    23  0.453      0.327  P > 0.05
 ```
 
+### 3. more details
+You could get the all the matrix and variables in the returned dicts of the function calculate_pk() and compare_pks().
+```python
+print(pk1.keys())
+print(ans.keys())
+```
+You will get the following output.
+```
+dict_keys(['type', 'A', 'S', 'C', 'D', 'T', 'SA', 'CA', 'DA', 'TA', 'jack_ok', 'n_case', 'n', 'Qc', 'Qd', 'Qtx', 'Qcdt', 'dyx', 'PK', 'Qcc', 'Qdd', 'Qcd', 'Term1', 'Term2', 'Term3', 'SE1', 'SE0', 'PKm', 'SPKm', 'SSPKm', 'PKj', 'SEj'])
+dict_keys(['type', 'n_case', 'PKD', 'SED', 'ZD', 'ZP', 'ZJ', 'PKmD', 'SumD', 'SSD', 'DF', 'PKDJ', 'SEDJ', 'TD', 'TP', 'TJ'])
+```
+Then just get the value with the key of the dict!
+
 # Development
 
 ## Contribute
 
 Please feel free to contact us(silencejiang@zju.edu.cn). Any kind of feedbacks is welcomed and appreciated.
 - Check out the wiki for development info (coming soon!).
 - Fork us from @xfz329's [main](https://github.com/xfz329/pk).
```

### Comparing `pk4adi-0.1.0/setup.py` & `pk4adi-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 """
 @File    :   setup.py
 @Contact :   Jiang Feng(silencejiang@zju.edu.cn)
 @License :   (C)Copyright 2004-2020, Zhejiang University
-
-@Modify Time        @Author       @Version    @Desciption
-------------        -------       --------    -----------
-2023/6/13 16:20   silencejiang      0.1.0         None
 """
 
 
 import os
 import re
 from setuptools import setup, find_packages
```

