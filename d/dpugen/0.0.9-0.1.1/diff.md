# Comparing `tmp/dpugen-0.0.9.tar.gz` & `tmp/dpugen-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpugen-0.0.9.tar", last modified: Thu Mar 16 22:08:27 2023, max compression
+gzip compressed data, was "dpugen-0.1.1.tar", last modified: Sat Jun 17 07:17:07 2023, max compression
```

## Comparing `dpugen-0.0.9.tar` & `dpugen-0.1.1.tar`

### file list

```diff
@@ -1,43 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:08:27.133363 dpugen-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-16 22:08:15.000000 dpugen-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-03-16 22:08:27.133363 dpugen-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-03-16 22:08:15.000000 dpugen-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:08:27.129363 dpugen-0.0.9/dpugen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:08:27.129363 dpugen-0.0.9/dpugen/dashgen/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/dashgen/DASH_APPLIANCE_TABLE.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/dashgen/DASH_ENI_TABLE.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/dashgen/DASH_ROUTE_RULE_TABLE.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/dashgen/DASH_ROUTE_TABLE.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/dashgen/DASH_VNET_MAPPING_TABLE.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/dashgen/DASH_VNET_TABLE.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/dashgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/dashgen/aclgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/dashgen/confbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/dashgen/confutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/dashgen/dflt_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/dashgen/prefixtags.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/dashgen/vpcmappingtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/dashgen/vpcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:08:27.129363 dpugen-0.0.9/dpugen/dpugen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-03-16 22:08:27.000000 dpugen-0.0.9/dpugen/dpugen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-16 22:08:27.000000 dpugen-0.0.9/dpugen/dpugen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 22:08:27.000000 dpugen-0.0.9/dpugen/dpugen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-16 22:08:27.000000 dpugen-0.0.9/dpugen/dpugen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-16 22:08:27.000000 dpugen-0.0.9/dpugen/dpugen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 22:08:27.133363 dpugen-0.0.9/dpugen/saigen/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/saigen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/saigen/acl_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/saigen/address_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/saigen/confbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/saigen/confutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/saigen/dflt_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/saigen/direction_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/saigen/enis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/saigen/inbound_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/saigen/outbound_ca_to_pa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/saigen/outbound_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/saigen/pa_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/saigen/vips.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-16 22:08:15.000000 dpugen-0.0.9/dpugen/saigen/vnets.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-16 22:08:15.000000 dpugen-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-16 22:08:27.133363 dpugen-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:17:07.136318 dpugen-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-17 07:16:57.000000 dpugen-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-06-17 07:17:07.136318 dpugen-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-06-17 07:16:57.000000 dpugen-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:17:07.132318 dpugen-0.1.1/dpugen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:17:07.136318 dpugen-0.1.1/dpugen/dashgen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/dashgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/dashgen/acl_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/dashgen/acl_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/dashgen/dash_appliance_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/dashgen/dash_eni_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/dashgen/dash_route_rule_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/dashgen/dash_route_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/dashgen/dash_vnet_mapping_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/dashgen/dash_vnet_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/dashgen/prefix_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/dashgen/vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/dashgen/vpcmappingtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:17:07.136318 dpugen-0.1.1/dpugen/dpugen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-06-17 07:17:07.000000 dpugen-0.1.1/dpugen/dpugen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-17 07:17:07.000000 dpugen-0.1.1/dpugen/dpugen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 07:17:07.000000 dpugen-0.1.1/dpugen/dpugen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-17 07:17:07.000000 dpugen-0.1.1/dpugen/dpugen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-17 07:17:07.000000 dpugen-0.1.1/dpugen/dpugen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:17:07.136318 dpugen-0.1.1/dpugen/saigen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/saigen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/saigen/acl_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/saigen/acl_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/saigen/address_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/saigen/direction_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/saigen/enis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/saigen/inbound_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/saigen/outbound_ca_to_pa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/saigen/outbound_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/saigen/pa_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/saigen/vips.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-17 07:16:57.000000 dpugen-0.1.1/dpugen/saigen/vnets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-17 07:16:57.000000 dpugen-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-17 07:17:07.136318 dpugen-0.1.1/setup.cfg
```

### Comparing `dpugen-0.0.9/LICENSE` & `dpugen-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dpugen-0.0.9/PKG-INFO` & `dpugen-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: dpugen
-Version: 0.0.9
+Version: 0.1.1
 Summary: Multi-vendor DPU library to generate its configuration
 Home-page: https://github.com/mgheorghe/dpugen
 Author: Mircea Dan Gheorghe
 Author-email: mircea-dan.gheorghe@keysight.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,>=2.7
+Requires-Python: <4,>=2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![PyPI version](https://badge.fury.io/py/dpugen.svg)](https://badge.fury.io/py/dpugen)
+
 <Contents>
 
 - [dpugen](#dpugen)
   - [Use Cases](#use-cases)
   - [Installation](#installation)
   - [Command-line vs. Module](#command-line-vs-module)
     - [Command-line mode](#command-line-mode)
@@ -26,25 +28,25 @@
 # dpugen
 
 `dpugen` is a Python package. Its purpose is to generate device configurations ranging from simple to complex. Its name derives from the types of devices it was designed for: DPUs (Data Processing Units), IPUs (Infrastructure Processing Units) or SmartNICs, as the case may be.
 
 ## Use Cases
 The initial version supports the [DASH](https://github.com/Azure/DASH) project. Specifically, `dpugen` generates entries used to configure a DASH-capable device for networking services. See [DASH](https://github.com/Azure/DASH) documentation for more details.
 
-The initial use-case focuses specifically on the DASH [SAI](https://github.com/opencomputeproject/SAI) or Switch-Abstraction Interface. SAI has been extended from traditional L2/L3 datacenter swtches and routers, to now support L4 stateful processing, offloaded by DPUs. 
+The initial use-case focuses specifically on the DASH [SAI](https://github.com/opencomputeproject/SAI) or Switch-Abstraction Interface. SAI has been extended from traditional L2/L3 datacenter swtches and routers, to now support L4 stateful processing, offloaded by DPUs.
 ## Installation
 The easiest way to install is via Pip:
 ```
 pip3 install dpugen
 ```
 ## Command-line vs. Module
-`dpugen` can be used either as a standalone executable or a Python module imported into another program. 
+`dpugen` can be used either as a standalone executable or a Python module imported into another program.
 ### Command-line mode
 
-In *command-line mode*, the program can generate text or files containing JSON "records." These records comprise the configuration of the device under test (DUT). The JSON would typically be stored in a file or observed/captured on "standard out," then used by some other tool such as a test runner: the file is read, then converted into comands to configure the DUT. 
+In *command-line mode*, the program can generate text or files containing JSON "records." These records comprise the configuration of the device under test (DUT). The JSON would typically be stored in a file or observed/captured on "standard out," then used by some other tool such as a test runner: the file is read, then converted into comands to configure the DUT.
 
 When loaded from a file using a package such as Python [json](https://docs.python.org/3/library/json.html), the resulting data structure is a list of dictionary items, each one comprising a configuration item. This item might be one table entry, or a list of bulk-table entries.
 
 **Command-line Usage:**
 
 Assuming you've pip-installed the module:
 ```
```

### Comparing `dpugen-0.0.9/README.md` & `dpugen-0.1.1/dpugen/dpugen.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: dpugen
+Version: 0.1.1
+Summary: Multi-vendor DPU library to generate its configuration
+Home-page: https://github.com/mgheorghe/dpugen
+Author: Mircea Dan Gheorghe
+Author-email: mircea-dan.gheorghe@keysight.com
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: <4,>=2.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI version](https://badge.fury.io/py/dpugen.svg)](https://badge.fury.io/py/dpugen)
+
 <Contents>
 
 - [dpugen](#dpugen)
   - [Use Cases](#use-cases)
   - [Installation](#installation)
   - [Command-line vs. Module](#command-line-vs-module)
     - [Command-line mode](#command-line-mode)
@@ -11,25 +28,25 @@
 # dpugen
 
 `dpugen` is a Python package. Its purpose is to generate device configurations ranging from simple to complex. Its name derives from the types of devices it was designed for: DPUs (Data Processing Units), IPUs (Infrastructure Processing Units) or SmartNICs, as the case may be.
 
 ## Use Cases
 The initial version supports the [DASH](https://github.com/Azure/DASH) project. Specifically, `dpugen` generates entries used to configure a DASH-capable device for networking services. See [DASH](https://github.com/Azure/DASH) documentation for more details.
 
-The initial use-case focuses specifically on the DASH [SAI](https://github.com/opencomputeproject/SAI) or Switch-Abstraction Interface. SAI has been extended from traditional L2/L3 datacenter swtches and routers, to now support L4 stateful processing, offloaded by DPUs. 
+The initial use-case focuses specifically on the DASH [SAI](https://github.com/opencomputeproject/SAI) or Switch-Abstraction Interface. SAI has been extended from traditional L2/L3 datacenter swtches and routers, to now support L4 stateful processing, offloaded by DPUs.
 ## Installation
 The easiest way to install is via Pip:
 ```
 pip3 install dpugen
 ```
 ## Command-line vs. Module
-`dpugen` can be used either as a standalone executable or a Python module imported into another program. 
+`dpugen` can be used either as a standalone executable or a Python module imported into another program.
 ### Command-line mode
 
-In *command-line mode*, the program can generate text or files containing JSON "records." These records comprise the configuration of the device under test (DUT). The JSON would typically be stored in a file or observed/captured on "standard out," then used by some other tool such as a test runner: the file is read, then converted into comands to configure the DUT. 
+In *command-line mode*, the program can generate text or files containing JSON "records." These records comprise the configuration of the device under test (DUT). The JSON would typically be stored in a file or observed/captured on "standard out," then used by some other tool such as a test runner: the file is read, then converted into comands to configure the DUT.
 
 When loaded from a file using a package such as Python [json](https://docs.python.org/3/library/json.html), the resulting data structure is a list of dictionary items, each one comprising a configuration item. This item might be one table entry, or a list of bulk-table entries.
 
 **Command-line Usage:**
 
 Assuming you've pip-installed the module:
 ```
@@ -76,8 +93,8 @@
 
 For example, [enis.py](dpugen/saigen/enis.py) generates ENIs (Elastic Network Interfaces), [acl_groups.py](dpugen/saigen/acl_groups.py) generates ACLs (Acess Control lists) and ACL Groups, etc. Each sub-generator can be used independently as a module or command-line executable, but the normal practice is to use the top-level generator.
 
 The generator can be fed scaling parameters to control the number of entities it generates. It also has defaults, allowing it to generate a configuration such as shown in the examples above with no parameters. Furthermore, you can specify things like starting IP address, address step, etc., but these lower-level parameters can usually be left to their defaults.
 
 The output is meant to be consumed by a test runner such as Pytest, which in turn would configure a device using its native API. The SAI records are in a generic format and need to be translated into device RPC calls. This is outside the scope of this document. One example test framework which does this is [SAI Challenger](https://github.com/opencomputeproject/SAI-Challenger) , and it is used in the [DASH](https://github.com/Azure/DASH) project.
 
-As explained above, `dpugen` can be used in command-line mode to emit JSON records, or in module mode to be imported by another program. The diagram above shows both of these modes.
+As explained above, `dpugen` can be used in command-line mode to emit JSON records, or in module mode to be imported by another program. The diagram above shows both of these modes.
```

### Comparing `dpugen-0.0.9/dpugen/dashgen/DASH_APPLIANCE_TABLE.py` & `dpugen-0.1.1/dpugen/dashgen/dash_appliance_table.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 #!/usr/bin/python3
 
-import sys
 import os
+import sys
 
-from dashgen.confbase import *
-from dashgen.confutils import *
+from dpugen.confbase import ConfBase
+from dpugen.confutils import common_main
 
 
 class Appliance(ConfBase):
 
     def __init__(self, params={}):
         super().__init__(params)
+        self.num_yields = 0
 
     def items(self):
-        self.num_yields = 0
         print('  Generating %s ...' % os.path.basename(__file__), file=sys.stderr)
         p = self.params
-        cp = self.cooked_params
-
+        '''
         for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT)):
             self.num_yields += 1
             yield {
                 'DASH_APPLIANCE_TABLE:appliance-%d' % eni: {
                     "sip": "221.0.0.1",
                     "vm_vni": f'{eni}'
                 },
                 'OP': 'SET'
             }
+        '''
+        self.num_yields += 1
+        yield {
+            'DASH_APPLIANCE_TABLE:appliance-%d' % p.ENI_START: {
+                'sip': '221.0.0.1',
+                'vm_vni': f'{p.ENI_START}'
+            },
+            'OP': 'SET'
+        }
 
 
 if __name__ == '__main__':
     conf = Appliance()
     common_main(conf)
```

### Comparing `dpugen-0.0.9/dpugen/dashgen/DASH_ENI_TABLE.py` & `dpugen-0.1.1/dpugen/saigen/acl_group.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,47 @@
 #!/usr/bin/python3
+"""SAI generator for Acl Groups"""
 
-import sys
 import os
+import sys
 
-from dashgen.confbase import *
-from dashgen.confutils import *
+from dpugen.confbase import ConfBase
+from dpugen.confutils import common_main
 
 
-class Enis(ConfBase):
+class AclGroups(ConfBase):
 
     def __init__(self, params={}):
         super().__init__(params)
+        self.num_yields = 0
 
     def items(self):
-        self.num_yields = 0
         print('  Generating %s ...' % os.path.basename(__file__), file=sys.stderr)
         p = self.params
-        cp = self.cooked_params
 
         for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):
-            local_mac = str(macaddress.MAC(int(cp.MAC_L_START)+eni_index*int(macaddress.MAC(p.ENI_MAC_STEP)))).replace('-', ':')
-            vm_underlay_dip = str(ipaddress.ip_address(p.PAL) + eni_index * int(ipaddress.ip_address(p.IP_STEP1)))
-
-            acl_nsgs_in = []
-            acl_nsgs_out = []
-
-            for nsg_index in range(1, (p.ACL_NSG_COUNT*2+1)):
-                nsg_id = eni_index * 1000 + nsg_index
+            for nsg_index in range(1, (p.ACL_NSG_COUNT+1)):
 
-                stage = (nsg_index - 1) % 3 + 1
-                if nsg_index < 4:
-                    acl_nsgs_in.append(
-                        {
-                            'acl-group-id': 'acl-group-%d' % nsg_id,
-                            'stage': stage
-                        }
-                    )
-                else:
-                    acl_nsgs_out.append(
-                        {
-                            'acl-group-id': 'acl-group-%d' % nsg_id,
-                            'stage': stage
-                        }
-                    )
-
-            self.num_yields += 1
-            yield {
-                'DASH_ENI_NSG:eni-%d' % eni: {
-                    'eni_id': 'eni-%d' % eni,
-                    'mac_address': local_mac,
-                    'underlay_ip': vm_underlay_dip,
-                    'admin_state': 'enabled',
-                    'vnet': 'vnet-%d' % eni,
-                },
-                'OP': 'SET'
-            }
+                self.num_yields += 1
+                yield {
+                    'name': f'in_acl_group_#eni{eni}nsg{nsg_index}',
+                    'op': 'create',
+                    'type': 'SAI_OBJECT_TYPE_DASH_ACL_GROUP',
+                    'attributes': [
+                        'SAI_DASH_ACL_GROUP_ATTR_IP_ADDR_FAMILY', 'SAI_IP_ADDR_FAMILY_IPV4',
+                    ]
+                }
+
+                self.num_yields += 1
+                yield {
+                    'name': f'out_acl_group_#eni{eni}nsg{nsg_index}',
+                    'op': 'create',
+                    'type': 'SAI_OBJECT_TYPE_DASH_ACL_GROUP',
+                    'attributes': [
+                        'SAI_DASH_ACL_GROUP_ATTR_IP_ADDR_FAMILY', 'SAI_IP_ADDR_FAMILY_IPV4',
+                    ]
+                }
 
 
 if __name__ == '__main__':
-    conf = Enis()
+    conf = AclGroups()
     common_main(conf)
```

### Comparing `dpugen-0.0.9/dpugen/dashgen/DASH_ROUTE_RULE_TABLE.py` & `dpugen-0.1.1/dpugen/dashgen/dash_route_rule_table.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,39 @@
 #!/usr/bin/python3
 
-import sys
-from copy import deepcopy
 import os
+import sys
 
-from dashgen.confbase import *
-from dashgen.confutils import *
+from dpugen.confbase import ConfBase
+from dpugen.confutils import common_main
 
 
 class RouteRules(ConfBase):
 
     def __init__(self, params={}):
         super().__init__(params)
+        self.num_yields = 0
 
     def items(self):
-        self.num_yields = 0
         print('  Generating %s ...' % os.path.basename(__file__), file=sys.stderr)
         p = self.params
         cp = self.cooked_params
 
-        for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT)):
+        for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):
             r_vni_id = eni + p.ENI_L2R_STEP
             vtep_remote = cp.PAR + eni_index * cp.IP_STEP1
             self.num_yields += 1
             yield {
-                "DASH_ROUTE_RULE_TABLE:eni-%d:%d:%s/32" % (eni, r_vni_id,vtep_remote ): {
-                    "action_type": "decap",
-                    "priority": "1",
-                    #"protocol": "0",
-                    "pa_validation": "true",
-                    "vnet":  "vnet-%d" % r_vni_id
+                'DASH_ROUTE_RULE_TABLE:eni-%d:%d:%s/32' % (eni, r_vni_id, vtep_remote): {
+                    'action_type': 'decap',
+                    'priority': '0',
+                    # "protocol": "0",
+                    'pa_validation': 'true',
+                    'vnet':  'vnet-%d' % r_vni_id
                 },
-                "OP": "SET"
+                'OP': 'SET'
             }
-'''
-            self.num_yields += 1
-            yield {
-                "DASH_ROUTE_RULE_TABLE:eni-%d:%d:10.0.2.0/24" % (eni, r_vpc): {
-                    "action_type": "decap",
-                    "priority": "1",
-                    "protocol": "0",
-                    "pa_validation": "false"
-                },
-                "OP": "SET"
-            }
-'''
 
-if __name__ == "__main__":
+
+if __name__ == '__main__':
     conf = RouteRules()
     common_main(conf)
```

### Comparing `dpugen-0.0.9/dpugen/dashgen/DASH_ROUTE_TABLE.py` & `dpugen-0.1.1/dpugen/saigen/outbound_routing.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,124 +1,109 @@
 #!/usr/bin/python3
+"""SAI generator for Outbound Routing"""
 
 import math
-import sys
-from copy import deepcopy
 import os
+import sys
 
-from dashgen.confbase import *
-from dashgen.confutils import *
+from dpugen.confbase import (
+    ConfBase,
+    ipa
+)
+from dpugen.confutils import common_main
 
 
-class RouteTables(ConfBase):
+class OutboundRouting(ConfBase):
 
     def __init__(self, params={}):
         super().__init__(params)
+        self.num_yields = 0
 
     def items(self):
-        self.num_yields = 0
         print('  Generating %s ...' % os.path.basename(__file__), file=sys.stderr)
         p = self.params
-        cp = self.cooked_params
-        cc=0
-        nr_of_routes_prefixes = int(math.log(p.IP_ROUTE_DIVIDER_PER_ACL_RULE, 2))
-        for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT)):
-            
-            ip_prefixes = []
-            ip_prefixes_append = ip_prefixes.append
 
-            IP_L = cp.IP_L_START + eni_index * cp.IP_STEP_ENI
+        nr_of_routes_prefixes = int(math.log(p.IP_ROUTE_DIVIDER_PER_ACL_RULE, 2))
+        for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):
+            print('     route:eni:%d' % eni, file=sys.stderr)
+            vtep_eni = str(ipa(p.PAL) + int(ipa(p.IP_STEP1)) * eni_index)
             added_route_count = 0
-            for table_index in range(1, (p.ACL_NSG_COUNT*2+1)):
+            for nsg_index in range(1, (p.ACL_NSG_COUNT*2+1)):
                 for acl_index in range(1, (p.ACL_RULES_NSG+1)):
                     ip_map_count = 0
-                    remote_ip = cp.IP_R_START + eni_index * cp.IP_STEP_ENI + (table_index - 1) * cp.IP_STEP_NSG + (acl_index - 1) * cp.IP_STEP_ACL
+                    remote_ip = str(ipa(p.IP_R_START) + eni_index * int(ipa(p.IP_STEP_ENI)) + (nsg_index - 1)
+                                    * int(ipa(p.IP_STEP_NSG)) + (acl_index - 1) * int(ipa(p.IP_STEP_ACL)))
                     no_of_route_groups = p.IP_PER_ACL_RULE * 2 // p.IP_ROUTE_DIVIDER_PER_ACL_RULE
+                    # for ip_index in range(0, no_of_route_groups + 1):
                     for ip_index in range(0, no_of_route_groups):
-                        ip_prefix = remote_ip - 1 + ip_index * p.IP_ROUTE_DIVIDER_PER_ACL_RULE * cp.IP_STEP1
+                        ip_prefix = str(ipa(remote_ip) - 1 + ip_index *
+                                        p.IP_ROUTE_DIVIDER_PER_ACL_RULE * int(ipa(p.IP_STEP1)))
                         for prefix_index in range(nr_of_routes_prefixes, 0, -1):
-                            # nr_of_ips = int(math.pow(2, prefix_index-1))
                             nr_of_ips = 1 << (prefix_index-1)
                             mask = 32 - prefix_index + 1
                             if mask == 32:
-                                ip_prefix = ip_prefix + 1
+                                ip_prefix = str(ipa(ip_prefix) + 1)
 
                             if (eni % 4) == 1:
+                                # routes that have a mac mapping
                                 self.num_yields += 1
                                 yield {
-                                    "DASH_ROUTE_TABLE:eni-%d:%s/%d" % (eni, ip_prefix, mask): {
-                                        "action_type": "vnet",
-                                        "vnet": "vnet-%d" % (eni + p.ENI_L2R_STEP)
+                                    'name': f'outbound_routing_#eni{eni}nsg{nsg_index}acl{acl_index}ip{ip_index}p{prefix_index}',
+                                    'op': 'create',
+                                    'type': 'SAI_OBJECT_TYPE_OUTBOUND_ROUTING_ENTRY',
+                                    'key': {
+                                        'switch_id': '$SWITCH_ID',
+                                        'eni_id': f'$eni_#{eni}',
+                                        'destination': f'{ip_prefix}/{mask}'
                                     },
-                                    "OP": "SET"
+                                    'attributes': [
+                                        'SAI_OUTBOUND_ROUTING_ENTRY_ATTR_ACTION', 'SAI_OUTBOUND_ROUTING_ENTRY_ACTION_ROUTE_VNET',
+                                        'SAI_OUTBOUND_ROUTING_ENTRY_ATTR_DST_VNET_ID', f'$vnet_#eni{eni}'
+                                    ]
                                 }
-
+                                added_route_count += 1
                             else:
                                 # routes that do not have a mac mapping
                                 self.num_yields += 1
                                 yield {
-                                    "DASH_ROUTE_TABLE:eni-%d:%s/%d" % (eni, ip_prefix, mask): {
-                                        "action_type": "vnet",
-                                        "vnet": "vnet-%d" % (eni + p.ENI_L2R_STEP)
+                                    'name': f'outbound_routing_#eni{eni}nsg{nsg_index}acl{acl_index}ip{ip_index}p{prefix_index}',
+                                    'op': 'create',
+                                    'type': 'SAI_OBJECT_TYPE_OUTBOUND_ROUTING_ENTRY',
+                                    'key': {
+                                        'switch_id': '$SWITCH_ID',
+                                        'eni_id': f'$eni_#{eni}',
+                                        'destination': f'{ip_prefix}/{mask}'
                                     },
-                                    "OP": "SET"
+                                    'attributes': [
+                                        'SAI_OUTBOUND_ROUTING_ENTRY_ATTR_ACTION', 'SAI_OUTBOUND_ROUTING_ENTRY_ACTION_ROUTE_VNET_DIRECT',
+                                        'SAI_OUTBOUND_ROUTING_ENTRY_ATTR_DST_VNET_ID', f'$vnet_#eni{eni}',
+                                        'SAI_OUTBOUND_ROUTING_ENTRY_ATTR_OVERLAY_IP', vtep_eni
+                                    ]
                                 }
-
-                            added_route_count += 1
-                            ip_prefix = ip_prefix + cp.IP_STEP1 * nr_of_ips
+                                added_route_count += 1
+                            ip_prefix = str(ipa(ip_prefix) + int(ipa(p.IP_STEP1)) * nr_of_ips)
                             ip_map_count += int(math.pow(2, (32 - mask)))
+                    # TODO: transition between mapped and routed ips
 
-
-
-
-                    # TODO1: transition between mapped and routed ips  
-
-            #TODO: write condition check here to add a default route if no route was added so curent ENI'
+            # TODO: write condition check here to add a default route if no route was added so curent ENI'
             if added_route_count == 0:
-                remote_ip_prefix = cp.IP_R_START + eni_index * cp.IP_STEP_ENI
-                self.numYields += 1
+                remote_ip_prefix = str(ipa(p.IP_R_START) + eni_index * int(ipa(p.IP_STEP_ENI)))
+                self.num_yields += 1
                 yield {
-                    "DASH_ROUTE_TABLE:eni-%d:%s/%d" % (eni, remote_ip_prefix, 10): {
-                        "action_type": "vnet",
-                        "vnet": "vnet-%d" % (eni + p.ENI_L2R_STEP)
+                    'name': f'outbound_routing_#eni{eni}',
+                    'op': 'create',
+                    'type': 'SAI_OBJECT_TYPE_OUTBOUND_ROUTING_ENTRY',
+                    'key': {
+                        'switch_id': '$SWITCH_ID',
+                        'eni_id': f'$eni_#{eni}',
+                        'destination': f'{remote_ip_prefix}/10'
                     },
-                    "OP": "SET"
+                    'attributes': [
+                        'SAI_OUTBOUND_ROUTING_ENTRY_ATTR_ACTION', 'SAI_OUTBOUND_ROUTING_ENTRY_ACTION_ROUTE_VNET',
+                        'SAI_OUTBOUND_ROUTING_ENTRY_ATTR_DST_VNET_ID', f'$vnet_#eni{eni}'
+                    ]
                 }
-            # route_layers = deepcopy(
-            #     {
-            #         "Name": "LAYER_%d_ROUTE" % eni, "Type": 1,
-            #         "Groups": [
-            #             {
-            #                 "Name": "GROUP_%d_OUT_ROUTE" % eni,
-            #                 "Type": 0, "Direction": 0,
-            #                 "Rules": {
-            #                     "subnet_routes": routes
-            #                 }
-            #             },
-            #             {
-            #                 "Name": "GROUP_%d_IN_ROUTE" % eni,
-            #                 "Type": 0,
-            #                 "Direction": 1,
-            #                 "Rules": [
-            #                     {
-            #                         "Name": "RULE_900%d_IN_ROUTE" % eni,
-            #                         "Priority": 1,
-            #                         "Action": 2,
-            #                         "Conditions": [
-            #                             {
-            #                                 "VNIKeyList": [eni, (eni + ENI_L2R_STEP)]
-            #                             }
-            #                         ]
-            #                     }
-            #                 ]
-            #             }
-            #         ]
-            #     }
-            # )
-        
-        
-                            
-        
 
-if __name__ == "__main__":
-    conf = RouteTables()
+
+if __name__ == '__main__':
+    conf = OutboundRouting()
     common_main(conf)
```

### Comparing `dpugen-0.0.9/dpugen/dpugen.egg-info/PKG-INFO` & `dpugen-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,8 @@
-Metadata-Version: 2.1
-Name: dpugen
-Version: 0.0.9
-Summary: Multi-vendor DPU library to generate its configuration
-Home-page: https://github.com/mgheorghe/dpugen
-Author: Mircea Dan Gheorghe
-Author-email: mircea-dan.gheorghe@keysight.com
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,>=2.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
+[![PyPI version](https://badge.fury.io/py/dpugen.svg)](https://badge.fury.io/py/dpugen)
 
 <Contents>
 
 - [dpugen](#dpugen)
   - [Use Cases](#use-cases)
   - [Installation](#installation)
   - [Command-line vs. Module](#command-line-vs-module)
@@ -26,25 +13,25 @@
 # dpugen
 
 `dpugen` is a Python package. Its purpose is to generate device configurations ranging from simple to complex. Its name derives from the types of devices it was designed for: DPUs (Data Processing Units), IPUs (Infrastructure Processing Units) or SmartNICs, as the case may be.
 
 ## Use Cases
 The initial version supports the [DASH](https://github.com/Azure/DASH) project. Specifically, `dpugen` generates entries used to configure a DASH-capable device for networking services. See [DASH](https://github.com/Azure/DASH) documentation for more details.
 
-The initial use-case focuses specifically on the DASH [SAI](https://github.com/opencomputeproject/SAI) or Switch-Abstraction Interface. SAI has been extended from traditional L2/L3 datacenter swtches and routers, to now support L4 stateful processing, offloaded by DPUs. 
+The initial use-case focuses specifically on the DASH [SAI](https://github.com/opencomputeproject/SAI) or Switch-Abstraction Interface. SAI has been extended from traditional L2/L3 datacenter swtches and routers, to now support L4 stateful processing, offloaded by DPUs.
 ## Installation
 The easiest way to install is via Pip:
 ```
 pip3 install dpugen
 ```
 ## Command-line vs. Module
-`dpugen` can be used either as a standalone executable or a Python module imported into another program. 
+`dpugen` can be used either as a standalone executable or a Python module imported into another program.
 ### Command-line mode
 
-In *command-line mode*, the program can generate text or files containing JSON "records." These records comprise the configuration of the device under test (DUT). The JSON would typically be stored in a file or observed/captured on "standard out," then used by some other tool such as a test runner: the file is read, then converted into comands to configure the DUT. 
+In *command-line mode*, the program can generate text or files containing JSON "records." These records comprise the configuration of the device under test (DUT). The JSON would typically be stored in a file or observed/captured on "standard out," then used by some other tool such as a test runner: the file is read, then converted into comands to configure the DUT.
 
 When loaded from a file using a package such as Python [json](https://docs.python.org/3/library/json.html), the resulting data structure is a list of dictionary items, each one comprising a configuration item. This item might be one table entry, or a list of bulk-table entries.
 
 **Command-line Usage:**
 
 Assuming you've pip-installed the module:
 ```
```

### Comparing `dpugen-0.0.9/dpugen/dpugen.egg-info/SOURCES.txt` & `dpugen-0.1.1/dpugen/dpugen.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
-dpugen/dashgen/DASH_APPLIANCE_TABLE.py
-dpugen/dashgen/DASH_ENI_TABLE.py
-dpugen/dashgen/DASH_ROUTE_RULE_TABLE.py
-dpugen/dashgen/DASH_ROUTE_TABLE.py
-dpugen/dashgen/DASH_VNET_MAPPING_TABLE.py
-dpugen/dashgen/DASH_VNET_TABLE.py
 dpugen/dashgen/__init__.py
-dpugen/dashgen/aclgroups.py
-dpugen/dashgen/confbase.py
-dpugen/dashgen/confutils.py
-dpugen/dashgen/dflt_params.py
-dpugen/dashgen/prefixtags.py
+dpugen/dashgen/acl_group.py
+dpugen/dashgen/acl_rule.py
+dpugen/dashgen/dash_appliance_table.py
+dpugen/dashgen/dash_eni_table.py
+dpugen/dashgen/dash_route_rule_table.py
+dpugen/dashgen/dash_route_table.py
+dpugen/dashgen/dash_vnet_mapping_table.py
+dpugen/dashgen/dash_vnet_table.py
+dpugen/dashgen/prefix_tag.py
+dpugen/dashgen/vpc.py
 dpugen/dashgen/vpcmappingtypes.py
-dpugen/dashgen/vpcs.py
 dpugen/dpugen.egg-info/PKG-INFO
 dpugen/dpugen.egg-info/SOURCES.txt
 dpugen/dpugen.egg-info/dependency_links.txt
 dpugen/dpugen.egg-info/requires.txt
 dpugen/dpugen.egg-info/top_level.txt
 dpugen/saigen/__init__.py
-dpugen/saigen/acl_groups.py
+dpugen/saigen/acl_group.py
+dpugen/saigen/acl_rule.py
 dpugen/saigen/address_maps.py
-dpugen/saigen/confbase.py
-dpugen/saigen/confutils.py
-dpugen/saigen/dflt_params.py
 dpugen/saigen/direction_lookup.py
 dpugen/saigen/enis.py
 dpugen/saigen/inbound_routing.py
 dpugen/saigen/outbound_ca_to_pa.py
 dpugen/saigen/outbound_routing.py
 dpugen/saigen/pa_validation.py
 dpugen/saigen/vips.py
```

### Comparing `dpugen-0.0.9/dpugen/saigen/address_maps.py` & `dpugen-0.1.1/dpugen/saigen/address_maps.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 #!/usr/bin/python3
+"""SAI generator for Address Maps"""
 
 import os
 import sys
 
-from saigen.confbase import *
-from saigen.confutils import *
+from dpugen.confbase import (
+    ConfBase,
+    maca
+)
+from dpugen.confutils import common_main
 
 
 class Mappings(ConfBase):
 
     def __init__(self, params={}):
         super().__init__(params)
+        self.num_yields = 0
 
     def items(self):
-        self.num_yields = 0
         print('  Generating %s ...' % os.path.basename(__file__), file=sys.stderr)
         p = self.params
 
         for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):
 
             eni_mac = str(
-                macaddress.MAC(
-                    int(macaddress.MAC(p.MAC_L_START)) + eni_index * int(macaddress.MAC(p.ENI_MAC_STEP))
+                maca(
+                    int(maca(p.MAC_L_START)) + eni_index * int(maca(p.ENI_MAC_STEP))
                 )
             ).replace('-', ':')
 
             self.num_yields += 1
             yield {
-                'name': 'eni_ether_address_map_#eni%d' % eni,
+                'name': f'eni_ether_address_map_#eni{eni}',
                 'op': 'create',
                 'type': 'SAI_OBJECT_TYPE_ENI_ETHER_ADDRESS_MAP_ENTRY',
                 'key': {
                     'switch_id': '$SWITCH_ID',
                     'address': eni_mac
                 },
                 'attributes': [
-                    'SAI_ENI_ETHER_ADDRESS_MAP_ENTRY_ATTR_ENI_ID', '$eni_#%d' % eni,
+                    'SAI_ENI_ETHER_ADDRESS_MAP_ENTRY_ATTR_ENI_ID', f'$eni_#{eni}',
                 ]
             }
 
 
 if __name__ == '__main__':
     conf = Mappings()
     common_main(conf)
```

### Comparing `dpugen-0.0.9/dpugen/saigen/direction_lookup.py` & `dpugen-0.1.1/dpugen/saigen/direction_lookup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 #!/usr/bin/python3
+"""SAI generator for Direction Lookup"""
 
 import os
 import sys
 
-from saigen.confbase import *
-from saigen.confutils import *
+from dpugen.confbase import ConfBase
+from dpugen.confutils import common_main
 
 
 class DirectionLookup(ConfBase):
 
     def __init__(self, params={}):
         super().__init__(params)
+        self.num_yields = 0
 
     def items(self):
         print('  Generating %s ...' % os.path.basename(__file__), file=sys.stderr)
-        self.num_yields = 0
         p = self.params
 
         for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):
 
             self.num_yields += 1
             yield {
-                'name': 'direction_lookup_entry_#eni%d' % eni,
+                'name': f'direction_lookup_entry_#eni{eni}',
                 'op': 'create',
                 'type': 'SAI_OBJECT_TYPE_DIRECTION_LOOKUP_ENTRY',
                 'key': {
                     'switch_id': '$SWITCH_ID',
-                    'vni': '%d' % eni,
+                    'vni': f'{eni}',
                 },
                 'attributes': [
                     'SAI_DIRECTION_LOOKUP_ENTRY_ATTR_ACTION', 'SAI_DIRECTION_LOOKUP_ENTRY_ACTION_SET_OUTBOUND_DIRECTION'
                 ]
             }
```

### Comparing `dpugen-0.0.9/dpugen/saigen/enis.py` & `dpugen-0.1.1/dpugen/saigen/enis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 #!/usr/bin/python3
+"""SAI generator for ENI"""
 
 import os
 import sys
 
-from saigen.confbase import *
-from saigen.confutils import *
+from dpugen.confbase import (
+    ConfBase,
+    ipa
+)
+from dpugen.confutils import common_main
 
 
 class Enis(ConfBase):
 
     def __init__(self, params={}):
         super().__init__(params)
+        self.num_yields = 0
 
     def items(self):
-        self.num_yields = 0
         print('  Generating %s ...' % os.path.basename(__file__), file=sys.stderr)
         p = self.params
 
         for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):
-            vm_underlay_dip = str(ipaddress.ip_address(p.PAL) + eni_index * int(ipaddress.ip_address(p.IP_STEP1)))
+            vm_underlay_dip = str(ipa(p.PAL) + eni_index * int(ipa(p.IP_STEP1)))
 
-            
             eni_data = {
-                'name': 'eni_#%d' % eni,
+                'name': f'eni_#{eni}',
                 'op': 'create',
                 'type': 'SAI_OBJECT_TYPE_ENI',
                 'attributes': [
                     'SAI_ENI_ATTR_CPS', '10000',
                     'SAI_ENI_ATTR_PPS', '100000',
                     'SAI_ENI_ATTR_FLOWS', '100000',
                     'SAI_ENI_ATTR_ADMIN_STATE', 'True',
                     'SAI_ENI_ATTR_VM_UNDERLAY_DIP', vm_underlay_dip,
-                    'SAI_ENI_ATTR_VM_VNI', '%d' % eni,
-                    'SAI_ENI_ATTR_VNET_ID', '$vnet_#eni%d' % eni,
+                    'SAI_ENI_ATTR_VM_VNI', f'{eni}',
+                    'SAI_ENI_ATTR_VNET_ID', f'$vnet_#eni{eni}',
                     'SAI_ENI_ATTR_INBOUND_V4_STAGE1_DASH_ACL_GROUP_ID', '0',
                     'SAI_ENI_ATTR_INBOUND_V4_STAGE2_DASH_ACL_GROUP_ID', '0',
                     'SAI_ENI_ATTR_INBOUND_V4_STAGE3_DASH_ACL_GROUP_ID', '0',
                     'SAI_ENI_ATTR_INBOUND_V4_STAGE4_DASH_ACL_GROUP_ID', '0',
                     'SAI_ENI_ATTR_INBOUND_V4_STAGE5_DASH_ACL_GROUP_ID', '0',
                     'SAI_ENI_ATTR_INBOUND_V6_STAGE1_DASH_ACL_GROUP_ID', '0',
                     'SAI_ENI_ATTR_INBOUND_V6_STAGE2_DASH_ACL_GROUP_ID', '0',
@@ -52,18 +55,20 @@
                     'SAI_ENI_ATTR_OUTBOUND_V6_STAGE2_DASH_ACL_GROUP_ID', '0',
                     'SAI_ENI_ATTR_OUTBOUND_V6_STAGE3_DASH_ACL_GROUP_ID', '0',
                     'SAI_ENI_ATTR_OUTBOUND_V6_STAGE4_DASH_ACL_GROUP_ID', '0',
                     'SAI_ENI_ATTR_OUTBOUND_V6_STAGE5_DASH_ACL_GROUP_ID', '0',
                 ]
             }
             for nsg_index in range(1, (p.ACL_NSG_COUNT + 1)):
-                stage_index = eni_data['attributes'].index('SAI_ENI_ATTR_INBOUND_V4_STAGE%d_DASH_ACL_GROUP_ID' % nsg_index)
-                eni_data['attributes'][stage_index + 1] = '$in_acl_group_#eni%dnsg%d' % (eni, nsg_index)
-                stage_index = eni_data['attributes'].index('SAI_ENI_ATTR_OUTBOUND_V4_STAGE%d_DASH_ACL_GROUP_ID' % nsg_index)
-                eni_data['attributes'][stage_index + 1] = '$out_acl_group_#eni%dnsg%d' % (eni, nsg_index)
+                stage_index = eni_data['attributes'].index(
+                    f'SAI_ENI_ATTR_INBOUND_V4_STAGE{nsg_index}_DASH_ACL_GROUP_ID')
+                eni_data['attributes'][stage_index + 1] = f'$in_acl_group_#eni{eni}nsg{nsg_index}'
+                stage_index = eni_data['attributes'].index(
+                    f'SAI_ENI_ATTR_OUTBOUND_V4_STAGE{nsg_index}_DASH_ACL_GROUP_ID')
+                eni_data['attributes'][stage_index + 1] = f'$out_acl_group_#eni{eni}nsg{nsg_index}'
 
             self.num_yields += 1
             yield eni_data
 
 
 if __name__ == '__main__':
     conf = Enis()
```

### Comparing `dpugen-0.0.9/dpugen/saigen/inbound_routing.py` & `dpugen-0.1.1/dpugen/saigen/inbound_routing.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 #!/usr/bin/python3
+"""SAI generator for Inbound Routing"""
 
 import os
 import sys
 
-from saigen.confbase import *
-from saigen.confutils import *
+from dpugen.confbase import (
+    ConfBase,
+    ipa
+)
+from dpugen.confutils import common_main
 
-ipa = ipaddress.ip_address  # optimization so the . does not get executed multiple times
 
 class InboundRouting(ConfBase):
 
     def __init__(self, params={}):
         super().__init__(params)
+        self.num_yields = 0
 
     def items(self):
         print('  Generating %s ...' % os.path.basename(__file__), file=sys.stderr)
-        self.num_yields = 0
         p = self.params
-        cp = self.params
 
         for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):
             remote_ip = str(ipa(p.IP_R_START) + eni_index * int(ipa(p.IP_STEP_ENI)))
 
             self.num_yields += 1
             yield {
-                'name': 'inbound_routing_#eni%d' % eni,
+                'name': f'inbound_routing_#eni{eni}',
                 'op': 'create',
                 'type': 'SAI_OBJECT_TYPE_INBOUND_ROUTING_ENTRY',
                 'key': {
                     'switch_id': '$SWITCH_ID',
-                    'eni_id': '$eni_#%d' % eni,
+                    'eni_id': f'$eni_#{eni}',
                     'vni': '%d' % (eni + p.ENI_L2R_STEP),
-                    'sip': '%s' % remote_ip,
+                    'sip': f'{remote_ip}',
                     'sip_mask': '255.192.0.0',
                     'priority': 0
                 },
                 'attributes': [
                     'SAI_INBOUND_ROUTING_ENTRY_ATTR_ACTION',       'SAI_INBOUND_ROUTING_ENTRY_ACTION_VXLAN_DECAP_PA_VALIDATE',
-                    'SAI_INBOUND_ROUTING_ENTRY_ATTR_SRC_VNET_ID',  '$vnet_#eni%d' % eni
+                    'SAI_INBOUND_ROUTING_ENTRY_ATTR_SRC_VNET_ID',  f'$vnet_#eni{eni}'
                 ]
             }
 
 
 if __name__ == '__main__':
     conf = InboundRouting()
     common_main(conf)
```

### Comparing `dpugen-0.0.9/dpugen/saigen/outbound_ca_to_pa.py` & `dpugen-0.1.1/dpugen/saigen/outbound_ca_to_pa.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 #!/usr/bin/python3
+"""SAI generator for Outbound CA PA"""
 
 import os
 import sys
 
-from saigen.confbase import *
-from saigen.confutils import *
-
-ipa = ipaddress.ip_address  # optimization so the . does not get executed multiple times
-maca = macaddress.MAC       # optimization so the . does not get executed multiple times
+from dpugen.confbase import (
+    ConfBase,
+    ipa,
+    maca
+)
+from dpugen.confutils import common_main
 
 
 class OutboundCaToPa(ConfBase):
 
     def __init__(self, params={}):
         super().__init__(params)
+        self.num_yields = 0
 
     def items(self):
         print('  Generating %s ...' % os.path.basename(__file__), file=sys.stderr)
-        self.num_yields = 0
         p = self.params
 
         for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):
 
             vtep_eni = str(ipa(p.PAL) + int(ipa(p.IP_STEP1)) * eni_index)
             vtep_remote = str(ipa(p.PAR) + int(ipa(p.IP_STEP1)) * eni_index)
 
             # 1 in 4 enis will have all its ips mapped
             if (eni % 4) == 1:
-                print('    mapped:eni:%d' % eni, file=sys.stderr)
+                print(f'    mapped:eni:{eni}', file=sys.stderr)
                 for nsg_index in range(1, (p.ACL_NSG_COUNT*2+1)):
                     for acl_index in range(1, (p.ACL_RULES_NSG//2+1)):
-                        remote_ip_a = ipa(p.IP_R_START) + eni_index * int(ipa(p.IP_STEP_ENI)) + (nsg_index - 1) * int(ipa(p.IP_STEP_NSG)) + (acl_index - 1) * int(ipa(p.IP_STEP_ACL))
+                        remote_ip_a = ipa(p.IP_R_START) + eni_index * int(ipa(p.IP_STEP_ENI)) + \
+                            (nsg_index - 1) * int(ipa(p.IP_STEP_NSG)) + (acl_index - 1) * int(ipa(p.IP_STEP_ACL))
                         remote_mac_a = str(
                             maca(
                                 int(maca(p.MAC_R_START)) +
                                 eni_index * int(maca(p.ENI_MAC_STEP)) +
                                 (nsg_index - 1) * int(maca(p.ACL_NSG_MAC_STEP)) +
                                 (acl_index - 1) * int(maca(p.ACL_POLICY_MAC_STEP))
                             )
@@ -47,20 +50,20 @@
                                 maca(
                                     int(maca(remote_mac_a)) + i * 2
                                 )
                             ).replace('-', ':')
 
                             self.num_yields += 1
                             yield {
-                                'name': 'outbound_ca_to_pa_#eni%dnsg%dacl%di%dA' % (eni, nsg_index, acl_index, i),
+                                'name': f'outbound_ca_to_pa_#eni{eni}nsg{nsg_index}acl{acl_index}i{i}A',
                                 'op': 'create',
                                 'type': 'SAI_OBJECT_TYPE_OUTBOUND_CA_TO_PA_ENTRY',
                                 'key': {
                                     'switch_id': '$SWITCH_ID',
-                                    'dst_vnet_id': '$vnet_#eni%d' % eni,
+                                    'dst_vnet_id': f'$vnet_#eni{eni}',
                                     'dip': remote_expanded_ip
                                 },
                                 'attributes': [
                                     'SAI_OUTBOUND_CA_TO_PA_ENTRY_ATTR_UNDERLAY_DIP', vtep_remote,
                                     'SAI_OUTBOUND_CA_TO_PA_ENTRY_ATTR_OVERLAY_DMAC', remote_expanded_mac,
                                     'SAI_OUTBOUND_CA_TO_PA_ENTRY_ATTR_USE_DST_VNET_VNI', 'True'
                                 ]
@@ -75,48 +78,48 @@
                                 maca(
                                     int(maca(remote_mac_a)) + i * 2 - 1
                                 )
                             ).replace('-', ':')
 
                             self.num_yields += 1
                             yield {
-                                'name': 'outbound_ca_to_pa_#eni%dnsg%dacl%di%dD' % (eni, nsg_index, acl_index, i),
+                                'name': f'outbound_ca_to_pa_#eni{eni}nsg{nsg_index}acl{acl_index}i{i}D',
                                 'op': 'create',
                                 'type': 'SAI_OBJECT_TYPE_OUTBOUND_CA_TO_PA_ENTRY',
                                 'key': {
                                     'switch_id': '$SWITCH_ID',
-                                    'dst_vnet_id': '$vnet_#eni%d' % eni,
+                                    'dst_vnet_id': f'$vnet_#eni{eni}',
                                     'dip': remote_expanded_ip
                                 },
                                 'attributes': [
                                     'SAI_OUTBOUND_CA_TO_PA_ENTRY_ATTR_UNDERLAY_DIP', vtep_remote,
                                     'SAI_OUTBOUND_CA_TO_PA_ENTRY_ATTR_OVERLAY_DMAC', remote_expanded_mac,
                                     'SAI_OUTBOUND_CA_TO_PA_ENTRY_ATTR_USE_DST_VNET_VNI', 'True'
                                 ]
                             }
 
             # 3 in 4 enis will have just mapping for gateway ip, for ip that are only routed and not mapped
             else:
-                print('    routed:eni:%d' % eni, file=sys.stderr)
+                print(f'    routed:eni:{eni}', file=sys.stderr)
 
                 remote_expanded_mac = str(
                     maca(
                         int(maca(p.MAC_R_START)) +
                         eni_index * int(maca(p.ENI_MAC_STEP))
                     )
                 ).replace('-', ':')
-                
+
                 self.num_yields += 1
                 yield {
-                    'name': 'outbound_ca_to_pa_#eni%d' % (eni),
+                    'name': f'outbound_ca_to_pa_#eni{eni}',
                     'op': 'create',
                     'type': 'SAI_OBJECT_TYPE_OUTBOUND_CA_TO_PA_ENTRY',
                     'key': {
                         'switch_id': '$SWITCH_ID',
-                        'dst_vnet_id': '$vnet_#eni%d' % eni,
+                        'dst_vnet_id': f'$vnet_#eni{eni}',
                         'dip': vtep_eni
                     },
                     'attributes': [
                         'SAI_OUTBOUND_CA_TO_PA_ENTRY_ATTR_UNDERLAY_DIP', vtep_remote,
                         'SAI_OUTBOUND_CA_TO_PA_ENTRY_ATTR_OVERLAY_DMAC', remote_expanded_mac,
                         'SAI_OUTBOUND_CA_TO_PA_ENTRY_ATTR_USE_DST_VNET_VNI', 'True'
                     ]
```

### Comparing `dpugen-0.0.9/dpugen/saigen/pa_validation.py` & `dpugen-0.1.1/dpugen/saigen/pa_validation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 #!/usr/bin/python3
+"""SAI generator for PA Validation"""
 
 import os
 import sys
 
-from saigen.confbase import *
-from saigen.confutils import *
+from dpugen.confbase import (
+    ConfBase,
+    ipa
+)
+from dpugen.confutils import common_main
 
-ipa = ipaddress.ip_address  # optimization so the . does not get executed multiple times
 
 class PaValidation(ConfBase):
 
     def __init__(self, params={}):
         super().__init__(params)
+        self.num_yields = 0
 
     def items(self):
         print('  Generating %s ...' % os.path.basename(__file__), file=sys.stderr)
-        self.num_yields = 0
         p = self.params
 
         for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):
             vtep_remote = str(ipa(p.PAR) + int(ipa(p.IP_STEP1)) * eni_index)
 
             self.num_yields += 1
             yield {
-                'name': 'pa_validation_#eni%d' % eni,
+                'name': f'pa_validation_#eni{eni}',
                 'op': 'create',
-                'type' : 'SAI_OBJECT_TYPE_PA_VALIDATION_ENTRY',
-                'key' : {
+                'type': 'SAI_OBJECT_TYPE_PA_VALIDATION_ENTRY',
+                'key': {
                     'switch_id': '$SWITCH_ID',
                     'sip': vtep_remote,
-                    'vnet_id': '$vnet_#eni%d' % eni
+                    'vnet_id': f'$vnet_#eni{eni}'
                 },
-                'attributes' : [
+                'attributes': [
                     'SAI_PA_VALIDATION_ENTRY_ATTR_ACTION', 'SAI_PA_VALIDATION_ENTRY_ACTION_PERMIT'
                 ]
             }
 
 
 if __name__ == '__main__':
     conf = PaValidation()
```

### Comparing `dpugen-0.0.9/dpugen/saigen/vips.py` & `dpugen-0.1.1/dpugen/saigen/vips.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 #!/usr/bin/python3
+"""SAI generator for VIP"""
 
 import os
 import sys
 
-from saigen.confbase import *
-from saigen.confutils import *
+from dpugen.confbase import ConfBase
+from dpugen.confutils import common_main
 
 
 class Vips(ConfBase):
 
     def __init__(self, params={}):
         super().__init__(params)
+        self.num_yields = 0
 
     def items(self):
         print('  Generating %s ...' % os.path.basename(__file__), file=sys.stderr)
-        self.num_yields = 0
         p = self.params
 
         self.num_yields += 1
         yield {
             'name': 'vip_#1',
             'op': 'create',
             'type': 'SAI_OBJECT_TYPE_VIP_ENTRY',
             'key': {
                 'switch_id': '$SWITCH_ID',
-                'vip': '%s' % p.LOOPBACK
+                'vip': p.LOOPBACK
             },
             'attributes': [
                 'SAI_VIP_ENTRY_ATTR_ACTION', 'SAI_VIP_ENTRY_ACTION_ACCEPT',
             ]
         }
```

### Comparing `dpugen-0.0.9/dpugen/saigen/vnets.py` & `dpugen-0.1.1/dpugen/saigen/vnets.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 #!/usr/bin/python3
+"""SAI generator for VNET"""
 
 import os
 import sys
 
-from saigen.confbase import *
-from saigen.confutils import *
+from dpugen.confbase import ConfBase
+from dpugen.confutils import common_main
 
 
 class Vnets(ConfBase):
 
     def __init__(self, params={}):
         super().__init__(params)
+        self.num_yields = 0
 
     def items(self):
         print('  Generating %s ...' % os.path.basename(__file__), file=sys.stderr)
-        self.num_yields = 0
         p = self.params
 
         for eni_index, eni in enumerate(range(p.ENI_START, p.ENI_START + p.ENI_COUNT * p.ENI_STEP, p.ENI_STEP)):
 
             self.num_yields += 1
             yield {
-                'name': 'vnet_#eni%d' % eni,
+                'name': f'vnet_#eni{eni}',
                 'op': 'create',
                 'type': 'SAI_OBJECT_TYPE_VNET',
                 'attributes': [
                     'SAI_VNET_ATTR_VNI', '%d' % (eni + p.ENI_L2R_STEP),
                 ]
             }
```

### Comparing `dpugen-0.0.9/setup.cfg` & `dpugen-0.1.1/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dpugen
-version = 0.0.9
+version = 0.1.1
 author = Mircea Dan Gheorghe
 author_email = mircea-dan.gheorghe@keysight.com
 description = Multi-vendor DPU library to generate its configuration
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mgheorghe/dpugen
 classifiers = 
@@ -13,22 +13,19 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= dpugen
 packages = find:
-python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*
+python_requires = >=2.7, <4
 install_requires = 
+	ipaddress
 	macaddress
 	munch
-	pyang
-	pyangbind
-	pytest
-	yangson
 
 [options.packages.find]
 where = dpugen
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

