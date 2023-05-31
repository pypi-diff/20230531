# Comparing `tmp/zwave-js-server-python-0.8.0.tar.gz` & `tmp/zwave-js-server-python-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zwave-js-server-python-0.8.0.tar", last modified: Thu Jan 14 21:51:12 2021, max compression
+gzip compressed data, was "zwave-js-server-python-0.9.0.tar", last modified: Fri Jan 15 09:35:40 2021, max compression
```

## Comparing `zwave-js-server-python-0.8.0.tar` & `zwave-js-server-python-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 21:51:12.342780 zwave-js-server-python-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (116)     1418 2021-01-14 21:51:12.342780 zwave-js-server-python-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      525 2021-01-14 21:51:10.000000 zwave-js-server-python-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      692 2021-01-14 21:51:12.342780 zwave-js-server-python-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1191 2021-01-14 21:51:10.000000 zwave-js-server-python-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 21:51:12.338780 zwave-js-server-python-0.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (116)      298 2021-01-14 21:51:10.000000 zwave-js-server-python-0.8.0/test/test_event.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 21:51:12.338780 zwave-js-server-python-0.8.0/zwave_js_server/
--rw-r--r--   0 runner    (1001) docker     (116)       45 2021-01-14 21:51:10.000000 zwave-js-server-python-0.8.0/zwave_js_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2935 2021-01-14 21:51:10.000000 zwave-js-server-python-0.8.0/zwave_js_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12005 2021-01-14 21:51:10.000000 zwave-js-server-python-0.8.0/zwave_js_server/client.py
--rw-r--r--   0 runner    (1001) docker     (116)     3299 2021-01-14 21:51:10.000000 zwave-js-server-python-0.8.0/zwave_js_server/const.py
--rw-r--r--   0 runner    (1001) docker     (116)     1772 2021-01-14 21:51:10.000000 zwave-js-server-python-0.8.0/zwave_js_server/event.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 21:51:12.338780 zwave-js-server-python-0.8.0/zwave_js_server/model/
--rw-r--r--   0 runner    (1001) docker     (116)      123 2021-01-14 21:51:10.000000 zwave-js-server-python-0.8.0/zwave_js_server/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5859 2021-01-14 21:51:10.000000 zwave-js-server-python-0.8.0/zwave_js_server/model/controller.py
--rw-r--r--   0 runner    (1001) docker     (116)     1417 2021-01-14 21:51:10.000000 zwave-js-server-python-0.8.0/zwave_js_server/model/device_class.py
--rw-r--r--   0 runner    (1001) docker     (116)     2745 2021-01-14 21:51:10.000000 zwave-js-server-python-0.8.0/zwave_js_server/model/device_config.py
--rw-r--r--   0 runner    (1001) docker     (116)      876 2021-01-14 21:51:10.000000 zwave-js-server-python-0.8.0/zwave_js_server/model/driver.py
--rw-r--r--   0 runner    (1001) docker     (116)     9688 2021-01-14 21:51:10.000000 zwave-js-server-python-0.8.0/zwave_js_server/model/node.py
--rw-r--r--   0 runner    (1001) docker     (116)     4604 2021-01-14 21:51:10.000000 zwave-js-server-python-0.8.0/zwave_js_server/model/value.py
--rw-r--r--   0 runner    (1001) docker     (116)      806 2021-01-14 21:51:10.000000 zwave-js-server-python-0.8.0/zwave_js_server/version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-14 21:51:12.342780 zwave-js-server-python-0.8.0/zwave_js_server_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1418 2021-01-14 21:51:12.000000 zwave-js-server-python-0.8.0/zwave_js_server_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      720 2021-01-14 21:51:12.000000 zwave-js-server-python-0.8.0/zwave_js_server_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-14 21:51:12.000000 zwave-js-server-python-0.8.0/zwave_js_server_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-14 21:51:12.000000 zwave-js-server-python-0.8.0/zwave_js_server_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       10 2021-01-14 21:51:12.000000 zwave-js-server-python-0.8.0/zwave_js_server_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2021-01-14 21:51:12.000000 zwave-js-server-python-0.8.0/zwave_js_server_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 09:35:40.663311 zwave-js-server-python-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (116)     1418 2021-01-15 09:35:40.663311 zwave-js-server-python-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      525 2021-01-15 09:35:36.000000 zwave-js-server-python-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)      692 2021-01-15 09:35:40.663311 zwave-js-server-python-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1191 2021-01-15 09:35:36.000000 zwave-js-server-python-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 09:35:40.663311 zwave-js-server-python-0.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (116)      298 2021-01-15 09:35:36.000000 zwave-js-server-python-0.9.0/test/test_event.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 09:35:40.663311 zwave-js-server-python-0.9.0/zwave_js_server/
+-rw-r--r--   0 runner    (1001) docker     (116)       45 2021-01-15 09:35:36.000000 zwave-js-server-python-0.9.0/zwave_js_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2935 2021-01-15 09:35:36.000000 zwave-js-server-python-0.9.0/zwave_js_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12005 2021-01-15 09:35:36.000000 zwave-js-server-python-0.9.0/zwave_js_server/client.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3299 2021-01-15 09:35:36.000000 zwave-js-server-python-0.9.0/zwave_js_server/const.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1772 2021-01-15 09:35:36.000000 zwave-js-server-python-0.9.0/zwave_js_server/event.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 09:35:40.663311 zwave-js-server-python-0.9.0/zwave_js_server/model/
+-rw-r--r--   0 runner    (1001) docker     (116)      123 2021-01-15 09:35:36.000000 zwave-js-server-python-0.9.0/zwave_js_server/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      509 2021-01-15 09:35:36.000000 zwave-js-server-python-0.9.0/zwave_js_server/model/association.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12717 2021-01-15 09:35:36.000000 zwave-js-server-python-0.9.0/zwave_js_server/model/controller.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1417 2021-01-15 09:35:36.000000 zwave-js-server-python-0.9.0/zwave_js_server/model/device_class.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2745 2021-01-15 09:35:36.000000 zwave-js-server-python-0.9.0/zwave_js_server/model/device_config.py
+-rw-r--r--   0 runner    (1001) docker     (116)      876 2021-01-15 09:35:36.000000 zwave-js-server-python-0.9.0/zwave_js_server/model/driver.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11329 2021-01-15 09:35:36.000000 zwave-js-server-python-0.9.0/zwave_js_server/model/node.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4607 2021-01-15 09:35:36.000000 zwave-js-server-python-0.9.0/zwave_js_server/model/value.py
+-rw-r--r--   0 runner    (1001) docker     (116)      806 2021-01-15 09:35:36.000000 zwave-js-server-python-0.9.0/zwave_js_server/version.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 09:35:40.663311 zwave-js-server-python-0.9.0/zwave_js_server_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     1418 2021-01-15 09:35:40.000000 zwave-js-server-python-0.9.0/zwave_js_server_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      757 2021-01-15 09:35:40.000000 zwave-js-server-python-0.9.0/zwave_js_server_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-15 09:35:40.000000 zwave-js-server-python-0.9.0/zwave_js_server_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-15 09:35:40.000000 zwave-js-server-python-0.9.0/zwave_js_server_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       10 2021-01-15 09:35:40.000000 zwave-js-server-python-0.9.0/zwave_js_server_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       16 2021-01-15 09:35:40.000000 zwave-js-server-python-0.9.0/zwave_js_server_python.egg-info/top_level.txt
```

### Comparing `zwave-js-server-python-0.8.0/PKG-INFO` & `zwave-js-server-python-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zwave-js-server-python
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python wrapper for zwave-js-server
 Home-page: https://github.com/home-assistant-libs/zwave-js-server-python
 Author: Home Assistant Team
 Author-email: hello@home-assistant.io
 License: UNKNOWN
 Download-URL: https://github.com/home-assistant-libs/zwave-js-server-python
 Description: # zwave-js-server-python
```

### Comparing `zwave-js-server-python-0.8.0/README.md` & `zwave-js-server-python-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `zwave-js-server-python-0.8.0/setup.cfg` & `zwave-js-server-python-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `zwave-js-server-python-0.8.0/setup.py` & `zwave-js-server-python-0.9.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Setup module for zwave-js-server-python."""
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "0.8.0"
+VERSION = "0.9.0"
 
 
 setup(
     name="zwave-js-server-python",
     version=VERSION,
     url="https://github.com/home-assistant-libs/zwave-js-server-python",
     download_url="https://github.com/home-assistant-libs/zwave-js-server-python",
```

### Comparing `zwave-js-server-python-0.8.0/zwave_js_server/__main__.py` & `zwave-js-server-python-0.9.0/zwave_js_server/__main__.py`

 * *Files identical despite different names*

### Comparing `zwave-js-server-python-0.8.0/zwave_js_server/client.py` & `zwave-js-server-python-0.9.0/zwave_js_server/client.py`

 * *Files identical despite different names*

### Comparing `zwave-js-server-python-0.8.0/zwave_js_server/const.py` & `zwave-js-server-python-0.9.0/zwave_js_server/const.py`

 * *Files identical despite different names*

### Comparing `zwave-js-server-python-0.8.0/zwave_js_server/event.py` & `zwave-js-server-python-0.9.0/zwave_js_server/event.py`

 * *Files identical despite different names*

### Comparing `zwave-js-server-python-0.8.0/zwave_js_server/model/device_class.py` & `zwave-js-server-python-0.9.0/zwave_js_server/model/device_class.py`

 * *Files identical despite different names*

### Comparing `zwave-js-server-python-0.8.0/zwave_js_server/model/device_config.py` & `zwave-js-server-python-0.9.0/zwave_js_server/model/device_config.py`

 * *Files identical despite different names*

### Comparing `zwave-js-server-python-0.8.0/zwave_js_server/model/driver.py` & `zwave-js-server-python-0.9.0/zwave_js_server/model/driver.py`

 * *Files identical despite different names*

### Comparing `zwave-js-server-python-0.8.0/zwave_js_server/model/node.py` & `zwave-js-server-python-0.9.0/zwave_js_server/model/node.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Provide a model for the Z-Wave JS node."""
 from typing import TYPE_CHECKING, Any, List, Optional, TypedDict, Union, cast
 
 from ..event import Event, EventBase
 from .device_class import DeviceClass, DeviceClassDataType
 from .device_config import DeviceConfig, DeviceConfigDataType
-from .value import Value, ValueDataType, get_value_id
+from .value import Value, ValueDataType, ValueMetadata, MetaDataType, get_value_id
 
 if TYPE_CHECKING:
     from ..client import Client
 
 
 class NodeDataType(TypedDict, total=False):
     """Represent a node data dict type."""
@@ -238,14 +238,59 @@
                 "nodeId": self.node_id,
                 "valueId": val.data,
                 "value": new_value,
             }
         )
         return cast(bool, result["success"])
 
+    async def async_refresh_info(self) -> None:
+        """Send refreshInfo command to Node."""
+        await self.client.async_send_json_message(
+            {
+                "command": "node.refresh_info",
+                "nodeId": self.node_id,
+            }
+        )
+
+    async def async_get_defined_value_ids(self) -> List[Value]:
+        """Send getDefinedValueIDs command to Node."""
+        data = await self.client.async_send_command(
+            {
+                "command": "node.get_defined_value_ids",
+                "nodeId": self.node_id,
+            }
+        )
+        return [
+            Value(self, cast(ValueDataType, valueId)) for valueId in data["valueIds"]
+        ]
+
+    async def async_get_value_metadata(self, val: Union[Value, str]) -> ValueMetadata:
+        """Send getValueMetadata command to Node."""
+        # a value may be specified as value_id or the value itself
+        if not isinstance(val, Value):
+            val = self.values[val]
+        # the value object needs to be send to the server
+        data = await self.client.async_send_command(
+            {
+                "command": "node.get_value_metadata",
+                "nodeId": self.node_id,
+                "valueId": val.data,
+            }
+        )
+        return ValueMetadata(cast(MetaDataType, data))
+
+    async def async_abort_firmware_update(self) -> None:
+        """Send abortFirmwareUpdate command to Node."""
+        await self.client.async_send_json_message(
+            {
+                "command": "node.abort_firmware_update",
+                "nodeId": self.node_id,
+            }
+        )
+
     def handle_wake_up(self, event: Event) -> None:
         """Process a node wake up event."""
 
     def handle_sleep(self, event: Event) -> None:
         """Process a node sleep event."""
 
     def handle_dead(self, event: Event) -> None:
```

### Comparing `zwave-js-server-python-0.8.0/zwave_js_server/model/value.py` & `zwave-js-server-python-0.9.0/zwave_js_server/model/value.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class MetaDataType(TypedDict, total=False):
     """Represent a metadata data dict type."""
 
     type: str  # required
     readable: bool  # required
-    writable: bool  # required
+    writeable: bool  # required
     description: str
     label: str
     min: int
     max: int
     unit: str
     states: Dict[int, str]
     ccSpecific: Dict[str, Any]
@@ -59,17 +59,17 @@
 
     @property
     def readable(self) -> Optional[bool]:
         """Return readable."""
         return self.data.get("readable")
 
     @property
-    def writable(self) -> Optional[bool]:
+    def writeable(self) -> Optional[bool]:
         """Return writeable."""
-        return self.data.get("writable")
+        return self.data.get("writeable")
 
     @property
     def label(self) -> Optional[str]:
         """Return label."""
         return self.data.get("label")
 
     @property
```

### Comparing `zwave-js-server-python-0.8.0/zwave_js_server/version.py` & `zwave-js-server-python-0.9.0/zwave_js_server/version.py`

 * *Files identical despite different names*

### Comparing `zwave-js-server-python-0.8.0/zwave_js_server_python.egg-info/PKG-INFO` & `zwave-js-server-python-0.9.0/zwave_js_server_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zwave-js-server-python
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python wrapper for zwave-js-server
 Home-page: https://github.com/home-assistant-libs/zwave-js-server-python
 Author: Home Assistant Team
 Author-email: hello@home-assistant.io
 License: UNKNOWN
 Download-URL: https://github.com/home-assistant-libs/zwave-js-server-python
 Description: # zwave-js-server-python
```

### Comparing `zwave-js-server-python-0.8.0/zwave_js_server_python.egg-info/SOURCES.txt` & `zwave-js-server-python-0.9.0/zwave_js_server_python.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 zwave_js_server/__init__.py
 zwave_js_server/__main__.py
 zwave_js_server/client.py
 zwave_js_server/const.py
 zwave_js_server/event.py
 zwave_js_server/version.py
 zwave_js_server/model/__init__.py
+zwave_js_server/model/association.py
 zwave_js_server/model/controller.py
 zwave_js_server/model/device_class.py
 zwave_js_server/model/device_config.py
 zwave_js_server/model/driver.py
 zwave_js_server/model/node.py
 zwave_js_server/model/value.py
 zwave_js_server_python.egg-info/PKG-INFO
```

