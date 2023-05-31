# Comparing `tmp/jupyterhub-backendspawner-0.3.1.tar.gz` & `tmp/jupyterhub-backendspawner-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-backendspawner-0.3.1.tar", last modified: Mon May 22 14:43:38 2023, max compression
+gzip compressed data, was "jupyterhub-backendspawner-0.3.2.tar", last modified: Wed May 31 10:15:58 2023, max compression
```

## Comparing `jupyterhub-backendspawner-0.3.1.tar` & `jupyterhub-backendspawner-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 14:43:38.757544 jupyterhub-backendspawner-0.3.1/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.3.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-22 14:43:38.757544 jupyterhub-backendspawner-0.3.1/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.3.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 14:43:38.757544 jupyterhub-backendspawner-0.3.1/backendspawner/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.3.1/backendspawner/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5150 2023-05-04 13:52:18.000000 jupyterhub-backendspawner-0.3.1/backendspawner/api_events.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17351 2023-05-15 14:54:00.000000 jupyterhub-backendspawner-0.3.1/backendspawner/backendspawner.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10209 2023-05-22 14:42:59.000000 jupyterhub-backendspawner-0.3.1/backendspawner/eventspawner.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-22 14:43:38.757544 jupyterhub-backendspawner-0.3.1/jupyterhub_backendspawner.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-22 14:43:38.000000 jupyterhub-backendspawner-0.3.1/jupyterhub_backendspawner.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-05-22 14:43:38.000000 jupyterhub-backendspawner-0.3.1/jupyterhub_backendspawner.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-22 14:43:38.000000 jupyterhub-backendspawner-0.3.1/jupyterhub_backendspawner.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-22 14:43:38.000000 jupyterhub-backendspawner-0.3.1/jupyterhub_backendspawner.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-05-22 14:43:38.000000 jupyterhub-backendspawner-0.3.1/jupyterhub_backendspawner.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-22 14:43:38.757544 jupyterhub-backendspawner-0.3.1/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-05-22 14:43:05.000000 jupyterhub-backendspawner-0.3.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 10:15:58.062293 jupyterhub-backendspawner-0.3.2/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.3.2/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-31 10:15:58.062293 jupyterhub-backendspawner-0.3.2/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.3.2/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 10:15:58.052293 jupyterhub-backendspawner-0.3.2/backendspawner/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.3.2/backendspawner/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5150 2023-05-04 13:52:18.000000 jupyterhub-backendspawner-0.3.2/backendspawner/api_events.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17765 2023-05-31 10:15:11.000000 jupyterhub-backendspawner-0.3.2/backendspawner/backendspawner.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10280 2023-05-31 10:13:29.000000 jupyterhub-backendspawner-0.3.2/backendspawner/eventspawner.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 10:15:58.052293 jupyterhub-backendspawner-0.3.2/jupyterhub_backendspawner.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-31 10:15:58.000000 jupyterhub-backendspawner-0.3.2/jupyterhub_backendspawner.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-05-31 10:15:58.000000 jupyterhub-backendspawner-0.3.2/jupyterhub_backendspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-31 10:15:58.000000 jupyterhub-backendspawner-0.3.2/jupyterhub_backendspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-31 10:15:58.000000 jupyterhub-backendspawner-0.3.2/jupyterhub_backendspawner.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-05-31 10:15:58.000000 jupyterhub-backendspawner-0.3.2/jupyterhub_backendspawner.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-31 10:15:58.062293 jupyterhub-backendspawner-0.3.2/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-05-31 10:15:44.000000 jupyterhub-backendspawner-0.3.2/setup.py
```

### Comparing `jupyterhub-backendspawner-0.3.1/LICENSE` & `jupyterhub-backendspawner-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.3.1/backendspawner/api_events.py` & `jupyterhub-backendspawner-0.3.2/backendspawner/api_events.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.3.1/backendspawner/backendspawner.py` & `jupyterhub-backendspawner-0.3.2/backendspawner/backendspawner.py`

 * *Files 3% similar despite different names*

```diff
@@ -384,15 +384,21 @@
                     "log_name": self._log_name,
                     "user": self.user.name,
                     "duration": toc,
                 },
             )
 
     async def start(self):
-        self.log.info(f"Start single-user server {self.name}-{self.start_id}")
+        self.log.info(f"Start single-user server {self.name}-{self.start_id}",
+            extra={
+                "uuidcode": self.name,
+                "log_name": self._log_name,
+                "user": self.user.name,
+            },
+        )
         request_body = await self.get_request_body_start()
         request_header = await self.get_request_headers_start()
         url = await self.get_request_url_start()
 
         req = HTTPRequest(
             url=url,
             method="POST",
@@ -402,14 +408,21 @@
         )
 
         try:
             resp_json = await self.send_request(req, action="start")
         except Exception as e:
             # If JupyterHub could not start the service, additional
             # actions may be required.
+            self.log.exception("Send Request failed",
+                extra={
+                    "uuidcode": self.name,
+                    "log_name": self._log_name,
+                    "user": self.user.name,
+                },
+            )
             await maybe_future(self.run_failed_spawn_request_hook(e))
 
             try:
                 await self.stop()
             except:
                 self.log.exception(
                     "Could not stop service which failed to start.",
```

### Comparing `jupyterhub-backendspawner-0.3.1/backendspawner/eventspawner.py` & `jupyterhub-backendspawner-0.3.2/backendspawner/eventspawner.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,14 +185,15 @@
                     summary = error.get("error")
                     details = error.get("detailed_error")
                 else:
                     summary = f"{exception.args[0]} - {exception.args[1]}"
                     details = str(error)
             except:
                 self.log.exception("Could not load detailed error message")
+                summary = f"{exception.args[0]} - {exception.args[1]}"
         elif hasattr(exception, "args") and len(exception.args) > 1:
             summary = f"{exception.args[0]} - {exception.args[1]}"
 
         async def _get_stop_event(spawner):
             now = datetime.now().strftime("%Y_%m_%d %H:%M:%S.%f")[:-3]
             event = {
                 "progress": 100,
```

### Comparing `jupyterhub-backendspawner-0.3.1/setup.py` & `jupyterhub-backendspawner-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="jupyterhub-backendspawner",
-    version="0.3.1",
+    version="0.3.2",
     description="JupyterHub Spawner to spawn on different systems.",
     url="https://github.com/kreuzert/jupyterhub-backendspawner",
     author="Tim Kreuzer",
     author_email="t.kreuzer@fz-juelich.de",
     license="3-BSD",
     packages=find_packages(),
     install_requires=["jupyterhub","traitlets"],
```

