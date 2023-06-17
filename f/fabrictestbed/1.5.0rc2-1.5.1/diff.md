# Comparing `tmp/fabrictestbed-1.5.0rc2.tar.gz` & `tmp/fabrictestbed-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-1.5.0rc2.tar", last modified: Fri May 12 13:47:33 2023, max compression
+gzip compressed data, was "fabrictestbed-1.5.1.tar", last modified: Sat Jun 17 10:06:29 2023, max compression
```

## Comparing `fabrictestbed-1.5.0rc2.tar` & `fabrictestbed-1.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1806 2023-05-11 17:40:59.099816 fabrictestbed-1.5.0rc2/.gitignore
--rw-r--r--   0        0        0     1071 2023-05-11 17:40:59.100151 fabrictestbed-1.5.0rc2/LICENSE
--rw-r--r--   0        0        0       24 2023-05-11 17:40:59.100302 fabrictestbed-1.5.0rc2/MANIFEST.in
--rw-r--r--   0        0        0     5603 2023-05-11 17:40:59.100450 fabrictestbed-1.5.0rc2/README.md
--rw-r--r--   0        0        0       25 2023-05-12 13:47:31.855483 fabrictestbed-1.5.0rc2/fabrictestbed/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 17:40:59.100987 fabrictestbed-1.5.0rc2/fabrictestbed/cli/__init__.py
--rw-r--r--   0        0        0    18169 2023-05-11 17:40:59.101162 fabrictestbed-1.5.0rc2/fabrictestbed/cli/cli.py
--rw-r--r--   0        0        0     1452 2023-05-11 17:40:59.101319 fabrictestbed-1.5.0rc2/fabrictestbed/cli/exceptions.py
--rw-r--r--   0        0        0     1914 2023-05-11 17:40:59.101479 fabrictestbed-1.5.0rc2/fabrictestbed/slice_editor/__init__.py
--rw-r--r--   0        0        0      201 2023-05-11 17:40:59.101641 fabrictestbed-1.5.0rc2/fabrictestbed/slice_manager/__init__.py
--rw-r--r--   0        0        0    17886 2023-05-11 17:40:59.101856 fabrictestbed-1.5.0rc2/fabrictestbed/slice_manager/slice_manager.py
--rw-r--r--   0        0        0        0 2023-05-11 17:40:59.101985 fabrictestbed-1.5.0rc2/fabrictestbed/util/__init__.py
--rw-r--r--   0        0        0     1452 2023-05-11 17:40:59.102200 fabrictestbed-1.5.0rc2/fabrictestbed/util/constants.py
--rw-r--r--   0        0        0      909 2023-05-12 13:47:25.949580 fabrictestbed-1.5.0rc2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-11 17:40:59.102597 fabrictestbed-1.5.0rc2/test/__init__.py
--rw-r--r--   0        0        0     2210 2023-05-11 17:40:59.102713 fabrictestbed-1.5.0rc2/test/test_cli.py
--rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 fabrictestbed-1.5.0rc2/PKG-INFO
+-rw-r--r--   0        0        0     1806 2023-05-11 17:40:59.099816 fabrictestbed-1.5.1/.gitignore
+-rw-r--r--   0        0        0     1071 2023-05-11 17:40:59.100151 fabrictestbed-1.5.1/LICENSE
+-rw-r--r--   0        0        0       24 2023-05-11 17:40:59.100302 fabrictestbed-1.5.1/MANIFEST.in
+-rw-r--r--   0        0        0     5603 2023-05-31 18:44:19.979642 fabrictestbed-1.5.1/README.md
+-rw-r--r--   0        0        0       22 2023-06-17 09:55:40.694524 fabrictestbed-1.5.1/fabrictestbed/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 17:40:59.100987 fabrictestbed-1.5.1/fabrictestbed/cli/__init__.py
+-rw-r--r--   0        0        0    18169 2023-05-11 17:40:59.101162 fabrictestbed-1.5.1/fabrictestbed/cli/cli.py
+-rw-r--r--   0        0        0     1452 2023-05-11 17:40:59.101319 fabrictestbed-1.5.1/fabrictestbed/cli/exceptions.py
+-rw-r--r--   0        0        0     1914 2023-05-11 17:40:59.101479 fabrictestbed-1.5.1/fabrictestbed/slice_editor/__init__.py
+-rw-r--r--   0        0        0      201 2023-05-11 17:40:59.101641 fabrictestbed-1.5.1/fabrictestbed/slice_manager/__init__.py
+-rw-r--r--   0        0        0    19811 2023-06-08 14:43:40.270937 fabrictestbed-1.5.1/fabrictestbed/slice_manager/slice_manager.py
+-rw-r--r--   0        0        0        0 2023-05-11 17:40:59.101985 fabrictestbed-1.5.1/fabrictestbed/util/__init__.py
+-rw-r--r--   0        0        0     1452 2023-05-11 17:40:59.102200 fabrictestbed-1.5.1/fabrictestbed/util/constants.py
+-rw-r--r--   0        0        0     1069 2023-06-17 09:55:40.689347 fabrictestbed-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-11 17:40:59.102597 fabrictestbed-1.5.1/test/__init__.py
+-rw-r--r--   0        0        0     2210 2023-05-11 17:40:59.102713 fabrictestbed-1.5.1/test/test_cli.py
+-rw-r--r--   0        0        0     6530 1970-01-01 00:00:00.000000 fabrictestbed-1.5.1/PKG-INFO
```

### Comparing `fabrictestbed-1.5.0rc2/.gitignore` & `fabrictestbed-1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.0rc2/LICENSE` & `fabrictestbed-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.0rc2/README.md` & `fabrictestbed-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.0rc2/fabrictestbed/cli/cli.py` & `fabrictestbed-1.5.1/fabrictestbed/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.0rc2/fabrictestbed/cli/exceptions.py` & `fabrictestbed-1.5.1/fabrictestbed/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.0rc2/fabrictestbed/slice_editor/__init__.py` & `fabrictestbed-1.5.1/fabrictestbed/slice_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.0rc2/fabrictestbed/slice_manager/slice_manager.py` & `fabrictestbed-1.5.1/fabrictestbed/slice_manager/slice_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,18 +22,19 @@
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 import json
 import os
 from datetime import datetime, timedelta
-from typing import Tuple, Union, List, Any
+from typing import Tuple, Union, List, Any, Dict
 
 import paramiko
 from fabric_cf.orchestrator.swagger_client import Sliver, Slice
+from fabric_cf.orchestrator.swagger_client.models import PoaData
 
 from fabrictestbed.slice_editor import ExperimentTopology, AdvertisedTopology, Node, GraphFormat
 from fabrictestbed.slice_manager import CredmgrProxy, OrchestratorProxy, CmStatus, Status, SliceState
 from fabrictestbed.util.constants import Constants
 
 
 class SliceManagerException(Exception):
@@ -186,26 +187,26 @@
         if cache_file_name is None:
             cache_file_name = self.token_location
         status, exception = self.cm_proxy.clear_token_cache(file_name=cache_file_name)
         if status == CmStatus.OK:
             return Status.OK, None
         return Status.FAILURE, f"Failed to clear token cache: {exception}"
 
-    def create(self, *, slice_name: str, ssh_key: str, topology: ExperimentTopology = None, slice_graph: str = None,
-               lease_end_time: str = None) -> Tuple[Status, Union[Exception, List[Sliver]]]:
+    def create(self, *, slice_name: str, ssh_key: Union[str, List[str]], topology: ExperimentTopology = None,
+               slice_graph: str = None, lease_end_time: str = None) -> Tuple[Status, Union[Exception, List[Sliver]]]:
         """
         Create a slice
         @param slice_name slice name
-        @param ssh_key SSH Key
+        @param ssh_key SSH Key(s)
         @param topology Experiment topology
         @param slice_graph Slice Graph string
         @param lease_end_time Lease End Time
         @return Tuple containing Status and Exception/Json containing slivers created
         """
-        if slice_name is None or not isinstance(slice_name, str) or ssh_key is None or not isinstance(ssh_key, str):
+        if slice_name is None or not isinstance(slice_name, str) or ssh_key is None:
             return Status.INVALID_ARGUMENTS, SliceManagerException("Invalid arguments - slice_name or ssh key")
 
         if topology is not None and not isinstance(topology, ExperimentTopology):
             return Status.INVALID_ARGUMENTS, SliceManagerException("Invalid arguments - topology")
 
         if slice_graph is not None and not isinstance(slice_graph, str):
             return Status.INVALID_ARGUMENTS, SliceManagerException("Invalid arguments - slice_graph")
@@ -264,58 +265,62 @@
         """
         if self.__should_renew():
             self.__load_tokens()
         slice_id = slice_object.slice_id if slice_object is not None else None
         return self.oc_proxy.delete(token=self.get_id_token(), slice_id=slice_id)
 
     def slices(self, includes: List[SliceState] = None, excludes: List[SliceState] = None, name: str = None,
-               limit: int = 20, offset: int = 0, slice_id: str = None) -> Tuple[Status, Union[Exception, List[Slice]]]:
+               limit: int = 20, offset: int = 0, slice_id: str = None,
+               as_self: bool = True) -> Tuple[Status, Union[Exception, List[Slice]]]:
         """
         Get slices
         @param includes list of the slice state used to include the slices in the output
         @param excludes list of the slice state used to exclude the slices from the output
         @param name name of the slice
         @param limit maximum number of slices to return
         @param offset offset of the first slice to return
         @param slice_id slice id
+        @param as_self
         @return Tuple containing Status and Exception/Json containing slices
         """
         if self.__should_renew():
             self.__load_tokens()
         return self.oc_proxy.slices(token=self.get_id_token(), includes=includes, excludes=excludes,
-                                    name=name, limit=limit, offset=offset, slice_id=slice_id)
+                                    name=name, limit=limit, offset=offset, slice_id=slice_id, as_self=as_self)
 
-    def get_slice_topology(self, *, slice_object: Slice,
-                           graph_format: GraphFormat = GraphFormat.GRAPHML) -> Tuple[Status, Union[Exception, ExperimentTopology]]:
+    def get_slice_topology(self, *, slice_object: Slice, graph_format: GraphFormat = GraphFormat.GRAPHML,
+                           as_self: bool = True) -> Tuple[Status, Union[Exception, ExperimentTopology]]:
         """
         Get slice topology
         @param slice_object Slice for which to retrieve the topology
         @param graph_format
+        @param as_self
         @return Tuple containing Status and Exception/Json containing slice
         """
         if slice_object is None or not isinstance(slice_object, Slice):
             return Status.INVALID_ARGUMENTS, SliceManagerException("Invalid arguments - slice_object")
         if self.__should_renew():
             self.__load_tokens()
         return self.oc_proxy.get_slice(token=self.get_id_token(), slice_id=slice_object.slice_id,
-                                       graph_format=graph_format)
+                                       graph_format=graph_format, as_self=as_self)
 
-    def slivers(self, *, slice_object: Slice) -> Tuple[Status, Union[Exception, List[Sliver]]]:
+    def slivers(self, *, slice_object: Slice, as_self: bool = True) -> Tuple[Status, Union[Exception, List[Sliver]]]:
         """
         Get slivers
         @param slice_object list of the slices
+        @param as_self
         @return Tuple containing Status and Exception/Json containing Sliver(s)
         """
         if slice_object is None or not isinstance(slice_object, Slice):
             return Status.INVALID_ARGUMENTS, SliceManagerException("Invalid arguments - slice_object")
 
         if self.__should_renew():
             self.__load_tokens()
 
-        return self.oc_proxy.slivers(token=self.get_id_token(), slice_id=slice_object.slice_id)
+        return self.oc_proxy.slivers(token=self.get_id_token(), slice_id=slice_object.slice_id, as_self=as_self)
 
     def resources(self, *, level: int = 1,
                   force_refresh: bool = False) -> Tuple[Status, Union[Exception, AdvertisedTopology]]:
         """
         Get resources
         @param level level
         @param force_refresh force_refresh
@@ -338,14 +343,48 @@
 
         if self.__should_renew():
             self.__load_tokens()
 
         return self.oc_proxy.renew(token=self.get_id_token(), slice_id=slice_object.slice_id,
                                    new_lease_end_time=new_lease_end_time)
 
+    def poa(self, *, sliver_id: str, operation: str, vcpu_cpu_map: List[Dict[str, str]] = None,
+            node_set: List[str] = None) ->Tuple[Status, Union[Exception, List[PoaData]]]:
+        """
+        Issue POA for a sliver
+        @param sliver_id sliver Id for which to trigger POA
+        @param operation operation
+        @param vcpu_cpu_map list of mappings from virtual CPU to physical cpu
+        @param node_set list of the numa nodes
+        @return Tuple containing Status and POA information
+       """
+        if sliver_id is None or operation is None:
+            return Status.INVALID_ARGUMENTS, SliceManagerException("Invalid arguments - sliver_id or operation")
+
+        if self.__should_renew():
+            self.__load_tokens()
+
+        return self.oc_proxy.poa(token=self.get_id_token(), sliver_id=sliver_id, operation=operation,
+                                 vcpu_cpu_map=vcpu_cpu_map, node_set=node_set)
+
+    def get_poas(self, sliver_id: str = None, poa_id: str = None, limit: int = 20,
+                 offset: int = 0, ) -> Tuple[Status, Union[Exception, List[PoaData]]]:
+        """
+        Get POAs
+        @param sliver_id sliver Id for which to trigger POA
+        @param limit maximum number of slices to return
+        @param offset offset of the first slice to return
+        @param poa_id POA id identifying the POA
+        @return Tuple containing Status and POA information
+        """
+        if self.__should_renew():
+            self.__load_tokens()
+        return self.oc_proxy.get_poas(token=self.get_id_token(), limit=limit, offset=offset, sliver_id=sliver_id,
+                                      poa_id=poa_id)
+
     @staticmethod
     def __get_ssh_client() -> paramiko.SSHClient():
         client = paramiko.SSHClient()
         client.load_system_host_keys()
         client.set_missing_host_key_policy(paramiko.MissingHostKeyPolicy())
         client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
         return client
```

### Comparing `fabrictestbed-1.5.0rc2/fabrictestbed/util/constants.py` & `fabrictestbed-1.5.1/fabrictestbed/util/constants.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.0rc2/pyproject.toml` & `fabrictestbed-1.5.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -14,21 +14,29 @@
 dynamic = ["version"]
 
 keywords = ["Swagger", "FABRIC Python Client Library with CLI"]
 
 requires-python = '>=3.9'
 dependencies = [
     "click",
-    "fabric-credmgr-client==1.5.0rc1",
-    "fabric-orchestrator-client==1.5.0rc2",
+    "fabric-credmgr-client==1.5.0",
+    "fabric-orchestrator-client==1.5.1",
     "paramiko"
     ]
 
 scripts = {"fabric-cli" = "fabrictestbed.cli.cli:cli"}
 
+[project.optional-dependencies]
+test = ["coverage>=4.0.3",
+        "nose>=1.3.7",
+        "pluggy>=0.3.1",
+        "py>=1.4.31",
+        "randomize>=0.13"
+        ]
+
 [project.urls]
 Home = "https://fabric-testbed.net/"
 Sources = "https://github.com/fabric-testbed/fabric-cli"
 
 
 [tool.flit.module]
 name = "fabrictestbed"
```

### Comparing `fabrictestbed-1.5.0rc2/test/test_cli.py` & `fabrictestbed-1.5.1/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-1.5.0rc2/PKG-INFO` & `fabrictestbed-1.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: fabrictestbed
-Version: 1.5.0rc2
+Version: 1.5.1
 Summary: FABRIC Python Client Library with CLI
 Keywords: Swagger,FABRIC Python Client Library with CLI
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: click
-Requires-Dist: fabric-credmgr-client==1.5.0rc1
-Requires-Dist: fabric-orchestrator-client==1.5.0rc2
+Requires-Dist: fabric-credmgr-client==1.5.0
+Requires-Dist: fabric-orchestrator-client==1.5.1
 Requires-Dist: paramiko
+Requires-Dist: coverage>=4.0.3 ; extra == "test"
+Requires-Dist: nose>=1.3.7 ; extra == "test"
+Requires-Dist: pluggy>=0.3.1 ; extra == "test"
+Requires-Dist: py>=1.4.31 ; extra == "test"
+Requires-Dist: randomize>=0.13 ; extra == "test"
 Project-URL: Home, https://fabric-testbed.net/
 Project-URL: Sources, https://github.com/fabric-testbed/fabric-cli
+Provides-Extra: test
 
 [![PyPI](https://img.shields.io/pypi/v/fabrictestbed?style=plastic)](https://pypi.org/project/fabrictestbed/)
 
 
 # FABRIC TESTBED USER LIBRARY AND CLI
 
 Fabric User CLI for experiments
```

