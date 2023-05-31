# Comparing `tmp/ibm-cloud-sdk-core-3.8.0.tar.gz` & `tmp/ibm-cloud-sdk-core-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ibm-cloud-sdk-core-3.8.0.tar", last modified: Wed Mar 17 21:53:38 2021, max compression
+gzip compressed data, was "dist/ibm-cloud-sdk-core-3.9.0.tar", last modified: Thu Mar 25 13:47:56 2021, max compression
```

## Comparing `ibm-cloud-sdk-core-3.8.0.tar` & `ibm-cloud-sdk-core-3.9.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 21:53:38.000000 ibm-cloud-sdk-core-3.8.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)       70 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 21:53:38.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/
--rw-rw-r--   0 travis    (2000) travis    (2000)    17033 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/base_service.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7867 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/iam_token_manager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4031 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/jwt_token_manager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4016 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/cp4d_token_manager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2717 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/get_authenticator.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 21:53:38.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/authenticators/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3025 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/authenticators/basic_authenticator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7091 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/authenticators/iam_authenticator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5618 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/authenticators/cp4d_authenticator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1433 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/authenticators/authenticator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2505 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/authenticators/bearer_token_authenticator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1958 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/authenticators/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      865 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/authenticators/no_auth_authenticator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12549 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7484 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/token_manager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2738 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/detailed_response.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2591 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3178 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/api_exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       69 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     5068 2021-03-17 21:53:38.000000 ibm-cloud-sdk-core-3.8.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3395 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      148 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/requirements-dev.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 21:53:38.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5068 2021-03-17 21:53:38.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-17 21:52:54.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-17 21:53:38.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2021-03-17 21:53:38.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1513 2021-03-17 21:53:38.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       70 2021-03-17 21:53:38.000000 ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-03-17 21:53:38.000000 ibm-cloud-sdk-core-3.8.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-17 21:53:38.000000 ibm-cloud-sdk-core-3.8.0/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1508 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/test/test_basic_authenticator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4063 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/test/test_cp4d_authenticator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28443 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/test/test_base_service.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      967 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/test/test_bearer_authenticator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2367 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/test/test_detailed_response.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12569 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/test/test_iam_token_manager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3738 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/test/test_iam_authenticator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1498 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/test/test_cp4d_token_manager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/test/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      411 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/test/test_no_auth_authenticator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3812 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/test/test_jwt_token_manager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22286 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/test/test_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2446 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/test/test_token_manager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2852 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/test/test_api_exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3014 2021-03-17 21:52:23.000000 ibm-cloud-sdk-core-3.8.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-25 13:47:56.000000 ibm-cloud-sdk-core-3.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       70 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/MANIFEST.in
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-25 13:47:56.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18754 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/base_service.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7867 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/iam_token_manager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4031 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/jwt_token_manager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4016 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/cp4d_token_manager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2717 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/get_authenticator.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-25 13:47:56.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/authenticators/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3025 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/authenticators/basic_authenticator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7091 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/authenticators/iam_authenticator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5618 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/authenticators/cp4d_authenticator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1433 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/authenticators/authenticator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2505 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/authenticators/bearer_token_authenticator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1958 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/authenticators/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      865 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/authenticators/no_auth_authenticator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12549 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       22 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7484 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/token_manager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2738 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/detailed_response.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2591 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3178 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/api_exception.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       69 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5068 2021-03-25 13:47:56.000000 ibm-cloud-sdk-core-3.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3395 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      148 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/requirements-dev.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-25 13:47:56.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5068 2021-03-25 13:47:56.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-25 13:47:13.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core.egg-info/zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-25 13:47:56.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       24 2021-03-25 13:47:56.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1513 2021-03-25 13:47:56.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       70 2021-03-25 13:47:56.000000 ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-03-25 13:47:56.000000 ibm-cloud-sdk-core-3.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/LICENSE
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-25 13:47:56.000000 ibm-cloud-sdk-core-3.9.0/test/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1508 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/test/test_basic_authenticator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4063 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/test/test_cp4d_authenticator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31319 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/test/test_base_service.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      967 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/test/test_bearer_authenticator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2367 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/test/test_detailed_response.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12569 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/test/test_iam_token_manager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3738 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/test/test_iam_authenticator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1498 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/test/test_cp4d_token_manager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/test/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      411 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/test/test_no_auth_authenticator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3812 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/test/test_jwt_token_manager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22286 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/test/test_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2446 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/test/test_token_manager.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2852 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/test/test_api_exception.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3014 2021-03-25 13:46:41.000000 ibm-cloud-sdk-core-3.9.0/setup.py
```

### Comparing `ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/base_service.py` & `ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/base_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 from os.path import basename
 import platform
 import sys
 import gzip
 from typing import Dict, List, Optional, Tuple, Union
 
 import requests
+from requests.adapters import HTTPAdapter
 from requests.structures import CaseInsensitiveDict
+from urllib3.util.retry import Retry
 from ibm_cloud_sdk_core.authenticators import Authenticator
 from .version import __version__
 from .utils import (has_bad_first_or_last_char, remove_null_values,
                     cleanup_values, read_external_sources, strip_extra_slashes)
 from .detailed_response import DetailedResponse
 from .api_exception import ApiException
 from .token_manager import TokenManager
@@ -84,19 +86,43 @@
         self.http_config = {}
         self.jar = CookieJar()
         self.authenticator = authenticator
         self.disable_ssl_verification = disable_ssl_verification
         self.default_headers = None
         self.enable_gzip_compression = enable_gzip_compression
         self._set_user_agent_header(self._build_user_agent())
+        self.retry_config = None
+        self.http_adapter = HTTPAdapter()
         if not self.authenticator:
             raise ValueError('authenticator must be provided')
         if not isinstance(self.authenticator, Authenticator):
             raise ValueError('authenticator should be of type Authenticator')
 
+    def enable_retries(self, max_retries: int = 4, retry_interval: float = 0.1) -> None:
+        """Setup http_client with retry_config and http_adapter"""
+        self.retry_config = Retry(
+            total = max_retries,
+            backoff_factor = retry_interval,
+            # List of HTTP status codes to retry on in addition to Timeout/Connection Errors
+            status_forcelist = [429, 500, 502, 503, 504],
+            # List of HTTP methods to retry on
+            # Omitting this will default to all methods except POST
+            allowed_methods=['HEAD', 'GET', 'PUT', 'DELETE', 'OPTIONS', 'TRACE', 'POST']
+        )
+        self.http_adapter = HTTPAdapter(max_retries=self.retry_config)
+        self.http_client.mount('http://', self.http_adapter)
+        self.http_client.mount('https://', self.http_adapter)
+
+    def disable_retries(self):
+        """Remove retry config from http_adapter"""
+        self.retry_config = None
+        self.http_adapter = HTTPAdapter()
+        self.http_client.mount('http://', self.http_adapter)
+        self.http_client.mount('https://', self.http_adapter)
+
     @staticmethod
     def _get_system_info() -> str:
         return '{0} {1} {2}'.format(
             platform.system(),  # OS
             platform.release(),  # OS version
             platform.python_version()  # Python version
         )
@@ -122,18 +148,27 @@
         if not isinstance(service_name, str):
             raise ValueError('Service_name must be of type string.')
 
         config = read_external_sources(service_name)
         if config.get('URL'):
             self.set_service_url(config.get('URL'))
         if config.get('DISABLE_SSL'):
-            self.set_disable_ssl_verification(bool(config.get('DISABLE_SSL')))
-        if config.get('ENABLE_GZIP') is not None:
+            self.set_disable_ssl_verification(
+                config.get('DISABLE_SSL').lower() == 'true')
+        if config.get('ENABLE_GZIP'):
             self.set_enable_gzip_compression(
-                config.get('ENABLE_GZIP') == 'True')
+                config.get('ENABLE_GZIP').lower() == 'true')
+        if config.get('ENABLE_RETRIES'):
+            if config.get('ENABLE_RETRIES').lower() == 'true':
+                kwargs = {}
+                if config.get('MAX_RETRIES'):
+                    kwargs["max_retries"] = int(config.get('MAX_RETRIES'))
+                if config.get('RETRY_INTERVAL'):
+                    kwargs["retry_interval"] = float(config.get('RETRY_INTERVAL'))
+                self.enable_retries(**kwargs)
 
     def _set_user_agent_header(self, user_agent_string: str) -> None:
         self.user_agent_header = {'User-Agent': user_agent_string}
 
     def set_http_config(self, http_config: dict) -> None:
         """Sets the http config dictionary.
```

### Comparing `ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/iam_token_manager.py` & `ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/iam_token_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/jwt_token_manager.py` & `ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/jwt_token_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/cp4d_token_manager.py` & `ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/cp4d_token_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/get_authenticator.py` & `ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/get_authenticator.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/authenticators/basic_authenticator.py` & `ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/authenticators/basic_authenticator.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/authenticators/iam_authenticator.py` & `ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/authenticators/iam_authenticator.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/authenticators/cp4d_authenticator.py` & `ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/authenticators/cp4d_authenticator.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/authenticators/authenticator.py` & `ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/authenticators/authenticator.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/authenticators/bearer_token_authenticator.py` & `ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/authenticators/bearer_token_authenticator.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/authenticators/__init__.py` & `ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/authenticators/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/authenticators/no_auth_authenticator.py` & `ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/authenticators/no_auth_authenticator.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/utils.py` & `ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/utils.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/token_manager.py` & `ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/token_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/detailed_response.py` & `ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/detailed_response.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/__init__.py` & `ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core/api_exception.py` & `ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core/api_exception.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/PKG-INFO` & `ibm-cloud-sdk-core-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ibm-cloud-sdk-core
-Version: 3.8.0
+Version: 3.9.0
 Summary: Core library used by SDKs for IBM Cloud Services
 Home-page: https://github.com/IBM/python-sdk-core
 Author: IBM
 Author-email: devexdev@us.ibm.com
 License: Apache 2.0
 Description: [![Build Status](https://travis-ci.com/IBM/python-sdk-core.svg?branch=main)](https://travis-ci.com/IBM/python-sdk-core)
         [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ibm-cloud-sdk-core)](https://pypi.org/project/ibm-cloud-sdk-core/)
         [![Latest Stable Version](https://img.shields.io/pypi/v/ibm-cloud-sdk-core.svg)](https://pypi.python.org/pypi/ibm-cloud-sdk-core)
         [![CLA assistant](https://cla-assistant.io/readme/badge/ibm/python-sdk-core)](https://cla-assistant.io/ibm/python-sdk-core)
         [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)[![codecov](https://codecov.io/gh/IBM/python-sdk-core/branch/main/graph/badge.svg)](https://codecov.io/gh/IBM/python-sdk-core)
         
-        # IBM Python SDK Core Version 3.8.0
+        # IBM Python SDK Core Version 3.9.0
         This project contains core functionality required by Python code generated by the IBM Cloud OpenAPI SDK Generator
         (openapi-sdkgen).
         
         # Python Version
         The current minimum Python version supported is 3.6.
         
         ## Installation
```

### Comparing `ibm-cloud-sdk-core-3.8.0/README.md` & `ibm-cloud-sdk-core-3.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [![Build Status](https://travis-ci.com/IBM/python-sdk-core.svg?branch=main)](https://travis-ci.com/IBM/python-sdk-core)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ibm-cloud-sdk-core)](https://pypi.org/project/ibm-cloud-sdk-core/)
 [![Latest Stable Version](https://img.shields.io/pypi/v/ibm-cloud-sdk-core.svg)](https://pypi.python.org/pypi/ibm-cloud-sdk-core)
 [![CLA assistant](https://cla-assistant.io/readme/badge/ibm/python-sdk-core)](https://cla-assistant.io/ibm/python-sdk-core)
 [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)[![codecov](https://codecov.io/gh/IBM/python-sdk-core/branch/main/graph/badge.svg)](https://codecov.io/gh/IBM/python-sdk-core)
 
-# IBM Python SDK Core Version 3.8.0
+# IBM Python SDK Core Version 3.9.0
 This project contains core functionality required by Python code generated by the IBM Cloud OpenAPI SDK Generator
 (openapi-sdkgen).
 
 # Python Version
 The current minimum Python version supported is 3.6.
 
 ## Installation
```

### Comparing `ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core.egg-info/PKG-INFO` & `ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ibm-cloud-sdk-core
-Version: 3.8.0
+Version: 3.9.0
 Summary: Core library used by SDKs for IBM Cloud Services
 Home-page: https://github.com/IBM/python-sdk-core
 Author: IBM
 Author-email: devexdev@us.ibm.com
 License: Apache 2.0
 Description: [![Build Status](https://travis-ci.com/IBM/python-sdk-core.svg?branch=main)](https://travis-ci.com/IBM/python-sdk-core)
         [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ibm-cloud-sdk-core)](https://pypi.org/project/ibm-cloud-sdk-core/)
         [![Latest Stable Version](https://img.shields.io/pypi/v/ibm-cloud-sdk-core.svg)](https://pypi.python.org/pypi/ibm-cloud-sdk-core)
         [![CLA assistant](https://cla-assistant.io/readme/badge/ibm/python-sdk-core)](https://cla-assistant.io/ibm/python-sdk-core)
         [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)[![codecov](https://codecov.io/gh/IBM/python-sdk-core/branch/main/graph/badge.svg)](https://codecov.io/gh/IBM/python-sdk-core)
         
-        # IBM Python SDK Core Version 3.8.0
+        # IBM Python SDK Core Version 3.9.0
         This project contains core functionality required by Python code generated by the IBM Cloud OpenAPI SDK Generator
         (openapi-sdkgen).
         
         # Python Version
         The current minimum Python version supported is 3.6.
         
         ## Installation
```

### Comparing `ibm-cloud-sdk-core-3.8.0/ibm_cloud_sdk_core.egg-info/SOURCES.txt` & `ibm-cloud-sdk-core-3.9.0/ibm_cloud_sdk_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/LICENSE` & `ibm-cloud-sdk-core-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/test/test_basic_authenticator.py` & `ibm-cloud-sdk-core-3.9.0/test/test_basic_authenticator.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/test/test_cp4d_authenticator.py` & `ibm-cloud-sdk-core-3.9.0/test/test_cp4d_authenticator.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/test/test_base_service.py` & `ibm-cloud-sdk-core-3.9.0/test/test_base_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Optional
 import gzip
 import tempfile
 import pytest
 import responses
 import requests
 import jwt
+from urllib3.exceptions import ConnectTimeoutError, MaxRetryError
 from ibm_cloud_sdk_core import BaseService, DetailedResponse
 from ibm_cloud_sdk_core import ApiException
 from ibm_cloud_sdk_core import CP4DTokenManager
 from ibm_cloud_sdk_core.authenticators import (IAMAuthenticator, NoAuthAuthenticator, Authenticator,
                                                BasicAuthenticator, CloudPakForDataAuthenticator)
 from ibm_cloud_sdk_core import get_authenticator_from_environment
 from ibm_cloud_sdk_core.utils import strip_extra_slashes
@@ -549,14 +550,80 @@
     service = IncludeExternalConfigService('v1', authenticator=NoAuthAuthenticator())
     assert service.service_url == 'https://mockurl'
     assert service.get_enable_gzip_compression() is True
     prepped = service.prepare_request('GET', url='', data=json.dumps({"foo": "bar"}))
     assert prepped['data'] == gzip.compress(b'{"foo": "bar"}')
     assert prepped['headers'].get('content-encoding') == 'gzip'
 
+def test_retry_config_default():
+    service = BaseService(service_url='https://mockurl/', authenticator=NoAuthAuthenticator())
+    service.enable_retries()
+    assert service.retry_config.total == 4
+    assert service.retry_config.backoff_factor == 0.1
+    assert service.http_client.get_adapter('https://').max_retries.total == 4
+
+    # Ensure retries fail after 4 retries
+    error = ConnectTimeoutError()
+    retry = service.http_client.get_adapter('https://').max_retries
+    retry = retry.increment(error=error)
+    retry = retry.increment(error=error)
+    retry = retry.increment(error=error)
+    retry = retry.increment(error=error)
+    with pytest.raises(MaxRetryError) as retry_err:
+        retry.increment(error=error)
+    assert retry_err.value.reason == error
+
+def test_retry_config_disable():
+    # Test disabling retries
+    service = BaseService(service_url='https://mockurl/', authenticator=NoAuthAuthenticator())
+    service.enable_retries()
+    service.disable_retries()
+    assert service.retry_config is None
+    assert service.http_client.get_adapter('https://').max_retries.total == 0
+
+    # Ensure retries are not started after one connection attempt
+    error = ConnectTimeoutError()
+    retry = service.http_client.get_adapter('https://').max_retries
+    with pytest.raises(MaxRetryError) as retry_err:
+        retry.increment(error=error)
+    assert retry_err.value.reason == error
+
+def test_retry_config_non_default():
+    service = BaseService(service_url='https://mockurl/', authenticator=NoAuthAuthenticator())
+    service.enable_retries(2, 0.3)
+    assert service.retry_config.total == 2
+    assert service.retry_config.backoff_factor == 0.3
+
+    # Ensure retries fail after 2 retries
+    error = ConnectTimeoutError()
+    retry = service.http_client.get_adapter('https://').max_retries
+    retry = retry.increment(error=error)
+    retry = retry.increment(error=error)
+    with pytest.raises(MaxRetryError) as retry_err:
+        retry.increment(error=error)
+    assert retry_err.value.reason == error
+
+def test_retry_config_external():
+    file_path = os.path.join(
+        os.path.dirname(__file__), '../resources/ibm-credentials-retry.env')
+    os.environ['IBM_CREDENTIALS_FILE'] = file_path
+    service = IncludeExternalConfigService('v1', authenticator=NoAuthAuthenticator())
+    assert service.retry_config.total == 3
+    assert service.retry_config.backoff_factor == 0.2
+
+    # Ensure retries fail after 3 retries
+    error = ConnectTimeoutError()
+    retry = service.http_client.get_adapter('https://').max_retries
+    retry = retry.increment(error=error)
+    retry = retry.increment(error=error)
+    retry = retry.increment(error=error)
+    with pytest.raises(MaxRetryError) as retry_err:
+        retry.increment(error=error)
+    assert retry_err.value.reason == error
+
 @responses.activate
 def test_user_agent_header():
     service = AnyServiceV1('2018-11-20', authenticator=NoAuthAuthenticator())
     user_agent_header = service.user_agent_header
     assert user_agent_header is not None
     assert user_agent_header['User-Agent'] is not None
```

### Comparing `ibm-cloud-sdk-core-3.8.0/test/test_bearer_authenticator.py` & `ibm-cloud-sdk-core-3.9.0/test/test_bearer_authenticator.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/test/test_detailed_response.py` & `ibm-cloud-sdk-core-3.9.0/test/test_detailed_response.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/test/test_iam_token_manager.py` & `ibm-cloud-sdk-core-3.9.0/test/test_iam_token_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/test/test_iam_authenticator.py` & `ibm-cloud-sdk-core-3.9.0/test/test_iam_authenticator.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/test/test_cp4d_token_manager.py` & `ibm-cloud-sdk-core-3.9.0/test/test_cp4d_token_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/test/test_jwt_token_manager.py` & `ibm-cloud-sdk-core-3.9.0/test/test_jwt_token_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/test/test_utils.py` & `ibm-cloud-sdk-core-3.9.0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/test/test_token_manager.py` & `ibm-cloud-sdk-core-3.9.0/test/test_token_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/test/test_api_exception.py` & `ibm-cloud-sdk-core-3.9.0/test/test_api_exception.py`

 * *Files identical despite different names*

### Comparing `ibm-cloud-sdk-core-3.8.0/setup.py` & `ibm-cloud-sdk-core-3.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import os
 import sys
 import pkg_resources
 from setuptools import setup, find_packages
 from setuptools.command.test import test as TestCommand
 
-__version__ = '3.8.0'
+__version__ = '3.9.0'
 
 if sys.argv[-1] == 'publish':
     # test server
     os.system('python setup.py register -r pypitest')
     os.system('python setup.py sdist upload -r pypitest')
 
     # production server
```

