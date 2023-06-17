# Comparing `tmp/bin2coe-1.1.0.tar.gz` & `tmp/bin2coe-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bin2coe-1.1.0.tar", last modified: Tue Aug 27 02:55:56 2019, max compression
+gzip compressed data, was "bin2coe-1.1.1.tar", last modified: Sat Jun 17 11:06:08 2023, max compression
```

## Comparing `bin2coe-1.1.0.tar` & `bin2coe-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2019-08-27 02:55:56.000000 bin2coe-1.1.0/
--rw-r--r--   0 anish      (501) staff       (20)     2205 2019-08-27 02:55:56.000000 bin2coe-1.1.0/PKG-INFO
--rw-r--r--   0 anish      (501) staff       (20)     1206 2019-08-23 04:22:11.000000 bin2coe-1.1.0/README.md
--rw-r--r--   0 anish      (501) staff       (20)       38 2019-08-27 02:55:56.000000 bin2coe-1.1.0/setup.cfg
--rw-r--r--   0 anish      (501) staff       (20)     1550 2019-08-20 19:15:00.000000 bin2coe-1.1.0/setup.py
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2019-08-27 02:55:56.000000 bin2coe-1.1.0/src/
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2019-08-27 02:55:56.000000 bin2coe-1.1.0/src/bin2coe/
--rw-r--r--   0 anish      (501) staff       (20)       22 2019-08-27 00:50:29.000000 bin2coe-1.1.0/src/bin2coe/__init__.py
--rw-r--r--   0 anish      (501) staff       (20)     3055 2019-08-27 01:07:31.000000 bin2coe-1.1.0/src/bin2coe/cli.py
--rw-r--r--   0 anish      (501) staff       (20)     1639 2019-08-27 01:03:47.000000 bin2coe-1.1.0/src/bin2coe/convert.py
-drwxr-xr-x   0 anish      (501) staff       (20)        0 2019-08-27 02:55:56.000000 bin2coe-1.1.0/src/bin2coe.egg-info/
--rw-r--r--   0 anish      (501) staff       (20)     2205 2019-08-27 02:55:56.000000 bin2coe-1.1.0/src/bin2coe.egg-info/PKG-INFO
--rw-r--r--   0 anish      (501) staff       (20)      262 2019-08-27 02:55:56.000000 bin2coe-1.1.0/src/bin2coe.egg-info/SOURCES.txt
--rw-r--r--   0 anish      (501) staff       (20)        1 2019-08-27 02:55:56.000000 bin2coe-1.1.0/src/bin2coe.egg-info/dependency_links.txt
--rw-r--r--   0 anish      (501) staff       (20)       46 2019-08-27 02:55:56.000000 bin2coe-1.1.0/src/bin2coe.egg-info/entry_points.txt
--rw-r--r--   0 anish      (501) staff       (20)        8 2019-08-27 02:55:56.000000 bin2coe-1.1.0/src/bin2coe.egg-info/top_level.txt
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-06-17 11:06:08.982108 bin2coe-1.1.1/
+-rw-r--r--   0 anish      (501) staff       (20)     1123 2023-03-05 13:21:19.000000 bin2coe-1.1.1/LICENSE.md
+-rw-r--r--   0 anish      (501) staff       (20)     1572 2023-06-17 11:06:08.981793 bin2coe-1.1.1/PKG-INFO
+-rw-r--r--   0 anish      (501) staff       (20)     1003 2023-03-07 13:21:54.000000 bin2coe-1.1.1/README.md
+-rw-r--r--   0 anish      (501) staff       (20)      110 2022-01-30 19:08:05.000000 bin2coe-1.1.1/pyproject.toml
+-rw-r--r--   0 anish      (501) staff       (20)       38 2023-06-17 11:06:08.982199 bin2coe-1.1.1/setup.cfg
+-rw-r--r--   0 anish      (501) staff       (20)     1484 2022-01-30 18:08:35.000000 bin2coe-1.1.1/setup.py
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-06-17 11:06:08.974959 bin2coe-1.1.1/src/
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-06-17 11:06:08.978466 bin2coe-1.1.1/src/bin2coe/
+-rw-r--r--   0 anish      (501) staff       (20)       22 2023-06-13 13:20:52.000000 bin2coe-1.1.1/src/bin2coe/__init__.py
+-rw-r--r--   0 anish      (501) staff       (20)     3444 2023-06-13 13:19:09.000000 bin2coe-1.1.1/src/bin2coe/cli.py
+-rw-r--r--   0 anish      (501) staff       (20)     1972 2022-04-10 11:10:46.000000 bin2coe-1.1.1/src/bin2coe/convert.py
+drwxr-xr-x   0 anish      (501) staff       (20)        0 2023-06-17 11:06:08.981292 bin2coe-1.1.1/src/bin2coe.egg-info/
+-rw-r--r--   0 anish      (501) staff       (20)     1572 2023-06-17 11:06:08.000000 bin2coe-1.1.1/src/bin2coe.egg-info/PKG-INFO
+-rw-r--r--   0 anish      (501) staff       (20)      288 2023-06-17 11:06:08.000000 bin2coe-1.1.1/src/bin2coe.egg-info/SOURCES.txt
+-rw-r--r--   0 anish      (501) staff       (20)        1 2023-06-17 11:06:08.000000 bin2coe-1.1.1/src/bin2coe.egg-info/dependency_links.txt
+-rw-r--r--   0 anish      (501) staff       (20)       45 2023-06-17 11:06:08.000000 bin2coe-1.1.1/src/bin2coe.egg-info/entry_points.txt
+-rw-r--r--   0 anish      (501) staff       (20)        8 2023-06-17 11:06:08.000000 bin2coe-1.1.1/src/bin2coe.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bin2coe-1.1.0/PKG-INFO` & `bin2coe-1.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,71 +1,57 @@
 Metadata-Version: 2.1
 Name: bin2coe
-Version: 1.1.0
+Version: 1.1.1
 Summary: A tool to convert binary files to COE files
 Home-page: https://github.com/anishathalye/bin2coe
 Author: Anish Athalye
 Author-email: me@anishathalye.com
 License: MIT
-Description: bin2coe
-        =======
-        
-        bin2coe is, as its name suggests, a tool to convert binary files to [COE] files
-        for initializing Xilinx FPGA block RAM.
-        
-        ---
-        
-        [![Build Status](https://travis-ci.com/anishathalye/bin2coe.svg?branch=master)](https://travis-ci.com/anishathalye/bin2coe)
-        
-        Usage
-        -----
-        
-        Basic usage looks like this:
-        
-        ```bash
-        bin2coe -i INPUT -w WIDTH -o OUTPUT
-        ```
-        
-        Additionally, you can specify depth manually (rather than having it be
-        inferred), specify a value to fill in empty words, and specify the radix. See
-        `bin2coe --help` for more information.
-        
-        Installation
-        ------------
-        
-        bin2coe can be installed from [PyPI]:
-        
-        ```bash
-        pip install bin2coe
-        ```
-        
-        After running this command, the `bin2coe` binary should be available on your
-        `$PATH`.
-        
-        Packaging
-        ---------
-        
-        1. Update version information.
-        
-        2. Build the package using ``python setup.py sdist bdist_wheel``.
-        
-        3. Sign and upload the package using ``twine upload -s dist/*``.
-        
-        License
-        -------
-        
-        Copyright (c) 2019 Anish Athalye. Released under the MIT License. See
-        [LICENSE.md][license] for details.
-        
-        [COE]: https://www.xilinx.com/support/documentation/sw_manuals/xilinx11/cgn_r_coe_file_syntax.htm
-        [PyPI]: https://pypi.org/project/bin2coe/
-        [license]: LICENSE.md
-        
 Keywords: xilinx coe bram
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# bin2coe [![Build Status](https://github.com/anishathalye/bin2coe/workflows/CI/badge.svg)](https://github.com/anishathalye/bin2coe/actions?query=workflow%3ACI)
+
+bin2coe is, as its name suggests, a tool to convert binary files to [COE] files
+for initializing Xilinx FPGA block RAM.
+
+Usage
+-----
+
+Basic usage looks like this:
+
+```bash
+bin2coe -i INPUT -w WIDTH -o OUTPUT
+```
+
+Additionally, you can specify depth manually (rather than having it be
+inferred), specify a value to fill in empty words, and specify the radix. See
+`bin2coe --help` for more information.
+
+Installation
+------------
+
+bin2coe can be installed from [PyPI]:
+
+```bash
+pip install bin2coe
+```
+
+After running this command, the `bin2coe` binary should be available on your
+`$PATH`.
+
+License
+-------
+
+Copyright (c) Anish Athalye. Released under the MIT License. See
+[LICENSE.md][license] for details.
+
+[COE]: https://docs.xilinx.com/r/en-US/ug896-vivado-ip/COE-File-Syntax
+[PyPI]: https://pypi.org/project/bin2coe/
+[license]: LICENSE.md
```

### Comparing `bin2coe-1.1.0/src/bin2coe/cli.py` & `bin2coe-1.1.1/src/bin2coe/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,81 +1,93 @@
 from .convert import convert
 from argparse import ArgumentParser
 import sys
 
 
-def main():
+from typing import NoReturn, BinaryIO
+
+
+def main() -> None:
     parser = ArgumentParser()
-    parser.add_argument('-i', '--input', type=str, required=True, help='input filename')
-    parser.add_argument('-o', '--output', type=str, required=True, help='output filename')
-    parser.add_argument('-w', '--width', type=int, required=True, help='block memory width in bits')
-    parser.add_argument('-d', '--depth', type=int, help='block memory depth in blocks')
-    parser.add_argument('-f', '--fill', type=str, help='value to fill in empty words')
-    parser.add_argument('-r', '--radix', type=int, default=16, help='fill radix and output radix')
-    parser.add_argument('--big-endian', action='store_true', default=False, help='big endian mode')
-    parser.add_argument('--mem', action='store_true', default=False, help='output mem file')
+    parser.add_argument("-i", "--input", type=str, required=True, help="input filename")
+    parser.add_argument("-o", "--output", type=str, required=True, help="output filename")
+    parser.add_argument("-w", "--width", type=int, required=True, help="block memory width in bits")
+    parser.add_argument("-d", "--depth", type=int, help="block memory depth in blocks")
+    parser.add_argument("-f", "--fill", type=str, help="value to fill in empty words")
+    parser.add_argument("-r", "--radix", type=int, default=16, help="fill radix and output radix")
+    parser.add_argument("--big-endian", action="store_true", default=False, help="big endian mode")
+    parser.add_argument("--mem", action="store_true", default=False, help="output mem file")
     options = parser.parse_args()
 
     # check radix
     if not (2 <= options.radix <= 36):
-        error('unsupported radix, must be between 2 and 36')
+        error("unsupported radix, must be between 2 and 36")
     if options.mem and not options.radix in [2, 16]:
-        error('mem requires radix 2 or 16')
+        error("mem requires radix 2 or 16")
 
     # check width
     if not 8 <= options.width:
-        error('width must be >= 8')
+        error("width must be >= 8")
     if not options.width & (options.width - 1) == 0:
-        error('width must be a power of 2')
+        error("width must be a power of 2")
 
     # if fill is specified, then depth must be specified too; otherwise, depth
     # can be inferred.
     if options.fill is not None and options.depth is None:
-        error('depth must be specified if fill is specified')
+        error("depth must be specified if fill is specified")
 
     # calculate fill
     fill = None
     if options.fill is not None:
         try:
             fill = int(options.fill, options.radix)
         except ValueError:
-            error('invalid fill ({}) for radix ({})'.format(options.fill, options.radix))
+            error("invalid fill ({}) for radix ({})".format(options.fill, options.radix))
 
-    with open(options.input, 'rb') as f:
+    with open(options.input, "rb") as f:
         data = f.read()
     bits = 8 * len(data)
 
     # infer / validate depth
     depth = options.depth
     if depth is None:
-        # infer depth if necessary
+        # infer depth if necessary, adding zero words if necessary
         if bits % options.width != 0:
-            error('cannot infer depth, {} total bits, width {}'.format(bits, options.width))
+            extra = options.width - bits % options.width
+            if extra % 8 != 0:
+                error("cannot infer depth, {} total bits, width {}".format(bits, options.width))
+            extra_words = extra // 8
+            data = data + bytes(extra_words)
+            bits = 8 * len(data)
         depth = bits // options.width
     else:
         # validate depth
         if fill is None:
             if bits != options.width * depth:
-                error('memory size / file size mismatch: {} x {} bit != {}'.format(depth, options.width, bits))
+                error(
+                    "memory size / file size mismatch: {} x {} bit != {}".format(
+                        depth, options.width, bits
+                    )
+                )
         else:
             # make sure it fills an integer number of words
             if bits % options.width != 0:
-                error('data must fill an integer number of words')
+                error("data must fill an integer number of words")
             if bits > options.width * depth:
-                error('memory size too small: {} x {} bit < {}'.format(depth, options.width, bits))
+                error("memory size too small: {} x {} bit < {}".format(depth, options.width, bits))
 
-    with open(options.output, 'wb') as f:
+    with open(options.output, "wb") as f:
         convert(
             f,
             data,
             options.width,
             depth,
             fill,
             options.radix,
             little_endian=(not options.big_endian),
-            mem=(options.mem)
+            mem=(options.mem),
         )
 
 
-def error(msg):
-    print('error: {}'.format(msg), file=sys.stderr)
+def error(msg: str) -> NoReturn:
+    print("error: {}".format(msg), file=sys.stderr)
     exit(1)
```

### Comparing `bin2coe-1.1.0/src/bin2coe.egg-info/PKG-INFO` & `bin2coe-1.1.1/src/bin2coe.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,71 +1,57 @@
 Metadata-Version: 2.1
 Name: bin2coe
-Version: 1.1.0
+Version: 1.1.1
 Summary: A tool to convert binary files to COE files
 Home-page: https://github.com/anishathalye/bin2coe
 Author: Anish Athalye
 Author-email: me@anishathalye.com
 License: MIT
-Description: bin2coe
-        =======
-        
-        bin2coe is, as its name suggests, a tool to convert binary files to [COE] files
-        for initializing Xilinx FPGA block RAM.
-        
-        ---
-        
-        [![Build Status](https://travis-ci.com/anishathalye/bin2coe.svg?branch=master)](https://travis-ci.com/anishathalye/bin2coe)
-        
-        Usage
-        -----
-        
-        Basic usage looks like this:
-        
-        ```bash
-        bin2coe -i INPUT -w WIDTH -o OUTPUT
-        ```
-        
-        Additionally, you can specify depth manually (rather than having it be
-        inferred), specify a value to fill in empty words, and specify the radix. See
-        `bin2coe --help` for more information.
-        
-        Installation
-        ------------
-        
-        bin2coe can be installed from [PyPI]:
-        
-        ```bash
-        pip install bin2coe
-        ```
-        
-        After running this command, the `bin2coe` binary should be available on your
-        `$PATH`.
-        
-        Packaging
-        ---------
-        
-        1. Update version information.
-        
-        2. Build the package using ``python setup.py sdist bdist_wheel``.
-        
-        3. Sign and upload the package using ``twine upload -s dist/*``.
-        
-        License
-        -------
-        
-        Copyright (c) 2019 Anish Athalye. Released under the MIT License. See
-        [LICENSE.md][license] for details.
-        
-        [COE]: https://www.xilinx.com/support/documentation/sw_manuals/xilinx11/cgn_r_coe_file_syntax.htm
-        [PyPI]: https://pypi.org/project/bin2coe/
-        [license]: LICENSE.md
-        
 Keywords: xilinx coe bram
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# bin2coe [![Build Status](https://github.com/anishathalye/bin2coe/workflows/CI/badge.svg)](https://github.com/anishathalye/bin2coe/actions?query=workflow%3ACI)
+
+bin2coe is, as its name suggests, a tool to convert binary files to [COE] files
+for initializing Xilinx FPGA block RAM.
+
+Usage
+-----
+
+Basic usage looks like this:
+
+```bash
+bin2coe -i INPUT -w WIDTH -o OUTPUT
+```
+
+Additionally, you can specify depth manually (rather than having it be
+inferred), specify a value to fill in empty words, and specify the radix. See
+`bin2coe --help` for more information.
+
+Installation
+------------
+
+bin2coe can be installed from [PyPI]:
+
+```bash
+pip install bin2coe
+```
+
+After running this command, the `bin2coe` binary should be available on your
+`$PATH`.
+
+License
+-------
+
+Copyright (c) Anish Athalye. Released under the MIT License. See
+[LICENSE.md][license] for details.
+
+[COE]: https://docs.xilinx.com/r/en-US/ug896-vivado-ip/COE-File-Syntax
+[PyPI]: https://pypi.org/project/bin2coe/
+[license]: LICENSE.md
```

