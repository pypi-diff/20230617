# Comparing `tmp/flask_signing-0.5.0.tar.gz` & `tmp/flask_signing-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_signing-0.5.0.tar", last modified: Fri Jun 16 04:29:25 2023, max compression
+gzip compressed data, was "flask_signing-0.6.0.tar", last modified: Sat Jun 17 03:24:13 2023, max compression
```

## Comparing `flask_signing-0.5.0.tar` & `flask_signing-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-16 04:29:25.418191 flask_signing-0.5.0/
--rw-rw-r--   0 sig       (1000) sig       (1000)     1503 2023-06-11 20:13:39.000000 flask_signing-0.5.0/LICENSE
--rw-rw-r--   0 sig       (1000) sig       (1000)       43 2023-06-15 20:25:19.000000 flask_signing-0.5.0/MANIFEST.in
--rw-rw-r--   0 sig       (1000) sig       (1000)     3890 2023-06-16 04:29:25.418191 flask_signing-0.5.0/PKG-INFO
--rw-rw-r--   0 sig       (1000) sig       (1000)     3158 2023-06-16 04:19:42.000000 flask_signing-0.5.0/README.md
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-16 04:29:25.414191 flask_signing-0.5.0/docs/
--rw-rw-r--   0 sig       (1000) sig       (1000)    78889 2023-06-13 00:10:22.000000 flask_signing-0.5.0/docs/combined.png
--rw-rw-r--   0 sig       (1000) sig       (1000)    65777 2023-06-13 00:01:06.000000 flask_signing-0.5.0/docs/logo.png
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-16 04:29:25.414191 flask_signing-0.5.0/flask_signing/
--rw-rw-r--   0 sig       (1000) sig       (1000)    20631 2023-06-16 04:28:00.000000 flask_signing-0.5.0/flask_signing/__init__.py
--rw-rw-r--   0 sig       (1000) sig       (1000)      213 2023-06-16 04:19:36.000000 flask_signing-0.5.0/flask_signing/__metadata__.py
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-16 04:29:25.418191 flask_signing-0.5.0/flask_signing.egg-info/
--rw-rw-r--   0 sig       (1000) sig       (1000)     3890 2023-06-16 04:29:25.000000 flask_signing-0.5.0/flask_signing.egg-info/PKG-INFO
--rw-rw-r--   0 sig       (1000) sig       (1000)      345 2023-06-16 04:29:25.000000 flask_signing-0.5.0/flask_signing.egg-info/SOURCES.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)        1 2023-06-16 04:29:25.000000 flask_signing-0.5.0/flask_signing.egg-info/dependency_links.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       35 2023-06-16 04:29:25.000000 flask_signing-0.5.0/flask_signing.egg-info/requires.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       20 2023-06-16 04:29:25.000000 flask_signing-0.5.0/flask_signing.egg-info/top_level.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       35 2023-06-11 20:04:40.000000 flask_signing-0.5.0/requirements.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       38 2023-06-16 04:29:25.418191 flask_signing-0.5.0/setup.cfg
--rw-rw-r--   0 sig       (1000) sig       (1000)     1587 2023-06-15 20:26:56.000000 flask_signing-0.5.0/setup.py
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-16 04:29:25.418191 flask_signing-0.5.0/tests/
--rw-rw-r--   0 sig       (1000) sig       (1000)    11035 2023-06-16 04:16:19.000000 flask_signing-0.5.0/tests/__init__.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-17 03:24:13.901771 flask_signing-0.6.0/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1503 2023-06-11 20:13:39.000000 flask_signing-0.6.0/LICENSE
+-rw-rw-r--   0 sig       (1000) sig       (1000)       43 2023-06-15 20:25:19.000000 flask_signing-0.6.0/MANIFEST.in
+-rw-rw-r--   0 sig       (1000) sig       (1000)     3870 2023-06-17 03:24:13.901771 flask_signing-0.6.0/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)     3138 2023-06-17 03:12:27.000000 flask_signing-0.6.0/README.md
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-17 03:24:13.901771 flask_signing-0.6.0/docs/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    78889 2023-06-13 00:10:22.000000 flask_signing-0.6.0/docs/combined.png
+-rw-rw-r--   0 sig       (1000) sig       (1000)    65777 2023-06-13 00:01:06.000000 flask_signing-0.6.0/docs/logo.png
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-17 03:24:13.901771 flask_signing-0.6.0/flask_signing/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    20649 2023-06-17 03:12:34.000000 flask_signing-0.6.0/flask_signing/__init__.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)      213 2023-06-17 03:23:40.000000 flask_signing-0.6.0/flask_signing/__metadata__.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-17 03:24:13.901771 flask_signing-0.6.0/flask_signing.egg-info/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     3870 2023-06-17 03:24:13.000000 flask_signing-0.6.0/flask_signing.egg-info/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)      372 2023-06-17 03:24:13.000000 flask_signing-0.6.0/flask_signing.egg-info/SOURCES.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)        1 2023-06-17 03:24:13.000000 flask_signing-0.6.0/flask_signing.egg-info/dependency_links.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       35 2023-06-17 03:24:13.000000 flask_signing-0.6.0/flask_signing.egg-info/requires.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       20 2023-06-17 03:24:13.000000 flask_signing-0.6.0/flask_signing.egg-info/top_level.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       35 2023-06-11 20:04:40.000000 flask_signing-0.6.0/requirements.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       38 2023-06-17 03:24:13.901771 flask_signing-0.6.0/setup.cfg
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1587 2023-06-15 20:26:56.000000 flask_signing-0.6.0/setup.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-17 03:24:13.901771 flask_signing-0.6.0/tests/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    10843 2023-06-17 02:47:54.000000 flask_signing-0.6.0/tests/__init__.py
+-rw-rw-r--   0 sig       (1000) sig       (1000)     7995 2023-06-17 03:12:37.000000 flask_signing-0.6.0/tests/performance_tests.py
```

### Comparing `flask_signing-0.5.0/LICENSE` & `flask_signing-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_signing-0.5.0/PKG-INFO` & `flask_signing-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_signing
-Version: 0.5.0
+Version: 0.6.0
 Summary: a signing key extension for flask
 Home-page: https://github.com/signebedi/Flask-Signing
 Author: Sig Janoska-Bedi
 Author-email: signe@atreeus.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -56,30 +56,30 @@
 
 with app.app_context():
     signatures = Signatures(app, byte_len=24)
 
 
 @app.route('/sign')
 def sign():
-    key = signatures.write_key_to_database(scope='test', expiration=1, active=True, email='test@example.com')
+    key = signatures.write_key(scope='test', expiration=1, active=True, email='test@example.com')
     return f'Key generated: {key}'
 
 @app.route('/verify/<key>')
 def verify(key):
-    valid = signatures.validate_request(signature=key, scope='example')
+    valid = signatures.verify_key(signature=key, scope='example')
     return f'Key valid: {valid}'
 
 @app.route('/expire/<key>')
 def expire(key):
     expired = signatures.expire_key(key)
     return f'Key expired: {expired}'
     
 @app.route('/all')
 def all():
-    all = signatures.query_all()
+    all = signatures.get_all()
     return f'Response: {all}'
 ```
 
 In this example, a new signing key is generated and written to the database when you visit the /sign route, and the key is displayed on the page. Then, when you visit the /verify/<key> route (replace <key> with the actual key), the validity of the key is checked and displayed. You can expire a key using the /expire/<key> route, and view all records with the /all route.
 
 Please note that this is a very basic example and your actual use of the flask_signing package may be more complex depending on your needs. It's important to secure your signing keys and handle them appropriately according to your application's security requirements.
```

### Comparing `flask_signing-0.5.0/README.md` & `flask_signing-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,30 +37,30 @@
 
 with app.app_context():
     signatures = Signatures(app, byte_len=24)
 
 
 @app.route('/sign')
 def sign():
-    key = signatures.write_key_to_database(scope='test', expiration=1, active=True, email='test@example.com')
+    key = signatures.write_key(scope='test', expiration=1, active=True, email='test@example.com')
     return f'Key generated: {key}'
 
 @app.route('/verify/<key>')
 def verify(key):
-    valid = signatures.validate_request(signature=key, scope='example')
+    valid = signatures.verify_key(signature=key, scope='example')
     return f'Key valid: {valid}'
 
 @app.route('/expire/<key>')
 def expire(key):
     expired = signatures.expire_key(key)
     return f'Key expired: {expired}'
     
 @app.route('/all')
 def all():
-    all = signatures.query_all()
+    all = signatures.get_all()
     return f'Response: {all}'
 ```
 
 In this example, a new signing key is generated and written to the database when you visit the /sign route, and the key is displayed on the page. Then, when you visit the /verify/<key> route (replace <key> with the actual key), the validity of the key is checked and displayed. You can expire a key using the /expire/<key> route, and view all records with the /all route.
 
 Please note that this is a very basic example and your actual use of the flask_signing package may be more complex depending on your needs. It's important to secure your signing keys and handle them appropriately according to your application's security requirements.
```

### Comparing `flask_signing-0.5.0/docs/combined.png` & `flask_signing-0.6.0/docs/combined.png`

 * *Files identical despite different names*

### Comparing `flask_signing-0.5.0/docs/logo.png` & `flask_signing-0.6.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `flask_signing-0.5.0/flask_signing/__init__.py` & `flask_signing-0.6.0/flask_signing/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
         def __get__(self, instance, owner):
             @wraps(self.func)
             def wrapper(signature, *args, **kwargs):
 
                 # If rate limiting has not been enabled, then we always return True
                 if not instance.rate_limiting:
-                    return True
+                    return self.func(instance, signature, *args, **kwargs)
 
                 Signing = instance.get_model()
 
                 signing_key = Signing.query.filter_by(signature=signature).first()
 
                 # If the key does not exist
                 if not signing_key:
@@ -106,48 +106,14 @@
                 signing_key.last_request_time = datetime.datetime.utcnow()
 
                 instance.db.session.commit()
 
                 return self.func(instance, signature, *args, **kwargs)
             return wrapper
 
-    @request_limiter
-    def validate_request(self, signature, scope):
-        """
-        Validates a request by verifying the given signing key against a specific scope.
-        
-        This function wraps the `verify_signature` function with rate limiting support. 
-        If rate limiting is enabled, it checks whether the request count for the signature 
-        has exceeded the maximum allowed requests within the specified time period.
-        
-        If the rate limit is exceeded, it raises a `RateLimitExceeded` exception and returns False.
-        If the rate limit is not exceeded, it calls the `verify_signature` function to verify the key.
-        
-        Args:
-            signature (str): The signing key to be verified.
-            scope (str): The scope against which the signing key will be validated.
-
-        Returns:
-            bool: True if the signing key is valid and hasn't exceeded rate limit, False otherwise.
-
-        Raises:
-            RateLimitExceeded: If the number of requests with this signing key exceeds 
-            the maximum allowed within the specified time period.
-        """
-
-        try:
-            valid = self.verify_signature(signature, scope)
-        except RateLimitExceeded as e:
-            print(e)  # Or handle the exception in some other way
-            return False
-
-        return valid
-
-
-
     def generate_key(self, length:int=None) -> str:
         """
         Generates a signing key with the specified byte length. 
         Note: byte length generally translates to about 1.3 times as many chars,
         see https://docs.python.org/3/library/secrets.html.
 
         Args:
@@ -157,15 +123,15 @@
             str: The generated signing key.
         """
 
         if not length: 
             length = self.byte_len
         return secrets.token_urlsafe(length)
 
-    def write_key_to_database(self, scope:str=None, expiration:int=1, active:bool=True, email:str=None, previous_key:str=None) -> str:
+    def write_key(self, scope:str=None, expiration:int=1, active:bool=True, email:str=None, previous_key:str=None) -> str:
         """
         Writes a newly generated signing key to the database.
 
         This function will continuously attempt to generate a key until a unique one is created. 
 
         Args:
             scope (str): The scope within which the signing key will be valid. Defaults to None.
@@ -232,18 +198,52 @@
         if not signing_key:
             return False
 
         # This will disable the key
         signing_key.active = False
         self.db.session.commit()
         return True
+    
+
+    @request_limiter
+    def verify_key(self, signature, scope):
+        """
+        Validates a request by verifying the given signing key against a specific scope.
+        
+        This function wraps the `check_key` function and adds rate limiting support. 
+        If rate limiting is enabled, it checks whether the request count for the signature 
+        has exceeded the maximum allowed requests within the specified time period.
+        
+        If the rate limit is exceeded, it raises a `RateLimitExceeded` exception and returns False.
+        If the rate limit is not exceeded, or is not enabled, this calls the `check_key` function 
+        to verify the key.
+        
+        Args:
+            signature (str): The signing key to be verified.
+            scope (str): The scope against which the signing key will be validated.
+
+        Returns:
+            bool: True if the signing key is valid and hasn't exceeded rate limit, False otherwise.
+
+        Raises:
+            RateLimitExceeded: If the number of requests with this signing key exceeds 
+            the maximum allowed within the specified time period.
+        """
+
+        try:
+            valid = self.check_key(signature, scope)
+        except RateLimitExceeded as e:
+            print(e)  # Or handle the exception in some other way
+            return False
+
+        return valid
 
-    def verify_signature(self, signature, scope):
+    def check_key(self, signature, scope):
         """
-        Verifies the validity of a given signing key against a specific scope.
+        Checks the validity of a given signing key against a specific scope.
 
         This function checks if the signing key exists, if it is active, if it has not expired,
         and if its scope matches the provided scope. If all these conditions are met, the function
         returns True, otherwise, it returns False.
 
         Args:
             signature (str): The signing key to be verified.
@@ -378,15 +378,15 @@
         result = query.all()
 
         if not result:
             return False
 
         return [{'signature': key.signature, 'email': key.email, 'scope': key.scope, 'active': key.active, 'timestamp': key.timestamp, 'expiration': key.expiration, 'previous_key': key.previous_key, 'rotated': key.rotated} for key in result]
 
-    def query_all(self) -> List[Dict[str, Any]]:
+    def get_all(self) -> List[Dict[str, Any]]:
 
         """
         Query all values in the Signing table.
         If no keys are found, it returns an empty list.
 
         Returns:
             List[Dict[str, Any]]: A list of dictionaries where each dictionary contains the details of a signing key.
@@ -474,15 +474,15 @@
 
             # Disable old key
             signing_key.active = False
             signing_key.rotated = True
             self.db.session.flush()
 
             # Generate a new key with the same properties
-            new_key = self.write_key_to_database(
+            new_key = self.write_key(
                 scope=signing_key.scope, 
                 expiration=expiration, 
                 active=True, 
                 email=signing_key.email,
                 previous_key=signing_key.signature,  # Assign old key's signature to the previous_key field of new key
             )
```

### Comparing `flask_signing-0.5.0/flask_signing.egg-info/PKG-INFO` & `flask_signing-0.6.0/flask_signing.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-signing
-Version: 0.5.0
+Version: 0.6.0
 Summary: a signing key extension for flask
 Home-page: https://github.com/signebedi/Flask-Signing
 Author: Sig Janoska-Bedi
 Author-email: signe@atreeus.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -56,30 +56,30 @@
 
 with app.app_context():
     signatures = Signatures(app, byte_len=24)
 
 
 @app.route('/sign')
 def sign():
-    key = signatures.write_key_to_database(scope='test', expiration=1, active=True, email='test@example.com')
+    key = signatures.write_key(scope='test', expiration=1, active=True, email='test@example.com')
     return f'Key generated: {key}'
 
 @app.route('/verify/<key>')
 def verify(key):
-    valid = signatures.validate_request(signature=key, scope='example')
+    valid = signatures.verify_key(signature=key, scope='example')
     return f'Key valid: {valid}'
 
 @app.route('/expire/<key>')
 def expire(key):
     expired = signatures.expire_key(key)
     return f'Key expired: {expired}'
     
 @app.route('/all')
 def all():
-    all = signatures.query_all()
+    all = signatures.get_all()
     return f'Response: {all}'
 ```
 
 In this example, a new signing key is generated and written to the database when you visit the /sign route, and the key is displayed on the page. Then, when you visit the /verify/<key> route (replace <key> with the actual key), the validity of the key is checked and displayed. You can expire a key using the /expire/<key> route, and view all records with the /all route.
 
 Please note that this is a very basic example and your actual use of the flask_signing package may be more complex depending on your needs. It's important to secure your signing keys and handle them appropriately according to your application's security requirements.
```

### Comparing `flask_signing-0.5.0/setup.py` & `flask_signing-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `flask_signing-0.5.0/tests/__init__.py` & `flask_signing-0.6.0/tests/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,57 +44,57 @@
             self.assertIsInstance(key, str)
 
     # def test_write_and_expire_key(self):
     #     """
     #     Test if a key can be written to the database and then successfully expired.
     #     """
     #     with self.app.app_context():
-    #         key = self.signatures.write_key_to_database(scope='test')
+    #         key = self.signatures.write_key(scope='test')
     #     self.assertIsNotNone(Signing.query.filter_by(signature=key).first())
     #     self.signatures.expire_key(key)
     #     self.assertFalse(Signing.query.filter_by(signature=key).first().active)
 
     def test_write_and_expire_key_string_scope(self):
         with self.app.app_context():
-            key = self.signatures.write_key_to_database(scope='test')
+            key = self.signatures.write_key(scope='test')
             Signing = self.signatures.get_model()
             self.assertIsNotNone(Signing.query.filter_by(signature=key).first())
             self.signatures.expire_key(key)
             self.assertFalse(Signing.query.filter_by(signature=key).first().active)
 
     def test_write_and_expire_key_list_scope(self):
         with self.app.app_context():
-            key = self.signatures.write_key_to_database(scope=['test', 'task', 'tusk'])
+            key = self.signatures.write_key(scope=['test', 'task', 'tusk'])
             Signing = self.signatures.get_model()
             self.assertIsNotNone(Signing.query.filter_by(signature=key).first())
             self.signatures.expire_key(key)
             self.assertFalse(Signing.query.filter_by(signature=key).first().active)
 
-    def test_verify_signature(self):
+    def test_verify_key(self):
         """
         Test if a signature can be successfully verified.
         """
         with self.app.app_context():
-            key = self.signatures.write_key_to_database(scope='test')
-            self.assertTrue(self.signatures.verify_signature(signature=key, scope='test'))
+            key = self.signatures.write_key(scope='test')
+            self.assertTrue(self.signatures.verify_key(signature=key, scope='test'))
 
             # Test expired key
-            expired_key = self.signatures.write_key_to_database(scope='test', expiration=-1)
-            self.assertFalse(self.signatures.verify_signature(signature=expired_key, scope='test'))
+            expired_key = self.signatures.write_key(scope='test', expiration=-1)
+            self.assertFalse(self.signatures.verify_key(signature=expired_key, scope='test'))
 
             # Test non-existent key
-            self.assertFalse(self.signatures.verify_signature(signature='non-existent-key', scope='test'))
+            self.assertFalse(self.signatures.verify_key(signature='non-existent-key', scope='test'))
 
     def test_query_keys(self):
         """
         Test if the query_keys method returns correct records.
         """
         with self.app.app_context():
-            key1 = self.signatures.write_key_to_database(scope='test1', email='test1@example.com')
-            key2 = self.signatures.write_key_to_database(scope='test2', email='test2@example.com', active=True)
+            key1 = self.signatures.write_key(scope='test1', email='test1@example.com')
+            key2 = self.signatures.write_key(scope='test2', email='test2@example.com', active=True)
             key3 = self.signatures.rotate_key(key2)  # Generate a new key using rotate_key which assigns previous_key
 
             # Test querying by active status
             result = self.signatures.query_keys(active=True)
             self.assertTrue(all(record['active'] for record in result))
 
             # Test querying by scope
@@ -130,15 +130,15 @@
 
 
     def test_rotate_key(self):
         """
         Test if a key can be rotated and replaced with a new one.
         """
         with self.app.app_context():
-            key = self.signatures.write_key_to_database(scope='test')
+            key = self.signatures.write_key(scope='test')
             Signing = self.signatures.get_model()
             signing_key = Signing.query.filter_by(signature=key).first()
 
             # Rotate the key
             new_key = self.signatures.rotate_key(key)
 
             # Check that the new key is different
@@ -177,19 +177,19 @@
 
     def test_rotate_keys(self):
         """
         Test if multiple keys can be rotated.
         """
         with self.app.app_context():
             # Create keys that will expire soon
-            soon_expire_key1 = self.signatures.write_key_to_database(scope='test1', expiration=1)
-            soon_expire_key2 = self.signatures.write_key_to_database(scope='test2', expiration=1)
+            soon_expire_key1 = self.signatures.write_key(scope='test1', expiration=1)
+            soon_expire_key2 = self.signatures.write_key(scope='test2', expiration=1)
 
             # Create a key that won't expire soon
-            late_expire_key = self.signatures.write_key_to_database(scope='test3', expiration=2)
+            late_expire_key = self.signatures.write_key(scope='test3', expiration=2)
 
             # Rotate keys
             self.signatures.rotate_keys(time_until=1)
 
             # Check that the keys that were about to expire have been rotated
             Signing = self.signatures.get_model()
             soon_expire_signing_key1 = Signing.query.filter_by(signature=soon_expire_key1).first()
@@ -223,28 +223,28 @@
             # Enable rate limiting
             self.signatures.rate_limiting = True
             self.signatures.rate_limiting_max_requests = 2
             self.signatures.rate_limiting_period = datetime.timedelta(seconds=2)
 
             # Generate a signature
             scope = ['example']
-            signature = self.signatures.write_key_to_database(scope=scope, active=True)
+            signature = self.signatures.write_key(scope=scope, active=True)
 
             # Validate the key once, should return True
-            self.assertTrue(self.signatures.validate_request(signature, scope))
+            self.assertTrue(self.signatures.verify_key(signature, scope))
 
             # Validate the key twice, should return True
-            self.assertTrue(self.signatures.validate_request(signature, scope))
+            self.assertTrue(self.signatures.verify_key(signature, scope))
 
             # Now we expect a RateLimitExceeded exception because we are exceeding the rate limit
             with self.assertRaises(RateLimitExceeded):
-                self.assertTrue(self.signatures.validate_request(signature, scope))
+                self.assertTrue(self.signatures.verify_key(signature, scope))
 
             # Wait for the rate limit period to pass
             time.sleep(2)
 
             # Validate the key again, should return True
-            self.assertTrue(self.signatures.validate_request(signature, scope))
+            self.assertTrue(self.signatures.verify_key(signature, scope))
 
 
 if __name__ == '__main__':
     unittest.main()
```

