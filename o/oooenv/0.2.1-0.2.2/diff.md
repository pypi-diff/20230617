# Comparing `tmp/oooenv-0.2.1.tar.gz` & `tmp/oooenv-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oooenv-0.2.1.tar", max compression
+gzip compressed data, was "oooenv-0.2.2.tar", max compression
```

## Comparing `oooenv-0.2.1.tar` & `oooenv-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1073 2023-06-04 18:27:08.699098 oooenv-0.2.1/LICENSE
--rw-r--r--   0        0        0        0 2023-06-04 18:27:08.700098 oooenv-0.2.1/oooenv/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 18:27:08.701098 oooenv-0.2.1/oooenv/cli/__init__.py
--rw-r--r--   0        0        0     8066 2023-06-12 21:27:05.393663 oooenv-0.2.1/oooenv/cli/main.py
--rw-r--r--   0        0        0        0 2023-06-04 18:27:08.702098 oooenv-0.2.1/oooenv/cmds/__init__.py
--rw-r--r--   0        0        0      174 2023-06-04 18:27:08.703098 oooenv-0.2.1/oooenv/cmds/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5103 2023-06-04 18:27:08.703098 oooenv-0.2.1/oooenv/cmds/__pycache__/manage_env_cfg.cpython-310.pyc
--rw-r--r--   0        0        0     2841 2023-06-04 18:27:08.704098 oooenv-0.2.1/oooenv/cmds/__pycache__/uno_lnk.cpython-310.pyc
--rw-r--r--   0        0        0      909 2023-06-12 21:32:53.696519 oooenv-0.2.1/oooenv/cmds/install.py
--rw-r--r--   0        0        0     5767 2023-06-04 22:49:18.217130 oooenv-0.2.1/oooenv/cmds/manage_env_cfg.py
--rw-r--r--   0        0        0     4627 2023-06-04 22:49:18.219134 oooenv-0.2.1/oooenv/cmds/uno_lnk.py
--rw-r--r--   0        0        0     1216 2023-06-04 22:49:18.220132 oooenv-0.2.1/oooenv/cmds/updater.py
--rw-r--r--   0        0        0        0 2023-06-04 18:27:08.705098 oooenv-0.2.1/oooenv/utils/__init__.py
--rw-r--r--   0        0        0      175 2023-06-04 18:27:08.705098 oooenv-0.2.1/oooenv/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3710 2023-06-04 18:27:08.706099 oooenv-0.2.1/oooenv/utils/__pycache__/local_paths.cpython-310.pyc
--rw-r--r--   0        0        0     1146 2023-06-04 18:27:08.706099 oooenv-0.2.1/oooenv/utils/__pycache__/sys_info.cpython-310.pyc
--rw-r--r--   0        0        0     5887 2023-06-04 18:27:08.707099 oooenv-0.2.1/oooenv/utils/__pycache__/uno_paths.cpython-310.pyc
--rw-r--r--   0        0        0     3708 2023-06-04 18:27:08.707099 oooenv-0.2.1/oooenv/utils/__pycache__/util.cpython-310.pyc
--rw-r--r--   0        0        0     3169 2023-06-12 21:31:08.327054 oooenv-0.2.1/oooenv/utils/local_paths.py
--rw-r--r--   0        0        0      773 2023-06-04 22:49:18.223133 oooenv-0.2.1/oooenv/utils/sys_info.py
--rw-r--r--   0        0        0     8556 2023-06-04 22:49:18.224131 oooenv-0.2.1/oooenv/utils/uno_paths.py
--rw-r--r--   0        0        0     1419 2023-06-12 20:44:28.886808 oooenv-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1804 2023-06-12 21:44:02.586192 oooenv-0.2.1/README.md
--rw-r--r--   0        0        0     2863 1970-01-01 00:00:00.000000 oooenv-0.2.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1073 2023-03-29 17:32:33.108507 oooenv-0.2.2/LICENSE
+-rwxr-xr-x   0        0        0     2681 2023-06-17 19:01:17.362300 oooenv-0.2.2/README.md
+-rwxr-xr-x   0        0        0        0 2023-03-29 14:28:44.487665 oooenv-0.2.2/oooenv/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-03-29 17:14:51.509563 oooenv-0.2.2/oooenv/cli/__init__.py
+-rwxr-xr-x   0        0        0     8066 2023-06-17 17:49:31.367107 oooenv-0.2.2/oooenv/cli/main.py
+-rwxr-xr-x   0        0        0        0 2023-03-29 14:36:41.949832 oooenv-0.2.2/oooenv/cmds/__init__.py
+-rwxr-xr-x   0        0        0      174 2023-03-29 15:00:18.797439 oooenv-0.2.2/oooenv/cmds/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     5103 2023-03-29 17:06:15.560117 oooenv-0.2.2/oooenv/cmds/__pycache__/manage_env_cfg.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2841 2023-03-29 15:00:18.802246 oooenv-0.2.2/oooenv/cmds/__pycache__/uno_lnk.cpython-310.pyc
+-rwxr-xr-x   0        0        0      883 2023-06-17 17:49:31.368191 oooenv-0.2.2/oooenv/cmds/install.py
+-rwxr-xr-x   0        0        0     5767 2023-06-17 17:49:31.369339 oooenv-0.2.2/oooenv/cmds/manage_env_cfg.py
+-rwxr-xr-x   0        0        0     4627 2023-06-17 17:49:31.370392 oooenv-0.2.2/oooenv/cmds/uno_lnk.py
+-rwxr-xr-x   0        0        0     1216 2023-06-17 17:49:31.371160 oooenv-0.2.2/oooenv/cmds/updater.py
+-rwxr-xr-x   0        0        0        0 2023-03-29 14:34:49.616759 oooenv-0.2.2/oooenv/utils/__init__.py
+-rwxr-xr-x   0        0        0      175 2023-03-29 15:00:18.812804 oooenv-0.2.2/oooenv/utils/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3710 2023-03-29 15:00:18.815799 oooenv-0.2.2/oooenv/utils/__pycache__/local_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1146 2023-03-29 15:00:18.820968 oooenv-0.2.2/oooenv/utils/__pycache__/sys_info.cpython-310.pyc
+-rwxr-xr-x   0        0        0     5887 2023-03-29 15:00:18.819281 oooenv-0.2.2/oooenv/utils/__pycache__/uno_paths.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3708 2023-03-29 14:34:49.621334 oooenv-0.2.2/oooenv/utils/__pycache__/util.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3573 2023-06-17 19:02:46.802447 oooenv-0.2.2/oooenv/utils/local_paths.py
+-rwxr-xr-x   0        0        0      773 2023-06-17 17:49:31.374581 oooenv-0.2.2/oooenv/utils/sys_info.py
+-rwxr-xr-x   0        0        0    10430 2023-06-17 19:02:37.679772 oooenv-0.2.2/oooenv/utils/uno_paths.py
+-rwxr-xr-x   0        0        0     1419 2023-06-17 17:50:51.464403 oooenv-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3740 1970-01-01 00:00:00.000000 oooenv-0.2.2/PKG-INFO
```

### Comparing `oooenv-0.2.1/LICENSE` & `oooenv-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.1/oooenv/cli/main.py` & `oooenv-0.2.2/oooenv/cli/main.py`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.1/oooenv/cmds/__pycache__/manage_env_cfg.cpython-310.pyc` & `oooenv-0.2.2/oooenv/cmds/__pycache__/manage_env_cfg.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.1/oooenv/cmds/__pycache__/uno_lnk.cpython-310.pyc` & `oooenv-0.2.2/oooenv/cmds/__pycache__/uno_lnk.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.1/oooenv/cmds/install.py` & `oooenv-0.2.2/oooenv/cmds/install.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from __future__ import annotations
-from pathlib import Path
-import os
-from ..utils import local_paths
-
-
-def pip_e() -> str:
-    """
-    Install root path in virtual environment site-packages directory.
-
-    Basically the same thing as ``pip -e .`` but without the need for pip.
-
-    Returns:
-        str: Message indicating success or failure. Empty string on failure.
-    """
-    try:
-        root_path = Path(local_paths.get_virtual_env_path()).parent
-        site_packages_dir = local_paths.get_site_packages_dir()
-        if site_packages_dir is None:
-            return ""
-        file_name = site_packages_dir / f"{root_path.name.replace('.', '_').replace(' ', '_')}.pth"
-        with open(file_name, "w") as f:
-            f.write(str(root_path))
-        return f"Created file: {file_name}"
-    except Exception as e:
-        return f"Failed to create file: {file_name}\n{e}"
+from __future__ import annotations
+from pathlib import Path
+import os
+from ..utils import local_paths
+
+
+def pip_e() -> str:
+    """
+    Install root path in virtual environment site-packages directory.
+
+    Basically the same thing as ``pip -e .`` but without the need for pip.
+
+    Returns:
+        str: Message indicating success or failure. Empty string on failure.
+    """
+    try:
+        root_path = Path(local_paths.get_virtual_env_path()).parent
+        site_packages_dir = local_paths.get_site_packages_dir()
+        if site_packages_dir is None:
+            return ""
+        file_name = site_packages_dir / f"{root_path.name.replace('.', '_').replace(' ', '_')}.pth"
+        with open(file_name, "w") as f:
+            f.write(str(root_path))
+        return f"Created file: {file_name}"
+    except Exception as e:
+        return f"Failed to create file: {file_name}\n{e}"
```

### Comparing `oooenv-0.2.1/oooenv/cmds/manage_env_cfg.py` & `oooenv-0.2.2/oooenv/cmds/manage_env_cfg.py`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.1/oooenv/cmds/uno_lnk.py` & `oooenv-0.2.2/oooenv/cmds/uno_lnk.py`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.1/oooenv/cmds/updater.py` & `oooenv-0.2.2/oooenv/cmds/updater.py`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.1/oooenv/utils/__pycache__/local_paths.cpython-310.pyc` & `oooenv-0.2.2/oooenv/utils/__pycache__/local_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.1/oooenv/utils/__pycache__/sys_info.cpython-310.pyc` & `oooenv-0.2.2/oooenv/utils/__pycache__/sys_info.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.1/oooenv/utils/__pycache__/uno_paths.cpython-310.pyc` & `oooenv-0.2.2/oooenv/utils/__pycache__/uno_paths.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.1/oooenv/utils/__pycache__/util.cpython-310.pyc` & `oooenv-0.2.2/oooenv/utils/__pycache__/util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.1/oooenv/utils/local_paths.py` & `oooenv-0.2.2/oooenv/utils/local_paths.py`

 * *Files 18% similar despite different names*

```diff
@@ -98,26 +98,35 @@
     Gets the Virtual Environment Path
 
     Returns:
         str: Virtual Environment Path
 
     Note:
         If unable to get virtual path from Environment then ``sys.base_exec_prefix`` is returned.
+
+        If ``OOOENV_VIRTUAL_ENV`` environment variable is set in environment then that path is returned.
     """
+    if ooo_env := os.environ.get("OOOENV_VIRTUAL_ENV", None):
+        return ooo_env
     s_path = os.environ.get("VIRTUAL_ENV", None)
     return s_path if s_path is not None else sys.base_exec_prefix
 
 
 def get_site_packages_dir() -> Union[Path, None]:
     """
     Gets the ``site-packages`` directory for current python environment.
 
     Returns:
         Union[Path, None]: site-packages dir if found; Otherwise, None.
+
+    Note:
+        If ``OOOENV_SITE_PACKAGES`` environment variable is set in environment then that path is returned.
     """
+    if site_dir := os.environ.get("OOOENV_SITE_PACKAGES", None):
+        return Path(site_dir)
     v_path = get_virtual_env_path()
     p_site = Path(v_path, "Lib", "site-packages")
     if p_site.exists() and p_site.is_dir():
         return p_site
 
     ver = f"{sys.version_info[0]}.{sys.version_info[1]}"
     p_site = Path(v_path, "lib", f"python{ver}", "site-packages")
```

### Comparing `oooenv-0.2.1/oooenv/utils/sys_info.py` & `oooenv-0.2.2/oooenv/utils/sys_info.py`

 * *Files identical despite different names*

### Comparing `oooenv-0.2.1/oooenv/utils/uno_paths.py` & `oooenv-0.2.2/oooenv/utils/uno_paths.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,30 +29,37 @@
     Gets the Soffice install path.
 
     For windows this will be something like: ``C:\\Program Files\\LibreOffice``.
     For Linux this will be something like: ``/usr/lib/libreoffice``
 
     Returns:
         Path: install as Path.
+
+    Note:
+        If `OOOENV_LO_PROGRAM_PATH` is set in the environment, then that path is returned.
     """
     # sourcery skip: assign-if-exp, extract-duplicate-method, extract-method, hoist-statement-from-if, inline-immediately-returned-variable, low-code-quality
     global _INSTALL_PATH
+    if install_pth := os.environ.get("OOOENV_LO_PROGRAM_PATH", ""):
+        # supersede all other methods
+        return Path(install_pth)
+
     if _INSTALL_PATH is not None:
         return _INSTALL_PATH
     if PLATFORM == SysInfo.PlatformEnum.WINDOWS:
         # get the path location from Registry
         value = ""
         for _key in (
             # LibreOffice 3.4.5,6,7 on Windows
             "SOFTWARE\\LibreOffice\\UNO\\InstallPath",
             # OpenOffice 3.3
             "SOFTWARE\\OpenOffice.org\\UNO\\InstallPath",
         ):
             try:
-                value = winreg.QueryValue(winreg.HKEY_LOCAL_MACHINE, _key)
+                value = winreg.QueryValue(winreg.HKEY_LOCAL_MACHINE, _key)  # type: ignore
             except Exception as detail:
                 value = ""
                 # _errMess = "%s" % detail
             else:
                 break  # first existing key will do
         if value != "":
             _INSTALL_PATH = Path("\\".join(value.split("\\")[:-1]))  # drop the program
@@ -116,49 +123,78 @@
         Path: path to soffice
     """
     if PLATFORM == SysInfo.PlatformEnum.WINDOWS:
         return Path(get_lo_path(), "soffice.exe")
     return Path(get_lo_path(), "soffice")
 
 
+def _get_soffice_which_path() -> Path | None:
+    """
+    Gets the path to soffice using shutil.which
+
+    Usually something like ``/usr/lib/libreoffice/program/soffice``
+    """
+    if link_path := shutil.which("soffice"):
+        relative_path = os.path.realpath(link_path)
+        if os.path.isabs(relative_path):
+            return Path(relative_path)
+        else:
+            return Path(os.path.abspath(relative_path))
+    return None
+
+
 def get_uno_path() -> Path:
     """
     Searches known paths for path that contains uno.py
 
     This path is different for windows and linux.
     Typically for Windows ``C:\\Program Files\\LibreOffice\\program``
     Typically for Linux ``/usr/lib/python3/dist-packages``
 
     Raises:
         FileNotFoundError: if path is not found
         NotADirectoryError: if path is not a directory
 
     Returns:
         Path: First found path.
+
+    Note:
+        If `OOOENV_LO_UNO_PATH` is set, it will be returned without any checks.
     """
-    # sourcery skip: extract-duplicate-method
-    if PLATFORM == SysInfo.PlatformEnum.WINDOWS:
+    if env_path := os.environ.get("OOOENV_LO_UNO_PATH", ""):
+        # special environment variable, no arguments just return it
+        return Path(env_path)
 
+    if PLATFORM == SysInfo.PlatformEnum.WINDOWS:
         p_uno = Path(os.environ["PROGRAMFILES"], "LibreOffice", "program")
         if not p_uno.exists() or not p_uno.is_dir():
             p_uno = Path(os.environ["PROGRAMFILES(X86)"], "LibreOffice", "program")
         if not p_uno.exists():
             raise FileNotFoundError("Uno Source Dir not found.")
         if not p_uno.is_dir():
             raise NotADirectoryError("UNO source is not a Directory")
         return p_uno
     elif PLATFORM == SysInfo.PlatformEnum.MAC:
         return Path("/Applications/LibreOffice.app/Contents/MacOS/soffice")
     else:
-        p_uno = Path("/usr/lib/python3/dist-packages")
-        if not p_uno.exists():
-            raise FileNotFoundError("Uno Source Dir not found.")
-        if not p_uno.is_dir():
-            raise NotADirectoryError("UNO source is not a Directory")
-        return p_uno
+        check_paths = ("/usr/lib/python3/dist-packages", "/usr/lib/libreoffice/program", "/opt/libreoffice/program")
+        p_uno = None
+        for pth in check_paths:
+            p_uno = Path(pth)
+            if p_uno.exists() and p_uno.is_dir() and (p_uno / "uno.py").exists():
+                return p_uno
+        # not found yet.
+        # try using shutil.which to extract the path from the link.
+        if which_path := _get_soffice_which_path():
+            # '/usr/lib/libreoffice/program/soffice'
+            p_uno = which_path.parent
+            if p_uno.exists() and p_uno.is_dir() and (p_uno / "uno.py").exists():
+                return p_uno
+
+    raise FileNotFoundError("Uno Source Dir not found.")
 
 
 def get_lo_path() -> Path:
     """
     Searches known paths for path that contains LibreOffice ``soffice``.
 
     This path is different for windows and linux.
@@ -167,15 +203,23 @@
 
     Raises:
         FileNotFoundError: if path is not found
         NotADirectoryError: if path is not a directory
 
     Returns:
         Path: First found path.
+
+    Note:
+        If `OOOENV_LO_PROGRAM_PATH` is set, it will be returned without any checks.
     """
+    # sourcery skip: assign-if-exp, extract-method, introduce-default-else
+    if lo_path := os.environ.get("OOOENV_LO_PROGRAM_PATH", ""):
+        # special environment variable, no arguments just return it
+        return Path(lo_path)
+
     if PLATFORM == SysInfo.PlatformEnum.WINDOWS:
         return Path(get_soffice_install_path(), "program")
 
     elif PLATFORM == SysInfo.PlatformEnum.MAC:
         return Path("/Applications/LibreOffice.app/Contents/MacOS")
     else:
         # search system path
@@ -214,15 +258,20 @@
 
     Raises:
         FileNotFoundError: In Windows if ``python.exe`` is not found.
         NotADirectoryError: In Windows if ``python.exe`` is not a file.
 
     Returns:
         str: file location of python executable.
+
+    Note:
+        If `OOOENV_LO_PY_EXE` environment variable is set, it will be returned without any checks.
     """
+    if env_path := os.environ.get("OOOENV_LO_PY_EXE", ""):
+        return env_path
     if PLATFORM != SysInfo.PlatformEnum.WINDOWS:
         return sys.executable
     p = Path(get_lo_path(), "python.exe")
 
     if not p.exists():
         raise FileNotFoundError("LibreOffice python executable not found.")
     if not p.is_file():
```

### Comparing `oooenv-0.2.1/pyproject.toml` & `oooenv-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oooenv"
-version = "0.2.1"
+version = "0.2.2"
 description = "Configures a project python environment for LibreOffice UNO."
 authors = [":Barry-Thomas-Paul: Moss <vibrationoflife@protonmail.com>"]
 keywords = ["libreoffice", "macro", "uno", "ooouno", "venv"]
 homepage = "https://github.com/Amourspirit/python_oooenv"
 documentation = "https://github.com/Amourspirit/python_oooenv"
 repository = "https://github.com/Amourspirit/python_oooenv"
 license = "MIT"
@@ -35,15 +35,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.3.0"
-pytest = ">=7.3.1"
+pytest = ">=7.3.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 extended-select=["ANN", "C4", "N", "SIM", "TCH"]
```

### Comparing `oooenv-0.2.1/PKG-INFO` & `oooenv-0.2.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oooenv
-Version: 0.2.1
+Version: 0.2.2
 Summary: Configures a project python environment for LibreOffice UNO.
 Home-page: https://github.com/Amourspirit/python_oooenv
 License: MIT
 Keywords: libreoffice,macro,uno,ooouno,venv
 Author: :Barry-Thomas-Paul: Moss
 Author-email: vibrationoflife@protonmail.com
 Requires-Python: >=3.8,<4.0
@@ -88,7 +88,19 @@
 oooenv update --update
 ```
 
 If virtual environment is managed by Poetry then it will be necessary to toggle into original config before running `poetry update`.
 
 When updates are done just run command again to toggle back to UNO environment configuration.
 
+## Environment Variables
+
+Special environment variables can be set. These are completely optional.
+This can be useful for docker containers.
+
+- `OOOENV_LO_UNO_PATH` The path where `uno.py` is located.
+- `OOOENV_LO_PROGRAM_PATH` The path to LibreOffice such as `C:\Program Files\LibreOffice\program` or `/usr/lib/libreoffice/program`.
+- `OOOENV_LO_PROGRAM_PATH` The path to LibreOffice installed directory, such as `C:\Program Files\LibreOffice` or `/usr/lib/libreoffice`.
+- `OOOENV_LO_PY_EXE` The path to LibreOffice Python. On Windows this is usually `C:\Program Files\LibreOffice\program\python.exe` and Linux is usually the virtual environment's python.
+- `OOOENV_VIRTUAL_ENV` The path containing the virtual environment for your project. Usually this is `venv` or `.venv`.`
+- `OOOENV_SITE_PACKAGES` The site packages directory of the virtual environment for your project.
+
```

