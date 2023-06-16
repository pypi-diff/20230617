# Comparing `tmp/flwr_nightly-1.5.0.dev20230615.tar.gz` & `tmp/flwr_nightly-1.5.0.dev20230616.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.5.0.dev20230615.tar", max compression
+gzip compressed data, was "flwr_nightly-1.5.0.dev20230616.tar", max compression
```

## Comparing `flwr_nightly-1.5.0.dev20230615.tar` & `flwr_nightly-1.5.0.dev20230616.tar`

### file list

```diff
@@ -1,113 +1,113 @@
--rw-r--r--   0        0        0    11358 2023-06-15 23:02:37.008046 flwr_nightly-1.5.0.dev20230615/LICENSE
--rw-r--r--   0        0        0    10363 2023-06-15 23:02:37.008046 flwr_nightly-1.5.0.dev20230615/README.md
--rw-r--r--   0        0        0     4397 2023-06-15 23:03:01.168183 flwr_nightly-1.5.0.dev20230615/pyproject.toml
--rw-r--r--   0        0        0      952 2023-06-15 23:02:37.296047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/__init__.py
--rw-r--r--   0        0        0     1164 2023-06-15 23:02:37.296047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    13835 2023-06-15 23:02:37.296047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     7677 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     7209 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      728 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     4293 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      745 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     5474 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0      712 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     5077 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1685 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     5318 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      728 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0     8333 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0     2877 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1875 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     1113 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0      884 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     1791 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     1889 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     3482 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0     2120 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0    16315 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7805 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     3714 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      848 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      809 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/driver/__init__.py
--rw-r--r--   0        0        0     4826 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/driver/app.py
--rw-r--r--   0        0        0     3906 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/driver/driver.py
--rw-r--r--   0        0        0     4877 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/driver/driver_client_manager.py
--rw-r--r--   0        0        0     5653 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/driver/driver_client_proxy.py
--rw-r--r--   0        0        0      676 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     4663 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     3815 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     5727 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     1617 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     4982 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     4554 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0     4275 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     1495 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1188 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     8232 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0    10889 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0    18721 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1370 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    26335 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     6120 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2227 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0     1054 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      705 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     3919 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/driver/driver_servicer.py
--rw-r--r--   0        0        0      704 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/__init__.py
--rw-r--r--   0        0        0      728 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     4467 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py
--rw-r--r--   0        0        0     5686 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6408 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4650 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11501 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0     6313 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py
--rw-r--r--   0        0        0      751 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     1858 2023-06-15 23:02:37.300047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0      724 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     2024 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      728 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     3718 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0     4897 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/history.py
--rw-r--r--   0        0        0    15958 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/server.py
--rw-r--r--   0        0        0      996 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/state/__init__.py
--rw-r--r--   0        0        0     6774 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/state/in_memory_state.py
--rw-r--r--   0        0        0    19296 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/state/sqlite_state.py
--rw-r--r--   0        0        0     4833 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/state/state.py
--rw-r--r--   0        0        0     1647 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/state/state_factory.py
--rw-r--r--   0        0        0     1667 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0     6099 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     4591 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     6932 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5830 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6722 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     7004 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11479 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9969 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8244 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2666 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5385 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     7057 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     5916 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     3368 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     7036 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6302 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10131 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7484 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      901 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5069 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     4940 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0     1271 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0     7826 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      727 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0     5535 2023-06-15 23:02:37.304047 flwr_nightly-1.5.0.dev20230615/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0    12494 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230615/setup.py
--rw-r--r--   0        0        0    12838 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230615/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-16 23:02:50.368907 flwr_nightly-1.5.0.dev20230616/LICENSE
+-rw-r--r--   0        0        0    10363 2023-06-16 23:02:50.368907 flwr_nightly-1.5.0.dev20230616/README.md
+-rw-r--r--   0        0        0     4840 2023-06-16 23:03:18.939159 flwr_nightly-1.5.0.dev20230616/pyproject.toml
+-rw-r--r--   0        0        0      952 2023-06-16 23:02:50.668907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0     1164 2023-06-16 23:02:50.668907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    13835 2023-06-16 23:02:50.668907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     7677 2023-06-16 23:02:50.668907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     7209 2023-06-16 23:02:50.668907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      728 2023-06-16 23:02:50.668907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     4293 2023-06-16 23:02:50.668907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      745 2023-06-16 23:02:50.668907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     5474 2023-06-16 23:02:50.668907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0      712 2023-06-16 23:02:50.668907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     5077 2023-06-16 23:02:50.668907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1685 2023-06-16 23:02:50.668907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     5318 2023-06-16 23:02:50.668907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      728 2023-06-16 23:02:50.668907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0     8333 2023-06-16 23:02:50.668907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0     2877 2023-06-16 23:02:50.668907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1875 2023-06-16 23:02:50.668907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     1113 2023-06-16 23:02:50.668907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0      884 2023-06-16 23:02:50.668907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     1791 2023-06-16 23:02:50.668907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     1889 2023-06-16 23:02:50.668907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     3482 2023-06-16 23:02:50.668907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0     2120 2023-06-16 23:02:50.668907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0    16315 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7805 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     3714 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      848 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      809 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/driver/__init__.py
+-rw-r--r--   0        0        0     4826 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/driver/app.py
+-rw-r--r--   0        0        0     3906 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/driver/driver.py
+-rw-r--r--   0        0        0     4877 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/driver/driver_client_manager.py
+-rw-r--r--   0        0        0     5653 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/driver/driver_client_proxy.py
+-rw-r--r--   0        0        0      676 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     4663 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     3815 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     5727 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     1617 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4982 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     4554 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0     4275 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     1495 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1188 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8232 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0    10889 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0    18721 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1370 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    26335 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     6120 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2227 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0     1054 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      705 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     3919 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/driver/driver_servicer.py
+-rw-r--r--   0        0        0      704 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/__init__.py
+-rw-r--r--   0        0        0      728 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     4467 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py
+-rw-r--r--   0        0        0     5686 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6408 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4650 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11501 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0     6313 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py
+-rw-r--r--   0        0        0      751 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     1858 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0      724 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     2024 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      728 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     3718 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0     4897 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0    15958 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0      996 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/state/__init__.py
+-rw-r--r--   0        0        0     6774 2023-06-16 23:02:50.672907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/state/in_memory_state.py
+-rw-r--r--   0        0        0    19296 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/state/sqlite_state.py
+-rw-r--r--   0        0        0     4833 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/state/state.py
+-rw-r--r--   0        0        0     1647 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/state/state_factory.py
+-rw-r--r--   0        0        0     1667 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0     6099 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     4654 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     6995 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5893 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6740 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     7014 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11522 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9991 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8286 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2708 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5428 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     7126 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     6026 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     3519 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     7079 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6343 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10154 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7484 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      901 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5069 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     4940 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0     1271 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0     7826 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      727 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0     5535 2023-06-16 23:02:50.676907 flwr_nightly-1.5.0.dev20230616/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0    12494 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230616/setup.py
+-rw-r--r--   0        0        0    12838 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230616/PKG-INFO
```

### Comparing `flwr_nightly-1.5.0.dev20230615/LICENSE` & `flwr_nightly-1.5.0.dev20230616/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/README.md` & `flwr_nightly-1.5.0.dev20230616/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/pyproject.toml` & `flwr_nightly-1.5.0.dev20230616/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.5.0-dev20230615"
+version = "1.5.0-dev20230616"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.dev>"]
 readme = "README.md"
 homepage = "https://flower.dev"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.dev"
@@ -94,14 +94,15 @@
 sphinx-design = "==0.4.1"
 sphinx-copybutton = "==0.5.2"
 sphinxcontrib-mermaid = "==0.8.1"
 furo = "==2022.12.7"
 sphinx-reredirects = "==0.1.2"
 nbsphinx = "==0.9.2"
 nbstripout = "==0.6.1"
+ruff = "==0.0.272"
 sphinx-argparse = "==0.4.0"
 pipreqs = "==0.4.13"
 
 [tool.isort]
 line_length = 88
 indent = "    "
 multi_line_output = 3
@@ -152,7 +153,39 @@
 module = "torch.*"
 follow_imports = "skip"
 follow_imports_for_stubs = true
 
 [tool.docformatter]
 wrap-summaries = 88
 wrap-descriptions = 88
+
+[tool.ruff]
+line-length = 88
+select = ["D"]
+fixable = ["D"]
+
+exclude = [
+    ".bzr",
+    ".direnv",
+    ".eggs",
+    ".git",
+    ".hg",
+    ".mypy_cache",
+    ".nox",
+    ".pants.d",
+    ".pytype",
+    ".ruff_cache",
+    ".svn",
+    ".tox",
+    ".venv",
+    "__pypackages__",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+    "node_modules",
+    "venv",
+    "proto",
+]
+
+[tool.ruff.pydocstyle]
+convention = "numpy"
```

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/__init__.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/__init__.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/app.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/client.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/grpc_rere_client/connection.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/grpc_rere_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/client/rest_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/__init__.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/address.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/constant.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/constant.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 Extra dependencies required for using the REST-based Fleet API are missing.
 
 To use the REST API, install `flwr` with the `rest` extra:
 
     `pip install flwr[rest]`.
 """
 
-TRANSPORT_TYPE_GRPC_BIDI = "grpc-bido"
+TRANSPORT_TYPE_GRPC_BIDI = "grpc-bidi"
 TRANSPORT_TYPE_GRPC_RERE = "grpc-rere"
 TRANSPORT_TYPE_REST = "rest"
 TRANSPORT_TYPES = [
     TRANSPORT_TYPE_GRPC_BIDI,
     TRANSPORT_TYPE_GRPC_RERE,
     TRANSPORT_TYPE_REST,
 ]
```

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/date.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/dp.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/grpc.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/logger.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/parameter.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/serde.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/typing.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/common/version.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/driver/__init__.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/driver/app.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/driver/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/driver/driver.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/driver/driver_client_manager.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/driver/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/driver/driver_client_proxy.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/driver/driver_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/__init__.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/app.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/criterion.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/driver/driver_servicer.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/__init__.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/message_handler/__init__.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/message_handler/message_handler.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/rest_rere/__init__.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/fleet/rest_rere/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/history.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/server.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/state/__init__.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/state/in_memory_state.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/state/sqlite_state.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/state/sqlite_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/state/state.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/state/state_factory.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 
         if noise_multiplier:
             self.noise_multiplier = (
                 self.noise_multiplier ** (-2) - (2 * self.clip_count_stddev) ** (-2)
             ) ** (-0.5)
 
     def __repr__(self) -> str:
+        """Compute a string representation of the strategy."""
         rep = "Strategy with DP with Adaptive Clipping enabled."
         return rep
 
     def configure_fit(
         self, server_round: int, parameters: Parameters, client_manager: ClientManager
     ) -> List[Tuple[ClientProxy, FitIns]]:
         """Configure the next round of training."""
```

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         if noise_multiplier < 0:
             raise Exception("The noise multiplier should be a non-negative value.")
         self.noise_multiplier = noise_multiplier
 
         self.server_side_noising = server_side_noising
 
     def __repr__(self) -> str:
+        """Compute a string representation of the strategy."""
         rep = "Strategy with DP with Fixed Clipping enabled."
         return rep
 
     def _calc_client_noise_stddev(self) -> float:
         return float(
             self.noise_multiplier * self.clip_norm / (self.num_sampled_clients ** (0.5))
         )
```

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
             fit_metrics_aggregation_fn=fit_metrics_aggregation_fn,
             evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
         )
         self.completion_rate_fit = min_completion_rate_fit
         self.completion_rate_evaluate = min_completion_rate_evaluate
 
     def __repr__(self) -> str:
+        """Compute a string representation of the strategy."""
         return "FaultTolerantFedAvg()"
 
     def aggregate_fit(
         self,
         server_round: int,
         results: List[Tuple[ClientProxy, FitRes]],
         failures: List[Union[Tuple[ClientProxy, FitRes], BaseException]],
```

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Adaptive Federated Optimization using Adagrad (FedAdagrad) [Reddi et al., 2020]
-strategy.
+"""FedAdagrad [Reddi et al., 2020] strategy.
+
+Adaptive Federated Optimization using Adagrad.
 
 Paper: arxiv.org/abs/2003.00295
 """
 
 
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
@@ -33,23 +34,21 @@
     parameters_to_ndarrays,
 )
 from flwr.server.client_proxy import ClientProxy
 
 from .fedopt import FedOpt
 
 
-# flake8: noqa: E501
 class FedAdagrad(FedOpt):
-    """Adaptive Federated Optimization using Adagrad (FedAdagrad) [Reddi et al., 2020]
-    strategy.
+    """FedAdagrad strategy - Adaptive Federated Optimization using Adagrad.
 
     Paper: https://arxiv.org/abs/2003.00295
     """
 
-    # pylint: disable=too-many-arguments,too-many-locals,too-many-instance-attributes,line-too-long
+    # pylint: disable=too-many-arguments,too-many-locals,too-many-instance-attributes, line-too-long
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
@@ -124,14 +123,15 @@
             eta_l=eta_l,
             beta_1=0.0,
             beta_2=0.0,
             tau=tau,
         )
 
     def __repr__(self) -> str:
+        """Compute a string representation of the strategy."""
         rep = f"FedAdagrad(accept_failures={self.accept_failures})"
         return rep
 
     def aggregate_fit(
         self,
         server_round: int,
         results: List[Tuple[ClientProxy, FitRes]],
```

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fedadam.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Adaptive Federated Optimization using Adam (FedAdam) [Reddi et al., 2020] strategy.
+"""Adaptive Federated Optimization using Adam (FedAdam) strategy.
+
+[Reddi et al., 2020]
 
 Paper: arxiv.org/abs/2003.00295
 """
 
 
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
@@ -32,23 +34,21 @@
     parameters_to_ndarrays,
 )
 from flwr.server.client_proxy import ClientProxy
 
 from .fedopt import FedOpt
 
 
-# flake8: noqa: E501
 class FedAdam(FedOpt):
-    """Adaptive Federated Optimization using Adam (FedAdam) [Reddi et al., 2020]
-    strategy.
+    """FedAdam - Adaptive Federated Optimization using Adam.
 
     Paper: https://arxiv.org/abs/2003.00295
     """
 
-    # pylint: disable=too-many-arguments,too-many-instance-attributes,too-many-locals,line-too-long
+    # pylint: disable=too-many-arguments,too-many-instance-attributes,too-many-locals, line-too-long
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
@@ -129,14 +129,15 @@
             eta_l=eta_l,
             beta_1=beta_1,
             beta_2=beta_2,
             tau=tau,
         )
 
     def __repr__(self) -> str:
+        """Compute a string representation of the strategy."""
         rep = f"FedAdam(accept_failures={self.accept_failures})"
         return rep
 
     def aggregate_fit(
         self,
         server_round: int,
         results: List[Tuple[ClientProxy, FitRes]],
```

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fedavg.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,19 +44,18 @@
 Setting `min_available_clients` lower than `min_fit_clients` or
 `min_evaluate_clients` can cause the server to fail when there are too few clients
 connected to the server. `min_available_clients` must be set to a value larger
 than or equal to the values of `min_fit_clients` and `min_evaluate_clients`.
 """
 
 
-# flake8: noqa: E501
 class FedAvg(Strategy):
     """Configurable FedAvg strategy implementation."""
 
-    # pylint: disable=too-many-arguments,too-many-instance-attributes,line-too-long
+    # pylint: disable=too-many-arguments,too-many-instance-attributes, line-too-long
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
@@ -82,16 +81,16 @@
         ----------
         fraction_fit : float, optional
             Fraction of clients used during training. In case `min_fit_clients`
             is larger than `fraction_fit * available_clients`, `min_fit_clients`
             will still be sampled. Defaults to 1.0.
         fraction_evaluate : float, optional
             Fraction of clients used during validation. In case `min_evaluate_clients`
-            is larger than `fraction_evaluate * available_clients`, `min_evaluate_clients`
-            will still be sampled. Defaults to 1.0.
+            is larger than `fraction_evaluate * available_clients`,
+            `min_evaluate_clients` will still be sampled. Defaults to 1.0.
         min_fit_clients : int, optional
             Minimum number of clients used during training. Defaults to 2.
         min_evaluate_clients : int, optional
             Minimum number of clients used during validation. Defaults to 2.
         min_available_clients : int, optional
             Minimum number of total clients in the system. Defaults to 2.
         evaluate_fn : Optional[Callable[[int, NDArrays, Dict[str, Scalar]], Optional[Tuple[float, Dict[str, Scalar]]]]]
@@ -127,14 +126,15 @@
         self.on_evaluate_config_fn = on_evaluate_config_fn
         self.accept_failures = accept_failures
         self.initial_parameters = initial_parameters
         self.fit_metrics_aggregation_fn = fit_metrics_aggregation_fn
         self.evaluate_metrics_aggregation_fn = evaluate_metrics_aggregation_fn
 
     def __repr__(self) -> str:
+        """Compute a string representation of the strategy."""
         rep = f"FedAvg(accept_failures={self.accept_failures})"
         return rep
 
     def num_fit_clients(self, num_available_clients: int) -> Tuple[int, int]:
         """Return the sample size and the required number of available clients."""
         num_clients = int(num_available_clients * self.fraction_fit)
         return max(num_clients, self.min_fit_clients), self.min_available_clients
```

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Federated Averaging (FedAvg) [McMahan et al., 2016] strategy with custom
-serialization for Android devices.
+"""FedAvg [McMahan et al., 2016] strategy with custom serialization for Android devices.
 
 Paper: arxiv.org/abs/1602.05629
 """
 
 
 from typing import Callable, Dict, List, Optional, Tuple, Union, cast
 
@@ -36,19 +35,18 @@
 from flwr.server.client_manager import ClientManager
 from flwr.server.client_proxy import ClientProxy
 
 from .aggregate import aggregate, weighted_loss_avg
 from .strategy import Strategy
 
 
-# flake8: noqa: E501
 class FedAvgAndroid(Strategy):
     """Configurable FedAvg strategy implementation."""
 
-    # pylint: disable=too-many-arguments,too-many-instance-attributes,line-too-long
+    # pylint: disable=too-many-arguments,too-many-instance-attributes, line-too-long
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
@@ -76,15 +74,15 @@
             Fraction of clients used during validation. Defaults to 0.1.
         min_fit_clients : Optional[int]
             Minimum number of clients used during training. Defaults to 2.
         min_evaluate_clients : Optional[int]
             Minimum number of clients used during validation. Defaults to 2.
         min_available_clients : Optional[int]
             Minimum number of total clients in the system. Defaults to 2.
-        evaluate_fn : Optional[Callable[[int, NDArrays, Dict[str, Scalar]],Optional[Tuple[float, Dict[str, Scalar]]]]]
+        evaluate_fn : Optional[Callable[[int, NDArrays, Dict[str, Scalar]], Optional[Tuple[float, Dict[str, Scalar]]]]]
             Optional function used for validation. Defaults to None.
         on_fit_config_fn : Optional[Callable[[int], Dict[str, Scalar]]]
             Function used to configure training. Defaults to None.
         on_evaluate_config_fn : Optional[Callable[[int], Dict[str, Scalar]]]
             Function used to configure validation. Defaults to None.
         accept_failures : Optional[bool]
             Whether or not accept rounds
@@ -101,14 +99,15 @@
         self.evaluate_fn = evaluate_fn
         self.on_fit_config_fn = on_fit_config_fn
         self.on_evaluate_config_fn = on_evaluate_config_fn
         self.accept_failures = accept_failures
         self.initial_parameters = initial_parameters
 
     def __repr__(self) -> str:
+        """Compute a string representation of the strategy."""
         rep = f"FedAvg(accept_failures={self.accept_failures})"
         return rep
 
     def num_fit_clients(self, num_available_clients: int) -> Tuple[int, int]:
         """Return the sample size and the required number of available clients."""
         num_clients = int(num_available_clients * self.fraction_fit)
         return max(num_clients, self.min_fit_clients), self.min_available_clients
```

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fedavgm.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,19 +34,18 @@
 from flwr.server.client_manager import ClientManager
 from flwr.server.client_proxy import ClientProxy
 
 from .aggregate import aggregate
 from .fedavg import FedAvg
 
 
-# flake8: noqa: E501
 class FedAvgM(FedAvg):
     """Configurable FedAvg with Momentum strategy implementation."""
 
-    # pylint: disable=too-many-arguments,too-many-instance-attributes,line-too-long
+    # pylint: disable=too-many-arguments,too-many-instance-attributes, line-too-long
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
@@ -94,15 +93,14 @@
             Initial global model parameters.
         server_learning_rate: float
             Server-side learning rate used in server-side optimization.
             Defaults to 1.0.
         server_momentum: float
             Server-side momentum factor used for FedAvgM. Defaults to 0.0.
         """
-
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
             evaluate_fn=evaluate_fn,
@@ -117,14 +115,15 @@
         self.server_momentum = server_momentum
         self.server_opt: bool = (self.server_momentum != 0.0) or (
             self.server_learning_rate != 1.0
         )
         self.momentum_vector: Optional[NDArrays] = None
 
     def __repr__(self) -> str:
+        """Compute a string representation of the strategy."""
         rep = f"FedAvgM(accept_failures={self.accept_failures})"
         return rep
 
     def initialize_parameters(
         self, client_manager: ClientManager
     ) -> Optional[Parameters]:
         """Initialize global model parameters."""
```

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fedmedian.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 from flwr.common.logger import log
 from flwr.server.client_proxy import ClientProxy
 
 from .aggregate import aggregate_median
 from .fedavg import FedAvg
 
 
-# flake8: noqa: E501
 class FedMedian(FedAvg):
     """Configurable FedAvg with Momentum strategy implementation."""
 
     def __repr__(self) -> str:
+        """Compute a string representation of the strategy."""
         rep = f"FedMedian(accept_failures={self.accept_failures})"
         return rep
 
     def aggregate_fit(
         self,
         server_round: int,
         results: List[Tuple[ClientProxy, FitRes]],
```

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fedopt.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,18 @@
     Scalar,
     parameters_to_ndarrays,
 )
 
 from .fedavg import FedAvg
 
 
-# flake8: noqa: E501
 class FedOpt(FedAvg):
     """Configurable FedAdagrad strategy implementation."""
 
-    # pylint: disable=too-many-arguments,too-many-instance-attributes,too-many-locals,line-too-long
+    # pylint: disable=too-many-arguments,too-many-instance-attributes,too-many-locals, line-too-long
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
@@ -123,9 +122,10 @@
         self.tau = tau
         self.beta_1 = beta_1
         self.beta_2 = beta_2
         self.m_t: Optional[NDArrays] = None
         self.v_t: Optional[NDArrays] = None
 
     def __repr__(self) -> str:
+        """Compute a string representation of the strategy."""
         rep = f"FedOpt(accept_failures={self.accept_failures})"
         return rep
```

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fedprox.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,19 +23,18 @@
 from flwr.common import FitIns, MetricsAggregationFn, NDArrays, Parameters, Scalar
 from flwr.server.client_manager import ClientManager
 from flwr.server.client_proxy import ClientProxy
 
 from .fedavg import FedAvg
 
 
-# flake8: noqa: E501
 class FedProx(FedAvg):
     """Configurable FedProx strategy implementation."""
 
-    # pylint: disable=too-many-arguments,too-many-instance-attributes,line-too-long
+    # pylint: disable=too-many-arguments,too-many-instance-attributes, line-too-long
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
@@ -50,57 +49,60 @@
         on_evaluate_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
         accept_failures: bool = True,
         initial_parameters: Optional[Parameters] = None,
         fit_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
         evaluate_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
         proximal_mu: float,
     ) -> None:
-        """Federated Optimization strategy.
+        r"""Federated Optimization strategy.
 
         Implementation based on https://arxiv.org/abs/1812.06127
 
-        The strategy in itself will not be different than FedAvg, the client needs to be adjusted.
+        The strategy in itself will not be different than FedAvg, the client needs to
+        be adjusted.
         A proximal term needs to be added to the loss function during the training:
 
         .. math::
             \\frac{\\mu}{2} || w - w^t ||^2
 
-        Where $w^t$ are the global parameters and $w$ are the local weights the function will
-        be optimized with.
+        Where $w^t$ are the global parameters and $w$ are the local weights the function
+        will be optimized with.
 
         In PyTorch, for example, the loss would go from:
 
         .. code:: python
 
           loss = criterion(net(inputs), labels)
 
         To:
 
         .. code:: python
 
           for local_weights, global_weights in zip(net.parameters(), global_params):
               proximal_term += (local_weights - global_weights).norm(2)
-          loss = criterion(net(inputs), labels) + (config["proximal_mu"] / 2) * proximal_term
+          loss = criterion(net(inputs), labels) + (config["proximal_mu"] / 2) *
+          proximal_term
 
-        With `global_params` being a copy of the parameters before the training takes place.
+        With `global_params` being a copy of the parameters before the training takes
+        place.
 
         .. code:: python
 
           global_params = copy.deepcopy(net).parameters()
 
         Parameters
         ----------
         fraction_fit : float, optional
             Fraction of clients used during training. In case `min_fit_clients`
             is larger than `fraction_fit * available_clients`, `min_fit_clients`
             will still be sampled. Defaults to 1.0.
         fraction_evaluate : float, optional
             Fraction of clients used during validation. In case `min_evaluate_clients`
-            is larger than `fraction_evaluate * available_clients`, `min_evaluate_clients`
-            will still be sampled. Defaults to 1.0.
+            is larger than `fraction_evaluate * available_clients`,
+            `min_evaluate_clients` will still be sampled. Defaults to 1.0.
         min_fit_clients : int, optional
             Minimum number of clients used during training. Defaults to 2.
         min_evaluate_clients : int, optional
             Minimum number of clients used during validation. Defaults to 2.
         min_available_clients : int, optional
             Minimum number of total clients in the system. Defaults to 2.
         evaluate_fn : Optional[Callable[[int, NDArrays, Dict[str, Scalar]], Optional[Tuple[float, Dict[str, Scalar]]]]]
@@ -119,15 +121,14 @@
             Metrics aggregation function, optional.
         proximal_mu : float
             The weight of the proximal term used in the optimization. 0.0 makes
             this strategy equivalent to FedAvg, and the higher the coefficient, the more
             regularization will be used (that is, the client parameters will need to be
             closer to the server parameters during training).
         """
-
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
             evaluate_fn=evaluate_fn,
@@ -137,14 +138,15 @@
             initial_parameters=initial_parameters,
             fit_metrics_aggregation_fn=fit_metrics_aggregation_fn,
             evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
         )
         self.proximal_mu = proximal_mu
 
     def __repr__(self) -> str:
+        """Compute a string representation of the strategy."""
         rep = f"FedProx(accept_failures={self.accept_failures})"
         return rep
 
     def configure_fit(
         self, server_round: int, parameters: Parameters, client_manager: ClientManager
     ) -> List[Tuple[ClientProxy, FitIns]]:
         """Configure the next round of training.
```

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Federated Averaging with Trimmed Mean [Dong Yin, et al., 2021]
+"""Federated Averaging with Trimmed Mean [Dong Yin, et al., 2021].
 
 Paper: arxiv.org/abs/1803.01498
 """
 from logging import WARNING
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
 from flwr.common import (
@@ -31,22 +31,21 @@
 from flwr.common.logger import log
 from flwr.server.client_proxy import ClientProxy
 
 from .aggregate import aggregate_trimmed_avg
 from .fedavg import FedAvg
 
 
-# flake8: noqa: E501
 class FedTrimmedAvg(FedAvg):
-    """Federated Averaging with Trimmed Mean [Dong Yin, et al., 2021]
+    """Federated Averaging with Trimmed Mean [Dong Yin, et al., 2021].
 
     Paper: https://arxiv.org/abs/1803.01498
     """
 
-    # pylint: disable=too-many-arguments,too-many-instance-attributes
+    # pylint: disable=too-many-arguments,too-many-instance-attributes, line-too-long
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
@@ -61,42 +60,41 @@
         on_evaluate_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
         accept_failures: bool = True,
         initial_parameters: Optional[Parameters] = None,
         fit_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
         evaluate_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
         beta: float = 0.2,
     ) -> None:
-        """
+        """Federated Averaging with Trimmed Mean [Dong Yin, et al., 2021].
+
         Parameters
         ----------
         fraction_fit : float, optional
             Fraction of clients used during training. Defaults to 0.1.
         fraction_evaluate : float, optional
             Fraction of clients used during validation. Defaults to 0.1.
         min_fit_clients : int, optional
             Minimum number of clients used during training. Defaults to 2.
         min_evaluate_clients : int, optional
             Minimum number of clients used during validation. Defaults to 2.
         min_available_clients : int, optional
             Minimum number of total clients in the system. Defaults to 2.
-        evaluate_fn : Optional[Callable[[int, NDArrays, Dict[str, Scalar]],
-            Optional[Tuple[float, Dict[str, Scalar]]]]]
+        evaluate_fn : Optional[Callable[[int, NDArrays, Dict[str, Scalar]], Optional[Tuple[float, Dict[str, Scalar]]]]]
             Optional function used for validation. Defaults to None.
         on_fit_config_fn : Callable[[int], Dict[str, Scalar]], optional
             Function used to configure training. Defaults to None.
         on_evaluate_config_fn : Callable[[int], Dict[str, Scalar]], optional
             Function used to configure validation. Defaults to None.
         accept_failures : bool, optional
             Whether or not accept rounds containing failures. Defaults to True.
         initial_parameters : Parameters, optional
             Initial global model parameters.
         beta : float, optional
             Fraction to cut off of both tails of the distribution. Defaults to 0.2.
         """
-
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
             evaluate_fn=evaluate_fn,
@@ -106,14 +104,15 @@
             initial_parameters=initial_parameters,
             fit_metrics_aggregation_fn=fit_metrics_aggregation_fn,
             evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
         )
         self.beta = beta
 
     def __repr__(self) -> str:
+        """Compute a string representation of the strategy."""
         rep = f"FedTrimmedAvg(accept_failures={self.accept_failures})"
         return rep
 
     def aggregate_fit(
         self,
         server_round: int,
         results: List[Tuple[ClientProxy, FitRes]],
```

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Federated XGBoost in the horizontal setting based on building Neural Network and
-averaging on prediction outcomes [Ma et al., 2023].
+"""Federated XGBoost [Ma et al., 2023] strategy.
+
+Strategy in the horizontal setting based on building Neural Network and averaging on
+prediction outcomes.
 
 Paper: Coming
 """
 
 
 from logging import WARNING
 from typing import Any, Dict, List, Optional, Tuple, Union
@@ -26,19 +28,19 @@
 from flwr.common.logger import log
 from flwr.server.client_proxy import ClientProxy
 
 from .aggregate import aggregate
 from .fedavg import FedAvg
 
 
-# flake8: noqa: E501
 class FedXgbNnAvg(FedAvg):
     """Configurable FedXgbNnAvg strategy implementation."""
 
     def __repr__(self) -> str:
+        """Compute a string representation of the strategy."""
         rep = f"FedXgbNnAvg(accept_failures={self.accept_failures})"
         return rep
 
     def evaluate(
         self, server_round: int, parameters: Any
     ) -> Optional[Tuple[float, Dict[str, Scalar]]]:
         """Evaluate model parameters using an evaluation function."""
@@ -52,34 +54,34 @@
         return loss, metrics
 
     def aggregate_fit(
         self,
         server_round: int,
         results: List[Tuple[ClientProxy, FitRes]],
         failures: List[Union[Tuple[ClientProxy, FitRes], BaseException]],
-    ) -> Tuple[Optional[Any], Dict[str, Scalar],]:
+    ) -> Tuple[Optional[Any], Dict[str, Scalar]]:
         """Aggregate fit results using weighted average."""
         if not results:
             return None, {}
         # Do not aggregate if there are failures and failures are not accepted
         if not self.accept_failures and failures:
             return None, {}
 
         # Convert results
         weights_results = [
             (
-                parameters_to_ndarrays(fit_res.parameters[0].parameters),  # type: ignore
+                parameters_to_ndarrays(fit_res.parameters[0].parameters),  # type: ignore # noqa: E501 # pylint: disable=line-too-long
                 fit_res.num_examples,
             )
             for _, fit_res in results
         ]
         parameters_aggregated = ndarrays_to_parameters(aggregate(weights_results))
 
         # Aggregate XGBoost trees from all clients
-        trees_aggregated = [fit_res.parameters[1] for _, fit_res in results]  # type: ignore
+        trees_aggregated = [fit_res.parameters[1] for _, fit_res in results]  # type: ignore # noqa: E501 # pylint: disable=line-too-long
 
         # Aggregate custom metrics if aggregation fn was provided
         metrics_aggregated = {}
         if self.fit_metrics_aggregation_fn:
             fit_metrics = [(res.num_examples, res.metrics) for _, res in results]
             metrics_aggregated = self.fit_metrics_aggregation_fn(fit_metrics)
         elif server_round == 1:  # Only log this warning once
```

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/fedyogi.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,23 +32,23 @@
     parameters_to_ndarrays,
 )
 from flwr.server.client_proxy import ClientProxy
 
 from .fedopt import FedOpt
 
 
-# flake8: noqa: E501
 class FedYogi(FedOpt):
-    """Adaptive Federated Optimization using Yogi (FedYogi) [Reddi et al., 2020]
-    strategy.
+    """FedYogi [Reddi et al., 2020] strategy.
+
+    Adaptive Federated Optimization using Yogi.
 
     Paper: https://arxiv.org/abs/2003.00295
     """
 
-    # pylint: disable=too-many-arguments,too-many-instance-attributes,too-many-locals,line-too-long
+    # pylint: disable=too-many-arguments,too-many-instance-attributes,too-many-locals, line-too-long
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
@@ -130,14 +130,15 @@
             eta_l=eta_l,
             beta_1=beta_1,
             beta_2=beta_2,
             tau=tau,
         )
 
     def __repr__(self) -> str:
+        """Compute a string representation of the strategy."""
         rep = f"FedYogi(accept_failures={self.accept_failures})"
         return rep
 
     def aggregate_fit(
         self,
         server_round: int,
         results: List[Tuple[ClientProxy, FitRes]],
```

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/krum.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,19 +35,18 @@
 from flwr.common.logger import log
 from flwr.server.client_proxy import ClientProxy
 
 from .aggregate import aggregate_krum
 from .fedavg import FedAvg
 
 
-# flake8: noqa: E501
 class Krum(FedAvg):
     """Configurable Krum strategy implementation."""
 
-    # pylint: disable=too-many-arguments,too-many-instance-attributes,line-too-long
+    # pylint: disable=too-many-arguments,too-many-instance-attributes, line-too-long
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
@@ -63,15 +62,15 @@
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
         on_evaluate_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
         accept_failures: bool = True,
         initial_parameters: Optional[Parameters] = None,
         fit_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
         evaluate_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
     ) -> None:
-        """Configurable Krum strategy.
+        """Krum strategy.
 
         Parameters
         ----------
         fraction_fit : float, optional
             Fraction of clients used during training. Defaults to 0.1.
         fraction_evaluate : float, optional
             Fraction of clients used during validation. Defaults to 0.1.
@@ -80,27 +79,27 @@
         min_evaluate_clients : int, optional
             Minimum number of clients used during validation. Defaults to 2.
         min_available_clients : int, optional
             Minimum number of total clients in the system. Defaults to 2.
         num_malicious_clients : int, optional
             Number of malicious clients in the system. Defaults to 0.
         num_clients_to_keep : int, optional
-            Number of clients to keep before averaging (MultiKrum). Defaults to 0, in that case classical Krum is applied.
+            Number of clients to keep before averaging (MultiKrum). Defaults to 0, in
+            that case classical Krum is applied.
         evaluate_fn : Optional[Callable[[int, NDArrays, Dict[str, Scalar]], Optional[Tuple[float, Dict[str, Scalar]]]]]
             Optional function used for validation. Defaults to None.
         on_fit_config_fn : Callable[[int], Dict[str, Scalar]], optional
             Function used to configure training. Defaults to None.
         on_evaluate_config_fn : Callable[[int], Dict[str, Scalar]], optional
             Function used to configure validation. Defaults to None.
         accept_failures : bool, optional
             Whether or not accept rounds containing failures. Defaults to True.
         initial_parameters : Parameters, optional
             Initial global model parameters.
         """
-
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
             evaluate_fn=evaluate_fn,
@@ -111,14 +110,15 @@
             fit_metrics_aggregation_fn=fit_metrics_aggregation_fn,
             evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
         )
         self.num_malicious_clients = num_malicious_clients
         self.num_clients_to_keep = num_clients_to_keep
 
     def __repr__(self) -> str:
+        """Compute a string representation of the strategy."""
         rep = f"Krum(accept_failures={self.accept_failures})"
         return rep
 
     def aggregate_fit(
         self,
         server_round: int,
         results: List[Tuple[ClientProxy, FitRes]],
```

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/qfedavg.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
         )
         self.learning_rate = qffl_learning_rate
         self.q_param = q_param
         self.pre_weights: Optional[NDArrays] = None
 
     def __repr__(self) -> str:
-        # pylint: disable=line-too-long
+        """Compute a string representation of the strategy."""
         rep = f"QffedAvg(learning_rate={self.learning_rate}, "
         rep += f"q_param={self.q_param}, pre_weights={self.pre_weights})"
         return rep
 
     def num_fit_clients(self, num_available_clients: int) -> Tuple[int, int]:
         """Return the sample size and the required number of available clients."""
         num_clients = int(num_available_clients * self.fraction_fit)
```

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/simulation/app.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.5.0.dev20230616/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230615/setup.py` & `flwr_nightly-1.5.0.dev20230616/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 {'console_scripts': ['flower-client = flwr.client:run_client',
                      'flower-driver-api = flwr.server:run_driver_api',
                      'flower-fleet-api = flwr.server:run_fleet_api',
                      'flower-server = flwr.server:run_server']}
 
 setup_kwargs = {
     'name': 'flwr-nightly',
-    'version': '1.5.0.dev20230615',
+    'version': '1.5.0.dev20230616',
     'description': 'Flower: A Friendly Federated Learning Framework',
     'long_description': '# Flower: A Friendly Federated Learning Framework\n\n<p align="center">\n  <a href="https://flower.dev/">\n    <img src="https://flower.dev/_next/image/?url=%2F_next%2Fstatic%2Fmedia%2Fflower_white_border.c2012e70.png&w=640&q=75" width="140px" alt="Flower Website" />\n  </a>\n</p>\n<p align="center">\n    <a href="https://flower.dev/">Website</a> |\n    <a href="https://flower.dev/blog">Blog</a> |\n    <a href="https://flower.dev/docs/">Docs</a> |\n    <a href="https://flower.dev/conf/flower-summit-2022">Conference</a> |\n    <a href="https://flower.dev/join-slack">Slack</a>\n    <br /><br />\n</p>\n\n[![GitHub license](https://img.shields.io/github/license/adap/flower)](https://github.com/adap/flower/blob/main/LICENSE)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/flower/blob/main/CONTRIBUTING.md)\n![Build](https://github.com/adap/flower/actions/workflows/flower.yml/badge.svg)\n![Downloads](https://pepy.tech/badge/flwr)\n[![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://flower.dev/join-slack)\n\nFlower (`flwr`) is a framework for building federated learning systems. The\ndesign of Flower is based on a few guiding principles:\n\n* **Customizable**: Federated learning systems vary wildly from one use case to\n  another. Flower allows for a wide range of different configurations depending\n  on the needs of each individual use case.\n\n* **Extendable**: Flower originated from a research project at the University of\n  Oxford, so it was built with AI research in mind. Many components can be\n  extended and overridden to build new state-of-the-art systems.\n\n* **Framework-agnostic**: Different machine learning frameworks have different\n  strengths. Flower can be used with any machine learning framework, for\n  example, [PyTorch](https://pytorch.org),\n  [TensorFlow](https://tensorflow.org), [Hugging Face Transformers](https://huggingface.co/), [PyTorch Lightning](https://pytorchlightning.ai/), [MXNet](https://mxnet.apache.org/), [scikit-learn](https://scikit-learn.org/), [JAX](https://jax.readthedocs.io/), [TFLite](https://tensorflow.org/lite/), [fastai](https://www.fast.ai/), [Pandas](https://pandas.pydata.org/\n) for federated analytics, or even raw [NumPy](https://numpy.org/)\n  for users who enjoy computing gradients by hand.\n\n* **Understandable**: Flower is written with maintainability in mind. The\n  community is encouraged to both read and contribute to the codebase.\n\nMeet the Flower community on [flower.dev](https://flower.dev)!\n\n## Federated Learning Tutorial\n\nFlower\'s goal is to make federated learning accessible to everyone. This series of tutorials introduces the fundamentals of federated learning and how to implement them in Flower.\n\n0. **What is Federated Learning?**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb))\n\n1. **An Introduction to Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb))\n\n2. **Using Strategies in Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb))\n   \n3. **Building Strategies for Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb))\n   \n4. **Custom Clients for Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb))\n\nStay tuned, more tutorials are coming soon. Topics include **Privacy and Security in Federated Learning**, and **Scaling Federated Learning**.\n\n## Documentation\n\n[Flower Docs](https://flower.dev/docs):\n* [Installation](https://flower.dev/docs/installation.html)\n* [Quickstart (TensorFlow)](https://flower.dev/docs/quickstart-tensorflow.html)\n* [Quickstart (PyTorch)](https://flower.dev/docs/quickstart-pytorch.html)\n* [Quickstart (Hugging Face [code example])](https://flower.dev/docs/quickstart-huggingface.html)\n* [Quickstart (PyTorch Lightning [code example])](https://flower.dev/docs/quickstart-pytorch-lightning.html)\n* [Quickstart (MXNet)](https://flower.dev/docs/example-mxnet-walk-through.html)\n* [Quickstart (Pandas)](https://flower.dev/docs/quickstart-pandas.html)\n* [Quickstart (fastai)](https://flower.dev/docs/quickstart-fastai.html)\n* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)\n* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)\n* [Quickstart (TFLite on Android [code example])](https://github.com/adap/flower/tree/main/examples/android)\n* [Quickstart (iOS)](https://flower.dev/docs/quickstart-ios.html)\n\n## Flower Baselines\n\nFlower Baselines is a collection of community-contributed experiments that reproduce the experiments performed in popular federated learning publications. Researchers can build on Flower Baselines to quickly evaluate new ideas:\n\n* [FedAvg](https://arxiv.org/abs/1602.05629):\n  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedavg_mnist)\n* [FedProx](https://arxiv.org/abs/1812.06127):\n  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedprox_mnist)\n* [FedBN: Federated Learning on non-IID Features via Local Batch Normalization](https://arxiv.org/abs/2102.07623):\n  * [Convergence Rate](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedbn/convergence_rate)\n* [Adaptive Federated Optimization](https://arxiv.org/abs/2003.00295):\n  * [CIFAR-10/100](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/adaptive_federated_optimization)\n\nCheck the Flower documentation to learn more: [Using Baselines](https://flower.dev/docs/using-baselines.html)\n\nThe Flower community loves contributions! Make your work more visible and enable others to build on it by contributing it as a baseline: [Contributing Baselines](https://flower.dev/docs/contributing-baselines.html)\n\n## Flower Usage Examples\n\nSeveral code examples show different usage scenarios of Flower (in combination with popular machine learning frameworks such as PyTorch or TensorFlow).\n\nQuickstart examples:\n\n* [Quickstart (TensorFlow)](https://github.com/adap/flower/tree/main/examples/quickstart_tensorflow)\n* [Quickstart (PyTorch)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch)\n* [Quickstart (Hugging Face)](https://github.com/adap/flower/tree/main/examples/quickstart_huggingface)\n* [Quickstart (PyTorch Lightning)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch_lightning)\n* [Quickstart (fastai)](https://github.com/adap/flower/tree/main/examples/quickstart_fastai)\n* [Quickstart (Pandas)](https://github.com/adap/flower/tree/main/examples/quickstart_pandas)\n* [Quickstart (MXNet)](https://github.com/adap/flower/tree/main/examples/quickstart_mxnet)\n* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)\n* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)\n* [Quickstart (TFLite on Android)](https://github.com/adap/flower/tree/main/examples/android)\n\nOther [examples](https://github.com/adap/flower/tree/main/examples):\n\n* [Raspberry Pi & Nvidia Jetson Tutorial](https://github.com/adap/flower/tree/main/examples/embedded_devices)\n* [Android & TFLite](https://github.com/adap/flower/tree/main/examples/android)\n* [PyTorch: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/pytorch_from_centralized_to_federated)\n* [MXNet: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/mxnet_from_centralized_to_federated)\n* [Advanced Flower with TensorFlow/Keras](https://github.com/adap/flower/tree/main/examples/advanced_tensorflow)\n* [Advanced Flower with PyTorch](https://github.com/adap/flower/tree/main/examples/advanced_pytorch)\n* Single-Machine Simulation of Federated Learning Systems ([PyTorch](https://github.com/adap/flower/tree/main/examples/simulation_pytorch)) ([Tensorflow](https://github.com/adap/flower/tree/main/examples/simulation_tensorflow))\n\n## Community\n\nFlower is built by a wonderful community of researchers and engineers. [Join Slack](https://flower.dev/join-slack) to meet them, [contributions](#contributing-to-flower) are welcome.\n\n<a href="https://github.com/adap/flower/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=adap/flower" />\n</a>\n\n## Citation\n\nIf you publish work that uses Flower, please cite Flower as follows: \n\n```bibtex\n@article{beutel2020flower,\n  title={Flower: A Friendly Federated Learning Research Framework},\n  author={Beutel, Daniel J and Topal, Taner and Mathur, Akhil and Qiu, Xinchi and Fernandez-Marques, Javier and Gao, Yan and Sani, Lorenzo and Kwing, Hei Li and Parcollet, Titouan and Gusmão, Pedro PB de and Lane, Nicholas D}, \n  journal={arXiv preprint arXiv:2007.14390},\n  year={2020}\n}\n```\n\nPlease also consider adding your publication to the list of Flower-based publications in the docs, just open a Pull Request.\n\n## Contributing to Flower\n\nWe welcome contributions. Please see [CONTRIBUTING.md](CONTRIBUTING.md) to get started!\n',
     'author': 'The Flower Authors',
     'author_email': 'hello@flower.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://flower.dev',
```

#### html2text {}

```diff
@@ -12,15 +12,15 @@
 extras_require = \ {':python_version < "3.8"': ['importlib-
 metadata>=4.0.0,<5.0.0'], 'rest': ['requests>=2.28.2,<3.0.0',
 'fastapi>=0.95.0,<0.96.0', 'starlette>=0.26.1,<0.27.0', 'uvicorn
 [standard]>=0.21.1,<0.22.0'], 'simulation': ['ray[default]>=2.4.0,<3.0.0']}
 entry_points = \ {'console_scripts': ['flower-client = flwr.client:run_client',
 'flower-driver-api = flwr.server:run_driver_api', 'flower-fleet-api =
 flwr.server:run_fleet_api', 'flower-server = flwr.server:run_server']}
-setup_kwargs = { 'name': 'flwr-nightly', 'version': '1.5.0.dev20230615',
+setup_kwargs = { 'name': 'flwr-nightly', 'version': '1.5.0.dev20230616',
 'description': 'Flower: A Friendly Federated Learning Framework',
 'long_description': '# Flower: A Friendly Federated Learning Framework\n\n
                           \n \n_[Flower_Website]\n\n
 \n
            \n Website |\n Blog |\n Docs |\n Conference |\n Slack\n
 
                                       \n
```

### Comparing `flwr_nightly-1.5.0.dev20230615/PKG-INFO` & `flwr_nightly-1.5.0.dev20230616/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.5.0.dev20230615
+Version: 1.5.0.dev20230616
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.dev
 License: Apache-2.0
 Author: The Flower Authors
 Author-email: hello@flower.dev
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.5.0.dev20230615 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.5.0.dev20230616 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.dev
 License: Apache-2.0 Author: The Flower Authors Author-email: hello@flower.dev
 Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: MacOS :: MacOS X Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
```

