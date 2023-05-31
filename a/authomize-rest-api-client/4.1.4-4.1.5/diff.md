# Comparing `tmp/authomize-rest-api-client-4.1.4.tar.gz` & `tmp/authomize-rest-api-client-4.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-4.1.4.tar", last modified: Tue May 30 14:06:16 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-4.1.5.tar", last modified: Wed May 31 13:11:24 2023, max compression
```

## Comparing `authomize-rest-api-client-4.1.4.tar` & `authomize-rest-api-client-4.1.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.251852 authomize-rest-api-client-4.1.4/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-05-30 14:06:16.251852 authomize-rest-api-client-4.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2194 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.247852 authomize-rest-api-client-4.1.4/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.247852 authomize-rest-api-client-4.1.4/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.247852 authomize-rest-api-client-4.1.4/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2538 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10358 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    13027 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.247852 authomize-rest-api-client-4.1.4/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.247852 authomize-rest-api-client-4.1.4/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.247852 authomize-rest-api-client-4.1.4/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75246 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.247852 authomize-rest-api-client-4.1.4/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37380 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.247852 authomize-rest-api-client-4.1.4/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.247852 authomize-rest-api-client-4.1.4/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   189364 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.251852 authomize-rest-api-client-4.1.4/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89370 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-30 14:05:55.000000 authomize-rest-api-client-4.1.4/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:06:16.251852 authomize-rest-api-client-4.1.4/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-05-30 14:06:16.000000 authomize-rest-api-client-4.1.4/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1356 2023-05-30 14:06:16.000000 authomize-rest-api-client-4.1.4/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 14:06:16.000000 authomize-rest-api-client-4.1.4/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-30 14:06:16.000000 authomize-rest-api-client-4.1.4/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-30 14:06:16.000000 authomize-rest-api-client-4.1.4/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-05-30 14:06:16.251852 authomize-rest-api-client-4.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1161 2023-05-30 14:05:58.000000 authomize-rest-api-client-4.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2194 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.742829 authomize-rest-api-client-4.1.5/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2538 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10358 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    13027 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    84288 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37380 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   200259 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89370 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-31 13:11:04.000000 authomize-rest-api-client-4.1.5/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-05-31 13:11:24.000000 authomize-rest-api-client-4.1.5/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-05-31 13:11:24.000000 authomize-rest-api-client-4.1.5/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 13:11:24.000000 authomize-rest-api-client-4.1.5/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      214 2023-05-31 13:11:24.000000 authomize-rest-api-client-4.1.5/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-31 13:11:24.000000 authomize-rest-api-client-4.1.5/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-05-31 13:11:24.746829 authomize-rest-api-client-4.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-05-31 13:11:08.000000 authomize-rest-api-client-4.1.5/setup.py
```

### Comparing `authomize-rest-api-client-4.1.4/LICENSE.txt` & `authomize-rest-api-client-4.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.4/README.md` & `authomize-rest-api-client-4.1.5/README.md`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.4/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-4.1.5/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.4/authomize/rest_api_client/client/base_client.py` & `authomize-rest-api-client-4.1.5/authomize/rest_api_client/client/base_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.4/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-4.1.5/authomize/rest_api_client/client/client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.4/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-4.1.5/authomize/rest_api_client/client/connectors_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.4/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-4.1.5/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.4/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-4.1.5/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2023-05-30T13:55:35+00:00
+#   timestamp: 2023-05-31T12:40:10+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional
 
@@ -250,14 +250,19 @@
     )
     data: Optional[NewAccountsAssociationResponseDataSchema] = Field(
         default={}, description='Response data.', title='Data'
     )
 
 
 class NewAccountsAssociationsListRequestSchema(BaseModel):
+    workflowId: Optional[str] = Field(
+        default='default',
+        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
+        title='Workflowid',
+    )
     data: List[NewAccountsAssociationRequestSchema] = Field(
         ...,
         description='New Accounts Associations',
         max_items=10000,
         min_items=1,
         title='Data',
     )
@@ -327,14 +332,19 @@
     )
     tags: Optional[List[constr(min_length=1)]] = Field(
         default=None, description='Tags associated with the asset.\n', title='Tags'
     )
 
 
 class NewAssetsInheritanceListRequestSchema(BaseModel):
+    workflowId: Optional[str] = Field(
+        default='default',
+        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
+        title='Workflowid',
+    )
     data: List[NewAssetInheritanceRequestSchema] = Field(
         ...,
         description='New Assets Inheritance',
         max_items=10000,
         min_items=1,
         title='Data',
     )
@@ -378,14 +388,19 @@
     )
     data: Optional[NewAssetsInheritanceResponseDataSchema] = Field(
         default={}, description='Response data.', title='Data'
     )
 
 
 class NewAssetsListRequestSchema(BaseModel):
+    workflowId: Optional[str] = Field(
+        default='default',
+        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
+        title='Workflowid',
+    )
     data: List[NewAssetRequestSchema] = Field(
         ..., description='New Assets', max_items=10000, min_items=1, title='Data'
     )
     validateOnly: Optional[bool] = Field(
         default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validateonly',
@@ -534,14 +549,19 @@
     )
     data: Optional[NewGroupingsAssociationResponseDataSchema] = Field(
         default={}, description='Response data.', title='Data'
     )
 
 
 class NewGroupingsAssociationsListRequestSchema(BaseModel):
+    workflowId: Optional[str] = Field(
+        default='default',
+        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
+        title='Workflowid',
+    )
     data: List[NewGroupingsAssociationRequestSchema] = Field(
         ...,
         description='New Groupings Associations',
         max_items=10000,
         min_items=1,
         title='Data',
     )
@@ -549,14 +569,19 @@
         default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validateonly',
     )
 
 
 class NewGroupingsListRequestSchema(BaseModel):
+    workflowId: Optional[str] = Field(
+        default='default',
+        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
+        title='Workflowid',
+    )
     data: List[NewGroupingRequestSchema] = Field(
         ..., description='New Groupings', max_items=10000, min_items=1, title='Data'
     )
     validateOnly: Optional[bool] = Field(
         default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validate Only\n',
@@ -672,14 +697,19 @@
     )
     data: Optional[NewPrivilegeGrantsResponseDataSchema] = Field(
         default={}, description='Response data.', title='Data'
     )
 
 
 class NewPrivilegesGrantsListRequestSchema(BaseModel):
+    workflowId: Optional[str] = Field(
+        default='default',
+        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
+        title='Workflowid',
+    )
     data: List[NewPrivilegeGrantsRequestSchema] = Field(
         ...,
         description='New Privileges Grants',
         max_items=10000,
         min_items=1,
         title='Data',
     )
@@ -897,14 +927,19 @@
     )
     tags: Optional[List[constr(min_length=1)]] = Field(
         default=None, description='Tags associated with the asset.\n', title='Tags'
     )
 
 
 class UpdateAssetsListRequestSchema(BaseModel):
+    workflowId: Optional[str] = Field(
+        default='default',
+        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
+        title='Workflowid',
+    )
     data: List[UpdateAssetRequestSchema] = Field(
         ..., description='Update Assets', max_items=10000, min_items=1, title='Data'
     )
 
 
 class UpdateGroupingsRequestSchema(BaseModel):
     uniqueId: constr(min_length=1) = Field(
@@ -988,14 +1023,19 @@
         default=None,
         description='The privilege name in the source system.',
         title='Originname',
     )
 
 
 class UpdatePrivilegesListRequestSchema(BaseModel):
+    workflowId: Optional[str] = Field(
+        default='default',
+        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
+        title='Workflowid',
+    )
     data: List[UpdatePrivilegeRequestSchema] = Field(
         ..., description='Update Privileges', max_items=10000, min_items=1, title='Data'
     )
 
 
 class UserStatus(Enum):
     Staged = 'Staged'
@@ -1372,14 +1412,19 @@
         default=False,
         description="If `true`, it's possible to perform a privilege escalation using the permission.   \nexample: User has Read access to a secret containing credentials of another user.  This allows \nprivilege escalation.\nopposite example: User has Read metadata permission to a secret containing credentials of another user. This *Does NOT* allows \nprivilege escalation.\n\n",
         title='Escalationpathpossible',
     )
 
 
 class NewPermissionsListRequestSchema(BaseModel):
+    workflowId: Optional[str] = Field(
+        default='default',
+        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
+        title='Workflowid',
+    )
     data: List[NewPermissionRequestSchema] = Field(
         ..., description='New Permissions', max_items=10000, min_items=1, title='Data'
     )
     validateOnly: Optional[bool] = Field(
         default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validate Only\n',
@@ -1405,14 +1450,19 @@
         default=None,
         description='The privilege name in the source system.',
         title='Originname',
     )
 
 
 class NewPrivilegesListRequestSchema(BaseModel):
+    workflowId: Optional[str] = Field(
+        default='default',
+        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
+        title='Workflowid',
+    )
     data: List[NewPrivilegeRequestSchema] = Field(
         ..., description='New Privileges', max_items=10000, min_items=1, title='Data'
     )
     validateOnly: Optional[bool] = Field(
         default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validateonly',
@@ -1468,14 +1518,19 @@
         default=None,
         description='One or more tags on the user account.\n',
         title='Tags',
     )
 
 
 class NewUsersListRequestSchema(BaseModel):
+    workflowId: Optional[str] = Field(
+        default='default',
+        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
+        title='Workflowid',
+    )
     data: List[NewUserRequestSchema] = Field(
         ..., description='New Users', max_items=10000, min_items=1, title='Data'
     )
     validateOnly: Optional[bool] = Field(
         default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validateonly',
@@ -1536,14 +1591,19 @@
         default=None,
         description='The privilege name in the source system.',
         title='Originname',
     )
 
 
 class RequestsBundleSchema(BaseModel):
+    workflow_id: Optional[str] = Field(
+        default='default',
+        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
+        title='Workflow Id',
+    )
     delete_app_data: Optional[bool] = Field(
         default=False,
         description='The Delete Application Data API is used to delete app data by `{appId}`.',
         title='Delete App Data',
     )
     createdAt: Optional[datetime] = Field(default=None, title='Createdat')
     new_users: Optional[List[NewUserRequestSchema]] = Field(
@@ -1634,14 +1694,19 @@
 
 class TransactionPaginatedSearchSchema(BaseModel):
     data: List[BundleTransactionSchema] = Field(..., title='Data')
     pagination: Pagination
 
 
 class UpdateGroupingsListRequestSchema(BaseModel):
+    workflowId: Optional[str] = Field(
+        default='default',
+        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
+        title='Workflowid',
+    )
     data: List[UpdateGroupingsRequestSchema] = Field(
         ...,
         description='List of update user requests.\n',
         max_items=10000,
         min_items=1,
         title='Data',
     )
@@ -1881,14 +1946,19 @@
         default=None,
         description='The Update Application Data API is used to update app data on `{appId}`.\n',
         title='App',
     )
 
 
 class NewIdentitiesListRequestSchema(BaseModel):
+    workflowId: Optional[str] = Field(
+        default='default',
+        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
+        title='Workflowid',
+    )
     data: List[NewIdentityRequestSchema] = Field(
         ..., description='New Identities', max_items=10000, min_items=1, title='Data'
     )
     validateOnly: Optional[bool] = Field(
         default=False,
         description='Validate the request without uploading the data into the system.',
         title='Validateonly',
@@ -1896,24 +1966,34 @@
 
 
 class SearchUsersListResponseSchema(BaseModel):
     data: List[UserSchema] = Field(..., description='Users', title='Data')
 
 
 class UpdateIdentitiesListRequestSchema(BaseModel):
+    workflowId: Optional[str] = Field(
+        default='default',
+        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
+        title='Workflowid',
+    )
     data: List[UpdateIdentityRequestSchema] = Field(
         ...,
         description='List of update identity requests.\n',
         max_items=10000,
         min_items=1,
         title='Data',
     )
 
 
 class UpdateUserListRequestSchema(BaseModel):
+    workflowId: Optional[str] = Field(
+        default='default',
+        description='The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n',
+        title='Workflowid',
+    )
     data: List[UpdateUserRequestSchema] = Field(
         ...,
         description='List of update user requests.\n',
         max_items=10000,
         min_items=1,
         title='Data',
     )
```

### Comparing `authomize-rest-api-client-4.1.4/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-4.1.5/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.4/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-4.1.5/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.987375785792865%*

 * *Differences: {"'components'": "{'schemas': {'NewAccountsAssociationsListRequestSchema': {'properties': "*

 * *                 "{'workflowId': OrderedDict([('title', 'Workflowid'), ('type', 'string'), "*

 * *                 "('description', 'The `workflowId` parameter can be use to allow an app to run as "*

 * *                 'a set of multiple, different workflows with different configurations.\\n\\nOnce '*

 * *                 'the data was uploaded using a certain `workflowId`, all other requests, '*

 * *                 'referring to the […]*

```diff
@@ -1131,14 +1131,20 @@
                         "type": "array"
                     },
                     "validateOnly": {
                         "default": false,
                         "description": "Validate the request without uploading the data into the system.",
                         "title": "Validateonly",
                         "type": "boolean"
+                    },
+                    "workflowId": {
+                        "default": "default",
+                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
+                        "title": "Workflowid",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NewAccountsAssociationsListRequestSchema",
                 "type": "object"
@@ -1259,14 +1265,20 @@
                         "type": "array"
                     },
                     "validateOnly": {
                         "default": false,
                         "description": "Validate the request without uploading the data into the system.",
                         "title": "Validateonly",
                         "type": "boolean"
+                    },
+                    "workflowId": {
+                        "default": "default",
+                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
+                        "title": "Workflowid",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NewAssetsInheritanceListRequestSchema",
                 "type": "object"
@@ -1367,14 +1379,20 @@
                         "type": "array"
                     },
                     "validateOnly": {
                         "default": false,
                         "description": "Validate the request without uploading the data into the system.",
                         "title": "Validateonly",
                         "type": "boolean"
+                    },
+                    "workflowId": {
+                        "default": "default",
+                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
+                        "title": "Workflowid",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NewAssetsListRequestSchema",
                 "type": "object"
@@ -1673,14 +1691,20 @@
                         "type": "array"
                     },
                     "validateOnly": {
                         "default": false,
                         "description": "Validate the request without uploading the data into the system.",
                         "title": "Validateonly",
                         "type": "boolean"
+                    },
+                    "workflowId": {
+                        "default": "default",
+                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
+                        "title": "Workflowid",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NewGroupingsAssociationsListRequestSchema",
                 "type": "object"
@@ -1699,14 +1723,20 @@
                         "type": "array"
                     },
                     "validateOnly": {
                         "default": false,
                         "description": "Validate the request without uploading the data into the system.",
                         "title": "Validate Only\n",
                         "type": "boolean"
+                    },
+                    "workflowId": {
+                        "default": "default",
+                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
+                        "title": "Workflowid",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NewGroupingsListRequestSchema",
                 "type": "object"
@@ -1725,14 +1755,20 @@
                         "type": "array"
                     },
                     "validateOnly": {
                         "default": false,
                         "description": "Validate the request without uploading the data into the system.",
                         "title": "Validateonly",
                         "type": "boolean"
+                    },
+                    "workflowId": {
+                        "default": "default",
+                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
+                        "title": "Workflowid",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NewIdentitiesListRequestSchema",
                 "type": "object"
@@ -1882,15 +1918,14 @@
                     "requestId",
                     "numberOfAcceptedEntities"
                 ],
                 "title": "NewIdentityResponseSchema",
                 "type": "object"
             },
             "NewPermissionRequestSchema": {
-                "description": "New permission request schema",
                 "properties": {
                     "assetId": {
                         "description": "The ID of the asset.\n\nWhen `null`, this is a global permission on the entire application (not just locally).",
                         "title": "Assetid",
                         "type": "string"
                     },
                     "escalationPathPossible": {
@@ -1957,14 +1992,20 @@
                         "type": "array"
                     },
                     "validateOnly": {
                         "default": false,
                         "description": "Validate the request without uploading the data into the system.",
                         "title": "Validate Only\n",
                         "type": "boolean"
+                    },
+                    "workflowId": {
+                        "default": "default",
+                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
+                        "title": "Workflowid",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NewPermissionsListRequestSchema",
                 "type": "object"
@@ -2242,14 +2283,20 @@
                         "type": "array"
                     },
                     "validateOnly": {
                         "default": false,
                         "description": "Validate the request without uploading the data into the system.",
                         "title": "Validateonly",
                         "type": "boolean"
+                    },
+                    "workflowId": {
+                        "default": "default",
+                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
+                        "title": "Workflowid",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NewPrivilegesGrantsListRequestSchema",
                 "type": "object"
@@ -2268,14 +2315,20 @@
                         "type": "array"
                     },
                     "validateOnly": {
                         "default": false,
                         "description": "Validate the request without uploading the data into the system.",
                         "title": "Validateonly",
                         "type": "boolean"
+                    },
+                    "workflowId": {
+                        "default": "default",
+                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
+                        "title": "Workflowid",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NewPrivilegesListRequestSchema",
                 "type": "object"
@@ -2457,14 +2510,20 @@
                         "type": "array"
                     },
                     "validateOnly": {
                         "default": false,
                         "description": "Validate the request without uploading the data into the system.",
                         "title": "Validateonly",
                         "type": "boolean"
+                    },
+                    "workflowId": {
+                        "default": "default",
+                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
+                        "title": "Workflowid",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "NewUsersListRequestSchema",
                 "type": "object"
@@ -2768,14 +2827,20 @@
                     "new_users": {
                         "description": "The Create Users APIs sets up App users(by App ID).",
                         "items": {
                             "$ref": "#/components/schemas/NewUserRequestSchema"
                         },
                         "title": "New Users",
                         "type": "array"
+                    },
+                    "workflow_id": {
+                        "default": "default",
+                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
+                        "title": "Workflow Id",
+                        "type": "string"
                     }
                 },
                 "title": "RequestsBundleSchema",
                 "type": "object"
             },
             "RestApiConnectorListSchema": {
                 "properties": {
@@ -3206,14 +3271,20 @@
                         "items": {
                             "$ref": "#/components/schemas/UpdateAssetRequestSchema"
                         },
                         "maxItems": 10000,
                         "minItems": 1,
                         "title": "Data",
                         "type": "array"
+                    },
+                    "workflowId": {
+                        "default": "default",
+                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
+                        "title": "Workflowid",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "UpdateAssetsListRequestSchema",
                 "type": "object"
@@ -3226,14 +3297,20 @@
                         "items": {
                             "$ref": "#/components/schemas/UpdateGroupingsRequestSchema"
                         },
                         "maxItems": 10000,
                         "minItems": 1,
                         "title": "Data",
                         "type": "array"
+                    },
+                    "workflowId": {
+                        "default": "default",
+                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
+                        "title": "Workflowid",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "UpdateGroupingsListRequestSchema",
                 "type": "object"
@@ -3353,14 +3430,20 @@
                         "items": {
                             "$ref": "#/components/schemas/UpdateIdentityRequestSchema"
                         },
                         "maxItems": 10000,
                         "minItems": 1,
                         "title": "Data",
                         "type": "array"
+                    },
+                    "workflowId": {
+                        "default": "default",
+                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
+                        "title": "Workflowid",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "UpdateIdentitiesListRequestSchema",
                 "type": "object"
@@ -3524,14 +3607,20 @@
                         "items": {
                             "$ref": "#/components/schemas/UpdatePrivilegeRequestSchema"
                         },
                         "maxItems": 10000,
                         "minItems": 1,
                         "title": "Data",
                         "type": "array"
+                    },
+                    "workflowId": {
+                        "default": "default",
+                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
+                        "title": "Workflowid",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "UpdatePrivilegesListRequestSchema",
                 "type": "object"
@@ -3544,14 +3633,20 @@
                         "items": {
                             "$ref": "#/components/schemas/UpdateUserRequestSchema"
                         },
                         "maxItems": 10000,
                         "minItems": 1,
                         "title": "Data",
                         "type": "array"
+                    },
+                    "workflowId": {
+                        "default": "default",
+                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
+                        "title": "Workflowid",
+                        "type": "string"
                     }
                 },
                 "required": [
                     "data"
                 ],
                 "title": "UpdateUserListRequestSchema",
                 "type": "object"
@@ -3764,15 +3859,15 @@
                 "type": "apiKey"
             }
         }
     },
     "info": {
         "description": "Authomize enables users to integrate your applications with Authomize via custom connectors.\n\nYou can use the APIs described in this document to create your connector.\n\nOnce data is uploaded and processed successfully, your custom connector will function in the same way as the connectors created by Authomize.\n\n## How does Authomize work?\nAuthomize works by gathering information about:\n\n\u00b7 individuals, teams and functions.\n\n\u00b7 apps, assets and accounts.\n\n\u00b7 all the relationships between them.\n\n![img.png](https://storagetry1.blob.core.windows.net/public/78d82650-71b0-4909-8444-022aab79add5.png)\n\n## Connector APIs\n\nAuthomize connector APIs enable pushing data into Authomize from external sources.\n\nThese APIs enable data extracted from outside applications (via application APIs) to be delivered to Authomize.\n\nA connector processes extracted application data to transform it into a format compatible with Authomize.\n\n![img_1.png](https://storagetry1.blob.core.windows.net/public/341bf6ef-2e5b-4284-b715-45105ffbf0f8.png)\n\n## Authentication\nTo Authenticate use the API Token, with the format: `Authorization: API_Token`.\n\nAn API Token is a token you provide when making API calls. \n\n\nThe API Token should be included in every request to the API in an `Authorization` header.\n```\ncurl -v -X POST \\n\n     -H \"Authorization: {API_Token}\" \\n\n     ...\n```\n\n## Limits\nRequests cannot exceed a size of 1MB.\n",
         "title": "Authomize API Reference",
-        "version": "4.1.3",
+        "version": "4.1.4",
         "x-logo": {
             "url": "https://static.authomize.com/public/icons/authomize-green.svg"
         }
     },
     "openapi": "3.0.2",
     "paths": {
         "/is_alive": {
@@ -5570,16 +5665,28 @@
                         "required": true,
                         "schema": {
                             "title": "Appid",
                             "type": "string"
                         }
                     },
                     {
+                        "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
+                        "in": "query",
+                        "name": "workflowId",
+                        "required": false,
+                        "schema": {
+                            "default": "default",
+                            "description": "The `workflowId` parameter can be use to allow an app to run as a set of multiple, different workflows with different configurations.\n\nOnce the data was uploaded using a certain `workflowId`, all other requests, referring to the same data using `GET`/`POST`/`PUT`/`DELETE`, should use the **same** `workflowId`.\n\n**Warning**, this parameter is an advanced feature and should be used with caution.\n\nThe **default** value is `default`.\n",
+                            "title": "Workflowid",
+                            "type": "string"
+                        }
+                    },
+                    {
                         "description": "Delete all the app data lastly updated before the given date.",
-                        "example": "2023-05-30T13:53:04.594383+00:00",
+                        "example": "2023-05-31T12:18:31.018274+00:00",
                         "in": "query",
                         "name": "modifiedBefore",
                         "required": false,
                         "schema": {
                             "description": "Delete all the app data lastly updated before the given date.",
                             "format": "date-time",
                             "title": "Modifiedbefore",
```

### Comparing `authomize-rest-api-client-4.1.4/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-4.1.5/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.4/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-4.1.5/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.1.4/setup.py` & `authomize-rest-api-client-4.1.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='4.1.4',
+        version='4.1.5',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
```

