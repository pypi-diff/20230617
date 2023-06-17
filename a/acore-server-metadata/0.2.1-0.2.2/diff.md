# Comparing `tmp/acore_server_metadata-0.2.1.tar.gz` & `tmp/acore_server_metadata-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_server_metadata-0.2.1.tar", last modified: Sat Jun 17 03:03:29 2023, max compression
+gzip compressed data, was "acore_server_metadata-0.2.2.tar", last modified: Sat Jun 17 18:03:11 2023, max compression
```

## Comparing `acore_server_metadata-0.2.1.tar` & `acore_server_metadata-0.2.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 03:03:29.270013 acore_server_metadata-0.2.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      329 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     6422 2023-06-17 03:03:29.269856 acore_server_metadata-0.2.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     5273 2023-06-17 02:59:40.000000 acore_server_metadata-0.2.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 03:03:29.267522 acore_server_metadata-0.2.1/acore_server_metadata/
--rw-r--r--   0 sanhehu    (501) staff       (20)      391 2023-06-16 02:28:42.000000 acore_server_metadata-0.2.1/acore_server_metadata/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-16 15:13:09.000000 acore_server_metadata-0.2.1/acore_server_metadata/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      101 2023-06-15 20:16:05.000000 acore_server_metadata-0.2.1/acore_server_metadata/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 03:03:29.268332 acore_server_metadata-0.2.1/acore_server_metadata/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/acore_server_metadata/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      496 2023-06-16 15:11:12.000000 acore_server_metadata-0.2.1/acore_server_metadata/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/acore_server_metadata/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    18210 2023-06-17 02:55:37.000000 acore_server_metadata-0.2.1/acore_server_metadata/server.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       89 2023-06-15 20:16:40.000000 acore_server_metadata-0.2.1/acore_server_metadata/settings.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 03:03:29.268955 acore_server_metadata-0.2.1/acore_server_metadata/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/acore_server_metadata/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/acore_server_metadata/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-16 01:30:10.000000 acore_server_metadata-0.2.1/acore_server_metadata/tests/mock_aws.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      155 2023-06-17 02:38:50.000000 acore_server_metadata-0.2.1/acore_server_metadata/utils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 03:03:29.269378 acore_server_metadata-0.2.1/acore_server_metadata/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/acore_server_metadata/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/acore_server_metadata/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 03:03:29.268198 acore_server_metadata-0.2.1/acore_server_metadata.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     6422 2023-06-17 03:03:29.000000 acore_server_metadata-0.2.1/acore_server_metadata.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      949 2023-06-17 03:03:29.000000 acore_server_metadata-0.2.1/acore_server_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-17 03:03:29.000000 acore_server_metadata-0.2.1/acore_server_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      242 2023-06-17 03:03:29.000000 acore_server_metadata-0.2.1/acore_server_metadata.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       22 2023-06-17 03:03:29.000000 acore_server_metadata-0.2.1/acore_server_metadata.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     1241 2023-06-17 02:58:20.000000 acore_server_metadata-0.2.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-16 01:31:27.000000 acore_server_metadata-0.2.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       88 2023-06-16 01:25:35.000000 acore_server_metadata-0.2.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-17 03:03:29.270060 acore_server_metadata-0.2.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7570 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 03:03:29.269652 acore_server_metadata-0.2.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      938 2023-06-17 03:01:13.000000 acore_server_metadata-0.2.1/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4733 2023-06-17 03:02:56.000000 acore_server_metadata-0.2.1/tests/test_server.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 18:03:11.713547 acore_server_metadata-0.2.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      329 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6597 2023-06-17 18:03:11.713402 acore_server_metadata-0.2.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5448 2023-06-17 17:14:49.000000 acore_server_metadata-0.2.2/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 18:03:11.711699 acore_server_metadata-0.2.2/acore_server_metadata/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      391 2023-06-16 02:28:42.000000 acore_server_metadata-0.2.2/acore_server_metadata/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-17 18:02:47.000000 acore_server_metadata-0.2.2/acore_server_metadata/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      101 2023-06-15 20:16:05.000000 acore_server_metadata-0.2.2/acore_server_metadata/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 18:03:11.712395 acore_server_metadata-0.2.2/acore_server_metadata/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/acore_server_metadata/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      496 2023-06-16 15:11:12.000000 acore_server_metadata-0.2.2/acore_server_metadata/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/acore_server_metadata/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    21479 2023-06-17 17:52:30.000000 acore_server_metadata-0.2.2/acore_server_metadata/server.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       89 2023-06-15 20:16:40.000000 acore_server_metadata-0.2.2/acore_server_metadata/settings.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 18:03:11.712752 acore_server_metadata-0.2.2/acore_server_metadata/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/acore_server_metadata/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/acore_server_metadata/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-16 01:30:10.000000 acore_server_metadata-0.2.2/acore_server_metadata/tests/mock_aws.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      155 2023-06-17 02:38:50.000000 acore_server_metadata-0.2.2/acore_server_metadata/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 18:03:11.712983 acore_server_metadata-0.2.2/acore_server_metadata/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/acore_server_metadata/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/acore_server_metadata/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 18:03:11.712274 acore_server_metadata-0.2.2/acore_server_metadata.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6597 2023-06-17 18:03:11.000000 acore_server_metadata-0.2.2/acore_server_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      949 2023-06-17 18:03:11.000000 acore_server_metadata-0.2.2/acore_server_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-17 18:03:11.000000 acore_server_metadata-0.2.2/acore_server_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      242 2023-06-17 18:03:11.000000 acore_server_metadata-0.2.2/acore_server_metadata.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       22 2023-06-17 18:03:11.000000 acore_server_metadata-0.2.2/acore_server_metadata.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1514 2023-06-17 17:06:47.000000 acore_server_metadata-0.2.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-16 01:31:27.000000 acore_server_metadata-0.2.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       88 2023-06-16 01:25:35.000000 acore_server_metadata-0.2.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-17 18:03:11.713588 acore_server_metadata-0.2.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7570 2023-06-15 16:37:48.000000 acore_server_metadata-0.2.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-17 18:03:11.713217 acore_server_metadata-0.2.2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      938 2023-06-17 03:01:13.000000 acore_server_metadata-0.2.2/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5190 2023-06-17 17:52:12.000000 acore_server_metadata-0.2.2/tests/test_server.py
```

### Comparing `acore_server_metadata-0.2.1/AUTHORS.rst` & `acore_server_metadata-0.2.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.2.1/LICENSE.txt` & `acore_server_metadata-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.2.1/PKG-INFO` & `acore_server_metadata-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore_server_metadata
-Version: 0.2.1
+Version: 0.2.2
 Summary: Azerothcore WOW server metadata for Fleet management.
 Home-page: https://github.com/MacHu-GWU/acore_server_metadata-project
-Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.2.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.2.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -88,15 +88,15 @@
 
 我假设游戏服务器虚拟机和数据库都是在 AWS 上用 EC2 和 RDS 部署的. 所以这个项目只能用于 AWS 环境下的服务器管理.
 
 **关于本项目**
 
 本项目是一个简单的 Python 包, 提供了对一个 realm 服务器的抽象.
 
-用例:
+**基础用例, 获取服务器状态**
 
 .. code-block:: python
 
     # 获取服务器的状态
     >>> import boto3
     >>> from acore_server_metadata.api import Server
     >>> server_id = "prod"
@@ -140,18 +140,22 @@
     {
         "prod-1": <Server id="prod-1">,
         "prod-2": <Server id="prod-2">,
         "dev-1": <Server id="dev-1">,
         "dev-2": <Server id="dev-2">,
     }
 
+**对服务器进行操作**
+
+.. code-block:: python
+
     # 启动新的 EC2
-    >>> server.run_ec2(...)
+    >>> server.run_ec2(ec_client, ami_id, instance_type, ...)
     # 启动新的 DB Instance
-    >>> server.run_rds(...)
+    >>> server.run_rds(rds_client, db_snapshot_identifier, db_instance_class, ...)
     # 关联 EIP 地址
     >>> server.associate_eip_address(...)
     # 创建数据库备份
     >>> server.create_db_snapshot(...)
     # 清理数据库备份
     >>> server.cleanup_db_snapshot(...)
```

### Comparing `acore_server_metadata-0.2.1/README.rst` & `acore_server_metadata-0.2.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 我假设游戏服务器虚拟机和数据库都是在 AWS 上用 EC2 和 RDS 部署的. 所以这个项目只能用于 AWS 环境下的服务器管理.
 
 **关于本项目**
 
 本项目是一个简单的 Python 包, 提供了对一个 realm 服务器的抽象.
 
-用例:
+**基础用例, 获取服务器状态**
 
 .. code-block:: python
 
     # 获取服务器的状态
     >>> import boto3
     >>> from acore_server_metadata.api import Server
     >>> server_id = "prod"
@@ -108,18 +108,22 @@
     {
         "prod-1": <Server id="prod-1">,
         "prod-2": <Server id="prod-2">,
         "dev-1": <Server id="dev-1">,
         "dev-2": <Server id="dev-2">,
     }
 
+**对服务器进行操作**
+
+.. code-block:: python
+
     # 启动新的 EC2
-    >>> server.run_ec2(...)
+    >>> server.run_ec2(ec_client, ami_id, instance_type, ...)
     # 启动新的 DB Instance
-    >>> server.run_rds(...)
+    >>> server.run_rds(rds_client, db_snapshot_identifier, db_instance_class, ...)
     # 关联 EIP 地址
     >>> server.associate_eip_address(...)
     # 创建数据库备份
     >>> server.create_db_snapshot(...)
     # 清理数据库备份
     >>> server.cleanup_db_snapshot(...)
```

### Comparing `acore_server_metadata-0.2.1/acore_server_metadata/paths.py` & `acore_server_metadata-0.2.2/acore_server_metadata/paths.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.2.1/acore_server_metadata/server.py` & `acore_server_metadata-0.2.2/acore_server_metadata/server.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import typing as T
 import dataclasses
 from datetime import timezone
 
-from simple_aws_ec2.api import Ec2Instance
-from simple_aws_rds.api import RDSDBInstance
+from simple_aws_ec2.api import Ec2Instance, EC2InstanceStatusEnum
+from simple_aws_rds.api import RDSDBInstance, RDSDBInstanceStatusEnum
 
 from .exc import (
     ServerNotFoundError,
     ServerNotUniqueError,
     ServerAlreadyExistsError,
 )
 from .settings import settings
@@ -40,46 +40,99 @@
     ec2_inst: T.Optional[Ec2Instance] = dataclasses.field(default=None)
     rds_inst: T.Optional[RDSDBInstance] = dataclasses.field(default=None)
 
     # --------------------------------------------------------------------------
     # Constructor
     # --------------------------------------------------------------------------
     @classmethod
+    def _get_existing_ec2(
+        cls,
+        ec2_client,
+        ids: T.List[str],
+    ) -> T.List[Ec2Instance]:
+        return Ec2Instance.query(
+            ec2_client=ec2_client,
+            filters=[
+                dict(Name=f"tag:{settings.ID_TAG_KEY}", Values=ids),
+                # we don't count terminated instances as existing
+                dict(
+                    Name="instance-state-name",
+                    Values=[
+                        EC2InstanceStatusEnum.pending.value,
+                        EC2InstanceStatusEnum.running.value,
+                        EC2InstanceStatusEnum.stopping.value,
+                        EC2InstanceStatusEnum.stopped.value,
+                    ],
+                ),
+            ],
+        ).all()
+
+    @classmethod
+    def _get_existing_rds(
+        cls,
+        rds_client,
+        ids: T.List[str],
+    ) -> T.List[RDSDBInstance]:
+        res = RDSDBInstance.query(rds_client)
+        ids = set(ids)
+        return [
+            rds_inst
+            for rds_inst in res
+            # we don't count deleted / failed db instances as existing
+            if (
+                (
+                    rds_inst.status
+                    not in [
+                        RDSDBInstanceStatusEnum.delete_precheck.value,
+                        RDSDBInstanceStatusEnum.deleting.value,
+                        RDSDBInstanceStatusEnum.failed.value,
+                        RDSDBInstanceStatusEnum.restore_error.value,
+                    ]
+                )
+                and (
+                    rds_inst.tags.get(
+                        settings.ID_TAG_KEY,
+                        "THIS_IS_IMPOSSIBLE_TO_MATCH",
+                    )
+                    in ids
+                )
+            )
+        ]
+
+    @classmethod
     def get_ec2(
         cls,
         ec2_client,
         id: str,
     ) -> T.Optional[Ec2Instance]:
         """
-        尝试获取某个 Server 的 EC2 实例信息. 如果 EC2 不存在则返回 None.
+        尝试获取某个 Server 的 EC2 实例信息. 如果 EC2 "不存在" 则返回 None.
+        "不存在" 的含义是这个机器没有被创建, 或是已经被永久删除了. 如果机器存在而是出于启动中,
+        停止中这一类的情况, 这个机器还可以被重新启动, 所以被视为存在.
         """
-        res = Ec2Instance.from_tag_key_value(
-            ec2_client, key=settings.ID_TAG_KEY, value=id
-        )
-        ec2_inst_list = res.all()
+        ec2_inst_list = cls._get_existing_ec2(ec2_client=ec2_client, ids=[id])
         if len(ec2_inst_list) > 1:
             raise ServerNotUniqueError(f"Found multiple EC2 instance with id {id}")
         elif len(ec2_inst_list) == 0:
             return None
         else:
             return ec2_inst_list[0]
 
     @classmethod
     def get_rds(
         cls,
         rds_client,
         id: str,
     ) -> T.Optional[RDSDBInstance]:
         """
-        尝试获取某个 Server 的 RDS 实例信息. 如果 RDS 不存在则返回 None.
+        尝试获取某个 Server 的 RDS 实例信息. 如果 RDS "不存在"则返回 None.
+        "不存在" 的含义是这个数据库没有被创建, 或是已经被永久删除了. 如果机器存在而是出于启动中,
+        停止中这一类的情况, 这个数据库还可以被重新启动, 所以被视为存在.
         """
-        res = RDSDBInstance.from_tag_key_value(
-            rds_client, key=settings.ID_TAG_KEY, value=id
-        )
-        rds_inst_list = res.all()
+        rds_inst_list = cls._get_existing_rds(rds_client=rds_client, ids=[id])
         if len(rds_inst_list) > 1:  # pragma: no cover
             raise ServerNotUniqueError(f"Found multiple RDS instance with id {id}")
         elif len(rds_inst_list) == 0:
             return None
         else:
             return rds_inst_list[0]
 
@@ -87,15 +140,16 @@
     def get_server(
         cls,
         id: str,
         ec2_client,
         rds_client,
     ) -> T.Optional["Server"]:
         """
-        尝试获得某个 Server 的 EC2 和 RDS 信息, 如果任意一个不存在则返回 None.
+        尝试获得某个 Server 的 EC2 和 RDS 信息, 如果任意一个 "不存在" 则返回 None.
+        关于 "不存在" 的定义请参考 :meth:`Server.get_ec2` 和 :meth:`Server.get_rds`.
         该方法是本模块最常用的方法之一. 用例如下:
 
         .. code-block:: python
 
             >>> server = Server.get_server("prod", ec2_client, rds_client)
             >>> server
             Server(
@@ -111,22 +165,24 @@
                     id='db-inst-1',
                     status='available',
                     tags={'realm': 'prod-1'},
                     data=...
                 ),
             )
 
-        如果你想要手动创建一个抽象对象而不立刻尝试获得 Server 的信息, 而是想之后再获取,
-        你可以这样:
+        如果你需要分开判断 EC2 和 RDS 的存在性, 你可以这样:
 
         .. code-block:: python
 
             >>> server = Server(id="prod")
             >>> server.refresh(ec2_client, rds_client)
-
+            >>> server.is_ec2_exists()
+            True
+            >>> server.is_rds_exists()
+            False
         """
         ec2_inst = cls.get_ec2(ec2_client, id)
         if ec2_inst is None:
             return None
         rds_inst = cls.get_rds(rds_client, id)
         if rds_inst is None:  # pragma: no cover
             return None
@@ -156,29 +212,17 @@
             {
                 "prod-1": <Server id="prod-1">,
                 "prod-2": <Server id="prod-2">,
                 "dev-1": <Server id="dev-1">,
                 "dev-2": <Server id="dev-2">,
             }
         """
-        id_set = set(ids)
-
         # batch get data
-        ec2_inst_list = Ec2Instance.from_tag_key_value(
-            ec2_client,
-            key=settings.ID_TAG_KEY,
-            value=ids,
-        ).all()
-        rds_inst_list = list()
-        for rds_inst in RDSDBInstance.query(rds_client):
-            if (
-                rds_inst.tags.get(settings.ID_TAG_KEY, "THIS_IS_IMPOSSIBLE_TO_MATCH")
-                in id_set
-            ):
-                rds_inst_list.append(rds_inst)
+        ec2_inst_list = cls._get_existing_ec2(ec2_client=ec2_client, ids=ids)
+        rds_inst_list = cls._get_existing_rds(rds_client=rds_client, ids=ids)
 
         # group by server id
         ec2_inst_mapper = dict()
         for ec2_inst in ec2_inst_list:
             key = ec2_inst.tags[settings.ID_TAG_KEY]
             try:
                 ec2_inst_mapper[key].append(ec2_inst)
@@ -267,15 +311,15 @@
 
     def refresh(
         self,
         ec2_client,
         rds_client,
     ):
         """
-        重新获取 EC2 和 RDS 实例的信息.
+        重新获取 EC2 和 RDS 实例的信息. 刷新当前类的 ``ec2_inst`` 和 ``rds_inst`` 属性.
         """
         self.ec2_inst = self.get_ec2(ec2_client, self.id)
         self.rds_inst = self.get_rds(rds_client, self.id)
 
     # --------------------------------------------------------------------------
     # Operations
     # --------------------------------------------------------------------------
@@ -291,14 +335,18 @@
         tags: T.Optional[T.Dict[str, str]] = None,
         check_exists: bool = True,
     ):
         """
         Launch a new EC2 instance as the Game server from the AMI.
         The configurations are already optimized for the Game server.
 
+        在服务器运维过程中, 我们都是从自己构建的游戏服务器 AMI 启动 EC2 实例. 它的 Tag 必须
+        要符合一定的规则 (详情请参考 :class:`Server`). 本方法会自动为新的 EC2 实例打上这些
+        必要的 Tag.
+
         Reference:
 
         - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/client/run_instances.html
 
         :param ec2_client: boto3 ec2 client
         :param ami_id: example: "ami-1a2b3c4d"
         :param instance_type: example "t3.small", "t3.medium", "t3.large", "t3.xlarge", "t3.2xlarge
@@ -350,14 +398,18 @@
         tags: T.Optional[T.Dict[str, str]] = None,
         check_exists: bool = True,
     ):
         """
         Launch a new RDS DB instance from the backup snapshot.
         The configurations are already optimized for the Game server.
 
+        在数据库运维过程中, 我们都是从自己备份的 Snapshot 启动 DB 实例. 它的 Tag 必须
+        要符合一定的规则 (详情请参考 :class:`Server`). 本方法会自动为新的 DB 实例打上这些
+        必要的 Tag.
+
         Reference:
 
         - https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds/client/restore_db_instance_from_db_snapshot.html
 
         :param rds_client: boto3 rds client
         :param db_snapshot_identifier: example "my-db-snapshot"
         :param db_instance_class: example "db.t4g.micro", "db.t4g.small", "db.t4g.medium", "db.t4g.large"
@@ -401,46 +453,55 @@
         """
         Associate the given Elastic IP address with the EC2 instance.
         Note that this operation is idempotent, it will disassociate and re-associate
         the Elastic IP address if it is already associated with another EC2 instance
         or this one, and each association will incur a small fee. So I would like
         to check before doing this.
 
+        当对生产服务器进行运维时, 我们需要维护给每个服务器一个固定 IP. 我们可以通过定义一个
+        映射表, 然后用这个方法确保每个服务器的 IP 是正确的 (该方法是幂等的, 如果已经设置好了
+        则什么也不会做).
+
         :param ec2_client: boto3 ec2 client
         :param allocation_id: the EIP allocation id, not the pulibc ip,
             example "eipalloc-1a2b3c4d"
         :param check_exists: check if the EC2 instance exists before associating.
         """
         if check_exists:
             ec2_inst = self.get_ec2(ec2_client, id=self.id)
             if ec2_inst is None:
                 raise ServerAlreadyExistsError(
                     f"EC2 instance {self.id!r} does not exist"
                 )
-            self.ec2_inst = ec2_inst
+
         # check if this allocation id is already associated with an instance
         res = ec2_client.describe_addresses(AllocationIds=[allocation_id])
         address_data = res["Addresses"][0]
         public_id = address_data["PublicIp"]
         instance_id = address_data.get("InstanceId", "invalid-instance-id")
         if instance_id == self.ec2_inst.id:
             return  # already associated
+
+        # associate eip address
         ec2_client.associate_address(
             AllocationId=allocation_id,
             InstanceId=self.ec2_inst.id,
         )
 
     def create_db_snapshot(
         self,
         rds_client,
         check_exists: bool = True,
     ):
         """
         Create a 'manual' DB snapshot for the RDS DB instance.
-        It use the server id and timestamp as the snapshot id.
+        The snapshot id naming convention is "${server_id}-%Y-%m-%d-%H-%M-%S".
+
+        在数据库运维过程中, 我们需要定期备份生产服务器的数据库. 该方法能为我们创建 DB snapshot
+        并合理明明, 打上对应的 Tag.
         """
         if check_exists:
             rds_inst = self.get_rds(rds_client, id=self.id)
             if rds_inst is None:
                 raise ServerNotFoundError(f"RDS DB instance {self.id!r} does not exist")
         now = get_utc_now()
         snapshot_id = "{}-{}".format(
@@ -461,20 +522,23 @@
         rds_client,
         keep_n: int = 3,
         keep_days: int = 365,
     ):
         """
         Clean up old RDS DB snapshots of this server.
 
+        在数据库运维过程中, 我们需要定期备份生产服务器的数据库. 该方法能为我们创建 DB snapshot
+        并合理明明, 打上对应的 Tag.
+
         :param rds_client: boto3 rds client
         :param keep_n: keep the latest N snapshots. this criteria has higher priority.
             for example, even the only N snapshots is very very old, but we still keep them.
         :param keep_days: delete snapshots older than N days if we have more than N snapshots.
 
-        todo: use paginator
+        todo: use paginator to list existing snapshots
         """
         # get the list of manual created snapshots
         res = rds_client.describe_db_snapshots(
             DBInstanceIdentifier=self.rds_inst.id,
             SnapshotType="manual",
             MaxRecords=100,
         )
```

### Comparing `acore_server_metadata-0.2.1/acore_server_metadata/tests/mock_aws.py` & `acore_server_metadata-0.2.2/acore_server_metadata/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.2.1/acore_server_metadata/vendor/pytest_cov_helper.py` & `acore_server_metadata-0.2.2/acore_server_metadata/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.2.1/acore_server_metadata.egg-info/PKG-INFO` & `acore_server_metadata-0.2.2/acore_server_metadata.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore-server-metadata
-Version: 0.2.1
+Version: 0.2.2
 Summary: Azerothcore WOW server metadata for Fleet management.
 Home-page: https://github.com/MacHu-GWU/acore_server_metadata-project
-Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.2.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.2.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -88,15 +88,15 @@
 
 我假设游戏服务器虚拟机和数据库都是在 AWS 上用 EC2 和 RDS 部署的. 所以这个项目只能用于 AWS 环境下的服务器管理.
 
 **关于本项目**
 
 本项目是一个简单的 Python 包, 提供了对一个 realm 服务器的抽象.
 
-用例:
+**基础用例, 获取服务器状态**
 
 .. code-block:: python
 
     # 获取服务器的状态
     >>> import boto3
     >>> from acore_server_metadata.api import Server
     >>> server_id = "prod"
@@ -140,18 +140,22 @@
     {
         "prod-1": <Server id="prod-1">,
         "prod-2": <Server id="prod-2">,
         "dev-1": <Server id="dev-1">,
         "dev-2": <Server id="dev-2">,
     }
 
+**对服务器进行操作**
+
+.. code-block:: python
+
     # 启动新的 EC2
-    >>> server.run_ec2(...)
+    >>> server.run_ec2(ec_client, ami_id, instance_type, ...)
     # 启动新的 DB Instance
-    >>> server.run_rds(...)
+    >>> server.run_rds(rds_client, db_snapshot_identifier, db_instance_class, ...)
     # 关联 EIP 地址
     >>> server.associate_eip_address(...)
     # 创建数据库备份
     >>> server.create_db_snapshot(...)
     # 清理数据库备份
     >>> server.cleanup_db_snapshot(...)
```

### Comparing `acore_server_metadata-0.2.1/acore_server_metadata.egg-info/SOURCES.txt` & `acore_server_metadata-0.2.2/acore_server_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.2.1/release-history.rst` & `acore_server_metadata-0.2.2/release-history.rst`

 * *Files 26% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.2.2 (2023-06-17)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Bugfixes**
+
+- Fix a bug that ``Server.get_ec2`` and ``Server.get_rds`` methods returns terminated ec2 and deleted rds instances. They should be considered as "not exists"
+
+
 0.2.1 (2023-06-16)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - add ``acore_server_metadata.api.Server.run_ec2`` and ``acore_server_metadata.api.Server.run_rds`` method to launch a new EC2 instance or RDS db instance.
 - add ``acore_server_metadata.api.Server.associate_eip_address`` to associate eip address to EC2 instance.
 - add ``acore_server_metadata.api.Server.create_db_snapshot`` to create a manual db snapshot for RDS DB instance.
```

### Comparing `acore_server_metadata-0.2.1/requirements-doc.txt` & `acore_server_metadata-0.2.2/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.2.1/setup.py` & `acore_server_metadata-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.2.1/tests/test_api.py` & `acore_server_metadata-0.2.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.2.1/tests/test_server.py` & `acore_server_metadata-0.2.2/tests/test_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 
 import typing as T
 import moto
+import time
 import pytest
 
 from acore_server_metadata.tests.mock_aws import BaseMockTest
 from acore_server_metadata.settings import settings
 from acore_server_metadata.server import ServerNotUniqueError, Server
 
 
@@ -124,15 +125,24 @@
                 ids=["prod-1", "prod-2"],
                 ec2_client=self.bsm.ec2_client,
                 rds_client=self.bsm.rds_client,
             )
 
     def _test_operations(self):
         server = Server(id="test-operations")
-        # todo
+        self.start_instance(server.id)
+        server.refresh(ec2_client=self.bsm.ec2_client, rds_client=self.bsm.rds_client)
+
+        server.create_db_snapshot(rds_client=self.bsm.rds_client)
+        time.sleep(1)
+        server.create_db_snapshot(rds_client=self.bsm.rds_client)
+        time.sleep(1)
+        server.create_db_snapshot(rds_client=self.bsm.rds_client)
+
+        server.cleanup_db_snapshot(rds_client=self.bsm.rds_client, keep_n=1, keep_days=0)
 
     def test(self):
         self._test()
         self._test_batch_get_server()
         self._test_operations()
```

