# Comparing `tmp/auto_everything-3.8.tar.gz` & `tmp/auto_everything-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/auto_everything-3.8.tar", last modified: Mon Nov  9 13:20:28 2020, max compression
+gzip compressed data, was "auto_everything-3.9.tar", last modified: Sun Jan 23 13:34:26 2022, max compression
```

## Comparing `auto_everything-3.8.tar` & `auto_everything-3.9.tar`

### file list

```diff
@@ -1,28 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-09 13:20:28.622648 auto_everything-3.8/
--rw-r--r--   0 root         (0) root         (0)     6092 2020-11-09 13:20:28.622648 auto_everything-3.8/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3818 2020-11-09 11:21:47.000000 auto_everything-3.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-09 13:20:28.622648 auto_everything-3.8/auto_everything/
--rw-rw-r--   0 root         (0) root         (0)        0 2020-06-15 13:44:12.000000 auto_everything-3.8/auto_everything/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    28459 2020-11-09 11:21:47.000000 auto_everything-3.8/auto_everything/base.py
--rw-rw-r--   0 root         (0) root         (0)     2071 2020-07-11 22:32:09.000000 auto_everything-3.8/auto_everything/camera.py
--rw-rw-r--   0 root         (0) root         (0)    10651 2020-10-25 17:33:35.000000 auto_everything-3.8/auto_everything/disk.py
--rw-rw-r--   0 root         (0) root         (0)    11780 2020-10-25 17:33:35.000000 auto_everything-3.8/auto_everything/gui.py
--rw-rw-r--   0 root         (0) root         (0)     3528 2020-06-15 13:44:12.000000 auto_everything-3.8/auto_everything/humanity.py
--rw-rw-r--   0 root         (0) root         (0)     3214 2020-06-15 13:44:12.000000 auto_everything-3.8/auto_everything/language.py
--rw-rw-r--   0 root         (0) root         (0)     2898 2020-06-15 13:44:12.000000 auto_everything-3.8/auto_everything/math.py
--rw-rw-r--   0 root         (0) root         (0)     1206 2020-10-25 17:33:35.000000 auto_everything-3.8/auto_everything/ml.py
--rw-rw-r--   0 root         (0) root         (0)     1805 2020-07-11 22:32:09.000000 auto_everything-3.8/auto_everything/network.py
--rw-rw-r--   0 root         (0) root         (0)       76 2020-11-09 13:20:20.000000 auto_everything-3.8/auto_everything/terminal.py
--rw-rw-r--   0 root         (0) root         (0)    46147 2020-10-25 17:33:35.000000 auto_everything-3.8/auto_everything/video.py
--rw-rw-r--   0 root         (0) root         (0)     2072 2020-06-30 08:21:04.000000 auto_everything-3.8/auto_everything/web.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-09 13:20:28.622648 auto_everything-3.8/auto_everything/x11/
--rw-rw-r--   0 root         (0) root         (0)    11191 2020-07-11 22:32:09.000000 auto_everything-3.8/auto_everything/x11/myx11.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-09 13:20:28.622648 auto_everything-3.8/auto_everything.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     6092 2020-11-09 13:20:28.000000 auto_everything-3.8/auto_everything.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      587 2020-11-09 13:20:28.000000 auto_everything-3.8/auto_everything.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2020-11-09 13:20:28.000000 auto_everything-3.8/auto_everything.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)      184 2020-11-09 13:20:28.000000 auto_everything-3.8/auto_everything.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       16 2020-11-09 13:20:28.000000 auto_everything-3.8/auto_everything.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2020-11-09 13:20:28.622648 auto_everything-3.8/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1420 2020-11-09 11:21:47.000000 auto_everything-3.8/setup.py
--rw-rw-r--   0 root         (0) root         (0)     4250 2020-10-25 17:33:35.000000 auto_everything-3.8/super_setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2022-01-23 13:34:26.132426 auto_everything-3.9/
+-rw-r--r--   0 root         (0) staff       (20)    35147 2021-12-30 01:14:24.000000 auto_everything-3.9/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     4499 2022-01-23 13:34:26.132258 auto_everything-3.9/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     3827 2021-12-30 01:14:24.000000 auto_everything-3.9/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2022-01-23 13:34:26.131541 auto_everything-3.9/auto_everything/
+-rw-r--r--   0 root         (0) staff       (20)      274 2021-12-30 01:14:24.000000 auto_everything-3.9/auto_everything/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      191 2021-12-30 01:14:24.000000 auto_everything-3.9/auto_everything/all.py
+-rw-r--r--   0 root         (0) staff       (20)     3162 2021-12-30 01:14:24.000000 auto_everything-3.9/auto_everything/audio.py
+-rw-r--r--   0 root         (0) staff       (20)     8829 2021-12-30 01:14:24.000000 auto_everything-3.9/auto_everything/base.py
+-rw-r--r--   0 root         (0) staff       (20)     2019 2021-12-30 01:14:24.000000 auto_everything-3.9/auto_everything/camera.py
+-rw-r--r--   0 root         (0) staff       (20)     2479 2021-12-30 01:14:24.000000 auto_everything-3.9/auto_everything/database.py
+-rw-r--r--   0 root         (0) staff       (20)     4009 2021-12-30 01:14:24.000000 auto_everything-3.9/auto_everything/develop.py
+-rw-r--r--   0 root         (0) staff       (20)    14846 2022-01-03 00:36:59.000000 auto_everything-3.9/auto_everything/disk.py
+-rw-r--r--   0 root         (0) staff       (20)    13803 2021-12-30 01:14:24.000000 auto_everything-3.9/auto_everything/gui.py
+-rw-r--r--   0 root         (0) staff       (20)     3533 2021-12-30 01:14:24.000000 auto_everything-3.9/auto_everything/humanity.py
+-rw-r--r--   0 root         (0) staff       (20)     1485 2021-12-30 01:14:24.000000 auto_everything-3.9/auto_everything/image.py
+-rw-r--r--   0 root         (0) staff       (20)     3570 2021-12-30 01:14:24.000000 auto_everything-3.9/auto_everything/io.py
+-rw-r--r--   0 root         (0) staff       (20)     3214 2021-12-30 01:14:24.000000 auto_everything-3.9/auto_everything/language.py
+-rw-r--r--   0 root         (0) staff       (20)     2902 2021-12-30 01:14:24.000000 auto_everything-3.9/auto_everything/math.py
+-rw-r--r--   0 root         (0) staff       (20)     1500 2021-12-30 01:14:24.000000 auto_everything-3.9/auto_everything/ml.py
+-rw-r--r--   0 root         (0) staff       (20)     2256 2021-12-30 01:14:24.000000 auto_everything-3.9/auto_everything/monitor.py
+-rw-r--r--   0 root         (0) staff       (20)      790 2021-12-30 01:14:24.000000 auto_everything-3.9/auto_everything/my_email.py
+-rw-r--r--   0 root         (0) staff       (20)     2193 2022-01-01 11:30:23.000000 auto_everything-3.9/auto_everything/network.py
+-rw-r--r--   0 root         (0) staff       (20)     8762 2021-12-30 01:14:24.000000 auto_everything-3.9/auto_everything/python.py
+-rw-r--r--   0 root         (0) staff       (20)    11855 2022-01-10 04:07:21.000000 auto_everything-3.9/auto_everything/terminal.py
+-rw-r--r--   0 root         (0) staff       (20)    61957 2022-01-08 07:30:16.000000 auto_everything-3.9/auto_everything/video.py
+-rw-r--r--   0 root         (0) staff       (20)     2577 2021-12-30 01:14:24.000000 auto_everything-3.9/auto_everything/web.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2022-01-23 13:34:26.132076 auto_everything-3.9/auto_everything.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     4499 2022-01-23 13:34:26.000000 auto_everything-3.9/auto_everything.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      781 2022-01-23 13:34:26.000000 auto_everything-3.9/auto_everything.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2022-01-23 13:34:26.000000 auto_everything-3.9/auto_everything.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)      218 2022-01-23 13:34:26.000000 auto_everything-3.9/auto_everything.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       16 2022-01-23 13:34:26.000000 auto_everything-3.9/auto_everything.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2022-01-23 13:34:26.132479 auto_everything-3.9/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     1503 2021-12-30 01:14:24.000000 auto_everything-3.9/setup.py
```

### Comparing `auto_everything-3.8/README.md` & `auto_everything-3.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 ```bash
 wget https://github.com/yingshaoxo/auto_everything/raw/master/env_setup.sh
 sudo bash env_setup.sh
 ```
 
 #### Magic
 ```bash
-wget https://github.com/yingshaoxo/auto_everything/raw/master/demo/install_YouCompleteMe.py
+wget https://github.com/yingshaoxo/auto_everything/raw/master/example/install_YouCompleteMe.py
 python3 install_YouCompleteMe.py
 ```
 
 #### Docs
 https://yingshaoxo.github.io/auto_everything
 
 ___
 
 
 ## Basic API
 #### Import
 ```python
-from auto_everything.base import Terminal
+from auto_everything.terminal import Terminal
 t = Terminal()
 ```
 
 #### Run a command and get reply
 ```python
 reply = t.run_command('uname -a')
 print(reply)
@@ -79,15 +79,15 @@
 
 ___
 
 
 ## For simplify Python development
 #### Import
 ```python
-from auto_everything.base import Python
+from auto_everything.python import Python
 py = Python()
 ```
 
 #### Turn `Python Class` into a `Command Line Program`
 ```python
 py.fire(your_class_name)
 ```
```

### Comparing `auto_everything-3.8/auto_everything/camera.py` & `auto_everything-3.9/auto_everything/camera.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-from typing import List
-from pathlib import Path
-import os
 import pyfakewebcam
 import cv2
 
 from auto_everything.base import Terminal
 t = Terminal(debug=True)
 
 
 class FakeCamera():
     """
     This module based on `pyfakewebcam`.
     """
+
     def __init__(self, device: str = None, width: int = 640, height: int = 480):
         list_command = "v4l2-ctl --list-devices"
         list_devices = t.run_command(list_command)
         assert "not found" not in list_devices, f"{list_devices}\n\nv4l2-ctl not found, you may have to install it with 'sudo apt install v4l2loopback-utils'"
         assert "v4l2loopback" in list_devices, f"{list_devices}\n\nTo create a fake camera, you have to add a dummy device first by 'sudo modprobe v4l2loopback'"
         lines = list_devices.split("\n")
         the_device = None
         for index, line in enumerate(lines):
-            if index < len(lines)-1:
-                if ("v4l2loopback" in line) and "/dev/video" in lines[index+1]:
-                    the_device = lines[index+1].strip()
+            if index < len(lines) - 1:
+                if ("v4l2loopback" in line) and "/dev/video" in lines[index + 1]:
+                    the_device = lines[index + 1].strip()
         if device == None:
             assert the_device != None, f"{list_devices}\n\ncan't auto find the dummy device, you may have to specify it manullay: FakeCamera('/dev/video*')"
             self.device = the_device
         else:
             self.device = device
         self.camera = pyfakewebcam.FakeWebcam(self.device, width, height)
```

### Comparing `auto_everything-3.8/auto_everything/disk.py` & `auto_everything-3.9/auto_everything/disk.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,88 @@
-from typing import List
+import datetime
+import pathlib
+import tempfile
+from typing import List, Tuple, Union
 from pathlib import Path
 import os
 import re
 import json
 import hashlib
 import unicodedata
 import string
+from io import BytesIO
 
-from auto_everything.base import Terminal
+from auto_everything.terminal import Terminal
 t = Terminal(debug=True)
 
 
-class Common():
+class Common:
     def __init__(self):
-        self._auto_everything_config_folder = os.path.expanduser("~/.auto_everything")
+        self._auto_everything_config_folder = os.path.expanduser(
+            "~/.auto_everything")
         # print(self._auto_everything_config_folder)
         if not os.path.exists(self._auto_everything_config_folder):
             os.mkdir(self._auto_everything_config_folder)
 
     def _create_a_sub_config_folder_for_auto_everything(self, module_name: str):
-        sub_folder_path = os.path.join(self._auto_everything_config_folder, module_name)
+        sub_folder_path = os.path.join(
+            self._auto_everything_config_folder, module_name)
         if not os.path.exists(sub_folder_path):
             os.mkdir(sub_folder_path)
         return sub_folder_path
 
 
-class Disk():
+class Disk:
     """
     Some useful functions to handle your disk
     """
 
     def __init__(self):
-        pass
+        self.temp_dir: str = tempfile.gettempdir()
+
+    def _expand_user(self, path: Union[str, pathlib.PosixPath]):
+        # print(type(path))
+        if type(path) == pathlib.PosixPath:
+            path = path.as_posix()
+        if len(path) > 0:
+            if path[0] == "~":
+                path = os.path.expanduser(path)
+        return path
 
     def exists(self, path: str) -> bool:
         """
         Check if a file or folder exist.
 
         Parameters
         ----------
         path: string
             the file path
         """
+        path = self._expand_user(path)
         return Path(path).exists()
 
+    def executable(self, path: str) -> bool:
+        return os.access(path, os.X_OK)
+
+    def concatenate_paths(self, *path):
+        return os.path.join(*path)
+
     def get_files(self, folder: str, recursive: bool = True, type_limiter: List[str] = None) -> List[str]:
         """
         Get files recursively under a folder.
 
         Parameters
         ----------
         folder: string
         recursive: bool
         type_limiter: List[str]
             a list used to do a type filter, like [".mp3", ".epub"]
         """
-        assert os.path.exists(folder), f"{path} is not exist!"
+        folder = self._expand_user(folder)
+        assert os.path.exists(folder), f"{folder} is not exist!"
         if recursive == True:
             files = []
             for root, dirnames, filenames in os.walk(folder):
                 for filename in filenames:
                     file = os.path.join(root, filename)
                     if os.path.isfile(file):
                         if type_limiter:
@@ -67,36 +90,47 @@
                             if p.suffix in type_limiter:
                                 files.append(file)
                         else:
                             files.append(file)
 
         else:
             if type_limiter:
-                files = [os.path.join(folder, f) for f in os.listdir(folder) if os.path.isfile(os.path.join(folder, f)) and Path(os.path.join(folder, f)).suffix in type_limiter]
+                files = [os.path.join(folder, f) for f in os.listdir(folder) if
+                         os.path.isfile(os.path.join(folder, f)) and Path(
+                             os.path.join(folder, f)).suffix in type_limiter]
             else:
-                files = [os.path.join(folder, f) for f in os.listdir(folder) if os.path.isfile(os.path.join(folder, f))]
+                files = [os.path.join(folder, f) for f in os.listdir(
+                    folder) if os.path.isfile(os.path.join(folder, f))]
         return files
 
     def sort_files_by_time(self, files: List[str], reverse: bool = False):
         files.sort(key=os.path.getmtime, reverse=reverse)
         return files
 
-    def get_stem_and_suffix_of_a_file(self, path: str) -> str:
+    def get_stem_and_suffix_of_a_file(self, path: str) -> Tuple[str, str]:
         p = Path(path)
         return p.stem, p.suffix
 
+    def getDirectoryName(self, path: str):
+        path = self._expand_user(path)
+        return os.path.dirname(path)
+
+    def getFileName(self, path: str):
+        return os.path.split(path)[-1]
+
     def get_hash_of_a_file(self, path: str) -> str:
         """
         calculate the blake2s hash string based on the bytes of a file.
 
         Parameters
         ----------
         path: string
             the file path
         """
+        path = self._expand_user(path)
         with open(path, "rb") as f:
             file_hash = hashlib.blake2s()
             while True:
                 data = f.read(8192)
                 if not data:
                     break
                 file_hash.update(data)
@@ -111,15 +145,15 @@
         path: string
             actually it can be any string
         """
         file_hash = hashlib.blake2s()
         file_hash.update(path.encode(encoding="UTF-8"))
         return file_hash.hexdigest()
 
-    def get_safe_name(self, filename: str, replace_chars=' ') -> str:
+    def get_safe_name(self, filename: str, replace_chars: str = ' ') -> str:
         """
         get a valid file name by doing a replacement. (English only)
 
         Parameters
         ----------
         filename: string
             the unsafe filename
@@ -131,99 +165,187 @@
         char_limit = 255
 
         # replace spaces
         for r in replace_chars:
             filename = filename.replace(r, '_')
 
         # keep only valid ascii chars
-        cleaned_filename = unicodedata.normalize('NFKD', filename).encode('ASCII', 'ignore').decode()
+        cleaned_filename = unicodedata.normalize(
+            'NFKD', filename).encode('ASCII', 'ignore').decode()
 
         # keep only whitelisted chars
-        cleaned_filename = ''.join(c for c in cleaned_filename if c in whitelist)
+        cleaned_filename = ''.join(
+            c for c in cleaned_filename if c in whitelist)
         if len(cleaned_filename) > char_limit:
-            print("Warning, filename truncated because it was over {}. Filenames may no longer be unique".format(char_limit))
+            print("Warning, filename truncated because it was over {}. Filenames may no longer be unique".format(
+                char_limit))
         return cleaned_filename[:char_limit]
 
-    def get_file_size(self, path: str, level: str = "B") -> int:
+    def get_file_size(self, path: str, level: str = "B", bytes_size: int = None) -> int:
         """
         Get file size in the unit of  B, KB, MB.
-
         Parameters
         ----------
         path: string
             the file path
         level: string
             B, KB, or MB
+        bytes_size: int
+            a number represent the file size in bytes level
         """
-        file = Path(path)
-        assert file.exists(), f"{path} is not exist!"
-        bytes = file.stat().st_size
-        if (level == "B"):
-            return int('{:,.0f}'.format(bytes))
-        elif (level == "KB"):
-            return int('{:,.0f}'.format(bytes/float(1 << 10)))
-        elif (level == "MB"):
-            return int('{:,.0f}'.format(bytes/float(1 << 20)))
+        if bytes_size is None:
+            path = self._expand_user(path)
+            file = Path(path)
+            assert file.exists(), f"{path} is not exist!"
+            bytes_size = file.stat().st_size
+        if level == "B":
+            return int('{:.0f}'.format(bytes_size))
+        elif level == "KB":
+            return int('{:.0f}'.format(bytes_size / float(1 << 10)))
+        elif level == "MB":
+            return int('{:.0f}'.format(bytes_size / float(1 << 20)))
 
     def uncompress(self, path: str, folder: str = None) -> bool:
         """
         uncompress a file.
 
         Parameters
         ----------
         path: string
             the compressed file path
         folder: string
             where you want to put the uncompressed files into
         """
+        path = self._expand_user(path)
+        folder = self._expand_user(folder)
         assert self.exists(path), f"{path} was not exist"
+
         t.run(f"rm {folder} -fr")
         t.run(f"mkdir -p {folder}")
         assert self.exists(folder), f"{folder} was not exit"
         try:
             suffix = Path(path).suffix
             if suffix == ".zip":
                 t.run(f"unzip '{path}' -d '{folder}'")
                 if len(os.listdir(folder)) == 1:
                     t.run(f"cd '{folder}' && cd * && mv * .. -f")
             elif suffix == ".gz":
-                t.run(f"tar zxfv '{path}' '{folder}' --strip-components=1")
+                t.run(
+                    f"tar zxfv '{path}' --directory '{folder}' --strip-components=1")
+                if len(os.listdir(folder)) == 0:
+                    t.run(f"tar zxfv '{path}' --directory '{folder}'")
             if len(os.listdir(folder)):
                 return True
             else:
                 return False
         except Exception as e:
             raise e
 
+    def compress(self, paths: List[str], target: str):
+        """
+        compress a files to a target.
+
+        Parameters
+        ----------
+        paths: string of list
+        target: string
+            the compressed output file path
+        """
+        paths = [self._expand_user(path) for path in paths]
+        target = self._expand_user(target)
+        t.run(f"rm {target}")
+        for i, path in enumerate(paths):
+            if not self.exists(path):
+                raise Exception(f"{path} is not exist")
+            paths[i] = f'"{path}"'
+        t.run(f"zip -r -D {target} {' '.join(paths)}")
+
+    def get_a_temp_file_path(self, filename):
+        m = hashlib.sha256()
+        m.update(str(datetime.datetime.now()).encode("utf-8"))
+        m.update(filename.encode("utf-8"))
+        stem, suffix = self.get_stem_and_suffix_of_a_file(filename)
+        tempFilePath = os.path.join(self.temp_dir, m.hexdigest()[:10] + suffix)
+        return tempFilePath
+
+    def get_the_temp_dir(self):
+        return self.temp_dir
+
+    def getATempFilePath(self, filename):
+        m = hashlib.sha256()
+        m.update(str(datetime.datetime.now()).encode("utf-8"))
+        m.update(filename.encode("utf-8"))
+        stem, suffix = self.get_stem_and_suffix_of_a_file(filename)
+        tempFilePath = os.path.join(self.temp_dir, m.hexdigest()[:10] + suffix)
+        return tempFilePath
+
+    def create_a_new_folder_under_home(self, folder_name: str):
+        folder_path = self._expand_user(f"~/{folder_name}")
+        if not os.path.exists(folder_path):
+            # os.mkdir(folder_path)
+            t.run_command(f"mkdir -p {folder_path}")
+        return folder_path
+
+    def get_bytesio_from_a_file(self, filepath: str) -> BytesIO:
+        with open(filepath, 'rb') as fh:
+            buffer = BytesIO(fh.read())
+        return buffer
+
+    def save_bytesio_to_file(self, bytes_io: BytesIO, file_path: str):
+        bytes_io.seek(0)
+        with open(file_path, "wb") as f:
+            f.write(bytes_io.read())
+
+    def removeAFile(self, file_path: str):
+        file_path = self._expand_user(file_path)
+        if self.exists(file_path):
+            os.remove(file_path)
+
+    def convertBytesToBytesIO(self, bytes_data: bytes) -> BytesIO:
+        bytes_io = BytesIO()
+        bytes_io.write(bytes_data)
+        bytes_io.seek(0)
+        return bytes_io
+
+    def createAFolder(self, folder_path: str):
+        folder_path = self._expand_user(folder_path)
+        if not os.path.exists(folder_path):
+            os.mkdir(folder_path)
+
 
 class Store():
     """
     A key-value store.
     """
 
     def __init__(self, store_name: str, save_to_folder: str = None):
         self._common = Common()
 
         if save_to_folder is None or not os.path.exists(save_to_folder):
-            self._store_folder = self._common._create_a_sub_config_folder_for_auto_everything("store")
+            self._store_folder = self._common._create_a_sub_config_folder_for_auto_everything(
+                "store")
         else:
             self._store_folder = save_to_folder
 
         self._store_name = store_name.strip()
         self.__initialize_SQL()
 
     def __initialize_SQL(self):
         import sqlite3 as sqlite3
-        self._SQL_DATA_FILE = os.path.join(self._store_folder, f"{self._store_name}.db")
-        self._sql_conn = sqlite3.connect(self._SQL_DATA_FILE, check_same_thread=False)
+        self._SQL_DATA_FILE = os.path.join(
+            self._store_folder, f"{self._store_name}.db")
+        self._sql_conn = sqlite3.connect(
+            self._SQL_DATA_FILE, check_same_thread=False)
 
         def regular_expression(expr, item):
             reg = re.compile(expr, flags=re.DOTALL)
             return reg.search(item) is not None
-        self._sql_conn.create_function("REGEXP", 2, regular_expression)  # 2 here means two parameters. REGEXP is a fixed value
+
+        self._sql_conn.create_function("REGEXP", 2,
+                                       regular_expression)  # 2 here means two parameters. REGEXP is a fixed value
 
         self._sql_cursor = self._sql_conn.cursor()
         self._sql_cursor.execute(f'''CREATE TABLE IF NOT EXISTS {self._store_name}
                     (key TEXT, value TEXT)''')
 
     def __pre_process_key(self, key):
         key = str(key)
@@ -231,15 +353,16 @@
 
     def __pre_process_value(self, value):
         if not isinstance(value, str):
             try:
                 value = json.dumps(value)
             except Exception as e:
                 print(e)
-                raise Exception(f"The value you gave me is not a json object: {str(value)}")
+                raise Exception(
+                    f"The value you gave me is not a json object: {str(value)}")
         return value
 
     def __active_json_value(self, value):
         try:
             value = json.loads(value)
         except Exception as e:
             value = value
@@ -260,15 +383,16 @@
 
         Parameters
         ----------
         key: string
         """
         key = self.__pre_process_key(key)
 
-        results = self._sql_cursor.execute(f'SELECT EXISTS(SELECT 1 FROM {self._store_name} WHERE key="{key}" LIMIT 1)')
+        results = self._sql_cursor.execute(
+            f'SELECT EXISTS(SELECT 1 FROM {self._store_name} WHERE key="{key}" LIMIT 1)')
         if self._sql_cursor.fetchone()[0] > 0:
             return True
         else:
             return False
 
     def get(self, key, default_value):
         """
@@ -277,15 +401,16 @@
         Parameters
         ----------
         key: string
         default_value: string or an object that jsonable
         """
         key = self.__pre_process_key(key)
 
-        self._sql_cursor.execute(f'SELECT * FROM {self._store_name} WHERE key=?', (key,))
+        self._sql_cursor.execute(
+            f'SELECT * FROM {self._store_name} WHERE key=?', (key,))
         result = self._sql_cursor.fetchone()
         if result:
             return self.__active_json_value(result[1])
         else:
             return default_value
 
     def set(self, key, value):
@@ -297,15 +422,16 @@
         key: string
         value: string or an object that jsonable
         """
         key = self.__pre_process_key(key)
         value = self.__pre_process_value(value)
 
         if self.has_key(key):
-            self._sql_cursor.execute(f'UPDATE {self._store_name} SET value=? WHERE key=?', (value, key))
+            self._sql_cursor.execute(
+                f'UPDATE {self._store_name} SET value=? WHERE key=?', (value, key))
         else:
             command = f''' INSERT INTO {self._store_name} VALUES(?,?) '''
             self._sql_cursor.execute(command, (key, value))
         self._sql_conn.commit()
 
     def reset(self):
         """
@@ -329,8 +455,8 @@
     print(store.get_items())
     print(store.has_key("o"))
     print(store.get("ok", "alsjdkfla"))
     store.reset()
     print(store.get_items())
     """
     disk = Disk()
-    #print(disk.get_hash_of_a_path("/home/yingshaoxo/.python_history"))
+    # print(disk.get_hash_of_a_path("/home/yingshaoxo/.python_history"))
```

### Comparing `auto_everything-3.8/auto_everything/gui.py` & `auto_everything-3.9/auto_everything/gui.py`

 * *Files 25% similar despite different names*

```diff
@@ -63,25 +63,25 @@
         target_path = os.path.join(self._data_folder, picture_name + '.png')
         t.run_command(f'gnome-screenshot -a -f "{target_path}"')
 
     def delay(self, milliseconds):
         """
         delay for milliseconds
         """
-        time.sleep(milliseconds/1000)
+        time.sleep(milliseconds / 1000)
 
     def find_text(self, target_text, from_image=None):
         """
         will return a list of center points
 
         a point: (x, y)
         """
 
         try:
-            #from PIL import Image
+            # from PIL import Image
             import pyscreenshot as ImageGrab
         except ImportError:
             error = """
 To use this module, you have to install pyscreenshot:
     sudo pip3 install pyscreenshot
             """
             raise Exception(error)
@@ -105,16 +105,16 @@
         if (len(target_index) != 0):
             for t_index in target_index:
                 list_ = ['top', 'left', 'width', 'height']
                 my_dict = {}
                 for attribute in list_:
                     value = result[attribute][t_index]
                     my_dict.update({attribute: value})
-                x = my_dict['left'] + my_dict['width']/2
-                y = my_dict['top'] + my_dict['height']/2
+                x = my_dict['left'] + my_dict['width'] / 2
+                y = my_dict['top'] + my_dict['height'] / 2
                 return_list.append((x, y))
         if (len(return_list) != 0):
             return return_list
         else:
             return None
 
 
@@ -127,15 +127,15 @@
         CommonGUI.__init__(self, project_name=project_name)
         self.__time_takes_for_one_click = time_takes_for_one_click
         self.__grayscale = grayscale
 
     def __click(self, x, y, game=False):
         self.pyautogui.click(x, y, interval=self.__time_takes_for_one_click)
         if game == True:
-            self.pyautogui.click(x, y+1, interval=self.__time_takes_for_one_click)
+            self.pyautogui.click(x, y + 1, interval=self.__time_takes_for_one_click)
 
     def __get_tuple(self, element_name, confidence=0.9):
         self._make_sure_img_dict_exists()
         element_name = self.img_dict[element_name]
         return self.pyautogui.locateCenterOnScreen(element_name, confidence=confidence, grayscale=self.__grayscale)
 
     def hide_mouse(self):
@@ -223,15 +223,49 @@
 
     def set_mouse_position(self, x, y):
         self.pyautogui.moveTo(x, y)
 
     def mouse_click(self, x=None, y=None, button='left', interval=0.5, game=False):
         self.pyautogui.click(x=x, y=y, button=button, interval=interval)
         if game == True:
-            self.pyautogui.click(x=x+1, y=y+1, button=button, interval=interval)
+            self.pyautogui.click(x=x + 1, y=y + 1, button=button, interval=interval)
+
+    def write(self, text: str):
+        self.pyautogui.write(text)
+
+    def press(self, key: str):
+        """
+        self.pyautogui.KEYBOARD_KEYS
+
+        or
+
+        ['\t', '\n', '\r', ' ', '!', '"', '#', '$', '%', '&', "'", '(',
+         ')', '*', '+', ',', '-', '.', '/', '0', '1', '2', '3', '4', '5', '6', '7',
+         '8', '9', ':', ';', '<', '=', '>', '?', '@', '[', '\\', ']', '^', '_', '`',
+         'a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o',
+         'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', '{', '|', '}', '~',
+         'accept', 'add', 'alt', 'altleft', 'altright', 'apps', 'backspace',
+         'browserback', 'browserfavorites', 'browserforward', 'browserhome',
+         'browserrefresh', 'browsersearch', 'browserstop', 'capslock', 'clear',
+         'convert', 'ctrl', 'ctrlleft', 'ctrlright', 'decimal', 'del', 'delete',
+         'divide', 'down', 'end', 'enter', 'esc', 'escape', 'execute', 'f1', 'f10',
+         'f11', 'f12', 'f13', 'f14', 'f15', 'f16', 'f17', 'f18', 'f19', 'f2', 'f20',
+         'f21', 'f22', 'f23', 'f24', 'f3', 'f4', 'f5', 'f6', 'f7', 'f8', 'f9',
+         'final', 'fn', 'hanguel', 'hangul', 'hanja', 'help', 'home', 'insert', 'junja',
+         'kana', 'kanji', 'launchapp1', 'launchapp2', 'launchmail',
+         'launchmediaselect', 'left', 'modechange', 'multiply', 'nexttrack',
+         'nonconvert', 'num0', 'num1', 'num2', 'num3', 'num4', 'num5', 'num6',
+         'num7', 'num8', 'num9', 'numlock', 'pagedown', 'pageup', 'pause', 'pgdn',
+         'pgup', 'playpause', 'prevtrack', 'print', 'printscreen', 'prntscrn',
+         'prtsc', 'prtscr', 'return', 'right', 'scrolllock', 'select', 'separator',
+         'shift', 'shiftleft', 'shiftright', 'sleep', 'space', 'stop', 'subtract', 'tab',
+         'up', 'volumedown', 'volumemute', 'volumeup', 'win', 'winleft', 'winright', 'yen',
+         'command', 'option', 'optionleft', 'optionright']
+        """
+        self.pyautogui.press(key)
 
 
 class AndroidGUI(CommonGUI):
     """
     To interact with scrcpy by x11 and OpenCV.
     """
 
@@ -243,21 +277,22 @@
         self.myx11 = MyX11()
         self.__window_name = scrcpy_window_name
 
         assert "not found" not in t.run_command("adb devices"), """
 To use this module, you have to install adb:
     sudo apt install android-tools-adb
 """
-        
+
         try:
             from uiautomator import device as d
             self.d = d
         except Exception as e:
             print(e)
-            print("I suggest you to use uiautomator to handle your android phone. You can install it by: \nsudo pip3 install uiautomator")
+            print(
+                "I suggest you to use uiautomator to handle your android phone. You can install it by: \nsudo pip3 install uiautomator")
 
         info_of_android = t.run_command("adb shell dumpsys display")
         for line in info_of_android.split("\n"):
             if "StableDisplayWidth" in line:
                 self.__android_width = int(line.split("=")[1].strip())
             if "StableDisplayHeight" in line:
                 self.__android_height = int(line.split("=")[1].strip())
@@ -296,15 +331,15 @@
         template = cv2.imread(self.img_dict[element_name], cv2.IMREAD_GRAYSCALE)
         res = cv2.matchTemplate(from_image_grayscale, template, cv2.TM_CCOEFF_NORMED)
 
         loc = np.where(res >= threshold)
         result = []
         w, h = template.shape[::-1]
         for pt in zip(*loc[::-1]):
-            x, y = (pt[0] + w/2), (pt[1] + h/2)
+            x, y = (pt[0] + w / 2), (pt[1] + h / 2)
             result.append({"x": x, "y": y})
             if visual:
                 cv2.rectangle(from_image, pt, (pt[0] + w, pt[1] + h), (0, 0, 255), 2)
         if visual:
             return from_image, result
         return result
 
@@ -331,22 +366,22 @@
         point: {"x": 1920, "y": 1080}
             it's actually the result you get from function find_all().
         """
         assert "x" in point and "y" in point, f"You gave me a wrong point: {str(point)}"
         x = point["x"]
         y = point["y"]
         if landscape:
-            x = int(x/self.__screen_width*self.__android_height)
-            y = int(y/self.__screen_height*self.__android_width)
+            x = int(x / self.__screen_width * self.__android_height)
+            y = int(y / self.__screen_height * self.__android_width)
         else:
-            x = int(x/self.__screen_width*self.__android_width)
-            y = int(y/self.__screen_height*self.__android_height)
+            x = int(x / self.__screen_width * self.__android_width)
+            y = int(y / self.__screen_height * self.__android_height)
         t.run(f"adb shell input tap {x} {y}")
 
 
 if __name__ == "__main__":
     androidGUI = AndroidGUI("pixel")
-    while(True):
+    while (True):
         data = androidGUI.capture_screen()
         cv2.imshow('frame', data)
         if cv2.waitKey(1) & 0xFF == ord('q'):
             break
```

### Comparing `auto_everything-3.8/auto_everything/humanity.py` & `auto_everything-3.9/auto_everything/humanity.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
                 'negative_power',
                 'balanced_times'
             ])
         else:
             self.df = pd.read_csv(self.__df_path)
 
     def __str__(self):
-        return '-'*30 + '\n' + str(self.df.head())
+        return '-' * 30 + '\n' + str(self.df.head())
 
     def add_person(self, name):
         temp_df = self.df.loc[self.df['name'] == name]
         if len(temp_df) >= 1:
             print('You already have it')
         else:
             self.df = self.df.append(
@@ -83,16 +83,16 @@
         print(sorted_df.head())
 
     def commit(self):
         self.df.to_csv(self.__df_path, index=False)
 
 
 if __name__ == "__main__":
-    print('\n'*50)
+    print('\n' * 50)
     friendship = Friendship('/home/yingshaoxo/Documents/friendship.csv')
     friendship.add_person('A')
     friendship.add_person('B')
     friendship.giving('A', 5)
     friendship.taking('B', 3)
     friendship.seek_for_help()
     friendship.can_i_help()
-    #friendship.commit()
+    # friendship.commit()
```

### Comparing `auto_everything-3.8/auto_everything/language.py` & `auto_everything-3.9/auto_everything/language.py`

 * *Files identical despite different names*

### Comparing `auto_everything-3.8/auto_everything/math.py` & `auto_everything-3.9/auto_everything/math.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 class Password():
     """
     This is for hash password generation
     """
+
     def __init__(self, base_string):
         """
         base_string: a base_string for PassWord generation
         """
         import hashlib
         self.hashlib = hashlib
         self.__base_data = base_string.encode("utf-8")
@@ -28,23 +29,24 @@
         m = self.hashlib.sha512()
         m.update(self.__base_data)
 
         for data in data_list:
             m.update(data)
 
         result = m.hexdigest()
-        result = result[:length-1]
+        result = result[:length - 1]
         result = "A" + result
         return result
 
 
 class Calculator():
     """
     A class for advanced mathematics
     """
+
     def __init__(self):
         import sympy
         self.sympy = sympy
         self.sympy.init_printing(use_unicode=True)
 
     def symbol(self, symbol_string):
         """
```

### Comparing `auto_everything-3.8/auto_everything/network.py` & `auto_everything-3.9/auto_everything/network.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,40 @@
-from auto_everything.disk import Disk 
+from auto_everything.disk import Disk
 from pathlib import Path
 import os
-from pprint import pprint
+import http.client as httplib
 
 from auto_everything.base import Terminal, OS
+
 t = Terminal(debug=True)
 os_ = OS()
-
 disk = Disk()
 
 
-class Network():
+class Network:
     """
     I use this module to handle network stuff.
     """
+
     def __init__(self):
-        assert "not found" not in t.run_command("wget"), '''
+        assert "not found" not in t.run_command(
+            "wget"
+        ), """
 'wget' is required for this module to work
-You can install it with `sudo apt install wget`'''
+You can install it with `sudo apt install wget`"""
+
+    def available(self, timeout: int = 1):
+        conn = httplib.HTTPConnection("www.google.com", timeout=timeout)
+        try:
+            conn.request("HEAD", "/")
+            conn.close()
+            return True
+        except:
+            conn.close()
+            return False
 
     def download(self, url: str, target: str, size: str = "0B") -> bool:
         """
         Download a file from internet.
 
         Parameters
         ----------
@@ -35,24 +48,32 @@
         Returns
         -------
         bool
             return `false` if the specified size less than the file we downloaded
         """
         target = Path(target).expanduser().absolute()
         directory = target.parent
-        assert os.path.exists(directory), f"target directory '{directory}' is not exits"
+        assert os.path.exists(
+            directory), f"target directory '{directory}' is not exits"
         t.run(f"wget {url} -O {target}")
 
         number = int("".join([i for i in list(size) if i.isdigit()]))
         unit = size.replace(str(number), "")
-        assert unit in ["B", "KB", "MB"], f"number={number}, unit={unit}\nsize error, it should be 700B, 5KB, 40MB and so on."
+        assert unit in [
+            "B",
+            "KB",
+            "MB",
+        ], f"number={number}, unit={unit}\nsize error, it should be 700B, 5KB, 40MB and so on."
         the_file_size = disk.get_file_size(target, unit)
-        if (the_file_size > number):
+        if the_file_size > number:
             return True
         else:
             return False
 
 
 if __name__ == "__main__":
     net = Network()
-    result = net.download("https://github.com/yingshaoxo/My-books/raw/master/Tools.py", "~/.auto_everything/hi.txt")
+    result = net.download(
+        "https://github.com/yingshaoxo/My-books/raw/master/Tools.py",
+        "~/.auto_everything/hi.txt",
+    )
     print(result)
```

### Comparing `auto_everything-3.8/auto_everything/video.py` & `auto_everything-3.9/auto_everything/video.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import moviepy.video.fx.all as vfx
-from moviepy.editor import VideoFileClip, concatenate_videoclips
+from moviepy.editor import VideoFileClip, concatenate_videoclips, AudioFileClip
 import shutil
 import datetime
 import librosa
 import numpy as np
 import os
 import math
 import multiprocessing
 import json
 
-import pyaudio
-import sys
-import wave
+#import pyaudio
+#import sys
+#import wave
 import subprocess
 
 from typing import List, Tuple
-from auto_everything.base import Terminal, Python, IO
+from auto_everything.io import IO
+from auto_everything.terminal import Terminal
 from auto_everything.network import Network
 from auto_everything.disk import Disk
+
 t = Terminal(debug=True)
-py = Python()
 io_ = IO()
 network = Network()
 disk = Disk()
 
 
 def print_split_line():
-    print('\n' + '-'*20 + '\n')
+    print('\n' + '-' * 20 + '\n')
 
 
 def done():
     print_split_line()
     print('We are done, sir.')
     print_split_line()
 
@@ -120,14 +121,161 @@
     wav_path = try_to_get_absolutely_path(wav_path)
     make_sure_source_is_absolute_path(wav_path)
 
     y, sr = librosa.load(wav_path, sr=None)
     return y, sr
 
 
+class VideoUtils():
+    def convert_video_to_wav(self, source_video_path, target_wav_path):
+        return convert_video_to_wav(source_video_path, target_wav_path)
+
+    def get_mono_16khz_audio_array(self, sourceWavePath: str):
+        y, s = librosa.load(sourceWavePath, mono=True, sr=16000)
+        # s is audio sample rate
+        return y, s
+
+    def convert_array_to_batch_samples(self, y, durationInSecondsForEach=1.0):
+        samplesForEachOne = librosa.time_to_samples(
+            durationInSecondsForEach, sr=16000)
+        num_sections = math.ceil(y.shape[0] / samplesForEachOne)
+        return np.array_split(y, num_sections, axis=0)
+
+    def get_wav_infomation(self, wav_path):
+        wav_path = try_to_get_absolutely_path(wav_path)
+        make_sure_source_is_absolute_path(wav_path)
+
+        y, sr = librosa.load(wav_path, sr=None)
+        return y, sr
+
+    def merge_continues_intervals(self, intervals, thresholdInSeconds):
+        # merge continues videos
+        # if time betewwn two intervals are less than thresholdInSeconds, we merge them
+        i = 0
+        length = len(intervals)
+        modified = True
+        while modified == True:
+            modified = False
+            i = 0
+            while i < len(intervals):
+                if i + 1 < len(intervals):
+                    A = intervals[i][1]
+                    B = intervals[i + 1][0]
+                    d = B - A
+                    # print(d)
+                    if d < thresholdInSeconds:
+                        intervals[i][1] = intervals[i + 1][1]
+                        del intervals[i + 1]
+                        modified = True
+                i += 1
+        return intervals
+
+    def drop_too_short_intervals(self, intervals, thresholdInSeconds):
+        # remove too short videos
+        # if the time delta in a interval is less than thresholdInSeconds, we drop it
+        i = 0
+        length = len(intervals)
+        modified = True
+        while modified == True:
+            modified = False
+            i = 0
+            while i < len(intervals):
+                A = intervals[i][0]
+                B = intervals[i][1]
+                d = B - A
+                # print(d)
+                if d < thresholdInSeconds:
+                    del intervals[i]
+                    i -= 1
+                    modified = True
+                i += 1
+
+        return intervals
+
+    def get_intersection_of_two_intervals(self, A, B):
+        i = j = 0
+        ans = []
+        while i < len(A) and j < len(B):
+            start_a, end_a = A[i]
+            start_b, end_b = B[j]
+            if start_b <= start_a <= end_b:
+                ans.append([start_a, min(end_a, end_b)])
+                if end_a < end_b:
+                    i += 1
+                else:
+                    j += 1
+            elif start_a <= start_b <= end_a:
+                ans.append([start_b, min(end_a, end_b)])
+                if end_a < end_b:
+                    i += 1
+                else:
+                    j += 1
+            elif start_a < start_b:
+                i += 1
+            else:
+                j += 1
+        return ans
+
+    def fix_rotation(self, video):
+        """
+            Rotate the video based on orientation
+        """
+        rotation = video.rotation
+        if rotation == 90:  # If video is in portrait
+            video = vfx.rotate(video, -90)
+        elif rotation == 270:  # Moviepy can only cope with 90, -90, and 180 degree turns
+            # Moviepy can only cope with 90, -90, and 180 degree turns
+            video = vfx.rotate(video, 90)
+        elif rotation == 180:
+            video = vfx.rotate(video, 180)
+        return video
+
+
+videoUtils = VideoUtils()
+
+
+class AudioProcessor:
+    def __init__(self):
+        try:
+            import pydub
+            self.pydub = pydub
+        except Exception as e:
+            print("brew install ffmpeg")
+            print("python3 -m pip install pydub")
+            raise e
+
+    def getCompleteTimeRangeForNoSilenceAndSilenceAudioSlice(self, soundObject, silence_threshold=-50):
+        originalSequenceLength = len(soundObject)
+
+        voiceNoSilenceTimeRangeList = self.pydub.silence.detect_nonsilent(
+            soundObject, silence_thresh=silence_threshold)
+
+        new_list = []
+
+        for index, item in enumerate(voiceNoSilenceTimeRangeList):
+            if index == 0:
+                new_list.append([item[0], item[1], 1])
+            else:
+                new_list.append([item[0], item[1], 1])
+                if item[0] != voiceNoSilenceTimeRangeList[index-1][1]:
+                    new_list.insert(-1,
+                                    [voiceNoSilenceTimeRangeList[index-1][1], item[0], 0])
+
+        if len(new_list):
+            if new_list[0][0] != 0:
+                new_list.insert(0, [0, new_list[0][0], 0])
+            if new_list[-1][1] != originalSequenceLength:
+                new_list.append([new_list[-1][1], originalSequenceLength, 0])
+
+        return new_list
+
+
+audioProcessor = AudioProcessor()
+
+
 # we'll use ffmpeg to do the real work
 class Video():
     """
     This is a powerful video module
 
     It's based on:
     1. ubuntu core
@@ -135,97 +283,120 @@
     3. ffmpeg
     4. moviepy
     """
 
     def __init__(self):
         self._cpu_core_numbers = multiprocessing.cpu_count()
 
-    def _get_voice_parts(self, source_audio_path, top_db, minimum_interval_time_in_seconds=1.0):
+    def _get_voice_parts(self, source_audio_path, top_db, minimum_interval_time_in_seconds=1.0, skip_sharp_noise=False):
         y, sr = get_wav_infomation(source_audio_path)
         minimum_interval_samples = librosa.core.time_to_samples(
             minimum_interval_time_in_seconds, sr)
 
         def ignore_short_noise(parts):
             # ignore short noise
             new_parts = []
             for index, part in enumerate(parts):
                 if index == 0:
                     new_parts.append(list(part))
                     continue
                 else:
-                    noise_interval = (part[0] - parts[index-1][1])
+                    noise_interval = (part[0] - parts[index - 1][1])
                     if (noise_interval > minimum_interval_samples):
-                        time_gaps = (part[0]-parts[index-1][1])*0.1
+                        time_gaps = (part[0] - parts[index - 1][1]) * 0.1
                         # we fear if the time_gaps is too long
                         if time_gaps >= minimum_interval_samples:
                             time_gaps = minimum_interval_samples // 2
                         new_parts.append(
-                            [parts[index-1][1],
-                             parts[index-1][1] + time_gaps
+                            [parts[index - 1][1],
+                             parts[index - 1][1] + time_gaps
                              ]
                         )
                         new_parts.append(
                             [part[0] - time_gaps,
                              part[0]
                              ]
                         )
                         new_parts.append(list(part))
                     else:
-                        new_parts.append([parts[index-1][1], part[0]])
+                        new_parts.append([parts[index - 1][1], part[0]])
                         new_parts.append(list(part))
 
             the_missing_final = new_parts[-1][1]
             # combine continuous voice
             final_parts = []
             first = -1
             for index, part in enumerate(new_parts):
                 if index == 0:
                     final_parts.append(part)
                     continue
                 else:
-                    inverval = (part[0] - new_parts[index-1][1])
+                    inverval = (part[0] - new_parts[index - 1][1])
                     if (inverval == 0):
                         if first == -1:
-                            first = new_parts[index-1][0]
+                            first = new_parts[index - 1][0]
                     else:
                         if (first == -1):
                             final_parts.append([part[0], part[1]])
                         else:
-                            final_parts.append([first, new_parts[index-1][1]])
+                            final_parts.append(
+                                [first, new_parts[index - 1][1]])
                             first = -1
 
             final_parts.append([final_parts[-1][1], the_missing_final])
 
             return np.array(final_parts)
 
         parts = librosa.effects.split(y, top_db=top_db)  # return samples
-        parts = ignore_short_noise(parts)
+
+        # parts = ignore_short_noise(parts)
 
         # new_y = librosa.effects.remix(self._y, parts) # receive samples
         # target_file_path = os.path.join(self._video_directory, "new_" + self._audio_name)
         # if t.exists(target_file_path):
         #    os.remove(target_file_path)
         # librosa.output.write_wav(target_file_path, new_y, self._sr)
 
         def from_samples_to_seconds(parts):
             parts = librosa.core.samples_to_time(parts, sr)  # return seconds
             new_parts = []
 
             def seconds_to_string_format(num):
                 return str(datetime.timedelta(seconds=num))
+
             for part in parts:
                 part1 = seconds_to_string_format(part[0])
                 part2 = seconds_to_string_format(part[1])
                 new_parts.append([part1, part2])
             return new_parts
 
-        parts[0] = [0, parts[0][1]]
+        # parts[0] = [0, parts[0][1]]
         parts = from_samples_to_seconds(parts)
 
-        return parts[1:]
+        newVersionOfParts = []
+
+        def to_seconds(s):
+            hr, min, sec = [float(x) for x in s.split(':')]
+            return hr * 3600 + min * 60 + sec
+
+        for part in parts:
+            A = part[0]
+            B = part[1]
+            A = to_seconds(A)
+            B = to_seconds(B)
+            newVersionOfParts.append([A, B])
+
+        parts = newVersionOfParts
+
+        if skip_sharp_noise:
+            parts = videoUtils.drop_too_short_intervals(parts, 0.1)  # 0.2
+            parts = videoUtils.merge_continues_intervals(
+                parts, thresholdInSeconds=0.5)  # 0.5
+
+        return parts
 
     def _get_voice_and_silence_parts(self, source_audio_path, top_db, minimum_interval_time_in_seconds=1.5):
         # let's assume 1=voice, 0=noise
         y, sr = get_wav_infomation(source_audio_path)
         minimum_interval_samples = librosa.core.time_to_samples(
             minimum_interval_time_in_seconds, sr)
 
@@ -235,70 +406,72 @@
             # ignore short noise
             new_parts = []
             for index, part in enumerate(parts):
                 if index == 0:
                     new_parts.append(list(part))
                     continue
                 else:
-                    noise_interval = (part[0] - parts[index-1][1])
+                    noise_interval = (part[0] - parts[index - 1][1])
                     if (noise_interval > minimum_interval_samples):
                         new_parts.append(
-                            [parts[index-1][1], parts[index-1][1]])
+                            [parts[index - 1][1], parts[index - 1][1]])
                         new_parts.append(list(part))
                     else:
-                        new_parts.append([parts[index-1][1], part[0]])
+                        new_parts.append([parts[index - 1][1], part[0]])
                         new_parts.append(list(part))
 
             the_missing_final = new_parts[-1][1]
             # combine continuous voice
             final_parts = []
             first = -1
             for index, part in enumerate(new_parts):
                 if index == 0:
                     final_parts.append(part)
                     continue
                 else:
-                    inverval = (part[0] - new_parts[index-1][1])
+                    inverval = (part[0] - new_parts[index - 1][1])
                     if (inverval == 0):
                         if first == -1:
-                            first = new_parts[index-1][0]
+                            first = new_parts[index - 1][0]
                     else:
                         if (first == -1):
                             final_parts.append([part[0], part[1]])
                         else:
-                            final_parts.append([first, new_parts[index-1][1]])
+                            final_parts.append(
+                                [first, new_parts[index - 1][1]])
                             first = -1
 
             final_parts.append([final_parts[-1][1], the_missing_final])
 
             return np.array(final_parts)
 
         parts = ignore_short_noise(parts)
         parts = parts[1:]
 
         def from_samples_to_seconds(part):
             part = librosa.core.samples_to_time(part, sr)  # return seconds
 
             def seconds_to_string_format(num):
                 return str(datetime.timedelta(seconds=num))
+
             return [seconds_to_string_format(part[0]), seconds_to_string_format(part[1])]
 
         voice_and_silence_parts = []
         for index, part in enumerate(parts):
             first = part[0]
             second = part[1]
             if index == 0:
                 if first != 0:
                     voice_and_silence_parts.append(
                         [0, from_samples_to_seconds([0, first])])
                     voice_and_silence_parts.append(
                         [1, from_samples_to_seconds([first, second])])
             else:
                 voice_and_silence_parts.append(
-                    [0, from_samples_to_seconds([parts[index-1][1], first])])
+                    [0, from_samples_to_seconds([parts[index - 1][1], first])])
                 voice_and_silence_parts.append(
                     [1, from_samples_to_seconds([first, second])])
 
         def remove_unwanted_parts(voice_and_silence_parts):
             return [part for part in voice_and_silence_parts if part[1][0] != part[1][1]]
 
         voice_and_silence_parts = remove_unwanted_parts(
@@ -317,17 +490,17 @@
             new_parts.append(
                 [part1 - start_timestamp, part2 - start_timestamp])
 
         all_silence = 0
         for index, part in enumerate(new_parts):
             if index == 0:
                 continue
-            all_silence += (part[0] - new_parts[index-1][1])
+            all_silence += (part[0] - new_parts[index - 1][1])
 
-        ratio = all_silence/new_parts[-1][1]
+        ratio = all_silence / new_parts[-1][1]
         return ratio
 
     def split_video_by_time_part(self, source_video_path, target_video_path, part):
         make_sure_source_is_absolute_path(source_video_path)
         make_sure_target_is_absolute_path(target_video_path)
         make_sure_target_does_not_exist(target_video_path)
 
@@ -351,17 +524,17 @@
         make_sure_target_is_absolute_path(target_folder)
 
         make_sure_target_does_not_exist(target_folder)
         if not t.exists(target_folder):
             os.mkdir(target_folder)
 
         for index, part in enumerate(time_intervals):
-            index = (6-len(str(index)))*'0' + str(index)
+            index = (6 - len(str(index))) * '0' + str(index)
 
-            target_video_path = add_path(target_folder, str(index)+".mp4")
+            target_video_path = add_path(target_folder, str(index) + ".mp4")
 
             self.split_video_by_time_part(
                 source_video_path, target_video_path, part)
 
         done()
 
     def link_videos(self, source_video_path_list, target_video_path, method=2, preset="ultrafast"):
@@ -398,19 +571,20 @@
             combine_command = f"ffmpeg -f concat -safe 0 -i '{txt_file_path}' '{target_video_path}'"
             t.run(combine_command, wait=True)
 
             make_sure_target_does_not_exist(txt_file_path)
         elif method == 2:
             # for the stupid moviepy library, it will case memory leak if you give it too much videos
             print(source_video_path_list)
-            clip_list = [VideoFileClip(clip)
+
+            clip_list = [videoUtils.fix_rotation(VideoFileClip(clip))
                          for clip in source_video_path_list]
             final_clip = concatenate_videoclips(clip_list)
             final_clip.write_videofile(
-                target_video_path, threads=self._cpu_core_numbers, preset=preset)
+                target_video_path, threads=self._cpu_core_numbers, preset=preset, audio_codec="aac", verbose=False)
 
             for clip in clip_list:
                 clip.close()
                 del clip
 
             del final_clip
 
@@ -495,15 +669,17 @@
         """)
 
         make_sure_target_does_not_exist(
             [audio_path, noise_sample_wav_path, noise_prof_path, no_noise_wav_path, loudnorm_wav_path])
 
         done()
 
-    def remove_silence_parts_from_video(self, source_video_path, target_video_path, db_for_split_silence_and_voice, minimum_interval_time_in_seconds=None, voice_only=False):
+    def remove_silence_parts_from_video(self, source_video_path, target_video_path, db_for_split_silence_and_voice,
+                                        minimum_interval_time_in_seconds=None, voice_only=False,
+                                        skip_sharp_noise=False):
         """
         Parameters
         ----------
         source_video_path: string
         target_video_path: string
         db_for_split_silence_and_voice: int
             normoly, it's `20` or `25`, but for some case if the volume is too small, `30` would be fine
@@ -518,43 +694,45 @@
         make_sure_source_is_absolute_path(source_video_path)
         make_sure_source_is_absolute_path(target_video_path)
 
         top_db = db_for_split_silence_and_voice
 
         working_dir = get_directory_name(target_video_path)
         audio_path = convert_video_to_wav(source_video_path, add_path(
-            working_dir, disk.get_hash_of_a_path(source_video_path)+'audio_for_remove_silence_parts_from_video.wav'))
+            working_dir, disk.get_hash_of_a_path(source_video_path) + 'audio_for_remove_silence_parts_from_video.wav'))
         temp_video_path = add_path(
-            working_dir, disk.get_hash_of_a_path(source_video_path)+'temp_for_remove_silence_parts_from_video.mp4')
+            working_dir, disk.get_hash_of_a_path(source_video_path) + 'temp_for_remove_silence_parts_from_video.mp4')
 
         if minimum_interval_time_in_seconds is None:
-            parts = self._get_voice_parts(audio_path, top_db)
+            parts = self._get_voice_parts(
+                audio_path, top_db, skip_sharp_noise=skip_sharp_noise)
         else:
             parts = self._get_voice_parts(
-                audio_path, top_db, minimum_interval_time_in_seconds)
+                audio_path, top_db, minimum_interval_time_in_seconds, skip_sharp_noise=skip_sharp_noise)
 
         # """
         parent_clip = VideoFileClip(source_video_path)
+        parent_clip = videoUtils.fix_rotation(parent_clip)
         clip_list = []
         length = len(parts)
         for index, part in enumerate(parts):
             try:
-                time_duration = (datetime.datetime.strptime(
-                    part[1], '%H:%M:%S.%f') - datetime.datetime.strptime(part[0], '%H:%M:%S.%f')).seconds
-                print(str(int(index/length*100))+"%,", "-".join(
-                    [p.split(".")[0] for p in part]) + ",", "cut " + str(time_duration) + " seconds")
+                time_duration = int(part[1] - part[0])
+                print(str(int(index / length * 100)) + "%,",
+                      "cut " + str(time_duration) + " seconds")
             except Exception as e:
                 print(e)
             clip_list.append(parent_clip.subclip(part[0], part[1]))
 
         concat_clip = concatenate_videoclips(clip_list)
 
         if not voice_only:
             concat_clip.write_videofile(
-                target_video_path, threads=self._cpu_core_numbers)
+                target_video_path, threads=self._cpu_core_numbers, audio_codec="aac", verbose=False
+            )
             concat_clip.close()
             del concat_clip
             make_sure_target_does_not_exist(audio_path)
             make_sure_target_does_not_exist(temp_video_path)
         else:
             if len(target_video_path.split(".")) >= 2:
                 target_audio_path = ".".join(
@@ -566,15 +744,16 @@
             concat_clip.close()
             make_sure_target_does_not_exist(audio_path)
             make_sure_target_does_not_exist(temp_video_path)
             return target_audio_path
 
         done()
 
-    def humanly_remove_silence_parts_from_video(self, source_video_path, target_video_path, db_for_split_silence_and_voice, minimum_interval=1):
+    def humanly_remove_silence_parts_from_video(self, source_video_path, target_video_path,
+                                                db_for_split_silence_and_voice, minimum_interval=1):
         """
         No difference with the last one, but in this function, you can check how many silence you can get rid of.
         Then you make the decision wheather you want to do this or not
 
         Parameters
         ----------
         source_video_path: string
@@ -586,44 +765,50 @@
         """
         source_video_path = try_to_get_absolutely_path(source_video_path)
         target_video_path = try_to_get_absolutely_path(target_video_path)
         source_video_path = os.path.abspath(source_video_path)
         target_video_path = os.path.abspath(target_video_path)
 
         working_dir = get_directory_name(target_video_path)
-        audio_path = convert_video_to_wav(source_video_path, add_path(
-            working_dir, 'audio_for_humanly_remove_silence_parts_from_video.wav'))
+        audio_path = add_path(
+            working_dir, 'audio_for_humanly_remove_silence_parts_from_video.wav')
+        if not os.path.exists(audio_path):
+            convert_video_to_wav(source_video_path, audio_path)
 
         temp_video_path = add_path(
             working_dir, 'temp_for_humanly_remove_silence_parts_from_video.mp4')
 
         try:
             # parts = self._get_voice_parts(
             #    source_audio_path=audio_path, top_db=db_for_split_silence_and_voice)
             # ratio = int(self._evaluate_voice_parts(parts) * 100)
             target_audio_path = self.remove_silence_parts_from_video(
-                source_video_path, target_video_path, db_for_split_silence_and_voice=db_for_split_silence_and_voice, minimum_interval_time_in_seconds=minimum_interval, voice_only=True)
+                source_video_path, target_video_path, db_for_split_silence_and_voice=db_for_split_silence_and_voice,
+                minimum_interval_time_in_seconds=minimum_interval, voice_only=True)
         except Exception as e:
             print(e)
             print()
             print(
                 "You probably gave me a wroung db value, try to make it smaller and try it again")
             exit()
 
         make_sure_target_does_not_exist(temp_video_path)
         make_sure_target_does_not_exist(audio_path)
 
+        os.system(f'xdg-open {target_audio_path}')
+
         answer = input(
-            f"Are you happy with the audio file: {target_audio_path}% ? (y/n) (you may have to exit this script to hear your audio from your computers)")
+            f"Are you happy with the audio file: {target_audio_path}% ? (y/n) (you may have to exit this script to hear your audio from your computers)\n")
         if answer.strip() == "y":
             print("ok, let's do it!")
 
             make_sure_target_does_not_exist(target_audio_path)
             self.remove_silence_parts_from_video(
-                source_video_path, target_video_path, db_for_split_silence_and_voice=db_for_split_silence_and_voice, minimum_interval_time_in_seconds=minimum_interval)
+                source_video_path, target_video_path, db_for_split_silence_and_voice=db_for_split_silence_and_voice,
+                minimum_interval_time_in_seconds=minimum_interval)
 
             done()
         else:
             print()
             print("you may want to change the db, and try again.")
             exit()
 
@@ -639,19 +824,19 @@
         source_video_path = try_to_get_absolutely_path(source_video_path)
         target_video_path = try_to_get_absolutely_path(target_video_path)
         make_sure_source_is_absolute_path(source_video_path)
         make_sure_target_is_absolute_path(target_video_path)
         make_sure_target_does_not_exist(target_video_path)
 
         speed = float(speed)
-        video_speed = str(float(1/speed))[:6]
+        video_speed = str(float(1 / speed))[:6]
 
         if speed <= 4:
-            parts = math.ceil(speed/2)
-            value_of_each_part = str(speed ** (1/parts))[:6]
+            parts = math.ceil(speed / 2)
+            value_of_each_part = str(speed ** (1 / parts))[:6]
             audio_speed = ",".join(
                 [f"atempo={value_of_each_part}" for i in range(parts)])
 
             t.run(f"""
                 ffmpeg -i "{source_video_path}" -filter_complex "[0:v]setpts={video_speed}*PTS[v];[0:a]{audio_speed}[a]" -map "[v]" -map "[a]" "{target_video_path}"
             """)
 
@@ -665,19 +850,23 @@
         target_video_path = try_to_get_absolutely_path(target_video_path)
         make_sure_source_is_absolute_path(source_video_path)
         make_sure_target_is_absolute_path(target_video_path)
         make_sure_target_does_not_exist(target_video_path)
 
         clip = VideoFileClip(source_video_path).without_audio().fx(
             vfx.speedx, speed)
-        clip.write_videofile(target_video_path, threads=self._cpu_core_numbers)
+
+        clip = videoUtils.fix_rotation(clip)
+        clip.write_videofile(
+            target_video_path, threads=self._cpu_core_numbers, audio_codec="aac", verbose=False)
 
         done()
 
-    def speedup_silence_parts_in_video(self, source_video_path, target_video_path, db_for_split_silence_and_voice, speed=4):
+    def speedup_silence_parts_in_video(self, source_video_path, target_video_path, db_for_split_silence_and_voice,
+                                       speed=4):
         """
         Instead remove silence, we can speed up the silence parts in a video
 
         Parameters
         ----------
         source_video_path: string
         target_video_path: string
@@ -691,46 +880,48 @@
         make_sure_source_is_absolute_path(source_video_path)
         make_sure_source_is_absolute_path(target_video_path)
 
         top_db = db_for_split_silence_and_voice
 
         working_dir = get_directory_name(target_video_path)
         audio_path = convert_video_to_wav(source_video_path, add_path(
-            working_dir, disk.get_hash_of_a_path(source_video_path)+'audio_for_speedup_silence_parts_in_video.wav'))
+            working_dir, disk.get_hash_of_a_path(source_video_path) + 'audio_for_speedup_silence_parts_in_video.wav'))
 
         voice_and_silence_parts = self._get_voice_and_silence_parts(
             audio_path, top_db)
 
         make_sure_target_does_not_exist(audio_path)
         parent_clip = VideoFileClip(source_video_path)
+        parent_clip = videoUtils.fix_rotation(parent_clip)
         clip_list = []
         length = len(voice_and_silence_parts)
         for index, part in enumerate(voice_and_silence_parts):
             if len(part[1][0].split(".")) < 2:
                 part[1][0] += ".000000"
             try:
                 time_duration = (datetime.datetime.strptime(
                     part[1][1], '%H:%M:%S.%f') - datetime.datetime.strptime(part[1][0], '%H:%M:%S.%f')).seconds
-                print(str(int(index/length*100))+"%,", "-".join([p.split(".")[
-                      0] for p in part[1]]) + ",", "cut " + str(time_duration) + " seconds")
+                print(str(int(index / length * 100)) + "%,", "-".join([p.split(".")[
+                    0] for p in part[1]]) + ",",
+                    "cut " + str(time_duration) + " seconds")
             except Exception as e:
                 print(e)
             if part[0] == 1:  # voice
                 clip_list.append(parent_clip.subclip(part[1][0], part[1][1]))
             else:  # silence
                 clip_list.append(
                     parent_clip.subclip(part[1][0], part[1][1]).without_audio().fx(
                         vfx.speedx, speed
                     )
                 )
 
         concat_clip = concatenate_videoclips(clip_list)
 
         concat_clip.write_videofile(
-            target_video_path, threads=self._cpu_core_numbers)
+            target_video_path, threads=self._cpu_core_numbers, audio_codec="aac", verbose=False)
         concat_clip.close()
         del concat_clip
 
         done()
 
     def replace_video_with_a_picture(self, source_video_path, target_video_path, picture):
         """
@@ -758,17 +949,14 @@
     def get_mp3_from_video(self, source_video_path, target_video_path):
         source_video_path = try_to_get_absolutely_path(source_video_path)
         target_video_path = try_to_get_absolutely_path(target_video_path)
         make_sure_source_is_absolute_path(source_video_path)
         make_sure_target_is_absolute_path(target_video_path)
         make_sure_target_does_not_exist(target_video_path)
 
-        delay = float(delay)
-        delay = str(delay)
-
         t.run(f"""
             ffmpeg -i "{source_video_path}" "{source_video_path}"
         """)
 
         done()
 
     def delay_audio_in_video(self, source_video_path, target_video_path, delay):
@@ -807,55 +995,103 @@
 
         t.run(f"""
             ffmpeg -i "{source_video_path}" -vcodec copy -af "volume={times}dB" "{target_video_path}"
         """)
 
         done()
 
-    def compress_videos_in_a_folder(self, source_folder, fps: int = 29, resolution: Tuple[int, int] = None, preset: str = 'placebo'):
+    def fix_corrupt_videos_in_a_folder(self, source_folder: str):
         source_folder = try_to_get_absolutely_path(source_folder)
         make_sure_source_is_absolute_path(source_folder)
 
+        if not os.path.isdir(source_folder):
+            raise Exception("it needs to be a folder")
+
         working_dir = get_directory_name(source_folder)
-        new_folder = add_path(working_dir, 'compressed_' +
+        new_folder = add_path(working_dir, 'fixed_' +
                               os.path.basename(source_folder))
         if not os.path.exists(new_folder):
-            os.mkdir(new_folder)
+            os.makedirs(new_folder, exist_ok=True)
 
-        filelist = [os.path.join(source_folder, f) for f in os.listdir(
-            source_folder) if f.endswith(".mp4")]
+        filelist = disk.get_files(source_folder, type_limiter=[
+                                  ".mp4", ".mkv", ".avi", ".rmvb", ".ts"])
 
-        def convert_bytes(num):
-            """
-            this function will convert bytes to MB.... GB... etc
-            """
-            for x in ['bytes', 'KB', 'MB', 'GB', 'TB']:
-                if num < 1024.0:
-                    return (int(float(f'{num:.1f}')), f'{x}')
-                num /= 1024.0
+        for file in filelist:
+            target_video_path = file.replace(source_folder, new_folder)
+            target_dir = get_directory_name(target_video_path)
+            if not os.path.exists(target_dir):
+                os.makedirs(target_dir, exist_ok=True)
 
-            return (0, 0)
+            if not os.path.exists(target_video_path):
+                try:
+                    t.run(f"""
+                        ffmpeg -i "{file}" -c copy {target_video_path}
+                    """)
+                except KeyboardInterrupt:
+                    t.kill("ffmpeg")
+                    t.run(f'rm "{target_video_path}"')
+                    exit()
 
-        for file in filelist:
-            basename = os.path.basename(file)
-            target_video_path = add_path(new_folder, basename)
-            make_sure_target_does_not_exist(target_video_path)
+        done()
 
-            #size, unit = convert_bytes(os.path.getsize(file))
-            # if unit == "GB":
-            #    if size > 2:
-            if fps and resolution and preset:
-                t.run(f"""
-                    ffmpeg -i "{file}" -c copy -c:v libx264 -vf scale={resolution[0]}:{resolution[1]} -r {fps} -preset {preset} "{target_video_path}"
-                """)
-            else:
-                t.run(f"""
-                    ffmpeg -i "{file}" -c copy -c:v libx264 -vf scale=-2:720 "{target_video_path}"
-                """)
+    def compress_videos_in_a_folder(self, source_folder, fps: int = 29, resolution: Tuple[int, int] = None,
+                                    preset: str = 'veryslow'):
+        """
+        Parameters
+        ----------
+        source_video_path: string
+        preset: string
+            A preset is a collection of options that will provide a certain encoding speed to compression ratio. A slower preset will provide better compression
+                ultrafast
+                superfast
+                veryfast
+                faster
+                fast
+                medium – default preset
+                slow
+                slower
+                veryslow
+                placebo – ignore this as it is not useful (see FAQ)
+        """
+        source_folder = try_to_get_absolutely_path(source_folder)
+        make_sure_source_is_absolute_path(source_folder)
+
+        if not os.path.isdir(source_folder):
+            raise Exception("it needs to be a folder")
 
+        working_dir = get_directory_name(source_folder)
+        new_folder = add_path(working_dir, 'compressed_' +
+                              os.path.basename(source_folder))
+        if not os.path.exists(new_folder):
+            os.makedirs(new_folder, exist_ok=True)
+
+        filelist = disk.get_files(source_folder, type_limiter=[
+                                  ".mp4", ".mkv", ".avi", ".rmvb", ".ts"])
+
+        for file in filelist:
+            target_video_path = file.replace(source_folder, new_folder)
+            target_dir = get_directory_name(target_video_path)
+            if not os.path.exists(target_dir):
+                os.makedirs(target_dir, exist_ok=True)
+
+            # make_sure_target_does_not_exist(target_video_path)
+            if not os.path.exists(target_video_path):
+                try:
+                    if resolution:
+                        t.run(f"""
+                            ffmpeg -i "{file}" -c copy -c:v libx264 -vf scale={resolution[0]}:{resolution[1]} -r {fps} -preset {preset} "{target_video_path}"
+                        """)
+                    else:
+                        t.run(f"""
+                            ffmpeg -i "{file}" -c copy -c:v libx264 -vf scale=-2:720 -r {fps} -preset {preset} "{target_video_path}"
+                        """)
+                except KeyboardInterrupt:
+                    t.kill("ffmpeg")
+                    t.run(f'rm "{target_video_path}"')
+                    exit()
         done()
 
     def format_videos_in_a_folder(self, source_folder):
         source_folder = try_to_get_absolutely_path(source_folder)
         make_sure_source_is_absolute_path(source_folder)
 
         working_dir = get_directory_name(source_folder)
@@ -874,24 +1110,127 @@
 
             t.run(f"""
                 ffmpeg -i "{file}" -c:v libx264 -pix_fmt yuv420p -vf scale=1920:1080 "{target_video_path}"
             """)
 
         done()
 
+    def removeTopAndBottomOfAVideo(self, source_video_path: str, target_video_path: str, cropRatio: int = 0.12):
+        make_sure_target_does_not_exist(target_video_path)
+
+        clip = VideoFileClip(source_video_path)
+        clip = videoUtils.fix_rotation(clip)
+        width = clip.w
+        height = clip.h
+        cropRatio = 0.12
+        cropPixels = int(cropRatio * height)
+        clip = clip.crop(x1=0, y1=cropPixels, x2=width, y2=height - cropPixels)
+        clip.write_videofile(
+            target_video_path, threads=self._cpu_core_numbers, audio_codec="aac", verbose=False)
+
+        done()
+
+    def splitVideoToParts(self, source_video_path: str, target_video_folder: str, numOfParts: int):
+        if not disk.exists(target_video_folder):
+            os.mkdir(target_video_folder)
+
+        clip = VideoFileClip(source_video_path)
+        clip = videoUtils.fix_rotation(clip)
+        length = clip.duration
+        partLength = length / numOfParts
+
+        clips = []
+        for i in range(numOfParts):
+            clips.append(clip.subclip(i * partLength, (i + 1) * partLength))
+
+        for i, c in enumerate(clips):
+            c.write_videofile(
+                f"{target_video_folder}/{i}.mp4", threads=self._cpu_core_numbers, audio_codec="aac", verbose=False)
+
+        done()
+
+    def addMusicFilesToVideoFile(self, source_file_path: str, target_file_path: str, musicFiles: List[str], preDecreaseDBValueForTheMusic: int = 0, howManyDBYouWannaTheMusicToDecreaseWhenYouSpeak: int = 15):
+        make_sure_target_does_not_exist(target_file_path)
+
+        if not disk.exists(source_file_path):
+            print("source video does not exist")
+            return
+
+        if not source_file_path.endswith(".mp4"):
+            print("source video must be a mp4 file")
+            return
+
+        if any([disk.exists(file) == False for file in musicFiles]):
+            print("one of the music files does not exist")
+            return
+
+        if len(musicFiles) == 0:
+            print("no music file gets provided")
+            return
+
+        # handle input voice
+        humanVoice = audioProcessor.pydub.AudioSegment.from_file(
+            source_file_path, format="mp4")
+
+        # handle input music
+        musicSound = audioProcessor.pydub.AudioSegment.from_file(
+            musicFiles[0], format="mp3")
+        for musicFile in musicFiles[1:]:
+            musicSound += audioProcessor.pydub.AudioSegment.from_file(
+                musicFile, format="mp3")
+
+        while len(musicSound) < len(humanVoice):
+            musicSound *= 2
+
+        musicSound = musicSound[:len(humanVoice)]
+        musicSound -= preDecreaseDBValueForTheMusic
+
+        # handle the silence
+        musicSlices = []
+
+        infoOfTheVoice = audioProcessor.getCompleteTimeRangeForNoSilenceAndSilenceAudioSlice(
+            humanVoice)
+
+        for a, b, c in infoOfTheVoice:
+            music_part = musicSound[a:b]
+            if c == 1:
+                music_part -= howManyDBYouWannaTheMusicToDecreaseWhenYouSpeak
+            musicSlices.append(music_part)
+
+        processedMusic = musicSlices[0]
+        for part in musicSlices[1:]:
+            processedMusic += part
+
+        # remix
+        finalSound = humanVoice.overlay(processedMusic)
+        tempMp3FilePath = disk.getATempFilePath(source_file_path)
+        finalSound.export(tempMp3FilePath, format="mp3")
+
+        # add all those sound to a video file
+        videoclip = VideoFileClip(source_file_path)
+        audioclip = AudioFileClip(tempMp3FilePath)
+
+        videoclip.audio = audioclip
+        videoclip.write_videofile(
+            target_file_path, threads=self._cpu_core_numbers, verbose=False)
+
+        done()
+
 
 class DeepVideo():
     """
     For this one, I'll use deep learning.
 
     It's based on:
     1. ubuntu core
     2. vosk
     3. ffmpeg
     4. moviepy
+    5. librosa
+    6. pornstar
     """
 
     def __init__(self):
         from pathlib import Path
 
         self._cpu_core_numbers = multiprocessing.cpu_count()
 
@@ -907,15 +1246,15 @@
                 "http://alphacephei.com/kaldi/models/vosk-model-small-en-us-0.3.zip", zip_file, "30MB")
             if success:
                 print("download successfully")
             else:
                 print("download error")
 
         # uncompress
-        self.vosk_model_folder = self.config_folder/Path("model")
+        self.vosk_model_folder = self.config_folder / Path("model")
         if not self.vosk_model_folder.exists():
             disk.uncompress(zip_file, self.vosk_model_folder)
 
     def __time_interval_filter(self, data, minimum_interval_time_in_seconds: float = 0.0, video_length: float = None):
         temp_data = []
         length = len(data)
         for index, item in enumerate(data):
@@ -923,28 +1262,28 @@
             end = item['end']
             start = start - minimum_interval_time_in_seconds
             end = end + minimum_interval_time_in_seconds
             if index == 0:
                 start = item['start'] - minimum_interval_time_in_seconds
                 if start < 0:
                     start = 0.0
-            if index == length-1:
+            if index == length - 1:
                 end = item['end']
             temp_data.append([start, end])
         parts = []
         index = 0
         length = len(temp_data)
         if length >= 2:
-            while index <= length-1:
+            while index <= length - 1:
                 first_start = temp_data[index][0]
                 first_end = temp_data[index][1]
                 if index == 0:
                     if first_start > 0:
                         parts.append([0.0, first_start, 'silence'])
-                if index == length-1:
+                if index == length - 1:
                     parts.append([first_start, first_end, 'voice'])
                     if video_length != None:
                         if first_end < video_length:
                             parts.append([first_end, video_length, 'silence'])
                     break
                 next_index = index + 1
                 second_start = temp_data[next_index][0]
@@ -957,15 +1296,58 @@
                     first_end = second_start
                     parts.append([first_start, first_end, 'voice'])
                 index += 1
             return parts
         else:
             return parts
 
-    def __get_data_from_video(self, path: str, minimum_interval_time_in_seconds: float = 0.0, video_length: float = None):
+    def __get_raw_data_from_video(self, path: str):
+        from vosk import Model, KaldiRecognizer, SetLogLevel
+
+        assert os.path.exists(
+            path), f"source video file {path} does not exist!"
+
+        SetLogLevel(0)
+        sample_rate = 16000
+        model = Model(self.vosk_model_folder.as_posix())
+        rec = KaldiRecognizer(model, sample_rate)
+
+        process = subprocess.Popen(['ffmpeg', '-loglevel', 'quiet', '-i',
+                                    path,
+                                    '-ar', str(sample_rate), '-ac', '1', '-f', 's16le', '-'],
+                                   stdout=subprocess.PIPE)
+
+        data_list = []
+        while True:
+            data = process.stdout.read(4000)
+            if len(data) == 0:
+                break
+            if rec.AcceptWaveform(data):
+                result = json.loads(rec.Result())
+                if len(result.keys()) >= 2:
+                    """
+                    {'result': 
+                        [
+                            {'conf': 0.875663, 'end': 4.35, 'start': 4.11, 'word': 'nice'}, 
+                            {'conf': 1.0, 'end': 5.13, 'start': 4.59, 'word': 'day'}
+                        ], 
+                     'text': 'nice day'}
+                    """
+                    start = result['result'][0]['start']
+                    end = result['result'][-1]['end']
+                    text = result['result']["text"]
+                    data_list.append(
+                        {"start": start, "end": end, "text": text})
+            else:
+                # print(rec.PartialResult())
+                pass
+        return data_list
+
+    def __get_data_from_video(self, path: str, minimum_interval_time_in_seconds: float = 0.0,
+                              video_length: float = None):
         from vosk import Model, KaldiRecognizer, SetLogLevel
 
         assert os.path.exists(
             path), f"source video file {path} does not exist!"
 
         SetLogLevel(0)
         sample_rate = 16000
@@ -990,15 +1372,17 @@
                     end = result['result'][-1]['end']
                     data_list.append({"start": start, "end": end})
             else:
                 # print(rec.PartialResult())
                 pass
         return self.__time_interval_filter(data_list, minimum_interval_time_in_seconds, video_length)
 
-    def remove_silence_parts_from_videos_in_a_folder(self, source_folder: str, target_video_path: str, minimum_interval_time_in_seconds: float = 1.0, fps: int = None, resolution: Tuple[int, int] = None, preset: str = 'placebo'):
+    def remove_silence_parts_from_videos_in_a_folder(self, source_folder: str, target_video_path: str,
+                                                     minimum_interval_time_in_seconds: float = 1.0, fps: int = None,
+                                                     resolution: Tuple[int, int] = None, preset: str = 'placebo'):
         """
         We will first concatenate the files under the source_folder into a video by created_time, then we remove those silence parts in that videoig
 
         Parameters
         ----------
         source_folder: string
         target_video_path: string
@@ -1013,36 +1397,40 @@
         make_sure_target_does_not_exist(target_video_path)
 
         video_files = [video for video in disk.get_files(
             source_folder, recursive=False)]
         video_files = disk.sort_files_by_time(video_files)
         if resolution != None:
             resolution = (resolution[1], resolution[0])
-        parent_clips = [VideoFileClip(
-            video, target_resolution=resolution) for video in video_files]
+
+        parent_clips = [videoUtils.fix_rotation(VideoFileClip(
+            video, target_resolution=resolution)) for video in video_files]
         length = len(video_files)
         remain_clips = []
         for index, video_file in enumerate(video_files):
-            print("Working on ", str(int(index/length*100)) + " %...")
+            print("Working on ", str(int(index / length * 100)) + " %...")
             parts = self.__get_data_from_video(
                 video_file, minimum_interval_time_in_seconds, parent_clips[index].duration)
             for part in parts:
                 if part[2] == 'voice':
                     remain_clips.append(
                         parent_clips[index].subclip(part[0], part[1]))
 
         concat_clip = concatenate_videoclips(remain_clips)
-        concat_clip.write_videofile(target_video_path, fps=fps, preset=preset)
+        concat_clip.write_videofile(
+            target_video_path, threads=self._cpu_core_numbers, fps=fps, preset=preset, audio_codec="aac", verbose=False)
         concat_clip.close()
         for parent_clip in parent_clips:
             parent_clip.close()
 
         done()
 
-    def speed_up_silence_parts_from_videos_in_a_folder(self, source_folder: str, target_video_path: str, speed: int = 4, minimum_interval_time_in_seconds: float = 1.0, fps: int = None, resolution: Tuple[int, int] = None, preset: str = 'placebo'):
+    def speed_up_silence_parts_from_videos_in_a_folder(self, source_folder: str, target_video_path: str, speed: int = 4,
+                                                       minimum_interval_time_in_seconds: float = 1.0, fps: int = None,
+                                                       resolution: Tuple[int, int] = None, preset: str = 'placebo'):
         """
         We will first concatenate the files under the source_folder into a video by created_time, then we speed up those silence parts in that videoig
 
         Parameters
         ----------
         source_folder: string
         target_video_path: string
@@ -1059,116 +1447,157 @@
         make_sure_target_does_not_exist(target_video_path)
 
         video_files = [video for video in disk.get_files(
             source_folder, recursive=False)]
         video_files = disk.sort_files_by_time(video_files)
         if resolution != None:
             resolution = (resolution[1], resolution[0])
-        parent_clips = [VideoFileClip(
-            video, target_resolution=resolution) for video in video_files]
+        parent_clips = [videoUtils.fix_rotation(VideoFileClip(
+            video, target_resolution=resolution)) for video in video_files]
         length = len(video_files)
         remain_clips = []
         for index, video_file in enumerate(video_files):
-            print("Working on ", str(int(index/length*100)) + " %...")
+            print("Working on ", str(int(index / length * 100)) + " %...")
             parts = self.__get_data_from_video(
                 video_file, minimum_interval_time_in_seconds, parent_clips[index].duration)
             for part in parts:
                 if part[2] == 'voice':
                     remain_clips.append(
                         parent_clips[index].subclip(part[0], part[1]))
                 elif part[2] == 'silence':
                     remain_clips.append(
                         parent_clips[index].subclip(part[0], part[1]).without_audio().fx(
                             vfx.speedx, speed
                         )
                     )
 
         concat_clip = concatenate_videoclips(remain_clips)
-        concat_clip.write_videofile(target_video_path, fps=fps, preset=preset)
+        concat_clip.write_videofile(
+            target_video_path, threads=self._cpu_core_numbers, fps=fps, preset=preset, audio_codec="aac", verbose=False)
         concat_clip.close()
         for parent_clip in parent_clips:
             parent_clip.close()
 
         done()
 
-    def remove_silence_parts_from_video(self, source_video_path: str, target_video_path: str, minimum_interval_time_in_seconds: float = 1.0):
+    def remove_silence_parts_from_video(self, source_video_path: str, target_video_path: str,
+                                        minimum_interval_time_in_seconds: float = 1.0):
         """
         Parameters
         ----------
         source_video_path: string
         target_video_path: string
         minimum_interval_time_in_seconds: float
             longer than this value, we will take it as silence and remove it
         """
         make_sure_target_does_not_exist(target_video_path)
 
         parent_clip = VideoFileClip(source_video_path)
+        parent_clip = videoUtils.fix_rotation(parent_clip)
         parts = self.__get_data_from_video(
             source_video_path, minimum_interval_time_in_seconds, parent_clip.duration)
         clip_list = []
         length = len(parts)
         for index, part in enumerate(parts):
             if part[2] == 'voice':
                 try:
                     time_duration = part[1] - part[0]
-                    print(str(int(index/length*100))+"%,", "remain " +
+                    print(str(int(index / length * 100)) + "%,", "remain " +
                           str(int(time_duration)) + " seconds")
                 except Exception as e:
                     print(e)
                 clip_list.append(parent_clip.subclip(part[0], part[1]))
 
         concat_clip = concatenate_videoclips(clip_list)
         concat_clip.write_videofile(
-            target_video_path, threads=self._cpu_core_numbers)
+            target_video_path, threads=self._cpu_core_numbers, audio_codec="aac", verbose=False)
         concat_clip.close()
         parent_clip.close()
 
         done()
 
-    def speedup_silence_parts_in_video(self, source_video_path: str, target_video_path: str, speed: int = 4, minimum_interval_time_in_seconds: float = 1.0, fps: int = None, resolution: Tuple[int, int] = None, preset: str = 'placebo'):
+    def speedup_silence_parts_in_video(self, source_video_path: str, target_video_path: str, speed: int = 4,
+                                       minimum_interval_time_in_seconds: float = 1.0, fps: int = None,
+                                       resolution: Tuple[int, int] = None, preset: str = 'placebo'):
         """
         Instead remove silence, we can speed up the silence parts in a video
 
         Parameters
         ----------
         source_video_path: string
         target_video_path: string
         speed: float
             how quick you want the silence parts to be
         """
         make_sure_target_does_not_exist(target_video_path)
 
         parent_clip = VideoFileClip(
             source_video_path, target_resolution=(resolution[1], resolution[0]))
+
+        parent_clip = videoUtils.fix_rotation(parent_clip)
         parts = self.__get_data_from_video(
             source_video_path, minimum_interval_time_in_seconds, parent_clip.duration)
         clip_list = []
         length = len(parts)
         for index, part in enumerate(parts):
             if part[2] == 'voice':
                 clip_list.append(parent_clip.subclip(part[0], part[1]))
             elif part[2] == 'silence':
                 try:
                     time_duration = part[1] - part[0]
-                    print(str(int(index/length*100))+"%,", "speed up " +
+                    print(str(int(index / length * 100)) + "%,", "speed up " +
                           str(int(time_duration)) + " seconds")
                 except Exception as e:
                     print(e)
                 clip_list.append(
                     parent_clip.subclip(part[0], part[1]).without_audio().fx(
                         vfx.speedx, speed
                     )
                 )
 
         concat_clip = concatenate_videoclips(clip_list)
         concat_clip.write_videofile(
-            target_video_path, threads=self._cpu_core_numbers, fps=fps, preset=preset)
+            target_video_path, threads=self._cpu_core_numbers, fps=fps, preset=preset, audio_codec="aac", verbose=False)
         concat_clip.close()
         parent_clip.close()
 
         done()
 
+    def _get_sounds_parts(self, source_audio_path, top_db):
+        y, sr = get_wav_infomation(source_audio_path)
+        parts = librosa.effects.split(y, top_db=top_db)  # return samples
+
+        def from_samples_to_seconds(parts):
+            parts = librosa.core.samples_to_time(parts, sr)  # return seconds
+            new_parts = []
+
+            for part in parts:
+                part1 = part[0]
+                part2 = part[1]
+                new_parts.append([part1, part2])
+
+            return new_parts
+
+        parts[0] = [0, parts[0][1]]
+        parts = from_samples_to_seconds(parts)
+
+        return parts[1:]
+
+    def blurPornGraphs(self, source_video_path: str, target_video_path: str):
+        # useless
+        import pornstar
+
+        def doit(frame):
+            if pornstar.store.nsfw_detector.isPorn(frame, 0.9):
+                classList, ScoreList, PositionList = pornstar.my_object_detector.detect(
+                    frame)
+                if "person" in classList:
+                    frame = pornstar.effect_of_blur(frame, kernel=30)
+            return frame
+
+        pornstar.process_video(path_of_video=source_video_path,
+                               effect_function=doit, save_to=target_video_path)
+
 
 if __name__ == "__main__":
-    video = DeepVideo()
-    video.speedup_silence_parts_in_video(
-        "/home/yingshaoxo/demo.mp4", "/home/yingshaoxo/ok.mp4", 10)
+    video = Video()
+    video.compress_videos_in_a_folder("/home/yingshaoxo/Videos/doing", fps=15)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `auto_everything-3.8/setup.py` & `auto_everything-3.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import Extension
 from setuptools.command.build_ext import build_ext
 
 from setuptools import setup, find_packages
 from os.path import dirname, join, abspath
 
-version = '3.8'
+version = '3.9'
 
 # main
 file_path = join(abspath(dirname(__file__)), "README.md")
 with open(file_path) as f:
     long_description = f.read()
 
 # Let's first try to install the normal version
@@ -30,14 +30,17 @@
       license='GPLv3',
       install_requires=[
           'setuptools',
           'fire',
           'psutil',
       ],
       extras_require={
-          "video":  ["numpy", "librosa", "moviepy>=1.0.0,<1.0.1", "pyaudio", "vosk"],
+          "database": ["pymongo"],
+          "video":  ["numpy", "librosa", "moviepy", "pyaudio", "vosk"],
           "gui": ["numpy", "opencv-python", "pyscreenshot", "pytesseract", "pyautogui"],
           "fakecamera": ["pyfakewebcam", "opencv-python"],
+          "image":  ["pillow"],
+          "all": ["o365"]
       },
       include_package_data=False,
-      packages=find_packages(),
+      packages=["auto_everything"],
       )
```

