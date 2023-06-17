# Comparing `tmp/vagd-0.3.9.tar.gz` & `tmp/vagd-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vagd-0.3.9.tar", last modified: Tue May 23 10:34:26 2023, max compression
+gzip compressed data, was "vagd-0.4.0.tar", last modified: Sat Jun 17 14:27:13 2023, max compression
```

## Comparing `vagd-0.3.9.tar` & `vagd-0.4.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-23 10:34:26.716432 vagd-0.3.9/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    35149 2023-03-05 14:43:59.000000 vagd-0.3.9/LICENSE
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2866 2023-05-23 10:34:26.716432 vagd-0.3.9/PKG-INFO
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2282 2023-03-21 08:25:45.000000 vagd-0.3.9/README.md
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      880 2023-05-23 10:33:24.000000 vagd-0.3.9/pyproject.toml
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       38 2023-05-23 10:34:26.716432 vagd-0.3.9/setup.cfg
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-23 10:34:26.709766 vagd-0.3.9/src/
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-23 10:34:26.713099 vagd-0.3.9/src/vagd/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       53 2023-03-20 14:52:11.000000 vagd-0.3.9/src/vagd/__init__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      220 2023-03-14 11:41:30.000000 vagd-0.3.9/src/vagd/__main__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      900 2023-04-15 11:40:48.000000 vagd-0.3.9/src/vagd/box.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-23 10:34:26.716432 vagd-0.3.9/src/vagd/gdb/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    20349 2023-03-04 14:19:11.000000 vagd-0.3.9/src/vagd/gdb/__init__.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4178 2023-03-04 12:55:58.000000 vagd-0.3.9/src/vagd/gdb/events.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      983 2023-03-04 12:55:58.000000 vagd-0.3.9/src/vagd/gdb/printing.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       47 2023-03-04 12:55:58.000000 vagd-0.3.9/src/vagd/gdb/prompt.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      865 2023-03-04 12:55:58.000000 vagd-0.3.9/src/vagd/gdb/types.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      135 2023-03-04 12:55:58.000000 vagd-0.3.9/src/vagd/gdb/unwinder.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      844 2023-03-04 12:55:58.000000 vagd-0.3.9/src/vagd/gdb/xmethod.pyi
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       44 2023-03-14 14:03:57.000000 vagd-0.3.9/src/vagd/gdb.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1195 2023-04-08 07:51:28.000000 vagd-0.3.9/src/vagd/helper.py
--rwxr-xr-x   0 gfelber   (1000) gfelber   (1000)      755 2023-05-23 10:32:45.000000 vagd-0.3.9/src/vagd/template.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      734 2023-03-20 14:52:11.000000 vagd-0.3.9/src/vagd/templates.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-23 10:34:26.716432 vagd-0.3.9/src/vagd/virts/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      132 2023-03-20 14:52:11.000000 vagd-0.3.9/src/vagd/virts/__init__.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4202 2023-03-21 09:12:24.000000 vagd-0.3.9/src/vagd/virts/dogd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10244 2023-05-17 09:35:51.000000 vagd-0.3.9/src/vagd/virts/pwngd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10853 2023-04-15 14:11:22.000000 vagd-0.3.9/src/vagd/virts/qegd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1345 2023-03-20 14:52:11.000000 vagd-0.3.9/src/vagd/virts/shgd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     3592 2023-03-20 14:52:11.000000 vagd-0.3.9/src/vagd/virts/vagd.py
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      843 2023-03-14 14:21:12.000000 vagd-0.3.9/src/vagd/wrapper.py
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-23 10:34:26.713099 vagd-0.3.9/src/vagd.egg-info/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2866 2023-05-23 10:34:26.000000 vagd-0.3.9/src/vagd.egg-info/PKG-INFO
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)      678 2023-05-23 10:34:26.000000 vagd-0.3.9/src/vagd.egg-info/SOURCES.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)        1 2023-05-23 10:34:26.000000 vagd-0.3.9/src/vagd.egg-info/dependency_links.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)       31 2023-05-23 10:34:26.000000 vagd-0.3.9/src/vagd.egg-info/requires.txt
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)        5 2023-05-23 10:34:26.000000 vagd-0.3.9/src/vagd.egg-info/top_level.txt
-drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-05-23 10:34:26.716432 vagd-0.3.9/test/
--rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1074 2023-03-20 14:52:11.000000 vagd-0.3.9/test/test.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 14:27:13.989793 vagd-0.4.0/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    35149 2023-03-05 14:43:59.000000 vagd-0.4.0/LICENSE
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2906 2023-06-17 14:27:13.989793 vagd-0.4.0/PKG-INFO
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2322 2023-06-17 13:45:28.000000 vagd-0.4.0/README.md
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      880 2023-06-17 14:23:26.000000 vagd-0.4.0/pyproject.toml
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       38 2023-06-17 14:27:13.989793 vagd-0.4.0/setup.cfg
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 14:27:13.983126 vagd-0.4.0/src/
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 14:27:13.986459 vagd-0.4.0/src/vagd/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       53 2023-03-20 14:52:11.000000 vagd-0.4.0/src/vagd/__init__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      220 2023-03-14 11:41:30.000000 vagd-0.4.0/src/vagd/__main__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      939 2023-06-17 11:38:21.000000 vagd-0.4.0/src/vagd/box.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 14:27:13.986459 vagd-0.4.0/src/vagd/gdb/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    20349 2023-03-04 14:19:11.000000 vagd-0.4.0/src/vagd/gdb/__init__.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     4178 2023-03-04 12:55:58.000000 vagd-0.4.0/src/vagd/gdb/events.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      983 2023-03-04 12:55:58.000000 vagd-0.4.0/src/vagd/gdb/printing.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       47 2023-03-04 12:55:58.000000 vagd-0.4.0/src/vagd/gdb/prompt.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      865 2023-03-04 12:55:58.000000 vagd-0.4.0/src/vagd/gdb/types.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      135 2023-03-04 12:55:58.000000 vagd-0.4.0/src/vagd/gdb/unwinder.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      844 2023-03-04 12:55:58.000000 vagd-0.4.0/src/vagd/gdb/xmethod.pyi
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       44 2023-03-14 14:03:57.000000 vagd-0.4.0/src/vagd/gdb.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1195 2023-04-08 07:51:28.000000 vagd-0.4.0/src/vagd/helper.py
+-rwxr-xr-x   0 gfelber   (1000) gfelber   (1000)      839 2023-06-17 11:43:56.000000 vagd-0.4.0/src/vagd/template.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1736 2023-06-17 14:24:55.000000 vagd-0.4.0/src/vagd/templates.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 14:27:13.989793 vagd-0.4.0/src/vagd/virts/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      132 2023-03-20 14:52:11.000000 vagd-0.4.0/src/vagd/virts/__init__.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     5160 2023-06-17 14:24:32.000000 vagd-0.4.0/src/vagd/virts/dogd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10643 2023-06-17 14:20:58.000000 vagd-0.4.0/src/vagd/virts/pwngd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)    10853 2023-04-15 14:11:22.000000 vagd-0.4.0/src/vagd/virts/qegd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1345 2023-03-20 14:52:11.000000 vagd-0.4.0/src/vagd/virts/shgd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     3592 2023-03-20 14:52:11.000000 vagd-0.4.0/src/vagd/virts/vagd.py
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      843 2023-03-14 14:21:12.000000 vagd-0.4.0/src/vagd/wrapper.py
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 14:27:13.986459 vagd-0.4.0/src/vagd.egg-info/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     2906 2023-06-17 14:27:13.000000 vagd-0.4.0/src/vagd.egg-info/PKG-INFO
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)      678 2023-06-17 14:27:13.000000 vagd-0.4.0/src/vagd.egg-info/SOURCES.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)        1 2023-06-17 14:27:13.000000 vagd-0.4.0/src/vagd.egg-info/dependency_links.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)       31 2023-06-17 14:27:13.000000 vagd-0.4.0/src/vagd.egg-info/requires.txt
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)        5 2023-06-17 14:27:13.000000 vagd-0.4.0/src/vagd.egg-info/top_level.txt
+drwxr-xr-x   0 gfelber   (1000) gfelber   (1000)        0 2023-06-17 14:27:13.989793 vagd-0.4.0/test/
+-rw-r--r--   0 gfelber   (1000) gfelber   (1000)     1074 2023-03-20 14:52:11.000000 vagd-0.4.0/test/test.py
```

### Comparing `vagd-0.3.9/LICENSE` & `vagd-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vagd-0.3.9/PKG-INFO` & `vagd-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vagd
-Version: 0.3.9
+Version: 0.4.0
 Summary: VirtuAlization GDb integrations in pwntools
 Author-email: 0x6fe1be2 <author@example.com>
 Project-URL: Homepage, https://github.com/gfelber/vagd
 Project-URL: Documentation, https://gfelber.github.io/vagd/
 Project-URL: Bug Tracker, https://github.com/gfelber/vagd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -70,14 +70,15 @@
   * [CLOUDIMAGE_BIONIC](https://cloud-images.ubuntu.com/bionic/current/bionic-server-cloudimg-amd64.img)
   * [CLOUDIMAGE_XENIAL](https://cloud-images.ubuntu.com/xenial/current/xenial-server-cloudimg-amd64-disk1.img)
 * Docker
   * DOCKER_JAMMY = 'ubuntu:jammy'
   * DOCKER_FOCAL = 'ubuntu:focal'
   * DOCKER_BIONIC = 'ubuntu:bionic'
   * DOCKER_XENIAL = 'ubuntu:xenial'
+  * DOCKER_ALPINE_316 = 'alpine:3.16.6'
 
 
 currently only distributions that use `apt` are supported
 
 
 
 ## Future plans
```

### Comparing `vagd-0.3.9/README.md` & `vagd-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,15 @@
   * [CLOUDIMAGE_BIONIC](https://cloud-images.ubuntu.com/bionic/current/bionic-server-cloudimg-amd64.img)
   * [CLOUDIMAGE_XENIAL](https://cloud-images.ubuntu.com/xenial/current/xenial-server-cloudimg-amd64-disk1.img)
 * Docker
   * DOCKER_JAMMY = 'ubuntu:jammy'
   * DOCKER_FOCAL = 'ubuntu:focal'
   * DOCKER_BIONIC = 'ubuntu:bionic'
   * DOCKER_XENIAL = 'ubuntu:xenial'
+  * DOCKER_ALPINE_316 = 'alpine:3.16.6'
 
 
 currently only distributions that use `apt` are supported
 
 
 
 ## Future plans
```

### Comparing `vagd-0.3.9/pyproject.toml` & `vagd-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "vagd"
-version = "0.3.9"
+version = "0.4.0"
 authors = [
   { name="0x6fe1be2", email="author@example.com" },
 ]
 description = "VirtuAlization GDb integrations in pwntools"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ['pwntools', 'python-vagrant', 'docker']
```

### Comparing `vagd-0.3.9/src/vagd/box.py` & `vagd-0.4.0/src/vagd/box.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,12 +4,13 @@
     UBUNTU_FOCAL64 = 'ubuntu/focal64'
     UBUNTU_BIONIC64 = 'ubuntu/bionic64'
     UBUNTU_XENIAL64 = 'ubuntu/xenial64'
     CLOUDIMAGE_JAMMY = 'https://cloud-images.ubuntu.com/jammy/current/jammy-server-cloudimg-amd64.img'
     CLOUDIMAGE_FOCAL = 'https://cloud-images.ubuntu.com/focal/current/focal-server-cloudimg-amd64.img'
     CLOUDIMAGE_BIONIC = 'https://cloud-images.ubuntu.com/bionic/current/bionic-server-cloudimg-amd64.img'
     CLOUDIMAGE_XENIAL = 'https://cloud-images.ubuntu.com/xenial/current/xenial-server-cloudimg-amd64-disk1.img'
-    CLOUDIMAGE_JAMMY_ARM = 'https://cloud-images.ubuntu.com/jammy/20230330/jammy-server-cloudimg-arm64.img'
+    CLOUDIMAGE_JAMMY_ARM = 'https://cloud-images.ubuntu.com/jammy/current/jammy-server-cloudimg-arm64.img'
     DOCKER_JAMMY = 'ubuntu:jammy'
     DOCKER_FOCAL = 'ubuntu:focal'
     DOCKER_BIONIC = 'ubuntu:bionic'
     DOCKER_XENIAL = 'ubuntu:xenial'
+    DOCKER_ALPINE_316 = 'alpine:3.16.6'
```

### Comparing `vagd-0.3.9/src/vagd/gdb/__init__.pyi` & `vagd-0.4.0/src/vagd/gdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.3.9/src/vagd/gdb/events.pyi` & `vagd-0.4.0/src/vagd/gdb/events.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.3.9/src/vagd/gdb/printing.pyi` & `vagd-0.4.0/src/vagd/gdb/printing.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.3.9/src/vagd/gdb/types.pyi` & `vagd-0.4.0/src/vagd/gdb/types.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.3.9/src/vagd/gdb/xmethod.pyi` & `vagd-0.4.0/src/vagd/gdb/xmethod.pyi`

 * *Files identical despite different names*

### Comparing `vagd-0.3.9/src/vagd/helper.py` & `vagd-0.4.0/src/vagd/helper.py`

 * *Files identical despite different names*

### Comparing `vagd-0.3.9/src/vagd/template.txt` & `vagd-0.4.0/test/test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,48 @@
 #!/bin/python
-from vagd import Vagd, Qegd, Dogd, Box
+import os
+import time
+
+from vagd import Vagd, Qegd, Shgd, Dogd, wrapper, Box
 from pwn import *
 
 GDB_OFF = 0x555555555000
 IP = ''
 PORT = 0
-BINARY = ''
+BINARY = './bin/sysinfo'
 ARGS = []
 ENV = {}
+API = True
 GDB = f"""
-
+b main
 c"""
 
 context.binary = exe = ELF(BINARY, checksec=False)
 context.aslr = False
 
 byt = lambda x: str(x).encode()
 
 
-vm = None
-def get_target(**kw):
-    global vm
-    if args.REMOTE:
-        context.log_level = 'debug'
-        return remote(IP, PORT)
-
-    if not vm:
-        vm = Vagd(exe.path, vbox=Box.UBUNTU_FOCAL64, ex=True, fast=True)
-        # vm = Qegd(exe.path, img=Box.CLOUDIMAGE_FOCAL, user='ubuntu', ex=True, fast=True)
-        # vm = Dogd(exe.path, image=Box.DOCKER_FOCAL, ex=True, fast=True)
-    return vm.start(argv=ARGS, env=ENV, gdbscript=GDB, **kw)
-
+def vms():
+    vm = Vagd(exe.path, vbox=Box.UBUNTU_FOCAL64, tmp=True, fast=True, ex=True)
+    yield vm
+    vm._v.halt()
+    vm = Dogd(exe.path, user='ubuntu', image=Box.DOCKER_FOCAL, tmp=True, ex=True, fast=True)
+    yield vm
+    vm._client.containers.get(vm._id).kill()
+    vm = Qegd(exe.path, user='ubuntu', img=Box.CLOUDIMAGE_FOCAL, tmp=True, ex=True, fast=True)
+    yield vm
+    yield Shgd(exe.path, user=vm._user, port=vm._port, tmp=True, ex=True, fast=True)
+    os.system('kill $(pgrep qemu)')
+    yield wrapper.Empty()
+
+
+for vm in vms():
+    t = vm.start(argv=ARGS, env=ENV, gdbscript=GDB, api=API)
+
+    g = wrapper.GDB(t)
+    g.execute('p "PWN"')
+    g.execute('c')
 
-t = get_target()
+    t.recvall()
 
-t.interactive()
+print("Everything executed without errors")
```

### Comparing `vagd-0.3.9/src/vagd/virts/pwngd.py` & `vagd-0.4.0/src/vagd/virts/pwngd.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,16 +10,18 @@
     LOCAL_DIR = './.vagd/'
     HOME_DIR = os.path.expanduser('~/.vagd/')
     SYSROOT = LOCAL_DIR + 'sysroot/'
     SYSROOT_LIB = SYSROOT + 'lib/'
     SYSROOT_LIB_DEBUG = SYSROOT + 'lib/debug'
     KEYFILE = LOCAL_DIR + 'keyfile'
     DEFAULT_PORT = 2222
+    STATIC_GDBSRV_PORT = 42069
 
     _path: str
+    _gdbsrvport: int
     _binary: str
     _ssh: pwn.ssh
     _experimental: bool
     _fast: bool
 
     @abstractmethod
     def _vm_setup(self) -> None:
@@ -52,19 +54,19 @@
         mount remote dir on local wiith sshfs
         :param remote_dir: directory on remote to mount
         :param local_dir: local mount point
         """
         if not which('sshfs'):
             pwn.log.error('sshfs isn\'t installed')
         cmd = Pwngd._SSHFS_TEMPLATE.format(port=self._ssh.port,
-                                               keyfile="$PWD/" + self._ssh.keyfile,
-                                               user=self._ssh.user,
-                                               host=self._ssh.host,
-                                               remote_dir=remote_dir,
-                                               local_dir=local_dir)
+                                           keyfile="$PWD/" + self._ssh.keyfile,
+                                           user=self._ssh.user,
+                                           host=self._ssh.host,
+                                           remote_dir=remote_dir,
+                                           local_dir=local_dir)
         pwn.log.info(cmd)
         os.system(cmd)
 
     def _mount_lib(self, remote_lib: str = '/usr/lib') -> None:
         """
         mount the lib directory of remote
         """
@@ -109,31 +111,34 @@
             self._ssh.upload(file, remote=remote)
 
     def __init__(self,
                  binary: str,
                  files: Union[str, list[str]] = None,
                  packages: Iterable = None,
                  tmp: bool = False,
+                 gdbsrvport: int = None,
                  fast: bool = False,
                  ex: bool = False):
         """
         Default init setups provided ssh machine
 
         :param binary: binary for VM debugging
         :param files: other files or directories that need to be uploaded to VM
         :param packages: packages to install on vm
         :param tmp: if a temporary directory should be created for files
+        :param gdbsrvport: specify static gdbserver port, REQURIES port forwarding to localhost
         :param fast: mounts libs locally for faster symbol extraction (experimental)
         :param ex: if experimental features should be enabled
         """
 
         if packages is not None:
             self._install_packages(packages)
 
         self._path = binary
+        self._gdbsrvport = gdbsrvport
         self._binary = './' + os.path.basename(binary)
 
         self._fast = fast
         self._experimental = ex
 
         if self._fast:
             if self._experimental:
@@ -194,27 +199,34 @@
 
         args, env = pwn.gdb.misc.normalize_argv_env(args, env, pwn.log)
         if env:
             env = {bytes(k): bytes(v) for k, v in env}
 
         args = pwn.gdb._gdbserver_args(args=args, which=which, env=env)
 
+        # set static port if wanted
+        if self._gdbsrvport is not None:
+            for i in range(len(args)):
+                if args[i] == 'localhost:0':
+                    args[i] = f':{self._gdbsrvport}'
+                    break
+
         # Make sure gdbserver/qemu is installed
         if not which(args[0]):
             pwn.log.error("%s is not installed" % args[0])
 
         # Start gdbserver/qemu
         # (Note: We override ASLR here for the gdbserver process itself.)
         gdbserver = runner(args, env=env, aslr=1, **kwargs)
 
         # Set the .executable on the process object.
         gdbserver.executable = exe
 
         # Find what port we need to connect to
-        port = pwn.gdb._gdbserver_port(gdbserver, ssh)
+        port = pwn.gdb._gdbserver_port(gdbserver, ssh) if self._gdbsrvport is None else self._gdbsrvport
 
         host = '127.0.0.1'
 
         if self._fast:
             gdb_args += ["-ex", f"set sysroot {pathlib.Path().resolve()}/{Pwngd.SYSROOT}"]
             gdbscript = f"set debug-file-directory {Pwngd.SYSROOT_LIB_DEBUG}\n" + gdbscript
         elif sysroot:
@@ -266,31 +278,29 @@
 
     def start(self,
               argv: list[str] = None,
               gdbscript: str = '',
               api: bool = None,
               sysroot: str = None,
               gdb_args: list = None,
-              ex: bool = False,
               **kwargs) -> pwn.process:
         """
         start binary on remote and return pwn.process
 
         :param argv: commandline arguments for binary
         :param gdbscript: GDB script for GDB
         :param api: if GDB API should be enabled (experimental)
         :param sysroot: sysroot dir (experimental)
         :param gdb_args: extra gdb args (experimental)
-        :param ex: enable experimental features (if not set in constructor)
         :param kwargs: pwntool parameters
         :return: pwntools process, if api=True tuple with gdb api
         """
         if pwn.args.GDB:
-            if ex or self._experimental:
+            if self._experimental:
                 return self.debug(argv=argv, gdbscript=gdbscript, gdb_args=gdb_args, sysroot=sysroot,
                                   api=api, **kwargs)
             else:
                 if gdb_args or sysroot or api:
-                    pwn.error('requires experimental features, activate with ex=True')
+                    pwn.error('requires experimental features, activate with ex=True in constructor')
                 return self.pwn_debug(argv=argv, gdbscript=gdbscript, sysroot=sysroot, **kwargs)
         else:
             return self.process(argv=argv, **kwargs)
```

### Comparing `vagd-0.3.9/src/vagd/virts/qegd.py` & `vagd-0.4.0/src/vagd/virts/qegd.py`

 * *Files identical despite different names*

### Comparing `vagd-0.3.9/src/vagd/virts/shgd.py` & `vagd-0.4.0/src/vagd/virts/shgd.py`

 * *Files identical despite different names*

### Comparing `vagd-0.3.9/src/vagd/virts/vagd.py` & `vagd-0.4.0/src/vagd/virts/vagd.py`

 * *Files identical despite different names*

### Comparing `vagd-0.3.9/src/vagd/wrapper.py` & `vagd-0.4.0/src/vagd/wrapper.py`

 * *Files identical despite different names*

### Comparing `vagd-0.3.9/src/vagd.egg-info/PKG-INFO` & `vagd-0.4.0/src/vagd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vagd
-Version: 0.3.9
+Version: 0.4.0
 Summary: VirtuAlization GDb integrations in pwntools
 Author-email: 0x6fe1be2 <author@example.com>
 Project-URL: Homepage, https://github.com/gfelber/vagd
 Project-URL: Documentation, https://gfelber.github.io/vagd/
 Project-URL: Bug Tracker, https://github.com/gfelber/vagd/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -70,14 +70,15 @@
   * [CLOUDIMAGE_BIONIC](https://cloud-images.ubuntu.com/bionic/current/bionic-server-cloudimg-amd64.img)
   * [CLOUDIMAGE_XENIAL](https://cloud-images.ubuntu.com/xenial/current/xenial-server-cloudimg-amd64-disk1.img)
 * Docker
   * DOCKER_JAMMY = 'ubuntu:jammy'
   * DOCKER_FOCAL = 'ubuntu:focal'
   * DOCKER_BIONIC = 'ubuntu:bionic'
   * DOCKER_XENIAL = 'ubuntu:xenial'
+  * DOCKER_ALPINE_316 = 'alpine:3.16.6'
 
 
 currently only distributions that use `apt` are supported
 
 
 
 ## Future plans
```

### Comparing `vagd-0.3.9/src/vagd.egg-info/SOURCES.txt` & `vagd-0.4.0/src/vagd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

