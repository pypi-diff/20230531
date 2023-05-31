# Comparing `tmp/csle_cluster-0.2.1.tar.gz` & `tmp/csle_cluster-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_cluster-0.2.1.tar", last modified: Wed May 31 11:27:26 2023, max compression
+gzip compressed data, was "csle_cluster-0.2.2.tar", last modified: Wed May 31 11:50:49 2023, max compression
```

## Comparing `csle_cluster-0.2.1.tar` & `csle_cluster-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:27:26.713790 csle_cluster-0.2.1/
--rw-r--r--   0 kimham     (501) staff       (20)      804 2023-05-31 11:27:26.713926 csle_cluster-0.2.1/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     4256 2023-03-05 07:26:30.000000 csle_cluster-0.2.1/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      672 2023-02-12 09:12:26.000000 csle_cluster-0.2.1/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1406 2023-05-31 11:27:26.714680 csle_cluster-0.2.1/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_cluster-0.2.1/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:27:26.691685 csle_cluster-0.2.1/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:27:26.696179 csle_cluster-0.2.1/src/csle_cluster/
--rw-r--r--   0 kimham     (501) staff       (20)       37 2023-02-12 09:44:18.000000 csle_cluster-0.2.1/src/csle_cluster/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 11:22:38.000000 csle_cluster-0.2.1/src/csle_cluster/__version__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:27:26.711528 csle_cluster-0.2.1/src/csle_cluster/cluster_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_cluster-0.2.1/src/csle_cluster/cluster_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)   229247 2023-04-19 06:25:48.000000 csle_cluster-0.2.1/src/csle_cluster/cluster_manager/cluster_controller.py
--rw-r--r--   0 kimham     (501) staff       (20)   269186 2023-05-01 07:57:15.000000 csle_cluster-0.2.1/src/csle_cluster/cluster_manager/cluster_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)   197343 2023-03-31 11:14:06.000000 csle_cluster-0.2.1/src/csle_cluster/cluster_manager/cluster_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)   349502 2023-03-31 11:14:06.000000 csle_cluster-0.2.1/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)   202990 2023-03-31 11:14:06.000000 csle_cluster-0.2.1/src/csle_cluster/cluster_manager/cluster_manager_util.py
--rw-r--r--   0 kimham     (501) staff       (20)   188175 2023-04-19 06:25:48.000000 csle_cluster-0.2.1/src/csle_cluster/cluster_manager/query_cluster_manager.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:27:26.713343 csle_cluster-0.2.1/src/csle_cluster/constants/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2023-03-05 07:26:30.000000 csle_cluster-0.2.1/src/csle_cluster/constants/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)      375 2023-03-16 16:24:28.000000 csle_cluster-0.2.1/src/csle_cluster/constants/constants.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:27:26.698873 csle_cluster-0.2.1/src/csle_cluster.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      804 2023-05-31 11:27:26.000000 csle_cluster-0.2.1/src/csle_cluster.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)      805 2023-05-31 11:27:26.000000 csle_cluster-0.2.1/src/csle_cluster.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 11:27:26.000000 csle_cluster-0.2.1/src/csle_cluster.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-02-12 09:44:23.000000 csle_cluster-0.2.1/src/csle_cluster.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      251 2023-05-31 11:27:26.000000 csle_cluster-0.2.1/src/csle_cluster.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)       13 2023-05-31 11:27:26.000000 csle_cluster-0.2.1/src/csle_cluster.egg-info/top_level.txt
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:50:49.871445 csle_cluster-0.2.2/
+-rw-r--r--   0 kimham     (501) staff       (20)      804 2023-05-31 11:50:49.871576 csle_cluster-0.2.2/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)     4256 2023-03-05 07:26:30.000000 csle_cluster-0.2.2/README.md
+-rw-r--r--   0 kimham     (501) staff       (20)      672 2023-02-12 09:12:26.000000 csle_cluster-0.2.2/pyproject.toml
+-rw-r--r--   0 kimham     (501) staff       (20)     1406 2023-05-31 11:50:49.872172 csle_cluster-0.2.2/setup.cfg
+-rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_cluster-0.2.2/setup.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:50:49.851875 csle_cluster-0.2.2/src/
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:50:49.854869 csle_cluster-0.2.2/src/csle_cluster/
+-rw-r--r--   0 kimham     (501) staff       (20)       37 2023-02-12 09:44:18.000000 csle_cluster-0.2.2/src/csle_cluster/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)       22 2023-05-31 11:45:39.000000 csle_cluster-0.2.2/src/csle_cluster/__version__.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:50:49.868822 csle_cluster-0.2.2/src/csle_cluster/cluster_manager/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_cluster-0.2.2/src/csle_cluster/cluster_manager/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)   229454 2023-05-31 11:33:47.000000 csle_cluster-0.2.2/src/csle_cluster/cluster_manager/cluster_controller.py
+-rw-r--r--   0 kimham     (501) staff       (20)   269186 2023-05-01 07:57:15.000000 csle_cluster-0.2.2/src/csle_cluster/cluster_manager/cluster_manager.py
+-rw-r--r--   0 kimham     (501) staff       (20)   197343 2023-03-31 11:14:06.000000 csle_cluster-0.2.2/src/csle_cluster/cluster_manager/cluster_manager_pb2.py
+-rw-r--r--   0 kimham     (501) staff       (20)   349502 2023-03-31 11:14:06.000000 csle_cluster-0.2.2/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py
+-rw-r--r--   0 kimham     (501) staff       (20)   202990 2023-03-31 11:14:06.000000 csle_cluster-0.2.2/src/csle_cluster/cluster_manager/cluster_manager_util.py
+-rw-r--r--   0 kimham     (501) staff       (20)   188175 2023-04-19 06:25:48.000000 csle_cluster-0.2.2/src/csle_cluster/cluster_manager/query_cluster_manager.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:50:49.870888 csle_cluster-0.2.2/src/csle_cluster/constants/
+-rw-r--r--   0 kimham     (501) staff       (20)        0 2023-03-05 07:26:30.000000 csle_cluster-0.2.2/src/csle_cluster/constants/__init__.py
+-rw-r--r--   0 kimham     (501) staff       (20)      375 2023-03-16 16:24:28.000000 csle_cluster-0.2.2/src/csle_cluster/constants/constants.py
+drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-05-31 11:50:49.856976 csle_cluster-0.2.2/src/csle_cluster.egg-info/
+-rw-r--r--   0 kimham     (501) staff       (20)      804 2023-05-31 11:50:49.000000 csle_cluster-0.2.2/src/csle_cluster.egg-info/PKG-INFO
+-rw-r--r--   0 kimham     (501) staff       (20)      805 2023-05-31 11:50:49.000000 csle_cluster-0.2.2/src/csle_cluster.egg-info/SOURCES.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2023-05-31 11:50:49.000000 csle_cluster-0.2.2/src/csle_cluster.egg-info/dependency_links.txt
+-rw-r--r--   0 kimham     (501) staff       (20)        1 2023-02-12 09:44:23.000000 csle_cluster-0.2.2/src/csle_cluster.egg-info/not-zip-safe
+-rw-r--r--   0 kimham     (501) staff       (20)      251 2023-05-31 11:50:49.000000 csle_cluster-0.2.2/src/csle_cluster.egg-info/requires.txt
+-rw-r--r--   0 kimham     (501) staff       (20)       13 2023-05-31 11:50:49.000000 csle_cluster-0.2.2/src/csle_cluster.egg-info/top_level.txt
```

### Comparing `csle_cluster-0.2.1/PKG-INFO` & `csle_cluster-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_cluster
-Version: 0.2.1
+Version: 0.2.2
 Summary: Scripts for cluster management in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cluster-0.2.1/README.md` & `csle_cluster-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.1/pyproject.toml` & `csle_cluster-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.1/setup.cfg` & `csle_cluster-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	grpcio>=1.27.2
 	grpcio-tools>=1.27.2
-	csle-collector>=0.2.1
-	csle-common>=0.2.1
-	csle-ryu>=0.2.1
+	csle-collector>=0.2.2
+	csle-common>=0.2.2
+	csle-ryu>=0.2.2
 python_requires = >=3.5
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_cluster-0.2.1/src/csle_cluster/cluster_manager/cluster_controller.py` & `csle_cluster-0.2.2/src/csle_cluster/cluster_manager/cluster_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -3894,93 +3894,93 @@
             Logger.__call__().get_logger().info(f"Starting the host managers on containers "
                                                 f"in emulation: {execution.emulation_env_config.name} on server: {ip}")
             ClusterController.start_host_managers(
                 ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
                 emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet)
         time.sleep(10)
 
-        current_step += 1
-        Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Applying filebeats configurations --")
-        for ip in physical_servers:
-            Logger.__call__().get_logger().info(f"Applying filebeat configurations on containers "
-                                                f"in emulation: {execution.emulation_env_config.name} on server: {ip}")
-            ClusterController.apply_filebeats_config(
-                ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
-                emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet)
-        time.sleep(10)
-
-        current_step += 1
-        Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Applying packetbeats configurations --")
-        for ip in physical_servers:
-            Logger.__call__().get_logger().info(f"Applying packetbeat configurations on containers "
-                                                f"in emulation: {execution.emulation_env_config.name} on server: {ip}")
-            ClusterController.apply_packetbeats_config(
-                ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
-                emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet)
-        time.sleep(10)
-
-        current_step += 1
-        Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Applying metricbeats configurations --")
-        for ip in physical_servers:
-            Logger.__call__().get_logger().info(f"Applying metricbeat configurations on containers "
-                                                f"in emulation: {execution.emulation_env_config.name} on server: {ip}")
-            ClusterController.apply_metricbeats_config(
-                ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
-                emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet)
-        time.sleep(10)
-
-        current_step += 1
-        Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Applying heartbeats configurations --")
-        for ip in physical_servers:
-            Logger.__call__().get_logger().info(f"Applying heartbeat configurations on containers"
-                                                f" in emulation: {execution.emulation_env_config.name} on server: {ip}")
-            ClusterController.apply_heartbeats_config(
-                ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
-                emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet)
-        time.sleep(10)
-
-        current_step += 1
-        Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Starting filebeats --")
-        for ip in physical_servers:
-            Logger.__call__().get_logger().info(f"Starting filebeats on containers "
-                                                f"in emulation: {execution.emulation_env_config.name} on server: {ip}")
-            ClusterController.start_filebeats(
-                ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
-                emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet, initial_start=True)
-        time.sleep(10)
-
-        current_step += 1
-        Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Starting packetbeats --")
-        for ip in physical_servers:
-            Logger.__call__().get_logger().info(f"Starting packetbeats on containers "
-                                                f"in emulation: {execution.emulation_env_config.name} on server: {ip}")
-            ClusterController.start_packetbeats(
-                ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
-                emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet, initial_start=True)
-        time.sleep(10)
-
-        current_step += 1
-        Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Starting metricbeats --")
-        for ip in physical_servers:
-            Logger.__call__().get_logger().info(f"Starting metricbeats on containers "
-                                                f"in emulation: {execution.emulation_env_config.name} on server: {ip}")
-            ClusterController.start_metricbeats(
-                ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
-                emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet, initial_start=True)
-        time.sleep(10)
-
-        current_step += 1
-        Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Starting heartbeats --")
-        for ip in physical_servers:
-            Logger.__call__().get_logger().info(f"Starting heartbeats on containers "
-                                                f"in emulation: {execution.emulation_env_config.name} on server: {ip}")
-            ClusterController.start_heartbeats(
-                ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
-                emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet, initial_start=True)
-        time.sleep(10)
+        # current_step += 1
+        # Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Applying filebeats configurations --")
+        # for ip in physical_servers:
+        #     Logger.__call__().get_logger().info(f"Applying filebeat configurations on containers "
+        #                                         f"in emulation: {execution.emulation_env_config.name} on server: {ip}")
+        #     ClusterController.apply_filebeats_config(
+        #         ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
+        #         emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet)
+        # time.sleep(10)
+        #
+        # current_step += 1
+        # Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Applying packetbeats configurations --")
+        # for ip in physical_servers:
+        #     Logger.__call__().get_logger().info(f"Applying packetbeat configurations on containers "
+        #                                         f"in emulation: {execution.emulation_env_config.name} on server: {ip}")
+        #     ClusterController.apply_packetbeats_config(
+        #         ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
+        #         emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet)
+        # time.sleep(10)
+        #
+        # current_step += 1
+        # Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Applying metricbeats configurations --")
+        # for ip in physical_servers:
+        #     Logger.__call__().get_logger().info(f"Applying metricbeat configurations on containers "
+        #                                         f"in emulation: {execution.emulation_env_config.name} on server: {ip}")
+        #     ClusterController.apply_metricbeats_config(
+        #         ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
+        #         emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet)
+        # time.sleep(10)
+        #
+        # current_step += 1
+        # Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Applying heartbeats configurations --")
+        # for ip in physical_servers:
+        #     Logger.__call__().get_logger().info(f"Applying heartbeat configurations on containers"
+        #                                         f" in emulation: {execution.emulation_env_config.name} on server: {ip}")
+        #     ClusterController.apply_heartbeats_config(
+        #         ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
+        #         emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet)
+        # time.sleep(10)
+        #
+        # current_step += 1
+        # Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Starting filebeats --")
+        # for ip in physical_servers:
+        #     Logger.__call__().get_logger().info(f"Starting filebeats on containers "
+        #                                         f"in emulation: {execution.emulation_env_config.name} on server: {ip}")
+        #     ClusterController.start_filebeats(
+        #         ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
+        #         emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet, initial_start=True)
+        # time.sleep(10)
+        #
+        # current_step += 1
+        # Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Starting packetbeats --")
+        # for ip in physical_servers:
+        #     Logger.__call__().get_logger().info(f"Starting packetbeats on containers "
+        #                                         f"in emulation: {execution.emulation_env_config.name} on server: {ip}")
+        #     ClusterController.start_packetbeats(
+        #         ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
+        #         emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet, initial_start=True)
+        # time.sleep(10)
+        #
+        # current_step += 1
+        # Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Starting metricbeats --")
+        # for ip in physical_servers:
+        #     Logger.__call__().get_logger().info(f"Starting metricbeats on containers "
+        #                                         f"in emulation: {execution.emulation_env_config.name} on server: {ip}")
+        #     ClusterController.start_metricbeats(
+        #         ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
+        #         emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet, initial_start=True)
+        # time.sleep(10)
+        #
+        # current_step += 1
+        # Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Starting heartbeats --")
+        # for ip in physical_servers:
+        #     Logger.__call__().get_logger().info(f"Starting heartbeats on containers "
+        #                                         f"in emulation: {execution.emulation_env_config.name} on server: {ip}")
+        #     ClusterController.start_heartbeats(
+        #         ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT,
+        #         emulation=execution.emulation_name, ip_first_octet=execution.ip_first_octet, initial_start=True)
+        # time.sleep(10)
 
         current_step += 1
         Logger.__call__().get_logger().info(f"-- Step {current_step}/{steps}: Starting the Docker stats monitor --")
         for ip in physical_servers:
             Logger.__call__().get_logger().info(f"Starting the Docker statsmanager on server: {ip}")
             ClusterController.start_docker_statsmanager(
                 ip=ip, port=constants.GRPC_SERVERS.CLUSTER_MANAGER_PORT)
```

### Comparing `csle_cluster-0.2.1/src/csle_cluster/cluster_manager/cluster_manager.py` & `csle_cluster-0.2.2/src/csle_cluster/cluster_manager/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.1/src/csle_cluster/cluster_manager/cluster_manager_pb2.py` & `csle_cluster-0.2.2/src/csle_cluster/cluster_manager/cluster_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.1/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py` & `csle_cluster-0.2.2/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.1/src/csle_cluster/cluster_manager/cluster_manager_util.py` & `csle_cluster-0.2.2/src/csle_cluster/cluster_manager/cluster_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.1/src/csle_cluster/cluster_manager/query_cluster_manager.py` & `csle_cluster-0.2.2/src/csle_cluster/cluster_manager/query_cluster_manager.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.2.1/src/csle_cluster.egg-info/PKG-INFO` & `csle_cluster-0.2.2/src/csle_cluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-cluster
-Version: 0.2.1
+Version: 0.2.2
 Summary: Scripts for cluster management in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cluster-0.2.1/src/csle_cluster.egg-info/SOURCES.txt` & `csle_cluster-0.2.2/src/csle_cluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

