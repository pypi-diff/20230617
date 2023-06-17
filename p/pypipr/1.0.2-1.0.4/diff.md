# Comparing `tmp/pypipr-1.0.2.tar.gz` & `tmp/pypipr-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypipr-1.0.2.tar", max compression
+gzip compressed data, was "pypipr-1.0.4.tar", max compression
```

## Comparing `pypipr-1.0.2.tar` & `pypipr-1.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    34252 2023-06-16 08:34:35.919415 pypipr-1.0.2/README.md
--rw-r--r--   0        0        0        0 2023-06-16 07:50:31.475417 pypipr-1.0.2/pypipr/__init__.py
--rw-r--r--   0        0        0    43701 2023-06-16 07:50:31.479416 pypipr-1.0.2/pypipr/pypipr.py
--rw-r--r--   0        0        0      538 2023-06-16 08:34:38.779415 pypipr-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    34657 1970-01-01 00:00:00.000000 pypipr-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    33945 2023-06-17 12:17:18.239399 pypipr-1.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-16 19:13:28.991476 pypipr-1.0.4/pypipr/__init__.py
+-rw-r--r--   0        0        0    43832 2023-06-16 20:16:42.367474 pypipr-1.0.4/pypipr/pypipr.py
+-rw-r--r--   0        0        0      498 2023-06-17 12:17:23.459399 pypipr-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    34600 1970-01-01 00:00:00.000000 pypipr-1.0.4/PKG-INFO
```

### Comparing `pypipr-1.0.2/README.md` & `pypipr-1.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: pypipr
+Version: 1.0.4
+Summary: The Python Package Index Project
+Author: ufiapjj
+Author-email: ufiapjj@gmail.com
+Requires-Python: >=3.9
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: black
+Requires-Dist: colorama
+Requires-Dist: cssselect
+Requires-Dist: getch ; platform_system == "Linux"
+Requires-Dist: lxml
+Requires-Dist: pint
+Requires-Dist: pytest
+Requires-Dist: pyyaml
+Requires-Dist: requests
+Requires-Dist: tzdata
+Description-Content-Type: text/markdown
+
 
 # About
 The Python Package Index Project (pypipr)
 
 pypi : https://pypi.org/project/pypipr
 
 
@@ -72,15 +95,15 @@
 s = "Urutan {1/6/3} dan {10:9} dan {j k} dan {Z - A - 15} saja."  
 print(generator.batchmaker(s))  
 print(batchmaker(s))  
 ```
 
 Output:
 ```py
-<generator object generator.batchmaker at 0x7c61eb7d00>
+<generator object generator.batchmaker at 0x74c82c3d00>
 ('Urutan 1 dan 10 dan j dan Z saja.', 'Urutan 1 dan 10 dan j dan K saja.', 'Urutan 1 dan 10 dan k dan Z saja.', 'Urutan 1 dan 10 dan k dan K saja.', 'Urutan 1 dan 9 dan j dan Z saja.', 'Urutan 1 dan 9 dan j dan K saja.', 'Urutan 1 dan 9 dan k dan Z saja.', 'Urutan 1 dan 9 dan k dan K saja.', 'Urutan 4 dan 10 dan j dan Z saja.', 'Urutan 4 dan 10 dan j dan K saja.', 'Urutan 4 dan 10 dan k dan Z saja.', 'Urutan 4 dan 10 dan k dan K saja.', 'Urutan 4 dan 9 dan j dan Z saja.', 'Urutan 4 dan 9 dan j dan K saja.', 'Urutan 4 dan 9 dan k dan Z saja.', 'Urutan 4 dan 9 dan k dan K saja.')
 ```
 
 ## calculate
 
 `calculate`
 
@@ -125,15 +148,15 @@
 array = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(generator.chunck_array(array, 5))  
 print(chunck_array(array, 5))  
 ```
 
 Output:
 ```py
-<generator object generator.chunck_array at 0x7c61f7fe40>
+<generator object generator.chunck_array at 0x74c8167e40>
 ([2, 3, 12, 3, 3], [42, 42, 1, 43, 2], [42, 41, 4, 24, 32], [42, 3, 12, 32, 42], [42])
 ```
 
 ## console_run
 
 `console_run`
 
@@ -184,17 +207,17 @@
 print(datetime_now("Asia/Jakarta"))  
 print(datetime_now("GMT"))  
 print(datetime_now("Etc/GMT+7"))  
 ```
 
 Output:
 ```py
-2023-06-16 15:34:30.771887+07:00
-2023-06-16 08:34:30.773421+00:00
-2023-06-16 01:34:30.778299-07:00
+2023-06-17 19:17:16.635844+07:00
+2023-06-17 12:17:16.637459+00:00
+2023-06-17 05:17:16.641513-07:00
 ```
 
 ## dict_first
 
 `dict_first`
 
 Mengambil nilai (key, value) pertama dari dictionary dalam bentuk tuple.  
@@ -285,45 +308,45 @@
         return [x for x in range(10)]  
 
 print(get_class_method(ExampleGetClassMethod))  
 ```
 
 Output:
 ```py
-(<function ExampleGetClassMethod.a at 0x7c61d428e0>, <function ExampleGetClassMethod.b at 0x7c61d42840>, <function ExampleGetClassMethod.c at 0x7c61d42a20>, <function ExampleGetClassMethod.d at 0x7c61d42ac0>)
+(<function ExampleGetClassMethod.a at 0x74c813e840>, <function ExampleGetClassMethod.b at 0x74c813e7a0>, <function ExampleGetClassMethod.c at 0x74c813e980>, <function ExampleGetClassMethod.d at 0x74c813ea20>)
 ```
 
 ## get_filemtime
 
 `get_filemtime`
 
 Mengambil informasi last modification time file dalam nano seconds  
 
 ```python  
 print(get_filemtime(__file__))  
 ```
 
 Output:
 ```py
-1686901831479416922
+1686946602367473992
 ```
 
 ## get_filesize
 
 `get_filesize`
 
 Mengambil informasi file size dalam bytes  
 
 ```python  
 print(get_filesize(__file__))  
 ```
 
 Output:
 ```py
-43701
+43832
 ```
 
 ## github_pull
 
 `github_pull`
 
 Menjalankan command `git pull`  
@@ -377,15 +400,15 @@
 print(implode(arr, separator='</li>\n<li>', start='<li>', end='</li>', recursive_flat=True))  
 print(implode(arr, separator='</div>\n<div>', start='<div>', end='</div>'))  
 print(implode(10, ' '))  
 ```
 
 Output:
 ```py
-qweqw, asd, dfs, weq
+weq, asd, dfs, qweqw
 ,ini,path,seperti,url,
 ini,path,seperti,url
 <li>satu</li>
 <li>12</li>
 <li>34</li>
 <li>56</li>
 <li>tiga</li>
@@ -445,15 +468,15 @@
 print(iopen("https://www.google.com/", dict(coba="dulu"), xpath="//a"))  
 ```
 
 Output:
 ```py
 8
 ['mana', 'aja']
-[<Element a at 0x7c631948c0>, <Element a at 0x7c61e23d40>, <Element a at 0x7c61ba3430>, <Element a at 0x7c61ba34d0>, <Element a at 0x7c61ba3520>, <Element a at 0x7c61ba3570>, <Element a at 0x7c61ba35c0>, <Element a at 0x7c61ba3610>, <Element a at 0x7c61ba3660>, <Element a at 0x7c61ba36b0>, <Element a at 0x7c61ba3700>, <Element a at 0x7c61ba3750>, <Element a at 0x7c61ba37a0>, <Element a at 0x7c61ba37f0>, <Element a at 0x7c61ba3840>, <Element a at 0x7c61ba3890>, <Element a at 0x7c61ba38e0>, <Element a at 0x7c61ba3930>]
+[<Element a at 0x74c821ef30>, <Element a at 0x74c821f9d0>, <Element a at 0x74c7fbf160>, <Element a at 0x74c7fbf200>, <Element a at 0x74c7fbf250>, <Element a at 0x74c7fbf2a0>, <Element a at 0x74c7fbf2f0>, <Element a at 0x74c7fbf340>, <Element a at 0x74c7fbf390>, <Element a at 0x74c7fbf3e0>, <Element a at 0x74c7fbf430>, <Element a at 0x74c7fbf480>, <Element a at 0x74c7fbf4d0>, <Element a at 0x74c7fbf520>, <Element a at 0x74c7fbf570>, <Element a at 0x74c7fbf5c0>, <Element a at 0x74c7fbf610>, <Element a at 0x74c7fbf660>]
 False
 ```
 
 ## irange
 
 `irange`
 
@@ -467,15 +490,15 @@
 # print(irange('a', 5, 3))  
 print(irange(-10, 4, 3))  
 print(irange(1, 5))  
 ```
 
 Output:
 ```py
-<generator object generator.irange at 0x7c64594bf0>
+<generator object generator.irange at 0x74ca994bf0>
 ['H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z', '[', '\\', ']', '^', '_', '`', 'a']
 ['1', '4']
 [1, 4]
 [-10, -7, -4, -1, 2]
 [1, 2, 3, 4, 5]
 ```
 
@@ -562,16 +585,16 @@
 ```python  
 print(generator.iscandir())  
 print(iscandir("./", recursive=False, scan_file=False))  
 ```
 
 Output:
 ```py
-<generator object generator.iscandir at 0x7c61f7e040>
-(PosixPath('.vscode'), PosixPath('pypipr'), PosixPath('dist'), PosixPath('.git'))
+<generator object generator.iscandir at 0x74c8166040>
+(PosixPath('.git'), PosixPath('.vscode'), PosixPath('pypipr'), PosixPath('dist'))
 ```
 
 ## log
 
 `log`
 
 Decorator untuk mempermudah pembuatan log karena tidak perlu mengubah fungsi yg sudah ada.  
@@ -625,29 +648,29 @@
              __doc__ : Path subclass for non-Windows systems.
 
     On a POSIX system, instantiating a Path should return this object.
     
            __enter__ : https:/www.google.com
           __fspath__ : https:/www.google.com
         __getstate__ : (None, {'_drv': '', '_root': '', '_parts': ['https:', 'www.google.com'], '_str': 'https:/www.google.com'})
-            __hash__ : 4473962716942053088
+            __hash__ : -6965287676073568923
             __init__ : None
    __init_subclass__ : None
           __module__ : pathlib
           __reduce__ : (<class 'pathlib.PosixPath'>, ('https:', 'www.google.com'))
             __repr__ : PosixPath('https:/www.google.com')
           __sizeof__ : 72
            __slots__ : ()
              __str__ : https:/www.google.com
     __subclasshook__ : NotImplemented
       _cached_cparts : ['https:', 'www.google.com']
              _cparts : ['https:', 'www.google.com']
                 _drv : 
-            _flavour : <pathlib._PosixFlavour object at 0x7c6393dd10>
-               _hash : 4473962716942053088
+            _flavour : <pathlib._PosixFlavour object at 0x74c9d41dd0>
+               _hash : -6965287676073568923
               _parts : ['https:', 'www.google.com']
                _root : 
                 _str : https:/www.google.com
             absolute : /data/data/com.termux/files/home/pypipr/https:/www.google.com
               anchor : 
             as_posix : https:/www.google.com
                  cwd : /data/data/com.termux/files/home/pypipr
@@ -661,15 +684,15 @@
               is_dir : False
              is_fifo : False
              is_file : False
             is_mount : False
          is_reserved : False
            is_socket : False
           is_symlink : False
-             iterdir : <generator object Path.iterdir at 0x7c61d47060>
+             iterdir : <generator object Path.iterdir at 0x74c8143060>
             joinpath : https:/www.google.com
                 name : www.google.com
               parent : https:
              parents : <PosixPath.parents>
                parts : ('https:', 'www.google.com')
              resolve : /data/data/com.termux/files/home/pypipr/https:/www.google.com
                 root : 
@@ -700,15 +723,15 @@
 
 ```python  
 print(random_bool())  
 ```
 
 Output:
 ```py
-False
+True
 ```
 
 ## serialize
 
 `serialize`
 
 Mengubah variabel data menjadi string untuk yang dapat dibaca untuk disimpan.  
@@ -891,15 +914,15 @@
 print(x)  
 print("menghentikan timeout 7")  
 x.cancel()  
 ```
 
 Output:
 ```py
-<Timer(Thread-2, started 534192831744)>
+<Timer(Thread-2, started 501548563712)>
 menghentikan timeout 7
 ```
 
 ## sets_ordered
 
 `sets_ordered`
 
@@ -909,15 +932,15 @@
 array = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(generator.sets_ordered(array))  
 print(sets_ordered(array))  
 ```
 
 Output:
 ```py
-<generator object generator.sets_ordered at 0x7c61d86810>
+<generator object generator.sets_ordered at 0x74c8182810>
 [2, 3, 12, 42, 1, 43, 41, 4, 24, 32]
 ```
 
 ## str_cmp
 
 `str_cmp`
 
@@ -1017,191 +1040,166 @@
 pprint.pprint(unserialize_html(iopen("https://harga-emas.org/")), depth=10)  
 pprint.pprint(unserialize_html(iopen("https://harga-emas.org/1-gram/")), depth=10)  
 ```
 
 Output:
 ```py
 (['Home', 'Emas 1 Gram', 'History', 'Trend', 'Perak 1 Gram'],
- [['Harga Emas Hari Ini - Jumat, 16 Juni 2023'],
-  ['Spot Emas USD↑1.961,18 (+1,93) / oz',
+ [['Harga Emas Hari Ini - Sabtu, 17 Juni 2023'],
+  ['Spot Emas USD↑1.957,84 (+3,32) / oz',
    'Kurs IDR15.140,00 / USD',
-   'Emas IDR↑954.628 (+939) / gr'],
-  ['LM Antam (Jual)↑1.061.000 (+9.000) / gr',
-   'LM Antam (Beli)↑942.000 (+9.000) / gr']],
+   'Emas IDR↑953.003 (+1.616) / gr'],
+  ['LM Antam (Jual)↑1.063.000 (+2.000) / gr',
+   'LM Antam (Beli)↑945.000 (+3.000) / gr']],
  [['Harga Emas Hari Ini'],
   ['Gram', 'Gedung Antam Jakarta', 'Pegadaian'],
   ['per Gram (Rp)', 'per Batangan (Rp)', 'per Gram (Rp)', 'per Batangan (Rp)'],
   ['1000',
-   '1.002 (+9)',
-   '1.001.600 (+9.000)',
-   '1.017.415 (-1.025)',
-   '1.017.415.000 (-1.025.000)'],
+   '1.004 (+2)',
+   '1.003.600 (+2.000)',
+   '1.026.640 (+9.225)',
+   '1.026.640.000 (+9.225.000)'],
   ['500',
-   '2.003 (+18)',
-   '1.001.640 (+9.000)',
-   '1.017.456 (-1.026)',
-   '508.728.000 (-513.000)'],
+   '2.007 (+4)',
+   '1.003.640 (+2.000)',
+   '1.026.682 (+9.226)',
+   '513.341.000 (+4.613.000)'],
   ['250',
-   '4.008 (+36)',
-   '1.002.060 (+9.000)',
-   '1.017.888 (-1.024)',
-   '254.472.000 (-256.000)'],
+   '4.016 (+8)',
+   '1.004.060 (+2.000)',
+   '1.027.112 (+9.224)',
+   '256.778.000 (+2.306.000)'],
   ['100',
-   '10.031 (+90)',
-   '1.003.120 (+9.000)',
-   '1.018.980 (-1.020)',
-   '101.898.000 (-102.000)'],
+   '10.051 (+20)',
+   '1.005.120 (+2.000)',
+   '1.028.200 (+9.220)',
+   '102.820.000 (+922.000)'],
   ['50',
-   '20.078 (+180)',
-   '1.003.900 (+9.000)',
-   '1.019.780 (-1.020)',
-   '50.989.000 (-51.000)'],
+   '20.118 (+40)',
+   '1.005.900 (+2.000)',
+   '1.029.000 (+9.220)',
+   '51.450.000 (+461.000)'],
   ['25',
-   '40.219 (+360)',
-   '1.005.480 (+9.000)',
-   '1.021.400 (-1.040)',
-   '25.535.000 (-26.000)'],
+   '40.299 (+80)',
+   '1.007.480 (+2.000)',
+   '1.030.640 (+9.240)',
+   '25.766.000 (+231.000)'],
   ['10',
-   '101.050 (+900)',
-   '1.010.500 (+9.000)',
-   '1.026.600 (-1.000)',
-   '10.266.000 (-10.000)'],
+   '101.250 (+200)',
+   '1.012.500 (+2.000)',
+   '1.035.800 (+9.200)',
+   '10.358.000 (+92.000)'],
   ['5',
-   '203.200 (+1.800)',
-   '1.016.000 (+9.000)',
-   '1.032.200 (-1.000)',
-   '5.161.000 (-5.000)'],
+   '203.600 (+400)',
+   '1.018.000 (+2.000)',
+   '1.041.400 (+9.200)',
+   '5.207.000 (+46.000)'],
   ['3',
-   '340.889 (+3.000)',
-   '1.022.667 (+9.000)',
-   '1.039.333 (-1.000)',
-   '3.118.000 (-3.000)'],
+   '341.556 (+667)',
+   '1.024.667 (+2.000)',
+   '1.048.333 (+9.000)',
+   '3.145.000 (+27.000)'],
   ['2',
-   '515.500 (+4.500)',
-   '1.031.000 (+9.000)',
-   '1.048.000 (-1.000)',
-   '2.096.000 (-2.000)'],
+   '516.500 (+1.000)',
+   '1.033.000 (+2.000)',
+   '1.057.000 (+9.000)',
+   '2.114.000 (+18.000)'],
   ['1',
-   '1.061.000 (+9.000)',
-   '1.061.000 (+9.000)',
-   '1.079.000 (-1.000)',
-   '1.079.000 (-1.000)'],
+   '1.063.000 (+2.000)',
+   '1.063.000 (+2.000)',
+   '1.088.000 (+9.000)',
+   '1.088.000 (+9.000)'],
   ['0.5',
-   '2.322.000 (+18.000)',
-   '1.161.000 (+9.000)',
-   '1.182.000 (-2.000)',
-   '591.000 (-1.000)'],
-  ['Update harga LM Antam :16 Juni 2023, pukul 08:16Harga pembelian kembali '
-   ':Rp. 942.000/gram (+9.000)',
-   'Update harga LM Pegadaian :16 Juni 2023']],
- [['Spot Harga Emas Hari Ini (Market Open)'],
+   '2.326.000 (+4.000)',
+   '1.163.000 (+2.000)',
+   '1.192.000 (+10.000)',
+   '596.000 (+5.000)'],
+  ['Update harga LM Antam :17 Juni 2023, pukul 08:23Harga pembelian kembali '
+   ':Rp. 945.000/gram (+3.000)',
+   'Update harga LM Pegadaian :17 Juni 2023']],
+ [['Spot Harga Emas Hari Ini (Market Close)'],
   ['Satuan', 'USD', 'Kurs\xa0Dollar', 'IDR'],
-  ['Ounce\xa0(oz)', '1.961,18 (+1,93)', '15.140,00', '29.692.265'],
-  ['Gram\xa0(gr)', '63,05', '15.140,00', '954.628 (+939)'],
-  ['Kilogram\xa0(kg)', '63.053,40', '15.140,00', '954.628.494'],
-  ['Update harga emas :16 Juni 2023, pukul 15:34Update kurs :13 Febuari 2023, '
+  ['Ounce\xa0(oz)', '1.957,84 (+3,32)', '15.140,00', '29.641.698'],
+  ['Gram\xa0(gr)', '62,95', '15.140,00', '953.003 (+1.616)'],
+  ['Kilogram\xa0(kg)', '62.946,02', '15.140,00', '953.002.708'],
+  ['Update harga emas :17 Juni 2023, pukul 19:17Update kurs :13 Febuari 2023, '
    'pukul 09:10']],
  [['Gram', 'UBS Gold 99.99%'],
   ['Jual', 'Beli'],
   ['/ Batang', '/ Gram', '/ Batang', '/ Gram'],
-  ['100',
-   '95.685.000 (+400.000)',
-   '956.850 (+4.000)',
-   '94.300.000 (+900.000)',
-   '943.000 (+9.000)'],
-  ['50',
-   '47.895.000 (+200.000)',
-   '957.900 (+4.000)',
-   '47.150.000 (+450.000)',
-   '943.000 (+9.000)'],
-  ['25',
-   '24.050.000 (+100.000)',
-   '962.000 (+4.000)',
-   '23.575.000 (+225.000)',
-   '943.000 (+9.000)'],
-  ['10',
-   '9.670.000 (+40.000)',
-   '967.000 (+4.000)',
-   '9.430.000 (+90.000)',
-   '943.000 (+9.000)'],
-  ['5',
-   '4.887.000 (+20.000)',
-   '977.400 (+4.000)',
-   '4.715.000 (+45.000)',
-   '943.000 (+9.000)'],
-  ['1',
-   '1.010.000 (+4.000)',
-   '1.010.000 (+4.000)',
-   '943.000 (+9.000)',
-   '943.000 (+9.000)'],
+  ['100', '95.685.000', '956.850', '94.300.000', '943.000'],
+  ['50', '47.895.000', '957.900', '47.150.000', '943.000'],
+  ['25', '24.050.000', '962.000', '23.575.000', '943.000'],
+  ['10', '9.670.000', '967.000', '9.430.000', '943.000'],
+  ['5', '4.887.000', '977.400', '4.715.000', '943.000'],
+  ['1', '1.010.000', '1.010.000', '943.000', '943.000'],
   ['', 'Update :16 Juni 2023, pukul 10:55']],
  [['Konversi Satuan'],
   ['Satuan', 'Ounce (oz)', 'Gram (gr)', 'Kilogram (kg)'],
   ['Ounce\xa0(oz)', '1', '31,1034767696', '0,0311034768'],
   ['Gram\xa0(gr)', '0,0321507466', '1', '0.001'],
   ['Kilogram\xa0(kg)', '32,1507466000', '1.000', '1']],
  [['Pergerakan Harga Emas Dunia'],
   ['Waktu', 'Emas'],
   ['Unit', 'USD', 'IDR'],
   ['Angka', '+/-', 'Angka', '+/-'],
   ['Hari Ini', 'Kurs', '', '', '15.140', '%'],
-  ['oz', '1.959,25', '+1,93+0,10%', '29.663.045', '+29.220+0,10%'],
-  ['gr', '62,99', '+0,06+0,10%', '953.689', '+939+0,10%'],
+  ['oz', '1.954,52', '+3,32+0,17%', '29.591.433', '+50.265+0,17%'],
+  ['gr', '62,84', '+0,11+0,17%', '951.387', '+1.616+0,17%'],
   ['30 Hari', 'Kurs', '', '', '15.140', '%'],
-  ['oz', '1.984,24', '-23,06-1,16%', '30.041.394', '-349.128-1,16%'],
-  ['gr', '63,79', '-0,74-1,16%', '965.853', '-11.225-1,16%'],
+  ['oz', '1.955,32', '+2,52+0,13%', '29.603.545', '+38.153+0,13%'],
+  ['gr', '62,86', '+0,08+0,13%', '951.776', '+1.227+0,13%'],
   ['2 Bulan', 'Kurs', '', '', '15.140', '%'],
-  ['oz', '1.991,63', '-30,45-1,53%', '30.153.278', '-461.013-1,53%'],
-  ['gr', '64,03', '-0,98-1,53', '969.450', '-14.822-1,53%'],
-  ['6 Bulan', 'Kurs', '', '', '15.630', '-490-3,13%'],
-  ['oz', '1.793,13', '+168,05+9,37%', '28.026.622', '+1.665.643+5,94%'],
-  ['gr', '57,65', '+5,40+9,37%', '901.077', '+53.552+5,94%'],
-  ['1 Tahun', 'Kurs', '', '', '14.746', '+394+2,67%'],
-  ['oz', '1.852,26', '+108,92+5,88%', '27.313.426', '+2.378.839+8,71%'],
-  ['gr', '59,55', '+3,50+5,88%', '878.147', '+76.481+8,71%'],
-  ['2 Tahun', 'Kurs', '', '', '14.244', '+896+6,29%'],
-  ['oz', '1.859,27', '+101,91+5,48%', '26.483.442', '+3.208.823+12,12%'],
-  ['gr', '59,78', '+3,28+5,48%', '851.462', '+103.166+12,12%'],
-  ['3 Tahun', 'Kurs', '', '', '14.155', '+985+6,96%'],
-  ['oz', '1.729,14', '+232,04+13,42%', '24.475.994', '+5.216.271+21,31%'],
-  ['gr', '55,59', '+7,46+13,42%', '786.921', '+167.707+21,31%'],
+  ['oz', '2.005,47', '-47,63-2,38%', '30.362.816', '-721.118-2,38%'],
+  ['gr', '64,48', '-1,53-2,38', '976.187', '-23.184-2,38%'],
+  ['6 Bulan', 'Kurs', '', '', '15.617', '-477-3,05%'],
+  ['oz', '1.788,31', '+169,53+9,48%', '27.928.037', '+1.713.660+6,14%'],
+  ['gr', '57,50', '+5,45+9,48%', '897.907', '+55.095+6,14%'],
+  ['1 Tahun', 'Kurs', '', '', '14.741', '+399+2,71%'],
+  ['oz', '1.838,69', '+119,15+6,48%', '27.104.148', '+2.537.550+9,36%'],
+  ['gr', '59,12', '+3,83+6,48%', '871.419', '+81.584+9,36%'],
+  ['2 Tahun', 'Kurs', '', '', '14.257', '+883+6,19%'],
+  ['oz', '1.772,06', '+185,78+10,48%', '25.264.277', '+4.377.420+17,33%'],
+  ['gr', '56,97', '+5,97+10,48%', '812.265', '+140.737+17,33%'],
+  ['3 Tahun', 'Kurs', '', '', '14.234', '+906+6,37%'],
+  ['oz', '1.726,92', '+230,92+13,37%', '24.580.979', '+5.060.718+20,59%'],
+  ['gr', '55,52', '+7,42+13,37%', '790.297', '+162.706+20,59%'],
   ['5 Tahun', 'Kurs', '', '', '13.902', '+1.238+8,91%'],
-  ['oz', '1.280,09', '+681,09+53,21%', '17.795.811', '+11.896.454+66,85%'],
-  ['gr', '41,16', '+21,90+53,21%', '572.149', '+382.480+66,85%']])
-Timeout 3
+  ['oz', '1.278,27', '+679,57+53,16%', '17.770.510', '+11.871.188+66,80%'],
+  ['gr', '41,10', '+21,85+53,16%', '571.335', '+381.668+66,80%']])
 (['Home', 'Emas 1 Gram', 'History', 'Trend', 'Perak 1 Gram'],
  [[''],
   ['Emas 24 KaratHarga Emas 1 Gram', ''],
-  ['USD', '63,05↑', '+0,06+0,10%'],
-  ['KURS', '14.945,75↑', '+41,75+0,28%'],
-  ['IDR', '942.380,37↑', '+3.557,29+0,38%'],
-  ['Jumat, 16 Juni 2023 15:34']],
+  ['USD', '62,95↑', '+0,11+0,18%'],
+  ['KURS', '14.961,45↓', '-0,40-0,00%'],
+  ['IDR', '941.763,70↑', '+1.571,86+0,17%'],
+  ['Sabtu, 17 Juni 2023 19:17']],
  [[''],
   ['Emas 1 Gram (IDR)Emas 1 Gram (USD)Kurs USD-IDR',
    'Hari Ini',
    '1 Bulan',
    '1 Tahun',
    '5 Tahun',
    'Max',
    '']],
  [['Pergerakkan Harga Emas 1 Gram'],
   ['', 'Penutupan Kemarin', 'Pergerakkan Hari Ini', 'Rata-rata'],
-  ['USD', '62,99', '62,99 - 63,05', '63,02'],
-  ['KURS', '14.904,00', '14.904,00 - 14.945,75', '14.924,88'],
-  ['IDR', '938.823,08', '938.823,08 - 942.380,37', '940.601,73'],
+  ['USD', '62,84', '62,84 - 62,95', '62,90'],
+  ['KURS', '14.961,85', '14.961,45 - 14.961,85', '14.961,65'],
+  ['IDR', '940.191,84', '940.191,84 - 941.763,70', '940.977,77'],
   [''],
   ['', 'Awal Tahun', 'Pergerakkan YTD', '+/- YTD'],
-  ['USD', '58,64', '58,23 - 65,97', '+4,41 (7,52%)'],
-  ['KURS', '15.538,50', '14.669,40 - 15.629,15', '-592,75(-3,81%)'],
-  ['IDR', '911.153,72', '888.842,84 - 982.694,10', '+31.226,65 (3,43%)'],
+  ['USD', '58,64', '58,23 - 65,97', '+4,31 (7,35%)'],
+  ['KURS', '15.538,50', '14.669,40 - 15.629,15', '-577,05(-3,71%)'],
+  ['IDR', '911.153,72', '888.842,84 - 982.694,10', '+30.609,98 (3,36%)'],
   [''],
   ['', 'Tahun Lalu / 52 Minggu', 'Pergerakkan 52 Minggu', '+/- 52 Minggu'],
-  ['USD', '58,52', '52,31 - 65,97', '+4,53 (7,74%)'],
-  ['KURS', '14.767,85', '14.653,00 - 15.785,40', '+177,90 (1,20%)'],
-  ['IDR', '864.259,47', '795.009,21 - 982.694,10', '+78.120,90 (9,04%)']])
+  ['USD', '59,55', '52,31 - 65,97', '+3,40 (5,71%)'],
+  ['KURS', '14.819,05', '14.653,00 - 15.785,40', '+142,40 (0,96%)'],
+  ['IDR', '882.497,28', '795.009,21 - 982.694,10', '+59.266,42 (6,72%)']])
 ```
 
 # CLASS
 
 ## ComparePerformance
 
 `ComparePerformance`
@@ -1233,23 +1231,23 @@
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 ```
 
 Output:
 ```py
-{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x7c61d85f20>,
+{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x74c8181f20>,
  'b': (0, 1, 2, 3, 4, 5, 6, 7, 8, 9),
  'c': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
  'd': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]}
-{'a': 104, 'b': 109, 'c': 100, 'd': 152}
-{'a': 144, 'b': 139, 'c': 100, 'd': 186}
-{'a': 143, 'b': 137, 'c': 100, 'd': 166}
-{'a': 117, 'b': 135, 'c': 100, 'd': 149}
-{'a': 126, 'b': 141, 'c': 100, 'd': 158}
+{'a': 113, 'b': 165, 'c': 100, 'd': 141}
+{'a': 117, 'b': 159, 'c': 100, 'd': 133}
+{'a': 121, 'b': 156, 'c': 100, 'd': 143}
+{'a': 114, 'b': 151, 'c': 100, 'd': 137}
+{'a': 111, 'b': 145, 'c': 100, 'd': 136}
 ```
 
 ## RunParallel
 
 `RunParallel`
 
 Menjalankan program secara bersamaan.  
@@ -1360,7 +1358,8 @@
 Class ini digunakan untuk serialize dan unserialize html
 
 ## html_ul
 
 `html_ul`
 
 Class ini digunakan untuk serialize dan unserialize html
+
```

### Comparing `pypipr-1.0.2/pypipr/pypipr.py` & `pypipr-1.0.4/pypipr/pypipr.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import urllib.request
 import urllib.parse
 import uuid
 import warnings
 import webbrowser
 import zoneinfo
 import textwrap
+import array
 
 
 __platform_system = platform.system()
 
 WINDOWS = __platform_system == "Windows"
 """
 True apabila berjalan di platform Windows
@@ -413,21 +414,28 @@
     input_char("Input char : ")
     input_char("Input char : ", default='Y')
     input_char("Input Char without print : ", echo_char=False)
     ```
     """
     if prompt:
         print(prompt, end=prompt_ending, flush=True)
+    
     if default is not None:
         a = default
     else:
         a = _getch.getche() if echo_char else _getch.getch()
+    
     if newline_after_input:
         print()
-    return a.decode()
+
+    if WINDOWS:
+        return a.decode()
+    if LINUX:
+        return a
+    raise Exception('Platform tidak didukung.')
 
 
 def datetime_now(timezone=None):
     """
     Memudahkan dalam membuat Datetime untuk suatu timezone tertentu
 
     ```python
```

### Comparing `pypipr-1.0.2/PKG-INFO` & `pypipr-1.0.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: pypipr
-Version: 1.0.2
-Summary: The Python Package Index Project
-Author: ufiapjj
-Author-email: ufiapjj@gmail.com
-Requires-Python: >=3.9
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-
 
 # About
 The Python Package Index Project (pypipr)
 
 pypi : https://pypi.org/project/pypipr
 
 
@@ -85,15 +72,15 @@
 s = "Urutan {1/6/3} dan {10:9} dan {j k} dan {Z - A - 15} saja."  
 print(generator.batchmaker(s))  
 print(batchmaker(s))  
 ```
 
 Output:
 ```py
-<generator object generator.batchmaker at 0x7c61eb7d00>
+<generator object generator.batchmaker at 0x74c82c3d00>
 ('Urutan 1 dan 10 dan j dan Z saja.', 'Urutan 1 dan 10 dan j dan K saja.', 'Urutan 1 dan 10 dan k dan Z saja.', 'Urutan 1 dan 10 dan k dan K saja.', 'Urutan 1 dan 9 dan j dan Z saja.', 'Urutan 1 dan 9 dan j dan K saja.', 'Urutan 1 dan 9 dan k dan Z saja.', 'Urutan 1 dan 9 dan k dan K saja.', 'Urutan 4 dan 10 dan j dan Z saja.', 'Urutan 4 dan 10 dan j dan K saja.', 'Urutan 4 dan 10 dan k dan Z saja.', 'Urutan 4 dan 10 dan k dan K saja.', 'Urutan 4 dan 9 dan j dan Z saja.', 'Urutan 4 dan 9 dan j dan K saja.', 'Urutan 4 dan 9 dan k dan Z saja.', 'Urutan 4 dan 9 dan k dan K saja.')
 ```
 
 ## calculate
 
 `calculate`
 
@@ -138,15 +125,15 @@
 array = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(generator.chunck_array(array, 5))  
 print(chunck_array(array, 5))  
 ```
 
 Output:
 ```py
-<generator object generator.chunck_array at 0x7c61f7fe40>
+<generator object generator.chunck_array at 0x74c8167e40>
 ([2, 3, 12, 3, 3], [42, 42, 1, 43, 2], [42, 41, 4, 24, 32], [42, 3, 12, 32, 42], [42])
 ```
 
 ## console_run
 
 `console_run`
 
@@ -197,17 +184,17 @@
 print(datetime_now("Asia/Jakarta"))  
 print(datetime_now("GMT"))  
 print(datetime_now("Etc/GMT+7"))  
 ```
 
 Output:
 ```py
-2023-06-16 15:34:30.771887+07:00
-2023-06-16 08:34:30.773421+00:00
-2023-06-16 01:34:30.778299-07:00
+2023-06-17 19:17:16.635844+07:00
+2023-06-17 12:17:16.637459+00:00
+2023-06-17 05:17:16.641513-07:00
 ```
 
 ## dict_first
 
 `dict_first`
 
 Mengambil nilai (key, value) pertama dari dictionary dalam bentuk tuple.  
@@ -298,45 +285,45 @@
         return [x for x in range(10)]  
 
 print(get_class_method(ExampleGetClassMethod))  
 ```
 
 Output:
 ```py
-(<function ExampleGetClassMethod.a at 0x7c61d428e0>, <function ExampleGetClassMethod.b at 0x7c61d42840>, <function ExampleGetClassMethod.c at 0x7c61d42a20>, <function ExampleGetClassMethod.d at 0x7c61d42ac0>)
+(<function ExampleGetClassMethod.a at 0x74c813e840>, <function ExampleGetClassMethod.b at 0x74c813e7a0>, <function ExampleGetClassMethod.c at 0x74c813e980>, <function ExampleGetClassMethod.d at 0x74c813ea20>)
 ```
 
 ## get_filemtime
 
 `get_filemtime`
 
 Mengambil informasi last modification time file dalam nano seconds  
 
 ```python  
 print(get_filemtime(__file__))  
 ```
 
 Output:
 ```py
-1686901831479416922
+1686946602367473992
 ```
 
 ## get_filesize
 
 `get_filesize`
 
 Mengambil informasi file size dalam bytes  
 
 ```python  
 print(get_filesize(__file__))  
 ```
 
 Output:
 ```py
-43701
+43832
 ```
 
 ## github_pull
 
 `github_pull`
 
 Menjalankan command `git pull`  
@@ -390,15 +377,15 @@
 print(implode(arr, separator='</li>\n<li>', start='<li>', end='</li>', recursive_flat=True))  
 print(implode(arr, separator='</div>\n<div>', start='<div>', end='</div>'))  
 print(implode(10, ' '))  
 ```
 
 Output:
 ```py
-qweqw, asd, dfs, weq
+weq, asd, dfs, qweqw
 ,ini,path,seperti,url,
 ini,path,seperti,url
 <li>satu</li>
 <li>12</li>
 <li>34</li>
 <li>56</li>
 <li>tiga</li>
@@ -458,15 +445,15 @@
 print(iopen("https://www.google.com/", dict(coba="dulu"), xpath="//a"))  
 ```
 
 Output:
 ```py
 8
 ['mana', 'aja']
-[<Element a at 0x7c631948c0>, <Element a at 0x7c61e23d40>, <Element a at 0x7c61ba3430>, <Element a at 0x7c61ba34d0>, <Element a at 0x7c61ba3520>, <Element a at 0x7c61ba3570>, <Element a at 0x7c61ba35c0>, <Element a at 0x7c61ba3610>, <Element a at 0x7c61ba3660>, <Element a at 0x7c61ba36b0>, <Element a at 0x7c61ba3700>, <Element a at 0x7c61ba3750>, <Element a at 0x7c61ba37a0>, <Element a at 0x7c61ba37f0>, <Element a at 0x7c61ba3840>, <Element a at 0x7c61ba3890>, <Element a at 0x7c61ba38e0>, <Element a at 0x7c61ba3930>]
+[<Element a at 0x74c821ef30>, <Element a at 0x74c821f9d0>, <Element a at 0x74c7fbf160>, <Element a at 0x74c7fbf200>, <Element a at 0x74c7fbf250>, <Element a at 0x74c7fbf2a0>, <Element a at 0x74c7fbf2f0>, <Element a at 0x74c7fbf340>, <Element a at 0x74c7fbf390>, <Element a at 0x74c7fbf3e0>, <Element a at 0x74c7fbf430>, <Element a at 0x74c7fbf480>, <Element a at 0x74c7fbf4d0>, <Element a at 0x74c7fbf520>, <Element a at 0x74c7fbf570>, <Element a at 0x74c7fbf5c0>, <Element a at 0x74c7fbf610>, <Element a at 0x74c7fbf660>]
 False
 ```
 
 ## irange
 
 `irange`
 
@@ -480,15 +467,15 @@
 # print(irange('a', 5, 3))  
 print(irange(-10, 4, 3))  
 print(irange(1, 5))  
 ```
 
 Output:
 ```py
-<generator object generator.irange at 0x7c64594bf0>
+<generator object generator.irange at 0x74ca994bf0>
 ['H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z', '[', '\\', ']', '^', '_', '`', 'a']
 ['1', '4']
 [1, 4]
 [-10, -7, -4, -1, 2]
 [1, 2, 3, 4, 5]
 ```
 
@@ -575,16 +562,16 @@
 ```python  
 print(generator.iscandir())  
 print(iscandir("./", recursive=False, scan_file=False))  
 ```
 
 Output:
 ```py
-<generator object generator.iscandir at 0x7c61f7e040>
-(PosixPath('.vscode'), PosixPath('pypipr'), PosixPath('dist'), PosixPath('.git'))
+<generator object generator.iscandir at 0x74c8166040>
+(PosixPath('.git'), PosixPath('.vscode'), PosixPath('pypipr'), PosixPath('dist'))
 ```
 
 ## log
 
 `log`
 
 Decorator untuk mempermudah pembuatan log karena tidak perlu mengubah fungsi yg sudah ada.  
@@ -638,29 +625,29 @@
              __doc__ : Path subclass for non-Windows systems.
 
     On a POSIX system, instantiating a Path should return this object.
     
            __enter__ : https:/www.google.com
           __fspath__ : https:/www.google.com
         __getstate__ : (None, {'_drv': '', '_root': '', '_parts': ['https:', 'www.google.com'], '_str': 'https:/www.google.com'})
-            __hash__ : 4473962716942053088
+            __hash__ : -6965287676073568923
             __init__ : None
    __init_subclass__ : None
           __module__ : pathlib
           __reduce__ : (<class 'pathlib.PosixPath'>, ('https:', 'www.google.com'))
             __repr__ : PosixPath('https:/www.google.com')
           __sizeof__ : 72
            __slots__ : ()
              __str__ : https:/www.google.com
     __subclasshook__ : NotImplemented
       _cached_cparts : ['https:', 'www.google.com']
              _cparts : ['https:', 'www.google.com']
                 _drv : 
-            _flavour : <pathlib._PosixFlavour object at 0x7c6393dd10>
-               _hash : 4473962716942053088
+            _flavour : <pathlib._PosixFlavour object at 0x74c9d41dd0>
+               _hash : -6965287676073568923
               _parts : ['https:', 'www.google.com']
                _root : 
                 _str : https:/www.google.com
             absolute : /data/data/com.termux/files/home/pypipr/https:/www.google.com
               anchor : 
             as_posix : https:/www.google.com
                  cwd : /data/data/com.termux/files/home/pypipr
@@ -674,15 +661,15 @@
               is_dir : False
              is_fifo : False
              is_file : False
             is_mount : False
          is_reserved : False
            is_socket : False
           is_symlink : False
-             iterdir : <generator object Path.iterdir at 0x7c61d47060>
+             iterdir : <generator object Path.iterdir at 0x74c8143060>
             joinpath : https:/www.google.com
                 name : www.google.com
               parent : https:
              parents : <PosixPath.parents>
                parts : ('https:', 'www.google.com')
              resolve : /data/data/com.termux/files/home/pypipr/https:/www.google.com
                 root : 
@@ -713,15 +700,15 @@
 
 ```python  
 print(random_bool())  
 ```
 
 Output:
 ```py
-False
+True
 ```
 
 ## serialize
 
 `serialize`
 
 Mengubah variabel data menjadi string untuk yang dapat dibaca untuk disimpan.  
@@ -904,15 +891,15 @@
 print(x)  
 print("menghentikan timeout 7")  
 x.cancel()  
 ```
 
 Output:
 ```py
-<Timer(Thread-2, started 534192831744)>
+<Timer(Thread-2, started 501548563712)>
 menghentikan timeout 7
 ```
 
 ## sets_ordered
 
 `sets_ordered`
 
@@ -922,15 +909,15 @@
 array = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]  
 print(generator.sets_ordered(array))  
 print(sets_ordered(array))  
 ```
 
 Output:
 ```py
-<generator object generator.sets_ordered at 0x7c61d86810>
+<generator object generator.sets_ordered at 0x74c8182810>
 [2, 3, 12, 42, 1, 43, 41, 4, 24, 32]
 ```
 
 ## str_cmp
 
 `str_cmp`
 
@@ -1030,191 +1017,166 @@
 pprint.pprint(unserialize_html(iopen("https://harga-emas.org/")), depth=10)  
 pprint.pprint(unserialize_html(iopen("https://harga-emas.org/1-gram/")), depth=10)  
 ```
 
 Output:
 ```py
 (['Home', 'Emas 1 Gram', 'History', 'Trend', 'Perak 1 Gram'],
- [['Harga Emas Hari Ini - Jumat, 16 Juni 2023'],
-  ['Spot Emas USD↑1.961,18 (+1,93) / oz',
+ [['Harga Emas Hari Ini - Sabtu, 17 Juni 2023'],
+  ['Spot Emas USD↑1.957,84 (+3,32) / oz',
    'Kurs IDR15.140,00 / USD',
-   'Emas IDR↑954.628 (+939) / gr'],
-  ['LM Antam (Jual)↑1.061.000 (+9.000) / gr',
-   'LM Antam (Beli)↑942.000 (+9.000) / gr']],
+   'Emas IDR↑953.003 (+1.616) / gr'],
+  ['LM Antam (Jual)↑1.063.000 (+2.000) / gr',
+   'LM Antam (Beli)↑945.000 (+3.000) / gr']],
  [['Harga Emas Hari Ini'],
   ['Gram', 'Gedung Antam Jakarta', 'Pegadaian'],
   ['per Gram (Rp)', 'per Batangan (Rp)', 'per Gram (Rp)', 'per Batangan (Rp)'],
   ['1000',
-   '1.002 (+9)',
-   '1.001.600 (+9.000)',
-   '1.017.415 (-1.025)',
-   '1.017.415.000 (-1.025.000)'],
+   '1.004 (+2)',
+   '1.003.600 (+2.000)',
+   '1.026.640 (+9.225)',
+   '1.026.640.000 (+9.225.000)'],
   ['500',
-   '2.003 (+18)',
-   '1.001.640 (+9.000)',
-   '1.017.456 (-1.026)',
-   '508.728.000 (-513.000)'],
+   '2.007 (+4)',
+   '1.003.640 (+2.000)',
+   '1.026.682 (+9.226)',
+   '513.341.000 (+4.613.000)'],
   ['250',
-   '4.008 (+36)',
-   '1.002.060 (+9.000)',
-   '1.017.888 (-1.024)',
-   '254.472.000 (-256.000)'],
+   '4.016 (+8)',
+   '1.004.060 (+2.000)',
+   '1.027.112 (+9.224)',
+   '256.778.000 (+2.306.000)'],
   ['100',
-   '10.031 (+90)',
-   '1.003.120 (+9.000)',
-   '1.018.980 (-1.020)',
-   '101.898.000 (-102.000)'],
+   '10.051 (+20)',
+   '1.005.120 (+2.000)',
+   '1.028.200 (+9.220)',
+   '102.820.000 (+922.000)'],
   ['50',
-   '20.078 (+180)',
-   '1.003.900 (+9.000)',
-   '1.019.780 (-1.020)',
-   '50.989.000 (-51.000)'],
+   '20.118 (+40)',
+   '1.005.900 (+2.000)',
+   '1.029.000 (+9.220)',
+   '51.450.000 (+461.000)'],
   ['25',
-   '40.219 (+360)',
-   '1.005.480 (+9.000)',
-   '1.021.400 (-1.040)',
-   '25.535.000 (-26.000)'],
+   '40.299 (+80)',
+   '1.007.480 (+2.000)',
+   '1.030.640 (+9.240)',
+   '25.766.000 (+231.000)'],
   ['10',
-   '101.050 (+900)',
-   '1.010.500 (+9.000)',
-   '1.026.600 (-1.000)',
-   '10.266.000 (-10.000)'],
+   '101.250 (+200)',
+   '1.012.500 (+2.000)',
+   '1.035.800 (+9.200)',
+   '10.358.000 (+92.000)'],
   ['5',
-   '203.200 (+1.800)',
-   '1.016.000 (+9.000)',
-   '1.032.200 (-1.000)',
-   '5.161.000 (-5.000)'],
+   '203.600 (+400)',
+   '1.018.000 (+2.000)',
+   '1.041.400 (+9.200)',
+   '5.207.000 (+46.000)'],
   ['3',
-   '340.889 (+3.000)',
-   '1.022.667 (+9.000)',
-   '1.039.333 (-1.000)',
-   '3.118.000 (-3.000)'],
+   '341.556 (+667)',
+   '1.024.667 (+2.000)',
+   '1.048.333 (+9.000)',
+   '3.145.000 (+27.000)'],
   ['2',
-   '515.500 (+4.500)',
-   '1.031.000 (+9.000)',
-   '1.048.000 (-1.000)',
-   '2.096.000 (-2.000)'],
+   '516.500 (+1.000)',
+   '1.033.000 (+2.000)',
+   '1.057.000 (+9.000)',
+   '2.114.000 (+18.000)'],
   ['1',
-   '1.061.000 (+9.000)',
-   '1.061.000 (+9.000)',
-   '1.079.000 (-1.000)',
-   '1.079.000 (-1.000)'],
+   '1.063.000 (+2.000)',
+   '1.063.000 (+2.000)',
+   '1.088.000 (+9.000)',
+   '1.088.000 (+9.000)'],
   ['0.5',
-   '2.322.000 (+18.000)',
-   '1.161.000 (+9.000)',
-   '1.182.000 (-2.000)',
-   '591.000 (-1.000)'],
-  ['Update harga LM Antam :16 Juni 2023, pukul 08:16Harga pembelian kembali '
-   ':Rp. 942.000/gram (+9.000)',
-   'Update harga LM Pegadaian :16 Juni 2023']],
- [['Spot Harga Emas Hari Ini (Market Open)'],
+   '2.326.000 (+4.000)',
+   '1.163.000 (+2.000)',
+   '1.192.000 (+10.000)',
+   '596.000 (+5.000)'],
+  ['Update harga LM Antam :17 Juni 2023, pukul 08:23Harga pembelian kembali '
+   ':Rp. 945.000/gram (+3.000)',
+   'Update harga LM Pegadaian :17 Juni 2023']],
+ [['Spot Harga Emas Hari Ini (Market Close)'],
   ['Satuan', 'USD', 'Kurs\xa0Dollar', 'IDR'],
-  ['Ounce\xa0(oz)', '1.961,18 (+1,93)', '15.140,00', '29.692.265'],
-  ['Gram\xa0(gr)', '63,05', '15.140,00', '954.628 (+939)'],
-  ['Kilogram\xa0(kg)', '63.053,40', '15.140,00', '954.628.494'],
-  ['Update harga emas :16 Juni 2023, pukul 15:34Update kurs :13 Febuari 2023, '
+  ['Ounce\xa0(oz)', '1.957,84 (+3,32)', '15.140,00', '29.641.698'],
+  ['Gram\xa0(gr)', '62,95', '15.140,00', '953.003 (+1.616)'],
+  ['Kilogram\xa0(kg)', '62.946,02', '15.140,00', '953.002.708'],
+  ['Update harga emas :17 Juni 2023, pukul 19:17Update kurs :13 Febuari 2023, '
    'pukul 09:10']],
  [['Gram', 'UBS Gold 99.99%'],
   ['Jual', 'Beli'],
   ['/ Batang', '/ Gram', '/ Batang', '/ Gram'],
-  ['100',
-   '95.685.000 (+400.000)',
-   '956.850 (+4.000)',
-   '94.300.000 (+900.000)',
-   '943.000 (+9.000)'],
-  ['50',
-   '47.895.000 (+200.000)',
-   '957.900 (+4.000)',
-   '47.150.000 (+450.000)',
-   '943.000 (+9.000)'],
-  ['25',
-   '24.050.000 (+100.000)',
-   '962.000 (+4.000)',
-   '23.575.000 (+225.000)',
-   '943.000 (+9.000)'],
-  ['10',
-   '9.670.000 (+40.000)',
-   '967.000 (+4.000)',
-   '9.430.000 (+90.000)',
-   '943.000 (+9.000)'],
-  ['5',
-   '4.887.000 (+20.000)',
-   '977.400 (+4.000)',
-   '4.715.000 (+45.000)',
-   '943.000 (+9.000)'],
-  ['1',
-   '1.010.000 (+4.000)',
-   '1.010.000 (+4.000)',
-   '943.000 (+9.000)',
-   '943.000 (+9.000)'],
+  ['100', '95.685.000', '956.850', '94.300.000', '943.000'],
+  ['50', '47.895.000', '957.900', '47.150.000', '943.000'],
+  ['25', '24.050.000', '962.000', '23.575.000', '943.000'],
+  ['10', '9.670.000', '967.000', '9.430.000', '943.000'],
+  ['5', '4.887.000', '977.400', '4.715.000', '943.000'],
+  ['1', '1.010.000', '1.010.000', '943.000', '943.000'],
   ['', 'Update :16 Juni 2023, pukul 10:55']],
  [['Konversi Satuan'],
   ['Satuan', 'Ounce (oz)', 'Gram (gr)', 'Kilogram (kg)'],
   ['Ounce\xa0(oz)', '1', '31,1034767696', '0,0311034768'],
   ['Gram\xa0(gr)', '0,0321507466', '1', '0.001'],
   ['Kilogram\xa0(kg)', '32,1507466000', '1.000', '1']],
  [['Pergerakan Harga Emas Dunia'],
   ['Waktu', 'Emas'],
   ['Unit', 'USD', 'IDR'],
   ['Angka', '+/-', 'Angka', '+/-'],
   ['Hari Ini', 'Kurs', '', '', '15.140', '%'],
-  ['oz', '1.959,25', '+1,93+0,10%', '29.663.045', '+29.220+0,10%'],
-  ['gr', '62,99', '+0,06+0,10%', '953.689', '+939+0,10%'],
+  ['oz', '1.954,52', '+3,32+0,17%', '29.591.433', '+50.265+0,17%'],
+  ['gr', '62,84', '+0,11+0,17%', '951.387', '+1.616+0,17%'],
   ['30 Hari', 'Kurs', '', '', '15.140', '%'],
-  ['oz', '1.984,24', '-23,06-1,16%', '30.041.394', '-349.128-1,16%'],
-  ['gr', '63,79', '-0,74-1,16%', '965.853', '-11.225-1,16%'],
+  ['oz', '1.955,32', '+2,52+0,13%', '29.603.545', '+38.153+0,13%'],
+  ['gr', '62,86', '+0,08+0,13%', '951.776', '+1.227+0,13%'],
   ['2 Bulan', 'Kurs', '', '', '15.140', '%'],
-  ['oz', '1.991,63', '-30,45-1,53%', '30.153.278', '-461.013-1,53%'],
-  ['gr', '64,03', '-0,98-1,53', '969.450', '-14.822-1,53%'],
-  ['6 Bulan', 'Kurs', '', '', '15.630', '-490-3,13%'],
-  ['oz', '1.793,13', '+168,05+9,37%', '28.026.622', '+1.665.643+5,94%'],
-  ['gr', '57,65', '+5,40+9,37%', '901.077', '+53.552+5,94%'],
-  ['1 Tahun', 'Kurs', '', '', '14.746', '+394+2,67%'],
-  ['oz', '1.852,26', '+108,92+5,88%', '27.313.426', '+2.378.839+8,71%'],
-  ['gr', '59,55', '+3,50+5,88%', '878.147', '+76.481+8,71%'],
-  ['2 Tahun', 'Kurs', '', '', '14.244', '+896+6,29%'],
-  ['oz', '1.859,27', '+101,91+5,48%', '26.483.442', '+3.208.823+12,12%'],
-  ['gr', '59,78', '+3,28+5,48%', '851.462', '+103.166+12,12%'],
-  ['3 Tahun', 'Kurs', '', '', '14.155', '+985+6,96%'],
-  ['oz', '1.729,14', '+232,04+13,42%', '24.475.994', '+5.216.271+21,31%'],
-  ['gr', '55,59', '+7,46+13,42%', '786.921', '+167.707+21,31%'],
+  ['oz', '2.005,47', '-47,63-2,38%', '30.362.816', '-721.118-2,38%'],
+  ['gr', '64,48', '-1,53-2,38', '976.187', '-23.184-2,38%'],
+  ['6 Bulan', 'Kurs', '', '', '15.617', '-477-3,05%'],
+  ['oz', '1.788,31', '+169,53+9,48%', '27.928.037', '+1.713.660+6,14%'],
+  ['gr', '57,50', '+5,45+9,48%', '897.907', '+55.095+6,14%'],
+  ['1 Tahun', 'Kurs', '', '', '14.741', '+399+2,71%'],
+  ['oz', '1.838,69', '+119,15+6,48%', '27.104.148', '+2.537.550+9,36%'],
+  ['gr', '59,12', '+3,83+6,48%', '871.419', '+81.584+9,36%'],
+  ['2 Tahun', 'Kurs', '', '', '14.257', '+883+6,19%'],
+  ['oz', '1.772,06', '+185,78+10,48%', '25.264.277', '+4.377.420+17,33%'],
+  ['gr', '56,97', '+5,97+10,48%', '812.265', '+140.737+17,33%'],
+  ['3 Tahun', 'Kurs', '', '', '14.234', '+906+6,37%'],
+  ['oz', '1.726,92', '+230,92+13,37%', '24.580.979', '+5.060.718+20,59%'],
+  ['gr', '55,52', '+7,42+13,37%', '790.297', '+162.706+20,59%'],
   ['5 Tahun', 'Kurs', '', '', '13.902', '+1.238+8,91%'],
-  ['oz', '1.280,09', '+681,09+53,21%', '17.795.811', '+11.896.454+66,85%'],
-  ['gr', '41,16', '+21,90+53,21%', '572.149', '+382.480+66,85%']])
-Timeout 3
+  ['oz', '1.278,27', '+679,57+53,16%', '17.770.510', '+11.871.188+66,80%'],
+  ['gr', '41,10', '+21,85+53,16%', '571.335', '+381.668+66,80%']])
 (['Home', 'Emas 1 Gram', 'History', 'Trend', 'Perak 1 Gram'],
  [[''],
   ['Emas 24 KaratHarga Emas 1 Gram', ''],
-  ['USD', '63,05↑', '+0,06+0,10%'],
-  ['KURS', '14.945,75↑', '+41,75+0,28%'],
-  ['IDR', '942.380,37↑', '+3.557,29+0,38%'],
-  ['Jumat, 16 Juni 2023 15:34']],
+  ['USD', '62,95↑', '+0,11+0,18%'],
+  ['KURS', '14.961,45↓', '-0,40-0,00%'],
+  ['IDR', '941.763,70↑', '+1.571,86+0,17%'],
+  ['Sabtu, 17 Juni 2023 19:17']],
  [[''],
   ['Emas 1 Gram (IDR)Emas 1 Gram (USD)Kurs USD-IDR',
    'Hari Ini',
    '1 Bulan',
    '1 Tahun',
    '5 Tahun',
    'Max',
    '']],
  [['Pergerakkan Harga Emas 1 Gram'],
   ['', 'Penutupan Kemarin', 'Pergerakkan Hari Ini', 'Rata-rata'],
-  ['USD', '62,99', '62,99 - 63,05', '63,02'],
-  ['KURS', '14.904,00', '14.904,00 - 14.945,75', '14.924,88'],
-  ['IDR', '938.823,08', '938.823,08 - 942.380,37', '940.601,73'],
+  ['USD', '62,84', '62,84 - 62,95', '62,90'],
+  ['KURS', '14.961,85', '14.961,45 - 14.961,85', '14.961,65'],
+  ['IDR', '940.191,84', '940.191,84 - 941.763,70', '940.977,77'],
   [''],
   ['', 'Awal Tahun', 'Pergerakkan YTD', '+/- YTD'],
-  ['USD', '58,64', '58,23 - 65,97', '+4,41 (7,52%)'],
-  ['KURS', '15.538,50', '14.669,40 - 15.629,15', '-592,75(-3,81%)'],
-  ['IDR', '911.153,72', '888.842,84 - 982.694,10', '+31.226,65 (3,43%)'],
+  ['USD', '58,64', '58,23 - 65,97', '+4,31 (7,35%)'],
+  ['KURS', '15.538,50', '14.669,40 - 15.629,15', '-577,05(-3,71%)'],
+  ['IDR', '911.153,72', '888.842,84 - 982.694,10', '+30.609,98 (3,36%)'],
   [''],
   ['', 'Tahun Lalu / 52 Minggu', 'Pergerakkan 52 Minggu', '+/- 52 Minggu'],
-  ['USD', '58,52', '52,31 - 65,97', '+4,53 (7,74%)'],
-  ['KURS', '14.767,85', '14.653,00 - 15.785,40', '+177,90 (1,20%)'],
-  ['IDR', '864.259,47', '795.009,21 - 982.694,10', '+78.120,90 (9,04%)']])
+  ['USD', '59,55', '52,31 - 65,97', '+3,40 (5,71%)'],
+  ['KURS', '14.819,05', '14.653,00 - 15.785,40', '+142,40 (0,96%)'],
+  ['IDR', '882.497,28', '795.009,21 - 982.694,10', '+59.266,42 (6,72%)']])
 ```
 
 # CLASS
 
 ## ComparePerformance
 
 `ComparePerformance`
@@ -1246,23 +1208,23 @@
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 print(ExampleComparePerformance().compare_performance())  
 ```
 
 Output:
 ```py
-{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x7c61d85f20>,
+{'a': <generator object ExampleComparePerformance.a.<locals>.<genexpr> at 0x74c8181f20>,
  'b': (0, 1, 2, 3, 4, 5, 6, 7, 8, 9),
  'c': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9],
  'd': [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]}
-{'a': 104, 'b': 109, 'c': 100, 'd': 152}
-{'a': 144, 'b': 139, 'c': 100, 'd': 186}
-{'a': 143, 'b': 137, 'c': 100, 'd': 166}
-{'a': 117, 'b': 135, 'c': 100, 'd': 149}
-{'a': 126, 'b': 141, 'c': 100, 'd': 158}
+{'a': 113, 'b': 165, 'c': 100, 'd': 141}
+{'a': 117, 'b': 159, 'c': 100, 'd': 133}
+{'a': 121, 'b': 156, 'c': 100, 'd': 143}
+{'a': 114, 'b': 151, 'c': 100, 'd': 137}
+{'a': 111, 'b': 145, 'c': 100, 'd': 136}
 ```
 
 ## RunParallel
 
 `RunParallel`
 
 Menjalankan program secara bersamaan.  
@@ -1373,8 +1335,7 @@
 Class ini digunakan untuk serialize dan unserialize html
 
 ## html_ul
 
 `html_ul`
 
 Class ini digunakan untuk serialize dan unserialize html
-
```

