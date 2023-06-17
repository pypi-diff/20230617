# Comparing `tmp/redis-limit-0.0.2.tar.gz` & `tmp/redis-limit-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-limit-0.0.2.tar", last modified: Sat Jun 17 06:10:39 2023, max compression
+gzip compressed data, was "redis-limit-0.0.3.tar", last modified: Sat Jun 17 06:35:26 2023, max compression
```

## Comparing `redis-limit-0.0.2.tar` & `redis-limit-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-17 06:10:39.299940 redis-limit-0.0.2/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      116 2023-06-17 06:10:39.297666 redis-limit-0.0.2/PKG-INFO
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-17 06:10:39.217948 redis-limit-0.0.2/redis_limit/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      180 2023-06-17 04:43:57.000000 redis-limit-0.0.2/redis_limit/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      677 2023-06-17 06:07:38.000000 redis-limit-0.0.2/redis_limit/conf.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7247 2023-06-17 06:07:38.000000 redis-limit-0.0.2/redis_limit/limit.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2746 2023-06-17 06:07:38.000000 redis-limit-0.0.2/redis_limit/lock.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3150 2023-06-17 03:02:52.000000 redis-limit-0.0.2/redis_limit/lua_script.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-17 06:10:39.275257 redis-limit-0.0.2/redis_limit.egg-info/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      116 2023-06-17 06:10:39.000000 redis-limit-0.0.2/redis_limit.egg-info/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      307 2023-06-17 06:10:39.000000 redis-limit-0.0.2/redis_limit.egg-info/SOURCES.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-17 06:10:39.000000 redis-limit-0.0.2/redis_limit.egg-info/dependency_links.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       13 2023-06-17 06:10:39.000000 redis-limit-0.0.2/redis_limit.egg-info/requires.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       12 2023-06-17 06:10:39.000000 redis-limit-0.0.2/redis_limit.egg-info/top_level.txt
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-17 06:10:39.302207 redis-limit-0.0.2/setup.cfg
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      355 2023-06-17 06:10:37.000000 redis-limit-0.0.2/setup.py
-drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-17 06:10:39.285738 redis-limit-0.0.2/test/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      486 2023-06-15 12:01:46.000000 redis-limit-0.0.2/test/test1.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-17 06:35:26.809166 redis-limit-0.0.3/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      116 2023-06-17 06:35:26.806379 redis-limit-0.0.3/PKG-INFO
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-17 06:35:26.729637 redis-limit-0.0.3/redis_limit/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      180 2023-06-17 04:43:57.000000 redis-limit-0.0.3/redis_limit/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      695 2023-06-17 06:23:12.000000 redis-limit-0.0.3/redis_limit/conf.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7247 2023-06-17 06:07:38.000000 redis-limit-0.0.3/redis_limit/limit.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2746 2023-06-17 06:07:38.000000 redis-limit-0.0.3/redis_limit/lock.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3150 2023-06-17 03:02:52.000000 redis-limit-0.0.3/redis_limit/lua_script.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-17 06:35:26.783652 redis-limit-0.0.3/redis_limit.egg-info/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      116 2023-06-17 06:35:26.000000 redis-limit-0.0.3/redis_limit.egg-info/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      307 2023-06-17 06:35:26.000000 redis-limit-0.0.3/redis_limit.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-17 06:35:26.000000 redis-limit-0.0.3/redis_limit.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       13 2023-06-17 06:35:26.000000 redis-limit-0.0.3/redis_limit.egg-info/requires.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       12 2023-06-17 06:35:26.000000 redis-limit-0.0.3/redis_limit.egg-info/top_level.txt
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-17 06:35:26.810164 redis-limit-0.0.3/setup.cfg
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      355 2023-06-17 06:35:22.000000 redis-limit-0.0.3/setup.py
+drwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-17 06:35:26.796306 redis-limit-0.0.3/test/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      486 2023-06-15 12:01:46.000000 redis-limit-0.0.3/test/test1.py
```

### Comparing `redis-limit-0.0.2/redis_limit/conf.py` & `redis-limit-0.0.3/redis_limit/conf.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,8 +16,9 @@
     elif rv is None:
         logger.warning("'{}' uses default value: {}".format(env_name, default))
         rv = default
     if arg_formatter is not None:
         rv = arg_formatter(rv)
     return rv
 
-REDIS_URL = getenv('REDIS_URL', 'redis://localhost:6379/0')
+
+REDIS_URL = get_env('REDIS_URL', 'redis://localhost:6379/0', required=True)
```

### Comparing `redis-limit-0.0.2/redis_limit/limit.py` & `redis-limit-0.0.3/redis_limit/limit.py`

 * *Files identical despite different names*

### Comparing `redis-limit-0.0.2/redis_limit/lock.py` & `redis-limit-0.0.3/redis_limit/lock.py`

 * *Files identical despite different names*

### Comparing `redis-limit-0.0.2/redis_limit/lua_script.py` & `redis-limit-0.0.3/redis_limit/lua_script.py`

 * *Files identical despite different names*

