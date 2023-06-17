# Comparing `tmp/vastaanottaa-2023.6.12.tar.gz` & `tmp/vastaanottaa-2023.6.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vastaanottaa-2023.6.12.tar", last modified: Sun Jun 11 18:48:40 2023, max compression
+gzip compressed data, was "vastaanottaa-2023.6.17.tar", last modified: Sat Jun 17 15:00:24 2023, max compression
```

## Comparing `vastaanottaa-2023.6.12.tar` & `vastaanottaa-2023.6.17.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-11 18:48:40.580314 vastaanottaa-2023.6.12/
--rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 vastaanottaa-2023.6.12/LICENSE
--rw-r--r--   0 ruth       (501) staff       (20)       34 2021-05-12 16:52:51.000000 vastaanottaa-2023.6.12/MANIFEST.in
--rw-r--r--   0 ruth       (501) staff       (20)     3291 2023-06-11 18:48:40.580175 vastaanottaa-2023.6.12/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     2224 2023-06-11 10:48:35.000000 vastaanottaa-2023.6.12/README.md
--rw-r--r--   0 ruth       (501) staff       (20)     2657 2023-06-11 16:15:51.000000 vastaanottaa-2023.6.12/pyproject.toml
--rw-r--r--   0 ruth       (501) staff       (20)       38 2023-06-11 18:48:40.580349 vastaanottaa-2023.6.12/setup.cfg
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-11 18:48:40.576903 vastaanottaa-2023.6.12/test/
--rw-r--r--   0 ruth       (501) staff       (20)     2458 2023-06-11 18:09:56.000000 vastaanottaa-2023.6.12/test/test_cli.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-11 18:48:40.578048 vastaanottaa-2023.6.12/vastaanottaa/
--rw-r--r--   0 ruth       (501) staff       (20)      641 2023-06-11 18:47:21.000000 vastaanottaa-2023.6.12/vastaanottaa/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)      125 2023-06-11 13:17:48.000000 vastaanottaa-2023.6.12/vastaanottaa/__main__.py
--rw-r--r--   0 ruth       (501) staff       (20)     3715 2023-06-11 18:09:09.000000 vastaanottaa-2023.6.12/vastaanottaa/cli.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-11 18:48:40.580004 vastaanottaa-2023.6.12/vastaanottaa.egg-info/
--rw-r--r--   0 ruth       (501) staff       (20)     3291 2023-06-11 18:48:40.000000 vastaanottaa-2023.6.12/vastaanottaa.egg-info/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)      349 2023-06-11 18:48:40.000000 vastaanottaa-2023.6.12/vastaanottaa.egg-info/SOURCES.txt
--rw-r--r--   0 ruth       (501) staff       (20)        1 2023-06-11 18:48:40.000000 vastaanottaa-2023.6.12/vastaanottaa.egg-info/dependency_links.txt
--rw-r--r--   0 ruth       (501) staff       (20)       54 2023-06-11 18:48:40.000000 vastaanottaa-2023.6.12/vastaanottaa.egg-info/entry_points.txt
--rw-r--r--   0 ruth       (501) staff       (20)       96 2023-06-11 18:48:40.000000 vastaanottaa-2023.6.12/vastaanottaa.egg-info/requires.txt
--rw-r--r--   0 ruth       (501) staff       (20)       13 2023-06-11 18:48:40.000000 vastaanottaa-2023.6.12/vastaanottaa.egg-info/top_level.txt
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-17 15:00:24.684983 vastaanottaa-2023.6.17/
+-rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 vastaanottaa-2023.6.17/LICENSE
+-rw-r--r--   0 ruth       (501) staff       (20)       34 2021-05-12 16:52:51.000000 vastaanottaa-2023.6.17/MANIFEST.in
+-rw-r--r--   0 ruth       (501) staff       (20)     3291 2023-06-17 15:00:24.684828 vastaanottaa-2023.6.17/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     2224 2023-06-11 10:48:35.000000 vastaanottaa-2023.6.17/README.md
+-rw-r--r--   0 ruth       (501) staff       (20)     2657 2023-06-17 14:54:05.000000 vastaanottaa-2023.6.17/pyproject.toml
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-06-17 15:00:24.685021 vastaanottaa-2023.6.17/setup.cfg
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-17 15:00:24.678164 vastaanottaa-2023.6.17/test/
+-rw-r--r--   0 ruth       (501) staff       (20)     3047 2023-06-17 12:53:55.000000 vastaanottaa-2023.6.17/test/test_cli.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-17 15:00:24.680717 vastaanottaa-2023.6.17/vastaanottaa/
+-rw-r--r--   0 ruth       (501) staff       (20)      641 2023-06-17 14:58:06.000000 vastaanottaa-2023.6.17/vastaanottaa/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      125 2023-06-11 13:17:48.000000 vastaanottaa-2023.6.17/vastaanottaa/__main__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     4097 2023-06-17 12:35:38.000000 vastaanottaa-2023.6.17/vastaanottaa/cli.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-17 15:00:24.684396 vastaanottaa-2023.6.17/vastaanottaa.egg-info/
+-rw-r--r--   0 ruth       (501) staff       (20)     3291 2023-06-17 15:00:24.000000 vastaanottaa-2023.6.17/vastaanottaa.egg-info/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)      349 2023-06-17 15:00:24.000000 vastaanottaa-2023.6.17/vastaanottaa.egg-info/SOURCES.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        1 2023-06-17 15:00:24.000000 vastaanottaa-2023.6.17/vastaanottaa.egg-info/dependency_links.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       54 2023-06-17 15:00:24.000000 vastaanottaa-2023.6.17/vastaanottaa.egg-info/entry_points.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       96 2023-06-17 15:00:24.000000 vastaanottaa-2023.6.17/vastaanottaa.egg-info/requires.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       13 2023-06-17 15:00:24.000000 vastaanottaa-2023.6.17/vastaanottaa.egg-info/top_level.txt
```

### Comparing `vastaanottaa-2023.6.12/LICENSE` & `vastaanottaa-2023.6.17/LICENSE`

 * *Files identical despite different names*

### Comparing `vastaanottaa-2023.6.12/PKG-INFO` & `vastaanottaa-2023.6.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vastaanottaa
-Version: 2023.6.12
+Version: 2023.6.17
 Summary: Receive (Finnish: vastaanottaa) text traversing unknown territories.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/vastaanottaa
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/vastaanottaa
 Project-URL: Documentation, https://codes.dilettant.life/docs/vastaanottaa
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/vastaanottaa
```

### Comparing `vastaanottaa-2023.6.12/README.md` & `vastaanottaa-2023.6.17/README.md`

 * *Files identical despite different names*

### Comparing `vastaanottaa-2023.6.12/pyproject.toml` & `vastaanottaa-2023.6.17/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vastaanottaa"
-version = "2023.6.12"
+version = "2023.6.17"
 description = "Receive (Finnish: vastaanottaa) text traversing unknown territories."
 readme = "README.md"
 authors = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 maintainers = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `vastaanottaa-2023.6.12/test/test_cli.py` & `vastaanottaa-2023.6.17/test/test_cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 TRG = """\
 Z0FBQUFBQmtoZERaTHN6Yk8tcnhRVFZfYzhPRnJMLWR2Q2Fnb2lRRGk4b0FxdkUyYWh3T3lUcm80
 TFloYTEyTmdfbWJMQXhjblpkX3VSZmxDQ0xRcm5FSEJvZHlzWlNfYXc9PQ==
 """
 
 SLT_NULL = ''
 
+SRC_ARMOR_A_1 = 'test/fixtures/basic/armored.vastaanottaa'
+SRC_RAW_A_1 = 'test/fixtures/basic/armored.vastaanottaa.raw'
+SEC_A_1 = 'ja'
+SLT_A_1 = '213gJL0ib2LC++IyWx97VA==\n'
+
 
 def test_cli_send_uc_1(capsys):
     rc = cli.app(['send', SEC, SRC, SLT])
     assert rc == 0
     out, err = capsys.readouterr()
     assert 'salt provided as parameter' in err
     assert 'MESSAGE' in out
@@ -24,14 +29,30 @@
     rc = cli.app(['recv', SEC, TRG, SLT])
     assert rc == 0
     out, err = capsys.readouterr()
     assert 'content' in err
     assert SRC in out
 
 
+def test_cli_recv_uc_armor_a_1(capsys):
+    rc = cli.app(['recv', SEC_A_1, SRC_ARMOR_A_1, SLT_A_1])
+    assert rc == 0
+    out, err = capsys.readouterr()
+    assert 'content' in err
+    assert 'nein' in out
+
+
+def test_cli_recv_uc_raw_a_1(capsys):
+    rc = cli.app(['recv', SEC_A_1, SRC_RAW_A_1, SLT_A_1])
+    assert rc == 0
+    out, err = capsys.readouterr()
+    assert 'content' in err
+    assert 'nein' in out
+
+
 def test_cli_uc_version_1(capsys):
     for arg in ('-V', '--version', 'version'):
         rc = cli.app([arg])
         assert rc == 0
         out, err = capsys.readouterr()
         assert APP_ALIAS in err
         assert VERSION in err
```

### Comparing `vastaanottaa-2023.6.12/vastaanottaa/__init__.py` & `vastaanottaa-2023.6.17/vastaanottaa/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Receive (Finnish: vastaanottaa) text traversing unknown territories."""
 # [[[fill git_describe()]]]
-__version__ = '2023.6.12+parent.gf1b5cf69'
-# [[[end]]] (checksum: c65b3f25c3013583a659479eccace65b)
+__version__ = '2023.6.17+parent.g290b9c34'
+# [[[end]]] (checksum: f906d477470ad7cc9067b497c89ebd43)
 __version_info__ = tuple(
     e if '-' not in e else e.split('-')[0] for part in __version__.split('+') for e in part.split('.') if e != 'parent'
 )
 
 APP_NAME = 'Receive (Finnish: vastaanottaa) text traversing unknown territories.'
 APP_ALIAS = 'vastaanottaa'
 APP_ENV = APP_ALIAS.upper()
```

### Comparing `vastaanottaa-2023.6.12/vastaanottaa/cli.py` & `vastaanottaa-2023.6.17/vastaanottaa/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,19 @@
 SALT_LEN = 16
 SALT = os.urandom(SALT_LEN)
 N_ITER = 480000
 
 ARMOR_MSG_BEGIN = f'---- BEGIN {APP_ENV} MESSAGE ----'
 ARMOR_MSG_END = f'---- END {APP_ENV} MESSAGE ----'
 
+ARMOR_MSG_BEGIN_BYTES = ARMOR_MSG_BEGIN.encode(ENCODING)
+ARMOR_MSG_END_BYTES = ARMOR_MSG_BEGIN.encode(ENCODING)
+
+ARMOR_PADDED_LENGTH = len(ARMOR_MSG_BEGIN_BYTES) + 1 + len(ARMOR_MSG_END_BYTES) + 1
+
 ARMOR_SALT_BEGIN = f'---- BEGIN {APP_ENV} SALT ----'
 ARMOR_SALT_END = f'---- END {APP_ENV} SALT ----'
 
 USAGE_INFO = f'usage: {APP_ALIAS} send|recv given text-or-file salt-for-recv'
 
 
 @no_type_check
@@ -104,11 +109,14 @@
         print(ARMOR_MSG_END)
         print(file=sys.stderr)
         print(ARMOR_SALT_BEGIN, file=sys.stderr)
         print(base64.encodebytes(salt), file=sys.stderr)
         print(ARMOR_SALT_END, file=sys.stderr)
         return 0
 
+    if src_data.startswith(ARMOR_MSG_BEGIN_BYTES) and len(src_data) > ARMOR_PADDED_LENGTH:
+        src_data = src_data[len(ARMOR_MSG_BEGIN_BYTES) + 1 : -len(ARMOR_MSG_END_BYTES) + 1]
+
     rcv = base64.decodebytes(src_data)
     print(f.decrypt(rcv).decode(ENCODING))
 
     return 0
```

### Comparing `vastaanottaa-2023.6.12/vastaanottaa.egg-info/PKG-INFO` & `vastaanottaa-2023.6.17/vastaanottaa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vastaanottaa
-Version: 2023.6.12
+Version: 2023.6.17
 Summary: Receive (Finnish: vastaanottaa) text traversing unknown territories.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/vastaanottaa
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/vastaanottaa
 Project-URL: Documentation, https://codes.dilettant.life/docs/vastaanottaa
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/vastaanottaa
```

