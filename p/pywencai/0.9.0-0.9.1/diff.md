# Comparing `tmp/pywencai-0.9.0.tar.gz` & `tmp/pywencai-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywencai-0.9.0.tar", max compression
+gzip compressed data, was "pywencai-0.9.1.tar", max compression
```

## Comparing `pywencai-0.9.0.tar` & `pywencai-0.9.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-06-09 16:19:20.730540 pywencai-0.9.0/LICENSE
--rw-r--r--   0        0        0     3402 2023-06-09 16:19:20.730540 pywencai-0.9.0/README.md
--rw-r--r--   0        0        0      612 2023-06-09 16:19:20.730540 pywencai-0.9.0/pyproject.toml
--rw-r--r--   0        0        0       23 2023-06-09 16:19:20.730540 pywencai-0.9.0/pywencai/__init__.py
--rw-r--r--   0        0        0     5118 2023-06-09 16:19:20.730540 pywencai-0.9.0/pywencai/convert.py
--rw-r--r--   0        0        0      433 2023-06-09 16:19:20.730540 pywencai-0.9.0/pywencai/headers.py
--rw-r--r--   0        0        0    39677 2023-06-09 16:19:20.734540 pywencai-0.9.0/pywencai/hexin-v.js
--rw-r--r--   0        0        0     5023 2023-06-09 16:19:20.734540 pywencai-0.9.0/pywencai/wencai.py
--rw-r--r--   0        0        0     4026 1970-01-01 00:00:00.000000 pywencai-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-17 06:59:41.684857 pywencai-0.9.1/LICENSE
+-rw-r--r--   0        0        0     3401 2023-06-17 06:59:41.684857 pywencai-0.9.1/README.md
+-rw-r--r--   0        0        0      612 2023-06-17 06:59:41.684857 pywencai-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-06-17 06:59:41.684857 pywencai-0.9.1/pywencai/__init__.py
+-rw-r--r--   0        0        0     5195 2023-06-17 06:59:41.684857 pywencai-0.9.1/pywencai/convert.py
+-rw-r--r--   0        0        0      433 2023-06-17 06:59:41.684857 pywencai-0.9.1/pywencai/headers.py
+-rw-r--r--   0        0        0    39677 2023-06-17 06:59:41.684857 pywencai-0.9.1/pywencai/hexin-v.js
+-rw-r--r--   0        0        0     5268 2023-06-17 06:59:41.684857 pywencai-0.9.1/pywencai/wencai.py
+-rw-r--r--   0        0        0     4025 1970-01-01 00:00:00.000000 pywencai-0.9.1/PKG-INFO
```

### Comparing `pywencai-0.9.0/LICENSE` & `pywencai-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pywencai-0.9.0/README.md` & `pywencai-0.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
 #### no_detail
 
 非必填，默认为`False`，当为`True`时，查询一些**详情类问题**不再会返回字典，而返回`None`，可以保证查询结果类型一直为`pd.DataFrame`或`None`。
 
 #### find
 
-非必填，默认为`None`，可以传一个数组，例如`['600519', '0000010']`，数组内的对应标的会排列在DataFrame的最前面。
+非必填，默认为`None`，可以传一个数组，例如`['600519', '000010']`，数组内的对应标的会排列在DataFrame的最前面。
 
 **【注意】** 1、该参数只有结果范围DataFrame时有效。2、配置该参数后，loop参数会失效，结果只会返回前100条。
 
 ### 返回值
 
 当查询的是列表时，该方法返回一个`pandas`的`Dataframe`
```

### Comparing `pywencai-0.9.0/pyproject.toml` & `pywencai-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pywencai"
-version = "0.9.0"
+version = "0.9.1"
 description = ""
 authors = ["pluto <mayuanchi1029@gmail.com>"]
 readme = "README.md"
 
 [[tool.poetry.source]]
 name = "tsinghua"
 url = "https://pypi.tuna.tsinghua.edu.cn/simple/"
```

### Comparing `pywencai-0.9.0/pywencai/convert.py` & `pywencai-0.9.1/pywencai/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,15 @@
     content = _.get(result, 'data.answer.0.txt.0.content')
     if type(content) == str:
         content = json.loads(content)
     components = content['components'] 
     params = {}
     if (len(components) == 1 and _.get(components[0], 'show_type') == 'xuangu_tableV1'):
         params = {
-            'data': xuangu_tableV1_handler(components[0], components)
+            'data': xuangu_tableV1_handler(components[0], components),
+            'row_count' : _.get(components[0], 'data.meta.extra.row_count')
         }
     else:
         params = {
             'data': multi_show_type_handler(components)
         }
     return params
```

### Comparing `pywencai-0.9.0/pywencai/hexin-v.js` & `pywencai-0.9.1/pywencai/hexin-v.js`

 * *Files identical despite different names*

### Comparing `pywencai-0.9.0/pywencai/wencai.py` & `pywencai-0.9.1/pywencai/wencai.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 from typing import List
+import math
 
 import requests as rq
 import pandas as pd
 import time
 import logging
 import pydash as _
 from pywencai.convert import convert
@@ -96,15 +97,15 @@
         target_url = 'http://www.iwencai.com/gateway/urp/v7/landing/getDataList'
         path = 'answer.components.0.data.datas'
     else:
         if isinstance(find, List):
             # 传入股票代码列表时，拼接
             find = ','.join(find)
         data = {
-            'perpage': 500,
+            'perpage': 100,
             'page': 1,
             'source': 'Ths_iwencai_Xuangu',
             'query_type': query_type,
             'question': find,
             **kwargs
         }
         target_url = 'http://www.iwencai.com/unifiedwap/unified-wap/v2/stock-pick/find'
@@ -119,46 +120,46 @@
             data=data,
             headers=headers(cookie),
             timeout=(5, 10),
             **request_params
         )
         result_do = json.loads(res.text)
         data_list = _.get(result_do, path)
+        # print(len(data_list))
+        if len(data_list) == 0:
+            log and logger.error(f'第{data.get("page")}页返回空！')
+            raise Exception("data_list is empty!")
         log and logger.info(f'第{data.get("page")}页成功')
         return pd.DataFrame.from_dict(data_list)
     
     result = while_do(do, retry, sleep, log)
 
     if result is None:
         log and logger.error(f'第{data.get("page")}页失败')
 
     return result
 
 
 def can_loop(loop, count):
-    '''是否继续循环'''
-    if (loop is True):
-        return True
-    else:
-        return count < loop
+    return count < loop
 
 
-def loop_page(loop, **kwargs):
+def loop_page(loop, row_count, **kwargs):
     '''循环分页'''
     count = 0
-    resultPageLen = 1
+    perpage = kwargs.pop('perpage', 100)
+    max_page = math.ceil(row_count / perpage)
     result = None
     if 'page' not in kwargs:
         kwargs['page'] = 1
     initPage = kwargs['page']
-
-    while resultPageLen > 0 and can_loop(loop, count):
+    loop_count = max_page if loop is True else loop
+    while can_loop(loop_count, count):
         kwargs['page'] = initPage + count
         resultPage = get_page(**kwargs)
-        resultPageLen = len(resultPage)
         count = count + 1
         if result is None:
             result = resultPage
         else:
             result = pd.concat([result, resultPage], ignore_index=True)
 
     return result
@@ -170,15 +171,16 @@
     params = get_robot_data(**kwargs)
     data = params.get('data')
     condition = _.get(data, 'condition')
     if condition is not None:
         kwargs = {**kwargs, **data}
         find = kwargs.get('find', None)
         if loop and find is None:
-            return loop_page(loop, **kwargs)
+            row_count = params.get('row_count')
+            return loop_page(loop, row_count, **kwargs)
         else:
             return get_page(**kwargs)
     else:
         no_detail = kwargs.get('no_detail')
         if no_detail != True:
             return data
         else:
```

### Comparing `pywencai-0.9.0/PKG-INFO` & `pywencai-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywencai
-Version: 0.9.0
+Version: 0.9.1
 Summary: 
 Author: pluto
 Author-email: mayuanchi1029@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -127,15 +127,15 @@
 
 #### no_detail
 
 非必填，默认为`False`，当为`True`时，查询一些**详情类问题**不再会返回字典，而返回`None`，可以保证查询结果类型一直为`pd.DataFrame`或`None`。
 
 #### find
 
-非必填，默认为`None`，可以传一个数组，例如`['600519', '0000010']`，数组内的对应标的会排列在DataFrame的最前面。
+非必填，默认为`None`，可以传一个数组，例如`['600519', '000010']`，数组内的对应标的会排列在DataFrame的最前面。
 
 **【注意】** 1、该参数只有结果范围DataFrame时有效。2、配置该参数后，loop参数会失效，结果只会返回前100条。
 
 ### 返回值
 
 当查询的是列表时，该方法返回一个`pandas`的`Dataframe`
```

