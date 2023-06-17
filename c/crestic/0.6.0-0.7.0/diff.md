# Comparing `tmp/crestic-0.6.0.tar.gz` & `tmp/crestic-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crestic-0.6.0.tar", last modified: Sun Sep  5 06:05:34 2021, max compression
+gzip compressed data, was "crestic-0.7.0.tar", last modified: Sat Jun 17 10:48:34 2023, max compression
```

## Comparing `crestic-0.6.0.tar` & `crestic-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 nils      (1000) nils      (1000)        0 2021-09-05 06:05:34.556699 crestic-0.6.0/
--rw-r--r--   0 nils      (1000) nils      (1000)     1051 2019-12-18 14:32:50.000000 crestic-0.6.0/LICENSE
--rw-r--r--   0 nils      (1000) nils      (1000)    11867 2021-09-05 06:05:34.556699 crestic-0.6.0/PKG-INFO
--rw-r--r--   0 nils      (1000) nils      (1000)     8087 2021-09-05 05:59:53.000000 crestic-0.6.0/README.md
-drwxr-xr-x   0 nils      (1000) nils      (1000)        0 2021-09-05 06:05:34.556699 crestic-0.6.0/crestic.egg-info/
--rw-r--r--   0 nils      (1000) nils      (1000)    11867 2021-09-05 06:05:34.000000 crestic-0.6.0/crestic.egg-info/PKG-INFO
--rw-r--r--   0 nils      (1000) nils      (1000)      250 2021-09-05 06:05:34.000000 crestic-0.6.0/crestic.egg-info/SOURCES.txt
--rw-r--r--   0 nils      (1000) nils      (1000)        1 2021-09-05 06:05:34.000000 crestic-0.6.0/crestic.egg-info/dependency_links.txt
--rw-r--r--   0 nils      (1000) nils      (1000)       41 2021-09-05 06:05:34.000000 crestic-0.6.0/crestic.egg-info/entry_points.txt
--rw-r--r--   0 nils      (1000) nils      (1000)       85 2021-09-05 06:05:34.000000 crestic-0.6.0/crestic.egg-info/requires.txt
--rw-r--r--   0 nils      (1000) nils      (1000)        8 2021-09-05 06:05:34.000000 crestic-0.6.0/crestic.egg-info/top_level.txt
--rwxr-xr-x   0 nils      (1000) nils      (1000)     6200 2021-09-05 05:59:53.000000 crestic-0.6.0/crestic.py
--rw-r--r--   0 nils      (1000) nils      (1000)      107 2020-05-25 07:41:55.000000 crestic-0.6.0/pyproject.toml
--rw-r--r--   0 nils      (1000) nils      (1000)     1512 2021-09-05 06:05:34.560032 crestic-0.6.0/setup.cfg
--rw-r--r--   0 nils      (1000) nils      (1000)       38 2020-05-25 07:41:55.000000 crestic-0.6.0/setup.py
+drwxr-xr-x   0 nils      (1000) nils      (1000)        0 2023-06-17 10:48:34.169087 crestic-0.7.0/
+-rw-r--r--   0 nils      (1000) nils      (1000)     1051 2019-12-17 10:20:16.000000 crestic-0.7.0/LICENSE
+-rw-r--r--   0 nils      (1000) nils      (1000)     2364 2023-06-17 10:48:34.169087 crestic-0.7.0/PKG-INFO
+-rw-r--r--   0 nils      (1000) nils      (1000)     1050 2023-06-17 09:20:20.000000 crestic-0.7.0/README.md
+drwxr-xr-x   0 nils      (1000) nils      (1000)        0 2023-06-17 10:48:34.168087 crestic-0.7.0/crestic.egg-info/
+-rw-r--r--   0 nils      (1000) nils      (1000)     2364 2023-06-17 10:48:34.000000 crestic-0.7.0/crestic.egg-info/PKG-INFO
+-rw-r--r--   0 nils      (1000) nils      (1000)      288 2023-06-17 10:48:34.000000 crestic-0.7.0/crestic.egg-info/SOURCES.txt
+-rw-r--r--   0 nils      (1000) nils      (1000)        1 2023-06-17 10:48:34.000000 crestic-0.7.0/crestic.egg-info/dependency_links.txt
+-rw-r--r--   0 nils      (1000) nils      (1000)       40 2023-06-17 10:48:34.000000 crestic-0.7.0/crestic.egg-info/entry_points.txt
+-rw-r--r--   0 nils      (1000) nils      (1000)       85 2023-06-17 10:48:34.000000 crestic-0.7.0/crestic.egg-info/requires.txt
+-rw-r--r--   0 nils      (1000) nils      (1000)        8 2023-06-17 10:48:34.000000 crestic-0.7.0/crestic.egg-info/top_level.txt
+-rwxr-xr-x   0 nils      (1000) nils      (1000)     6657 2023-06-17 10:18:09.000000 crestic-0.7.0/crestic.py
+-rw-r--r--   0 nils      (1000) nils      (1000)      107 2020-05-24 10:02:32.000000 crestic-0.7.0/pyproject.toml
+-rw-r--r--   0 nils      (1000) nils      (1000)     1523 2023-06-17 10:48:34.169087 crestic-0.7.0/setup.cfg
+-rw-r--r--   0 nils      (1000) nils      (1000)       38 2020-05-24 10:02:32.000000 crestic-0.7.0/setup.py
+drwxr-xr-x   0 nils      (1000) nils      (1000)        0 2023-06-17 10:48:34.169087 crestic-0.7.0/tests/
+-rw-r--r--   0 nils      (1000) nils      (1000)     7528 2023-06-17 10:18:09.000000 crestic-0.7.0/tests/test_all.py
+-rw-r--r--   0 nils      (1000) nils      (1000)      845 2020-05-24 08:48:43.000000 crestic-0.7.0/tests/test_utils.py
```

### Comparing `crestic-0.6.0/LICENSE` & `crestic-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crestic-0.6.0/crestic.py` & `crestic-0.7.0/crestic.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 #!/usr/bin/env python3
 
 import os
 import re
 import sys
+import glob
 import argparse
+import warnings
 import subprocess
 import configparser
 
 
 def config_files(environ=None):
     if environ is None:
         environ = {}
 
     # Lowest priority: hardcoded values
-    paths = os.pathsep.join([
-        pathexpand('~/.config/crestic'),
-        '/etc/crestic'
-    ])
+    paths = [
+        '/usr/share/crestic/config.cfg',
+        *sorted(glob.glob('/usr/share/crestic/conf.d/*.cfg')),
 
-    # Low priority: optional appdirs import
-    try:
-        import appdirs
-        paths = os.pathsep.join([
-            appdirs.user_config_dir('crestic'),
-            appdirs.site_config_dir('crestic', multipath=True)
-        ])
-    except ImportError as e:
-        pass
+        '/etc/crestic/config.cfg',
+        *sorted(glob.glob('/etc/crestic/conf.d/*.cfg')),
+
+        pathexpand('~/.config/crestic/config.cfg'),
+        *sorted(glob.glob(pathexpand('~/.config/crestic/conf.d/*.cfg'))),
+    ]
 
     # Medium priority: CRESTIC_CONFIG_PATHS
     try:
-        paths = environ['CRESTIC_CONFIG_PATHS']
+        paths = paths + [
+            f
+            for d in environ['CRESTIC_CONFIG_PATHS'].split(os.pathsep)
+            for f in sorted(glob.glob(pathexpand(d)))
+        ]
     except KeyError:
         pass
 
-    # High priority: CRESTIC_CONFIG_FILE
+    # High priority: CRESTIC_CONFIG_FILE, dropping the rest
     try:
-        return [environ['CRESTIC_CONFIG_FILE']]
+        paths = [environ['CRESTIC_CONFIG_FILE']]
     except KeyError:
         pass
 
-    return [os.path.join(x, 'crestic.cfg') for x in paths.split(os.pathsep)]
+    return paths
 
 
 def split(string, delimiter="@", maxsplit=1):
     """
     Split a string using a delimiter string. But keep the delimiter in all returned segments
 
     """
@@ -62,14 +64,27 @@
     return value
 
 
 def pathexpand(val):
     return os.path.expanduser(os.path.expandvars(val))
 
 
+def splitlines(val):
+    """
+    str.splitlines() that is tolerant to empty strings and None values
+
+    """
+    if val == "":
+        return [None]
+    if val is None:
+        return [None]
+    else:
+        return val.splitlines()
+
+
 def main(argv, environ=None, conffile=None, dryrun=None, executable=None):
     if environ is None:
         environ = os.environ
 
     if conffile is None:
         conffile = config_files(environ)
 
@@ -95,15 +110,15 @@
         "arguments", nargs="*", help="positional arguments for the restic command"
     )
     try:
         python_args = parser.parse_intermixed_args(argv)
     except AttributeError:
         python_args = parser.parse_args(argv)
 
-    config = configparser.ConfigParser()
+    config = configparser.ConfigParser(allow_no_value=True)
     config.optionxform = str  # dont map config keys to lower case
     conffile_read = config.read(conffile)
 
     sections = [
         "global",
         f"global.{python_args.command}",
     ]
@@ -122,14 +137,21 @@
     envsections = [f"{section}.environ" for section in sections]
 
     # Load restic options from config, in ascending precedence
     restic_options = {}
     sections_read = []
     for section in sections:
         try:
+            if "" in config[section].values():
+                warnings.warn(
+                    'The behaviour of empty config keys will change in 1.0.0! '
+                    'Please consult the documentation at https://nils-werner.github.io/crestic/config/options.html',
+                    DeprecationWarning,
+                )
+
             restic_options.update(**dict(config[section]))
             sections_read.append(section)
         except KeyError:
             pass
 
     # Load restic environment variables from config, in ascending precedence
     restic_environ = dict(environ)
@@ -138,15 +160,15 @@
         try:
             restic_environ.update(**dict(config[envsection]))
             envsections_read.append(envsection)
         except KeyError:
             pass
 
     restic_options = {
-        k: v.splitlines() if v != "" else [""]
+        k: splitlines(v)
         for k, v in restic_options.items()
     }
 
     # Override config arguments with arguments from CLI
     if python_args.arguments:
         restic_options['arguments'] = python_args.arguments
 
@@ -164,42 +186,37 @@
     del python_args_dict['arguments']
     restic_options.update(python_args_dict)
 
     # Construct command
     argstring = executable
     argstring.append(f"{python_args.command}")
     for key, lines in restic_options.items():
-        if lines is not None:
-            for value in lines:
-                if len(key) == 1:
-                    argstring.append(f"-{key}")
-                else:
-                    argstring.append(f"--{key}")
-                if value is not None:
-                    argstring.append(f"{value}")
+        for value in lines:
+            if len(key) == 1:
+                argstring.append(f"-{key}")
+            else:
+                argstring.append(f"--{key}")
+            if value is not None:
+                argstring.append(f"{value}")
     argstring += restic_arguments
 
-    argstring = [val for val in argstring if val != ""]
     argstring = [pathexpand(val) for val in argstring]
 
     if dryrun:
         print("             Warning:", "Executing in debug mode. restic will not run, backups are not touched!")
         print("        Config files:", ", ".join(conffile))
         print("   Config files used:", ", ".join(conffile_read))
         print("     Config sections:", ", ".join(sections))
         print("Config sections used:", ", ".join(sections_read))
         print("        Env sections:", ", ".join(envsections))
         print("   Env sections used:", ", ".join(envsections_read))
         print("    Expanded command:", " ".join(argstring))
         return 0
     else:
-        try:
-            return subprocess.call(argstring, env=restic_environ, shell=False)
-        except KeyboardInterrupt:
-            return 130
+        return os.execvpe(argstring[0], argstring, env=restic_environ)
 
 
 def cli():
     return main(sys.argv[1:])
 
 
 if __name__ == "__main__":
```

### Comparing `crestic-0.6.0/setup.cfg` & `crestic-0.7.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [metadata]
 name = crestic
-version = 0.6.0
+version = 0.7.0
 author = Nils Werner
 author_email = nils.werner@gmail.com
 description = Configurable restic
-license_file = LICENSE
+license_files = 
+	LICENSE
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/nils-werner/crestic/
 project_urls = 
 	Circle CI = https://app.circleci.com/pipelines/github/nils-werner/crestic
 	Crestic source = https://github.com/nils-werner/crestic/
 classifiers = 
@@ -45,15 +46,15 @@
 	appdirs
 	pytest
 	pytest-cov
 	pytest-mock
 	pytest-pycodestyle
 
 [tool:pytest]
-addopts = --doctest-modules --cov-report term-missing --cov crestic --pycodestyle
+addopts = --doctest-modules --cov-report term-missing --cov crestic --pycodestyle -Werror
 
 [pycodestyle]
 max-line-length = 127
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

