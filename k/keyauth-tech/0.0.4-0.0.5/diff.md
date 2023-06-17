# Comparing `tmp/keyauth-tech-0.0.4.tar.gz` & `tmp/keyauth-tech-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyauth-tech-0.0.4.tar", last modified: Tue May 30 15:02:13 2023, max compression
+gzip compressed data, was "keyauth-tech-0.0.5.tar", last modified: Sat Jun 17 15:22:31 2023, max compression
```

## Comparing `keyauth-tech-0.0.4.tar` & `keyauth-tech-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-05-30 15:02:13.485990 keyauth-tech-0.0.4/
--rw-r--r--   0 ecom       (502) staff       (20)      262 2023-05-30 14:59:42.000000 keyauth-tech-0.0.4/CHANGELOG.txt
--rw-r--r--   0 ecom       (502) staff       (20)     1046 2023-05-24 11:06:49.000000 keyauth-tech-0.0.4/LICENSE.txt
--rw-r--r--   0 ecom       (502) staff       (20)       25 2023-05-24 11:06:11.000000 keyauth-tech-0.0.4/MANIFEST.in
--rw-r--r--   0 ecom       (502) staff       (20)     1564 2023-05-30 15:02:13.485838 keyauth-tech-0.0.4/PKG-INFO
--rw-r--r--   0 ecom       (502) staff       (20)      559 2023-05-30 15:01:43.000000 keyauth-tech-0.0.4/README.md
-drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-05-30 15:02:13.484898 keyauth-tech-0.0.4/keyauth/
--rw-r--r--   0 ecom       (502) staff       (20)     2487 2023-05-25 15:13:23.000000 keyauth-tech-0.0.4/keyauth/__init__.py
-drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-05-30 15:02:13.485623 keyauth-tech-0.0.4/keyauth_tech.egg-info/
--rw-r--r--   0 ecom       (502) staff       (20)     1564 2023-05-30 15:02:13.000000 keyauth-tech-0.0.4/keyauth_tech.egg-info/PKG-INFO
--rw-r--r--   0 ecom       (502) staff       (20)      263 2023-05-30 15:02:13.000000 keyauth-tech-0.0.4/keyauth_tech.egg-info/SOURCES.txt
--rw-r--r--   0 ecom       (502) staff       (20)        1 2023-05-30 15:02:13.000000 keyauth-tech-0.0.4/keyauth_tech.egg-info/dependency_links.txt
--rw-r--r--   0 ecom       (502) staff       (20)       18 2023-05-30 15:02:13.000000 keyauth-tech-0.0.4/keyauth_tech.egg-info/requires.txt
--rw-r--r--   0 ecom       (502) staff       (20)        8 2023-05-30 15:02:13.000000 keyauth-tech-0.0.4/keyauth_tech.egg-info/top_level.txt
--rw-r--r--   0 ecom       (502) staff       (20)       38 2023-05-30 15:02:13.486033 keyauth-tech-0.0.4/setup.cfg
--rw-r--r--   0 ecom       (502) staff       (20)     1240 2023-05-30 15:02:03.000000 keyauth-tech-0.0.4/setup.py
--rw-r--r--   0 ecom       (502) staff       (20)      232 2023-05-26 15:27:52.000000 keyauth-tech-0.0.4/test.py
+drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-06-17 15:22:31.670267 keyauth-tech-0.0.5/
+-rw-r--r--   0 ecom       (502) staff       (20)      318 2023-06-17 15:20:56.000000 keyauth-tech-0.0.5/CHANGELOG.txt
+-rw-r--r--   0 ecom       (502) staff       (20)     1046 2023-05-24 11:06:49.000000 keyauth-tech-0.0.5/LICENSE.txt
+-rw-r--r--   0 ecom       (502) staff       (20)       25 2023-05-24 11:06:11.000000 keyauth-tech-0.0.5/MANIFEST.in
+-rw-r--r--   0 ecom       (502) staff       (20)     2074 2023-06-17 15:22:31.670139 keyauth-tech-0.0.5/PKG-INFO
+-rw-r--r--   0 ecom       (502) staff       (20)     1068 2023-06-17 15:18:08.000000 keyauth-tech-0.0.5/README.md
+drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-06-17 15:22:31.669137 keyauth-tech-0.0.5/keyauth/
+-rw-r--r--   0 ecom       (502) staff       (20)     3914 2023-06-17 15:17:41.000000 keyauth-tech-0.0.5/keyauth/__init__.py
+drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-06-17 15:22:31.669931 keyauth-tech-0.0.5/keyauth_tech.egg-info/
+-rw-r--r--   0 ecom       (502) staff       (20)     2074 2023-06-17 15:22:31.000000 keyauth-tech-0.0.5/keyauth_tech.egg-info/PKG-INFO
+-rw-r--r--   0 ecom       (502) staff       (20)      263 2023-06-17 15:22:31.000000 keyauth-tech-0.0.5/keyauth_tech.egg-info/SOURCES.txt
+-rw-r--r--   0 ecom       (502) staff       (20)        1 2023-06-17 15:22:31.000000 keyauth-tech-0.0.5/keyauth_tech.egg-info/dependency_links.txt
+-rw-r--r--   0 ecom       (502) staff       (20)       18 2023-06-17 15:22:31.000000 keyauth-tech-0.0.5/keyauth_tech.egg-info/requires.txt
+-rw-r--r--   0 ecom       (502) staff       (20)        8 2023-06-17 15:22:31.000000 keyauth-tech-0.0.5/keyauth_tech.egg-info/top_level.txt
+-rw-r--r--   0 ecom       (502) staff       (20)       38 2023-06-17 15:22:31.670326 keyauth-tech-0.0.5/setup.cfg
+-rw-r--r--   0 ecom       (502) staff       (20)     1240 2023-06-17 15:21:01.000000 keyauth-tech-0.0.5/setup.py
+-rw-r--r--   0 ecom       (502) staff       (20)      577 2023-06-17 15:14:53.000000 keyauth-tech-0.0.5/test.py
```

### Comparing `keyauth-tech-0.0.4/LICENSE.txt` & `keyauth-tech-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `keyauth-tech-0.0.4/PKG-INFO` & `keyauth-tech-0.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyauth-tech
-Version: 0.0.4
+Version: 0.0.5
 Summary: Authentication Tool for Authenticating Users, HWIDs and Licenses to keep your Code secure from malicious activities.
 Home-page: https://keyauth.tech
 Author: Collin Stokes
 Author-email: rehan009a@outlook.com
 License: MIT
 Keywords: authentication,auth,keys,hwid
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,36 +24,48 @@
 
 
 # Key Auth
 
 Authentication Tool for Authenticating Users, HWIDs and Licenses to keep your Code secure from malicious activities.
 
 
-
-
 ## Installation
 
 Install keyauth-tech with pip
 
 ```bash
-  pip install keyauth-tech
+pip install keyauth-tech
 ```
     
 ## Usage/Examples
 
 ```python
-from keyauth import KeyAuth 
+from keyauth import KeyAuth
+
+def main():
+    print("Hack the matrix!") # Replace with your Code (success)
+
+def exit_program():
+    print("Authentication failed.") # Replace with your Code (fail)
+    authenticator.exit()
 
-authenticator = KeyAuth(app_id="")  # Replace with your actual app_id
+# Creating the authenticator instance
+authenticator = KeyAuth(app_id="", max_tries=3, success=main, fail=exit_program) # Replace with your APP ID
 
-if authenticator.authenticate():
-    print("Authentication successful!")
-else:
-    print("Authentication failed.")
+# Authenticating
+authenticator.authenticate()
+
+# Install Packages if not installed 
+authenticator.install(["requests", "random"]) # Replace with your Packages
+
+# Print your HWID
+print(authenticator.get_hwid())
 
 ```
 
+## Note
 
-## Support
+To get your `APP_ID` make an Account on https://keyauth.tech/signup, you can get a Auth Key by contacting Support for completly free. 
 
-For support, email keyauthtech@gmail.com or join our Slack channel.
+## Support
 
+For support, email `keyauthtech@gmail.com` or contact `flankdev` on Discord.
```

### Comparing `keyauth-tech-0.0.4/keyauth/__init__.py` & `keyauth-tech-0.0.5/keyauth/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,52 @@
 import subprocess
 import requests
 import platform
 import os
+import sys
 from colorama import Fore, init
 
 init(autoreset=True)  # Automatically reset colorama color styles after they're printed
 
 def clear():
     os.system('cls' if os.name == 'nt' else 'clear')
 
-class KeyAuth:
+def install_package(package):
+    try:
+        subprocess.check_call(["pip", "install", package])
+    except subprocess.CalledProcessError:
+        try:
+            subprocess.check_call(["pip3", "install", package])
+        except subprocess.CalledProcessError:
+            print(f"{Fore.RED}[!] Failed to install {package} using pip or pip3.{Fore.RESET}")
+
+def import_or_install(packages):
+    for package in packages:
+        try:
+            __import__(package)
+        except ImportError:
+            print(f"{Fore.RED}[!] {package} not found! Installing...{Fore.RESET}")
+            install_package(package)
+            print(f"{Fore.GREEN}[+] {package} has been successfully installed!{Fore.RESET}")
 
-    def __init__(self, app_id, base_url="https://api.keyauth.tech/api/v1"):
+class KeyAuth:
+    def __init__(self, app_id, base_url="https://api.keyauth.tech/api/v1", max_tries=3, success=None, fail=None):
         self.app_id = app_id
         self.auth_url = f"{base_url}/auth/{app_id}"
         self.license_url = f"{base_url}/license"
-
+        self.max_tries = max_tries
+        self.success = success
+        self.fail = fail
+
+    def exit(self):
+        sys.exit()
+
+    def install(self, packages):
+        import_or_install(packages)
+        
     def get_hwid(self):
         system = platform.system()
         if system == 'Darwin':
             cmd = ['system_profiler', 'SPHardwareDataType']
             output = subprocess.check_output(cmd).decode()
             for line in output.split('\n'):
                 if 'Hardware UUID' in line:
@@ -33,30 +60,41 @@
                     uuid = line.strip()
                     break
         else:
             uuid = None
         return str(uuid)
 
     def authenticate(self):
-        data = {"hwid": self.get_hwid()}
-        response = requests.post(self.auth_url, json=data, timeout=100)
-        json_response = response.json()
-        if json_response.get('message') == 'Login Success' and json_response.get('status') == 'success':
-            print(f"{Fore.GREEN}[+] Successfully authenticated!{Fore.RESET}")
-            return True
-        else:
-            print(f"{Fore.RED}[!] HWID: {self.get_hwid()} is not authenticated!{Fore.RESET}")
-            key = input(f"{Fore.RED}License Key: {Fore.RESET}")
-            clear()
-            key_payload = {'license_key': key, 'hwid': self.get_hwid()}
-            headers = {'x-app-id': self.app_id}
-
-            key_response = requests.post(self.license_url, json=key_payload, headers=headers, timeout=100)
-            license_response = key_response.json()
-            if license_response.get('message') == 'License key is valid. HWID added.' and license_response.get('status') == 'success':
+        tries = 0
+        while tries < self.max_tries:
+            data = {"hwid": self.get_hwid()}
+            response = requests.post(self.auth_url, json=data, timeout=100)
+            json_response = response.json()
+            if json_response.get('message') == 'Login Success' and json_response.get('status') == 'success':
                 clear()
                 print(f"{Fore.GREEN}[+] Successfully authenticated!{Fore.RESET}")
+                if self.success:
+                    self.success()
                 return True
             else:
+                print(f"{Fore.RED}[!] HWID: {self.get_hwid()} is not authenticated!{Fore.RESET}")
+                key = input(f"{Fore.RED}License Key: {Fore.RESET}")
                 clear()
-                print(f"{Fore.RED}[!] Invalid License Key!{Fore.RESET}")
-                return False
+                key_payload = {'license_key': key, 'hwid': self.get_hwid()}
+                headers = {'x-app-id': self.app_id}
+
+                key_response = requests.post(self.license_url, json=key_payload, headers=headers, timeout=100)
+                license_response = key_response.json()
+                if license_response.get('message') == 'License key is valid. HWID added.' and license_response.get('status') == 'success':
+                    clear()
+                    print(f"{Fore.GREEN}[+] Successfully authenticated!{Fore.RESET}")
+                    if self.success:
+                        self.success()
+                    return True
+                else:
+                    clear()
+                    print(f"{Fore.RED}[!] Invalid License Key!{Fore.RESET}")
+                    tries += 1
+        print(f"{Fore.RED}[!] Maximum authentication attempts exceeded!{Fore.RESET}")
+        if self.fail:
+            self.fail()
+        return False
```

### Comparing `keyauth-tech-0.0.4/keyauth_tech.egg-info/PKG-INFO` & `keyauth-tech-0.0.5/keyauth_tech.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyauth-tech
-Version: 0.0.4
+Version: 0.0.5
 Summary: Authentication Tool for Authenticating Users, HWIDs and Licenses to keep your Code secure from malicious activities.
 Home-page: https://keyauth.tech
 Author: Collin Stokes
 Author-email: rehan009a@outlook.com
 License: MIT
 Keywords: authentication,auth,keys,hwid
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,36 +24,48 @@
 
 
 # Key Auth
 
 Authentication Tool for Authenticating Users, HWIDs and Licenses to keep your Code secure from malicious activities.
 
 
-
-
 ## Installation
 
 Install keyauth-tech with pip
 
 ```bash
-  pip install keyauth-tech
+pip install keyauth-tech
 ```
     
 ## Usage/Examples
 
 ```python
-from keyauth import KeyAuth 
+from keyauth import KeyAuth
+
+def main():
+    print("Hack the matrix!") # Replace with your Code (success)
+
+def exit_program():
+    print("Authentication failed.") # Replace with your Code (fail)
+    authenticator.exit()
 
-authenticator = KeyAuth(app_id="")  # Replace with your actual app_id
+# Creating the authenticator instance
+authenticator = KeyAuth(app_id="", max_tries=3, success=main, fail=exit_program) # Replace with your APP ID
 
-if authenticator.authenticate():
-    print("Authentication successful!")
-else:
-    print("Authentication failed.")
+# Authenticating
+authenticator.authenticate()
+
+# Install Packages if not installed 
+authenticator.install(["requests", "random"]) # Replace with your Packages
+
+# Print your HWID
+print(authenticator.get_hwid())
 
 ```
 
+## Note
 
-## Support
+To get your `APP_ID` make an Account on https://keyauth.tech/signup, you can get a Auth Key by contacting Support for completly free. 
 
-For support, email keyauthtech@gmail.com or join our Slack channel.
+## Support
 
+For support, email `keyauthtech@gmail.com` or contact `flankdev` on Discord.
```

### Comparing `keyauth-tech-0.0.4/setup.py` & `keyauth-tech-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Operating System :: OS Independent',
 ]
 
 setup(
     name='keyauth-tech',
-    version='0.0.4',
+    version='0.0.5',
     description='Authentication Tool for Authenticating Users, HWIDs and Licenses to keep your Code secure from malicious activities.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://keyauth.tech',
     author='Collin Stokes',
     author_email='rehan009a@outlook.com',
     license='MIT',
```

