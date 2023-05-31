# Comparing `tmp/ploomes-api-client-0.1.3.tar.gz` & `tmp/ploomes-api-client-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ploomes-api-client-0.1.3.tar", last modified: Tue May 30 15:36:34 2023, max compression
+gzip compressed data, was "ploomes-api-client-0.1.5.tar", last modified: Wed May 31 19:32:35 2023, max compression
```

## Comparing `ploomes-api-client-0.1.3.tar` & `ploomes-api-client-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-30 15:36:34.776379 ploomes-api-client-0.1.3/
--rw-r--r--   0 filterfeed   (501) staff       (20)     1072 2023-05-25 21:00:11.000000 ploomes-api-client-0.1.3/LICENSE
--rw-r--r--   0 filterfeed   (501) staff       (20)     2275 2023-05-30 15:36:34.776217 ploomes-api-client-0.1.3/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)     1137 2023-05-26 14:13:51.000000 ploomes-api-client-0.1.3/README.md
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-30 15:36:34.775336 ploomes-api-client-0.1.3/ploomes_api_client.egg-info/
--rw-r--r--   0 filterfeed   (501) staff       (20)     2275 2023-05-30 15:36:34.000000 ploomes-api-client-0.1.3/ploomes_api_client.egg-info/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)      295 2023-05-30 15:36:34.000000 ploomes-api-client-0.1.3/ploomes_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-05-30 15:36:34.000000 ploomes-api-client-0.1.3/ploomes_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       26 2023-05-30 15:36:34.000000 ploomes-api-client-0.1.3/ploomes_api_client.egg-info/requires.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       15 2023-05-30 15:36:34.000000 ploomes-api-client-0.1.3/ploomes_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-30 15:36:34.775660 ploomes-api-client-0.1.3/ploomes_client/
--rw-r--r--   0 filterfeed   (501) staff       (20)       43 2023-05-26 18:47:42.000000 ploomes-api-client-0.1.3/ploomes_client/__init__.py
--rw-r--r--   0 filterfeed   (501) staff       (20)    22837 2023-05-30 15:35:09.000000 ploomes-api-client-0.1.3/ploomes_client/ploomes_client.py
--rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-05-30 15:36:34.776435 ploomes-api-client-0.1.3/setup.cfg
--rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-05-30 15:36:33.000000 ploomes-api-client-0.1.3/setup.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-31 19:32:35.965228 ploomes-api-client-0.1.5/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1072 2023-05-25 21:00:11.000000 ploomes-api-client-0.1.5/LICENSE
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2275 2023-05-31 19:32:35.965070 ploomes-api-client-0.1.5/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1137 2023-05-26 14:13:51.000000 ploomes-api-client-0.1.5/README.md
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-31 19:32:35.964264 ploomes-api-client-0.1.5/ploomes_api_client.egg-info/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2275 2023-05-31 19:32:35.000000 ploomes-api-client-0.1.5/ploomes_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)      295 2023-05-31 19:32:35.000000 ploomes-api-client-0.1.5/ploomes_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-05-31 19:32:35.000000 ploomes-api-client-0.1.5/ploomes_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       26 2023-05-31 19:32:35.000000 ploomes-api-client-0.1.5/ploomes_api_client.egg-info/requires.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       15 2023-05-31 19:32:35.000000 ploomes-api-client-0.1.5/ploomes_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-31 19:32:35.964498 ploomes-api-client-0.1.5/ploomes_client/
+-rw-r--r--   0 filterfeed   (501) staff       (20)       43 2023-05-26 18:47:42.000000 ploomes-api-client-0.1.5/ploomes_client/__init__.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)    24681 2023-05-31 19:31:38.000000 ploomes-api-client-0.1.5/ploomes_client/ploomes_client.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-05-31 19:32:35.965283 ploomes-api-client-0.1.5/setup.cfg
+-rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-05-31 19:32:32.000000 ploomes-api-client-0.1.5/setup.py
```

### Comparing `ploomes-api-client-0.1.3/LICENSE` & `ploomes-api-client-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.1.3/PKG-INFO` & `ploomes-api-client-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ploomes-api-client
-Version: 0.1.3
+Version: 0.1.5
 Summary: Python client for the Ploomes API
 Home-page: https://github.com/victorfigueredo/ploomes-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
 Description: # Ploomes API Python Client
```

### Comparing `ploomes-api-client-0.1.3/README.md` & `ploomes-api-client-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.1.3/ploomes_api_client.egg-info/PKG-INFO` & `ploomes-api-client-0.1.5/ploomes_api_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ploomes-api-client
-Version: 0.1.3
+Version: 0.1.5
 Summary: Python client for the Ploomes API
 Home-page: https://github.com/victorfigueredo/ploomes-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
 Description: # Ploomes API Python Client
```

### Comparing `ploomes-api-client-0.1.3/ploomes_client/ploomes_client.py` & `ploomes-api-client-0.1.5/ploomes_client/ploomes_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     def __init__(self, api_key) -> None:
         self.host = "https://public-api2.ploomes.com"
         self.api_key = api_key
         self.headers = {"User-Key": api_key,
                         "Content-Type": "application/json"}
 
     def retry(func):
-        MAX_RETRIES = 1  # maximum number of retries
+        MAX_RETRIES = 3  # maximum number of retries
         TIMEOUT = 5  # time to wait before retrying (in seconds)
 
         def wrapper(*args, **kwargs):
             retries = 0  # current number of retries
 
             while retries < MAX_RETRIES:
                 try:
@@ -50,14 +50,76 @@
     def get_user_account(self):
         r = requests.get(f"{self.host}/Account", headers=self.headers)
         if r.status_code == 401:
             return None
         response = r.json()
         return response
 
+
+
+    @retry
+    @sleep_and_retry
+    @limits(calls=MAX_REQUESTS_PER_SECOND, period=1)
+    def get_contact_products(self, filter=None):
+        if filter:
+            filter = f"?$filter={filter}"
+        r = requests.get(
+            f"{self.host}/Contacts@Products{filter}", headers=self.headers
+        )
+        response = r.json().get("value")
+        return response
+
+    @retry
+    @sleep_and_retry
+    @limits(calls=MAX_REQUESTS_PER_SECOND, period=1)
+    def update_contact_product(self, id_, fields):
+        payload = json.dumps(fields)
+        r = requests.patch(
+            f"{self.host}/Contacts@Products({id_})?$expand=OtherProperties", data=payload, headers=self.headers
+        )
+        response = r.json()
+        return response
+
+    @retry
+    @sleep_and_retry
+    @limits(calls=MAX_REQUESTS_PER_SECOND, period=1)
+    def post_contact_product(self, fields):
+        payload = json.dumps(fields)
+        r = requests.post(
+            f"{self.host}/Contacts@Products", data=payload, headers=self.headers
+        )
+        response = r.json()
+        return response
+
+    @retry
+    @sleep_and_retry
+    @limits(calls=MAX_REQUESTS_PER_SECOND, period=1)
+    def get_products(self, _filter: Optional[str] = None, top: int = 1000, orderby: Optional[str] = None) -> List[Dict]:
+        url = f"{self.host}/Products?$expand=OtherProperties"
+
+        if _filter:
+            url += f"&$filter={_filter}"
+        
+        if top:
+            url += f"&$top={top}"
+        
+        if orderby:
+            url += f"&$orderby={orderby}"
+
+        print(url)
+        r = requests.get(url, headers=self.headers)
+
+        print(f"Response status code: {r.status_code}")  # print status code
+        print(f"Response content: {r.content}")  # print response content
+
+        response = r.json()
+
+        return response.get("value", [])
+
+
     @retry
     @sleep_and_retry
     @limits(calls=MAX_REQUESTS_PER_SECOND, period=1)
     def get_user_info(self, filter=None):
         url = f"{self.host}/Users?"
         if filter:
             url += f"$filter={filter}"
```

### Comparing `ploomes-api-client-0.1.3/setup.py` & `ploomes-api-client-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ploomes-api-client',
-    version='0.1.3',
+    version='0.1.5',
     packages=find_packages(),   
     url='https://github.com/victorfigueredo/ploomes-api-client',
     author='Victor Figueredo',
     author_email='cto@filterfeed.com.br',
     description='Python client for the Ploomes API',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

