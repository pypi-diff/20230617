# Comparing `tmp/revproxy_auth-0.1.7.tar.gz` & `tmp/revproxy_auth-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revproxy_auth-0.1.7.tar", last modified: Tue Jun 13 06:47:11 2023, max compression
+gzip compressed data, was "revproxy_auth-0.1.8.tar", last modified: Sat Jun 17 14:07:06 2023, max compression
```

## Comparing `revproxy_auth-0.1.7.tar` & `revproxy_auth-0.1.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:11.611762 revproxy_auth-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-13 06:47:11.611762 revproxy_auth-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:11.607762 revproxy_auth-0.1.7/revproxy_auth/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/revproxy_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/revproxy_auth/config-template.yml
--rw-r--r--   0 runner    (1001) docker     (123)    19577 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/revproxy_auth/revproxy_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:11.607762 revproxy_auth-0.1.7/revproxy_auth/revproxy_auth_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:11.611762 revproxy_auth-0.1.7/revproxy_auth/revproxy_auth_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/revproxy_auth/revproxy_auth_static/css/view.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:11.611762 revproxy_auth-0.1.7/revproxy_auth/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/revproxy_auth/templates/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:11.611762 revproxy_auth-0.1.7/revproxy_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-13 06:47:11.000000 revproxy_auth-0.1.7/revproxy_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-13 06:47:11.000000 revproxy_auth-0.1.7/revproxy_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:47:11.000000 revproxy_auth-0.1.7/revproxy_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-13 06:47:11.000000 revproxy_auth-0.1.7/revproxy_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-13 06:47:11.000000 revproxy_auth-0.1.7/revproxy_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 06:47:11.611762 revproxy_auth-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:11.611762 revproxy_auth-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:11.611762 revproxy_auth-0.1.7/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/tests/data/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/tests/test_000.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/tests/test_001.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:07:06.314477 revproxy_auth-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-17 14:06:55.000000 revproxy_auth-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-17 14:07:06.314477 revproxy_auth-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-17 14:06:55.000000 revproxy_auth-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:07:06.310477 revproxy_auth-0.1.8/revproxy_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-17 14:06:55.000000 revproxy_auth-0.1.8/revproxy_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-17 14:06:55.000000 revproxy_auth-0.1.8/revproxy_auth/config-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    20036 2023-06-17 14:06:55.000000 revproxy_auth-0.1.8/revproxy_auth/revproxy_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:07:06.310477 revproxy_auth-0.1.8/revproxy_auth/revproxy_auth_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:07:06.314477 revproxy_auth-0.1.8/revproxy_auth/revproxy_auth_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-17 14:06:55.000000 revproxy_auth-0.1.8/revproxy_auth/revproxy_auth_static/css/view.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:07:06.314477 revproxy_auth-0.1.8/revproxy_auth/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-17 14:06:55.000000 revproxy_auth-0.1.8/revproxy_auth/templates/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:07:06.314477 revproxy_auth-0.1.8/revproxy_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-17 14:07:06.000000 revproxy_auth-0.1.8/revproxy_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-17 14:07:06.000000 revproxy_auth-0.1.8/revproxy_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:07:06.000000 revproxy_auth-0.1.8/revproxy_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-17 14:07:06.000000 revproxy_auth-0.1.8/revproxy_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-17 14:07:06.000000 revproxy_auth-0.1.8/revproxy_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:07:06.314477 revproxy_auth-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-17 14:06:55.000000 revproxy_auth-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:07:06.314477 revproxy_auth-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:06:55.000000 revproxy_auth-0.1.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:07:06.314477 revproxy_auth-0.1.8/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-17 14:06:55.000000 revproxy_auth-0.1.8/tests/data/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-17 14:06:55.000000 revproxy_auth-0.1.8/tests/test_000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-06-17 14:06:55.000000 revproxy_auth-0.1.8/tests/test_001.py
```

### Comparing `revproxy_auth-0.1.7/PKG-INFO` & `revproxy_auth-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revproxy_auth
-Version: 0.1.7
+Version: 0.1.8
 Summary: Reverse proxy with synology authentication
 Home-page: https://github.com/Phornee/revproxy_auth
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # revproxy_auth
         This class implements a reverse proxy intended to work inside a Flask server, allows to use the synology auth credentials for all your services behind the synology service proxy.
```

### Comparing `revproxy_auth-0.1.7/README.md` & `revproxy_auth-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.1.7/revproxy_auth/revproxy_auth.py` & `revproxy_auth-0.1.8/revproxy_auth/revproxy_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,17 @@
         response = None
 
         if req.form.get('revproxy_auth', None):
             session_cookie, session_cookie_name = self._creates_session_token_from_popup_data(req)
             if session_cookie_name:
                 self.logger.info('Credentials validated.')
                 # To get rid of the POST form data, and reenter with the valid session token
-                response = redirect(parse.urljoin(session_cookie['host'], session_cookie['endpoint']))
+                url_redirect = parse.urljoin(session_cookie['host'], session_cookie['endpoint'])
+                self.logger.debug('Redirecting to %s', url_redirect)
+                response = redirect(url_redirect)
                 response.set_cookie('token', session_cookie_name, max_age=COOKIE_LIFE_MINUTES*60)
             else:
                 response = self._reask_credentials(req)
         else:
             # Try to get authentication from the cookie
             cookie_name = req.cookies.get('token', None)
             self.logger.debug('Incomming Session token Cookie name: %s', cookie_name)
@@ -192,61 +194,67 @@
             # replace the cookie name
             env = jinja2.Environment()
             template = env.from_string(buff)
             content = template.render(revproxy_auth=cookie_name)
             return Response(content, status=HTTP_200_OK,  content_type='text/html')
 
     def _get_local_auth_cookie(self, cookie_name:str = None):
+        self._clear_expired_cookies(self.auth_cookie_folder)
         cookie = None
         if cookie_name:
             cookie_path = os.path.join(self.auth_cookie_folder, cookie_name)
             if os.path.exists(cookie_path):
                 with open(cookie_path, 'r', encoding="utf-8") as cookie_file:
                     cookie = json.load(cookie_file)
 
                     cookie['headers'] = json.loads(cookie['headers'])
         return cookie
 
     def _get_local_session_cookie(self, cookie_name:str = None):
+        self._clear_expired_cookies(self.session_cookie_folder)
         cookie = None
         if cookie_name:
             cookie_path = os.path.join(self.session_cookie_folder, cookie_name)
             if os.path.exists(cookie_path):
                 with open(cookie_path, 'r', encoding="utf-8") as cookie_file:
                     cookie = json.load(cookie_file)
         return cookie
 
     def _credentials_valid(self, form):
         token = form.get('revproxy_auth', None)
         if token:
             user = form.get('user', '').strip(' \t\n\r')
             password = form.get('password', '').strip(' \t\n\r')
             otp = form.get('OTP', '').strip(' \t\n\r')
-            for credential in self._config['credentials']:
-                if credential['user'] == user and credential['password'] == password and credential['OTP'] == otp:
-                    self.logger.info('Validating credentials by user/password...')
-                    return True
+            fixed_credentials = self._config['credentials']
+            if fixed_credentials:
+                for credential in fixed_credentials:
+                    if credential['user'] == user and credential['password'] == password and credential['OTP'] == otp:
+                        self.logger.info('Validating credentials by user/password...')
+                        return True
             self.logger.info('Validating credentials Synology Auth...')
             url = (f'{self._config["NAS"]}/webapi/entry.cgi?api=SYNO.API.Auth&version=6&method=login'
                    f'&account={user}&passwd={password}&otp_code={otp}')
             auth_response = requests.get(url, timeout=10)
             # Verify authentication
             return auth_response.json()['success']
         return False
 
     def _call_inner_get(self, host, endpoint, params, headers) -> Response:
         fullpath = parse.urljoin(host, endpoint)
+        self.logger.debug('Calling inner GET %s', fullpath)
         resp = requests.get(fullpath,
                             params=params,
                             headers = headers,
                             timeout=10)
         return Response(resp.text, status=resp.status_code, content_type=resp.headers['content-type'])
 
     def _call_inner_post(self, host, endpoint, data, headers) -> Response:
         fullpath = parse.urljoin(host, endpoint)
+        self.logger.debug('Calling inner POST %s', fullpath)
         resp = requests.post(fullpath,
                              data = data,
                              headers = headers,
                              timeout=10)
         return Response(resp.text, status=resp.status_code, content_type=resp.headers['content-type'])
 
     def _reask_credentials(self, req: Request, old_cookie_name: str = None) -> Response:
```

### Comparing `revproxy_auth-0.1.7/revproxy_auth/revproxy_auth_static/css/view.css` & `revproxy_auth-0.1.8/revproxy_auth/revproxy_auth_static/css/view.css`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.1.7/revproxy_auth/templates/form.html` & `revproxy_auth-0.1.8/revproxy_auth/templates/form.html`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.1.7/revproxy_auth.egg-info/PKG-INFO` & `revproxy_auth-0.1.8/revproxy_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revproxy-auth
-Version: 0.1.7
+Version: 0.1.8
 Summary: Reverse proxy with synology authentication
 Home-page: https://github.com/Phornee/revproxy_auth
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # revproxy_auth
         This class implements a reverse proxy intended to work inside a Flask server, allows to use the synology auth credentials for all your services behind the synology service proxy.
```

### Comparing `revproxy_auth-0.1.7/setup.py` & `revproxy_auth-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="revproxy_auth",
-    version="0.1.7",
+    version="0.1.8",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Reverse proxy with synology authentication",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/revproxy_auth",
     packages=setuptools.find_packages(),
```

### Comparing `revproxy_auth-0.1.7/tests/test_000.py` & `revproxy_auth-0.1.8/tests/test_000.py`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.1.7/tests/test_001.py` & `revproxy_auth-0.1.8/tests/test_001.py`

 * *Files identical despite different names*

