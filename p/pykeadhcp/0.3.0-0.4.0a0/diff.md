# Comparing `tmp/pykeadhcp-0.3.0.tar.gz` & `tmp/pykeadhcp-0.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykeadhcp-0.3.0.tar", max compression
+gzip compressed data, was "pykeadhcp-0.4.0a0.tar", max compression
```

## Comparing `pykeadhcp-0.3.0.tar` & `pykeadhcp-0.4.0a0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0    11356 2023-06-03 22:25:51.648940 pykeadhcp-0.3.0/LICENSE
--rw-r--r--   0        0        0     7331 2023-06-03 22:25:51.648940 pykeadhcp-0.3.0/README.md
--rw-r--r--   0        0        0       30 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/__init__.py
--rw-r--r--   0        0        0      174 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/daemons/__init__.py
--rw-r--r--   0        0        0     4508 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/daemons/ctrlagent.py
--rw-r--r--   0        0        0     4526 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/daemons/ddns.py
--rw-r--r--   0        0        0    25840 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/daemons/dhcp4.py
--rw-r--r--   0        0        0    22098 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/daemons/dhcp6.py
--rw-r--r--   0        0        0     2718 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/exceptions.py
--rw-r--r--   0        0        0     7934 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/kea.py
--rw-r--r--   0        0        0        0 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/__init__.py
--rw-r--r--   0        0        0        0 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/ctrlagent/__init__.py
--rw-r--r--   0        0        0      457 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/ctrlagent/config.py
--rw-r--r--   0        0        0        0 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp4/__init__.py
--rw-r--r--   0        0        0      331 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp4/client_class.py
--rw-r--r--   0        0        0      798 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp4/config.py
--rw-r--r--   0        0        0      212 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp4/lease.py
--rw-r--r--   0        0        0      303 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp4/reservation.py
--rw-r--r--   0        0        0      453 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp4/shared_network.py
--rw-r--r--   0        0        0      684 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp4/subnet.py
--rw-r--r--   0        0        0        0 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp6/__init__.py
--rw-r--r--   0        0        0      253 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp6/client_class.py
--rw-r--r--   0        0        0      922 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp6/config.py
--rw-r--r--   0        0        0      346 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp6/lease.py
--rw-r--r--   0        0        0      543 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp6/pd_pool.py
--rw-r--r--   0        0        0      212 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp6/reservation.py
--rw-r--r--   0        0        0      296 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp6/server_id.py
--rw-r--r--   0        0        0      380 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp6/shared_network.py
--rw-r--r--   0        0        0      501 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/dhcp6/subnet.py
--rw-r--r--   0        0        0     1550 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/enums.py
--rw-r--r--   0        0        0      169 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/__init__.py
--rw-r--r--   0        0        0      181 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/api_response.py
--rw-r--r--   0        0        0      477 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/authentication.py
--rw-r--r--   0        0        0      278 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/base.py
--rw-r--r--   0        0        0      403 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/client_class.py
--rw-r--r--   0        0        0     1499 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/config.py
--rw-r--r--   0        0        0      396 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/control_socket.py
--rw-r--r--   0        0        0     2458 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/daemon.py
--rw-r--r--   0        0        0      734 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/database.py
--rw-r--r--   0        0        0      399 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/dhcp_common.py
--rw-r--r--   0        0        0      873 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/dhcp_ddns.py
--rw-r--r--   0        0        0      158 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/dhcp_queue_control.py
--rw-r--r--   0        0        0      183 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/hook.py
--rw-r--r--   0        0        0      403 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/lease.py
--rw-r--r--   0        0        0      629 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/logger.py
--rw-r--r--   0        0        0      181 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/multi_threading.py
--rw-r--r--   0        0        0      364 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/option_data.py
--rw-r--r--   0        0        0      294 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/option_def.py
--rw-r--r--   0        0        0      411 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/pool.py
--rw-r--r--   0        0        0      141 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/relay.py
--rw-r--r--   0        0        0      484 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/reservation.py
--rw-r--r--   0        0        0      112 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/sanity_check.py
--rw-r--r--   0        0        0      175 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/shared_network.py
--rw-r--r--   0        0        0      249 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/sockets.py
--rw-r--r--   0        0        0      477 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/status.py
--rw-r--r--   0        0        0      390 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/models/generic/subnet.py
--rw-r--r--   0        0        0      152 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/parsers/__init__.py
--rw-r--r--   0        0        0      508 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/parsers/ctrlagent.py
--rw-r--r--   0        0        0        0 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/parsers/ddns.py
--rw-r--r--   0        0        0    17838 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/parsers/dhcp4.py
--rw-r--r--   0        0        0      522 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/parsers/dhcp6.py
--rw-r--r--   0        0        0     2915 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/parsers/exceptions.py
--rw-r--r--   0        0        0      825 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pykeadhcp/parsers/generic.py
--rw-r--r--   0        0        0      447 2023-06-03 22:25:51.652940 pykeadhcp-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7936 1970-01-01 00:00:00.000000 pykeadhcp-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-06-17 10:43:47.271062 pykeadhcp-0.4.0a0/LICENSE
+-rw-r--r--   0        0        0     7331 2023-06-17 10:43:47.271062 pykeadhcp-0.4.0a0/README.md
+-rw-r--r--   0        0        0       30 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/__init__.py
+-rw-r--r--   0        0        0      174 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/daemons/__init__.py
+-rw-r--r--   0        0        0     4508 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/daemons/ctrlagent.py
+-rw-r--r--   0        0        0     4526 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/daemons/ddns.py
+-rw-r--r--   0        0        0    25840 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/daemons/dhcp4.py
+-rw-r--r--   0        0        0    22098 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/daemons/dhcp6.py
+-rw-r--r--   0        0        0     2718 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/exceptions.py
+-rw-r--r--   0        0        0     8243 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/kea.py
+-rw-r--r--   0        0        0        0 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/ctrlagent/__init__.py
+-rw-r--r--   0        0        0      457 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/ctrlagent/config.py
+-rw-r--r--   0        0        0        0 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/dhcp4/__init__.py
+-rw-r--r--   0        0        0      331 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/dhcp4/client_class.py
+-rw-r--r--   0        0        0      798 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/dhcp4/config.py
+-rw-r--r--   0        0        0      212 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/dhcp4/lease.py
+-rw-r--r--   0        0        0      303 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/dhcp4/reservation.py
+-rw-r--r--   0        0        0      453 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/dhcp4/shared_network.py
+-rw-r--r--   0        0        0      684 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/dhcp4/subnet.py
+-rw-r--r--   0        0        0        0 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/dhcp6/__init__.py
+-rw-r--r--   0        0        0      253 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/dhcp6/client_class.py
+-rw-r--r--   0        0        0      922 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/dhcp6/config.py
+-rw-r--r--   0        0        0      346 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/dhcp6/lease.py
+-rw-r--r--   0        0        0      438 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/dhcp6/pd_pool.py
+-rw-r--r--   0        0        0      212 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/dhcp6/reservation.py
+-rw-r--r--   0        0        0      296 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/dhcp6/server_id.py
+-rw-r--r--   0        0        0      380 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/dhcp6/shared_network.py
+-rw-r--r--   0        0        0      501 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/dhcp6/subnet.py
+-rw-r--r--   0        0        0     1550 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/enums.py
+-rw-r--r--   0        0        0      169 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/api_response.py
+-rw-r--r--   0        0        0      477 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/authentication.py
+-rw-r--r--   0        0        0      435 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/base.py
+-rw-r--r--   0        0        0      403 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/client_class.py
+-rw-r--r--   0        0        0     1394 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/config.py
+-rw-r--r--   0        0        0      396 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/control_socket.py
+-rw-r--r--   0        0        0     2458 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/daemon.py
+-rw-r--r--   0        0        0      734 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/database.py
+-rw-r--r--   0        0        0      399 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/dhcp_common.py
+-rw-r--r--   0        0        0      873 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/dhcp_ddns.py
+-rw-r--r--   0        0        0      158 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/dhcp_queue_control.py
+-rw-r--r--   0        0        0      183 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/hook.py
+-rw-r--r--   0        0        0      403 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/lease.py
+-rw-r--r--   0        0        0      538 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/logger.py
+-rw-r--r--   0        0        0      181 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/multi_threading.py
+-rw-r--r--   0        0        0      259 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/option_data.py
+-rw-r--r--   0        0        0      294 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/option_def.py
+-rw-r--r--   0        0        0      306 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/pool.py
+-rw-r--r--   0        0        0      141 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/relay.py
+-rw-r--r--   0        0        0      379 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/reservation.py
+-rw-r--r--   0        0        0      112 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/sanity_check.py
+-rw-r--r--   0        0        0      175 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/shared_network.py
+-rw-r--r--   0        0        0      249 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/sockets.py
+-rw-r--r--   0        0        0      477 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/status.py
+-rw-r--r--   0        0        0      390 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/models/generic/subnet.py
+-rw-r--r--   0        0        0      152 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/parsers/__init__.py
+-rw-r--r--   0        0        0      508 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/parsers/ctrlagent.py
+-rw-r--r--   0        0        0        0 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/parsers/ddns.py
+-rw-r--r--   0        0        0    17838 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/parsers/dhcp4.py
+-rw-r--r--   0        0        0    20361 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/parsers/dhcp6.py
+-rw-r--r--   0        0        0     3436 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/parsers/exceptions.py
+-rw-r--r--   0        0        0      825 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pykeadhcp/parsers/generic.py
+-rw-r--r--   0        0        0      449 2023-06-17 10:43:47.275062 pykeadhcp-0.4.0a0/pyproject.toml
+-rw-r--r--   0        0        0     7938 1970-01-01 00:00:00.000000 pykeadhcp-0.4.0a0/PKG-INFO
```

### Comparing `pykeadhcp-0.3.0/LICENSE` & `pykeadhcp-0.4.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.3.0/README.md` & `pykeadhcp-0.4.0a0/README.md`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.3.0/pykeadhcp/daemons/ctrlagent.py` & `pykeadhcp-0.4.0a0/pykeadhcp/daemons/ctrlagent.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.3.0/pykeadhcp/daemons/ddns.py` & `pykeadhcp-0.4.0a0/pykeadhcp/daemons/ddns.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.3.0/pykeadhcp/daemons/dhcp4.py` & `pykeadhcp-0.4.0a0/pykeadhcp/daemons/dhcp4.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.3.0/pykeadhcp/daemons/dhcp6.py` & `pykeadhcp-0.4.0a0/pykeadhcp/daemons/dhcp6.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.3.0/pykeadhcp/exceptions.py` & `pykeadhcp-0.4.0a0/pykeadhcp/exceptions.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.3.0/pykeadhcp/kea.py` & `pykeadhcp-0.4.0a0/pykeadhcp/kea.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 from requests.auth import HTTPBasicAuth
 from requests.exceptions import HTTPError
 from pathlib import Path
-from typing import List
+from typing import List, Union
 
 from pykeadhcp.daemons import CtrlAgent, Ddns, Dhcp4, Dhcp6
 from pykeadhcp.models.generic import KeaResponse
 from pykeadhcp.models.generic.hook import Hook
 from pykeadhcp.exceptions import (
     KeaGenericException,
     KeaCommandNotSupportedException,
@@ -28,34 +28,38 @@
         use_basic_auth:         Use HTTP Basic Auth if Kea is configured for it
         username:               Username for HTTP Basic Auth
         password:               Password for HTTP Basic Auth
         raise_generic_errors:   If True, it will raise a generic error based on Kea Documentation
             (as per self.RESPONSE_CODES). Set this to False if you want to catch the API endpoint specific
             errors such as `v4 Shared Network not found` vs `Code 3: the requested operation has been completed but the requested resource was not found.
             This status code is returned when a command returns no resources or affects no resources.`
+        verify:                 Boolean is used if the server TLS cert is verified or not, however you can
+            pass in a string which should be a path to a CA bundle to use with each request.
     """
 
     def __init__(
         self,
         host: str,
         port: int,
         headers: dict = {"Content-Type": "application/json"},
         use_basic_auth: bool = False,
         username: str = "",
         password: str = "",
         raise_generic_errors: bool = False,
+        verify: Union[bool, str] = True,
     ):
         self.host = host
         self.port = port
         self.headers = headers
         self.use_basic_auth = use_basic_auth
         self.basic_auth = HTTPBasicAuth(username, password)
         self.services = ["dhcp4", "dhcp6", "ddns", None]  # None = Control-Agent Daemon
         self.url = f"{self.host}:{self.port}"
         self.raise_generic_errors = raise_generic_errors
+        self.verify = verify
         self.RESPONSE_CODES = {
             1: KeaGenericException,
             2: KeaCommandNotSupportedException,
             3: KeaObjectNotFoundException,
             4: KeaServerConflictException,
         }
         self.hook_library = {}
@@ -118,14 +122,15 @@
         """
         url = self.url + endpoint
         response = requests.post(
             url=url,
             json=body,
             headers=self.headers,
             auth=self.basic_auth if self.use_basic_auth else None,
+            verify=self.verify,
             **kwargs,
         )
 
         if response.status_code == 401:
             raise KeaUnauthorizedAccessException
 
         if response.status_code >= 400 and response.status_code <= 500:
```

### Comparing `pykeadhcp-0.3.0/pykeadhcp/models/dhcp4/config.py` & `pykeadhcp-0.4.0a0/pykeadhcp/models/dhcp4/config.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.3.0/pykeadhcp/models/dhcp4/subnet.py` & `pykeadhcp-0.4.0a0/pykeadhcp/models/dhcp4/subnet.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.3.0/pykeadhcp/models/dhcp6/config.py` & `pykeadhcp-0.4.0a0/pykeadhcp/models/dhcp6/config.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.3.0/pykeadhcp/models/enums.py` & `pykeadhcp-0.4.0a0/pykeadhcp/models/enums.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.3.0/pykeadhcp/models/generic/config.py` & `pykeadhcp-0.4.0a0/pykeadhcp/models/generic/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 from typing import Optional, List, Union
-from pykeadhcp.models.generic.base import KeaBaseModel
+from pykeadhcp.models.generic.base import KeaModel
 from pykeadhcp.models.generic.hook import Hook
 from pykeadhcp.models.generic.logger import Logger
 from pykeadhcp.models.generic.option_data import OptionData
 from pykeadhcp.models.enums import ReservationMode, DDNSReplaceClientNameEnum
 
 
-class CommonConfig(KeaBaseModel):
+class CommonConfig(KeaModel):
     store_extended_info: Optional[bool]
-    user_context: Optional[dict]
-    comment: Optional[str]
-    unknown_map_entry: Optional[str]
 
 
 class CommonDhcpConfig(CommonConfig):
     valid_lifetime: Optional[int]
     min_valid_lifetime: Optional[int]
     max_valid_lifetime: Optional[int]
     renew_timer: Optional[int]
```

### Comparing `pykeadhcp-0.3.0/pykeadhcp/models/generic/daemon.py` & `pykeadhcp-0.4.0a0/pykeadhcp/models/generic/daemon.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.3.0/pykeadhcp/models/generic/database.py` & `pykeadhcp-0.4.0a0/pykeadhcp/models/generic/database.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.3.0/pykeadhcp/models/generic/dhcp_ddns.py` & `pykeadhcp-0.4.0a0/pykeadhcp/models/generic/dhcp_ddns.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.3.0/pykeadhcp/models/generic/logger.py` & `pykeadhcp-0.4.0a0/pykeadhcp/models/generic/logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 from typing import Optional, List
 from pydantic import conint
-from pykeadhcp.models.generic.base import KeaBaseModel
+from pykeadhcp.models.generic.base import KeaBaseModel, KeaModel
 from pykeadhcp.models.enums import LoggerLevelEnum
 
 
 class Output(KeaBaseModel):
     output: str
     flush: bool
     maxsize: int
     maxver: int
     pattern: Optional[str]
 
 
-class Logger(KeaBaseModel):
+class Logger(KeaModel):
     name: str
     output_options: Optional[List[Output]] = []
     debuglevel: conint(ge=0, le=100)
     severity: Optional[LoggerLevelEnum]
-    user_context: Optional[dict]
-    comment: Optional[str]
-    unknown_map_entry: Optional[str]
 
     class Config:
         fields = {"output_options": "output_options"}
```

### Comparing `pykeadhcp-0.3.0/pykeadhcp/parsers/dhcp4.py` & `pykeadhcp-0.4.0a0/pykeadhcp/parsers/dhcp4.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.3.0/pykeadhcp/parsers/exceptions.py` & `pykeadhcp-0.4.0a0/pykeadhcp/parsers/exceptions.py`

 * *Files 27% similar despite different names*

```diff
@@ -76,7 +76,21 @@
         super().__init__(self.message)
 
 
 class ParserInvalidHostReservationIdentifierError(GenericParserError):
     def __init__(self, identifier_type: str):
         self.message = f"Identifier Typer {identifier_type} is not a valid type"
         super().__init__(self.message)
+
+
+class ParserPDPoolAlreadyExistError(GenericParserError):
+    def __init__(self, prefix: str, prefix_len: int, id: int):
+        self.message = (
+            f"PD Prefix {prefix}/{prefix_len} already exist in a subnet ({id})"
+        )
+        super().__init__(self.message)
+
+
+class ParserPDPoolNotFoundError(GenericParserError):
+    def __init__(self, id: int, prefix: str, prefix_len: int):
+        self.message = f"Unable to find PD Prefix {prefix}/{prefix_len} in subnet {id}"
+        super().__init__(self.message)
```

### Comparing `pykeadhcp-0.3.0/pykeadhcp/parsers/generic.py` & `pykeadhcp-0.4.0a0/pykeadhcp/parsers/generic.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.3.0/PKG-INFO` & `pykeadhcp-0.4.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykeadhcp
-Version: 0.3.0
+Version: 0.4.0a0
 Summary: Wrapper around requests module to query ISC Kea DHCP API Daemons (ctrlagent, dhcp4, dhcp6, ddns)
 License: Apache 2.0
 Author: Brandon Spendlove
 Author-email: brandon-spendlove@hotmail.co.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

