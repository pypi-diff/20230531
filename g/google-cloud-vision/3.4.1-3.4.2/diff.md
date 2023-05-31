# Comparing `tmp/google-cloud-vision-3.4.1.tar.gz` & `tmp/google-cloud-vision-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-vision-3.4.1.tar", last modified: Mon Mar 27 15:52:30 2023, max compression
+gzip compressed data, was "google-cloud-vision-3.4.2.tar", last modified: Wed May 31 20:49:38 2023, max compression
```

## Comparing `google-cloud-vision-3.4.1.tar` & `google-cloud-vision-3.4.2.tar`

### file list

```diff
@@ -1,210 +1,210 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.401527 google-cloud-vision-3.4.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5881 2023-03-27 15:52:30.401527 google-cloud-vision-3.4.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4968 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.361518 google-cloud-vision-3.4.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.365519 google-cloud-vision-3.4.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.369520 google-cloud-vision-3.4.1/google/cloud/vision/
--rw-rw-r--   0 root         (0)     1003    10158 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.369520 google-cloud-vision-3.4.1/google/cloud/vision_helpers/
--rw-rw-r--   0 root         (0)     1003     3638 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_helpers/__init__.py
--rw-rw-r--   0 root         (0)     1003     4181 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_helpers/decorators.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.369520 google-cloud-vision-3.4.1/google/cloud/vision_v1/
--rw-rw-r--   0 root         (0)     1003     8417 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    10150 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.369520 google-cloud-vision-3.4.1/google/cloud/vision_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.369520 google-cloud-vision-3.4.1/google/cloud/vision_v1/services/image_annotator/
--rw-rw-r--   0 root         (0)     1003      769 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/services/image_annotator/__init__.py
--rw-rw-r--   0 root         (0)     1003    30191 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/services/image_annotator/async_client.py
--rw-rw-r--   0 root         (0)     1003    39745 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/services/image_annotator/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.369520 google-cloud-vision-3.4.1/google/cloud/vision_v1/services/image_annotator/transports/
--rw-rw-r--   0 root         (0)     1003     1418 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/services/image_annotator/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9543 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/services/image_annotator/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17763 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/services/image_annotator/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18097 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/services/image_annotator/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    33053 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/services/image_annotator/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.373521 google-cloud-vision-3.4.1/google/cloud/vision_v1/services/product_search/
--rw-rw-r--   0 root         (0)     1003      765 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/services/product_search/__init__.py
--rw-rw-r--   0 root         (0)     1003   110841 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/services/product_search/async_client.py
--rw-rw-r--   0 root         (0)     1003   118546 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/services/product_search/client.py
--rw-rw-r--   0 root         (0)     1003    21786 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/services/product_search/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.373521 google-cloud-vision-3.4.1/google/cloud/vision_v1/services/product_search/transports/
--rw-rw-r--   0 root         (0)     1003     1404 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/services/product_search/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    22251 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/services/product_search/transports/base.py
--rw-rw-r--   0 root         (0)     1003    41006 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/services/product_search/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    41751 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/services/product_search/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   106831 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/services/product_search/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.373521 google-cloud-vision-3.4.1/google/cloud/vision_v1/types/
--rw-rw-r--   0 root         (0)     1003     5104 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3163 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/types/geometry.py
--rw-rw-r--   0 root         (0)     1003    57369 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/types/image_annotator.py
--rw-rw-r--   0 root         (0)     1003     8095 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/types/product_search.py
--rw-rw-r--   0 root         (0)     1003    34296 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/types/product_search_service.py
--rw-rw-r--   0 root         (0)     1003    14108 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/types/text_annotation.py
--rw-rw-r--   0 root         (0)     1003     6798 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1/types/web_detection.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.373521 google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/
--rw-rw-r--   0 root         (0)     1003     3530 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1073 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.377522 google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.377522 google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/services/image_annotator/
--rw-rw-r--   0 root         (0)     1003      769 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/services/image_annotator/__init__.py
--rw-rw-r--   0 root         (0)     1003    13774 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/services/image_annotator/async_client.py
--rw-rw-r--   0 root         (0)     1003    22190 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/services/image_annotator/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.377522 google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/services/image_annotator/transports/
--rw-rw-r--   0 root         (0)     1003     1418 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/services/image_annotator/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6594 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/services/image_annotator/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12086 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    12291 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    12849 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/services/image_annotator/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.377522 google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/types/
--rw-rw-r--   0 root         (0)     1003     2054 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2372 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/types/geometry.py
--rw-rw-r--   0 root         (0)     1003    36850 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/types/image_annotator.py
--rw-rw-r--   0 root         (0)     1003    13946 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/types/text_annotation.py
--rw-rw-r--   0 root         (0)     1003     6774 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/types/web_detection.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.377522 google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/
--rw-rw-r--   0 root         (0)     1003     4513 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1505 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.377522 google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.377522 google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/services/image_annotator/
--rw-rw-r--   0 root         (0)     1003      769 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/services/image_annotator/__init__.py
--rw-rw-r--   0 root         (0)     1003    19293 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/services/image_annotator/async_client.py
--rw-rw-r--   0 root         (0)     1003    27703 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/services/image_annotator/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.381523 google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/services/image_annotator/transports/
--rw-rw-r--   0 root         (0)     1003     1418 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/services/image_annotator/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7741 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/services/image_annotator/transports/base.py
--rw-rw-r--   0 root         (0)     1003    14438 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14719 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    19695 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/services/image_annotator/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.381523 google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/types/
--rw-rw-r--   0 root         (0)     1003     2684 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3184 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/types/geometry.py
--rw-rw-r--   0 root         (0)     1003    47056 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/types/image_annotator.py
--rw-rw-r--   0 root         (0)     1003    14255 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/types/text_annotation.py
--rw-rw-r--   0 root         (0)     1003     6774 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/types/web_detection.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.381523 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/
--rw-rw-r--   0 root         (0)     1003     7754 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8961 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.381523 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.381523 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/image_annotator/
--rw-rw-r--   0 root         (0)     1003      769 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/image_annotator/__init__.py
--rw-rw-r--   0 root         (0)     1003    19480 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/image_annotator/async_client.py
--rw-rw-r--   0 root         (0)     1003    29175 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/image_annotator/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.385524 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/image_annotator/transports/
--rw-rw-r--   0 root         (0)     1003     1418 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/image_annotator/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7602 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/image_annotator/transports/base.py
--rw-rw-r--   0 root         (0)     1003    14454 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14735 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    19695 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/image_annotator/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.385524 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/product_search/
--rw-rw-r--   0 root         (0)     1003      765 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/product_search/__init__.py
--rw-rw-r--   0 root         (0)     1003   104793 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/product_search/async_client.py
--rw-rw-r--   0 root         (0)     1003   113091 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/product_search/client.py
--rw-rw-r--   0 root         (0)     1003    22017 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/product_search/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.385524 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/product_search/transports/
--rw-rw-r--   0 root         (0)     1003     1404 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/product_search/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    21005 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/product_search/transports/base.py
--rw-rw-r--   0 root         (0)     1003    39061 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    39775 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   100971 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/product_search/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.385524 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/types/
--rw-rw-r--   0 root         (0)     1003     4658 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3184 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/types/geometry.py
--rw-rw-r--   0 root         (0)     1003    49756 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/types/image_annotator.py
--rw-rw-r--   0 root         (0)     1003     8172 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/types/product_search.py
--rw-rw-r--   0 root         (0)     1003    31431 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/types/product_search_service.py
--rw-rw-r--   0 root         (0)     1003    14255 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/types/text_annotation.py
--rw-rw-r--   0 root         (0)     1003     6774 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/types/web_detection.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.389525 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/
--rw-rw-r--   0 root         (0)     1003     8625 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    10164 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.389525 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.389525 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/image_annotator/
--rw-rw-r--   0 root         (0)     1003      769 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/image_annotator/__init__.py
--rw-rw-r--   0 root         (0)     1003    29872 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/image_annotator/async_client.py
--rw-rw-r--   0 root         (0)     1003    39934 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/image_annotator/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.389525 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/image_annotator/transports/
--rw-rw-r--   0 root         (0)     1003     1418 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/image_annotator/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9001 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/image_annotator/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17798 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18132 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    30869 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/image_annotator/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.389525 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/product_search/
--rw-rw-r--   0 root         (0)     1003      765 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/product_search/__init__.py
--rw-rw-r--   0 root         (0)     1003   110849 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/product_search/async_client.py
--rw-rw-r--   0 root         (0)     1003   119297 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/product_search/client.py
--rw-rw-r--   0 root         (0)     1003    22017 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/product_search/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.393525 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/product_search/transports/
--rw-rw-r--   0 root         (0)     1003     1404 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/product_search/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    21446 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/product_search/transports/base.py
--rw-rw-r--   0 root         (0)     1003    41195 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    41940 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   106302 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/product_search/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.393525 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/types/
--rw-rw-r--   0 root         (0)     1003     5270 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2803 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/types/face.py
--rw-rw-r--   0 root         (0)     1003     3184 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/types/geometry.py
--rw-rw-r--   0 root         (0)     1003    56382 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/types/image_annotator.py
--rw-rw-r--   0 root         (0)     1003     8172 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/types/product_search.py
--rw-rw-r--   0 root         (0)     1003    34408 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/types/product_search_service.py
--rw-rw-r--   0 root         (0)     1003    14255 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/types/text_annotation.py
--rw-rw-r--   0 root         (0)     1003     6861 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/types/web_detection.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.393525 google-cloud-vision-3.4.1/google_cloud_vision.egg-info/
--rw-r--r--   0 root         (0)     1003     5881 2023-03-27 15:52:30.000000 google-cloud-vision-3.4.1/google_cloud_vision.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     8892 2023-03-27 15:52:30.000000 google-cloud-vision-3.4.1/google_cloud_vision.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:52:30.000000 google-cloud-vision-3.4.1/google_cloud_vision.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 15:52:30.000000 google-cloud-vision-3.4.1/google_cloud_vision.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:52:30.000000 google-cloud-vision-3.4.1/google_cloud_vision.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 15:52:30.000000 google-cloud-vision-3.4.1/google_cloud_vision.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:52:30.000000 google-cloud-vision-3.4.1/google_cloud_vision.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:52:30.401527 google-cloud-vision-3.4.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2917 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.393525 google-cloud-vision-3.4.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.397526 google-cloud-vision-3.4.1/tests/data/
--rw-rw-r--   0 root         (0)     1003   283497 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/tests/data/faces.jpg
--rw-rw-r--   0 root         (0)     1003    21568 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/tests/data/logo.png
--rw-rw-r--   0 root         (0)     1003    15615 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/tests/data/pdf_test.pdf
--rw-rw-r--   0 root         (0)     1003    38159 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/tests/system.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.397526 google-cloud-vision-3.4.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.397526 google-cloud-vision-3.4.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.397526 google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   127996 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1/test_image_annotator.py
--rw-rw-r--   0 root         (0)     1003   460770 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1/test_product_search.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.397526 google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    70208 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p1beta1/test_image_annotator.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.401527 google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p2beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p2beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    90057 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p2beta1/test_image_annotator.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.401527 google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p3beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p3beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    91693 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p3beta1/test_image_annotator.py
--rw-rw-r--   0 root         (0)     1003   443181 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p3beta1/test_product_search.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:52:30.401527 google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p4beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p4beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   128156 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p4beta1/test_image_annotator.py
--rw-rw-r--   0 root         (0)     1003   461030 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p4beta1/test_product_search.py
--rw-rw-r--   0 root         (0)     1003     4068 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/tests/unit/test_decorators.py
--rw-rw-r--   0 root         (0)     1003     5105 2023-03-27 15:50:01.000000 google-cloud-vision-3.4.1/tests/unit/test_helpers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.287655 google-cloud-vision-3.4.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5881 2023-05-31 20:49:38.287655 google-cloud-vision-3.4.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4968 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.243637 google-cloud-vision-3.4.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.247639 google-cloud-vision-3.4.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.251640 google-cloud-vision-3.4.2/google/cloud/vision/
+-rw-rw-r--   0 root         (0)     1003    10158 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.251640 google-cloud-vision-3.4.2/google/cloud/vision_helpers/
+-rw-rw-r--   0 root         (0)     1003     3638 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_helpers/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4181 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_helpers/decorators.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.251640 google-cloud-vision-3.4.2/google/cloud/vision_v1/
+-rw-rw-r--   0 root         (0)     1003     8417 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10150 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.251640 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.251640 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/
+-rw-rw-r--   0 root         (0)     1003      769 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/__init__.py
+-rw-rw-r--   0 root         (0)     1003    30191 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/async_client.py
+-rw-rw-r--   0 root         (0)     1003    39070 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.255642 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/transports/
+-rw-rw-r--   0 root         (0)     1003     1418 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9543 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17763 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18097 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    33053 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.255642 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/
+-rw-rw-r--   0 root         (0)     1003      765 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/__init__.py
+-rw-rw-r--   0 root         (0)     1003   110841 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/async_client.py
+-rw-rw-r--   0 root         (0)     1003   118546 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/client.py
+-rw-rw-r--   0 root         (0)     1003    21786 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.255642 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/transports/
+-rw-rw-r--   0 root         (0)     1003     1404 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22251 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    41006 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    41751 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   106831 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.259644 google-cloud-vision-3.4.2/google/cloud/vision_v1/types/
+-rw-rw-r--   0 root         (0)     1003     5104 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3163 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/types/geometry.py
+-rw-rw-r--   0 root         (0)     1003    57369 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/types/image_annotator.py
+-rw-rw-r--   0 root         (0)     1003     8095 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/types/product_search.py
+-rw-rw-r--   0 root         (0)     1003    34296 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/types/product_search_service.py
+-rw-rw-r--   0 root         (0)     1003    14108 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/types/text_annotation.py
+-rw-rw-r--   0 root         (0)     1003     6798 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1/types/web_detection.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.259644 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/
+-rw-rw-r--   0 root         (0)     1003     3530 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1073 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.259644 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.259644 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/
+-rw-rw-r--   0 root         (0)     1003      769 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13774 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/async_client.py
+-rw-rw-r--   0 root         (0)     1003    22022 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.259644 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/transports/
+-rw-rw-r--   0 root         (0)     1003     1418 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6594 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12086 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    12291 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    12849 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.259644 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     2054 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2372 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/types/geometry.py
+-rw-rw-r--   0 root         (0)     1003    36850 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/types/image_annotator.py
+-rw-rw-r--   0 root         (0)     1003    13946 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/types/text_annotation.py
+-rw-rw-r--   0 root         (0)     1003     6774 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/types/web_detection.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.263645 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/
+-rw-rw-r--   0 root         (0)     1003     4513 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1505 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.263645 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.263645 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/
+-rw-rw-r--   0 root         (0)     1003      769 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19293 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/async_client.py
+-rw-rw-r--   0 root         (0)     1003    27363 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.263645 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/transports/
+-rw-rw-r--   0 root         (0)     1003     1418 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7741 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    14438 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14719 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    19695 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.263645 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/types/
+-rw-rw-r--   0 root         (0)     1003     2684 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3184 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/types/geometry.py
+-rw-rw-r--   0 root         (0)     1003    47056 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/types/image_annotator.py
+-rw-rw-r--   0 root         (0)     1003    14255 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/types/text_annotation.py
+-rw-rw-r--   0 root         (0)     1003     6774 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/types/web_detection.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.263645 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/
+-rw-rw-r--   0 root         (0)     1003     7754 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8961 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.263645 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.267647 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/
+-rw-rw-r--   0 root         (0)     1003      769 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19480 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28835 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.267647 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/transports/
+-rw-rw-r--   0 root         (0)     1003     1418 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7602 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    14454 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14735 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    19695 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.267647 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/
+-rw-rw-r--   0 root         (0)     1003      765 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/__init__.py
+-rw-rw-r--   0 root         (0)     1003   104793 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/async_client.py
+-rw-rw-r--   0 root         (0)     1003   113091 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/client.py
+-rw-rw-r--   0 root         (0)     1003    22017 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.267647 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/transports/
+-rw-rw-r--   0 root         (0)     1003     1404 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21005 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    39061 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    39775 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   100971 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.271648 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/
+-rw-rw-r--   0 root         (0)     1003     4658 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3184 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/geometry.py
+-rw-rw-r--   0 root         (0)     1003    49756 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/image_annotator.py
+-rw-rw-r--   0 root         (0)     1003     8172 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/product_search.py
+-rw-rw-r--   0 root         (0)     1003    31431 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/product_search_service.py
+-rw-rw-r--   0 root         (0)     1003    14255 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/text_annotation.py
+-rw-rw-r--   0 root         (0)     1003     6774 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/web_detection.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.271648 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/
+-rw-rw-r--   0 root         (0)     1003     8625 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10164 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.271648 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.271648 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/
+-rw-rw-r--   0 root         (0)     1003      769 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/__init__.py
+-rw-rw-r--   0 root         (0)     1003    29872 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/async_client.py
+-rw-rw-r--   0 root         (0)     1003    39259 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.275650 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/transports/
+-rw-rw-r--   0 root         (0)     1003     1418 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9001 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17798 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18132 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    30869 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.275650 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/
+-rw-rw-r--   0 root         (0)     1003      765 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/__init__.py
+-rw-rw-r--   0 root         (0)     1003   110849 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/async_client.py
+-rw-rw-r--   0 root         (0)     1003   119297 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/client.py
+-rw-rw-r--   0 root         (0)     1003    22017 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.275650 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/transports/
+-rw-rw-r--   0 root         (0)     1003     1404 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21446 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    41195 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    41940 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   106302 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.279651 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/
+-rw-rw-r--   0 root         (0)     1003     5270 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2803 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/face.py
+-rw-rw-r--   0 root         (0)     1003     3184 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/geometry.py
+-rw-rw-r--   0 root         (0)     1003    56382 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/image_annotator.py
+-rw-rw-r--   0 root         (0)     1003     8172 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/product_search.py
+-rw-rw-r--   0 root         (0)     1003    34408 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/product_search_service.py
+-rw-rw-r--   0 root         (0)     1003    14255 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/text_annotation.py
+-rw-rw-r--   0 root         (0)     1003     6861 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/web_detection.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.279651 google-cloud-vision-3.4.2/google_cloud_vision.egg-info/
+-rw-r--r--   0 root         (0)     1003     5881 2023-05-31 20:49:38.000000 google-cloud-vision-3.4.2/google_cloud_vision.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     8892 2023-05-31 20:49:38.000000 google-cloud-vision-3.4.2/google_cloud_vision.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-31 20:49:38.000000 google-cloud-vision-3.4.2/google_cloud_vision.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-05-31 20:49:38.000000 google-cloud-vision-3.4.2/google_cloud_vision.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-31 20:49:38.000000 google-cloud-vision-3.4.2/google_cloud_vision.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-05-31 20:49:38.000000 google-cloud-vision-3.4.2/google_cloud_vision.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-05-31 20:49:38.000000 google-cloud-vision-3.4.2/google_cloud_vision.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-05-31 20:49:38.287655 google-cloud-vision-3.4.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2917 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.279651 google-cloud-vision-3.4.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.279651 google-cloud-vision-3.4.2/tests/data/
+-rw-rw-r--   0 root         (0)     1003   283497 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/data/faces.jpg
+-rw-rw-r--   0 root         (0)     1003    21568 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/data/logo.png
+-rw-rw-r--   0 root         (0)     1003    15615 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/data/pdf_test.pdf
+-rw-rw-r--   0 root         (0)     1003    38159 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/system.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.279651 google-cloud-vision-3.4.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.279651 google-cloud-vision-3.4.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.283653 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   127996 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1/test_image_annotator.py
+-rw-rw-r--   0 root         (0)     1003   460770 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1/test_product_search.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.283653 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    70208 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p1beta1/test_image_annotator.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.283653 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p2beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p2beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    90057 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p2beta1/test_image_annotator.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.283653 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p3beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p3beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    91693 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p3beta1/test_image_annotator.py
+-rw-rw-r--   0 root         (0)     1003   443181 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p3beta1/test_product_search.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-31 20:49:38.283653 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p4beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p4beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   128156 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p4beta1/test_image_annotator.py
+-rw-rw-r--   0 root         (0)     1003   461030 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p4beta1/test_product_search.py
+-rw-rw-r--   0 root         (0)     1003     4068 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/test_decorators.py
+-rw-rw-r--   0 root         (0)     1003     5105 2023-05-31 20:46:56.000000 google-cloud-vision-3.4.2/tests/unit/test_helpers.py
```

### Comparing `google-cloud-vision-3.4.1/LICENSE` & `google-cloud-vision-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/MANIFEST.in` & `google-cloud-vision-3.4.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/PKG-INFO` & `google-cloud-vision-3.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-vision
-Version: 3.4.1
+Version: 3.4.2
 Summary: Google Cloud Vision API client library
 Home-page: https://github.com/googleapis/python-vision
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-vision-3.4.1/README.rst` & `google-cloud-vision-3.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision/gapic_version.py` & `google-cloud-vision-3.4.2/google/cloud/vision/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "3.4.1"  # {x-release-please-version}
+__version__ = "3.4.2"  # {x-release-please-version}
```

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_helpers/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_helpers/decorators.py` & `google-cloud-vision-3.4.2/google/cloud/vision_helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/gapic_metadata.json` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/gapic_version.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "3.4.1"  # {x-release-please-version}
+__version__ = "3.4.2"  # {x-release-please-version}
```

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/services/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/services/image_annotator/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/services/image_annotator/async_client.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/services/image_annotator/client.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -547,17 +547,14 @@
 
         # Minor optimization to avoid making a copy if the user passes
         # in a image_annotator.BatchAnnotateImagesRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
         if not isinstance(request, image_annotator.BatchAnnotateImagesRequest):
             request = image_annotator.BatchAnnotateImagesRequest(request)
-            if requests is not None:
-                for i in range(len(requests)):
-                    requests[i] = image_annotator.AnnotateImageRequest(requests[i])
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if requests is not None:
                 request.requests = requests
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
@@ -654,17 +651,14 @@
 
         # Minor optimization to avoid making a copy if the user passes
         # in a image_annotator.BatchAnnotateFilesRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
         if not isinstance(request, image_annotator.BatchAnnotateFilesRequest):
             request = image_annotator.BatchAnnotateFilesRequest(request)
-            if requests is not None:
-                for i in range(len(requests)):
-                    requests[i] = image_annotator.AnnotateFileRequest(requests[i])
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if requests is not None:
                 request.requests = requests
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
@@ -782,17 +776,14 @@
 
         # Minor optimization to avoid making a copy if the user passes
         # in a image_annotator.AsyncBatchAnnotateImagesRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
         if not isinstance(request, image_annotator.AsyncBatchAnnotateImagesRequest):
             request = image_annotator.AsyncBatchAnnotateImagesRequest(request)
-            if requests is not None:
-                for i in range(len(requests)):
-                    requests[i] = image_annotator.AnnotateImageRequest(requests[i])
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if requests is not None:
                 request.requests = requests
             if output_config is not None:
                 request.output_config = output_config
 
@@ -910,17 +901,14 @@
 
         # Minor optimization to avoid making a copy if the user passes
         # in a image_annotator.AsyncBatchAnnotateFilesRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
         if not isinstance(request, image_annotator.AsyncBatchAnnotateFilesRequest):
             request = image_annotator.AsyncBatchAnnotateFilesRequest(request)
-            if requests is not None:
-                for i in range(len(requests)):
-                    requests[i] = image_annotator.AsyncAnnotateFileRequest(requests[i])
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if requests is not None:
                 request.requests = requests
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
```

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/services/image_annotator/transports/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/services/image_annotator/transports/base.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/services/image_annotator/transports/grpc.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/services/image_annotator/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/services/image_annotator/transports/rest.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/image_annotator/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/services/product_search/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/services/product_search/async_client.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/services/product_search/client.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/services/product_search/pagers.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/services/product_search/transports/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/services/product_search/transports/base.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/services/product_search/transports/grpc.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/services/product_search/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/services/product_search/transports/rest.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/services/product_search/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/types/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/types/geometry.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/types/geometry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/types/image_annotator.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/types/image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/types/product_search.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/types/product_search.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/types/product_search_service.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/types/product_search_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/types/text_annotation.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/types/text_annotation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1/types/web_detection.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1/types/web_detection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/gapic_metadata.json` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/gapic_version.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "3.4.1"  # {x-release-please-version}
+__version__ = "3.4.2"  # {x-release-please-version}
```

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/services/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/services/image_annotator/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/services/image_annotator/async_client.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/services/image_annotator/client.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -499,17 +499,14 @@
 
         # Minor optimization to avoid making a copy if the user passes
         # in a image_annotator.BatchAnnotateImagesRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
         if not isinstance(request, image_annotator.BatchAnnotateImagesRequest):
             request = image_annotator.BatchAnnotateImagesRequest(request)
-            if requests is not None:
-                for i in range(len(requests)):
-                    requests[i] = image_annotator.AnnotateImageRequest(requests[i])
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if requests is not None:
                 request.requests = requests
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
```

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/services/image_annotator/transports/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/services/image_annotator/transports/base.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/services/image_annotator/transports/rest.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/services/image_annotator/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/types/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/types/geometry.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/types/geometry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/types/image_annotator.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/types/image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/types/text_annotation.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/types/text_annotation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p1beta1/types/web_detection.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p1beta1/types/web_detection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/gapic_metadata.json` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/gapic_version.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "3.4.1"  # {x-release-please-version}
+__version__ = "3.4.2"  # {x-release-please-version}
```

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/services/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/services/image_annotator/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/services/image_annotator/async_client.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/services/image_annotator/client.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     Sequence,
     Tuple,
     Type,
     Union,
     cast,
 )
 
-from google.cloud.vision_v1p2beta1 import gapic_version as package_version
+from google.cloud.vision_v1p3beta1 import gapic_version as package_version
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport import mtls  # type: ignore
@@ -44,15 +44,15 @@
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
-from google.cloud.vision_v1p2beta1.types import image_annotator
+from google.cloud.vision_v1p3beta1.types import image_annotator
 from .transports.base import ImageAnnotatorTransport, DEFAULT_CLIENT_INFO
 from .transports.grpc import ImageAnnotatorGrpcTransport
 from .transports.grpc_asyncio import ImageAnnotatorGrpcAsyncIOTransport
 from .transports.rest import ImageAnnotatorRestTransport
 
 
 class ImageAnnotatorClientMeta(type):
@@ -178,14 +178,60 @@
         Returns:
             ImageAnnotatorTransport: The transport used by the client
                 instance.
         """
         return self._transport
 
     @staticmethod
+    def product_path(
+        project: str,
+        location: str,
+        product: str,
+    ) -> str:
+        """Returns a fully-qualified product string."""
+        return "projects/{project}/locations/{location}/products/{product}".format(
+            project=project,
+            location=location,
+            product=product,
+        )
+
+    @staticmethod
+    def parse_product_path(path: str) -> Dict[str, str]:
+        """Parses a product path into its component segments."""
+        m = re.match(
+            r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)/products/(?P<product>.+?)$",
+            path,
+        )
+        return m.groupdict() if m else {}
+
+    @staticmethod
+    def product_set_path(
+        project: str,
+        location: str,
+        product_set: str,
+    ) -> str:
+        """Returns a fully-qualified product_set string."""
+        return (
+            "projects/{project}/locations/{location}/productSets/{product_set}".format(
+                project=project,
+                location=location,
+                product_set=product_set,
+            )
+        )
+
+    @staticmethod
+    def parse_product_set_path(path: str) -> Dict[str, str]:
+        """Parses a product_set path into its component segments."""
+        m = re.match(
+            r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)/productSets/(?P<product_set>.+?)$",
+            path,
+        )
+        return m.groupdict() if m else {}
+
+    @staticmethod
     def common_billing_account_path(
         billing_account: str,
     ) -> str:
         """Returns a fully-qualified billing_account string."""
         return "billingAccounts/{billing_account}".format(
             billing_account=billing_account,
         )
@@ -446,49 +492,49 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import vision_v1p2beta1
+            from google.cloud import vision_v1p3beta1
 
             def sample_batch_annotate_images():
                 # Create a client
-                client = vision_v1p2beta1.ImageAnnotatorClient()
+                client = vision_v1p3beta1.ImageAnnotatorClient()
 
                 # Initialize request argument(s)
-                request = vision_v1p2beta1.BatchAnnotateImagesRequest(
+                request = vision_v1p3beta1.BatchAnnotateImagesRequest(
                 )
 
                 # Make the request
                 response = client.batch_annotate_images(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.vision_v1p2beta1.types.BatchAnnotateImagesRequest, dict]):
+            request (Union[google.cloud.vision_v1p3beta1.types.BatchAnnotateImagesRequest, dict]):
                 The request object. Multiple image annotation requests
                 are batched into a single service call.
-            requests (MutableSequence[google.cloud.vision_v1p2beta1.types.AnnotateImageRequest]):
-                Required. Individual image annotation
-                requests for this batch.
+            requests (MutableSequence[google.cloud.vision_v1p3beta1.types.AnnotateImageRequest]):
+                Individual image annotation requests
+                for this batch.
 
                 This corresponds to the ``requests`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.vision_v1p2beta1.types.BatchAnnotateImagesResponse:
+            google.cloud.vision_v1p3beta1.types.BatchAnnotateImagesResponse:
                 Response to a batch image annotation
                 request.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -501,17 +547,14 @@
 
         # Minor optimization to avoid making a copy if the user passes
         # in a image_annotator.BatchAnnotateImagesRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
         if not isinstance(request, image_annotator.BatchAnnotateImagesRequest):
             request = image_annotator.BatchAnnotateImagesRequest(request)
-            if requests is not None:
-                for i in range(len(requests)):
-                    requests[i] = image_annotator.AnnotateImageRequest(requests[i])
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if requests is not None:
                 request.requests = requests
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
@@ -537,57 +580,57 @@
         requests: Optional[
             MutableSequence[image_annotator.AsyncAnnotateFileRequest]
         ] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
-        r"""Run async image detection and annotation for a list of generic
-        files (e.g. PDF) which may contain multiple pages and multiple
-        images per page. Progress and results can be retrieved through
-        the ``google.longrunning.Operations`` interface.
-        ``Operation.metadata`` contains ``OperationMetadata``
+        r"""Run asynchronous image detection and annotation for a list of
+        generic files, such as PDF files, which may contain multiple
+        pages and multiple images per page. Progress and results can be
+        retrieved through the ``google.longrunning.Operations``
+        interface. ``Operation.metadata`` contains ``OperationMetadata``
         (metadata). ``Operation.response`` contains
         ``AsyncBatchAnnotateFilesResponse`` (results).
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import vision_v1p2beta1
+            from google.cloud import vision_v1p3beta1
 
             def sample_async_batch_annotate_files():
                 # Create a client
-                client = vision_v1p2beta1.ImageAnnotatorClient()
+                client = vision_v1p3beta1.ImageAnnotatorClient()
 
                 # Initialize request argument(s)
-                request = vision_v1p2beta1.AsyncBatchAnnotateFilesRequest(
+                request = vision_v1p3beta1.AsyncBatchAnnotateFilesRequest(
                 )
 
                 # Make the request
                 operation = client.async_batch_annotate_files(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.vision_v1p2beta1.types.AsyncBatchAnnotateFilesRequest, dict]):
+            request (Union[google.cloud.vision_v1p3beta1.types.AsyncBatchAnnotateFilesRequest, dict]):
                 The request object. Multiple async file annotation
                 requests are batched into a single
                 service call.
-            requests (MutableSequence[google.cloud.vision_v1p2beta1.types.AsyncAnnotateFileRequest]):
+            requests (MutableSequence[google.cloud.vision_v1p3beta1.types.AsyncAnnotateFileRequest]):
                 Required. Individual async file
                 annotation requests for this batch.
 
                 This corresponds to the ``requests`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
@@ -597,15 +640,15 @@
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
                 The result type for the operation will be
-                :class:`google.cloud.vision_v1p2beta1.types.AsyncBatchAnnotateFilesResponse`
+                :class:`google.cloud.vision_v1p3beta1.types.AsyncBatchAnnotateFilesResponse`
                 Response to an async batch file annotation request.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([requests])
@@ -617,17 +660,14 @@
 
         # Minor optimization to avoid making a copy if the user passes
         # in a image_annotator.AsyncBatchAnnotateFilesRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
         if not isinstance(request, image_annotator.AsyncBatchAnnotateFilesRequest):
             request = image_annotator.AsyncBatchAnnotateFilesRequest(request)
-            if requests is not None:
-                for i in range(len(requests)):
-                    requests[i] = image_annotator.AsyncAnnotateFileRequest(requests[i])
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if requests is not None:
                 request.requests = requests
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
```

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/services/image_annotator/transports/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/services/image_annotator/transports/base.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/services/image_annotator/transports/rest.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/types/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/types/geometry.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/types/geometry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/types/image_annotator.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/types/image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/types/text_annotation.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/types/text_annotation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p2beta1/types/web_detection.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/types/web_detection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/gapic_metadata.json` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/gapic_version.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "3.4.1"  # {x-release-please-version}
+__version__ = "3.4.2"  # {x-release-please-version}
```

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/image_annotator/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/image_annotator/async_client.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/image_annotator/client.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p2beta1/services/image_annotator/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     Sequence,
     Tuple,
     Type,
     Union,
     cast,
 )
 
-from google.cloud.vision_v1p3beta1 import gapic_version as package_version
+from google.cloud.vision_v1p2beta1 import gapic_version as package_version
 
 from google.api_core import client_options as client_options_lib
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport import mtls  # type: ignore
@@ -44,15 +44,15 @@
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
-from google.cloud.vision_v1p3beta1.types import image_annotator
+from google.cloud.vision_v1p2beta1.types import image_annotator
 from .transports.base import ImageAnnotatorTransport, DEFAULT_CLIENT_INFO
 from .transports.grpc import ImageAnnotatorGrpcTransport
 from .transports.grpc_asyncio import ImageAnnotatorGrpcAsyncIOTransport
 from .transports.rest import ImageAnnotatorRestTransport
 
 
 class ImageAnnotatorClientMeta(type):
@@ -178,60 +178,14 @@
         Returns:
             ImageAnnotatorTransport: The transport used by the client
                 instance.
         """
         return self._transport
 
     @staticmethod
-    def product_path(
-        project: str,
-        location: str,
-        product: str,
-    ) -> str:
-        """Returns a fully-qualified product string."""
-        return "projects/{project}/locations/{location}/products/{product}".format(
-            project=project,
-            location=location,
-            product=product,
-        )
-
-    @staticmethod
-    def parse_product_path(path: str) -> Dict[str, str]:
-        """Parses a product path into its component segments."""
-        m = re.match(
-            r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)/products/(?P<product>.+?)$",
-            path,
-        )
-        return m.groupdict() if m else {}
-
-    @staticmethod
-    def product_set_path(
-        project: str,
-        location: str,
-        product_set: str,
-    ) -> str:
-        """Returns a fully-qualified product_set string."""
-        return (
-            "projects/{project}/locations/{location}/productSets/{product_set}".format(
-                project=project,
-                location=location,
-                product_set=product_set,
-            )
-        )
-
-    @staticmethod
-    def parse_product_set_path(path: str) -> Dict[str, str]:
-        """Parses a product_set path into its component segments."""
-        m = re.match(
-            r"^projects/(?P<project>.+?)/locations/(?P<location>.+?)/productSets/(?P<product_set>.+?)$",
-            path,
-        )
-        return m.groupdict() if m else {}
-
-    @staticmethod
     def common_billing_account_path(
         billing_account: str,
     ) -> str:
         """Returns a fully-qualified billing_account string."""
         return "billingAccounts/{billing_account}".format(
             billing_account=billing_account,
         )
@@ -492,49 +446,49 @@
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import vision_v1p3beta1
+            from google.cloud import vision_v1p2beta1
 
             def sample_batch_annotate_images():
                 # Create a client
-                client = vision_v1p3beta1.ImageAnnotatorClient()
+                client = vision_v1p2beta1.ImageAnnotatorClient()
 
                 # Initialize request argument(s)
-                request = vision_v1p3beta1.BatchAnnotateImagesRequest(
+                request = vision_v1p2beta1.BatchAnnotateImagesRequest(
                 )
 
                 # Make the request
                 response = client.batch_annotate_images(request=request)
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.vision_v1p3beta1.types.BatchAnnotateImagesRequest, dict]):
+            request (Union[google.cloud.vision_v1p2beta1.types.BatchAnnotateImagesRequest, dict]):
                 The request object. Multiple image annotation requests
                 are batched into a single service call.
-            requests (MutableSequence[google.cloud.vision_v1p3beta1.types.AnnotateImageRequest]):
-                Individual image annotation requests
-                for this batch.
+            requests (MutableSequence[google.cloud.vision_v1p2beta1.types.AnnotateImageRequest]):
+                Required. Individual image annotation
+                requests for this batch.
 
                 This corresponds to the ``requests`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
                 sent along with the request as metadata.
 
         Returns:
-            google.cloud.vision_v1p3beta1.types.BatchAnnotateImagesResponse:
+            google.cloud.vision_v1p2beta1.types.BatchAnnotateImagesResponse:
                 Response to a batch image annotation
                 request.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
@@ -547,17 +501,14 @@
 
         # Minor optimization to avoid making a copy if the user passes
         # in a image_annotator.BatchAnnotateImagesRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
         if not isinstance(request, image_annotator.BatchAnnotateImagesRequest):
             request = image_annotator.BatchAnnotateImagesRequest(request)
-            if requests is not None:
-                for i in range(len(requests)):
-                    requests[i] = image_annotator.AnnotateImageRequest(requests[i])
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if requests is not None:
                 request.requests = requests
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
@@ -583,57 +534,57 @@
         requests: Optional[
             MutableSequence[image_annotator.AsyncAnnotateFileRequest]
         ] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> operation.Operation:
-        r"""Run asynchronous image detection and annotation for a list of
-        generic files, such as PDF files, which may contain multiple
-        pages and multiple images per page. Progress and results can be
-        retrieved through the ``google.longrunning.Operations``
-        interface. ``Operation.metadata`` contains ``OperationMetadata``
+        r"""Run async image detection and annotation for a list of generic
+        files (e.g. PDF) which may contain multiple pages and multiple
+        images per page. Progress and results can be retrieved through
+        the ``google.longrunning.Operations`` interface.
+        ``Operation.metadata`` contains ``OperationMetadata``
         (metadata). ``Operation.response`` contains
         ``AsyncBatchAnnotateFilesResponse`` (results).
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
             # - It may require specifying regional endpoints when creating the service
             #   client as shown in:
             #   https://googleapis.dev/python/google-api-core/latest/client_options.html
-            from google.cloud import vision_v1p3beta1
+            from google.cloud import vision_v1p2beta1
 
             def sample_async_batch_annotate_files():
                 # Create a client
-                client = vision_v1p3beta1.ImageAnnotatorClient()
+                client = vision_v1p2beta1.ImageAnnotatorClient()
 
                 # Initialize request argument(s)
-                request = vision_v1p3beta1.AsyncBatchAnnotateFilesRequest(
+                request = vision_v1p2beta1.AsyncBatchAnnotateFilesRequest(
                 )
 
                 # Make the request
                 operation = client.async_batch_annotate_files(request=request)
 
                 print("Waiting for operation to complete...")
 
                 response = operation.result()
 
                 # Handle the response
                 print(response)
 
         Args:
-            request (Union[google.cloud.vision_v1p3beta1.types.AsyncBatchAnnotateFilesRequest, dict]):
+            request (Union[google.cloud.vision_v1p2beta1.types.AsyncBatchAnnotateFilesRequest, dict]):
                 The request object. Multiple async file annotation
                 requests are batched into a single
                 service call.
-            requests (MutableSequence[google.cloud.vision_v1p3beta1.types.AsyncAnnotateFileRequest]):
+            requests (MutableSequence[google.cloud.vision_v1p2beta1.types.AsyncAnnotateFileRequest]):
                 Required. Individual async file
                 annotation requests for this batch.
 
                 This corresponds to the ``requests`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
@@ -643,15 +594,15 @@
                 sent along with the request as metadata.
 
         Returns:
             google.api_core.operation.Operation:
                 An object representing a long-running operation.
 
                 The result type for the operation will be
-                :class:`google.cloud.vision_v1p3beta1.types.AsyncBatchAnnotateFilesResponse`
+                :class:`google.cloud.vision_v1p2beta1.types.AsyncBatchAnnotateFilesResponse`
                 Response to an async batch file annotation request.
 
         """
         # Create or coerce a protobuf request object.
         # Quick check: If we got a request object, we should *not* have
         # gotten any keyword arguments that map to the request.
         has_flattened_params = any([requests])
@@ -663,17 +614,14 @@
 
         # Minor optimization to avoid making a copy if the user passes
         # in a image_annotator.AsyncBatchAnnotateFilesRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
         if not isinstance(request, image_annotator.AsyncBatchAnnotateFilesRequest):
             request = image_annotator.AsyncBatchAnnotateFilesRequest(request)
-            if requests is not None:
-                for i in range(len(requests)):
-                    requests[i] = image_annotator.AsyncAnnotateFileRequest(requests[i])
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if requests is not None:
                 request.requests = requests
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
```

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/image_annotator/transports/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/image_annotator/transports/base.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/image_annotator/transports/rest.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/image_annotator/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/product_search/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/product_search/async_client.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/product_search/client.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/product_search/pagers.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/product_search/transports/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/product_search/transports/base.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/services/product_search/transports/rest.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/services/product_search/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/types/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/types/geometry.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/geometry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/types/image_annotator.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/types/product_search.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/product_search.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/types/product_search_service.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/product_search_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/types/text_annotation.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/text_annotation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p3beta1/types/web_detection.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p3beta1/types/web_detection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/gapic_metadata.json` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/gapic_version.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "3.4.1"  # {x-release-please-version}
+__version__ = "3.4.2"  # {x-release-please-version}
```

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/image_annotator/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/image_annotator/async_client.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/image_annotator/client.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -547,17 +547,14 @@
 
         # Minor optimization to avoid making a copy if the user passes
         # in a image_annotator.BatchAnnotateImagesRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
         if not isinstance(request, image_annotator.BatchAnnotateImagesRequest):
             request = image_annotator.BatchAnnotateImagesRequest(request)
-            if requests is not None:
-                for i in range(len(requests)):
-                    requests[i] = image_annotator.AnnotateImageRequest(requests[i])
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if requests is not None:
                 request.requests = requests
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
@@ -654,17 +651,14 @@
 
         # Minor optimization to avoid making a copy if the user passes
         # in a image_annotator.BatchAnnotateFilesRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
         if not isinstance(request, image_annotator.BatchAnnotateFilesRequest):
             request = image_annotator.BatchAnnotateFilesRequest(request)
-            if requests is not None:
-                for i in range(len(requests)):
-                    requests[i] = image_annotator.AnnotateFileRequest(requests[i])
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if requests is not None:
                 request.requests = requests
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
@@ -782,17 +776,14 @@
 
         # Minor optimization to avoid making a copy if the user passes
         # in a image_annotator.AsyncBatchAnnotateImagesRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
         if not isinstance(request, image_annotator.AsyncBatchAnnotateImagesRequest):
             request = image_annotator.AsyncBatchAnnotateImagesRequest(request)
-            if requests is not None:
-                for i in range(len(requests)):
-                    requests[i] = image_annotator.AnnotateImageRequest(requests[i])
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if requests is not None:
                 request.requests = requests
             if output_config is not None:
                 request.output_config = output_config
 
@@ -910,17 +901,14 @@
 
         # Minor optimization to avoid making a copy if the user passes
         # in a image_annotator.AsyncBatchAnnotateFilesRequest.
         # There's no risk of modifying the input as we've already verified
         # there are no flattened fields.
         if not isinstance(request, image_annotator.AsyncBatchAnnotateFilesRequest):
             request = image_annotator.AsyncBatchAnnotateFilesRequest(request)
-            if requests is not None:
-                for i in range(len(requests)):
-                    requests[i] = image_annotator.AsyncAnnotateFileRequest(requests[i])
             # If we have keyword arguments corresponding to fields on the
             # request, apply these.
             if requests is not None:
                 request.requests = requests
 
         # Wrap the RPC method; this adds retry and timeout information,
         # and friendly error handling.
```

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/image_annotator/transports/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/image_annotator/transports/base.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/image_annotator/transports/rest.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/image_annotator/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/product_search/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/product_search/async_client.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/product_search/client.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/product_search/pagers.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/product_search/transports/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/product_search/transports/base.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc_asyncio.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/services/product_search/transports/rest.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/services/product_search/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/types/__init__.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/types/face.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/face.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/types/geometry.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/geometry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/types/image_annotator.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/types/product_search.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/product_search.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/types/product_search_service.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/product_search_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/types/text_annotation.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/text_annotation.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google/cloud/vision_v1p4beta1/types/web_detection.py` & `google-cloud-vision-3.4.2/google/cloud/vision_v1p4beta1/types/web_detection.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/google_cloud_vision.egg-info/PKG-INFO` & `google-cloud-vision-3.4.2/google_cloud_vision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-vision
-Version: 3.4.1
+Version: 3.4.2
 Summary: Google Cloud Vision API client library
 Home-page: https://github.com/googleapis/python-vision
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-vision-3.4.1/google_cloud_vision.egg-info/SOURCES.txt` & `google-cloud-vision-3.4.2/google_cloud_vision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/setup.py` & `google-cloud-vision-3.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/tests/__init__.py` & `google-cloud-vision-3.4.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/tests/data/faces.jpg` & `google-cloud-vision-3.4.2/tests/data/faces.jpg`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/tests/data/logo.png` & `google-cloud-vision-3.4.2/tests/data/logo.png`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/tests/data/pdf_test.pdf` & `google-cloud-vision-3.4.2/tests/data/pdf_test.pdf`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/tests/system.py` & `google-cloud-vision-3.4.2/tests/system.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/tests/unit/__init__.py` & `google-cloud-vision-3.4.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/tests/unit/gapic/__init__.py` & `google-cloud-vision-3.4.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1/__init__.py` & `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1/test_image_annotator.py` & `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1/test_image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1/test_product_search.py` & `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1/test_product_search.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p1beta1/__init__.py` & `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p1beta1/test_image_annotator.py` & `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p1beta1/test_image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p2beta1/__init__.py` & `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p2beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p2beta1/test_image_annotator.py` & `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p2beta1/test_image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p3beta1/__init__.py` & `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p3beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p3beta1/test_image_annotator.py` & `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p3beta1/test_image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p3beta1/test_product_search.py` & `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p3beta1/test_product_search.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p4beta1/__init__.py` & `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p4beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p4beta1/test_image_annotator.py` & `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p4beta1/test_image_annotator.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/tests/unit/gapic/vision_v1p4beta1/test_product_search.py` & `google-cloud-vision-3.4.2/tests/unit/gapic/vision_v1p4beta1/test_product_search.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/tests/unit/test_decorators.py` & `google-cloud-vision-3.4.2/tests/unit/test_decorators.py`

 * *Files identical despite different names*

### Comparing `google-cloud-vision-3.4.1/tests/unit/test_helpers.py` & `google-cloud-vision-3.4.2/tests/unit/test_helpers.py`

 * *Files identical despite different names*

