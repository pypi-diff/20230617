# Comparing `tmp/zdatabase-0.4.3.tar.gz` & `tmp/zdatabase-0.4.6.tar.gz`

## Comparing `zdatabase-0.4.3.tar` & `zdatabase-0.4.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 zdatabase-0.4.3/src/zdatabase/__init__.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 zdatabase-0.4.3/src/zdatabase/model.py
--rw-r--r--   0        0        0     5710 2020-02-02 00:00:00.000000 zdatabase-0.4.3/src/zdatabase/utility.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 zdatabase-0.4.3/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zdatabase-0.4.3/LICENSE
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zdatabase-0.4.3/README.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 zdatabase-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 zdatabase-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 zdatabase-0.4.6/src/zdatabase/__init__.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 zdatabase-0.4.6/src/zdatabase/model.py
+-rw-r--r--   0        0        0     5887 2020-02-02 00:00:00.000000 zdatabase-0.4.6/src/zdatabase/utility.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 zdatabase-0.4.6/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zdatabase-0.4.6/LICENSE
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zdatabase-0.4.6/README.md
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 zdatabase-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 zdatabase-0.4.6/PKG-INFO
```

### Comparing `zdatabase-0.4.3/src/zdatabase/__init__.py` & `zdatabase-0.4.6/src/zdatabase/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 from sqlalchemy import create_engine, MetaData
 from sqlalchemy.orm import Session, sessionmaker
 from sqlalchemy.ext.declarative import declarative_base
 
 
 class Database:
-    def make_url(self, config, db_type):
-        if db_type == 'postgre':
-            url = 'postgresql://{user}:{password}@{host}:{port}/{db}'.format(**config)
-        else:
-            url = 'mysql+pymysql://{user}:{password}@{host}:{port}/{db}?charset=utf8mb4'.format(**config)
-        return url
-
-    def init(self, url):
+    def init(self, config):
+        url = 'mysql+pymysql://{user}:{password}@{host}:{port}/{db}?charset=utf8mb4'.format(**config)
         engine = create_engine(url)
         metadata = MetaData(bind=engine)
         Session = sessionmaker(autocommit=False, autoflush=False, bind=engine)
         self.session = Session()
         return engine, metadata
```

### Comparing `zdatabase-0.4.3/src/zdatabase/model.py` & `zdatabase-0.4.6/src/zdatabase/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,51 @@
-from zdatabase import Base, db
+from zdatabase import db
 from zdatabase.utility import DatabaseUtility, QueryUtility, MapperUtility
 from inspirare import time
 
 
-class Model(Base, DatabaseUtility, QueryUtility, MapperUtility):
+class Model(db.Model, DatabaseUtility, QueryUtility, MapperUtility):
     __abstract__ = True
+    __schema__ = {}
 
     @classmethod
     def filter(cls, *args, **kwargs):
         return cls.query.filter(*args, **kwargs)
 
     @classmethod
     def clean_params(cls, dict_):
         dict_ = dict_.copy()
         keys = list(dict_.keys())
         for key in keys:
             if key not in cls.keys():  # 无关字段过滤
                 dict_.pop(key)
         return dict_
-    
+
     @classmethod
     def keys(cls):
         return cls.__table__.columns.keys()
-    
+
     def get(self, key):
         return self.__getattribute__(key)
 
     def raw_json(self):
         return {key: self.get(key) for key in self.keys()}
-    
+
     def to_json(self):
         return self.to_json_()
-    
+
     @property
     def key_map(self):
         return {}
-    
+
     @property
     def key_derive_map(self):
         return {}
-    
-    def to_json_(self): # 新方法，待替换
+
+    def to_json_(self):  # 新方法，待替换
         tmp = {}
         for k in self.keys():
             v = self.get(k)
             tmp[k] = v
             for key, func in self.key_map.items():
                 if k == key:
                     tmp[k] = func(v)
@@ -56,27 +57,27 @@
                             func = map_['func']
                             tmp[name] = func(v)
                     else:
                         name = map['name']
                         func = map['func']
                         tmp[name] = func(v)
         return tmp
-    
+
     @staticmethod
     def format_date(value):
         return time.format(value, 'YYYY-MM-DD') if value is not None else ''
-    
+
     @staticmethod
     def format_datetime(value):
         return time.format(value, 'YYYY-MM-DD HH:mm:ss') if value is not None else None
-    
+
     @classmethod
     def new(cls, dict_):
         return cls(**cls.clean_params(dict_))
-    
+
     def add_one(self):
         """添加到数据库缓存"""
         db.session.add(self)
         db.session.flush()
         return self
 
     def update(self, dict_):
@@ -86,9 +87,7 @@
             setattr(self, k, v)
         return self
 
     def merge(self):
         """合并"""
         db.session.merge(self)
         return self
-
-
```

### Comparing `zdatabase-0.4.3/src/zdatabase/utility.py` & `zdatabase-0.4.6/src/zdatabase/utility.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-from zdatabase import db
+from zdatabase import session
+from jsonschema import validate
 
 
 class DatabaseUtility:
     @staticmethod
     def flush():
-        db.session.flush()
+        session.flush()
 
     @staticmethod
     def commit():
-        db.session.commit()
+        session.commit()
 
     @staticmethod
     def query_(*args, **kwargs):
-        return db.session.query(*args, **kwargs)
+        return session.query(*args, **kwargs)
 
     @staticmethod
     def add_all(items):
-        db.session.add_all(items)
-        db.session.commit()
+        session.add_all(items)
+        session.commit()
         return items
 
 
 class QueryUtility:
     @classmethod
     def select(cls, params, conds):
         """ 筛选(模糊匹配）
@@ -29,15 +30,15 @@
         """
         flts = []
         for cond in conds:
             value = params.get(cond)
             if value:
                 flts.append(getattr(cls, cond).like(f'%{value}%'))
         return flts
-    
+
     @classmethod
     def select_(cls, params, conds):
         """ 筛选(精确匹配）
         ?name=1&asset_sn=2019-BG-5453
         """
         flts = []
         for cond in conds:
@@ -102,15 +103,15 @@
         return rst
 
 
 class MapperUtility:
     @staticmethod
     def jsonlize(items):
         return [item.to_json() for item in items]
-    
+
     @classmethod
     def make_flts(cls, **kwargs):
         flts = []
         for k, v in kwargs.items():
             flts += [getattr(cls, k) == v]
         return flts
 
@@ -123,40 +124,40 @@
     def add_(cls, data):
         obj = cls.new(data)
         obj.add_one()
         return obj
 
     @classmethod
     def add(cls, data):
+        validate(instance=data, schema=cls.__schema__)
         obj = cls.add_(data)
         cls.commit()
         return obj
 
     @classmethod
     def add_list_(cls, items):
         for item in items:
             cls.add_(item)
         cls.commit()
 
     @classmethod
     def save_(cls, primary_key, data):
+        validate(instance=data, schema=cls.__schema__)
         obj = cls.get_(primary_key)
         if obj:
             obj.update(data)
         else:
-            obj = cls.add_(data)
+            cls.add_(data)
         cls.commit()
-        return obj
 
     @classmethod
     def update_(cls, primary_key, data):
         obj = cls.get_(primary_key)
-        if obj:
-            obj.update(data)
-            cls.commit()
+        obj.update(data)
+        cls.commit()
 
     @classmethod
     def get_(cls, primary_key):
         return cls.query.get(primary_key)
 
     @classmethod
     def get_json(cls, primary_key):
@@ -174,15 +175,15 @@
 
     @classmethod
     def get_page(cls, **kwargs):
         pagination = {
             'page_size': kwargs.pop('page_size', 20),
             'page_num': kwargs.pop('page_num', 1)
         }
-        query = cls.make_query(**kwargs).order_by(cls.id.desc())
+        query = cls.make_query(**kwargs)
         return cls.paginate(query, pagination)
 
     @classmethod
     def get_all_(cls):
         return cls.filter().all()
 
     @classmethod
@@ -203,8 +204,12 @@
             a, b = item
             rst_map[a] = b
         return rst_map
 
     @classmethod
     def delete_list_(cls, **kwargs):
         cls.make_query(**kwargs).delete(synchronize_session=False)
+
+    @classmethod
+    def delete_list(cls, **kwargs):
+        cls.make_query(**kwargs).delete(synchronize_session=False)
         cls.commit()
```

### Comparing `zdatabase-0.4.3/LICENSE` & `zdatabase-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zdatabase-0.4.3/pyproject.toml` & `zdatabase-0.4.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zdatabase"
-version = "0.4.3"
+version = "0.4.6"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen database library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
   "sqlalchemy==1.4.39",
+  "jsonschema==4.17.3",
   "inspirare"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `zdatabase-0.4.3/PKG-INFO` & `zdatabase-0.4.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: zdatabase
-Version: 0.4.3
+Version: 0.4.6
 Summary: zen database library
 Project-URL: Homepage, https://github.com/inspirare6/zdatabase
 Project-URL: Bug Tracker, https://github.com/inspirare6/zdatabase/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: inspirare
+Requires-Dist: jsonschema==4.17.3
 Requires-Dist: sqlalchemy==1.4.39
 Description-Content-Type: text/markdown
 
 # zdb
 
 Zen database library.
```

