# Comparing `tmp/browser-cookie3-0.9.0.tar.gz` & `tmp/browser-cookie3-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/browser-cookie3-0.9.0.tar", last modified: Thu Dec 19 15:41:20 2019, max compression
+gzip compressed data, was "dist/browser-cookie3-0.9.1.tar", last modified: Fri Dec 20 09:47:57 2019, max compression
```

## Comparing `browser-cookie3-0.9.0.tar` & `browser-cookie3-0.9.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
-drwxr-xr-x   0 boris     (1000) users      (100)        0 2019-12-19 15:41:20.000000 browser-cookie3-0.9.0/
--rw-r--r--   0 boris     (1000) users      (100)      388 2019-12-19 15:41:20.000000 browser-cookie3-0.9.0/PKG-INFO
-lrwxrwxrwx   0 boris     (1000) users      (100)        0 2019-03-18 10:01:26.000000 browser-cookie3-0.9.0/README -> README.md
--rw-r--r--   0 boris     (1000) users      (100)     4550 2019-12-19 15:38:11.000000 browser-cookie3-0.9.0/README.md
--rw-r--r--   0 boris     (1000) users      (100)    15580 2019-12-19 15:38:11.000000 browser-cookie3-0.9.0/__init__.py
--rw-r--r--   0 boris     (1000) users      (100)      608 2019-12-19 15:40:12.000000 browser-cookie3-0.9.0/setup.py
+drwxr-xr-x   0 boris     (1000) users      (100)        0 2019-12-20 09:47:57.000000 browser-cookie3-0.9.1/
+-rw-r--r--   0 boris     (1000) users      (100)      388 2019-12-20 09:47:57.000000 browser-cookie3-0.9.1/PKG-INFO
+lrwxrwxrwx   0 boris     (1000) users      (100)        0 2019-03-18 10:01:26.000000 browser-cookie3-0.9.1/README -> README.md
+-rw-r--r--   0 boris     (1000) users      (100)     4550 2019-12-19 15:38:11.000000 browser-cookie3-0.9.1/README.md
+-rw-r--r--   0 boris     (1000) users      (100)    15714 2019-12-20 09:47:19.000000 browser-cookie3-0.9.1/__init__.py
+-rw-r--r--   0 boris     (1000) users      (100)      608 2019-12-20 09:47:35.000000 browser-cookie3-0.9.1/setup.py
```

### Comparing `browser-cookie3-0.9.0/README.md` & `browser-cookie3-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `browser-cookie3-0.9.0/__init__.py` & `browser-cookie3-0.9.1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,17 @@
                         'FROM cookies WHERE host_key like "%{}%";'.format(self.domain_name))
 
         cj = http.cookiejar.CookieJar()
         epoch_start = datetime.datetime(1601,1,1)
         for item in cur.fetchall():
             host, path, secure, expires, name = item[:5]
             if item[3] != 0:
-                delta = datetime.timedelta(microseconds=int(item[3]))
+                # ensure dates don't exceed the datetime limit of year 10000
+                offset = min(int(item[3]), 265000000000000000)
+                delta = datetime.timedelta(microseconds=offset)
                 expires = epoch_start + delta
                 expires = expires.timestamp()
             value = self._decrypt(item[5], item[6])
             c = create_cookie(host, path, secure, expires, name, value)
             cj.set_cookie(c)
         con.close()
         return cj
```

### Comparing `browser-cookie3-0.9.0/setup.py` & `browser-cookie3-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='browser-cookie3',
-    version='0.9.0',
+    version='0.9.1',
     packages=['browser_cookie3'],
     package_dir={'browser_cookie3' : '.'}, # look for package contents in current directory
     author='Boris Babic',
     author_email='boris.ivan.babic@gmail.com',
     description='Loads cookies from your browser into a cookiejar object so can download with urllib and other libraries the same content you see in the web browser.',
     url='https://github.com/borisbabic/browser_cookie3',
     install_requires=['pyaes','pbkdf2','keyring','lz4', 'configparser'],
```

