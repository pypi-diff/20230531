# Comparing `tmp/jsa-0.4.0.tar.gz` & `tmp/jsa-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsa-0.4.0.tar", max compression
+gzip compressed data, was "jsa-0.5.0.tar", max compression
```

## Comparing `jsa-0.4.0.tar` & `jsa-0.5.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0        0 2023-05-31 08:34:45.131459 jsa-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-05-31 08:34:45.131408 jsa-0.4.0/jsa/__init__.py
--rw-r--r--   0        0        0     2438 2023-05-31 08:34:46.264600 jsa-0.4.0/jsa/api_client.py
--rw-r--r--   0        0        0     2450 2023-05-31 08:34:46.285433 jsa-0.4.0/jsa/apis/apis_request_builder.py
--rw-r--r--   0        0        0     2347 2023-05-31 08:34:46.279517 jsa-0.4.0/jsa/apis/beta/acs/acs_request_builder.py
--rw-r--r--   0        0        0     4188 2023-05-31 08:34:46.278800 jsa-0.4.0/jsa/apis/beta/acs/v1/item/with_client_item_request_builder.py
--rw-r--r--   0        0        0     4909 2023-05-31 08:34:46.278185 jsa-0.4.0/jsa/apis/beta/acs/v1/v1_request_builder.py
--rw-r--r--   0        0        0     1596 2023-05-31 08:34:46.279758 jsa-0.4.0/jsa/apis/beta/beta_request_builder.py
--rw-r--r--   0        0        0     2307 2023-05-31 08:34:46.286902 jsa-0.4.0/jsa/apis/organizations/organizations_request_builder.py
--rw-r--r--   0        0        0     6794 2023-05-31 08:34:46.286301 jsa-0.4.0/jsa/apis/organizations/v1/item/authentication_policy/authentication_policy_request_builder.py
--rw-r--r--   0        0        0     1811 2023-05-31 08:34:46.286621 jsa-0.4.0/jsa/apis/organizations/v1/item/v1_item_request_builder.py
--rw-r--r--   0        0        0     1285 2023-05-31 08:34:46.285714 jsa-0.4.0/jsa/apis/organizations/v1/v1_request_builder.py
--rw-r--r--   0        0        0     2322 2023-05-31 08:34:46.280107 jsa-0.4.0/jsa/apis/service_accounts/service_accounts_request_builder.py
--rw-r--r--   0        0        0     4349 2023-05-31 08:34:46.285008 jsa-0.4.0/jsa/apis/service_accounts/v1/item/reset_secret/reset_secret_request_builder.py
--rw-r--r--   0        0        0     9985 2023-05-31 08:34:46.281632 jsa-0.4.0/jsa/apis/service_accounts/v1/item/v1_item_request_builder.py
--rw-r--r--   0        0        0     8123 2023-05-31 08:34:46.280715 jsa-0.4.0/jsa/apis/service_accounts/v1/v1_request_builder.py
--rw-r--r--   0        0        0     1109 2023-05-31 08:34:46.294784 jsa-0.4.0/jsa/kiota-lock.json
--rw-r--r--   0        0        0     4723 2023-05-31 08:34:46.273865 jsa-0.4.0/jsa/models/acs_client_request_data.py
--rw-r--r--   0        0        0     5331 2023-05-31 08:34:46.270919 jsa-0.4.0/jsa/models/acs_client_response_data.py
--rw-r--r--   0        0        0     3298 2023-05-31 08:34:46.268745 jsa-0.4.0/jsa/models/authentication_factors.py
--rw-r--r--   0        0        0     3813 2023-05-31 08:34:46.269929 jsa-0.4.0/jsa/models/authentication_policy.py
--rw-r--r--   0        0        0     3196 2023-05-31 08:34:46.270481 jsa-0.4.0/jsa/models/error.py
--rw-r--r--   0        0        0     3197 2023-05-31 08:34:46.268202 jsa-0.4.0/jsa/models/otp.py
--rw-r--r--   0        0        0     4579 2023-05-31 08:34:46.269426 jsa-0.4.0/jsa/models/red_hat_error_representation.py
--rw-r--r--   0        0        0      865 2023-05-31 08:34:46.272130 jsa-0.4.0/jsa/models/red_hat_error_representation_error.py
--rw-r--r--   0        0        0     4019 2023-05-31 08:34:46.273014 jsa-0.4.0/jsa/models/service_account_create_request_data.py
--rw-r--r--   0        0        0     7558 2023-05-31 08:34:46.271603 jsa-0.4.0/jsa/models/service_account_data.py
--rw-r--r--   0        0        0     3989 2023-05-31 08:34:46.273358 jsa-0.4.0/jsa/models/service_account_request_data.py
--rw-r--r--   0        0        0     5226 2023-05-31 08:34:46.272561 jsa-0.4.0/jsa/models/validation_exception_data.py
--rw-r--r--   0        0        0     2622 2023-05-31 08:34:46.270192 jsa-0.4.0/jsa/models/validation_exception_data_fields.py
--rw-r--r--   0        0        0      388 2023-05-31 08:37:34.839379 jsa-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      410 1970-01-01 00:00:00.000000 jsa-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0        5 2023-05-31 08:48:45.448903 jsa-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 08:47:30.991564 jsa-0.5.0/jsa/__init__.py
+-rw-r--r--   0        0        0     2438 2023-05-31 08:47:44.244244 jsa-0.5.0/jsa/client/api_client.py
+-rw-r--r--   0        0        0     2450 2023-05-31 08:47:44.243648 jsa-0.5.0/jsa/client/apis/apis_request_builder.py
+-rw-r--r--   0        0        0     2347 2023-05-31 08:47:44.238767 jsa-0.5.0/jsa/client/apis/beta/acs/acs_request_builder.py
+-rw-r--r--   0        0        0     4188 2023-05-31 08:47:44.237902 jsa-0.5.0/jsa/client/apis/beta/acs/v1/item/with_client_item_request_builder.py
+-rw-r--r--   0        0        0     4909 2023-05-31 08:47:44.238366 jsa-0.5.0/jsa/client/apis/beta/acs/v1/v1_request_builder.py
+-rw-r--r--   0        0        0     1596 2023-05-31 08:47:44.238987 jsa-0.5.0/jsa/client/apis/beta/beta_request_builder.py
+-rw-r--r--   0        0        0     2307 2023-05-31 08:47:44.239263 jsa-0.5.0/jsa/client/apis/organizations/organizations_request_builder.py
+-rw-r--r--   0        0        0     6794 2023-05-31 08:47:44.243070 jsa-0.5.0/jsa/client/apis/organizations/v1/item/authentication_policy/authentication_policy_request_builder.py
+-rw-r--r--   0        0        0     1811 2023-05-31 08:47:44.242439 jsa-0.5.0/jsa/client/apis/organizations/v1/item/v1_item_request_builder.py
+-rw-r--r--   0        0        0     1285 2023-05-31 08:47:44.243375 jsa-0.5.0/jsa/client/apis/organizations/v1/v1_request_builder.py
+-rw-r--r--   0        0        0     2322 2023-05-31 08:47:44.232485 jsa-0.5.0/jsa/client/apis/service_accounts/service_accounts_request_builder.py
+-rw-r--r--   0        0        0     4349 2023-05-31 08:47:44.236624 jsa-0.5.0/jsa/client/apis/service_accounts/v1/item/reset_secret/reset_secret_request_builder.py
+-rw-r--r--   0        0        0     9985 2023-05-31 08:47:44.236119 jsa-0.5.0/jsa/client/apis/service_accounts/v1/item/v1_item_request_builder.py
+-rw-r--r--   0        0        0     8123 2023-05-31 08:47:44.237294 jsa-0.5.0/jsa/client/apis/service_accounts/v1/v1_request_builder.py
+-rw-r--r--   0        0        0     1109 2023-05-31 08:47:44.252201 jsa-0.5.0/jsa/client/kiota-lock.json
+-rw-r--r--   0        0        0     4723 2023-05-31 08:47:44.227541 jsa-0.5.0/jsa/client/models/acs_client_request_data.py
+-rw-r--r--   0        0        0     5331 2023-05-31 08:47:44.224667 jsa-0.5.0/jsa/client/models/acs_client_response_data.py
+-rw-r--r--   0        0        0     3298 2023-05-31 08:47:44.227101 jsa-0.5.0/jsa/client/models/authentication_factors.py
+-rw-r--r--   0        0        0     3813 2023-05-31 08:47:44.228829 jsa-0.5.0/jsa/client/models/authentication_policy.py
+-rw-r--r--   0        0        0     3196 2023-05-31 08:47:44.227980 jsa-0.5.0/jsa/client/models/error.py
+-rw-r--r--   0        0        0     3197 2023-05-31 08:47:44.223992 jsa-0.5.0/jsa/client/models/otp.py
+-rw-r--r--   0        0        0     4579 2023-05-31 08:47:44.226192 jsa-0.5.0/jsa/client/models/red_hat_error_representation.py
+-rw-r--r--   0        0        0      865 2023-05-31 08:47:44.226773 jsa-0.5.0/jsa/client/models/red_hat_error_representation_error.py
+-rw-r--r--   0        0        0     4019 2023-05-31 08:47:44.229165 jsa-0.5.0/jsa/client/models/service_account_create_request_data.py
+-rw-r--r--   0        0        0     7558 2023-05-31 08:47:44.229789 jsa-0.5.0/jsa/client/models/service_account_data.py
+-rw-r--r--   0        0        0     3989 2023-05-31 08:47:44.230253 jsa-0.5.0/jsa/client/models/service_account_request_data.py
+-rw-r--r--   0        0        0     5226 2023-05-31 08:47:44.228414 jsa-0.5.0/jsa/client/models/validation_exception_data.py
+-rw-r--r--   0        0        0     2622 2023-05-31 08:47:44.222138 jsa-0.5.0/jsa/client/models/validation_exception_data_fields.py
+-rw-r--r--   0        0        0      559 2023-05-31 08:46:07.159328 jsa-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 jsa-0.5.0/PKG-INFO
```

### Comparing `jsa-0.4.0/jsa/api_client.py` & `jsa-0.5.0/jsa/client/api_client.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/apis/apis_request_builder.py` & `jsa-0.5.0/jsa/client/apis/apis_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/apis/beta/acs/acs_request_builder.py` & `jsa-0.5.0/jsa/client/apis/beta/acs/acs_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/apis/beta/acs/v1/item/with_client_item_request_builder.py` & `jsa-0.5.0/jsa/client/apis/beta/acs/v1/item/with_client_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/apis/beta/acs/v1/v1_request_builder.py` & `jsa-0.5.0/jsa/client/apis/beta/acs/v1/v1_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/apis/beta/beta_request_builder.py` & `jsa-0.5.0/jsa/client/apis/beta/beta_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/apis/organizations/organizations_request_builder.py` & `jsa-0.5.0/jsa/client/apis/organizations/organizations_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/apis/organizations/v1/item/authentication_policy/authentication_policy_request_builder.py` & `jsa-0.5.0/jsa/client/apis/organizations/v1/item/authentication_policy/authentication_policy_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/apis/organizations/v1/item/v1_item_request_builder.py` & `jsa-0.5.0/jsa/client/apis/organizations/v1/item/v1_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/apis/organizations/v1/v1_request_builder.py` & `jsa-0.5.0/jsa/client/apis/organizations/v1/v1_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/apis/service_accounts/service_accounts_request_builder.py` & `jsa-0.5.0/jsa/client/apis/service_accounts/service_accounts_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/apis/service_accounts/v1/item/reset_secret/reset_secret_request_builder.py` & `jsa-0.5.0/jsa/client/apis/service_accounts/v1/item/reset_secret/reset_secret_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/apis/service_accounts/v1/item/v1_item_request_builder.py` & `jsa-0.5.0/jsa/client/apis/service_accounts/v1/item/v1_item_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/apis/service_accounts/v1/v1_request_builder.py` & `jsa-0.5.0/jsa/client/apis/service_accounts/v1/v1_request_builder.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/kiota-lock.json` & `jsa-0.5.0/jsa/client/kiota-lock.json`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/models/acs_client_request_data.py` & `jsa-0.5.0/jsa/client/models/acs_client_request_data.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/models/acs_client_response_data.py` & `jsa-0.5.0/jsa/client/models/acs_client_response_data.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/models/authentication_factors.py` & `jsa-0.5.0/jsa/client/models/authentication_factors.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/models/authentication_policy.py` & `jsa-0.5.0/jsa/client/models/authentication_policy.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/models/error.py` & `jsa-0.5.0/jsa/client/models/error.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/models/otp.py` & `jsa-0.5.0/jsa/client/models/otp.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/models/red_hat_error_representation.py` & `jsa-0.5.0/jsa/client/models/red_hat_error_representation.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/models/red_hat_error_representation_error.py` & `jsa-0.5.0/jsa/client/models/red_hat_error_representation_error.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/models/service_account_create_request_data.py` & `jsa-0.5.0/jsa/client/models/service_account_create_request_data.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/models/service_account_data.py` & `jsa-0.5.0/jsa/client/models/service_account_data.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/models/service_account_request_data.py` & `jsa-0.5.0/jsa/client/models/service_account_request_data.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/models/validation_exception_data.py` & `jsa-0.5.0/jsa/client/models/validation_exception_data.py`

 * *Files identical despite different names*

### Comparing `jsa-0.4.0/jsa/models/validation_exception_data_fields.py` & `jsa-0.5.0/jsa/client/models/validation_exception_data_fields.py`

 * *Files identical despite different names*

