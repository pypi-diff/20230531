# Comparing `tmp/thrivve_core-0.3.0.tar.gz` & `tmp/thrivve_core-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/thrivve_core/dist/.tmp-rwcuqihl/thrivve_core-0.3.0.tar", last modified: Mon May 29 13:55:59 2023, max compression
+gzip compressed data, was "/home/runner/work/platformLibraries/platformLibraries/thrivve_core/dist/.tmp-gjrrt91r/thrivve_core-0.3.1.tar", last modified: Wed May 31 13:41:38 2023, max compression
```

## Comparing `thrivve_core-0.3.0.tar` & `thrivve_core-0.3.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 13:55:59.000000 thrivve_core-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-05-29 13:55:59.000000 thrivve_core-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-29 13:55:59.000000 thrivve_core-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 13:55:59.000000 thrivve_core-0.3.0/thrivve_core/
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 13:55:59.000000 thrivve_core-0.3.0/thrivve_core/app_decorators/
--rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/app_decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      979 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/app_decorators/app_entry.py
--rw-r--r--   0 runner    (1001) docker     (122)     2464 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/app_decorators/handle_auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2327 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/app_decorators/handle_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/app_decorators/handle_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     4611 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/app_decorators/serializer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 13:55:59.000000 thrivve_core-0.3.0/thrivve_core/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      855 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/acl_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 13:55:59.000000 thrivve_core-0.3.0/thrivve_core/helpers/amazon/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/amazon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      579 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)     1353 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/amazon/get_file_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/amazon/get_plain_url.py
--rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/amazon/get_s3_client.py
--rw-r--r--   0 runner    (1001) docker     (122)      564 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/amazon/upload_file.py
--rw-r--r--   0 runner    (1001) docker     (122)      833 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/atomic_transactions.py
--rw-r--r--   0 runner    (1001) docker     (122)      921 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/atomic_transactions_v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     1797 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 13:55:59.000000 thrivve_core-0.3.0/thrivve_core/helpers/database/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      677 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/database/base_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/database/log_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2244 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/enums.py
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/fetch_relational_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     4723 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/format_exception.py
--rw-r--r--   0 runner    (1001) docker     (122)      385 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/get_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/get_country_code.py
--rw-r--r--   0 runner    (1001) docker     (122)      622 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/get_embedded_function.py
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/get_obj_value.py
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/get_prefix.py
--rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/kafka_listener.py
--rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/kafka_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 13:55:59.000000 thrivve_core-0.3.0/thrivve_core/helpers/kafka_producers/
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/kafka_producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/kafka_producers/log_model_changes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2061 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/kafka_producers/notification_center.py
--rw-r--r--   0 runner    (1001) docker     (122)      276 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/kafka_producers/send_sms.py
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/kafka_producers/send_topic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/log_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    12352 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/micro_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/numbers.py
--rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/search_function.py
--rw-r--r--   0 runner    (1001) docker     (122)      644 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/service_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      825 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/sql.py
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/system_roles.py
--rw-r--r--   0 runner    (1001) docker     (122)     7350 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/time.py
--rw-r--r--   0 runner    (1001) docker     (122)      393 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/topics.py
--rw-r--r--   0 runner    (1001) docker     (122)     1198 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/validate_mobile_number.py
--rw-r--r--   0 runner    (1001) docker     (122)      995 2023-05-29 13:55:48.000000 thrivve_core-0.3.0/thrivve_core/helpers/validate_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 13:55:59.000000 thrivve_core-0.3.0/thrivve_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-05-29 13:55:59.000000 thrivve_core-0.3.0/thrivve_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2246 2023-05-29 13:55:59.000000 thrivve_core-0.3.0/thrivve_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 13:55:59.000000 thrivve_core-0.3.0/thrivve_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-29 13:55:59.000000 thrivve_core-0.3.0/thrivve_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-29 13:55:59.000000 thrivve_core-0.3.0/thrivve_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:41:38.000000 thrivve_core-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-05-31 13:41:38.000000 thrivve_core-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-31 13:41:38.000000 thrivve_core-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:41:38.000000 thrivve_core-0.3.1/thrivve_core/
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:41:38.000000 thrivve_core-0.3.1/thrivve_core/app_decorators/
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/app_decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      979 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/app_decorators/app_entry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/app_decorators/handle_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2327 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/app_decorators/handle_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/app_decorators/handle_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4714 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/app_decorators/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2328 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:41:38.000000 thrivve_core-0.3.1/thrivve_core/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      855 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/acl_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:41:38.000000 thrivve_core-0.3.1/thrivve_core/helpers/amazon/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/amazon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1353 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/amazon/get_file_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/amazon/get_plain_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1607 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/amazon/get_s3_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      564 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/amazon/upload_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/atomic_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/atomic_transactions_v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1838 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:41:38.000000 thrivve_core-0.3.1/thrivve_core/helpers/database/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/database/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/database/log_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2244 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/fetch_relational_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4723 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2183 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/format_exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)      385 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/get_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/get_country_code.py
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/get_embedded_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      424 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/get_obj_value.py
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/get_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2723 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/kafka_listener.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/kafka_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:41:38.000000 thrivve_core-0.3.1/thrivve_core/helpers/kafka_producers/
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/kafka_producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/kafka_producers/log_model_changes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2061 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/kafka_producers/notification_center.py
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/kafka_producers/send_sms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      315 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/kafka_producers/send_topic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2007 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12452 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/micro_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/search_function.py
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/service_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      825 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/sql.py
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/system_roles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7350 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)      393 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/topics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1198 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/validate_mobile_number.py
+-rw-r--r--   0 runner    (1001) docker     (122)      995 2023-05-31 13:41:27.000000 thrivve_core-0.3.1/thrivve_core/helpers/validate_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-31 13:41:38.000000 thrivve_core-0.3.1/thrivve_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      746 2023-05-31 13:41:38.000000 thrivve_core-0.3.1/thrivve_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2246 2023-05-31 13:41:38.000000 thrivve_core-0.3.1/thrivve_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-31 13:41:38.000000 thrivve_core-0.3.1/thrivve_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-31 13:41:38.000000 thrivve_core-0.3.1/thrivve_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-31 13:41:38.000000 thrivve_core-0.3.1/thrivve_core.egg-info/top_level.txt
```

### Comparing `thrivve_core-0.3.0/PKG-INFO` & `thrivve_core-0.3.1/thrivve_core.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: thrivve_core
-Version: 0.3.0
+Name: thrivve-core
+Version: 0.3.1
 Summary: thrivveCore package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `thrivve_core-0.3.0/setup.py` & `thrivve_core-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     "Programming Language :: Python :: 3.4",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
 ]
 
 setup(
     name="thrivve_core",
-    version="0.3.0",
+    version="0.3.1",
     description="thrivveCore package",
     long_description="""# Markdown supported!\n\n* thrivve\n* List of features\n""",
     long_description_content_type="text/markdown",
     url="https://www.wedeliverapp.com/",
     author="Eyad Farra",
     author_email="info@wedeliverapp.com",
     license="MIT",
```

### Comparing `thrivve_core-0.3.0/thrivve_core/__init__.py` & `thrivve_core-0.3.1/thrivve_core/__init__.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/app_decorators/app_entry.py` & `thrivve_core-0.3.1/thrivve_core/app_decorators/app_entry.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/app_decorators/handle_auth.py` & `thrivve_core-0.3.1/thrivve_core/app_decorators/handle_auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 from functools import wraps
 
 from flask import request
 
-from thrivve_core.helpers.auth import verify_user_token_v2
+from thrivve_core.helpers.auth import verify_user_token_v2, Auth
 from thrivve_core.helpers.exceptions import (
     AppValidationError,
     AppMissingAuthError,
 )
-# from thrivve_core.helpers.acl_enum import Permission
-from flask_babel import force_locale, _
+from flask_babel import  _
 
 
 def handle_auth(require_auth, append_auth_args=None, allowed_roles=None, pre_login=False, allowed_permissions=None):
     def factory(func):
         @wraps(func)
         def inner_function(*args, **kws):
-            with force_locale('en'):
-                if not require_auth:
-                    return func(*args, **kws)
-
-                if "Authorization" not in request.headers:
-                    raise AppMissingAuthError(_("Missing authentication"))
-
-                token = request.headers["Authorization"]
-                if "country_code" not in request.headers and request.endpoint != "health_check":
-                    raise AppValidationError(_("Country Code is Required (c)"))
-
-                user = verify_user_token_v2(token=token)
-
-                with force_locale(user.get("language")):
-                    if not pre_login:
-                        if not user.get("is_logged"):
-                            raise AppValidationError(_("Not Logged Token, please complete login process"))
-
-                    if allowed_roles:
-                        if user.get("role") not in allowed_roles:
-                            raise AppValidationError(_("Not Allowed Role"))
-
-                    if append_auth_args and isinstance(append_auth_args, list):
-                        for arg in append_auth_args:
-                            if not kws.get('appended_kws'):
-                                kws['appended_kws'] = dict()
-                            if '.' in arg:
-
-                                if 'as' in arg:
-                                    arg, as_arg = arg.split(' as ')
-                                else:
-                                    as_arg = arg.replace('.', '_')
-
-                                obj, key = arg.split('.')
-                                value = user.get(obj, {}).get(key)
-
-                                kws['appended_kws'][as_arg] = value
-                            else:
-                                value = user.get(arg)
-                                kws['appended_kws'][arg] = value
+            # user_language = Auth.get_user_language()
+            # with force_locale(user_language):
+            if not require_auth:
+                return func(*args, **kws)
+
+            if "Authorization" not in request.headers:
+                raise AppMissingAuthError(_("Missing authentication"))
+
+            token = request.headers["Authorization"]
+            if "country_code" not in request.headers and request.endpoint != "health_check":
+                raise AppValidationError(_("Country Code is Required (c)"))
+
+            user = verify_user_token_v2(token=token)
+
+            # with force_locale(user.get("language")):
+            if not pre_login:
+                if not user.get("is_logged"):
+                    raise AppValidationError(_("Not Logged Token, please complete login process"))
+
+            if allowed_roles:
+                if user.get("role") not in allowed_roles:
+                    raise AppValidationError(_("Not Allowed Role"))
+
+            if append_auth_args and isinstance(append_auth_args, list):
+                for arg in append_auth_args:
+                    if not kws.get('appended_kws'):
+                        kws['appended_kws'] = dict()
+                    if '.' in arg:
+
+                        if 'as' in arg:
+                            arg, as_arg = arg.split(' as ')
+                        else:
+                            as_arg = arg.replace('.', '_')
+
+                        obj, key = arg.split('.')
+                        value = user.get(obj, {}).get(key)
+
+                        kws['appended_kws'][as_arg] = value
+                    else:
+                        value = user.get(arg)
+                        kws['appended_kws'][arg] = value
 
-                    return func(*args, **kws)
+            return func(*args, **kws)
 
         return inner_function
 
     return factory
```

### Comparing `thrivve_core-0.3.0/thrivve_core/app_decorators/handle_exceptions.py` & `thrivve_core-0.3.1/thrivve_core/app_decorators/handle_exceptions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/app_decorators/handle_response.py` & `thrivve_core-0.3.1/thrivve_core/app_decorators/handle_response.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/app_decorators/serializer.py` & `thrivve_core-0.3.1/thrivve_core/app_decorators/serializer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import ast
 import json
 from functools import wraps
+
 from sqlalchemy.orm.base import object_mapper
 import flask_sqlalchemy
 from flask import request
 from marshmallow import ValidationError
 from sqlalchemy.orm.exc import UnmappedInstanceError
 
 from thrivve_core.helpers.exceptions import AppValidationError
@@ -33,15 +34,16 @@
     return False
 
 
 def serializer(schema=None, many=False):
     def factory(func):
         @wraps(func)
         def decorator(*args, **kwargs):
-
+            # user_language = Auth.get_user_language()
+            # with force_locale(user_language):
             is_function_with_validated_data = False
             if hasattr(func, '__wrapped__'):
                 old_vars = func.__wrapped__.__code__.co_varnames
                 is_function_with_validated_data = old_vars.__contains__('validated_data')
 
             appended_kws = kwargs.pop('appended_kws', None)
```

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/acl_enum.py` & `thrivve_core-0.3.1/thrivve_core/helpers/acl_enum.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py` & `thrivve_core-0.3.1/thrivve_core/helpers/amazon/append_plain_urls_to_list_dict.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/amazon/get_file_url.py` & `thrivve_core-0.3.1/thrivve_core/helpers/amazon/get_file_url.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/amazon/get_s3_client.py` & `thrivve_core-0.3.1/thrivve_core/helpers/amazon/get_s3_client.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/amazon/upload_file.py` & `thrivve_core-0.3.1/thrivve_core/helpers/amazon/upload_file.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/atomic_transactions.py` & `thrivve_core-0.3.1/thrivve_core/helpers/atomic_transactions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/atomic_transactions_v2.py` & `thrivve_core-0.3.1/thrivve_core/helpers/atomic_transactions_v2.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/auth.py` & `thrivve_core-0.3.1/thrivve_core/helpers/auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from flask import request
+from flask import request, g
 
 from flask import session
 
-from .. import ThrivveCore
 from .micro_fetcher import MicroFetcher
 
 
 class Auth:
     def __init__(self):
         pass
 
     @staticmethod
     def set_user(user):
-        app = ThrivveCore.get_app()
-        app.logger.debug(user)
+        """
+        Set user in flask global object and session
+        """
+        g.user=user # store user in flask global object
         session["user"] = user
 
     @staticmethod
     def get_user():
         default_user_str = 'Guest'
         try:
             user = session.get("user", dict())
```

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/config.py` & `thrivve_core-0.3.1/thrivve_core/helpers/config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/database/base_model.py` & `thrivve_core-0.3.1/thrivve_core/helpers/database/base_model.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/database/log_model.py` & `thrivve_core-0.3.1/thrivve_core/helpers/database/log_model.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/enums.py` & `thrivve_core-0.3.1/thrivve_core/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/exceptions.py` & `thrivve_core-0.3.1/thrivve_core/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/fetch_relational_data.py` & `thrivve_core-0.3.1/thrivve_core/helpers/fetch_relational_data.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/filters.py` & `thrivve_core-0.3.1/thrivve_core/helpers/filters.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/format_exception.py` & `thrivve_core-0.3.1/thrivve_core/helpers/format_exception.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/get_embedded_function.py` & `thrivve_core-0.3.1/thrivve_core/helpers/get_embedded_function.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/kafka_listener.py` & `thrivve_core-0.3.1/thrivve_core/helpers/kafka_listener.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/kafka_producer.py` & `thrivve_core-0.3.1/thrivve_core/helpers/kafka_producer.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/kafka_producers/notification_center.py` & `thrivve_core-0.3.1/thrivve_core/helpers/kafka_producers/notification_center.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/log_config.py` & `thrivve_core-0.3.1/thrivve_core/helpers/log_config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/micro_fetcher.py` & `thrivve_core-0.3.1/thrivve_core/helpers/micro_fetcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import flask_sqlalchemy
+from flask import g
 
 from thrivve_core import ThrivveCore
 from thrivve_core.helpers.exceptions import AppMicroFetcherError, AppFetchServiceDataError
 import requests
 import json
 
 from thrivve_core.helpers.get_obj_value import get_obj_value, set_obj_value
@@ -175,15 +176,17 @@
         self.module_name = module_name
         return self
 
     def _call_api(self):
 
         url = "{}/fetch_relational_data".format(self.service_url)
 
-        payload_dict = dict()
+        payload_dict = dict(
+            __user_auth_data__=g.user if hasattr(g, 'user') else None,
+        )
         if self.query_type in [QueryTypes.SIMPLE_TABLE.value, QueryTypes.FUNCTION.value]:
             payload_dict.update(
                 dict(
                     fields=self.fields,
                     table_name=self.table_name,
                     column_name=self.column_name,
                     compair_operator=self.compair_operator,
```

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/search_function.py` & `thrivve_core-0.3.1/thrivve_core/helpers/search_function.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/service_config.py` & `thrivve_core-0.3.1/thrivve_core/helpers/service_config.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/sql.py` & `thrivve_core-0.3.1/thrivve_core/helpers/sql.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/time.py` & `thrivve_core-0.3.1/thrivve_core/helpers/time.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/validate_mobile_number.py` & `thrivve_core-0.3.1/thrivve_core/helpers/validate_mobile_number.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core/helpers/validate_parameters.py` & `thrivve_core-0.3.1/thrivve_core/helpers/validate_parameters.py`

 * *Files identical despite different names*

### Comparing `thrivve_core-0.3.0/thrivve_core.egg-info/PKG-INFO` & `thrivve_core-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: thrivve-core
-Version: 0.3.0
+Name: thrivve_core
+Version: 0.3.1
 Summary: thrivveCore package
 Home-page: https://www.wedeliverapp.com/
 Author: Eyad Farra
 Author-email: info@wedeliverapp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `thrivve_core-0.3.0/thrivve_core.egg-info/SOURCES.txt` & `thrivve_core-0.3.1/thrivve_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

