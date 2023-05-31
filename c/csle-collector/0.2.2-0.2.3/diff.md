# Comparing `tmp/csle_collector-0.2.2.tar.gz` & `tmp/csle_collector-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_collector-0.2.2.tar", last modified: Wed May 31 11:46:09 2023, max compression
+gzip compressed data, was "csle_collector-0.2.3.tar", last modified: Wed May 31 12:12:46 2023, max compression
```

## Comparing `csle_collector-0.2.2.tar` & `csle_collector-0.2.3.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:46:09.253456 csle_collector-0.2.2/
--rw-r--r--   0 kimham     (501) staff       (20)      803 2023-05-31 11:46:09.253613 csle_collector-0.2.2/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     5807 2023-03-05 07:26:30.000000 csle_collector-0.2.2/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      674 2023-02-12 08:59:32.000000 csle_collector-0.2.2/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1454 2023-05-31 11:46:09.254553 csle_collector-0.2.2/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_collector-0.2.2/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:46:09.140123 csle_collector-0.2.2/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:46:09.146719 csle_collector-0.2.2/src/csle_collector/
--rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 11:45:39.000000 csle_collector-0.2.2/src/csle_collector/__version__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:46:09.156161 csle_collector-0.2.2/src/csle_collector/client_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/client_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     9996 2023-05-31 11:11:40.000000 csle_collector-0.2.2/src/csle_collector/client_manager/client_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)    11826 2023-05-31 09:26:56.000000 csle_collector-0.2.2/src/csle_collector/client_manager/client_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)     8592 2023-05-31 09:27:14.000000 csle_collector-0.2.2/src/csle_collector/client_manager/client_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)     2179 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/client_manager/client_manager_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     4316 2023-05-24 17:43:06.000000 csle_collector-0.2.2/src/csle_collector/client_manager/client_population_metrics.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:46:09.175873 csle_collector-0.2.2/src/csle_collector/client_manager/dao/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2023-05-31 07:06:48.000000 csle_collector-0.2.2/src/csle_collector/client_manager/dao/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     2379 2023-05-31 08:44:30.000000 csle_collector-0.2.2/src/csle_collector/client_manager/dao/arrival_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     9508 2023-05-31 11:02:02.000000 csle_collector-0.2.2/src/csle_collector/client_manager/dao/client.py
--rw-r--r--   0 kimham     (501) staff       (20)      340 2023-05-31 07:06:48.000000 csle_collector-0.2.2/src/csle_collector/client_manager/dao/client_arrival_type.py
--rw-r--r--   0 kimham     (501) staff       (20)     2140 2023-05-31 08:47:06.000000 csle_collector-0.2.2/src/csle_collector/client_manager/dao/constant_arrival_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     2859 2023-05-31 08:49:42.000000 csle_collector-0.2.2/src/csle_collector/client_manager/dao/eptmp_arrival_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     1780 2023-05-31 07:06:48.000000 csle_collector-0.2.2/src/csle_collector/client_manager/dao/eptmp_rate_function.py
--rw-r--r--   0 kimham     (501) staff       (20)     2695 2023-05-31 08:50:44.000000 csle_collector-0.2.2/src/csle_collector/client_manager/dao/piece_wise_constant_arrival_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     3098 2023-05-31 08:52:02.000000 csle_collector-0.2.2/src/csle_collector/client_manager/dao/sine_arrival_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     2447 2023-05-31 08:53:06.000000 csle_collector-0.2.2/src/csle_collector/client_manager/dao/spiking_arrival_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     5539 2023-05-31 09:04:14.000000 csle_collector-0.2.2/src/csle_collector/client_manager/dao/workflow_markov_chain.py
--rw-r--r--   0 kimham     (501) staff       (20)     4932 2023-05-31 09:49:45.000000 csle_collector-0.2.2/src/csle_collector/client_manager/dao/workflow_service.py
--rw-r--r--   0 kimham     (501) staff       (20)     5268 2023-05-31 09:47:00.000000 csle_collector-0.2.2/src/csle_collector/client_manager/dao/workflows_config.py
--rw-r--r--   0 kimham     (501) staff       (20)     4064 2023-05-31 11:16:13.000000 csle_collector-0.2.2/src/csle_collector/client_manager/query_clients.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:46:09.181488 csle_collector-0.2.2/src/csle_collector/client_manager/threads/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2023-05-31 07:06:48.000000 csle_collector-0.2.2/src/csle_collector/client_manager/threads/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     6971 2023-05-31 11:09:17.000000 csle_collector-0.2.2/src/csle_collector/client_manager/threads/arrival_thread.py
--rw-r--r--   0 kimham     (501) staff       (20)      971 2023-05-31 11:06:56.000000 csle_collector-0.2.2/src/csle_collector/client_manager/threads/client_thread.py
--rw-r--r--   0 kimham     (501) staff       (20)     2374 2023-05-31 11:10:19.000000 csle_collector-0.2.2/src/csle_collector/client_manager/threads/producer_thread.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:46:09.182685 csle_collector-0.2.2/src/csle_collector/constants/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/constants/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    36309 2023-04-19 06:25:48.000000 csle_collector-0.2.2/src/csle_collector/constants/constants.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:46:09.202436 csle_collector-0.2.2/src/csle_collector/docker_stats_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2023-02-12 12:41:34.000000 csle_collector-0.2.2/src/csle_collector/docker_stats_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    12394 2023-03-15 11:36:56.000000 csle_collector-0.2.2/src/csle_collector/docker_stats_manager/docker_stats.py
--rw-r--r--   0 kimham     (501) staff       (20)    13540 2023-03-05 11:13:10.000000 csle_collector-0.2.2/src/csle_collector/docker_stats_manager/docker_stats_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     4589 2023-02-12 12:41:34.000000 csle_collector-0.2.2/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)     6193 2023-02-12 12:41:34.000000 csle_collector-0.2.2/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)     8801 2023-02-12 12:41:34.000000 csle_collector-0.2.2/src/csle_collector/docker_stats_manager/docker_stats_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     3994 2023-03-20 09:39:38.000000 csle_collector-0.2.2/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:46:09.212051 csle_collector-0.2.2/src/csle_collector/elk_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/elk_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    10740 2023-03-22 11:50:26.000000 csle_collector-0.2.2/src/csle_collector/elk_manager/elk_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     5923 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/elk_manager/elk_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)    14300 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)     1540 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/elk_manager/elk_manager_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     5768 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/elk_manager/query_elk_server.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:46:09.226262 csle_collector-0.2.2/src/csle_collector/host_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/host_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)      875 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/host_manager/failed_login_attempt.py
--rw-r--r--   0 kimham     (501) staff       (20)    65375 2023-03-31 11:14:06.000000 csle_collector-0.2.2/src/csle_collector/host_manager/host_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)    13966 2023-03-31 11:14:06.000000 csle_collector-0.2.2/src/csle_collector/host_manager/host_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)    28800 2023-03-31 11:14:06.000000 csle_collector-0.2.2/src/csle_collector/host_manager/host_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)    33850 2023-03-05 07:26:30.000000 csle_collector-0.2.2/src/csle_collector/host_manager/host_manager_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     7783 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/host_manager/host_metrics.py
--rw-r--r--   0 kimham     (501) staff       (20)    16572 2023-03-31 11:14:06.000000 csle_collector-0.2.2/src/csle_collector/host_manager/query_host_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     1292 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/host_manager/successful_login.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:46:09.230614 csle_collector-0.2.2/src/csle_collector/kafka_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/kafka_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     6616 2023-03-22 11:50:26.000000 csle_collector-0.2.2/src/csle_collector/kafka_manager/kafka_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     4116 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/kafka_manager/kafka_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)     8484 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)     1442 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/kafka_manager/kafka_manager_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     3233 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/kafka_manager/query_kafka_server.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:46:09.239003 csle_collector-0.2.2/src/csle_collector/ossec_ids_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/ossec_ids_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     2931 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/ossec_ids_manager/ossec_ids_alert.py
--rw-r--r--   0 kimham     (501) staff       (20)    10847 2023-03-16 08:28:05.000000 csle_collector-0.2.2/src/csle_collector/ossec_ids_manager/ossec_ids_alert_counters.py
--rw-r--r--   0 kimham     (501) staff       (20)    11386 2023-03-22 11:50:26.000000 csle_collector-0.2.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     7479 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)    10801 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)    13329 2022-11-30 17:44:15.000000 csle_collector-0.2.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     5377 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:46:09.244810 csle_collector-0.2.2/src/csle_collector/ryu_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/ryu_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     3936 2022-12-07 13:13:59.000000 csle_collector-0.2.2/src/csle_collector/ryu_manager/query_ryu_server.py
--rw-r--r--   0 kimham     (501) staff       (20)    18068 2023-04-19 06:25:48.000000 csle_collector-0.2.2/src/csle_collector/ryu_manager/ryu_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     4363 2022-12-07 08:23:15.000000 csle_collector-0.2.2/src/csle_collector/ryu_manager/ryu_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)     8368 2022-12-07 08:23:40.000000 csle_collector-0.2.2/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)     2086 2022-12-07 08:18:55.000000 csle_collector-0.2.2/src/csle_collector/ryu_manager/ryu_manager_util.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:46:09.250134 csle_collector-0.2.2/src/csle_collector/snort_ids_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/snort_ids_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     5787 2023-03-31 11:14:06.000000 csle_collector-0.2.2/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     7996 2023-03-31 11:14:06.000000 csle_collector-0.2.2/src/csle_collector/snort_ids_manager/snort_ids_alert.py
--rw-r--r--   0 kimham     (501) staff       (20)    11779 2023-03-31 11:14:06.000000 csle_collector-0.2.2/src/csle_collector/snort_ids_manager/snort_ids_alert_counters.py
--rw-r--r--   0 kimham     (501) staff       (20)     9176 2023-03-31 11:14:06.000000 csle_collector-0.2.2/src/csle_collector/snort_ids_manager/snort_ids_ip_alert_counters.py
--rw-r--r--   0 kimham     (501) staff       (20)    13005 2023-03-31 11:14:06.000000 csle_collector-0.2.2/src/csle_collector/snort_ids_manager/snort_ids_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     8283 2023-03-31 11:14:06.000000 csle_collector-0.2.2/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)    10801 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)    16748 2023-03-31 11:14:06.000000 csle_collector-0.2.2/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     4288 2023-03-31 11:14:06.000000 csle_collector-0.2.2/src/csle_collector/snort_ids_manager/snort_ids_rule_counters.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:46:09.253094 csle_collector-0.2.2/src/csle_collector/traffic_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/traffic_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     2534 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/traffic_manager/query_traffic_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     7492 2023-05-31 11:44:33.000000 csle_collector-0.2.2/src/csle_collector/traffic_manager/traffic_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     3087 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/traffic_manager/traffic_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)     5596 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)     1477 2022-11-28 13:00:49.000000 csle_collector-0.2.2/src/csle_collector/traffic_manager/traffic_manager_util.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:46:09.150284 csle_collector-0.2.2/src/csle_collector.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      803 2023-05-31 11:46:08.000000 csle_collector-0.2.2/src/csle_collector.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     5103 2023-05-31 11:46:09.000000 csle_collector-0.2.2/src/csle_collector.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 11:46:08.000000 csle_collector-0.2.2/src/csle_collector.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:03:14.000000 csle_collector-0.2.2/src/csle_collector.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      293 2023-05-31 11:46:08.000000 csle_collector-0.2.2/src/csle_collector.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)       15 2023-05-31 11:46:09.000000 csle_collector-0.2.2/src/csle_collector.egg-info/top_level.txt
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:12:46.907273 csle_collector-0.2.3/
+-rw-r--r--   0 kimham     (501) staff       (20)      803 2023-05-31 12:12:46.908196 csle_collector-0.2.3/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)     5807 2023-03-05 07:26:30.000000 csle_collector-0.2.3/README.md
+-rw-r--r--   0 kimham     (501) staff       (20)      674 2023-02-12 08:59:32.000000 csle_collector-0.2.3/pyproject.toml
+-rw-r--r--   0 kimham     (501) staff       (20)     1454 2023-05-31 12:12:46.909636 csle_collector-0.2.3/setup.cfg
+-rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_collector-0.2.3/setup.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:12:46.845627 csle_collector-0.2.3/src/
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:12:46.849662 csle_collector-0.2.3/src/csle_collector/
+-rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 12:12:15.000000 csle_collector-0.2.3/src/csle_collector/__version__.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:12:46.855355 csle_collector-0.2.3/src/csle_collector/client_manager/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/client_manager/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     9996 2023-05-31 11:11:40.000000 csle_collector-0.2.3/src/csle_collector/client_manager/client_manager.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5660 2023-05-31 12:09:00.000000 csle_collector-0.2.3/src/csle_collector/client_manager/client_manager_pb2.py
+-rw-r--r--   0 kimham     (501) staff       (20)     8592 2023-05-31 12:09:30.000000 csle_collector-0.2.3/src/csle_collector/client_manager/client_manager_pb2_grpc.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2179 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/client_manager/client_manager_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4316 2023-05-24 17:43:06.000000 csle_collector-0.2.3/src/csle_collector/client_manager/client_population_metrics.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:12:46.862187 csle_collector-0.2.3/src/csle_collector/client_manager/dao/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2023-05-31 07:06:48.000000 csle_collector-0.2.3/src/csle_collector/client_manager/dao/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2379 2023-05-31 08:44:30.000000 csle_collector-0.2.3/src/csle_collector/client_manager/dao/arrival_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     9508 2023-05-31 11:02:02.000000 csle_collector-0.2.3/src/csle_collector/client_manager/dao/client.py
+-rw-r--r--   0 kimham     (501) staff       (20)      340 2023-05-31 07:06:48.000000 csle_collector-0.2.3/src/csle_collector/client_manager/dao/client_arrival_type.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2140 2023-05-31 08:47:06.000000 csle_collector-0.2.3/src/csle_collector/client_manager/dao/constant_arrival_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2859 2023-05-31 08:49:42.000000 csle_collector-0.2.3/src/csle_collector/client_manager/dao/eptmp_arrival_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1780 2023-05-31 07:06:48.000000 csle_collector-0.2.3/src/csle_collector/client_manager/dao/eptmp_rate_function.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2695 2023-05-31 08:50:44.000000 csle_collector-0.2.3/src/csle_collector/client_manager/dao/piece_wise_constant_arrival_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3098 2023-05-31 08:52:02.000000 csle_collector-0.2.3/src/csle_collector/client_manager/dao/sine_arrival_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2447 2023-05-31 08:53:06.000000 csle_collector-0.2.3/src/csle_collector/client_manager/dao/spiking_arrival_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5539 2023-05-31 09:04:14.000000 csle_collector-0.2.3/src/csle_collector/client_manager/dao/workflow_markov_chain.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5131 2023-05-31 12:11:16.000000 csle_collector-0.2.3/src/csle_collector/client_manager/dao/workflow_service.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5268 2023-05-31 09:47:00.000000 csle_collector-0.2.3/src/csle_collector/client_manager/dao/workflows_config.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4064 2023-05-31 11:16:13.000000 csle_collector-0.2.3/src/csle_collector/client_manager/query_clients.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:12:46.864033 csle_collector-0.2.3/src/csle_collector/client_manager/threads/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2023-05-31 07:06:48.000000 csle_collector-0.2.3/src/csle_collector/client_manager/threads/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     6971 2023-05-31 11:09:17.000000 csle_collector-0.2.3/src/csle_collector/client_manager/threads/arrival_thread.py
+-rw-r--r--   0 kimham     (501) staff       (20)      971 2023-05-31 11:06:56.000000 csle_collector-0.2.3/src/csle_collector/client_manager/threads/client_thread.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2374 2023-05-31 11:10:19.000000 csle_collector-0.2.3/src/csle_collector/client_manager/threads/producer_thread.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:12:46.864729 csle_collector-0.2.3/src/csle_collector/constants/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/constants/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    36309 2023-04-19 06:25:48.000000 csle_collector-0.2.3/src/csle_collector/constants/constants.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:12:46.870682 csle_collector-0.2.3/src/csle_collector/docker_stats_manager/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2023-02-12 12:41:34.000000 csle_collector-0.2.3/src/csle_collector/docker_stats_manager/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    12394 2023-03-15 11:36:56.000000 csle_collector-0.2.3/src/csle_collector/docker_stats_manager/docker_stats.py
+-rw-r--r--   0 kimham     (501) staff       (20)    13540 2023-03-05 11:13:10.000000 csle_collector-0.2.3/src/csle_collector/docker_stats_manager/docker_stats_manager.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4589 2023-02-12 12:41:34.000000 csle_collector-0.2.3/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py
+-rw-r--r--   0 kimham     (501) staff       (20)     6193 2023-02-12 12:41:34.000000 csle_collector-0.2.3/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py
+-rw-r--r--   0 kimham     (501) staff       (20)     8801 2023-02-12 12:41:34.000000 csle_collector-0.2.3/src/csle_collector/docker_stats_manager/docker_stats_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3994 2023-03-20 09:39:38.000000 csle_collector-0.2.3/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:12:46.874793 csle_collector-0.2.3/src/csle_collector/elk_manager/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/elk_manager/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)    10740 2023-03-22 11:50:26.000000 csle_collector-0.2.3/src/csle_collector/elk_manager/elk_manager.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5923 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/elk_manager/elk_manager_pb2.py
+-rw-r--r--   0 kimham     (501) staff       (20)    14300 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1540 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/elk_manager/elk_manager_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5768 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/elk_manager/query_elk_server.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:12:46.880577 csle_collector-0.2.3/src/csle_collector/host_manager/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/host_manager/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)      875 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/host_manager/failed_login_attempt.py
+-rw-r--r--   0 kimham     (501) staff       (20)    65375 2023-03-31 11:14:06.000000 csle_collector-0.2.3/src/csle_collector/host_manager/host_manager.py
+-rw-r--r--   0 kimham     (501) staff       (20)    13966 2023-03-31 11:14:06.000000 csle_collector-0.2.3/src/csle_collector/host_manager/host_manager_pb2.py
+-rw-r--r--   0 kimham     (501) staff       (20)    28800 2023-03-31 11:14:06.000000 csle_collector-0.2.3/src/csle_collector/host_manager/host_manager_pb2_grpc.py
+-rw-r--r--   0 kimham     (501) staff       (20)    33850 2023-03-05 07:26:30.000000 csle_collector-0.2.3/src/csle_collector/host_manager/host_manager_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)     7783 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/host_manager/host_metrics.py
+-rw-r--r--   0 kimham     (501) staff       (20)    16572 2023-03-31 11:14:06.000000 csle_collector-0.2.3/src/csle_collector/host_manager/query_host_manager.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1292 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/host_manager/successful_login.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:12:46.883428 csle_collector-0.2.3/src/csle_collector/kafka_manager/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/kafka_manager/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     6616 2023-03-22 11:50:26.000000 csle_collector-0.2.3/src/csle_collector/kafka_manager/kafka_manager.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4116 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/kafka_manager/kafka_manager_pb2.py
+-rw-r--r--   0 kimham     (501) staff       (20)     8484 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1442 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/kafka_manager/kafka_manager_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3233 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/kafka_manager/query_kafka_server.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:12:46.888605 csle_collector-0.2.3/src/csle_collector/ossec_ids_manager/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/ossec_ids_manager/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2931 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/ossec_ids_manager/ossec_ids_alert.py
+-rw-r--r--   0 kimham     (501) staff       (20)    10847 2023-03-16 08:28:05.000000 csle_collector-0.2.3/src/csle_collector/ossec_ids_manager/ossec_ids_alert_counters.py
+-rw-r--r--   0 kimham     (501) staff       (20)    11386 2023-03-22 11:50:26.000000 csle_collector-0.2.3/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py
+-rw-r--r--   0 kimham     (501) staff       (20)     7479 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py
+-rw-r--r--   0 kimham     (501) staff       (20)    10801 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py
+-rw-r--r--   0 kimham     (501) staff       (20)    13329 2022-11-30 17:44:15.000000 csle_collector-0.2.3/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5377 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:12:46.893688 csle_collector-0.2.3/src/csle_collector/ryu_manager/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/ryu_manager/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3936 2022-12-07 13:13:59.000000 csle_collector-0.2.3/src/csle_collector/ryu_manager/query_ryu_server.py
+-rw-r--r--   0 kimham     (501) staff       (20)    18068 2023-04-19 06:25:48.000000 csle_collector-0.2.3/src/csle_collector/ryu_manager/ryu_manager.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4363 2022-12-07 08:23:15.000000 csle_collector-0.2.3/src/csle_collector/ryu_manager/ryu_manager_pb2.py
+-rw-r--r--   0 kimham     (501) staff       (20)     8368 2022-12-07 08:23:40.000000 csle_collector-0.2.3/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2086 2022-12-07 08:18:55.000000 csle_collector-0.2.3/src/csle_collector/ryu_manager/ryu_manager_util.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:12:46.901510 csle_collector-0.2.3/src/csle_collector/snort_ids_manager/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/snort_ids_manager/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5787 2023-03-31 11:14:06.000000 csle_collector-0.2.3/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py
+-rw-r--r--   0 kimham     (501) staff       (20)     7996 2023-03-31 11:14:06.000000 csle_collector-0.2.3/src/csle_collector/snort_ids_manager/snort_ids_alert.py
+-rw-r--r--   0 kimham     (501) staff       (20)    11779 2023-03-31 11:14:06.000000 csle_collector-0.2.3/src/csle_collector/snort_ids_manager/snort_ids_alert_counters.py
+-rw-r--r--   0 kimham     (501) staff       (20)     9176 2023-03-31 11:14:06.000000 csle_collector-0.2.3/src/csle_collector/snort_ids_manager/snort_ids_ip_alert_counters.py
+-rw-r--r--   0 kimham     (501) staff       (20)    13005 2023-03-31 11:14:06.000000 csle_collector-0.2.3/src/csle_collector/snort_ids_manager/snort_ids_manager.py
+-rw-r--r--   0 kimham     (501) staff       (20)     8283 2023-03-31 11:14:06.000000 csle_collector-0.2.3/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py
+-rw-r--r--   0 kimham     (501) staff       (20)    10801 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py
+-rw-r--r--   0 kimham     (501) staff       (20)    16748 2023-03-31 11:14:06.000000 csle_collector-0.2.3/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)     4288 2023-03-31 11:14:06.000000 csle_collector-0.2.3/src/csle_collector/snort_ids_manager/snort_ids_rule_counters.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:12:46.906192 csle_collector-0.2.3/src/csle_collector/traffic_manager/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/traffic_manager/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)     2534 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/traffic_manager/query_traffic_manager.py
+-rw-r--r--   0 kimham     (501) staff       (20)     7492 2023-05-31 11:44:33.000000 csle_collector-0.2.3/src/csle_collector/traffic_manager/traffic_manager.py
+-rw-r--r--   0 kimham     (501) staff       (20)     3087 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/traffic_manager/traffic_manager_pb2.py
+-rw-r--r--   0 kimham     (501) staff       (20)     5596 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py
+-rw-r--r--   0 kimham     (501) staff       (20)     1477 2022-11-28 13:00:49.000000 csle_collector-0.2.3/src/csle_collector/traffic_manager/traffic_manager_util.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 12:12:46.851701 csle_collector-0.2.3/src/csle_collector.egg-info/
+-rw-r--r--   0 kimham     (501) staff       (20)      803 2023-05-31 12:12:46.000000 csle_collector-0.2.3/src/csle_collector.egg-info/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)     5103 2023-05-31 12:12:46.000000 csle_collector-0.2.3/src/csle_collector.egg-info/SOURCES.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 12:12:46.000000 csle_collector-0.2.3/src/csle_collector.egg-info/dependency_links.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:03:14.000000 csle_collector-0.2.3/src/csle_collector.egg-info/not-zip-safe
+-rw-r--r--   0 kimham     (501) staff       (20)      293 2023-05-31 12:12:46.000000 csle_collector-0.2.3/src/csle_collector.egg-info/requires.txt
+-rw-r--r--   0 kimham     (501) staff       (20)       15 2023-05-31 12:12:46.000000 csle_collector-0.2.3/src/csle_collector.egg-info/top_level.txt
```

### Comparing `csle_collector-0.2.2/PKG-INFO` & `csle_collector-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_collector
-Version: 0.2.2
+Version: 0.2.3
 Summary: Scripts for data collection in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_collector-0.2.2/README.md` & `csle_collector-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/pyproject.toml` & `csle_collector-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/setup.cfg` & `csle_collector-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/client_manager/client_manager.py` & `csle_collector-0.2.3/src/csle_collector/client_manager/client_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/client_manager/client_manager_pb2_grpc.py` & `csle_collector-0.2.3/src/csle_collector/client_manager/client_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/client_manager/client_manager_util.py` & `csle_collector-0.2.3/src/csle_collector/client_manager/client_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/client_manager/client_population_metrics.py` & `csle_collector-0.2.3/src/csle_collector/client_manager/client_population_metrics.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/client_manager/dao/arrival_config.py` & `csle_collector-0.2.3/src/csle_collector/client_manager/dao/arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/client_manager/dao/client.py` & `csle_collector-0.2.3/src/csle_collector/client_manager/dao/client.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/client_manager/dao/constant_arrival_config.py` & `csle_collector-0.2.3/src/csle_collector/client_manager/dao/constant_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/client_manager/dao/eptmp_arrival_config.py` & `csle_collector-0.2.3/src/csle_collector/client_manager/dao/eptmp_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/client_manager/dao/eptmp_rate_function.py` & `csle_collector-0.2.3/src/csle_collector/client_manager/dao/eptmp_rate_function.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/client_manager/dao/piece_wise_constant_arrival_config.py` & `csle_collector-0.2.3/src/csle_collector/client_manager/dao/piece_wise_constant_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/client_manager/dao/sine_arrival_config.py` & `csle_collector-0.2.3/src/csle_collector/client_manager/dao/sine_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/client_manager/dao/spiking_arrival_config.py` & `csle_collector-0.2.3/src/csle_collector/client_manager/dao/spiking_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/client_manager/dao/workflow_markov_chain.py` & `csle_collector-0.2.3/src/csle_collector/client_manager/dao/workflow_markov_chain.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/client_manager/dao/workflow_service.py` & `csle_collector-0.2.3/src/csle_collector/client_manager/dao/workflow_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,31 +105,35 @@
                                                                                     ip_first_octet=ip_first_octet)
         return config
 
     def to_grpc_object(self) -> csle_collector.client_manager.client_manager_pb2.WorkflowServiceDTO:
         """
         :return: a GRPC serializable version of the object
         """
+        ips = []
+        commands = []
+        for i in range(len(self.ips_and_commands)):
+            ips.append(self.ips_and_commands[i][0])
+            commands.append(csle_collector.client_manager.client_manager_pb2.NodeCommandsDTO(
+                commands=self.ips_and_commands[i][1]))
         return csle_collector.client_manager.client_manager_pb2.WorkflowServiceDTO(
-            id=self.id, ips = list(map(lambda x: x[0], self.ips_and_commands)),
-            commands = list(map(lambda x: x[1], self.ips_and_commands))
-        )
+            id=self.id, ips = ips, commands = commands)
 
     @staticmethod
     def from_grpc_object(obj: csle_collector.client_manager.client_manager_pb2.WorkflowServiceDTO) \
             -> "WorkflowService":
         """
         Instantiates the object from a GRPC DTO
 
         :param obj: the object to instantiate from
         :return: the instantiated object
         """
         ips_and_commands = []
         for i in range(obj.ips):
-            ips_and_commands.append((obj.ips[i], obj.commands[i]))
+            ips_and_commands.append((obj.ips[i], obj.commands[i].commands))
         return WorkflowService(id=obj.id, ips_and_commands=ips_and_commands)
 
     def get_commands(self) -> List[str]:
         """
         :return: the list of commands for the service
         """
         commands = []
```

### Comparing `csle_collector-0.2.2/src/csle_collector/client_manager/dao/workflows_config.py` & `csle_collector-0.2.3/src/csle_collector/client_manager/dao/workflows_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/client_manager/query_clients.py` & `csle_collector-0.2.3/src/csle_collector/client_manager/query_clients.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/client_manager/threads/arrival_thread.py` & `csle_collector-0.2.3/src/csle_collector/client_manager/threads/arrival_thread.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/client_manager/threads/client_thread.py` & `csle_collector-0.2.3/src/csle_collector/client_manager/threads/client_thread.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/client_manager/threads/producer_thread.py` & `csle_collector-0.2.3/src/csle_collector/client_manager/threads/producer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/constants/constants.py` & `csle_collector-0.2.3/src/csle_collector/constants/constants.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/docker_stats_manager/docker_stats.py` & `csle_collector-0.2.3/src/csle_collector/docker_stats_manager/docker_stats.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/docker_stats_manager/docker_stats_manager.py` & `csle_collector-0.2.3/src/csle_collector/docker_stats_manager/docker_stats_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py` & `csle_collector-0.2.3/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py` & `csle_collector-0.2.3/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/docker_stats_manager/docker_stats_util.py` & `csle_collector-0.2.3/src/csle_collector/docker_stats_manager/docker_stats_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py` & `csle_collector-0.2.3/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/elk_manager/elk_manager.py` & `csle_collector-0.2.3/src/csle_collector/elk_manager/elk_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/elk_manager/elk_manager_pb2.py` & `csle_collector-0.2.3/src/csle_collector/elk_manager/elk_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py` & `csle_collector-0.2.3/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/elk_manager/elk_manager_util.py` & `csle_collector-0.2.3/src/csle_collector/elk_manager/elk_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/elk_manager/query_elk_server.py` & `csle_collector-0.2.3/src/csle_collector/elk_manager/query_elk_server.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/host_manager/failed_login_attempt.py` & `csle_collector-0.2.3/src/csle_collector/host_manager/failed_login_attempt.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/host_manager/host_manager.py` & `csle_collector-0.2.3/src/csle_collector/host_manager/host_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/host_manager/host_manager_pb2.py` & `csle_collector-0.2.3/src/csle_collector/host_manager/host_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/host_manager/host_manager_pb2_grpc.py` & `csle_collector-0.2.3/src/csle_collector/host_manager/host_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/host_manager/host_manager_util.py` & `csle_collector-0.2.3/src/csle_collector/host_manager/host_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/host_manager/host_metrics.py` & `csle_collector-0.2.3/src/csle_collector/host_manager/host_metrics.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/host_manager/query_host_manager.py` & `csle_collector-0.2.3/src/csle_collector/host_manager/query_host_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/host_manager/successful_login.py` & `csle_collector-0.2.3/src/csle_collector/host_manager/successful_login.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/kafka_manager/kafka_manager.py` & `csle_collector-0.2.3/src/csle_collector/kafka_manager/kafka_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/kafka_manager/kafka_manager_pb2.py` & `csle_collector-0.2.3/src/csle_collector/kafka_manager/kafka_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py` & `csle_collector-0.2.3/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/kafka_manager/kafka_manager_util.py` & `csle_collector-0.2.3/src/csle_collector/kafka_manager/kafka_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/kafka_manager/query_kafka_server.py` & `csle_collector-0.2.3/src/csle_collector/kafka_manager/query_kafka_server.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/ossec_ids_manager/ossec_ids_alert.py` & `csle_collector-0.2.3/src/csle_collector/ossec_ids_manager/ossec_ids_alert.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/ossec_ids_manager/ossec_ids_alert_counters.py` & `csle_collector-0.2.3/src/csle_collector/ossec_ids_manager/ossec_ids_alert_counters.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py` & `csle_collector-0.2.3/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py` & `csle_collector-0.2.3/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py` & `csle_collector-0.2.3/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py` & `csle_collector-0.2.3/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py` & `csle_collector-0.2.3/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/ryu_manager/query_ryu_server.py` & `csle_collector-0.2.3/src/csle_collector/ryu_manager/query_ryu_server.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/ryu_manager/ryu_manager.py` & `csle_collector-0.2.3/src/csle_collector/ryu_manager/ryu_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/ryu_manager/ryu_manager_pb2.py` & `csle_collector-0.2.3/src/csle_collector/ryu_manager/ryu_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py` & `csle_collector-0.2.3/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/ryu_manager/ryu_manager_util.py` & `csle_collector-0.2.3/src/csle_collector/ryu_manager/ryu_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py` & `csle_collector-0.2.3/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/snort_ids_manager/snort_ids_alert.py` & `csle_collector-0.2.3/src/csle_collector/snort_ids_manager/snort_ids_alert.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/snort_ids_manager/snort_ids_alert_counters.py` & `csle_collector-0.2.3/src/csle_collector/snort_ids_manager/snort_ids_alert_counters.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/snort_ids_manager/snort_ids_ip_alert_counters.py` & `csle_collector-0.2.3/src/csle_collector/snort_ids_manager/snort_ids_ip_alert_counters.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/snort_ids_manager/snort_ids_manager.py` & `csle_collector-0.2.3/src/csle_collector/snort_ids_manager/snort_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py` & `csle_collector-0.2.3/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py` & `csle_collector-0.2.3/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py` & `csle_collector-0.2.3/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/snort_ids_manager/snort_ids_rule_counters.py` & `csle_collector-0.2.3/src/csle_collector/snort_ids_manager/snort_ids_rule_counters.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/traffic_manager/query_traffic_manager.py` & `csle_collector-0.2.3/src/csle_collector/traffic_manager/query_traffic_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/traffic_manager/traffic_manager.py` & `csle_collector-0.2.3/src/csle_collector/traffic_manager/traffic_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/traffic_manager/traffic_manager_pb2.py` & `csle_collector-0.2.3/src/csle_collector/traffic_manager/traffic_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py` & `csle_collector-0.2.3/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector/traffic_manager/traffic_manager_util.py` & `csle_collector-0.2.3/src/csle_collector/traffic_manager/traffic_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.2.2/src/csle_collector.egg-info/PKG-INFO` & `csle_collector-0.2.3/src/csle_collector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-collector
-Version: 0.2.2
+Version: 0.2.3
 Summary: Scripts for data collection in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_collector-0.2.2/src/csle_collector.egg-info/SOURCES.txt` & `csle_collector-0.2.3/src/csle_collector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

