# Comparing `tmp/wipac-keycloak-rest-services-1.3.9.tar.gz` & `tmp/wipac-keycloak-rest-services-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wipac-keycloak-rest-services-1.3.9.tar", last modified: Fri May  5 20:18:18 2023, max compression
+gzip compressed data, was "wipac-keycloak-rest-services-1.4.0.tar", last modified: Wed May 31 19:55:53 2023, max compression
```

## Comparing `wipac-keycloak-rest-services-1.3.9.tar` & `wipac-keycloak-rest-services-1.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 20:18:18.278320 wipac-keycloak-rest-services-1.3.9/
--rw-r--r--   0 root         (0) root         (0)     1103 2023-05-05 20:18:15.000000 wipac-keycloak-rest-services-1.3.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4044 2023-05-05 20:18:18.278320 wipac-keycloak-rest-services-1.3.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3036 2023-05-05 20:18:15.000000 wipac-keycloak-rest-services-1.3.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 20:18:18.278320 wipac-keycloak-rest-services-1.3.9/krs/
--rw-r--r--   0 root         (0) root         (0)      513 2023-05-05 20:18:16.000000 wipac-keycloak-rest-services-1.3.9/krs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20266 2023-05-05 20:18:15.000000 wipac-keycloak-rest-services-1.3.9/krs/apps.py
--rw-r--r--   0 root         (0) root         (0)    15733 2023-05-05 20:18:15.000000 wipac-keycloak-rest-services-1.3.9/krs/bootstrap.py
--rw-r--r--   0 root         (0) root         (0)     2870 2023-05-05 20:18:15.000000 wipac-keycloak-rest-services-1.3.9/krs/email.py
--rw-r--r--   0 root         (0) root         (0)    10971 2023-05-05 20:18:15.000000 wipac-keycloak-rest-services-1.3.9/krs/groups.py
--rw-r--r--   0 root         (0) root         (0)     8766 2023-05-05 20:18:15.000000 wipac-keycloak-rest-services-1.3.9/krs/institutions.py
--rw-r--r--   0 root         (0) root         (0)    22784 2023-05-05 20:18:15.000000 wipac-keycloak-rest-services-1.3.9/krs/ldap.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 20:18:15.000000 wipac-keycloak-rest-services-1.3.9/krs/py.typed
--rw-r--r--   0 root         (0) root         (0)     5722 2023-05-05 20:18:15.000000 wipac-keycloak-rest-services-1.3.9/krs/rabbitmq.py
--rw-r--r--   0 root         (0) root         (0)     2250 2023-05-05 20:18:15.000000 wipac-keycloak-rest-services-1.3.9/krs/token.py
--rw-r--r--   0 root         (0) root         (0)     9213 2023-05-05 20:18:15.000000 wipac-keycloak-rest-services-1.3.9/krs/users.py
--rw-r--r--   0 root         (0) root         (0)     2281 2023-05-05 20:18:18.278320 wipac-keycloak-rest-services-1.3.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-05 20:18:15.000000 wipac-keycloak-rest-services-1.3.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 20:18:18.278320 wipac-keycloak-rest-services-1.3.9/wipac_keycloak_rest_services.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4044 2023-05-05 20:18:18.000000 wipac-keycloak-rest-services-1.3.9/wipac_keycloak_rest_services.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      454 2023-05-05 20:18:18.000000 wipac-keycloak-rest-services-1.3.9/wipac_keycloak_rest_services.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 20:18:18.000000 wipac-keycloak-rest-services-1.3.9/wipac_keycloak_rest_services.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-05 20:18:18.000000 wipac-keycloak-rest-services-1.3.9/wipac_keycloak_rest_services.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-05 20:18:18.000000 wipac-keycloak-rest-services-1.3.9/wipac_keycloak_rest_services.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:55:53.000389 wipac-keycloak-rest-services-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-05-31 19:55:50.000000 wipac-keycloak-rest-services-1.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-05-31 19:55:53.000389 wipac-keycloak-rest-services-1.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3036 2023-05-31 19:55:50.000000 wipac-keycloak-rest-services-1.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:55:53.000389 wipac-keycloak-rest-services-1.4.0/krs/
+-rw-r--r--   0 root         (0) root         (0)      513 2023-05-31 19:55:50.000000 wipac-keycloak-rest-services-1.4.0/krs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20266 2023-05-31 19:55:50.000000 wipac-keycloak-rest-services-1.4.0/krs/apps.py
+-rw-r--r--   0 root         (0) root         (0)    15733 2023-05-31 19:55:50.000000 wipac-keycloak-rest-services-1.4.0/krs/bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)     2870 2023-05-31 19:55:50.000000 wipac-keycloak-rest-services-1.4.0/krs/email.py
+-rw-r--r--   0 root         (0) root         (0)    10971 2023-05-31 19:55:50.000000 wipac-keycloak-rest-services-1.4.0/krs/groups.py
+-rw-r--r--   0 root         (0) root         (0)     8766 2023-05-31 19:55:50.000000 wipac-keycloak-rest-services-1.4.0/krs/institutions.py
+-rw-r--r--   0 root         (0) root         (0)    22784 2023-05-31 19:55:50.000000 wipac-keycloak-rest-services-1.4.0/krs/ldap.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 19:55:50.000000 wipac-keycloak-rest-services-1.4.0/krs/py.typed
+-rw-r--r--   0 root         (0) root         (0)     5722 2023-05-31 19:55:50.000000 wipac-keycloak-rest-services-1.4.0/krs/rabbitmq.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2023-05-31 19:55:50.000000 wipac-keycloak-rest-services-1.4.0/krs/token.py
+-rw-r--r--   0 root         (0) root         (0)     9213 2023-05-31 19:55:50.000000 wipac-keycloak-rest-services-1.4.0/krs/users.py
+-rw-r--r--   0 root         (0) root         (0)     2281 2023-05-31 19:55:53.000389 wipac-keycloak-rest-services-1.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-31 19:55:50.000000 wipac-keycloak-rest-services-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 19:55:53.000389 wipac-keycloak-rest-services-1.4.0/wipac_keycloak_rest_services.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-05-31 19:55:52.000000 wipac-keycloak-rest-services-1.4.0/wipac_keycloak_rest_services.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      454 2023-05-31 19:55:52.000000 wipac-keycloak-rest-services-1.4.0/wipac_keycloak_rest_services.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 19:55:52.000000 wipac-keycloak-rest-services-1.4.0/wipac_keycloak_rest_services.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-31 19:55:52.000000 wipac-keycloak-rest-services-1.4.0/wipac_keycloak_rest_services.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-31 19:55:52.000000 wipac-keycloak-rest-services-1.4.0/wipac_keycloak_rest_services.egg-info/top_level.txt
```

### Comparing `wipac-keycloak-rest-services-1.3.9/LICENSE` & `wipac-keycloak-rest-services-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.3.9/PKG-INFO` & `wipac-keycloak-rest-services-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-keycloak-rest-services
-Version: 1.3.9
+Version: 1.4.0
 Summary: Services surrounding KeyCloak, that use the REST API to read/update state
 Home-page: https://github.com/WIPACrepo/keycloak-rest-services
 Download-URL: https://pypi.org/project/wipac-keycloak-rest-services/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_b3p5qfvd_/tmprnb3fssf_TarContainer/0/2", line 93, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_b3p5qfvd_/tmprnb3fssf_TarContainer/0/2", line 93, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.3.9
+Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.4.0
 Summary: Services surrounding KeyCloak, that use the REST API to read/update
 state Home-page: https://github.com/WIPACrepo/keycloak-rest-services Download-
 URL: https://pypi.org/project/wipac-keycloak-rest-services/ Author: WIPAC
 Developers Author-email: developers@icecube.wisc.edu License: MIT Project-URL:
 Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues Project-
 URL: Source, https://github.com/WIPACrepo/keycloak-rest-services Keywords:
 keycloak,rest,tools,utilities Classifier: Development Status :: 5 - Production/
```

### Comparing `wipac-keycloak-rest-services-1.3.9/README.md` & `wipac-keycloak-rest-services-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.3.9/krs/__init__.py` & `wipac-keycloak-rest-services-1.4.0/krs/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "1.3.9"
+__version__ = "1.4.0"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `wipac-keycloak-rest-services-1.3.9/krs/apps.py` & `wipac-keycloak-rest-services-1.4.0/krs/apps.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.3.9/krs/bootstrap.py` & `wipac-keycloak-rest-services-1.4.0/krs/bootstrap.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.3.9/krs/email.py` & `wipac-keycloak-rest-services-1.4.0/krs/email.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.3.9/krs/groups.py` & `wipac-keycloak-rest-services-1.4.0/krs/groups.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.3.9/krs/institutions.py` & `wipac-keycloak-rest-services-1.4.0/krs/institutions.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.3.9/krs/ldap.py` & `wipac-keycloak-rest-services-1.4.0/krs/ldap.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.3.9/krs/rabbitmq.py` & `wipac-keycloak-rest-services-1.4.0/krs/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.3.9/krs/token.py` & `wipac-keycloak-rest-services-1.4.0/krs/token.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 Get an admin token for KeyCloak.
 """
 import logging
-from functools import partial
 
 import requests
 from wipac_dev_tools import from_environment
-from rest_tools.client import RestClient
+from rest_tools.client import ClientCredentialsAuth, SavedDeviceGrantAuth
 
 
 def get_token(url, client_id, client_secret, client_realm='master'):
     url = f'{url}/auth/realms/{client_realm}/protocol/openid-connect/token'
     args = {
         'grant_type': 'client_credentials',
         'client_id': client_id,
@@ -22,49 +21,57 @@
     r.raise_for_status()
     req = r.json()
     return req['access_token']
 
 
 def get_rest_client(retries=None, timeout=10):
     config = from_environment({
-        'KEYCLOAK_REALM': None,
-        'KEYCLOAK_URL': None,
+        'KEYCLOAK_REALM': 'icecube',
+        'KEYCLOAK_URL': 'https://keycloak.icecube.wisc.edu',
         'KEYCLOAK_CLIENT_ID': 'rest-access',
-        'KEYCLOAK_CLIENT_SECRET': None,
+        'KEYCLOAK_CLIENT_SECRET': '',
         'KEYCLOAK_CLIENT_REALM': 'master',
     })
-    token_func = partial(
-        get_token,
-        config["KEYCLOAK_URL"],
-        client_id=config['KEYCLOAK_CLIENT_ID'],
-        client_secret=config['KEYCLOAK_CLIENT_SECRET'],
-        client_realm=config['KEYCLOAK_CLIENT_REALM'],
-    )
     kwargs = {'timeout': timeout}
     if retries:
         kwargs['retries'] = retries
-    return RestClient(
-        f'{config["KEYCLOAK_URL"]}/auth/admin/realms/{config["KEYCLOAK_REALM"]}',
-        token=token_func,
-        **kwargs
-    )
+    if config['KEYCLOAK_CLIENT_SECRET']:
+        return ClientCredentialsAuth(
+            address=f'{config["KEYCLOAK_URL"]}/auth/admin/realms/{config["KEYCLOAK_REALM"]}',
+            token_url=f'{config["KEYCLOAK_URL"]}/auth/realms/{config["KEYCLOAK_CLIENT_REALM"]}',
+            client_id=config['KEYCLOAK_CLIENT_ID'],
+            client_secret=config['KEYCLOAK_CLIENT_SECRET'],
+            **kwargs
+        )
+    else:
+        if config['KEYCLOAK_CLIENT_ID'] == 'rest-access':
+            config['KEYCLOAK_CLIENT_ID'] = 'rest-access-admin'
+        return SavedDeviceGrantAuth(
+            address=f'{config["KEYCLOAK_URL"]}/auth/admin/realms/{config["KEYCLOAK_REALM"]}',
+            token_url=f'{config["KEYCLOAK_URL"]}/auth/realms/{config["KEYCLOAK_CLIENT_REALM"]}',
+            filename='.keycloak-rest-services-auth',
+            client_id=config['KEYCLOAK_CLIENT_ID'],
+            **kwargs
+        )
 
 
 def main():
     import argparse
     from pprint import pprint
 
     parser = argparse.ArgumentParser(description='Keycloak tokens')
     subparsers = parser.add_subparsers()
     parser_get = subparsers.add_parser('get', help='get token')
     parser_get.add_argument('url', help='keycloak base url')
     parser_get.add_argument('client_id', help='keycloak client id')
     parser_get.add_argument('client_secret', help='keycloak client secret')
     parser_get.add_argument('--client_realm', default='master', help='keycloak client realm')
     parser_get.set_defaults(func=get_token)
+    parser_rc = subparsers.add_parser('rc', help='get rest client')
+    parser_rc.set_defaults(func=get_rest_client)
     args = vars(parser.parse_args())
 
     logging.basicConfig(format='%(levelname)s: %(message)s', level=logging.INFO)
 
     func = args.pop('func')
     ret = func(**args)
     if ret is not None:
```

### Comparing `wipac-keycloak-rest-services-1.3.9/krs/users.py` & `wipac-keycloak-rest-services-1.4.0/krs/users.py`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.3.9/setup.cfg` & `wipac-keycloak-rest-services-1.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `wipac-keycloak-rest-services-1.3.9/wipac_keycloak_rest_services.egg-info/PKG-INFO` & `wipac-keycloak-rest-services-1.4.0/wipac_keycloak_rest_services.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-keycloak-rest-services
-Version: 1.3.9
+Version: 1.4.0
 Summary: Services surrounding KeyCloak, that use the REST API to read/update state
 Home-page: https://github.com/WIPACrepo/keycloak-rest-services
 Download-URL: https://pypi.org/project/wipac-keycloak-rest-services/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_b3p5qfvd_/tmprnb3fssf_TarContainer/0/19", line 93, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_b3p5qfvd_/tmprnb3fssf_TarContainer/0/19", line 93, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.3.9
+Metadata-Version: 2.1 Name: wipac-keycloak-rest-services Version: 1.4.0
 Summary: Services surrounding KeyCloak, that use the REST API to read/update
 state Home-page: https://github.com/WIPACrepo/keycloak-rest-services Download-
 URL: https://pypi.org/project/wipac-keycloak-rest-services/ Author: WIPAC
 Developers Author-email: developers@icecube.wisc.edu License: MIT Project-URL:
 Tracker, https://github.com/WIPACrepo/keycloak-rest-services/issues Project-
 URL: Source, https://github.com/WIPACrepo/keycloak-rest-services Keywords:
 keycloak,rest,tools,utilities Classifier: Development Status :: 5 - Production/
```

