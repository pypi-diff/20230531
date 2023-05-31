# Comparing `tmp/aioairzone-cloud-0.1.6.tar.gz` & `tmp/aioairzone-cloud-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairzone-cloud-0.1.6.tar", last modified: Thu May 25 09:36:44 2023, max compression
+gzip compressed data, was "aioairzone-cloud-0.1.7.tar", last modified: Wed May 31 18:00:15 2023, max compression
```

## Comparing `aioairzone-cloud-0.1.6.tar` & `aioairzone-cloud-0.1.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-25 09:36:44.321146 aioairzone-cloud-0.1.6/
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.6/LICENSE
--rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.6/MANIFEST.in
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-25 09:36:44.321146 aioairzone-cloud-0.1.6/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      746 2023-05-22 17:43:05.000000 aioairzone-cloud-0.1.6/README.md
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-25 09:36:44.321146 aioairzone-cloud-0.1.6/aioairzone_cloud/
--rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.1.6/aioairzone_cloud/__init__.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      156 2023-05-25 09:17:49.000000 aioairzone-cloud-0.1.6/aioairzone_cloud/aidoo.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    18280 2023-05-24 19:18:04.000000 aioairzone-cloud-0.1.6/aioairzone_cloud/cloudapi.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1527 2023-05-23 16:19:08.000000 aioairzone-cloud-0.1.6/aioairzone_cloud/common.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     6705 2023-05-25 09:35:02.000000 aioairzone-cloud-0.1.6/aioairzone_cloud/const.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     3706 2023-05-25 09:35:02.000000 aioairzone-cloud-0.1.6/aioairzone_cloud/device.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      806 2023-05-21 08:34:57.000000 aioairzone-cloud-0.1.6/aioairzone_cloud/exceptions.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    16988 2023-05-25 06:16:28.000000 aioairzone-cloud-0.1.6/aioairzone_cloud/hvac.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1181 2023-05-24 18:32:54.000000 aioairzone-cloud-0.1.6/aioairzone_cloud/installation.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-05-22 07:54:27.000000 aioairzone-cloud-0.1.6/aioairzone_cloud/py.typed
--rw-r--r--   0 noltari   (1000) noltari   (1000)      976 2023-05-25 09:18:17.000000 aioairzone-cloud-0.1.6/aioairzone_cloud/system.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     4141 2023-05-25 08:46:37.000000 aioairzone-cloud-0.1.6/aioairzone_cloud/webserver.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2231 2023-05-25 06:23:06.000000 aioairzone-cloud-0.1.6/aioairzone_cloud/zone.py
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-25 09:36:44.321146 aioairzone-cloud-0.1.6/aioairzone_cloud.egg-info/
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-25 09:36:44.000000 aioairzone-cloud-0.1.6/aioairzone_cloud.egg-info/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      670 2023-05-25 09:36:44.000000 aioairzone-cloud-0.1.6/aioairzone_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-25 09:36:44.000000 aioairzone-cloud-0.1.6/aioairzone_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-25 09:36:44.000000 aioairzone-cloud-0.1.6/aioairzone_cloud.egg-info/not-zip-safe
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-25 09:36:44.000000 aioairzone-cloud-0.1.6/aioairzone_cloud.egg-info/requires.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-05-25 09:36:44.000000 aioairzone-cloud-0.1.6/aioairzone_cloud.egg-info/top_level.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1029 2023-05-25 09:35:39.000000 aioairzone-cloud-0.1.6/pyproject.toml
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.6/requirements.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-05-25 09:36:44.321146 aioairzone-cloud-0.1.6/setup.cfg
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-31 18:00:15.290126 aioairzone-cloud-0.1.7/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.7/LICENSE
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.7/MANIFEST.in
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-31 18:00:15.290126 aioairzone-cloud-0.1.7/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      746 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.7/README.md
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-31 18:00:15.290126 aioairzone-cloud-0.1.7/aioairzone_cloud/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/__init__.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      156 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/aidoo.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    18280 2023-05-31 17:41:58.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/cloudapi.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1527 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/common.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     6843 2023-05-31 17:41:58.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/const.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     4293 2023-05-31 17:51:01.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/device.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      806 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/exceptions.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    16988 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/hvac.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1181 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/installation.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/py.typed
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      976 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/system.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     4140 2023-05-31 17:58:06.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/webserver.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2231 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/zone.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-31 18:00:15.290126 aioairzone-cloud-0.1.7/aioairzone_cloud.egg-info/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-31 18:00:15.000000 aioairzone-cloud-0.1.7/aioairzone_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      670 2023-05-31 18:00:15.000000 aioairzone-cloud-0.1.7/aioairzone_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-31 18:00:15.000000 aioairzone-cloud-0.1.7/aioairzone_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-31 18:00:15.000000 aioairzone-cloud-0.1.7/aioairzone_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-31 18:00:15.000000 aioairzone-cloud-0.1.7/aioairzone_cloud.egg-info/requires.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-05-31 18:00:15.000000 aioairzone-cloud-0.1.7/aioairzone_cloud.egg-info/top_level.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1029 2023-05-31 17:59:14.000000 aioairzone-cloud-0.1.7/pyproject.toml
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.7/requirements.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-05-31 18:00:15.290126 aioairzone-cloud-0.1.7/setup.cfg
```

### Comparing `aioairzone-cloud-0.1.6/LICENSE` & `aioairzone-cloud-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.6/PKG-INFO` & `aioairzone-cloud-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.1.6
+Version: 0.1.7
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.1.6/README.md` & `aioairzone-cloud-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.6/aioairzone_cloud/cloudapi.py` & `aioairzone-cloud-0.1.7/aioairzone_cloud/cloudapi.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.6/aioairzone_cloud/common.py` & `aioairzone-cloud-0.1.7/aioairzone_cloud/common.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.6/aioairzone_cloud/const.py` & `aioairzone-cloud-0.1.7/aioairzone_cloud/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,36 +72,38 @@
 API_USER: Final[str] = "user"
 API_USER_ID: Final[str] = "user_id"
 API_USER_LOGOUT: Final[str] = "user/logout"
 API_USER_MODE_CONF: Final[str] = "usermode_conf"
 API_V1: Final[str] = "api/v1"
 API_WARNINGS: Final[str] = "warnings"
 API_WS: Final[str] = "ws"
+API_WS_CONNECTED: Final[str] = "ws_connected"
 API_WS_FW: Final[str] = "ws_fw"
 API_WS_ID: Final[str] = "ws_id"
 API_WS_IDS: Final[str] = "ws_ids"
 API_WS_TYPE: Final[str] = "ws_type"
 API_ZONE_NUMBER: Final[str] = "zone_number"
 
 API_AZ_AIDOO: Final[str] = "aidoo"
 API_AZ_SYSTEM: Final[str] = "az_system"
 API_AZ_ZONE: Final[str] = "az_zone"
 
 API_DEFAULT_TEMP_STEP: Final[float] = 0.5
 
 AZD_AIDOOS: Final[str] = "aidoos"
-AZD_CONNECTED: Final[str] = "connected"
+AZD_AVAILABLE: Final[str] = "available"
 AZD_CONNECTION_DATE: Final[str] = "connection-date"
 AZD_DISCONNECTION_DATE: Final[str] = "disconnection-date"
 AZD_ERRORS: Final[str] = "errors"
 AZD_FIRMWARE: Final[str] = "firmware"
 AZD_HUMIDITY: Final[str] = "humidity"
 AZD_ID: Final[str] = "id"
 AZD_INSTALLATION: Final[str] = "installation"
 AZD_INSTALLATIONS: Final[str] = "installations"
+AZD_IS_CONNECTED: Final[str] = "is-connected"
 AZD_MASTER: Final[str] = "master"
 AZD_MODE: Final[str] = "mode"
 AZD_MODES: Final[str] = "modes"
 AZD_NAME: Final[str] = "name"
 AZD_POWER: Final[str] = "power"
 AZD_PROBLEMS: Final[str] = "problems"
 AZD_SYSTEM: Final[str] = "system"
@@ -134,14 +136,15 @@
 AZD_WEBSERVER: Final[str] = "web-server"
 AZD_WEBSERVERS: Final[str] = "web-servers"
 AZD_WIFI_CHANNEL: Final[str] = "wifi-channel"
 AZD_WIFI_MAC: Final[str] = "wifi-mac"
 AZD_WIFI_QUALITY: Final[str] = "wifi-quality"
 AZD_WIFI_RSSI: Final[str] = "wifi-rssi"
 AZD_WIFI_SSID: Final[str] = "wifi-ssid"
+AZD_WS_CONNECTED: Final[str] = "ws-connected"
 AZD_ZONE: Final[str] = "zone"
 AZD_ZONES: Final[str] = "zones"
 
 HEADER_AUTHORIZATION: Final[str] = "Authorization"
 HEADER_BEARER: Final[str] = "Bearer"
 
 HTTP_CALL_TIMEOUT: Final[int] = 10
```

### Comparing `aioairzone-cloud-0.1.6/aioairzone_cloud/device.py` & `aioairzone-cloud-0.1.7/aioairzone_cloud/device.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 from .const import (
     API_DEVICE_ID,
     API_ERRORS,
     API_IS_CONNECTED,
     API_MODE,
     API_MODE_AVAIL,
     API_WARNINGS,
-    AZD_CONNECTED,
+    API_WS_CONNECTED,
+    AZD_AVAILABLE,
     AZD_ERRORS,
     AZD_ID,
     AZD_INSTALLATION,
+    AZD_IS_CONNECTED,
     AZD_MODE,
     AZD_MODES,
     AZD_NAME,
     AZD_PROBLEMS,
     AZD_WARNINGS,
     AZD_WEBSERVER,
+    AZD_WS_CONNECTED,
 )
 
 
 class Device:
     """Airzone Cloud Device."""
 
     name: str
@@ -34,30 +37,33 @@
         self.errors: list[str] = []
         self.id = str(device_data[API_DEVICE_ID])
         self.installation_id = inst_id
         self.mode: OperationMode | None = None
         self.modes: list[OperationMode] = []
         self.warnings: list[str] = []
         self.webserver_id = ws_id
+        self.ws_connected: bool = True
 
         if API_IS_CONNECTED in device_data:
-            self.connected = bool(device_data[API_IS_CONNECTED])
+            self.is_connected = bool(device_data[API_IS_CONNECTED])
         else:
-            self.connected = True
+            self.is_connected = True
 
     def data(self) -> dict[str, Any]:
         """Return Device data."""
         data = {
-            AZD_CONNECTED: self.get_connected(),
+            AZD_AVAILABLE: self.get_available(),
             AZD_ID: self.get_id(),
             AZD_INSTALLATION: self.get_installation(),
+            AZD_IS_CONNECTED: self.get_is_connected(),
             AZD_MODE: self.get_mode(),
             AZD_NAME: self.get_name(),
             AZD_PROBLEMS: self.get_problems(),
             AZD_WEBSERVER: self.get_webserver(),
+            AZD_WS_CONNECTED: self.get_ws_connected(),
         }
 
         errors = self.get_errors()
         if len(errors) > 0:
             data[AZD_ERRORS] = errors
 
         modes = self.get_modes()
@@ -66,30 +72,34 @@
 
         warnings = self.get_warnings()
         if len(warnings) > 0:
             data[AZD_WARNINGS] = warnings
 
         return data
 
-    def get_connected(self) -> bool:
-        """Return Device connection status."""
-        return self.connected
+    def get_available(self) -> bool:
+        """Return availability status."""
+        return self.is_connected and self.ws_connected
 
     def get_errors(self) -> list[str]:
         """Return Device errors."""
         return self.errors
 
     def get_id(self) -> str:
         """Return Device ID."""
         return self.id
 
     def get_installation(self) -> str:
         """Return Installation ID."""
         return self.installation_id
 
+    def get_is_connected(self) -> bool:
+        """Return Device connection status."""
+        return self.is_connected
+
     def get_mode(self) -> OperationMode | None:
         """Return Device mode."""
         return self.mode
 
     def get_modes(self) -> list[OperationMode] | None:
         """Return Device modes."""
         if len(self.modes) > 0:
@@ -108,18 +118,24 @@
         """Return Device warnings."""
         return self.warnings
 
     def get_webserver(self) -> str:
         """Return WebServer ID."""
         return self.webserver_id
 
+    def get_ws_connected(self) -> bool:
+        """Return WebServer connection status."""
+        return self.ws_connected
+
     def update(self, data: dict[str, Any]) -> None:
         """Update Device data."""
         if API_IS_CONNECTED in data:
-            self.connected = bool(data[API_IS_CONNECTED])
+            self.is_connected = bool(data[API_IS_CONNECTED])
+        if API_WS_CONNECTED in data:
+            self.ws_connected = bool(data[API_WS_CONNECTED])
 
         if API_ERRORS in data:
             self.errors = []
             for error in data[API_ERRORS]:
                 self.errors += [error]
 
         if API_MODE in data:
```

### Comparing `aioairzone-cloud-0.1.6/aioairzone_cloud/exceptions.py` & `aioairzone-cloud-0.1.7/aioairzone_cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.6/aioairzone_cloud/hvac.py` & `aioairzone-cloud-0.1.7/aioairzone_cloud/hvac.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.6/aioairzone_cloud/installation.py` & `aioairzone-cloud-0.1.7/aioairzone_cloud/installation.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.6/aioairzone_cloud/system.py` & `aioairzone-cloud-0.1.7/aioairzone_cloud/system.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.6/aioairzone_cloud/webserver.py` & `aioairzone-cloud-0.1.7/aioairzone_cloud/webserver.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     API_STAT_CHANNEL,
     API_STAT_QUALITY,
     API_STAT_RSSI,
     API_STAT_SSID,
     API_STATUS,
     API_WS_FW,
     API_WS_TYPE,
-    AZD_CONNECTED,
+    AZD_AVAILABLE,
     AZD_CONNECTION_DATE,
     AZD_DISCONNECTION_DATE,
     AZD_FIRMWARE,
     AZD_ID,
     AZD_INSTALLATION,
     AZD_TYPE,
     AZD_WIFI_CHANNEL,
@@ -32,63 +32,63 @@
 
 
 class WebServer:
     """Airzone Cloud WebServer."""
 
     def __init__(self, inst_id: str, ws_id: str):
         """Airzone Cloud WebServer init."""
-        self.connected: bool | None = None
         self.connection_date: str | None = None
         self.disconnection_date: str | None = None
         self.firmware: str | None = None
         self.id = ws_id
         self.installation_id = inst_id
+        self.is_connected: bool = False
         self.stat_quality: int | None = None
         self.type: str | None = None
         self.wifi_channel: int | None = None
         self.wifi_mac: str | None = None
         self.wifi_quality: int | None = None
         self.wifi_rssi: int | None = None
         self.wifi_ssid: str | None = None
 
     def update(self, data: dict[str, Any]) -> None:
         """Update WebServer data."""
-        self.connected = bool(data[API_STATUS][API_IS_CONNECTED])
         self.connection_date = str(data[API_STATUS][API_CONNECTION_DATE])
         self.disconnection_date = str(data[API_STATUS][API_DISCONNECTION_DATE])
         self.firmware = str(data[API_CONFIG][API_WS_FW])
+        self.is_connected = bool(data[API_STATUS][API_IS_CONNECTED])
         self.type = str(data[API_WS_TYPE])
         self.wifi_channel = int(data[API_CONFIG][API_STAT_CHANNEL])
         self.wifi_quality = int(data[API_STATUS][API_STAT_QUALITY])
         self.wifi_rssi = int(data[API_STATUS][API_STAT_RSSI])
         self.wifi_ssid = str(data[API_CONFIG][API_STAT_SSID])
 
         if API_STAT_AP_MAC in data[API_CONFIG]:
             self.wifi_mac = str(data[API_CONFIG][API_STAT_AP_MAC])
 
     def data(self) -> dict[str, Any]:
         """Return WebServer data."""
         return {
-            AZD_CONNECTED: self.get_connected(),
+            AZD_AVAILABLE: self.get_available(),
             AZD_CONNECTION_DATE: self.get_connection_date(),
             AZD_DISCONNECTION_DATE: self.get_disconnection_date(),
             AZD_FIRMWARE: self.get_firmware(),
             AZD_ID: self.get_id(),
             AZD_INSTALLATION: self.get_installation(),
             AZD_TYPE: self.get_type(),
             AZD_WIFI_CHANNEL: self.get_wifi_channel(),
             AZD_WIFI_MAC: self.get_wifi_mac(),
             AZD_WIFI_QUALITY: self.get_wifi_quality(),
             AZD_WIFI_RSSI: self.get_wifi_rssi(),
             AZD_WIFI_SSID: self.get_wifi_ssid(),
         }
 
-    def get_connected(self) -> bool | None:
-        """Return connected status."""
-        return self.connected
+    def get_available(self) -> bool:
+        """Return availability status."""
+        return self.is_connected
 
     def get_connection_date(self) -> str | None:
         """Return connection date."""
         return self.connection_date
 
     def get_disconnection_date(self) -> str | None:
         """Return disconnection date."""
```

### Comparing `aioairzone-cloud-0.1.6/aioairzone_cloud/zone.py` & `aioairzone-cloud-0.1.7/aioairzone_cloud/zone.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.6/aioairzone_cloud.egg-info/PKG-INFO` & `aioairzone-cloud-0.1.7/aioairzone_cloud.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.1.6
+Version: 0.1.7
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.1.6/aioairzone_cloud.egg-info/SOURCES.txt` & `aioairzone-cloud-0.1.7/aioairzone_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.6/pyproject.toml` & `aioairzone-cloud-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aioairzone-cloud"
-version = "0.1.6"
+version = "0.1.7"
 description = "Library to control Airzone Cloud devices"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "Apache-2.0"}
 keywords = ["airzone", "cloud", "hvac", "home"] 
 authors = [
   {name = "Álvaro Fernández Rojas", email = "noltari@gmail.com" }
```

