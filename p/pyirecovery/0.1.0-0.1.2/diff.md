# Comparing `tmp/pyirecovery-0.1.0.tar.gz` & `tmp/pyirecovery-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyirecovery-0.1.0.tar", max compression
+gzip compressed data, was "pyirecovery-0.1.2.tar", max compression
```

## Comparing `pyirecovery-0.1.0.tar` & `pyirecovery-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,6 @@
--rw-r--r--   0        0        0      403 2023-01-27 10:02:13.363762 pyirecovery-0.1.0/README.md
--rw-r--r--   0        0        0      269 2023-01-27 07:02:46.257760 pyirecovery-0.1.0/pyirecovery/.irecovery
--rw-r--r--   0        0        0        0 2023-01-27 01:48:54.692260 pyirecovery-0.1.0/pyirecovery/.pyirecovery_history
--rw-r--r--   0        0        0      233 2023-01-27 09:35:14.508076 pyirecovery-0.1.0/pyirecovery/__init__.py
--rw-r--r--   0        0        0     7539 2023-01-27 10:08:25.781465 pyirecovery-0.1.0/pyirecovery/__main__.py
--rw-r--r--   0        0        0      471 2023-01-27 09:47:31.594518 pyirecovery-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 pyirecovery-0.1.0/setup.py
--rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 pyirecovery-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      451 2023-01-28 07:00:22.567534 pyirecovery-0.1.2/README.md
+-rw-r--r--   0        0        0      233 2023-01-28 07:00:22.569414 pyirecovery-0.1.2/pyirecovery/__init__.py
+-rw-r--r--   0        0        0     7610 2023-01-28 08:33:20.006307 pyirecovery-0.1.2/pyirecovery/__main__.py
+-rw-r--r--   0        0        0      471 2023-01-28 08:33:54.944158 pyirecovery-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1275 1970-01-01 00:00:00.000000 pyirecovery-0.1.2/setup.py
+-rw-r--r--   0        0        0     1173 1970-01-01 00:00:00.000000 pyirecovery-0.1.2/PKG-INFO
```

### Comparing `pyirecovery-0.1.0/pyirecovery/__main__.py` & `pyirecovery-0.1.2/pyirecovery/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pyirecovery - A CLI wrapper of pymobiledevice3 that interacts with Recovery/DFU Apple devices
 # Copyright (C) 2023 MiniExploit
 
 import click
 from pymobiledevice3 import irecv, irecv_devices
-from pymobiledevice3.exceptions import PyMobileDevice3Exception
+from pymobiledevice3.exceptions import PyMobileDevice3Exception, IRecvNoDeviceConnectedError
 import usb.core, usb.util
 import binascii
 import readline
 import os, sys
 from enum import Enum
 
 BUFFER_SIZE = 0x1000
@@ -115,15 +115,15 @@
                 print(e)
 
 def print_device_info(client):
     click.echo(f'CPID: {hex(client.chip_id)}')
     cprv = client._device_info['CPRV']
     click.echo(f'CPRV: 0x{cprv}')
     click.echo(f'BDID: {hex(client.board_id)}')
-    click.echo(f'CPID: {hex(client.ecid)}')
+    click.echo(f'ECID: {hex(client.ecid)}')
     cpfm = client._device_info['CPFM']
     click.echo(f'CPFM: 0x{cpfm}')
     scep = client._device_info['SCEP']
     click.echo(f'SCEP: 0x{scep}')
     ibfl = client._device_info['IBFL']
     click.echo(f'IBFL: 0x{ibfl}')
     try:
@@ -221,27 +221,28 @@
 
 def main(infile, reboot, command, shell, mode, query, reset):
     if len(sys.argv) == 1:
         main(['--help'])
 
     client = None
     try:
-        client = irecv.IRecv()
-    except:
-        click.secho('[ERROR] Could not init IRecv client', fg='red')
+        client = irecv.IRecv(timeout=5)
+    except IRecvNoDeviceConnectedError:
+        click.secho('[ERROR] Unable to connect to device', fg='red')
+        return -1
+    except Exception as e:
+        click.secho(f'[ERROR] Could not init IRecv client {str(e)}', fg='red')
         return -1
 
     if infile:
         data = infile.read()
         try:
             client.send_buffer(data)
         except PyMobileDevice3Exception as e:
-            if e == 'Unexpected state 5, issuing ABORT':
-                click.echo('ABORT issued')
-                client.send_buffer(data)
+            return -1
         return 0
     elif reboot:
         client.set_autoboot(1)
         client.reboot()
         return 0
     elif command:
         try:
```

### Comparing `pyirecovery-0.1.0/setup.py` & `pyirecovery-0.1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['pymobiledevice3>=1.36.2,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['pyirecovery = pyirecovery.__main__:main']}
 
 setup_kwargs = {
     'name': 'pyirecovery',
-    'version': '0.1.0',
+    'version': '0.1.2',
     'description': 'A CLI wrapper of pymobiledevice3 that interacts with Recovery/DFU Apple devices',
-    'long_description': '## pyirecovery\nA CLI wrapper of pymobiledevice3 that interacts with Recovery/DFU Apple devices\n# Installation\n* Install with PIP:\n```\npython3 -m pip install pyirecovery\n```\n* Install locally:\n```\ngit clone https://github.com/Mini-Exploit/pyirecovery\ncd pyirecovery\nbash ./install.sh\n```\n# Credits\n* [doronz88](https://github.com/doronz88) - [pymobiledevice3](https://github.com/doronz88/pymobiledevice3)',
+    'long_description': '## pyirecovery\nA CLI wrapper of pymobiledevice3 that interacts with Recovery/DFU Apple devices\n# Installation\n* Install with PIP:\n```\npython3 -m pip install pyirecovery\n```\n* Install locally:\n```\ngit clone https://github.com/Mini-Exploit/pyirecovery\ncd pyirecovery\nbash ./install.sh\n```\n# Usage\n* Run `pyirecovery` and see the usage\n\n# Credits\n* [doronz88](https://github.com/doronz88) - [pymobiledevice3](https://github.com/doronz88/pymobiledevice3)\n',
     'author': 'Mini-Exploit',
     'author_email': 'miniexploitttt@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pyirecovery-0.1.0/PKG-INFO` & `pyirecovery-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyirecovery
-Version: 0.1.0
+Version: 0.1.2
 Summary: A CLI wrapper of pymobiledevice3 that interacts with Recovery/DFU Apple devices
 License: GPL-3.0-only
 Author: Mini-Exploit
 Author-email: miniexploitttt@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -25,9 +25,13 @@
 ```
 * Install locally:
 ```
 git clone https://github.com/Mini-Exploit/pyirecovery
 cd pyirecovery
 bash ./install.sh
 ```
+# Usage
+* Run `pyirecovery` and see the usage
+
 # Credits
 * [doronz88](https://github.com/doronz88) - [pymobiledevice3](https://github.com/doronz88/pymobiledevice3)
+
```

