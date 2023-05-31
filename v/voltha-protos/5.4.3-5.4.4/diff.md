# Comparing `tmp/voltha-protos-5.4.3.tar.gz` & `tmp/voltha-protos-5.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/voltha-protos-5.4.3.tar", last modified: Wed May 17 20:37:55 2023, max compression
+gzip compressed data, was "dist/voltha-protos-5.4.4.tar", last modified: Wed May 31 16:03:31 2023, max compression
```

## Comparing `voltha-protos-5.4.3.tar` & `voltha-protos-5.4.4.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      635 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/PKG-INFO
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     3151 2023-05-17 20:37:18.000000 voltha-protos-5.4.3/README.md
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     1663 2023-05-17 20:37:18.000000 voltha-protos-5.4.3/setup.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       38 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/setup.cfg
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)       17 2023-05-17 20:37:18.000000 voltha-protos-5.4.3/MANIFEST.in
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/python/
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/python/voltha_protos/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:45.000000 voltha-protos-5.4.3/python/voltha_protos/ietf_interfaces_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19060 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/omci_alarm_db_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    25293 2023-05-17 20:37:45.000000 voltha-protos-5.4.3/python/voltha_protos/inter_adapter_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    64403 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/events_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19758 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/ext_config_pb2.py
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)      622 2023-05-17 20:37:18.000000 voltha-protos-5.4.3/python/voltha_protos/__init__.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    59478 2023-05-17 20:37:43.000000 voltha-protos-5.4.3/python/voltha_protos/adapter_service_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    13326 2023-05-17 20:37:45.000000 voltha-protos-5.4.3/python/voltha_protos/logical_device_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/core_adapter_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    48518 2023-05-17 20:37:47.000000 voltha-protos-5.4.3/python/voltha_protos/voltha_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/device_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   108159 2023-05-17 20:37:47.000000 voltha-protos-5.4.3/python/voltha_protos/voltha_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/omci_test_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4572 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/core_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/omci_mib_db_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4295 2023-05-17 20:37:45.000000 voltha-protos-5.4.3/python/voltha_protos/extensions_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    16809 2023-05-17 20:37:45.000000 voltha-protos-5.4.3/python/voltha_protos/ietf_interfaces_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5050 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/omci_test_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:45.000000 voltha-protos-5.4.3/python/voltha_protos/logical_device_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5344 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/onu_inter_adapter_service_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:43.000000 voltha-protos-5.4.3/python/voltha_protos/common_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:43.000000 voltha-protos-5.4.3/python/voltha_protos/adapter_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   421230 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/openflow_13_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   106603 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/device_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/ext_config_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    49438 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/core_adapter_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:45.000000 voltha-protos-5.4.3/python/voltha_protos/inter_adapter_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    40916 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/core_services_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4707 2023-05-17 20:37:45.000000 voltha-protos-5.4.3/python/voltha_protos/health_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    96862 2023-05-17 20:37:47.000000 voltha-protos-5.4.3/python/voltha_protos/tech_profile_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4435 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/olt_inter_adapter_service_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/core_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/events_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    16961 2023-05-17 20:37:43.000000 voltha-protos-5.4.3/python/voltha_protos/common_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19653 2023-05-17 20:37:43.000000 voltha-protos-5.4.3/python/voltha_protos/adapter_service_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    13096 2023-05-17 20:37:44.000000 voltha-protos-5.4.3/python/voltha_protos/core_services_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/openflow_13_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8405 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/olt_inter_adapter_service_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9978 2023-05-17 20:37:43.000000 voltha-protos-5.4.3/python/voltha_protos/adapter_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   162370 2023-05-17 20:37:45.000000 voltha-protos-5.4.3/python/voltha_protos/extensions_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    52525 2023-05-17 20:37:47.000000 voltha-protos-5.4.3/python/voltha_protos/openolt_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2588 2023-05-17 20:37:45.000000 voltha-protos-5.4.3/python/voltha_protos/health_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    18434 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/omci_mib_db_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11674 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/onu_inter_adapter_service_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   247532 2023-05-17 20:37:47.000000 voltha-protos-5.4.3/python/voltha_protos/openolt_pb2.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:47.000000 voltha-protos-5.4.3/python/voltha_protos/tech_profile_pb2_grpc.py
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-17 20:37:46.000000 voltha-protos-5.4.3/python/voltha_protos/omci_alarm_db_pb2_grpc.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/python/test/
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)      622 2023-05-17 20:37:18.000000 voltha-protos-5.4.3/python/test/__init__.py
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     1007 2023-05-17 20:37:18.000000 voltha-protos-5.4.3/python/test/test_protos.py
-drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/python/voltha_protos.egg-info/
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      635 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/python/voltha_protos.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        1 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/python/voltha_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2302 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/python/voltha_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       86 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/python/voltha_protos.egg-info/requires.txt
--rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       19 2023-05-17 20:37:55.000000 voltha-protos-5.4.3/python/voltha_protos.egg-info/top_level.txt
--rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        6 2023-05-17 20:37:18.000000 voltha-protos-5.4.3/VERSION
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-05-31 16:03:31.000000 voltha-protos-5.4.4/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      635 2023-05-31 16:03:31.000000 voltha-protos-5.4.4/PKG-INFO
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     3151 2023-05-31 16:02:54.000000 voltha-protos-5.4.4/README.md
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     1663 2023-05-31 16:02:54.000000 voltha-protos-5.4.4/setup.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       38 2023-05-31 16:03:31.000000 voltha-protos-5.4.4/setup.cfg
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)       17 2023-05-31 16:02:54.000000 voltha-protos-5.4.4/MANIFEST.in
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-05-31 16:03:31.000000 voltha-protos-5.4.4/python/
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-05-31 16:03:31.000000 voltha-protos-5.4.4/python/voltha_protos/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-31 16:03:22.000000 voltha-protos-5.4.4/python/voltha_protos/ietf_interfaces_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19060 2023-05-31 16:03:22.000000 voltha-protos-5.4.4/python/voltha_protos/omci_alarm_db_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    25293 2023-05-31 16:03:22.000000 voltha-protos-5.4.4/python/voltha_protos/inter_adapter_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    64403 2023-05-31 16:03:21.000000 voltha-protos-5.4.4/python/voltha_protos/events_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19758 2023-05-31 16:03:21.000000 voltha-protos-5.4.4/python/voltha_protos/ext_config_pb2.py
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)      622 2023-05-31 16:02:54.000000 voltha-protos-5.4.4/python/voltha_protos/__init__.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    59478 2023-05-31 16:03:20.000000 voltha-protos-5.4.4/python/voltha_protos/adapter_service_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    13326 2023-05-31 16:03:22.000000 voltha-protos-5.4.4/python/voltha_protos/logical_device_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-31 16:03:20.000000 voltha-protos-5.4.4/python/voltha_protos/core_adapter_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    48518 2023-05-31 16:03:24.000000 voltha-protos-5.4.4/python/voltha_protos/voltha_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-31 16:03:21.000000 voltha-protos-5.4.4/python/voltha_protos/device_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   108159 2023-05-31 16:03:24.000000 voltha-protos-5.4.4/python/voltha_protos/voltha_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-31 16:03:23.000000 voltha-protos-5.4.4/python/voltha_protos/omci_test_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4572 2023-05-31 16:03:20.000000 voltha-protos-5.4.4/python/voltha_protos/core_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-31 16:03:23.000000 voltha-protos-5.4.4/python/voltha_protos/omci_mib_db_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4295 2023-05-31 16:03:21.000000 voltha-protos-5.4.4/python/voltha_protos/extensions_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    16809 2023-05-31 16:03:22.000000 voltha-protos-5.4.4/python/voltha_protos/ietf_interfaces_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5050 2023-05-31 16:03:23.000000 voltha-protos-5.4.4/python/voltha_protos/omci_test_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-31 16:03:22.000000 voltha-protos-5.4.4/python/voltha_protos/logical_device_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     5344 2023-05-31 16:03:23.000000 voltha-protos-5.4.4/python/voltha_protos/onu_inter_adapter_service_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-31 16:03:20.000000 voltha-protos-5.4.4/python/voltha_protos/common_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-31 16:03:20.000000 voltha-protos-5.4.4/python/voltha_protos/adapter_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   421230 2023-05-31 16:03:23.000000 voltha-protos-5.4.4/python/voltha_protos/openflow_13_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   106603 2023-05-31 16:03:21.000000 voltha-protos-5.4.4/python/voltha_protos/device_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-31 16:03:21.000000 voltha-protos-5.4.4/python/voltha_protos/ext_config_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    49438 2023-05-31 16:03:20.000000 voltha-protos-5.4.4/python/voltha_protos/core_adapter_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-31 16:03:22.000000 voltha-protos-5.4.4/python/voltha_protos/inter_adapter_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    40916 2023-05-31 16:03:21.000000 voltha-protos-5.4.4/python/voltha_protos/core_services_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4707 2023-05-31 16:03:21.000000 voltha-protos-5.4.4/python/voltha_protos/health_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    96862 2023-05-31 16:03:24.000000 voltha-protos-5.4.4/python/voltha_protos/tech_profile_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     4435 2023-05-31 16:03:22.000000 voltha-protos-5.4.4/python/voltha_protos/olt_inter_adapter_service_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-31 16:03:20.000000 voltha-protos-5.4.4/python/voltha_protos/core_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-31 16:03:21.000000 voltha-protos-5.4.4/python/voltha_protos/events_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    16961 2023-05-31 16:03:20.000000 voltha-protos-5.4.4/python/voltha_protos/common_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    19653 2023-05-31 16:03:20.000000 voltha-protos-5.4.4/python/voltha_protos/adapter_service_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    13096 2023-05-31 16:03:21.000000 voltha-protos-5.4.4/python/voltha_protos/core_services_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-31 16:03:23.000000 voltha-protos-5.4.4/python/voltha_protos/openflow_13_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     8405 2023-05-31 16:03:22.000000 voltha-protos-5.4.4/python/voltha_protos/olt_inter_adapter_service_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     9978 2023-05-31 16:03:20.000000 voltha-protos-5.4.4/python/voltha_protos/adapter_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   162370 2023-05-31 16:03:21.000000 voltha-protos-5.4.4/python/voltha_protos/extensions_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    52525 2023-05-31 16:03:23.000000 voltha-protos-5.4.4/python/voltha_protos/openolt_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2588 2023-05-31 16:03:21.000000 voltha-protos-5.4.4/python/voltha_protos/health_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    18434 2023-05-31 16:03:23.000000 voltha-protos-5.4.4/python/voltha_protos/omci_mib_db_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)    11674 2023-05-31 16:03:23.000000 voltha-protos-5.4.4/python/voltha_protos/onu_inter_adapter_service_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)   247532 2023-05-31 16:03:23.000000 voltha-protos-5.4.4/python/voltha_protos/openolt_pb2.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-31 16:03:24.000000 voltha-protos-5.4.4/python/voltha_protos/tech_profile_pb2_grpc.py
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      159 2023-05-31 16:03:22.000000 voltha-protos-5.4.4/python/voltha_protos/omci_alarm_db_pb2_grpc.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-05-31 16:03:31.000000 voltha-protos-5.4.4/python/test/
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)      622 2023-05-31 16:02:54.000000 voltha-protos-5.4.4/python/test/__init__.py
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)     1007 2023-05-31 16:02:54.000000 voltha-protos-5.4.4/python/test/test_protos.py
+drwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        0 2023-05-31 16:03:31.000000 voltha-protos-5.4.4/python/voltha_protos.egg-info/
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)      635 2023-05-31 16:03:31.000000 voltha-protos-5.4.4/python/voltha_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)        1 2023-05-31 16:03:31.000000 voltha-protos-5.4.4/python/voltha_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)     2302 2023-05-31 16:03:31.000000 voltha-protos-5.4.4/python/voltha_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       86 2023-05-31 16:03:31.000000 voltha-protos-5.4.4/python/voltha_protos.egg-info/requires.txt
+-rw-rw-r--   0 jenkins   (1001) jenkins   (1001)       19 2023-05-31 16:03:31.000000 voltha-protos-5.4.4/python/voltha_protos.egg-info/top_level.txt
+-rwxrwxr-x   0 jenkins   (1001) jenkins   (1001)        6 2023-05-31 16:02:54.000000 voltha-protos-5.4.4/VERSION
```

### Comparing `voltha-protos-5.4.3/PKG-INFO` & `voltha-protos-5.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: voltha-protos
-Version: 5.4.3
+Version: 5.4.4
 Summary: Protobuf interface definitions
 Home-page: https://gerrit.opencord.org/gitweb?p=voltha-protos.git
 Author: VOLTHA project
 Author-email: voltha-dev@opencord.org
 License: Apache Software License
 Description: UNKNOWN
 Keywords: protobuf voltha
```

### Comparing `voltha-protos-5.4.3/README.md` & `voltha-protos-5.4.4/README.md`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/setup.py` & `voltha-protos-5.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/omci_alarm_db_pb2.py` & `voltha-protos-5.4.4/python/voltha_protos/omci_alarm_db_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/inter_adapter_pb2.py` & `voltha-protos-5.4.4/python/voltha_protos/inter_adapter_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/events_pb2.py` & `voltha-protos-5.4.4/python/voltha_protos/events_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/ext_config_pb2.py` & `voltha-protos-5.4.4/python/voltha_protos/ext_config_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/__init__.py` & `voltha-protos-5.4.4/python/voltha_protos/__init__.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/adapter_service_pb2_grpc.py` & `voltha-protos-5.4.4/python/voltha_protos/adapter_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/logical_device_pb2.py` & `voltha-protos-5.4.4/python/voltha_protos/logical_device_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/voltha_pb2.py` & `voltha-protos-5.4.4/python/voltha_protos/voltha_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/voltha_pb2_grpc.py` & `voltha-protos-5.4.4/python/voltha_protos/voltha_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/core_pb2.py` & `voltha-protos-5.4.4/python/voltha_protos/core_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/extensions_pb2_grpc.py` & `voltha-protos-5.4.4/python/voltha_protos/extensions_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/ietf_interfaces_pb2.py` & `voltha-protos-5.4.4/python/voltha_protos/ietf_interfaces_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/omci_test_pb2.py` & `voltha-protos-5.4.4/python/voltha_protos/omci_test_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/onu_inter_adapter_service_pb2.py` & `voltha-protos-5.4.4/python/voltha_protos/onu_inter_adapter_service_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/openflow_13_pb2.py` & `voltha-protos-5.4.4/python/voltha_protos/openflow_13_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/device_pb2.py` & `voltha-protos-5.4.4/python/voltha_protos/device_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/core_adapter_pb2.py` & `voltha-protos-5.4.4/python/voltha_protos/core_adapter_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/core_services_pb2_grpc.py` & `voltha-protos-5.4.4/python/voltha_protos/core_services_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/health_pb2.py` & `voltha-protos-5.4.4/python/voltha_protos/health_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/tech_profile_pb2.py` & `voltha-protos-5.4.4/python/voltha_protos/tech_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/olt_inter_adapter_service_pb2.py` & `voltha-protos-5.4.4/python/voltha_protos/olt_inter_adapter_service_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/common_pb2.py` & `voltha-protos-5.4.4/python/voltha_protos/common_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/adapter_service_pb2.py` & `voltha-protos-5.4.4/python/voltha_protos/adapter_service_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/core_services_pb2.py` & `voltha-protos-5.4.4/python/voltha_protos/core_services_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/olt_inter_adapter_service_pb2_grpc.py` & `voltha-protos-5.4.4/python/voltha_protos/olt_inter_adapter_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/adapter_pb2.py` & `voltha-protos-5.4.4/python/voltha_protos/adapter_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/extensions_pb2.py` & `voltha-protos-5.4.4/python/voltha_protos/extensions_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/openolt_pb2_grpc.py` & `voltha-protos-5.4.4/python/voltha_protos/openolt_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/health_pb2_grpc.py` & `voltha-protos-5.4.4/python/voltha_protos/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/omci_mib_db_pb2.py` & `voltha-protos-5.4.4/python/voltha_protos/omci_mib_db_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/onu_inter_adapter_service_pb2_grpc.py` & `voltha-protos-5.4.4/python/voltha_protos/onu_inter_adapter_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos/openolt_pb2.py` & `voltha-protos-5.4.4/python/voltha_protos/openolt_pb2.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/test/__init__.py` & `voltha-protos-5.4.4/python/test/__init__.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/test/test_protos.py` & `voltha-protos-5.4.4/python/test/test_protos.py`

 * *Files identical despite different names*

### Comparing `voltha-protos-5.4.3/python/voltha_protos.egg-info/PKG-INFO` & `voltha-protos-5.4.4/python/voltha_protos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: voltha-protos
-Version: 5.4.3
+Version: 5.4.4
 Summary: Protobuf interface definitions
 Home-page: https://gerrit.opencord.org/gitweb?p=voltha-protos.git
 Author: VOLTHA project
 Author-email: voltha-dev@opencord.org
 License: Apache Software License
 Description: UNKNOWN
 Keywords: protobuf voltha
```

### Comparing `voltha-protos-5.4.3/python/voltha_protos.egg-info/SOURCES.txt` & `voltha-protos-5.4.4/python/voltha_protos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

