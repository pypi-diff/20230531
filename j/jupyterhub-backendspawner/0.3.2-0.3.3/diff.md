# Comparing `tmp/jupyterhub-backendspawner-0.3.2.tar.gz` & `tmp/jupyterhub-backendspawner-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterhub-backendspawner-0.3.2.tar", last modified: Wed May 31 10:15:58 2023, max compression
+gzip compressed data, was "jupyterhub-backendspawner-0.3.3.tar", last modified: Wed May 31 12:30:58 2023, max compression
```

## Comparing `jupyterhub-backendspawner-0.3.2.tar` & `jupyterhub-backendspawner-0.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 10:15:58.062293 jupyterhub-backendspawner-0.3.2/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.3.2/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-31 10:15:58.062293 jupyterhub-backendspawner-0.3.2/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.3.2/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 10:15:58.052293 jupyterhub-backendspawner-0.3.2/backendspawner/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.3.2/backendspawner/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5150 2023-05-04 13:52:18.000000 jupyterhub-backendspawner-0.3.2/backendspawner/api_events.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17765 2023-05-31 10:15:11.000000 jupyterhub-backendspawner-0.3.2/backendspawner/backendspawner.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10280 2023-05-31 10:13:29.000000 jupyterhub-backendspawner-0.3.2/backendspawner/eventspawner.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 10:15:58.052293 jupyterhub-backendspawner-0.3.2/jupyterhub_backendspawner.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-31 10:15:58.000000 jupyterhub-backendspawner-0.3.2/jupyterhub_backendspawner.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-05-31 10:15:58.000000 jupyterhub-backendspawner-0.3.2/jupyterhub_backendspawner.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-31 10:15:58.000000 jupyterhub-backendspawner-0.3.2/jupyterhub_backendspawner.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-31 10:15:58.000000 jupyterhub-backendspawner-0.3.2/jupyterhub_backendspawner.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-05-31 10:15:58.000000 jupyterhub-backendspawner-0.3.2/jupyterhub_backendspawner.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-31 10:15:58.062293 jupyterhub-backendspawner-0.3.2/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-05-31 10:15:44.000000 jupyterhub-backendspawner-0.3.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 12:30:58.691146 jupyterhub-backendspawner-0.3.3/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1498 2023-04-24 08:18:45.000000 jupyterhub-backendspawner-0.3.3/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-31 12:30:58.691146 jupyterhub-backendspawner-0.3.3/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      102 2023-04-24 08:20:17.000000 jupyterhub-backendspawner-0.3.3/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 12:30:58.691146 jupyterhub-backendspawner-0.3.3/backendspawner/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2023-04-24 08:20:47.000000 jupyterhub-backendspawner-0.3.3/backendspawner/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5197 2023-05-31 12:29:40.000000 jupyterhub-backendspawner-0.3.3/backendspawner/api_events.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    17765 2023-05-31 10:15:11.000000 jupyterhub-backendspawner-0.3.3/backendspawner/backendspawner.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10280 2023-05-31 10:13:29.000000 jupyterhub-backendspawner-0.3.3/backendspawner/eventspawner.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 12:30:58.691146 jupyterhub-backendspawner-0.3.3/jupyterhub_backendspawner.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2023-05-31 12:30:58.000000 jupyterhub-backendspawner-0.3.3/jupyterhub_backendspawner.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      390 2023-05-31 12:30:58.000000 jupyterhub-backendspawner-0.3.3/jupyterhub_backendspawner.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-31 12:30:58.000000 jupyterhub-backendspawner-0.3.3/jupyterhub_backendspawner.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-05-31 12:30:58.000000 jupyterhub-backendspawner-0.3.3/jupyterhub_backendspawner.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-05-31 12:30:58.000000 jupyterhub-backendspawner-0.3.3/jupyterhub_backendspawner.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-31 12:30:58.691146 jupyterhub-backendspawner-0.3.3/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      566 2023-05-31 12:30:14.000000 jupyterhub-backendspawner-0.3.3/setup.py
```

### Comparing `jupyterhub-backendspawner-0.3.2/LICENSE` & `jupyterhub-backendspawner-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.3.2/backendspawner/api_events.py` & `jupyterhub-backendspawner-0.3.3/backendspawner/api_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 
 user_cancel_message = (
     "Start cancelled by user.</summary>You clicked the cancel button.</details>"
 )
 
 
 class SpawnEventsAPIHandler(APIHandler):
+    def check_xsrf_cookie(self):
+        pass
+
     @needs_scope("read:servers")
     async def get(self, user_name, server_name=""):
         user = self.find_user(user_name)
         if user is None:
             # no such user
             raise web.HTTPError(404)
         if server_name not in user.spawners:
```

### Comparing `jupyterhub-backendspawner-0.3.2/backendspawner/backendspawner.py` & `jupyterhub-backendspawner-0.3.3/backendspawner/backendspawner.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.3.2/backendspawner/eventspawner.py` & `jupyterhub-backendspawner-0.3.3/backendspawner/eventspawner.py`

 * *Files identical despite different names*

### Comparing `jupyterhub-backendspawner-0.3.2/setup.py` & `jupyterhub-backendspawner-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="jupyterhub-backendspawner",
-    version="0.3.2",
+    version="0.3.3",
     description="JupyterHub Spawner to spawn on different systems.",
     url="https://github.com/kreuzert/jupyterhub-backendspawner",
     author="Tim Kreuzer",
     author_email="t.kreuzer@fz-juelich.de",
     license="3-BSD",
     packages=find_packages(),
     install_requires=["jupyterhub","traitlets"],
```

