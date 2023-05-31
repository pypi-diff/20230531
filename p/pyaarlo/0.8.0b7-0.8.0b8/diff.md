# Comparing `tmp/pyaarlo-0.8.0b7.tar.gz` & `tmp/pyaarlo-0.8.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaarlo-0.8.0b7.tar", last modified: Wed May 10 11:32:06 2023, max compression
+gzip compressed data, was "pyaarlo-0.8.0b8.tar", last modified: Wed May 31 18:16:25 2023, max compression
```

## Comparing `pyaarlo-0.8.0b7.tar` & `pyaarlo-0.8.0b8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-05-10 11:32:06.282720 pyaarlo-0.8.0b7/
--rw-r--r--   0 steve     (1000) steve     (1000)     7652 2019-08-16 18:58:59.000000 pyaarlo-0.8.0b7/LICENSE
--rw-rw-r--   0 steve     (1000) steve     (1000)    19613 2023-05-10 11:32:06.282720 pyaarlo-0.8.0b7/PKG-INFO
--rw-rw-r--   0 steve     (1000) steve     (1000)    18439 2022-02-13 14:58:05.000000 pyaarlo-0.8.0b7/README.md
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-05-10 11:32:06.282720 pyaarlo-0.8.0b7/pyaarlo/
--rw-rw-r--   0 steve     (1000) steve     (1000)    27069 2023-05-10 11:30:32.000000 pyaarlo-0.8.0b7/pyaarlo/__init__.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    42574 2023-05-10 11:30:32.000000 pyaarlo-0.8.0b7/pyaarlo/backend.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     4925 2023-05-10 01:20:55.000000 pyaarlo-0.8.0b7/pyaarlo/background.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    21900 2023-02-07 02:39:52.000000 pyaarlo-0.8.0b7/pyaarlo/base.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    50293 2023-04-11 00:17:07.000000 pyaarlo-0.8.0b7/pyaarlo/camera.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     6630 2023-05-10 11:30:32.000000 pyaarlo-0.8.0b7/pyaarlo/cfg.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     9513 2023-05-09 23:31:57.000000 pyaarlo-0.8.0b7/pyaarlo/constant.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    11646 2023-02-06 16:43:11.000000 pyaarlo-0.8.0b7/pyaarlo/device.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     7676 2022-10-27 14:08:34.000000 pyaarlo-0.8.0b7/pyaarlo/doorbell.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     2569 2023-02-06 18:29:36.000000 pyaarlo-0.8.0b7/pyaarlo/light.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     6190 2023-05-10 01:12:15.000000 pyaarlo-0.8.0b7/pyaarlo/location.py
--rw-r--r--   0 steve     (1000) steve     (1000)    12449 2021-04-08 13:02:02.000000 pyaarlo-0.8.0b7/pyaarlo/main.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    16749 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b7/pyaarlo/media.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     5412 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b7/pyaarlo/ratls.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     3801 2022-03-03 18:35:12.000000 pyaarlo-0.8.0b7/pyaarlo/security_utils.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     1701 2023-02-05 15:10:18.000000 pyaarlo-0.8.0b7/pyaarlo/sensor.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     6294 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b7/pyaarlo/sseclient.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     2259 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b7/pyaarlo/storage.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     5183 2023-05-10 01:12:15.000000 pyaarlo-0.8.0b7/pyaarlo/super.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     7381 2022-11-27 01:24:01.000000 pyaarlo-0.8.0b7/pyaarlo/tfa.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     3365 2021-11-28 01:11:18.000000 pyaarlo-0.8.0b7/pyaarlo/util.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-05-10 11:32:06.282720 pyaarlo-0.8.0b7/pyaarlo.egg-info/
--rw-rw-r--   0 steve     (1000) steve     (1000)    19613 2023-05-10 11:32:06.000000 pyaarlo-0.8.0b7/pyaarlo.egg-info/PKG-INFO
--rw-rw-r--   0 steve     (1000) steve     (1000)      623 2023-05-10 11:32:06.000000 pyaarlo-0.8.0b7/pyaarlo.egg-info/SOURCES.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)        1 2023-05-10 11:32:06.000000 pyaarlo-0.8.0b7/pyaarlo.egg-info/dependency_links.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)       51 2023-05-10 11:32:06.000000 pyaarlo-0.8.0b7/pyaarlo.egg-info/entry_points.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)       82 2023-05-10 11:32:06.000000 pyaarlo-0.8.0b7/pyaarlo.egg-info/requires.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)        8 2023-05-10 11:32:06.000000 pyaarlo-0.8.0b7/pyaarlo.egg-info/top_level.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)       38 2023-05-10 11:32:06.282720 pyaarlo-0.8.0b7/setup.cfg
--rw-rw-r--   0 steve     (1000) steve     (1000)     1847 2023-05-10 11:30:32.000000 pyaarlo-0.8.0b7/setup.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-05-10 11:32:06.282720 pyaarlo-0.8.0b7/tests/
--rw-rw-r--   0 steve     (1000) steve     (1000)      269 2022-10-27 13:44:57.000000 pyaarlo-0.8.0b7/tests/test_backend.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-05-31 18:16:25.668292 pyaarlo-0.8.0b8/
+-rw-r--r--   0 steve     (1000) steve     (1000)     7652 2019-08-16 18:58:59.000000 pyaarlo-0.8.0b8/LICENSE
+-rw-rw-r--   0 steve     (1000) steve     (1000)    19613 2023-05-31 18:16:25.668292 pyaarlo-0.8.0b8/PKG-INFO
+-rw-rw-r--   0 steve     (1000) steve     (1000)    18439 2022-02-13 14:58:05.000000 pyaarlo-0.8.0b8/README.md
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-05-31 18:16:25.664292 pyaarlo-0.8.0b8/pyaarlo/
+-rw-rw-r--   0 steve     (1000) steve     (1000)    27069 2023-05-31 18:13:25.000000 pyaarlo-0.8.0b8/pyaarlo/__init__.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    42982 2023-05-31 18:13:25.000000 pyaarlo-0.8.0b8/pyaarlo/backend.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     4925 2023-05-10 01:20:55.000000 pyaarlo-0.8.0b8/pyaarlo/background.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    22075 2023-05-31 18:13:25.000000 pyaarlo-0.8.0b8/pyaarlo/base.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    50293 2023-04-11 00:17:07.000000 pyaarlo-0.8.0b8/pyaarlo/camera.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     6630 2023-05-10 11:30:32.000000 pyaarlo-0.8.0b8/pyaarlo/cfg.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     9513 2023-05-31 17:38:42.000000 pyaarlo-0.8.0b8/pyaarlo/constant.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    11646 2023-02-06 16:43:11.000000 pyaarlo-0.8.0b8/pyaarlo/device.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     7676 2022-10-27 14:08:34.000000 pyaarlo-0.8.0b8/pyaarlo/doorbell.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     2569 2023-02-06 18:29:36.000000 pyaarlo-0.8.0b8/pyaarlo/light.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     6190 2023-05-10 01:12:15.000000 pyaarlo-0.8.0b8/pyaarlo/location.py
+-rw-r--r--   0 steve     (1000) steve     (1000)    12449 2021-04-08 13:02:02.000000 pyaarlo-0.8.0b8/pyaarlo/main.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    16749 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b8/pyaarlo/media.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     5412 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b8/pyaarlo/ratls.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     3801 2022-03-03 18:35:12.000000 pyaarlo-0.8.0b8/pyaarlo/security_utils.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1701 2023-02-05 15:10:18.000000 pyaarlo-0.8.0b8/pyaarlo/sensor.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     6294 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b8/pyaarlo/sseclient.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     2259 2022-10-20 23:23:33.000000 pyaarlo-0.8.0b8/pyaarlo/storage.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     5183 2023-05-10 01:12:15.000000 pyaarlo-0.8.0b8/pyaarlo/super.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     7381 2022-11-27 01:24:01.000000 pyaarlo-0.8.0b8/pyaarlo/tfa.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     3365 2021-11-28 01:11:18.000000 pyaarlo-0.8.0b8/pyaarlo/util.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-05-31 18:16:25.664292 pyaarlo-0.8.0b8/pyaarlo.egg-info/
+-rw-rw-r--   0 steve     (1000) steve     (1000)    19613 2023-05-31 18:16:25.000000 pyaarlo-0.8.0b8/pyaarlo.egg-info/PKG-INFO
+-rw-rw-r--   0 steve     (1000) steve     (1000)      623 2023-05-31 18:16:25.000000 pyaarlo-0.8.0b8/pyaarlo.egg-info/SOURCES.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)        1 2023-05-31 18:16:25.000000 pyaarlo-0.8.0b8/pyaarlo.egg-info/dependency_links.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)       51 2023-05-31 18:16:25.000000 pyaarlo-0.8.0b8/pyaarlo.egg-info/entry_points.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)       82 2023-05-31 18:16:25.000000 pyaarlo-0.8.0b8/pyaarlo.egg-info/requires.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)        8 2023-05-31 18:16:25.000000 pyaarlo-0.8.0b8/pyaarlo.egg-info/top_level.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)       38 2023-05-31 18:16:25.668292 pyaarlo-0.8.0b8/setup.cfg
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1847 2023-05-31 18:13:25.000000 pyaarlo-0.8.0b8/setup.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2023-05-31 18:16:25.664292 pyaarlo-0.8.0b8/tests/
+-rw-rw-r--   0 steve     (1000) steve     (1000)      269 2022-10-27 13:44:57.000000 pyaarlo-0.8.0b8/tests/test_backend.py
```

### Comparing `pyaarlo-0.8.0b7/LICENSE` & `pyaarlo-0.8.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b7/PKG-INFO` & `pyaarlo-0.8.0b8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaarlo
-Version: 0.8.0b7
+Version: 0.8.0b8
 Summary: PyAarlo is a library that provides asynchronous access to Arlo security cameras.
 Home-page: https://github.com/twrecked/pyaarlo.git
 Author: Steve Herrell
 Author-email: steve.herrell@gmail.com
 License: LGPLv3+
 Project-URL: Bug Tracker, https://github.com/twrecked/pyaarlo/issues
 Project-URL: Documentation, https://github.com/twrecked/pyaarlo/blob/master/README.md
```

### Comparing `pyaarlo-0.8.0b7/README.md` & `pyaarlo-0.8.0b8/README.md`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b7/pyaarlo/__init__.py` & `pyaarlo-0.8.0b8/pyaarlo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from .storage import ArloStorage
 from .location import ArloLocation
 from .sensor import ArloSensor
 from .util import time_to_arlotime
 
 _LOGGER = logging.getLogger("pyaarlo")
 
-__version__ = "0.8.0b7"
+__version__ = "0.8.0b8"
 
 
 class PyArlo(object):
     """Entry point for all Arlo operations.
 
     This is used to login to Arlo, open and maintain an evenstream with Arlo, find and store devices and device
     state, provide keep-alive services and make sure media sources are kept up to date.
```

### Comparing `pyaarlo-0.8.0b7/pyaarlo/backend.py` & `pyaarlo-0.8.0b8/pyaarlo/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 
 # include token and session details
 class ArloBackEnd(object):
 
     _session_lock = threading.Lock()
     _session_info = {}
     _multi_location = False
+    _user_device_id = None
 
     def __init__(self, arlo):
 
         self._arlo = arlo
         self._lock = threading.Condition()
         self._req_lock = threading.Lock()
 
@@ -59,14 +60,15 @@
         self._use_mqtt = False
 
         self._requests = {}
         self._callbacks = {}
         self._resource_types = DEFAULT_RESOURCES
 
         self._load_session()
+        self._user_device_id = str(uuid.uuid4())
 
         # event thread stuff
         self._event_thread = None
         self._event_client = None
         self._event_connected = False
         self._stop_thread = False
 
@@ -145,28 +147,33 @@
         method="GET",
         params=None,
         headers=None,
         stream=False,
         raw=False,
         timeout=None,
         host=None,
+        authpost=False,
     ):
         if params is None:
             params = {}
         if headers is None:
             headers = {}
         if timeout is None:
             timeout = self._arlo.cfg.request_timeout
         try:
             with self._req_lock:
                 if host is None:
                     host = self._arlo.cfg.host
-                tid = self._transaction_id()
-                url = self._build_url(host + path, tid)
-                headers['x-transaction-id'] = tid
+                if authpost:
+                    url = host + path
+                else:
+                    tid = self._transaction_id()
+                    url = self._build_url(host + path, tid)
+                    headers['x-transaction-id'] = tid
+
                 self.vdebug("request-url={}".format(url))
                 self.vdebug("request-params=\n{}".format(pprint.pformat(params)))
                 self.vdebug("request-headers=\n{}".format(pprint.pformat(headers)))
                 if method == "GET":
                     r = self._session.get(
                         url,
                         params=params,
@@ -671,15 +678,15 @@
             "Accept": "application/json, text/plain, */*",
             "Accept-Encoding": "gzip, deflate, br",
             "Accept-Language": "en-GB,en;q=0.9,en-US;q=0.8",
             "Origin": ORIGIN_HOST,
             "Referer": REFERER_HOST,
             "Source": "arloCamWeb",
             "User-Agent": self._user_agent,
-            "x-user-device-id": self._user_id,
+            "x-user-device-id": self._user_device_id,
             "x-user-device-automation-name": "QlJPV1NFUg==",
             "x-user-device-type": "BROWSER",
         }
 
         # Handle 1015 error
         attempt = 0
         body = None
@@ -752,15 +759,20 @@
                     self._arlo.error("2fa startup failed")
                     return False
 
                 # start authentication with email
                 self.debug(
                     "starting auth with {}".format(self._arlo.cfg.tfa_type)
                 )
-                body = self.auth_post(AUTH_START_PATH, {"factorId": factor_id}, headers)
+                payload = {
+                    "factorId": factor_id,
+                    "factorType": "BROWSER",
+                    "userId": self._user_id
+                }
+                body = self.auth_post(AUTH_START_PATH, payload, headers)
                 if body is None:
                     self._arlo.error("2fa startAuth failed")
                     return False
                 factor_auth_code = body["factorAuthCode"]
 
                 # get code from TFA source
                 code = tfa.get()
@@ -822,15 +834,15 @@
             "Accept-Encoding": "gzip, deflate, br",
             "Accept-Language": "en-GB,en;q=0.9,en-US;q=0.8",
             "Authorization": self._token64,
             "Origin": ORIGIN_HOST,
             "Referer": REFERER_HOST,
             "User-Agent": self._user_agent,
             "Source": "arloCamWeb",
-            "x-user-device-id": self._user_id,
+            "x-user-device-id": self._user_device_id,
             "x-user-device-automation-name": "QlJPV1NFUg==",
             "x-user-device-type": "BROWSER",
         }
 
         # Validate it!
         validated = self.auth_get(
             AUTH_VALIDATE_PATH + "?data = {}".format(int(time.time())), {}, headers
@@ -1072,22 +1084,22 @@
             self.vdebug("post sent")
             self._arlo.bg.run(
                 self._request, path, "POST", params, headers, False, raw, timeout
             )
 
     def auth_post(self, path, params=None, headers=None, raw=False, timeout=None):
         return self._request(
-            path, "POST", params, headers, False, raw, timeout, self._arlo.cfg.auth_host
+            path, "POST", params, headers, False, raw, timeout, self._arlo.cfg.auth_host, authpost=True
         )
 
     def auth_get(
         self, path, params=None, headers=None, stream=False, raw=False, timeout=None
     ):
         return self._request(
-            path, "GET", params, headers, stream, raw, timeout, self._arlo.cfg.auth_host
+            path, "GET", params, headers, stream, raw, timeout, self._arlo.cfg.auth_host, authpost=True
         )
 
     @property
     def session(self):
         return self._session
 
     @property
```

### Comparing `pyaarlo-0.8.0b7/pyaarlo/background.py` & `pyaarlo-0.8.0b8/pyaarlo/background.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b7/pyaarlo/base.py` & `pyaarlo-0.8.0b8/pyaarlo/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     MODE_UPDATE_INTERVAL,
     MODEL_BABY,
     MODEL_ESSENTIAL,
     MODEL_GO,
     MODEL_HUB,
     MODEL_PRO_3_FLOODLIGHT,
     MODEL_PRO_4,
+    MODEL_WIRED_VIDEO_DOORBELL,
     MODEL_WIREFREE_VIDEO_DOORBELL,
     PING_CAPABILITY,
     RESOURCE_CAPABILITY,
     RESTART_PATH,
     SCHEDULE_KEY,
     SIREN_STATE_KEY,
     TEMPERATURE_KEY,
@@ -549,33 +550,37 @@
             if (
                 self.model_id.startswith(("VMB400", "VMB450"))
                 or self.model_id == MODEL_GO
             ):
                 return True
 
         if cap in (PING_CAPABILITY,):
+
+            # Always true for these devices.
             if self.model_id.startswith(MODEL_BABY):
                 return True
+            if self.model_id.startswith(MODEL_WIRED_VIDEO_DOORBELL):
+                return True
+
+            # Don't ping these devices ever.
+            if self.model_id.startswith(
+                    (MODEL_WIREFREE_VIDEO_DOORBELL, MODEL_ESSENTIAL, MODEL_PRO_3_FLOODLIGHT, MODEL_PRO_4)
+            ):
+                return False
 
             # We have to be careful pinging some base stations because it can rapidly
             # drain the battery power. Don't ping if:
             # - it is a device that acts as its own base station
             # - it does not have a power supply or charger connected
             # - it is using WiFi directly rather than an Arlo base station
             if self.is_own_parent:
                 if not self.is_corded and not self.has_charger:
                     if self.using_wifi:
                         return False
 
-            # Don't ping these devices ever.
-            if self.model_id.startswith(
-                    (MODEL_WIREFREE_VIDEO_DOORBELL, MODEL_ESSENTIAL, MODEL_PRO_3_FLOODLIGHT, MODEL_PRO_4)
-            ):
-                return False
-
             # All others, then ping.
             return True
 
         if cap in (RESOURCE_CAPABILITY,):
             # Not all devices need (or want) to get their resources queried.
             if self.model_id.startswith(
                     (MODEL_WIREFREE_VIDEO_DOORBELL, MODEL_ESSENTIAL)
```

### Comparing `pyaarlo-0.8.0b7/pyaarlo/camera.py` & `pyaarlo-0.8.0b8/pyaarlo/camera.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b7/pyaarlo/cfg.py` & `pyaarlo-0.8.0b8/pyaarlo/cfg.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b7/pyaarlo/constant.py` & `pyaarlo-0.8.0b8/pyaarlo/constant.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b7/pyaarlo/device.py` & `pyaarlo-0.8.0b8/pyaarlo/device.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b7/pyaarlo/doorbell.py` & `pyaarlo-0.8.0b8/pyaarlo/doorbell.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b7/pyaarlo/light.py` & `pyaarlo-0.8.0b8/pyaarlo/light.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b7/pyaarlo/location.py` & `pyaarlo-0.8.0b8/pyaarlo/location.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b7/pyaarlo/main.py` & `pyaarlo-0.8.0b8/pyaarlo/main.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b7/pyaarlo/media.py` & `pyaarlo-0.8.0b8/pyaarlo/media.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b7/pyaarlo/ratls.py` & `pyaarlo-0.8.0b8/pyaarlo/ratls.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b7/pyaarlo/security_utils.py` & `pyaarlo-0.8.0b8/pyaarlo/security_utils.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b7/pyaarlo/sensor.py` & `pyaarlo-0.8.0b8/pyaarlo/sensor.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b7/pyaarlo/sseclient.py` & `pyaarlo-0.8.0b8/pyaarlo/sseclient.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b7/pyaarlo/storage.py` & `pyaarlo-0.8.0b8/pyaarlo/storage.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b7/pyaarlo/super.py` & `pyaarlo-0.8.0b8/pyaarlo/super.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b7/pyaarlo/tfa.py` & `pyaarlo-0.8.0b8/pyaarlo/tfa.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b7/pyaarlo/util.py` & `pyaarlo-0.8.0b8/pyaarlo/util.py`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b7/pyaarlo.egg-info/PKG-INFO` & `pyaarlo-0.8.0b8/pyaarlo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaarlo
-Version: 0.8.0b7
+Version: 0.8.0b8
 Summary: PyAarlo is a library that provides asynchronous access to Arlo security cameras.
 Home-page: https://github.com/twrecked/pyaarlo.git
 Author: Steve Herrell
 Author-email: steve.herrell@gmail.com
 License: LGPLv3+
 Project-URL: Bug Tracker, https://github.com/twrecked/pyaarlo/issues
 Project-URL: Documentation, https://github.com/twrecked/pyaarlo/blob/master/README.md
```

### Comparing `pyaarlo-0.8.0b7/pyaarlo.egg-info/SOURCES.txt` & `pyaarlo-0.8.0b8/pyaarlo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyaarlo-0.8.0b7/setup.py` & `pyaarlo-0.8.0b8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     with open('README.md') as desc:
         return desc.read()
 
 
 setup(
 
     name='pyaarlo',
-    version='0.8.0b7',
+    version='0.8.0b8',
     packages=['pyaarlo'],
 
     python_requires='>=3.6',
     install_requires=[
         'requests',
         'click',
         'pycryptodome',
```

