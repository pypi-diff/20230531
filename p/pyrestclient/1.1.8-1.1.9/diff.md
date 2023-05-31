# Comparing `tmp/pyrestclient-1.1.8.tar.gz` & `tmp/pyrestclient-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrestclient-1.1.8.tar", last modified: Tue Sep 13 16:57:35 2022, max compression
+gzip compressed data, was "pyrestclient-1.1.9.tar", last modified: Wed May 31 11:20:58 2023, max compression
```

## Comparing `pyrestclient-1.1.8.tar` & `pyrestclient-1.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-09-13 16:57:35.123765 pyrestclient-1.1.8/
--rw-rw-rw-   0        0        0     1095 2020-02-16 17:53:11.000000 pyrestclient-1.1.8/LICENSE
--rw-rw-rw-   0        0        0     4519 2022-09-13 16:57:35.122760 pyrestclient-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     3700 2022-09-13 16:56:19.000000 pyrestclient-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2022-09-13 16:57:35.109764 pyrestclient-1.1.8/pyrestclient/
--rw-rw-rw-   0        0        0    17782 2022-09-13 16:51:24.000000 pyrestclient-1.1.8/pyrestclient/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-13 16:57:35.120765 pyrestclient-1.1.8/pyrestclient.egg-info/
--rw-rw-rw-   0        0        0     4519 2022-09-13 16:57:35.000000 pyrestclient-1.1.8/pyrestclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2022-09-13 16:57:35.000000 pyrestclient-1.1.8/pyrestclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-13 16:57:35.000000 pyrestclient-1.1.8/pyrestclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2022-09-13 16:57:35.000000 pyrestclient-1.1.8/pyrestclient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-09-13 16:57:35.000000 pyrestclient-1.1.8/pyrestclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-13 16:57:35.123765 pyrestclient-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1320 2022-09-13 16:51:24.000000 pyrestclient-1.1.8/setup.py
+drwxr-xr-x   0 c-pher     (502) staff       (20)        0 2023-05-31 11:20:57.998537 pyrestclient-1.1.9/
+-rw-r--r--   0 c-pher     (502) staff       (20)     1074 2023-05-31 09:43:03.000000 pyrestclient-1.1.9/LICENSE
+-rw-r--r--   0 c-pher     (502) staff       (20)     4478 2023-05-31 11:20:57.998111 pyrestclient-1.1.9/PKG-INFO
+-rw-r--r--   0 c-pher     (502) staff       (20)     3681 2023-05-31 11:14:14.000000 pyrestclient-1.1.9/README.md
+drwxr-xr-x   0 c-pher     (502) staff       (20)        0 2023-05-31 11:20:57.995077 pyrestclient-1.1.9/pyrestclient/
+-rw-r--r--   0 c-pher     (502) staff       (20)    19619 2023-05-31 11:20:41.000000 pyrestclient-1.1.9/pyrestclient/__init__.py
+drwxr-xr-x   0 c-pher     (502) staff       (20)        0 2023-05-31 11:20:57.997517 pyrestclient-1.1.9/pyrestclient.egg-info/
+-rw-r--r--   0 c-pher     (502) staff       (20)     4478 2023-05-31 11:20:57.000000 pyrestclient-1.1.9/pyrestclient.egg-info/PKG-INFO
+-rw-r--r--   0 c-pher     (502) staff       (20)      230 2023-05-31 11:20:57.000000 pyrestclient-1.1.9/pyrestclient.egg-info/SOURCES.txt
+-rw-r--r--   0 c-pher     (502) staff       (20)        1 2023-05-31 11:20:57.000000 pyrestclient-1.1.9/pyrestclient.egg-info/dependency_links.txt
+-rw-r--r--   0 c-pher     (502) staff       (20)       40 2023-05-31 11:20:57.000000 pyrestclient-1.1.9/pyrestclient.egg-info/requires.txt
+-rw-r--r--   0 c-pher     (502) staff       (20)       13 2023-05-31 11:20:57.000000 pyrestclient-1.1.9/pyrestclient.egg-info/top_level.txt
+-rw-r--r--   0 c-pher     (502) staff       (20)       38 2023-05-31 11:20:57.998669 pyrestclient-1.1.9/setup.cfg
+-rw-r--r--   0 c-pher     (502) staff       (20)     1282 2023-05-31 11:05:35.000000 pyrestclient-1.1.9/setup.py
```

### Comparing `pyrestclient-1.1.8/PKG-INFO` & `pyrestclient-1.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,198 +1,204 @@
-Metadata-Version: 2.1
-Name: pyrestclient
-Version: 1.1.8
-Summary: The simple http client and REST test tool for humans.
-Home-page: https://github.com/c-pher/RESTClient.git
-Author: Andrey Komissarov
-Author-email: a.komisssarov@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: System Administrators
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: System :: Systems Administration
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![PyPI version](https://badge.fury.io/py/pyrestclient.svg)](https://badge.fury.io/py/pyrestclient)
-
-# RESTClient
-
-The cross-platform tool to work with http.
-
-## Installation
-
-For most users, the recommended method to install is via pip:
-
-```cmd
-pip install pyrestclient
-```
-
-or from source:
-
-```cmd
-python setup.py install
-```
-
-## Import
-
-```python
-from pyrestclient import RESTClient
-```
-
----
-
-## Changelog
-
-##### UNRELEASED
-
-##### 1.1.8 (13.09.2022)
-
-Read timeout adjustment added. From now on you can set read and connection timeout simultaneously
-
-- "auth_timeout" renamed to "connect_timeout" and value reduced to 5
-- "read_timeout" global param added. Default value - 60.
-- logger_enabled renamed to log_enabled
-- logger_level renamed to log_level
-- minor refactoring
-
-##### 1.1.7.post0 (8.07.2022)
-
-- logger error fixed
-- log level handler added
-
-##### 1.1.7 (8.07.2022)
-
-- typo fixed
-- requested_url() refactored
-- encode_to_base64 logger added
-- "[Response]" replaces with the "<-"
-
-##### 1.1.6 (3.06.2022)
-
-- logger name is now `RESTClient`
-
-##### 1.1.5 (24.05.2022)
-
-Breaking changes:
-REST assertion renamed and changed:
-
-- return bool now
-- is_success()
-- is_ok()
-- is_not_found()
-- is_bad_request()
-- is_unauthorized() new method
-
-##### 1.1.4 (23.05.2022)
-
-- response logger added
-- json_data() removed
-
-##### 1.1.3 (17.04.2022)
-
-- updated to manage logger state
-
-##### 1.1.2 (29.03.2022)
-
-- 'host' attr is '127.0.0.1' by default
-- 'auth_timeout=7': new attr added
-- '.encode_to_base64()': new method added
-- plogger package added as dependency
-- internal logger removed as unused
-
-##### 1.1.1 (15.02.2022)
-
-wait_service_start fixed. added interval parameter
-
-##### 1.1.0 (8.02.2022)
-
-- Fixed custom header usage
-
-##### 1.0.9.post0 (29.12.2021)
-
-Fixed get token logger
-
-##### 1.0.9 (06.12.2021)
-
-- token property changed to catch unavailability occasions (not verifying base URL availability)
-
-##### 1.0.8.post0 (31.08.2021)
-
-- post without data fixed
-- refactored custom header
-
-##### 1.0.8 (31.08.2021)
-
-- logger added as attr
-
-##### 1.0.7 (21.05.2021)
-
-- POST, PUT, DELETE extended with header=None param
-
-##### 1.0.6 (24.02.2021)
-
-- refactoring. used lazy initialization to get token
-- wait_service_start: for the is_service_initialized under the hood used 0.1 sec by default
-
-##### 1.0.5 (24.02.2021)
-
-is_service_initialized updated to use timeout
-
-##### 1.0.4 (21.12.2020)
-
-logger auth link fixed
-
-##### 1.0.3 (21.12.2020)
-
-header param added to the GET method
-
-##### 1.0.2 (31.10.2020)
-
-New base method added:
-
-- is_host_available (Check remote host availability using socket and specified port)
-- is_service_initialized (GET https://{IP}:{PORT})
-- wait_service_start
-
-##### 1.0.1 (29.10.2020)
-
-- PUT fixed
-- RESTClient inherited from RESTAssertion. No need to import RESTAssertion directly
-
-#####1.0.0 (14.10.2020)
-- removed "extend_header"
-
-#####0.1.0 (21.05.2020)
-- file logging removed
-
-#####0.0.9 (28.03.2020)
-DELETE fixed
-POST: added file support
-
-#####0.0.8 (28.03.2020)
-header typing hint fixed. Now it is dict
-
-#####0.0.7 (10.03.2020)
-- Added query_params to all methods
-- POST method was refactored to use .send_request()
-
-#####0.0.6 (01.03.2020)
-- removed full_url param. now it will automatically convert url. use "http[s]://site.com" format in methods to use full url.
-- code refactoring
-
-#####0.0.5 (01.03.2020)
-- query params refactored to use urlencode
-- added DELETE method
-
-##### 0.0.4 (27.02.2020)
-should_be_bad_request: assert text fixed
-...
-
-##### 0.0.1 (9.02.2020)
-- initial commit
+Metadata-Version: 2.1
+Name: pyrestclient
+Version: 1.1.9
+Summary: The simple http client and REST test tool for humans.
+Home-page: https://github.com/c-pher/RESTClient.git
+Author: Andrey Komissarov
+Author-email: a.komisssarov@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: System Administrators
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: System :: Systems Administration
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI version](https://badge.fury.io/py/pyrestclient.svg)](https://badge.fury.io/py/pyrestclient)
+
+# RESTClient
+
+The cross-platform tool to work with http.
+
+## Installation
+
+For most users, the recommended method to install is via pip:
+
+```cmd
+pip install pyrestclient
+```
+
+or from source:
+
+```cmd
+python setup.py install
+```
+
+## Import
+
+```python
+from pyrestclient import RESTClient
+```
+
+---
+
+## Changelog
+
+##### UNRELEASED
+
+##### 1.1.9 (31.05.2023)
+
+- auth_key attr added to customize auth response
+- AuthToken removed. all it methods moved inside core class
+- debug log extended
+
+##### 1.1.8 (13.09.2022)
+
+Read timeout adjustment added. From now on you can set read and connection timeout simultaneously
+
+- "auth_timeout" renamed to "connect_timeout" and value reduced to 5
+- "read_timeout" global param added. Default value - 60.
+- logger_enabled renamed to log_enabled
+- logger_level renamed to log_level
+- minor refactoring
+
+##### 1.1.7.post0 (8.07.2022)
+
+- logger error fixed
+- log level handler added
+
+##### 1.1.7 (8.07.2022)
+
+- typo fixed
+- requested_url() refactored
+- encode_to_base64 logger added
+- "[Response]" replaces with the "<-"
+
+##### 1.1.6 (3.06.2022)
+
+- logger name is now `RESTClient`
+
+##### 1.1.5 (24.05.2022)
+
+Breaking changes:
+REST assertion renamed and changed:
+
+- return bool now
+- is_success()
+- is_ok()
+- is_not_found()
+- is_bad_request()
+- is_unauthorized() new method
+
+##### 1.1.4 (23.05.2022)
+
+- response logger added
+- json_data() removed
+
+##### 1.1.3 (17.04.2022)
+
+- updated to manage logger state
+
+##### 1.1.2 (29.03.2022)
+
+- 'host' attr is '127.0.0.1' by default
+- 'auth_timeout=7': new attr added
+- '.encode_to_base64()': new method added
+- plogger package added as dependency
+- internal logger removed as unused
+
+##### 1.1.1 (15.02.2022)
+
+wait_service_start fixed. added interval parameter
+
+##### 1.1.0 (8.02.2022)
+
+- Fixed custom header usage
+
+##### 1.0.9.post0 (29.12.2021)
+
+Fixed get token logger
+
+##### 1.0.9 (06.12.2021)
+
+- token property changed to catch unavailability occasions (not verifying base URL availability)
+
+##### 1.0.8.post0 (31.08.2021)
+
+- post without data fixed
+- refactored custom header
+
+##### 1.0.8 (31.08.2021)
+
+- logger added as attr
+
+##### 1.0.7 (21.05.2021)
+
+- POST, PUT, DELETE extended with header=None param
+
+##### 1.0.6 (24.02.2021)
+
+- refactoring. used lazy initialization to get token
+- wait_service_start: for the is_service_initialized under the hood used 0.1 sec by default
+
+##### 1.0.5 (24.02.2021)
+
+is_service_initialized updated to use timeout
+
+##### 1.0.4 (21.12.2020)
+
+logger auth link fixed
+
+##### 1.0.3 (21.12.2020)
+
+header param added to the GET method
+
+##### 1.0.2 (31.10.2020)
+
+New base method added:
+
+- is_host_available (Check remote host availability using socket and specified port)
+- is_service_initialized (GET https://{IP}:{PORT})
+- wait_service_start
+
+##### 1.0.1 (29.10.2020)
+
+- PUT fixed
+- RESTClient inherited from RESTAssertion. No need to import RESTAssertion directly
+
+#####1.0.0 (14.10.2020)
+- removed "extend_header"
+
+#####0.1.0 (21.05.2020)
+- file logging removed
+
+#####0.0.9 (28.03.2020)
+DELETE fixed
+POST: added file support
+
+#####0.0.8 (28.03.2020)
+header typing hint fixed. Now it is dict
+
+#####0.0.7 (10.03.2020)
+- Added query_params to all methods
+- POST method was refactored to use .send_request()
+
+#####0.0.6 (01.03.2020)
+- removed full_url param. now it will automatically convert url. use "http[s]://site.com" format in methods to use full url.
+- code refactoring
+
+#####0.0.5 (01.03.2020)
+- query params refactored to use urlencode
+- added DELETE method
+
+##### 0.0.4 (27.02.2020)
+should_be_bad_request: assert text fixed
+...
+
+##### 0.0.1 (9.02.2020)
+- initial commit
```

### Comparing `pyrestclient-1.1.8/README.md` & `pyrestclient-1.1.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,177 +1,183 @@
-[![PyPI version](https://badge.fury.io/py/pyrestclient.svg)](https://badge.fury.io/py/pyrestclient)
-
-# RESTClient
-
-The cross-platform tool to work with http.
-
-## Installation
-
-For most users, the recommended method to install is via pip:
-
-```cmd
-pip install pyrestclient
-```
-
-or from source:
-
-```cmd
-python setup.py install
-```
-
-## Import
-
-```python
-from pyrestclient import RESTClient
-```
-
----
-
-## Changelog
-
-##### UNRELEASED
-
-##### 1.1.8 (13.09.2022)
-
-Read timeout adjustment added. From now on you can set read and connection timeout simultaneously
-
-- "auth_timeout" renamed to "connect_timeout" and value reduced to 5
-- "read_timeout" global param added. Default value - 60.
-- logger_enabled renamed to log_enabled
-- logger_level renamed to log_level
-- minor refactoring
-
-##### 1.1.7.post0 (8.07.2022)
-
-- logger error fixed
-- log level handler added
-
-##### 1.1.7 (8.07.2022)
-
-- typo fixed
-- requested_url() refactored
-- encode_to_base64 logger added
-- "[Response]" replaces with the "<-"
-
-##### 1.1.6 (3.06.2022)
-
-- logger name is now `RESTClient`
-
-##### 1.1.5 (24.05.2022)
-
-Breaking changes:
-REST assertion renamed and changed:
-
-- return bool now
-- is_success()
-- is_ok()
-- is_not_found()
-- is_bad_request()
-- is_unauthorized() new method
-
-##### 1.1.4 (23.05.2022)
-
-- response logger added
-- json_data() removed
-
-##### 1.1.3 (17.04.2022)
-
-- updated to manage logger state
-
-##### 1.1.2 (29.03.2022)
-
-- 'host' attr is '127.0.0.1' by default
-- 'auth_timeout=7': new attr added
-- '.encode_to_base64()': new method added
-- plogger package added as dependency
-- internal logger removed as unused
-
-##### 1.1.1 (15.02.2022)
-
-wait_service_start fixed. added interval parameter
-
-##### 1.1.0 (8.02.2022)
-
-- Fixed custom header usage
-
-##### 1.0.9.post0 (29.12.2021)
-
-Fixed get token logger
-
-##### 1.0.9 (06.12.2021)
-
-- token property changed to catch unavailability occasions (not verifying base URL availability)
-
-##### 1.0.8.post0 (31.08.2021)
-
-- post without data fixed
-- refactored custom header
-
-##### 1.0.8 (31.08.2021)
-
-- logger added as attr
-
-##### 1.0.7 (21.05.2021)
-
-- POST, PUT, DELETE extended with header=None param
-
-##### 1.0.6 (24.02.2021)
-
-- refactoring. used lazy initialization to get token
-- wait_service_start: for the is_service_initialized under the hood used 0.1 sec by default
-
-##### 1.0.5 (24.02.2021)
-
-is_service_initialized updated to use timeout
-
-##### 1.0.4 (21.12.2020)
-
-logger auth link fixed
-
-##### 1.0.3 (21.12.2020)
-
-header param added to the GET method
-
-##### 1.0.2 (31.10.2020)
-
-New base method added:
-
-- is_host_available (Check remote host availability using socket and specified port)
-- is_service_initialized (GET https://{IP}:{PORT})
-- wait_service_start
-
-##### 1.0.1 (29.10.2020)
-
-- PUT fixed
-- RESTClient inherited from RESTAssertion. No need to import RESTAssertion directly
-
-#####1.0.0 (14.10.2020)
-- removed "extend_header"
-
-#####0.1.0 (21.05.2020)
-- file logging removed
-
-#####0.0.9 (28.03.2020)
-DELETE fixed
-POST: added file support
-
-#####0.0.8 (28.03.2020)
-header typing hint fixed. Now it is dict
-
-#####0.0.7 (10.03.2020)
-- Added query_params to all methods
-- POST method was refactored to use .send_request()
-
-#####0.0.6 (01.03.2020)
-- removed full_url param. now it will automatically convert url. use "http[s]://site.com" format in methods to use full url.
-- code refactoring
-
-#####0.0.5 (01.03.2020)
-- query params refactored to use urlencode
-- added DELETE method
-
-##### 0.0.4 (27.02.2020)
-should_be_bad_request: assert text fixed
-...
-
-##### 0.0.1 (9.02.2020)
+[![PyPI version](https://badge.fury.io/py/pyrestclient.svg)](https://badge.fury.io/py/pyrestclient)
+
+# RESTClient
+
+The cross-platform tool to work with http.
+
+## Installation
+
+For most users, the recommended method to install is via pip:
+
+```cmd
+pip install pyrestclient
+```
+
+or from source:
+
+```cmd
+python setup.py install
+```
+
+## Import
+
+```python
+from pyrestclient import RESTClient
+```
+
+---
+
+## Changelog
+
+##### UNRELEASED
+
+##### 1.1.9 (31.05.2023)
+
+- auth_key attr added to customize auth response
+- AuthToken removed. all it methods moved inside core class
+- debug log extended
+
+##### 1.1.8 (13.09.2022)
+
+Read timeout adjustment added. From now on you can set read and connection timeout simultaneously
+
+- "auth_timeout" renamed to "connect_timeout" and value reduced to 5
+- "read_timeout" global param added. Default value - 60.
+- logger_enabled renamed to log_enabled
+- logger_level renamed to log_level
+- minor refactoring
+
+##### 1.1.7.post0 (8.07.2022)
+
+- logger error fixed
+- log level handler added
+
+##### 1.1.7 (8.07.2022)
+
+- typo fixed
+- requested_url() refactored
+- encode_to_base64 logger added
+- "[Response]" replaces with the "<-"
+
+##### 1.1.6 (3.06.2022)
+
+- logger name is now `RESTClient`
+
+##### 1.1.5 (24.05.2022)
+
+Breaking changes:
+REST assertion renamed and changed:
+
+- return bool now
+- is_success()
+- is_ok()
+- is_not_found()
+- is_bad_request()
+- is_unauthorized() new method
+
+##### 1.1.4 (23.05.2022)
+
+- response logger added
+- json_data() removed
+
+##### 1.1.3 (17.04.2022)
+
+- updated to manage logger state
+
+##### 1.1.2 (29.03.2022)
+
+- 'host' attr is '127.0.0.1' by default
+- 'auth_timeout=7': new attr added
+- '.encode_to_base64()': new method added
+- plogger package added as dependency
+- internal logger removed as unused
+
+##### 1.1.1 (15.02.2022)
+
+wait_service_start fixed. added interval parameter
+
+##### 1.1.0 (8.02.2022)
+
+- Fixed custom header usage
+
+##### 1.0.9.post0 (29.12.2021)
+
+Fixed get token logger
+
+##### 1.0.9 (06.12.2021)
+
+- token property changed to catch unavailability occasions (not verifying base URL availability)
+
+##### 1.0.8.post0 (31.08.2021)
+
+- post without data fixed
+- refactored custom header
+
+##### 1.0.8 (31.08.2021)
+
+- logger added as attr
+
+##### 1.0.7 (21.05.2021)
+
+- POST, PUT, DELETE extended with header=None param
+
+##### 1.0.6 (24.02.2021)
+
+- refactoring. used lazy initialization to get token
+- wait_service_start: for the is_service_initialized under the hood used 0.1 sec by default
+
+##### 1.0.5 (24.02.2021)
+
+is_service_initialized updated to use timeout
+
+##### 1.0.4 (21.12.2020)
+
+logger auth link fixed
+
+##### 1.0.3 (21.12.2020)
+
+header param added to the GET method
+
+##### 1.0.2 (31.10.2020)
+
+New base method added:
+
+- is_host_available (Check remote host availability using socket and specified port)
+- is_service_initialized (GET https://{IP}:{PORT})
+- wait_service_start
+
+##### 1.0.1 (29.10.2020)
+
+- PUT fixed
+- RESTClient inherited from RESTAssertion. No need to import RESTAssertion directly
+
+#####1.0.0 (14.10.2020)
+- removed "extend_header"
+
+#####0.1.0 (21.05.2020)
+- file logging removed
+
+#####0.0.9 (28.03.2020)
+DELETE fixed
+POST: added file support
+
+#####0.0.8 (28.03.2020)
+header typing hint fixed. Now it is dict
+
+#####0.0.7 (10.03.2020)
+- Added query_params to all methods
+- POST method was refactored to use .send_request()
+
+#####0.0.6 (01.03.2020)
+- removed full_url param. now it will automatically convert url. use "http[s]://site.com" format in methods to use full url.
+- code refactoring
+
+#####0.0.5 (01.03.2020)
+- query params refactored to use urlencode
+- added DELETE method
+
+##### 0.0.4 (27.02.2020)
+should_be_bad_request: assert text fixed
+...
+
+##### 0.0.1 (9.02.2020)
 - initial commit
```

### Comparing `pyrestclient-1.1.8/pyrestclient/__init__.py` & `pyrestclient-1.1.9/pyrestclient/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,493 +1,567 @@
-import base64
-import json
-import re
-import socket
-import time
-from http import HTTPStatus
-from typing import Union
-from urllib.parse import urljoin, urlencode
-
-import requests
-from plogger import logger
-from urllib3 import disable_warnings, exceptions
-
-disable_warnings(exceptions.InsecureRequestWarning)
-
-
-def get_header_default(user_agent='ide', content_type='application/json-patch+json', accept='application/json'):
-    return {
-        'User-Agent': user_agent,
-        'Content-Type': content_type,
-        'Accept': accept,
-        # 'UserAgentInternal': 'webfrontend/1.0'
-    }
-
-
-class RESTAssertion:
-    """Parse requests response to get status code."""
-
-    @staticmethod
-    def is_success(response) -> bool:
-        """200 <= status_code < 400"""
-        return response.ok
-
-    @staticmethod
-    def is_ok(response) -> bool:
-        """OK, 200. Request fulfilled, document follows"""
-        return response.status_code == HTTPStatus.OK
-
-    @staticmethod
-    def is_not_found(response) -> bool:
-        """Nothing matches the given URI. 404"""
-
-        return response.status_code == HTTPStatus.NOT_FOUND
-
-    @staticmethod
-    def is_bad_request(response) -> bool:
-        """Bad request syntax or unsupported method. 400"""
-        return response.status_code == HTTPStatus.BAD_REQUEST
-
-    @staticmethod
-    def is_unauthorized(response) -> bool:
-        """Bad request syntax or unsupported method. 401"""
-        return response.status_code == HTTPStatus.UNAUTHORIZED
-
-
-# noinspection PyPep8Naming
-class RESTClient(RESTAssertion):
-    """ Main class for RestAPI """
-
-    def __init__(self,
-                 protocol: str = 'https',
-                 host: str = None,
-                 port: int = 0,
-                 username: str = None,
-                 password: str = None,
-                 header: dict = None,
-                 auth_basic: bool = False,
-                 auth_uri: str = '',
-                 auth_payload: dict = None,
-                 connect_timeout: int = 5,
-                 read_timeout: int = 60,
-                 log_enabled: bool = True,
-                 log_level: str = 'INFO'):
-
-        # Enable/disable logger
-        self.logger = logger('RESTClient', enabled=log_enabled, level=log_level)
-
-        # Credentials and settings for api url
-        self.username = username
-        self.password = password
-        self.protocol = protocol  # HTTP or HTTPS
-        self.host = host if host is not None else '127.0.0.1'
-        self.port = port
-        self.auth_uri = auth_uri
-        self.auth_payload = auth_payload
-        self.auth_basic = auth_basic
-        self.connect_timeout = connect_timeout
-        self.read_timeout = read_timeout
-        self.header = header or get_header_default()  # Default header
-
-    def __str__(self):
-        msg_print = (f'Username: {self.username}\n'
-                     f'Password: {self.password}\n'
-                     f'Base URL: {self.base_url}\n')
-
-        return msg_print
-
-    @property
-    def base_url(self):
-        """Create tested URL. Add port if it provided"""
-
-        base_url = f'{self.protocol}://{self.host}:{self.port}' if self.port else f'{self.protocol}://{self.host}'
-
-        return base_url
-
-    def requested_url(self, url) -> str:
-        """Return full URL if link specified starts with <http>"""
-
-        try:
-            requested_url = url if url.startswith('http') else urljoin(self.base_url, url)
-        except Exception as err:
-            self.logger.exception(f'URL does not specified. Used: "{url}" only. Specify full URL or use constructor')
-            raise err
-
-        return requested_url
-
-    @staticmethod
-    def _validate_url(url):
-        return re.match(r'https?://[\w/.]+', url)
-
-    def encode_to_base64(self, string: str) -> str:
-        """Encode string to base64. Do not use it during creating class instance (logger won't work)
-
-        Args:
-            string: Some text to encode.
-
-        Returns:
-            Base64 encoded string.
-        """
-
-        try:
-            str_text = string.encode()
-            base64_encoded = base64.b64encode(str_text)
-        except AttributeError as err:
-            self.logger.error(f'Cannot encode specific data ({string}, {type(string)})')
-            raise err
-
-        result = base64_encoded.decode()
-        return result
-
-    def get_token(self) -> str:
-        """Get auth (Bearer) token"""
-
-        return AuthToken(self).token
-
-    def get_auth_header(self, header: dict = None) -> dict:
-        """Get auth header with a token
-
-        :param header: custom header is needed
-        :return:
-        """
-
-        try:
-            self.header = header.copy()
-        except AttributeError:
-            self.header = get_header_default()
-
-        try:
-            # noinspection PyAttributeOutsideInit
-            self.token = self.get_token()
-            self.header['Authorization'] = self.token
-            return self.header
-        except KeyError as err:
-            self.logger.error(f'Cannot get token. {err}')
-
-    def _auth_basic(self):
-        """Enable basic auth if provided"""
-
-        self.header = {}
-        return self.username, self.password
-
-    def send_request(self,
-                     method: str,
-                     url: str,
-                     data: dict = None,
-                     files=None,
-                     query_params: dict = None,
-                     verify: bool = False,
-                     custom_header: dict = None,
-                     cookies=None,
-                     read_timeout: int = None):
-        """Send common REST request
-
-        To upload file use:
-
-        with open(files, 'rb') as f:
-             files = {'licenseFile': (License.name, f)}
-
-        Args:
-            method: GET, POST, DELETE
-            url: unified identifier, self.url (BASE) + url
-            data: json data
-            files: "files: {'licenseFile': (License.name, f)}"
-            query_params: Query parameters in the url
-            cookies:
-            verify: Ignore SSL verification?
-            custom_header: Use specified header
-            read_timeout: Read timeout in sec.
-
-        Returns:
-            requests.request('POST', url=url, headers=HEADER, files=files, verify=False)
-        """
-
-        # Get timeouts
-        read_timeout_ = self.read_timeout if read_timeout is None else read_timeout
-        common_timeout = self.read_timeout, read_timeout_
-
-        # Set auth method
-        if self.auth_payload is not None:
-            self.header = self.get_auth_header(header=custom_header)
-        elif self.auth_basic:
-            self.auth_basic = self._auth_basic()
-
-        if custom_header:
-            self.header = custom_header
-
-        # Make full url to use in request
-        link = self.requested_url(url)
-
-        # Add params to requested link
-        if query_params:
-            link += '?' + urlencode(query_params)
-
-        method = method.upper()
-        methods_available = 'GET', 'HEAD', 'DELETE', 'POST', 'PUT', 'PATCH', 'OPTIONS'
-        assert method in methods_available, 'Specified methods is not compatible.'
-
-        if data and files:
-            self.logger.error('Data parameter cannot be used with files parameter simultaneously.')
-            raise ValueError('Data parameter cannot be used with files parameter simultaneously.')
-
-        # Extend header
-        if 'Content-Type' not in self.header:
-            self.header['Content-Type'] = 'application/json'
-
-        response = 'Invalid requests. Check parameters'
-
-        self.logger.info(f'[{method}] {link}')
-
-        try:
-            # For 'POST', 'PUT', 'PATCH', 'OPTIONS', 'DELETE'
-            if method in ['POST', 'PUT', 'PATCH', 'OPTIONS', 'DELETE']:
-                if data and not files:
-
-                    self.logger.debug(f'{self.header = }, {cookies = }, {common_timeout = }')
-                    self.logger.info('PAYLOAD:\n' + json.dumps(data, indent=4))
-
-                    response = requests.request(method=method,
-                                                url=link,
-                                                auth=self.auth_basic,
-                                                headers=self.header,
-                                                json=data,
-                                                cookies=cookies,
-                                                verify=verify,
-                                                timeout=common_timeout)
-
-                elif files:
-                    files_header = self.header.copy()
-                    del files_header['Content-Type']
-
-                    self.logger.debug(f'{files_header = }, {cookies = }, {common_timeout = }')
-                    self.logger.info('PAYLOAD:\n' + json.dumps(data, indent=4))
-
-                    response = requests.request(method=method,
-                                                url=link,
-                                                auth=self.auth_basic,
-                                                headers=files_header,
-                                                cookies=cookies,
-                                                files=files,
-                                                verify=verify,
-                                                timeout=common_timeout)
-
-                elif not files and not data:
-                    self.logger.debug(f'{self.header = }, {cookies = }, {common_timeout = }')
-
-                    response = requests.request(method=method,
-                                                url=link,
-                                                auth=self.auth_basic,
-                                                headers=self.header,
-                                                cookies=cookies,
-                                                verify=verify,
-                                                timeout=common_timeout)
-
-            # For 'GET', 'HEAD' request
-            else:
-                # For usual 'GET' without query params
-                self.logger.debug(f'{self.header = }, {cookies = }, {common_timeout = }')
-
-                response = requests.request(method=method,
-                                            url=link,
-                                            auth=self.auth_basic,
-                                            cookies=cookies,
-                                            headers=self.header,
-                                            verify=verify,
-                                            timeout=common_timeout)
-        except requests.exceptions.ReadTimeout as err:
-            self.logger.exception(f'The request took too long. Read timed out. (read timeout={common_timeout[1]})')
-            raise err
-        except BaseException as err:
-            self.logger.exception('Something went wrong.')
-            raise err
-
-        self.logger.info(f'<- {response.status_code}: "{response.text}"')
-
-        return response
-
-    @property
-    def is_service_available(self):
-        """Check base url availability within 10 sec."""
-
-        try:
-            response = requests.get(self.base_url, timeout=10, verify=False)
-            if response.status_code == 200:
-                return True
-            return False
-        except requests.exceptions.Timeout:
-            return False
-        except requests.exceptions.ConnectionError:
-            return False
-
-    def download(self, url: str, dst: str):
-        """Download file.
-
-        :param url: Full url to file
-        :param dst: path to store
-        :return:
-        """
-
-        response = self.GET(url)
-        try:
-            if response.ok:
-                with open(dst, 'wb') as f:
-                    f.write(response.content)
-                    return True
-            else:
-                return False
-        except (ConnectionError, ConnectionRefusedError) as err:
-            self.logger.exception('Download failed')
-            return err
-
-    # noinspection PyPep8Naming
-    def GET(self,
-            url: str = '',
-            query_params: dict = None,
-            cookies=None,
-            read_timeout: int = None,
-            header: dict = None):
-
-        return self.send_request(method='GET',
-                                 url=url,
-                                 query_params=query_params,
-                                 cookies=cookies,
-                                 read_timeout=read_timeout,
-                                 custom_header=header)
-
-    # noinspection PyPep8Naming
-    def POST(self,
-             url: str = '',
-             data: dict = None,
-             file=None,
-             query_params: dict = None,
-             cookies=None,
-             read_timeout: int = None,
-             header: dict = None):
-
-        return self.send_request(method='POST',
-                                 url=url,
-                                 query_params=query_params,
-                                 data=data,
-                                 files=file,
-                                 cookies=cookies,
-                                 read_timeout=read_timeout,
-                                 custom_header=header)
-
-    # noinspection PyPep8Naming
-    def PUT(self,
-            url: str = '',
-            data: dict = '',
-            files='',
-            query_params: dict = None,
-            cookies=None,
-            read_timeout: int = None,
-            header: dict = None):
-
-        header_original = self.header.copy()
-
-        if files:  # FIXME
-            del header_original['Content-Type']
-
-        return self.send_request(method='PUT',
-                                 url=url,
-                                 data=data,
-                                 files=files,
-                                 query_params=query_params,
-                                 cookies=cookies,
-                                 read_timeout=read_timeout,
-                                 custom_header=header)
-
-    def DELETE(self,
-               url: str = '',
-               data: dict = '',
-               query_params: dict = None,
-               cookies=None,
-               read_timeout: int = None,
-               header: dict = None):
-
-        return self.send_request(method='DELETE',
-                                 url=url,
-                                 query_params=query_params,
-                                 data=data,
-                                 cookies=cookies,
-                                 read_timeout=read_timeout,
-                                 custom_header=header)
-
-    def is_host_available(self, port: int = 0, timeout: int = 5) -> bool:
-        """Check remote host availability using socket and specified port"""
-
-        port_ = port or self.port
-        with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
-            sock.settimeout(timeout)
-            result = sock.connect_ex((self.host, port_))
-            return False if result else True
-
-    def is_service_initialized(self, timeout: Union[int, float] = 20) -> bool:
-        """Send GET to base URL https://{IP}:{PORT}
-
-        :param timeout:
-        :return:
-        """
-
-        try:
-            response = requests.get(self.base_url, verify=False, timeout=timeout)
-            return response.ok
-        except requests.exceptions.ConnectionError:
-            return False
-
-    def wait_service_start(self, timeout: int = 30, interval: int = 3) -> bool:
-        """Waiting for the service start.
-
-        :param timeout: in sec.
-        :param interval: in sec.
-        :return:
-        """
-
-        timer = 0
-        status = self.is_service_initialized(1)
-
-        while not status:
-            status = self.is_service_initialized(1)
-            timer += interval
-
-            if timer > timeout - 2:
-                raise TimeoutError(f'The service was not started within {timeout} seconds.')
-            time.sleep(interval)
-        return status
-
-
-class AuthToken:
-    """Class to get auth token"""
-
-    def __init__(self, client: RESTClient):
-        self.client = client
-
-    @property
-    def auth_url(self):
-        """Get full authorization URL"""
-        return urljoin(self.client.base_url, self.client.auth_uri)
-
-    @property
-    def token(self):
-        """Get token"""
-
-        response_json = None
-
-        try:
-            payload = self.client.auth_payload
-            timeout = (self.client.connect_timeout, self.client.read_timeout)
-            response = requests.post(self.auth_url, json=payload, verify=False, timeout=timeout)
-            response_json = response.json()
-            return response_json['token']
-        except KeyError as err:
-            self.client.logger.exception(f'Cannot get key (token) from json data. {response_json}')
-            raise err
-        except json.decoder.JSONDecodeError as err:
-            msg = f'Cannot get token property. URL: {self.auth_url} ({self.client.auth_payload})'
-            self.client.logger.exception(msg)
-            raise err
-        except TypeError as err:
-            self.client.logger.exception('Endpoint is available but "token" key cannot be retrieved.')
-            raise err
-        except requests.exceptions.ConnectTimeout as err:
-            self.client.logger.exception(f'Perhaps, URI ({self.auth_url}) or service is unreachable.')
-            raise err
+import base64
+import ipaddress
+import json
+import re
+import socket
+import time
+from datetime import datetime, date
+from http import HTTPStatus
+from json import JSONDecodeError
+from typing import Union
+from urllib.parse import urljoin, urlencode
+
+import requests
+from plogger import logger
+from urllib3 import disable_warnings, exceptions
+
+disable_warnings(exceptions.InsecureRequestWarning)
+
+
+class RESTAssertion:
+    """Parse requests response to get status code."""
+
+    @staticmethod
+    def is_success(response) -> bool:
+        """200 <= status_code < 400"""
+        return response.ok
+
+    @staticmethod
+    def is_ok(response) -> bool:
+        """OK, 200. Request fulfilled, document follows"""
+        return response.status_code == HTTPStatus.OK
+
+    @staticmethod
+    def is_not_found(response) -> bool:
+        """Nothing matches the given URI. 404"""
+
+        return response.status_code == HTTPStatus.NOT_FOUND
+
+    @staticmethod
+    def is_bad_request(response) -> bool:
+        """Bad request syntax or unsupported method. 400"""
+        return response.status_code == HTTPStatus.BAD_REQUEST
+
+    @staticmethod
+    def is_unauthorized(response) -> bool:
+        """Bad request syntax or unsupported method. 401"""
+        return response.status_code == HTTPStatus.UNAUTHORIZED
+
+
+# noinspection PyPep8Naming
+class RESTClient(RESTAssertion):
+    """ Main class for RestAPI """
+
+    def __init__(self,
+                 protocol: str = 'https',
+                 host: str = None,
+                 port: int = 0,
+                 username: str = None,
+                 password: str = None,
+                 header: dict = None,
+                 auth_basic: bool = False,
+                 auth_uri: str = '',
+                 auth_key: str = 'token',
+                 auth_payload: dict = None,
+                 connect_timeout: int = 5,
+                 read_timeout: int = 60,
+                 log_enabled: bool = True,
+                 log_level: str = 'INFO'):
+
+        # Enable/disable logger
+        self.logger = logger('RESTClient', enabled=log_enabled, level=log_level)
+
+        # Credentials and settings for api url
+        self.username = username
+        self.password = password
+        self.protocol = protocol  # HTTP or HTTPS
+        self.host = host if host is not None else '127.0.0.1'
+        self.port = port
+        self.auth_uri = auth_uri
+        self.auth_key = auth_key
+        self.auth_payload = auth_payload
+        self.auth_basic = auth_basic
+        self.connect_timeout = connect_timeout
+        self.read_timeout = read_timeout
+        self.header = header or get_header_default()  # Default header
+
+    def __str__(self):
+        msg_print = (f'Username: {self.username}\n'
+                     f'Password: {self.password}\n'
+                     f'Base URL: {self.base_url}\n')
+
+        return msg_print
+
+    @property
+    def base_url(self):
+        """Create tested URL. Add port if it provided"""
+
+        base_url = f'{self.protocol}://{self.host}:{self.port}' if self.port else f'{self.protocol}://{self.host}'
+
+        return base_url
+
+    def requested_url(self, url) -> str:
+        """Return full URL if link specified starts with <http>"""
+
+        try:
+            requested_url = url if url.startswith('http') else urljoin(self.base_url, url)
+        except Exception as err:
+            self.logger.exception(f'URL does not specified. Used: "{url}" only. Specify full URL or use constructor')
+            raise err
+
+        return requested_url
+
+    @property
+    def auth_url(self):
+        """Get full authorization URL"""
+
+        return urljoin(self.base_url, self.auth_uri)
+
+    @staticmethod
+    def _validate_url(url):
+        return re.match(r'https?://[\w/.]+', url)
+
+    def encode_to_base64(self, string: str) -> str:
+        """Encode string to base64. Do not use it during creating class instance (logger won't work)
+
+        Args:
+            string: Some text to encode.
+
+        Returns:
+            Base64 encoded string.
+        """
+
+        try:
+            str_text = string.encode()
+            base64_encoded = base64.b64encode(str_text)
+        except AttributeError as err:
+            self.logger.error(f'Cannot encode specific data ({string}, {type(string)})')
+            raise err
+
+        result = base64_encoded.decode()
+        return result
+
+    def get_token(self):
+        """Get token.
+
+        - Send request to auth URL
+        - Get dict
+        - Get specific key
+
+        :return:
+        """
+
+        self.logger.debug(f'-> Get auth token by "{self.auth_key}"')
+
+        response_json = None
+        payload = self.auth_payload
+        timeout = (self.connect_timeout, self.read_timeout)
+        params = {
+            'url': self.auth_url,
+            'json': payload,
+            'verify': False,
+            'timeout': timeout,
+        }
+
+        self.logger.debug(f'Body: {dict_to_log(params)}')
+
+        try:
+            response = requests.post(**params)
+
+            resp_to_log = f'{response.status_code}: {dict_to_log(response.json())}'
+            self.logger.debug(resp_to_log)
+
+            response_json = response.json()
+            return response_json[self.auth_key]
+        except KeyError as err:
+            self.logger.exception(f'Cannot get key (token) from json data:{dict_to_log(response_json)}')
+            raise err
+        except json.decoder.JSONDecodeError as err:
+            msg = f'Cannot get token property. URL: {self.auth_url} ({self.auth_payload})'
+            self.logger.exception(msg)
+            raise err
+        except TypeError as err:
+            self.logger.exception('Endpoint is available but "token" key cannot be retrieved.')
+            raise err
+        except requests.exceptions.ConnectTimeout as err:
+            self.logger.exception(f'Perhaps, URI ({self.auth_url}) or service is unreachable:\n\t{err}')
+            raise err
+
+    def get_auth_header(self, header: dict = '') -> dict:
+        """Get auth header with a token
+
+        :param header: custom header is needed
+        :return:
+        """
+
+        self.logger.debug('Get auth header with a token')
+
+        try:
+            self.header = header.copy()
+        except AttributeError:
+            self.header = get_header_default()
+
+        # if 'Authorization' in self.header:
+        #     self.logger.debug('Header already contains "Authorization"')
+        #     return self.header
+        # else:
+        #     self.logger.debug('Try to get token to header')
+
+        try:
+            # noinspection PyAttributeOutsideInit
+            self.token = self.get_token()
+            self.header['Authorization'] = self.token
+
+            self.logger.debug(self.header)
+
+            return self.header
+        except KeyError as err:
+            self.logger.error(f'Cannot get token: {err}')
+            raise err
+
+    def _auth_basic(self):
+        """Enable basic auth if provided"""
+
+        self.header = {}
+        return self.username, self.password
+
+    def send_request(self,
+                     method: str,
+                     url: str,
+                     data: dict = None,
+                     files=None,
+                     query_params: dict = None,
+                     verify: bool = False,
+                     custom_header: dict = None,
+                     cookies=None,
+                     read_timeout: int = None):
+        """Send common REST request
+
+        To upload file use:
+
+        with open(files, 'rb') as f:
+             files = {'licenseFile': (License.name, f)}
+
+        Args:
+            method: GET, POST, DELETE
+            url: unified identifier, self.url (BASE) + url
+            data: json data
+            files: "files: {'licenseFile': (License.name, f)}"
+            query_params: Query parameters in the url
+            cookies:
+            verify: Ignore SSL verification?
+            custom_header: Use specified header
+            read_timeout: Read timeout in sec.
+
+        Returns:
+            requests.request('POST', url=url, headers=HEADER, files=files, verify=False)
+        """
+
+        # Get timeouts
+        read_timeout_ = self.read_timeout if read_timeout is None else read_timeout
+        common_timeout = self.read_timeout, read_timeout_
+
+        # Set auth method
+        if self.auth_payload is not None:
+            self.header = self.get_auth_header(header=custom_header)
+        elif self.auth_basic:
+            self.auth_basic = self._auth_basic()
+
+        if custom_header:
+            self.header = custom_header
+
+        # Make full url to use in request
+        link = self.requested_url(url)
+
+        # Add params to requested link
+        if query_params:
+            link += '?' + urlencode(query_params)
+
+        method = method.upper()
+        methods_available = 'GET', 'HEAD', 'DELETE', 'POST', 'PUT', 'PATCH', 'OPTIONS'
+        assert method in methods_available, 'Specified methods is not compatible.'
+
+        if data and files:
+            self.logger.error('Data parameter cannot be used with files parameter simultaneously.')
+            raise ValueError('Data parameter cannot be used with files parameter simultaneously.')
+
+        # Extend header
+        if 'Content-Type' not in self.header:
+            self.header['Content-Type'] = 'application/json'
+
+        response = 'Invalid requests. Check parameters'
+
+        self.logger.info(f'[{method}] {link}')
+
+        try:
+            # For 'POST', 'PUT', 'PATCH', 'OPTIONS', 'DELETE'
+            if method in ['POST', 'PUT', 'PATCH', 'OPTIONS', 'DELETE']:
+                if data and not files:
+
+                    self.logger.debug(f'Parameters:\n\t{self.header = }\n\t{cookies = }\n\t{common_timeout = }')
+                    self.logger.info('PAYLOAD:\n' + json.dumps(data, indent=4))
+
+                    response = requests.request(method=method,
+                                                url=link,
+                                                auth=self.auth_basic,
+                                                headers=self.header,
+                                                json=data,
+                                                cookies=cookies,
+                                                verify=verify,
+                                                timeout=common_timeout)
+
+                elif files:
+                    files_header = self.header.copy()
+                    del files_header['Content-Type']
+
+                    self.logger.debug(f'{files_header = }, {cookies = }, {common_timeout = }')
+                    self.logger.info('PAYLOAD:\n' + json.dumps(data, indent=4))
+
+                    response = requests.request(method=method,
+                                                url=link,
+                                                auth=self.auth_basic,
+                                                headers=files_header,
+                                                cookies=cookies,
+                                                files=files,
+                                                verify=verify,
+                                                timeout=common_timeout)
+
+                elif not files and not data:
+                    self.logger.debug(f'Parameters:\n\t{self.header = }\n\t{cookies = }\n\t{common_timeout = }')
+
+                    response = requests.request(method=method,
+                                                url=link,
+                                                auth=self.auth_basic,
+                                                headers=self.header,
+                                                cookies=cookies,
+                                                verify=verify,
+                                                timeout=common_timeout)
+
+            # For 'GET', 'HEAD' request
+            else:
+                # For usual 'GET' without query params
+                self.logger.debug(f'Parameters:\n\t{self.header = }\n\t{cookies = }\n\t{common_timeout = }')
+
+                response = requests.request(method=method,
+                                            url=link,
+                                            auth=self.auth_basic,
+                                            cookies=cookies,
+                                            headers=self.header,
+                                            verify=verify,
+                                            timeout=common_timeout)
+        except requests.exceptions.ReadTimeout as err:
+            self.logger.exception(f'The request took too long. Read timed out. (read timeout={common_timeout[1]})')
+            raise err
+        except BaseException as err:
+            self.logger.exception('Something went wrong.')
+            raise err
+
+        self.logger.info(f'{response.status_code}: "{response.text}"')
+
+        return response
+
+    @property
+    def is_service_available(self):
+        """Check base url availability within 10 sec."""
+
+        try:
+            response = requests.get(self.base_url, timeout=10, verify=False)
+            if response.status_code == 200:
+                return True
+            return False
+        except requests.exceptions.Timeout:
+            return False
+        except requests.exceptions.ConnectionError:
+            return False
+
+    def download(self, url: str, dst: str):
+        """Download file.
+
+        :param url: Full url to file
+        :param dst: path to store
+        :return:
+        """
+
+        response = self.GET(url)
+        try:
+            if response.ok:
+                with open(dst, 'wb') as f:
+                    f.write(response.content)
+                    return True
+            else:
+                return False
+        except (ConnectionError, ConnectionRefusedError) as err:
+            self.logger.exception('Download failed')
+            return err
+
+    # noinspection PyPep8Naming
+    def GET(self,
+            url: str = '',
+            query_params: dict = None,
+            cookies=None,
+            read_timeout: int = None,
+            header: dict = None):
+
+        return self.send_request(method='GET',
+                                 url=url,
+                                 query_params=query_params,
+                                 cookies=cookies,
+                                 read_timeout=read_timeout,
+                                 custom_header=header)
+
+    # noinspection PyPep8Naming
+    def POST(self,
+             url: str = '',
+             data: dict = None,
+             file=None,
+             query_params: dict = None,
+             cookies=None,
+             read_timeout: int = None,
+             header: dict = None):
+
+        return self.send_request(method='POST',
+                                 url=url,
+                                 query_params=query_params,
+                                 data=data,
+                                 files=file,
+                                 cookies=cookies,
+                                 read_timeout=read_timeout,
+                                 custom_header=header)
+
+    # noinspection PyPep8Naming
+    def PUT(self,
+            url: str = '',
+            data: dict = '',
+            files='',
+            query_params: dict = None,
+            cookies=None,
+            read_timeout: int = None,
+            header: dict = None):
+
+        header_original = self.header.copy()
+
+        if files:  # FIXME
+            del header_original['Content-Type']
+
+        return self.send_request(method='PUT',
+                                 url=url,
+                                 data=data,
+                                 files=files,
+                                 query_params=query_params,
+                                 cookies=cookies,
+                                 read_timeout=read_timeout,
+                                 custom_header=header)
+
+    def DELETE(self,
+               url: str = '',
+               data: dict = '',
+               query_params: dict = None,
+               cookies=None,
+               read_timeout: int = None,
+               header: dict = None):
+
+        return self.send_request(method='DELETE',
+                                 url=url,
+                                 query_params=query_params,
+                                 data=data,
+                                 cookies=cookies,
+                                 read_timeout=read_timeout,
+                                 custom_header=header)
+
+    def is_host_available(self, port: int = 0, timeout: int = 5) -> bool:
+        """Check remote host availability using socket and specified port"""
+
+        port_ = port or self.port
+        with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sock:
+            sock.settimeout(timeout)
+            result = sock.connect_ex((self.host, port_))
+            return False if result else True
+
+    def is_service_initialized(self, timeout: Union[int, float] = 20) -> bool:
+        """Send GET to base URL https://{IP}:{PORT}
+
+        :param timeout:
+        :return:
+        """
+
+        try:
+            response = requests.get(self.base_url, verify=False, timeout=timeout)
+            return response.ok
+        except requests.exceptions.ConnectionError:
+            return False
+
+    def wait_service_start(self, timeout: int = 30, interval: int = 3) -> bool:
+        """Waiting for the service start.
+
+        :param timeout: in sec.
+        :param interval: in sec.
+        :return:
+        """
+
+        timer = 0
+        status = self.is_service_initialized(1)
+
+        while not status:
+            status = self.is_service_initialized(1)
+            timer += interval
+
+            if timer > timeout - 2:
+                raise TimeoutError(f'The service was not started within {timeout} seconds.')
+            time.sleep(interval)
+        return status
+
+
+def get_header_default(user_agent='ide', content_type='application/json-patch+json', accept='application/json'):
+    return {
+        'User-Agent': user_agent,
+        'Content-Type': content_type,
+        'Accept': accept,
+        # 'UserAgentInternal': 'webfrontend/1.0'
+    }
+
+
+def dict_to_log(data: dict | list, sort: bool = False, ensure_ascii: bool = False) -> str:
+    """Pretty dict data to log"""
+
+    def convert_data_to_log(obj):
+        """Convert datetime, IPv4Address, requests Response...
+
+        :param obj: Object to convert
+        :return:
+        """
+
+        from requests.models import Response
+        from io import BufferedReader
+
+        match obj:
+            # IP address object handler
+            case ipaddress.IPv4Address() | set():
+                return obj.__str__()
+            # Datetime handler
+            case datetime() | date():
+                return obj.isoformat()
+            # REST response handler
+            case Response():
+                try:
+                    response_json_data = obj.json()
+                except JSONDecodeError:
+                    response_json_data = None
+
+                msg = {
+                    'ok': obj.ok,
+                    'response_code': obj.status_code,
+                    'text': obj.text,
+                    'json': response_json_data,
+                    'reason': obj.reason,
+                    'url': obj.url,
+                }
+                return msg
+            # Stream object handler
+            case BufferedReader():
+                return f'[BufferedReader] {obj.name}'
+            # case _:
+            # logger.debug('No data types detected to convert. Pass data directly.')
+            # return obj
+
+    json_data = json.dumps(obj=data, sort_keys=sort, ensure_ascii=ensure_ascii, indent=4, default=convert_data_to_log)
+
+    return f'\n{json_data}'
```

### Comparing `pyrestclient-1.1.8/pyrestclient.egg-info/PKG-INFO` & `pyrestclient-1.1.9/pyrestclient.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,198 +1,204 @@
-Metadata-Version: 2.1
-Name: pyrestclient
-Version: 1.1.8
-Summary: The simple http client and REST test tool for humans.
-Home-page: https://github.com/c-pher/RESTClient.git
-Author: Andrey Komissarov
-Author-email: a.komisssarov@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: System Administrators
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: System :: Systems Administration
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![PyPI version](https://badge.fury.io/py/pyrestclient.svg)](https://badge.fury.io/py/pyrestclient)
-
-# RESTClient
-
-The cross-platform tool to work with http.
-
-## Installation
-
-For most users, the recommended method to install is via pip:
-
-```cmd
-pip install pyrestclient
-```
-
-or from source:
-
-```cmd
-python setup.py install
-```
-
-## Import
-
-```python
-from pyrestclient import RESTClient
-```
-
----
-
-## Changelog
-
-##### UNRELEASED
-
-##### 1.1.8 (13.09.2022)
-
-Read timeout adjustment added. From now on you can set read and connection timeout simultaneously
-
-- "auth_timeout" renamed to "connect_timeout" and value reduced to 5
-- "read_timeout" global param added. Default value - 60.
-- logger_enabled renamed to log_enabled
-- logger_level renamed to log_level
-- minor refactoring
-
-##### 1.1.7.post0 (8.07.2022)
-
-- logger error fixed
-- log level handler added
-
-##### 1.1.7 (8.07.2022)
-
-- typo fixed
-- requested_url() refactored
-- encode_to_base64 logger added
-- "[Response]" replaces with the "<-"
-
-##### 1.1.6 (3.06.2022)
-
-- logger name is now `RESTClient`
-
-##### 1.1.5 (24.05.2022)
-
-Breaking changes:
-REST assertion renamed and changed:
-
-- return bool now
-- is_success()
-- is_ok()
-- is_not_found()
-- is_bad_request()
-- is_unauthorized() new method
-
-##### 1.1.4 (23.05.2022)
-
-- response logger added
-- json_data() removed
-
-##### 1.1.3 (17.04.2022)
-
-- updated to manage logger state
-
-##### 1.1.2 (29.03.2022)
-
-- 'host' attr is '127.0.0.1' by default
-- 'auth_timeout=7': new attr added
-- '.encode_to_base64()': new method added
-- plogger package added as dependency
-- internal logger removed as unused
-
-##### 1.1.1 (15.02.2022)
-
-wait_service_start fixed. added interval parameter
-
-##### 1.1.0 (8.02.2022)
-
-- Fixed custom header usage
-
-##### 1.0.9.post0 (29.12.2021)
-
-Fixed get token logger
-
-##### 1.0.9 (06.12.2021)
-
-- token property changed to catch unavailability occasions (not verifying base URL availability)
-
-##### 1.0.8.post0 (31.08.2021)
-
-- post without data fixed
-- refactored custom header
-
-##### 1.0.8 (31.08.2021)
-
-- logger added as attr
-
-##### 1.0.7 (21.05.2021)
-
-- POST, PUT, DELETE extended with header=None param
-
-##### 1.0.6 (24.02.2021)
-
-- refactoring. used lazy initialization to get token
-- wait_service_start: for the is_service_initialized under the hood used 0.1 sec by default
-
-##### 1.0.5 (24.02.2021)
-
-is_service_initialized updated to use timeout
-
-##### 1.0.4 (21.12.2020)
-
-logger auth link fixed
-
-##### 1.0.3 (21.12.2020)
-
-header param added to the GET method
-
-##### 1.0.2 (31.10.2020)
-
-New base method added:
-
-- is_host_available (Check remote host availability using socket and specified port)
-- is_service_initialized (GET https://{IP}:{PORT})
-- wait_service_start
-
-##### 1.0.1 (29.10.2020)
-
-- PUT fixed
-- RESTClient inherited from RESTAssertion. No need to import RESTAssertion directly
-
-#####1.0.0 (14.10.2020)
-- removed "extend_header"
-
-#####0.1.0 (21.05.2020)
-- file logging removed
-
-#####0.0.9 (28.03.2020)
-DELETE fixed
-POST: added file support
-
-#####0.0.8 (28.03.2020)
-header typing hint fixed. Now it is dict
-
-#####0.0.7 (10.03.2020)
-- Added query_params to all methods
-- POST method was refactored to use .send_request()
-
-#####0.0.6 (01.03.2020)
-- removed full_url param. now it will automatically convert url. use "http[s]://site.com" format in methods to use full url.
-- code refactoring
-
-#####0.0.5 (01.03.2020)
-- query params refactored to use urlencode
-- added DELETE method
-
-##### 0.0.4 (27.02.2020)
-should_be_bad_request: assert text fixed
-...
-
-##### 0.0.1 (9.02.2020)
-- initial commit
+Metadata-Version: 2.1
+Name: pyrestclient
+Version: 1.1.9
+Summary: The simple http client and REST test tool for humans.
+Home-page: https://github.com/c-pher/RESTClient.git
+Author: Andrey Komissarov
+Author-email: a.komisssarov@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: System Administrators
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: System :: Systems Administration
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI version](https://badge.fury.io/py/pyrestclient.svg)](https://badge.fury.io/py/pyrestclient)
+
+# RESTClient
+
+The cross-platform tool to work with http.
+
+## Installation
+
+For most users, the recommended method to install is via pip:
+
+```cmd
+pip install pyrestclient
+```
+
+or from source:
+
+```cmd
+python setup.py install
+```
+
+## Import
+
+```python
+from pyrestclient import RESTClient
+```
+
+---
+
+## Changelog
+
+##### UNRELEASED
+
+##### 1.1.9 (31.05.2023)
+
+- auth_key attr added to customize auth response
+- AuthToken removed. all it methods moved inside core class
+- debug log extended
+
+##### 1.1.8 (13.09.2022)
+
+Read timeout adjustment added. From now on you can set read and connection timeout simultaneously
+
+- "auth_timeout" renamed to "connect_timeout" and value reduced to 5
+- "read_timeout" global param added. Default value - 60.
+- logger_enabled renamed to log_enabled
+- logger_level renamed to log_level
+- minor refactoring
+
+##### 1.1.7.post0 (8.07.2022)
+
+- logger error fixed
+- log level handler added
+
+##### 1.1.7 (8.07.2022)
+
+- typo fixed
+- requested_url() refactored
+- encode_to_base64 logger added
+- "[Response]" replaces with the "<-"
+
+##### 1.1.6 (3.06.2022)
+
+- logger name is now `RESTClient`
+
+##### 1.1.5 (24.05.2022)
+
+Breaking changes:
+REST assertion renamed and changed:
+
+- return bool now
+- is_success()
+- is_ok()
+- is_not_found()
+- is_bad_request()
+- is_unauthorized() new method
+
+##### 1.1.4 (23.05.2022)
+
+- response logger added
+- json_data() removed
+
+##### 1.1.3 (17.04.2022)
+
+- updated to manage logger state
+
+##### 1.1.2 (29.03.2022)
+
+- 'host' attr is '127.0.0.1' by default
+- 'auth_timeout=7': new attr added
+- '.encode_to_base64()': new method added
+- plogger package added as dependency
+- internal logger removed as unused
+
+##### 1.1.1 (15.02.2022)
+
+wait_service_start fixed. added interval parameter
+
+##### 1.1.0 (8.02.2022)
+
+- Fixed custom header usage
+
+##### 1.0.9.post0 (29.12.2021)
+
+Fixed get token logger
+
+##### 1.0.9 (06.12.2021)
+
+- token property changed to catch unavailability occasions (not verifying base URL availability)
+
+##### 1.0.8.post0 (31.08.2021)
+
+- post without data fixed
+- refactored custom header
+
+##### 1.0.8 (31.08.2021)
+
+- logger added as attr
+
+##### 1.0.7 (21.05.2021)
+
+- POST, PUT, DELETE extended with header=None param
+
+##### 1.0.6 (24.02.2021)
+
+- refactoring. used lazy initialization to get token
+- wait_service_start: for the is_service_initialized under the hood used 0.1 sec by default
+
+##### 1.0.5 (24.02.2021)
+
+is_service_initialized updated to use timeout
+
+##### 1.0.4 (21.12.2020)
+
+logger auth link fixed
+
+##### 1.0.3 (21.12.2020)
+
+header param added to the GET method
+
+##### 1.0.2 (31.10.2020)
+
+New base method added:
+
+- is_host_available (Check remote host availability using socket and specified port)
+- is_service_initialized (GET https://{IP}:{PORT})
+- wait_service_start
+
+##### 1.0.1 (29.10.2020)
+
+- PUT fixed
+- RESTClient inherited from RESTAssertion. No need to import RESTAssertion directly
+
+#####1.0.0 (14.10.2020)
+- removed "extend_header"
+
+#####0.1.0 (21.05.2020)
+- file logging removed
+
+#####0.0.9 (28.03.2020)
+DELETE fixed
+POST: added file support
+
+#####0.0.8 (28.03.2020)
+header typing hint fixed. Now it is dict
+
+#####0.0.7 (10.03.2020)
+- Added query_params to all methods
+- POST method was refactored to use .send_request()
+
+#####0.0.6 (01.03.2020)
+- removed full_url param. now it will automatically convert url. use "http[s]://site.com" format in methods to use full url.
+- code refactoring
+
+#####0.0.5 (01.03.2020)
+- query params refactored to use urlencode
+- added DELETE method
+
+##### 0.0.4 (27.02.2020)
+should_be_bad_request: assert text fixed
+...
+
+##### 0.0.1 (9.02.2020)
+- initial commit
```

### Comparing `pyrestclient-1.1.8/setup.py` & `pyrestclient-1.1.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from os import path
-
-from setuptools import setup
-
-INSTALL_REQUIRES = [
-    'requests>=2.22.0',
-    'urllib3',
-    'plogger>=1.0.6'
-]
-
-this_directory = path.abspath(path.dirname(__file__))
-with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
-    long_description = f.read()
-
-setup(name='pyrestclient',
-      version='1.1.8',
-      packages=['pyrestclient'],
-      url='https://github.com/c-pher/RESTClient.git',
-      license='MIT',
-      author='Andrey Komissarov',
-      author_email='a.komisssarov@gmail.com',
-      description='The simple http client and REST test tool for humans.',
-      long_description=long_description,
-      long_description_content_type='text/markdown',
-      classifiers=[
-          'Programming Language :: Python :: 3',
-          'License :: OSI Approved :: MIT License',
-          'Operating System :: OS Independent',
-          'Intended Audience :: System Administrators',
-          'Intended Audience :: Developers',
-          'Natural Language :: English',
-          'Programming Language :: Python :: 3.6',
-          'Topic :: System :: Systems Administration',
-          'Topic :: Software Development :: Libraries :: Python Modules'
-      ],
-      install_requires=INSTALL_REQUIRES,
-      python_requires='>=3.6',
-      )
+from os import path
+
+from setuptools import setup
+
+INSTALL_REQUIRES = [
+    'requests>=2.22.0',
+    'urllib3',
+    'plogger>=1.0.6'
+]
+
+this_directory = path.abspath(path.dirname(__file__))
+with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
+
+setup(name='pyrestclient',
+      version='1.1.9',
+      packages=['pyrestclient'],
+      url='https://github.com/c-pher/RESTClient.git',
+      license='MIT',
+      author='Andrey Komissarov',
+      author_email='a.komisssarov@gmail.com',
+      description='The simple http client and REST test tool for humans.',
+      long_description=long_description,
+      long_description_content_type='text/markdown',
+      classifiers=[
+          'Programming Language :: Python :: 3',
+          'License :: OSI Approved :: MIT License',
+          'Operating System :: OS Independent',
+          'Intended Audience :: System Administrators',
+          'Intended Audience :: Developers',
+          'Natural Language :: English',
+          'Programming Language :: Python :: 3.6',
+          'Topic :: System :: Systems Administration',
+          'Topic :: Software Development :: Libraries :: Python Modules'
+      ],
+      install_requires=INSTALL_REQUIRES,
+      python_requires='>=3.6',
+      )
```

