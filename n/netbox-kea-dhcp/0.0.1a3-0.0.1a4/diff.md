# Comparing `tmp/netbox_kea_dhcp-0.0.1a3.tar.gz` & `tmp/netbox_kea_dhcp-0.0.1a4.tar.gz`

## Comparing `netbox_kea_dhcp-0.0.1a3.tar` & `netbox_kea_dhcp-0.0.1a4.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/netboxkea/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/netboxkea/__init__.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/netboxkea/config.py
--rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/netboxkea/connector.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/netboxkea/entry_point.py
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/netboxkea/listener.py
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/netboxkea/netbox.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/netboxkea/kea/__init__.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/netboxkea/kea/api.py
--rw-r--r--   0        0        0     9024 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/netboxkea/kea/app.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/netboxkea/kea/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/fixtures/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/__init__.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/devices.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/interfaces.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/ip_addresses.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/ip_ranges.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/prefixes.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/virtual_machines.py
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/vminterfaces.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/unit/__init__.py
--rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/unit/test_connector.py
--rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/tests/unit/test_kea.py
--rw-r--r--   0        0        0   792962 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/examples/kea-dhcp4-examples.conf
--rw-r--r--   0        0        0   627796 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/examples/kea-dhcp4.conf
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/examples/netbox-kea-dhcp.example.toml
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/LICENSE
--rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/README.md
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/pyproject.toml
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/netboxkea/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/netboxkea/__init__.py
+-rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/netboxkea/config.py
+-rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/netboxkea/connector.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/netboxkea/entry_point.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/netboxkea/listener.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/netboxkea/logger.py
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/netboxkea/netbox.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/netboxkea/kea/__init__.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/netboxkea/kea/api.py
+-rw-r--r--   0        0        0     9024 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/netboxkea/kea/app.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/netboxkea/kea/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/tests/fixtures/pynetbox/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/tests/fixtures/pynetbox/devices.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/tests/fixtures/pynetbox/interfaces.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/tests/fixtures/pynetbox/ip_addresses.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/tests/fixtures/pynetbox/ip_ranges.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/tests/fixtures/pynetbox/prefixes.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/tests/fixtures/pynetbox/virtual_machines.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/tests/fixtures/pynetbox/vminterfaces.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/tests/unit/__init__.py
+-rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/tests/unit/test_connector.py
+-rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/tests/unit/test_kea.py
+-rw-r--r--   0        0        0   792962 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/examples/kea-dhcp4-examples.conf
+-rw-r--r--   0        0        0   627796 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/examples/kea-dhcp4.conf
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/examples/netbox-kea-dhcp.example.toml
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/LICENSE
+-rw-r--r--   0        0        0     6036 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/README.md
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/pyproject.toml
+-rw-r--r--   0        0        0     6927 2020-02-02 00:00:00.000000 netbox_kea_dhcp-0.0.1a4/PKG-INFO
```

### Comparing `netbox_kea_dhcp-0.0.1a3/netboxkea/config.py` & `netbox_kea_dhcp-0.0.1a4/netboxkea/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     listen: bool = False
     bind: str = '127.0.0.1'
     port: int = 8001
     secret: str = None
     secret_header: str = 'X-netbox2kea-secret'
     log_level: str = 'warning'
     ext_log_level: str = 'warning'
-    # TODO: syslog: bool = False
+    syslog_level_prefix: bool = False
     kea_url: str = None
     netbox_url: str = None
     netbox_token: str = None
     prefix_filter: dict = field(default_factory=dict)
     ipaddress_filter: dict = field(default_factory=lambda: {'status': 'dhcp'})
     iprange_filter: dict = field(default_factory=dict)
     prefix_dhcp_map: dict = field(default_factory=lambda: {
```

### Comparing `netbox_kea_dhcp-0.0.1a3/netboxkea/connector.py` & `netbox_kea_dhcp-0.0.1a4/netboxkea/connector.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a3/netboxkea/listener.py` & `netbox_kea_dhcp-0.0.1a4/netboxkea/listener.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a3/netboxkea/netbox.py` & `netbox_kea_dhcp-0.0.1a4/netboxkea/netbox.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a3/netboxkea/kea/api.py` & `netbox_kea_dhcp-0.0.1a4/netboxkea/kea/api.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a3/netboxkea/kea/app.py` & `netbox_kea_dhcp-0.0.1a4/netboxkea/kea/app.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/devices.py` & `netbox_kea_dhcp-0.0.1a4/tests/fixtures/pynetbox/devices.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/interfaces.py` & `netbox_kea_dhcp-0.0.1a4/tests/fixtures/pynetbox/interfaces.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/ip_addresses.py` & `netbox_kea_dhcp-0.0.1a4/tests/fixtures/pynetbox/ip_addresses.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/ip_ranges.py` & `netbox_kea_dhcp-0.0.1a4/tests/fixtures/pynetbox/ip_ranges.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/prefixes.py` & `netbox_kea_dhcp-0.0.1a4/tests/fixtures/pynetbox/prefixes.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/virtual_machines.py` & `netbox_kea_dhcp-0.0.1a4/tests/fixtures/pynetbox/virtual_machines.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a3/tests/fixtures/pynetbox/vminterfaces.py` & `netbox_kea_dhcp-0.0.1a4/tests/fixtures/pynetbox/vminterfaces.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a3/tests/unit/test_connector.py` & `netbox_kea_dhcp-0.0.1a4/tests/unit/test_connector.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a3/tests/unit/test_kea.py` & `netbox_kea_dhcp-0.0.1a4/tests/unit/test_kea.py`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a3/examples/kea-dhcp4-examples.conf` & `netbox_kea_dhcp-0.0.1a4/examples/kea-dhcp4-examples.conf`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a3/examples/kea-dhcp4.conf` & `netbox_kea_dhcp-0.0.1a4/examples/kea-dhcp4.conf`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a3/examples/netbox-kea-dhcp.example.toml` & `netbox_kea_dhcp-0.0.1a4/examples/netbox-kea-dhcp.example.toml`

 * *Files 21% similar despite different names*

```diff
@@ -6,22 +6,28 @@
 listen = false
 bind = "0.0.0.0"
 port = 8000
 secret = "azerQSDF1234uiopJKLM7890"
 # This is the default value:
 #secret_header = "X-netbox2kea-secret"
 
-#log_level = "debug"    # or "info", "warning" (default), "error"
-#ext_log_level = "warning"    # Log level for external modules
-# TODO: syslog = false
-
 netbox_url = "http://10.94.135.32:8000/"
 netbox_token = "9123456789abcdef0123456789abcdef01234568"
 kea_url = "http://10.94.135.209:8000/"
 
+#log_level = "debug"          # or "info", "warning" (default), "error"
+#ext_log_level = "warning"    # Log level for external modules
+
+# Prefix log messages with syslog level. Intended for systemd unit parameter
+# "SyslogLevelPrefix", as described on
+# https://www.freedesktop.org/software/systemd/man/systemd.exec.html#SyslogLevelPrefix=.
+# Messages are always sent to standard or error outputs.
+# If set to false (default), a date-time prefix will be used instead.
+#syslog_level_prefix = true
+
 #
 # Netbox-DHCP maps: mapping from netbox custom fields to Kea DHCP attributes
 #
 # Below is the default prefixes’map
 #[prefix_dhcp_map]
 #dhcp_option_data_routers = "option-data.routers"
 #dhcp_option_data_domain_search = "option-data.domain-search"
```

### Comparing `netbox_kea_dhcp-0.0.1a3/.gitignore` & `netbox_kea_dhcp-0.0.1a4/.gitignore`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a3/LICENSE` & `netbox_kea_dhcp-0.0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a3/README.md` & `netbox_kea_dhcp-0.0.1a4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -97,16 +97,16 @@
   * `DCIM`: `Interface`, `Device`.
   * `Virtualization`: `Interface`, `Virtual Machine`.
 - Events: `Creations`, `Updates`, `Deletions`.
 - HTTP Request:
   * URL: `http://{netbox-connector-host}:{port}/event/{free-text}/`
   * HTTP Method: `POST`.
 
-The field `free-text` permits to define several webhooks with same events. The
-connector only uses it in logs.
+The field `free-text` is necessary to define several webhooks with same events.
+The connector only uses it in logs.
 
 More help with `netbox-kea-dhcp --help` and in the configuration file example
 under `examples/` (or under
 `~/.local/pipx/venvs/netbox-kea-dhcp/lib/python3.10/site-packages/examples/` if
 app was installed with pipx).
 
 Recommended Netbox webhooks
@@ -114,15 +114,15 @@
 
 It’s recommended to set several webhooks with conditions and restricted body
 template, in order to filter events and avoid unecessary network and CPU load:
 
 Common to all webhooks:
 
 - HTTP Request:
-  * URL: `http://{netbox-connector-host}:{port}/event/{optional-free-text}`
+  * URL: `http://{netbox-connector-host}:{port}/event/{optional-free-text}/`
   * HTTP Method: `POST`.
 - Body template:
 
     ```json
     { "event": "{{ event }}",
       "model": "{{ model }}",
       "data": { "id": {{ data["id"] }} }
```

### Comparing `netbox_kea_dhcp-0.0.1a3/pyproject.toml` & `netbox_kea_dhcp-0.0.1a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `netbox_kea_dhcp-0.0.1a3/PKG-INFO` & `netbox_kea_dhcp-0.0.1a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-kea-dhcp
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: Use netbox as subnets source for ISC Kea DHCP server
 Project-URL: Homepage, https://github.com/francoismdj/netbox-kea-dhcp
 Author: francoismdj
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
@@ -120,16 +120,16 @@
   * `DCIM`: `Interface`, `Device`.
   * `Virtualization`: `Interface`, `Virtual Machine`.
 - Events: `Creations`, `Updates`, `Deletions`.
 - HTTP Request:
   * URL: `http://{netbox-connector-host}:{port}/event/{free-text}/`
   * HTTP Method: `POST`.
 
-The field `free-text` permits to define several webhooks with same events. The
-connector only uses it in logs.
+The field `free-text` is necessary to define several webhooks with same events.
+The connector only uses it in logs.
 
 More help with `netbox-kea-dhcp --help` and in the configuration file example
 under `examples/` (or under
 `~/.local/pipx/venvs/netbox-kea-dhcp/lib/python3.10/site-packages/examples/` if
 app was installed with pipx).
 
 Recommended Netbox webhooks
@@ -137,15 +137,15 @@
 
 It’s recommended to set several webhooks with conditions and restricted body
 template, in order to filter events and avoid unecessary network and CPU load:
 
 Common to all webhooks:
 
 - HTTP Request:
-  * URL: `http://{netbox-connector-host}:{port}/event/{optional-free-text}`
+  * URL: `http://{netbox-connector-host}:{port}/event/{optional-free-text}/`
   * HTTP Method: `POST`.
 - Body template:
 
     ```json
     { "event": "{{ event }}",
       "model": "{{ model }}",
       "data": { "id": {{ data["id"] }} }
```

