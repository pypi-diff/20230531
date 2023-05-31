# Comparing `tmp/python-matter-server-3.4.1.tar.gz` & `tmp/python-matter-server-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-matter-server-3.4.1.tar", last modified: Tue May 23 13:16:02 2023, max compression
+gzip compressed data, was "python-matter-server-3.4.2.tar", last modified: Wed May 31 18:23:39 2023, max compression
```

## Comparing `python-matter-server-3.4.1.tar` & `python-matter-server-3.4.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:16:02.787005 python-matter-server-3.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-05-23 13:16:02.787005 python-matter-server-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:16:02.783004 python-matter-server-3.4.1/matter_server/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:16:02.783004 python-matter-server-3.4.1/matter_server/client/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:16:02.783004 python-matter-server-3.4.1/matter_server/client/models/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14068 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/client/models/device_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13630 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/client/models/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:16:02.783004 python-matter-server-3.4.1/matter_server/common/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/common/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/common/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:16:02.783004 python-matter-server-3.4.1/matter_server/common/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/common/helpers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/common/helpers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/common/helpers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/common/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:16:02.783004 python-matter-server-3.4.1/matter_server/server/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/server/client_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/server/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/server/device_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:16:02.783004 python-matter-server-3.4.1/matter_server/server/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/server/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/server/helpers/paa_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/server/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/server/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/matter_server/server/vendor_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-23 13:15:44.000000 python-matter-server-3.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:16:02.787005 python-matter-server-3.4.1/python_matter_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-05-23 13:16:02.000000 python-matter-server-3.4.1/python_matter_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-23 13:16:02.000000 python-matter-server-3.4.1/python_matter_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:16:02.000000 python-matter-server-3.4.1/python_matter_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 13:16:02.000000 python-matter-server-3.4.1/python_matter_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:16:00.000000 python-matter-server-3.4.1/python_matter_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-23 13:16:02.000000 python-matter-server-3.4.1/python_matter_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 13:16:02.000000 python-matter-server-3.4.1/python_matter_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 13:16:02.787005 python-matter-server-3.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:23:39.704531 python-matter-server-3.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9391 2023-05-31 18:23:39.704531 python-matter-server-3.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8793 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:23:39.700531 python-matter-server-3.4.2/matter_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:23:39.700531 python-matter-server-3.4.2/matter_server/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:23:39.704531 python-matter-server-3.4.2/matter_server/client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14068 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/client/models/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13630 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/client/models/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:23:39.704531 python-matter-server-3.4.2/matter_server/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/common/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:23:39.704531 python-matter-server-3.4.2/matter_server/common/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/common/helpers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/common/helpers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/common/helpers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:23:39.704531 python-matter-server-3.4.2/matter_server/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/server/client_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/server/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/server/device_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:23:39.704531 python-matter-server-3.4.2/matter_server/server/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/server/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/server/helpers/paa_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/server/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/server/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/matter_server/server/vendor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-31 18:23:27.000000 python-matter-server-3.4.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:23:39.704531 python-matter-server-3.4.2/python_matter_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9391 2023-05-31 18:23:39.000000 python-matter-server-3.4.2/python_matter_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-31 18:23:39.000000 python-matter-server-3.4.2/python_matter_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 18:23:39.000000 python-matter-server-3.4.2/python_matter_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-31 18:23:39.000000 python-matter-server-3.4.2/python_matter_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 18:23:37.000000 python-matter-server-3.4.2/python_matter_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-31 18:23:39.000000 python-matter-server-3.4.2/python_matter_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 18:23:39.000000 python-matter-server-3.4.2/python_matter_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-31 18:23:39.704531 python-matter-server-3.4.2/setup.cfg
```

### Comparing `python-matter-server-3.4.1/LICENSE` & `python-matter-server-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.1/PKG-INFO` & `python-matter-server-3.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 3.4.1
+Version: 3.4.2
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
@@ -222,7 +222,20 @@
 
 ### Run
 
 ```sh
 docker compose up -d
 docker compose logs -f
 ```
+
+### Note when using Thread based Matter devices
+
+When communicating with Thread devices through a non-local Thread border router,
+your host must process ICMPv6 Router Advertisements. See the [openthread.io
+Bidirectional IPv6 Connectivity code labs](https://openthread.io/codelabs/openthread-border-router#6)
+on how-to setup your host correctly. Note that NetworkManager has its own ICMPv6
+Router Advertisement processing. A recent version of NetworkManager is
+necessary, and there are still known issues (see NetworkManager issue
+[#1232](https://gitlab.freedesktop.org/NetworkManager/NetworkManager/-/issues/1232)).
+
+The Home Assistant Operating System 10 and newer correctly processes ICMPv6
+Router Advertisements.
```

### Comparing `python-matter-server-3.4.1/README.md` & `python-matter-server-3.4.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -203,7 +203,20 @@
 
 ### Run
 
 ```sh
 docker compose up -d
 docker compose logs -f
 ```
+
+### Note when using Thread based Matter devices
+
+When communicating with Thread devices through a non-local Thread border router,
+your host must process ICMPv6 Router Advertisements. See the [openthread.io
+Bidirectional IPv6 Connectivity code labs](https://openthread.io/codelabs/openthread-border-router#6)
+on how-to setup your host correctly. Note that NetworkManager has its own ICMPv6
+Router Advertisement processing. A recent version of NetworkManager is
+necessary, and there are still known issues (see NetworkManager issue
+[#1232](https://gitlab.freedesktop.org/NetworkManager/NetworkManager/-/issues/1232)).
+
+The Home Assistant Operating System 10 and newer correctly processes ICMPv6
+Router Advertisements.
```

### Comparing `python-matter-server-3.4.1/matter_server/client/client.py` & `python-matter-server-3.4.2/matter_server/client/client.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.1/matter_server/client/connection.py` & `python-matter-server-3.4.2/matter_server/client/connection.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.1/matter_server/client/exceptions.py` & `python-matter-server-3.4.2/matter_server/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.1/matter_server/client/models/device_types.py` & `python-matter-server-3.4.2/matter_server/client/models/device_types.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.1/matter_server/client/models/node.py` & `python-matter-server-3.4.2/matter_server/client/models/node.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.1/matter_server/common/errors.py` & `python-matter-server-3.4.2/matter_server/common/errors.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.1/matter_server/common/helpers/api.py` & `python-matter-server-3.4.2/matter_server/common/helpers/api.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.1/matter_server/common/helpers/json.py` & `python-matter-server-3.4.2/matter_server/common/helpers/json.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.1/matter_server/common/helpers/util.py` & `python-matter-server-3.4.2/matter_server/common/helpers/util.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.1/matter_server/common/models.py` & `python-matter-server-3.4.2/matter_server/common/models.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.1/matter_server/server/__main__.py` & `python-matter-server-3.4.2/matter_server/server/__main__.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.1/matter_server/server/client_handler.py` & `python-matter-server-3.4.2/matter_server/server/client_handler.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.1/matter_server/server/const.py` & `python-matter-server-3.4.2/matter_server/server/const.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.1/matter_server/server/device_controller.py` & `python-matter-server-3.4.2/matter_server/server/device_controller.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.1/matter_server/server/helpers/paa_certificates.py` & `python-matter-server-3.4.2/matter_server/server/helpers/paa_certificates.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.1/matter_server/server/server.py` & `python-matter-server-3.4.2/matter_server/server/server.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.1/matter_server/server/stack.py` & `python-matter-server-3.4.2/matter_server/server/stack.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.1/matter_server/server/storage.py` & `python-matter-server-3.4.2/matter_server/server/storage.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.1/matter_server/server/vendor_info.py` & `python-matter-server-3.4.2/matter_server/server/vendor_info.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.4.1/pyproject.toml` & `python-matter-server-3.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-matter-server"
-version = "3.4.1"
+version = "3.4.2"
 license     = {text = "Apache-2.0"}
 description = "Python Matter WebSocket Server"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
@@ -22,32 +22,32 @@
 ]
 dependencies = [
   "aiohttp",
   "aiorun",
   "coloredlogs",
   "dacite",
   "orjson",
-  "home-assistant-chip-clusters==2023.5.2"
+  "home-assistant-chip-clusters==2023.5.3"
 ]
 
 [project.optional-dependencies]
 server = [
-  "home-assistant-chip-core==2023.5.2",
+  "home-assistant-chip-core==2023.5.3",
   "cryptography==40.0.2"
 ]
 test = [
   "black==23.3.0",
   "flake8==6.0.0",
   "flake8-docstrings==1.7.0",
   "isort==5.12.0",
   "mypy==1.3.0",
   "pylint==2.17.4",
   "pytest==7.3.1",
   "pytest-aiohttp==1.0.4",
-  "pytest-cov==4.0.0",
+  "pytest-cov==4.1.0",
 ]
 
 [project.scripts]
 matter-server = "matter_server.server.__main__:main"
 
 [tool.mypy]
 python_version = "3.10"
```

### Comparing `python-matter-server-3.4.1/python_matter_server.egg-info/PKG-INFO` & `python-matter-server-3.4.2/python_matter_server.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 3.4.1
+Version: 3.4.2
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
@@ -222,7 +222,20 @@
 
 ### Run
 
 ```sh
 docker compose up -d
 docker compose logs -f
 ```
+
+### Note when using Thread based Matter devices
+
+When communicating with Thread devices through a non-local Thread border router,
+your host must process ICMPv6 Router Advertisements. See the [openthread.io
+Bidirectional IPv6 Connectivity code labs](https://openthread.io/codelabs/openthread-border-router#6)
+on how-to setup your host correctly. Note that NetworkManager has its own ICMPv6
+Router Advertisement processing. A recent version of NetworkManager is
+necessary, and there are still known issues (see NetworkManager issue
+[#1232](https://gitlab.freedesktop.org/NetworkManager/NetworkManager/-/issues/1232)).
+
+The Home Assistant Operating System 10 and newer correctly processes ICMPv6
+Router Advertisements.
```

### Comparing `python-matter-server-3.4.1/python_matter_server.egg-info/SOURCES.txt` & `python-matter-server-3.4.2/python_matter_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

