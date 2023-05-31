# Comparing `tmp/th2_data_services-2.0.0.dev5122037338.tar.gz` & `tmp/th2_data_services-2.0.0.dev5129283461.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services-2.0.0.dev5122037338.tar", last modified: Tue May 30 13:25:54 2023, max compression
+gzip compressed data, was "dist/th2_data_services-2.0.0.dev5129283461.tar", last modified: Wed May 31 05:40:07 2023, max compression
```

## Comparing `th2_data_services-2.0.0.dev5122037338.tar` & `th2_data_services-2.0.0.dev5129283461.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:25:54.000000 th2_data_services-2.0.0.dev5122037338/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    28243 2023-05-30 13:25:54.000000 th2_data_services-2.0.0.dev5122037338/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    23148 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-30 13:25:37.000000 th2_data_services-2.0.0.dev5122037338/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-30 13:25:54.000000 th2_data_services-2.0.0.dev5122037338/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:25:54.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:25:54.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/config/
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/config/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    32815 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:25:54.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      806 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/event_tree/etc_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)    16045 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/event_tree/event_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)    25893 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/event_tree/event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/event_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/event_tree/parent_event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1680 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:25:54.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/interfaces/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      706 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/interfaces/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/interfaces/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:25:54.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/interfaces/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/interfaces/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/interfaces/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2705 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/interfaces/utils/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:25:54.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     3360 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/_json.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/_types.py
--rw-r--r--   0 runner    (1001) docker     (122)    15883 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/aggregation_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/az_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)      742 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/categorizers.py
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/category.py
--rw-r--r--   0 runner    (1001) docker     (122)     3296 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (122)      908 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/decode_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:25:54.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/event_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/event_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/event_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (122)     7107 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/event_utils/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5291 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/event_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    12089 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/event_utils/select.py
--rw-r--r--   0 runner    (1001) docker     (122)     6805 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/event_utils/totals.py
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    15216 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/json_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:25:54.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/message_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/message_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/message_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    14456 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/message_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    15739 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10508 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/perfect_table.py
--rw-r--r--   0 runner    (1001) docker     (122)    33801 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/script_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/sse_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5285 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     6538 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/total_category_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:25:54.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/viewer_structs/
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/viewer_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6185 2023-05-30 13:22:19.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/viewer_structs/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 13:25:54.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    28243 2023-05-30 13:25:53.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-30 13:25:54.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 13:25:53.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-05-30 13:25:53.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-30 13:25:53.000000 th2_data_services-2.0.0.dev5122037338/th2_data_services.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 05:40:07.000000 th2_data_services-2.0.0.dev5129283461/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    28243 2023-05-31 05:40:07.000000 th2_data_services-2.0.0.dev5129283461/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    23148 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-31 05:39:55.000000 th2_data_services-2.0.0.dev5129283461/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-31 05:40:07.000000 th2_data_services-2.0.0.dev5129283461/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 05:40:07.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 05:40:07.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34453 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 05:40:07.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      806 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/event_tree/etc_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16045 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/event_tree/event_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25893 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/event_tree/event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/event_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/event_tree/parent_event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1680 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 05:40:07.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/interfaces/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      706 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/interfaces/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/interfaces/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 05:40:07.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/interfaces/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/interfaces/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/interfaces/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2705 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/interfaces/utils/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 05:40:07.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     3360 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15883 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/aggregation_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/az_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/categorizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/category.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3296 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      908 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/decode_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 05:40:07.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/event_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/event_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/event_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7107 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/event_utils/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5291 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/event_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12089 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/event_utils/select.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6805 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/event_utils/totals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15216 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/json_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 05:40:07.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/message_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/message_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/message_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14456 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/message_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15739 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10508 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/perfect_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33801 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/script_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/sse_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5285 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6538 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/total_category_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 05:40:07.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/viewer_structs/
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/viewer_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6185 2023-05-31 05:38:41.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/viewer_structs/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 05:40:07.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    28243 2023-05-31 05:40:07.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-31 05:40:07.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 05:40:07.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-05-31 05:40:07.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-31 05:40:07.000000 th2_data_services-2.0.0.dev5129283461/th2_data_services.egg-info/top_level.txt
```

### Comparing `th2_data_services-2.0.0.dev5122037338/PKG-INFO` & `th2_data_services-2.0.0.dev5129283461/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 325f  : 2.1.Name: th2_
 00000020: 6461 7461 5f73 6572 7669 6365 730a 5665  data_services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3531 3232 3033 3733 3338 0a53 756d 6d61  5122037338.Summa
+00000040: 3531 3239 3238 3334 3631 0a53 756d 6d61  5129283461.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev5122037338/README.md` & `th2_data_services-2.0.0.dev5129283461/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/setup.py` & `th2_data_services-2.0.0.dev5129283461/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/config/__init__.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/config/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/config/config.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/config/config.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/data.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,26 @@
 import pickle
 import pprint
 from warnings import warn
 from functools import partial
 from os import rename
 from pathlib import Path
 from time import time
-from typing import Callable, Dict, Generator, List, Optional, Union, Iterable, Iterator, Any, Generic
+from typing import (
+    Callable,
+    Dict,
+    Generator,
+    List,
+    Optional,
+    Union,
+    Iterable,
+    Iterator,
+    Any,
+    Generic,
+)
 from weakref import finalize
 import types
 from inspect import isgeneratorfunction
 from typing import TypeVar
 from th2_data_services.interfaces.adapter import IStreamAdapter, IRecordAdapter
 from th2_data_services.config import options
 from th2_data_services.utils._json import iter_json_file
@@ -77,18 +88,22 @@
             self._data_stream = self._create_data_set_from_iterables(data)
         else:
             self._data_stream = data
 
         self._id = id(self)
         self._cache_filename = f"{self._id}_{time()}.pickle"
         self._cache_path = Path("temp", self._cache_filename).resolve().absolute()
-        self._pending_cache_path = self._cache_path.with_name("[PENDING]" + self._cache_filename).resolve().absolute()
+        self._pending_cache_path = (
+            self._cache_path.with_name("[PENDING]" + self._cache_filename).resolve().absolute()
+        )
         self._cache_file_obj = None
         self._len = None
-        self._workflow = [] if workflow is None else workflow  # Normally it has empty list or one Step.
+        self._workflow = (
+            [] if workflow is None else workflow
+        )  # Normally it has empty list or one Step.
         self._length_hint = None  # The value is populated when we use limit method.
         self._cache_status = cache
         # We use finalize instead of __del__ because __del__ won't be executed sometimes.
         # Read more about __del__ problems here: https://stackoverflow.com/a/2452895
         self._finalizer = finalize(self, self.__remove)
         # LOG         self._logger = _DataLogger(logger, {"id": self._id})
         # It used to indicate the number of current iteration of the Data object.
@@ -127,15 +142,17 @@
             self._cache_file_obj.close()
             path.unlink()
 
     def _create_data_set_from_iterables(self, iterables_list: List[Iterable]) -> DataSet:
         """Creates a generator from the list of iterables."""
         return partial(self._create_generator_data_source_from_iterables, iterables_list)
 
-    def _create_generator_data_source_from_iterables(self, iterables_list: List[Iterable]) -> Generator:
+    def _create_generator_data_source_from_iterables(
+        self, iterables_list: List[Iterable]
+    ) -> Generator:
         """Creates a generator from the list of iterables."""
         for data in iterables_list:
             yield from data
 
     def _is_iterables_list(self, data: DataSet) -> bool:
         if not isinstance(data, (list, tuple)):
             return False
@@ -288,15 +305,17 @@
         """Returns filepath for a pending cache file."""
         return self._pending_cache_path
 
     def get_cache_filepath(self) -> Path:
         """Returns filepath for a cache file."""
         return self._cache_path
 
-    def _iterate_modified_data_stream(self, data_stream: DataGenerator, workflow: WorkFlow) -> DataGenerator:
+    def _iterate_modified_data_stream(
+        self, data_stream: DataGenerator, workflow: WorkFlow
+    ) -> DataGenerator:
         """Returns generator that iterates data stream with applied workflow.
 
         StopIteration from limit function will be handled here.
         """
         # LOG         self._logger.debug("Iterating data stream = '%s'", id(data_stream))
         for record in data_stream:
             try:
@@ -321,15 +340,17 @@
             if modified_records is None:
                 continue
             elif isinstance(modified_records, (list, tuple)):
                 yield from modified_records
             else:  # Just one record.
                 yield modified_records
 
-    def __change_data(self, data_stream: DataGenerator, workflow: WorkFlow, cache: bool) -> DataGenerator:
+    def __change_data(
+        self, data_stream: DataGenerator, workflow: WorkFlow, cache: bool
+    ) -> DataGenerator:
         """Applies workflow for data.
 
         Args:
             data_stream: Data for apply workflow.
             workflow: Workflow.
             cache: Set True if you are going to write and read from the cache.
 
@@ -383,15 +404,17 @@
                     break
 
     def _process_step(self, step: dict, record):
         res = step["callback"](record)
         # LOG         self._logger.debug("    - step '%s' -> %s", step["type"], res)
         return res
 
-    def __apply_workflow(self, record: Any, workflow: WorkFlow) -> Optional[Union[dict, List[dict]]]:
+    def __apply_workflow(
+        self, record: Any, workflow: WorkFlow
+    ) -> Optional[Union[dict, List[dict]]]:
         """Creates generator records with apply workflow.
 
         Returns:
             obj: Generator records.
 
         """
         # LOG         self._logger.debug("Apply workflow for %s", record)
@@ -468,15 +491,17 @@
             new_workflow = [{"type": "map", "callback": callback_or_adapter.handle}]
         else:
             new_workflow = [{"type": "map", "callback": callback_or_adapter}]
         data = Data(data=self, workflow=new_workflow)
         data._set_metadata(self.metadata)
         return data
 
-    def map_stream(self, adapter_or_generator: Union[IStreamAdapter, Callable[..., Generator]]) -> "Data":
+    def map_stream(
+        self, adapter_or_generator: Union[IStreamAdapter, Callable[..., Generator]]
+    ) -> "Data":
         """Append `stream-transform` function to workflow.
 
         If StreamAdapter is passed StreamAdapter.handle method will be used as a map function.
 
         Difference between map and map_stream:
         1. map_stream allows you return None values.
         2. map_stream allows you work with the whole stream but not with only 1 element, so you can implement some buffers inside handler.
@@ -489,15 +514,17 @@
             Data: Data object.
 
         """
 
         def get_source(handler):
             yield from handler(self)
 
-        if isinstance(adapter_or_generator, IStreamAdapter) and isgeneratorfunction(adapter_or_generator.handle):
+        if isinstance(adapter_or_generator, IStreamAdapter) and isgeneratorfunction(
+            adapter_or_generator.handle
+        ):
             source = partial(get_source, adapter_or_generator.handle)
         elif isgeneratorfunction(adapter_or_generator):
             source = partial(get_source, adapter_or_generator)
         else:
             raise Exception(
                 "map_stream Only accepts IStreamAdapter class with generator function or Generator function"
             )
@@ -527,14 +554,38 @@
         Args:
             num: How many records will be provided.
 
         Returns:
             Data: Data object.
         """
         # LOG         self._logger.info("Apply limit = %s", num)
+        # def get_source(handler):
+        #     try:
+        #         yield from handler(self)
+        #     except StopIteration as e:
+        #
+        #         # There is some magic.
+        #         # It'll stop data stream and will be handled in the finally statements.
+        #         # If you put return not under except block it will NOT work.
+        #         #
+        #         # It happens because python returns control to data_stream here due to `yield`.
+        #         return
+        #
+        # def filter_yield(stream):
+        #     callback = self._build_limit_callback(num)
+        #     for record in stream:
+        #         if callback(record):
+        #             yield record
+        #
+        # source = partial(get_source, filter_yield)
+        # data = Data(source)
+        # data._length_hint = num
+        # data._set_metadata(self.metadata)
+        # return data
+
         new_workflow = [{"type": "limit", "callback": self._build_limit_callback(num)}]
         data_obj = Data(data=self, workflow=new_workflow)
         data_obj._length_hint = num
         data_obj._set_metadata(self.metadata)
         return data_obj
 
     def sift(self, limit: int = None, skip: int = None) -> Generator[dict, None, None]:
@@ -712,15 +763,15 @@
 
         data_obj = cls([], cache=True)
         data_obj._set_custom_cache_destination(filename=filename)
         data_obj.update_metadata({"source_file": filename})
         return data_obj
 
     @classmethod
-    def from_json(cls, filename, buffer_limit=250) -> "Data":
+    def from_json(cls, filename, buffer_limit=250) -> "Data[dict]":
         """Creates Data object from json file with provided name.
 
         Args:
             filename: Name or path to cache file.
             buffer_limit: If limit is 0 buffer will not be used. Number of messages in buffer before parsing.
 
         Returns:
@@ -734,15 +785,15 @@
             raise FileNotFoundError(f"{filename} doesn't exist")
 
         data = cls(iter_json_file(filename, buffer_limit))
         data.update_metadata({"source_file": filename})
         return data
 
     @classmethod
-    def from_any_file(cls, filename, mode="r") -> "Data":
+    def from_any_file(cls, filename, mode="r") -> "Data[str]":
         """Creates Data object from any file with provided name.
 
         It will just iterate file and return data line be line.
 
         Args:
             filename: Name or path to the file.
             mode: Read mode of open function.
@@ -758,15 +809,17 @@
             raise FileNotFoundError(f"{filename} doesn't exist")
 
         data = cls(_iter_any_file(filename, mode))
         data.update_metadata({"source_file": filename})
         return data
 
     @classmethod
-    def from_csv(cls, filename, header=None, header_first_line=False, mode="r", delimiter=",") -> "Data":
+    def from_csv(
+        cls, filename, header=None, header_first_line=False, mode="r", delimiter=","
+    ) -> "Data":
         """Creates Data object from any file with provided name.
 
         It will iterate the CSV file as if you were doing it with CSV module.
 
         Args:
             filename: Name or path to the file.
             header: If provided header for csv, Data object will yield Dict[str].
@@ -779,19 +832,33 @@
         Returns:
             Data: Data object.
 
         Raises:
             FileNotFoundError if provided file does not exist.
 
         """
+        # TODO - bug here TH2-4930 - new data object doesn't work with limit method
         if not Path(filename).resolve().exists():
             raise FileNotFoundError(f"{filename} doesn't exist")
 
         data = cls(_iter_csv(filename, header, header_first_line, mode, delimiter))
         data.update_metadata({"source_file": filename})
+
+        # TH2-4930
+        # TODO - should be deleted after bugfix
+        if header is None and not header_first_line:
+
+            def limit(*args, **kwargs):
+                raise RuntimeError(
+                    "The data object that was get by using 'from_csv' "
+                    "cannot work with 'limit' method. Known issue TH2-4930."
+                )
+
+            data.limit = limit
+
         return data
 
     def _set_metadata(self, metadata: Dict) -> None:
         """Set metadata of object to metadata argument.
 
         Args:
             metadata (dict): New Metadata
@@ -831,15 +898,17 @@
 
         for k, v in metadata.items():
             if k in self.metadata:
                 current = self.metadata[k]
                 # Check For Iterable Types
                 if isinstance(v, dict):
                     self.__metadata[k].update({**current, **v})
-                elif isinstance(v, Iterable) and not (isinstance(v, str) or isinstance(current, str)):
+                elif isinstance(v, Iterable) and not (
+                    isinstance(v, str) or isinstance(current, str)
+                ):
                     if isinstance(current, Iterable):
                         self.__metadata[k] = [*current, *v]
                     else:
                         self.__metadata[k] = [current, *v]
                 else:  # Single Item
                     if isinstance(current, Iterable):
                         self.__metadata[k] = [*current, v]
```

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/event_tree/__init__.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/event_tree/etc_driver.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/event_tree/etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/event_tree/event_tree.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/event_tree/event_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/event_tree/event_tree_collection.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/event_tree/event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/event_tree/exceptions.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/event_tree/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/event_tree/parent_event_tree_collection.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/event_tree/parent_event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/exceptions.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/interfaces/__init__.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/interfaces/adapter.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/interfaces/command.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/interfaces/data_source.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/interfaces/source_api.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/interfaces/struct.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/interfaces/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/interfaces/stub_builder.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/interfaces/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/interfaces/utils/__init__.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/interfaces/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/interfaces/utils/converter.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/interfaces/utils/converter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/interfaces/utils/resolver.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/interfaces/utils/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/_json.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/_json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/_types.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/_types.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/aggregation_classes.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/aggregation_classes.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/az_tree.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/az_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/categorizers.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/categorizers.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/category.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/category.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/converters.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/converters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/decode_error_handler.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/decode_error_handler.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/display.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/event_utils/__init__.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/event_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/event_utils/display.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/event_utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/event_utils/event_utils.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/event_utils/event_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/event_utils/frequencies.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/event_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/event_utils/select.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/event_utils/select.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/event_utils/totals.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/event_utils/totals.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/experimental.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/experimental.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/json_tree.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/json_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/message_utils/__init__.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/message_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/message_utils/frequencies.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/message_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/message_utils/message_utils.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/message_utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/misc_utils.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/perfect_table.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/perfect_table.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/script_report_utils.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/script_report_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/sse_client.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/time.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/time.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/total_category_calculator.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/total_category_calculator.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/viewer_structs/__init__.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/viewer_structs/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services/utils/viewer_structs/verification.py` & `th2_data_services-2.0.0.dev5129283461/th2_data_services/utils/viewer_structs/verification.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services.egg-info/PKG-INFO` & `th2_data_services-2.0.0.dev5129283461/th2_data_services.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 322d  : 2.1.Name: th2-
 00000020: 6461 7461 2d73 6572 7669 6365 730a 5665  data-services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3531 3232 3033 3733 3338 0a53 756d 6d61  5122037338.Summa
+00000040: 3531 3239 3238 3334 3631 0a53 756d 6d61  5129283461.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services.egg-info/SOURCES.txt` & `th2_data_services-2.0.0.dev5129283461/th2_data_services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5122037338/th2_data_services.egg-info/requires.txt` & `th2_data_services-2.0.0.dev5129283461/th2_data_services.egg-info/requires.txt`

 * *Files identical despite different names*

