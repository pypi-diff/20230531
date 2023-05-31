# Comparing `tmp/pyechorobotics-0.0.1.tar.gz` & `tmp/pyechorobotics-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyechorobotics-0.0.1.tar", last modified: Wed May 31 16:35:39 2023, max compression
+gzip compressed data, was "pyechorobotics-0.0.2.tar", last modified: Wed May 31 16:41:05 2023, max compression
```

## Comparing `pyechorobotics-0.0.1.tar` & `pyechorobotics-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 16:35:39.044872 pyechorobotics-0.0.1/
--rw-rw-rw-   0        0        0    35149 2023-05-31 13:54:07.000000 pyechorobotics-0.0.1/LICENSE.md
--rw-rw-rw-   0        0        0     1376 2023-05-31 16:35:39.044872 pyechorobotics-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      802 2023-05-31 16:24:57.000000 pyechorobotics-0.0.1/README.md
--rw-rw-rw-   0        0        0      684 2023-05-31 13:55:20.000000 pyechorobotics-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      173 2023-05-31 16:35:39.045872 pyechorobotics-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       94 2023-05-31 13:54:07.000000 pyechorobotics-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-31 16:35:39.019873 pyechorobotics-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-31 16:35:39.033372 pyechorobotics-0.0.1/src/echoroboticsapi/
--rw-rw-rw-   0        0        0       74 2023-05-31 14:46:45.000000 pyechorobotics-0.0.1/src/echoroboticsapi/__init__.py
--rw-rw-rw-   0        0        0     2262 2023-05-31 16:17:13.000000 pyechorobotics-0.0.1/src/echoroboticsapi/api.py
--rw-rw-rw-   0        0        0     1289 2023-05-31 16:03:00.000000 pyechorobotics-0.0.1/src/echoroboticsapi/models.py
-drwxrwxrwx   0        0        0        0 2023-05-31 16:35:39.044372 pyechorobotics-0.0.1/src/pyechorobotics.egg-info/
--rw-rw-rw-   0        0        0     1376 2023-05-31 16:35:39.000000 pyechorobotics-0.0.1/src/pyechorobotics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-05-31 16:35:39.000000 pyechorobotics-0.0.1/src/pyechorobotics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 16:35:39.000000 pyechorobotics-0.0.1/src/pyechorobotics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-31 16:35:39.000000 pyechorobotics-0.0.1/src/pyechorobotics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-31 16:35:39.000000 pyechorobotics-0.0.1/src/pyechorobotics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:41:05.207104 pyechorobotics-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-31 16:40:54.000000 pyechorobotics-0.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-31 16:41:05.207104 pyechorobotics-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-31 16:40:54.000000 pyechorobotics-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-31 16:40:54.000000 pyechorobotics-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-31 16:41:05.207104 pyechorobotics-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-31 16:40:54.000000 pyechorobotics-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:41:05.207104 pyechorobotics-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:41:05.207104 pyechorobotics-0.0.2/src/echoroboticsapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 16:40:54.000000 pyechorobotics-0.0.2/src/echoroboticsapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-05-31 16:40:54.000000 pyechorobotics-0.0.2/src/echoroboticsapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-31 16:40:54.000000 pyechorobotics-0.0.2/src/echoroboticsapi/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:41:05.207104 pyechorobotics-0.0.2/src/pyechorobotics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-31 16:41:05.000000 pyechorobotics-0.0.2/src/pyechorobotics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-31 16:41:05.000000 pyechorobotics-0.0.2/src/pyechorobotics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 16:41:05.000000 pyechorobotics-0.0.2/src/pyechorobotics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 16:41:05.000000 pyechorobotics-0.0.2/src/pyechorobotics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 16:41:05.000000 pyechorobotics-0.0.2/src/pyechorobotics.egg-info/top_level.txt
```

### Comparing `pyechorobotics-0.0.1/LICENSE.md` & `pyechorobotics-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyechorobotics-0.0.1/PKG-INFO` & `pyechorobotics-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-Metadata-Version: 2.1
-Name: pyechorobotics
-Version: 0.0.1
-Summary: Access API for echorobotics robot lawn mowers
-Author-email: functionpointer <suspendfunction@gmail.com>
-License: GNU General Public License v3 or later (GPLv3+)
-Project-URL: homepage, https://github.com/functionpointer/pyechorobotics
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-pyechorobotics
-=============
-
-![echorobotics_logo](https://brands.home-assistant.io/_/echorobotics/logo@2x.png)
-
-Allows control and reads status of robot lawn mowers by echorobotics.
-
-Example:
-```python
-import sys
-
-import echoroboticsapi
-import aiohttp
-import asyncio
-import logging
-
-
-async def main():
-    async with aiohttp.ClientSession(cookies=echoroboticsapi.create_cookies(user_id="your-user-id", user_token="user-user-token")) as session:
-        api = echoroboticsapi.Api(session, robot_ids=["your-robot-id"])
-        print(await api.last_statuses())
-        print(await api.set_mode("chargeAndWork"))
-
-
-if __name__ == "__main__":
-    logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
-    loop = asyncio.new_event_loop()
-    loop.run_until_complete(main())
-
-```
-
-See also src/main.py
+Metadata-Version: 2.1
+Name: pyechorobotics
+Version: 0.0.2
+Summary: Access API for echorobotics robot lawn mowers
+Author-email: functionpointer <suspendfunction@gmail.com>
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: homepage, https://github.com/functionpointer/pyechorobotics
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+pyechorobotics
+=============
+
+![echorobotics_logo](https://brands.home-assistant.io/_/echorobotics/logo@2x.png)
+
+Allows control and reads status of robot lawn mowers by echorobotics.
+
+Example:
+```python
+import sys
+
+import echoroboticsapi
+import aiohttp
+import asyncio
+import logging
+
+
+async def main():
+    async with aiohttp.ClientSession(cookies=echoroboticsapi.create_cookies(user_id="your-user-id", user_token="user-user-token")) as session:
+        api = echoroboticsapi.Api(session, robot_ids=["your-robot-id"])
+        print(await api.last_statuses())
+        print(await api.set_mode("chargeAndWork"))
+
+
+if __name__ == "__main__":
+    logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
+    loop = asyncio.new_event_loop()
+    loop.run_until_complete(main())
+
+```
+
+See also src/main.py
```

### Comparing `pyechorobotics-0.0.1/README.md` & `pyechorobotics-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pyechorobotics-0.0.1/pyproject.toml` & `pyechorobotics-0.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyechorobotics"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
     "aiohttp",
     "yarl",
     "pydantic",
 ]
 readme = "README.md"
 license = {text = "GNU General Public License v3 or later (GPLv3+)"}
```

### Comparing `pyechorobotics-0.0.1/src/echoroboticsapi/api.py` & `pyechorobotics-0.0.2/src/echoroboticsapi/api.py`

 * *Files identical despite different names*

### Comparing `pyechorobotics-0.0.1/src/echoroboticsapi/models.py` & `pyechorobotics-0.0.2/src/echoroboticsapi/models.py`

 * *Files identical despite different names*

### Comparing `pyechorobotics-0.0.1/src/pyechorobotics.egg-info/PKG-INFO` & `pyechorobotics-0.0.2/src/pyechorobotics.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-Metadata-Version: 2.1
-Name: pyechorobotics
-Version: 0.0.1
-Summary: Access API for echorobotics robot lawn mowers
-Author-email: functionpointer <suspendfunction@gmail.com>
-License: GNU General Public License v3 or later (GPLv3+)
-Project-URL: homepage, https://github.com/functionpointer/pyechorobotics
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-pyechorobotics
-=============
-
-![echorobotics_logo](https://brands.home-assistant.io/_/echorobotics/logo@2x.png)
-
-Allows control and reads status of robot lawn mowers by echorobotics.
-
-Example:
-```python
-import sys
-
-import echoroboticsapi
-import aiohttp
-import asyncio
-import logging
-
-
-async def main():
-    async with aiohttp.ClientSession(cookies=echoroboticsapi.create_cookies(user_id="your-user-id", user_token="user-user-token")) as session:
-        api = echoroboticsapi.Api(session, robot_ids=["your-robot-id"])
-        print(await api.last_statuses())
-        print(await api.set_mode("chargeAndWork"))
-
-
-if __name__ == "__main__":
-    logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
-    loop = asyncio.new_event_loop()
-    loop.run_until_complete(main())
-
-```
-
-See also src/main.py
+Metadata-Version: 2.1
+Name: pyechorobotics
+Version: 0.0.2
+Summary: Access API for echorobotics robot lawn mowers
+Author-email: functionpointer <suspendfunction@gmail.com>
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: homepage, https://github.com/functionpointer/pyechorobotics
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+pyechorobotics
+=============
+
+![echorobotics_logo](https://brands.home-assistant.io/_/echorobotics/logo@2x.png)
+
+Allows control and reads status of robot lawn mowers by echorobotics.
+
+Example:
+```python
+import sys
+
+import echoroboticsapi
+import aiohttp
+import asyncio
+import logging
+
+
+async def main():
+    async with aiohttp.ClientSession(cookies=echoroboticsapi.create_cookies(user_id="your-user-id", user_token="user-user-token")) as session:
+        api = echoroboticsapi.Api(session, robot_ids=["your-robot-id"])
+        print(await api.last_statuses())
+        print(await api.set_mode("chargeAndWork"))
+
+
+if __name__ == "__main__":
+    logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
+    loop = asyncio.new_event_loop()
+    loop.run_until_complete(main())
+
+```
+
+See also src/main.py
```

