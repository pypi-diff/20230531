# Comparing `tmp/qlapi-0.1.5.tar.gz` & `tmp/qlapi-0.1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlapi-0.1.5.tar", last modified: Tue May 30 09:49:45 2023, max compression
+gzip compressed data, was "qlapi-0.1.5.1.tar", last modified: Wed May 31 04:58:18 2023, max compression
```

## Comparing `qlapi-0.1.5.tar` & `qlapi-0.1.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 09:49:45.135702 qlapi-0.1.5/
--rw-rw-rw-   0        0        0    35821 2023-05-16 09:18:13.000000 qlapi-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0      182 2023-05-30 09:49:45.134704 qlapi-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2677 2023-05-16 09:18:13.000000 qlapi-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 09:49:45.026632 qlapi-0.1.5/qlapi/
--rw-rw-rw-   0        0        0      123 2023-05-25 05:37:56.000000 qlapi-0.1.5/qlapi/__init__.py
--rw-rw-rw-   0        0        0     1382 2023-05-16 09:18:13.000000 qlapi-0.1.5/qlapi/base.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:49:45.045578 qlapi-0.1.5/qlapi/lib/
--rw-rw-rw-   0        0        0  1713152 2023-05-24 02:10:07.000000 qlapi-0.1.5/qlapi/lib/QLNRSdk.dll
--rw-rw-rw-   0        0        0     3218 2023-05-30 08:52:27.000000 qlapi-0.1.5/qlapi/nrsdk.py
--rw-rw-rw-   0        0        0     1997 2023-05-25 03:06:01.000000 qlapi-0.1.5/qlapi/paradigm.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:49:45.130715 qlapi-0.1.5/qlapi/recorder/
--rw-rw-rw-   0        0        0    18502 2023-05-16 09:18:13.000000 qlapi-0.1.5/qlapi/recorder/__init__.py
--rw-rw-rw-   0        0        0      200 2023-05-16 09:18:13.000000 qlapi-0.1.5/qlapi/rsa.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:49:45.132710 qlapi-0.1.5/qlapi/stimulator/
--rw-rw-rw-   0        0        0     3559 2023-05-30 08:54:51.000000 qlapi-0.1.5/qlapi/stimulator/__init__.py
--rw-rw-rw-   0        0        0     1976 2023-05-25 06:29:17.000000 qlapi-0.1.5/qlapi/stimulator/mcf_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-30 09:49:45.044581 qlapi-0.1.5/qlapi.egg-info/
--rw-rw-rw-   0        0        0      182 2023-05-30 09:49:44.000000 qlapi-0.1.5/qlapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-05-30 09:49:44.000000 qlapi-0.1.5/qlapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 09:49:44.000000 qlapi-0.1.5/qlapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-21 09:08:30.000000 qlapi-0.1.5/qlapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-05-30 09:49:44.000000 qlapi-0.1.5/qlapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 09:49:45.136700 qlapi-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      533 2023-05-30 09:46:19.000000 qlapi-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:58:18.123579 qlapi-0.1.5.1/
+-rw-rw-rw-   0        0        0    35821 2023-05-16 09:18:13.000000 qlapi-0.1.5.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      184 2023-05-31 04:58:18.123579 qlapi-0.1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2677 2023-05-16 09:18:13.000000 qlapi-0.1.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 04:58:17.980005 qlapi-0.1.5.1/qlapi/
+-rw-rw-rw-   0        0        0      123 2023-05-25 05:37:56.000000 qlapi-0.1.5.1/qlapi/__init__.py
+-rw-rw-rw-   0        0        0     1382 2023-05-16 09:18:13.000000 qlapi-0.1.5.1/qlapi/base.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:58:18.030096 qlapi-0.1.5.1/qlapi/lib/
+-rw-rw-rw-   0        0        0  1713152 2023-05-24 02:10:07.000000 qlapi-0.1.5.1/qlapi/lib/QLNRSdk.dll
+-rw-rw-rw-   0        0        0     3234 2023-05-31 03:23:01.000000 qlapi-0.1.5.1/qlapi/nrsdk.py
+-rw-rw-rw-   0        0        0     1997 2023-05-25 03:06:01.000000 qlapi-0.1.5.1/qlapi/paradigm.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:58:18.067153 qlapi-0.1.5.1/qlapi/recorder/
+-rw-rw-rw-   0        0        0    18502 2023-05-16 09:18:13.000000 qlapi-0.1.5.1/qlapi/recorder/__init__.py
+-rw-rw-rw-   0        0        0      200 2023-05-16 09:18:13.000000 qlapi-0.1.5.1/qlapi/rsa.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:58:18.122616 qlapi-0.1.5.1/qlapi/stimulator/
+-rw-rw-rw-   0        0        0     3559 2023-05-30 08:54:51.000000 qlapi-0.1.5.1/qlapi/stimulator/__init__.py
+-rw-rw-rw-   0        0        0     1976 2023-05-25 06:29:17.000000 qlapi-0.1.5.1/qlapi/stimulator/mcf_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-31 04:58:17.992400 qlapi-0.1.5.1/qlapi.egg-info/
+-rw-rw-rw-   0        0        0      184 2023-05-31 04:58:17.000000 qlapi-0.1.5.1/qlapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2023-05-31 04:58:17.000000 qlapi-0.1.5.1/qlapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 04:58:17.000000 qlapi-0.1.5.1/qlapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-21 09:08:30.000000 qlapi-0.1.5.1/qlapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-05-31 04:58:17.000000 qlapi-0.1.5.1/qlapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 04:58:18.124576 qlapi-0.1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      535 2023-05-31 04:57:52.000000 qlapi-0.1.5.1/setup.py
```

### Comparing `qlapi-0.1.5/LICENSE.txt` & `qlapi-0.1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qlapi-0.1.5/README.md` & `qlapi-0.1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `qlapi-0.1.5/qlapi/base.py` & `qlapi-0.1.5.1/qlapi/base.py`

 * *Files identical despite different names*

### Comparing `qlapi-0.1.5/qlapi/lib/QLNRSdk.dll` & `qlapi-0.1.5.1/qlapi/lib/QLNRSdk.dll`

 * *Files identical despite different names*

### Comparing `qlapi-0.1.5/qlapi/nrsdk.py` & `qlapi-0.1.5.1/qlapi/nrsdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,20 +49,21 @@
         self._assert_connected()
 
         # 字符串格式统一为dict
         if isinstance(param, str):
             param = json.loads(param)
 
         s = json.dumps(param, indent=4)
-        # print(s)
+        print(s)
 
         param_2 = c_char_p(s.encode('utf-8'))
         resp = (c_char * 512)(0)
         len = c_int(512)
         device_code = c_char_p(device.encode('utf-8')) if device else c_char_p(None)
+        res = -1
         try:
             res = _api.QLNR_StartStimulationEx(self.login_handle, param_2, resp, pointer(len), device_code)
             print("start stimulation {}".format(resp_result(res)))
         except Exception as e:
             print(e)
     
         return _SUCCESS if res == _RESP_SUCCESS else _FAIL
```

### Comparing `qlapi-0.1.5/qlapi/paradigm.py` & `qlapi-0.1.5.1/qlapi/paradigm.py`

 * *Files identical despite different names*

### Comparing `qlapi-0.1.5/qlapi/recorder/__init__.py` & `qlapi-0.1.5.1/qlapi/recorder/__init__.py`

 * *Files identical despite different names*

### Comparing `qlapi-0.1.5/qlapi/stimulator/__init__.py` & `qlapi-0.1.5.1/qlapi/stimulator/__init__.py`

 * *Files identical despite different names*

### Comparing `qlapi-0.1.5/qlapi/stimulator/mcf_reader.py` & `qlapi-0.1.5.1/qlapi/stimulator/mcf_reader.py`

 * *Files identical despite different names*

### Comparing `qlapi-0.1.5/setup.py` & `qlapi-0.1.5.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 from setuptools import find_packages
 
-VERSION = '0.1.5'
+VERSION = '0.1.5.1'
 AUTHOR='eegion'
 EMAIL='hehuajun@eegion.com'
 REQUIRED = [
     'mne',
 ]
 
 setup(
```

