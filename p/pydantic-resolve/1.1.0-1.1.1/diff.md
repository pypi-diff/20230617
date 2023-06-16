# Comparing `tmp/pydantic_resolve-1.1.0.tar.gz` & `tmp/pydantic_resolve-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_resolve-1.1.0.tar", max compression
+gzip compressed data, was "pydantic_resolve-1.1.1.tar", max compression
```

## Comparing `pydantic_resolve-1.1.0.tar` & `pydantic_resolve-1.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.1.0/LICENSE
--rw-r--r--   0        0        0      550 2023-06-16 10:18:24.373879 pydantic_resolve-1.1.0/pydantic_resolve/__init__.py
--rw-r--r--   0        0        0       19 2023-04-05 08:27:57.212146 pydantic_resolve-1.1.0/pydantic_resolve/constant.py
--rw-r--r--   0        0        0     2040 2023-06-10 09:29:05.251120 pydantic_resolve-1.1.0/pydantic_resolve/core.py
--rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.1.0/pydantic_resolve/exceptions.py
--rw-r--r--   0        0        0     4678 2023-06-16 10:28:47.894705 pydantic_resolve-1.1.0/pydantic_resolve/resolver.py
--rw-r--r--   0        0        0     1482 2023-06-16 10:23:24.885805 pydantic_resolve-1.1.0/pydantic_resolve/util.py
--rw-r--r--   0        0        0      814 2023-06-16 10:26:09.328880 pydantic_resolve-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    12153 2023-06-11 08:33:24.276635 pydantic_resolve-1.1.0/README.md
--rw-r--r--   0        0        0    12694 1970-01-01 00:00:00.000000 pydantic_resolve-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.1.1/LICENSE
+-rw-r--r--   0        0        0      550 2023-06-16 10:18:24.373879 pydantic_resolve-1.1.1/pydantic_resolve/__init__.py
+-rw-r--r--   0        0        0       19 2023-04-05 08:27:57.212146 pydantic_resolve-1.1.1/pydantic_resolve/constant.py
+-rw-r--r--   0        0        0     1990 2023-06-16 21:31:45.713490 pydantic_resolve-1.1.1/pydantic_resolve/core.py
+-rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.1.1/pydantic_resolve/exceptions.py
+-rw-r--r--   0        0        0     4620 2023-06-16 21:32:01.947620 pydantic_resolve-1.1.1/pydantic_resolve/resolver.py
+-rw-r--r--   0        0        0     2833 2023-06-16 23:09:49.647683 pydantic_resolve-1.1.1/pydantic_resolve/util.py
+-rw-r--r--   0        0        0      814 2023-06-16 23:13:04.858829 pydantic_resolve-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5622 2023-06-16 21:48:45.117807 pydantic_resolve-1.1.1/README.md
+-rw-r--r--   0        0        0     6283 1970-01-01 00:00:00.000000 pydantic_resolve-1.1.1/PKG-INFO
```

### Comparing `pydantic_resolve-1.1.0/LICENSE` & `pydantic_resolve-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.1.0/pydantic_resolve/__init__.py` & `pydantic_resolve-1.1.1/pydantic_resolve/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.1.0/pydantic_resolve/core.py` & `pydantic_resolve-1.1.1/pydantic_resolve/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,18 +31,15 @@
         val = item()
     except AttributeError as e:
         if str(e) == "'Depends' object has no attribute 'load'":  
             # TODO: str(e) may changes in future, not stable
             raise DataloaderDependCantBeResolved("DataLoader used in schema, use Resolver().resolve() instead")
         raise e
 
-    if iscoroutine(val):  # async def func()
-        val = await val
-
-    if asyncio.isfuture(val):
+    while iscoroutine(val) or asyncio.isfuture(val):
         val = await val
 
     val = await resolve(val)  
 
     replace_attr_name = field.replace(PREFIX, '')
     if hasattr(target, replace_attr_name):
         target.__setattr__(replace_attr_name, val)
```

### Comparing `pydantic_resolve-1.1.0/pydantic_resolve/resolver.py` & `pydantic_resolve-1.1.1/pydantic_resolve/resolver.py`

 * *Files 7% similar despite different names*

```diff
@@ -93,18 +93,15 @@
         if not hasattr(target, target_attr_name):
             raise ResolverTargetAttrNotFound(f"attribute {target_attr_name} not found")
 
         if self.ensure_type:
             if not item.__annotations__:
                 raise MissingAnnotationError(f'{field}: return annotation is required')
 
-        if iscoroutine(val):  # async def func()
-            val = await val
-
-        if asyncio.isfuture(val):
+        while iscoroutine(val) or asyncio.isfuture(val):
             val = await val
 
         val = await self.resolve(val)  
 
         target.__setattr__(target_attr_name, val)
 
     async def resolve(self, target: T) -> T:
```

### Comparing `pydantic_resolve-1.1.0/pyproject.toml` & `pydantic_resolve-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-resolve"
-version = "1.1.0"
+version = "1.1.1"
 description = "Make pydantic have a GraphQL-like assembly experience."
 authors = ["tangkikodo <allmonday@126.com>"]
 readme = "README.md"
 repository = "https://github.com/allmonday/pydantic_resolve"
 keywords = ["pydantic", "fastapi"]
 license = "MIT"
 packages = [{include = "pydantic_resolve"}]
```

