# Comparing `tmp/qwak_core-0.0.89.tar.gz` & `tmp/qwak_core-0.0.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.89.tar", max compression
+gzip compressed data, was "qwak_core-0.0.90.tar", max compression
```

## Comparing `qwak_core-0.0.89.tar` & `qwak_core-0.0.90.tar`

### file list

```diff
@@ -1,588 +1,588 @@
--rw-r--r--   0        0        0      264 2023-05-31 06:58:55.462013 qwak_core-0.0.89/README.md
--rw-r--r--   0        0        0        0 2023-05-31 07:00:44.034683 qwak_core-0.0.89/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-05-31 07:00:44.082683 qwak_core-0.0.89/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-05-31 07:00:20.226536 qwak_core-0.0.89/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.082683 qwak_core-0.0.89/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-05-31 07:00:44.078683 qwak_core-0.0.89/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-05-31 07:00:19.786534 qwak_core-0.0.89/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.078683 qwak_core-0.0.89/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-05-31 07:00:44.078683 qwak_core-0.0.89/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-05-31 07:00:20.006535 qwak_core-0.0.89/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.082683 qwak_core-0.0.89/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-05-31 07:00:44.070683 qwak_core-0.0.89/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-05-31 07:00:19.110530 qwak_core-0.0.89/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-05-31 07:00:44.070683 qwak_core-0.0.89/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-31 07:00:44.074683 qwak_core-0.0.89/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-05-31 07:00:19.326531 qwak_core-0.0.89/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.074683 qwak_core-0.0.89/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4901 2023-05-31 07:00:44.074683 qwak_core-0.0.89/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5995 2023-05-31 07:00:19.550532 qwak_core-0.0.89/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.074683 qwak_core-0.0.89/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-05-31 07:00:44.038683 qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-05-31 07:00:18.878528 qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-05-31 07:00:44.038683 qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5707 2023-05-31 07:00:44.038683 qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8170 2023-05-31 07:00:20.490538 qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.042683 qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-05-31 07:00:44.042683 qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-05-31 07:00:20.930541 qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.062683 qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-05-31 07:00:44.062683 qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-05-31 07:00:21.182542 qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-05-31 07:00:44.066683 qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-05-31 07:00:44.042683 qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-31 07:00:20.718539 qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.042683 qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-05-31 07:00:44.066683 qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-05-31 07:00:21.406544 qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.070683 qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-05-31 07:00:44.114684 qwak_core-0.0.89/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-05-31 07:00:24.678564 qwak_core-0.0.89/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.114684 qwak_core-0.0.89/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-05-31 07:00:44.118684 qwak_core-0.0.89/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-05-31 07:00:24.886565 qwak_core-0.0.89/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-05-31 07:00:44.118684 qwak_core-0.0.89/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-05-31 07:00:44.210684 qwak_core-0.0.89/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-05-31 07:00:31.098603 qwak_core-0.0.89/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.214684 qwak_core-0.0.89/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-05-31 07:00:44.214684 qwak_core-0.0.89/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-05-31 07:00:31.302605 qwak_core-0.0.89/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-05-31 07:00:44.214684 qwak_core-0.0.89/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-05-31 07:00:44.218684 qwak_core-0.0.89/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-05-31 07:00:32.306611 qwak_core-0.0.89/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-05-31 07:00:44.218684 qwak_core-0.0.89/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-05-31 07:00:44.214684 qwak_core-0.0.89/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-05-31 07:00:32.118610 qwak_core-0.0.89/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.218684 qwak_core-0.0.89/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5777 2023-05-31 07:00:44.222684 qwak_core-0.0.89/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8264 2023-05-31 07:00:32.502612 qwak_core-0.0.89/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.222684 qwak_core-0.0.89/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-05-31 07:00:44.222684 qwak_core-0.0.89/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-05-31 07:00:32.714613 qwak_core-0.0.89/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-05-31 07:00:44.222684 qwak_core-0.0.89/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    12352 2023-05-31 07:00:44.342685 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    18970 2023-05-31 07:00:41.326666 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.362685 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5775 2023-05-31 07:00:44.338685 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8308 2023-05-31 07:00:40.910664 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.338685 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-05-31 07:00:44.342685 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-05-31 07:00:41.102665 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.342685 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-05-31 07:00:44.334685 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-05-31 07:00:40.506661 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-05-31 07:00:44.334685 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-05-31 07:00:44.334685 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-05-31 07:00:40.714663 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.338685 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-05-31 07:00:44.370685 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-05-31 07:00:41.914670 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.370685 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-05-31 07:00:44.366685 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-05-31 07:00:41.718669 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.366685 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-05-31 07:00:44.362685 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-05-31 07:00:41.522668 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.366685 qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-05-31 07:00:44.330685 qwak_core-0.0.89/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-05-31 07:00:40.286660 qwak_core-0.0.89/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.334685 qwak_core-0.0.89/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-05-31 07:00:44.326685 qwak_core-0.0.89/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-05-31 07:00:39.866657 qwak_core-0.0.89/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.326685 qwak_core-0.0.89/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    42145 2023-05-31 07:00:44.330685 qwak_core-0.0.89/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    55993 2023-05-31 07:00:40.078659 qwak_core-0.0.89/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-05-31 07:00:44.330685 qwak_core-0.0.89/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    20255 2023-05-31 07:00:44.270685 qwak_core-0.0.89/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    17495 2023-05-31 07:00:34.750626 qwak_core-0.0.89/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    20359 2023-05-31 07:00:44.270685 qwak_core-0.0.89/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-05-31 07:00:44.266685 qwak_core-0.0.89/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-05-31 07:00:34.550625 qwak_core-0.0.89/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.270685 qwak_core-0.0.89/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11691 2023-05-31 07:00:44.238684 qwak_core-0.0.89/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18850 2023-05-31 07:00:34.158622 qwak_core-0.0.89/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.238684 qwak_core-0.0.89/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-05-31 07:00:44.242684 qwak_core-0.0.89/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-05-31 07:00:34.350623 qwak_core-0.0.89/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.242684 qwak_core-0.0.89/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-05-31 07:00:44.242684 qwak_core-0.0.89/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-05-31 07:00:34.942627 qwak_core-0.0.89/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-05-31 07:00:44.262684 qwak_core-0.0.89/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38290 2023-05-31 07:00:44.262684 qwak_core-0.0.89/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52702 2023-05-31 07:00:35.394630 qwak_core-0.0.89/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-05-31 07:00:44.266685 qwak_core-0.0.89/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-05-31 07:00:44.278685 qwak_core-0.0.89/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-05-31 07:00:35.794632 qwak_core-0.0.89/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.278685 qwak_core-0.0.89/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-05-31 07:00:44.278685 qwak_core-0.0.89/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-31 07:00:35.998633 qwak_core-0.0.89/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-31 07:00:44.282685 qwak_core-0.0.89/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-05-31 07:00:44.230684 qwak_core-0.0.89/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-05-31 07:00:33.554618 qwak_core-0.0.89/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.234684 qwak_core-0.0.89/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-05-31 07:00:44.234684 qwak_core-0.0.89/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-05-31 07:00:33.750620 qwak_core-0.0.89/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-05-31 07:00:44.234684 qwak_core-0.0.89/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-05-31 07:00:44.226684 qwak_core-0.0.89/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-05-31 07:00:33.138616 qwak_core-0.0.89/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.230684 qwak_core-0.0.89/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    43712 2023-05-31 07:00:44.226684 qwak_core-0.0.89/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    63341 2023-05-31 07:00:32.934615 qwak_core-0.0.89/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.226684 qwak_core-0.0.89/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-05-31 07:00:44.230684 qwak_core-0.0.89/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-05-31 07:00:33.362617 qwak_core-0.0.89/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-05-31 07:00:44.230684 qwak_core-0.0.89/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-05-31 07:00:44.102684 qwak_core-0.0.89/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-05-31 07:00:23.590557 qwak_core-0.0.89/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.102684 qwak_core-0.0.89/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-31 07:00:44.106684 qwak_core-0.0.89/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-05-31 07:00:23.818559 qwak_core-0.0.89/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.106684 qwak_core-0.0.89/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-05-31 07:00:44.106684 qwak_core-0.0.89/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-05-31 07:00:24.050560 qwak_core-0.0.89/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-05-31 07:00:44.110684 qwak_core-0.0.89/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-05-31 07:00:44.190684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-05-31 07:00:29.842596 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.190684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-05-31 07:00:44.190684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-05-31 07:00:29.610594 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-05-31 07:00:44.190684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0    11432 2023-05-31 07:00:44.142684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    12882 2023-05-31 07:00:27.350580 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.154684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5303 2023-05-31 07:00:44.142684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8604 2023-05-31 07:00:27.150579 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.142684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-05-31 07:00:44.134684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-05-31 07:00:26.522575 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.134684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    28920 2023-05-31 07:00:44.138684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20665 2023-05-31 07:00:26.954578 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    35307 2023-05-31 07:00:44.138684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-05-31 07:00:44.162684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-05-31 07:00:27.546581 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.162684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-05-31 07:00:44.166684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-05-31 07:00:27.746583 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-05-31 07:00:44.166684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    25269 2023-05-31 07:00:44.134684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    37664 2023-05-31 07:00:26.734576 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.138684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-05-31 07:00:44.170684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-31 07:00:27.946584 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.170684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0    10238 2023-05-31 07:00:44.174684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.py
--rw-r--r--   0        0        0    16741 2023-05-31 07:00:28.362587 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.174684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2_grpc.py
--rw-r--r--   0        0        0     3559 2023-05-31 07:00:44.178684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.py
--rw-r--r--   0        0        0     1759 2023-05-31 07:00:28.562588 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.pyi
--rw-r--r--   0        0        0     3608 2023-05-31 07:00:44.178684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0    11281 2023-05-31 07:00:44.170684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
--rw-r--r--   0        0        0    15070 2023-05-31 07:00:28.154585 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.174684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-05-31 07:00:44.194684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-05-31 07:00:43.422679 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.194684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-05-31 07:00:44.194684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-05-31 07:00:43.662681 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-05-31 07:00:44.198684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-05-31 07:00:44.198684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-05-31 07:00:30.454599 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.198684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-31 07:00:44.198684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-05-31 07:00:30.670601 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-05-31 07:00:44.202684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-05-31 07:00:44.202684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-05-31 07:00:30.894602 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.202684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-05-31 07:00:44.206684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-05-31 07:00:31.718607 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.206684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-05-31 07:00:44.206684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-05-31 07:00:31.510606 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-05-31 07:00:44.206684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-05-31 07:00:44.210684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-05-31 07:00:31.914608 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.210684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-05-31 07:00:44.178684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-05-31 07:00:28.762589 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.178684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-05-31 07:00:44.182684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-05-31 07:00:28.970590 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.182684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-05-31 07:00:44.182684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-05-31 07:00:29.174591 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-05-31 07:00:44.186684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-05-31 07:00:44.186684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-05-31 07:00:29.398593 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.186684 qwak_core-0.0.89/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-05-31 07:00:44.370685 qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-05-31 07:00:42.118671 qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.374685 qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-05-31 07:00:44.374685 qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-05-31 07:00:42.322672 qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-31 07:00:44.374685 qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-05-31 07:00:44.378685 qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-05-31 07:00:42.522674 qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.378685 qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-05-31 07:00:44.378685 qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-05-31 07:00:42.730675 qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-31 07:00:44.378685 qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-05-31 07:00:44.382685 qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-05-31 07:00:42.954676 qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-05-31 07:00:44.382685 qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-05-31 07:00:44.382685 qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-05-31 07:00:43.178678 qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.386685 qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-05-31 07:00:44.282685 qwak_core-0.0.89/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-05-31 07:00:36.202635 qwak_core-0.0.89/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.282685 qwak_core-0.0.89/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-05-31 07:00:44.286685 qwak_core-0.0.89/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-31 07:00:36.402636 qwak_core-0.0.89/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-31 07:00:44.286685 qwak_core-0.0.89/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-05-31 07:00:44.118684 qwak_core-0.0.89/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-05-31 07:00:25.710570 qwak_core-0.0.89/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.122684 qwak_core-0.0.89/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-31 07:00:44.122684 qwak_core-0.0.89/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-05-31 07:00:25.910571 qwak_core-0.0.89/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.126684 qwak_core-0.0.89/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-05-31 07:00:44.126684 qwak_core-0.0.89/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-05-31 07:00:26.110573 qwak_core-0.0.89/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-05-31 07:00:44.130684 qwak_core-0.0.89/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-05-31 07:00:44.130684 qwak_core-0.0.89/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-05-31 07:00:26.306574 qwak_core-0.0.89/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.134684 qwak_core-0.0.89/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-05-31 07:00:44.238684 qwak_core-0.0.89/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-05-31 07:00:33.950621 qwak_core-0.0.89/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-05-31 07:00:44.238684 qwak_core-0.0.89/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     3757 2023-05-31 07:00:44.286685 qwak_core-0.0.89/_qwak_proto/qwak/instance_template/instance_template_pb2.py
--rw-r--r--   0        0        0     4235 2023-05-31 07:00:36.606637 qwak_core-0.0.89/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.290685 qwak_core-0.0.89/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
--rw-r--r--   0        0        0     4722 2023-05-31 07:00:44.290685 qwak_core-0.0.89/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
--rw-r--r--   0        0        0     3245 2023-05-31 07:00:36.806639 qwak_core-0.0.89/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
--rw-r--r--   0        0        0     5240 2023-05-31 07:00:44.290685 qwak_core-0.0.89/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-05-31 07:00:44.306685 qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-05-31 07:00:38.002646 qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.306685 qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-05-31 07:00:44.306685 qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-05-31 07:00:38.198647 qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.306685 qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-05-31 07:00:44.310685 qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-05-31 07:00:38.394648 qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.310685 qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-05-31 07:00:44.310685 qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-05-31 07:00:38.594650 qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.314685 qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-31 07:00:44.314685 qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-05-31 07:00:38.802651 qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.314685 qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-05-31 07:00:44.318685 qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-05-31 07:00:39.034652 qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-05-31 07:00:44.318685 qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-05-31 07:00:44.318685 qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-05-31 07:00:39.234654 qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.318685 qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-05-31 07:00:44.294685 qwak_core-0.0.89/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-05-31 07:00:37.198641 qwak_core-0.0.89/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.294685 qwak_core-0.0.89/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-05-31 07:00:44.302685 qwak_core-0.0.89/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-05-31 07:00:37.798645 qwak_core-0.0.89/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.302685 qwak_core-0.0.89/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-05-31 07:00:44.298685 qwak_core-0.0.89/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-05-31 07:00:37.394642 qwak_core-0.0.89/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-05-31 07:00:44.298685 qwak_core-0.0.89/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0    10138 2023-05-31 07:00:44.298685 qwak_core-0.0.89/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    14337 2023-05-31 07:00:37.602643 qwak_core-0.0.89/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.302685 qwak_core-0.0.89/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-05-31 07:00:44.274685 qwak_core-0.0.89/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-05-31 07:00:35.602631 qwak_core-0.0.89/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-05-31 07:00:44.274685 qwak_core-0.0.89/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-05-31 07:00:44.098683 qwak_core-0.0.89/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-05-31 07:00:25.298568 qwak_core-0.0.89/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-05-31 07:00:44.098683 qwak_core-0.0.89/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-05-31 07:00:44.094684 qwak_core-0.0.89/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-05-31 07:00:25.090566 qwak_core-0.0.89/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.098683 qwak_core-0.0.89/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-05-31 07:00:44.102684 qwak_core-0.0.89/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-05-31 07:00:25.506569 qwak_core-0.0.89/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-05-31 07:00:44.102684 qwak_core-0.0.89/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-05-31 07:00:44.270685 qwak_core-0.0.89/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-05-31 07:00:35.178629 qwak_core-0.0.89/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-05-31 07:00:44.274685 qwak_core-0.0.89/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-05-31 07:00:44.290685 qwak_core-0.0.89/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-05-31 07:00:36.998640 qwak_core-0.0.89/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-05-31 07:00:44.294685 qwak_core-0.0.89/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-05-31 07:00:44.094684 qwak_core-0.0.89/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-05-31 07:00:22.574551 qwak_core-0.0.89/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.094684 qwak_core-0.0.89/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-05-31 07:00:44.090684 qwak_core-0.0.89/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-05-31 07:00:22.326549 qwak_core-0.0.89/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-05-31 07:00:44.094684 qwak_core-0.0.89/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-05-31 07:00:44.086683 qwak_core-0.0.89/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-05-31 07:00:21.626545 qwak_core-0.0.89/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.086683 qwak_core-0.0.89/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-31 07:00:44.086683 qwak_core-0.0.89/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-05-31 07:00:21.838546 qwak_core-0.0.89/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.086683 qwak_core-0.0.89/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-05-31 07:00:44.090684 qwak_core-0.0.89/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-05-31 07:00:22.078548 qwak_core-0.0.89/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-05-31 07:00:44.090684 qwak_core-0.0.89/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-05-31 07:00:44.322685 qwak_core-0.0.89/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-05-31 07:00:39.674656 qwak_core-0.0.89/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-05-31 07:00:44.326685 qwak_core-0.0.89/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-05-31 07:00:44.322685 qwak_core-0.0.89/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-05-31 07:00:39.466655 qwak_core-0.0.89/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.322685 qwak_core-0.0.89/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    10851 2023-05-31 07:00:44.110684 qwak_core-0.0.89/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    13974 2023-05-31 07:00:24.250561 qwak_core-0.0.89/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.110684 qwak_core-0.0.89/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     3044 2023-05-31 07:00:44.110684 qwak_core-0.0.89/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2641 2023-05-31 07:00:24.450562 qwak_core-0.0.89/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-31 07:00:44.114684 qwak_core-0.0.89/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-05-31 07:00:46.826700 qwak_core-0.0.89/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-31 07:00:46.826700 qwak_core-0.0.89/qwak/__init__.py
--rw-r--r--   0        0        0     1501 2023-05-31 06:58:55.462013 qwak_core-0.0.89/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-31 06:58:55.462013 qwak_core-0.0.89/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    12899 2023-05-31 06:58:55.462013 qwak_core-0.0.89/qwak/automations/automations.py
--rw-r--r--   0        0        0     9638 2023-05-31 06:58:55.462013 qwak_core-0.0.89/qwak/automations/batch_execution_action.py
--rw-r--r--   0        0        0    19120 2023-05-31 06:58:55.462013 qwak_core-0.0.89/qwak/automations/build_and_deploy_action.py
--rw-r--r--   0        0        0     1697 2023-05-31 06:58:55.462013 qwak_core-0.0.89/qwak/automations/common.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.462013 qwak_core-0.0.89/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-05-31 06:58:55.462013 qwak_core-0.0.89/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.462013 qwak_core-0.0.89/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-31 06:58:55.462013 qwak_core-0.0.89/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.462013 qwak_core-0.0.89/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-31 06:58:55.462013 qwak_core-0.0.89/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.462013 qwak_core-0.0.89/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-31 06:58:55.462013 qwak_core-0.0.89/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.462013 qwak_core-0.0.89/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-31 06:58:55.462013 qwak_core-0.0.89/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.462013 qwak_core-0.0.89/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-05-31 06:58:55.462013 qwak_core-0.0.89/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-05-31 06:58:55.462013 qwak_core-0.0.89/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-31 06:58:55.462013 qwak_core-0.0.89/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-05-31 06:58:55.462013 qwak_core-0.0.89/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-05-31 06:58:55.462013 qwak_core-0.0.89/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-05-31 06:58:55.462013 qwak_core-0.0.89/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    18388 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14847 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/instance_template/__init__.py
--rw-r--r--   0        0        0     2495 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/instance_template/client.py
--rw-r--r--   0        0        0       41 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9261 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/inner/const.py
--rw-r--r--   0        0        0     1435 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6083 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-05-31 06:58:55.466013 qwak_core-0.0.89/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      873 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12316 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     3905 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/instance_template_management_service.py
--rw-r--r--   0        0        0     2696 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     4186 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13583 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-05-31 06:58:55.470013 qwak_core-0.0.89/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.89/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.89/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-05-31 08:24:37.641605 qwak_core-0.0.90/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 08:26:28.566255 qwak_core-0.0.90/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-05-31 08:26:28.590256 qwak_core-0.0.90/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-05-31 08:26:05.286124 qwak_core-0.0.90/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.594256 qwak_core-0.0.90/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-05-31 08:26:28.586255 qwak_core-0.0.90/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-05-31 08:26:04.898121 qwak_core-0.0.90/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.586255 qwak_core-0.0.90/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-05-31 08:26:28.590256 qwak_core-0.0.90/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-05-31 08:26:05.090123 qwak_core-0.0.90/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.590256 qwak_core-0.0.90/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-05-31 08:26:28.578256 qwak_core-0.0.90/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-05-31 08:26:04.286118 qwak_core-0.0.90/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-05-31 08:26:28.582255 qwak_core-0.0.90/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-31 08:26:28.582255 qwak_core-0.0.90/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-05-31 08:26:04.490119 qwak_core-0.0.90/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.582255 qwak_core-0.0.90/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4901 2023-05-31 08:26:28.586255 qwak_core-0.0.90/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5995 2023-05-31 08:26:04.702120 qwak_core-0.0.90/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.586255 qwak_core-0.0.90/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-05-31 08:26:28.566255 qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-05-31 08:26:04.086117 qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-05-31 08:26:28.566255 qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5707 2023-05-31 08:26:28.570255 qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8170 2023-05-31 08:26:05.478125 qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.570255 qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-05-31 08:26:28.574255 qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-05-31 08:26:05.866127 qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.574255 qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-05-31 08:26:28.574255 qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-05-31 08:26:06.066128 qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-05-31 08:26:28.578256 qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-05-31 08:26:28.570255 qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-05-31 08:26:05.670126 qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.570255 qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-05-31 08:26:28.578256 qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-05-31 08:26:06.262130 qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.578256 qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-05-31 08:26:28.622256 qwak_core-0.0.90/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-05-31 08:26:09.150147 qwak_core-0.0.90/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.626256 qwak_core-0.0.90/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-05-31 08:26:28.626256 qwak_core-0.0.90/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-05-31 08:26:09.346148 qwak_core-0.0.90/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-05-31 08:26:28.626256 qwak_core-0.0.90/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-05-31 08:26:28.710256 qwak_core-0.0.90/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-05-31 08:26:15.430183 qwak_core-0.0.90/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.714256 qwak_core-0.0.90/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-05-31 08:26:28.714256 qwak_core-0.0.90/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-05-31 08:26:15.634184 qwak_core-0.0.90/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-05-31 08:26:28.714256 qwak_core-0.0.90/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-05-31 08:26:28.718256 qwak_core-0.0.90/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-05-31 08:26:16.682191 qwak_core-0.0.90/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-05-31 08:26:28.718256 qwak_core-0.0.90/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-05-31 08:26:28.718256 qwak_core-0.0.90/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-05-31 08:26:16.486189 qwak_core-0.0.90/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.718256 qwak_core-0.0.90/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5777 2023-05-31 08:26:28.722256 qwak_core-0.0.90/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8264 2023-05-31 08:26:16.878192 qwak_core-0.0.90/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.722256 qwak_core-0.0.90/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-05-31 08:26:28.722256 qwak_core-0.0.90/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-05-31 08:26:17.078193 qwak_core-0.0.90/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-05-31 08:26:28.726256 qwak_core-0.0.90/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12352 2023-05-31 08:26:28.822257 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    18970 2023-05-31 08:26:26.094242 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.826257 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5775 2023-05-31 08:26:28.818257 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8308 2023-05-31 08:26:25.682239 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.818257 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-05-31 08:26:28.822257 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-05-31 08:26:25.886241 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.822257 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-05-31 08:26:28.814257 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-05-31 08:26:25.262237 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-05-31 08:26:28.814257 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-05-31 08:26:28.814257 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-05-31 08:26:25.474238 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.818257 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-05-31 08:26:28.830257 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-05-31 08:26:26.682245 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.830257 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-05-31 08:26:28.826257 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-05-31 08:26:26.486244 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.830257 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-05-31 08:26:28.826257 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-05-31 08:26:26.290243 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.826257 qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-05-31 08:26:28.810257 qwak_core-0.0.90/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-05-31 08:26:25.054236 qwak_core-0.0.90/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.810257 qwak_core-0.0.90/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-05-31 08:26:28.806257 qwak_core-0.0.90/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-05-31 08:26:24.590234 qwak_core-0.0.90/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.806257 qwak_core-0.0.90/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    42145 2023-05-31 08:26:28.810257 qwak_core-0.0.90/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    55993 2023-05-31 08:26:24.850235 qwak_core-0.0.90/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-05-31 08:26:28.810257 qwak_core-0.0.90/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    20255 2023-05-31 08:26:28.754257 qwak_core-0.0.90/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    17495 2023-05-31 08:26:19.130205 qwak_core-0.0.90/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    20359 2023-05-31 08:26:28.754257 qwak_core-0.0.90/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-05-31 08:26:28.750256 qwak_core-0.0.90/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-05-31 08:26:18.894203 qwak_core-0.0.90/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.750256 qwak_core-0.0.90/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11691 2023-05-31 08:26:28.742256 qwak_core-0.0.90/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18850 2023-05-31 08:26:18.498201 qwak_core-0.0.90/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.742256 qwak_core-0.0.90/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-05-31 08:26:28.742256 qwak_core-0.0.90/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-05-31 08:26:18.690202 qwak_core-0.0.90/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.742256 qwak_core-0.0.90/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-05-31 08:26:28.746256 qwak_core-0.0.90/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-05-31 08:26:19.334206 qwak_core-0.0.90/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-05-31 08:26:28.746256 qwak_core-0.0.90/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38290 2023-05-31 08:26:28.746256 qwak_core-0.0.90/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52702 2023-05-31 08:26:19.790208 qwak_core-0.0.90/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-05-31 08:26:28.750256 qwak_core-0.0.90/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-05-31 08:26:28.758257 qwak_core-0.0.90/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-05-31 08:26:20.206210 qwak_core-0.0.90/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.762256 qwak_core-0.0.90/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-05-31 08:26:28.762256 qwak_core-0.0.90/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-31 08:26:20.410211 qwak_core-0.0.90/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-31 08:26:28.762256 qwak_core-0.0.90/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-05-31 08:26:28.734256 qwak_core-0.0.90/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-05-31 08:26:17.910198 qwak_core-0.0.90/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.734256 qwak_core-0.0.90/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-05-31 08:26:28.734256 qwak_core-0.0.90/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-05-31 08:26:18.106199 qwak_core-0.0.90/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-05-31 08:26:28.738256 qwak_core-0.0.90/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-05-31 08:26:28.730256 qwak_core-0.0.90/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-05-31 08:26:17.494196 qwak_core-0.0.90/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.730256 qwak_core-0.0.90/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    43712 2023-05-31 08:26:28.726256 qwak_core-0.0.90/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    63341 2023-05-31 08:26:17.290194 qwak_core-0.0.90/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.726256 qwak_core-0.0.90/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-05-31 08:26:28.730256 qwak_core-0.0.90/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-05-31 08:26:17.710197 qwak_core-0.0.90/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-05-31 08:26:28.734256 qwak_core-0.0.90/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-05-31 08:26:28.610256 qwak_core-0.0.90/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-05-31 08:26:08.150141 qwak_core-0.0.90/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.614256 qwak_core-0.0.90/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-31 08:26:28.614256 qwak_core-0.0.90/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-05-31 08:26:08.358142 qwak_core-0.0.90/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.614256 qwak_core-0.0.90/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-05-31 08:26:28.618256 qwak_core-0.0.90/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-05-31 08:26:08.558143 qwak_core-0.0.90/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-05-31 08:26:28.618256 qwak_core-0.0.90/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-05-31 08:26:28.686256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-05-31 08:26:14.170176 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.690256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-05-31 08:26:28.686256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-05-31 08:26:13.966175 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-05-31 08:26:28.686256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11432 2023-05-31 08:26:28.654256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    12882 2023-05-31 08:26:11.810162 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.654256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5303 2023-05-31 08:26:28.654256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8604 2023-05-31 08:26:11.614161 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.654256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-05-31 08:26:28.646256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-05-31 08:26:10.990157 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.646256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    28920 2023-05-31 08:26:28.650256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20665 2023-05-31 08:26:11.418160 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    35307 2023-05-31 08:26:28.650256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-05-31 08:26:28.658256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-05-31 08:26:12.006163 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.658256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-05-31 08:26:28.658256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-05-31 08:26:12.202165 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-05-31 08:26:28.662256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    25269 2023-05-31 08:26:28.646256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    37664 2023-05-31 08:26:11.194158 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.650256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-05-31 08:26:28.662256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-31 08:26:12.394166 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.662256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0    10238 2023-05-31 08:26:28.666256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.py
+-rw-r--r--   0        0        0    16741 2023-05-31 08:26:12.782168 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.670256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0     3559 2023-05-31 08:26:28.670256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.py
+-rw-r--r--   0        0        0     1759 2023-05-31 08:26:12.978169 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.pyi
+-rw-r--r--   0        0        0     3608 2023-05-31 08:26:28.670256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11281 2023-05-31 08:26:28.666256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
+-rw-r--r--   0        0        0    15070 2023-05-31 08:26:12.590167 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.666256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-05-31 08:26:28.690256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-05-31 08:26:28.074252 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.690256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-05-31 08:26:28.694256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-05-31 08:26:28.270254 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-05-31 08:26:28.694256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-05-31 08:26:28.694256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-05-31 08:26:14.758180 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.698256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-31 08:26:28.698256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-05-31 08:26:14.982181 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-05-31 08:26:28.698256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-05-31 08:26:28.702256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-05-31 08:26:15.186182 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.702256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-05-31 08:26:28.706256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-05-31 08:26:16.054187 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.706256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-05-31 08:26:28.702256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-05-31 08:26:15.842186 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-05-31 08:26:28.706256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-05-31 08:26:28.710256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-05-31 08:26:16.258188 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.710256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-05-31 08:26:28.674256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-05-31 08:26:13.178170 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.674256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-05-31 08:26:28.674256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-05-31 08:26:13.386171 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.678256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-05-31 08:26:28.678256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-05-31 08:26:13.582172 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-05-31 08:26:28.678256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-05-31 08:26:28.682256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-05-31 08:26:13.774174 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.682256 qwak_core-0.0.90/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-05-31 08:26:28.834257 qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-05-31 08:26:26.882246 qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.834257 qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-05-31 08:26:28.834257 qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-05-31 08:26:27.082247 qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-31 08:26:28.838257 qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-05-31 08:26:28.838257 qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-05-31 08:26:27.282248 qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.838257 qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-05-31 08:26:28.838257 qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-05-31 08:26:27.482249 qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-31 08:26:28.842257 qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-05-31 08:26:28.842257 qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-05-31 08:26:27.686250 qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-05-31 08:26:28.842257 qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-05-31 08:26:28.846257 qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-05-31 08:26:27.878251 qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.846257 qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-05-31 08:26:28.766257 qwak_core-0.0.90/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-05-31 08:26:20.622213 qwak_core-0.0.90/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.766257 qwak_core-0.0.90/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-05-31 08:26:28.766257 qwak_core-0.0.90/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-31 08:26:20.846214 qwak_core-0.0.90/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-31 08:26:28.766257 qwak_core-0.0.90/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-05-31 08:26:28.630256 qwak_core-0.0.90/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-05-31 08:26:10.182153 qwak_core-0.0.90/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.630256 qwak_core-0.0.90/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-31 08:26:28.634256 qwak_core-0.0.90/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-05-31 08:26:10.386154 qwak_core-0.0.90/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.634256 qwak_core-0.0.90/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-05-31 08:26:28.638256 qwak_core-0.0.90/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-05-31 08:26:10.586155 qwak_core-0.0.90/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-05-31 08:26:28.638256 qwak_core-0.0.90/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-05-31 08:26:28.642256 qwak_core-0.0.90/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-05-31 08:26:10.782156 qwak_core-0.0.90/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.642256 qwak_core-0.0.90/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-05-31 08:26:28.738256 qwak_core-0.0.90/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-05-31 08:26:18.298200 qwak_core-0.0.90/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-05-31 08:26:28.738256 qwak_core-0.0.90/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     3757 2023-05-31 08:26:28.770257 qwak_core-0.0.90/_qwak_proto/qwak/instance_template/instance_template_pb2.py
+-rw-r--r--   0        0        0     4235 2023-05-31 08:26:21.066215 qwak_core-0.0.90/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.770257 qwak_core-0.0.90/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
+-rw-r--r--   0        0        0     4722 2023-05-31 08:26:28.770257 qwak_core-0.0.90/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
+-rw-r--r--   0        0        0     3245 2023-05-31 08:26:21.270216 qwak_core-0.0.90/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
+-rw-r--r--   0        0        0     5240 2023-05-31 08:26:28.774257 qwak_core-0.0.90/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-05-31 08:26:28.786257 qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-05-31 08:26:22.610223 qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.786257 qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-05-31 08:26:28.786257 qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-05-31 08:26:22.818224 qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.790257 qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-05-31 08:26:28.790257 qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-05-31 08:26:23.058225 qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.790257 qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-05-31 08:26:28.790257 qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-05-31 08:26:23.286227 qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.794257 qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-31 08:26:28.794257 qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-05-31 08:26:23.498228 qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.794257 qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-05-31 08:26:28.798257 qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-05-31 08:26:23.750229 qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-05-31 08:26:28.798257 qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-05-31 08:26:28.798257 qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-05-31 08:26:23.954230 qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.802257 qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-05-31 08:26:28.778257 qwak_core-0.0.90/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-05-31 08:26:21.690218 qwak_core-0.0.90/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.778257 qwak_core-0.0.90/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-05-31 08:26:28.782257 qwak_core-0.0.90/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-05-31 08:26:22.386222 qwak_core-0.0.90/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.782257 qwak_core-0.0.90/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-05-31 08:26:28.778257 qwak_core-0.0.90/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-05-31 08:26:21.906219 qwak_core-0.0.90/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-05-31 08:26:28.778257 qwak_core-0.0.90/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10138 2023-05-31 08:26:28.782257 qwak_core-0.0.90/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    14337 2023-05-31 08:26:22.130221 qwak_core-0.0.90/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.782257 qwak_core-0.0.90/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-05-31 08:26:28.758257 qwak_core-0.0.90/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-05-31 08:26:20.006209 qwak_core-0.0.90/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-05-31 08:26:28.758257 qwak_core-0.0.90/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-05-31 08:26:28.606256 qwak_core-0.0.90/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-05-31 08:26:09.738150 qwak_core-0.0.90/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-05-31 08:26:28.610256 qwak_core-0.0.90/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-05-31 08:26:28.606256 qwak_core-0.0.90/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-05-31 08:26:09.538149 qwak_core-0.0.90/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.606256 qwak_core-0.0.90/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-05-31 08:26:28.610256 qwak_core-0.0.90/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-05-31 08:26:09.950151 qwak_core-0.0.90/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-05-31 08:26:28.610256 qwak_core-0.0.90/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-05-31 08:26:28.754257 qwak_core-0.0.90/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-05-31 08:26:19.562207 qwak_core-0.0.90/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-05-31 08:26:28.758257 qwak_core-0.0.90/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-05-31 08:26:28.774257 qwak_core-0.0.90/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-05-31 08:26:21.478217 qwak_core-0.0.90/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-05-31 08:26:28.774257 qwak_core-0.0.90/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-05-31 08:26:28.602256 qwak_core-0.0.90/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-05-31 08:26:07.334136 qwak_core-0.0.90/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.602256 qwak_core-0.0.90/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-05-31 08:26:28.602256 qwak_core-0.0.90/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-05-31 08:26:07.134135 qwak_core-0.0.90/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-05-31 08:26:28.602256 qwak_core-0.0.90/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-05-31 08:26:28.594256 qwak_core-0.0.90/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-05-31 08:26:06.482131 qwak_core-0.0.90/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.594256 qwak_core-0.0.90/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-31 08:26:28.594256 qwak_core-0.0.90/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-05-31 08:26:06.694132 qwak_core-0.0.90/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.598255 qwak_core-0.0.90/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-05-31 08:26:28.598255 qwak_core-0.0.90/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-05-31 08:26:06.910133 qwak_core-0.0.90/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-05-31 08:26:28.598255 qwak_core-0.0.90/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-05-31 08:26:28.802257 qwak_core-0.0.90/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-05-31 08:26:24.390233 qwak_core-0.0.90/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-05-31 08:26:28.806257 qwak_core-0.0.90/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-05-31 08:26:28.802257 qwak_core-0.0.90/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-05-31 08:26:24.190232 qwak_core-0.0.90/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.802257 qwak_core-0.0.90/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    10851 2023-05-31 08:26:28.618256 qwak_core-0.0.90/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    13974 2023-05-31 08:26:08.754144 qwak_core-0.0.90/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.618256 qwak_core-0.0.90/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     3044 2023-05-31 08:26:28.622256 qwak_core-0.0.90/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2641 2023-05-31 08:26:08.954145 qwak_core-0.0.90/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-31 08:26:28.622256 qwak_core-0.0.90/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-05-31 08:26:32.882281 qwak_core-0.0.90/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-31 08:26:32.882281 qwak_core-0.0.90/qwak/__init__.py
+-rw-r--r--   0        0        0     1501 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    12899 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/automations/automations.py
+-rw-r--r--   0        0        0     9638 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/automations/batch_execution_action.py
+-rw-r--r--   0        0        0    19120 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/automations/build_and_deploy_action.py
+-rw-r--r--   0        0        0     1697 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/automations/common.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    18388 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14847 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/instance_template/__init__.py
+-rw-r--r--   0        0        0     2495 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/instance_template/client.py
+-rw-r--r--   0        0        0       41 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-05-31 08:24:37.645604 qwak_core-0.0.90/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9261 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/inner/const.py
+-rw-r--r--   0        0        0     1435 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6083 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      873 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12316 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-05-31 08:24:37.649604 qwak_core-0.0.90/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-05-31 08:24:37.653605 qwak_core-0.0.90/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-05-31 08:24:37.653605 qwak_core-0.0.90/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-05-31 08:24:37.653605 qwak_core-0.0.90/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-05-31 08:24:37.653605 qwak_core-0.0.90/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     3905 2023-05-31 08:24:37.653605 qwak_core-0.0.90/qwak_services_mock/mocks/instance_template_management_service.py
+-rw-r--r--   0        0        0     2696 2023-05-31 08:24:37.653605 qwak_core-0.0.90/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-05-31 08:24:37.653605 qwak_core-0.0.90/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-05-31 08:24:37.653605 qwak_core-0.0.90/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-05-31 08:24:37.653605 qwak_core-0.0.90/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-05-31 08:24:37.653605 qwak_core-0.0.90/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     4186 2023-05-31 08:24:37.653605 qwak_core-0.0.90/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-05-31 08:24:37.653605 qwak_core-0.0.90/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-05-31 08:24:37.653605 qwak_core-0.0.90/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-05-31 08:24:37.653605 qwak_core-0.0.90/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.653605 qwak_core-0.0.90/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-31 08:24:37.653605 qwak_core-0.0.90/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13583 2023-05-31 08:24:37.653605 qwak_core-0.0.90/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:24:37.653605 qwak_core-0.0.90/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-31 08:24:37.653605 qwak_core-0.0.90/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4984 1970-01-01 00:00:00.000000 qwak_core-0.0.90/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.90/PKG-INFO
```

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/instance_template/instance_template_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/instance_template/instance_template_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.90/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.90/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.90/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/pyproject.toml` & `qwak_core-0.0.90/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.89"
+version = "0.0.90"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.89/qwak/automations/__init__.py` & `qwak_core-0.0.90/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/automations/automation_executions.py` & `qwak_core-0.0.90/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/automations/automations.py` & `qwak_core-0.0.90/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/automations/batch_execution_action.py` & `qwak_core-0.0.90/qwak/automations/batch_execution_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/automations/build_and_deploy_action.py` & `qwak_core-0.0.90/qwak/automations/build_and_deploy_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/automations/common.py` & `qwak_core-0.0.90/qwak/automations/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.90/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.90/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.90/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.90/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.90/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/alert_management/client.py` & `qwak_core-0.0.90/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/analytics/client.py` & `qwak_core-0.0.90/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/audience/client.py` & `qwak_core-0.0.90/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/automation_management/client.py` & `qwak_core-0.0.90/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.90/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.90/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.90/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.90/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/build_management/client.py` & `qwak_core-0.0.90/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.90/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.90/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/deployment/client.py` & `qwak_core-0.0.90/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.90/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.90/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.90/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.90/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/instance_template/client.py` & `qwak_core-0.0.90/qwak/clients/instance_template/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.90/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/logging_client/client.py` & `qwak_core-0.0.90/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/model_management/client.py` & `qwak_core-0.0.90/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/project/client.py` & `qwak_core-0.0.90/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/secret_service/client.py` & `qwak_core-0.0.90/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.90/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.90/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.90/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.90/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.90/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.90/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.90/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.90/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.90/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.90/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.90/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.90/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.90/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.90/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.90/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.90/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/offline/client.py` & `qwak_core-0.0.90/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/feature_store/online/client.py` & `qwak_core-0.0.90/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/inner/const.py` & `qwak_core-0.0.90/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.90/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.90/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.90/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.90/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/inner/singleton_meta.py` & `qwak_core-0.0.90/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/inner/tool/auth.py` & `qwak_core-0.0.90/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.90/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.90/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.90/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.90/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/adapters/__init__.py` & `qwak_core-0.0.90/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.90/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.90/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.90/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.90/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.90/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/base.py` & `qwak_core-0.0.90/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/decorators/api.py` & `qwak_core-0.0.90/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.90/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/experiment_tracking.py` & `qwak_core-0.0.90/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/schema.py` & `qwak_core-0.0.90/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/schema_entities.py` & `qwak_core-0.0.90/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.90/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.90/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.90/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.90/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.90/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.90/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.90/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.90/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.90/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.90/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.90/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.90/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.90/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.90/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.90/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.90/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.90/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.90/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.90/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/qwak_client/client.py` & `qwak_core-0.0.90/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.90/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/qwak_client/models/model.py` & `qwak_core-0.0.90/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.90/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.90/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/tools/logger/logger.py` & `qwak_core-0.0.90/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak/tools/logger/logging.yml` & `qwak_core-0.0.90/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/instance_template_management_service.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/instance_template_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.90/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/qwak_services_mock/services_mock.py` & `qwak_core-0.0.90/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.89/setup.py` & `qwak_core-0.0.90/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.89',
+    'version': '0.0.90',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.89/PKG-INFO` & `qwak_core-0.0.90/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.89
+Version: 0.0.90
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

