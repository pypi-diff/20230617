# Comparing `tmp/fsociety-3.2.8.tar.gz` & `tmp/fsociety-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fsociety-3.2.8.tar", last modified: Tue Sep  6 13:30:29 2022, max compression
+gzip compressed data, was "dist/fsociety-3.2.9.tar", last modified: Fri Jun 16 22:27:10 2023, max compression
```

## Comparing `fsociety-3.2.8.tar` & `fsociety-3.2.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:30:29.000000 fsociety-3.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)     5198 2022-09-06 13:30:10.000000 fsociety-3.2.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-09-06 13:30:10.000000 fsociety-3.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-09-06 13:30:10.000000 fsociety-3.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1610 2022-09-06 13:30:10.000000 fsociety-3.2.8/PACKAGES.md
--rw-r--r--   0 runner    (1001) docker     (121)     4360 2022-09-06 13:30:29.000000 fsociety-3.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2368 2022-09-06 13:30:10.000000 fsociety-3.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:30:29.000000 fsociety-3.2.8/fsociety/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5204 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/console.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:30:29.000000 fsociety-3.2.8/fsociety/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1721 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/core/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/core/hosts.py
--rw-r--r--   0 runner    (1001) docker     (121)     3733 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/core/menu.py
--rw-r--r--   0 runner    (1001) docker     (121)     7023 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/core/repo.py
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/core/usernames.py
--rw-r--r--   0 runner    (1001) docker     (121)     2763 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/core/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:30:29.000000 fsociety-3.2.8/fsociety/information_gathering/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/information_gathering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/information_gathering/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/information_gathering/gitgraber.py
--rw-r--r--   0 runner    (1001) docker     (121)      782 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/information_gathering/hydrarecon.py
--rw-r--r--   0 runner    (1001) docker     (121)      848 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/information_gathering/s3scanner.py
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/information_gathering/sherlock.py
--rw-r--r--   0 runner    (1001) docker     (121)      738 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/information_gathering/sqlmap.py
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/information_gathering/striker.py
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/information_gathering/sublist3r.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:30:29.000000 fsociety-3.2.8/fsociety/networking/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/networking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      873 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/networking/bettercap.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/networking/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2125 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/networking/nmap.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:30:29.000000 fsociety-3.2.8/fsociety/obfuscation/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/obfuscation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/obfuscation/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/obfuscation/cuteit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:30:29.000000 fsociety-3.2.8/fsociety/passwords/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/passwords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/passwords/changeme.py
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/passwords/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      573 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/passwords/cr3dov3r.py
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/passwords/cupp.py
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/passwords/hash_buster.py
--rw-r--r--   0 runner    (1001) docker     (121)     1997 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/passwords/traitor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:30:29.000000 fsociety-3.2.8/fsociety/web_apps/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/web_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/web_apps/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      782 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/web_apps/photon.py
--rw-r--r--   0 runner    (1001) docker     (121)      779 2022-09-06 13:30:10.000000 fsociety-3.2.8/fsociety/web_apps/xsstrike.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-06 13:30:29.000000 fsociety-3.2.8/fsociety.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4360 2022-09-06 13:30:29.000000 fsociety-3.2.8/fsociety.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-09-06 13:30:29.000000 fsociety-3.2.8/fsociety.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-06 13:30:29.000000 fsociety-3.2.8/fsociety.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-09-06 13:30:29.000000 fsociety-3.2.8/fsociety.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-09-06 13:30:29.000000 fsociety-3.2.8/fsociety.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-06 13:30:29.000000 fsociety-3.2.8/fsociety.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-09-06 13:30:10.000000 fsociety-3.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-06 13:30:29.000000 fsociety-3.2.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     3176 2022-09-06 13:30:10.000000 fsociety-3.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:27:10.000000 fsociety-3.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-06-16 22:26:52.000000 fsociety-3.2.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-16 22:26:52.000000 fsociety-3.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-16 22:26:52.000000 fsociety-3.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-16 22:26:52.000000 fsociety-3.2.9/PACKAGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-16 22:27:10.000000 fsociety-3.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-16 22:26:52.000000 fsociety-3.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:27:10.000000 fsociety-3.2.9/fsociety/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:27:10.000000 fsociety-3.2.9/fsociety/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/core/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/core/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/core/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/core/usernames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/core/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:27:10.000000 fsociety-3.2.9/fsociety/information_gathering/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/information_gathering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/information_gathering/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/information_gathering/gitgraber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/information_gathering/hydrarecon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/information_gathering/s3scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/information_gathering/sherlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/information_gathering/sqlmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/information_gathering/striker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/information_gathering/sublist3r.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:27:10.000000 fsociety-3.2.9/fsociety/networking/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/networking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/networking/bettercap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/networking/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/networking/nmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:27:10.000000 fsociety-3.2.9/fsociety/obfuscation/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/obfuscation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/obfuscation/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/obfuscation/cuteit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:27:10.000000 fsociety-3.2.9/fsociety/passwords/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/passwords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/passwords/changeme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/passwords/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/passwords/cr3dov3r.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/passwords/cupp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/passwords/hash_buster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/passwords/traitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:27:10.000000 fsociety-3.2.9/fsociety/web_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/web_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/web_apps/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/web_apps/photon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-16 22:26:52.000000 fsociety-3.2.9/fsociety/web_apps/xsstrike.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:27:10.000000 fsociety-3.2.9/fsociety.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-16 22:27:09.000000 fsociety-3.2.9/fsociety.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-16 22:27:10.000000 fsociety-3.2.9/fsociety.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 22:27:09.000000 fsociety-3.2.9/fsociety.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-16 22:27:09.000000 fsociety-3.2.9/fsociety.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-16 22:27:09.000000 fsociety-3.2.9/fsociety.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 22:27:09.000000 fsociety-3.2.9/fsociety.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 22:26:52.000000 fsociety-3.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 22:27:10.000000 fsociety-3.2.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3204 2023-06-16 22:26:52.000000 fsociety-3.2.9/setup.py
```

### Comparing `fsociety-3.2.8/CHANGELOG.md` & `fsociety-3.2.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fsociety-3.2.8/LICENSE` & `fsociety-3.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fsociety-3.2.8/PACKAGES.md` & `fsociety-3.2.9/PACKAGES.md`

 * *Files identical despite different names*

### Comparing `fsociety-3.2.8/PKG-INFO` & `fsociety-3.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsociety
-Version: 3.2.8
+Version: 3.2.9
 Summary: A Modular Penetration Testing Framework
 Home-page: https://fsociety.dev/
 Author: fsociety-team
 Author-email: contact@fsociety.dev
 License: MIT
 Project-URL: Packages, https://github.com/fsociety-team/fsociety/blob/main/PACKAGES.md
 Project-URL: Changelog, https://github.com/fsociety-team/fsociety/blob/main/CHANGELOG.md
```

### Comparing `fsociety-3.2.8/README.md` & `fsociety-3.2.9/README.md`

 * *Files identical despite different names*

### Comparing `fsociety-3.2.8/fsociety/__main__.py` & `fsociety-3.2.9/fsociety/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
-
 import argparse
 import platform
+import sys
 from random import choice
 
 from rich.columns import Columns
 from rich.text import Text
 
 import fsociety.core.utilities
 import fsociety.information_gathering
@@ -78,19 +78,19 @@
     fsociety.passwords,
     fsociety.obfuscation,
     fsociety.core.utilities,
 ]
 BUILTIN_FUNCTIONS = {
     "exit": lambda: exec("raise KeyboardInterrupt"),
 }
-items = dict()
+items = {}
 
 
 def print_menu_items():
-    cols = list()
+    cols = []
     for value in MENU_ITEMS:
         name = module_name(value)
         tools = format_tools(value.__tools__)
         tools_str = Text()
         tools_str.append("\n")
         tools_str.append(name, style="command")
         tools_str.append(tools)
@@ -122,30 +122,30 @@
     agreement()
     console.print(choice(BANNERS), style="red", highlight=False)
     print_menu_items()
     selected_command = input(prompt()).strip()
     if not selected_command or (selected_command not in commands):
         console.print("Invalid Command", style="bold yellow")
         return
-    if selected_command in BUILTIN_FUNCTIONS.keys():
+    if selected_command in BUILTIN_FUNCTIONS:
         func = BUILTIN_FUNCTIONS.get(selected_command)
         return func()
     try:
         func = items[selected_command].cli
         return func()
     except Exception as error:
         console.print(str(error))
         console.print_exception()
     return
 
 
 def info():
-    data = dict()
+    data = {}
     # Config File
-    with open(CONFIG_FILE) as file:
+    with open(CONFIG_FILE, encoding="utf-8") as file:
         data["Config File"] = file.read().strip()
     data["Python Version"] = platform.python_version()
     data["Platform"] = platform.platform()
     os = config.get("fsociety", "os")
     if os == "macos":
         data["macOS"] = platform.mac_ver()[0]
     elif os == "windows":
@@ -153,23 +153,22 @@
 
     for key, value in data.items():
         console.print(f"# {key}")
         console.print(value, end="\n\n")
 
 
 def interactive():
-
     try:
         while True:
             set_readline(commands)
             mainloop()
     except KeyboardInterrupt:
         console.print("\nExitting...")
         write_config(config)
-        exit(0)
+        sys.exit(0)
 
 
 def main():
     parser = argparse.ArgumentParser(description="A Penetration Testing Framework")
     parser.add_argument("-i", "--info", action="store_true", help="gets fsociety info")
     parser.add_argument("-s", "--suggest", action="store_true", help="suggest a tool")
```

### Comparing `fsociety-3.2.8/fsociety/core/config.py` & `fsociety-3.2.9/fsociety/core/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,26 +31,26 @@
 
 def get_config() -> RawConfigParser:
     config = RawConfigParser()
     if not os.path.exists(INSTALL_DIR):
         os.mkdir(INSTALL_DIR)
     if not os.path.exists(CONFIG_FILE):
         config["fsociety"] = DEFAULT_CONFIG
-        with open(CONFIG_FILE, "w") as configfile:
+        with open(CONFIG_FILE, "w", encoding="utf-8") as configfile:
             config.write(configfile)
     config.read(CONFIG_FILE)
     check_config(config)
     if config.get("fsociety", "version") != __version__:
         config.set("fsociety", "version", __version__)
         write_config(config)
     return config
 
 
 def write_config(config: RawConfigParser) -> None:
-    with open(CONFIG_FILE, "w") as configfile:
+    with open(CONFIG_FILE, "w", encoding="utf-8") as configfile:
         config.write(configfile)
 
 
 def check_config(config: RawConfigParser) -> None:
     for key in DEFAULT_CONFIG:
         try:
             config.get("fsociety", key)
```

### Comparing `fsociety-3.2.8/fsociety/core/hosts.py` & `fsociety-3.2.9/fsociety/core/hosts.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 class InvalidHost(Exception):
     pass
 
 
 def get_hosts() -> List[str]:
     try:
-        with open(full_path) as hostfile:
+        with open(full_path, encoding="utf-8") as hostfile:
             return [host.strip() for host in hostfile]
     except FileNotFoundError:
-        return list()
+        return []
 
 
 def add_host(host: str) -> None:
     if not host:
         raise ValueError
-    with open(full_path, "a") as hostfile:
+    with open(full_path, "a", encoding="utf-8") as hostfile:
         hostfile.write(f"\n{host}")
```

### Comparing `fsociety-3.2.8/fsociety/core/menu.py` & `fsociety-3.2.9/fsociety/core/menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,29 +81,29 @@
 def tools_cli(name, tools, links=True):
     table = Table(box=box.HEAVY_HEAD)
     table.add_column("Name", style="red", no_wrap=True)
     table.add_column("Description", style="magenta")
     if links:
         table.add_column("Link", no_wrap=True)
 
-    tools_dict = dict()
+    tools_dict = {}
     for tool in tools:
         tools_dict[str(tool)] = tool
         args = [str(tool), tool.description]
         if links:
             text_link = Text(f"{tool.path}")
             text_link.stylize(Style(link=f"https://github.com/{tool.path}"))
             args.append(text_link)
         table.add_row(*args)
 
     console.print(table)
     console.print("back", style="command")
     set_readline(list(tools_dict.keys()) + BACK_COMMANDS)
     selected_tool = input(prompt(name.split(".")[-2])).strip()
-    if selected_tool not in tools_dict.keys():
+    if selected_tool not in tools_dict:
         if selected_tool in BACK_COMMANDS:
             return
         if selected_tool == "exit":
             raise KeyboardInterrupt
         console.print("Invalid Command", style="bold yellow")
         return tools_cli(name, tools, links)
     tool = tools_dict.get(selected_tool)
```

### Comparing `fsociety-3.2.8/fsociety/core/repo.py` & `fsociety-3.2.9/fsociety/core/repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 config = get_config()
 
 
 def print_pip_deps(packages: Union[str, Iterable[str]]) -> None:
     requirements = []
     if isinstance(packages, str) and os.path.exists(packages):
-        with open(packages) as requirements_file:
+        with open(packages, encoding="utf-8") as requirements_file:
             for line in requirements_file:
                 if line.strip():
                     requirements.append(line)
     elif isinstance(packages, Iterable):
         requirements = list(packages)
     else:
         raise ValueError
```

### Comparing `fsociety-3.2.8/fsociety/core/usernames.py` & `fsociety-3.2.9/fsociety/core/usernames.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 config = get_config()
 
 full_path = os.path.join(INSTALL_DIR, config.get("fsociety", "usernames_file"))
 
 
 def get_usernames() -> List[str]:
     try:
-        with open(full_path) as usernamefile:
+        with open(full_path, encoding="utf-8") as usernamefile:
             return [username.strip() for username in usernamefile]
     except FileNotFoundError:
-        return list()
+        return []
 
 
 def add_username(username: str) -> None:
-    with open(full_path, "a") as usernamefile:
+    with open(full_path, "a", encoding="utf-8") as usernamefile:
         usernamefile.write(f"\n{username}")
```

### Comparing `fsociety-3.2.8/fsociety/core/utilities.py` & `fsociety-3.2.9/fsociety/core/utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,15 +80,17 @@
     8I  Yb 88__    Yb  dP  `Ybo."
     8I  dY 88""     YbdP   o.`Y8b
     8888Y"  888888    YP    8bodP'
     """,
             style="bold yellow",
             highlight=False,
         )
-        response = get(f"https://api.github.com/repos/{GITHUB_PATH}/contributors")
+        response = get(
+            f"https://api.github.com/repos/{GITHUB_PATH}/contributors", timeout=30
+        )
         contributors = response.json()
         for contributor in sorted(
             contributors, key=lambda c: c["contributions"], reverse=True
         ):
             username = contributor.get("login")
             console.print(f" {username} ".center(30, "-"))
```

### Comparing `fsociety-3.2.8/fsociety/information_gathering/gitgraber.py` & `fsociety-3.2.9/fsociety/information_gathering/gitgraber.py`

 * *Files identical despite different names*

### Comparing `fsociety-3.2.8/fsociety/information_gathering/hydrarecon.py` & `fsociety-3.2.9/fsociety/information_gathering/hydrarecon.py`

 * *Files identical despite different names*

### Comparing `fsociety-3.2.8/fsociety/information_gathering/s3scanner.py` & `fsociety-3.2.9/fsociety/information_gathering/s3scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,14 @@
         )
 
     def run(self):
         os.chdir(self.full_path)
         set_readline([])
         user_domains = input("\nEnter one or more domains: ").strip()
         txt_path = os.path.join(INSTALL_DIR, "s3_domains.txt")
-        with open(txt_path, "w") as domains_file:
+        with open(txt_path, "w", encoding="utf-8") as domains_file:
             for domain in user_domains.split():
                 domains_file.write(domain)
         return os.system(f"python3 s3scanner.py {txt_path}")
 
 
 s3scanner = S3scannerRepo()
```

### Comparing `fsociety-3.2.8/fsociety/information_gathering/sherlock.py` & `fsociety-3.2.9/fsociety/information_gathering/sherlock.py`

 * *Files identical despite different names*

### Comparing `fsociety-3.2.8/fsociety/information_gathering/sqlmap.py` & `fsociety-3.2.9/fsociety/information_gathering/sqlmap.py`

 * *Files identical despite different names*

### Comparing `fsociety-3.2.8/fsociety/information_gathering/striker.py` & `fsociety-3.2.9/fsociety/information_gathering/striker.py`

 * *Files identical despite different names*

### Comparing `fsociety-3.2.8/fsociety/information_gathering/sublist3r.py` & `fsociety-3.2.9/fsociety/information_gathering/sublist3r.py`

 * *Files identical despite different names*

### Comparing `fsociety-3.2.8/fsociety/networking/bettercap.py` & `fsociety-3.2.9/fsociety/networking/bettercap.py`

 * *Files identical despite different names*

### Comparing `fsociety-3.2.8/fsociety/networking/nmap.py` & `fsociety-3.2.9/fsociety/networking/nmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,14 @@
             add_host(host)
         longest_key = max(len(key) for key in premade_args) + 2
         print("\nName".ljust(longest_key) + " | Args")
         for name, args in premade_args.items():
             print(f"{name.ljust(longest_key)}: {args.format(host=host)}")
         set_readline(premade_args.keys())
         selected = input("\nMake a selection: ")
-        if selected and selected in premade_args.keys():
+        if selected and selected in premade_args:
             args = premade_args.get(selected).format(host=host)
             return os.system(f"nmap {args}")
         return self.run()
 
 
 nmap = NmapRepo()
```

### Comparing `fsociety-3.2.8/fsociety/passwords/changeme.py` & `fsociety-3.2.9/fsociety/passwords/changeme.py`

 * *Files identical despite different names*

### Comparing `fsociety-3.2.8/fsociety/passwords/cr3dov3r.py` & `fsociety-3.2.9/fsociety/passwords/cr3dov3r.py`

 * *Files identical despite different names*

### Comparing `fsociety-3.2.8/fsociety/passwords/traitor.py` & `fsociety-3.2.9/fsociety/passwords/traitor.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 premade_args = {"any": "-a"}
 arch_map = {"x86_64": "amd64", "i386": "386"}
 
 
 class TraitorRepo(GitHubRepo):
     def __init__(self):
-        if os.uname().machine in arch_map.keys():
+        if os.uname().machine in arch_map:
             self.arch = arch_map.get(os.uname().machine)
         else:
             self.arch = ""
         self.version = "v0.0.14"
         super().__init__(
             path="liamg/traitor",
             install={"binary": ""},
@@ -42,15 +42,15 @@
             print(f"{name.ljust(longest_key)}: {args.format()}")
         set_readline(premade_args.keys())
         selected = input("\nMake a selection: ")
         if selected and selected in premade_args:
             return os.system(
                 f"{self.full_path}/{self.name} {premade_args.get(selected)}"
             )
-        elif (
-            selected and selected not in premade_args.keys()
+        if (
+            selected and selected not in premade_args
         ):  # allow passing custom specific exploits
             return os.system(f"{self.full_path}/{self.name} -e {selected}")
         return self.run()
 
 
 traitor = TraitorRepo()
```

### Comparing `fsociety-3.2.8/fsociety/web_apps/photon.py` & `fsociety-3.2.9/fsociety/web_apps/photon.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
             install={"pip": "requirements.txt"},
             description="Incredibly fast crawler designed for OSINT",
         )
 
     def run(self):
         os.chdir(self.full_path)
         user_url = input("\nEnter a url to scan: ").strip()
-        args = list()
+        args = []
         if confirm("Do you want to clone the site?"):
             args.append("--clone")
         if confirm("Do you want to use wayback?"):
             args.append("--wayback")
         args_str = " ".join(args)
         return os.system(f"python3 photon.py --url {user_url} {args_str}")
```

### Comparing `fsociety-3.2.8/fsociety/web_apps/xsstrike.py` & `fsociety-3.2.9/fsociety/web_apps/xsstrike.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,15 @@
             install={"pip": "requirements.txt"},
             description="Advanced XSS Detection Suite",
         )
 
     def run(self):
         os.chdir(self.full_path)
         user_url = input("\nEnter a url to scan: ").strip()
-        args = list()
+        args = []
         if confirm("Do you want to crawl?"):
             args.append("--crawl")
         if confirm("Do you want to find hidden parameters?"):
             args.append("--params")
         args_str = " ".join(args)
         return os.system(f"python3 xsstrike.py --url {user_url} {args_str}")
```

### Comparing `fsociety-3.2.8/fsociety.egg-info/PKG-INFO` & `fsociety-3.2.9/fsociety.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsociety
-Version: 3.2.8
+Version: 3.2.9
 Summary: A Modular Penetration Testing Framework
 Home-page: https://fsociety.dev/
 Author: fsociety-team
 Author-email: contact@fsociety.dev
 License: MIT
 Project-URL: Packages, https://github.com/fsociety-team/fsociety/blob/main/PACKAGES.md
 Project-URL: Changelog, https://github.com/fsociety-team/fsociety/blob/main/CHANGELOG.md
```

### Comparing `fsociety-3.2.8/fsociety.egg-info/SOURCES.txt` & `fsociety-3.2.9/fsociety.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fsociety-3.2.8/setup.py` & `fsociety-3.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 AUTHOR = "fsociety-team"
 REQUIRES_PYTHON = ">=3.7.0"
 VERSION = None
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 pkg_vars = {}  # type: ignore
-with open(os.path.join(here, NAME, "__version__.py")) as f:
+with open(os.path.join(here, NAME, "__version__.py"), encoding="utf-8") as f:
     exec(f.read(), pkg_vars)
 
 try:
     with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
         long_description = "\n" + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 
 def get_requirements(path: str) -> list:
-    with open(path) as f:
+    with open(path, encoding="utf-8") as f:
         return f.read().splitlines()
 
 
 class TagCommand(Command):
     """Support setup.py push_tag."""
 
     description = "Push latest version as tag."
@@ -54,15 +54,15 @@
         pass
 
     def finalize_options(self):
         pass
 
     def run(self):
         self.status("Pushing git tags…")
-        os.system("git tag v{}".format(pkg_vars["__version__"]))
+        os.system(f'git tag v{pkg_vars["__version__"]}')
         os.system("git push --tags")
 
         sys.exit()
 
 
 setup(
     name=NAME,
```

