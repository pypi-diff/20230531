# Comparing `tmp/auth_package-1.0.tar.gz` & `tmp/auth_package-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth_package-1.0.tar", last modified: Mon May 29 20:13:53 2023, max compression
+gzip compressed data, was "dist/auth_package-1.1.tar", last modified: Wed May 31 05:07:40 2023, max compression
```

## Comparing `auth_package-1.0.tar` & `auth_package-1.1.tar`

### file list

```diff
@@ -1,16 +1,8 @@
-drwxr-xr-x   0 raminzamani   (501) staff       (20)        0 2023-05-29 20:13:53.904017 auth_package-1.0/
--rw-r--r--   0 raminzamani   (501) staff       (20)     1061 2023-05-29 19:53:56.000000 auth_package-1.0/LICENSE.txt
--rw-r--r--   0 raminzamani   (501) staff       (20)      989 2023-05-29 20:13:53.904093 auth_package-1.0/PKG-INFO
--rw-r--r--   0 raminzamani   (501) staff       (20)        0 2023-05-29 19:40:35.000000 auth_package-1.0/README.md
-drwxr-xr-x   0 raminzamani   (501) staff       (20)        0 2023-05-29 20:13:53.903002 auth_package-1.0/auth_package/
--rw-r--r--   0 raminzamani   (501) staff       (20)      233 2023-05-29 19:39:45.000000 auth_package-1.0/auth_package/__init__.py
--rw-r--r--   0 raminzamani   (501) staff       (20)     2947 2023-05-29 18:31:36.000000 auth_package-1.0/auth_package/permission.py
--rw-r--r--   0 raminzamani   (501) staff       (20)     1794 2023-05-29 19:21:46.000000 auth_package-1.0/auth_package/user.py
-drwxr-xr-x   0 raminzamani   (501) staff       (20)        0 2023-05-29 20:13:53.903852 auth_package-1.0/auth_package.egg-info/
--rw-r--r--   0 raminzamani   (501) staff       (20)      989 2023-05-29 20:13:53.000000 auth_package-1.0/auth_package.egg-info/PKG-INFO
--rw-r--r--   0 raminzamani   (501) staff       (20)      292 2023-05-29 20:13:53.000000 auth_package-1.0/auth_package.egg-info/SOURCES.txt
--rw-r--r--   0 raminzamani   (501) staff       (20)        1 2023-05-29 20:13:53.000000 auth_package-1.0/auth_package.egg-info/dependency_links.txt
--rw-r--r--   0 raminzamani   (501) staff       (20)        9 2023-05-29 20:13:53.000000 auth_package-1.0/auth_package.egg-info/requires.txt
--rw-r--r--   0 raminzamani   (501) staff       (20)       13 2023-05-29 20:13:53.000000 auth_package-1.0/auth_package.egg-info/top_level.txt
--rw-r--r--   0 raminzamani   (501) staff       (20)       79 2023-05-29 20:13:53.904708 auth_package-1.0/setup.cfg
--rw-r--r--   0 raminzamani   (501) staff       (20)     1862 2023-05-29 20:13:50.000000 auth_package-1.0/setup.py
+drwxr-xr-x   0 raminzamani   (501) staff       (20)        0 2023-05-31 05:07:40.000000 auth_package-1.1/
+-rw-r--r--   0 raminzamani   (501) staff       (20)     1002 2023-05-31 05:07:40.000000 auth_package-1.1/PKG-INFO
+-rw-r--r--   0 raminzamani   (501) staff       (20)     1862 2023-05-31 05:07:21.000000 auth_package-1.1/setup.py
+drwxr-xr-x   0 raminzamani   (501) staff       (20)        0 2023-05-31 05:07:40.000000 auth_package-1.1/auth_package/
+-rw-r--r--   0 raminzamani   (501) staff       (20)     1793 2023-05-31 05:04:37.000000 auth_package-1.1/auth_package/user.py
+-rw-r--r--   0 raminzamani   (501) staff       (20)     2938 2023-05-31 05:03:43.000000 auth_package-1.1/auth_package/permission.py
+-rw-r--r--   0 raminzamani   (501) staff       (20)      233 2023-05-29 19:39:45.000000 auth_package-1.1/auth_package/__init__.py
+-rw-r--r--   0 raminzamani   (501) staff       (20)       39 2023-05-29 19:53:39.000000 auth_package-1.1/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `auth_package-1.0/PKG-INFO` & `auth_package-1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: auth_package
-Version: 1.0
+Version: 1.1
 Summary: Auth package for authentication with microservices
 Home-page: https://www.ramzamani.com/
-Download-URL: https://github.com/zamaniramin549/auth_project_package/archive/refs/tags/1.0.tar.gz
 Author: Ramin Zamanighiri
 Author-email: zamaniramin549@gmail.com
 License: mit
+Download-URL: https://github.com/zamaniramin549/auth_project_package/archive/refs/tags/1.1.tar.gz
+Description: UNKNOWN
 Keywords: microservices,Auth package,API
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-License-File: LICENSE.txt
```

### Comparing `auth_package-1.0/auth_package/permission.py` & `auth_package-1.1/auth_package/permission.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import requests
 import json
 
+base_url = 'http://authpackage.pythonanywhere.com'
+
 
 
 def permission_list(api_key:str):
 
-    url = "http://localhost:8000/user-api-permission-name"
+    url = f"{base_url}/user-api-permission-name"
 
     payload = {}
     headers = {
         'api-key': api_key
     }
 
     response = requests.request("GET", url, headers=headers, data=payload)
 
     return response.json()
 
 
 def permission(permission_name:int, api_key:str):
-    url = "http://localhost:8000/user-api-permission-name/"
+    url = f"{base_url}/user-api-permission-name/"
     payload = json.dumps({
         "permission_name": permission_name
     })
     headers = {
         'api-key': api_key,
         'Content-Type': 'application/json'
     }
@@ -35,15 +37,15 @@
         user_id:int, 
         read_permission:bool, 
         write_permission:bool, 
         edit_permission:bool, 
         delete_permission:bool,
         api_key:str
     ):
-    url = "http://localhost:8000/user-api-permission/"
+    url = f"{base_url}/user-api-permission/"
 
     payload = json.dumps({
         "permission_id": int(permission_id),
         "user_id": int(user_id),
         "read_permission": read_permission,
         "write_permission": write_permission,
         "edit_permission": edit_permission,
@@ -64,15 +66,15 @@
         read_permission:bool, 
         write_permission:bool, 
         edit_permission:bool, 
         delete_permission:bool,
         api_key:str
         ):
 
-    url = f"http://localhost:8000/edit-user-permission/{permission_id}/"
+    url = f"{base_url}/edit-user-permission/{permission_id}/"
 
     payload = json.dumps({
         "read_permission": read_permission,
         "write_permission": write_permission,
         "edit_permission": edit_permission,
         "delete_permission": delete_permission
     })
@@ -83,15 +85,15 @@
 
     response = requests.request("PUT", url, headers=headers, data=payload)
 
     return response.json()
 
 
 def delete_user_permission(permission_id:int, api_key:str):
-    url = "http://localhost:8000/delete-user-permission/"
+    url = f"{base_url}/delete-user-permission/"
 
     payload = json.dumps({
         "user_permission_id": permission_id
     })
     headers = {
         'api-key': api_key,
         'Content-Type': 'application/json'
@@ -99,15 +101,15 @@
 
     response = requests.request("DELETE", url, headers=headers, data=payload)
 
     return response.json()
 
 
 def delete_permission(permission_id:int, api_key:str):
-    url = "http://localhost:8000/delete-permission/"
+    url = f"{base_url}/delete-permission/"
 
     payload = json.dumps({
         "permission_id": permission_id
     })
     headers = {
         'api-key': api_key,
         'Content-Type': 'application/json'
```

### Comparing `auth_package-1.0/auth_package/user.py` & `auth_package-1.1/auth_package/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import requests
 import json
-
+base_url = 'http://authpackage.pythonanywhere.com'
 
 def create_user(email:str, first_name:str, last_name:str, password:str, api_key:str):
 
-    url = "http://localhost:8000/user-api/"
+    url = f"{base_url}/user-api/"
 
     payload = json.dumps({
         "email": email,
         "first_name": first_name,
         "last_name": last_name,
         "password": password
     })
@@ -19,43 +19,43 @@
 
     response = requests.request("POST", url, headers=headers, data=payload)
     return response.json()
 
 
 def user_list(api_key:str):
 
-    url = "http://localhost:8000/user-api/"
+    url = f"{base_url}/user-api/"
 
     payload = {}
     headers = {
         'api-key': api_key
     }
 
     response = requests.request("GET", url, headers=headers, data=payload)
 
     return response.json()
 
 
 def get_single_user(user_id:int, api_key:str):
 
-    url = f"http://localhost:8000/user-api/{user_id}/"
+    url = f"{base_url}/user-api/{user_id}/"
 
     payload = {}
     headers = {
         'api-key': api_key
     }
 
     response = requests.request("GET", url, headers=headers, data=payload)
 
     return response.json()
 
 
 def delete_user(user_id:int, api_key:str):
  
-    url = "http://localhost:8000/delete-user/"
+    url = f"{base_url}/delete-user/"
 
     payload = json.dumps({
         "user_id": user_id
     })
     headers = {
         'api-key': api_key,
         'Content-Type': 'application/json'
@@ -63,15 +63,15 @@
 
     response = requests.request("DELETE", url, headers=headers, data=payload)
 
     return response.json()
 
 
 def authenticate_user(email:str, password:str, api_key:str):
-    url = "http://localhost:8000/authenticate-user/"
+    url = f"{base_url}/authenticate-user/"
 
     payload = json.dumps({
         "email": email,
         "password": password
     })
     headers = {
         'api-key': api_key,
```

### Comparing `auth_package-1.0/setup.py` & `auth_package-1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'auth_package',         # How you named your package folder (MyLib)
   packages = ['auth_package'],   # Chose the same as "name"
-  version = '1.0',      # Start with a small number and increase it with every change you make
+  version = '1.1',      # Start with a small number and increase it with every change you make
   license='mit',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Auth package for authentication with microservices',   # Give a short description about your library
   author = 'Ramin Zamanighiri',                   # Type in your name
   author_email = 'zamaniramin549@gmail.com',      # Type in your E-Mail
   url = 'https://www.ramzamani.com/',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/zamaniramin549/auth_project_package/archive/refs/tags/1.0.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/zamaniramin549/auth_project_package/archive/refs/tags/1.1.tar.gz',    # I explain this later on
   keywords = ['microservices', 'Auth package', 'API'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'requests',
       ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
```

