# Comparing `tmp/selis-2.8.tar.gz` & `tmp/selis-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selis-2.8.tar", last modified: Fri Jun 16 09:50:46 2023, max compression
+gzip compressed data, was "selis-2.9.tar", last modified: Sat Jun 17 15:03:12 2023, max compression
```

## Comparing `selis-2.8.tar` & `selis-2.9.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-16 09:50:46.150571 selis-2.8/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-16 09:50:46.150462 selis-2.8/PKG-INFO
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-16 09:50:46.149399 selis-2.8/selis/
--rw-r--r--   0 client     (501) staff       (20)        0 2023-06-13 15:24:14.000000 selis-2.8/selis/__init__.py
--rw-r--r--   0 client     (501) staff       (20)     4582 2023-06-16 09:28:05.000000 selis-2.8/selis/client.py
--rw-r--r--   0 client     (501) staff       (20)     1712 2023-06-16 09:50:26.000000 selis-2.8/selis/selis.py
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-16 09:50:46.150269 selis-2.8/selis.egg-info/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-16 09:50:46.000000 selis-2.8/selis.egg-info/PKG-INFO
--rw-r--r--   0 client     (501) staff       (20)      233 2023-06-16 09:50:46.000000 selis-2.8/selis.egg-info/SOURCES.txt
--rw-r--r--   0 client     (501) staff       (20)        1 2023-06-16 09:50:46.000000 selis-2.8/selis.egg-info/dependency_links.txt
--rw-r--r--   0 client     (501) staff       (20)       44 2023-06-16 09:50:46.000000 selis-2.8/selis.egg-info/entry_points.txt
--rw-r--r--   0 client     (501) staff       (20)       24 2023-06-16 09:50:46.000000 selis-2.8/selis.egg-info/requires.txt
--rw-r--r--   0 client     (501) staff       (20)        6 2023-06-16 09:50:46.000000 selis-2.8/selis.egg-info/top_level.txt
--rw-r--r--   0 client     (501) staff       (20)       38 2023-06-16 09:50:46.150609 selis-2.8/setup.cfg
--rw-r--r--   0 client     (501) staff       (20)      279 2023-06-16 09:50:39.000000 selis-2.8/setup.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-17 15:03:12.265353 selis-2.9/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-17 15:03:12.265238 selis-2.9/PKG-INFO
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-17 15:03:12.264104 selis-2.9/selis/
+-rw-r--r--   0 client     (501) staff       (20)        0 2023-06-17 14:59:11.000000 selis-2.9/selis/__init__.py
+-rw-r--r--   0 client     (501) staff       (20)     4194 2023-06-17 15:02:50.000000 selis-2.9/selis/client.py
+-rw-r--r--   0 client     (501) staff       (20)      786 2023-06-17 15:02:08.000000 selis-2.9/selis/computerinfo.py
+-rw-r--r--   0 client     (501) staff       (20)     1149 2023-06-17 15:02:05.000000 selis-2.9/selis/selis.py
+-rw-r--r--   0 client     (501) staff       (20)      185 2023-06-17 15:01:59.000000 selis-2.9/selis/utils.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-17 15:03:12.265069 selis-2.9/selis.egg-info/
+-rw-r--r--   0 client     (501) staff       (20)      128 2023-06-17 15:03:12.000000 selis-2.9/selis.egg-info/PKG-INFO
+-rw-r--r--   0 client     (501) staff       (20)      270 2023-06-17 15:03:12.000000 selis-2.9/selis.egg-info/SOURCES.txt
+-rw-r--r--   0 client     (501) staff       (20)        1 2023-06-17 15:03:12.000000 selis-2.9/selis.egg-info/dependency_links.txt
+-rw-r--r--   0 client     (501) staff       (20)       44 2023-06-17 15:03:12.000000 selis-2.9/selis.egg-info/entry_points.txt
+-rw-r--r--   0 client     (501) staff       (20)       24 2023-06-17 15:03:12.000000 selis-2.9/selis.egg-info/requires.txt
+-rw-r--r--   0 client     (501) staff       (20)        6 2023-06-17 15:03:12.000000 selis-2.9/selis.egg-info/top_level.txt
+-rw-r--r--   0 client     (501) staff       (20)       38 2023-06-17 15:03:12.265392 selis-2.9/setup.cfg
+-rw-r--r--   0 client     (501) staff       (20)      279 2023-06-17 15:03:01.000000 selis-2.9/setup.py
```

### Comparing `selis-2.8/selis/selis.py` & `selis-2.9/selis/selis.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,69 +1,48 @@
-import getpass
 import sys
 
 from optparse import OptionParser
-from selis.client import Client
+from selis.client import ChatClient
 
 
 def return_arguments():
     parser = OptionParser()
     parser.add_option("-v", "--version", dest="version", action="store_true", help="Show version then exit")
-    parser.add_option("-r", "--root", dest="root", action="store_true", help="Use root to become the admin")
     parser.add_option("-p", "--port", dest="port", help="Connect to sever through this port")
     parser.add_option("-n", "--nickname", dest="nickname", help="Choose your name or a nickname")
     (options, arguments) = parser.parse_args()
-    print_version(options)
-    return_error(parser, options)
-    return options
-
 
-def print_version(options):
     if options.version:
         print("selis 2.7")
         sys.exit()
+        
+    return_error(parser, options)
+    return options
 
 
 def return_error(parser, options):
     if not options.port:
         parser.error("[-] Port not found")
 
 
-def return_admin_mode():
-    keypass = getpass.getpass("Admin's Password: ")
-    if keypass == "selis.py":
-        print("[+] You're now the admin")
-        admin_mode = True
-    else:
-        print("\033[91m[-] Password is wrong!")
-        admin_mode = False
-
-    return admin_mode
-    
-
 def main():
     options = return_arguments()
 
     ip = "0.tcp.ap.ngrok.io"
     port = int(options.port)
     nickname = options.nickname
 
     if nickname:
         pass
     else:
-        nickname = input("[+] Choose a name: ")
-
-    if options.root:
-        admin_mode = return_admin_mode()
-    else:
-        admin_mode = False
+        nickname = input("\033[0m[*] Choose a name: \n>> ")
 
 
     try:
-        client = Client(ip=ip, port=port, nickname=nickname, admin_mode=admin_mode)
+        client = ChatClient(ip=ip, port=port, nickname=nickname)
         client.start()
     except KeyboardInterrupt:
         sys.exit()
 
 
 if __name__ == "__main__":
     main()
```

