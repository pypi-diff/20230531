# Comparing `tmp/zhonghong_climate-1.0.2.tar.gz` & `tmp/zhonghong_climate-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhonghong_climate-1.0.2.tar", last modified: Tue May 30 07:35:50 2023, max compression
+gzip compressed data, was "zhonghong_climate-1.0.3.tar", last modified: Wed May 31 06:19:51 2023, max compression
```

## Comparing `zhonghong_climate-1.0.2.tar` & `zhonghong_climate-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 07:35:50.603321 zhonghong_climate-1.0.2/
--rw-rw-rw-   0        0        0      752 2023-05-30 07:35:50.603321 zhonghong_climate-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       62 2023-05-30 07:21:52.000000 zhonghong_climate-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-30 07:35:50.608339 zhonghong_climate-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1051 2023-05-30 07:21:52.000000 zhonghong_climate-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 07:35:50.568614 zhonghong_climate-1.0.2/zhonghong_climate/
--rw-rw-rw-   0        0        0       31 2023-05-30 07:22:47.000000 zhonghong_climate-1.0.2/zhonghong_climate/__init__.py
--rw-rw-rw-   0        0        0     3485 2023-05-30 07:21:52.000000 zhonghong_climate-1.0.2/zhonghong_climate/helper.py
--rw-rw-rw-   0        0        0     8456 2023-05-30 07:24:22.000000 zhonghong_climate-1.0.2/zhonghong_climate/hub.py
--rw-rw-rw-   0        0        0     4850 2023-05-30 07:21:52.000000 zhonghong_climate-1.0.2/zhonghong_climate/hvac.py
--rw-rw-rw-   0        0        0     8297 2023-05-30 07:21:52.000000 zhonghong_climate-1.0.2/zhonghong_climate/protocol.py
--rw-rw-rw-   0        0        0       23 2023-05-30 07:25:48.000000 zhonghong_climate-1.0.2/zhonghong_climate/version.py
-drwxrwxrwx   0        0        0        0 2023-05-30 07:35:50.603321 zhonghong_climate-1.0.2/zhonghong_climate.egg-info/
--rw-rw-rw-   0        0        0      752 2023-05-30 07:35:50.000000 zhonghong_climate-1.0.2/zhonghong_climate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-05-30 07:35:50.000000 zhonghong_climate-1.0.2/zhonghong_climate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 07:35:50.000000 zhonghong_climate-1.0.2/zhonghong_climate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-30 07:35:50.000000 zhonghong_climate-1.0.2/zhonghong_climate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-30 07:35:50.000000 zhonghong_climate-1.0.2/zhonghong_climate.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 06:19:51.883732 zhonghong_climate-1.0.3/
+-rw-rw-rw-   0        0        0      752 2023-05-31 06:19:51.883732 zhonghong_climate-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       62 2023-05-30 07:21:52.000000 zhonghong_climate-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-31 06:19:51.883732 zhonghong_climate-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1051 2023-05-30 07:21:52.000000 zhonghong_climate-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:19:51.861629 zhonghong_climate-1.0.3/zhonghong_climate/
+-rw-rw-rw-   0        0        0       31 2023-05-30 07:22:47.000000 zhonghong_climate-1.0.3/zhonghong_climate/__init__.py
+-rw-rw-rw-   0        0        0     3485 2023-05-30 07:21:52.000000 zhonghong_climate-1.0.3/zhonghong_climate/helper.py
+-rw-rw-rw-   0        0        0     8990 2023-05-31 06:15:04.000000 zhonghong_climate-1.0.3/zhonghong_climate/hub.py
+-rw-rw-rw-   0        0        0     4958 2023-05-31 06:15:14.000000 zhonghong_climate-1.0.3/zhonghong_climate/hvac.py
+-rw-rw-rw-   0        0        0     8297 2023-05-30 07:21:52.000000 zhonghong_climate-1.0.3/zhonghong_climate/protocol.py
+-rw-rw-rw-   0        0        0       23 2023-05-31 06:15:17.000000 zhonghong_climate-1.0.3/zhonghong_climate/version.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:19:51.882572 zhonghong_climate-1.0.3/zhonghong_climate.egg-info/
+-rw-rw-rw-   0        0        0      752 2023-05-31 06:19:51.000000 zhonghong_climate-1.0.3/zhonghong_climate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-05-31 06:19:51.000000 zhonghong_climate-1.0.3/zhonghong_climate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 06:19:51.000000 zhonghong_climate-1.0.3/zhonghong_climate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-31 06:19:51.000000 zhonghong_climate-1.0.3/zhonghong_climate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-31 06:19:51.000000 zhonghong_climate-1.0.3/zhonghong_climate.egg-info/top_level.txt
```

### Comparing `zhonghong_climate-1.0.2/PKG-INFO` & `zhonghong_climate-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhonghong_climate
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python library for interfacing with ZhongHong HVAC controller
 Home-page: https://github.com/heculess/zhonghong_hvac
 Author: heculess lau
 Author-email: heculess@hotmail.com
 License: Apache
 Keywords: zhonghong climate hvac
 Classifier: Development Status :: 4 - Beta
```

### Comparing `zhonghong_climate-1.0.2/setup.py` & `zhonghong_climate-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `zhonghong_climate-1.0.2/zhonghong_climate/helper.py` & `zhonghong_climate-1.0.3/zhonghong_climate/helper.py`

 * *Files identical despite different names*

### Comparing `zhonghong_climate-1.0.2/zhonghong_climate/hub.py` & `zhonghong_climate-1.0.3/zhonghong_climate/hub.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,24 +2,22 @@
 import logging
 import socket
 import time
 from collections import defaultdict
 from sys import platform
 from threading import Thread
 from typing import Callable, DefaultDict, List
-
 import attr
 
 from . import helper, protocol
 
 logger = logging.getLogger(__name__)
 
 SOCKET_BUFSIZE = 1024
 
-
 class ZhongHongGateway:
     def __init__(self, ip_addr: str, port: int, gw_addr: int):
         self.gw_addr = gw_addr
         self.ip_addr = ip_addr
         self.port = port
         self.available = True
         self.sock = None
@@ -67,85 +65,100 @@
         message = protocol.AcData()
         message.header = protocol.Header(self.gw_addr,
                                          protocol.FuncCode.STATUS.value,
                                          protocol.CtlStatus.ONE.value, 1)
         message.add(ac_addr)
         return self.send(message)
 
+    def update_gw_status(self, status: bool) -> None:
+    	
+        if self.available == status:
+            return
+            
+        self.available = status
+        
+        if not self.available:
+            for addr in self.devices:
+                self.devices[addr].error_code = -1     	                
+                self.devices[addr].call_status_update()
+        
     def send(self, ac_data: protocol.AcData) -> None:
         def _send(retry_count):
             try:
+                if self.sock is None:
+                    self.open_socket()
                 self.sock.settimeout(10.0)
                 logger.debug("send >> %s", ac_data.hex())
                 self.sock.send(ac_data.encode())
                 self.sock.settimeout(None)
 
             except socket.timeout:
-                logger.error("Connot connect to gateway %s:%s", self.ip_addr,
+                logger.debug("Connot connect to gateway %s:%s", self.ip_addr,
                              self.port)
-                self.available = False
+                self.update_gw_status(False)
                 return
 
             except OSError as e:
                 if e.errno == 32:  # Broken pipe
-                    logger.error("OSError 32 raise, Broken pipe", exc_info=e)
+                    logger.debug("OSError 32 raise, Broken pipe", exc_info=e)
                 if retry_count < self.max_retry:
                     retry_count += 1
                     self.open_socket()
                     _send(retry_count)
-                self.available = False
+                self.update_gw_status(False)
 
         _send(0)
 
     def _validate_data(self, data):
         if data is None:
             logger.error('No data in response from hub %s', data)
             return False
 
         return True
 
     def _get_data(self):
-        if self.sock is None:
-            self.open_socket()
-
+  
         try:
+            if self.sock is None:
+                self.open_socket()
+                
             return self.sock.recv(SOCKET_BUFSIZE)
 
         except ConnectionResetError:
             logger.debug("Connection reset by peer")
             self.open_socket()
-            self.available = False
+            self.update_gw_status(False)
 
         except socket.timeout as e:
-            logger.error("timeout error", exc_info=e)
-            self.available = False
+            logger.debug("timeout error", exc_info=e)
+            self.update_gw_status(False)
 
         except OSError as e:
             if e.errno == 9:  # when socket close, errorno 9 will raise
                 logger.debug("OSError 9 raise, socket is closed")
 
             else:
-                logger.error("unknown error when recv", exc_info=e)
-            self.available = False
+                logger.debug("unknown error when recv", exc_info=e)
+            self.update_gw_status(False)
 
         except Exception as e:
-            logger.error("unknown error when recv", exc_info=e)
-            self.available = False
+            logger.debug("unknown error when recv", exc_info=e)
+            self.update_gw_status(False)
 
         return None
 
     def _listen_to_msg(self):
         while self._listening:
             data = self._get_data()
 
             if not data:
                 continue
 
             logger.debug("recv data << %s", protocol.bytes_debug_str(data))
-            self.available = True
+            self.update_gw_status(True)
 
             for ac_data in helper.get_ac_data(data):
                 logger.debug("get ac_data << %s", ac_data)
 
                 if ac_data.func_code == protocol.FuncCode.STATUS:
                     for payload in ac_data:
                         if not isinstance(payload, protocol.AcStatus):
```

### Comparing `zhonghong_climate-1.0.2/zhonghong_climate/hvac.py` & `zhonghong_climate-1.0.3/zhonghong_climate/hvac.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import enum
 import json
 import logging
+import socket
 from typing import Callable, List
 
 from . import hub, protocol
 
 logger = logging.getLogger(__name__)
 
 
@@ -21,15 +22,15 @@
         self.target_temperature = None
         self.current_operation = None
         self.current_fan_mode = None
         self.current_temperature = None
         self.error_code = None
         self.gw.add_device(self)
 
-    def _call_status_update(self):
+    def call_status_update(self):
         for func in self.status_callback:
             if callable(func):
                 func(self)
 
     def _status_update(self, ac_status: protocol.AcStatus) -> bool:
         assert self.ac_addr == ac_status.ac_addr
         dirty = False
@@ -42,38 +43,41 @@
             if getattr(self, _attr) != value:
                 setattr(self, _attr, value)
                 dirty = True
 
         if dirty:
             logger.debug("[callback]hvac %s status updated: %s", self.ac_addr,
                          self.status())
-            self._call_status_update()
+            self.call_status_update()
         else:
             logger.debug("[callback]hvac %s status remains the same: %s",
                          self.ac_addr, self.status())
 
     def set_attr(self, func_code, value) -> bool:
         if func_code == protocol.FuncCode.CTL_POWER:
             self.switch_status = value.name
         elif func_code == protocol.FuncCode.CTL_TEMPERATURE:
             self.target_temperature = value
         elif func_code == protocol.FuncCode.CTL_OPERATION:
             self.current_operation = value.name
         elif func_code == protocol.FuncCode.CTL_FAN_MODE:
             self.current_fan_mode = value.name
-        self._call_status_update()
+        self.call_status_update()
 
     def register_update_callback(self, _callable: Callable) -> bool:
         if callable(_callable):
             self.status_callback.append(_callable)
             return True
         return False
 
     def send(self, ac_data: protocol.AcData) -> None:
-        self.gw.send(ac_data)
+        try:
+            self.gw.send(ac_data)
+        except Exception as e:
+            self.error_code = "lost gateway"
 
     def update(self) -> bool:
         message = protocol.AcData()
         message.header = protocol.Header(
             self.gw_addr, protocol.FuncCode.STATUS, protocol.CtlStatus.ONE, 1)
         message.add(self.ac_addr)
         self.gw.query_status(self.ac_addr)
```

### Comparing `zhonghong_climate-1.0.2/zhonghong_climate/protocol.py` & `zhonghong_climate-1.0.3/zhonghong_climate/protocol.py`

 * *Files identical despite different names*

### Comparing `zhonghong_climate-1.0.2/zhonghong_climate.egg-info/PKG-INFO` & `zhonghong_climate-1.0.3/zhonghong_climate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhonghong-climate
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python library for interfacing with ZhongHong HVAC controller
 Home-page: https://github.com/heculess/zhonghong_hvac
 Author: heculess lau
 Author-email: heculess@hotmail.com
 License: Apache
 Keywords: zhonghong climate hvac
 Classifier: Development Status :: 4 - Beta
```

