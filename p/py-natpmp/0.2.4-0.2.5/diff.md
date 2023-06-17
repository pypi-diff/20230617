# Comparing `tmp/py-natpmp-0.2.4.tar.gz` & `tmp/py-natpmp-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py-natpmp-0.2.4.tar", last modified: Thu Jan 21 01:06:49 2016, max compression
+gzip compressed data, was "py-natpmp-0.2.5.tar", last modified: Sat Jun 17 19:14:47 2023, max compression
```

## Comparing `py-natpmp-0.2.4.tar` & `py-natpmp-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 yliu       (501) staff       (20)        0 2016-01-21 01:06:49.000000 py-natpmp-0.2.4/
-drwxr-xr-x   0 yliu       (501) staff       (20)        0 2016-01-21 01:06:49.000000 py-natpmp-0.2.4/natpmp/
--rw-r--r--   0 yliu       (501) staff       (20)       28 2010-02-10 04:04:37.000000 py-natpmp-0.2.4/natpmp/__init__.py
--rw-r--r--   0 yliu       (501) staff       (20)    20693 2016-01-21 00:35:24.000000 py-natpmp-0.2.4/natpmp/NATPMP.py
--rw-r--r--   0 yliu       (501) staff       (20)      985 2014-04-12 16:00:12.000000 py-natpmp-0.2.4/natpmp/natpmp_client.py
--rw-r--r--   0 yliu       (501) staff       (20)      685 2016-01-21 01:06:49.000000 py-natpmp-0.2.4/PKG-INFO
-drwxr-xr-x   0 yliu       (501) staff       (20)        0 2016-01-21 01:06:49.000000 py-natpmp-0.2.4/py_natpmp.egg-info/
--rw-r--r--   0 yliu       (501) staff       (20)        1 2016-01-21 01:06:49.000000 py-natpmp-0.2.4/py_natpmp.egg-info/dependency_links.txt
--rw-r--r--   0 yliu       (501) staff       (20)       64 2016-01-21 01:06:49.000000 py-natpmp-0.2.4/py_natpmp.egg-info/entry_points.txt
--rw-r--r--   0 yliu       (501) staff       (20)      685 2016-01-21 01:06:49.000000 py-natpmp-0.2.4/py_natpmp.egg-info/PKG-INFO
--rw-r--r--   0 yliu       (501) staff       (20)      281 2016-01-21 01:06:49.000000 py-natpmp-0.2.4/py_natpmp.egg-info/SOURCES.txt
--rw-r--r--   0 yliu       (501) staff       (20)        7 2016-01-21 01:06:49.000000 py-natpmp-0.2.4/py_natpmp.egg-info/top_level.txt
--rw-r--r--   0 yliu       (501) staff       (20)        1 2010-02-11 01:10:55.000000 py-natpmp-0.2.4/py_natpmp.egg-info/zip-safe
--rw-r--r--   0 yliu       (501) staff       (20)     4496 2012-10-12 11:27:06.000000 py-natpmp-0.2.4/README
--rw-r--r--   0 yliu       (501) staff       (20)       59 2016-01-21 01:06:49.000000 py-natpmp-0.2.4/setup.cfg
--rw-r--r--   0 yliu       (501) staff       (20)     1480 2016-01-21 01:03:38.000000 py-natpmp-0.2.4/setup.py
+drwxr-xr-x   0 yliu       (501) staff       (20)        0 2023-06-17 19:14:47.454755 py-natpmp-0.2.5/
+-rw-r--r--   0 yliu       (501) staff       (20)     1431 2023-06-17 19:05:01.000000 py-natpmp-0.2.5/LICENSE
+-rw-r--r--   0 yliu       (501) staff       (20)      725 2023-06-17 19:14:47.454892 py-natpmp-0.2.5/PKG-INFO
+-rw-r--r--   0 yliu       (501) staff       (20)     4514 2023-02-10 17:13:49.000000 py-natpmp-0.2.5/README.md
+drwxr-xr-x   0 yliu       (501) staff       (20)        0 2023-06-17 19:14:47.452646 py-natpmp-0.2.5/natpmp/
+-rw-r--r--   0 yliu       (501) staff       (20)    20506 2023-02-26 02:46:58.000000 py-natpmp-0.2.5/natpmp/NATPMP.py
+-rw-r--r--   0 yliu       (501) staff       (20)       28 2010-02-10 04:04:37.000000 py-natpmp-0.2.5/natpmp/__init__.py
+-rw-r--r--   0 yliu       (501) staff       (20)     1024 2023-02-10 17:13:49.000000 py-natpmp-0.2.5/natpmp/natpmp_client.py
+drwxr-xr-x   0 yliu       (501) staff       (20)        0 2023-06-17 19:14:47.454451 py-natpmp-0.2.5/py_natpmp.egg-info/
+-rw-r--r--   0 yliu       (501) staff       (20)      725 2023-06-17 19:14:47.000000 py-natpmp-0.2.5/py_natpmp.egg-info/PKG-INFO
+-rw-r--r--   0 yliu       (501) staff       (20)      292 2023-06-17 19:14:47.000000 py-natpmp-0.2.5/py_natpmp.egg-info/SOURCES.txt
+-rw-r--r--   0 yliu       (501) staff       (20)        1 2023-06-17 19:14:47.000000 py-natpmp-0.2.5/py_natpmp.egg-info/dependency_links.txt
+-rw-r--r--   0 yliu       (501) staff       (20)       63 2023-06-17 19:14:47.000000 py-natpmp-0.2.5/py_natpmp.egg-info/entry_points.txt
+-rw-r--r--   0 yliu       (501) staff       (20)        7 2023-06-17 19:14:47.000000 py-natpmp-0.2.5/py_natpmp.egg-info/top_level.txt
+-rw-r--r--   0 yliu       (501) staff       (20)        1 2010-02-11 01:10:55.000000 py-natpmp-0.2.5/py_natpmp.egg-info/zip-safe
+-rw-r--r--   0 yliu       (501) staff       (20)       63 2023-06-17 19:14:47.455333 py-natpmp-0.2.5/setup.cfg
+-rw-r--r--   0 yliu       (501) staff       (20)     1521 2023-06-17 18:57:29.000000 py-natpmp-0.2.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `py-natpmp-0.2.4/natpmp/NATPMP.py` & `py-natpmp-0.2.5/natpmp/NATPMP.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,26 +17,18 @@
 * It does not have a proper request queuing system, meaning that
 multiple requests may be issued in parallel, against spec recommendations.
 
 For more information on NAT-PMP, see the NAT-PMP draft specification:
 
 http://files.dns-sd.org/draft-cheshire-nat-pmp.txt
 
-Requires Python 2.3 or later.
-Tested on Python 2.5, 2.6 against Apple AirPort Express.
-
-Coinbend change log:
-* Changed gateway auto-detection to use netifaces which makes
-this library more cross-platform.
-* Added an easy to use port forwarding function with the same
-interface as that seen in the UPnP module.
 """
 
-__version__ = "0.2.3"
-__license__ = """Copyright (c) 2008-2014, Yiming Liu, All rights reserved.
+__version__ = "0.2.5"
+__license__ = """Copyright (c) 2008-2023, Yiming Liu, All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice,
   this list of conditions and the following disclaimer.
 * Redistributions in binary form must reproduce the above copyright notice,
@@ -109,15 +101,15 @@
 
 class NATPMPRequest(object):
     """Represents a basic NAT-PMP request.  This currently consists of the
        1-byte fields version and opcode.
        
        Other requests are derived from NATPMPRequest.
     """
-    retry_increment = 0.250  # seconds
+    initial_timeout = 0.250  # seconds
 
     def __init__(self, version, opcode):
         self.version = version
         self.opcode = opcode
 
     def toBytes(self):
         """Converts the request object to a byte string."""
@@ -160,14 +152,17 @@
        the original request.
     """
     def __init__(self, version, opcode, result, sec_since_epoch):
         self.version = version
         self.opcode = opcode
         self.result = result
         self.sec_since_epoch = sec_since_epoch
+
+    def is_successful(self):
+        return self.result == NATPMP_RESULT_SUCCESS
         
     def __str__(self):
         return "NATPMPResponse(%d, %d, %d, $d)".format(self.version,
                                                        self.opcode,
                                                        self.result,
                                                        self.sec_since_epoch)
 
@@ -435,24 +430,28 @@
     return data, source_addr
 
 
 def send_request_with_retry(gateway_ip, request, response_data_class=None,
                             retry=9, response_size=16):
     gateway_socket = get_gateway_socket(gateway_ip)
     n = 1
+    timeout = request.initial_timeout
     data = ""
     while n <= retry and not data:
         send_request(gateway_socket, request)
         data, source_addr = read_response(gateway_socket,
-                                          n * request.retry_increment,
+                                          timeout,
                                           response_size=response_size)
         if data is None or source_addr[0] != gateway_ip or\
                 source_addr[1] != NATPMP_PORT:
             data = ""  # discard data if source mismatch, as per specification
+
         n += 1
+        timeout *= 2
+
     if n >= retry and not data:
         raise NATPMPUnsupportedError(NATPMP_GATEWAY_NO_SUPPORT,
                                      error_str(NATPMP_GATEWAY_NO_SUPPORT))
     if data and response_data_class:
         data = response_data_class(data)
     return data
```

### Comparing `py-natpmp-0.2.4/natpmp/natpmp_client.py` & `py-natpmp-0.2.5/natpmp/natpmp_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 # Yiming Liu
 # A NAT-PMP client implementation using NATPMP.py 
+from __future__ import print_function
 
 import getopt, sys
 try:
     import natpmp as NATPMP
 except ImportError:
     import NATPMP
 
@@ -27,13 +28,13 @@
         elif name == "-l":
             lifetime = int(val)
         elif name == "-g":
             gateway = val
 
     if not gateway:
         gateway = NATPMP.get_gateway_addr()
-    print NATPMP.map_port(protocol, public_port, private_port, lifetime, gateway_ip=gateway)
+    print(NATPMP.map_port(protocol, public_port, private_port, lifetime, gateway_ip=gateway))
 
 if __name__=="__main__":
     main()
```

### Comparing `py-natpmp-0.2.4/PKG-INFO` & `py-natpmp-0.2.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: py-natpmp
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python classes for interacting with NAT-PMP v0
 Home-page: https://github.com/yimingliu/py-natpmp
 Author: Yiming Liu
 Author-email: yliu@ischool.berkeley.edu
 License: BSD
-Description: Provides functions to interact with NAT-PMP gateways implementing version 0 of the NAT-PMP draft specification.
 Keywords: NAT-PMP NAT networking port port_forwarding port_mapping AirPort Apple
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Topic :: System :: Networking
+License-File: LICENSE
+
+Provides functions to interact with NAT-PMP gateways implementing version 0 of the NAT-PMP draft specification.
```

### Comparing `py-natpmp-0.2.4/py_natpmp.egg-info/PKG-INFO` & `py-natpmp-0.2.5/py_natpmp.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: py-natpmp
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python classes for interacting with NAT-PMP v0
 Home-page: https://github.com/yimingliu/py-natpmp
 Author: Yiming Liu
 Author-email: yliu@ischool.berkeley.edu
 License: BSD
-Description: Provides functions to interact with NAT-PMP gateways implementing version 0 of the NAT-PMP draft specification.
 Keywords: NAT-PMP NAT networking port port_forwarding port_mapping AirPort Apple
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Topic :: System :: Networking
+License-File: LICENSE
+
+Provides functions to interact with NAT-PMP gateways implementing version 0 of the NAT-PMP draft specification.
```

### Comparing `py-natpmp-0.2.4/README` & `py-natpmp-0.2.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,40 @@
-** Introduction
+## Introduction
 py-natpmp is a NAT-PMP (Network Address Translation Port Mapping Protocol) library and testing client in Python. The client allows you to set up dynamic port mappings on NAT-PMP compatible routers. Thus this is a means for dynamic NAT traversal with routers that talk NAT-PMP. In practical terms, this is basically limited to the newer Apple AirPort base stations and the AirPort Express, which have support for this protocol.
 
 In any case, this library puts a thin layer of Python abstraction over the NAT-PMP protocol, version 0, as specified by the NAT-PMP draft standard.
 
-** Library
+## Library
 The library provides a set of high-level and low-level functions to interact via the NAT-PMP protocol. The functions map_port and get_public_address provide the two high-level functions offered by NAT-PMP. Responses are stored as Python objects.
 
-** Client
+## Client
 To use the client, grab it and the above library. Make sure you have the library in the same directory as the client script or otherwise on your Python instance’s sys.path. Invoke the client on the command-line (Terminal.app) as python natpmp-client.py [-u] [-l lifetime] [-g gateway_addr] public_port private_port.
 
 For example:
 
-python natpmp-client.py -u -l 1800 60009 60009
-Create a mapping for the public UDP port 60009 to the private UDP port 60009 for 1,800 seconds (30 minutes)
-python natpmp-client.py 60010 60010
-Create a mapping for the public TCP port 60010 to the private TCP port 60010
-python natpmp-client.py -g 10.0.1.1 60011 60022
-Explicitly instruct the gateway router 10.0.1.1 to create the TCP mapping from 60010 to 60022
+- `python natpmp-client.py -u -l 1800 60009 60009`
+    Create a mapping for the public UDP port 60009 to the private UDP port 60009 for 1,800 seconds (30 minutes)
+- `python natpmp-client.py 60010 60010`
+    Create a mapping for the public TCP port 60010 to the private TCP port 60010
+- `python natpmp-client.py -g 10.0.1.1 60011 60022`
+    Explicitly instruct the gateway router 10.0.1.1 to create the TCP mapping from 60010 to 60022
 
 Remember to turn off your firewall for those ports that you map.
 
-** Caveats
+## Caveats
 This is an incomplete implementation of the specification.  When the router reboots, all dynamic mappings are lost.  The specification provides for notification packets to be sent by the router to each client when this happens.  There is no support in this library and client to monitor for such notifications, nor does it implement a daemon process to do so.  The specification recommends queuing requests – that is, all NAT-PMP interactions should happen serially.  This simple library does not queue requests – if you abuse it with multithreading, it will send those requests in parallel and possibly overwhelm the router.
 
 The library will attempt to auto-detect your NAT gateway. This is done via a popen to netstat on BSDs/Darwin and ip on Linux. This is likely to fail miserably, depending on how standard the output is. In the library, a keyword argument is provided to override the default and specify your own gateway address. In the client, use the -g switch to manually specify your gateway.
 
-** License & Disclaimer
-In short, this little package is licensed under the new BSD license.  I keep copyright on the code, but let you use it to do whatever you want, including putting it into your own software.  Do not hold me responsible if things blow up -- you're the one downloading random code from the Internet.
+## License & Disclaimer
+In abstract, this little package is licensed under the new BSD license.  I keep copyright on the code, but let you use it to do whatever you want, including putting it into your own software.  Do not hold me responsible if things blow up -- you're the one downloading random code from the Internet.
 
-Boilerplate legalese follows:
-Copyright: 2008+ Yiming Liu, all rights reserved.
+### In legalese
+
+Copyright: 2008-2023 Yiming Liu, all rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice,
   this list of conditions and the following disclaimer.
 * Redistributions in binary form must reproduce the above copyright notice,
```

### Comparing `py-natpmp-0.2.4/setup.py` & `py-natpmp-0.2.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from setuptools import setup, find_packages
 import sys, os
 
-version = '0.2.4'
+version = '0.2.5'
 
 setup(name='py-natpmp',
       version=version,
       description="Python classes for interacting with NAT-PMP v0",
-      long_description="""\
-Provides functions to interact with NAT-PMP gateways implementing version 0 of the NAT-PMP draft specification.""",
+      long_description="""Provides functions to interact with NAT-PMP gateways implementing version 0 of the NAT-PMP draft specification.""",
       keywords='NAT-PMP NAT networking port port_forwarding port_mapping AirPort Apple',
       author='Yiming Liu',
       author_email='yliu@ischool.berkeley.edu',
       url='https://github.com/yimingliu/py-natpmp',
       license='BSD',
       packages=find_packages(exclude=['ez_setup', 'examples', 'tests']),
       include_package_data=True,
@@ -30,14 +29,15 @@
     'Intended Audience :: Developers',
 
     # Pick your license as you wish (should match "license" above)
      'License :: OSI Approved :: BSD License',
 
     # Specify the Python versions you support here. In particular, ensure
     # that you indicate whether you support Python 2, Python 3 or both.
+    'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 2.7',
     'Topic :: System :: Networking',
     ],
       entry_points={'console_scripts': [
             'natpmp-client.py = natpmp.natpmp_client:main',
             ],}
 )
```

