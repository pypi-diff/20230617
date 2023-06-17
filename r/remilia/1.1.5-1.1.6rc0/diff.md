# Comparing `tmp/Remilia-1.1.5.tar.gz` & `tmp/remilia-1.1.6rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Remilia-1.1.5.tar", last modified: Fri Apr 21 07:17:00 2023, max compression
+gzip compressed data, was "remilia-1.1.6rc0.tar", last modified: Sat Jun 17 05:29:55 2023, max compression
```

## Comparing `Remilia-1.1.5.tar` & `remilia-1.1.6rc0.tar`

### file list

```diff
@@ -1,64 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.062905 Remilia-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-21 07:16:45.000000 Remilia-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-21 07:17:00.062905 Remilia-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-21 07:16:45.000000 Remilia-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.050905 Remilia-1.1.5/Remilia/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-21 07:16:59.000000 Remilia-1.1.5/Remilia/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.054905 Remilia-1.1.5/Remilia/base/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/base/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/base/directorys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/base/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/base/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/base/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.058905 Remilia-1.1.5/Remilia/jsondb/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/jsondb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/jsondb/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/jsondb/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/jsondb/dbbase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.062905 Remilia-1.1.5/Remilia/lite/
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/LiteData.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/LiteEvent.py
--rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/LiteLog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/LiteMixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/LitePGL.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/LiteResource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/LiteThread.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.062905 Remilia-1.1.5/Remilia/lite/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/v2/ClassMixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/v2/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/v2/DictoryTreeBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/v2/InstanceManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/v2/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/v2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.062905 Remilia-1.1.5/Remilia/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/DecoratorUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/SignParas.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.062905 Remilia-1.1.5/Remilia/utils/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.062905 Remilia-1.1.5/Remilia/utils/cli/prompts_extension/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/cli/prompts_extension/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.062905 Remilia-1.1.5/Remilia/utils/net/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/net/pixiv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.062905 Remilia-1.1.5/Remilia/utils/os/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/os/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.062905 Remilia-1.1.5/Remilia/utils/os/win/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/os/win/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/os/win/exeutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.062905 Remilia-1.1.5/Remilia/utils/thread/
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/thread/Timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/thread/terminable_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.054905 Remilia-1.1.5/Remilia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-21 07:16:59.000000 Remilia-1.1.5/Remilia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-21 07:16:59.000000 Remilia-1.1.5/Remilia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 07:16:59.000000 Remilia-1.1.5/Remilia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 07:16:59.000000 Remilia-1.1.5/Remilia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 07:16:59.000000 Remilia-1.1.5/Remilia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 07:17:00.062905 Remilia-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-21 07:16:45.000000 Remilia-1.1.5/setup.py
+-rw-r--r--   0        0        0     1063 2023-06-17 05:29:17.612915 remilia-1.1.6rc0/LICENSE
+-rw-r--r--   0        0        0     1063 2023-06-17 05:29:17.612915 remilia-1.1.6rc0/LICENSE
+-rw-r--r--   0        0        0      785 2023-06-17 05:29:17.612915 remilia-1.1.6rc0/README.md
+-rw-r--r--   0        0        0      785 2023-06-17 05:29:17.612915 remilia-1.1.6rc0/README.md
+-rw-r--r--   0        0        0     1441 2023-06-17 05:29:55.846594 remilia-1.1.6rc0/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-06-17 05:29:17.612915 remilia-1.1.6rc0/src/Remilia/__init__.py
+-rw-r--r--   0        0        0       68 2023-06-17 05:29:17.612915 remilia-1.1.6rc0/src/Remilia/base/__init__.py
+-rw-r--r--   0        0        0     1697 2023-06-17 05:29:17.612915 remilia-1.1.6rc0/src/Remilia/base/rtypes.py
+-rw-r--r--   0        0        0     4464 2023-06-17 05:29:17.612915 remilia-1.1.6rc0/src/Remilia/log.py
+-rw-r--r--   0        0        0     3104 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/mixin.py
+-rw-r--r--   0        0        0     5120 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/mixin_decorations/__init__.py
+-rw-r--r--   0        0        0     3255 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/mixin_decorations/omixin.py
+-rw-r--r--   0        0        0      997 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/DecoratorUtils.py
+-rw-r--r--   0        0        0     1851 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/SignParas.py
+-rw-r--r--   0        0        0      158 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/__init__.py
+-rw-r--r--   0        0        0      764 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/cli/prompts_extension/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/net/__init__.py
+-rw-r--r--   0        0        0     6605 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/net/pixiv.py
+-rw-r--r--   0        0        0       41 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/os/__init__.py
+-rw-r--r--   0        0        0       51 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/os/win/__init__.py
+-rw-r--r--   0        0        0      360 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/os/win/exeutils.py
+-rw-r--r--   0        0        0     4163 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/thread/Timeout.py
+-rw-r--r--   0        0        0      241 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/thread/__init__.py
+-rw-r--r--   0        0        0     1149 2023-06-17 05:29:17.616916 remilia-1.1.6rc0/src/Remilia/utils/thread/terminable_thread.py
+-rw-r--r--   0        0        0     3258 1970-01-01 00:00:00.000000 remilia-1.1.6rc0/PKG-INFO
```

### Comparing `Remilia-1.1.5/LICENSE` & `remilia-1.1.6rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.5/Remilia/lite/LiteMixin.py` & `remilia-1.1.6rc0/src/Remilia/mixin_decorations/omixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import types,gc,traceback
 
+def collect_attr(target):
+    return [{_:getattr(target,_)} for _ in dir(target) if not _.startswith("__") and not _.endswith("_") and not _.startswith("_") and  not _.endswith("_")]
 
 def safe_mixin(pyClass:object,mixinClass:object):
-   mixin=[{_:getattr(mixinClass,_)} for _ in dir(mixinClass) if not _.startswith("__") and not _.endswith("_") and not _.startswith("_") and  not _.endswith("_")]
+   mixin=collect_attr(mixinClass)
    for liter in mixin:
       for k,v in liter.items():
          setattr(pyClass,k,v)
+         
+         
 def MixInClass(pyClass:object, mixInClass:object, makeAncestor:bool=False,ignoreMagicMethod=False) -> None:
    '''
    :param pyClass: the target class\n
    :param mixInClass: your class\n
    :param makeAncestor: modify the Ancestor of pyClass
    '''
    if makeAncestor:
```

### Comparing `Remilia-1.1.5/Remilia/utils/DecoratorUtils.py` & `remilia-1.1.6rc0/src/Remilia/utils/DecoratorUtils.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.5/Remilia/utils/SignParas.py` & `remilia-1.1.6rc0/src/Remilia/utils/SignParas.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,59 @@
 from inspect import _empty, signature,Parameter
 from types import FunctionType
 from typing import List
 
 
 class ParaFilter:
     def __init__(self,target:FunctionType) -> None:
-        self.args:List=[]
         self.signargs:List[Parameter]=[]
         self.kwargs={}
         self.target=target
         self.__handle()
         self.load_default()
         
     def __handle(self):
         self.signargs=[signarg for _,signarg in signature(self.target).parameters.items()]
             
     def __check(self,raw,sub):
         return issubclass(sub,raw)
     
+    def get_index(self,index):
+        return self.signargs[index]
+    
+    def get_name(self,name) -> Parameter:
+        for para in self.signargs:
+            if para.name == name:
+                return para
+            
+    def index_put(self,index,value):
+        self.update_kwg({self.signargs[index].name:value})
+    
     def check_put(self,atype,value):
-        self.kwargs.update(*[{_.name:value} for _ in self.check_get(atype)])
+        self.update_kwg(*[{_.name:value} for _ in self.check_get(atype)])
 
     def check_put_anno(self,atype):
-        self.kwargs.update(*[{_.name:_.annotation} for _ in self.check_get(atype)])
+        self.update_kwg(*[{_.name:_.annotation} for _ in self.check_get(atype)])
         
     def check_put_handle(self,atype,func):
-        self.kwargs.update(*[{_.name:func(_)} for _ in self.check_get(atype)])
+        self.update_kwg(*[{_.name:func(_)} for _ in self.check_get(atype)])
 
     def check_get(self,atype):
         return [_ for _ in self.signargs if self.__check(atype,_.annotation)]
     
     def load_default(self):
-        self.kwargs.update(*[{_.name:_.default} for _ in self.signargs if _.default != _empty])
+        self.update_kwg(*[{_.name:_.default} for _ in self.signargs if _.default != _empty])
         
     def fill_none(self):
-        self.kwargs.update(*[{_.name:None} for _ in self.signargs if _.default == _empty and _.name not in self.kwargs])
-        
+            
+        self.update_kwg(*[{_.name:None} for _ in self.signargs if _.default == _empty and _.name not in self.kwargs])
+    
+    def update_kwg(self,*dicts):
+        for d in dicts:
+            self.kwargs.update(d)
+    
     def __enter__(self):
+        self.load_default()
         return self
     
     def __exit__(self,*args,**kwargs):
         self.fill_none()
```

### Comparing `Remilia-1.1.5/Remilia/utils/cli/__init__.py` & `remilia-1.1.6rc0/src/Remilia/utils/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.5/Remilia/utils/net/pixiv.py` & `remilia-1.1.6rc0/src/Remilia/utils/net/pixiv.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.5/Remilia/utils/thread/Timeout.py` & `remilia-1.1.6rc0/src/Remilia/utils/thread/Timeout.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.5/Remilia/utils/thread/terminable_thread.py` & `remilia-1.1.6rc0/src/Remilia/utils/thread/terminable_thread.py`

 * *Files identical despite different names*

