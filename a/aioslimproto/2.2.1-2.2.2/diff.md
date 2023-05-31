# Comparing `tmp/aioslimproto-2.2.1.tar.gz` & `tmp/aioslimproto-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioslimproto-2.2.1.tar", last modified: Mon May 29 21:37:27 2023, max compression
+gzip compressed data, was "aioslimproto-2.2.2.tar", last modified: Wed May 31 11:54:06 2023, max compression
```

## Comparing `aioslimproto-2.2.1.tar` & `aioslimproto-2.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:37:27.813711 aioslimproto-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-29 21:37:27.813711 aioslimproto-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:37:27.813711 aioslimproto-2.2.1/aioslimproto/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/aioslimproto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22638 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/aioslimproto/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    30608 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/aioslimproto/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/aioslimproto/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/aioslimproto/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/aioslimproto/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/aioslimproto/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/aioslimproto/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:37:27.813711 aioslimproto-2.2.1/aioslimproto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-29 21:37:27.000000 aioslimproto-2.2.1/aioslimproto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-29 21:37:27.000000 aioslimproto-2.2.1/aioslimproto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 21:37:27.000000 aioslimproto-2.2.1/aioslimproto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-29 21:37:27.000000 aioslimproto-2.2.1/aioslimproto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 21:37:27.000000 aioslimproto-2.2.1/aioslimproto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 21:37:27.000000 aioslimproto-2.2.1/aioslimproto.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-29 21:37:27.813711 aioslimproto-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:54:06.440146 aioslimproto-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-31 11:54:06.440146 aioslimproto-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:54:06.436145 aioslimproto-2.2.2/aioslimproto/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/aioslimproto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22638 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/aioslimproto/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30608 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/aioslimproto/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/aioslimproto/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/aioslimproto/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/aioslimproto/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/aioslimproto/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/aioslimproto/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:54:06.440146 aioslimproto-2.2.2/aioslimproto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-31 11:54:06.000000 aioslimproto-2.2.2/aioslimproto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-31 11:54:06.000000 aioslimproto-2.2.2/aioslimproto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 11:54:06.000000 aioslimproto-2.2.2/aioslimproto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 11:54:06.000000 aioslimproto-2.2.2/aioslimproto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 11:54:06.000000 aioslimproto-2.2.2/aioslimproto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 11:54:06.000000 aioslimproto-2.2.2/aioslimproto.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-31 11:54:06.440146 aioslimproto-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/setup.py
```

### Comparing `aioslimproto-2.2.1/LICENSE` & `aioslimproto-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.2.1/PKG-INFO` & `aioslimproto-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioslimproto
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python module to talk to Logitech Squeezebox players directly (without Logitech server).
 Home-page: https://github.com/music-assistant/aioslimproto
 Author: Marcel van der Veldt
 Author-email: marcelveldt@users.noreply.github.com
 License: Apache License 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `aioslimproto-2.2.1/aioslimproto/cli.py` & `aioslimproto-2.2.2/aioslimproto/cli.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.2.1/aioslimproto/client.py` & `aioslimproto-2.2.2/aioslimproto/client.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.2.1/aioslimproto/const.py` & `aioslimproto-2.2.2/aioslimproto/const.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.2.1/aioslimproto/discovery.py` & `aioslimproto-2.2.2/aioslimproto/discovery.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     device = None
     firmware = None
     client = None
 
     def __init__(self, data):
         """Initialize class."""
         msg = struct.unpack("!cxBB8x6B", data.encode())
-        assert msg[0] == "d"
         self.device = msg[1]
         self.firmware = hex(msg[2])
         self.client = ":".join(["%02x" % (x,) for x in msg[3:]])
 
     def __repr__(self):
         """Print the class contents."""
         return "<%s device=%r firmware=%r client=%r>" % (
@@ -88,15 +87,14 @@
 
 class TLVDiscoveryRequestDatagram(Datagram):
     """Description of a discovery request datagram."""
 
     def __init__(self, data):
         """Initialize class."""
         requestdata = OrderedDict()
-        assert data[0] == "e"
         idx = 1
         length = len(data) - 5
         while idx <= length:
             typ, _len = struct.unpack_from("4sB", data.encode(), idx)
             if _len:
                 val = data[idx + 5 : idx + 5 + _len]
                 idx += 5 + _len
```

### Comparing `aioslimproto-2.2.1/aioslimproto/server.py` & `aioslimproto-2.2.2/aioslimproto/server.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.2.1/aioslimproto/util.py` & `aioslimproto-2.2.2/aioslimproto/util.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.2.1/aioslimproto.egg-info/PKG-INFO` & `aioslimproto-2.2.2/aioslimproto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioslimproto
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python module to talk to Logitech Squeezebox players directly (without Logitech server).
 Home-page: https://github.com/music-assistant/aioslimproto
 Author: Marcel van der Veldt
 Author-email: marcelveldt@users.noreply.github.com
 License: Apache License 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `aioslimproto-2.2.1/setup.cfg` & `aioslimproto-2.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.2.1/setup.py` & `aioslimproto-2.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 README_FILE = PROJECT_DIR / "README.md"
 REQUIREMENTS_FILE = PROJECT_DIR / "requirements.txt"
 PACKAGES = find_packages(exclude=["tests", "tests.*"])
 PROJECT_REQ_PYTHON_VERSION = "3.9"
 
 setup(
     name="aioslimproto",
-    version="2.2.1",
+    version="2.2.2",
     license="Apache License 2.0",
     url="https://github.com/music-assistant/aioslimproto",
     author="Marcel van der Veldt",
     author_email="marcelveldt@users.noreply.github.com",
     description="Python module to talk to Logitech Squeezebox players directly (without Logitech server).",
     long_description=README_FILE.read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
```

