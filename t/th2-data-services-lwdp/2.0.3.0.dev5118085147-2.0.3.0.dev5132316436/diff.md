# Comparing `tmp/th2_data_services_lwdp-2.0.3.0.dev5118085147.tar.gz` & `tmp/th2_data_services_lwdp-2.0.3.0.dev5132316436.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services_lwdp-2.0.3.0.dev5118085147.tar", last modified: Tue May 30 06:05:03 2023, max compression
+gzip compressed data, was "dist/th2_data_services_lwdp-2.0.3.0.dev5132316436.tar", last modified: Wed May 31 11:35:58 2023, max compression
```

## Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147.tar` & `th2_data_services_lwdp-2.0.3.0.dev5132316436.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 06:05:03.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-05-30 06:05:03.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7699 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-30 06:04:43.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-30 06:05:03.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 06:05:03.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 06:05:03.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 06:05:03.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 06:05:03.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/adapters/
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
--rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/adapters/basic_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/adapters/event_adapters.py
--rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/adapters/message_adapters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 06:05:03.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/commands/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/commands/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    38907 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/commands/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 06:05:03.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/data_source/
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/data_source/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/data_source/http.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 06:05:03.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      658 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 06:05:03.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/filters/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/filters/event_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/filters/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 06:05:03.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)      614 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/interfaces/filter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      722 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/message_response_format.py
--rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/page.py
--rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 06:05:03.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/source_api/
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/source_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16862 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/source_api/grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)    13123 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/source_api/http.py
--rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/streams.py
--rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 06:05:03.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1497 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/utils/_response_formats.py
--rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-05-30 06:02:55.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 06:05:03.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services_lwdp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-05-30 06:05:03.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services_lwdp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-05-30 06:05:03.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services_lwdp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 06:05:03.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services_lwdp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-30 06:05:03.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services_lwdp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-30 06:05:03.000000 th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services_lwdp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:35:58.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-05-31 11:35:58.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7699 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-05-31 11:35:30.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-31 11:35:58.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1658 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:35:58.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:35:58.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:35:58.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:35:58.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2000 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/adapters/adapter_sse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2442 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/adapters/basic_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/adapters/event_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1906 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/adapters/message_adapters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:35:58.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/commands/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40696 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/commands/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:35:58.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/data_source/
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/data_source/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3586 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/data_source/http.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:35:58.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:35:58.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/filters/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/filters/event_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3527 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/filters/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:35:58.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)      614 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/interfaces/filter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/message_response_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/page.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3593 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:35:58.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/source_api/
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/source_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16862 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/source_api/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13470 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/source_api/http.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4687 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/streams.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2995 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4571 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:35:58.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1497 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/utils/_response_formats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2441 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-05-31 11:33:51.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 11:35:58.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services_lwdp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-05-31 11:35:58.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services_lwdp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2229 2023-05-31 11:35:58.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services_lwdp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 11:35:58.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services_lwdp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-31 11:35:58.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services_lwdp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-31 11:35:58.000000 th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services_lwdp.egg-info/top_level.txt
```

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/PKG-INFO` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_data_services_lwdp
-Version: 2.0.3.0.dev5118085147
+Version: 2.0.3.0.dev5132316436
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/README.md` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/setup.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/__init__.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/adapters/__init__.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/adapters/adapter_sse.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/adapters/adapter_sse.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/adapters/basic_adapters.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/adapters/basic_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/adapters/event_adapters.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/adapters/event_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/adapters/message_adapters.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/adapters/message_adapters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/commands/__init__.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/commands/grpc.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/commands/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/commands/http.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/commands/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,40 +181,86 @@
         url = api.get_url_get_scopes(self._book_id)
 
         # LOG         logger.info(url)
 
         return api.execute_request(url).json()
 
 
-class GetMessageAliases(IHTTPCommand):
+class GetMessageAliases(SSEHandlerClassBase):
     """A Class-Command for request to lw-data-provider.
 
     It retrieves a list of message aliases in book.
 
     Returns:
         dict: List[str].
     """
 
-    def __init__(self, book_id: str):
-        """GetMessageAliases constructor.
+    def __init__(
+        self,
+        book_id: str,
+        start_timestamp: datetime = None,
+        end_timestamp: datetime = None,
+        buffer_limit: int = DEFAULT_BUFFER_LIMIT,
+        cache: bool = False,
+    ) -> None:
+        """GetPages Constructor.
+
+        If start_timestamp and end_timestamp are not provided, it returns all Pages.
 
         Args:
-            book_id: Name of book to search in.
+            book_id (str): Book ID.
+            start_timestamp (datetime): Start Timestamp.
+            end_timestamp (datetime): End Timestamp.
+            cache (Optional, bool): Cache Status. Defaults To `False`.
+            buffer_limit: SSEAdapter BufferedJSONProcessor buffer limit.
         """
-        super().__init__()
+        super().__init__(cache, buffer_limit=buffer_limit)
+        if all(timestamp is None for timestamp in (start_timestamp, end_timestamp)):
+            self._all_results = True
+        else:
+            _check_datetime(start_timestamp)
+            _check_datetime(end_timestamp)
+            self._start_timestamp = DatetimeConverter.to_nanoseconds(start_timestamp)
+            self._end_timestamp = DatetimeConverter.to_nanoseconds(end_timestamp)
+            self._all_results = False
         self._book_id = book_id
 
-    def handle(self, data_source: HTTPDataSource) -> List[str]:  # noqa: D102
-        api: HTTPAPI = data_source.source_api
-        url = api.get_url_get_message_aliases(self._book_id)
+    def _get_urls(self, data_source: HTTPDataSource):
+        api = data_source.source_api
+        if self._all_results:
+            return [api.get_url_get_message_aliases(book_id = self._book_id)]
+        else:
+            return [
+                api.get_url_get_message_aliases(
+                    self._book_id, self._start_timestamp, self._end_timestamp
+                )
+            ]
+
+    def _stream_chunk_data(sse_events_stream):
+        for chunk in sse_events_stream:
+            for event in chunk:
+                yield event
 
-        # LOG         logger.info(url)
+    def _data_object(self, data_source: HTTPDataSource) -> Data[Page]:
+        """Parses SSEEvents Into Data Object.
 
-        return api.execute_request(url).json()
+        Args:
+            data_source: HTTPDataSource
 
+        Returns:
+             Data
+        """
+        sse_events_stream = partial(self._stream_chunk_data(self._sse_events_stream), data_source)
+        data = (
+            Data(sse_events_stream)
+            .map_stream(self._sse_handler)
+            .use_cache(self._cache)
+        )
+        data.metadata["urls"] = self._get_urls(data_source)
+        return data
 
 class GetMessageGroups(IHTTPCommand):
     """A Class-Command for request to lw-data-provider.
 
     It retrieves a list of message groups in book.
 
     Returns:
```

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/data_source/__init__.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/data_source/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/data_source/grpc.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/data_source/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/data_source/http.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/data_source/http.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/event_tree/__init__.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/event_tree/http_etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/filters/__init__.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/filters/event_filters.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/filters/event_filters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/filters/filter.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/filters/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/interfaces/__init__.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/interfaces/command.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/interfaces/data_source.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/interfaces/filter.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/interfaces/filter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/interfaces/source_api.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/message_response_format.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/message_response_format.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/page.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/page.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/resolver.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/source_api/__init__.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/source_api/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/source_api/grpc.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/source_api/grpc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/source_api/http.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/source_api/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,26 @@
         """REST-API `books` call returns a list of books in cradleAPI."""
         return self.__encode_url(f"{self._url}/books")
 
     def get_url_get_scopes(self, book_id: str) -> str:
         """REST-API `book/{bookID}/event/scopes` call returns a list of scopes in book named bookID."""
         return self.__encode_url(f"{self._url}/book/{book_id}/event/scopes")
 
-    def get_url_get_message_aliases(self, book_id: str) -> str:
+    def get_url_get_message_aliases(self, book_id: str, start_timestamp: int = None, end_timestamp: int = None, chunked_size: int = None) -> str:
         """REST-API `book/{bookID}/message/aliases` call returns a list of message aliases in book named bookID."""
-        return self.__encode_url(f"{self._url}/book/{book_id}/message/aliases")
+        url = f"{self._url}/book/{book_id}/message/aliases/sse?"
+
+        kwargs = {
+            "startTimestamp": start_timestamp,
+            "endTimestamp": end_timestamp,
+            "chunkedSize": chunked_size,
+        }
+
+        url += "&".join(f"{k}={v}" for k, v in kwargs.items() if v is not None)
+        return self.__encode_url(url)
 
     def get_url_get_message_groups(self, book_id: str) -> str:
         """REST-API `book/{bookID}/message/groups` call returns a list of message groups in book named bookID."""
         return self.__encode_url(f"{self._url}/book/{book_id}/message/groups")
 
     def get_url_find_event_by_id(self, event_id: str) -> str:
         """REST-API `event` call returns a single event with the specified id."""
```

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/streams.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/streams.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/struct.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/stub_builder.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/utils/__init__.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/utils/_response_formats.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/utils/_response_formats.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/utils/json.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/utils/json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services/data_source/lwdp/utils/misc.py` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services/data_source/lwdp/utils/misc.py`

 * *Files identical despite different names*

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services_lwdp.egg-info/PKG-INFO` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services_lwdp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-data-services-lwdp
-Version: 2.0.3.0.dev5118085147
+Version: 2.0.3.0.dev5132316436
 Summary: th2_data_services_lwdp
 Home-page: https://github.com/th2-net/th2-ds-source-lwdp
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # Lightweight Data Provider Data Source (major version 2).
         # Introduction
```

### Comparing `th2_data_services_lwdp-2.0.3.0.dev5118085147/th2_data_services_lwdp.egg-info/SOURCES.txt` & `th2_data_services_lwdp-2.0.3.0.dev5132316436/th2_data_services_lwdp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

