# Comparing `tmp/integra-0.0.3.tar.gz` & `tmp/integra-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integra-0.0.3.tar", last modified: Tue May  9 17:36:39 2023, max compression
+gzip compressed data, was "integra-0.0.5.tar", last modified: Wed May 31 15:57:12 2023, max compression
```

## Comparing `integra-0.0.3.tar` & `integra-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,14 @@
-drwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-09 17:36:39.480740 integra-0.0.3/
--rw-rw-r--   0 pmus      (1000) pmus      (1000)     1089 2023-05-08 23:32:21.000000 integra-0.0.3/LICENSE
--rw-rw-r--   0 pmus      (1000) pmus      (1000)      405 2023-05-09 17:36:39.480740 integra-0.0.3/PKG-INFO
--rwxrwxr-x   0 pmus      (1000) pmus      (1000)      541 2023-05-09 17:36:22.000000 integra-0.0.3/pyproject.toml
--rw-rw-r--   0 pmus      (1000) pmus      (1000)       38 2023-05-09 17:36:39.480740 integra-0.0.3/setup.cfg
-drwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-09 17:36:39.480740 integra-0.0.3/src/
--rwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-09 14:54:31.000000 integra-0.0.3/src/__init__.py
-drwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-09 17:36:39.480740 integra-0.0.3/src/integra.egg-info/
--rw-rw-r--   0 pmus      (1000) pmus      (1000)      405 2023-05-09 17:36:39.000000 integra-0.0.3/src/integra.egg-info/PKG-INFO
--rw-rw-r--   0 pmus      (1000) pmus      (1000)      313 2023-05-09 17:36:39.000000 integra-0.0.3/src/integra.egg-info/SOURCES.txt
--rw-rw-r--   0 pmus      (1000) pmus      (1000)        1 2023-05-09 17:36:39.000000 integra-0.0.3/src/integra.egg-info/dependency_links.txt
--rw-rw-r--   0 pmus      (1000) pmus      (1000)       23 2023-05-09 17:36:39.000000 integra-0.0.3/src/integra.egg-info/top_level.txt
--rwxrwxr-x   0 pmus      (1000) pmus      (1000)     8617 2023-05-09 17:33:34.000000 integra-0.0.3/src/integra.py
-drwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-09 17:36:39.480740 integra-0.0.3/src/tests/
--rw-rw-r--   0 pmus      (1000) pmus      (1000)      823 2023-05-09 14:54:31.000000 integra-0.0.3/src/tests/bench-recv.py
--rw-rw-r--   0 pmus      (1000) pmus      (1000)      845 2023-05-09 14:54:31.000000 integra-0.0.3/src/tests/infinite-recv.py
--rwxrwxr-x   0 pmus      (1000) pmus      (1000)      485 2023-05-09 14:54:31.000000 integra-0.0.3/src/tests/receive.py
--rw-rw-r--   0 pmus      (1000) pmus      (1000)      886 2023-05-09 14:54:31.000000 integra-0.0.3/src/tests/serve-localhost.py
--rwxrwxr-x   0 pmus      (1000) pmus      (1000)      857 2023-05-09 17:33:30.000000 integra-0.0.3/src/tests/serve.py
+drwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-31 15:57:12.601405 integra-0.0.5/
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)     1089 2023-05-31 15:53:06.000000 integra-0.0.5/LICENSE
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)     1278 2023-05-31 15:57:12.601405 integra-0.0.5/PKG-INFO
+-rwxrwxr-x   0 pmus      (1000) pmus      (1000)      541 2023-05-31 15:54:06.000000 integra-0.0.5/pyproject.toml
+-rwxrwxr-x   0 pmus      (1000) pmus      (1000)      872 2023-05-31 15:53:06.000000 integra-0.0.5/readme.md
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)       38 2023-05-31 15:57:12.601405 integra-0.0.5/setup.cfg
+drwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-31 15:57:12.601405 integra-0.0.5/src/
+-rwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-31 15:53:06.000000 integra-0.0.5/src/__init__.py
+drwxrwxr-x   0 pmus      (1000) pmus      (1000)        0 2023-05-31 15:57:12.601405 integra-0.0.5/src/integra.egg-info/
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)     1278 2023-05-31 15:57:12.000000 integra-0.0.5/src/integra.egg-info/PKG-INFO
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)      203 2023-05-31 15:57:12.000000 integra-0.0.5/src/integra.egg-info/SOURCES.txt
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)        1 2023-05-31 15:57:12.000000 integra-0.0.5/src/integra.egg-info/dependency_links.txt
+-rw-rw-r--   0 pmus      (1000) pmus      (1000)       17 2023-05-31 15:57:12.000000 integra-0.0.5/src/integra.egg-info/top_level.txt
+-rwxrwxr-x   0 pmus      (1000) pmus      (1000)     8510 2023-05-31 15:53:06.000000 integra-0.0.5/src/integra.py
```

### Comparing `integra-0.0.3/LICENSE` & `integra-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `integra-0.0.3/pyproject.toml` & `integra-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=61.0", "loguru==0.7.0", "pyzmq==25.0.2", "zeroconf==0.62.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "integra"
-version = "0.0.3"
+version = "0.0.5"
 authors = [
   { name="pmus", email="pmus.me@yandex.ru" },
 ]
 description = "ZeroMQ Zeroconf RPC"
-readme = "README.md"
+readme = "readme.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `integra-0.0.3/src/integra.py` & `integra-0.0.5/src/integra.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,25 @@
 system_hostname: str = socket.gethostname()
 default_short_sleep_sec: float = 0.1
 default_poll_timeout_sec: int = 3
 default_wait_timeout_sec: int = 10
 
 
 def myasync(func) -> None:
-
     @wraps(func)
     def async_func(*args, **kwargs):
         func_hl = Thread(target=func, args=args, kwargs=kwargs)
         func_hl.daemon = False
         func_hl.start()
         return func_hl
 
     return async_func
 
 
 class ServiceProxy(object):
-
     def __init__(self, integra_instance: object, service_name: str) -> None:
         self.integra_instance: Integra = integra_instance
         self.service_name: str = service_name
         self.client_update_service_data()
 
     def client_update_service_data(self):
         self.service_data: dict = self.integra_instance.dict_services[self.service_name]
@@ -44,15 +42,14 @@
                           if self.service_data["ip"] != self.integra_instance.ip else "127.0.0.1")
         self.remote_port = self.service_data["port"]
         logger.info(f"Creating ZMQ proxy at: {self.remote_ip}:{self.remote_port}")
         self.socket.setsockopt(zmq.LINGER, 0)  # Add timeout feature
         self.socket.connect(f"tcp://{self.remote_ip}:{self.remote_port}")
 
     def __getattr__(self, attr) -> object:
-
         def callable(*args, **kwargs):
             res: object = self.method_missing(attr, *args, **kwargs)
             return res
 
         return callable
 
     def method_missing(self, attr, *args, **kwargs) -> object:
@@ -78,18 +75,17 @@
             while not self.service_name in self.integra_instance.dict_services:
                 time.sleep(default_poll_timeout_sec)
             self.client_update_service_data()  # This is service recovery
         return recv["result"] if recv else None
 
 
 class Integra(object):
-
     def __init__(self, zmq_port: int = 0, local_only=False) -> None:
         with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as s:
-            s.connect(("10.254.254.254", 1))  #s.settimeout(0)
+            s.connect(("10.254.254.254", 1))  # s.settimeout(0)
             self.ip: str = s.getsockname()[0]  # on error, we don't mute it.
         self.run: bool = True
         self.zeroconf: Zeroconf = Zeroconf()
         self.dict_objects: dict = dict()  # What I offer
         self.dict_services: dict = dict()  # What do neighbours offer
         self.zmq_addr: str = "127.0.0.1" if local_only else "*"
         self.zmq_port = zmq_port
@@ -113,17 +109,17 @@
         self.zmq_port = int(real_endpoint.split(":")[2])
         reply: dict = dict()
         while self.run:
             request: object = self.socket.recv_pyobj()
             service, attr, args, kwargs = (request[key] for key in ["service", "attr", "args", "kwargs"])
             service_obj: object = self.dict_objects.get(service, None)
             service_attr: object = getattr(service_obj, attr, None)
-            reply["error"] = RuntimeError(f"Error: Service object {service} missing.") if not service_obj else None
-            reply["error"] = AttributeError(f"No attribute {attr} in {service}.") if not service_attr else None
-            reply["result"] = service_attr(*args, **kwargs) if callable(service_attr) else service_attr
+            reply["error"] = (RuntimeError(f"Error: Service object {service} missing.") if not service_obj else None)
+            reply["error"] = (AttributeError(f"No attribute {attr} in {service}.") if not service_attr else None)
+            reply["result"] = (service_attr(*args, **kwargs) if callable(service_attr) else service_attr)
             self.socket.send_pyobj(reply)
 
     def on_service_state_change(
         self,
         zeroconf: Zeroconf,
         service_type: str,
         name: str,
@@ -140,25 +136,22 @@
             self.forget_service(name)
         elif state_change is ServiceStateChange.Added:
             for service_name in info["services"]:
                 self.dict_services[service_name] = info
 
     def forget_service(self, name) -> None:
         logger.info(f"Deleting {name} from {self.dict_services}")
-        del self.dict_services[name]
+        self.dict_services.pop(name, None) # Instead of 'del''
 
+    @logger.catch
     def service_info_to_dict(self, service_info: ServiceInfo) -> dict:
         res: dict = {key: getattr(service_info, key, None) for key in ["name", "port", "server"]}
         properties: dict = service_info.properties
-        properties = dict({
-            key.decode("utf-8"): value.decode("utf-8")
-            for key, value in properties.items()
-        })  # Properties transmitted in binary, we decode...
-        properties["services"] = json.loads(properties["services"].replace(
-            "'", '"'))  # Not my fault, but zeroconf passes them this way
+        properties = {key.decode("utf-8"): value.decode("utf-8") for key, value in properties.items()}
+        properties["services"] = json.loads(properties["services"].replace("'", '"'))
         res.update(properties)
         return res
 
     def add_service(self, service_name: str, some_object: object) -> None:
         self.dict_objects[service_name] = some_object
         self.desc["services"].append(service_name)
         logger.info(f"Registering service '{service_name}'...")
```

