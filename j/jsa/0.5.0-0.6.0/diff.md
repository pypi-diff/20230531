# Comparing `tmp/jsa-0.5.0.tar.gz` & `tmp/jsa-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsa-0.5.0.tar", max compression
+gzip compressed data, was "jsa-0.6.0.tar", max compression
```

## Comparing `jsa-0.5.0.tar` & `jsa-0.6.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0        5 2023-05-31 08:48:45.448903 jsa-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-05-31 08:47:30.991564 jsa-0.5.0/jsa/__init__.py
--rw-r--r--   0        0        0     2438 2023-05-31 08:47:44.244244 jsa-0.5.0/jsa/client/api_client.py
--rw-r--r--   0        0        0     2450 2023-05-31 08:47:44.243648 jsa-0.5.0/jsa/client/apis/apis_request_builder.py
--rw-r--r--   0        0        0     2347 2023-05-31 08:47:44.238767 jsa-0.5.0/jsa/client/apis/beta/acs/acs_request_builder.py
--rw-r--r--   0        0        0     4188 2023-05-31 08:47:44.237902 jsa-0.5.0/jsa/client/apis/beta/acs/v1/item/with_client_item_request_builder.py
--rw-r--r--   0        0        0     4909 2023-05-31 08:47:44.238366 jsa-0.5.0/jsa/client/apis/beta/acs/v1/v1_request_builder.py
--rw-r--r--   0        0        0     1596 2023-05-31 08:47:44.238987 jsa-0.5.0/jsa/client/apis/beta/beta_request_builder.py
--rw-r--r--   0        0        0     2307 2023-05-31 08:47:44.239263 jsa-0.5.0/jsa/client/apis/organizations/organizations_request_builder.py
--rw-r--r--   0        0        0     6794 2023-05-31 08:47:44.243070 jsa-0.5.0/jsa/client/apis/organizations/v1/item/authentication_policy/authentication_policy_request_builder.py
--rw-r--r--   0        0        0     1811 2023-05-31 08:47:44.242439 jsa-0.5.0/jsa/client/apis/organizations/v1/item/v1_item_request_builder.py
--rw-r--r--   0        0        0     1285 2023-05-31 08:47:44.243375 jsa-0.5.0/jsa/client/apis/organizations/v1/v1_request_builder.py
--rw-r--r--   0        0        0     2322 2023-05-31 08:47:44.232485 jsa-0.5.0/jsa/client/apis/service_accounts/service_accounts_request_builder.py
--rw-r--r--   0        0        0     4349 2023-05-31 08:47:44.236624 jsa-0.5.0/jsa/client/apis/service_accounts/v1/item/reset_secret/reset_secret_request_builder.py
--rw-r--r--   0        0        0     9985 2023-05-31 08:47:44.236119 jsa-0.5.0/jsa/client/apis/service_accounts/v1/item/v1_item_request_builder.py
--rw-r--r--   0        0        0     8123 2023-05-31 08:47:44.237294 jsa-0.5.0/jsa/client/apis/service_accounts/v1/v1_request_builder.py
--rw-r--r--   0        0        0     1109 2023-05-31 08:47:44.252201 jsa-0.5.0/jsa/client/kiota-lock.json
--rw-r--r--   0        0        0     4723 2023-05-31 08:47:44.227541 jsa-0.5.0/jsa/client/models/acs_client_request_data.py
--rw-r--r--   0        0        0     5331 2023-05-31 08:47:44.224667 jsa-0.5.0/jsa/client/models/acs_client_response_data.py
--rw-r--r--   0        0        0     3298 2023-05-31 08:47:44.227101 jsa-0.5.0/jsa/client/models/authentication_factors.py
--rw-r--r--   0        0        0     3813 2023-05-31 08:47:44.228829 jsa-0.5.0/jsa/client/models/authentication_policy.py
--rw-r--r--   0        0        0     3196 2023-05-31 08:47:44.227980 jsa-0.5.0/jsa/client/models/error.py
--rw-r--r--   0        0        0     3197 2023-05-31 08:47:44.223992 jsa-0.5.0/jsa/client/models/otp.py
--rw-r--r--   0        0        0     4579 2023-05-31 08:47:44.226192 jsa-0.5.0/jsa/client/models/red_hat_error_representation.py
--rw-r--r--   0        0        0      865 2023-05-31 08:47:44.226773 jsa-0.5.0/jsa/client/models/red_hat_error_representation_error.py
--rw-r--r--   0        0        0     4019 2023-05-31 08:47:44.229165 jsa-0.5.0/jsa/client/models/service_account_create_request_data.py
--rw-r--r--   0        0        0     7558 2023-05-31 08:47:44.229789 jsa-0.5.0/jsa/client/models/service_account_data.py
--rw-r--r--   0        0        0     3989 2023-05-31 08:47:44.230253 jsa-0.5.0/jsa/client/models/service_account_request_data.py
--rw-r--r--   0        0        0     5226 2023-05-31 08:47:44.228414 jsa-0.5.0/jsa/client/models/validation_exception_data.py
--rw-r--r--   0        0        0     2622 2023-05-31 08:47:44.222138 jsa-0.5.0/jsa/client/models/validation_exception_data_fields.py
--rw-r--r--   0        0        0      559 2023-05-31 08:46:07.159328 jsa-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 jsa-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0        5 2023-05-31 08:48:45.448903 jsa-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 08:47:30.991564 jsa-0.6.0/jsa/__init__.py
+-rw-r--r--   0        0        0     3455 2023-05-31 09:17:48.674569 jsa-0.6.0/jsa/client/__pycache__/service_account_client.cpython-311.pyc
+-rw-r--r--   0        0        0     2450 2023-05-31 09:09:22.362787 jsa-0.6.0/jsa/client/apis/apis_request_builder.py
+-rw-r--r--   0        0        0     2347 2023-05-31 09:09:22.367327 jsa-0.6.0/jsa/client/apis/beta/acs/acs_request_builder.py
+-rw-r--r--   0        0        0     4188 2023-05-31 09:09:22.365947 jsa-0.6.0/jsa/client/apis/beta/acs/v1/item/with_client_item_request_builder.py
+-rw-r--r--   0        0        0     4909 2023-05-31 09:09:22.366588 jsa-0.6.0/jsa/client/apis/beta/acs/v1/v1_request_builder.py
+-rw-r--r--   0        0        0     1596 2023-05-31 09:09:22.367574 jsa-0.6.0/jsa/client/apis/beta/beta_request_builder.py
+-rw-r--r--   0        0        0     2307 2023-05-31 09:09:22.367919 jsa-0.6.0/jsa/client/apis/organizations/organizations_request_builder.py
+-rw-r--r--   0        0        0     6794 2023-05-31 09:09:22.368755 jsa-0.6.0/jsa/client/apis/organizations/v1/item/authentication_policy/authentication_policy_request_builder.py
+-rw-r--r--   0        0        0     1811 2023-05-31 09:09:22.368213 jsa-0.6.0/jsa/client/apis/organizations/v1/item/v1_item_request_builder.py
+-rw-r--r--   0        0        0     1285 2023-05-31 09:09:22.369051 jsa-0.6.0/jsa/client/apis/organizations/v1/v1_request_builder.py
+-rw-r--r--   0        0        0     2322 2023-05-31 09:09:22.374400 jsa-0.6.0/jsa/client/apis/service_accounts/service_accounts_request_builder.py
+-rw-r--r--   0        0        0     4349 2023-05-31 09:09:22.369581 jsa-0.6.0/jsa/client/apis/service_accounts/v1/item/reset_secret/reset_secret_request_builder.py
+-rw-r--r--   0        0        0     9985 2023-05-31 09:09:22.373335 jsa-0.6.0/jsa/client/apis/service_accounts/v1/item/v1_item_request_builder.py
+-rw-r--r--   0        0        0     8123 2023-05-31 09:09:22.373995 jsa-0.6.0/jsa/client/apis/service_accounts/v1/v1_request_builder.py
+-rw-r--r--   0        0        0     1120 2023-05-31 09:09:22.401119 jsa-0.6.0/jsa/client/kiota-lock.json
+-rw-r--r--   0        0        0     4723 2023-05-31 09:09:22.358845 jsa-0.6.0/jsa/client/models/acs_client_request_data.py
+-rw-r--r--   0        0        0     5331 2023-05-31 09:09:22.357841 jsa-0.6.0/jsa/client/models/acs_client_response_data.py
+-rw-r--r--   0        0        0     3298 2023-05-31 09:09:22.353633 jsa-0.6.0/jsa/client/models/authentication_factors.py
+-rw-r--r--   0        0        0     3813 2023-05-31 09:09:22.359323 jsa-0.6.0/jsa/client/models/authentication_policy.py
+-rw-r--r--   0        0        0     3196 2023-05-31 09:09:22.356916 jsa-0.6.0/jsa/client/models/error.py
+-rw-r--r--   0        0        0     3197 2023-05-31 09:09:22.359665 jsa-0.6.0/jsa/client/models/otp.py
+-rw-r--r--   0        0        0     4579 2023-05-31 09:09:22.360119 jsa-0.6.0/jsa/client/models/red_hat_error_representation.py
+-rw-r--r--   0        0        0      865 2023-05-31 09:09:22.355016 jsa-0.6.0/jsa/client/models/red_hat_error_representation_error.py
+-rw-r--r--   0        0        0     4019 2023-05-31 09:09:22.358281 jsa-0.6.0/jsa/client/models/service_account_create_request_data.py
+-rw-r--r--   0        0        0     7558 2023-05-31 09:09:22.356493 jsa-0.6.0/jsa/client/models/service_account_data.py
+-rw-r--r--   0        0        0     3989 2023-05-31 09:09:22.355622 jsa-0.6.0/jsa/client/models/service_account_request_data.py
+-rw-r--r--   0        0        0     5226 2023-05-31 09:09:22.357311 jsa-0.6.0/jsa/client/models/validation_exception_data.py
+-rw-r--r--   0        0        0     2622 2023-05-31 09:09:22.355903 jsa-0.6.0/jsa/client/models/validation_exception_data_fields.py
+-rw-r--r--   0        0        0     2460 2023-05-31 09:09:22.361472 jsa-0.6.0/jsa/client/service_account_client.py
+-rw-r--r--   0        0        0      666 2023-05-31 09:18:13.436999 jsa-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 jsa-0.6.0/PKG-INFO
```

### Comparing `jsa-0.5.0/jsa/client/api_client.py` & `jsa-0.6.0/jsa/client/service_account_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from kiota_serialization_text.text_parse_node_factory import TextParseNodeFactory
 from kiota_serialization_text.text_serialization_writer_factory import TextSerializationWriterFactory
 from typing import Any, Callable, Dict, List, Optional, TYPE_CHECKING, Union
 
 if TYPE_CHECKING:
     from .apis import apis_request_builder
 
-class ApiClient():
+class ServiceAccountClient():
     """
     The main entry point of the SDK, exposes the configuration and the fluent API.
     """
     def __init__(self,request_adapter: RequestAdapter) -> None:
         """
-        Instantiates a new ApiClient and sets the default values.
+        Instantiates a new ServiceAccountClient and sets the default values.
         Args:
             requestAdapter: The request adapter to use to execute the requests.
         """
         if request_adapter is None:
             raise Exception("request_adapter cannot be undefined")
         # Path parameters for the request
         self.path_parameters: Dict[str, Any] = {}
```

### Comparing `jsa-0.5.0/jsa/client/apis/apis_request_builder.py` & `jsa-0.6.0/jsa/client/apis/apis_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.5.0/jsa/client/apis/beta/acs/acs_request_builder.py` & `jsa-0.6.0/jsa/client/apis/beta/acs/acs_request_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
         url_tpl_params = get_path_parameters(path_parameters)
         self.path_parameters = url_tpl_params
         self.request_adapter = request_adapter
     
     def v1_by_id(self,id: str) -> with_client_item_request_builder.WithClientItemRequestBuilder:
         """
-        Gets an item from the ApiSdk.apis.beta.acs.v1.item collection
+        Gets an item from the client.apis.beta.acs.v1.item collection
         Args:
             id: Unique identifier of the item
         Returns: with_client_item_request_builder.WithClientItemRequestBuilder
         """
         if id is None:
             raise Exception("id cannot be undefined")
         from .v1.item import with_client_item_request_builder
```

### Comparing `jsa-0.5.0/jsa/client/apis/beta/acs/v1/item/with_client_item_request_builder.py` & `jsa-0.6.0/jsa/client/apis/beta/acs/v1/item/with_client_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.5.0/jsa/client/apis/beta/acs/v1/v1_request_builder.py` & `jsa-0.6.0/jsa/client/apis/beta/acs/v1/v1_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.5.0/jsa/client/apis/beta/beta_request_builder.py` & `jsa-0.6.0/jsa/client/apis/beta/beta_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.5.0/jsa/client/apis/organizations/organizations_request_builder.py` & `jsa-0.6.0/jsa/client/apis/organizations/organizations_request_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
         url_tpl_params = get_path_parameters(path_parameters)
         self.path_parameters = url_tpl_params
         self.request_adapter = request_adapter
     
     def v1_by_id(self,id: str) -> v1_item_request_builder.V1ItemRequestBuilder:
         """
-        Gets an item from the ApiSdk.apis.organizations.v1.item collection
+        Gets an item from the client.apis.organizations.v1.item collection
         Args:
             id: Unique identifier of the item
         Returns: v1_item_request_builder.V1ItemRequestBuilder
         """
         if id is None:
             raise Exception("id cannot be undefined")
         from .v1.item import v1_item_request_builder
```

### Comparing `jsa-0.5.0/jsa/client/apis/organizations/v1/item/authentication_policy/authentication_policy_request_builder.py` & `jsa-0.6.0/jsa/client/apis/organizations/v1/item/authentication_policy/authentication_policy_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.5.0/jsa/client/apis/organizations/v1/item/v1_item_request_builder.py` & `jsa-0.6.0/jsa/client/apis/organizations/v1/item/v1_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.5.0/jsa/client/apis/organizations/v1/v1_request_builder.py` & `jsa-0.6.0/jsa/client/apis/organizations/v1/v1_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.5.0/jsa/client/apis/service_accounts/service_accounts_request_builder.py` & `jsa-0.6.0/jsa/client/apis/service_accounts/service_accounts_request_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
         url_tpl_params = get_path_parameters(path_parameters)
         self.path_parameters = url_tpl_params
         self.request_adapter = request_adapter
     
     def v1_by_id(self,id: str) -> v1_item_request_builder.V1ItemRequestBuilder:
         """
-        Gets an item from the ApiSdk.apis.service_accounts.v1.item collection
+        Gets an item from the client.apis.service_accounts.v1.item collection
         Args:
             id: Unique identifier of the item
         Returns: v1_item_request_builder.V1ItemRequestBuilder
         """
         if id is None:
             raise Exception("id cannot be undefined")
         from .v1.item import v1_item_request_builder
```

### Comparing `jsa-0.5.0/jsa/client/apis/service_accounts/v1/item/reset_secret/reset_secret_request_builder.py` & `jsa-0.6.0/jsa/client/apis/service_accounts/v1/item/reset_secret/reset_secret_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.5.0/jsa/client/apis/service_accounts/v1/item/v1_item_request_builder.py` & `jsa-0.6.0/jsa/client/apis/service_accounts/v1/item/v1_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.5.0/jsa/client/apis/service_accounts/v1/v1_request_builder.py` & `jsa-0.6.0/jsa/client/apis/service_accounts/v1/v1_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.5.0/jsa/client/kiota-lock.json` & `jsa-0.6.0/jsa/client/kiota-lock.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'clientClassName'": "'ServiceAccountClient'",*

 * * "'clientNamespaceName'": "'client'",*

 * * "'descriptionHash'": "'A382034132DD3C43612B41CAD36DED010A51CFF46F12049028362F75B1ED6678A01FF563F7DEE38F86EA265680B3E70EAC11026EB09DED17BA627D08D9CB948A'"}*

```diff
@@ -1,11 +1,11 @@
 {
-    "clientClassName": "ApiClient",
-    "clientNamespaceName": "ApiSdk",
-    "descriptionHash": "8A6443BA66A069C98588A05FEE1987ACA3DC9E836682619B8AF9FA9D1531716CD235A7CD3A75B31B7CBBB82C66BA1CD7A16C5407F2EBEF22307C84E8FEA9D888",
+    "clientClassName": "ServiceAccountClient",
+    "clientNamespaceName": "client",
+    "descriptionHash": "A382034132DD3C43612B41CAD36DED010A51CFF46F12049028362F75B1ED6678A01FF563F7DEE38F86EA265680B3E70EAC11026EB09DED17BA627D08D9CB948A",
     "descriptionLocation": "/Users/jackdelahunt/Projects/sdks-demo/service-accounts.yaml",
     "deserializers": [
         "Microsoft.Kiota.Serialization.Json.JsonParseNodeFactory",
         "Microsoft.Kiota.Serialization.Text.TextParseNodeFactory",
         "Microsoft.Kiota.Serialization.Form.FormParseNodeFactory"
     ],
     "disabledValidationRules": [],
```

### Comparing `jsa-0.5.0/jsa/client/models/acs_client_request_data.py` & `jsa-0.6.0/jsa/client/models/acs_client_request_data.py`

 * *Files identical despite different names*

### Comparing `jsa-0.5.0/jsa/client/models/acs_client_response_data.py` & `jsa-0.6.0/jsa/client/models/acs_client_response_data.py`

 * *Files identical despite different names*

### Comparing `jsa-0.5.0/jsa/client/models/authentication_factors.py` & `jsa-0.6.0/jsa/client/models/authentication_factors.py`

 * *Files identical despite different names*

### Comparing `jsa-0.5.0/jsa/client/models/authentication_policy.py` & `jsa-0.6.0/jsa/client/models/authentication_policy.py`

 * *Files identical despite different names*

### Comparing `jsa-0.5.0/jsa/client/models/error.py` & `jsa-0.6.0/jsa/client/models/error.py`

 * *Files identical despite different names*

### Comparing `jsa-0.5.0/jsa/client/models/otp.py` & `jsa-0.6.0/jsa/client/models/otp.py`

 * *Files identical despite different names*

### Comparing `jsa-0.5.0/jsa/client/models/red_hat_error_representation.py` & `jsa-0.6.0/jsa/client/models/red_hat_error_representation.py`

 * *Files identical despite different names*

### Comparing `jsa-0.5.0/jsa/client/models/red_hat_error_representation_error.py` & `jsa-0.6.0/jsa/client/models/red_hat_error_representation_error.py`

 * *Files identical despite different names*

### Comparing `jsa-0.5.0/jsa/client/models/service_account_create_request_data.py` & `jsa-0.6.0/jsa/client/models/service_account_create_request_data.py`

 * *Files identical despite different names*

### Comparing `jsa-0.5.0/jsa/client/models/service_account_data.py` & `jsa-0.6.0/jsa/client/models/service_account_data.py`

 * *Files identical despite different names*

### Comparing `jsa-0.5.0/jsa/client/models/service_account_request_data.py` & `jsa-0.6.0/jsa/client/models/service_account_request_data.py`

 * *Files identical despite different names*

### Comparing `jsa-0.5.0/jsa/client/models/validation_exception_data.py` & `jsa-0.6.0/jsa/client/models/validation_exception_data.py`

 * *Files identical despite different names*

### Comparing `jsa-0.5.0/jsa/client/models/validation_exception_data_fields.py` & `jsa-0.6.0/jsa/client/models/validation_exception_data_fields.py`

 * *Files identical despite different names*

### Comparing `jsa-0.5.0/PKG-INFO` & `jsa-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsa
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 Author: Jack Delahunt
 Author-email: 45426048+jackdelahunt@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

