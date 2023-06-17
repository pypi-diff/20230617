# Comparing `tmp/nonebot_plugin_sentry-0.4.0.tar.gz` & `tmp/nonebot_plugin_sentry-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_sentry-0.4.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_sentry-0.4.1.tar", max compression
```

## Comparing `nonebot_plugin_sentry-0.4.0.tar` & `nonebot_plugin_sentry-0.4.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1413 2023-06-05 08:16:27.647737 nonebot_plugin_sentry-0.4.0/README.md
--rw-r--r--   0        0        0     1544 2023-06-05 08:16:27.651737 nonebot_plugin_sentry-0.4.0/__init__.py
--rw-r--r--   0        0        0     1071 2023-06-05 08:16:27.651737 nonebot_plugin_sentry-0.4.0/config.py
--rw-r--r--   0        0        0      804 2023-06-05 08:16:27.651737 nonebot_plugin_sentry-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2453 1970-01-01 00:00:00.000000 nonebot_plugin_sentry-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1413 2023-06-17 03:32:38.911058 nonebot_plugin_sentry-0.4.1/README.md
+-rw-r--r--   0        0        0     1544 2023-06-17 03:32:38.911058 nonebot_plugin_sentry-0.4.1/__init__.py
+-rw-r--r--   0        0        0     1077 2023-06-17 03:32:38.911058 nonebot_plugin_sentry-0.4.1/config.py
+-rw-r--r--   0        0        0      804 2023-06-17 03:32:38.911058 nonebot_plugin_sentry-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2453 1970-01-01 00:00:00.000000 nonebot_plugin_sentry-0.4.1/PKG-INFO
```

### Comparing `nonebot_plugin_sentry-0.4.0/README.md` & `nonebot_plugin_sentry-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sentry-0.4.0/__init__.py` & `nonebot_plugin_sentry-0.4.1/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_sentry-0.4.0/config.py` & `nonebot_plugin_sentry-0.4.1/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 @Author         : yanyongyu
 @Date           : 2020-11-23 18:44:18
 @LastEditors    : yanyongyu
-@LastEditTime   : 2023-03-30 19:56:41
+@LastEditTime   : 2023-06-17 10:45:33
 @Description    : Config for Sentry plugin
 @GitHub         : https://github.com/yanyongyu
 """
 __author__ = "yanyongyu"
 
-from typing import Any, Optional
+from typing import Any, Dict, Optional
 
 from nonebot.log import logger
 from pydantic import Extra, BaseModel, validator, root_validator
 
 
 class Config(BaseModel, extra=Extra.allow):
     sentry_dsn: Optional[str]
     sentry_environment: Optional[str] = None
 
     # https://github.com/getsentry/sentry-python/issues/653
     sentry_default_integrations: bool = False
 
     @root_validator(pre=True)
-    def filter_sentry_configs(cls, values: dict[str, Any]):
+    def filter_sentry_configs(cls, values: Dict[str, Any]):
         return {
             key: value for key, value in values.items() if key.startswith("sentry_")
         }
 
     @validator("sentry_dsn", allow_reuse=True)
     def validate_dsn(cls, v: Optional[str]):
         if not v:
```

### Comparing `nonebot_plugin_sentry-0.4.0/pyproject.toml` & `nonebot_plugin_sentry-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-sentry"
-version = "0.4.0"
+version = "0.4.1"
 description = "Push your bot errors to Sentry.io"
 license = "MIT"
 authors = ["yanyongyu <yyy@nonebot.dev>"]
 readme = "README.md"
 homepage = "https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_sentry"
 repository = "https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_sentry"
 documentation = "https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_sentry#readme"
```

### Comparing `nonebot_plugin_sentry-0.4.0/PKG-INFO` & `nonebot_plugin_sentry-0.4.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sentry
-Version: 0.4.0
+Version: 0.4.1
 Summary: Push your bot errors to Sentry.io
 Home-page: https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_sentry
 License: MIT
 Keywords: nonebot,nonebot2,sentry
 Author: yanyongyu
 Author-email: yyy@nonebot.dev
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sentry Version: 0.4.0 Summary: Push
+Metadata-Version: 2.1 Name: nonebot-plugin-sentry Version: 0.4.1 Summary: Push
 your bot errors to Sentry.io Home-page: https://github.com/cscs181/QQ-GitHub-
 Bot/tree/master/src/plugins/nonebot_plugin_sentry License: MIT Keywords:
 nonebot,nonebot2,sentry Author: yanyongyu Author-email: yyy@nonebot.dev
 Requires-Python: >=3.7,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

