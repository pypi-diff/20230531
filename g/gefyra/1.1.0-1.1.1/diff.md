# Comparing `tmp/gefyra-1.1.0.tar.gz` & `tmp/gefyra-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gefyra-1.1.0.tar", max compression
+gzip compressed data, was "gefyra-1.1.1.tar", max compression
```

## Comparing `gefyra-1.1.0.tar` & `gefyra-1.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2151 2023-05-25 13:38:51.145910 gefyra-1.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/__init__.py
--rw-r--r--   0        0        0    15368 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/__main__.py
--rw-r--r--   0        0        0      200 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/api/__init__.py
--rw-r--r--   0        0        0     9037 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/api/bridge.py
--rw-r--r--   0        0        0     1306 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/api/down.py
--rw-r--r--   0        0        0     1605 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/api/list.py
--rw-r--r--   0        0        0     2523 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/api/reflect.py
--rw-r--r--   0        0        0     6142 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/api/run.py
--rw-r--r--   0        0        0     6277 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/api/status.py
--rw-r--r--   0        0        0     2917 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/api/up.py
--rw-r--r--   0        0        0     1562 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/api/utils.py
--rw-r--r--   0        0        0        0 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/cluster/__init__.py
--rw-r--r--   0        0        0     7090 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/cluster/manager.py
--rw-r--r--   0        0        0     8850 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/cluster/resources.py
--rw-r--r--   0        0        0     3016 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/cluster/utils.py
--rw-r--r--   0        0        0     8959 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/configuration.py
--rw-r--r--   0        0        0      260 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/local/__init__.py
--rw-r--r--   0        0        0     6677 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/local/bridge.py
--rw-r--r--   0        0        0     4609 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/local/cargo.py
--rw-r--r--   0        0        0        0 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/local/cargoimage/__init__.py
--rw-r--r--   0        0        0     1037 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/local/cargoimage/cargo_dockerfile.py
--rw-r--r--   0        0        0     1121 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/local/check.py
--rw-r--r--   0        0        0     2150 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/local/minikube.py
--rw-r--r--   0        0        0     4300 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/local/networking.py
--rw-r--r--   0        0        0     3948 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/local/telemetry.py
--rw-r--r--   0        0        0     8109 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/local/utils.py
--rw-r--r--   0        0        0     1326 2023-05-25 13:38:51.145910 gefyra-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 gefyra-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2151 2023-05-31 07:45:19.989690 gefyra-1.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/__init__.py
+-rw-r--r--   0        0        0    15368 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/__main__.py
+-rw-r--r--   0        0        0      200 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/api/__init__.py
+-rw-r--r--   0        0        0     9037 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/api/bridge.py
+-rw-r--r--   0        0        0     1306 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/api/down.py
+-rw-r--r--   0        0        0     1605 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/api/list.py
+-rw-r--r--   0        0        0     2523 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/api/reflect.py
+-rw-r--r--   0        0        0     6142 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/api/run.py
+-rw-r--r--   0        0        0     6277 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/api/status.py
+-rw-r--r--   0        0        0     2917 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/api/up.py
+-rw-r--r--   0        0        0     1562 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/api/utils.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/cluster/__init__.py
+-rw-r--r--   0        0        0     7090 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/cluster/manager.py
+-rw-r--r--   0        0        0     8850 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/cluster/resources.py
+-rw-r--r--   0        0        0     3016 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/cluster/utils.py
+-rw-r--r--   0        0        0     8650 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/configuration.py
+-rw-r--r--   0        0        0      260 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/local/__init__.py
+-rw-r--r--   0        0        0     6677 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/local/bridge.py
+-rw-r--r--   0        0        0     4609 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/local/cargo.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/local/cargoimage/__init__.py
+-rw-r--r--   0        0        0     1098 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/local/cargoimage/cargo_dockerfile.py
+-rw-r--r--   0        0        0     1121 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/local/check.py
+-rw-r--r--   0        0        0     2150 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/local/minikube.py
+-rw-r--r--   0        0        0     4300 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/local/networking.py
+-rw-r--r--   0        0        0     3948 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/local/telemetry.py
+-rw-r--r--   0        0        0     8109 2023-05-31 07:45:19.989690 gefyra-1.1.1/gefyra/local/utils.py
+-rw-r--r--   0        0        0     1326 2023-05-31 07:45:19.989690 gefyra-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 gefyra-1.1.1/PKG-INFO
```

### Comparing `gefyra-1.1.0/README.md` & `gefyra-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.0/gefyra/__main__.py` & `gefyra-1.1.1/gefyra/__main__.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.0/gefyra/api/bridge.py` & `gefyra-1.1.1/gefyra/api/bridge.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.0/gefyra/api/down.py` & `gefyra-1.1.1/gefyra/api/down.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.0/gefyra/api/list.py` & `gefyra-1.1.1/gefyra/api/list.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.0/gefyra/api/reflect.py` & `gefyra-1.1.1/gefyra/api/reflect.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.0/gefyra/api/run.py` & `gefyra-1.1.1/gefyra/api/run.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.0/gefyra/api/status.py` & `gefyra-1.1.1/gefyra/api/status.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.0/gefyra/api/up.py` & `gefyra-1.1.1/gefyra/api/up.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.0/gefyra/api/utils.py` & `gefyra-1.1.1/gefyra/api/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.0/gefyra/cluster/manager.py` & `gefyra-1.1.1/gefyra/cluster/manager.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.0/gefyra/cluster/resources.py` & `gefyra-1.1.1/gefyra/cluster/resources.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.0/gefyra/cluster/utils.py` & `gefyra-1.1.1/gefyra/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.0/gefyra/configuration.py` & `gefyra-1.1.1/gefyra/configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from os import path
+import platform
 import struct
 import socket
 import sys
 import logging
 
 console = logging.StreamHandler(sys.stdout)
 formatter = logging.Formatter("[%(levelname)s] %(message)s")
 console.setFormatter(formatter)
 
 logger = logging.getLogger("gefyra")
 logger.addHandler(console)
 
-__VERSION__ = "1.1.0"
+__VERSION__ = "1.1.1"
 
 
 def fix_pywin32_in_frozen_build() -> None:  # pragma: no cover
     import os
     import site
 
     if sys.platform != "win32" or not getattr(sys, "frozen", False):
@@ -96,45 +97,41 @@
         if cargo_image_url:
             logger.debug(f"Using Cargo image (other than default): {cargo_image_url}")
         if docker_client:
             self.DOCKER = docker_client
         if cargo_endpoint_host:
             self.CARGO_ENDPOINT = f"{cargo_endpoint_host}:{cargo_endpoint_port}"
         else:
-            docker_os = self._get_docker_info_by_name("OperatingSystem")
-            docker_server_name = self._get_docker_info_by_name("Name")
-            logger.debug(f"Docker OS: {docker_os}")
-            logger.debug(f"Docker Server Name: {docker_server_name}")
-            # virtualized envs don't expose network interface to host
+            self.DOCKER.info
             if (
-                "docker desktop" in docker_os
-                or "windows" in docker_os
-                or "colima" in docker_server_name
+                platform.system().lower() == "linux"
+                and "microsoft" not in platform.release().lower()
             ):
-                try:
-                    _ip_output = self.DOCKER.containers.run(
-                        "alpine", "getent hosts host.docker.internal", remove=True
-                    )
-                    _ip = _ip_output.decode("utf-8").split(" ")[0]
-                    self.CARGO_ENDPOINT = f"{_ip}:{cargo_endpoint_port}"
-                except Exception as e:
-                    logger.error("Could not create a valid configuration: " + str(e))
-            else:
                 # get linux docker0 network address
                 import fcntl
 
                 _soc = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
                 _ip = socket.inet_ntoa(
                     fcntl.ioctl(
                         _soc.fileno(),
                         0x8915,
                         struct.pack("256s", "docker0".encode("utf-8")[:15]),
                     )[20:24]
                 )
                 self.CARGO_ENDPOINT = f"{_ip}:{cargo_endpoint_port}"
+            else:
+                try:
+                    _ip_output = self.DOCKER.containers.run(
+                        "alpine", "getent hosts host.docker.internal", remove=True
+                    )
+                    _ip = _ip_output.decode("utf-8").split(" ")[0]
+                    self.CARGO_ENDPOINT = f"{_ip}:{cargo_endpoint_port}"
+                except Exception as e:
+                    logger.error("Could not create a valid configuration: " + str(e))
+
         self.CARGO_CONTAINER_NAME = cargo_container_name or "gefyra-cargo"
         self.STOWAWAY_IP = "192.168.99.1"
         self.NETWORK_NAME = network_name or "gefyra"
         self.BRIDGE_TIMEOUT = 60  # in seconds
         self.CARGO_PROBE_TIMEOUT = 10  # in seconds
         self.CONTAINER_RUN_TIMEOUT = 10  # in seconds
         if kube_config_file:
```

### Comparing `gefyra-1.1.0/gefyra/local/bridge.py` & `gefyra-1.1.1/gefyra/local/bridge.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.0/gefyra/local/cargo.py` & `gefyra-1.1.1/gefyra/local/cargo.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.0/gefyra/local/cargoimage/cargo_dockerfile.py` & `gefyra-1.1.1/gefyra/local/cargoimage/cargo_dockerfile.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # flake8: noqa
 import io
+import platform
 import sys
 
 
 def get_dockerfile(cargo_image):
     run_patch = ""
-    if sys.platform == "win32":
+    if sys.platform == "win32" or "microsoft" in platform.release().lower():
         run_patch = "RUN patch /usr/bin/wg-quick /wgquick.patch"
     return io.BytesIO(
         f""" 
 FROM {cargo_image}
 {run_patch}
 
 ARG ADDRESS
```

### Comparing `gefyra-1.1.0/gefyra/local/check.py` & `gefyra-1.1.1/gefyra/local/check.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.0/gefyra/local/minikube.py` & `gefyra-1.1.1/gefyra/local/minikube.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.0/gefyra/local/networking.py` & `gefyra-1.1.1/gefyra/local/networking.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.0/gefyra/local/telemetry.py` & `gefyra-1.1.1/gefyra/local/telemetry.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.0/gefyra/local/utils.py` & `gefyra-1.1.1/gefyra/local/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.1.0/pyproject.toml` & `gefyra-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Gefyra"
-version = "1.1.0"
+version = "1.1.1"
 description = "Gefyra runs all developer machine side components of Gefyra's Kubernetes-based development infrastructure"
 authors = ["Michael Schilonka <michael@unikube.io>"]
 readme = "README.md"
 homepage = "https://gefyra.dev"
 repository = "https://github.com/gefyrahq/gefyra"
 documentation = "https://gefyra.dev"
 keywords = [
```

### Comparing `gefyra-1.1.0/PKG-INFO` & `gefyra-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gefyra
-Version: 1.1.0
+Version: 1.1.1
 Summary: Gefyra runs all developer machine side components of Gefyra's Kubernetes-based development infrastructure
 Home-page: https://gefyra.dev
 Keywords: Kubernetes,Development,Cloud-native
 Author: Michael Schilonka
 Author-email: michael@unikube.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

