# Comparing `tmp/aliyun-python-sdk-airticketopen-1.0.6.tar.gz` & `tmp/aliyun-python-sdk-airticketopen-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-airticketopen-1.0.6.tar", last modified: Thu May 18 09:19:56 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-airticketopen-1.0.7.tar", last modified: Wed May 31 12:52:27 2023, max compression
```

## Comparing `aliyun-python-sdk-airticketopen-1.0.6.tar` & `aliyun-python-sdk-airticketopen-1.0.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/
--rw-r--r--   0 root         (0) root         (0)      575 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1587 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      547 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyun_python_sdk_airticketopen.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1587 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyun_python_sdk_airticketopen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1860 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyun_python_sdk_airticketopen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyun_python_sdk_airticketopen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyun_python_sdk_airticketopen.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyun_python_sdk_airticketopen.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/
--rw-r--r--   0 root         (0) root         (0)     3578 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/AccountFlowListRequest.py
--rw-r--r--   0 root         (0) root         (0)     3018 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/AncillarySuggestRequest.py
--rw-r--r--   0 root         (0) root         (0)     3977 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/BookRequest.py
--rw-r--r--   0 root         (0) root         (0)     2977 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/CancelRequest.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/ChangeApplyRequest.py
--rw-r--r--   0 root         (0) root         (0)     3032 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/ChangeCancelRequest.py
--rw-r--r--   0 root         (0) root         (0)     3035 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/ChangeConfirmRequest.py
--rw-r--r--   0 root         (0) root         (0)     3649 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/ChangeDetailListOfBuyerRequest.py
--rw-r--r--   0 root         (0) root         (0)     3406 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/ChangeDetailListOfOrderNumRequest.py
--rw-r--r--   0 root         (0) root         (0)     3025 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/ChangeDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     3971 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/EnrichRequest.py
--rw-r--r--   0 root         (0) root         (0)     3192 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/FileUploadRequest.py
--rw-r--r--   0 root         (0) root         (0)     3005 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/FlightChangeOfOrderRequest.py
--rw-r--r--   0 root         (0) root         (0)     1406 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/GetTokenRequest.py
--rw-r--r--   0 root         (0) root         (0)     3195 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/OrderDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     3770 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/OrderListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2996 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/PricingRequest.py
--rw-r--r--   0 root         (0) root         (0)     3703 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/RefundApplyRequest.py
--rw-r--r--   0 root         (0) root         (0)     3906 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/RefundDetailListRequest.py
--rw-r--r--   0 root         (0) root         (0)     3025 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/RefundDetailRequest.py
--rw-r--r--   0 root         (0) root         (0)     3715 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/SearchRequest.py
--rw-r--r--   0 root         (0) root         (0)     2986 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/TicketingRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2502 2023-05-18 09:19:56.000000 aliyun-python-sdk-airticketopen-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:52:27.000000 aliyun-python-sdk-airticketopen-1.0.7/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1587 2023-05-31 12:52:27.000000 aliyun-python-sdk-airticketopen-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      547 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:52:27.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyun_python_sdk_airticketopen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1587 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyun_python_sdk_airticketopen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1860 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyun_python_sdk_airticketopen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyun_python_sdk_airticketopen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyun_python_sdk_airticketopen.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyun_python_sdk_airticketopen.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:52:27.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:52:27.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:52:27.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/
+-rw-r--r--   0 root         (0) root         (0)     3578 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/AccountFlowListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3018 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/AncillarySuggestRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3977 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/BookRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2977 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/CancelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/ChangeApplyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3032 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/ChangeCancelRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3035 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/ChangeConfirmRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3649 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/ChangeDetailListOfBuyerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3406 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/ChangeDetailListOfOrderNumRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3025 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/ChangeDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3971 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/EnrichRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3192 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/FileUploadRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/FlightChangeOfOrderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/GetTokenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3195 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/OrderDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3770 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/OrderListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/PricingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3703 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/RefundApplyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3906 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/RefundDetailListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3025 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/RefundDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/SearchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2986 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/TicketingRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-31 12:52:27.000000 aliyun-python-sdk-airticketopen-1.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-05-31 12:52:26.000000 aliyun-python-sdk-airticketopen-1.0.7/setup.py
```

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/LICENSE` & `aliyun-python-sdk-airticketopen-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/PKG-INFO` & `aliyun-python-sdk-airticketopen-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-airticketopen
-Version: 1.0.6
+Version: 1.0.7
 Summary: The airticketopen module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-airticketopen
```

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/README.rst` & `aliyun-python-sdk-airticketopen-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyun_python_sdk_airticketopen.egg-info/PKG-INFO` & `aliyun-python-sdk-airticketopen-1.0.7/aliyun_python_sdk_airticketopen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-airticketopen
-Version: 1.0.6
+Version: 1.0.7
 Summary: The airticketopen module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-airticketopen
```

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyun_python_sdk_airticketopen.egg-info/SOURCES.txt` & `aliyun-python-sdk-airticketopen-1.0.7/aliyun_python_sdk_airticketopen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/AccountFlowListRequest.py` & `aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/AccountFlowListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/AncillarySuggestRequest.py` & `aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/AncillarySuggestRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/BookRequest.py` & `aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/BookRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/CancelRequest.py` & `aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/CancelRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/ChangeApplyRequest.py` & `aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/ChangeApplyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/ChangeCancelRequest.py` & `aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/ChangeCancelRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/ChangeConfirmRequest.py` & `aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/ChangeConfirmRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/ChangeDetailListOfBuyerRequest.py` & `aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/ChangeDetailListOfBuyerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/ChangeDetailListOfOrderNumRequest.py` & `aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/ChangeDetailListOfOrderNumRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/ChangeDetailRequest.py` & `aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/ChangeDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/EnrichRequest.py` & `aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/EnrichRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/FileUploadRequest.py` & `aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/FileUploadRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/FlightChangeOfOrderRequest.py` & `aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/FlightChangeOfOrderRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/GetTokenRequest.py` & `aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/GetTokenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/OrderDetailRequest.py` & `aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/OrderDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/OrderListRequest.py` & `aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/OrderListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/PricingRequest.py` & `aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/PricingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/RefundApplyRequest.py` & `aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/RefundApplyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/RefundDetailListRequest.py` & `aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/RefundDetailListRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/RefundDetailRequest.py` & `aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/RefundDetailRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/SearchRequest.py` & `aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/SearchRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/aliyunsdkairticketopen/request/v20230117/TicketingRequest.py` & `aliyun-python-sdk-airticketopen-1.0.7/aliyunsdkairticketopen/request/v20230117/TicketingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-airticketopen-1.0.6/setup.py` & `aliyun-python-sdk-airticketopen-1.0.7/setup.py`

 * *Files identical despite different names*

