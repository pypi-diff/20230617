# Comparing `tmp/opensearch-orm-0.1.6.tar.gz` & `tmp/opensearch_orm-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensearch-orm-0.1.6.tar", max compression
+gzip compressed data, was "opensearch_orm-0.1.7.tar", max compression
```

## Comparing `opensearch-orm-0.1.6.tar` & `opensearch_orm-0.1.7.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1061 2022-09-22 05:39:58.892875 opensearch-orm-0.1.6/LICENSE
--rw-r--r--   0        0        0     2647 2022-09-22 14:28:28.556141 opensearch-orm-0.1.6/README.md
--rw-r--r--   0        0        0      120 2022-09-22 05:51:55.452010 opensearch-orm-0.1.6/opensearchorm/__init__.py
--rw-r--r--   0        0        0     1456 2022-09-22 07:03:20.086683 opensearch-orm-0.1.6/opensearchorm/aggs.py
--rw-r--r--   0        0        0      254 2022-09-22 05:39:58.892875 opensearch-orm-0.1.6/opensearchorm/model.py
--rw-r--r--   0        0        0     5530 2022-09-22 14:28:28.566141 opensearch-orm-0.1.6/opensearchorm/query.py
--rw-r--r--   0        0        0     5085 2022-09-26 14:29:08.428407 opensearch-orm-0.1.6/opensearchorm/session.py
--rw-r--r--   0        0        0      497 2022-09-22 07:26:55.969236 opensearch-orm-0.1.6/opensearchorm/utils.py
--rw-r--r--   0        0        0      444 2022-09-26 14:29:25.868406 opensearch-orm-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3409 1970-01-01 00:00:00.000000 opensearch-orm-0.1.6/setup.py
--rw-r--r--   0        0        0     3211 1970-01-01 00:00:00.000000 opensearch-orm-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-16 08:43:48.684499 opensearch_orm-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3199 2023-06-17 07:12:43.411841 opensearch_orm-0.1.7/README.md
+-rw-r--r--   0        0        0      120 2023-04-16 08:43:48.684682 opensearch_orm-0.1.7/opensearchorm/__init__.py
+-rw-r--r--   0        0        0     1456 2023-04-16 08:43:48.684860 opensearch_orm-0.1.7/opensearchorm/aggs.py
+-rw-r--r--   0        0        0      254 2023-04-16 08:43:48.684942 opensearch_orm-0.1.7/opensearchorm/model.py
+-rw-r--r--   0        0        0     5570 2023-06-17 04:45:40.491762 opensearch_orm-0.1.7/opensearchorm/query.py
+-rw-r--r--   0        0        0     6281 2023-04-16 09:17:40.380146 opensearch_orm-0.1.7/opensearchorm/session.py
+-rw-r--r--   0        0        0      497 2023-04-16 08:43:48.685191 opensearch_orm-0.1.7/opensearchorm/utils.py
+-rw-r--r--   0        0        0      444 2023-06-17 07:09:39.781719 opensearch_orm-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3814 1970-01-01 00:00:00.000000 opensearch_orm-0.1.7/PKG-INFO
```

### Comparing `opensearch-orm-0.1.6/LICENSE` & `opensearch_orm-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `opensearch-orm-0.1.6/README.md` & `opensearch_orm-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,22 @@
 
     # equals to
     result = (
         session.select(UserLog)
         .filter(Contains('method', ['GET', 'POST']))
         .fetch()
     )
+
+    # single value
+    result = (
+        session.select(UserLog)
+        .filter(method__contains='GET')
+        .fetch()
+    )
+    print(result)
 ```
 
 ## exclude
 ``` python
 # {'bool': {'must_not': [{'match_phrase': {'method': 'get'}}, {'match_phrase': {'path': '/login'}}], 'should': [], 'filter': []}}
 with SearchSession() as session:
     result = (
@@ -101,7 +109,26 @@
     result = (
         session.select(UserLog)
         .aggregate(Terms('path.keyword').nested(Cardinality('remote_ip,keyword')), request_timeout=300)
     )
     print(result)
     # result -> {'path': 1, 'path2': 2}
 ```
+
+## scroll
+```
+with SearchSession() as session:
+    start = datetime(2023, 4, 15, 19, tzinfo=TZ)
+    end = datetime(2023, 4, 15, 21, tzinfo=TZ)
+
+    scroll = (
+        session.select(Model)
+        .filter(
+            created__gte=start,
+            created__lte=end,
+        )
+        .limit(10000)
+        .scroll('1m')
+    )
+    for records in scroll:
+        print('-------scroll', len(records))
+```
```

### Comparing `opensearch-orm-0.1.6/opensearchorm/aggs.py` & `opensearch_orm-0.1.7/opensearchorm/aggs.py`

 * *Files identical despite different names*

### Comparing `opensearch-orm-0.1.6/opensearchorm/query.py` & `opensearch_orm-0.1.7/opensearchorm/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     GTE = '__gte'
     GT = '__gt'
     LTE = '__lte'
     LT = '__lt'
 
 
 OPERATOR_FUNCTIONS: Dict[Operator, Callable[[str, Any], Expr]] = {
-    Operator.CONTAINS: lambda field, value: Contains(field, value),
+    Operator.CONTAINS: lambda field, value: Contains(field, value if isinstance(value, list) else [value]),
     Operator.PREFIX: lambda field, value: MatchPhrasePrefix(field, value),
     Operator.REGEXP: lambda field, value: RegExp(field, value),
     Operator.GTE: lambda field, value: Range(field, (value, None)),
     Operator.GT: lambda field, value: Range(field, (value, None), left_open=True),
     Operator.LTE: lambda field, value: Range(field, (None, value)),
     Operator.LT: lambda field, value: Range(field, (None, value), right_open=True),
 }
```

### Comparing `opensearch-orm-0.1.6/setup.py` & `opensearch_orm-0.1.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,152 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['opensearchorm']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['opensearch-py>=2.0.0,<3.0.0',
- 'pydantic>=1.10.2,<2.0.0',
- 'pytz>=2022.2.1,<2023.0.0']
-
-setup_kwargs = {
-    'name': 'opensearch-orm',
-    'version': '0.1.6',
-    'description': '',
-    'long_description': "# OpenSearch ORM\n`opensearch-orm` is a high-level OpenSearch ORM for Python. The query syntax is similar to django-orm.\n\nMay be compatible with Elasticsearch, depending on opensearch-py.\n\n\n# Installation\n``` bash\npip install opensearch-orm\n```\n\n\n# Getting Started\n\nFirst, define your document model with indexing pattern.\n``` python\nfrom opensearchorm import SearchSession, BaseModel\n\n\nclass UserLog(BaseModel):\n    __index__ = 'user_access_log-*'\n\n    method: str\n    path: str\n    remote_ip: str\n    created: datetime\n```\n\n\nYou can use django-like syntax or typed query expressions together.\n## filter\n``` python\n# {'bool': {'must_not': [], 'should': [], 'filter': [{'range': {'created': {'gte': '2022-09-01'}}}, {'match_phrase': {'remote_ip': '127.0.0.1'}}]}}        \nwith SearchSession() as session:\n    result = (\n        session.select(UserLog)\n        .filter(created__gte='2022-09-01', remote_ip='127.0.0.1')\n        .fetch()\n    )\n    print(result)\n\n    # equals to\n    result = (\n        session.select(UserLog)\n        .filter(Range('created', date(2022, 9, 1)), remote_ip='127.0.0.1')\n        .fetch()\n    )\n```\n## contains\n``` python\n# {'bool': {'must_not': [], 'should': [], 'filter': [{'bool': {'should': [{'match_phrase': {'method': 'GET'}}, {'match_phrase': {'method': 'POST'}}], 'minimum_should_match': 1}}]}}      \nwith SearchSession() as session:\n    result = (\n        session.select(UserLog)\n        .filter(method__contains=['GET', 'POST'])\n        .fetch()\n    )\n    print(result)\n\n    # equals to\n    result = (\n        session.select(UserLog)\n        .filter(Contains('method', ['GET', 'POST']))\n        .fetch()\n    )\n```\n\n## exclude\n``` python\n# {'bool': {'must_not': [{'match_phrase': {'method': 'get'}}, {'match_phrase': {'path': '/login'}}], 'should': [], 'filter': []}}\nwith SearchSession() as session:\n    result = (\n        session.select(UserLog)\n        .exclude(method='get', path='/login')\n        .fetch()\n    )\n    print(result)\n```\n\n\n## paginate\n``` python\nwith SearchSession() as session:\n    result = (\n        session.select(UserLog)\n        .filter(method='get')\n        .limit(100)\n        .offset(100)\n        .fetch()\n    )\n    print(result)\n```\n\n## aggregations\ngroup by path and count unique remote_ip.\n\n``` python\nwith SearchSession() as session:\n    # aggregate text field need use a keyword field instead\n    # request_timeout argument will be passed on to the opensearch-py\n    result = (\n        session.select(UserLog)\n        .aggregate(Terms('path.keyword').nested(Cardinality('remote_ip,keyword')), request_timeout=300)\n    )\n    print(result)\n    # result -> {'path': 1, 'path2': 2}\n```\n",
-    'author': 'yim7',
-    'author_email': 'yimchiu7@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: opensearch-orm
+Version: 0.1.7
+Summary: 
+Author: yim7
+Author-email: yimchiu7@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: opensearch-py (>=2.0.0,<3.0.0)
+Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Requires-Dist: pytz (>=2022.2.1,<2023.0.0)
+Description-Content-Type: text/markdown
+
+# OpenSearch ORM
+`opensearch-orm` is a high-level OpenSearch ORM for Python. The query syntax is similar to django-orm.
+
+May be compatible with Elasticsearch, depending on opensearch-py.
+
+
+# Installation
+``` bash
+pip install opensearch-orm
+```
+
+
+# Getting Started
+
+First, define your document model with indexing pattern.
+``` python
+from opensearchorm import SearchSession, BaseModel
+
+
+class UserLog(BaseModel):
+    __index__ = 'user_access_log-*'
+
+    method: str
+    path: str
+    remote_ip: str
+    created: datetime
+```
+
+
+You can use django-like syntax or typed query expressions together.
+## filter
+``` python
+# {'bool': {'must_not': [], 'should': [], 'filter': [{'range': {'created': {'gte': '2022-09-01'}}}, {'match_phrase': {'remote_ip': '127.0.0.1'}}]}}        
+with SearchSession() as session:
+    result = (
+        session.select(UserLog)
+        .filter(created__gte='2022-09-01', remote_ip='127.0.0.1')
+        .fetch()
+    )
+    print(result)
+
+    # equals to
+    result = (
+        session.select(UserLog)
+        .filter(Range('created', date(2022, 9, 1)), remote_ip='127.0.0.1')
+        .fetch()
+    )
+```
+## contains
+``` python
+# {'bool': {'must_not': [], 'should': [], 'filter': [{'bool': {'should': [{'match_phrase': {'method': 'GET'}}, {'match_phrase': {'method': 'POST'}}], 'minimum_should_match': 1}}]}}      
+with SearchSession() as session:
+    result = (
+        session.select(UserLog)
+        .filter(method__contains=['GET', 'POST'])
+        .fetch()
+    )
+    print(result)
+
+    # equals to
+    result = (
+        session.select(UserLog)
+        .filter(Contains('method', ['GET', 'POST']))
+        .fetch()
+    )
+
+    # single value
+    result = (
+        session.select(UserLog)
+        .filter(method__contains='GET')
+        .fetch()
+    )
+    print(result)
+```
+
+## exclude
+``` python
+# {'bool': {'must_not': [{'match_phrase': {'method': 'get'}}, {'match_phrase': {'path': '/login'}}], 'should': [], 'filter': []}}
+with SearchSession() as session:
+    result = (
+        session.select(UserLog)
+        .exclude(method='get', path='/login')
+        .fetch()
+    )
+    print(result)
+```
+
+
+## paginate
+``` python
+with SearchSession() as session:
+    result = (
+        session.select(UserLog)
+        .filter(method='get')
+        .limit(100)
+        .offset(100)
+        .fetch()
+    )
+    print(result)
+```
+
+## aggregations
+group by path and count unique remote_ip.
+
+``` python
+with SearchSession() as session:
+    # aggregate text field need use a keyword field instead
+    # request_timeout argument will be passed on to the opensearch-py
+    result = (
+        session.select(UserLog)
+        .aggregate(Terms('path.keyword').nested(Cardinality('remote_ip,keyword')), request_timeout=300)
+    )
+    print(result)
+    # result -> {'path': 1, 'path2': 2}
+```
+
+## scroll
+```
+with SearchSession() as session:
+    start = datetime(2023, 4, 15, 19, tzinfo=TZ)
+    end = datetime(2023, 4, 15, 21, tzinfo=TZ)
+
+    scroll = (
+        session.select(Model)
+        .filter(
+            created__gte=start,
+            created__lte=end,
+        )
+        .limit(10000)
+        .scroll('1m')
+    )
+    for records in scroll:
+        print('-------scroll', len(records))
+```
```

