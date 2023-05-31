# Comparing `tmp/automation_anywhere-2.1.2.tar.gz` & `tmp/automation_anywhere-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_anywhere-2.1.2.tar", last modified: Fri May 19 19:59:46 2023, max compression
+gzip compressed data, was "automation_anywhere-2.1.3.tar", last modified: Wed May 31 14:30:47 2023, max compression
```

## Comparing `automation_anywhere-2.1.2.tar` & `automation_anywhere-2.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-05-19 19:59:46.541676 automation_anywhere-2.1.2/
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     1067 2023-05-11 13:45:41.000000 automation_anywhere-2.1.2/LICENSE
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4008 2023-05-19 19:59:46.541676 automation_anywhere-2.1.2/PKG-INFO
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     3431 2023-05-19 18:02:53.000000 automation_anywhere-2.1.2/README.md
-drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-05-19 19:59:46.541676 automation_anywhere-2.1.2/automation_anywhere/
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)       56 2023-05-11 13:45:41.000000 automation_anywhere-2.1.2/automation_anywhere/__init__.py
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4068 2023-05-11 13:45:41.000000 automation_anywhere-2.1.2/automation_anywhere/base.py
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)      187 2023-05-11 13:45:41.000000 automation_anywhere-2.1.2/automation_anywhere/errors.py
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)    10135 2023-05-19 19:58:23.000000 automation_anywhere-2.1.2/automation_anywhere/executor.py
-drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-05-19 19:59:46.541676 automation_anywhere-2.1.2/automation_anywhere.egg-info/
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4008 2023-05-19 19:59:46.000000 automation_anywhere-2.1.2/automation_anywhere.egg-info/PKG-INFO
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)      326 2023-05-19 19:59:46.000000 automation_anywhere-2.1.2/automation_anywhere.egg-info/SOURCES.txt
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)        1 2023-05-19 19:59:46.000000 automation_anywhere-2.1.2/automation_anywhere.egg-info/dependency_links.txt
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)       20 2023-05-19 19:59:46.000000 automation_anywhere-2.1.2/automation_anywhere.egg-info/top_level.txt
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)      642 2023-05-19 19:58:58.000000 automation_anywhere-2.1.2/pyproject.toml
--rw-r--r--   0 minterciso  (1000) minterciso  (1000)       38 2023-05-19 19:59:46.541676 automation_anywhere-2.1.2/setup.cfg
+drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-05-31 14:30:47.137302 automation_anywhere-2.1.3/
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     1067 2023-05-11 13:45:41.000000 automation_anywhere-2.1.3/LICENSE
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4008 2023-05-31 14:30:47.137302 automation_anywhere-2.1.3/PKG-INFO
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     3431 2023-05-19 18:02:53.000000 automation_anywhere-2.1.3/README.md
+drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-05-31 14:30:47.137302 automation_anywhere-2.1.3/automation_anywhere/
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)       56 2023-05-11 13:45:41.000000 automation_anywhere-2.1.3/automation_anywhere/__init__.py
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4371 2023-05-31 14:28:01.000000 automation_anywhere-2.1.3/automation_anywhere/base.py
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)      187 2023-05-11 13:45:41.000000 automation_anywhere-2.1.3/automation_anywhere/errors.py
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)    10423 2023-05-31 14:29:22.000000 automation_anywhere-2.1.3/automation_anywhere/executor.py
+drwxr-xr-x   0 minterciso  (1000) minterciso  (1000)        0 2023-05-31 14:30:47.137302 automation_anywhere-2.1.3/automation_anywhere.egg-info/
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)     4008 2023-05-31 14:30:47.000000 automation_anywhere-2.1.3/automation_anywhere.egg-info/PKG-INFO
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)      326 2023-05-31 14:30:47.000000 automation_anywhere-2.1.3/automation_anywhere.egg-info/SOURCES.txt
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)        1 2023-05-31 14:30:47.000000 automation_anywhere-2.1.3/automation_anywhere.egg-info/dependency_links.txt
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)       20 2023-05-31 14:30:47.000000 automation_anywhere-2.1.3/automation_anywhere.egg-info/top_level.txt
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)      642 2023-05-31 14:29:48.000000 automation_anywhere-2.1.3/pyproject.toml
+-rw-r--r--   0 minterciso  (1000) minterciso  (1000)       38 2023-05-31 14:30:47.137302 automation_anywhere-2.1.3/setup.cfg
```

### Comparing `automation_anywhere-2.1.2/LICENSE` & `automation_anywhere-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_anywhere-2.1.2/PKG-INFO` & `automation_anywhere-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation_anywhere
-Version: 2.1.2
+Version: 2.1.3
 Summary: A Python Package to deploy tasks on Automation Anywhere 360
 Author-email: Mateus Interciso <minterciso@gmail.com>
 Project-URL: Homepage, https://github.com/minterciso/pyAutomationAnywhere
 Project-URL: Bug Tracker, https://github.com/minterciso/pyAutomationAnywhere/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `automation_anywhere-2.1.2/README.md` & `automation_anywhere-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `automation_anywhere-2.1.2/automation_anywhere/base.py` & `automation_anywhere-2.1.3/automation_anywhere/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from requests import post, get
 
 from automation_anywhere.errors import AuthenticationError
 
 
 class Base:
     """This class is responsible for handling authentication on the AA360 cloud environment, and can help with more specific tasks."""
-    def __init__(self, base_url: str):
+    def __init__(self, base_url: str, verify_ssl: bool = True):
         """Initialize the class.
 
         :param base_url: The AA360 Orchestrator URL
         :type base_url: str
+        :param ignore_ssl: If set to False, it'll ignore the SSL on the requests, defaults to True
+        :type ignore_ssl: bool, optional
         """
         self.token = None
         self.user_info = None
         self.headers = None
+        self._verify_ssl = verify_ssl
         self._base_url = base_url
 
     def authenticate(self, username: str, password: str, multiple_login: bool = False) -> tuple[bool, str]:
         """Authenticate the user via username/password and store the token internally on the "token" variable.
 
         :param username: The username to login to
         :type username: str
@@ -32,15 +35,15 @@
         success = False
         endpoint = f'{self._base_url}v1/authentication'
         payload = {
             'username': username,
             'password': password,
             'multiLogin': multiple_login
         }
-        response = post(url=endpoint, json=payload)
+        response = post(url=endpoint, json=payload, verify=self._verify_ssl)
         if response.status_code == 200:
             self.token = response.json()['token']
             self.user_info = response.json()['user']
             self.headers = {'X-Authorization': self.token}
             success = True
         elif response.status_code == 401:
             error = 'Unable to login: Invalid username/password'
@@ -54,15 +57,15 @@
         :return: A tuple depicting if the token is valid (bool) and a string to show any errors.
         :rtype: tuple[bool, str]
         """
         status = False
         error = None
         endpoint = f'{self._base_url}v1/authentication/token'
         query = {'token': self.token}
-        response = get(url=endpoint, params=query)
+        response = get(url=endpoint, params=query, verify=self._verify_ssl)
         if response.status_code == 200:
             status = response.json()['valid']
         else:
             error = f'Unknown error: {response.json()["message"]}'
         return status, error
 
     def refresh(self) -> tuple[bool, str]:
@@ -73,15 +76,15 @@
         """
         success = False
         error = None
         endpoint = f'{self._base_url}v1/authentication/token'
         payload = {
             'token': self.token
         }
-        response = post(url=endpoint, json=payload)
+        response = post(url=endpoint, json=payload, verify=self._verify_ssl)
         if response.status_code == 200:
             success = True
             self.token = response.json()['token']
             self.headers = {'X-Authorization': self.token}
         else:
             error = f'Unknown error: {response.json()["message"]}'
         return success, error
@@ -91,13 +94,13 @@
 
         :return: A tuple depicting success for logging out, and a string for errors, if any
         :rtype: tuple[bool, str]
         """
         success = False
         error = None
         endpoint = f'{self._base_url}v1/authentication/logout'
-        response = post(url=endpoint, headers=self.headers)
+        response = post(url=endpoint, headers=self.headers, verify=self._verify_ssl)
         if response.status_code == 204:
             success = True
         else:
             error = f'Unknown error: {response.json()["message"]}'
         return success, error
```

### Comparing `automation_anywhere-2.1.2/automation_anywhere/executor.py` & `automation_anywhere-2.1.3/automation_anywhere/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from requests import post
 
 from automation_anywhere.base import Base
 from automation_anywhere.errors import AuthenticationError
 
 class Executor(Base):
     """Class used to deploy (and hopefully execute) a bot on the AA360 control room"""
-    def __init__(self, base_url: str, username: str, password: str, multiple_logins: bool = False):
+    def __init__(self, base_url: str, username: str, password: str, multiple_logins: bool = False, verify_ssl: bool = True):
         """The constructor.
 
         :param base_url: The AA360 ControlRoom URL.
         :type base_url: str
         :param username: The user used to deploy the bot.
         :type username: str
         :param password: The password to authenticate the user.
         :type password: str
         :param multiple_logins: If the user can and should have multiple logins, set to True, defaults to False
+        :param ignore_ssl: If set to False, it'll ignore the SSL on the requests, defaults to True
+        :type ignore_ssl: bool, optional
         :type multiple_logins: bool, optional
         :raises AuthenticationError: If there was an issue authenticating, it'll raise an AuthenticationError Exception
         """
-        super().__init__(base_url=base_url)
+        super().__init__(base_url=base_url, verify_ssl=verify_ssl)
         success, error = self.authenticate(
             username=username, password=password, multiple_login=multiple_logins)
         if success is False:
             raise AuthenticationError(error)
 
     def list_devices(self, sort: list = None, page: dict = None) -> tuple[list, dict, str]:
         """List all devices that can execute something. You need the user id of the device in order to execute something.
@@ -38,15 +40,15 @@
         page_data = None
         error = None
         endpoint = f'{self._base_url}v1/devices/runasusers/list'
         payload = dict()
         payload['page'] = page
         payload['sort'] = sort if sort is not None else [
             {'field': 'username', 'direction': 'asc'}]
-        response = post(url=endpoint, headers=self.headers, json=payload)
+        response = post(url=endpoint, headers=self.headers, json=payload, verify=self._verify_ssl)
         if response.status_code == 200:
             page_data = response.json()['page']
             devices = response.json()['list']
         elif response.status_code == 400:
             error = f'Bad Request - {response.json()["code"]}: {response.json()["message"]}'
         elif response.status_code == 401:
             error = f'Authentication Error - {response.json()["code"]}: {response.json()["message"]}'
@@ -86,15 +88,15 @@
             payload['filter'] = {
                 'operator': 'eq',
                 'field': 'name',
                 'value': name
             }
         else:
             payload['filter'] = filter
-        response = post(url=endpoint, json=payload, headers=self.headers)
+        response = post(url=endpoint, json=payload, headers=self.headers, verify=self._verify_ssl)
         if response.status_code == 200:
             page_data = response.json()['page']
             automations = response.json()['list']
         elif response.status_code == 400:
             error = f'Bad Request - {response.json()["code"]}: {response.json()["message"]}'
         elif response.status_code == 401:
             error = f'Authentication Error - {response.json()["code"]}: {response.json()["message"]}'
@@ -130,15 +132,15 @@
         payload = dict()
         payload['fileId'] = automation_id
         payload['runAsUserIds'] = users_ids
         payload['poolIds'] = pool_ids
         payload['callBackInfo'] = call_back_info
         payload['botInput'] = bot_input
         payload['overrideDefaultDevice'] = override_default_device
-        response = post(url=endpoint, json=payload, headers=self.headers)
+        response = post(url=endpoint, json=payload, headers=self.headers, verify=self._verify_ssl)
         if response.status_code == 200:
             deployment_id = response.json()['deploymentId']
             automation_name = response.json()['automationName']
             success = True
         elif response.status_code == 400:
             error = f'Bad Request - {response.json()["message"]}'
         elif response.status_code == 401:
@@ -187,15 +189,15 @@
             })
         payload = {
             'filter': filter if filter else local_filter,
             'page': page,
             'sort': sort
         }        
         endpoint = f'{self._base_url}v3/activity/list'
-        response = post(url=endpoint, headers=self.headers, json=payload)
+        response = post(url=endpoint, headers=self.headers, json=payload, verify=self._verify_ssl)
         if response.status_code == 200:
             return_data['executions'] = response.json()['list']
             return_data['page'] = response.json()['page']
             success = True
         elif response.status_code == 400:
             error = f'Bad Request - {response.json()["code"]}: {response.json()["message"]}'
         elif response.status_code == 401:
```

### Comparing `automation_anywhere-2.1.2/automation_anywhere.egg-info/PKG-INFO` & `automation_anywhere-2.1.3/automation_anywhere.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation-anywhere
-Version: 2.1.2
+Version: 2.1.3
 Summary: A Python Package to deploy tasks on Automation Anywhere 360
 Author-email: Mateus Interciso <minterciso@gmail.com>
 Project-URL: Homepage, https://github.com/minterciso/pyAutomationAnywhere
 Project-URL: Bug Tracker, https://github.com/minterciso/pyAutomationAnywhere/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `automation_anywhere-2.1.2/pyproject.toml` & `automation_anywhere-2.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="automation_anywhere"
-version="2.1.2"
+version="2.1.3"
 authors=[{name="Mateus Interciso", email="minterciso@gmail.com"}]
 description="A Python Package to deploy tasks on Automation Anywhere 360"
 readme="README.md"
 requires-python=">=3.9"
 classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

