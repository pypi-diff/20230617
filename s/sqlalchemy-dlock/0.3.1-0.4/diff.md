# Comparing `tmp/sqlalchemy-dlock-0.3.1.tar.gz` & `tmp/sqlalchemy-dlock-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-dlock-0.3.1.tar", last modified: Thu Jun 15 02:24:29 2023, max compression
+gzip compressed data, was "sqlalchemy-dlock-0.4.tar", last modified: Sat Jun 17 13:42:00 2023, max compression
```

## Comparing `sqlalchemy-dlock-0.3.1.tar` & `sqlalchemy-dlock-0.4.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:24:29.933449 sqlalchemy-dlock-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-06-15 02:24:29.933449 sqlalchemy-dlock-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 02:24:29.933449 sqlalchemy-dlock-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:24:29.925449 sqlalchemy-dlock-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:24:29.929449 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:24:29.933449 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/asyncio/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:24:29.933449 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/asyncio/impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/asyncio/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/asyncio/impl/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/asyncio/impl/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/asyncio/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:24:29.933449 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/impl/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/impl/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-15 02:24:19.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-15 02:24:29.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 02:24:29.929449 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-06-15 02:24:29.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-15 02:24:29.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 02:24:29.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 02:24:29.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-15 02:24:29.000000 sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:42:00.618011 sqlalchemy-dlock-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-17 13:41:52.000000 sqlalchemy-dlock-0.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-06-17 13:41:52.000000 sqlalchemy-dlock-0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-17 13:41:52.000000 sqlalchemy-dlock-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-17 13:41:52.000000 sqlalchemy-dlock-0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-06-17 13:42:00.618011 sqlalchemy-dlock-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-06-17 13:41:52.000000 sqlalchemy-dlock-0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-17 13:41:52.000000 sqlalchemy-dlock-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 13:42:00.618011 sqlalchemy-dlock-0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:42:00.614011 sqlalchemy-dlock-0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:42:00.618011 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-17 13:41:52.000000 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:42:00.618011 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-17 13:41:52.000000 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-17 13:41:52.000000 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/asyncio/baselock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-17 13:41:52.000000 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/asyncio/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:42:00.618011 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/asyncio/lock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 13:41:52.000000 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/asyncio/lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-17 13:41:52.000000 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/asyncio/lock/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-17 13:41:52.000000 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/asyncio/lock/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-06-17 13:41:52.000000 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/baselock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-17 13:41:52.000000 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-17 13:41:52.000000 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:42:00.618011 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/lock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 13:41:52.000000 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/lock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-06-17 13:41:52.000000 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/lock/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-17 13:41:52.000000 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/lock/postgresql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:42:00.618011 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/statement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 13:41:52.000000 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-17 13:41:52.000000 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/statement/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-17 13:41:52.000000 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/statement/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-17 13:41:52.000000 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-17 13:42:00.000000 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:42:00.618011 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-06-17 13:42:00.000000 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-17 13:42:00.000000 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 13:42:00.000000 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-17 13:42:00.000000 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-17 13:42:00.000000 sqlalchemy-dlock-0.4/src/sqlalchemy_dlock.egg-info/top_level.txt
```

### Comparing `sqlalchemy-dlock-0.3.1/CHANGELOG.md` & `sqlalchemy-dlock-0.4/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,27 @@
 # CHANGELOG
 
+## v0.4
+
+Date: 2023-06-17
+
+- Remove:
+  - remove `acquired` property, it's alias of `locked`
+  - remove setter of `locked` property
+
+- Optimize:
+  - re-arrange package's structure
+  - Many optimizations
+
+- CI/Test:
+  - Github action: Python 3.8~3.11 x SQLAlchemy 1.x/2.x matrix testing
+  - Local compose: Python 3.7~3.11 x SQLAlchemy 1.x/2.x matrix testing
+
+- Doc: Update to Sphinx 7.x, and Furo theme
+
 ## v0.3.1
 
 Date: 2023-06-13
 
 - A hotfix for project's dependencies setup error.
 
 ## v0.3
```

### Comparing `sqlalchemy-dlock-0.3.1/LICENSE` & `sqlalchemy-dlock-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-dlock-0.3.1/PKG-INFO` & `sqlalchemy-dlock-0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,33 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-dlock
-Version: 0.3.1
+Version: 0.4
 Summary: A distributed lock implementation based on SQLAlchemy
 Author-email: liu xue yan <liu_xue_yan@foxmail.com>
-License: BSD 3-Clause License
-        
-        Copyright (c) 2020, liu xue yan
-        All rights reserved.
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        1. Redistributions of source code must retain the above copyright notice, this
-           list of conditions and the following disclaimer.
-        
-        2. Redistributions in binary form must reproduce the above copyright notice,
-           this list of conditions and the following disclaimer in the documentation
-           and/or other materials provided with the distribution.
-        
-        3. Neither the name of the copyright holder nor the names of its
-           contributors may be used to endorse or promote products derived from
-           this software without specific prior written permission.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
+License: BSD-3-Clause
 Project-URL: homepage, https://github.com/tanbro/sqlalchemy-dlock
+Project-URL: documentation, https://sqlalchemy-dlock.readthedocs.io/
 Project-URL: repository, https://github.com/tanbro/sqlalchemy-dlock.git
 Keywords: SQLAlchemy,lock,distributed,distributed lock,SQL,database,DBMS
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: asyncio
+Provides-Extra: mysqlclient
+Provides-Extra: pymysql
+Provides-Extra: aiomysql
+Provides-Extra: psycopg2
+Provides-Extra: psycopg2-binary
+Provides-Extra: psycopg3
+Provides-Extra: psycopg3-binary
+Provides-Extra: psycopg3-c
+Provides-Extra: asyncpg3
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # SQLAlchemy-DLock
 
 [![Python package](https://github.com/tanbro/sqlalchemy-dlock/actions/workflows/python-package.yml/badge.svg)](https://github.com/tanbro/sqlalchemy-dlock/actions/workflows/python-package.yml)
 [![PyPI](https://img.shields.io/pypi/v/sqlalchemy-dlock)](https://pypi.org/project/sqlalchemy-dlock/)
@@ -58,172 +39,220 @@
 It currently supports below locks:
 
  Database  |                                             Lock
 ---------- | ---------------------------------------------------------------------------------------------
 MySQL      | [named lock](https://dev.mysql.com/doc/refman/8.0/en/locking-functions.html)
 PostgreSQL | [advisory lock](https://www.postgresql.org/docs/current/explicit-locking.html#ADVISORY-LOCKS)
 
-## Usages
+## Install
+
+```bash
+pip install sqlalchemy-dlock
+```
+
+## Usage
 
 - Work with [SQLAlchemy][] `Connection`:
 
   ```python
   from sqlalchemy import create_engine
   from sqlalchemy_dlock import create_sadlock
 
   key = 'user/001'
 
-  engine = create_engine('postgresql://scott:tiger@localhost/')
+  engine = create_engine('postgresql://scott:tiger@127.0.0.1/')
   conn = engine.connect()
 
   # Create the D-Lock on the connection
   lock = create_sadlock(conn, key)
 
   # it's not lock when constructed
-  assert not lock.acquired
+  assert not lock.locked
 
   # lock
   lock.acquire()
-  assert lock.acquired
+  assert lock.locked
 
   # un-lock
   lock.release()
-  assert not lock.acquired
+  assert not lock.locked
   ```
 
 - `with` statement
 
   ```python
   from contextlib import closing
 
   from sqlalchemy import create_engine
   from sqlalchemy_dlock import create_sadlock
 
   key = 'user/001'
 
-  engine = create_engine('postgresql://scott:tiger@localhost/')
+  engine = create_engine('postgresql://scott:tiger@127.0.0.1/')
   with engine.connect() as conn:
 
       # Create the D-Lock on the connection
       with create_sadlock(conn, key) as lock:
           # It's locked
-          assert lock.acquired
+          assert lock.locked
 
       # Auto un-locked
-      assert not lock.acquired
+      assert not lock.locked
 
       # If do not want to be locked in `with`, a `closing` wrapper may help
       with closing(create_sadlock(conn, key)) as lock2:
-          # It's NOT locked here
-          assert not lock2.acquired
+          # It's NOT locked here !!!
+          assert not lock2.locked
           # lock it now:
           lock2.acquire()
-          assert lock2.acquired
+          assert lock2.locked
 
       # Auto un-locked
-      assert not lock2.acquired
+      assert not lock2.locked
   ```
 
 - Work with [SQLAlchemy][] `ORM` session:
 
   ```python
   from sqlalchemy import create_engine
   from sqlalchemy.orm import sessionmaker
   from sqlalchemy_dlock import create_sadlock
 
   key = 'user/001'
 
-  engine = create_engine('postgresql://scott:tiger@localhost/')
+  engine = create_engine('postgresql://scott:tiger@127.0.0.1/')
   Session = sessionmaker(bind=engine)
 
   with Session() as session:
     with create_sadlock(session, key) as lock:
-        assert lock.acquired
-    assert not lock.acquired
+        assert lock.locked
+    assert not lock.locked
   ```
 
 - Asynchronous I/O Support
 
-  > ℹ️ **info**:
+  > **Note**:
   >
   > - [SQLAlchemy][] `1.x`: <https://docs.sqlalchemy.org/14/orm/extensions/asyncio.html>
   > - [SQLAlchemy][] `2.x`: <https://docs.sqlalchemy.org/20/orm/extensions/asyncio.html>
 
   ```python
   from sqlalchemy.ext.asyncio import create_async_engine
   from sqlalchemy_dlock.asyncio import create_async_sadlock
 
   key = 'user/001'
 
-  engine = create_async_engine('postgresql+asyncpg://scott:tiger@localhost/')
+  engine = create_async_engine('postgresql+asyncpg://scott:tiger@127.0.0.1/')
 
   async with engine.begin() as conn:
       async with create_async_sadlock(conn, key) as lock:
           assert lock.locked
           await lock.release()
           assert not lock.locked
           await lock.acquire()
       assert not lock.locked
   ```
 
-## Tests
+  > **Note**:
+  >
+  > [aiomysql][], [asyncpg][] and [psycopg][] are tested asynchronous drivers
+  >
+  > We can install asynchronous DB libraries like one of blows:
+  >
+  > - ```bash
+  >   pip install sqlalchemy-dlock[asyncpg]
+  >   ```
+  >
+  > - ```bash
+  >   pip install sqlalchemy-dlock[asyncio] aiomysql
+  >   ```
+  >
+  > - ```bash
+  >   pip install SQLALchemy[asyncio] sqlalchemy-dlock psycopg
+  >   ```
+
+## Test
 
-Following [SQLAlchemy][] engines are tested:
+Following drivers are tested:
 
 - MySQL:
+  - [mysqlclient][] (synchronous)
+  - [pymysql][] (synchronous)
+  - [aiomysql][] (asynchronous)
+- Postgres:
+  - [psycopg2][] (asynchronous)
+  - [asyncpg][] (asynchronous)
+  - [psycopg][] (synchronous and asynchronous)
 
-  - mysqlclient
-  - PyMySQL
-  - aiomysql ([asyncio][])
+You can run unit-tests
 
-- Postgres:
+- on local environment:
 
-  - psycopg2
-  - asyncpg ([asyncio][])
+  1. Install the project with drivers and `asyncio` extra requires, a virtual environment ([venv][]) is strongly advised:
 
-You can run unit-tests:
+     ```bash
+     pip install -e .[mysqlclient psycopg2-binary aiomysql asyncpg]
+     ```
 
-- directly:
+  1. start up mysql and postgresql
 
-  1. Install the project (A virtual environment ([venv][]) is strongly advised):
+     There is a docker [compose][] file `db.docker-compose.yml` in the project dir,
+     which can be used to run mysql and postgresql develop environment conveniently:
 
      ```bash
-     pip install -e .
+     docker compose -f db.docker-compose.yml up
      ```
 
-  1. Start up your mysql and postgresql
-
-  1. Set environment variables `TEST_URLS` and `TEST_ASYNC_URLS` for sync and async database connection url.
+  1. set environment variables `TEST_URLS` and `TEST_ASYNC_URLS` for sync and async database connection url.
      Multiple connections separated by space.
      The test cases load environment variables in `tests/.env`.
 
      eg (and also the defaults):
 
      ```ini
-     TEST_URLS=mysql://test:test@localhost/test postgresql://postgres:test@localhost/
-     TEST_ASYNC_URLS=mysql+aiomysql://test:test@localhost/test postgresql+asyncpg://postgres:test@localhost/
+     TEST_URLS=mysql://test:test@127.0.0.1/test postgresql://postgres:test@127.0.0.1/
+     TEST_ASYNC_URLS=mysql+aiomysql://test:test@127.0.0.1/test postgresql+asyncpg://postgres:test@127.0.0.1/
      ```
 
   1. run unit-test
 
      ```bash
      python -m unittest
      ```
 
-- in docker-compose:
+- or on docker-compose:
 
   1. build the project
 
      ```bash
      python -m pip install build && python -m build -w
      ```
 
   1. run unit-test
 
+     Name of services for Python and [SQLAlchemy][] version matrix in the [compose][] file has such format:
+
+         python{{X.Y}}-sqlalchemy{{X}}
+
+     For example, if want to take a test for Python `3.9` and [SQLAlchemy][] `2.x`, we shall up to run unit-tests as below:
+
+     ```bash
+     cd tests
+     docker compose up python3.9-sqlalchemy2
+     ```
+
+     For Python `3.8` and [SQLAlchemy][] `1.x`:
+
      ```bash
      cd tests
-     docker compose up
+     docker compose up python3.8-sqlalchemy1
      ```
 
 [SQLAlchemy]: https://www.sqlalchemy.org/ "The Python SQL Toolkit and Object Relational Mapper"
-[asyncio]: https://docs.python.org/library/asyncio.html "asyncio is a library to write concurrent code using the async/await syntax."
 [venv]: https://docs.python.org/library/venv.html "The venv module supports creating lightweight “virtual environments”, each with their own independent set of Python packages installed in their site directories. "
+[mysqlclient]: https://pypi.org/project/mysqlclient/ "Python interface to MySQL"
+[psycopg2]: https://pypi.org/project/psycopg2/ "PostgreSQL database adapter for Python"
+[psycopg]: https://pypi.org/project/psycopg/ "Psycopg 3 is a modern implementation of a PostgreSQL adapter for Python."
+[aiomysql]: https://pypi.org/project/aiomysql/ "aiomysql is a “driver” for accessing a MySQL database from the asyncio (PEP-3156/tulip) framework."
+[asyncpg]: https://pypi.org/project/asyncpg/ "asyncpg is a database interface library designed specifically for PostgreSQL and Python/asyncio. "
+[pymysql]: https://pypi.org/project/pymysql/ "Pure Python MySQL Driver"
+[compose]: https://docs.docker.com/compose/ "Compose is a tool for defining and running multi-container Docker applications."
```

### Comparing `sqlalchemy-dlock-0.3.1/README.md` & `sqlalchemy-dlock-0.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -10,172 +10,220 @@
 It currently supports below locks:
 
  Database  |                                             Lock
 ---------- | ---------------------------------------------------------------------------------------------
 MySQL      | [named lock](https://dev.mysql.com/doc/refman/8.0/en/locking-functions.html)
 PostgreSQL | [advisory lock](https://www.postgresql.org/docs/current/explicit-locking.html#ADVISORY-LOCKS)
 
-## Usages
+## Install
+
+```bash
+pip install sqlalchemy-dlock
+```
+
+## Usage
 
 - Work with [SQLAlchemy][] `Connection`:
 
   ```python
   from sqlalchemy import create_engine
   from sqlalchemy_dlock import create_sadlock
 
   key = 'user/001'
 
-  engine = create_engine('postgresql://scott:tiger@localhost/')
+  engine = create_engine('postgresql://scott:tiger@127.0.0.1/')
   conn = engine.connect()
 
   # Create the D-Lock on the connection
   lock = create_sadlock(conn, key)
 
   # it's not lock when constructed
-  assert not lock.acquired
+  assert not lock.locked
 
   # lock
   lock.acquire()
-  assert lock.acquired
+  assert lock.locked
 
   # un-lock
   lock.release()
-  assert not lock.acquired
+  assert not lock.locked
   ```
 
 - `with` statement
 
   ```python
   from contextlib import closing
 
   from sqlalchemy import create_engine
   from sqlalchemy_dlock import create_sadlock
 
   key = 'user/001'
 
-  engine = create_engine('postgresql://scott:tiger@localhost/')
+  engine = create_engine('postgresql://scott:tiger@127.0.0.1/')
   with engine.connect() as conn:
 
       # Create the D-Lock on the connection
       with create_sadlock(conn, key) as lock:
           # It's locked
-          assert lock.acquired
+          assert lock.locked
 
       # Auto un-locked
-      assert not lock.acquired
+      assert not lock.locked
 
       # If do not want to be locked in `with`, a `closing` wrapper may help
       with closing(create_sadlock(conn, key)) as lock2:
-          # It's NOT locked here
-          assert not lock2.acquired
+          # It's NOT locked here !!!
+          assert not lock2.locked
           # lock it now:
           lock2.acquire()
-          assert lock2.acquired
+          assert lock2.locked
 
       # Auto un-locked
-      assert not lock2.acquired
+      assert not lock2.locked
   ```
 
 - Work with [SQLAlchemy][] `ORM` session:
 
   ```python
   from sqlalchemy import create_engine
   from sqlalchemy.orm import sessionmaker
   from sqlalchemy_dlock import create_sadlock
 
   key = 'user/001'
 
-  engine = create_engine('postgresql://scott:tiger@localhost/')
+  engine = create_engine('postgresql://scott:tiger@127.0.0.1/')
   Session = sessionmaker(bind=engine)
 
   with Session() as session:
     with create_sadlock(session, key) as lock:
-        assert lock.acquired
-    assert not lock.acquired
+        assert lock.locked
+    assert not lock.locked
   ```
 
 - Asynchronous I/O Support
 
-  > ℹ️ **info**:
+  > **Note**:
   >
   > - [SQLAlchemy][] `1.x`: <https://docs.sqlalchemy.org/14/orm/extensions/asyncio.html>
   > - [SQLAlchemy][] `2.x`: <https://docs.sqlalchemy.org/20/orm/extensions/asyncio.html>
 
   ```python
   from sqlalchemy.ext.asyncio import create_async_engine
   from sqlalchemy_dlock.asyncio import create_async_sadlock
 
   key = 'user/001'
 
-  engine = create_async_engine('postgresql+asyncpg://scott:tiger@localhost/')
+  engine = create_async_engine('postgresql+asyncpg://scott:tiger@127.0.0.1/')
 
   async with engine.begin() as conn:
       async with create_async_sadlock(conn, key) as lock:
           assert lock.locked
           await lock.release()
           assert not lock.locked
           await lock.acquire()
       assert not lock.locked
   ```
 
-## Tests
+  > **Note**:
+  >
+  > [aiomysql][], [asyncpg][] and [psycopg][] are tested asynchronous drivers
+  >
+  > We can install asynchronous DB libraries like one of blows:
+  >
+  > - ```bash
+  >   pip install sqlalchemy-dlock[asyncpg]
+  >   ```
+  >
+  > - ```bash
+  >   pip install sqlalchemy-dlock[asyncio] aiomysql
+  >   ```
+  >
+  > - ```bash
+  >   pip install SQLALchemy[asyncio] sqlalchemy-dlock psycopg
+  >   ```
+
+## Test
 
-Following [SQLAlchemy][] engines are tested:
+Following drivers are tested:
 
 - MySQL:
+  - [mysqlclient][] (synchronous)
+  - [pymysql][] (synchronous)
+  - [aiomysql][] (asynchronous)
+- Postgres:
+  - [psycopg2][] (asynchronous)
+  - [asyncpg][] (asynchronous)
+  - [psycopg][] (synchronous and asynchronous)
 
-  - mysqlclient
-  - PyMySQL
-  - aiomysql ([asyncio][])
+You can run unit-tests
 
-- Postgres:
+- on local environment:
 
-  - psycopg2
-  - asyncpg ([asyncio][])
+  1. Install the project with drivers and `asyncio` extra requires, a virtual environment ([venv][]) is strongly advised:
 
-You can run unit-tests:
+     ```bash
+     pip install -e .[mysqlclient psycopg2-binary aiomysql asyncpg]
+     ```
 
-- directly:
+  1. start up mysql and postgresql
 
-  1. Install the project (A virtual environment ([venv][]) is strongly advised):
+     There is a docker [compose][] file `db.docker-compose.yml` in the project dir,
+     which can be used to run mysql and postgresql develop environment conveniently:
 
      ```bash
-     pip install -e .
+     docker compose -f db.docker-compose.yml up
      ```
 
-  1. Start up your mysql and postgresql
-
-  1. Set environment variables `TEST_URLS` and `TEST_ASYNC_URLS` for sync and async database connection url.
+  1. set environment variables `TEST_URLS` and `TEST_ASYNC_URLS` for sync and async database connection url.
      Multiple connections separated by space.
      The test cases load environment variables in `tests/.env`.
 
      eg (and also the defaults):
 
      ```ini
-     TEST_URLS=mysql://test:test@localhost/test postgresql://postgres:test@localhost/
-     TEST_ASYNC_URLS=mysql+aiomysql://test:test@localhost/test postgresql+asyncpg://postgres:test@localhost/
+     TEST_URLS=mysql://test:test@127.0.0.1/test postgresql://postgres:test@127.0.0.1/
+     TEST_ASYNC_URLS=mysql+aiomysql://test:test@127.0.0.1/test postgresql+asyncpg://postgres:test@127.0.0.1/
      ```
 
   1. run unit-test
 
      ```bash
      python -m unittest
      ```
 
-- in docker-compose:
+- or on docker-compose:
 
   1. build the project
 
      ```bash
      python -m pip install build && python -m build -w
      ```
 
   1. run unit-test
 
+     Name of services for Python and [SQLAlchemy][] version matrix in the [compose][] file has such format:
+
+         python{{X.Y}}-sqlalchemy{{X}}
+
+     For example, if want to take a test for Python `3.9` and [SQLAlchemy][] `2.x`, we shall up to run unit-tests as below:
+
+     ```bash
+     cd tests
+     docker compose up python3.9-sqlalchemy2
+     ```
+
+     For Python `3.8` and [SQLAlchemy][] `1.x`:
+
      ```bash
      cd tests
-     docker compose up
+     docker compose up python3.8-sqlalchemy1
      ```
 
 [SQLAlchemy]: https://www.sqlalchemy.org/ "The Python SQL Toolkit and Object Relational Mapper"
-[asyncio]: https://docs.python.org/library/asyncio.html "asyncio is a library to write concurrent code using the async/await syntax."
 [venv]: https://docs.python.org/library/venv.html "The venv module supports creating lightweight “virtual environments”, each with their own independent set of Python packages installed in their site directories. "
+[mysqlclient]: https://pypi.org/project/mysqlclient/ "Python interface to MySQL"
+[psycopg2]: https://pypi.org/project/psycopg2/ "PostgreSQL database adapter for Python"
+[psycopg]: https://pypi.org/project/psycopg/ "Psycopg 3 is a modern implementation of a PostgreSQL adapter for Python."
+[aiomysql]: https://pypi.org/project/aiomysql/ "aiomysql is a “driver” for accessing a MySQL database from the asyncio (PEP-3156/tulip) framework."
+[asyncpg]: https://pypi.org/project/asyncpg/ "asyncpg is a database interface library designed specifically for PostgreSQL and Python/asyncio. "
+[pymysql]: https://pypi.org/project/pymysql/ "Pure Python MySQL Driver"
+[compose]: https://docs.docker.com/compose/ "Compose is a tool for defining and running multi-container Docker applications."
```

### Comparing `sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/asyncio/functions.py` & `sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/asyncio/functions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from importlib import import_module
 
+from sqlalchemy.engine import Connection
 from sqlalchemy.ext.asyncio import AsyncConnection
 
 from ..utils import safe_name
-from .types import BaseAsyncSadLock, TAsyncConnectionOrSession
+from .baselock import BaseAsyncSadLock, TAsyncConnectionOrSession
 
 __all__ = ["create_async_sadlock"]
 
 
-def create_async_sadlock(connection_or_engine: TAsyncConnectionOrSession, key, *args, **kwargs) -> BaseAsyncSadLock:
-    if isinstance(connection_or_engine, AsyncConnection):
-        name = safe_name(connection_or_engine.sync_engine.engine.name)
+def create_async_sadlock(connection_or_session: TAsyncConnectionOrSession, key, *args, **kwargs) -> BaseAsyncSadLock:
+    if isinstance(connection_or_session, AsyncConnection):
+        sync_engine = connection_or_session.sync_engine
     else:
-        name = safe_name(connection_or_engine.get_bind().name)
+        bind = connection_or_session.get_bind()
+        if isinstance(bind, Connection):
+            sync_engine = bind.engine
+        else:
+            sync_engine = bind
+    engine_name = safe_name(sync_engine.name)
     try:
-        mod = import_module("..impl.{}".format(name), __name__)
+        mod = import_module(f"..lock.{engine_name}", __name__)
     except ImportError as exception:  # pragma: no cover
-        raise NotImplementedError("{}: {}".format(name, exception))
+        raise NotImplementedError(f"{engine_name}: {exception}")
     lock_cls = getattr(mod, "AsyncSadLock")
-    return lock_cls(connection_or_engine, key, *args, **kwargs)
+    return lock_cls(connection_or_session, key, *args, **kwargs)
```

### Comparing `sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/asyncio/impl/mysql.py` & `sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/lock/mysql.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,107 +1,104 @@
-from textwrap import dedent
 from typing import Any, Callable, Optional, Union
 
-from sqlalchemy import text
-
-from ...exceptions import SqlAlchemyDLockDatabaseError
-from ..types import BaseAsyncSadLock, TAsyncConnectionOrSession
+from ..exceptions import SqlAlchemyDLockDatabaseError
+from ..statement.mysql import STATEMENTS
+from ..baselock import BaseSadLock, TConnectionOrSession
 
 MYSQL_LOCK_NAME_MAX_LENGTH = 64
 
-GET_LOCK = text(
-    dedent(
-        """
-        SELECT GET_LOCK(:str, :timeout)
-        """
-    ).strip()
-)
-
-RELEASE_LOCK = text(
-    dedent(
-        """
-        SELECT RELEASE_LOCK(:str)
-        """
-    ).strip()
-)
-
 TConvertFunction = Callable[[Any], str]
 
 
 def default_convert(key: Union[bytearray, bytes, int, float]) -> str:
     if isinstance(key, (bytearray, bytes)):
         result = key.decode()
     elif isinstance(key, (int, float)):
         result = str(key)
     else:
-        raise TypeError("{}".format(type(key)))
+        raise TypeError(f"{type(key)}")
     return result
 
 
-class AsyncSadLock(BaseAsyncSadLock):
-    def __init__(
-        self,
-        connection_or_session: TAsyncConnectionOrSession,
-        key,
-        convert: Optional[TConvertFunction] = None,
-    ):
+class SadLock(BaseSadLock):
+    """MySQL named-lock
+
+    .. seealso:: https://dev.mysql.com/doc/refman/8.0/en/locking-functions.html
+    """
+
+    def __init__(self, connection_or_session: TConnectionOrSession, key, convert: Optional[TConvertFunction] = None):
+        """
+        MySQL named lock requires the key given by string.
+
+        If `key` is not a :class:`str`:
+
+        - When :class:`bytes` or alike, the constructor tries to decode it with default encoding::
+
+            key = key.decode()
+
+        - Otherwise the constructor force convert it to :class:`str`::
+
+            key = str(key)
+
+        - Or you can specify a ``convert`` function to that argument.
+          The function is like::
+
+            def convert(val: Any) -> str:
+                # do something with `val`...
+                return string
+        """
         if convert:
             key = convert(key)
         elif not isinstance(key, str):
             key = default_convert(key)
         if not isinstance(key, str):
             raise TypeError("MySQL named lock requires the key given by string")
         if len(key) > MYSQL_LOCK_NAME_MAX_LENGTH:
-            raise ValueError(
-                "MySQL enforces a maximum length on lock names of {} characters.".format(MYSQL_LOCK_NAME_MAX_LENGTH)
-            )
+            raise ValueError(f"MySQL enforces a maximum length on lock names of {MYSQL_LOCK_NAME_MAX_LENGTH} characters.")
         #
         super().__init__(connection_or_session, key)
 
-    async def acquire(self, block: bool = True, timeout: Union[float, int, None] = None) -> bool:
+    def acquire(self, block: bool = True, timeout: Union[float, int, None] = None) -> bool:
         if self._acquired:
             raise ValueError("invoked on a locked lock")
         if block:
             # None: set the timeout period to infinite.
             if timeout is None:
                 timeout = -1
             # negative value for `timeout` are equivalent to a `timeout` of zero
             elif timeout < 0:
                 timeout = 0
         else:
             timeout = 0
-        stmt = GET_LOCK.params(str=self._key, timeout=timeout)
-        r = await self.connection_or_session.stream(stmt)
-        ret_val = (await r.one())[0]
-
+        stmt = STATEMENTS["lock"].params(str=self._key, timeout=timeout)
+        ret_val = self.connection_or_session.execute(stmt).scalar_one()
         if ret_val == 1:
             self._acquired = True
         elif ret_val == 0:
             pass  # 直到超时也没有成功锁定
         elif ret_val is None:  # pragma: no cover
-            raise SqlAlchemyDLockDatabaseError('An error occurred while attempting to obtain the lock "{}"'.format(self._key))
+            raise SqlAlchemyDLockDatabaseError(f"An error occurred while attempting to obtain the lock {self._key!r}")
         else:  # pragma: no cover
-            raise SqlAlchemyDLockDatabaseError('GET_LOCK("{}", {}) returns {}'.format(self._key, timeout, ret_val))
+            raise SqlAlchemyDLockDatabaseError(f"GET_LOCK({self._key!r}, {timeout}) returns {ret_val}")
         return self._acquired
 
-    async def release(self):
+    def release(self):
         if not self._acquired:
             raise ValueError("invoked on an unlocked lock")
-        stmt = RELEASE_LOCK.params(str=self._key)
-        r = await self.connection_or_session.stream(stmt)
-        ret_val = (await r.one())[0]
+        stmt = STATEMENTS["unlock"].params(str=self._key)
+        ret_val = self.connection_or_session.execute(stmt).scalar_one()
         if ret_val == 1:
             self._acquired = False
         elif ret_val == 0:  # pragma: no cover
             self._acquired = False
             raise SqlAlchemyDLockDatabaseError(
-                'The named lock "{}" was not established by this thread, ' "and the lock is not released.".format(self._key)
+                f"The named lock {self._key!r} was not established by this thread, and the lock is not released."
             )
         elif ret_val is None:  # pragma: no cover
             self._acquired = False
             raise SqlAlchemyDLockDatabaseError(
-                'The named lock "{}" did not exist, '
+                f"The named lock {self._key!r} did not exist, "
                 "was never obtained by a call to GET_LOCK(), "
-                "or has previously been released.".format(self._key)
+                "or has previously been released."
             )
-        else:
-            raise SqlAlchemyDLockDatabaseError('RELEASE_LOCK("{}") returns {}'.format(self._key, ret_val))
+        else:  # pragma: no cover
+            raise SqlAlchemyDLockDatabaseError(f"RELEASE_LOCK({self._key!r}) returns {ret_val}")
```

### Comparing `sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/asyncio/types.py` & `sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/asyncio/baselock.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,45 @@
 from typing import Any, Union
 
-from sqlalchemy.ext.asyncio import (AsyncConnection, AsyncSession,
-                                    async_scoped_session)
+from sqlalchemy.ext.asyncio import AsyncConnection, AsyncSession, async_scoped_session
 
-TAsyncConnectionOrSession = Union[AsyncConnection,
-                                  AsyncSession, async_scoped_session]
+TAsyncConnectionOrSession = Union[AsyncConnection, AsyncSession, async_scoped_session]
 
 
 class BaseAsyncSadLock:
-    def __init__(self,
-                 connection_or_session: TAsyncConnectionOrSession,
-                 key: Any,
-                 *args, **kwargs
-                 ):
+    def __init__(self, connection_or_session: TAsyncConnectionOrSession, key: Any, *args, **kwargs):
         self._acquired = False
         self._connection_or_session = connection_or_session
         self._key = key
 
     async def __aenter__(self):
         await self.acquire()
         return self
 
-    async def __aexit__(self, type_, value, traceback):
+    async def __aexit__(self, exc_type, exc_value, exc_tb):
         await self.close()
 
     def __str__(self):  # pragma: no cover
-        return '<{} {} key={} at 0x{:x}>'.format(
-            'locked' if self._acquired else 'unlocked',
-            self.__class__.__name__,
-            self._key, id(self)
+        return "<{} {} key={} at 0x{:x}>".format(
+            "locked" if self._acquired else "unlocked", self.__class__.__name__, self._key, id(self)
         )
 
     @property
     def connection_or_session(self) -> TAsyncConnectionOrSession:
         return self._connection_or_session
 
     @property
     def key(self):
         return self._key
 
     @property
-    def acquired(self) -> bool:
-        return self._acquired
-
-    @property
     def locked(self) -> bool:
-        return self.acquired
+        return self._acquired
 
-    async def acquire(self,
-                      block: bool = True,
-                      timeout: Union[float, int, None] = None,
-                      *args, **kwargs
-                      ) -> bool:
+    async def acquire(self, block: bool = True, timeout: Union[float, int, None] = None, *args, **kwargs) -> bool:
         raise NotImplementedError()
 
     async def release(self, *args, **kwargs):
         raise NotImplementedError()
 
     async def close(self, *args, **kwargs):
         if self._acquired:
```

### Comparing `sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/functions.py` & `sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from importlib import import_module
 
 from sqlalchemy.engine import Connection
 
-from .types import BaseSadLock, TConnectionOrSession
+from .baselock import BaseSadLock, TConnectionOrSession
 from .utils import safe_name
 
 __all__ = ["create_sadlock"]
 
 
 def create_sadlock(connection_or_session: TConnectionOrSession, key, *args, **kwargs) -> BaseSadLock:
     """Create a database distributed lock object
@@ -26,16 +26,21 @@
 
         Type of the lock object is sub-class of :class:`.BaseSadLock`,
         which depends on the passed-in SQLAlchemy `connection` or `session`.
 
         MySQL and PostgreSQL connection/session are supported til now.
     """
     if isinstance(connection_or_session, Connection):
-        name = safe_name(connection_or_session.engine.name)
+        engine = connection_or_session.engine
     else:
-        name = safe_name(connection_or_session.get_bind().name)
+        bind = connection_or_session.get_bind()
+        if isinstance(bind, Connection):
+            engine = bind.engine
+        else:
+            engine = bind
+    engine_name = safe_name(engine.name)
     try:
-        mod = import_module("..impl.{}".format(name), __name__)
+        mod = import_module(f"..lock.{engine_name}", __name__)
     except ImportError as exception:  # pragma: no cover
-        raise NotImplementedError("{}: {}".format(name, exception))
+        raise NotImplementedError(f"{engine_name}: {exception}")
     lock_cls = getattr(mod, "SadLock")
     return lock_cls(connection_or_session, key, *args, **kwargs)
```

### Comparing `sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/impl/mysql.py` & `sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/asyncio/lock/mysql.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,127 +1,87 @@
-from textwrap import dedent
 from typing import Any, Callable, Optional, Union
 
-from sqlalchemy import text
-
-from ..types import BaseSadLock
-from ..exceptions import SqlAlchemyDLockDatabaseError
-from ..types import TConnectionOrSession
+from ...exceptions import SqlAlchemyDLockDatabaseError
+from ...statement.mysql import STATEMENTS
+from ..baselock import BaseAsyncSadLock, TAsyncConnectionOrSession
 
 MYSQL_LOCK_NAME_MAX_LENGTH = 64
 
-GET_LOCK = text(
-    dedent(
-        """
-        SELECT GET_LOCK(:str, :timeout)
-        """
-    ).strip()
-)
-
-RELEASE_LOCK = text(
-    dedent(
-        """
-        SELECT RELEASE_LOCK(:str)
-        """
-    ).strip()
-)
-
 TConvertFunction = Callable[[Any], str]
 
 
 def default_convert(key: Union[bytearray, bytes, int, float]) -> str:
     if isinstance(key, (bytearray, bytes)):
         result = key.decode()
     elif isinstance(key, (int, float)):
         result = str(key)
     else:
-        raise TypeError("{}".format(type(key)))
+        raise TypeError(f"{type(key)}")
     return result
 
 
-class SadLock(BaseSadLock):
-    """MySQL named-lock
-
-    .. seealso:: https://dev.mysql.com/doc/refman/8.0/en/locking-functions.html
-    """
-
-    def __init__(self, connection_or_session: TConnectionOrSession, key, convert: Optional[TConvertFunction] = None):
-        """
-        MySQL named lock requires the key given by string.
-
-        If `key` is not a :class:`str`:
-
-        - When :class:`int` or :class:`float`,
-          the constructor will force convert it to :class:`str`::
-
-            key = str(key)
-
-        - When :class:`bytes`,
-          the constructor tries to decode it with default encoding::
-
-            key = key.decode()
-
-        - Or you can specify a `convert` function to that argument.
-          The function is like::
-
-            def convert(val: Any) -> str:
-                # do something ...
-                return string
-        """
+class AsyncSadLock(BaseAsyncSadLock):
+    def __init__(
+        self,
+        connection_or_session: TAsyncConnectionOrSession,
+        key,
+        convert: Optional[TConvertFunction] = None,
+    ):
         if convert:
             key = convert(key)
         elif not isinstance(key, str):
             key = default_convert(key)
         if not isinstance(key, str):
             raise TypeError("MySQL named lock requires the key given by string")
         if len(key) > MYSQL_LOCK_NAME_MAX_LENGTH:
-            raise ValueError(
-                "MySQL enforces a maximum length on lock names of {} characters.".format(MYSQL_LOCK_NAME_MAX_LENGTH)
-            )
+            raise ValueError(f"MySQL enforces a maximum length on lock names of {MYSQL_LOCK_NAME_MAX_LENGTH} characters.")
         #
         super().__init__(connection_or_session, key)
 
-    def acquire(self, block: bool = True, timeout: Union[float, int, None] = None) -> bool:
+    async def acquire(self, block: bool = True, timeout: Union[float, int, None] = None) -> bool:
         if self._acquired:
             raise ValueError("invoked on a locked lock")
         if block:
             # None: set the timeout period to infinite.
             if timeout is None:
                 timeout = -1
             # negative value for `timeout` are equivalent to a `timeout` of zero
             elif timeout < 0:
                 timeout = 0
         else:
             timeout = 0
-        stmt = GET_LOCK.params(str=self._key, timeout=timeout)
-        ret_val = self.connection_or_session.execute(stmt).scalar_one()
+        stmt = STATEMENTS["lock"].params(str=self._key, timeout=timeout)
+        r = await self.connection_or_session.stream(stmt)
+        ret_val = (await r.one())[0]
+
         if ret_val == 1:
             self._acquired = True
         elif ret_val == 0:
             pass  # 直到超时也没有成功锁定
         elif ret_val is None:  # pragma: no cover
-            raise SqlAlchemyDLockDatabaseError('An error occurred while attempting to obtain the lock "{}"'.format(self._key))
+            raise SqlAlchemyDLockDatabaseError(f"An error occurred while attempting to obtain the lock {self._key!r}")
         else:  # pragma: no cover
-            raise SqlAlchemyDLockDatabaseError('GET_LOCK("{}", {}) returns {}'.format(self._key, timeout, ret_val))
+            raise SqlAlchemyDLockDatabaseError(f"GET_LOCK({self._key!r}, {timeout}) returns {ret_val}")
         return self._acquired
 
-    def release(self):
+    async def release(self):
         if not self._acquired:
             raise ValueError("invoked on an unlocked lock")
-        stmt = RELEASE_LOCK.params(str=self._key)
-        ret_val = self.connection_or_session.execute(stmt).scalar_one()
+        stmt = STATEMENTS["unlock"].params(str=self._key)
+        r = await self.connection_or_session.stream(stmt)
+        ret_val = (await r.one())[0]
         if ret_val == 1:
             self._acquired = False
         elif ret_val == 0:  # pragma: no cover
             self._acquired = False
             raise SqlAlchemyDLockDatabaseError(
-                'The named lock "{}" was not established by this thread, ' "and the lock is not released.".format(self._key)
+                f"The named lock {self._key!r} was not established by this thread, " "and the lock is not released."
             )
         elif ret_val is None:  # pragma: no cover
             self._acquired = False
             raise SqlAlchemyDLockDatabaseError(
-                'The named lock "{}" did not exist, '
+                f"The named lock {self._key!r} did not exist, "
                 "was never obtained by a call to GET_LOCK(), "
-                "or has previously been released.".format(self._key)
+                "or has previously been released."
             )
-        else:  # pragma: no cover
-            raise SqlAlchemyDLockDatabaseError('RELEASE_LOCK("{}") returns {}'.format(self._key, ret_val))
+        else:
+            raise SqlAlchemyDLockDatabaseError(f"RELEASE_LOCK({self._key!r}) returns {ret_val}")
```

### Comparing `sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/types.py` & `sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/baselock.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         self._connection_or_session = connection_or_session
         self._key = key
 
     def __enter__(self):
         self.acquire()
         return self
 
-    def __exit__(self, exc_type, exc_value, traceback):
+    def __exit__(self, exc_type, exc_value, exc_tb):
         self.close()
 
     def __str__(self):  # pragma: no cover
         return "<{} {} key={} at 0x{:x}>".format(
             "locked" if self._acquired else "unlocked", self.__class__.__name__, self._key, id(self)
         )
 
@@ -66,44 +66,21 @@
 
     @property
     def key(self):
         """Returns `key` parameter of the constructor"""
         return self._key
 
     @property
-    def acquired(self) -> bool:
+    def locked(self) -> bool:
         """locked/unlocked state property
 
-        As a `Getter`:
-
-        - It returns ``True`` if the lock has been acquired, ``False`` otherwise.
-
-        As a `Setter`:
-
-        - Set to ``True`` is equivalent to call :meth:`acquire`
-        - Set to ``False`` is equivalent to call :meth:`release`
+        Return ``True`` if the lock is acquired.
         """
         return self._acquired
 
-    @acquired.setter
-    def acquired(self, value: bool):
-        if value:
-            self.acquire()
-        else:
-            self.release()
-
-    @property
-    def locked(self) -> bool:
-        """Alias of :data:`acquired`"""
-        return self.acquired
-
-    @locked.setter
-    def locked(self, value: bool):
-        self.acquired = value
-
     def acquire(self, block: bool = True, timeout: Union[float, int, None] = None, *args, **kwargs) -> bool:
         """
         Acquire a lock, blocking or non-blocking.
 
         - With the `block` argument set to ``True`` (the default),
           the method call will block until the lock is in an unlocked state,
           then set it to locked and return ``True``.
@@ -142,15 +119,15 @@
     def close(self, *args, **kwargs):
         """Same as :meth:`release`
 
         Except that the :class:`ValueError` is **NOT** raised when invoked on an unlocked lock.
 
         An invocation of this method is equivalent to::
 
-            if not some_lock.acquired:
+            if not some_lock.locked:
                 some_lock.release()
 
         This method maybe useful together with :func:`contextlib.closing`,
         when we need a :keyword:`with` statement, but don't want it to acquire at the beginning of the block.
 
         eg::
 
@@ -159,18 +136,18 @@
             from contextlib import closing
             from sqlalchemy_dlock import create_sadlock
 
             # ...
 
             with closing(create_sadlock(some_connection, some_key)) as lock:
                 # will not acquire at the begin of with-block
-                assert not lock.acquired
+                assert not lock.locked
                 # ...
                 # lock when need
                 lock.acquire()
-                assert lock.acquired
+                assert lock.locked
                 # ...
             # `close` will be called at the end with-block
-            assert not lock.acquired
+            assert not lock.locked
         """
         if self._acquired:
             self.release(*args, **kwargs)
```

### Comparing `sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock/utils.py` & `sqlalchemy-dlock-0.4/src/sqlalchemy_dlock/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 import re
 from hashlib import blake2b
 from sys import byteorder
 from typing import Union
 
-SAFE_NAME_PATTERN = re.compile(r'[^A-Za-z0-9_]+')
+SAFE_NAME_PATTERN = re.compile(r"[^A-Za-z0-9_]+")
 
 
 def safe_name(s):
-    return SAFE_NAME_PATTERN.sub('_', s).strip().lower()
+    return SAFE_NAME_PATTERN.sub("_", s).strip().lower()
 
 
 def to_int64_key(k: Union[bytearray, bytes, memoryview, str, int]) -> int:
     if isinstance(k, str):
         k = k.encode()
     if isinstance(k, (bytearray, bytes, memoryview)):
         return int.from_bytes(blake2b(k, digest_size=8).digest(), byteorder, signed=True)
     elif isinstance(k, int):
         return ensure_int64(k)
-    raise TypeError('{}'.format(type(k)))
+    raise TypeError(f"{type(k)}")
 
 
-INT64_MAX = 2**63-1  # max of signed int64: 2**63-1(+0x7fff_ffff_ffff_ffff)
-INT64_MIN = -2**63  # min of signed int64: -2**63(-0x8000_0000_0000_0000)
+INT64_MAX = 2**63 - 1  # max of signed int64: 2**63-1(+0x7fff_ffff_ffff_ffff)
+INT64_MIN = -(2**63)  # min of signed int64: -2**63(-0x8000_0000_0000_0000)
 
 
 def ensure_int64(i: int) -> int:
     if i > INT64_MAX:
-        i = int.from_bytes(
-            i.to_bytes(8, byteorder, signed=False),
-            byteorder, signed=True
-        )
+        i = int.from_bytes(i.to_bytes(8, byteorder, signed=False), byteorder, signed=True)
     elif i < INT64_MIN:
-        raise OverflowError('int too small to convert')
+        raise OverflowError("int too small to convert")
     return i
```

### Comparing `sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock.egg-info/PKG-INFO` & `sqlalchemy-dlock-0.4/src/sqlalchemy_dlock.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,33 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-dlock
-Version: 0.3.1
+Version: 0.4
 Summary: A distributed lock implementation based on SQLAlchemy
 Author-email: liu xue yan <liu_xue_yan@foxmail.com>
-License: BSD 3-Clause License
-        
-        Copyright (c) 2020, liu xue yan
-        All rights reserved.
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        1. Redistributions of source code must retain the above copyright notice, this
-           list of conditions and the following disclaimer.
-        
-        2. Redistributions in binary form must reproduce the above copyright notice,
-           this list of conditions and the following disclaimer in the documentation
-           and/or other materials provided with the distribution.
-        
-        3. Neither the name of the copyright holder nor the names of its
-           contributors may be used to endorse or promote products derived from
-           this software without specific prior written permission.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
+License: BSD-3-Clause
 Project-URL: homepage, https://github.com/tanbro/sqlalchemy-dlock
+Project-URL: documentation, https://sqlalchemy-dlock.readthedocs.io/
 Project-URL: repository, https://github.com/tanbro/sqlalchemy-dlock.git
 Keywords: SQLAlchemy,lock,distributed,distributed lock,SQL,database,DBMS
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: asyncio
+Provides-Extra: mysqlclient
+Provides-Extra: pymysql
+Provides-Extra: aiomysql
+Provides-Extra: psycopg2
+Provides-Extra: psycopg2-binary
+Provides-Extra: psycopg3
+Provides-Extra: psycopg3-binary
+Provides-Extra: psycopg3-c
+Provides-Extra: asyncpg3
 License-File: LICENSE
 License-File: AUTHORS.md
 
 # SQLAlchemy-DLock
 
 [![Python package](https://github.com/tanbro/sqlalchemy-dlock/actions/workflows/python-package.yml/badge.svg)](https://github.com/tanbro/sqlalchemy-dlock/actions/workflows/python-package.yml)
 [![PyPI](https://img.shields.io/pypi/v/sqlalchemy-dlock)](https://pypi.org/project/sqlalchemy-dlock/)
@@ -58,172 +39,220 @@
 It currently supports below locks:
 
  Database  |                                             Lock
 ---------- | ---------------------------------------------------------------------------------------------
 MySQL      | [named lock](https://dev.mysql.com/doc/refman/8.0/en/locking-functions.html)
 PostgreSQL | [advisory lock](https://www.postgresql.org/docs/current/explicit-locking.html#ADVISORY-LOCKS)
 
-## Usages
+## Install
+
+```bash
+pip install sqlalchemy-dlock
+```
+
+## Usage
 
 - Work with [SQLAlchemy][] `Connection`:
 
   ```python
   from sqlalchemy import create_engine
   from sqlalchemy_dlock import create_sadlock
 
   key = 'user/001'
 
-  engine = create_engine('postgresql://scott:tiger@localhost/')
+  engine = create_engine('postgresql://scott:tiger@127.0.0.1/')
   conn = engine.connect()
 
   # Create the D-Lock on the connection
   lock = create_sadlock(conn, key)
 
   # it's not lock when constructed
-  assert not lock.acquired
+  assert not lock.locked
 
   # lock
   lock.acquire()
-  assert lock.acquired
+  assert lock.locked
 
   # un-lock
   lock.release()
-  assert not lock.acquired
+  assert not lock.locked
   ```
 
 - `with` statement
 
   ```python
   from contextlib import closing
 
   from sqlalchemy import create_engine
   from sqlalchemy_dlock import create_sadlock
 
   key = 'user/001'
 
-  engine = create_engine('postgresql://scott:tiger@localhost/')
+  engine = create_engine('postgresql://scott:tiger@127.0.0.1/')
   with engine.connect() as conn:
 
       # Create the D-Lock on the connection
       with create_sadlock(conn, key) as lock:
           # It's locked
-          assert lock.acquired
+          assert lock.locked
 
       # Auto un-locked
-      assert not lock.acquired
+      assert not lock.locked
 
       # If do not want to be locked in `with`, a `closing` wrapper may help
       with closing(create_sadlock(conn, key)) as lock2:
-          # It's NOT locked here
-          assert not lock2.acquired
+          # It's NOT locked here !!!
+          assert not lock2.locked
           # lock it now:
           lock2.acquire()
-          assert lock2.acquired
+          assert lock2.locked
 
       # Auto un-locked
-      assert not lock2.acquired
+      assert not lock2.locked
   ```
 
 - Work with [SQLAlchemy][] `ORM` session:
 
   ```python
   from sqlalchemy import create_engine
   from sqlalchemy.orm import sessionmaker
   from sqlalchemy_dlock import create_sadlock
 
   key = 'user/001'
 
-  engine = create_engine('postgresql://scott:tiger@localhost/')
+  engine = create_engine('postgresql://scott:tiger@127.0.0.1/')
   Session = sessionmaker(bind=engine)
 
   with Session() as session:
     with create_sadlock(session, key) as lock:
-        assert lock.acquired
-    assert not lock.acquired
+        assert lock.locked
+    assert not lock.locked
   ```
 
 - Asynchronous I/O Support
 
-  > ℹ️ **info**:
+  > **Note**:
   >
   > - [SQLAlchemy][] `1.x`: <https://docs.sqlalchemy.org/14/orm/extensions/asyncio.html>
   > - [SQLAlchemy][] `2.x`: <https://docs.sqlalchemy.org/20/orm/extensions/asyncio.html>
 
   ```python
   from sqlalchemy.ext.asyncio import create_async_engine
   from sqlalchemy_dlock.asyncio import create_async_sadlock
 
   key = 'user/001'
 
-  engine = create_async_engine('postgresql+asyncpg://scott:tiger@localhost/')
+  engine = create_async_engine('postgresql+asyncpg://scott:tiger@127.0.0.1/')
 
   async with engine.begin() as conn:
       async with create_async_sadlock(conn, key) as lock:
           assert lock.locked
           await lock.release()
           assert not lock.locked
           await lock.acquire()
       assert not lock.locked
   ```
 
-## Tests
+  > **Note**:
+  >
+  > [aiomysql][], [asyncpg][] and [psycopg][] are tested asynchronous drivers
+  >
+  > We can install asynchronous DB libraries like one of blows:
+  >
+  > - ```bash
+  >   pip install sqlalchemy-dlock[asyncpg]
+  >   ```
+  >
+  > - ```bash
+  >   pip install sqlalchemy-dlock[asyncio] aiomysql
+  >   ```
+  >
+  > - ```bash
+  >   pip install SQLALchemy[asyncio] sqlalchemy-dlock psycopg
+  >   ```
+
+## Test
 
-Following [SQLAlchemy][] engines are tested:
+Following drivers are tested:
 
 - MySQL:
+  - [mysqlclient][] (synchronous)
+  - [pymysql][] (synchronous)
+  - [aiomysql][] (asynchronous)
+- Postgres:
+  - [psycopg2][] (asynchronous)
+  - [asyncpg][] (asynchronous)
+  - [psycopg][] (synchronous and asynchronous)
 
-  - mysqlclient
-  - PyMySQL
-  - aiomysql ([asyncio][])
+You can run unit-tests
 
-- Postgres:
+- on local environment:
 
-  - psycopg2
-  - asyncpg ([asyncio][])
+  1. Install the project with drivers and `asyncio` extra requires, a virtual environment ([venv][]) is strongly advised:
 
-You can run unit-tests:
+     ```bash
+     pip install -e .[mysqlclient psycopg2-binary aiomysql asyncpg]
+     ```
 
-- directly:
+  1. start up mysql and postgresql
 
-  1. Install the project (A virtual environment ([venv][]) is strongly advised):
+     There is a docker [compose][] file `db.docker-compose.yml` in the project dir,
+     which can be used to run mysql and postgresql develop environment conveniently:
 
      ```bash
-     pip install -e .
+     docker compose -f db.docker-compose.yml up
      ```
 
-  1. Start up your mysql and postgresql
-
-  1. Set environment variables `TEST_URLS` and `TEST_ASYNC_URLS` for sync and async database connection url.
+  1. set environment variables `TEST_URLS` and `TEST_ASYNC_URLS` for sync and async database connection url.
      Multiple connections separated by space.
      The test cases load environment variables in `tests/.env`.
 
      eg (and also the defaults):
 
      ```ini
-     TEST_URLS=mysql://test:test@localhost/test postgresql://postgres:test@localhost/
-     TEST_ASYNC_URLS=mysql+aiomysql://test:test@localhost/test postgresql+asyncpg://postgres:test@localhost/
+     TEST_URLS=mysql://test:test@127.0.0.1/test postgresql://postgres:test@127.0.0.1/
+     TEST_ASYNC_URLS=mysql+aiomysql://test:test@127.0.0.1/test postgresql+asyncpg://postgres:test@127.0.0.1/
      ```
 
   1. run unit-test
 
      ```bash
      python -m unittest
      ```
 
-- in docker-compose:
+- or on docker-compose:
 
   1. build the project
 
      ```bash
      python -m pip install build && python -m build -w
      ```
 
   1. run unit-test
 
+     Name of services for Python and [SQLAlchemy][] version matrix in the [compose][] file has such format:
+
+         python{{X.Y}}-sqlalchemy{{X}}
+
+     For example, if want to take a test for Python `3.9` and [SQLAlchemy][] `2.x`, we shall up to run unit-tests as below:
+
+     ```bash
+     cd tests
+     docker compose up python3.9-sqlalchemy2
+     ```
+
+     For Python `3.8` and [SQLAlchemy][] `1.x`:
+
      ```bash
      cd tests
-     docker compose up
+     docker compose up python3.8-sqlalchemy1
      ```
 
 [SQLAlchemy]: https://www.sqlalchemy.org/ "The Python SQL Toolkit and Object Relational Mapper"
-[asyncio]: https://docs.python.org/library/asyncio.html "asyncio is a library to write concurrent code using the async/await syntax."
 [venv]: https://docs.python.org/library/venv.html "The venv module supports creating lightweight “virtual environments”, each with their own independent set of Python packages installed in their site directories. "
+[mysqlclient]: https://pypi.org/project/mysqlclient/ "Python interface to MySQL"
+[psycopg2]: https://pypi.org/project/psycopg2/ "PostgreSQL database adapter for Python"
+[psycopg]: https://pypi.org/project/psycopg/ "Psycopg 3 is a modern implementation of a PostgreSQL adapter for Python."
+[aiomysql]: https://pypi.org/project/aiomysql/ "aiomysql is a “driver” for accessing a MySQL database from the asyncio (PEP-3156/tulip) framework."
+[asyncpg]: https://pypi.org/project/asyncpg/ "asyncpg is a database interface library designed specifically for PostgreSQL and Python/asyncio. "
+[pymysql]: https://pypi.org/project/pymysql/ "Pure Python MySQL Driver"
+[compose]: https://docs.docker.com/compose/ "Compose is a tool for defining and running multi-container Docker applications."
```

### Comparing `sqlalchemy-dlock-0.3.1/src/sqlalchemy_dlock.egg-info/SOURCES.txt` & `sqlalchemy-dlock-0.4/src/sqlalchemy_dlock.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 AUTHORS.md
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 src/sqlalchemy_dlock/__init__.py
+src/sqlalchemy_dlock/baselock.py
 src/sqlalchemy_dlock/exceptions.py
 src/sqlalchemy_dlock/functions.py
-src/sqlalchemy_dlock/types.py
 src/sqlalchemy_dlock/utils.py
 src/sqlalchemy_dlock/version.py
 src/sqlalchemy_dlock.egg-info/PKG-INFO
 src/sqlalchemy_dlock.egg-info/SOURCES.txt
 src/sqlalchemy_dlock.egg-info/dependency_links.txt
 src/sqlalchemy_dlock.egg-info/requires.txt
 src/sqlalchemy_dlock.egg-info/top_level.txt
 src/sqlalchemy_dlock/asyncio/__init__.py
+src/sqlalchemy_dlock/asyncio/baselock.py
 src/sqlalchemy_dlock/asyncio/functions.py
-src/sqlalchemy_dlock/asyncio/types.py
-src/sqlalchemy_dlock/asyncio/impl/__init__.py
-src/sqlalchemy_dlock/asyncio/impl/mysql.py
-src/sqlalchemy_dlock/asyncio/impl/postgresql.py
-src/sqlalchemy_dlock/impl/__init__.py
-src/sqlalchemy_dlock/impl/mysql.py
-src/sqlalchemy_dlock/impl/postgresql.py
+src/sqlalchemy_dlock/asyncio/lock/__init__.py
+src/sqlalchemy_dlock/asyncio/lock/mysql.py
+src/sqlalchemy_dlock/asyncio/lock/postgresql.py
+src/sqlalchemy_dlock/lock/__init__.py
+src/sqlalchemy_dlock/lock/mysql.py
+src/sqlalchemy_dlock/lock/postgresql.py
+src/sqlalchemy_dlock/statement/__init__.py
+src/sqlalchemy_dlock/statement/mysql.py
+src/sqlalchemy_dlock/statement/postgresql.py
```

