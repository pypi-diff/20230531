# Comparing `tmp/daisyfl-0.4.3.tar.gz` & `tmp/daisyfl-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daisyfl-0.4.3.tar", max compression
+gzip compressed data, was "daisyfl-0.4.4.tar", max compression
```

## Comparing `daisyfl-0.4.3.tar` & `daisyfl-0.4.4.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0    11358 2023-01-10 07:20:47.485254 daisyfl-0.4.3/LICENSE
--rw-r--r--   0        0        0      691 2023-01-10 07:20:47.485254 daisyfl-0.4.3/README.md
--rw-r--r--   0        0        0     3661 2023-05-30 05:35:43.266033 daisyfl-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     1093 2023-01-10 07:20:47.633253 daisyfl-0.4.3/src/py/daisyfl/__init__.py
--rw-r--r--   0        0        0     1171 2023-01-10 07:20:47.633253 daisyfl-0.4.3/src/py/daisyfl/client/__init__.py
--rw-r--r--   0        0        0     9951 2023-05-19 12:59:40.857765 daisyfl-0.4.3/src/py/daisyfl/client/app.py
--rw-r--r--   0        0        0     3733 2023-01-10 07:20:47.633253 daisyfl-0.4.3/src/py/daisyfl/client/client.py
--rw-r--r--   0        0        0     1363 2023-05-11 01:39:32.910194 daisyfl-0.4.3/src/py/daisyfl/client/client_api_handler.py
--rw-r--r--   0        0        0     3780 2023-01-10 07:20:47.633253 daisyfl-0.4.3/src/py/daisyfl/client/client_operator_manager.py
--rw-r--r--   0        0        0     3367 2023-01-10 07:20:47.633253 daisyfl-0.4.3/src/py/daisyfl/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      714 2023-01-10 07:20:47.633253 daisyfl-0.4.3/src/py/daisyfl/client/grpc_client/__init__.py
--rw-r--r--   0        0        0    10038 2023-05-16 08:32:20.489432 daisyfl-0.4.3/src/py/daisyfl/client/grpc_client/connection.py
--rw-r--r--   0        0        0     6704 2023-04-22 08:34:34.572565 daisyfl-0.4.3/src/py/daisyfl/client/grpc_client/message_handler.py
--rw-r--r--   0        0        0     5084 2023-01-10 07:20:47.633253 daisyfl-0.4.3/src/py/daisyfl/client/numpy_client.py
--rw-r--r--   0        0        0     4913 2023-05-16 09:25:04.651405 daisyfl-0.4.3/src/py/daisyfl/client/trainer.py
--rw-r--r--   0        0        0     1663 2023-04-24 08:39:30.199565 daisyfl-0.4.3/src/py/daisyfl/client/zone_client.py
--rw-r--r--   0        0        0     5109 2023-05-29 12:06:10.760431 daisyfl-0.4.3/src/py/daisyfl/common/__init__.py
--rw-r--r--   0        0        0     1830 2023-01-10 07:20:47.633253 daisyfl-0.4.3/src/py/daisyfl/common/dp.py
--rw-r--r--   0        0        0     3482 2023-05-03 08:10:21.588582 daisyfl-0.4.3/src/py/daisyfl/common/logger.py
--rw-r--r--   0        0        0     1421 2023-05-29 12:06:19.556411 daisyfl-0.4.3/src/py/daisyfl/common/metadata.py
--rw-r--r--   0        0        0     3938 2023-01-10 07:20:47.633253 daisyfl-0.4.3/src/py/daisyfl/common/parameter.py
--rw-r--r--   0        0        0    16903 2023-05-14 06:48:53.590144 daisyfl-0.4.3/src/py/daisyfl/common/serde.py
--rw-r--r--   0        0        0     4044 2023-05-16 07:23:10.624100 daisyfl-0.4.3/src/py/daisyfl/common/typing.py
--rw-r--r--   0        0        0        0 2023-01-10 07:20:47.633253 daisyfl-0.4.3/src/py/daisyfl/operator/__init__.py
--rw-r--r--   0        0        0        0 2023-01-10 07:20:47.633253 daisyfl-0.4.3/src/py/daisyfl/operator/base/__init__.py
--rw-r--r--   0        0        0     1162 2023-01-10 07:20:47.633253 daisyfl-0.4.3/src/py/daisyfl/operator/base/client_logic.py
--rw-r--r--   0        0        0     5314 2023-05-16 08:40:46.238319 daisyfl-0.4.3/src/py/daisyfl/operator/base/server_logic.py
--rw-r--r--   0        0        0        0 2023-02-08 08:28:14.950340 daisyfl-0.4.3/src/py/daisyfl/operator/base_async/__init__.py
--rw-r--r--   0        0        0     1162 2023-02-09 07:20:06.916018 daisyfl-0.4.3/src/py/daisyfl/operator/base_async/client_logic.py
--rw-r--r--   0        0        0     5381 2023-05-16 11:59:38.489016 daisyfl-0.4.3/src/py/daisyfl/operator/base_async/server_logic.py
--rw-r--r--   0        0        0     1987 2023-01-10 07:20:47.633253 daisyfl-0.4.3/src/py/daisyfl/operator/msg_demo/client_logic.py
--rw-r--r--   0        0        0      381 2023-01-10 07:20:47.637253 daisyfl-0.4.3/src/py/daisyfl/operator/msg_demo/msg.py
--rw-r--r--   0        0        0     5320 2023-05-16 11:35:42.881982 daisyfl-0.4.3/src/py/daisyfl/operator/msg_demo/server_logic.py
--rw-r--r--   0        0        0      961 2023-01-10 07:20:47.637253 daisyfl-0.4.3/src/py/daisyfl/operator/msg_demo/zone_client_logic.py
--rw-r--r--   0        0        0     5409 2023-05-16 11:40:56.320957 daisyfl-0.4.3/src/py/daisyfl/operator/msg_demo/zone_server_logic.py
--rw-r--r--   0        0        0    12049 2023-01-10 07:20:47.637253 daisyfl-0.4.3/src/py/daisyfl/operator/sec_agg/client_logic.py
--rw-r--r--   0        0        0     1755 2023-01-10 07:20:47.637253 daisyfl-0.4.3/src/py/daisyfl/operator/sec_agg/common.py
--rw-r--r--   0        0        0    10070 2023-01-10 07:20:47.637253 daisyfl-0.4.3/src/py/daisyfl/operator/sec_agg/primitives.py
--rw-r--r--   0        0        0    20378 2023-05-16 11:45:43.312726 daisyfl-0.4.3/src/py/daisyfl/operator/sec_agg/server_logic.py
--rw-r--r--   0        0        0     1456 2023-02-09 06:56:21.776202 daisyfl-0.4.3/src/py/daisyfl/operator/strategy/__init__.py
--rw-r--r--   0        0        0     3012 2023-02-09 06:53:49.280829 daisyfl-0.4.3/src/py/daisyfl/operator/strategy/aggregate.py
--rw-r--r--   0        0        0     4538 2023-05-16 12:09:01.916334 daisyfl-0.4.3/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     5095 2023-05-16 12:13:03.915973 daisyfl-0.4.3/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     6134 2023-05-16 12:14:40.331823 daisyfl-0.4.3/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6993 2023-05-16 12:15:36.883734 daisyfl-0.4.3/src/py/daisyfl/operator/strategy/fedadagrad.py
--rw-r--r--   0        0        0     7245 2023-05-16 12:16:34.455643 daisyfl-0.4.3/src/py/daisyfl/operator/strategy/fedadam.py
--rw-r--r--   0        0        0    13114 2023-05-16 12:17:30.311554 daisyfl-0.4.3/src/py/daisyfl/operator/strategy/fedasync.py
--rw-r--r--   0        0        0    12454 2023-05-16 07:22:14.364120 daisyfl-0.4.3/src/py/daisyfl/operator/strategy/fedavg.py
--rw-r--r--   0        0        0    10983 2023-05-16 12:18:28.123569 daisyfl-0.4.3/src/py/daisyfl/operator/strategy/fedavg_android.py
--rw-r--r--   0        0        0     9115 2023-05-16 12:19:23.807713 daisyfl-0.4.3/src/py/daisyfl/operator/strategy/fedavgm.py
--rw-r--r--   0        0        0     5513 2023-05-16 12:20:07.411811 daisyfl-0.4.3/src/py/daisyfl/operator/strategy/fedopt.py
--rw-r--r--   0        0        0     7263 2023-05-16 12:20:50.715896 daisyfl-0.4.3/src/py/daisyfl/operator/strategy/fedyogi.py
--rw-r--r--   0        0        0    11020 2023-05-16 12:22:36.468058 daisyfl-0.4.3/src/py/daisyfl/operator/strategy/qfedavg.py
--rw-r--r--   0        0        0     7867 2023-05-15 01:53:20.710219 daisyfl-0.4.3/src/py/daisyfl/operator/strategy/strategy.py
--rw-r--r--   0        0        0      728 2023-05-16 06:37:26.602959 daisyfl-0.4.3/src/py/daisyfl/operator/utils/__init__.py
--rw-r--r--   0        0        0     5003 2023-05-16 07:20:49.404138 daisyfl-0.4.3/src/py/daisyfl/operator/utils/op_tools.py
--rw-r--r--   0        0        0      676 2023-01-10 07:20:47.637253 daisyfl-0.4.3/src/py/daisyfl/proto/__init__.py
--rw-r--r--   0        0        0    70900 2023-05-14 06:35:47.413527 daisyfl-0.4.3/src/py/daisyfl/proto/transport_pb2.py
--rw-r--r--   0        0        0    25816 2023-05-14 06:35:47.413527 daisyfl-0.4.3/src/py/daisyfl/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2631 2023-05-14 06:35:47.413527 daisyfl-0.4.3/src/py/daisyfl/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      781 2023-05-14 06:35:47.413527 daisyfl-0.4.3/src/py/daisyfl/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0     1064 2023-01-10 07:20:47.637253 daisyfl-0.4.3/src/py/daisyfl/server/__init__.py
--rw-r--r--   0        0        0     5085 2023-05-16 03:16:56.626232 daisyfl-0.4.3/src/py/daisyfl/server/app.py
--rw-r--r--   0        0        0     6901 2023-05-16 07:14:08.099939 daisyfl-0.4.3/src/py/daisyfl/server/client_manager.py
--rw-r--r--   0        0        0     2371 2023-05-16 06:58:02.621351 daisyfl-0.4.3/src/py/daisyfl/server/client_proxy.py
--rw-r--r--   0        0        0      714 2023-01-10 07:20:47.637253 daisyfl-0.4.3/src/py/daisyfl/server/grpc_server/__init__.py
--rw-r--r--   0        0        0    12768 2023-05-29 12:11:49.083658 daisyfl-0.4.3/src/py/daisyfl/server/grpc_server/flower_service_servicer.py
--rw-r--r--   0        0        0     6707 2023-05-16 08:08:05.114034 daisyfl-0.4.3/src/py/daisyfl/server/grpc_server/grpc_bridge.py
--rw-r--r--   0        0        0     4459 2023-05-16 08:12:28.157478 daisyfl-0.4.3/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py
--rw-r--r--   0        0        0    11290 2023-05-09 06:31:30.706022 daisyfl-0.4.3/src/py/daisyfl/server/grpc_server/grpc_server.py
--rw-r--r--   0        0        0     3626 2023-01-10 07:20:47.637253 daisyfl-0.4.3/src/py/daisyfl/server/history.py
--rw-r--r--   0        0        0    11104 2023-05-16 11:51:48.437191 daisyfl-0.4.3/src/py/daisyfl/server/server.py
--rw-r--r--   0        0        0     1011 2023-04-24 07:53:15.707000 daisyfl-0.4.3/src/py/daisyfl/server/server_api_handler.py
--rw-r--r--   0        0        0     4560 2023-05-16 03:14:42.710438 daisyfl-0.4.3/src/py/daisyfl/server/server_operator_manager.py
--rw-r--r--   0        0        0    11969 2023-04-24 08:56:27.545364 daisyfl-0.4.3/src/py/daisyfl/server/task_manager.py
--rw-r--r--   0        0        0     1273 2023-01-10 07:20:47.637253 daisyfl-0.4.3/src/py/daisyfl/simulation/__init__.py
--rw-r--r--   0        0        0     7335 2023-01-10 07:20:47.637253 daisyfl-0.4.3/src/py/daisyfl/simulation/app.py
--rw-r--r--   0        0        0      727 2023-01-10 07:20:47.637253 daisyfl-0.4.3/src/py/daisyfl/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0     4661 2023-01-10 07:20:47.637253 daisyfl-0.4.3/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0      859 2023-01-10 07:20:47.637253 daisyfl-0.4.3/src/py/daisyfl/utils/__init__.py
--rw-r--r--   0        0        0      121 2023-01-10 07:20:47.637253 daisyfl-0.4.3/src/py/daisyfl/utils/dynamic_loader.py
--rw-r--r--   0        0        0     2277 2023-05-30 05:38:00.740875 daisyfl-0.4.3/setup.py
--rw-r--r--   0        0        0     2819 2023-05-30 05:38:00.741076 daisyfl-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-01-10 07:20:47.485254 daisyfl-0.4.4/LICENSE
+-rw-r--r--   0        0        0      691 2023-01-10 07:20:47.485254 daisyfl-0.4.4/README.md
+-rw-r--r--   0        0        0     3661 2023-05-31 06:45:05.872346 daisyfl-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1093 2023-01-10 07:20:47.633253 daisyfl-0.4.4/src/py/daisyfl/__init__.py
+-rw-r--r--   0        0        0     1171 2023-01-10 07:20:47.633253 daisyfl-0.4.4/src/py/daisyfl/client/__init__.py
+-rw-r--r--   0        0        0     9951 2023-05-19 12:59:40.857765 daisyfl-0.4.4/src/py/daisyfl/client/app.py
+-rw-r--r--   0        0        0     3733 2023-01-10 07:20:47.633253 daisyfl-0.4.4/src/py/daisyfl/client/client.py
+-rw-r--r--   0        0        0     1363 2023-05-11 01:39:32.910194 daisyfl-0.4.4/src/py/daisyfl/client/client_api_handler.py
+-rw-r--r--   0        0        0     3780 2023-01-10 07:20:47.633253 daisyfl-0.4.4/src/py/daisyfl/client/client_operator_manager.py
+-rw-r--r--   0        0        0     3367 2023-01-10 07:20:47.633253 daisyfl-0.4.4/src/py/daisyfl/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      714 2023-01-10 07:20:47.633253 daisyfl-0.4.4/src/py/daisyfl/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0    10038 2023-05-16 08:32:20.489432 daisyfl-0.4.4/src/py/daisyfl/client/grpc_client/connection.py
+-rw-r--r--   0        0        0     6704 2023-04-22 08:34:34.572565 daisyfl-0.4.4/src/py/daisyfl/client/grpc_client/message_handler.py
+-rw-r--r--   0        0        0     5084 2023-01-10 07:20:47.633253 daisyfl-0.4.4/src/py/daisyfl/client/numpy_client.py
+-rw-r--r--   0        0        0     4913 2023-05-16 09:25:04.651405 daisyfl-0.4.4/src/py/daisyfl/client/trainer.py
+-rw-r--r--   0        0        0     1663 2023-04-24 08:39:30.199565 daisyfl-0.4.4/src/py/daisyfl/client/zone_client.py
+-rw-r--r--   0        0        0     5109 2023-05-29 12:06:10.760431 daisyfl-0.4.4/src/py/daisyfl/common/__init__.py
+-rw-r--r--   0        0        0     1830 2023-01-10 07:20:47.633253 daisyfl-0.4.4/src/py/daisyfl/common/dp.py
+-rw-r--r--   0        0        0     3482 2023-05-03 08:10:21.588582 daisyfl-0.4.4/src/py/daisyfl/common/logger.py
+-rw-r--r--   0        0        0     1421 2023-05-29 12:06:19.556411 daisyfl-0.4.4/src/py/daisyfl/common/metadata.py
+-rw-r--r--   0        0        0     3938 2023-01-10 07:20:47.633253 daisyfl-0.4.4/src/py/daisyfl/common/parameter.py
+-rw-r--r--   0        0        0    16903 2023-05-14 06:48:53.590144 daisyfl-0.4.4/src/py/daisyfl/common/serde.py
+-rw-r--r--   0        0        0     4044 2023-05-16 07:23:10.624100 daisyfl-0.4.4/src/py/daisyfl/common/typing.py
+-rw-r--r--   0        0        0        0 2023-01-10 07:20:47.633253 daisyfl-0.4.4/src/py/daisyfl/operator/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-10 07:20:47.633253 daisyfl-0.4.4/src/py/daisyfl/operator/base/__init__.py
+-rw-r--r--   0        0        0     1162 2023-01-10 07:20:47.633253 daisyfl-0.4.4/src/py/daisyfl/operator/base/client_logic.py
+-rw-r--r--   0        0        0     5314 2023-05-16 08:40:46.238319 daisyfl-0.4.4/src/py/daisyfl/operator/base/server_logic.py
+-rw-r--r--   0        0        0        0 2023-02-08 08:28:14.950340 daisyfl-0.4.4/src/py/daisyfl/operator/base_async/__init__.py
+-rw-r--r--   0        0        0     1162 2023-02-09 07:20:06.916018 daisyfl-0.4.4/src/py/daisyfl/operator/base_async/client_logic.py
+-rw-r--r--   0        0        0     5381 2023-05-16 11:59:38.489016 daisyfl-0.4.4/src/py/daisyfl/operator/base_async/server_logic.py
+-rw-r--r--   0        0        0     1987 2023-01-10 07:20:47.633253 daisyfl-0.4.4/src/py/daisyfl/operator/msg_demo/client_logic.py
+-rw-r--r--   0        0        0      381 2023-01-10 07:20:47.637253 daisyfl-0.4.4/src/py/daisyfl/operator/msg_demo/msg.py
+-rw-r--r--   0        0        0     5320 2023-05-16 11:35:42.881982 daisyfl-0.4.4/src/py/daisyfl/operator/msg_demo/server_logic.py
+-rw-r--r--   0        0        0      961 2023-01-10 07:20:47.637253 daisyfl-0.4.4/src/py/daisyfl/operator/msg_demo/zone_client_logic.py
+-rw-r--r--   0        0        0     5409 2023-05-16 11:40:56.320957 daisyfl-0.4.4/src/py/daisyfl/operator/msg_demo/zone_server_logic.py
+-rw-r--r--   0        0        0    12049 2023-01-10 07:20:47.637253 daisyfl-0.4.4/src/py/daisyfl/operator/sec_agg/client_logic.py
+-rw-r--r--   0        0        0     1755 2023-01-10 07:20:47.637253 daisyfl-0.4.4/src/py/daisyfl/operator/sec_agg/common.py
+-rw-r--r--   0        0        0    10070 2023-01-10 07:20:47.637253 daisyfl-0.4.4/src/py/daisyfl/operator/sec_agg/primitives.py
+-rw-r--r--   0        0        0    20378 2023-05-16 11:45:43.312726 daisyfl-0.4.4/src/py/daisyfl/operator/sec_agg/server_logic.py
+-rw-r--r--   0        0        0     1456 2023-02-09 06:56:21.776202 daisyfl-0.4.4/src/py/daisyfl/operator/strategy/__init__.py
+-rw-r--r--   0        0        0     3012 2023-02-09 06:53:49.280829 daisyfl-0.4.4/src/py/daisyfl/operator/strategy/aggregate.py
+-rw-r--r--   0        0        0     4538 2023-05-16 12:09:01.916334 daisyfl-0.4.4/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     5095 2023-05-16 12:13:03.915973 daisyfl-0.4.4/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     6134 2023-05-16 12:14:40.331823 daisyfl-0.4.4/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6993 2023-05-16 12:15:36.883734 daisyfl-0.4.4/src/py/daisyfl/operator/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     7245 2023-05-16 12:16:34.455643 daisyfl-0.4.4/src/py/daisyfl/operator/strategy/fedadam.py
+-rw-r--r--   0        0        0    13114 2023-05-16 12:17:30.311554 daisyfl-0.4.4/src/py/daisyfl/operator/strategy/fedasync.py
+-rw-r--r--   0        0        0    12454 2023-05-16 07:22:14.364120 daisyfl-0.4.4/src/py/daisyfl/operator/strategy/fedavg.py
+-rw-r--r--   0        0        0    10983 2023-05-16 12:18:28.123569 daisyfl-0.4.4/src/py/daisyfl/operator/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     9115 2023-05-16 12:19:23.807713 daisyfl-0.4.4/src/py/daisyfl/operator/strategy/fedavgm.py
+-rw-r--r--   0        0        0     5513 2023-05-16 12:20:07.411811 daisyfl-0.4.4/src/py/daisyfl/operator/strategy/fedopt.py
+-rw-r--r--   0        0        0     7263 2023-05-16 12:20:50.715896 daisyfl-0.4.4/src/py/daisyfl/operator/strategy/fedyogi.py
+-rw-r--r--   0        0        0    11020 2023-05-16 12:22:36.468058 daisyfl-0.4.4/src/py/daisyfl/operator/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7867 2023-05-15 01:53:20.710219 daisyfl-0.4.4/src/py/daisyfl/operator/strategy/strategy.py
+-rw-r--r--   0        0        0      728 2023-05-16 06:37:26.602959 daisyfl-0.4.4/src/py/daisyfl/operator/utils/__init__.py
+-rw-r--r--   0        0        0     5003 2023-05-16 07:20:49.404138 daisyfl-0.4.4/src/py/daisyfl/operator/utils/op_tools.py
+-rw-r--r--   0        0        0      676 2023-01-10 07:20:47.637253 daisyfl-0.4.4/src/py/daisyfl/proto/__init__.py
+-rw-r--r--   0        0        0    70900 2023-05-14 06:35:47.413527 daisyfl-0.4.4/src/py/daisyfl/proto/transport_pb2.py
+-rw-r--r--   0        0        0    25816 2023-05-14 06:35:47.413527 daisyfl-0.4.4/src/py/daisyfl/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2631 2023-05-14 06:35:47.413527 daisyfl-0.4.4/src/py/daisyfl/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      781 2023-05-14 06:35:47.413527 daisyfl-0.4.4/src/py/daisyfl/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1064 2023-01-10 07:20:47.637253 daisyfl-0.4.4/src/py/daisyfl/server/__init__.py
+-rw-r--r--   0        0        0     5085 2023-05-16 03:16:56.626232 daisyfl-0.4.4/src/py/daisyfl/server/app.py
+-rw-r--r--   0        0        0     6901 2023-05-16 07:14:08.099939 daisyfl-0.4.4/src/py/daisyfl/server/client_manager.py
+-rw-r--r--   0        0        0     2371 2023-05-16 06:58:02.621351 daisyfl-0.4.4/src/py/daisyfl/server/client_proxy.py
+-rw-r--r--   0        0        0      714 2023-01-10 07:20:47.637253 daisyfl-0.4.4/src/py/daisyfl/server/grpc_server/__init__.py
+-rw-r--r--   0        0        0    12768 2023-05-31 06:44:12.408360 daisyfl-0.4.4/src/py/daisyfl/server/grpc_server/flower_service_servicer.py
+-rw-r--r--   0        0        0     6827 2023-05-31 06:44:25.516356 daisyfl-0.4.4/src/py/daisyfl/server/grpc_server/grpc_bridge.py
+-rw-r--r--   0        0        0     4459 2023-05-16 08:12:28.157478 daisyfl-0.4.4/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11290 2023-05-09 06:31:30.706022 daisyfl-0.4.4/src/py/daisyfl/server/grpc_server/grpc_server.py
+-rw-r--r--   0        0        0     3626 2023-01-10 07:20:47.637253 daisyfl-0.4.4/src/py/daisyfl/server/history.py
+-rw-r--r--   0        0        0    11104 2023-05-16 11:51:48.437191 daisyfl-0.4.4/src/py/daisyfl/server/server.py
+-rw-r--r--   0        0        0     1011 2023-04-24 07:53:15.707000 daisyfl-0.4.4/src/py/daisyfl/server/server_api_handler.py
+-rw-r--r--   0        0        0     4560 2023-05-16 03:14:42.710438 daisyfl-0.4.4/src/py/daisyfl/server/server_operator_manager.py
+-rw-r--r--   0        0        0    11969 2023-04-24 08:56:27.545364 daisyfl-0.4.4/src/py/daisyfl/server/task_manager.py
+-rw-r--r--   0        0        0     1273 2023-01-10 07:20:47.637253 daisyfl-0.4.4/src/py/daisyfl/simulation/__init__.py
+-rw-r--r--   0        0        0     7335 2023-01-10 07:20:47.637253 daisyfl-0.4.4/src/py/daisyfl/simulation/app.py
+-rw-r--r--   0        0        0      727 2023-01-10 07:20:47.637253 daisyfl-0.4.4/src/py/daisyfl/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0     4661 2023-01-10 07:20:47.637253 daisyfl-0.4.4/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0      859 2023-01-10 07:20:47.637253 daisyfl-0.4.4/src/py/daisyfl/utils/__init__.py
+-rw-r--r--   0        0        0      121 2023-01-10 07:20:47.637253 daisyfl-0.4.4/src/py/daisyfl/utils/dynamic_loader.py
+-rw-r--r--   0        0        0     2277 2023-05-31 06:48:36.849507 daisyfl-0.4.4/setup.py
+-rw-r--r--   0        0        0     2819 2023-05-31 06:48:36.849741 daisyfl-0.4.4/PKG-INFO
```

### Comparing `daisyfl-0.4.3/LICENSE` & `daisyfl-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/README.md` & `daisyfl-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/pyproject.toml` & `daisyfl-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "daisyfl"
-version = "0.4.3"
+version = "0.4.4"
 description = "Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing"
 license = "Apache-2.0"
 authors = ["tcfwbper <b05208031@ntu.edu.tw>"]
 readme = "README.md"
 homepage = "https://github.com/Intelligent-Systems-Lab/daisy"
 repository = "https://github.com/Intelligent-Systems-Lab/daisy"
 documentation = "https://github.com/Intelligent-Systems-Lab/daisy/tree/main/doc/daisy"
```

### Comparing `daisyfl-0.4.3/src/py/daisyfl/__init__.py` & `daisyfl-0.4.4/src/py/daisyfl/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/client/__init__.py` & `daisyfl-0.4.4/src/py/daisyfl/client/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/client/app.py` & `daisyfl-0.4.4/src/py/daisyfl/client/app.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/client/client.py` & `daisyfl-0.4.4/src/py/daisyfl/client/client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/client/client_api_handler.py` & `daisyfl-0.4.4/src/py/daisyfl/client/client_api_handler.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/client/client_operator_manager.py` & `daisyfl-0.4.4/src/py/daisyfl/client/client_operator_manager.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/client/dpfedavg_numpy_client.py` & `daisyfl-0.4.4/src/py/daisyfl/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/client/grpc_client/__init__.py` & `daisyfl-0.4.4/src/py/daisyfl/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/client/grpc_client/connection.py` & `daisyfl-0.4.4/src/py/daisyfl/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/client/grpc_client/message_handler.py` & `daisyfl-0.4.4/src/py/daisyfl/client/grpc_client/message_handler.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/client/numpy_client.py` & `daisyfl-0.4.4/src/py/daisyfl/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/client/trainer.py` & `daisyfl-0.4.4/src/py/daisyfl/client/trainer.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/client/zone_client.py` & `daisyfl-0.4.4/src/py/daisyfl/client/zone_client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/common/__init__.py` & `daisyfl-0.4.4/src/py/daisyfl/common/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/common/dp.py` & `daisyfl-0.4.4/src/py/daisyfl/common/dp.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/common/logger.py` & `daisyfl-0.4.4/src/py/daisyfl/common/logger.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/common/metadata.py` & `daisyfl-0.4.4/src/py/daisyfl/common/metadata.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/common/parameter.py` & `daisyfl-0.4.4/src/py/daisyfl/common/parameter.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/common/serde.py` & `daisyfl-0.4.4/src/py/daisyfl/common/serde.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/common/typing.py` & `daisyfl-0.4.4/src/py/daisyfl/common/typing.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/base/client_logic.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/base/client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/base/server_logic.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/base/server_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/base_async/client_logic.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/base_async/client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/base_async/server_logic.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/base_async/server_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/msg_demo/client_logic.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/msg_demo/client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/msg_demo/server_logic.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/msg_demo/server_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/msg_demo/zone_client_logic.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/msg_demo/zone_client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/msg_demo/zone_server_logic.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/msg_demo/zone_server_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/sec_agg/client_logic.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/sec_agg/client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/sec_agg/common.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/sec_agg/common.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/sec_agg/primitives.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/sec_agg/primitives.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/sec_agg/server_logic.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/sec_agg/server_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/strategy/__init__.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/strategy/aggregate.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/strategy/fedadagrad.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/strategy/fedadam.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/strategy/fedasync.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/strategy/fedasync.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/strategy/fedavg.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/strategy/fedavg_android.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/strategy/fedavgm.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/strategy/fedopt.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/strategy/fedyogi.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/strategy/qfedavg.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/strategy/strategy.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/utils/__init__.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/operator/utils/op_tools.py` & `daisyfl-0.4.4/src/py/daisyfl/operator/utils/op_tools.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/proto/__init__.py` & `daisyfl-0.4.4/src/py/daisyfl/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/proto/transport_pb2.py` & `daisyfl-0.4.4/src/py/daisyfl/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/proto/transport_pb2.pyi` & `daisyfl-0.4.4/src/py/daisyfl/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/proto/transport_pb2_grpc.py` & `daisyfl-0.4.4/src/py/daisyfl/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/proto/transport_pb2_grpc.pyi` & `daisyfl-0.4.4/src/py/daisyfl/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/server/__init__.py` & `daisyfl-0.4.4/src/py/daisyfl/server/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/server/app.py` & `daisyfl-0.4.4/src/py/daisyfl/server/app.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/server/client_manager.py` & `daisyfl-0.4.4/src/py/daisyfl/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/server/client_proxy.py` & `daisyfl-0.4.4/src/py/daisyfl/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/server/grpc_server/__init__.py` & `daisyfl-0.4.4/src/py/daisyfl/server/grpc_server/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/server/grpc_server/flower_service_servicer.py` & `daisyfl-0.4.4/src/py/daisyfl/server/grpc_server/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/server/grpc_server/grpc_bridge.py` & `daisyfl-0.4.4/src/py/daisyfl/server/grpc_server/grpc_bridge.py`

 * *Files 3% similar despite different names*

```diff
@@ -161,15 +161,16 @@
             self._cv.wait_for(
                 lambda: self._status in [Status.CLOSED, Status.CLIENT_MESSAGE_AVAILABLE]
             )
 
             self._raise_if_closed()
             client_message = self._client_message  # Read
             self._client_message = None  # Reset
-            self._transition(Status.AWAITING_SERVER_MESSAGE)
+            # NOTE: if connection will break after receving client_message, don't transfer to AWAITING_SERVER_MESSAGE
+            # self._transition(Status.AWAITING_SERVER_MESSAGE)
 
         if client_message is None:
             raise Exception("client_message can not be None")
         
         self.submit_client_message(client_message)
 
     def client_available(self,) -> bool:
```

### Comparing `daisyfl-0.4.3/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py` & `daisyfl-0.4.4/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/server/grpc_server/grpc_server.py` & `daisyfl-0.4.4/src/py/daisyfl/server/grpc_server/grpc_server.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/server/history.py` & `daisyfl-0.4.4/src/py/daisyfl/server/history.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/server/server.py` & `daisyfl-0.4.4/src/py/daisyfl/server/server.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/server/server_api_handler.py` & `daisyfl-0.4.4/src/py/daisyfl/server/server_api_handler.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/server/server_operator_manager.py` & `daisyfl-0.4.4/src/py/daisyfl/server/server_operator_manager.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/server/task_manager.py` & `daisyfl-0.4.4/src/py/daisyfl/server/task_manager.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/simulation/__init__.py` & `daisyfl-0.4.4/src/py/daisyfl/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/simulation/app.py` & `daisyfl-0.4.4/src/py/daisyfl/simulation/app.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/simulation/ray_transport/__init__.py` & `daisyfl-0.4.4/src/py/daisyfl/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py` & `daisyfl-0.4.4/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/src/py/daisyfl/utils/__init__.py` & `daisyfl-0.4.4/src/py/daisyfl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.3/setup.py` & `daisyfl-0.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 extras_require = \
 {':python_version < "3.8"': ['importlib-metadata>=4.0.0,<5.0.0'],
  'simulation': ['ray[default]>=2.0.0,<2.1.0']}
 
 setup_kwargs = {
     'name': 'daisyfl',
-    'version': '0.4.3',
+    'version': '0.4.4',
     'description': 'Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing',
     'long_description': "# Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing\n\n## dev mode\n1. clone the source code\n```\ngit clone https://github.com/Intelligent-Systems-Lab/daisy\n```\n2. build up environment\n```\ndocker run -it -v <daisy_source_code>:/root/daisy tcfwbper/daisyfl-dev:<version_tag> /bin/bash\n```\n3. develop<br>\n4. setup examples<br>\ndon't overwrite daisyfl dependency in this step.<br>\n```\ndocker attach <container_id>\n```\n```\ncd <example_path> && conda activate daisy\npip install <pkgs_for_your_example>\n```\n5. run examples\n\n## user mode\n1. install daisyfl\n```\npip install <daisyfl_version>\n```\n2. setup examples\n```\npip install <pkgs_for_your_example>\n```\n3. run examples",
     'author': 'tcfwbper',
     'author_email': 'b05208031@ntu.edu.tw',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Intelligent-Systems-Lab/daisy',
```

### Comparing `daisyfl-0.4.3/PKG-INFO` & `daisyfl-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daisyfl
-Version: 0.4.3
+Version: 0.4.4
 Summary: Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing
 Home-page: https://github.com/Intelligent-Systems-Lab/daisy
 License: Apache-2.0
 Author: tcfwbper
 Author-email: b05208031@ntu.edu.tw
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

