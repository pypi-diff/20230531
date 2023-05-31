# Comparing `tmp/lusid-notification-sdk-preview-0.1.711.tar.gz` & `tmp/lusid-notification-sdk-preview-0.1.715.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.711.tar", last modified: Tue May 30 12:02:19 2023, max compression
+gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.715.tar", last modified: Wed May 31 12:25:41 2023, max compression
```

## Comparing `lusid-notification-sdk-preview-0.1.711.tar` & `lusid-notification-sdk-preview-0.1.715.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 12:02:19.000000 lusid-notification-sdk-preview-0.1.711/
--rw-r--r--   0 root         (0) root         (0)       53 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      371 2023-05-30 12:02:19.000000 lusid-notification-sdk-preview-0.1.711/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8040 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 12:02:19.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/
--rw-r--r--   0 root         (0) root         (0)     4452 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 12:02:19.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/api/
--rw-r--r--   0 root         (0) root         (0)      506 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6847 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    10519 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/api/deliveries_api.py
--rw-r--r--   0 root         (0) root         (0)    13984 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/api/event_types_api.py
--rw-r--r--   0 root         (0) root         (0)     7820 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/api/manual_event_api.py
--rw-r--r--   0 root         (0) root         (0)    52797 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/api/notifications_api.py
--rw-r--r--   0 root         (0) root         (0)    47803 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/api/subscriptions_api.py
--rw-r--r--   0 root         (0) root         (0)    27431 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16631 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5099 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 12:02:19.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/
--rw-r--r--   0 root         (0) root         (0)     3100 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7254 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     9017 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7231 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)     9643 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/amazon_sqs_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     7916 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/api_request_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     6508 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/attempt.py
--rw-r--r--   0 root         (0) root         (0)     5556 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/attempt_status.py
--rw-r--r--   0 root         (0) root         (0)    11191 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/create_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    10603 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/create_subscription.py
--rw-r--r--   0 root         (0) root         (0)    12390 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/delivery.py
--rw-r--r--   0 root         (0) root         (0)    13637 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/email_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     9337 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     8021 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9510 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     6425 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9539 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10704 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     5086 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/manual_event.py
--rw-r--r--   0 root         (0) root         (0)     7863 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/manual_event_body.py
--rw-r--r--   0 root         (0) root         (0)     6827 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/manual_event_header.py
--rw-r--r--   0 root         (0) root         (0)     4162 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/manual_event_request.py
--rw-r--r--   0 root         (0) root         (0)     7436 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)    18055 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/notification.py
--rw-r--r--   0 root         (0) root         (0)     5154 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/notification_status.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7768 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7320 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/resource_list_of_delivery.py
--rw-r--r--   0 root         (0) root         (0)     7516 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/resource_list_of_event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     7432 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/resource_list_of_notification.py
--rw-r--r--   0 root         (0) root         (0)     7432 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/resource_list_of_subscription.py
--rw-r--r--   0 root         (0) root         (0)     6722 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/sms_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    14424 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/subscription.py
--rw-r--r--   0 root         (0) root         (0)     9020 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/update_notification_request.py
--rw-r--r--   0 root         (0) root         (0)     9723 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/update_subscription.py
--rw-r--r--   0 root         (0) root         (0)    14497 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/models/webhook_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    13560 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 12:02:19.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/utilities/
--rw-r--r--   0 root         (0) root         (0)       64 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 12:02:19.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      371 2023-05-30 12:02:19.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2734 2023-05-30 12:02:19.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 12:02:19.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-05-30 12:02:19.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-30 12:02:19.000000 lusid-notification-sdk-preview-0.1.711/lusid_notification_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 12:02:19.000000 lusid-notification-sdk-preview-0.1.711/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2319 2023-05-30 12:02:01.000000 lusid-notification-sdk-preview-0.1.711/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:25:41.000000 lusid-notification-sdk-preview-0.1.715/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      379 2023-05-31 12:25:41.000000 lusid-notification-sdk-preview-0.1.715/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8040 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:25:41.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/
+-rw-r--r--   0 root         (0) root         (0)     4452 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:25:41.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/api/
+-rw-r--r--   0 root         (0) root         (0)      506 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6847 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    10519 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/api/deliveries_api.py
+-rw-r--r--   0 root         (0) root         (0)    13984 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/api/event_types_api.py
+-rw-r--r--   0 root         (0) root         (0)     7820 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/api/manual_event_api.py
+-rw-r--r--   0 root         (0) root         (0)    52797 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/api/notifications_api.py
+-rw-r--r--   0 root         (0) root         (0)    47803 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/api/subscriptions_api.py
+-rw-r--r--   0 root         (0) root         (0)    27431 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16631 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:25:41.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/
+-rw-r--r--   0 root         (0) root         (0)     3100 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7254 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     9017 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7231 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)    10957 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/amazon_sqs_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     9234 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/api_request_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     6508 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/attempt.py
+-rw-r--r--   0 root         (0) root         (0)     5556 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/attempt_status.py
+-rw-r--r--   0 root         (0) root         (0)    11191 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/create_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    10603 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/create_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    12390 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/delivery.py
+-rw-r--r--   0 root         (0) root         (0)    14935 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/email_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     9337 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     8021 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9510 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     6425 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9539 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10704 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     5086 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/manual_event.py
+-rw-r--r--   0 root         (0) root         (0)     7863 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/manual_event_body.py
+-rw-r--r--   0 root         (0) root         (0)     6827 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/manual_event_header.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/manual_event_request.py
+-rw-r--r--   0 root         (0) root         (0)     7436 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    14867 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/notification.py
+-rw-r--r--   0 root         (0) root         (0)     5154 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/notification_status.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7768 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7320 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/resource_list_of_delivery.py
+-rw-r--r--   0 root         (0) root         (0)     7516 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/resource_list_of_event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     7432 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/resource_list_of_notification.py
+-rw-r--r--   0 root         (0) root         (0)     7432 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/resource_list_of_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     8012 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/sms_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    14424 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     9020 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/update_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)     9723 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/update_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    15803 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/models/webhook_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    13560 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:25:41.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/utilities/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 12:25:41.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      379 2023-05-31 12:25:41.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2734 2023-05-31 12:25:41.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 12:25:41.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-05-31 12:25:41.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-31 12:25:41.000000 lusid-notification-sdk-preview-0.1.715/lusid_notification_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 12:25:41.000000 lusid-notification-sdk-preview-0.1.715/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-05-31 12:25:06.000000 lusid-notification-sdk-preview-0.1.715/setup.py
```

### Comparing `lusid-notification-sdk-preview-0.1.711/README.md` & `lusid-notification-sdk-preview-0.1.715/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-notification-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.711
-- Package version: 0.1.711
+- API version: 0.1.715
+- Package version: 0.1.715
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/__init__.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.711"
+__version__ = "0.1.715"
 
 # import apis into sdk package
 from lusid_notification.api.application_metadata_api import ApplicationMetadataApi
 from lusid_notification.api.deliveries_api import DeliveriesApi
 from lusid_notification.api.event_types_api import EventTypesApi
 from lusid_notification.api.manual_event_api import ManualEventApi
 from lusid_notification.api.notifications_api import NotificationsApi
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/api/application_metadata_api.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/api/application_metadata_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -141,15 +141,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.711'
+        header_params['X-LUSID-SDK-Version'] = '0.1.715'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
         }
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/api/deliveries_api.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/api/deliveries_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -179,15 +179,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.711'
+        header_params['X-LUSID-SDK-Version'] = '0.1.715'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfDelivery",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/api/event_types_api.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/api/event_types_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -160,15 +160,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.711'
+        header_params['X-LUSID-SDK-Version'] = '0.1.715'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "EventTypeSchema",
             400: "LusidValidationProblemDetails",
@@ -292,15 +292,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.711'
+        header_params['X-LUSID-SDK-Version'] = '0.1.715'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfEventTypeSchema",
             404: "str",
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/api/manual_event_api.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/api/manual_event_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -155,15 +155,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.711'
+        header_params['X-LUSID-SDK-Version'] = '0.1.715'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "ManualEvent",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/api/notifications_api.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/api/notifications_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -195,15 +195,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.711'
+        header_params['X-LUSID-SDK-Version'] = '0.1.715'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -375,15 +375,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.711'
+        header_params['X-LUSID-SDK-Version'] = '0.1.715'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -552,15 +552,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.711'
+        header_params['X-LUSID-SDK-Version'] = '0.1.715'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -722,15 +722,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.711'
+        header_params['X-LUSID-SDK-Version'] = '0.1.715'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfNotification",
             400: "LusidValidationProblemDetails",
@@ -925,15 +925,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.711'
+        header_params['X-LUSID-SDK-Version'] = '0.1.715'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/api/subscriptions_api.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/api/subscriptions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -157,15 +157,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.711'
+        header_params['X-LUSID-SDK-Version'] = '0.1.715'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -326,15 +326,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.711'
+        header_params['X-LUSID-SDK-Version'] = '0.1.715'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -492,15 +492,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.711'
+        header_params['X-LUSID-SDK-Version'] = '0.1.715'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -680,15 +680,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.711'
+        header_params['X-LUSID-SDK-Version'] = '0.1.715'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfSubscription",
             400: "LusidValidationProblemDetails",
@@ -863,15 +863,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.711'
+        header_params['X-LUSID-SDK-Version'] = '0.1.715'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/api_client.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.711/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.715/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/configuration.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.711\n"\
-               "SDK Package Version: 0.1.711".\
+               "Version of the API: 0.1.715\n"\
+               "SDK Package Version: 0.1.715".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/exceptions.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/__init__.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/access_controlled_action.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/access_controlled_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/action_id.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/action_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/amazon_sqs_notification_type.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/amazon_sqs_notification_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -35,63 +35,98 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
+        'type': 'str',
         'api_key_ref': 'str',
         'api_secret_ref': 'str',
         'body': 'str',
         'queue_url_ref': 'str'
     }
 
     attribute_map = {
+        'type': 'type',
         'api_key_ref': 'apiKeyRef',
         'api_secret_ref': 'apiSecretRef',
         'body': 'body',
         'queue_url_ref': 'queueUrlRef'
     }
 
     required_map = {
+        'type': 'required',
         'api_key_ref': 'required',
         'api_secret_ref': 'required',
         'body': 'required',
         'queue_url_ref': 'required'
     }
 
-    def __init__(self, api_key_ref=None, api_secret_ref=None, body=None, queue_url_ref=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, type=None, api_key_ref=None, api_secret_ref=None, body=None, queue_url_ref=None, local_vars_configuration=None):  # noqa: E501
         """AmazonSqsNotificationType - a model defined in OpenAPI"
         
+        :param type:  The type of delivery mechanism for this notification (required)
+        :type type: str
         :param api_key_ref:  Reference to API key from Configuration Store (required)
         :type api_key_ref: str
         :param api_secret_ref:  Reference to API secret from Configuration Store (required)
         :type api_secret_ref: str
         :param body:  The body of the Amazon Queue Message (required)
         :type body: str
         :param queue_url_ref:  Reference to queue url from Configuration Store (required)
         :type queue_url_ref: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
+        self._type = None
         self._api_key_ref = None
         self._api_secret_ref = None
         self._body = None
         self._queue_url_ref = None
         self.discriminator = None
 
+        self.type = type
         self.api_key_ref = api_key_ref
         self.api_secret_ref = api_secret_ref
         self.body = body
         self.queue_url_ref = queue_url_ref
 
     @property
+    def type(self):
+        """Gets the type of this AmazonSqsNotificationType.  # noqa: E501
+
+        The type of delivery mechanism for this notification  # noqa: E501
+
+        :return: The type of this AmazonSqsNotificationType.  # noqa: E501
+        :rtype: str
+        """
+        return self._type
+
+    @type.setter
+    def type(self, type):
+        """Sets the type of this AmazonSqsNotificationType.
+
+        The type of delivery mechanism for this notification  # noqa: E501
+
+        :param type: The type of this AmazonSqsNotificationType.  # noqa: E501
+        :type type: str
+        """
+        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
+            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                type is not None and len(type) < 1):
+            raise ValueError("Invalid value for `type`, length must be greater than or equal to `1`")  # noqa: E501
+
+        self._type = type
+
+    @property
     def api_key_ref(self):
         """Gets the api_key_ref of this AmazonSqsNotificationType.  # noqa: E501
 
         Reference to API key from Configuration Store  # noqa: E501
 
         :return: The api_key_ref of this AmazonSqsNotificationType.  # noqa: E501
         :rtype: str
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/api_request_notification_type.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/api_request_notification_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -35,56 +35,91 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
+        'type': 'str',
         'http_method': 'str',
         'path_and_query': 'str',
         'content': 'object'
     }
 
     attribute_map = {
+        'type': 'type',
         'http_method': 'httpMethod',
         'path_and_query': 'pathAndQuery',
         'content': 'content'
     }
 
     required_map = {
+        'type': 'required',
         'http_method': 'required',
         'path_and_query': 'required',
         'content': 'optional'
     }
 
-    def __init__(self, http_method=None, path_and_query=None, content=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, type=None, http_method=None, path_and_query=None, content=None, local_vars_configuration=None):  # noqa: E501
         """ApiRequestNotificationType - a model defined in OpenAPI"
         
+        :param type:  The type of delivery mechanism for this notification (required)
+        :type type: str
         :param http_method:  The HTTP method such as GET, POST, etc. to use on the Api Request (required)
         :type http_method: str
         :param path_and_query:  The url to send the request to. (required)
         :type path_and_query: str
         :param content:  The content of the request
         :type content: object
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
+        self._type = None
         self._http_method = None
         self._path_and_query = None
         self._content = None
         self.discriminator = None
 
+        self.type = type
         self.http_method = http_method
         self.path_and_query = path_and_query
         self.content = content
 
     @property
+    def type(self):
+        """Gets the type of this ApiRequestNotificationType.  # noqa: E501
+
+        The type of delivery mechanism for this notification  # noqa: E501
+
+        :return: The type of this ApiRequestNotificationType.  # noqa: E501
+        :rtype: str
+        """
+        return self._type
+
+    @type.setter
+    def type(self, type):
+        """Sets the type of this ApiRequestNotificationType.
+
+        The type of delivery mechanism for this notification  # noqa: E501
+
+        :param type: The type of this ApiRequestNotificationType.  # noqa: E501
+        :type type: str
+        """
+        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
+            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                type is not None and len(type) < 1):
+            raise ValueError("Invalid value for `type`, length must be greater than or equal to `1`")  # noqa: E501
+
+        self._type = type
+
+    @property
     def http_method(self):
         """Gets the http_method of this ApiRequestNotificationType.  # noqa: E501
 
         The HTTP method such as GET, POST, etc. to use on the Api Request  # noqa: E501
 
         :return: The http_method of this ApiRequestNotificationType.  # noqa: E501
         :rtype: str
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/attempt.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/attempt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/attempt_status.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/attempt_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/create_notification_request.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/create_notification_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/create_subscription.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/create_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/delivery.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/delivery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/email_notification_type.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/email_notification_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -35,43 +35,48 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
+        'type': 'str',
         'subject': 'str',
         'plain_text_body': 'str',
         'html_body': 'str',
         'email_address_to': 'list[str]',
         'email_address_cc': 'list[str]',
         'email_address_bcc': 'list[str]'
     }
 
     attribute_map = {
+        'type': 'type',
         'subject': 'subject',
         'plain_text_body': 'plainTextBody',
         'html_body': 'htmlBody',
         'email_address_to': 'emailAddressTo',
         'email_address_cc': 'emailAddressCc',
         'email_address_bcc': 'emailAddressBcc'
     }
 
     required_map = {
+        'type': 'required',
         'subject': 'required',
         'plain_text_body': 'required',
         'html_body': 'optional',
         'email_address_to': 'required',
         'email_address_cc': 'optional',
         'email_address_bcc': 'optional'
     }
 
-    def __init__(self, subject=None, plain_text_body=None, html_body=None, email_address_to=None, email_address_cc=None, email_address_bcc=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, type=None, subject=None, plain_text_body=None, html_body=None, email_address_to=None, email_address_cc=None, email_address_bcc=None, local_vars_configuration=None):  # noqa: E501
         """EmailNotificationType - a model defined in OpenAPI"
         
+        :param type:  The type of delivery mechanism for this notification (required)
+        :type type: str
         :param subject:  The subject of the email (required)
         :type subject: str
         :param plain_text_body:  The plain text body of the email (required)
         :type plain_text_body: str
         :param html_body:  The HTML body of the email (if any)
         :type html_body: str
         :param email_address_to:  'To' recipients of the email (required)
@@ -82,30 +87,60 @@
         :type email_address_bcc: list[str]
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
+        self._type = None
         self._subject = None
         self._plain_text_body = None
         self._html_body = None
         self._email_address_to = None
         self._email_address_cc = None
         self._email_address_bcc = None
         self.discriminator = None
 
+        self.type = type
         self.subject = subject
         self.plain_text_body = plain_text_body
         self.html_body = html_body
         self.email_address_to = email_address_to
         self.email_address_cc = email_address_cc
         self.email_address_bcc = email_address_bcc
 
     @property
+    def type(self):
+        """Gets the type of this EmailNotificationType.  # noqa: E501
+
+        The type of delivery mechanism for this notification  # noqa: E501
+
+        :return: The type of this EmailNotificationType.  # noqa: E501
+        :rtype: str
+        """
+        return self._type
+
+    @type.setter
+    def type(self, type):
+        """Sets the type of this EmailNotificationType.
+
+        The type of delivery mechanism for this notification  # noqa: E501
+
+        :param type: The type of this EmailNotificationType.  # noqa: E501
+        :type type: str
+        """
+        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
+            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                type is not None and len(type) < 1):
+            raise ValueError("Invalid value for `type`, length must be greater than or equal to `1`")  # noqa: E501
+
+        self._type = type
+
+    @property
     def subject(self):
         """Gets the subject of this EmailNotificationType.  # noqa: E501
 
         The subject of the email  # noqa: E501
 
         :return: The subject of this EmailNotificationType.  # noqa: E501
         :rtype: str
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/event_type_schema.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/id_selector_definition.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/id_selector_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/identifier_part_schema.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/identifier_part_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/link.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/lusid_problem_details.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/lusid_validation_problem_details.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/manual_event.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/manual_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/manual_event_body.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/manual_event_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/manual_event_header.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/manual_event_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/manual_event_request.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/manual_event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/matching_pattern.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/matching_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/notification.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/subscription.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -18,15 +18,15 @@
 import pprint
 import re  # noqa: F401
 import six
 
 from lusid_notification.configuration import Configuration
 
 
-class Notification(object):
+class Subscription(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
@@ -35,408 +35,327 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'id': 'str',
-        'description': 'str',
+        'id': 'ResourceId',
         'display_name': 'str',
-        'delivery_channel': 'str',
-        'recipients': 'dict(str, object)',
-        'content': 'dict(str, object)',
-        'status': 'NotificationStatus',
+        'description': 'str',
+        'status': 'str',
+        'matching_pattern': 'MatchingPattern',
         'created_at': 'datetime',
-        'created_by': 'str',
-        'last_modified_at': 'datetime',
-        'last_modified_by': 'str'
+        'user_id_created': 'str',
+        'modified_at': 'datetime',
+        'user_id_modified': 'str'
     }
 
     attribute_map = {
         'id': 'id',
-        'description': 'description',
         'display_name': 'displayName',
-        'delivery_channel': 'deliveryChannel',
-        'recipients': 'recipients',
-        'content': 'content',
+        'description': 'description',
         'status': 'status',
+        'matching_pattern': 'matchingPattern',
         'created_at': 'createdAt',
-        'created_by': 'createdBy',
-        'last_modified_at': 'lastModifiedAt',
-        'last_modified_by': 'lastModifiedBy'
+        'user_id_created': 'userIdCreated',
+        'modified_at': 'modifiedAt',
+        'user_id_modified': 'userIdModified'
     }
 
     required_map = {
         'id': 'required',
+        'display_name': 'required',
         'description': 'optional',
-        'display_name': 'optional',
-        'delivery_channel': 'required',
-        'recipients': 'required',
-        'content': 'required',
-        'status': 'optional',
+        'status': 'required',
+        'matching_pattern': 'required',
         'created_at': 'required',
-        'created_by': 'required',
-        'last_modified_at': 'required',
-        'last_modified_by': 'required'
+        'user_id_created': 'required',
+        'modified_at': 'required',
+        'user_id_modified': 'required'
     }
 
-    def __init__(self, id=None, description=None, display_name=None, delivery_channel=None, recipients=None, content=None, status=None, created_at=None, created_by=None, last_modified_at=None, last_modified_by=None, local_vars_configuration=None):  # noqa: E501
-        """Notification - a model defined in OpenAPI"
+    def __init__(self, id=None, display_name=None, description=None, status=None, matching_pattern=None, created_at=None, user_id_created=None, modified_at=None, user_id_modified=None, local_vars_configuration=None):  # noqa: E501
+        """Subscription - a model defined in OpenAPI"
         
-        :param id:  The identifier of the notification (required)
-        :type id: str
-        :param description:  The summary of the services provided by the notification
-        :type description: str
-        :param display_name:  The name of the notification
+        :param id:  (required)
+        :type id: lusid_notification.ResourceId
+        :param display_name:  The name of the subscription (required)
         :type display_name: str
-        :param delivery_channel:  The medium through which the notification is delivered (required)
-        :type delivery_channel: str
-        :param recipients:  Recipient of the notification (required)
-        :type recipients: dict(str, object)
-        :param content:  The contents of the notification (required)
-        :type content: dict(str, object)
-        :param status: 
-        :type status: lusid_notification.NotificationStatus
+        :param description:  The summary of the services provided by the subscription
+        :type description: str
+        :param status:  The current status of the subscription (required)
+        :type status: str
+        :param matching_pattern:  (required)
+        :type matching_pattern: lusid_notification.MatchingPattern
         :param created_at:  The time at which the subscription was made (required)
         :type created_at: datetime
-        :param created_by:  The user who made the subscription (required)
-        :type created_by: str
-        :param last_modified_at:  The time at which the subscription was last modified (required)
-        :type last_modified_at: datetime
-        :param last_modified_by:  The user who last modified the subscription (required)
-        :type last_modified_by: str
+        :param user_id_created:  The user who made the subscription (required)
+        :type user_id_created: str
+        :param modified_at:  The time at which the subscription was last modified (required)
+        :type modified_at: datetime
+        :param user_id_modified:  The user who last modified the subscription (required)
+        :type user_id_modified: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
-        self._description = None
         self._display_name = None
-        self._delivery_channel = None
-        self._recipients = None
-        self._content = None
+        self._description = None
         self._status = None
+        self._matching_pattern = None
         self._created_at = None
-        self._created_by = None
-        self._last_modified_at = None
-        self._last_modified_by = None
+        self._user_id_created = None
+        self._modified_at = None
+        self._user_id_modified = None
         self.discriminator = None
 
         self.id = id
-        self.description = description
         self.display_name = display_name
-        self.delivery_channel = delivery_channel
-        self.recipients = recipients
-        self.content = content
-        if status is not None:
-            self.status = status
+        self.description = description
+        self.status = status
+        self.matching_pattern = matching_pattern
         self.created_at = created_at
-        self.created_by = created_by
-        self.last_modified_at = last_modified_at
-        self.last_modified_by = last_modified_by
+        self.user_id_created = user_id_created
+        self.modified_at = modified_at
+        self.user_id_modified = user_id_modified
 
     @property
     def id(self):
-        """Gets the id of this Notification.  # noqa: E501
+        """Gets the id of this Subscription.  # noqa: E501
 
-        The identifier of the notification  # noqa: E501
 
-        :return: The id of this Notification.  # noqa: E501
-        :rtype: str
+        :return: The id of this Subscription.  # noqa: E501
+        :rtype: lusid_notification.ResourceId
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this Notification.
+        """Sets the id of this Subscription.
 
-        The identifier of the notification  # noqa: E501
 
-        :param id: The id of this Notification.  # noqa: E501
-        :type id: str
+        :param id: The id of this Subscription.  # noqa: E501
+        :type id: lusid_notification.ResourceId
         """
         if self.local_vars_configuration.client_side_validation and id is None:  # noqa: E501
             raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                id is not None and len(id) < 1):
-            raise ValueError("Invalid value for `id`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._id = id
 
     @property
-    def description(self):
-        """Gets the description of this Notification.  # noqa: E501
-
-        The summary of the services provided by the notification  # noqa: E501
-
-        :return: The description of this Notification.  # noqa: E501
-        :rtype: str
-        """
-        return self._description
-
-    @description.setter
-    def description(self, description):
-        """Sets the description of this Notification.
-
-        The summary of the services provided by the notification  # noqa: E501
-
-        :param description: The description of this Notification.  # noqa: E501
-        :type description: str
-        """
-        if (self.local_vars_configuration.client_side_validation and
-                description is not None and len(description) > 512):
-            raise ValueError("Invalid value for `description`, length must be less than or equal to `512`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                description is not None and len(description) < 1):
-            raise ValueError("Invalid value for `description`, length must be greater than or equal to `1`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                description is not None and not re.search(r'^[\s\S]*$', description)):  # noqa: E501
-            raise ValueError(r"Invalid value for `description`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
-
-        self._description = description
-
-    @property
     def display_name(self):
-        """Gets the display_name of this Notification.  # noqa: E501
+        """Gets the display_name of this Subscription.  # noqa: E501
 
-        The name of the notification  # noqa: E501
+        The name of the subscription  # noqa: E501
 
-        :return: The display_name of this Notification.  # noqa: E501
+        :return: The display_name of this Subscription.  # noqa: E501
         :rtype: str
         """
         return self._display_name
 
     @display_name.setter
     def display_name(self, display_name):
-        """Sets the display_name of this Notification.
+        """Sets the display_name of this Subscription.
 
-        The name of the notification  # noqa: E501
+        The name of the subscription  # noqa: E501
 
-        :param display_name: The display_name of this Notification.  # noqa: E501
+        :param display_name: The display_name of this Subscription.  # noqa: E501
         :type display_name: str
         """
+        if self.local_vars_configuration.client_side_validation and display_name is None:  # noqa: E501
+            raise ValueError("Invalid value for `display_name`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                display_name is not None and len(display_name) > 64):
-            raise ValueError("Invalid value for `display_name`, length must be less than or equal to `64`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                display_name is not None and len(display_name) < 0):
-            raise ValueError("Invalid value for `display_name`, length must be greater than or equal to `0`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                display_name is not None and not re.search(r'^[\s\S]*$', display_name)):  # noqa: E501
-            raise ValueError(r"Invalid value for `display_name`, must be a follow pattern or equal to `/^[\s\S]*$/`")  # noqa: E501
+                display_name is not None and len(display_name) < 1):
+            raise ValueError("Invalid value for `display_name`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._display_name = display_name
 
     @property
-    def delivery_channel(self):
-        """Gets the delivery_channel of this Notification.  # noqa: E501
+    def description(self):
+        """Gets the description of this Subscription.  # noqa: E501
 
-        The medium through which the notification is delivered  # noqa: E501
+        The summary of the services provided by the subscription  # noqa: E501
 
-        :return: The delivery_channel of this Notification.  # noqa: E501
+        :return: The description of this Subscription.  # noqa: E501
         :rtype: str
         """
-        return self._delivery_channel
-
-    @delivery_channel.setter
-    def delivery_channel(self, delivery_channel):
-        """Sets the delivery_channel of this Notification.
-
-        The medium through which the notification is delivered  # noqa: E501
-
-        :param delivery_channel: The delivery_channel of this Notification.  # noqa: E501
-        :type delivery_channel: str
-        """
-        if self.local_vars_configuration.client_side_validation and delivery_channel is None:  # noqa: E501
-            raise ValueError("Invalid value for `delivery_channel`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                delivery_channel is not None and len(delivery_channel) < 1):
-            raise ValueError("Invalid value for `delivery_channel`, length must be greater than or equal to `1`")  # noqa: E501
-
-        self._delivery_channel = delivery_channel
-
-    @property
-    def recipients(self):
-        """Gets the recipients of this Notification.  # noqa: E501
-
-        Recipient of the notification  # noqa: E501
-
-        :return: The recipients of this Notification.  # noqa: E501
-        :rtype: dict(str, object)
-        """
-        return self._recipients
+        return self._description
 
-    @recipients.setter
-    def recipients(self, recipients):
-        """Sets the recipients of this Notification.
+    @description.setter
+    def description(self, description):
+        """Sets the description of this Subscription.
 
-        Recipient of the notification  # noqa: E501
+        The summary of the services provided by the subscription  # noqa: E501
 
-        :param recipients: The recipients of this Notification.  # noqa: E501
-        :type recipients: dict(str, object)
+        :param description: The description of this Subscription.  # noqa: E501
+        :type description: str
         """
-        if self.local_vars_configuration.client_side_validation and recipients is None:  # noqa: E501
-            raise ValueError("Invalid value for `recipients`, must not be `None`")  # noqa: E501
 
-        self._recipients = recipients
+        self._description = description
 
     @property
-    def content(self):
-        """Gets the content of this Notification.  # noqa: E501
+    def status(self):
+        """Gets the status of this Subscription.  # noqa: E501
 
-        The contents of the notification  # noqa: E501
+        The current status of the subscription  # noqa: E501
 
-        :return: The content of this Notification.  # noqa: E501
-        :rtype: dict(str, object)
+        :return: The status of this Subscription.  # noqa: E501
+        :rtype: str
         """
-        return self._content
+        return self._status
 
-    @content.setter
-    def content(self, content):
-        """Sets the content of this Notification.
+    @status.setter
+    def status(self, status):
+        """Sets the status of this Subscription.
 
-        The contents of the notification  # noqa: E501
+        The current status of the subscription  # noqa: E501
 
-        :param content: The content of this Notification.  # noqa: E501
-        :type content: dict(str, object)
+        :param status: The status of this Subscription.  # noqa: E501
+        :type status: str
         """
-        if self.local_vars_configuration.client_side_validation and content is None:  # noqa: E501
-            raise ValueError("Invalid value for `content`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and status is None:  # noqa: E501
+            raise ValueError("Invalid value for `status`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                status is not None and len(status) < 1):
+            raise ValueError("Invalid value for `status`, length must be greater than or equal to `1`")  # noqa: E501
 
-        self._content = content
+        self._status = status
 
     @property
-    def status(self):
-        """Gets the status of this Notification.  # noqa: E501
+    def matching_pattern(self):
+        """Gets the matching_pattern of this Subscription.  # noqa: E501
 
 
-        :return: The status of this Notification.  # noqa: E501
-        :rtype: lusid_notification.NotificationStatus
+        :return: The matching_pattern of this Subscription.  # noqa: E501
+        :rtype: lusid_notification.MatchingPattern
         """
-        return self._status
+        return self._matching_pattern
 
-    @status.setter
-    def status(self, status):
-        """Sets the status of this Notification.
+    @matching_pattern.setter
+    def matching_pattern(self, matching_pattern):
+        """Sets the matching_pattern of this Subscription.
 
 
-        :param status: The status of this Notification.  # noqa: E501
-        :type status: lusid_notification.NotificationStatus
+        :param matching_pattern: The matching_pattern of this Subscription.  # noqa: E501
+        :type matching_pattern: lusid_notification.MatchingPattern
         """
+        if self.local_vars_configuration.client_side_validation and matching_pattern is None:  # noqa: E501
+            raise ValueError("Invalid value for `matching_pattern`, must not be `None`")  # noqa: E501
 
-        self._status = status
+        self._matching_pattern = matching_pattern
 
     @property
     def created_at(self):
-        """Gets the created_at of this Notification.  # noqa: E501
+        """Gets the created_at of this Subscription.  # noqa: E501
 
         The time at which the subscription was made  # noqa: E501
 
-        :return: The created_at of this Notification.  # noqa: E501
+        :return: The created_at of this Subscription.  # noqa: E501
         :rtype: datetime
         """
         return self._created_at
 
     @created_at.setter
     def created_at(self, created_at):
-        """Sets the created_at of this Notification.
+        """Sets the created_at of this Subscription.
 
         The time at which the subscription was made  # noqa: E501
 
-        :param created_at: The created_at of this Notification.  # noqa: E501
+        :param created_at: The created_at of this Subscription.  # noqa: E501
         :type created_at: datetime
         """
         if self.local_vars_configuration.client_side_validation and created_at is None:  # noqa: E501
             raise ValueError("Invalid value for `created_at`, must not be `None`")  # noqa: E501
 
         self._created_at = created_at
 
     @property
-    def created_by(self):
-        """Gets the created_by of this Notification.  # noqa: E501
+    def user_id_created(self):
+        """Gets the user_id_created of this Subscription.  # noqa: E501
 
         The user who made the subscription  # noqa: E501
 
-        :return: The created_by of this Notification.  # noqa: E501
+        :return: The user_id_created of this Subscription.  # noqa: E501
         :rtype: str
         """
-        return self._created_by
+        return self._user_id_created
 
-    @created_by.setter
-    def created_by(self, created_by):
-        """Sets the created_by of this Notification.
+    @user_id_created.setter
+    def user_id_created(self, user_id_created):
+        """Sets the user_id_created of this Subscription.
 
         The user who made the subscription  # noqa: E501
 
-        :param created_by: The created_by of this Notification.  # noqa: E501
-        :type created_by: str
+        :param user_id_created: The user_id_created of this Subscription.  # noqa: E501
+        :type user_id_created: str
         """
-        if self.local_vars_configuration.client_side_validation and created_by is None:  # noqa: E501
-            raise ValueError("Invalid value for `created_by`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and user_id_created is None:  # noqa: E501
+            raise ValueError("Invalid value for `user_id_created`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                created_by is not None and len(created_by) < 1):
-            raise ValueError("Invalid value for `created_by`, length must be greater than or equal to `1`")  # noqa: E501
+                user_id_created is not None and len(user_id_created) < 1):
+            raise ValueError("Invalid value for `user_id_created`, length must be greater than or equal to `1`")  # noqa: E501
 
-        self._created_by = created_by
+        self._user_id_created = user_id_created
 
     @property
-    def last_modified_at(self):
-        """Gets the last_modified_at of this Notification.  # noqa: E501
+    def modified_at(self):
+        """Gets the modified_at of this Subscription.  # noqa: E501
 
         The time at which the subscription was last modified  # noqa: E501
 
-        :return: The last_modified_at of this Notification.  # noqa: E501
+        :return: The modified_at of this Subscription.  # noqa: E501
         :rtype: datetime
         """
-        return self._last_modified_at
+        return self._modified_at
 
-    @last_modified_at.setter
-    def last_modified_at(self, last_modified_at):
-        """Sets the last_modified_at of this Notification.
+    @modified_at.setter
+    def modified_at(self, modified_at):
+        """Sets the modified_at of this Subscription.
 
         The time at which the subscription was last modified  # noqa: E501
 
-        :param last_modified_at: The last_modified_at of this Notification.  # noqa: E501
-        :type last_modified_at: datetime
+        :param modified_at: The modified_at of this Subscription.  # noqa: E501
+        :type modified_at: datetime
         """
-        if self.local_vars_configuration.client_side_validation and last_modified_at is None:  # noqa: E501
-            raise ValueError("Invalid value for `last_modified_at`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and modified_at is None:  # noqa: E501
+            raise ValueError("Invalid value for `modified_at`, must not be `None`")  # noqa: E501
 
-        self._last_modified_at = last_modified_at
+        self._modified_at = modified_at
 
     @property
-    def last_modified_by(self):
-        """Gets the last_modified_by of this Notification.  # noqa: E501
+    def user_id_modified(self):
+        """Gets the user_id_modified of this Subscription.  # noqa: E501
 
         The user who last modified the subscription  # noqa: E501
 
-        :return: The last_modified_by of this Notification.  # noqa: E501
+        :return: The user_id_modified of this Subscription.  # noqa: E501
         :rtype: str
         """
-        return self._last_modified_by
+        return self._user_id_modified
 
-    @last_modified_by.setter
-    def last_modified_by(self, last_modified_by):
-        """Sets the last_modified_by of this Notification.
+    @user_id_modified.setter
+    def user_id_modified(self, user_id_modified):
+        """Sets the user_id_modified of this Subscription.
 
         The user who last modified the subscription  # noqa: E501
 
-        :param last_modified_by: The last_modified_by of this Notification.  # noqa: E501
-        :type last_modified_by: str
+        :param user_id_modified: The user_id_modified of this Subscription.  # noqa: E501
+        :type user_id_modified: str
         """
-        if self.local_vars_configuration.client_side_validation and last_modified_by is None:  # noqa: E501
-            raise ValueError("Invalid value for `last_modified_by`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and user_id_modified is None:  # noqa: E501
+            raise ValueError("Invalid value for `user_id_modified`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
-                last_modified_by is not None and len(last_modified_by) < 1):
-            raise ValueError("Invalid value for `last_modified_by`, length must be greater than or equal to `1`")  # noqa: E501
+                user_id_modified is not None and len(user_id_modified) < 1):
+            raise ValueError("Invalid value for `user_id_modified`, length must be greater than or equal to `1`")  # noqa: E501
 
-        self._last_modified_by = last_modified_by
+        self._user_id_modified = user_id_modified
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
@@ -472,18 +391,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Notification):
+        if not isinstance(other, Subscription):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Notification):
+        if not isinstance(other, Subscription):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/notification_status.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/notification_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/resource_id.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/resource_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/resource_list_of_access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/resource_list_of_access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/resource_list_of_delivery.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/resource_list_of_delivery.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/resource_list_of_event_type_schema.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/resource_list_of_event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/resource_list_of_notification.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/resource_list_of_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/resource_list_of_subscription.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/resource_list_of_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/sms_notification_type.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/sms_notification_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -35,49 +35,84 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
+        'type': 'str',
         'body': 'str',
         'recipients': 'list[str]'
     }
 
     attribute_map = {
+        'type': 'type',
         'body': 'body',
         'recipients': 'recipients'
     }
 
     required_map = {
+        'type': 'required',
         'body': 'required',
         'recipients': 'required'
     }
 
-    def __init__(self, body=None, recipients=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, type=None, body=None, recipients=None, local_vars_configuration=None):  # noqa: E501
         """SmsNotificationType - a model defined in OpenAPI"
         
+        :param type:  The type of delivery mechanism for this notification (required)
+        :type type: str
         :param body:  The body of the SMS (required)
         :type body: str
         :param recipients:  The phone numbers to which the SMS will be sent to (E.164 format) (required)
         :type recipients: list[str]
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
+        self._type = None
         self._body = None
         self._recipients = None
         self.discriminator = None
 
+        self.type = type
         self.body = body
         self.recipients = recipients
 
     @property
+    def type(self):
+        """Gets the type of this SmsNotificationType.  # noqa: E501
+
+        The type of delivery mechanism for this notification  # noqa: E501
+
+        :return: The type of this SmsNotificationType.  # noqa: E501
+        :rtype: str
+        """
+        return self._type
+
+    @type.setter
+    def type(self, type):
+        """Sets the type of this SmsNotificationType.
+
+        The type of delivery mechanism for this notification  # noqa: E501
+
+        :param type: The type of this SmsNotificationType.  # noqa: E501
+        :type type: str
+        """
+        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
+            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                type is not None and len(type) < 1):
+            raise ValueError("Invalid value for `type`, length must be greater than or equal to `1`")  # noqa: E501
+
+        self._type = type
+
+    @property
     def body(self):
         """Gets the body of this SmsNotificationType.  # noqa: E501
 
         The body of the SMS  # noqa: E501
 
         :return: The body of this SmsNotificationType.  # noqa: E501
         :rtype: str
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/update_notification_request.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/update_notification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/update_subscription.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/update_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/models/webhook_notification_type.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/models/webhook_notification_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -35,43 +35,48 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
+        'type': 'str',
         'http_method': 'str',
         'url': 'str',
         'authentication_type': 'str',
         'authentication_configuration_item_paths': 'dict(str, str)',
         'content_type': 'str',
         'content': 'object'
     }
 
     attribute_map = {
+        'type': 'type',
         'http_method': 'httpMethod',
         'url': 'url',
         'authentication_type': 'authenticationType',
         'authentication_configuration_item_paths': 'authenticationConfigurationItemPaths',
         'content_type': 'contentType',
         'content': 'content'
     }
 
     required_map = {
+        'type': 'required',
         'http_method': 'required',
         'url': 'required',
         'authentication_type': 'required',
         'authentication_configuration_item_paths': 'optional',
         'content_type': 'required',
         'content': 'optional'
     }
 
-    def __init__(self, http_method=None, url=None, authentication_type=None, authentication_configuration_item_paths=None, content_type=None, content=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, type=None, http_method=None, url=None, authentication_type=None, authentication_configuration_item_paths=None, content_type=None, content=None, local_vars_configuration=None):  # noqa: E501
         """WebhookNotificationType - a model defined in OpenAPI"
         
+        :param type:  The type of delivery mechanism for this notification (required)
+        :type type: str
         :param http_method:  The HTTP method such as GET, POST, etc. to use on the request (required)
         :type http_method: str
         :param url:  The URL to send the request to (required)
         :type url: str
         :param authentication_type:  The type of authentication to use on the request (required)
         :type authentication_type: str
         :param authentication_configuration_item_paths:  The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }
@@ -82,30 +87,60 @@
         :type content: object
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
+        self._type = None
         self._http_method = None
         self._url = None
         self._authentication_type = None
         self._authentication_configuration_item_paths = None
         self._content_type = None
         self._content = None
         self.discriminator = None
 
+        self.type = type
         self.http_method = http_method
         self.url = url
         self.authentication_type = authentication_type
         self.authentication_configuration_item_paths = authentication_configuration_item_paths
         self.content_type = content_type
         self.content = content
 
     @property
+    def type(self):
+        """Gets the type of this WebhookNotificationType.  # noqa: E501
+
+        The type of delivery mechanism for this notification  # noqa: E501
+
+        :return: The type of this WebhookNotificationType.  # noqa: E501
+        :rtype: str
+        """
+        return self._type
+
+    @type.setter
+    def type(self, type):
+        """Sets the type of this WebhookNotificationType.
+
+        The type of delivery mechanism for this notification  # noqa: E501
+
+        :param type: The type of this WebhookNotificationType.  # noqa: E501
+        :type type: str
+        """
+        if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
+            raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
+        if (self.local_vars_configuration.client_side_validation and
+                type is not None and len(type) < 1):
+            raise ValueError("Invalid value for `type`, length must be greater than or equal to `1`")  # noqa: E501
+
+        self._type = type
+
+    @property
     def http_method(self):
         """Gets the http_method of this WebhookNotificationType.  # noqa: E501
 
         The HTTP method such as GET, POST, etc. to use on the request  # noqa: E501
 
         :return: The http_method of this WebhookNotificationType.  # noqa: E501
         :rtype: str
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/rest.py` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.711
+    The version of the OpenAPI document: 0.1.715
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification/utilities/config_keys.json` & `lusid-notification-sdk-preview-0.1.715/lusid_notification/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-notification-sdk-preview-0.1.711/lusid_notification_sdk_preview.egg-info/SOURCES.txt` & `lusid-notification-sdk-preview-0.1.715/lusid_notification_sdk_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lusid-notification-sdk-preview-0.1.711/setup.py` & `lusid-notification-sdk-preview-0.1.715/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     exec(fp.read(), version)
 
 setup(
 
     name='lusid-notification-sdk-preview',
     version=version['__version__'],
     description='Python Preview SDK for Notification API',
-    url='https://github.com/finbourne/notifications-sdk-python-preview',
+    url='https://github.com/finbourne/notifications-sdk-python-preview/tree/v2',
     author='FINBOURNE Technology',
     author_email='engineering@finbourne.com',
     license='MIT',
     keywords=["OpenAPI", "FINBOURNE", "LUSID", "Notifications API"],
     install_requires=REQUIRES,
     packages=find_packages(exclude=['tests*']),
     include_package_data=True
```

