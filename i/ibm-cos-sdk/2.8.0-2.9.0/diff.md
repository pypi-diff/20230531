# Comparing `tmp/ibm-cos-sdk-2.8.0.tar.gz` & `tmp/ibm-cos-sdk-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ibm-cos-sdk-2.8.0.tar", last modified: Tue Oct 27 20:35:34 2020, max compression
+gzip compressed data, was "dist/ibm-cos-sdk-2.9.0.tar", last modified: Mon Dec 14 21:54:51 2020, max compression
```

## Comparing `ibm-cos-sdk-2.8.0.tar` & `ibm-cos-sdk-2.9.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/
--rw-r--r--   0 root         (0) root         (0)      124 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7751 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5914 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_cos_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)       77 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_cos_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     7751 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_cos_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1047 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_cos_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_cos_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_cos_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    10174 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/LICENSE
--rwxr-xr-x   0 root         (0) root         (0)      176 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/
--rwxr-xr-x   0 root         (0) root         (0)     3428 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1601 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/compat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/s3/
--rw-r--r--   0 root         (0) root         (0)      561 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/s3/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12908 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/s3/transfer.py
--rwxr-xr-x   0 root         (0) root         (0)    26400 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/s3/inject.py
--rwxr-xr-x   0 root         (0) root         (0)    22678 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/session.py
--rw-r--r--   0 root         (0) root         (0)     4017 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/data/s3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/data/s3/2006-03-01/
--rwxr-xr-x   0 root         (0) root         (0)    34856 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/data/s3/2006-03-01/resources-1.json
--rw-r--r--   0 root         (0) root         (0)     3107 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/resources/
--rw-r--r--   0 root         (0) root         (0)    19101 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/resources/collection.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/resources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9548 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/resources/action.py
--rw-r--r--   0 root         (0) root         (0)     5070 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/resources/base.py
--rw-r--r--   0 root         (0) root         (0)    22425 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/resources/factory.py
--rw-r--r--   0 root         (0) root         (0)    20687 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/resources/model.py
--rw-r--r--   0 root         (0) root         (0)    11589 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/resources/response.py
--rw-r--r--   0 root         (0) root         (0)     6140 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/resources/params.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/docs/
--rw-r--r--   0 root         (0) root         (0)     9749 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/docs/collection.py
--rw-r--r--   0 root         (0) root         (0)     1537 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/docs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6210 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/docs/action.py
--rw-r--r--   0 root         (0) root         (0)     2669 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/docs/docstring.py
--rw-r--r--   0 root         (0) root         (0)     4070 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/docs/waiter.py
--rw-r--r--   0 root         (0) root         (0)     1334 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/docs/base.py
--rw-r--r--   0 root         (0) root         (0)     2225 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/docs/attr.py
--rw-r--r--   0 root         (0) root         (0)     2772 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/docs/method.py
--rwxr-xr-x   0 root         (0) root         (0)    11060 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/docs/resource.py
--rwxr-xr-x   0 root         (0) root         (0)     5519 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/docs/service.py
--rw-r--r--   0 root         (0) root         (0)     5714 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/docs/utils.py
--rwxr-xr-x   0 root         (0) root         (0)     1076 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/docs/client.py
--rw-r--r--   0 root         (0) root         (0)     4648 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/ibm_boto3/docs/subresource.py
--rwxr-xr-x   0 root         (0) root         (0)     1534 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/setup.py
--rwxr-xr-x   0 root         (0) root         (0)      269 2020-10-27 20:35:34.000000 ibm-cos-sdk-2.8.0/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/
+-rw-r--r--   0 root         (0) root         (0)      124 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7383 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5906 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_cos_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       77 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_cos_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     7383 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_cos_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1047 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_cos_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_cos_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_cos_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    10174 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/LICENSE
+-rwxr-xr-x   0 root         (0) root         (0)      176 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/
+-rwxr-xr-x   0 root         (0) root         (0)     3428 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/compat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/s3/
+-rw-r--r--   0 root         (0) root         (0)      561 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/s3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12908 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/s3/transfer.py
+-rwxr-xr-x   0 root         (0) root         (0)    26400 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/s3/inject.py
+-rwxr-xr-x   0 root         (0) root         (0)    22678 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/session.py
+-rw-r--r--   0 root         (0) root         (0)     4017 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/data/s3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/data/s3/2006-03-01/
+-rwxr-xr-x   0 root         (0) root         (0)    34856 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/data/s3/2006-03-01/resources-1.json
+-rw-r--r--   0 root         (0) root         (0)     3107 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/resources/
+-rw-r--r--   0 root         (0) root         (0)    19101 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/resources/collection.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/resources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9548 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/resources/action.py
+-rw-r--r--   0 root         (0) root         (0)     5070 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/resources/base.py
+-rw-r--r--   0 root         (0) root         (0)    22425 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/resources/factory.py
+-rw-r--r--   0 root         (0) root         (0)    20687 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/resources/model.py
+-rw-r--r--   0 root         (0) root         (0)    11589 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/resources/response.py
+-rw-r--r--   0 root         (0) root         (0)     6140 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/resources/params.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/docs/
+-rw-r--r--   0 root         (0) root         (0)     9749 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/docs/collection.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/docs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6210 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/docs/action.py
+-rw-r--r--   0 root         (0) root         (0)     2669 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/docs/docstring.py
+-rw-r--r--   0 root         (0) root         (0)     4070 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/docs/waiter.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/docs/base.py
+-rw-r--r--   0 root         (0) root         (0)     2225 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/docs/attr.py
+-rw-r--r--   0 root         (0) root         (0)     2772 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/docs/method.py
+-rwxr-xr-x   0 root         (0) root         (0)    11060 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/docs/resource.py
+-rwxr-xr-x   0 root         (0) root         (0)     5519 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/docs/service.py
+-rw-r--r--   0 root         (0) root         (0)     5714 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/docs/utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     1076 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/docs/client.py
+-rw-r--r--   0 root         (0) root         (0)     4648 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/ibm_boto3/docs/subresource.py
+-rwxr-xr-x   0 root         (0) root         (0)     1534 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/setup.py
+-rwxr-xr-x   0 root         (0) root         (0)      269 2020-12-14 21:54:51.000000 ibm-cos-sdk-2.9.0/requirements.txt
```

### Comparing `ibm-cos-sdk-2.8.0/PKG-INFO` & `ibm-cos-sdk-2.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 Metadata-Version: 2.1
 Name: ibm-cos-sdk
-Version: 2.8.0
+Version: 2.9.0
 Summary: IBM SDK for Python
 Home-page: https://github.com/ibm/ibm-cos-sdk-python
 Author: IBM
 License: Apache License 2.0
 Description: # IBM Cloud Object Storage - Python SDK
         
-        This package allows Python developers to write software that interacts
-        with [IBM Cloud Object
-        Storage](https://cloud.ibm.com/docs/services/cloud-object-storage/about-cos.html).
-        It is a fork of the [`boto3` library](https://github.com/boto/boto3) and
-        can stand as a drop-in replacement if the application needs to connect
-        to object storage using an S3-like API and does not make use of other
-        AWS services.
+        This package allows Python developers to write software that interacts with [IBM Cloud Object Storage](https://cloud.ibm.com/docs/services/cloud-object-storage/about-cos.html). It is a fork of the [`boto3` library](https://github.com/boto/boto3) and can stand as a drop-in replacement if the application needs to connect to object storage using an S3-like API and does not make use of other AWS services.
         
         ## Notice
         
-        IBM has added a [Language Support Policy](#language-support-policy). Language
-        versions will be deprecated on the published schedule without additional notice.
+        IBM has added a [Language Support Policy](#language-support-policy). Language versions will be deprecated on the published schedule without additional notice.
         
         ## Documentation
         
         * [Core documentation for IBM COS](https://cloud.ibm.com/docs/services/cloud-object-storage/getting-started.html)
         * [Python API reference documentation](https://ibm.github.io/ibm-cos-sdk-python)
         * [REST API reference documentation](https://cloud.ibm.com/docs/services/cloud-object-storage/api-reference/about-api.html)
         
@@ -32,117 +25,79 @@
         * [Getting Help](#getting-help)
         
         ## Quick start
         
         You\'ll need:
         
         * An instance of COS.
-        * An API key from [IBM Cloud Identity and Access Management](https://cloud.ibm.com/docs/iam/users_roles.html) with at
-            least `Writer` permissions.
+        * An API key from [IBM Cloud Identity and Access Management](https://cloud.ibm.com/docs/iam/users_roles.html) with at least `Writer` permissions.
         * The ID of the instance of COS that you are working with.
         * Token acquisition endpoint.
         * Service endpoint.
         
         These values can be found in the IBM Cloud Console by [generating a \'service credential\'](https://cloud.ibm.com/docs/services/cloud-object-storage/iam/service-credentials.html).
         
         ## Using Python
         
-        Use of the Python SDK and example code can be found
-        [here](https://cloud.ibm.com/docs/services/cloud-object-storage/libraries/python.html#using-python).
+        Use of the Python SDK and example code can be found [here](https://cloud.ibm.com/docs/services/cloud-object-storage/libraries/python.html#using-python).
         
         ## Using a Service Credential
         
-        You can source credentials directly from a [Service
-        Credential](https://cloud.ibm.com/docs/services/cloud-object-storage/iam/service-credentials.html)
-        JSON document generated in the IBM Cloud console saved to
-        `~/.bluemix/cos_credentials`. The SDK will automatically load these
-        providing you have not explicitly set other credentials during client
-        creation. If the Service Credential contain [HMAC
-        keys](https://cloud.ibm.com/docs/services/cloud-object-storage/hmac/credentials.html)
-        the client will use those and authenticate using a signature, otherwise
-        the client will use the provided API key to authenticate using bearer
-        tokens.
+        You can source credentials directly from a [Service Credential](https://cloud.ibm.com/docs/services/cloud-object-storage/iam/service-credentials.html) JSON document generated in the IBM Cloud console saved to `~/.bluemix/cos_credentials`. The SDK will automatically load these providing you have not explicitly set other credentials during client creation. If the Service Credential contain [HMAC keys](https://cloud.ibm.com/docs/services/cloud-object-storage/hmac/credentials.html) the client will use those and authenticate using a signature, otherwise the client will use the provided API key to authenticate using bearer tokens.
         
         ## Aspera high-speed transfer
         
-        It is now possible to use the IBM Aspera high-speed transfer service as
-        an alternative method to managed transfers of larger objects. The Aspera
-        high-speed transfer service is especially effective across long
-        distances or in environments with high rates of packet loss. For more
-        details, check out the [IBM Cloud
-        documentation](https://cloud.ibm.com/docs/services/cloud-object-storage/basics/aspera.html#using-libraries-and-sdks).
+        It is now possible to use the IBM Aspera high-speed transfer service as an alternative method to managed transfers of larger objects. The Aspera high-speed transfer service is especially effective across long distances or in environments with high rates of packet loss. For more details, check out the [IBM Cloud documentation](https://cloud.ibm.com/docs/services/cloud-object-storage/basics/aspera.html#using-libraries-and-sdks).
         
         ## Archive Tier Support
         
-        You can automatically archive objects after a specified length of time
-        or after a specified date. Once archived, a temporary copy of an object
-        can be restored for access as needed. Restore time may take up to 15
-        hours.
-        
-        An archive policy is set at the bucket level by calling the
-        `put_bucket_lifecycle_configuration` method on a client instance. A
-        newly added or modified archive policy applies to new objects uploaded
-        and does not affect existing objects. For more detail, [see the
-        documentation](https://cloud.ibm.com/docs/services/cloud-object-storage/libraries/python.html#python).
+        You can automatically archive objects after a specified length of time or after a specified date. Once archived, a temporary copy of an object can be restored for access as needed. Restore time may take up to 15 hours.
+        
+        An archive policy is set at the bucket level by calling the `put_bucket_lifecycle_configuration` method on a client instance. A newly added or modified archive policy applies to new objects uploaded and does not affect existing objects. For more detail, [see the documentation](https://cloud.ibm.com/docs/services/cloud-object-storage/libraries/python.html#python).
         
         ## Immutable Object Storage
         
-        Users can configure buckets with an Immutable Object Storage policy to
-        prevent objects from being modified or deleted for a defined period of
-        time. The retention period can be specified on a per-object basis, or
-        objects can inherit a default retention period set on the bucket. It is
-        also possible to set open-ended and permanent retention periods.
-        Immutable Object Storage meets the rules set forth by the SEC governing
-        record retention, and IBM Cloud administrators are unable to bypass
-        these restrictions. For more detail, [see the IBM Cloud
-        documentation](https://cloud.ibm.com/docs/services/cloud-object-storage/libraries/python.html#python).
+        Users can configure buckets with an Immutable Object Storage policy to prevent objects from being modified or deleted for a defined period of time. The retention period can be specified on a per-object basis, or objects can inherit a default retention period set on the bucket. It is also possible to set open-ended and permanent retention periods. Immutable Object Storage meets the rules set forth by the SEC governing record retention, and IBM Cloud administrators are unable to bypass these restrictions. For more detail, [see the IBM Cloud documentation](https://cloud.ibm.com/docs/services/cloud-object-storage/libraries/python.html#python).
         
-        Note: Immutable Object Storage does not support Aspera transfers via the
-        SDK to upload objects or directories at this stage.
+        Note: Immutable Object Storage does not support Aspera transfers via the SDK to upload objects or directories at this stage.
         
         ## Accelerated Archive
         
         Users can set an archive rule that would allow data restore from an archive in 2 hours or 12 hours.
         
         ## Building from source
         
-        Assuming that you have Python and `virtualenv` installed, set up your
-        environment and install the required dependencies like this instead of
-        the `pip install ibm-cos-sdk` defined above:
+        Assuming that you have Python and `virtualenv` installed, set up your environment and install the required dependencies like this instead of the `pip install ibm-cos-sdk` defined above:
         
         ```sh
         git clone https://github.com/ibm/ibm-cos-sdk-python.git
         cd ibm-cos-sdk-python
         $ virtualenv venv
         ...
         . venv/bin/activate
         pip install -r requirements.txt
         pip install -e .
         ```
         
         ## Getting Help
         
-        Feel free to use GitHub issues for tracking bugs and feature requests,
-        but for help please use one of the following resources:
+        Feel free to use GitHub issues for tracking bugs and feature requests, but for help please use one of the following resources:
         
         * Read a quick start guide in [IBM Cloud Docs](https://cloud.ibm.com/docs/services/cloud-object-storage/libraries/python.html#python).
-        * Ask a question on [Stack Overflow](https://stackoverflow.com/) and tag it with `ibm`
-            and `object-storage`.
+        * Ask a question on [Stack Overflow](https://stackoverflow.com/) and tag it with `ibm` and `object-storage`.
         * Open a support ticket with [IBM Cloud Support](https://cloud.ibm.com/unifiedsupport/supportcenter/)
         * If it turns out that you may have found a bug, please [open an issue](https://github.com/ibm/ibm-cos-sdk-python/issues/new).
         
         ## Language Support Policy
         
         IBM supports [current public releases](https://devguide.python.org/#status-of-python-branches). IBM will deprecate language versions 90 days after a version reaches end-of-life. All clients will need to upgrade to a supported version before the end of the grace period.
         
         ## License
         
-        This SDK is distributed under the [Apache License, Version
-        2.0](http://www.apache.org/licenses/LICENSE-2.0), see LICENSE.txt and
-        NOTICE.txt for more information.
+        This SDK is distributed under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0), see LICENSE.txt and NOTICE.txt for more information.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `ibm-cos-sdk-2.8.0/README.md` & `ibm-cos-sdk-2.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 # IBM Cloud Object Storage - Python SDK
 
-This package allows Python developers to write software that interacts
-with [IBM Cloud Object
-Storage](https://cloud.ibm.com/docs/services/cloud-object-storage/about-cos.html).
-It is a fork of the [`boto3` library](https://github.com/boto/boto3) and
-can stand as a drop-in replacement if the application needs to connect
-to object storage using an S3-like API and does not make use of other
-AWS services.
+This package allows Python developers to write software that interacts with [IBM Cloud Object Storage](https://cloud.ibm.com/docs/services/cloud-object-storage/about-cos.html). It is a fork of the [`boto3` library](https://github.com/boto/boto3) and can stand as a drop-in replacement if the application needs to connect to object storage using an S3-like API and does not make use of other AWS services.
 
 ## Notice
 
-IBM has added a [Language Support Policy](#language-support-policy). Language
-versions will be deprecated on the published schedule without additional notice.
+IBM has added a [Language Support Policy](#language-support-policy). Language versions will be deprecated on the published schedule without additional notice.
 
 ## Documentation
 
 * [Core documentation for IBM COS](https://cloud.ibm.com/docs/services/cloud-object-storage/getting-started.html)
 * [Python API reference documentation](https://ibm.github.io/ibm-cos-sdk-python)
 * [REST API reference documentation](https://cloud.ibm.com/docs/services/cloud-object-storage/api-reference/about-api.html)
 
@@ -25,110 +18,72 @@
 * [Getting Help](#getting-help)
 
 ## Quick start
 
 You\'ll need:
 
 * An instance of COS.
-* An API key from [IBM Cloud Identity and Access Management](https://cloud.ibm.com/docs/iam/users_roles.html) with at
-    least `Writer` permissions.
+* An API key from [IBM Cloud Identity and Access Management](https://cloud.ibm.com/docs/iam/users_roles.html) with at least `Writer` permissions.
 * The ID of the instance of COS that you are working with.
 * Token acquisition endpoint.
 * Service endpoint.
 
 These values can be found in the IBM Cloud Console by [generating a \'service credential\'](https://cloud.ibm.com/docs/services/cloud-object-storage/iam/service-credentials.html).
 
 ## Using Python
 
-Use of the Python SDK and example code can be found
-[here](https://cloud.ibm.com/docs/services/cloud-object-storage/libraries/python.html#using-python).
+Use of the Python SDK and example code can be found [here](https://cloud.ibm.com/docs/services/cloud-object-storage/libraries/python.html#using-python).
 
 ## Using a Service Credential
 
-You can source credentials directly from a [Service
-Credential](https://cloud.ibm.com/docs/services/cloud-object-storage/iam/service-credentials.html)
-JSON document generated in the IBM Cloud console saved to
-`~/.bluemix/cos_credentials`. The SDK will automatically load these
-providing you have not explicitly set other credentials during client
-creation. If the Service Credential contain [HMAC
-keys](https://cloud.ibm.com/docs/services/cloud-object-storage/hmac/credentials.html)
-the client will use those and authenticate using a signature, otherwise
-the client will use the provided API key to authenticate using bearer
-tokens.
+You can source credentials directly from a [Service Credential](https://cloud.ibm.com/docs/services/cloud-object-storage/iam/service-credentials.html) JSON document generated in the IBM Cloud console saved to `~/.bluemix/cos_credentials`. The SDK will automatically load these providing you have not explicitly set other credentials during client creation. If the Service Credential contain [HMAC keys](https://cloud.ibm.com/docs/services/cloud-object-storage/hmac/credentials.html) the client will use those and authenticate using a signature, otherwise the client will use the provided API key to authenticate using bearer tokens.
 
 ## Aspera high-speed transfer
 
-It is now possible to use the IBM Aspera high-speed transfer service as
-an alternative method to managed transfers of larger objects. The Aspera
-high-speed transfer service is especially effective across long
-distances or in environments with high rates of packet loss. For more
-details, check out the [IBM Cloud
-documentation](https://cloud.ibm.com/docs/services/cloud-object-storage/basics/aspera.html#using-libraries-and-sdks).
+It is now possible to use the IBM Aspera high-speed transfer service as an alternative method to managed transfers of larger objects. The Aspera high-speed transfer service is especially effective across long distances or in environments with high rates of packet loss. For more details, check out the [IBM Cloud documentation](https://cloud.ibm.com/docs/services/cloud-object-storage/basics/aspera.html#using-libraries-and-sdks).
 
 ## Archive Tier Support
 
-You can automatically archive objects after a specified length of time
-or after a specified date. Once archived, a temporary copy of an object
-can be restored for access as needed. Restore time may take up to 15
-hours.
-
-An archive policy is set at the bucket level by calling the
-`put_bucket_lifecycle_configuration` method on a client instance. A
-newly added or modified archive policy applies to new objects uploaded
-and does not affect existing objects. For more detail, [see the
-documentation](https://cloud.ibm.com/docs/services/cloud-object-storage/libraries/python.html#python).
+You can automatically archive objects after a specified length of time or after a specified date. Once archived, a temporary copy of an object can be restored for access as needed. Restore time may take up to 15 hours.
+
+An archive policy is set at the bucket level by calling the `put_bucket_lifecycle_configuration` method on a client instance. A newly added or modified archive policy applies to new objects uploaded and does not affect existing objects. For more detail, [see the documentation](https://cloud.ibm.com/docs/services/cloud-object-storage/libraries/python.html#python).
 
 ## Immutable Object Storage
 
-Users can configure buckets with an Immutable Object Storage policy to
-prevent objects from being modified or deleted for a defined period of
-time. The retention period can be specified on a per-object basis, or
-objects can inherit a default retention period set on the bucket. It is
-also possible to set open-ended and permanent retention periods.
-Immutable Object Storage meets the rules set forth by the SEC governing
-record retention, and IBM Cloud administrators are unable to bypass
-these restrictions. For more detail, [see the IBM Cloud
-documentation](https://cloud.ibm.com/docs/services/cloud-object-storage/libraries/python.html#python).
+Users can configure buckets with an Immutable Object Storage policy to prevent objects from being modified or deleted for a defined period of time. The retention period can be specified on a per-object basis, or objects can inherit a default retention period set on the bucket. It is also possible to set open-ended and permanent retention periods. Immutable Object Storage meets the rules set forth by the SEC governing record retention, and IBM Cloud administrators are unable to bypass these restrictions. For more detail, [see the IBM Cloud documentation](https://cloud.ibm.com/docs/services/cloud-object-storage/libraries/python.html#python).
 
-Note: Immutable Object Storage does not support Aspera transfers via the
-SDK to upload objects or directories at this stage.
+Note: Immutable Object Storage does not support Aspera transfers via the SDK to upload objects or directories at this stage.
 
 ## Accelerated Archive
 
 Users can set an archive rule that would allow data restore from an archive in 2 hours or 12 hours.
 
 ## Building from source
 
-Assuming that you have Python and `virtualenv` installed, set up your
-environment and install the required dependencies like this instead of
-the `pip install ibm-cos-sdk` defined above:
+Assuming that you have Python and `virtualenv` installed, set up your environment and install the required dependencies like this instead of the `pip install ibm-cos-sdk` defined above:
 
 ```sh
 git clone https://github.com/ibm/ibm-cos-sdk-python.git
 cd ibm-cos-sdk-python
 $ virtualenv venv
 ...
 . venv/bin/activate
 pip install -r requirements.txt
 pip install -e .
 ```
 
 ## Getting Help
 
-Feel free to use GitHub issues for tracking bugs and feature requests,
-but for help please use one of the following resources:
+Feel free to use GitHub issues for tracking bugs and feature requests, but for help please use one of the following resources:
 
 * Read a quick start guide in [IBM Cloud Docs](https://cloud.ibm.com/docs/services/cloud-object-storage/libraries/python.html#python).
-* Ask a question on [Stack Overflow](https://stackoverflow.com/) and tag it with `ibm`
-    and `object-storage`.
+* Ask a question on [Stack Overflow](https://stackoverflow.com/) and tag it with `ibm` and `object-storage`.
 * Open a support ticket with [IBM Cloud Support](https://cloud.ibm.com/unifiedsupport/supportcenter/)
 * If it turns out that you may have found a bug, please [open an issue](https://github.com/ibm/ibm-cos-sdk-python/issues/new).
 
 ## Language Support Policy
 
 IBM supports [current public releases](https://devguide.python.org/#status-of-python-branches). IBM will deprecate language versions 90 days after a version reaches end-of-life. All clients will need to upgrade to a supported version before the end of the grace period.
 
 ## License
 
-This SDK is distributed under the [Apache License, Version
-2.0](http://www.apache.org/licenses/LICENSE-2.0), see LICENSE.txt and
-NOTICE.txt for more information.
+This SDK is distributed under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0), see LICENSE.txt and NOTICE.txt for more information.
```

### Comparing `ibm-cos-sdk-2.8.0/ibm_cos_sdk.egg-info/PKG-INFO` & `ibm-cos-sdk-2.9.0/ibm_cos_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 Metadata-Version: 2.1
 Name: ibm-cos-sdk
-Version: 2.8.0
+Version: 2.9.0
 Summary: IBM SDK for Python
 Home-page: https://github.com/ibm/ibm-cos-sdk-python
 Author: IBM
 License: Apache License 2.0
 Description: # IBM Cloud Object Storage - Python SDK
         
-        This package allows Python developers to write software that interacts
-        with [IBM Cloud Object
-        Storage](https://cloud.ibm.com/docs/services/cloud-object-storage/about-cos.html).
-        It is a fork of the [`boto3` library](https://github.com/boto/boto3) and
-        can stand as a drop-in replacement if the application needs to connect
-        to object storage using an S3-like API and does not make use of other
-        AWS services.
+        This package allows Python developers to write software that interacts with [IBM Cloud Object Storage](https://cloud.ibm.com/docs/services/cloud-object-storage/about-cos.html). It is a fork of the [`boto3` library](https://github.com/boto/boto3) and can stand as a drop-in replacement if the application needs to connect to object storage using an S3-like API and does not make use of other AWS services.
         
         ## Notice
         
-        IBM has added a [Language Support Policy](#language-support-policy). Language
-        versions will be deprecated on the published schedule without additional notice.
+        IBM has added a [Language Support Policy](#language-support-policy). Language versions will be deprecated on the published schedule without additional notice.
         
         ## Documentation
         
         * [Core documentation for IBM COS](https://cloud.ibm.com/docs/services/cloud-object-storage/getting-started.html)
         * [Python API reference documentation](https://ibm.github.io/ibm-cos-sdk-python)
         * [REST API reference documentation](https://cloud.ibm.com/docs/services/cloud-object-storage/api-reference/about-api.html)
         
@@ -32,117 +25,79 @@
         * [Getting Help](#getting-help)
         
         ## Quick start
         
         You\'ll need:
         
         * An instance of COS.
-        * An API key from [IBM Cloud Identity and Access Management](https://cloud.ibm.com/docs/iam/users_roles.html) with at
-            least `Writer` permissions.
+        * An API key from [IBM Cloud Identity and Access Management](https://cloud.ibm.com/docs/iam/users_roles.html) with at least `Writer` permissions.
         * The ID of the instance of COS that you are working with.
         * Token acquisition endpoint.
         * Service endpoint.
         
         These values can be found in the IBM Cloud Console by [generating a \'service credential\'](https://cloud.ibm.com/docs/services/cloud-object-storage/iam/service-credentials.html).
         
         ## Using Python
         
-        Use of the Python SDK and example code can be found
-        [here](https://cloud.ibm.com/docs/services/cloud-object-storage/libraries/python.html#using-python).
+        Use of the Python SDK and example code can be found [here](https://cloud.ibm.com/docs/services/cloud-object-storage/libraries/python.html#using-python).
         
         ## Using a Service Credential
         
-        You can source credentials directly from a [Service
-        Credential](https://cloud.ibm.com/docs/services/cloud-object-storage/iam/service-credentials.html)
-        JSON document generated in the IBM Cloud console saved to
-        `~/.bluemix/cos_credentials`. The SDK will automatically load these
-        providing you have not explicitly set other credentials during client
-        creation. If the Service Credential contain [HMAC
-        keys](https://cloud.ibm.com/docs/services/cloud-object-storage/hmac/credentials.html)
-        the client will use those and authenticate using a signature, otherwise
-        the client will use the provided API key to authenticate using bearer
-        tokens.
+        You can source credentials directly from a [Service Credential](https://cloud.ibm.com/docs/services/cloud-object-storage/iam/service-credentials.html) JSON document generated in the IBM Cloud console saved to `~/.bluemix/cos_credentials`. The SDK will automatically load these providing you have not explicitly set other credentials during client creation. If the Service Credential contain [HMAC keys](https://cloud.ibm.com/docs/services/cloud-object-storage/hmac/credentials.html) the client will use those and authenticate using a signature, otherwise the client will use the provided API key to authenticate using bearer tokens.
         
         ## Aspera high-speed transfer
         
-        It is now possible to use the IBM Aspera high-speed transfer service as
-        an alternative method to managed transfers of larger objects. The Aspera
-        high-speed transfer service is especially effective across long
-        distances or in environments with high rates of packet loss. For more
-        details, check out the [IBM Cloud
-        documentation](https://cloud.ibm.com/docs/services/cloud-object-storage/basics/aspera.html#using-libraries-and-sdks).
+        It is now possible to use the IBM Aspera high-speed transfer service as an alternative method to managed transfers of larger objects. The Aspera high-speed transfer service is especially effective across long distances or in environments with high rates of packet loss. For more details, check out the [IBM Cloud documentation](https://cloud.ibm.com/docs/services/cloud-object-storage/basics/aspera.html#using-libraries-and-sdks).
         
         ## Archive Tier Support
         
-        You can automatically archive objects after a specified length of time
-        or after a specified date. Once archived, a temporary copy of an object
-        can be restored for access as needed. Restore time may take up to 15
-        hours.
-        
-        An archive policy is set at the bucket level by calling the
-        `put_bucket_lifecycle_configuration` method on a client instance. A
-        newly added or modified archive policy applies to new objects uploaded
-        and does not affect existing objects. For more detail, [see the
-        documentation](https://cloud.ibm.com/docs/services/cloud-object-storage/libraries/python.html#python).
+        You can automatically archive objects after a specified length of time or after a specified date. Once archived, a temporary copy of an object can be restored for access as needed. Restore time may take up to 15 hours.
+        
+        An archive policy is set at the bucket level by calling the `put_bucket_lifecycle_configuration` method on a client instance. A newly added or modified archive policy applies to new objects uploaded and does not affect existing objects. For more detail, [see the documentation](https://cloud.ibm.com/docs/services/cloud-object-storage/libraries/python.html#python).
         
         ## Immutable Object Storage
         
-        Users can configure buckets with an Immutable Object Storage policy to
-        prevent objects from being modified or deleted for a defined period of
-        time. The retention period can be specified on a per-object basis, or
-        objects can inherit a default retention period set on the bucket. It is
-        also possible to set open-ended and permanent retention periods.
-        Immutable Object Storage meets the rules set forth by the SEC governing
-        record retention, and IBM Cloud administrators are unable to bypass
-        these restrictions. For more detail, [see the IBM Cloud
-        documentation](https://cloud.ibm.com/docs/services/cloud-object-storage/libraries/python.html#python).
+        Users can configure buckets with an Immutable Object Storage policy to prevent objects from being modified or deleted for a defined period of time. The retention period can be specified on a per-object basis, or objects can inherit a default retention period set on the bucket. It is also possible to set open-ended and permanent retention periods. Immutable Object Storage meets the rules set forth by the SEC governing record retention, and IBM Cloud administrators are unable to bypass these restrictions. For more detail, [see the IBM Cloud documentation](https://cloud.ibm.com/docs/services/cloud-object-storage/libraries/python.html#python).
         
-        Note: Immutable Object Storage does not support Aspera transfers via the
-        SDK to upload objects or directories at this stage.
+        Note: Immutable Object Storage does not support Aspera transfers via the SDK to upload objects or directories at this stage.
         
         ## Accelerated Archive
         
         Users can set an archive rule that would allow data restore from an archive in 2 hours or 12 hours.
         
         ## Building from source
         
-        Assuming that you have Python and `virtualenv` installed, set up your
-        environment and install the required dependencies like this instead of
-        the `pip install ibm-cos-sdk` defined above:
+        Assuming that you have Python and `virtualenv` installed, set up your environment and install the required dependencies like this instead of the `pip install ibm-cos-sdk` defined above:
         
         ```sh
         git clone https://github.com/ibm/ibm-cos-sdk-python.git
         cd ibm-cos-sdk-python
         $ virtualenv venv
         ...
         . venv/bin/activate
         pip install -r requirements.txt
         pip install -e .
         ```
         
         ## Getting Help
         
-        Feel free to use GitHub issues for tracking bugs and feature requests,
-        but for help please use one of the following resources:
+        Feel free to use GitHub issues for tracking bugs and feature requests, but for help please use one of the following resources:
         
         * Read a quick start guide in [IBM Cloud Docs](https://cloud.ibm.com/docs/services/cloud-object-storage/libraries/python.html#python).
-        * Ask a question on [Stack Overflow](https://stackoverflow.com/) and tag it with `ibm`
-            and `object-storage`.
+        * Ask a question on [Stack Overflow](https://stackoverflow.com/) and tag it with `ibm` and `object-storage`.
         * Open a support ticket with [IBM Cloud Support](https://cloud.ibm.com/unifiedsupport/supportcenter/)
         * If it turns out that you may have found a bug, please [open an issue](https://github.com/ibm/ibm-cos-sdk-python/issues/new).
         
         ## Language Support Policy
         
         IBM supports [current public releases](https://devguide.python.org/#status-of-python-branches). IBM will deprecate language versions 90 days after a version reaches end-of-life. All clients will need to upgrade to a supported version before the end of the grace period.
         
         ## License
         
-        This SDK is distributed under the [Apache License, Version
-        2.0](http://www.apache.org/licenses/LICENSE-2.0), see LICENSE.txt and
-        NOTICE.txt for more information.
+        This SDK is distributed under the [Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0), see LICENSE.txt and NOTICE.txt for more information.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `ibm-cos-sdk-2.8.0/ibm_cos_sdk.egg-info/SOURCES.txt` & `ibm-cos-sdk-2.9.0/ibm_cos_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/LICENSE` & `ibm-cos-sdk-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/__init__.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import logging
 
 from ibm_boto3.session import Session
 
 
 __author__ = 'IBM'
-__version__ = '2.8.0'
+__version__ = '2.9.0'
 
 
 # The default Boto3 session; autoloaded when needed.
 DEFAULT_SESSION = None
 
 
 def setup_default_session(**kwargs):
```

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/compat.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/compat.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/s3/__init__.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/s3/transfer.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/s3/transfer.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/s3/inject.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/s3/inject.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/session.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/session.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/exceptions.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/exceptions.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/data/s3/2006-03-01/resources-1.json` & `ibm-cos-sdk-2.9.0/ibm_boto3/data/s3/2006-03-01/resources-1.json`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/utils.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/utils.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/resources/collection.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/resources/collection.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/resources/action.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/resources/action.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/resources/base.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/resources/base.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/resources/factory.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/resources/factory.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/resources/model.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/resources/model.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/resources/response.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/resources/response.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/resources/params.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/resources/params.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/docs/collection.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/docs/collection.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/docs/__init__.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/docs/action.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/docs/action.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/docs/docstring.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/docs/docstring.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/docs/waiter.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/docs/waiter.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/docs/base.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/docs/base.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/docs/attr.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/docs/attr.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/docs/method.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/docs/method.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/docs/resource.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/docs/resource.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/docs/service.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/docs/service.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/docs/utils.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/docs/utils.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/docs/client.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/docs/client.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/ibm_boto3/docs/subresource.py` & `ibm-cos-sdk-2.9.0/ibm_boto3/docs/subresource.py`

 * *Files identical despite different names*

### Comparing `ibm-cos-sdk-2.8.0/setup.py` & `ibm-cos-sdk-2.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from setuptools import setup, find_packages
 
 ROOT = os.path.dirname(__file__)
 VERSION_RE = re.compile(r'''__version__ = ['"]([a-z0-9.]+)['"]''')
 
 
 requires = [
-    'ibm-cos-sdk-core==2.8.0',
-    'ibm-cos-sdk-s3transfer==2.8.0',
+    'ibm-cos-sdk-core==2.9.0',
+    'ibm-cos-sdk-s3transfer==2.9.0',
     'jmespath>=0.7.1,<1.0.0'
 ]
 
 
 def get_version():
     init = open(os.path.join(ROOT, 'ibm_boto3', '__init__.py')).read()
     return VERSION_RE.search(init).group(1)
```

