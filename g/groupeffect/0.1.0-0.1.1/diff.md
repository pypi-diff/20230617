# Comparing `tmp/groupeffect-0.1.0.tar.gz` & `tmp/groupeffect-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groupeffect-0.1.0.tar", last modified: Sat Apr  1 18:05:45 2023, max compression
+gzip compressed data, was "groupeffect-0.1.1.tar", last modified: Sat Jun 17 14:15:07 2023, max compression
```

## Comparing `groupeffect-0.1.0.tar` & `groupeffect-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:05:45.677182 groupeffect-0.1.0/
--rwxrwxrwx   0 root         (0) root         (0)     1068 2023-04-01 17:28:52.000000 groupeffect-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      438 2023-04-01 18:05:45.677182 groupeffect-0.1.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       33 2023-04-01 17:48:50.000000 groupeffect-0.1.0/README.md
--rwxrwxrwx   0 root         (0) root         (0)      487 2023-04-01 18:05:08.000000 groupeffect-0.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-01 18:05:45.677182 groupeffect-0.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:05:45.677182 groupeffect-0.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:05:45.677182 groupeffect-0.1.0/src/groupeffect/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-01 16:23:02.000000 groupeffect-0.1.0/src/groupeffect/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      335 2023-04-01 16:37:08.000000 groupeffect-0.1.0/src/groupeffect/framework.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 18:05:45.677182 groupeffect-0.1.0/src/groupeffect.egg-info/
--rw-r--r--   0 root         (0) root         (0)      438 2023-04-01 18:05:45.000000 groupeffect-0.1.0/src/groupeffect.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      245 2023-04-01 18:05:45.000000 groupeffect-0.1.0/src/groupeffect.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-01 18:05:45.000000 groupeffect-0.1.0/src/groupeffect.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-01 18:05:45.000000 groupeffect-0.1.0/src/groupeffect.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/
+-rwxrwxrwx   0 root         (0) root         (0)     1068 2023-04-01 18:23:21.000000 groupeffect-0.1.1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       75 2023-06-17 11:59:17.000000 groupeffect-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-06-17 14:15:07.321877 groupeffect-0.1.1/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)     1128 2023-06-17 14:14:46.000000 groupeffect-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/groupeffect/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      160 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/admin.py
+-rw-rw-r--   0 root         (0) root         (0)      154 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/groupeffect/database/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/database/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      273 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/database/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/groupeffect/management/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/groupeffect/management/commands/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/management/commands/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       52 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/management/commands/effect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/groupeffect/migrations/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/migrations/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       59 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/groupeffect/serializers/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/serializers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      252 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/serializers/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.317877 groupeffect-0.1.1/groupeffect/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/groupeffect/templates/rest_framework/
+-rw-rw-r--   0 root         (0) root         (0)     2056 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/templates/rest_framework/api.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/groupeffect/tests/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/groupeffect/urls/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/urls/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      253 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/urls/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/groupeffect/views/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/views/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      423 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/views/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/groupeffect.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-06-17 14:15:07.000000 groupeffect-0.1.1/groupeffect.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      781 2023-06-17 14:15:07.000000 groupeffect-0.1.1/groupeffect.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 14:15:07.000000 groupeffect-0.1.1/groupeffect.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-06-17 14:15:07.000000 groupeffect-0.1.1/groupeffect.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-17 14:15:07.000000 groupeffect-0.1.1/groupeffect.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      814 2023-06-17 14:15:07.321877 groupeffect-0.1.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-06-17 11:59:17.000000 groupeffect-0.1.1/setup.py
```

### Comparing `groupeffect-0.1.0/LICENSE` & `groupeffect-0.1.1/LICENSE`

 * *Files identical despite different names*

