# Comparing `tmp/mysql-to-sqlite3-1.4.9.tar.gz` & `tmp/mysql_to_sqlite3-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql-to-sqlite3-1.4.9.tar", last modified: Sun Oct 10 12:25:33 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `mysql-to-sqlite3-1.4.9.tar` & `mysql_to_sqlite3-2.0.0.tar`

### file list

```diff
@@ -1,41 +1,25 @@
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 12:25:33.642385 mysql-to-sqlite3-1.4.9/
--rw-r--r--   0 klemen     (501) staff       (20)     5513 2021-09-19 12:14:51.000000 mysql-to-sqlite3-1.4.9/CODE-OF-CONDUCT.md
--rw-r--r--   0 klemen     (501) staff       (20)     1069 2021-02-13 10:59:16.000000 mysql-to-sqlite3-1.4.9/LICENSE
--rw-r--r--   0 klemen     (501) staff       (20)      166 2020-07-19 22:16:56.000000 mysql-to-sqlite3-1.4.9/MANIFEST.in
--rw-r--r--   0 klemen     (501) staff       (20)     6136 2021-10-10 12:25:33.643053 mysql-to-sqlite3-1.4.9/PKG-INFO
--rw-r--r--   0 klemen     (501) staff       (20)     4735 2021-10-10 11:20:53.000000 mysql-to-sqlite3-1.4.9/README.md
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 12:25:33.595304 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/
--rw-r--r--   0 klemen     (501) staff       (20)       95 2020-07-18 12:41:29.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/__init__.py
--rw-r--r--   0 klemen     (501) staff       (20)      363 2021-10-10 12:24:54.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/__version__.py
--rw-r--r--   0 klemen     (501) staff       (20)     4740 2021-10-10 11:20:53.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/cli.py
--rw-r--r--   0 klemen     (501) staff       (20)     2598 2021-08-07 15:18:45.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/click_utils.py
--rw-r--r--   0 klemen     (501) staff       (20)     3451 2020-11-05 17:57:09.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/debug_info.py
--rw-r--r--   0 klemen     (501) staff       (20)      175 2020-08-31 13:42:08.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/sixeptions.py
--rw-r--r--   0 klemen     (501) staff       (20)     1183 2021-08-01 13:08:36.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/sqlite_utils.py
--rw-r--r--   0 klemen     (501) staff       (20)    21698 2021-10-10 11:20:52.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/transporter.py
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 12:25:33.611977 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3.egg-info/
--rw-r--r--   0 klemen     (501) staff       (20)     6136 2021-10-10 12:25:33.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3.egg-info/PKG-INFO
--rw-r--r--   0 klemen     (501) staff       (20)      874 2021-10-10 12:25:33.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3.egg-info/SOURCES.txt
--rw-r--r--   0 klemen     (501) staff       (20)        1 2021-10-10 12:25:33.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3.egg-info/dependency_links.txt
--rw-r--r--   0 klemen     (501) staff       (20)       77 2021-10-10 12:25:33.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3.egg-info/entry_points.txt
--rw-r--r--   0 klemen     (501) staff       (20)        1 2020-07-18 12:41:59.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3.egg-info/not-zip-safe
--rw-r--r--   0 klemen     (501) staff       (20)      347 2021-10-10 12:25:33.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3.egg-info/requires.txt
--rw-r--r--   0 klemen     (501) staff       (20)       17 2021-10-10 12:25:33.000000 mysql-to-sqlite3-1.4.9/mysql_to_sqlite3.egg-info/top_level.txt
--rw-r--r--   0 klemen     (501) staff       (20)      337 2020-07-18 12:41:29.000000 mysql-to-sqlite3-1.4.9/pytest.ini
--rw-r--r--   0 klemen     (501) staff       (20)      736 2021-08-07 16:16:06.000000 mysql-to-sqlite3-1.4.9/requirements_dev.txt
--rw-r--r--   0 klemen     (501) staff       (20)      191 2021-10-10 12:25:33.648235 mysql-to-sqlite3-1.4.9/setup.cfg
--rw-r--r--   0 klemen     (501) staff       (20)     2486 2021-10-10 11:59:45.000000 mysql-to-sqlite3-1.4.9/setup.py
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 12:25:33.628152 mysql-to-sqlite3-1.4.9/tests/
--rw-r--r--   0 klemen     (501) staff       (20)        0 2020-07-18 12:41:29.000000 mysql-to-sqlite3-1.4.9/tests/__init__.py
--rw-r--r--   0 klemen     (501) staff       (20)    12783 2020-08-31 13:37:27.000000 mysql-to-sqlite3-1.4.9/tests/conftest.py
--rw-r--r--   0 klemen     (501) staff       (20)     1321 2020-07-26 12:31:00.000000 mysql-to-sqlite3-1.4.9/tests/database.py
--rw-r--r--   0 klemen     (501) staff       (20)     3820 2020-07-18 12:41:29.000000 mysql-to-sqlite3-1.4.9/tests/factories.py
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 12:25:33.633165 mysql-to-sqlite3-1.4.9/tests/func/
--rw-r--r--   0 klemen     (501) staff       (20)        0 2020-07-18 12:41:29.000000 mysql-to-sqlite3-1.4.9/tests/func/__init__.py
--rw-r--r--   0 klemen     (501) staff       (20)    38476 2021-08-07 11:14:10.000000 mysql-to-sqlite3-1.4.9/tests/func/mysql_to_sqlite3_test.py
--rw-r--r--   0 klemen     (501) staff       (20)    12737 2021-08-07 14:23:37.000000 mysql-to-sqlite3-1.4.9/tests/func/test_cli.py
--rw-r--r--   0 klemen     (501) staff       (20)     5877 2021-03-04 20:56:52.000000 mysql-to-sqlite3-1.4.9/tests/models.py
--rw-r--r--   0 klemen     (501) staff       (20)      201 2020-07-18 12:41:29.000000 mysql-to-sqlite3-1.4.9/tests/sixeptions.py
-drwxr-xr-x   0 klemen     (501) staff       (20)        0 2021-10-10 12:25:33.639234 mysql-to-sqlite3-1.4.9/tests/unit/
--rw-r--r--   0 klemen     (501) staff       (20)        0 2020-07-18 12:41:29.000000 mysql-to-sqlite3-1.4.9/tests/unit/__init__.py
--rw-r--r--   0 klemen     (501) staff       (20)    20853 2021-10-10 11:20:52.000000 mysql-to-sqlite3-1.4.9/tests/unit/mysql_to_sqlite3_test.py
+-rw-r--r--   0        0        0     5513 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/requirements_dev.txt
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/__init__.py
+-rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/cli.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/click_utils.py
+-rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/debug_info.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/py.typed
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/sqlite_utils.py
+-rw-r--r--   0        0        0    24622 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/transporter.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/tests/database.py
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/tests/factories.py
+-rw-r--r--   0        0        0     6924 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/tests/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/tests/func/__init__.py
+-rw-r--r--   0        0        0    47466 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/tests/func/mysql_to_sqlite3_test.py
+-rw-r--r--   0        0        0    15572 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/tests/func/test_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0    24408 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/tests/unit/mysql_to_sqlite3_test.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/LICENSE
+-rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/README.md
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 mysql_to_sqlite3-2.0.0/PKG-INFO
```

### Comparing `mysql-to-sqlite3-1.4.9/CODE-OF-CONDUCT.md` & `mysql_to_sqlite3-2.0.0/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mysql-to-sqlite3-1.4.9/LICENSE` & `mysql_to_sqlite3-2.0.0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Klemen Tusar
+Copyright (c) 2023 Klemen Tusar
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mysql-to-sqlite3-1.4.9/PKG-INFO` & `mysql_to_sqlite3-2.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 Metadata-Version: 2.1
 Name: mysql-to-sqlite3
-Version: 1.4.9
+Version: 2.0.0
 Summary: A simple Python tool to transfer data from MySQL to SQLite 3
-Home-page: https://github.com/techouse/mysql-to-sqlite3
-Author: Klemen Tusar
-Author-email: techouse@gmail.com
-License: MIT
 Project-URL: Source, https://github.com/techouse/mysql-to-sqlite3
-Platform: UNKNOWN
+Author-email: Klemen Tusar <techouse@gmail.com>
+License: MIT
+License-File: LICENSE
+Keywords: data,migrate,migration,mysql,sqlite3,transfer
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Database
-Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
+Requires-Python: >=3.7
+Requires-Dist: click>=8.1.3
+Requires-Dist: mysql-connector-python!=8.0.30,!=8.0.31,>=8.0.18
+Requires-Dist: python-slugify>=7.0.0
+Requires-Dist: pytimeparse2
+Requires-Dist: simplejson>=3.19.0
+Requires-Dist: tabulate
+Requires-Dist: tqdm>=4.65.0
+Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 [![PyPI](https://img.shields.io/pypi/v/mysql-to-sqlite3)](https://pypi.org/project/mysql-to-sqlite3/)
 [![Downloads](https://pepy.tech/badge/mysql-to-sqlite3)](https://pepy.tech/project/mysql-to-sqlite3)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mysql-to-sqlite3)](https://pypi.org/project/mysql-to-sqlite3/)
 [![MySQL Support](https://img.shields.io/static/v1?label=MySQL&message=5.5+|+5.6+|+5.7+|+8.0&color=2b5d80)](https://img.shields.io/static/v1?label=MySQL&message=5.6+|+5.7+|+8.0&color=2b5d80)
-[![MariaDB Support](https://img.shields.io/static/v1?label=MariaDB&message=5.5+|+10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5+|+10.6&color=C0765A)](https://img.shields.io/static/v1?label=MariaDB&message=10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5&color=C0765A)
+[![MariaDB Support](https://img.shields.io/static/v1?label=MariaDB&message=5.5+|+10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5+|+10.6|+10.11&color=C0765A)](https://img.shields.io/static/v1?label=MariaDB&message=10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5&color=C0765A)
 [![GitHub license](https://img.shields.io/github/license/techouse/mysql-to-sqlite3)](https://github.com/techouse/mysql-to-sqlite3/blob/master/LICENSE)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE-OF-CONDUCT.md)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/64aae8e9599746d58d277852b35cc2bd)](https://www.codacy.com/manual/techouse/mysql-to-sqlite3?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=techouse/mysql-to-sqlite3&amp;utm_campaign=Badge_Grade)
 [![Build Status](https://github.com/techouse/mysql-to-sqlite3/workflows/Test/badge.svg)](https://github.com/techouse/mysql-to-sqlite3/actions?query=workflow%3ATest)
 [![codecov](https://codecov.io/gh/techouse/mysql-to-sqlite3/branch/master/graph/badge.svg)](https://codecov.io/gh/techouse/mysql-to-sqlite3)
 [![GitHub stars](https://img.shields.io/github/stars/techouse/mysql-to-sqlite3.svg?style=social&label=Star&maxAge=2592000)](https://github.com/techouse/mysql-to-sqlite3/stargazers)
@@ -70,38 +73,52 @@
   -d, --mysql-database TEXT       MySQL database name  [required]
   -u, --mysql-user TEXT           MySQL user  [required]
   -p, --prompt-mysql-password     Prompt for MySQL password
   --mysql-password TEXT           MySQL password
   -t, --mysql-tables TUPLE        Transfer only these specific tables (space
                                   separated table names). Implies --without-
                                   foreign-keys which inhibits the transfer of
-                                  foreign keys.
+                                  foreign keys. Can not be used together with
+                                  --exclude-mysql-tables.
+
+  -e, --exclude-mysql-tables TUPLE
+                                  Transfer all tables except these specific
+                                  tables (space separated table names).
+                                  Implies --without-foreign-keys which
+                                  inhibits the transfer of foreign keys. Can
+                                  not be used together with --mysql-tables.
+
   -L, --limit-rows INTEGER        Transfer only a limited number of rows from
                                   each table.
+
   -C, --collation [BINARY|NOCASE|RTRIM]
                                   Create datatypes of TEXT affinity using a
                                   specified collation sequence.  [default:
                                   BINARY]
+
   -K, --prefix-indices            Prefix indices with their corresponding
                                   tables. This ensures that their names remain
                                   unique across the SQLite database.
+
   -X, --without-foreign-keys      Do not transfer foreign keys.
+  -W, --without-data              Do not transfer table data, DDL only.
   -h, --mysql-host TEXT           MySQL host. Defaults to localhost.
   -P, --mysql-port INTEGER        MySQL port. Defaults to 3306.
   -S, --skip-ssl                  Disable MySQL connection encryption.
   -c, --chunk INTEGER             Chunk reading/writing SQL records
   -l, --log-file PATH             Log file
   --json-as-text                  Transfer JSON columns as TEXT.
   -V, --vacuum                    Use the VACUUM command to rebuild the SQLite
                                   database file, repacking it into a minimal
                                   amount of disk space
+
   --use-buffered-cursors          Use MySQLCursorBuffered for reading the
                                   MySQL database. This can be useful in
                                   situations where multiple queries, with
                                   small result sets, need to be combined or
                                   computed with each other.
+
   -q, --quiet                     Quiet. Display only errors.
+  --debug                         Debug mode. Will throw exceptions.
   --version                       Show the version and exit.
   --help                          Show this message and exit.
 ```
-
-
```

### Comparing `mysql-to-sqlite3-1.4.9/README.md` & `mysql_to_sqlite3-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![PyPI](https://img.shields.io/pypi/v/mysql-to-sqlite3)](https://pypi.org/project/mysql-to-sqlite3/)
 [![Downloads](https://pepy.tech/badge/mysql-to-sqlite3)](https://pepy.tech/project/mysql-to-sqlite3)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mysql-to-sqlite3)](https://pypi.org/project/mysql-to-sqlite3/)
 [![MySQL Support](https://img.shields.io/static/v1?label=MySQL&message=5.5+|+5.6+|+5.7+|+8.0&color=2b5d80)](https://img.shields.io/static/v1?label=MySQL&message=5.6+|+5.7+|+8.0&color=2b5d80)
-[![MariaDB Support](https://img.shields.io/static/v1?label=MariaDB&message=5.5+|+10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5+|+10.6&color=C0765A)](https://img.shields.io/static/v1?label=MariaDB&message=10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5&color=C0765A)
+[![MariaDB Support](https://img.shields.io/static/v1?label=MariaDB&message=5.5+|+10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5+|+10.6|+10.11&color=C0765A)](https://img.shields.io/static/v1?label=MariaDB&message=10.0+|+10.1+|+10.2+|+10.3+|+10.4+|+10.5&color=C0765A)
 [![GitHub license](https://img.shields.io/github/license/techouse/mysql-to-sqlite3)](https://github.com/techouse/mysql-to-sqlite3/blob/master/LICENSE)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE-OF-CONDUCT.md)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/64aae8e9599746d58d277852b35cc2bd)](https://www.codacy.com/manual/techouse/mysql-to-sqlite3?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=techouse/mysql-to-sqlite3&amp;utm_campaign=Badge_Grade)
 [![Build Status](https://github.com/techouse/mysql-to-sqlite3/workflows/Test/badge.svg)](https://github.com/techouse/mysql-to-sqlite3/actions?query=workflow%3ATest)
 [![codecov](https://codecov.io/gh/techouse/mysql-to-sqlite3/branch/master/graph/badge.svg)](https://codecov.io/gh/techouse/mysql-to-sqlite3)
 [![GitHub stars](https://img.shields.io/github/stars/techouse/mysql-to-sqlite3.svg?style=social&label=Star&maxAge=2592000)](https://github.com/techouse/mysql-to-sqlite3/stargazers)
@@ -37,36 +37,52 @@
   -d, --mysql-database TEXT       MySQL database name  [required]
   -u, --mysql-user TEXT           MySQL user  [required]
   -p, --prompt-mysql-password     Prompt for MySQL password
   --mysql-password TEXT           MySQL password
   -t, --mysql-tables TUPLE        Transfer only these specific tables (space
                                   separated table names). Implies --without-
                                   foreign-keys which inhibits the transfer of
-                                  foreign keys.
+                                  foreign keys. Can not be used together with
+                                  --exclude-mysql-tables.
+
+  -e, --exclude-mysql-tables TUPLE
+                                  Transfer all tables except these specific
+                                  tables (space separated table names).
+                                  Implies --without-foreign-keys which
+                                  inhibits the transfer of foreign keys. Can
+                                  not be used together with --mysql-tables.
+
   -L, --limit-rows INTEGER        Transfer only a limited number of rows from
                                   each table.
+
   -C, --collation [BINARY|NOCASE|RTRIM]
                                   Create datatypes of TEXT affinity using a
                                   specified collation sequence.  [default:
                                   BINARY]
+
   -K, --prefix-indices            Prefix indices with their corresponding
                                   tables. This ensures that their names remain
                                   unique across the SQLite database.
+
   -X, --without-foreign-keys      Do not transfer foreign keys.
+  -W, --without-data              Do not transfer table data, DDL only.
   -h, --mysql-host TEXT           MySQL host. Defaults to localhost.
   -P, --mysql-port INTEGER        MySQL port. Defaults to 3306.
   -S, --skip-ssl                  Disable MySQL connection encryption.
   -c, --chunk INTEGER             Chunk reading/writing SQL records
   -l, --log-file PATH             Log file
   --json-as-text                  Transfer JSON columns as TEXT.
   -V, --vacuum                    Use the VACUUM command to rebuild the SQLite
                                   database file, repacking it into a minimal
                                   amount of disk space
+
   --use-buffered-cursors          Use MySQLCursorBuffered for reading the
                                   MySQL database. This can be useful in
                                   situations where multiple queries, with
                                   small result sets, need to be combined or
                                   computed with each other.
+
   -q, --quiet                     Quiet. Display only errors.
+  --debug                         Debug mode. Will throw exceptions.
   --version                       Show the version and exit.
   --help                          Show this message and exit.
 ```
```

### Comparing `mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/click_utils.py` & `mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/click_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """Click utilities."""
 
+import typing as t
+
 import click
 
 
 class OptionEatAll(click.Option):
     """Taken from https://stackoverflow.com/questions/48391777/nargs-equivalent-for-options-in-click#answer-48394004."""  # noqa: ignore=E501 pylint: disable=C0301
 
     def __init__(self, *args, **kwargs):
         """Override."""
         self.save_other_options = kwargs.pop("save_other_options", True)
         nargs = kwargs.pop("nargs", -1)
         if nargs != -1:
-            raise ValueError("nargs, if set, must be -1 not {}".format(nargs))
+            raise ValueError(f"nargs, if set, must be -1 not {nargs}")
         super(OptionEatAll, self).__init__(*args, **kwargs)
         self._previous_parser_process = None
         self._eat_all_parser = None
 
-    def add_to_parser(self, parser, ctx):
+    def add_to_parser(self, parser, ctx) -> None:
         """Override."""
 
         def parser_process(value, state):
             # method to hook to the parser.process
             done = False
             value = [value]
             if self.save_other_options:
@@ -36,36 +38,34 @@
                 value += state.rargs
                 state.rargs[:] = []
             value = tuple(value)
 
             # call the actual process
             self._previous_parser_process(value, state)
 
-        retval = super(OptionEatAll, self).add_to_parser(  # pylint: disable=E1111
-            parser, ctx
-        )
+        retval = super(OptionEatAll, self).add_to_parser(parser, ctx)  # pylint: disable=E1111
         for name in self.opts:
             # pylint: disable=W0212
             our_parser = parser._long_opt.get(name) or parser._short_opt.get(name)
             if our_parser:
                 self._eat_all_parser = our_parser
                 self._previous_parser_process = our_parser.process
                 our_parser.process = parser_process
                 break
         return retval
 
 
-def prompt_password(ctx, param, use_password):  # pylint: disable=W0613
+def prompt_password(ctx: click.core.Context, param: t.Any, use_password: bool):  # pylint: disable=W0613
     """Prompt for password."""
     if use_password:
         mysql_password = ctx.params.get("mysql_password")
         if not mysql_password:
             mysql_password = click.prompt("MySQL password", hide_input=True)
 
         return mysql_password
 
 
-def validate_positive_integer(ctx, param, value):  # pylint: disable=W0613
+def validate_positive_integer(ctx: click.core.Context, param: t.Any, value: int):  # pylint: disable=W0613
     """Allow only positive integers and 0."""
     if value < 0:
         raise click.BadParameter("Should be a positive integer or 0.")
     return value
```

### Comparing `mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/debug_info.py` & `mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/debug_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,103 +1,93 @@
 """Module containing bug report helper(s).
 
 Adapted from https://github.com/psf/requests/blob/master/requests/help.py
 """
 
-from __future__ import print_function
-
 import platform
 import sqlite3
 import sys
-from distutils.spawn import find_executable
+import typing as t
+from distutils.spawn import find_executable  # pylint: disable=W0402
 from subprocess import check_output
 
 import click
 import mysql.connector
-import pytimeparse
+import pytimeparse2
 import simplejson
-import six
 import slugify
 import tabulate
 import tqdm
 
 from . import __version__ as package_version
 
 
-def _implementation():
+def _implementation() -> str:
     """Return a dict with the Python implementation and version.
 
     Provide both the name and the version of the Python implementation
     currently running. For example, on CPython 2.7.5 it will return
     {'name': 'CPython', 'version': '2.7.5'}.
 
     This function works best on CPython and PyPy: in particular, it probably
     doesn't work for Jython or IronPython. Future investigation should be done
     to work out the correct shape of the code for those platforms.
     """
-    implementation = platform.python_implementation()
+    implementation: str = platform.python_implementation()
 
     if implementation == "CPython":
         implementation_version = platform.python_version()
     elif implementation == "PyPy":
         implementation_version = "%s.%s.%s" % (
-            sys.pypy_version_info.major,  # noqa: ignore=E1101 pylint: disable=E1101
-            sys.pypy_version_info.minor,  # noqa: ignore=E1101 pylint: disable=E1101
-            sys.pypy_version_info.micro,  # noqa: ignore=E1101 pylint: disable=E1101
-        )
-        rel = (
-            sys.pypy_version_info.releaselevel  # noqa: ignore=E1101 pylint: disable=E1101
+            sys.pypy_version_info.major,  # type: ignore # noqa: ignore=E1101 pylint: disable=E1101
+            sys.pypy_version_info.minor,  # type: ignore # noqa: ignore=E1101 pylint: disable=E1101
+            sys.pypy_version_info.micro,  # type: ignore # noqa: ignore=E1101 pylint: disable=E1101
         )
+        rel = sys.pypy_version_info.releaselevel  # type: ignore # noqa: ignore=E1101 pylint: disable=E1101
         if rel != "final":
             implementation_version = "".join([implementation_version, rel])
     elif implementation == "Jython":
         implementation_version = platform.python_version()  # Complete Guess
     elif implementation == "IronPython":
         implementation_version = platform.python_version()  # Complete Guess
     else:
         implementation_version = "Unknown"
 
-    return "{implementation} {implementation_version}".format(
-        implementation=implementation, implementation_version=implementation_version
-    )
+    return f"{implementation} {implementation_version}"
 
 
-def _mysql_version():
+def _mysql_version() -> str:
     if find_executable("mysql"):
         try:
-            mysql_version = check_output(["mysql", "-V"])
+            mysql_version: t.Union[str, bytes] = check_output(["mysql", "-V"])
             try:
-                return mysql_version.decode().strip()
+                return mysql_version.decode().strip()  # type: ignore
             except (UnicodeDecodeError, AttributeError):
-                return mysql_version
+                return str(mysql_version)
         except Exception:  # nosec pylint: disable=W0703
             pass
     return "MySQL client not found on the system"
 
 
-def info():
+def info() -> t.List[t.List[str]]:
     """Generate information for a bug report."""
     try:
-        platform_info = "{system} {release}".format(
-            system=platform.system(),
-            release=platform.release(),
-        )
+        platform_info: str = f"{platform.system()} {platform.release()}"
     except IOError:
         platform_info = "Unknown"
 
     return [
-        ["mysql-to-sqlite3", package_version.__version__],
+        ["mysql-to-sqlite3", package_version],
         ["", ""],
         ["Operating System", platform_info],
         ["Python", _implementation()],
         ["MySQL", _mysql_version()],
         ["SQLite", sqlite3.sqlite_version],
         ["", ""],
         ["click", click.__version__],
         ["mysql-connector-python", mysql.connector.__version__],
         ["python-slugify", slugify.__version__],
-        ["pytimeparse", pytimeparse.__version__],
-        ["simplejson", simplejson.__version__],
-        ["six", six.__version__],
+        ["pytimeparse2", pytimeparse2.__version__],
+        ["simplejson", simplejson.__version__],  # type: ignore
         ["tabulate", tabulate.__version__],
         ["tqdm", tqdm.__version__],
     ]
```

### Comparing `mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/sqlite_utils.py` & `mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/sqlite_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 """SQLite adapters and converters for unsupported data types."""
 
-from __future__ import division
-
 import sqlite3
-from datetime import timedelta
+import typing as t
+from datetime import date, timedelta
 from decimal import Decimal
 
-from pytimeparse.timeparse import timeparse
+from pytimeparse2 import parse
 
 
-def adapt_decimal(value):
+def adapt_decimal(value: t.Any) -> str:
     """Convert decimal.Decimal to string."""
     return str(value)
 
 
-def convert_decimal(value):
-    """Convert string to decimalDecimal."""
+def convert_decimal(value: t.Any) -> Decimal:
+    """Convert string to decimal.Decimal."""
     return Decimal(value)
 
 
-def adapt_timedelta(value):
+def adapt_timedelta(value: t.Any) -> str:
     """Convert datetime.timedelta to %H:%M:%S string."""
     hours, remainder = divmod(value.total_seconds(), 3600)
     minutes, seconds = divmod(remainder, 60)
     return "{:02}:{:02}:{:02}".format(int(hours), int(minutes), int(seconds))
 
 
-def convert_timedelta(value):
+def convert_timedelta(value: t.Any) -> timedelta:
     """Convert %H:%M:%S string to datetime.timedelta."""
-    return timedelta(seconds=timeparse(value))
+    return timedelta(seconds=parse(value))
 
 
-def encode_data_for_sqlite(value):
+def encode_data_for_sqlite(value: t.Any) -> t.Any:
     """Fix encoding bytes."""
     try:
         return value.decode()
     except (UnicodeDecodeError, AttributeError):
         return sqlite3.Binary(value)
 
 
 class CollatingSequences:
     """Taken from https://www.sqlite.org/datatype3.html#collating_sequences."""
 
-    BINARY = "BINARY"
-    NOCASE = "NOCASE"
-    RTRIM = "RTRIM"
+    BINARY: str = "BINARY"
+    NOCASE: str = "NOCASE"
+    RTRIM: str = "RTRIM"
+
+
+def convert_date(value: t.Any) -> date:
+    """Handle SQLite date conversion."""
+    try:
+        return date.fromisoformat(value.decode())
+    except ValueError as err:
+        raise ValueError(f"DATE field contains {err}")  # pylint: disable=W0707
```

### Comparing `mysql-to-sqlite3-1.4.9/mysql_to_sqlite3/transporter.py` & `mysql_to_sqlite3-2.0.0/mysql_to_sqlite3/transporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,137 +1,141 @@
 """Use to transfer a MySQL database to SQLite."""
 
-from __future__ import division
-
 import logging
+import os
 import re
 import sqlite3
+import typing as t
 from datetime import timedelta
 from decimal import Decimal
 from math import ceil
 from os.path import realpath
 from sys import stdout
 
 import mysql.connector
-import six
-from mysql.connector import errorcode
+import typing_extensions as tx
+from mysql.connector import CMySQLConnection, MySQLConnection, errorcode
+from mysql.connector.types import ToPythonOutputTypes
 from tqdm import tqdm, trange
 
 from mysql_to_sqlite3.sqlite_utils import (
     CollatingSequences,
     adapt_decimal,
     adapt_timedelta,
+    convert_date,
     convert_decimal,
     convert_timedelta,
     encode_data_for_sqlite,
 )
-
-if six.PY2:
-    from .sixeptions import *  # pylint: disable=W0401
+from mysql_to_sqlite3.types import MySQLtoSQLiteAttributes, MySQLtoSQLiteParams
 
 
-class MySQLtoSQLite:
+class MySQLtoSQLite(MySQLtoSQLiteAttributes):
     """Use this class to transfer a MySQL database to SQLite."""
 
-    COLUMN_PATTERN = re.compile(r"^[^(]+")
-    COLUMN_LENGTH_PATTERN = re.compile(r"\(\d+\)$")
+    COLUMN_PATTERN: t.Pattern[str] = re.compile(r"^[^(]+")
+    COLUMN_LENGTH_PATTERN: t.Pattern[str] = re.compile(r"\(\d+\)$")
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs: tx.Unpack[MySQLtoSQLiteParams]) -> None:
         """Constructor."""
-        if not kwargs.get("mysql_database"):
+        if kwargs.get("mysql_database") is not None:
+            self._mysql_database = str(kwargs.get("mysql_database"))
+        else:
             raise ValueError("Please provide a MySQL database")
 
-        if not kwargs.get("mysql_user"):
+        if kwargs.get("mysql_user") is not None:
+            self._mysql_user = str(kwargs.get("mysql_user"))
+        else:
             raise ValueError("Please provide a MySQL user")
 
-        self._mysql_database = str(kwargs.get("mysql_database"))
+        if kwargs.get("sqlite_file") is None:
+            raise ValueError("Please provide an SQLite file")
+        else:
+            self._sqlite_file = realpath(str(kwargs.get("sqlite_file")))
 
-        self._mysql_tables = (
-            tuple(kwargs.get("mysql_tables"))
-            if kwargs.get("mysql_tables") is not None
-            else tuple()
-        )
+        self._mysql_password = str(kwargs.get("mysql_password")) or None
+
+        self._mysql_host = kwargs.get("mysql_host") or "localhost"
+
+        self._mysql_port = kwargs.get("mysql_port") or 3306
+
+        self._mysql_tables = kwargs.get("mysql_tables") or tuple()
 
-        self._limit_rows = int(kwargs.get("limit_rows") or 0)
+        self._exclude_mysql_tables = kwargs.get("exclude_mysql_tables") or tuple()
 
-        if kwargs.get("collation") is not None and kwargs.get("collation").upper() in {
+        if len(self._mysql_tables) > 0 and len(self._exclude_mysql_tables) > 0:
+            raise ValueError("mysql_tables and exclude_mysql_tables are mutually exclusive")
+
+        self._limit_rows = kwargs.get("limit_rows") or 0
+
+        if kwargs.get("collation") is not None and str(kwargs.get("collation")).upper() in {
             CollatingSequences.BINARY,
             CollatingSequences.NOCASE,
             CollatingSequences.RTRIM,
         }:
-            self._collation = kwargs.get("collation").upper()
+            self._collation = str(kwargs.get("collation")).upper()
         else:
             self._collation = CollatingSequences.BINARY
 
         self._prefix_indices = kwargs.get("prefix_indices") or False
 
-        self._without_foreign_keys = (
-            True
-            if len(self._mysql_tables) > 0
-            else (kwargs.get("without_foreign_keys") or False)
-        )
-
-        self._mysql_user = str(kwargs.get("mysql_user"))
-
-        self._mysql_password = (
-            str(kwargs.get("mysql_password")) if kwargs.get("mysql_password") else None
-        )
-
-        self._mysql_host = str(kwargs.get("mysql_host") or "localhost")
+        if len(self._mysql_tables) > 0 or len(self._exclude_mysql_tables) > 0:
+            self._without_foreign_keys = True
+        else:
+            self._without_foreign_keys = kwargs.get("without_foreign_keys") or False
 
-        self._mysql_port = int(kwargs.get("mysql_port") or 3306)
+        self._without_data = kwargs.get("without_data") or False
 
         self._mysql_ssl_disabled = kwargs.get("mysql_ssl_disabled") or False
 
         self._current_chunk_number = 0
-        self._chunk_size = int(kwargs.get("chunk")) if kwargs.get("chunk") else None
 
-        self._sqlite_file = kwargs.get("sqlite_file") or None
+        self._chunk_size = kwargs.get("chunk") or None
 
         self._buffered = kwargs.get("buffered") or False
 
         self._vacuum = kwargs.get("vacuum") or False
 
         self._quiet = kwargs.get("quiet") or False
 
-        self._logger = self._setup_logger(
-            log_file=kwargs.get("log_file") or None, quiet=self._quiet
-        )
+        self._logger = self._setup_logger(log_file=kwargs.get("log_file") or None, quiet=self._quiet)
 
         sqlite3.register_adapter(Decimal, adapt_decimal)
         sqlite3.register_converter("DECIMAL", convert_decimal)
         sqlite3.register_adapter(timedelta, adapt_timedelta)
+        sqlite3.register_converter("DATE", convert_date)
         sqlite3.register_converter("TIME", convert_timedelta)
 
-        self._sqlite = sqlite3.connect(
-            realpath(self._sqlite_file), detect_types=sqlite3.PARSE_DECLTYPES
-        )
+        self._sqlite = sqlite3.connect(realpath(self._sqlite_file), detect_types=sqlite3.PARSE_DECLTYPES)
         self._sqlite.row_factory = sqlite3.Row
 
         self._sqlite_cur = self._sqlite.cursor()
 
         self._json_as_text = kwargs.get("json_as_text") or False
-        self._sqlite_json1_extension_enabled = (
-            not self._json_as_text and self._check_sqlite_json1_extension_enabled()
-        )
+
+        self._sqlite_json1_extension_enabled = not self._json_as_text and self._check_sqlite_json1_extension_enabled()
 
         try:
-            self._mysql = mysql.connector.connect(
+            _mysql_connection = mysql.connector.connect(
                 user=self._mysql_user,
                 password=self._mysql_password,
                 host=self._mysql_host,
                 port=self._mysql_port,
                 ssl_disabled=self._mysql_ssl_disabled,
             )
+            if isinstance(_mysql_connection, (MySQLConnection, CMySQLConnection)):
+                self._mysql = _mysql_connection
+            else:
+                raise ConnectionError("Unable to connect to MySQL")
             if not self._mysql.is_connected():
                 raise ConnectionError("Unable to connect to MySQL")
 
-            self._mysql_cur = self._mysql.cursor(buffered=self._buffered, raw=True)
-            self._mysql_cur_prepared = self._mysql.cursor(prepared=True)
-            self._mysql_cur_dict = self._mysql.cursor(
+            self._mysql_cur = self._mysql.cursor(buffered=self._buffered, raw=True)  # type: ignore[assignment]
+            self._mysql_cur_prepared = self._mysql.cursor(prepared=True)  # type: ignore[assignment]
+            self._mysql_cur_dict = self._mysql.cursor(  # type: ignore[assignment]
                 buffered=self._buffered,
                 dictionary=True,
             )
             try:
                 self._mysql.database = self._mysql_database
             except (mysql.connector.Error, Exception) as err:
                 if hasattr(err, "errno") and err.errno == errorcode.ER_BAD_DB_ERROR:
@@ -140,19 +144,21 @@
                 self._logger.error(err)
                 raise
         except mysql.connector.Error as err:
             self._logger.error(err)
             raise
 
     @classmethod
-    def _setup_logger(cls, log_file=None, quiet=False):
-        formatter = logging.Formatter(
+    def _setup_logger(
+        cls, log_file: t.Optional[t.Union[str, "os.PathLike[t.Any]"]] = None, quiet: bool = False
+    ) -> logging.Logger:
+        formatter: logging.Formatter = logging.Formatter(
             fmt="%(asctime)s %(levelname)-8s %(message)s", datefmt="%Y-%m-%d %H:%M:%S"
         )
-        logger = logging.getLogger(cls.__name__)
+        logger: logging.Logger = logging.getLogger(cls.__name__)
         logger.setLevel(logging.DEBUG)
 
         if not quiet:
             screen_handler = logging.StreamHandler(stream=stdout)
             screen_handler.setFormatter(formatter)
             logger.addHandler(screen_handler)
 
@@ -160,40 +166,47 @@
             file_handler = logging.FileHandler(realpath(log_file), mode="w")
             file_handler.setFormatter(formatter)
             logger.addHandler(file_handler)
 
         return logger
 
     @classmethod
-    def _valid_column_type(cls, column_type):
+    def _valid_column_type(cls, column_type: str) -> t.Optional[t.Match[str]]:
         return cls.COLUMN_PATTERN.match(column_type.strip())
 
     @classmethod
-    def _column_type_length(cls, column_type):
-        suffix = cls.COLUMN_LENGTH_PATTERN.search(column_type)
+    def _column_type_length(cls, column_type: str) -> str:
+        suffix: t.Optional[t.Match[str]] = cls.COLUMN_LENGTH_PATTERN.search(column_type)
         if suffix:
             return suffix.group(0)
         return ""
 
+    @staticmethod
+    def _decode_column_type(column_type: t.Union[str, bytes]) -> str:
+        if isinstance(column_type, str):
+            return column_type
+        if isinstance(column_type, bytes):
+            try:
+                return column_type.decode()
+            except (UnicodeDecodeError, AttributeError):
+                pass
+        return str(column_type)
+
     @classmethod
     def _translate_type_from_mysql_to_sqlite(
-        cls, column_type, sqlite_json1_extension_enabled=False
-    ):
-        """Handle MySQL 8."""
-        try:
-            column_type = column_type.decode()
-        except (UnicodeDecodeError, AttributeError):
-            pass
+        cls, column_type: t.Union[str, bytes], sqlite_json1_extension_enabled=False
+    ) -> str:
+        _column_type: str = cls._decode_column_type(column_type)
 
         # This could be optimized even further, however is seems adequate.
-        match = cls._valid_column_type(column_type)
+        match: t.Optional[t.Match[str]] = cls._valid_column_type(_column_type)
         if not match:
             raise ValueError("Invalid column_type!")
 
-        data_type = match.group(0).upper()
+        data_type: str = match.group(0).upper()
 
         if data_type.endswith(" UNSIGNED"):
             data_type = data_type.replace(" UNSIGNED", "")
 
         if data_type in {
             "BIGINT",
             "BLOB",
@@ -219,103 +232,105 @@
             "LONGBLOB",
             "MEDIUMBLOB",
             "TINYBLOB",
             "VARBINARY",
         }:
             return "BLOB"
         if data_type in {"NCHAR", "NVARCHAR", "VARCHAR"}:
-            return data_type + cls._column_type_length(column_type)
+            return data_type + cls._column_type_length(_column_type)
         if data_type == "CHAR":
-            return "CHARACTER" + cls._column_type_length(column_type)
+            return "CHARACTER" + cls._column_type_length(_column_type)
         if data_type == "INT":
             return "INTEGER"
         if data_type in "TIMESTAMP":
             return "DATETIME"
         if data_type == "JSON" and sqlite_json1_extension_enabled:
             return "JSON"
         return "TEXT"
 
     @classmethod
     def _translate_default_from_mysql_to_sqlite(
-        cls, column_default=None, column_type=None
-    ):
-        try:
-            column_default = column_default.decode()
-        except (UnicodeDecodeError, AttributeError):
-            pass
-
+        cls, column_default: t.Optional[t.Any] = None, column_type: t.Optional[str] = None
+    ) -> str:
+        if isinstance(column_default, bytes):
+            if column_type in {
+                "BIT",
+                "BINARY",
+                "BLOB",
+                "LONGBLOB",
+                "MEDIUMBLOB",
+                "TINYBLOB",
+                "VARBINARY",
+            }:
+                return f"DEFAULT x'{column_default.hex()}'"
+            try:
+                column_default = column_default.decode()
+            except (UnicodeDecodeError, AttributeError):
+                pass
         if column_default is None:
             return ""
         if isinstance(column_default, bool):
             if column_type == "BOOLEAN" and sqlite3.sqlite_version >= "3.23.0":
                 if column_default:
                     return "DEFAULT(TRUE)"
                 return "DEFAULT(FALSE)"
-            return "DEFAULT '{}'".format(int(column_default))
-        if (
-            six.PY2
-            and isinstance(
-                column_default, unicode  # noqa: ignore=F405 pylint: disable=E0602
-            )
-        ) or isinstance(column_default, str):
+            return f"DEFAULT '{int(column_default)}'"
+        if isinstance(column_default, str):
             if column_default.upper() in {
                 "CURRENT_TIME",
                 "CURRENT_DATE",
                 "CURRENT_TIMESTAMP",
             }:
-                return "DEFAULT {}".format(column_default.upper())
-        return "DEFAULT '{}'".format(column_default)
+                return f"DEFAULT {column_default.upper()}"
+        return f"DEFAULT '{str(column_default)}'"
 
     @classmethod
     def _data_type_collation_sequence(
-        cls, collation=CollatingSequences.BINARY, column_type=None
-    ):
+        cls, collation: str = CollatingSequences.BINARY, column_type: t.Optional[str] = None
+    ) -> str:
         if column_type and collation != CollatingSequences.BINARY:
             if column_type.startswith(
                 (
                     "CHARACTER",
                     "NCHAR",
                     "NVARCHAR",
                     "TEXT",
                     "VARCHAR",
                 )
             ):
-                return "COLLATE {collation}".format(collation=collation)
+                return f"COLLATE {collation}"
         return ""
 
-    def _check_sqlite_json1_extension_enabled(self):
+    def _check_sqlite_json1_extension_enabled(self) -> bool:
         try:
             self._sqlite_cur.execute("PRAGMA compile_options")
             return "ENABLE_JSON1" in set(row[0] for row in self._sqlite_cur.fetchall())
         except sqlite3.Error:
             return False
 
-    def _build_create_table_sql(self, table_name):
-        sql = 'CREATE TABLE IF NOT EXISTS "{}" ('.format(table_name)
-        primary = ""
-        indices = ""
+    def _build_create_table_sql(self, table_name: str) -> str:
+        sql: str = f'CREATE TABLE IF NOT EXISTS "{table_name}" ('
+        primary: str = ""
+        indices: str = ""
 
-        self._mysql_cur_dict.execute("SHOW COLUMNS FROM `{}`".format(table_name))
+        self._mysql_cur_dict.execute(f"SHOW COLUMNS FROM `{table_name}`")
 
         for row in self._mysql_cur_dict.fetchall():
-            column_type = self._translate_type_from_mysql_to_sqlite(
-                column_type=row["Type"],
-                sqlite_json1_extension_enabled=self._sqlite_json1_extension_enabled,
-            )
-            sql += '\n\t"{name}" {type} {notnull} {default} {collation},'.format(
-                name=row["Field"],
-                type=column_type,
-                notnull="NULL" if row["Null"] == "YES" else "NOT NULL",
-                default=self._translate_default_from_mysql_to_sqlite(
-                    row["Default"], column_type
-                ),
-                collation=self._data_type_collation_sequence(
-                    self._collation, column_type
-                ),
-            )
+            if row is not None:
+                column_type = self._translate_type_from_mysql_to_sqlite(
+                    column_type=row["Type"],  # type: ignore[arg-type]
+                    sqlite_json1_extension_enabled=self._sqlite_json1_extension_enabled,
+                )
+                sql += '\n\t"{name}" {type} {notnull} {default} {collation},'.format(
+                    name=row["Field"].decode() if isinstance(row["Field"], bytes) else row["Field"],
+                    type=column_type,
+                    notnull="NULL" if row["Null"] == "YES" else "NOT NULL",
+                    default=self._translate_default_from_mysql_to_sqlite(row["Default"], column_type),
+                    collation=self._data_type_collation_sequence(self._collation, column_type),
+                )
 
         self._mysql_cur_dict.execute(
             """
             SELECT INDEX_NAME AS `name`,
                   IF (NON_UNIQUE = 0 AND INDEX_NAME = 'PRIMARY', 1, 0) AS `primary`,
                   IF (NON_UNIQUE = 0 AND INDEX_NAME <> 'PRIMARY', 1, 0) AS `unique`,
                   GROUP_CONCAT(COLUMN_NAME ORDER BY SEQ_IN_INDEX) AS `columns`
@@ -323,37 +338,46 @@
             WHERE TABLE_SCHEMA = %s
             AND TABLE_NAME = %s
             GROUP BY INDEX_NAME, NON_UNIQUE
             """,
             (self._mysql_database, table_name),
         )
         for index in self._mysql_cur_dict.fetchall():
-            if int(index["primary"]) == 1:
-                primary += "\n\tPRIMARY KEY ({columns})".format(
-                    columns=", ".join(
-                        '"{}"'.format(column) for column in index["columns"].split(",")
-                    )
-                )
-            else:
-                indices += """CREATE {unique} INDEX IF NOT EXISTS "{name}" ON "{table}" ({columns});""".format(
-                    unique="UNIQUE" if int(index["unique"]) == 1 else "",
-                    name="{table}_{name}".format(table=table_name, name=index["name"])
-                    if self._prefix_indices
-                    else index["name"],
-                    table=table_name,
-                    columns=", ".join(
-                        '"{}"'.format(column) for column in index["columns"].split(",")
-                    ),
-                )
+            if index is not None:
+                columns: str = ""
+                if isinstance(index["columns"], bytes):
+                    columns = index["columns"].decode()
+                elif isinstance(index["columns"], str):
+                    columns = index["columns"]
+
+                if len(columns) > 0:
+                    if index["primary"] in {1, "1"}:
+                        primary += "\n\tPRIMARY KEY ({})".format(
+                            ", ".join(f'"{column}"' for column in columns.split(","))
+                        )
+                    else:
+                        indices += """CREATE {unique} INDEX IF NOT EXISTS "{name}" ON "{table}" ({columns});""".format(
+                            unique="UNIQUE" if index["unique"] in {1, "1"} else "",
+                            name="{table}_{name}".format(
+                                table=table_name,
+                                name=index["name"].decode() if isinstance(index["name"], bytes) else index["name"],
+                            )
+                            if self._prefix_indices
+                            else index["name"].decode()
+                            if isinstance(index["name"], bytes)
+                            else index["name"],
+                            table=table_name,
+                            columns=", ".join(f'"{column}"' for column in columns.split(",")),
+                        )
 
         sql += primary
         sql = sql.rstrip(", ")
 
         if not self._without_foreign_keys:
-            server_version = self._mysql.get_server_version()
+            server_version: t.Tuple[int, ...] = self._mysql.get_server_version()
             self._mysql_cur_dict.execute(
                 """
                 SELECT k.COLUMN_NAME AS `column`,
                        k.REFERENCED_TABLE_NAME AS `ref_table`,
                        k.REFERENCED_COLUMN_NAME AS `ref_column`,
                        c.UPDATE_RULE AS `on_update`,
                        c.DELETE_RULE AS `on_delete`
@@ -368,114 +392,100 @@
                 GROUP BY i.CONSTRAINT_NAME,
                          k.COLUMN_NAME,
                          k.REFERENCED_TABLE_NAME,
                          k.REFERENCED_COLUMN_NAME,
                          c.UPDATE_RULE,
                          c.DELETE_RULE
                 """.format(
-                    JOIN="JOIN"
-                    if (server_version[0] == 8 and server_version[2] > 19)
-                    else "LEFT JOIN"
+                    JOIN="JOIN" if (server_version[0] == 8 and server_version[2] > 19) else "LEFT JOIN"
                 ),
                 (self._mysql_database, table_name, "FOREIGN KEY"),
             )
             for foreign_key in self._mysql_cur_dict.fetchall():
-                sql += """,\n\tFOREIGN KEY("{column}") REFERENCES "{ref_table}" ("{ref_column}") ON UPDATE {on_update} ON DELETE {on_delete}""".format(
-                    **foreign_key
-                )
+                if foreign_key is not None:
+                    sql += (
+                        ',\n\tFOREIGN KEY("{column}") REFERENCES "{ref_table}" ("{ref_column}") '
+                        "ON UPDATE {on_update} "
+                        "ON DELETE {on_delete}".format(**foreign_key)  # type: ignore[str-bytes-safe]
+                    )
 
         sql += "\n);"
         sql += indices
+
         return sql
 
-    def _create_table(self, table_name, attempting_reconnect=False):
+    def _create_table(self, table_name: str, attempting_reconnect: bool = False) -> None:
         try:
             if attempting_reconnect:
                 self._mysql.reconnect()
             self._sqlite_cur.executescript(self._build_create_table_sql(table_name))
             self._sqlite.commit()
         except mysql.connector.Error as err:
             if err.errno == errorcode.CR_SERVER_LOST:
                 if not attempting_reconnect:
-                    self._logger.warning(
-                        "Connection to MySQL server lost." "\nAttempting to reconnect."
-                    )
+                    self._logger.warning("Connection to MySQL server lost.\nAttempting to reconnect.")
                     self._create_table(table_name, True)
                 else:
-                    self._logger.warning(
-                        "Connection to MySQL server lost."
-                        "\nReconnection attempt aborted."
-                    )
+                    self._logger.warning("Connection to MySQL server lost.\nReconnection attempt aborted.")
                     raise
             self._logger.error(
                 "MySQL failed reading table definition from table %s: %s",
                 table_name,
                 err,
             )
             raise
         except sqlite3.Error as err:
             self._logger.error("SQLite failed creating table %s: %s", table_name, err)
             raise
 
     def _transfer_table_data(
-        self, table_name, sql, total_records=0, attempting_reconnect=False
-    ):
+        self, table_name: str, sql: str, total_records: int = 0, attempting_reconnect: bool = False
+    ) -> None:
         if attempting_reconnect:
             self._mysql.reconnect()
         try:
             if self._chunk_size is not None and self._chunk_size > 0:
                 for chunk in trange(
                     self._current_chunk_number,
                     int(ceil(total_records / self._chunk_size)),
                     disable=self._quiet,
                 ):
                     self._current_chunk_number = chunk
                     self._sqlite_cur.executemany(
                         sql,
                         (
-                            tuple(
-                                encode_data_for_sqlite(col) if col is not None else None
-                                for col in row
-                            )
+                            tuple(encode_data_for_sqlite(col) if col is not None else None for col in row)
                             for row in self._mysql_cur.fetchmany(self._chunk_size)
                         ),
                     )
             else:
                 self._sqlite_cur.executemany(
                     sql,
                     (
-                        tuple(
-                            encode_data_for_sqlite(col) if col is not None else None
-                            for col in row
-                        )
+                        tuple(encode_data_for_sqlite(col) if col is not None else None for col in row)
                         for row in tqdm(
                             self._mysql_cur.fetchall(),
                             total=total_records,
                             disable=self._quiet,
                         )
                     ),
                 )
             self._sqlite.commit()
         except mysql.connector.Error as err:
             if err.errno == errorcode.CR_SERVER_LOST:
                 if not attempting_reconnect:
-                    self._logger.warning(
-                        "Connection to MySQL server lost." "\nAttempting to reconnect."
-                    )
+                    self._logger.warning("Connection to MySQL server lost.\nAttempting to reconnect.")
                     self._transfer_table_data(
                         table_name=table_name,
                         sql=sql,
                         total_records=total_records,
                         attempting_reconnect=True,
                     )
                 else:
-                    self._logger.warning(
-                        "Connection to MySQL server lost."
-                        "\nReconnection attempt aborted."
-                    )
+                    self._logger.warning("Connection to MySQL server lost.\nReconnection attempt aborted.")
                     raise
             self._logger.error(
                 "MySQL transfer failed reading table data from table %s: %s",
                 table_name,
                 err,
             )
             raise
@@ -483,105 +493,113 @@
             self._logger.error(
                 "SQLite transfer failed inserting data into table %s: %s",
                 table_name,
                 err,
             )
             raise
 
-    def transfer(self):
+    def transfer(self) -> None:
         """The primary and only method with which we transfer all the data."""
-        if len(self._mysql_tables) > 0:
+        if len(self._mysql_tables) > 0 or len(self._exclude_mysql_tables) > 0:
             # transfer only specific tables
+            specific_tables: t.Sequence[str] = (
+                self._exclude_mysql_tables if len(self._exclude_mysql_tables) > 0 else self._mysql_tables
+            )
 
             self._mysql_cur_prepared.execute(
                 """
                 SELECT TABLE_NAME
                 FROM information_schema.TABLES
                 WHERE TABLE_SCHEMA = SCHEMA()
-                AND TABLE_NAME IN ({placeholders})
+                AND TABLE_NAME {exclude} IN ({placeholders})
             """.format(
-                    placeholders=("%s, " * len(self._mysql_tables)).rstrip(" ,")
+                    exclude="NOT" if len(self._exclude_mysql_tables) > 0 else "",
+                    placeholders=("%s, " * len(specific_tables)).rstrip(" ,"),
                 ),
-                self._mysql_tables,
+                specific_tables,
             )
-            tables = (row[0] for row in self._mysql_cur_prepared.fetchall())
+            tables: t.Iterable[ToPythonOutputTypes] = (row[0] for row in self._mysql_cur_prepared.fetchall())
         else:
             # transfer all tables
             self._mysql_cur.execute(
                 """
                 SELECT TABLE_NAME
                 FROM information_schema.TABLES
                 WHERE TABLE_SCHEMA = SCHEMA()
             """
             )
-            tables = (row[0].decode() for row in self._mysql_cur.fetchall())
+            tables = (row[0].decode() for row in self._mysql_cur.fetchall())  # type: ignore[union-attr]
 
         try:
             # turn off foreign key checking in SQLite while transferring data
             self._sqlite_cur.execute("PRAGMA foreign_keys=OFF")
 
             for table_name in tables:
+                if isinstance(table_name, bytes):
+                    table_name = table_name.decode()
+
+                self._logger.info(
+                    "%sTransferring table %s",
+                    "[WITHOUT DATA] " if self._without_data else "",
+                    table_name,
+                )
+
                 # reset the chunk
                 self._current_chunk_number = 0
 
                 # create the table
-                self._create_table(table_name)
+                self._create_table(table_name)  # type: ignore[arg-type]
 
-                # get the size of the data
-                if self._limit_rows > 0:
-                    # limit to the requested number of rows
-                    self._mysql_cur_dict.execute(
-                        """
-                            SELECT COUNT(*) AS `total_records`
-                            FROM (SELECT * FROM `{table_name}` LIMIT {limit}) AS `table`
-                        """.format(
-                            table_name=table_name, limit=self._limit_rows
+                if not self._without_data:
+                    # get the size of the data
+                    if self._limit_rows > 0:
+                        # limit to the requested number of rows
+                        self._mysql_cur_dict.execute(
+                            "SELECT COUNT(*) AS `total_records` "
+                            f"FROM (SELECT * FROM `{table_name}` LIMIT {self._limit_rows}) AS `table`"
                         )
-                    )
-                else:
-                    # get all rows
-                    self._mysql_cur_dict.execute(
-                        "SELECT COUNT(*) AS `total_records` FROM `{table_name}`".format(
-                            table_name=table_name
+                    else:
+                        # get all rows
+                        self._mysql_cur_dict.execute(f"SELECT COUNT(*) AS `total_records` FROM `{table_name}`")
+
+                    total_records: t.Optional[t.Dict[str, ToPythonOutputTypes]] = self._mysql_cur_dict.fetchone()
+                    if total_records is not None:
+                        total_records_count: int = int(total_records["total_records"])  # type: ignore[arg-type]
+                    else:
+                        total_records_count = 0
+
+                    # only continue if there is anything to transfer
+                    if total_records_count > 0:
+                        # populate it
+                        self._mysql_cur.execute(
+                            "SELECT * FROM `{table_name}` {limit}".format(
+                                table_name=table_name,
+                                limit=f"LIMIT {self._limit_rows}" if self._limit_rows > 0 else "",
+                            )
                         )
-                    )
-                total_records = int(self._mysql_cur_dict.fetchone()["total_records"])
-
-                # only continue if there is anything to transfer
-                if total_records > 0:
-                    # populate it
-                    self._logger.info("Transferring table %s", table_name)
-                    self._mysql_cur.execute(
-                        "SELECT * FROM `{table_name}` {limit}".format(
-                            table_name=table_name,
-                            limit="LIMIT {}".format(self._limit_rows)
-                            if self._limit_rows > 0
-                            else "",
+                        columns: t.Tuple[str, ...] = tuple(column[0] for column in self._mysql_cur.description)  # type: ignore[union-attr]
+                        # build the SQL string
+                        sql = """
+                            INSERT OR IGNORE
+                            INTO "{table}" ({fields})
+                            VALUES ({placeholders})
+                        """.format(
+                            table=table_name,
+                            fields=('"{}", ' * len(columns)).rstrip(" ,").format(*columns),
+                            placeholders=("?, " * len(columns)).rstrip(" ,"),
+                        )
+                        self._transfer_table_data(
+                            table_name=table_name,  # type: ignore[arg-type]
+                            sql=sql,
+                            total_records=total_records_count,
                         )
-                    )
-                    columns = [column[0] for column in self._mysql_cur.description]
-                    # build the SQL string
-                    sql = """
-                        INSERT OR IGNORE
-                        INTO "{table}" ({fields})
-                        VALUES ({placeholders})
-                    """.format(
-                        table=table_name,
-                        fields=('"{}", ' * len(columns)).rstrip(" ,").format(*columns),
-                        placeholders=("?, " * len(columns)).rstrip(" ,"),
-                    )
-                    self._transfer_table_data(
-                        table_name=table_name, sql=sql, total_records=total_records
-                    )
         except Exception:  # pylint: disable=W0706
             raise
         finally:
             # re-enable foreign key checking once done transferring
             self._sqlite_cur.execute("PRAGMA foreign_keys=ON")
 
         if self._vacuum:
-            self._logger.info(
-                "Vacuuming created SQLite database file.\nThis might take a while."
-            )
+            self._logger.info("Vacuuming created SQLite database file.\nThis might take a while.")
             self._sqlite_cur.execute("VACUUM")
 
         self._logger.info("Done!")
```

### Comparing `mysql-to-sqlite3-1.4.9/setup.py` & `mysql_to_sqlite3-2.0.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,73 +1,125 @@
-from codecs import open
-from os.path import abspath, dirname, join
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "mysql-to-sqlite3"
+description = "A simple Python tool to transfer data from MySQL to SQLite 3"
+readme = "README.md"
+license = { text = "MIT" }
+requires-python = ">=3.7"
+authors = [
+    { name = "Klemen Tusar", email = "techouse@gmail.com" },
+]
+urls = { Source = "https://github.com/techouse/mysql-to-sqlite3" }
+keywords = [
+    "mysql",
+    "sqlite3",
+    "transfer",
+    "data",
+    "migrate",
+    "migration",
+]
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Environment :: Console",
+    "Intended Audience :: End Users/Desktop",
+    "Intended Audience :: Developers",
+    "Intended Audience :: System Administrators",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Topic :: Database",
+]
+dependencies = [
+    "Click>=8.1.3",
+    "mysql-connector-python>=8.0.18,!=8.0.30,!=8.0.31",
+    "pytimeparse2",
+    "python-slugify>=7.0.0",
+    "simplejson>=3.19.0",
+    "tqdm>=4.65.0",
+    "tabulate",
+    "typing_extensions",
+]
+dynamic = ["version"]
 
-from setuptools import setup
+[tool.hatch.version]
+path = "mysql_to_sqlite3/__init__.py"
 
-here = abspath(dirname(__file__))
+[tool.hatch.build.targets.sdist]
+include = [
+    "mysql_to_sqlite3",
+    "tests",
+    "README.md",
+    "CODE-OF-CONDUCT.md",
+    "LICENSE",
+    "requirements_dev.txt",
+]
 
-packages = ["mysql_to_sqlite3"]
+[project.scripts]
+mysql2sqlite = "mysql_to_sqlite3.cli:cli"
 
-requires = [
-    "Click>=7.0,<8.0.0 ; python_version<'3.6'",
-    "Click>=7.0 ; python_version>='3.6'",
-    "mysql-connector-python>=8.0.18,<8.0.24 ; python_version<'3.6'",
-    "mysql-connector-python>=8.0.18 ; python_version>='3.6'",
-    "pytimeparse>=1.1.8",
-    "python-slugify>=3.0.3,<5.0.0 ; python_version<'3.6'",
-    "python-slugify>=3.0.3 ; python_version>='3.6'",
-    "simplejson>=3.16.0",
-    "six>=1.12.0",
-    "tqdm>=4.35.0",
-    "tabulate<0.8.6 ; python_version<'3.5'",
-    "tabulate ; python_version>='3.5'",
-]
-
-about = {}
-with open(join(here, "mysql_to_sqlite3", "__version__.py"), "r", "utf-8") as fh:
-    exec(fh.read(), about)
-
-with open(join(here, "README.md"), "r", "utf-8") as fh:
-    readme = fh.read()
-
-setup(
-    name=about["__title__"],
-    version=about["__version__"],
-    description=about["__description__"],
-    long_description=readme,
-    long_description_content_type="text/markdown",
-    author=about["__author__"],
-    author_email=about["__author_email__"],
-    url=about["__url__"],
-    packages=packages,
-    include_package_data=True,
-    python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*",
-    install_requires=requires,
-    license=about["__license__"],
-    zip_safe=False,
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Environment :: Console",
-        "Intended Audience :: End Users/Desktop",
-        "Intended Audience :: Developers",
-        "Intended Audience :: System Administrators",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: Implementation :: CPython",
-        "Topic :: Database",
-    ],
-    project_urls={"Source": about["__url__"]},
-    entry_points="""
-        [console_scripts]
-        mysql2sqlite=mysql_to_sqlite3.cli:cli
-    """,
+[tool.black]
+line-length = 120
+target-version = ["py37", "py38", "py39", "py310", "py311"]
+include = '\.pyi?$'
+exclude = '''
+(
+    /(
+        \.eggs
+        | \.git
+        | \.hg
+        | \.mypy_cache
+        | \.tox
+        | \.venv
+        | _build
+        | buck-out
+        | build
+        | dist
+    )/
+    | foo.py
 )
+'''
+
+[tool.isort]
+line_length = 120
+profile = "black"
+lines_after_imports = 2
+known_first_party = "mysql_to_sqlite3"
+skip_gitignore = true
+
+[tool.pytest.ini_options]
+testpaths = ["tests"]
+norecursedirs = [".*", "venv", "env", "*.egg", "dist", "build"]
+minversion = "7.3.1"
+addopts = "-rsxX -l --tb=short --strict-markers"
+timeout = 300
+markers = [
+    "init: Run the initialisation test functions",
+    "transfer: Run the main transfer test functions",
+    "exceptions: Run SQL exception test functions",
+    "cli: Run the cli test functions",
+]
+
+[tool.mypy]
+python_version = "3.7"
+exclude = [
+    "tests",
+    "build",
+    "dist",
+    "venv",
+    "env",
+]
+warn_return_any = true
+warn_unused_configs = true
+
+[[tool.mypy.overrides]]
+module = "pytimeparse2.*,factory.*,docker.*"
+ignore_missing_imports = true
```

### Comparing `mysql-to-sqlite3-1.4.9/tests/database.py` & `mysql_to_sqlite3-2.0.0/tests/database.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,43 @@
+import typing as t
 from datetime import datetime, timedelta
 from decimal import Decimal
 
 import simplejson as json
 from sqlalchemy import create_engine
+from sqlalchemy.engine import Engine
 from sqlalchemy.orm import sessionmaker
-from sqlalchemy_utils import database_exists, create_database
+from sqlalchemy_utils import create_database, database_exists
 
 from .models import Base
 
 
 class Database:
-    engine = None
-    Session = None
+    engine: Engine
+    Session: sessionmaker
 
     def __init__(self, database_uri):
         self.Session = sessionmaker()
-        self.engine = create_engine(
-            database_uri, json_serializer=self.dumps, json_deserializer=json.loads
-        )
+        self.engine = create_engine(database_uri, json_serializer=self.dumps, json_deserializer=json.loads)
         if not database_exists(self.engine.url):
             create_database(self.engine.url)
         self._create_db_tables()
         self.Session.configure(bind=self.engine)
 
-    def _create_db_tables(self):
+    def _create_db_tables(self) -> None:
         Base.metadata.create_all(self.engine)
 
     @classmethod
-    def dumps(cls, data):
+    def dumps(cls, data: t.Any) -> str:
         return json.dumps(data, default=cls.json_serializer)
 
     @staticmethod
-    def json_serializer(data):
+    def json_serializer(data: t.Any) -> t.Optional[str]:
         if isinstance(data, datetime):
             return data.isoformat()
         if isinstance(data, Decimal):
             return str(data)
         if isinstance(data, timedelta):
             hours, remainder = divmod(data.total_seconds(), 3600)
             minutes, seconds = divmod(remainder, 60)
             return "{:02}:{:02}:{:02}".format(int(hours), int(minutes), int(seconds))
+        return None
```

### Comparing `mysql-to-sqlite3-1.4.9/tests/func/mysql_to_sqlite3_test.py` & `mysql_to_sqlite3-2.0.0/tests/func/mysql_to_sqlite3_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,94 @@
 import logging
+import os
 import re
+import typing as t
 from collections import namedtuple
 from decimal import Decimal
+from pathlib import Path
 from random import choice, sample
 
 import mysql.connector
 import pytest
 import simplejson as json
-import six
-from mysql.connector import errorcode, MySQLConnection
-from sqlalchemy import MetaData, Table, select, create_engine, inspect, text
+from _pytest._py.path import LocalPath
+from _pytest.logging import LogCaptureFixture
+from faker import Faker
+from mysql.connector import CMySQLConnection, MySQLConnection, errorcode
+from mysql.connector.cursor import MySQLCursor
+from mysql.connector.pooling import PooledMySQLConnection
+from pytest_mock import MockFixture
+from sqlalchemy import (
+    Connection,
+    CursorResult,
+    Engine,
+    Inspector,
+    MetaData,
+    Row,
+    Select,
+    Table,
+    TextClause,
+    create_engine,
+    inspect,
+    select,
+    text,
+)
+from sqlalchemy.engine.interfaces import ReflectedIndex
 
 from mysql_to_sqlite3 import MySQLtoSQLite
-
-if six.PY2:
-    from ..sixeptions import *
+from tests.conftest import Helpers, MySQLCredentials
+from tests.database import Database
 
 
 @pytest.mark.usefixtures("mysql_instance")
 class TestMySQLtoSQLite:
     @pytest.mark.init
     @pytest.mark.parametrize(
         "quiet",
         [
             pytest.param(False, id="verbose"),
             pytest.param(True, id="quiet"),
         ],
     )
-    def test_missing_mysql_user_raises_exception(self, mysql_credentials, quiet):
+    def test_missing_mysql_user_raises_exception(self, mysql_credentials: MySQLCredentials, quiet: bool) -> None:
         with pytest.raises(ValueError) as excinfo:
-            MySQLtoSQLite(mysql_database=mysql_credentials.database, quiet=quiet)
+            MySQLtoSQLite(mysql_database=mysql_credentials.database, quiet=quiet)  # type: ignore[call-arg]
         assert "Please provide a MySQL user" in str(excinfo.value)
 
     @pytest.mark.init
     @pytest.mark.parametrize(
         "quiet",
         [
             pytest.param(False, id="verbose"),
             pytest.param(True, id="quiet"),
         ],
     )
-    def test_missing_mysql_database_raises_exception(self, faker, quiet):
+    def test_missing_mysql_database_raises_exception(self, faker: Faker, quiet: bool) -> None:
         with pytest.raises(ValueError) as excinfo:
-            MySQLtoSQLite(mysql_user=faker.first_name().lower(), quiet=quiet)
+            MySQLtoSQLite(mysql_user=faker.first_name().lower(), quiet=quiet)  # type: ignore[call-arg]
         assert "Please provide a MySQL database" in str(excinfo.value)
 
     @pytest.mark.init
     @pytest.mark.parametrize(
         "quiet",
         [
             pytest.param(False, id="verbose"),
             pytest.param(True, id="quiet"),
         ],
     )
     def test_invalid_mysql_credentials_raises_access_denied_exception(
-        self, sqlite_database, mysql_database, mysql_credentials, faker, quiet
-    ):
+        self,
+        sqlite_database: "os.PathLike[t.Any]",
+        mysql_database: Database,
+        mysql_credentials: MySQLCredentials,
+        faker: Faker,
+        quiet: bool,
+    ) -> None:
         with pytest.raises(mysql.connector.Error) as excinfo:
-            MySQLtoSQLite(
+            MySQLtoSQLite(  # type: ignore[call-arg]
                 sqlite_file=sqlite_database,
                 mysql_user=faker.first_name().lower(),
                 mysql_password=faker.password(length=16),
                 mysql_database=mysql_credentials.database,
                 mysql_host=mysql_credentials.host,
                 mysql_port=mysql_credentials.port,
                 quiet=quiet,
@@ -73,24 +100,28 @@
         "quiet",
         [
             pytest.param(False, id="verbose"),
             pytest.param(True, id="quiet"),
         ],
     )
     def test_bad_mysql_connection(
-        self, sqlite_database, mysql_credentials, mocker, quiet
-    ):
+        self,
+        sqlite_database: "os.PathLike[t.Any]",
+        mysql_credentials: MySQLCredentials,
+        mocker: MockFixture,
+        quiet: bool,
+    ) -> None:
         FakeConnector = namedtuple("FakeConnector", ["is_connected"])
         mocker.patch.object(
             mysql.connector,
             "connect",
             return_value=FakeConnector(is_connected=lambda: False),
         )
         with pytest.raises((ConnectionError, IOError)) as excinfo:
-            MySQLtoSQLite(
+            MySQLtoSQLite(  # type: ignore[call-arg]
                 sqlite_file=sqlite_database,
                 mysql_user=mysql_credentials.user,
                 mysql_password=mysql_credentials.password,
                 mysql_host=mysql_credentials.host,
                 mysql_port=mysql_credentials.port,
                 mysql_database=mysql_credentials.database,
                 chunk=1000,
@@ -99,114 +130,101 @@
         assert "Unable to connect to MySQL" in str(excinfo.value)
 
     @pytest.mark.init
     @pytest.mark.parametrize(
         "exception, quiet",
         [
             pytest.param(
-                mysql.connector.Error(
-                    msg="Unknown database 'test_db'", errno=errorcode.ER_BAD_DB_ERROR
-                ),
+                mysql.connector.Error(msg="Unknown database 'test_db'", errno=errorcode.ER_BAD_DB_ERROR),
                 False,
                 id="mysql.connector.Error verbose",
             ),
             pytest.param(
-                mysql.connector.Error(
-                    msg="Unknown database 'test_db'", errno=errorcode.ER_BAD_DB_ERROR
-                ),
+                mysql.connector.Error(msg="Unknown database 'test_db'", errno=errorcode.ER_BAD_DB_ERROR),
                 True,
                 id="mysql.connector.Error quiet",
             ),
-            pytest.param(
-                Exception("Unknown database 'test_db'"), False, id="Exception verbose"
-            ),
-            pytest.param(
-                Exception("Unknown database 'test_db'"), True, id="Exception quiet"
-            ),
+            pytest.param(Exception("Unknown database 'test_db'"), False, id="Exception verbose"),
+            pytest.param(Exception("Unknown database 'test_db'"), True, id="Exception quiet"),
         ],
     )
     def test_non_existing_mysql_database_raises_exception(
         self,
-        sqlite_database,
-        mysql_database,
-        mysql_credentials,
-        faker,
-        mocker,
-        caplog,
-        exception,
-        quiet,
-    ):
+        sqlite_database: "os.PathLike[t.Any]",
+        mysql_database: Database,
+        mysql_credentials: MySQLCredentials,
+        faker: Faker,
+        mocker: MockFixture,
+        caplog: LogCaptureFixture,
+        exception: Exception,
+        quiet: bool,
+    ) -> None:
         class FakeMySQLConnection(MySQLConnection):
             @property
-            def database(self):
+            def database(self) -> str:
                 return self._database
 
             @database.setter
-            def database(self, value):
+            def database(self, value) -> None:
                 self._database = value
                 # raise a fake exception
                 raise exception
 
-            def is_connected(self):
+            def is_connected(self) -> bool:
                 return True
 
             def cursor(
                 self,
-                buffered=None,
-                raw=None,
-                prepared=None,
-                cursor_class=None,
-                dictionary=None,
-                named_tuple=None,
-            ):
+                buffered: t.Optional[bool] = None,
+                raw: t.Optional[bool] = None,
+                prepared: t.Optional[bool] = None,
+                cursor_class: t.Optional[t.Type[MySQLCursor]] = None,
+                dictionary: t.Optional[bool] = None,
+                named_tuple: t.Optional[bool] = None,
+            ) -> t.Union[t.Any, MySQLCursor]:
                 return True
 
         caplog.set_level(logging.DEBUG)
-        mocker.patch.object(
-            mysql.connector, "connect", return_value=FakeMySQLConnection()
-        )
+        mocker.patch.object(mysql.connector, "connect", return_value=FakeMySQLConnection())
         with pytest.raises((mysql.connector.Error, Exception)) as excinfo:
-            MySQLtoSQLite(
+            MySQLtoSQLite(  # type: ignore[call-arg]
                 sqlite_file=sqlite_database,
                 mysql_user=mysql_credentials.user,
                 mysql_password=mysql_credentials.password,
                 mysql_database=mysql_credentials.database,
                 mysql_host=mysql_credentials.host,
                 mysql_port=mysql_credentials.port,
                 quiet=quiet,
             )
-            assert any(
-                "MySQL Database does not exist!" in message
-                for message in caplog.messages
-            )
+            assert any("MySQL Database does not exist!" in message for message in caplog.messages)
         assert "Unknown database" in str(excinfo.value)
 
     @pytest.mark.xfail
     @pytest.mark.init
     @pytest.mark.parametrize(
         "quiet",
         [
             pytest.param(False, id="verbose"),
             pytest.param(True, id="quiet"),
         ],
     )
     def test_log_to_file(
         self,
-        sqlite_database,
-        mysql_database,
-        mysql_credentials,
-        caplog,
-        tmpdir,
-        faker,
-        quiet,
-    ):
-        log_file = tmpdir.join("db.log")
+        sqlite_database: "os.PathLike[t.Any]",
+        mysql_database: Database,
+        mysql_credentials: MySQLCredentials,
+        caplog: LogCaptureFixture,
+        tmpdir: LocalPath,
+        faker: Faker,
+        quiet: bool,
+    ) -> None:
+        log_file: LocalPath = tmpdir.join(Path("db.log"))
         caplog.set_level(logging.DEBUG)
         with pytest.raises(mysql.connector.Error):
-            MySQLtoSQLite(
+            MySQLtoSQLite(  # type: ignore[call-arg]
                 sqlite_file=sqlite_database,
                 mysql_user=faker.first_name().lower(),
                 mysql_password=faker.password(length=16),
                 mysql_database=mysql_credentials.database,
                 mysql_host=mysql_credentials.host,
                 mysql_port=mysql_credentials.port,
                 log_file=str(log_file),
@@ -215,18 +233,15 @@
         assert any("Access denied for user" in message for message in caplog.messages)
         with log_file.open("r") as log_fh:
             log = log_fh.read()
             if len(caplog.messages) > 1:
                 assert caplog.messages[1] in log
             else:
                 assert caplog.messages[0] in log
-            assert (
-                re.match(r"^\d{4,}-\d{2,}-\d{2,}\s+\d{2,}:\d{2,}:\d{2,}\s+\w+\s+", log)
-                is not None
-            )
+            assert re.match(r"^\d{4,}-\d{2,}-\d{2,}\s+\d{2,}:\d{2,}:\d{2,}\s+\w+\s+", log) is not None
 
     @pytest.mark.transfer
     @pytest.mark.parametrize(
         "chunk, vacuum, buffered, prefix_indices",
         [
             # 0000
             pytest.param(
@@ -356,25 +371,25 @@
                 True,
                 id="chunk, no vacuum, buffered cursor, prefix indices",
             ),
         ],
     )
     def test_transfer_transfers_all_tables_from_mysql_to_sqlite(
         self,
-        sqlite_database,
-        mysql_database,
-        mysql_credentials,
-        helpers,
-        caplog,
-        chunk,
-        vacuum,
-        buffered,
-        prefix_indices,
-    ):
-        proc = MySQLtoSQLite(
+        sqlite_database: "os.PathLike[t.Any]",
+        mysql_database: Database,
+        mysql_credentials: MySQLCredentials,
+        helpers: Helpers,
+        caplog: LogCaptureFixture,
+        chunk: t.Optional[int],
+        vacuum: bool,
+        buffered: bool,
+        prefix_indices: bool,
+    ) -> None:
+        proc: MySQLtoSQLite = MySQLtoSQLite(  # type: ignore[call-arg]
             sqlite_file=sqlite_database,
             mysql_user=mysql_credentials.user,
             mysql_password=mysql_credentials.password,
             mysql_database=mysql_credentials.database,
             mysql_host=mysql_credentials.host,
             mysql_port=mysql_credentials.port,
             chunk=chunk,
@@ -397,78 +412,73 @@
                 "Transferring table misc",
                 "Done!",
             }
         )
         assert all(record.levelname == "INFO" for record in caplog.records)
         assert not any(record.levelname == "ERROR" for record in caplog.records)
 
-        sqlite_engine = create_engine(
-            "sqlite:///{database}".format(
-                database=sqlite_database,
-                json_serializer=json.dumps,
-                json_deserializer=json.loads,
-            )
-        )
-        sqlite_cnx = sqlite_engine.connect()
-        sqlite_inspect = inspect(sqlite_engine)
-        sqlite_tables = sqlite_inspect.get_table_names()
-        mysql_engine = create_engine(
-            "mysql+mysqldb://{user}:{password}@{host}:{port}/{database}".format(
-                user=mysql_credentials.user,
-                password=mysql_credentials.password,
-                host=mysql_credentials.host,
-                port=mysql_credentials.port,
-                database=mysql_credentials.database,
-            )
+        sqlite_engine: Engine = create_engine(
+            f"sqlite:///{sqlite_database}",
+            json_serializer=json.dumps,
+            json_deserializer=json.loads,
         )
-        mysql_cnx = mysql_engine.connect()
-        mysql_inspect = inspect(mysql_engine)
-        mysql_tables = mysql_inspect.get_table_names()
 
-        mysql_connector_connection = mysql.connector.connect(
+        sqlite_cnx: Connection = sqlite_engine.connect()
+        sqlite_inspect: Inspector = inspect(sqlite_engine)
+        sqlite_tables: t.List[str] = sqlite_inspect.get_table_names()
+        mysql_engine: Engine = create_engine(
+            f"mysql+mysqldb://{mysql_credentials.user}:{mysql_credentials.password}@{mysql_credentials.host}:{mysql_credentials.port}/{mysql_credentials.database}"
+        )
+        mysql_cnx: Connection = mysql_engine.connect()
+        mysql_inspect: Inspector = inspect(mysql_engine)
+        mysql_tables: t.List[str] = mysql_inspect.get_table_names()
+
+        mysql_connector_connection: t.Union[
+            PooledMySQLConnection, MySQLConnection, CMySQLConnection
+        ] = mysql.connector.connect(
             user=mysql_credentials.user,
             password=mysql_credentials.password,
             host=mysql_credentials.host,
             port=mysql_credentials.port,
             database=mysql_credentials.database,
         )
-        server_version = mysql_connector_connection.get_server_version()
+        server_version: t.Tuple[int, ...] = mysql_connector_connection.get_server_version()
 
         """ Test if both databases have the same table names """
         assert sqlite_tables == mysql_tables
 
         """ Test if all the tables have the same column names """
         for table_name in sqlite_tables:
-            assert [
-                column["name"] for column in sqlite_inspect.get_columns(table_name)
-            ] == [column["name"] for column in mysql_inspect.get_columns(table_name)]
+            assert [column["name"] for column in sqlite_inspect.get_columns(table_name)] == [
+                column["name"] for column in mysql_inspect.get_columns(table_name)
+            ]
 
         """ Test if all the tables have the same indices """
-        index_keys = {"name", "column_names", "unique"}
-        mysql_indices = []
+        index_keys: t.Tuple[str, ...] = ("name", "column_names", "unique")
+        mysql_indices: t.List[ReflectedIndex] = []
         for table_name in mysql_tables:
             for index in mysql_inspect.get_indexes(table_name):
-                mysql_index = {}
+                mysql_index: t.Dict[str, t.Any] = {}
                 for key in index_keys:
                     if key == "name" and prefix_indices:
-                        mysql_index[key] = "{table}_{name}".format(
-                            table=table_name, name=index[key]
-                        )
+                        mysql_index[key] = f"{table_name}_{index[key]}"  # type: ignore[literal-required]
                     else:
-                        mysql_index[key] = index[key]
-                mysql_indices.append(mysql_index)
+                        mysql_index[key] = index[key]  # type: ignore[literal-required]
+                mysql_indices.append(t.cast(ReflectedIndex, mysql_index))
 
         for table_name in sqlite_tables:
             for sqlite_index in sqlite_inspect.get_indexes(table_name):
                 sqlite_index["unique"] = bool(sqlite_index["unique"])
+                if "dialect_options" in sqlite_index:
+                    sqlite_index.pop("dialect_options", None)
                 assert sqlite_index in mysql_indices
 
         """ Test if all the tables have the same foreign keys """
         for table_name in mysql_tables:
-            mysql_fk_stmt = text(
+            mysql_fk_stmt: TextClause = text(
                 """
                 SELECT k.COLUMN_NAME AS `from`,
                        k.REFERENCED_TABLE_NAME AS `table`,
                        k.REFERENCED_COLUMN_NAME AS `to`,
                        c.UPDATE_RULE AS `on_update`,
                        c.DELETE_RULE AS `on_delete`
                 FROM information_schema.TABLE_CONSTRAINTS AS i
@@ -484,327 +494,505 @@
                     else "LEFT JOIN"
                 )
             ).bindparams(
                 table_schema=mysql_credentials.database,
                 table_name=table_name,
                 constraint_type="FOREIGN KEY",
             )
-            mysql_fk_result = mysql_cnx.execute(mysql_fk_stmt)
-            mysql_foreign_keys = [dict(row) for row in mysql_fk_result]
+            mysql_fk_result: CursorResult = mysql_cnx.execute(mysql_fk_stmt)
+            mysql_foreign_keys: t.List[t.Dict[str, t.Any]] = [dict(row) for row in mysql_fk_result.mappings()]
 
-            sqlite_fk_stmt = 'PRAGMA foreign_key_list("{table}")'.format(
-                table=table_name
-            )
-            sqlite_fk_result = sqlite_cnx.execute(sqlite_fk_stmt)
+            sqlite_fk_stmt: TextClause = text(f'PRAGMA foreign_key_list("{table_name}")')
+            sqlite_fk_result: CursorResult = sqlite_cnx.execute(sqlite_fk_stmt)
             if sqlite_fk_result.returns_rows:
-                for row in sqlite_fk_result:
-                    fk = dict(row)
+                for row in sqlite_fk_result.mappings():
+                    fk: t.Dict[str, t.Any] = dict(row)
                     assert {
                         "table": fk["table"],
                         "from": fk["from"],
                         "to": fk["to"],
                         "on_update": fk["on_update"],
                         "on_delete": fk["on_delete"],
                     } in mysql_foreign_keys
 
         """ Check if all the data was transferred correctly """
-        sqlite_results = []
-        mysql_results = []
+        sqlite_results: t.List[t.Tuple[t.Tuple[t.Any, ...], ...]] = []
+        mysql_results: t.List[t.Tuple[t.Tuple[t.Any, ...], ...]] = []
 
-        meta = MetaData(bind=None)
+        meta: MetaData = MetaData()
         for table_name in sqlite_tables:
-            sqlite_table = Table(
-                table_name, meta, autoload=True, autoload_with=sqlite_engine
-            )
-            sqlite_stmt = select([sqlite_table])
-            sqlite_result = sqlite_cnx.execute(sqlite_stmt).fetchall()
+            sqlite_table: Table = Table(table_name, meta, autoload_with=sqlite_engine)
+            sqlite_stmt: Select = select(sqlite_table)
+            sqlite_result: t.List[Row[t.Any]] = list(sqlite_cnx.execute(sqlite_stmt).fetchall())
             sqlite_result.sort()
-            sqlite_result = [
-                [float(data) if isinstance(data, Decimal) else data for data in row]
-                for row in sqlite_result
-            ]
-            sqlite_results.append(sqlite_result)
+            sqlite_result_adapted: t.Tuple[t.Tuple[t.Any, ...], ...] = tuple(
+                tuple(float(data) if isinstance(data, Decimal) else data for data in row) for row in sqlite_result
+            )
+            sqlite_results.append(sqlite_result_adapted)
 
         for table_name in mysql_tables:
-            mysql_table = Table(
-                table_name, meta, autoload=True, autoload_with=mysql_engine
-            )
-            mysql_stmt = select([mysql_table])
-            mysql_result = mysql_cnx.execute(mysql_stmt).fetchall()
+            mysql_table: Table = Table(table_name, meta, autoload_with=mysql_engine)
+            mysql_stmt: Select = select(mysql_table)
+            mysql_result: t.List[Row[t.Any]] = list(mysql_cnx.execute(mysql_stmt).fetchall())
             mysql_result.sort()
-            mysql_result = [
-                [float(data) if isinstance(data, Decimal) else data for data in row]
-                for row in mysql_result
-            ]
-            mysql_results.append(mysql_result)
+            mysql_result_adapted: t.Tuple[t.Tuple[t.Any, ...], ...] = tuple(
+                tuple(float(data) if isinstance(data, Decimal) else data for data in row) for row in mysql_result
+            )
+            mysql_results.append(mysql_result_adapted)
 
         assert sqlite_results == mysql_results
 
+        mysql_cnx.close()
+        sqlite_cnx.close()
+        mysql_engine.dispose()
+        sqlite_engine.dispose()
+
+    @pytest.mark.transfer
+    def test_specific_tables_include_and_exclude_are_mutually_exclusive_options(
+        self,
+        sqlite_database: "os.PathLike[t.Any]",
+        mysql_credentials: MySQLCredentials,
+        caplog: LogCaptureFixture,
+        faker: Faker,
+    ) -> None:
+        with pytest.raises(ValueError) as excinfo:
+            MySQLtoSQLite(  # type: ignore[call-arg]
+                sqlite_file=sqlite_database,
+                mysql_user=mysql_credentials.user,
+                mysql_password=mysql_credentials.password,
+                mysql_database=mysql_credentials.database,
+                mysql_tables=faker.words(nb=3),
+                exclude_mysql_tables=faker.words(nb=3),
+                mysql_host=mysql_credentials.host,
+                mysql_port=mysql_credentials.port,
+            )
+        assert "mysql_tables and exclude_mysql_tables are mutually exclusive" in str(excinfo.value)
+
     @pytest.mark.transfer
     @pytest.mark.parametrize(
-        "chunk, vacuum, buffered, prefix_indices",
+        "chunk, vacuum, buffered, prefix_indices, exclude_tables",
         [
-            # 0000
+            # 00000
             pytest.param(
                 None,
                 False,
                 False,
                 False,
-                id="no chunk, no vacuum, no buffered cursor, no prefix indices",
+                False,
+                id="no chunk, no vacuum, no buffered cursor, no prefix indices, include tables",
             ),
-            # 0001
+            # 00001
             pytest.param(
                 None,
                 False,
                 False,
+                False,
                 True,
-                id="no chunk, no vacuum, no buffered cursor, prefix indices",
+                id="no chunk, no vacuum, no buffered cursor, no prefix indices, exclude tables",
             ),
-            # 1110
+            # 00010
+            pytest.param(
+                None,
+                False,
+                False,
+                True,
+                False,
+                id="no chunk, no vacuum, no buffered cursor, prefix indices, include tables",
+            ),
+            # 00011
+            pytest.param(
+                None,
+                False,
+                False,
+                True,
+                True,
+                id="no chunk, no vacuum, no buffered cursor, prefix indices, exclude tables",
+            ),
+            # 11100
             pytest.param(
                 10,
                 True,
                 True,
                 False,
-                id="chunk, vacuum, buffered cursor, no prefix indices",
+                False,
+                id="chunk, vacuum, buffered cursor, no prefix indices, include tables",
             ),
-            # 1111
+            # 11101
             pytest.param(
                 10,
                 True,
                 True,
+                False,
                 True,
-                id="chunk, vacuum, buffered cursor, prefix indices",
+                id="chunk, vacuum, buffered cursor, no prefix indices, exclude tables",
             ),
-            # 1100
+            # 11110
+            pytest.param(
+                10,
+                True,
+                True,
+                True,
+                False,
+                id="chunk, vacuum, buffered cursor, prefix indices, include tables",
+            ),
+            # 11111
+            pytest.param(
+                10,
+                True,
+                True,
+                True,
+                True,
+                id="chunk, vacuum, buffered cursor, prefix indices, exclude tables",
+            ),
+            # 11000
             pytest.param(
                 10,
                 True,
                 False,
                 False,
-                id="chunk, vacuum, no buffered cursor, no prefix indices",
+                False,
+                id="chunk, vacuum, no buffered cursor, no prefix indices, include tables",
             ),
-            # 1101
+            # 11001
             pytest.param(
                 10,
                 True,
                 False,
+                False,
                 True,
-                id="chunk, vacuum, no buffered cursor, prefix indices",
+                id="chunk, vacuum, no buffered cursor, no prefix indices, exclude tables",
             ),
-            # 0110
+            # 11010
+            pytest.param(
+                10,
+                True,
+                False,
+                True,
+                False,
+                id="chunk, vacuum, no buffered cursor, prefix indices, include tables",
+            ),
+            # 11011
+            pytest.param(
+                10,
+                True,
+                False,
+                True,
+                True,
+                id="chunk, vacuum, no buffered cursor, prefix indices, exclude tables",
+            ),
+            # 01100
             pytest.param(
                 None,
                 True,
                 True,
                 False,
-                id="no chunk, vacuum, buffered cursor, no prefix indices",
+                False,
+                id="no chunk, vacuum, buffered cursor, no prefix indices, include tables",
             ),
-            # 0111
+            # 01101
             pytest.param(
                 None,
                 True,
                 True,
+                False,
                 True,
-                id="no chunk, vacuum, buffered cursor, prefix indices",
+                id="no chunk, vacuum, buffered cursor, no prefix indices, exclude tables",
             ),
-            # 0100
+            # 01110
+            pytest.param(
+                None,
+                True,
+                True,
+                True,
+                False,
+                id="no chunk, vacuum, buffered cursor, prefix indices, include tables",
+            ),
+            # 01111
+            pytest.param(
+                None,
+                True,
+                True,
+                True,
+                True,
+                id="no chunk, vacuum, buffered cursor, prefix indices, exclude tables",
+            ),
+            # 01000
             pytest.param(
                 None,
                 True,
                 False,
                 False,
-                id="no chunk, vacuum, no buffered cursor, no prefix indices",
+                False,
+                id="no chunk, vacuum, no buffered cursor, no prefix indices, include tables",
             ),
-            # 0101
+            # 01001
             pytest.param(
                 None,
                 True,
                 False,
+                False,
                 True,
-                id="no chunk, vacuum, no buffered cursor, prefix indices",
+                id="no chunk, vacuum, no buffered cursor, no prefix indices, exclude tables",
             ),
-            # 1000
+            # 01010
+            pytest.param(
+                None,
+                True,
+                False,
+                True,
+                False,
+                id="no chunk, vacuum, no buffered cursor, prefix indices, include tables",
+            ),
+            # 01011
+            pytest.param(
+                None,
+                True,
+                False,
+                True,
+                True,
+                id="no chunk, vacuum, no buffered cursor, prefix indices, exclude tables",
+            ),
+            # 10000
             pytest.param(
                 10,
                 False,
                 False,
                 False,
-                id="chunk, no vacuum, no buffered cursor, no prefix indices",
+                False,
+                id="chunk, no vacuum, no buffered cursor, no prefix indices, include tables",
             ),
-            # 1001
+            # 10001
             pytest.param(
                 10,
                 False,
                 False,
+                False,
                 True,
-                id="chunk, no vacuum, no buffered cursor, prefix indices",
+                id="chunk, no vacuum, no buffered cursor, no prefix indices, exclude tables",
             ),
-            # 0010
+            # 10010
+            pytest.param(
+                10,
+                False,
+                False,
+                True,
+                False,
+                id="chunk, no vacuum, no buffered cursor, prefix indices, include tables",
+            ),
+            # 10011
+            pytest.param(
+                10,
+                False,
+                False,
+                True,
+                True,
+                id="chunk, no vacuum, no buffered cursor, prefix indices, exclude tables",
+            ),
+            # 00100
             pytest.param(
                 None,
                 False,
                 True,
                 False,
-                id="no chunk, no vacuum, buffered cursor, no prefix indices",
+                False,
+                id="no chunk, no vacuum, buffered cursor, no prefix indices, include tables",
             ),
-            # 0011
+            # 00101
             pytest.param(
                 None,
                 False,
                 True,
+                False,
                 True,
-                id="no chunk, no vacuum, buffered cursor, prefix indices",
+                id="no chunk, no vacuum, buffered cursor, no prefix indices, exclude tables",
             ),
-            # 1010
+            # 00110
+            pytest.param(
+                None,
+                False,
+                True,
+                True,
+                False,
+                id="no chunk, no vacuum, buffered cursor, prefix indices, include tables",
+            ),
+            # 00111
+            pytest.param(
+                None,
+                False,
+                True,
+                True,
+                True,
+                id="no chunk, no vacuum, buffered cursor, prefix indices, exclude tables",
+            ),
+            # 10100
             pytest.param(
                 10,
                 False,
                 True,
                 False,
-                id="chunk, no vacuum, buffered cursor, no prefix indices",
+                False,
+                id="chunk, no vacuum, buffered cursor, no prefix indices, include tables",
             ),
-            # 1011
+            # 10101
             pytest.param(
                 10,
                 False,
                 True,
+                False,
                 True,
-                id="chunk, no vacuum, buffered cursor, prefix indices",
+                id="chunk, no vacuum, buffered cursor, no prefix indices, exclude tables",
+            ),
+            # 10110
+            pytest.param(
+                10,
+                False,
+                True,
+                True,
+                False,
+                id="chunk, no vacuum, buffered cursor, prefix indices, include tables",
+            ),
+            # 10111
+            pytest.param(
+                10,
+                False,
+                True,
+                True,
+                True,
+                id="chunk, no vacuum, buffered cursor, prefix indices, exclude tables",
             ),
         ],
     )
     def test_transfer_specific_tables_transfers_only_specified_tables_from_mysql_to_sqlite(
         self,
-        sqlite_database,
-        mysql_database,
-        mysql_credentials,
-        helpers,
-        caplog,
-        chunk,
-        vacuum,
-        buffered,
-        prefix_indices,
-    ):
-        mysql_engine = create_engine(
-            "mysql+mysqldb://{user}:{password}@{host}:{port}/{database}".format(
-                user=mysql_credentials.user,
-                password=mysql_credentials.password,
-                host=mysql_credentials.host,
-                port=mysql_credentials.port,
-                database=mysql_credentials.database,
-            )
+        sqlite_database: "os.PathLike[t.Any]",
+        mysql_database: Database,
+        mysql_credentials: MySQLCredentials,
+        helpers: Helpers,
+        caplog: LogCaptureFixture,
+        chunk: t.Optional[int],
+        vacuum: bool,
+        buffered: bool,
+        prefix_indices: bool,
+        exclude_tables: bool,
+    ) -> None:
+        mysql_engine: Engine = create_engine(
+            f"mysql+mysqldb://{mysql_credentials.user}:{mysql_credentials.password}@{mysql_credentials.host}:{mysql_credentials.port}/{mysql_credentials.database}"
         )
-        mysql_cnx = mysql_engine.connect()
-        mysql_inspect = inspect(mysql_engine)
-        mysql_tables = mysql_inspect.get_table_names()
+        mysql_cnx: Connection = mysql_engine.connect()
+        mysql_inspect: Inspector = inspect(mysql_engine)
+        mysql_tables: t.List[str] = mysql_inspect.get_table_names()
 
-        if six.PY2:
-            table_number = choice(xrange(1, len(mysql_tables)))
-        else:
-            table_number = choice(range(1, len(mysql_tables)))
+        table_number: int = choice(range(1, len(mysql_tables)))
 
-        random_mysql_tables = sample(mysql_tables, table_number)
+        random_mysql_tables: t.List[str] = sample(mysql_tables, table_number)
         random_mysql_tables.sort()
 
-        proc = MySQLtoSQLite(
+        remaining_tables: t.List[str] = list(set(mysql_tables) - set(random_mysql_tables))
+        remaining_tables.sort()
+
+        proc: MySQLtoSQLite = MySQLtoSQLite(  # type: ignore[call-arg]
             sqlite_file=sqlite_database,
             mysql_user=mysql_credentials.user,
             mysql_password=mysql_credentials.password,
             mysql_database=mysql_credentials.database,
-            mysql_tables=random_mysql_tables,
+            mysql_tables=None if exclude_tables else random_mysql_tables,
+            exclude_mysql_tables=random_mysql_tables if exclude_tables else None,
             mysql_host=mysql_credentials.host,
             mysql_port=mysql_credentials.port,
             prefix_indices=prefix_indices,
         )
         caplog.set_level(logging.DEBUG)
         proc.transfer()
         assert all(
             message in [record.message for record in caplog.records]
             for message in set(
-                ["Transferring table {}".format(table) for table in random_mysql_tables]
+                [
+                    f"Transferring table {table}"
+                    for table in (remaining_tables if exclude_tables else random_mysql_tables)
+                ]
                 + ["Done!"]
             )
         )
         assert all(record.levelname == "INFO" for record in caplog.records)
         assert not any(record.levelname == "ERROR" for record in caplog.records)
 
-        sqlite_engine = create_engine(
-            "sqlite:///{database}".format(
-                database=sqlite_database,
-                json_serializer=json.dumps,
-                json_deserializer=json.loads,
-            )
+        sqlite_engine: Engine = create_engine(
+            f"sqlite:///{sqlite_database}",
+            json_serializer=json.dumps,
+            json_deserializer=json.loads,
         )
-        sqlite_cnx = sqlite_engine.connect()
-        sqlite_inspect = inspect(sqlite_engine)
-        sqlite_tables = sqlite_inspect.get_table_names()
+
+        sqlite_cnx: Connection = sqlite_engine.connect()
+        sqlite_inspect: Inspector = inspect(sqlite_engine)
+        sqlite_tables: t.List[str] = sqlite_inspect.get_table_names()
 
         """ Test if both databases have the same table names """
-        assert sqlite_tables == random_mysql_tables
+        if exclude_tables:
+            assert set(sqlite_tables) == set(remaining_tables)
+        else:
+            assert set(sqlite_tables) == set(random_mysql_tables)
 
         """ Test if all the tables have the same column names """
         for table_name in sqlite_tables:
-            assert [
-                column["name"] for column in sqlite_inspect.get_columns(table_name)
-            ] == [column["name"] for column in mysql_inspect.get_columns(table_name)]
+            assert [column["name"] for column in sqlite_inspect.get_columns(table_name)] == [
+                column["name"] for column in mysql_inspect.get_columns(table_name)
+            ]
 
         """ Test if all the tables have the same indices """
-        index_keys = {"name", "column_names", "unique"}
-        mysql_indices = []
-        for table_name in random_mysql_tables:
+        index_keys: t.Tuple[str, ...] = ("name", "column_names", "unique")
+        mysql_indices: t.List[ReflectedIndex] = []
+        for table_name in remaining_tables if exclude_tables else random_mysql_tables:
             for index in mysql_inspect.get_indexes(table_name):
-                mysql_index = {}
+                mysql_index: t.Dict[str, t.Any] = {}
                 for key in index_keys:
                     if key == "name" and prefix_indices:
-                        mysql_index[key] = "{table}_{name}".format(
-                            table=table_name, name=index[key]
-                        )
+                        mysql_index[key] = f"{table_name}_{index[key]}"  # type: ignore[literal-required]
                     else:
-                        mysql_index[key] = index[key]
-                mysql_indices.append(mysql_index)
+                        mysql_index[key] = index[key]  # type: ignore[literal-required]
+                mysql_indices.append(t.cast(ReflectedIndex, mysql_index))
 
         for table_name in sqlite_tables:
             for sqlite_index in sqlite_inspect.get_indexes(table_name):
                 sqlite_index["unique"] = bool(sqlite_index["unique"])
+                if "dialect_options" in sqlite_index:
+                    sqlite_index.pop("dialect_options", None)
                 assert sqlite_index in mysql_indices
 
         """ Check if all the data was transferred correctly """
-        sqlite_results = []
-        mysql_results = []
+        sqlite_results: t.List[t.Tuple[t.Tuple[t.Any, ...], ...]] = []
+        mysql_results: t.List[t.Tuple[t.Tuple[t.Any, ...], ...]] = []
 
-        meta = MetaData(bind=None)
+        meta: MetaData = MetaData()
         for table_name in sqlite_tables:
-            sqlite_table = Table(
-                table_name, meta, autoload=True, autoload_with=sqlite_engine
-            )
-            sqlite_stmt = select([sqlite_table])
-            sqlite_result = sqlite_cnx.execute(sqlite_stmt).fetchall()
+            sqlite_table: Table = Table(table_name, meta, autoload_with=sqlite_engine)
+            sqlite_stmt: Select = select(sqlite_table)
+            sqlite_result: t.List[Row[t.Any]] = list(sqlite_cnx.execute(sqlite_stmt).fetchall())
             sqlite_result.sort()
-            sqlite_result = [
-                [float(data) if isinstance(data, Decimal) else data for data in row]
-                for row in sqlite_result
-            ]
-            sqlite_results.append(sqlite_result)
-
-        for table_name in random_mysql_tables:
-            mysql_table = Table(
-                table_name, meta, autoload=True, autoload_with=mysql_engine
+            sqlite_result_adapted = tuple(
+                tuple(float(data) if isinstance(data, Decimal) else data for data in row) for row in sqlite_result
             )
-            mysql_stmt = select([mysql_table])
-            mysql_result = mysql_cnx.execute(mysql_stmt).fetchall()
+            sqlite_results.append(sqlite_result_adapted)
+
+        for table_name in remaining_tables if exclude_tables else random_mysql_tables:
+            mysql_table: Table = Table(table_name, meta, autoload_with=mysql_engine)
+            mysql_stmt: Select = select(mysql_table)
+            mysql_result: t.List[Row[t.Any]] = list(mysql_cnx.execute(mysql_stmt).fetchall())
             mysql_result.sort()
-            mysql_result = [
-                [float(data) if isinstance(data, Decimal) else data for data in row]
-                for row in mysql_result
-            ]
-            mysql_results.append(mysql_result)
+            mysql_result_adapted = tuple(
+                tuple(float(data) if isinstance(data, Decimal) else data for data in row) for row in mysql_result
+            )
+            mysql_results.append(mysql_result_adapted)
 
         assert sqlite_results == mysql_results
 
+        mysql_cnx.close()
+        sqlite_cnx.close()
+        mysql_engine.dispose()
+        sqlite_engine.dispose()
+
     @pytest.mark.transfer
     @pytest.mark.parametrize(
         "chunk, vacuum, buffered, prefix_indices",
         [
             # 0000
             pytest.param(
                 None,
@@ -933,30 +1121,27 @@
                 True,
                 id="chunk, no vacuum, buffered cursor, prefix indices",
             ),
         ],
     )
     def test_transfer_limited_rows_from_mysql_to_sqlite(
         self,
-        sqlite_database,
-        mysql_database,
-        mysql_credentials,
-        helpers,
-        caplog,
-        chunk,
-        vacuum,
-        buffered,
-        prefix_indices,
-    ):
-        if six.PY2:
-            limit_rows = choice(xrange(1, 10))
-        else:
-            limit_rows = choice(range(1, 10))
+        sqlite_database: "os.PathLike[t.Any]",
+        mysql_database: Database,
+        mysql_credentials: MySQLCredentials,
+        helpers: Helpers,
+        caplog: LogCaptureFixture,
+        chunk: t.Optional[int],
+        vacuum: bool,
+        buffered: bool,
+        prefix_indices: bool,
+    ) -> None:
+        limit_rows: int = choice(range(1, 10))
 
-        proc = MySQLtoSQLite(
+        proc: MySQLtoSQLite = MySQLtoSQLite(  # type: ignore[call-arg]
             sqlite_file=sqlite_database,
             mysql_user=mysql_credentials.user,
             mysql_password=mysql_credentials.password,
             mysql_database=mysql_credentials.database,
             limit_rows=limit_rows,
             mysql_host=mysql_credentials.host,
             mysql_port=mysql_credentials.port,
@@ -977,78 +1162,73 @@
                 "Transferring table misc",
                 "Done!",
             }
         )
         assert all(record.levelname == "INFO" for record in caplog.records)
         assert not any(record.levelname == "ERROR" for record in caplog.records)
 
-        sqlite_engine = create_engine(
-            "sqlite:///{database}".format(
-                database=sqlite_database,
-                json_serializer=json.dumps,
-                json_deserializer=json.loads,
-            )
-        )
-        sqlite_cnx = sqlite_engine.connect()
-        sqlite_inspect = inspect(sqlite_engine)
-        sqlite_tables = sqlite_inspect.get_table_names()
-        mysql_engine = create_engine(
-            "mysql+mysqldb://{user}:{password}@{host}:{port}/{database}".format(
-                user=mysql_credentials.user,
-                password=mysql_credentials.password,
-                host=mysql_credentials.host,
-                port=mysql_credentials.port,
-                database=mysql_credentials.database,
-            )
+        sqlite_engine: Engine = create_engine(
+            f"sqlite:///{sqlite_database}",
+            json_serializer=json.dumps,
+            json_deserializer=json.loads,
         )
-        mysql_cnx = mysql_engine.connect()
-        mysql_inspect = inspect(mysql_engine)
-        mysql_tables = mysql_inspect.get_table_names()
 
-        mysql_connector_connection = mysql.connector.connect(
+        sqlite_cnx: Connection = sqlite_engine.connect()
+        sqlite_inspect: Inspector = inspect(sqlite_engine)
+        sqlite_tables: t.List[str] = sqlite_inspect.get_table_names()
+        mysql_engine: Engine = create_engine(
+            f"mysql+mysqldb://{mysql_credentials.user}:{mysql_credentials.password}@{mysql_credentials.host}:{mysql_credentials.port}/{mysql_credentials.database}"
+        )
+        mysql_cnx: Connection = mysql_engine.connect()
+        mysql_inspect: Inspector = inspect(mysql_engine)
+        mysql_tables: t.List[str] = mysql_inspect.get_table_names()
+
+        mysql_connector_connection: t.Union[
+            PooledMySQLConnection, MySQLConnection, CMySQLConnection
+        ] = mysql.connector.connect(
             user=mysql_credentials.user,
             password=mysql_credentials.password,
             host=mysql_credentials.host,
             port=mysql_credentials.port,
             database=mysql_credentials.database,
         )
-        server_version = mysql_connector_connection.get_server_version()
+        server_version: t.Tuple[int, ...] = mysql_connector_connection.get_server_version()
 
         """ Test if both databases have the same table names """
         assert sqlite_tables == mysql_tables
 
         """ Test if all the tables have the same column names """
         for table_name in sqlite_tables:
-            assert [
-                column["name"] for column in sqlite_inspect.get_columns(table_name)
-            ] == [column["name"] for column in mysql_inspect.get_columns(table_name)]
+            assert [column["name"] for column in sqlite_inspect.get_columns(table_name)] == [
+                column["name"] for column in mysql_inspect.get_columns(table_name)
+            ]
 
         """ Test if all the tables have the same indices """
-        index_keys = {"name", "column_names", "unique"}
-        mysql_indices = []
+        index_keys: t.Tuple[str, ...] = ("name", "column_names", "unique")
+        mysql_indices: t.List[ReflectedIndex] = []
         for table_name in mysql_tables:
             for index in mysql_inspect.get_indexes(table_name):
-                mysql_index = {}
+                mysql_index: t.Dict[str, t.Any] = {}
                 for key in index_keys:
                     if key == "name" and prefix_indices:
-                        mysql_index[key] = "{table}_{name}".format(
-                            table=table_name, name=index[key]
-                        )
+                        mysql_index[key] = f"{table_name}_{index[key]}"  # type: ignore[literal-required]
                     else:
-                        mysql_index[key] = index[key]
-                mysql_indices.append(mysql_index)
+                        mysql_index[key] = index[key]  # type: ignore[literal-required]
+                mysql_indices.append(t.cast(ReflectedIndex, mysql_index))
 
         for table_name in sqlite_tables:
             for sqlite_index in sqlite_inspect.get_indexes(table_name):
                 sqlite_index["unique"] = bool(sqlite_index["unique"])
+                if "dialect_options" in sqlite_index:
+                    sqlite_index.pop("dialect_options", None)
                 assert sqlite_index in mysql_indices
 
         """ Test if all the tables have the same foreign keys """
         for table_name in mysql_tables:
-            mysql_fk_stmt = text(
+            mysql_fk_stmt: TextClause = text(
                 """
                 SELECT k.COLUMN_NAME AS `from`,
                        k.REFERENCED_TABLE_NAME AS `table`,
                        k.REFERENCED_COLUMN_NAME AS `to`,
                        c.UPDATE_RULE AS `on_update`,
                        c.DELETE_RULE AS `on_delete`
                 FROM information_schema.TABLE_CONSTRAINTS AS i
@@ -1064,57 +1244,54 @@
                     else "LEFT JOIN"
                 )
             ).bindparams(
                 table_schema=mysql_credentials.database,
                 table_name=table_name,
                 constraint_type="FOREIGN KEY",
             )
-            mysql_fk_result = mysql_cnx.execute(mysql_fk_stmt)
-            mysql_foreign_keys = [dict(row) for row in mysql_fk_result]
+            mysql_fk_result: CursorResult = mysql_cnx.execute(mysql_fk_stmt)
+            mysql_foreign_keys: t.List[t.Dict[str, t.Any]] = [dict(row) for row in mysql_fk_result.mappings()]
 
-            sqlite_fk_stmt = 'PRAGMA foreign_key_list("{table}")'.format(
-                table=table_name
-            )
-            sqlite_fk_result = sqlite_cnx.execute(sqlite_fk_stmt)
+            sqlite_fk_stmt: TextClause = text(f'PRAGMA foreign_key_list("{table_name}")')
+            sqlite_fk_result: CursorResult = sqlite_cnx.execute(sqlite_fk_stmt)
             if sqlite_fk_result.returns_rows:
-                for row in sqlite_fk_result:
-                    fk = dict(row)
+                for row in sqlite_fk_result.mappings():
+                    fk: t.Dict[str, t.Any] = dict(row)
                     assert {
                         "table": fk["table"],
                         "from": fk["from"],
                         "to": fk["to"],
                         "on_update": fk["on_update"],
                         "on_delete": fk["on_delete"],
                     } in mysql_foreign_keys
 
         """ Check if all the data was transferred correctly """
-        sqlite_results = []
-        mysql_results = []
+        sqlite_results: t.List[t.Tuple[t.Tuple[t.Any, ...], ...]] = []
+        mysql_results: t.List[t.Tuple[t.Tuple[t.Any, ...], ...]] = []
 
-        meta = MetaData(bind=None)
+        meta: MetaData = MetaData()
         for table_name in sqlite_tables:
-            sqlite_table = Table(
-                table_name, meta, autoload=True, autoload_with=sqlite_engine
-            )
-            sqlite_stmt = select([sqlite_table])
-            sqlite_result = sqlite_cnx.execute(sqlite_stmt).fetchall()
+            sqlite_table: Table = Table(table_name, meta, autoload_with=sqlite_engine)
+            sqlite_stmt: Select = select(sqlite_table)
+            sqlite_result: t.List[Row[t.Any]] = list(sqlite_cnx.execute(sqlite_stmt).fetchall())
             sqlite_result.sort()
-            sqlite_result = [
-                [float(data) if isinstance(data, Decimal) else data for data in row]
-                for row in sqlite_result
-            ]
-            sqlite_results.append(sqlite_result)
+            sqlite_result_adapted = tuple(
+                tuple(float(data) if isinstance(data, Decimal) else data for data in row) for row in sqlite_result
+            )
+            sqlite_results.append(sqlite_result_adapted)
 
         for table_name in mysql_tables:
-            mysql_table = Table(
-                table_name, meta, autoload=True, autoload_with=mysql_engine
-            )
-            mysql_stmt = select([mysql_table]).limit(limit_rows)
-            mysql_result = mysql_cnx.execute(mysql_stmt).fetchall()
+            mysql_table: Table = Table(table_name, meta, autoload_with=mysql_engine)
+            mysql_stmt: Select = select(mysql_table).limit(limit_rows)
+            mysql_result: t.List[Row[t.Any]] = list(mysql_cnx.execute(mysql_stmt).fetchall())
             mysql_result.sort()
-            mysql_result = [
-                [float(data) if isinstance(data, Decimal) else data for data in row]
-                for row in mysql_result
-            ]
-            mysql_results.append(mysql_result)
+            sqlite_result_adapted = tuple(
+                tuple(float(data) if isinstance(data, Decimal) else data for data in row) for row in mysql_result
+            )
+            mysql_results.append(sqlite_result_adapted)
 
         assert sqlite_results == mysql_results
+
+        mysql_cnx.close()
+        sqlite_cnx.close()
+        mysql_engine.dispose()
+        sqlite_engine.dispose()
```

### Comparing `mysql-to-sqlite3-1.4.9/tests/unit/mysql_to_sqlite3_test.py` & `mysql_to_sqlite3-2.0.0/tests/unit/mysql_to_sqlite3_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,143 +1,105 @@
 import logging
+import os
 import sqlite3
+import typing as t
 from random import choice
 
 import mysql.connector
 import pytest
+from _pytest.logging import LogCaptureFixture
 from mysql.connector import errorcode
-from sqlalchemy import inspect
+from pytest_mock import MockerFixture, MockFixture
+from sqlalchemy import Inspector, inspect
 from sqlalchemy.dialects.mysql import __all__ as mysql_column_types
 
 from mysql_to_sqlite3 import MySQLtoSQLite
 from mysql_to_sqlite3.sqlite_utils import CollatingSequences
+from tests.conftest import MySQLCredentials
+from tests.database import Database
 
 
 class TestMySQLtoSQLiteClassmethods:
-    def test_translate_type_from_mysql_to_sqlite_invalid_column_type(self, mocker):
+    def test_translate_type_from_mysql_to_sqlite_invalid_column_type(
+        self,
+        mocker: MockFixture,
+    ) -> None:
         with pytest.raises(ValueError) as excinfo:
             mocker.patch.object(MySQLtoSQLite, "_valid_column_type", return_value=False)
             MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type="text")
         assert "Invalid column_type!" in str(excinfo.value)
 
-    def test_translate_type_from_mysql_to_sqlite_all_valid_columns(self):
+    def test_translate_type_from_mysql_to_sqlite_all_valid_columns(self) -> None:
         for column_type in mysql_column_types + (
             "BIGINT UNSIGNED",
             "INTEGER UNSIGNED",
             "INT",
             "INT UNSIGNED",
             "SMALLINT UNSIGNED",
             "TINYINT UNSIGNED",
             "MEDIUMINT UNSIGNED",
             "CHAR(2)",
             "NCHAR(7)",
             "NVARCHAR(17)",
             "VARCHAR(123)",
         ):
-            if column_type in {"dialect", "insert", "Insert"}:
+            if any(c for c in column_type if c.islower()):
                 continue
             elif column_type == "INT":
-                assert (
-                    MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type)
-                    == "INTEGER"
-                )
+                assert MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type) == "INTEGER"
             elif column_type == "DECIMAL":
-                assert (
-                    MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type)
-                    == "DECIMAL"
-                )
+                assert MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type) == "DECIMAL"
             elif column_type == "YEAR":
-                assert (
-                    MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type)
-                    == "YEAR"
-                )
+                assert MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type) == "YEAR"
             elif column_type == "TIME":
-                assert (
-                    MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type)
-                    == "TIME"
-                )
+                assert MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type) == "TIME"
             elif column_type == "TIMESTAMP":
-                assert (
-                    MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type)
-                    == "DATETIME"
-                )
+                assert MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type) == "DATETIME"
             elif column_type in {
                 "BINARY",
                 "BIT",
                 "LONGBLOB",
                 "MEDIUMBLOB",
                 "TINYBLOB",
                 "VARBINARY",
             }:
-                assert (
-                    MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type)
-                    == "BLOB"
-                )
+                assert MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type) == "BLOB"
             elif column_type == "CHAR":
-                assert (
-                    MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type)
-                    == "CHARACTER"
-                )
+                assert MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type) == "CHARACTER"
             elif column_type == "CHAR(2)":
-                assert (
-                    MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type)
-                    == "CHARACTER(2)"
-                )
+                assert MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type) == "CHARACTER(2)"
             elif column_type == "NCHAR(7)":
-                assert (
-                    MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type)
-                    == "NCHAR(7)"
-                )
+                assert MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type) == "NCHAR(7)"
             elif column_type == "NVARCHAR(17)":
-                assert (
-                    MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type)
-                    == "NVARCHAR(17)"
-                )
+                assert MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type) == "NVARCHAR(17)"
             elif column_type == "VARCHAR(123)":
-                assert (
-                    MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type)
-                    == "VARCHAR(123)"
-                )
+                assert MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type) == "VARCHAR(123)"
             elif column_type in {
                 "ENUM",
                 "LONGTEXT",
                 "MEDIUMTEXT",
                 "SET",
                 "TINYTEXT",
             }:
-                assert (
-                    MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type)
-                    == "TEXT"
-                )
+                assert MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type) == "TEXT"
             elif column_type == "JSON":
+                assert MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type) == "TEXT"
                 assert (
-                    MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type)
-                    == "TEXT"
-                )
-                assert (
-                    MySQLtoSQLite._translate_type_from_mysql_to_sqlite(
-                        column_type, sqlite_json1_extension_enabled=True
-                    )
+                    MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type, sqlite_json1_extension_enabled=True)
                     == "JSON"
                 )
             elif column_type.endswith(" UNSIGNED"):
                 if column_type.startswith("INT "):
-                    assert (
-                        MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type)
-                        == "INTEGER"
-                    )
+                    assert MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type) == "INTEGER"
                 else:
-                    assert MySQLtoSQLite._translate_type_from_mysql_to_sqlite(
-                        column_type
-                    ) == column_type.replace(" UNSIGNED", "")
+                    assert MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type) == column_type.replace(
+                        " UNSIGNED", ""
+                    )
             else:
-                assert (
-                    MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type)
-                    == column_type
-                )
+                assert MySQLtoSQLite._translate_type_from_mysql_to_sqlite(column_type) == column_type
 
     @pytest.mark.parametrize(
         "column_default, sqlite_default_translation",
         [
             pytest.param(None, "", id="None"),
             pytest.param("", "DEFAULT ''", id='""'),
             pytest.param("lorem", "DEFAULT 'lorem'", id='"lorem"'),
@@ -159,185 +121,200 @@
                 "current_timestamp",
                 "DEFAULT CURRENT_TIMESTAMP",
                 id='"current_timestamp"',
             ),
         ],
     )
     def test_translate_default_from_mysql_to_sqlite(
-        self, column_default, sqlite_default_translation
-    ):
-        assert (
-            MySQLtoSQLite._translate_default_from_mysql_to_sqlite(column_default)
-            == sqlite_default_translation
-        )
+        self,
+        column_default: str,
+        sqlite_default_translation: str,
+    ) -> None:
+        assert MySQLtoSQLite._translate_default_from_mysql_to_sqlite(column_default) == sqlite_default_translation
 
     @pytest.mark.parametrize(
         "column_default, sqlite_default_translation, sqlite_version",
         [
             pytest.param(False, "DEFAULT(FALSE)", "3.23.0", id="False (NEW)"),
             pytest.param(True, "DEFAULT(TRUE)", "3.23.0", id="True (NEW)"),
             pytest.param(False, "DEFAULT '0'", "3.22.0", id="False (OLD)"),
             pytest.param(True, "DEFAULT '1'", "3.22.0", id="True (OLD)"),
         ],
     )
     def test_translate_default_booleans_from_mysql_to_sqlite(
-        self, mocker, column_default, sqlite_default_translation, sqlite_version
-    ):
+        self,
+        mocker: MockerFixture,
+        column_default: bool,
+        sqlite_default_translation: str,
+        sqlite_version: str,
+    ) -> None:
         mocker.patch.object(sqlite3, "sqlite_version", sqlite_version)
         assert (
-            MySQLtoSQLite._translate_default_from_mysql_to_sqlite(
-                column_default, "BOOLEAN"
-            )
+            MySQLtoSQLite._translate_default_from_mysql_to_sqlite(column_default, "BOOLEAN")
             == sqlite_default_translation
         )
 
     @pytest.mark.parametrize(
         "column_default, sqlite_default_translation, column_type",
         [
             pytest.param("0", "DEFAULT '0'", "NUMERIC", id='"0" (NUMERIC)'),
             pytest.param("1", "DEFAULT '1'", "NUMERIC", id='"1" (NUMERIC)'),
             pytest.param("0", "DEFAULT '0'", "TEXT", id='"0" (TEXT)'),
             pytest.param("1", "DEFAULT '1'", "TEXT", id='"1" (TEXT)'),
             pytest.param(0, "DEFAULT '0'", "NUMERIC", id="0 (NUMERIC)"),
             pytest.param(1, "DEFAULT '1'", "NUMERIC", id="1 (NUMERIC)"),
             pytest.param(0, "DEFAULT '0'", "TEXT", id="0 (TEXT)"),
             pytest.param(1, "DEFAULT '1'", "TEXT", id="1 (TEXT)"),
-            pytest.param(
-                123456789, "DEFAULT '123456789'", "NUMERIC", id="123456789 (NUMERIC)"
-            ),
-            pytest.param(
-                1234.56789, "DEFAULT '1234.56789'", "NUMERIC", id="1234.56789 (NUMERIC)"
-            ),
-            pytest.param(
-                123456789, "DEFAULT '123456789'", "TEXT", id="123456789 (TEXT)"
-            ),
-            pytest.param(
-                1234.56789, "DEFAULT '1234.56789'", "TEXT", id="1234.56789 (TEXT)"
-            ),
+            pytest.param(123456789, "DEFAULT '123456789'", "NUMERIC", id="123456789 (NUMERIC)"),
+            pytest.param(1234.56789, "DEFAULT '1234.56789'", "NUMERIC", id="1234.56789 (NUMERIC)"),
+            pytest.param(123456789, "DEFAULT '123456789'", "TEXT", id="123456789 (TEXT)"),
+            pytest.param(1234.56789, "DEFAULT '1234.56789'", "TEXT", id="1234.56789 (TEXT)"),
         ],
     )
     def test_translate_default_numbers_from_mysql_to_sqlite(
-        self, column_default, sqlite_default_translation, column_type
-    ):
+        self,
+        column_default: t.Union[int, float, str],
+        sqlite_default_translation: str,
+        column_type: str,
+    ) -> None:
         assert (
-            MySQLtoSQLite._translate_default_from_mysql_to_sqlite(
-                column_default, column_type
-            )
+            MySQLtoSQLite._translate_default_from_mysql_to_sqlite(column_default, column_type)
             == sqlite_default_translation
         )
 
     @pytest.mark.parametrize(
+        "column_default, sqlite_default_translation",
+        [
+            pytest.param(b"", "DEFAULT x''", id="b''"),
+            pytest.param(b"-1", "DEFAULT x'2d31'", id="b'-1'"),
+            pytest.param(b"0", "DEFAULT x'30'", id="b'0'"),
+            pytest.param(b"1", "DEFAULT x'31'", id="b'1'"),
+            pytest.param(b"-1234567890", "DEFAULT x'2d31323334353637383930'", id="b'-1234567890'"),
+            pytest.param(b"1234567890", "DEFAULT x'31323334353637383930'", id="b'1234567890'"),
+            pytest.param(b"SQLite", "DEFAULT x'53514c697465'", id="b'SQLite'"),
+            pytest.param(
+                b"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam pretium, purus vitae sollicitudin varius, nisi lectus vehicula dui, ut dignissim felis dolor blandit justo. Donec eleifend lectus ut feugiat rhoncus. Donec erat nibh, dapibus nec diam id, lacinia lacinia nisl. Mauris sagittis efficitur nisl. Ut tincidunt elementum rhoncus. Cras suscipit dolor sed est ultricies, quis dapibus neque suscipit. Etiam ac enim eu ligula bibendum blandit quis sit amet felis. Praesent mi nisi, luctus sit amet nunc ut, fermentum tempus purus. Suspendisse vel purus a nibh aliquam hendrerit. Aliquam sit amet tristique lorem. Sed elementum congue ante id mollis. Donec vitae pretium neque.",
+                "DEFAULT x'4c6f72656d20697073756d20646f6c6f722073697420616d65742c20636f6e73656374657475722061646970697363696e6720656c69742e204e616d207072657469756d2c20707572757320766974616520736f6c6c696369747564696e207661726975732c206e697369206c6563747573207665686963756c61206475692c207574206469676e697373696d2066656c697320646f6c6f7220626c616e646974206a7573746f2e20446f6e656320656c656966656e64206c656374757320757420666575676961742072686f6e6375732e20446f6e65632065726174206e6962682c2064617069627573206e6563206469616d2069642c206c6163696e6961206c6163696e6961206e69736c2e204d617572697320736167697474697320656666696369747572206e69736c2e2055742074696e636964756e7420656c656d656e74756d2072686f6e6375732e204372617320737573636970697420646f6c6f72207365642065737420756c747269636965732c20717569732064617069627573206e657175652073757363697069742e20457469616d20616320656e696d206575206c6967756c6120626962656e64756d20626c616e64697420717569732073697420616d65742066656c69732e205072616573656e74206d69206e6973692c206c75637475732073697420616d6574206e756e632075742c206665726d656e74756d2074656d7075732070757275732e2053757370656e64697373652076656c2070757275732061206e69626820616c697175616d2068656e6472657269742e20416c697175616d2073697420616d657420747269737469717565206c6f72656d2e2053656420656c656d656e74756d20636f6e67756520616e7465206964206d6f6c6c69732e20446f6e6563207669746165207072657469756d206e657175652e'",
+                id="b'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam pretium, purus vitae sollicitudin varius, nisi lectus vehicula dui, ut dignissim felis dolor blandit justo. Donec eleifend lectus ut feugiat rhoncus. Donec erat nibh, dapibus nec diam id, lacinia lacinia nisl. Mauris sagittis efficitur nisl. Ut tincidunt elementum rhoncus. Cras suscipit dolor sed est ultricies, quis dapibus neque suscipit. Etiam ac enim eu ligula bibendum blandit quis sit amet felis. Praesent mi nisi, luctus sit amet nunc ut, fermentum tempus purus. Suspendisse vel purus a nibh aliquam hendrerit. Aliquam sit amet tristique lorem. Sed elementum congue ante id mollis. Donec vitae pretium neque.'",
+            ),
+        ],
+    )
+    def test_translate_default_blob_bytes_from_mysql_to_sqlite(
+        self,
+        column_default: bytes,
+        sqlite_default_translation: str,
+    ) -> None:
+        assert (
+            MySQLtoSQLite._translate_default_from_mysql_to_sqlite(column_default, "BLOB") == sqlite_default_translation
+        )
+
+    @pytest.mark.parametrize(
         "collation, resulting_column_collation, column_type",
         [
             pytest.param(
                 CollatingSequences.BINARY,
                 "",
                 "CHARACTER",
-                id="{} (CHARACTER)".format(CollatingSequences.BINARY),
+                id=f"{CollatingSequences.BINARY} (CHARACTER)",
             ),
             pytest.param(
                 CollatingSequences.NOCASE,
-                "COLLATE {}".format(CollatingSequences.NOCASE),
+                f"COLLATE {CollatingSequences.NOCASE}",
                 "CHARACTER",
-                id="{} (CHARACTER)".format(CollatingSequences.NOCASE),
+                id=f"{CollatingSequences.NOCASE} (CHARACTER)",
             ),
             pytest.param(
                 CollatingSequences.RTRIM,
-                "COLLATE {}".format(CollatingSequences.RTRIM),
+                f"COLLATE {CollatingSequences.RTRIM}",
                 "CHARACTER",
-                id="{} (CHARACTER)".format(CollatingSequences.RTRIM),
+                id=f"{CollatingSequences.RTRIM} (CHARACTER)",
             ),
             pytest.param(
                 CollatingSequences.BINARY,
                 "",
                 "NCHAR",
-                id="{} (NCHAR)".format(CollatingSequences.BINARY),
+                id=f"{CollatingSequences.BINARY} (NCHAR)",
             ),
             pytest.param(
                 CollatingSequences.NOCASE,
-                "COLLATE {}".format(CollatingSequences.NOCASE),
+                f"COLLATE {CollatingSequences.NOCASE}",
                 "NCHAR",
-                id="{} (NCHAR)".format(CollatingSequences.NOCASE),
+                id=f"{CollatingSequences.NOCASE} (NCHAR)",
             ),
             pytest.param(
                 CollatingSequences.RTRIM,
-                "COLLATE {}".format(CollatingSequences.RTRIM),
+                f"COLLATE {CollatingSequences.RTRIM}",
                 "NCHAR",
-                id="{} (NCHAR)".format(CollatingSequences.RTRIM),
+                id=f"{CollatingSequences.RTRIM} (NCHAR)",
             ),
             pytest.param(
                 CollatingSequences.BINARY,
                 "",
                 "NVARCHAR",
-                id="{} (NVARCHAR)".format(CollatingSequences.BINARY),
+                id=f"{CollatingSequences.BINARY} (NVARCHAR)",
             ),
             pytest.param(
                 CollatingSequences.NOCASE,
-                "COLLATE {}".format(CollatingSequences.NOCASE),
+                f"COLLATE {CollatingSequences.NOCASE}",
                 "NVARCHAR",
-                id="{} (NVARCHAR)".format(CollatingSequences.NOCASE),
+                id=f"{CollatingSequences.NOCASE} (NVARCHAR)",
             ),
             pytest.param(
                 CollatingSequences.RTRIM,
-                "COLLATE {}".format(CollatingSequences.RTRIM),
+                f"COLLATE {CollatingSequences.RTRIM}",
                 "NVARCHAR",
-                id="{} (NVARCHAR)".format(CollatingSequences.RTRIM),
+                id=f"{CollatingSequences.RTRIM} (NVARCHAR)",
             ),
             pytest.param(
                 CollatingSequences.BINARY,
                 "",
                 "TEXT",
-                id="{} (TEXT)".format(CollatingSequences.BINARY),
+                id=f"{CollatingSequences.BINARY} (TEXT)",
             ),
             pytest.param(
                 CollatingSequences.NOCASE,
-                "COLLATE {}".format(CollatingSequences.NOCASE),
+                f"COLLATE {CollatingSequences.NOCASE}",
                 "TEXT",
-                id="{} (TEXT)".format(CollatingSequences.NOCASE),
+                id=f"{CollatingSequences.NOCASE} (TEXT)",
             ),
             pytest.param(
                 CollatingSequences.RTRIM,
-                "COLLATE {}".format(CollatingSequences.RTRIM),
+                f"COLLATE {CollatingSequences.RTRIM}",
                 "TEXT",
-                id="{} (TEXT)".format(CollatingSequences.RTRIM),
+                id=f"{CollatingSequences.RTRIM} (TEXT)",
             ),
             pytest.param(
                 CollatingSequences.BINARY,
                 "",
                 "VARCHAR",
-                id="{} (VARCHAR)".format(CollatingSequences.BINARY),
+                id=f"{CollatingSequences.BINARY} (VARCHAR)",
             ),
             pytest.param(
                 CollatingSequences.NOCASE,
-                "COLLATE {}".format(CollatingSequences.NOCASE),
+                f"COLLATE {CollatingSequences.NOCASE}",
                 "VARCHAR",
-                id="{} (VARCHAR)".format(CollatingSequences.NOCASE),
+                id=f"{CollatingSequences.NOCASE} (VARCHAR)",
             ),
             pytest.param(
                 CollatingSequences.RTRIM,
-                "COLLATE {}".format(CollatingSequences.RTRIM),
+                f"COLLATE {CollatingSequences.RTRIM}",
                 "VARCHAR",
-                id="{} (VARCHAR)".format(CollatingSequences.RTRIM),
+                id=f"{CollatingSequences.RTRIM} (VARCHAR)",
             ),
         ],
     )
     def test_data_type_collation_sequence_is_applied_on_textual_data_types(
         self,
-        collation,
-        resulting_column_collation,
-        column_type,
-    ):
-        assert (
-            MySQLtoSQLite._data_type_collation_sequence(collation, column_type)
-            == resulting_column_collation
-        )
+        collation: str,
+        resulting_column_collation: str,
+        column_type: str,
+    ) -> None:
+        assert MySQLtoSQLite._data_type_collation_sequence(collation, column_type) == resulting_column_collation
 
-    def test_data_type_collation_sequence_is_not_applied_on_non_textual_data_types(
-        self,
-    ):
+    def test_data_type_collation_sequence_is_not_applied_on_non_textual_data_types(self) -> None:
         for column_type in (
             "BIGINT",
             "BINARY",
             "BIT",
             "BLOB",
             "BOOLEAN",
             "DATE",
@@ -361,56 +338,59 @@
             "YEAR",
         ):
             for collation in (
                 CollatingSequences.BINARY,
                 CollatingSequences.NOCASE,
                 CollatingSequences.RTRIM,
             ):
-                assert (
-                    MySQLtoSQLite._data_type_collation_sequence(collation, column_type)
-                    == ""
-                )
+                assert MySQLtoSQLite._data_type_collation_sequence(collation, column_type) == ""
 
 
 @pytest.mark.exceptions
 @pytest.mark.usefixtures("mysql_instance")
 class TestMySQLtoSQLiteSQLExceptions:
     @pytest.mark.parametrize(
         "quiet",
         [
             pytest.param(False, id="verbose"),
             pytest.param(True, id="quiet"),
         ],
     )
     def test_create_table_server_lost_connection_error(
-        self, sqlite_database, mysql_database, mysql_credentials, mocker, caplog, quiet
-    ):
-        proc = MySQLtoSQLite(
+        self,
+        sqlite_database: "os.PathLike[t.Any]",
+        mysql_database: Database,
+        mysql_credentials: MySQLCredentials,
+        mocker: MockerFixture,
+        caplog: LogCaptureFixture,
+        quiet: bool,
+    ) -> None:
+        proc: MySQLtoSQLite = MySQLtoSQLite(  # type: ignore[call-arg]
             sqlite_file=sqlite_database,
             mysql_user=mysql_credentials.user,
             mysql_password=mysql_credentials.password,
             mysql_database=mysql_credentials.database,
             mysql_host=mysql_credentials.host,
             mysql_port=mysql_credentials.port,
             quiet=quiet,
         )
 
         class FakeSQLiteCursor:
-            def executescript(self, *args, **kwargs):
+            def executescript(self, *args, **kwargs) -> t.Any:
                 raise mysql.connector.Error(
                     msg="Error Code: 2013. Lost connection to MySQL server during query",
                     errno=errorcode.CR_SERVER_LOST,
                 )
 
         class FakeSQLiteConnector:
-            def commit(self, *args, **kwargs):
+            def commit(self, *args, **kwargs) -> t.Any:
                 return True
 
-        mysql_inspect = inspect(mysql_database.engine)
-        mysql_tables = mysql_inspect.get_table_names()
+        mysql_inspect: Inspector = inspect(mysql_database.engine)
+        mysql_tables: t.List[str] = mysql_inspect.get_table_names()
 
         mocker.patch.object(proc, "_sqlite_cur", FakeSQLiteCursor())
         mocker.patch.object(proc._mysql, "reconnect", return_value=True)
         mocker.patch.object(proc, "_sqlite", FakeSQLiteConnector())
         caplog.set_level(logging.DEBUG)
         with pytest.raises(mysql.connector.Error):
             proc._create_table(choice(mysql_tables))
@@ -419,66 +399,78 @@
         "quiet",
         [
             pytest.param(False, id="verbose"),
             pytest.param(True, id="quiet"),
         ],
     )
     def test_create_table_unknown_mysql_connector_error(
-        self, sqlite_database, mysql_database, mysql_credentials, mocker, caplog, quiet
-    ):
-        proc = MySQLtoSQLite(
+        self,
+        sqlite_database: "os.PathLike[t.Any]",
+        mysql_database: Database,
+        mysql_credentials: MySQLCredentials,
+        mocker: MockerFixture,
+        caplog: LogCaptureFixture,
+        quiet: bool,
+    ) -> None:
+        proc: MySQLtoSQLite = MySQLtoSQLite(  # type: ignore[call-arg]
             sqlite_file=sqlite_database,
             mysql_user=mysql_credentials.user,
             mysql_password=mysql_credentials.password,
             mysql_database=mysql_credentials.database,
             mysql_host=mysql_credentials.host,
             mysql_port=mysql_credentials.port,
             quiet=quiet,
         )
 
         class FakeSQLiteCursor:
-            def executescript(self, statement):
+            def executescript(self, statement: t.Any) -> t.Any:
                 raise mysql.connector.Error(
                     msg="Error Code: 2000. Unknown MySQL error",
                     errno=errorcode.CR_UNKNOWN_ERROR,
                 )
 
-        mysql_inspect = inspect(mysql_database.engine)
-        mysql_tables = mysql_inspect.get_table_names()
+        mysql_inspect: Inspector = inspect(mysql_database.engine)
+        mysql_tables: t.List[str] = mysql_inspect.get_table_names()
         mocker.patch.object(proc, "_sqlite_cur", FakeSQLiteCursor())
         caplog.set_level(logging.DEBUG)
         with pytest.raises(mysql.connector.Error):
             proc._create_table(choice(mysql_tables))
 
     @pytest.mark.parametrize(
         "quiet",
         [
             pytest.param(False, id="verbose"),
             pytest.param(True, id="quiet"),
         ],
     )
     def test_create_table_sqlite3_error(
-        self, sqlite_database, mysql_database, mysql_credentials, mocker, caplog, quiet
-    ):
-        proc = MySQLtoSQLite(
+        self,
+        sqlite_database: "os.PathLike[t.Any]",
+        mysql_database: Database,
+        mysql_credentials: MySQLCredentials,
+        mocker: MockerFixture,
+        caplog: LogCaptureFixture,
+        quiet: bool,
+    ) -> None:
+        proc: MySQLtoSQLite = MySQLtoSQLite(  # type: ignore[call-arg]
             sqlite_file=sqlite_database,
             mysql_user=mysql_credentials.user,
             mysql_password=mysql_credentials.password,
             mysql_database=mysql_credentials.database,
             mysql_host=mysql_credentials.host,
             mysql_port=mysql_credentials.port,
             quiet=quiet,
         )
 
         class FakeSQLiteCursor:
-            def executescript(self, *args, **kwargs):
+            def executescript(self, *args, **kwargs) -> t.Any:
                 raise sqlite3.Error("Unknown SQLite error")
 
-        mysql_inspect = inspect(mysql_database.engine)
-        mysql_tables = mysql_inspect.get_table_names()
+        mysql_inspect: Inspector = inspect(mysql_database.engine)
+        mysql_tables: t.List[str] = mysql_inspect.get_table_names()
         mocker.patch.object(proc, "_sqlite_cur", FakeSQLiteCursor())
         caplog.set_level(logging.DEBUG)
         with pytest.raises(sqlite3.Error):
             proc._create_table(choice(mysql_tables))
 
     @pytest.mark.parametrize(
         "exception, quiet",
@@ -511,60 +503,54 @@
                 mysql.connector.Error(
                     msg="Error Code: 2000. Unknown MySQL error",
                     errno=errorcode.CR_UNKNOWN_ERROR,
                 ),
                 True,
                 id="errorcode.CR_UNKNOWN_ERROR quiet",
             ),
-            pytest.param(
-                sqlite3.Error("Unknown SQLite error"), False, id="sqlite3.Error verbose"
-            ),
-            pytest.param(
-                sqlite3.Error("Unknown SQLite error"), True, id="sqlite3.Error quiet"
-            ),
+            pytest.param(sqlite3.Error("Unknown SQLite error"), False, id="sqlite3.Error verbose"),
+            pytest.param(sqlite3.Error("Unknown SQLite error"), True, id="sqlite3.Error quiet"),
         ],
     )
     def test_transfer_table_data_exceptions(
         self,
-        sqlite_database,
-        mysql_database,
-        mysql_credentials,
-        mocker,
-        caplog,
-        exception,
-        quiet,
-    ):
-        proc = MySQLtoSQLite(
+        sqlite_database: "os.PathLike[t.Any]",
+        mysql_database: Database,
+        mysql_credentials: MySQLCredentials,
+        mocker: MockerFixture,
+        caplog: LogCaptureFixture,
+        exception: Exception,
+        quiet: bool,
+    ) -> None:
+        proc: MySQLtoSQLite = MySQLtoSQLite(  # type: ignore[call-arg]
             sqlite_file=sqlite_database,
             mysql_user=mysql_credentials.user,
             mysql_password=mysql_credentials.password,
             mysql_database=mysql_credentials.database,
             mysql_host=mysql_credentials.host,
             mysql_port=mysql_credentials.port,
             quiet=quiet,
         )
 
         class FakeMySQLCursor:
-            def fetchall(self):
+            def fetchall(self) -> t.Any:
                 raise exception
 
-            def fetchmany(self, size=1):
+            def fetchmany(self, size: int = 1) -> t.Any:
                 raise exception
 
-        mysql_inspect = inspect(mysql_database.engine)
-        mysql_tables = mysql_inspect.get_table_names()
+        mysql_inspect: Inspector = inspect(mysql_database.engine)
+        mysql_tables: t.List[str] = mysql_inspect.get_table_names()
 
-        table_name = choice(mysql_tables)
-        columns = [column["name"] for column in mysql_inspect.get_columns(table_name)]
+        table_name: str = choice(mysql_tables)
+        columns: t.List[str] = [column["name"] for column in mysql_inspect.get_columns(table_name)]
 
-        sql = (
-            'INSERT OR IGNORE INTO "{table}" ({fields}) VALUES ({placeholders})'.format(
-                table=table_name,
-                fields=('"{}", ' * len(columns)).rstrip(" ,").format(*columns),
-                placeholders=("?, " * len(columns)).rstrip(" ,"),
-            )
+        sql: str = 'INSERT OR IGNORE INTO "{table}" ({fields}) VALUES ({placeholders})'.format(
+            table=table_name,
+            fields=('"{}", ' * len(columns)).rstrip(" ,").format(*columns),
+            placeholders=("?, " * len(columns)).rstrip(" ,"),
         )
 
         mocker.patch.object(proc, "_mysql_cur", FakeMySQLCursor())
 
         with pytest.raises((mysql.connector.Error, sqlite3.Error)):
             proc._transfer_table_data(table_name, sql)
```

