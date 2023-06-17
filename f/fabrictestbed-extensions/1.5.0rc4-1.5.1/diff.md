# Comparing `tmp/fabrictestbed-extensions-1.5.0rc4.tar.gz` & `tmp/fabrictestbed-extensions-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrictestbed-extensions-1.5.0rc4.tar", last modified: Mon Jun 12 17:31:24 2023, max compression
+gzip compressed data, was "fabrictestbed-extensions-1.5.1.tar", last modified: Sat Jun 17 10:20:23 2023, max compression
```

## Comparing `fabrictestbed-extensions-1.5.0rc4.tar` & `fabrictestbed-extensions-1.5.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1025 2023-05-11 18:23:24.341681 fabrictestbed-extensions-1.5.0rc4/.github/workflows/build.yml
--rw-r--r--   0        0        0     1618 2023-05-11 18:23:24.341808 fabrictestbed-extensions-1.5.0rc4/.github/workflows/checks.yml
--rw-r--r--   0        0        0     2402 2023-05-11 18:23:24.341926 fabrictestbed-extensions-1.5.0rc4/.github/workflows/test.yml
--rw-r--r--   0        0        0     1806 2023-05-12 13:41:06.568624 fabrictestbed-extensions-1.5.0rc4/.gitignore
--rw-r--r--   0        0        0      666 2023-05-11 18:23:24.342134 fabrictestbed-extensions-1.5.0rc4/.readthedocs.yaml
--rw-r--r--   0        0        0     2897 2023-06-08 17:08:10.775764 fabrictestbed-extensions-1.5.0rc4/CHANGELOG.md
--rw-r--r--   0        0        0     1071 2023-05-11 18:23:24.342656 fabrictestbed-extensions-1.5.0rc4/LICENSE
--rw-r--r--   0        0        0     4054 2023-05-11 18:23:24.342855 fabrictestbed-extensions-1.5.0rc4/README.md
--rw-r--r--   0        0        0      638 2023-05-11 18:23:24.343022 fabrictestbed-extensions-1.5.0rc4/docs/Makefile
--rw-r--r--   0        0        0      799 2023-05-11 18:23:24.343131 fabrictestbed-extensions-1.5.0rc4/docs/make.bat
--rw-r--r--   0        0        0     1996 2023-05-11 18:23:24.343312 fabrictestbed-extensions-1.5.0rc4/docs/source/conf.py
--rw-r--r--   0        0        0     8903 2023-05-12 13:41:06.569256 fabrictestbed-extensions-1.5.0rc4/docs/source/fablib.rst
--rw-r--r--   0        0        0     4470 2023-05-11 18:23:24.343613 fabrictestbed-extensions-1.5.0rc4/docs/source/index.rst
--rw-r--r--   0        0        0      150 2023-06-12 17:31:16.009089 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/__init__.py
--rw-r--r--   0        0        0        2 2023-05-11 18:23:24.344271 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/editors/__init__.py
--rw-r--r--   0        0        0    18044 2023-05-11 18:23:24.344572 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/editors/abc_topology_editor.py
--rw-r--r--   0        0        0     6277 2023-05-11 18:23:24.345052 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
--rw-r--r--   0        0        0    68479 2023-05-11 18:23:24.345347 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/editors/geo_topology_editor.py
--rw-r--r--   0        0        0        1 2023-05-11 18:23:24.345570 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/__init__.py
--rw-r--r--   0        0        0     4793 2023-05-11 18:23:24.345738 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/abc_fablib.py
--rw-r--r--   0        0        0    21402 2023-06-11 18:11:35.985267 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/component.py
--rw-r--r--   0        0        0    77331 2023-06-12 00:53:42.710305 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/fablib.py
--rw-r--r--   0        0        0     5821 2023-06-08 17:08:10.777119 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/facility_port.py
--rw-r--r--   0        0        0    26262 2023-06-11 18:14:38.646369 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/interface.py
--rw-r--r--   0        0        0    40019 2023-06-08 17:08:10.777971 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/network_service.py
--rw-r--r--   0        0        0    96366 2023-06-10 11:36:12.662165 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/node.py
--rw-r--r--   0        0        0    38331 2023-06-12 00:52:03.202648 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/resources.py
--rw-r--r--   0        0        0    81762 2023-06-08 17:08:10.780745 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/slice.py
--rw-r--r--   0        0        0        2 2023-05-11 18:23:24.350075 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/images/__init__.py
--rw-r--r--   0        0        0   199914 2023-05-11 18:23:24.351514 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/images/fabric_logo.png
--rw-r--r--   0        0        0     1316 2023-05-11 18:23:24.351919 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/images/server.png
--rw-r--r--   0        0        0    62250 2023-05-11 18:23:24.352243 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/images/slice_rack.png
--rw-r--r--   0        0        0        2 2023-05-11 18:23:24.352522 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/__init__.py
--rw-r--r--   0        0        0    14765 2023-05-11 18:23:24.352740 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/abc_test.py
--rw-r--r--   0        0        0    34389 2023-06-09 15:08:19.572155 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/component_tests.py
--rw-r--r--   0        0        0       85 2023-05-11 18:23:24.353250 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/dummy-token.json
--rw-r--r--   0        0        0    13366 2023-05-11 18:23:24.353667 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py
--rw-r--r--   0        0        0    10227 2023-05-11 18:23:24.353942 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/hello_fabric.py
--rw-r--r--   0        0        0    20659 2023-05-11 18:23:24.354269 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/link_benchmark.py
--rw-r--r--   0        0        0    20919 2023-05-11 18:23:24.354513 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/local_network_benchmark.py
--rw-r--r--   0        0        0    44883 2023-05-11 18:23:24.354856 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/network_benchmark_tests.py
--rw-r--r--   0        0        0    10052 2023-05-11 18:23:24.355043 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/nvme_benchmark.py
--rw-r--r--   0        0        0     5095 2023-05-11 18:23:24.355416 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/test_basic.py
--rw-r--r--   0        0        0        2 2023-05-11 18:23:24.355793 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/utils/__init__.py
--rw-r--r--   0        0        0     3082 2023-05-11 18:23:24.356170 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/utils/abc_utils.py
--rw-r--r--   0        0        0     3304 2023-05-11 18:23:24.356417 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/utils/node.py
--rw-r--r--   0        0        0     8436 2023-05-11 18:23:24.356653 fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/utils/slice.py
--rw-r--r--   0        0        0     1340 2023-06-12 17:30:38.138232 fabrictestbed-extensions-1.5.0rc4/pyproject.toml
--rwxr-xr-x   0        0        0      122 2023-05-11 18:23:24.357218 fabrictestbed-extensions-1.5.0rc4/sphinx.sh
--rw-r--r--   0        0        0     5275 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.5.0rc4/PKG-INFO
+-rw-r--r--   0        0        0     1025 2023-05-11 18:23:24.341681 fabrictestbed-extensions-1.5.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1618 2023-05-11 18:23:24.341808 fabrictestbed-extensions-1.5.1/.github/workflows/checks.yml
+-rw-r--r--   0        0        0     2402 2023-05-11 18:23:24.341926 fabrictestbed-extensions-1.5.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1806 2023-05-12 13:41:06.568624 fabrictestbed-extensions-1.5.1/.gitignore
+-rw-r--r--   0        0        0      666 2023-05-11 18:23:24.342134 fabrictestbed-extensions-1.5.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     2897 2023-06-08 17:08:10.775764 fabrictestbed-extensions-1.5.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2023-05-11 18:23:24.342656 fabrictestbed-extensions-1.5.1/LICENSE
+-rw-r--r--   0        0        0     4054 2023-05-11 18:23:24.342855 fabrictestbed-extensions-1.5.1/README.md
+-rw-r--r--   0        0        0      638 2023-05-11 18:23:24.343022 fabrictestbed-extensions-1.5.1/docs/Makefile
+-rw-r--r--   0        0        0      799 2023-05-11 18:23:24.343131 fabrictestbed-extensions-1.5.1/docs/make.bat
+-rw-r--r--   0        0        0     1996 2023-05-11 18:23:24.343312 fabrictestbed-extensions-1.5.1/docs/source/conf.py
+-rw-r--r--   0        0        0     8968 2023-06-12 18:07:22.395922 fabrictestbed-extensions-1.5.1/docs/source/fablib.rst
+-rw-r--r--   0        0        0     4470 2023-05-11 18:23:24.343613 fabrictestbed-extensions-1.5.1/docs/source/index.rst
+-rw-r--r--   0        0        0      147 2023-06-16 15:42:46.821851 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/__init__.py
+-rw-r--r--   0        0        0        2 2023-05-11 18:23:24.344271 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/editors/__init__.py
+-rw-r--r--   0        0        0    18044 2023-05-11 18:23:24.344572 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/editors/abc_topology_editor.py
+-rw-r--r--   0        0        0     6277 2023-05-11 18:23:24.345052 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/editors/cytoscape_topology_editor.py
+-rw-r--r--   0        0        0    68479 2023-05-11 18:23:24.345347 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/editors/geo_topology_editor.py
+-rw-r--r--   0        0        0        1 2023-05-11 18:23:24.345570 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/__init__.py
+-rw-r--r--   0        0        0     4793 2023-05-11 18:23:24.345738 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/abc_fablib.py
+-rw-r--r--   0        0        0    21455 2023-06-14 14:18:40.297506 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/component.py
+-rw-r--r--   0        0        0    77331 2023-06-15 15:40:37.951763 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/fablib.py
+-rw-r--r--   0        0        0     5821 2023-06-08 17:08:10.777119 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/facility_port.py
+-rw-r--r--   0        0        0    26311 2023-06-16 15:44:08.976055 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/interface.py
+-rw-r--r--   0        0        0    40019 2023-06-08 17:08:10.777971 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/network_service.py
+-rw-r--r--   0        0        0    96366 2023-06-10 11:36:12.662165 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/node.py
+-rw-r--r--   0        0        0    38331 2023-06-12 00:52:03.202648 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/resources.py
+-rw-r--r--   0        0        0    81762 2023-06-08 17:08:10.780745 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/slice.py
+-rw-r--r--   0        0        0        2 2023-05-11 18:23:24.350075 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/images/__init__.py
+-rw-r--r--   0        0        0   199914 2023-05-11 18:23:24.351514 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/images/fabric_logo.png
+-rw-r--r--   0        0        0     1316 2023-05-11 18:23:24.351919 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/images/server.png
+-rw-r--r--   0        0        0    62250 2023-05-11 18:23:24.352243 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/images/slice_rack.png
+-rw-r--r--   0        0        0        2 2023-05-11 18:23:24.352522 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/__init__.py
+-rw-r--r--   0        0        0    14765 2023-05-11 18:23:24.352740 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/abc_test.py
+-rw-r--r--   0        0        0    34389 2023-06-09 15:08:19.572155 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/component_tests.py
+-rw-r--r--   0        0        0       85 2023-05-11 18:23:24.353250 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/dummy-token.json
+-rw-r--r--   0        0        0    13366 2023-05-11 18:23:24.353667 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py
+-rw-r--r--   0        0        0    10227 2023-05-11 18:23:24.353942 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/hello_fabric.py
+-rw-r--r--   0        0        0    20659 2023-05-11 18:23:24.354269 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/link_benchmark.py
+-rw-r--r--   0        0        0    20919 2023-05-11 18:23:24.354513 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/local_network_benchmark.py
+-rw-r--r--   0        0        0    44883 2023-05-11 18:23:24.354856 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/network_benchmark_tests.py
+-rw-r--r--   0        0        0    10052 2023-05-11 18:23:24.355043 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/nvme_benchmark.py
+-rw-r--r--   0        0        0     5095 2023-05-11 18:23:24.355416 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/test_basic.py
+-rw-r--r--   0        0        0        2 2023-05-11 18:23:24.355793 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/utils/__init__.py
+-rw-r--r--   0        0        0     3082 2023-05-11 18:23:24.356170 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/utils/abc_utils.py
+-rw-r--r--   0        0        0     3304 2023-05-11 18:23:24.356417 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/utils/node.py
+-rw-r--r--   0        0        0     8436 2023-05-11 18:23:24.356653 fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/utils/slice.py
+-rw-r--r--   0        0        0     1340 2023-06-17 09:55:40.708206 fabrictestbed-extensions-1.5.1/pyproject.toml
+-rwxr-xr-x   0        0        0      122 2023-05-11 18:23:24.357218 fabrictestbed-extensions-1.5.1/sphinx.sh
+-rw-r--r--   0        0        0     5272 1970-01-01 00:00:00.000000 fabrictestbed-extensions-1.5.1/PKG-INFO
```

### Comparing `fabrictestbed-extensions-1.5.0rc4/.github/workflows/build.yml` & `fabrictestbed-extensions-1.5.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/.github/workflows/checks.yml` & `fabrictestbed-extensions-1.5.1/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/.github/workflows/test.yml` & `fabrictestbed-extensions-1.5.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/.gitignore` & `fabrictestbed-extensions-1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/.readthedocs.yaml` & `fabrictestbed-extensions-1.5.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/CHANGELOG.md` & `fabrictestbed-extensions-1.5.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/LICENSE` & `fabrictestbed-extensions-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/README.md` & `fabrictestbed-extensions-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/docs/Makefile` & `fabrictestbed-extensions-1.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/docs/make.bat` & `fabrictestbed-extensions-1.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/docs/source/conf.py` & `fabrictestbed-extensions-1.5.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/docs/source/fablib.rst` & `fabrictestbed-extensions-1.5.1/docs/source/fablib.rst`

 * *Files 0% similar despite different names*

```diff
@@ -385,14 +385,16 @@
 
   .. automethod:: get_reservation_state
 
   .. automethod:: get_error_message
 
   .. automethod:: configure_nvme
 
+  .. automethod:: get_numa_node
+
 
 
 .. automodule:: interface
 
 ``Interface``
 ----------------------
 
@@ -447,14 +449,15 @@
 
   .. automethod:: get_ip_link
 
   .. automethod::  get_ip_addr
 
   .. automethod::  get_ips
 
+  .. automethod:: get_numa_node
 
 .. automodule:: network_service
 
 
 ``NetworkService``
 ------------------------------------
```

### Comparing `fabrictestbed-extensions-1.5.0rc4/docs/source/index.rst` & `fabrictestbed-extensions-1.5.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/editors/abc_topology_editor.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/editors/abc_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/editors/cytoscape_topology_editor.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/editors/cytoscape_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/editors/geo_topology_editor.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/editors/geo_topology_editor.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/abc_fablib.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/abc_fablib.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/component.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,15 +401,16 @@
         """
         return self.get_fim_component().details
 
     def get_numa_node(self) -> str:
         """
         Get the Numa Node assigned to the device
         """
-        return self.get_fim_component().get_property(pname="label_allocations").numa
+        if self.get_fim_component() is not None:
+            return self.get_fim_component().get_property(pname="label_allocations").numa
 
     def get_disk(self) -> int:
         """
         Gets the amount of disk space on this component.
 
         :return: this component's disk space
         :rtype: int
```

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/fablib.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/fablib.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/facility_port.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/facility_port.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/interface.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,16 @@
             "physical_dev": physical_dev,
             "dev": dev,
             "ip_addr": ip_addr,
             "numa": str(self.get_numa_node()),
         }
 
     def get_numa_node(self) -> str:
-        return self.get_component().get_numa_node()
+        if self.get_component() is not None:
+            return self.get_component().get_numa_node()
 
     def generate_template_context(self):
         context = self.toDict()
         return context
 
     def get_template_context(self):
         return self.get_slice().get_template_context(self)
```

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/network_service.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/network_service.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/node.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/node.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/resources.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/resources.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/fablib/slice.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/fablib/slice.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/images/fabric_logo.png` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/images/fabric_logo.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/images/server.png` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/images/server.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/images/slice_rack.png` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/images/slice_rack.png`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/abc_test.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/abc_test.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/component_tests.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/component_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/gpu_tesla_t4_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/hello_fabric.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/hello_fabric.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/link_benchmark.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/link_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/local_network_benchmark.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/local_network_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/network_benchmark_tests.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/network_benchmark_tests.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/nvme_benchmark.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/nvme_benchmark.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/tests/test_basic.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/utils/abc_utils.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/utils/abc_utils.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/utils/node.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/utils/node.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/fabrictestbed_extensions/utils/slice.py` & `fabrictestbed-extensions-1.5.1/fabrictestbed_extensions/utils/slice.py`

 * *Files identical despite different names*

### Comparing `fabrictestbed-extensions-1.5.0rc4/pyproject.toml` & `fabrictestbed-extensions-1.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 requires-python = ">=3.9"
 dependencies = [
     "ipycytoscape",
     "ipywidgets",
     "ipyleaflet",
     "ipycytoscape",
     "tabulate",
-    "fabrictestbed==1.5.0",
+    "fabrictestbed==1.5.1",
     "paramiko",
     "jinja2>=3.0.0",
     "pandas",
     "numpy",
     "ipython>=8.12.0"
     ]
```

### Comparing `fabrictestbed-extensions-1.5.0rc4/PKG-INFO` & `fabrictestbed-extensions-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: fabrictestbed-extensions
-Version: 1.5.0rc4
+Version: 1.5.1
 Summary: FABRIC Python Client Library and CLI Extensions
 Author-email: Paul Ruth <pruth@renci.org>, Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: ipycytoscape
 Requires-Dist: ipywidgets
 Requires-Dist: ipyleaflet
 Requires-Dist: ipycytoscape
 Requires-Dist: tabulate
-Requires-Dist: fabrictestbed==1.5.0
+Requires-Dist: fabrictestbed==1.5.1
 Requires-Dist: paramiko
 Requires-Dist: jinja2>=3.0.0
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: ipython>=8.12.0
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: furo ; extra == "doc"
```

