# Comparing `tmp/acore_server_metadata-0.1.1.tar.gz` & `tmp/acore_server_metadata-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_server_metadata-0.1.1.tar", last modified: Fri Jun 16 02:43:22 2023, max compression
+gzip compressed data, was "acore_server_metadata-0.2.1.tar", last modified: Sat Jun 17 03:03:29 2023, max compression
```

## Comparing `acore_server_metadata-0.1.1.tar` & `acore_server_metadata-0.2.1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 02:43:22.659211 acore_server_metadata-0.1.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 16:37:48.000000 acore_server_metadata-0.1.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2023-06-15 16:37:48.000000 acore_server_metadata-0.1.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      329 2023-06-15 16:37:48.000000 acore_server_metadata-0.1.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     6110 2023-06-16 02:43:22.659067 acore_server_metadata-0.1.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     4961 2023-06-16 02:34:23.000000 acore_server_metadata-0.1.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 02:43:22.656475 acore_server_metadata-0.1.1/acore_server_metadata/
--rw-r--r--   0 sanhehu    (501) staff       (20)      391 2023-06-16 02:28:42.000000 acore_server_metadata-0.1.1/acore_server_metadata/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-15 16:37:48.000000 acore_server_metadata-0.1.1/acore_server_metadata/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      101 2023-06-15 20:16:05.000000 acore_server_metadata-0.1.1/acore_server_metadata/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 02:43:22.657361 acore_server_metadata-0.1.1/acore_server_metadata/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-15 16:37:48.000000 acore_server_metadata-0.1.1/acore_server_metadata/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      336 2023-06-15 19:55:44.000000 acore_server_metadata-0.1.1/acore_server_metadata/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-15 16:37:48.000000 acore_server_metadata-0.1.1/acore_server_metadata/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     9256 2023-06-16 02:26:07.000000 acore_server_metadata-0.1.1/acore_server_metadata/server.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       89 2023-06-15 20:16:40.000000 acore_server_metadata-0.1.1/acore_server_metadata/settings.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 02:43:22.658027 acore_server_metadata-0.1.1/acore_server_metadata/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-15 16:37:48.000000 acore_server_metadata-0.1.1/acore_server_metadata/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-15 16:37:48.000000 acore_server_metadata-0.1.1/acore_server_metadata/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-16 01:30:10.000000 acore_server_metadata-0.1.1/acore_server_metadata/tests/mock_aws.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 02:43:22.658403 acore_server_metadata-0.1.1/acore_server_metadata/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 16:37:48.000000 acore_server_metadata-0.1.1/acore_server_metadata/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-15 16:37:48.000000 acore_server_metadata-0.1.1/acore_server_metadata/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 02:43:22.657251 acore_server_metadata-0.1.1/acore_server_metadata.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     6110 2023-06-16 02:43:22.000000 acore_server_metadata-0.1.1/acore_server_metadata.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      918 2023-06-16 02:43:22.000000 acore_server_metadata-0.1.1/acore_server_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-16 02:43:22.000000 acore_server_metadata-0.1.1/acore_server_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      242 2023-06-16 02:43:22.000000 acore_server_metadata-0.1.1/acore_server_metadata.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       22 2023-06-16 02:43:22.000000 acore_server_metadata-0.1.1/acore_server_metadata.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      620 2023-06-16 02:21:58.000000 acore_server_metadata-0.1.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-15 16:37:48.000000 acore_server_metadata-0.1.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-15 16:37:48.000000 acore_server_metadata-0.1.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-15 16:37:48.000000 acore_server_metadata-0.1.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-16 01:31:27.000000 acore_server_metadata-0.1.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       88 2023-06-16 01:25:35.000000 acore_server_metadata-0.1.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-16 02:43:22.659255 acore_server_metadata-0.1.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7570 2023-06-15 16:37:48.000000 acore_server_metadata-0.1.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-16 02:43:22.658761 acore_server_metadata-0.1.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      766 2023-06-16 02:21:18.000000 acore_server_metadata-0.1.1/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4608 2023-06-16 02:23:10.000000 acore_server_metadata-0.1.1/tests/test_server.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 03:03:29.270013 acore_server_metadata-0.2.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      329 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6422 2023-06-17 03:03:29.269856 acore_server_metadata-0.2.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5273 2023-06-17 02:59:40.000000 acore_server_metadata-0.2.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 03:03:29.267522 acore_server_metadata-0.2.1/acore_server_metadata/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      391 2023-06-16 02:28:42.000000 acore_server_metadata-0.2.1/acore_server_metadata/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-16 15:13:09.000000 acore_server_metadata-0.2.1/acore_server_metadata/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      101 2023-06-15 20:16:05.000000 acore_server_metadata-0.2.1/acore_server_metadata/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 03:03:29.268332 acore_server_metadata-0.2.1/acore_server_metadata/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/acore_server_metadata/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      496 2023-06-16 15:11:12.000000 acore_server_metadata-0.2.1/acore_server_metadata/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/acore_server_metadata/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    18210 2023-06-17 02:55:37.000000 acore_server_metadata-0.2.1/acore_server_metadata/server.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       89 2023-06-15 20:16:40.000000 acore_server_metadata-0.2.1/acore_server_metadata/settings.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 03:03:29.268955 acore_server_metadata-0.2.1/acore_server_metadata/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/acore_server_metadata/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/acore_server_metadata/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-16 01:30:10.000000 acore_server_metadata-0.2.1/acore_server_metadata/tests/mock_aws.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      155 2023-06-17 02:38:50.000000 acore_server_metadata-0.2.1/acore_server_metadata/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 03:03:29.269378 acore_server_metadata-0.2.1/acore_server_metadata/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/acore_server_metadata/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/acore_server_metadata/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 03:03:29.268198 acore_server_metadata-0.2.1/acore_server_metadata.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6422 2023-06-17 03:03:29.000000 acore_server_metadata-0.2.1/acore_server_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      949 2023-06-17 03:03:29.000000 acore_server_metadata-0.2.1/acore_server_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-17 03:03:29.000000 acore_server_metadata-0.2.1/acore_server_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      242 2023-06-17 03:03:29.000000 acore_server_metadata-0.2.1/acore_server_metadata.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       22 2023-06-17 03:03:29.000000 acore_server_metadata-0.2.1/acore_server_metadata.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1241 2023-06-17 02:58:20.000000 acore_server_metadata-0.2.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-16 01:31:27.000000 acore_server_metadata-0.2.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       88 2023-06-16 01:25:35.000000 acore_server_metadata-0.2.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-17 03:03:29.270060 acore_server_metadata-0.2.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7570 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 03:03:29.269652 acore_server_metadata-0.2.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      938 2023-06-17 03:01:13.000000 acore_server_metadata-0.2.1/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4733 2023-06-17 03:02:56.000000 acore_server_metadata-0.2.1/tests/test_server.py
```

### Comparing `acore_server_metadata-0.1.1/AUTHORS.rst` & `acore_server_metadata-0.2.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.1.1/LICENSE.txt` & `acore_server_metadata-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.1.1/PKG-INFO` & `acore_server_metadata-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore_server_metadata
-Version: 0.1.1
+Version: 0.2.1
 Summary: Azerothcore WOW server metadata for Fleet management.
 Home-page: https://github.com/MacHu-GWU/acore_server_metadata-project
-Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.2.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -140,14 +140,25 @@
     {
         "prod-1": <Server id="prod-1">,
         "prod-2": <Server id="prod-2">,
         "dev-1": <Server id="dev-1">,
         "dev-2": <Server id="dev-2">,
     }
 
+    # 启动新的 EC2
+    >>> server.run_ec2(...)
+    # 启动新的 DB Instance
+    >>> server.run_rds(...)
+    # 关联 EIP 地址
+    >>> server.associate_eip_address(...)
+    # 创建数据库备份
+    >>> server.create_db_snapshot(...)
+    # 清理数据库备份
+    >>> server.cleanup_db_snapshot(...)
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``acore_server_metadata`` is released on PyPI, so all you need is to:
```

### Comparing `acore_server_metadata-0.1.1/README.rst` & `acore_server_metadata-0.2.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -108,14 +108,25 @@
     {
         "prod-1": <Server id="prod-1">,
         "prod-2": <Server id="prod-2">,
         "dev-1": <Server id="dev-1">,
         "dev-2": <Server id="dev-2">,
     }
 
+    # 启动新的 EC2
+    >>> server.run_ec2(...)
+    # 启动新的 DB Instance
+    >>> server.run_rds(...)
+    # 关联 EIP 地址
+    >>> server.associate_eip_address(...)
+    # 创建数据库备份
+    >>> server.create_db_snapshot(...)
+    # 清理数据库备份
+    >>> server.cleanup_db_snapshot(...)
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``acore_server_metadata`` is released on PyPI, so all you need is to:
```

### Comparing `acore_server_metadata-0.1.1/acore_server_metadata/paths.py` & `acore_server_metadata-0.2.1/acore_server_metadata/paths.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.1.1/acore_server_metadata/tests/mock_aws.py` & `acore_server_metadata-0.2.1/acore_server_metadata/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.1.1/acore_server_metadata/vendor/pytest_cov_helper.py` & `acore_server_metadata-0.2.1/acore_server_metadata/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.1.1/acore_server_metadata.egg-info/PKG-INFO` & `acore_server_metadata-0.2.1/acore_server_metadata.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore-server-metadata
-Version: 0.1.1
+Version: 0.2.1
 Summary: Azerothcore WOW server metadata for Fleet management.
 Home-page: https://github.com/MacHu-GWU/acore_server_metadata-project
-Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.2.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -140,14 +140,25 @@
     {
         "prod-1": <Server id="prod-1">,
         "prod-2": <Server id="prod-2">,
         "dev-1": <Server id="dev-1">,
         "dev-2": <Server id="dev-2">,
     }
 
+    # 启动新的 EC2
+    >>> server.run_ec2(...)
+    # 启动新的 DB Instance
+    >>> server.run_rds(...)
+    # 关联 EIP 地址
+    >>> server.associate_eip_address(...)
+    # 创建数据库备份
+    >>> server.create_db_snapshot(...)
+    # 清理数据库备份
+    >>> server.cleanup_db_snapshot(...)
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``acore_server_metadata`` is released on PyPI, so all you need is to:
```

### Comparing `acore_server_metadata-0.1.1/acore_server_metadata.egg-info/SOURCES.txt` & `acore_server_metadata-0.2.1/acore_server_metadata.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 acore_server_metadata/__init__.py
 acore_server_metadata/_version.py
 acore_server_metadata/api.py
 acore_server_metadata/exc.py
 acore_server_metadata/paths.py
 acore_server_metadata/server.py
 acore_server_metadata/settings.py
+acore_server_metadata/utils.py
 acore_server_metadata.egg-info/PKG-INFO
 acore_server_metadata.egg-info/SOURCES.txt
 acore_server_metadata.egg-info/dependency_links.txt
 acore_server_metadata.egg-info/requires.txt
 acore_server_metadata.egg-info/top_level.txt
 acore_server_metadata/docs/__init__.py
 acore_server_metadata/tests/__init__.py
```

### Comparing `acore_server_metadata-0.1.1/requirements-doc.txt` & `acore_server_metadata-0.2.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.1.1/setup.py` & `acore_server_metadata-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.1.1/tests/test_api.py` & `acore_server_metadata-0.2.1/tests/test_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,13 +22,18 @@
     _ = api.Server.is_exists
     _ = api.Server.is_running
     _ = api.Server.is_ec2_exists
     _ = api.Server.is_ec2_running
     _ = api.Server.is_rds_exists
     _ = api.Server.is_rds_running
     _ = api.Server.refresh
+    _ = api.Server.run_ec2
+    _ = api.Server.run_rds
+    _ = api.Server.associate_eip_address
+    _ = api.Server.create_db_snapshot
+    _ = api.Server.cleanup_db_snapshot
 
 
 if __name__ == "__main__":
     from acore_server_metadata.tests import run_cov_test
 
     run_cov_test(__file__, "acore_server_metadata.api", preview=False)
```

### Comparing `acore_server_metadata-0.1.1/tests/test_server.py` & `acore_server_metadata-0.2.1/tests/test_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,17 +122,21 @@
         with pytest.raises(ServerNotUniqueError):
             Server.batch_get_server(
                 ids=["prod-1", "prod-2"],
                 ec2_client=self.bsm.ec2_client,
                 rds_client=self.bsm.rds_client,
             )
 
+    def _test_operations(self):
+        server = Server(id="test-operations")
+        # todo
 
     def test(self):
         self._test()
         self._test_batch_get_server()
+        self._test_operations()
 
 
 if __name__ == "__main__":
     from acore_server_metadata.tests import run_cov_test
 
     run_cov_test(__file__, "acore_server_metadata.server", preview=False)
```

