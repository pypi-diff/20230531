# Comparing `tmp/edge_addons_api-0.3.1.tar.gz` & `tmp/edge_addons_api-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge_addons_api-0.3.1.tar", max compression
+gzip compressed data, was "edge_addons_api-0.3.2.tar", max compression
```

## Comparing `edge_addons_api-0.3.1.tar` & `edge_addons_api-0.3.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1089 2023-05-27 06:58:29.715550 edge_addons_api-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-05-27 06:58:29.715550 edge_addons_api-0.3.1/edge_addons_api/__init__.py
--rw-r--r--   0        0        0     4435 2023-05-27 06:58:29.715550 edge_addons_api-0.3.1/edge_addons_api/client.py
--rw-r--r--   0        0        0      272 2023-05-27 06:58:29.715550 edge_addons_api-0.3.1/edge_addons_api/exceptions.py
--rw-r--r--   0        0        0      496 2023-05-27 06:58:29.715550 edge_addons_api-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 edge_addons_api-0.3.1/setup.py
--rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 edge_addons_api-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-05-31 20:54:31.854313 edge_addons_api-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 20:54:31.854313 edge_addons_api-0.3.2/edge_addons_api/__init__.py
+-rw-r--r--   0        0        0     4745 2023-05-31 20:54:31.854313 edge_addons_api-0.3.2/edge_addons_api/client.py
+-rw-r--r--   0        0        0      272 2023-05-31 20:54:31.854313 edge_addons_api-0.3.2/edge_addons_api/exceptions.py
+-rw-r--r--   0        0        0      496 2023-05-31 20:54:31.854313 edge_addons_api-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 edge_addons_api-0.3.2/PKG-INFO
```

### Comparing `edge_addons_api-0.3.1/README.md` & `edge_addons_api-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `edge_addons_api-0.3.1/edge_addons_api/client.py` & `edge_addons_api-0.3.2/edge_addons_api/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     product_id: str
     client_id: str
     client_secret: str
     access_token_url: str
 
 
 class Client:
-
     BASE_URL = "https://api.addons.microsoftedge.microsoft.com"
 
     def __init__(self, options: Options):
         self.options = options
 
     def submit(self, file_path: str, notes: str) -> str:
         if not path.exists(file_path):
@@ -37,26 +36,30 @@
 
         access_token = self._get_access_token()
         operation_id = self._upload(file_path, access_token)
         self._check_upload(operation_id, access_token)
         return self._publish(notes, access_token)
 
     def fetch_publish_status(self, operation_id: str) -> dict:
+        logger.debug(f"Fetching publish status for {operation_id}")
         access_token = self._get_access_token()
         response = requests.get(
             self._publish_status_endpoint(operation_id),
             headers={
                 "Authorization": f"Bearer {access_token}",
             },
         )
 
         response.raise_for_status()
+
+        logger.debug(f"Publish status response: {response.content.decode()}")
         return response.json()
 
     def _publish(self, notes: str, access_token: str) -> str:
+        logger.debug("Publishing")
         response = requests.post(
             self._publish_endpoint(),
             data={"notes": notes},
             headers={
                 "Authorization": f"Bearer {access_token}",
             },
         )
@@ -64,35 +67,40 @@
         response.raise_for_status()
 
         logger.debug(f"Publish response: {response.content.decode()}")
 
         return response.headers["Location"]
 
     def _upload(self, file_path: str, access_token: str) -> str:
+        logger.debug(f"Uploading {file_path}")
         with open(file_path, "rb") as f:
             response = requests.post(
                 self._upload_endpoint(),
                 data=f,
                 headers={
                     "Authorization": f"Bearer {access_token}",
                     "Content-Type": "application/zip",
                 },
             )
 
         response.raise_for_status()
 
+        logger.debug("Finished upload")
+
         return response.headers["Location"]
 
     def _check_upload(
         self,
         operation_id,
         access_token: str,
         retry_count: int = 5,
         sleep_seconds: int = 3,
     ) -> str:
+        logger.debug("Checking upload")
+
         upload_status = ""
         attempts = 0
 
         while upload_status != ResponseStatus.SUCCEEDED and attempts < retry_count:
             response = requests.get(
                 self._status_endpoint(operation_id),
                 headers={
```

### Comparing `edge_addons_api-0.3.1/PKG-INFO` & `edge_addons_api-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-addons-api
-Version: 0.3.1
+Version: 0.3.2
 Summary: API client for uploading addons to the Edge store
 License: MIT
 Author: Malachi Soord
 Author-email: inverse.chi@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

