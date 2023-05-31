# Comparing `tmp/alibabacloud_dingtalk-2.0.17.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.17.tar", last modified: Fri May 26 10:34:14 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.18.tar", last modified: Wed May 31 06:47:25 2023, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.17.tar` & `alibabacloud_dingtalk-2.0.18.tar`

### file list

```diff
@@ -1,365 +1,365 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/
--rw-r--r--   0 root         (0) root         (0)    19752 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2309 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1021 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1106 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23314 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169621 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46194 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21260 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23341 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90648 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138912 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   165948 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   322772 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    62246 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   201848 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   569113 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4942 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3871 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   138814 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   331545 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42229 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35138 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   101075 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6044 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10446 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123179 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    85810 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110530 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124904 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   293352 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   387566 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42332 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6576 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10253 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30852 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223914 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   552073 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7385 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46898 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   515455 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152480 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56301 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48073 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    67303 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   211006 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   267473 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   150160 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   269103 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   195538 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   453174 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   705965 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   116546 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123749 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5096 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     6148 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   312544 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   433417 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   155788 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   302125 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5282 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     5179 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4431 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4668 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9742 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   138362 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18903 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5382 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4660 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92926 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137528 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   302532 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   378971 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13884 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18281 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    92472 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   606316 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   855474 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   155140 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108695 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91118 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   135110 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23076 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   138339 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   166104 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54521 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31076 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40802 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7507 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76720 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137701 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123420 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60347 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    69069 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   260568 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   413706 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    11593 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   174524 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81780 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    93746 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56986 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    83842 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46018 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   361006 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   503423 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26678 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    96217 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   353698 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53470 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    89290 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28559 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65344 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   148231 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16170 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21677 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17519 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18718 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    32237 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   110849 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4269 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3363 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20486 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66210 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   130783 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8325 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27686 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    29689 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   179772 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   377816 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3772 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   464194 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   687148 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5452 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4490 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2309 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12014 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      239 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2684 2023-05-26 10:34:14.000000 alibabacloud_dingtalk-2.0.17/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/
+-rw-r--r--   0 root         (0) root         (0)    19817 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1106 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23314 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169621 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46194 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21260 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23341 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90648 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138912 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   165948 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   322772 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    62246 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   201848 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   569113 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4942 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3871 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   138814 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   331545 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42229 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35138 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   101075 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10446 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123179 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90334 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   117347 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124904 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   297108 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   392984 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42332 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6576 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10253 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30852 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223914 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   552073 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7385 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46898 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   515455 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152480 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56301 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48073 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    67303 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   211006 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   267473 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   150160 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   269103 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   195538 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   453174 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   705965 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   116546 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123749 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5096 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     6148 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   312544 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   433417 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   155788 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   302125 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9368 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    12542 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4431 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4668 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9742 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   138362 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18903 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4660 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92926 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137528 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   302532 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   378971 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22430 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    31875 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    92472 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   606316 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   855474 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   155140 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108695 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   135110 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   144945 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   173192 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54521 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31076 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40802 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7507 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76720 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137701 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123420 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60347 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    69069 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260568 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   413706 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    11593 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   174524 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81780 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    93746 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56986 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    83842 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46018 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   361006 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   503423 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26678 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    96217 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   353698 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53470 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    89290 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28559 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65344 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   148231 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16170 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21677 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17519 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18718 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    32237 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   110849 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4269 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20486 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66210 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   130783 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8325 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27686 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    29689 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   179772 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   377816 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3772 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   464194 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   687148 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4490 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2309 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12014 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      239 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2684 2023-05-31 06:47:25.000000 alibabacloud_dingtalk-2.0.18/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.17/ChangeLog.md` & `alibabacloud_dingtalk-2.0.18/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-05-26 Version: 2.0.17
+- Update AddOfficialAccountFollower.
+
 2023-05-24 Version: 2.0.16
 - Update AddOfficialAccountFollower.
 
 2023-05-18 Version: 2.0.15
 - Update AddOfficialAccountFollower.
 
 2023-05-17 Version: 2.0.14
```

### Comparing `alibabacloud_dingtalk-2.0.17/LICENSE` & `alibabacloud_dingtalk-2.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/PKG-INFO` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_dingtalk
-Version: 2.0.17
+Name: alibabacloud-dingtalk
+Version: 2.0.18
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.17/README-CN.md` & `alibabacloud_dingtalk-2.0.18/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/README.md` & `alibabacloud_dingtalk-2.0.18/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1327,14 +1327,108 @@
         conference_id: str,
         request: dingtalkconference__1__0_models.QueryConferenceMembersRequest,
     ) -> dingtalkconference__1__0_models.QueryConferenceMembersResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkconference__1__0_models.QueryConferenceMembersHeaders()
         return await self.query_conference_members_with_options_async(conference_id, request, headers, runtime)
 
+    def query_schedule_conference_info_with_options(
+        self,
+        schedule_conference_id: str,
+        request: dingtalkconference__1__0_models.QueryScheduleConferenceInfoRequest,
+        headers: dingtalkconference__1__0_models.QueryScheduleConferenceInfoHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkconference__1__0_models.QueryScheduleConferenceInfoResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.max_results):
+            query['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['nextToken'] = request.next_token
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='QueryScheduleConferenceInfo',
+            version='conference_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/conference/videoConferences/scheduleConferences/{schedule_conference_id}',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkconference__1__0_models.QueryScheduleConferenceInfoResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def query_schedule_conference_info_with_options_async(
+        self,
+        schedule_conference_id: str,
+        request: dingtalkconference__1__0_models.QueryScheduleConferenceInfoRequest,
+        headers: dingtalkconference__1__0_models.QueryScheduleConferenceInfoHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkconference__1__0_models.QueryScheduleConferenceInfoResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.max_results):
+            query['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['nextToken'] = request.next_token
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='QueryScheduleConferenceInfo',
+            version='conference_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/conference/videoConferences/scheduleConferences/{schedule_conference_id}',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkconference__1__0_models.QueryScheduleConferenceInfoResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def query_schedule_conference_info(
+        self,
+        schedule_conference_id: str,
+        request: dingtalkconference__1__0_models.QueryScheduleConferenceInfoRequest,
+    ) -> dingtalkconference__1__0_models.QueryScheduleConferenceInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkconference__1__0_models.QueryScheduleConferenceInfoHeaders()
+        return self.query_schedule_conference_info_with_options(schedule_conference_id, request, headers, runtime)
+
+    async def query_schedule_conference_info_async(
+        self,
+        schedule_conference_id: str,
+        request: dingtalkconference__1__0_models.QueryScheduleConferenceInfoRequest,
+    ) -> dingtalkconference__1__0_models.QueryScheduleConferenceInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkconference__1__0_models.QueryScheduleConferenceInfoHeaders()
+        return await self.query_schedule_conference_info_with_options_async(schedule_conference_id, request, headers, runtime)
+
     def start_cloud_record_with_options(
         self,
         conference_id: str,
         request: dingtalkconference__1__0_models.StartCloudRecordRequest,
         headers: dingtalkconference__1__0_models.StartCloudRecordHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkconference__1__0_models.StartCloudRecordResponse:
```

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2743,14 +2743,228 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = QueryConferenceMembersResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class QueryScheduleConferenceInfoHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class QueryScheduleConferenceInfoRequest(TeaModel):
+    def __init__(
+        self,
+        max_results: int = None,
+        next_token: str = None,
+    ):
+        self.max_results = max_results
+        self.next_token = next_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        return self
+
+
+class QueryScheduleConferenceInfoResponseBodyConferenceList(TeaModel):
+    def __init__(
+        self,
+        conference_id: str = None,
+        end_time: int = None,
+        room_code: str = None,
+        start_time: int = None,
+        status: int = None,
+        title: str = None,
+    ):
+        self.conference_id = conference_id
+        self.end_time = end_time
+        self.room_code = room_code
+        self.start_time = start_time
+        self.status = status
+        self.title = title
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.conference_id is not None:
+            result['conferenceId'] = self.conference_id
+        if self.end_time is not None:
+            result['endTime'] = self.end_time
+        if self.room_code is not None:
+            result['roomCode'] = self.room_code
+        if self.start_time is not None:
+            result['startTime'] = self.start_time
+        if self.status is not None:
+            result['status'] = self.status
+        if self.title is not None:
+            result['title'] = self.title
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('conferenceId') is not None:
+            self.conference_id = m.get('conferenceId')
+        if m.get('endTime') is not None:
+            self.end_time = m.get('endTime')
+        if m.get('roomCode') is not None:
+            self.room_code = m.get('roomCode')
+        if m.get('startTime') is not None:
+            self.start_time = m.get('startTime')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('title') is not None:
+            self.title = m.get('title')
+        return self
+
+
+class QueryScheduleConferenceInfoResponseBody(TeaModel):
+    def __init__(
+        self,
+        conference_list: List[QueryScheduleConferenceInfoResponseBodyConferenceList] = None,
+        next_token: str = None,
+        total_count: int = None,
+    ):
+        self.conference_list = conference_list
+        self.next_token = next_token
+        self.total_count = total_count
+
+    def validate(self):
+        if self.conference_list:
+            for k in self.conference_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['conferenceList'] = []
+        if self.conference_list is not None:
+            for k in self.conference_list:
+                result['conferenceList'].append(k.to_map() if k else None)
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.total_count is not None:
+            result['totalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.conference_list = []
+        if m.get('conferenceList') is not None:
+            for k in m.get('conferenceList'):
+                temp_model = QueryScheduleConferenceInfoResponseBodyConferenceList()
+                self.conference_list.append(temp_model.from_map(k))
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('totalCount') is not None:
+            self.total_count = m.get('totalCount')
+        return self
+
+
+class QueryScheduleConferenceInfoResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: QueryScheduleConferenceInfoResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = QueryScheduleConferenceInfoResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class StartCloudRecordHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4279,14 +4279,100 @@
         self,
         user_id: str,
     ) -> dingtalkcontact__1__0_models.QueryUserManagementResourcesResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkcontact__1__0_models.QueryUserManagementResourcesHeaders()
         return await self.query_user_management_resources_with_options_async(user_id, headers, runtime)
 
+    def query_verify_result_with_options(
+        self,
+        request: dingtalkcontact__1__0_models.QueryVerifyResultRequest,
+        headers: dingtalkcontact__1__0_models.QueryVerifyResultHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkcontact__1__0_models.QueryVerifyResultResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.verify_id):
+            query['verifyId'] = request.verify_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='QueryVerifyResult',
+            version='contact_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/contact/verifyIdentitys/verifyResults',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkcontact__1__0_models.QueryVerifyResultResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def query_verify_result_with_options_async(
+        self,
+        request: dingtalkcontact__1__0_models.QueryVerifyResultRequest,
+        headers: dingtalkcontact__1__0_models.QueryVerifyResultHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkcontact__1__0_models.QueryVerifyResultResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.verify_id):
+            query['verifyId'] = request.verify_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='QueryVerifyResult',
+            version='contact_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/contact/verifyIdentitys/verifyResults',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkcontact__1__0_models.QueryVerifyResultResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def query_verify_result(
+        self,
+        request: dingtalkcontact__1__0_models.QueryVerifyResultRequest,
+    ) -> dingtalkcontact__1__0_models.QueryVerifyResultResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkcontact__1__0_models.QueryVerifyResultHeaders()
+        return self.query_verify_result_with_options(request, headers, runtime)
+
+    async def query_verify_result_async(
+        self,
+        request: dingtalkcontact__1__0_models.QueryVerifyResultRequest,
+    ) -> dingtalkcontact__1__0_models.QueryVerifyResultResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkcontact__1__0_models.QueryVerifyResultHeaders()
+        return await self.query_verify_result_with_options_async(request, headers, runtime)
+
     def search_department_with_options(
         self,
         request: dingtalkcontact__1__0_models.SearchDepartmentRequest,
         headers: dingtalkcontact__1__0_models.SearchDepartmentHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkcontact__1__0_models.SearchDepartmentResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8787,14 +8787,187 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = QueryUserManagementResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class QueryVerifyResultHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class QueryVerifyResultRequest(TeaModel):
+    def __init__(
+        self,
+        verify_id: str = None,
+    ):
+        self.verify_id = verify_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.verify_id is not None:
+            result['verifyId'] = self.verify_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('verifyId') is not None:
+            self.verify_id = m.get('verifyId')
+        return self
+
+
+class QueryVerifyResultResponseBody(TeaModel):
+    def __init__(
+        self,
+        corp_id: str = None,
+        factor_code: str = None,
+        factor_desc: str = None,
+        result_code: str = None,
+        result_desc: str = None,
+        state: str = None,
+        user_id: str = None,
+        verify_timestamp: int = None,
+    ):
+        self.corp_id = corp_id
+        self.factor_code = factor_code
+        self.factor_desc = factor_desc
+        self.result_code = result_code
+        self.result_desc = result_desc
+        self.state = state
+        self.user_id = user_id
+        self.verify_timestamp = verify_timestamp
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.corp_id is not None:
+            result['corpId'] = self.corp_id
+        if self.factor_code is not None:
+            result['factorCode'] = self.factor_code
+        if self.factor_desc is not None:
+            result['factorDesc'] = self.factor_desc
+        if self.result_code is not None:
+            result['resultCode'] = self.result_code
+        if self.result_desc is not None:
+            result['resultDesc'] = self.result_desc
+        if self.state is not None:
+            result['state'] = self.state
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        if self.verify_timestamp is not None:
+            result['verifyTimestamp'] = self.verify_timestamp
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('corpId') is not None:
+            self.corp_id = m.get('corpId')
+        if m.get('factorCode') is not None:
+            self.factor_code = m.get('factorCode')
+        if m.get('factorDesc') is not None:
+            self.factor_desc = m.get('factorDesc')
+        if m.get('resultCode') is not None:
+            self.result_code = m.get('resultCode')
+        if m.get('resultDesc') is not None:
+            self.result_desc = m.get('resultDesc')
+        if m.get('state') is not None:
+            self.state = m.get('state')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        if m.get('verifyTimestamp') is not None:
+            self.verify_timestamp = m.get('verifyTimestamp')
+        return self
+
+
+class QueryVerifyResultResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: QueryVerifyResultResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = QueryVerifyResultResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class SearchDepartmentHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from Tea.core import TeaCore
 
 from alibabacloud_gateway_spi.client import Client as SPIClient
 from alibabacloud_tea_openapi.client import Client as OpenApiClient
 from alibabacloud_tea_openapi import models as open_api_models
 from alibabacloud_gateway_dingtalk.client import Client as GatewayClientClient
 from alibabacloud_tea_util.client import Client as UtilClient
-from alibabacloud_dingtalk.flashmeeting_1_0 import models as dingtalkflashmeeting__1__0_models
+from alibabacloud_dingtalk.wms_1_0 import models as dingtalkwms__1__0_models
 from alibabacloud_tea_util import models as util_models
 from alibabacloud_openapi_util.client import Client as OpenApiUtilClient
 
 
 class Client(OpenApiClient):
     """
     *\
@@ -25,100 +25,104 @@
         super().__init__(config)
         self._client = GatewayClientClient()
         self._spi = self._client
         self._endpoint_rule = ''
         if UtilClient.empty(self._endpoint):
             self._endpoint = 'api.dingtalk.com'
 
-    def create_flash_meeting_with_options(
+    def query_goods_list_with_options(
         self,
-        request: dingtalkflashmeeting__1__0_models.CreateFlashMeetingRequest,
-        headers: dingtalkflashmeeting__1__0_models.CreateFlashMeetingHeaders,
+        request: dingtalkwms__1__0_models.QueryGoodsListRequest,
+        headers: dingtalkwms__1__0_models.QueryGoodsListHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalkflashmeeting__1__0_models.CreateFlashMeetingResponse:
+    ) -> dingtalkwms__1__0_models.QueryGoodsListResponse:
         UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.creator):
-            body['creator'] = request.creator
-        if not UtilClient.is_unset(request.event_id):
-            body['eventId'] = request.event_id
-        if not UtilClient.is_unset(request.title):
-            body['title'] = request.title
+        query = {}
+        if not UtilClient.is_unset(request.end_time_in_mills):
+            query['endTimeInMills'] = request.end_time_in_mills
+        if not UtilClient.is_unset(request.max_results):
+            query['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.start_time_in_mills):
+            query['startTimeInMills'] = request.start_time_in_mills
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
-            body=OpenApiUtilClient.parse_to_map(body)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='CreateFlashMeeting',
-            version='flashmeeting_1.0',
+            action='QueryGoodsList',
+            version='wms_1.0',
             protocol='HTTP',
-            pathname=f'/v1.0/flashmeeting/meetings',
-            method='POST',
+            pathname=f'/v1.0/wms/goods',
+            method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalkflashmeeting__1__0_models.CreateFlashMeetingResponse(),
+            dingtalkwms__1__0_models.QueryGoodsListResponse(),
             self.execute(params, req, runtime)
         )
 
-    async def create_flash_meeting_with_options_async(
+    async def query_goods_list_with_options_async(
         self,
-        request: dingtalkflashmeeting__1__0_models.CreateFlashMeetingRequest,
-        headers: dingtalkflashmeeting__1__0_models.CreateFlashMeetingHeaders,
+        request: dingtalkwms__1__0_models.QueryGoodsListRequest,
+        headers: dingtalkwms__1__0_models.QueryGoodsListHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalkflashmeeting__1__0_models.CreateFlashMeetingResponse:
+    ) -> dingtalkwms__1__0_models.QueryGoodsListResponse:
         UtilClient.validate_model(request)
-        body = {}
-        if not UtilClient.is_unset(request.creator):
-            body['creator'] = request.creator
-        if not UtilClient.is_unset(request.event_id):
-            body['eventId'] = request.event_id
-        if not UtilClient.is_unset(request.title):
-            body['title'] = request.title
+        query = {}
+        if not UtilClient.is_unset(request.end_time_in_mills):
+            query['endTimeInMills'] = request.end_time_in_mills
+        if not UtilClient.is_unset(request.max_results):
+            query['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.start_time_in_mills):
+            query['startTimeInMills'] = request.start_time_in_mills
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
-            body=OpenApiUtilClient.parse_to_map(body)
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
-            action='CreateFlashMeeting',
-            version='flashmeeting_1.0',
+            action='QueryGoodsList',
+            version='wms_1.0',
             protocol='HTTP',
-            pathname=f'/v1.0/flashmeeting/meetings',
-            method='POST',
+            pathname=f'/v1.0/wms/goods',
+            method='GET',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalkflashmeeting__1__0_models.CreateFlashMeetingResponse(),
+            dingtalkwms__1__0_models.QueryGoodsListResponse(),
             await self.execute_async(params, req, runtime)
         )
 
-    def create_flash_meeting(
+    def query_goods_list(
         self,
-        request: dingtalkflashmeeting__1__0_models.CreateFlashMeetingRequest,
-    ) -> dingtalkflashmeeting__1__0_models.CreateFlashMeetingResponse:
+        request: dingtalkwms__1__0_models.QueryGoodsListRequest,
+    ) -> dingtalkwms__1__0_models.QueryGoodsListResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalkflashmeeting__1__0_models.CreateFlashMeetingHeaders()
-        return self.create_flash_meeting_with_options(request, headers, runtime)
+        headers = dingtalkwms__1__0_models.QueryGoodsListHeaders()
+        return self.query_goods_list_with_options(request, headers, runtime)
 
-    async def create_flash_meeting_async(
+    async def query_goods_list_async(
         self,
-        request: dingtalkflashmeeting__1__0_models.CreateFlashMeetingRequest,
-    ) -> dingtalkflashmeeting__1__0_models.CreateFlashMeetingResponse:
+        request: dingtalkwms__1__0_models.QueryGoodsListRequest,
+    ) -> dingtalkwms__1__0_models.QueryGoodsListResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalkflashmeeting__1__0_models.CreateFlashMeetingHeaders()
-        return await self.create_flash_meeting_with_options_async(request, headers, runtime)
+        headers = dingtalkwms__1__0_models.QueryGoodsListHeaders()
+        return await self.query_goods_list_with_options_async(request, headers, runtime)
```

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import Dict
 
 
-class CreateFlashMeetingHeaders(TeaModel):
+class RunCallUserHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -33,110 +33,92 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class CreateFlashMeetingRequest(TeaModel):
+class RunCallUserRequest(TeaModel):
     def __init__(
         self,
-        creator: str = None,
-        event_id: str = None,
-        title: str = None,
+        authorize_corp_id: str = None,
+        authorize_user_id: str = None,
+        order_id: str = None,
+        user_id: str = None,
     ):
-        self.creator = creator
-        self.event_id = event_id
-        self.title = title
+        self.authorize_corp_id = authorize_corp_id
+        self.authorize_user_id = authorize_user_id
+        self.order_id = order_id
+        self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.creator is not None:
-            result['creator'] = self.creator
-        if self.event_id is not None:
-            result['eventId'] = self.event_id
-        if self.title is not None:
-            result['title'] = self.title
+        if self.authorize_corp_id is not None:
+            result['authorizeCorpId'] = self.authorize_corp_id
+        if self.authorize_user_id is not None:
+            result['authorizeUserId'] = self.authorize_user_id
+        if self.order_id is not None:
+            result['orderId'] = self.order_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('creator') is not None:
-            self.creator = m.get('creator')
-        if m.get('eventId') is not None:
-            self.event_id = m.get('eventId')
-        if m.get('title') is not None:
-            self.title = m.get('title')
+        if m.get('authorizeCorpId') is not None:
+            self.authorize_corp_id = m.get('authorizeCorpId')
+        if m.get('authorizeUserId') is not None:
+            self.authorize_user_id = m.get('authorizeUserId')
+        if m.get('orderId') is not None:
+            self.order_id = m.get('orderId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
         return self
 
 
-class CreateFlashMeetingResponseBody(TeaModel):
+class RunCallUserResponseBody(TeaModel):
     def __init__(
         self,
-        end_time: int = None,
-        flash_meeting_key: str = None,
-        start_time: int = None,
-        title: str = None,
-        url: str = None,
+        success: str = None,
     ):
-        self.end_time = end_time
-        self.flash_meeting_key = flash_meeting_key
-        self.start_time = start_time
-        self.title = title
-        self.url = url
+        self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.end_time is not None:
-            result['endTime'] = self.end_time
-        if self.flash_meeting_key is not None:
-            result['flashMeetingKey'] = self.flash_meeting_key
-        if self.start_time is not None:
-            result['startTime'] = self.start_time
-        if self.title is not None:
-            result['title'] = self.title
-        if self.url is not None:
-            result['url'] = self.url
+        if self.success is not None:
+            result['success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('endTime') is not None:
-            self.end_time = m.get('endTime')
-        if m.get('flashMeetingKey') is not None:
-            self.flash_meeting_key = m.get('flashMeetingKey')
-        if m.get('startTime') is not None:
-            self.start_time = m.get('startTime')
-        if m.get('title') is not None:
-            self.title = m.get('title')
-        if m.get('url') is not None:
-            self.url = m.get('url')
+        if m.get('success') is not None:
+            self.success = m.get('success')
         return self
 
 
-class CreateFlashMeetingResponse(TeaModel):
+class RunCallUserResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: CreateFlashMeetingResponseBody = None,
+        body: RunCallUserResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -162,12 +144,12 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = CreateFlashMeetingResponseBody()
+            temp_model = RunCallUserResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from Tea.core import TeaCore
 
 from alibabacloud_gateway_spi.client import Client as SPIClient
 from alibabacloud_tea_openapi.client import Client as OpenApiClient
 from alibabacloud_tea_openapi import models as open_api_models
 from alibabacloud_gateway_dingtalk.client import Client as GatewayClientClient
 from alibabacloud_tea_util.client import Client as UtilClient
-from alibabacloud_dingtalk.im_2_0 import models as dingtalkim__2__0_models
+from alibabacloud_dingtalk.trip_1_0 import models as dingtalktrip__1__0_models
 from alibabacloud_tea_util import models as util_models
 from alibabacloud_openapi_util.client import Client as OpenApiUtilClient
 
 
 class Client(OpenApiClient):
     """
     *\
@@ -25,274 +25,384 @@
         super().__init__(config)
         self._client = GatewayClientClient()
         self._spi = self._client
         self._endpoint_rule = ''
         if UtilClient.empty(self._endpoint):
             self._endpoint = 'api.dingtalk.com'
 
-    def close_topbox_with_options(
+    def sync_business_sign_info_with_options(
         self,
-        request: dingtalkim__2__0_models.CloseTopboxRequest,
-        headers: dingtalkim__2__0_models.CloseTopboxHeaders,
+        request: dingtalktrip__1__0_models.SyncBusinessSignInfoRequest,
+        headers: dingtalktrip__1__0_models.SyncBusinessSignInfoHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalkim__2__0_models.CloseTopboxResponse:
+    ) -> dingtalktrip__1__0_models.SyncBusinessSignInfoResponse:
         UtilClient.validate_model(request)
         body = {}
-        if not UtilClient.is_unset(request.conversation_type):
-            body['conversationType'] = request.conversation_type
-        if not UtilClient.is_unset(request.cool_app_code):
-            body['coolAppCode'] = request.cool_app_code
-        if not UtilClient.is_unset(request.group_template_id):
-            body['groupTemplateId'] = request.group_template_id
-        if not UtilClient.is_unset(request.open_conversation_id):
-            body['openConversationId'] = request.open_conversation_id
-        if not UtilClient.is_unset(request.out_track_id):
-            body['outTrackId'] = request.out_track_id
-        if not UtilClient.is_unset(request.robot_code):
-            body['robotCode'] = request.robot_code
-        if not UtilClient.is_unset(request.unoin_id):
-            body['unoinId'] = request.unoin_id
-        if not UtilClient.is_unset(request.user_id):
-            body['userId'] = request.user_id
+        if not UtilClient.is_unset(request.biz_type_list):
+            body['bizTypeList'] = request.biz_type_list
+        if not UtilClient.is_unset(request.gmt_org_pay):
+            body['gmtOrgPay'] = request.gmt_org_pay
+        if not UtilClient.is_unset(request.gmt_sign):
+            body['gmtSign'] = request.gmt_sign
+        if not UtilClient.is_unset(request.org_pay_status):
+            body['orgPayStatus'] = request.org_pay_status
+        if not UtilClient.is_unset(request.sign_status):
+            body['signStatus'] = request.sign_status
+        if not UtilClient.is_unset(request.target_corp_id):
+            body['targetCorpId'] = request.target_corp_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
-            action='CloseTopbox',
-            version='im_2.0',
+            action='SyncBusinessSignInfo',
+            version='trip_1.0',
             protocol='HTTP',
-            pathname=f'/v2.0/im/topBoxes/close',
+            pathname=f'/v1.0/trip/businessSignInfos/sync',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalkim__2__0_models.CloseTopboxResponse(),
+            dingtalktrip__1__0_models.SyncBusinessSignInfoResponse(),
             self.execute(params, req, runtime)
         )
 
-    async def close_topbox_with_options_async(
+    async def sync_business_sign_info_with_options_async(
         self,
-        request: dingtalkim__2__0_models.CloseTopboxRequest,
-        headers: dingtalkim__2__0_models.CloseTopboxHeaders,
+        request: dingtalktrip__1__0_models.SyncBusinessSignInfoRequest,
+        headers: dingtalktrip__1__0_models.SyncBusinessSignInfoHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalkim__2__0_models.CloseTopboxResponse:
+    ) -> dingtalktrip__1__0_models.SyncBusinessSignInfoResponse:
         UtilClient.validate_model(request)
         body = {}
-        if not UtilClient.is_unset(request.conversation_type):
-            body['conversationType'] = request.conversation_type
-        if not UtilClient.is_unset(request.cool_app_code):
-            body['coolAppCode'] = request.cool_app_code
-        if not UtilClient.is_unset(request.group_template_id):
-            body['groupTemplateId'] = request.group_template_id
-        if not UtilClient.is_unset(request.open_conversation_id):
-            body['openConversationId'] = request.open_conversation_id
-        if not UtilClient.is_unset(request.out_track_id):
-            body['outTrackId'] = request.out_track_id
-        if not UtilClient.is_unset(request.robot_code):
-            body['robotCode'] = request.robot_code
-        if not UtilClient.is_unset(request.unoin_id):
-            body['unoinId'] = request.unoin_id
-        if not UtilClient.is_unset(request.user_id):
-            body['userId'] = request.user_id
+        if not UtilClient.is_unset(request.biz_type_list):
+            body['bizTypeList'] = request.biz_type_list
+        if not UtilClient.is_unset(request.gmt_org_pay):
+            body['gmtOrgPay'] = request.gmt_org_pay
+        if not UtilClient.is_unset(request.gmt_sign):
+            body['gmtSign'] = request.gmt_sign
+        if not UtilClient.is_unset(request.org_pay_status):
+            body['orgPayStatus'] = request.org_pay_status
+        if not UtilClient.is_unset(request.sign_status):
+            body['signStatus'] = request.sign_status
+        if not UtilClient.is_unset(request.target_corp_id):
+            body['targetCorpId'] = request.target_corp_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
-            action='CloseTopbox',
-            version='im_2.0',
+            action='SyncBusinessSignInfo',
+            version='trip_1.0',
             protocol='HTTP',
-            pathname=f'/v2.0/im/topBoxes/close',
+            pathname=f'/v1.0/trip/businessSignInfos/sync',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalkim__2__0_models.CloseTopboxResponse(),
+            dingtalktrip__1__0_models.SyncBusinessSignInfoResponse(),
             await self.execute_async(params, req, runtime)
         )
 
-    def close_topbox(
+    def sync_business_sign_info(
         self,
-        request: dingtalkim__2__0_models.CloseTopboxRequest,
-    ) -> dingtalkim__2__0_models.CloseTopboxResponse:
+        request: dingtalktrip__1__0_models.SyncBusinessSignInfoRequest,
+    ) -> dingtalktrip__1__0_models.SyncBusinessSignInfoResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalkim__2__0_models.CloseTopboxHeaders()
-        return self.close_topbox_with_options(request, headers, runtime)
+        headers = dingtalktrip__1__0_models.SyncBusinessSignInfoHeaders()
+        return self.sync_business_sign_info_with_options(request, headers, runtime)
 
-    async def close_topbox_async(
+    async def sync_business_sign_info_async(
         self,
-        request: dingtalkim__2__0_models.CloseTopboxRequest,
-    ) -> dingtalkim__2__0_models.CloseTopboxResponse:
+        request: dingtalktrip__1__0_models.SyncBusinessSignInfoRequest,
+    ) -> dingtalktrip__1__0_models.SyncBusinessSignInfoResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalkim__2__0_models.CloseTopboxHeaders()
-        return await self.close_topbox_with_options_async(request, headers, runtime)
+        headers = dingtalktrip__1__0_models.SyncBusinessSignInfoHeaders()
+        return await self.sync_business_sign_info_with_options_async(request, headers, runtime)
 
-    def create_topbox_with_options(
+    def sync_secret_key_with_options(
         self,
-        request: dingtalkim__2__0_models.CreateTopboxRequest,
-        headers: dingtalkim__2__0_models.CreateTopboxHeaders,
+        request: dingtalktrip__1__0_models.SyncSecretKeyRequest,
+        headers: dingtalktrip__1__0_models.SyncSecretKeyHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalkim__2__0_models.CreateTopboxResponse:
+    ) -> dingtalktrip__1__0_models.SyncSecretKeyResponse:
         UtilClient.validate_model(request)
         body = {}
-        if not UtilClient.is_unset(request.callback_route_key):
-            body['callbackRouteKey'] = request.callback_route_key
-        if not UtilClient.is_unset(request.card_data):
-            body['cardData'] = request.card_data
-        if not UtilClient.is_unset(request.card_settings):
-            body['cardSettings'] = request.card_settings
-        if not UtilClient.is_unset(request.card_template_id):
-            body['cardTemplateId'] = request.card_template_id
-        if not UtilClient.is_unset(request.conversation_type):
-            body['conversationType'] = request.conversation_type
-        if not UtilClient.is_unset(request.cool_app_code):
-            body['coolAppCode'] = request.cool_app_code
-        if not UtilClient.is_unset(request.expired_time):
-            body['expiredTime'] = request.expired_time
-        if not UtilClient.is_unset(request.group_template_id):
-            body['groupTemplateId'] = request.group_template_id
-        if not UtilClient.is_unset(request.open_conversation_id):
-            body['openConversationId'] = request.open_conversation_id
-        if not UtilClient.is_unset(request.out_track_id):
-            body['outTrackId'] = request.out_track_id
-        if not UtilClient.is_unset(request.platforms):
-            body['platforms'] = request.platforms
-        if not UtilClient.is_unset(request.receiver_union_id_list):
-            body['receiverUnionIdList'] = request.receiver_union_id_list
-        if not UtilClient.is_unset(request.receiver_user_id_list):
-            body['receiverUserIdList'] = request.receiver_user_id_list
-        if not UtilClient.is_unset(request.robot_code):
-            body['robotCode'] = request.robot_code
-        if not UtilClient.is_unset(request.union_id_private_data_map):
-            body['unionIdPrivateDataMap'] = request.union_id_private_data_map
-        if not UtilClient.is_unset(request.unoin_id):
-            body['unoinId'] = request.unoin_id
-        if not UtilClient.is_unset(request.user_id):
-            body['userId'] = request.user_id
-        if not UtilClient.is_unset(request.user_id_private_data_map):
-            body['userIdPrivateDataMap'] = request.user_id_private_data_map
+        if not UtilClient.is_unset(request.action_type):
+            body['actionType'] = request.action_type
+        if not UtilClient.is_unset(request.secret_string):
+            body['secretString'] = request.secret_string
+        if not UtilClient.is_unset(request.target_corp_id):
+            body['targetCorpId'] = request.target_corp_id
+        if not UtilClient.is_unset(request.trip_app_key):
+            body['tripAppKey'] = request.trip_app_key
+        if not UtilClient.is_unset(request.trip_app_security):
+            body['tripAppSecurity'] = request.trip_app_security
+        if not UtilClient.is_unset(request.trip_corp_id):
+            body['tripCorpId'] = request.trip_corp_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
-            action='CreateTopbox',
-            version='im_2.0',
+            action='SyncSecretKey',
+            version='trip_1.0',
             protocol='HTTP',
-            pathname=f'/v2.0/im/topBoxes',
+            pathname=f'/v1.0/trip/secretKeys/sync',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalkim__2__0_models.CreateTopboxResponse(),
+            dingtalktrip__1__0_models.SyncSecretKeyResponse(),
             self.execute(params, req, runtime)
         )
 
-    async def create_topbox_with_options_async(
+    async def sync_secret_key_with_options_async(
         self,
-        request: dingtalkim__2__0_models.CreateTopboxRequest,
-        headers: dingtalkim__2__0_models.CreateTopboxHeaders,
+        request: dingtalktrip__1__0_models.SyncSecretKeyRequest,
+        headers: dingtalktrip__1__0_models.SyncSecretKeyHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalkim__2__0_models.CreateTopboxResponse:
+    ) -> dingtalktrip__1__0_models.SyncSecretKeyResponse:
         UtilClient.validate_model(request)
         body = {}
-        if not UtilClient.is_unset(request.callback_route_key):
-            body['callbackRouteKey'] = request.callback_route_key
-        if not UtilClient.is_unset(request.card_data):
-            body['cardData'] = request.card_data
-        if not UtilClient.is_unset(request.card_settings):
-            body['cardSettings'] = request.card_settings
-        if not UtilClient.is_unset(request.card_template_id):
-            body['cardTemplateId'] = request.card_template_id
-        if not UtilClient.is_unset(request.conversation_type):
-            body['conversationType'] = request.conversation_type
-        if not UtilClient.is_unset(request.cool_app_code):
-            body['coolAppCode'] = request.cool_app_code
-        if not UtilClient.is_unset(request.expired_time):
-            body['expiredTime'] = request.expired_time
-        if not UtilClient.is_unset(request.group_template_id):
-            body['groupTemplateId'] = request.group_template_id
-        if not UtilClient.is_unset(request.open_conversation_id):
-            body['openConversationId'] = request.open_conversation_id
-        if not UtilClient.is_unset(request.out_track_id):
-            body['outTrackId'] = request.out_track_id
-        if not UtilClient.is_unset(request.platforms):
-            body['platforms'] = request.platforms
-        if not UtilClient.is_unset(request.receiver_union_id_list):
-            body['receiverUnionIdList'] = request.receiver_union_id_list
-        if not UtilClient.is_unset(request.receiver_user_id_list):
-            body['receiverUserIdList'] = request.receiver_user_id_list
-        if not UtilClient.is_unset(request.robot_code):
-            body['robotCode'] = request.robot_code
-        if not UtilClient.is_unset(request.union_id_private_data_map):
-            body['unionIdPrivateDataMap'] = request.union_id_private_data_map
-        if not UtilClient.is_unset(request.unoin_id):
-            body['unoinId'] = request.unoin_id
-        if not UtilClient.is_unset(request.user_id):
-            body['userId'] = request.user_id
-        if not UtilClient.is_unset(request.user_id_private_data_map):
-            body['userIdPrivateDataMap'] = request.user_id_private_data_map
+        if not UtilClient.is_unset(request.action_type):
+            body['actionType'] = request.action_type
+        if not UtilClient.is_unset(request.secret_string):
+            body['secretString'] = request.secret_string
+        if not UtilClient.is_unset(request.target_corp_id):
+            body['targetCorpId'] = request.target_corp_id
+        if not UtilClient.is_unset(request.trip_app_key):
+            body['tripAppKey'] = request.trip_app_key
+        if not UtilClient.is_unset(request.trip_app_security):
+            body['tripAppSecurity'] = request.trip_app_security
+        if not UtilClient.is_unset(request.trip_corp_id):
+            body['tripCorpId'] = request.trip_corp_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
-            action='CreateTopbox',
-            version='im_2.0',
+            action='SyncSecretKey',
+            version='trip_1.0',
             protocol='HTTP',
-            pathname=f'/v2.0/im/topBoxes',
+            pathname=f'/v1.0/trip/secretKeys/sync',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalkim__2__0_models.CreateTopboxResponse(),
+            dingtalktrip__1__0_models.SyncSecretKeyResponse(),
             await self.execute_async(params, req, runtime)
         )
 
-    def create_topbox(
+    def sync_secret_key(
         self,
-        request: dingtalkim__2__0_models.CreateTopboxRequest,
-    ) -> dingtalkim__2__0_models.CreateTopboxResponse:
+        request: dingtalktrip__1__0_models.SyncSecretKeyRequest,
+    ) -> dingtalktrip__1__0_models.SyncSecretKeyResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalkim__2__0_models.CreateTopboxHeaders()
-        return self.create_topbox_with_options(request, headers, runtime)
+        headers = dingtalktrip__1__0_models.SyncSecretKeyHeaders()
+        return self.sync_secret_key_with_options(request, headers, runtime)
 
-    async def create_topbox_async(
+    async def sync_secret_key_async(
         self,
-        request: dingtalkim__2__0_models.CreateTopboxRequest,
-    ) -> dingtalkim__2__0_models.CreateTopboxResponse:
+        request: dingtalktrip__1__0_models.SyncSecretKeyRequest,
+    ) -> dingtalktrip__1__0_models.SyncSecretKeyResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalkim__2__0_models.CreateTopboxHeaders()
-        return await self.create_topbox_with_options_async(request, headers, runtime)
+        headers = dingtalktrip__1__0_models.SyncSecretKeyHeaders()
+        return await self.sync_secret_key_with_options_async(request, headers, runtime)
+
+    def sync_trip_order_with_options(
+        self,
+        request: dingtalktrip__1__0_models.SyncTripOrderRequest,
+        headers: dingtalktrip__1__0_models.SyncTripOrderHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalktrip__1__0_models.SyncTripOrderResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.channel_type):
+            body['channelType'] = request.channel_type
+        if not UtilClient.is_unset(request.currency):
+            body['currency'] = request.currency
+        if not UtilClient.is_unset(request.ding_user_id):
+            body['dingUserId'] = request.ding_user_id
+        if not UtilClient.is_unset(request.discount_amount):
+            body['discountAmount'] = request.discount_amount
+        if not UtilClient.is_unset(request.endorse_flag):
+            body['endorseFlag'] = request.endorse_flag
+        if not UtilClient.is_unset(request.event):
+            body['event'] = request.event
+        if not UtilClient.is_unset(request.gmt_order):
+            body['gmtOrder'] = request.gmt_order
+        if not UtilClient.is_unset(request.gmt_pay):
+            body['gmtPay'] = request.gmt_pay
+        if not UtilClient.is_unset(request.gmt_refund):
+            body['gmtRefund'] = request.gmt_refund
+        if not UtilClient.is_unset(request.invoice_apply_url):
+            body['invoiceApplyUrl'] = request.invoice_apply_url
+        if not UtilClient.is_unset(request.journey_biz_no):
+            body['journeyBizNo'] = request.journey_biz_no
+        if not UtilClient.is_unset(request.order_details):
+            body['orderDetails'] = request.order_details
+        if not UtilClient.is_unset(request.order_no):
+            body['orderNo'] = request.order_no
+        if not UtilClient.is_unset(request.order_url):
+            body['orderUrl'] = request.order_url
+        if not UtilClient.is_unset(request.real_amount):
+            body['realAmount'] = request.real_amount
+        if not UtilClient.is_unset(request.refund_amount):
+            body['refundAmount'] = request.refund_amount
+        if not UtilClient.is_unset(request.relative_order_no):
+            body['relativeOrderNo'] = request.relative_order_no
+        if not UtilClient.is_unset(request.source):
+            body['source'] = request.source
+        if not UtilClient.is_unset(request.target_corp_id):
+            body['targetCorpId'] = request.target_corp_id
+        if not UtilClient.is_unset(request.total_amount):
+            body['totalAmount'] = request.total_amount
+        if not UtilClient.is_unset(request.type):
+            body['type'] = request.type
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='SyncTripOrder',
+            version='trip_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/trip/tripOrders/sync',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalktrip__1__0_models.SyncTripOrderResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def sync_trip_order_with_options_async(
+        self,
+        request: dingtalktrip__1__0_models.SyncTripOrderRequest,
+        headers: dingtalktrip__1__0_models.SyncTripOrderHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalktrip__1__0_models.SyncTripOrderResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.channel_type):
+            body['channelType'] = request.channel_type
+        if not UtilClient.is_unset(request.currency):
+            body['currency'] = request.currency
+        if not UtilClient.is_unset(request.ding_user_id):
+            body['dingUserId'] = request.ding_user_id
+        if not UtilClient.is_unset(request.discount_amount):
+            body['discountAmount'] = request.discount_amount
+        if not UtilClient.is_unset(request.endorse_flag):
+            body['endorseFlag'] = request.endorse_flag
+        if not UtilClient.is_unset(request.event):
+            body['event'] = request.event
+        if not UtilClient.is_unset(request.gmt_order):
+            body['gmtOrder'] = request.gmt_order
+        if not UtilClient.is_unset(request.gmt_pay):
+            body['gmtPay'] = request.gmt_pay
+        if not UtilClient.is_unset(request.gmt_refund):
+            body['gmtRefund'] = request.gmt_refund
+        if not UtilClient.is_unset(request.invoice_apply_url):
+            body['invoiceApplyUrl'] = request.invoice_apply_url
+        if not UtilClient.is_unset(request.journey_biz_no):
+            body['journeyBizNo'] = request.journey_biz_no
+        if not UtilClient.is_unset(request.order_details):
+            body['orderDetails'] = request.order_details
+        if not UtilClient.is_unset(request.order_no):
+            body['orderNo'] = request.order_no
+        if not UtilClient.is_unset(request.order_url):
+            body['orderUrl'] = request.order_url
+        if not UtilClient.is_unset(request.real_amount):
+            body['realAmount'] = request.real_amount
+        if not UtilClient.is_unset(request.refund_amount):
+            body['refundAmount'] = request.refund_amount
+        if not UtilClient.is_unset(request.relative_order_no):
+            body['relativeOrderNo'] = request.relative_order_no
+        if not UtilClient.is_unset(request.source):
+            body['source'] = request.source
+        if not UtilClient.is_unset(request.target_corp_id):
+            body['targetCorpId'] = request.target_corp_id
+        if not UtilClient.is_unset(request.total_amount):
+            body['totalAmount'] = request.total_amount
+        if not UtilClient.is_unset(request.type):
+            body['type'] = request.type
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='SyncTripOrder',
+            version='trip_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/trip/tripOrders/sync',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalktrip__1__0_models.SyncTripOrderResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def sync_trip_order(
+        self,
+        request: dingtalktrip__1__0_models.SyncTripOrderRequest,
+    ) -> dingtalktrip__1__0_models.SyncTripOrderResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalktrip__1__0_models.SyncTripOrderHeaders()
+        return self.sync_trip_order_with_options(request, headers, runtime)
+
+    async def sync_trip_order_async(
+        self,
+        request: dingtalktrip__1__0_models.SyncTripOrderRequest,
+    ) -> dingtalktrip__1__0_models.SyncTripOrderResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalktrip__1__0_models.SyncTripOrderHeaders()
+        return await self.sync_trip_order_with_options_async(request, headers, runtime)
```

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,240 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import Dict, List
 
 
-class UnionIdPrivateDataMapValue(TeaModel):
+class QueryAppActiveUsersHeaders(TeaModel):
     def __init__(
         self,
-        card_param_map: Dict[str, str] = None,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class QueryAppActiveUsersRequest(TeaModel):
+    def __init__(
+        self,
+        max_results: int = None,
+        need_position_info: bool = None,
+        next_token: int = None,
     ):
-        self.card_param_map = card_param_map
+        self.max_results = max_results
+        self.need_position_info = need_position_info
+        self.next_token = next_token
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.card_param_map is not None:
-            result['cardParamMap'] = self.card_param_map
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.need_position_info is not None:
+            result['needPositionInfo'] = self.need_position_info
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('cardParamMap') is not None:
-            self.card_param_map = m.get('cardParamMap')
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('needPositionInfo') is not None:
+            self.need_position_info = m.get('needPositionInfo')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
         return self
 
 
-class UserIdPrivateDataMapValue(TeaModel):
+class QueryAppActiveUsersResponseBodyList(TeaModel):
     def __init__(
         self,
-        card_param_map: Dict[str, str] = None,
+        app_trace_id: str = None,
+        latitude: float = None,
+        longitude: float = None,
+        report_time: int = None,
+        start_time: int = None,
+        user_id: str = None,
     ):
-        self.card_param_map = card_param_map
+        self.app_trace_id = app_trace_id
+        self.latitude = latitude
+        self.longitude = longitude
+        self.report_time = report_time
+        self.start_time = start_time
+        self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.card_param_map is not None:
-            result['cardParamMap'] = self.card_param_map
+        if self.app_trace_id is not None:
+            result['appTraceId'] = self.app_trace_id
+        if self.latitude is not None:
+            result['latitude'] = self.latitude
+        if self.longitude is not None:
+            result['longitude'] = self.longitude
+        if self.report_time is not None:
+            result['reportTime'] = self.report_time
+        if self.start_time is not None:
+            result['startTime'] = self.start_time
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('appTraceId') is not None:
+            self.app_trace_id = m.get('appTraceId')
+        if m.get('latitude') is not None:
+            self.latitude = m.get('latitude')
+        if m.get('longitude') is not None:
+            self.longitude = m.get('longitude')
+        if m.get('reportTime') is not None:
+            self.report_time = m.get('reportTime')
+        if m.get('startTime') is not None:
+            self.start_time = m.get('startTime')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class QueryAppActiveUsersResponseBody(TeaModel):
+    def __init__(
+        self,
+        has_more: bool = None,
+        list: List[QueryAppActiveUsersResponseBodyList] = None,
+        next_token: int = None,
+        total_count: int = None,
+    ):
+        self.has_more = has_more
+        self.list = list
+        self.next_token = next_token
+        self.total_count = total_count
+
+    def validate(self):
+        if self.list:
+            for k in self.list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.has_more is not None:
+            result['hasMore'] = self.has_more
+        result['list'] = []
+        if self.list is not None:
+            for k in self.list:
+                result['list'].append(k.to_map() if k else None)
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.total_count is not None:
+            result['totalCount'] = self.total_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('cardParamMap') is not None:
-            self.card_param_map = m.get('cardParamMap')
+        if m.get('hasMore') is not None:
+            self.has_more = m.get('hasMore')
+        self.list = []
+        if m.get('list') is not None:
+            for k in m.get('list'):
+                temp_model = QueryAppActiveUsersResponseBodyList()
+                self.list.append(temp_model.from_map(k))
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('totalCount') is not None:
+            self.total_count = m.get('totalCount')
         return self
 
 
-class CloseTopboxHeaders(TeaModel):
+class QueryAppActiveUsersResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: QueryAppActiveUsersResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = QueryAppActiveUsersResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class QueryCollectingTraceTaskHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -87,116 +259,145 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class CloseTopboxRequest(TeaModel):
+class QueryCollectingTraceTaskRequest(TeaModel):
     def __init__(
         self,
-        conversation_type: int = None,
-        cool_app_code: str = None,
-        group_template_id: str = None,
-        open_conversation_id: str = None,
-        out_track_id: str = None,
-        robot_code: str = None,
-        unoin_id: str = None,
+        user_ids: List[str] = None,
+    ):
+        self.user_ids = user_ids
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.user_ids is not None:
+            result['userIds'] = self.user_ids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('userIds') is not None:
+            self.user_ids = m.get('userIds')
+        return self
+
+
+class QueryCollectingTraceTaskResponseBodyList(TeaModel):
+    def __init__(
+        self,
+        app_trace_id: str = None,
+        geo_collect_period: int = None,
+        geo_report_period: int = None,
+        geo_report_status: int = None,
+        report_end_time: int = None,
+        report_start_time: int = None,
         user_id: str = None,
     ):
-        self.conversation_type = conversation_type
-        self.cool_app_code = cool_app_code
-        self.group_template_id = group_template_id
-        self.open_conversation_id = open_conversation_id
-        self.out_track_id = out_track_id
-        self.robot_code = robot_code
-        self.unoin_id = unoin_id
+        self.app_trace_id = app_trace_id
+        self.geo_collect_period = geo_collect_period
+        self.geo_report_period = geo_report_period
+        self.geo_report_status = geo_report_status
+        self.report_end_time = report_end_time
+        self.report_start_time = report_start_time
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.conversation_type is not None:
-            result['conversationType'] = self.conversation_type
-        if self.cool_app_code is not None:
-            result['coolAppCode'] = self.cool_app_code
-        if self.group_template_id is not None:
-            result['groupTemplateId'] = self.group_template_id
-        if self.open_conversation_id is not None:
-            result['openConversationId'] = self.open_conversation_id
-        if self.out_track_id is not None:
-            result['outTrackId'] = self.out_track_id
-        if self.robot_code is not None:
-            result['robotCode'] = self.robot_code
-        if self.unoin_id is not None:
-            result['unoinId'] = self.unoin_id
+        if self.app_trace_id is not None:
+            result['appTraceId'] = self.app_trace_id
+        if self.geo_collect_period is not None:
+            result['geoCollectPeriod'] = self.geo_collect_period
+        if self.geo_report_period is not None:
+            result['geoReportPeriod'] = self.geo_report_period
+        if self.geo_report_status is not None:
+            result['geoReportStatus'] = self.geo_report_status
+        if self.report_end_time is not None:
+            result['reportEndTime'] = self.report_end_time
+        if self.report_start_time is not None:
+            result['reportStartTime'] = self.report_start_time
         if self.user_id is not None:
             result['userId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('conversationType') is not None:
-            self.conversation_type = m.get('conversationType')
-        if m.get('coolAppCode') is not None:
-            self.cool_app_code = m.get('coolAppCode')
-        if m.get('groupTemplateId') is not None:
-            self.group_template_id = m.get('groupTemplateId')
-        if m.get('openConversationId') is not None:
-            self.open_conversation_id = m.get('openConversationId')
-        if m.get('outTrackId') is not None:
-            self.out_track_id = m.get('outTrackId')
-        if m.get('robotCode') is not None:
-            self.robot_code = m.get('robotCode')
-        if m.get('unoinId') is not None:
-            self.unoin_id = m.get('unoinId')
+        if m.get('appTraceId') is not None:
+            self.app_trace_id = m.get('appTraceId')
+        if m.get('geoCollectPeriod') is not None:
+            self.geo_collect_period = m.get('geoCollectPeriod')
+        if m.get('geoReportPeriod') is not None:
+            self.geo_report_period = m.get('geoReportPeriod')
+        if m.get('geoReportStatus') is not None:
+            self.geo_report_status = m.get('geoReportStatus')
+        if m.get('reportEndTime') is not None:
+            self.report_end_time = m.get('reportEndTime')
+        if m.get('reportStartTime') is not None:
+            self.report_start_time = m.get('reportStartTime')
         if m.get('userId') is not None:
             self.user_id = m.get('userId')
         return self
 
 
-class CloseTopboxResponseBody(TeaModel):
+class QueryCollectingTraceTaskResponseBody(TeaModel):
     def __init__(
         self,
-        success: bool = None,
+        list: List[QueryCollectingTraceTaskResponseBodyList] = None,
     ):
-        self.success = success
+        self.list = list
 
     def validate(self):
-        pass
+        if self.list:
+            for k in self.list:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.success is not None:
-            result['success'] = self.success
+        result['list'] = []
+        if self.list is not None:
+            for k in self.list:
+                result['list'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('success') is not None:
-            self.success = m.get('success')
+        self.list = []
+        if m.get('list') is not None:
+            for k in m.get('list'):
+                temp_model = QueryCollectingTraceTaskResponseBodyList()
+                self.list.append(temp_model.from_map(k))
         return self
 
 
-class CloseTopboxResponse(TeaModel):
+class QueryCollectingTraceTaskResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: CloseTopboxResponseBody = None,
+        body: QueryCollectingTraceTaskResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -222,20 +423,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = CloseTopboxResponseBody()
+            temp_model = QueryCollectingTraceTaskResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class CreateTopboxHeaders(TeaModel):
+class QueryPageTraceDataHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -260,253 +461,198 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class CreateTopboxRequestCardData(TeaModel):
+class QueryPageTraceDataRequest(TeaModel):
     def __init__(
         self,
-        card_param_map: Dict[str, str] = None,
-    ):
-        self.card_param_map = card_param_map
+        end_time: int = None,
+        max_results: int = None,
+        next_token: int = None,
+        staff_id: str = None,
+        start_time: int = None,
+        trace_id: str = None,
+    ):
+        self.end_time = end_time
+        self.max_results = max_results
+        self.next_token = next_token
+        self.staff_id = staff_id
+        self.start_time = start_time
+        self.trace_id = trace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.card_param_map is not None:
-            result['cardParamMap'] = self.card_param_map
+        if self.end_time is not None:
+            result['endTime'] = self.end_time
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.staff_id is not None:
+            result['staffId'] = self.staff_id
+        if self.start_time is not None:
+            result['startTime'] = self.start_time
+        if self.trace_id is not None:
+            result['traceId'] = self.trace_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('cardParamMap') is not None:
-            self.card_param_map = m.get('cardParamMap')
+        if m.get('endTime') is not None:
+            self.end_time = m.get('endTime')
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('staffId') is not None:
+            self.staff_id = m.get('staffId')
+        if m.get('startTime') is not None:
+            self.start_time = m.get('startTime')
+        if m.get('traceId') is not None:
+            self.trace_id = m.get('traceId')
         return self
 
 
-class CreateTopboxRequestCardSettings(TeaModel):
+class QueryPageTraceDataResponseBodyListCoordinates(TeaModel):
     def __init__(
         self,
-        pull_strategy: bool = None,
+        latitude: float = None,
+        longitude: float = None,
     ):
-        self.pull_strategy = pull_strategy
+        self.latitude = latitude
+        self.longitude = longitude
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.pull_strategy is not None:
-            result['pullStrategy'] = self.pull_strategy
+        if self.latitude is not None:
+            result['latitude'] = self.latitude
+        if self.longitude is not None:
+            result['longitude'] = self.longitude
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('pullStrategy') is not None:
-            self.pull_strategy = m.get('pullStrategy')
+        if m.get('latitude') is not None:
+            self.latitude = m.get('latitude')
+        if m.get('longitude') is not None:
+            self.longitude = m.get('longitude')
         return self
 
 
-class CreateTopboxRequest(TeaModel):
+class QueryPageTraceDataResponseBodyList(TeaModel):
     def __init__(
         self,
-        callback_route_key: str = None,
-        card_data: CreateTopboxRequestCardData = None,
-        card_settings: CreateTopboxRequestCardSettings = None,
-        card_template_id: str = None,
-        conversation_type: int = None,
-        cool_app_code: str = None,
-        expired_time: int = None,
-        group_template_id: str = None,
-        open_conversation_id: str = None,
-        out_track_id: str = None,
-        platforms: str = None,
-        receiver_union_id_list: List[str] = None,
-        receiver_user_id_list: List[str] = None,
-        robot_code: str = None,
-        union_id_private_data_map: Dict[str, UnionIdPrivateDataMapValue] = None,
-        unoin_id: str = None,
-        user_id: str = None,
-        user_id_private_data_map: Dict[str, UserIdPrivateDataMapValue] = None,
+        coordinates: QueryPageTraceDataResponseBodyListCoordinates = None,
+        gmt_location: int = None,
+        gmt_upload: int = None,
     ):
-        self.callback_route_key = callback_route_key
-        self.card_data = card_data
-        self.card_settings = card_settings
-        self.card_template_id = card_template_id
-        self.conversation_type = conversation_type
-        self.cool_app_code = cool_app_code
-        self.expired_time = expired_time
-        self.group_template_id = group_template_id
-        self.open_conversation_id = open_conversation_id
-        self.out_track_id = out_track_id
-        self.platforms = platforms
-        self.receiver_union_id_list = receiver_union_id_list
-        self.receiver_user_id_list = receiver_user_id_list
-        self.robot_code = robot_code
-        self.union_id_private_data_map = union_id_private_data_map
-        self.unoin_id = unoin_id
-        self.user_id = user_id
-        self.user_id_private_data_map = user_id_private_data_map
+        self.coordinates = coordinates
+        self.gmt_location = gmt_location
+        self.gmt_upload = gmt_upload
 
     def validate(self):
-        if self.card_data:
-            self.card_data.validate()
-        if self.card_settings:
-            self.card_settings.validate()
-        if self.union_id_private_data_map:
-            for v in self.union_id_private_data_map.values():
-                if v:
-                    v.validate()
-        if self.user_id_private_data_map:
-            for v in self.user_id_private_data_map.values():
-                if v:
-                    v.validate()
+        if self.coordinates:
+            self.coordinates.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.callback_route_key is not None:
-            result['callbackRouteKey'] = self.callback_route_key
-        if self.card_data is not None:
-            result['cardData'] = self.card_data.to_map()
-        if self.card_settings is not None:
-            result['cardSettings'] = self.card_settings.to_map()
-        if self.card_template_id is not None:
-            result['cardTemplateId'] = self.card_template_id
-        if self.conversation_type is not None:
-            result['conversationType'] = self.conversation_type
-        if self.cool_app_code is not None:
-            result['coolAppCode'] = self.cool_app_code
-        if self.expired_time is not None:
-            result['expiredTime'] = self.expired_time
-        if self.group_template_id is not None:
-            result['groupTemplateId'] = self.group_template_id
-        if self.open_conversation_id is not None:
-            result['openConversationId'] = self.open_conversation_id
-        if self.out_track_id is not None:
-            result['outTrackId'] = self.out_track_id
-        if self.platforms is not None:
-            result['platforms'] = self.platforms
-        if self.receiver_union_id_list is not None:
-            result['receiverUnionIdList'] = self.receiver_union_id_list
-        if self.receiver_user_id_list is not None:
-            result['receiverUserIdList'] = self.receiver_user_id_list
-        if self.robot_code is not None:
-            result['robotCode'] = self.robot_code
-        result['unionIdPrivateDataMap'] = {}
-        if self.union_id_private_data_map is not None:
-            for k, v in self.union_id_private_data_map.items():
-                result['unionIdPrivateDataMap'][k] = v.to_map()
-        if self.unoin_id is not None:
-            result['unoinId'] = self.unoin_id
-        if self.user_id is not None:
-            result['userId'] = self.user_id
-        result['userIdPrivateDataMap'] = {}
-        if self.user_id_private_data_map is not None:
-            for k, v in self.user_id_private_data_map.items():
-                result['userIdPrivateDataMap'][k] = v.to_map()
+        if self.coordinates is not None:
+            result['coordinates'] = self.coordinates.to_map()
+        if self.gmt_location is not None:
+            result['gmtLocation'] = self.gmt_location
+        if self.gmt_upload is not None:
+            result['gmtUpload'] = self.gmt_upload
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('callbackRouteKey') is not None:
-            self.callback_route_key = m.get('callbackRouteKey')
-        if m.get('cardData') is not None:
-            temp_model = CreateTopboxRequestCardData()
-            self.card_data = temp_model.from_map(m['cardData'])
-        if m.get('cardSettings') is not None:
-            temp_model = CreateTopboxRequestCardSettings()
-            self.card_settings = temp_model.from_map(m['cardSettings'])
-        if m.get('cardTemplateId') is not None:
-            self.card_template_id = m.get('cardTemplateId')
-        if m.get('conversationType') is not None:
-            self.conversation_type = m.get('conversationType')
-        if m.get('coolAppCode') is not None:
-            self.cool_app_code = m.get('coolAppCode')
-        if m.get('expiredTime') is not None:
-            self.expired_time = m.get('expiredTime')
-        if m.get('groupTemplateId') is not None:
-            self.group_template_id = m.get('groupTemplateId')
-        if m.get('openConversationId') is not None:
-            self.open_conversation_id = m.get('openConversationId')
-        if m.get('outTrackId') is not None:
-            self.out_track_id = m.get('outTrackId')
-        if m.get('platforms') is not None:
-            self.platforms = m.get('platforms')
-        if m.get('receiverUnionIdList') is not None:
-            self.receiver_union_id_list = m.get('receiverUnionIdList')
-        if m.get('receiverUserIdList') is not None:
-            self.receiver_user_id_list = m.get('receiverUserIdList')
-        if m.get('robotCode') is not None:
-            self.robot_code = m.get('robotCode')
-        self.union_id_private_data_map = {}
-        if m.get('unionIdPrivateDataMap') is not None:
-            for k, v in m.get('unionIdPrivateDataMap').items():
-                temp_model = UnionIdPrivateDataMapValue()
-                self.union_id_private_data_map[k] = temp_model.from_map(v)
-        if m.get('unoinId') is not None:
-            self.unoin_id = m.get('unoinId')
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
-        self.user_id_private_data_map = {}
-        if m.get('userIdPrivateDataMap') is not None:
-            for k, v in m.get('userIdPrivateDataMap').items():
-                temp_model = UserIdPrivateDataMapValue()
-                self.user_id_private_data_map[k] = temp_model.from_map(v)
+        if m.get('coordinates') is not None:
+            temp_model = QueryPageTraceDataResponseBodyListCoordinates()
+            self.coordinates = temp_model.from_map(m['coordinates'])
+        if m.get('gmtLocation') is not None:
+            self.gmt_location = m.get('gmtLocation')
+        if m.get('gmtUpload') is not None:
+            self.gmt_upload = m.get('gmtUpload')
         return self
 
 
-class CreateTopboxResponseBody(TeaModel):
+class QueryPageTraceDataResponseBody(TeaModel):
     def __init__(
         self,
-        success: bool = None,
+        has_more: bool = None,
+        list: List[QueryPageTraceDataResponseBodyList] = None,
+        next_token: int = None,
     ):
-        self.success = success
+        self.has_more = has_more
+        self.list = list
+        self.next_token = next_token
 
     def validate(self):
-        pass
+        if self.list:
+            for k in self.list:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.success is not None:
-            result['success'] = self.success
+        if self.has_more is not None:
+            result['hasMore'] = self.has_more
+        result['list'] = []
+        if self.list is not None:
+            for k in self.list:
+                result['list'].append(k.to_map() if k else None)
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('success') is not None:
-            self.success = m.get('success')
+        if m.get('hasMore') is not None:
+            self.has_more = m.get('hasMore')
+        self.list = []
+        if m.get('list') is not None:
+            for k in m.get('list'):
+                temp_model = QueryPageTraceDataResponseBodyList()
+                self.list.append(temp_model.from_map(k))
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
         return self
 
 
-class CreateTopboxResponse(TeaModel):
+class QueryPageTraceDataResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: CreateTopboxResponseBody = None,
+        body: QueryPageTraceDataResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -532,12 +678,12 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = CreateTopboxResponseBody()
+            temp_model = QueryPageTraceDataResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -449,14 +449,72 @@
         return self.anhei_test_bwith_options(headers, runtime)
 
     async def anhei_test_b_async(self) -> dingtalkmicro_app__1__0_models.AnheiTestBResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.anhei_test_bwith_options_async(headers, runtime)
 
+    def anhei_test_nine_with_options(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkmicro_app__1__0_models.AnheiTestNineResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='AnheiTestNine',
+            version='microApp_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/microApp/anheiTestNine',
+            method='POST',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkmicro_app__1__0_models.AnheiTestNineResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def anhei_test_nine_with_options_async(
+        self,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkmicro_app__1__0_models.AnheiTestNineResponse:
+        req = open_api_models.OpenApiRequest(
+            headers=headers
+        )
+        params = open_api_models.Params(
+            action='AnheiTestNine',
+            version='microApp_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/microApp/anheiTestNine',
+            method='POST',
+            auth_type='Anonymous',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkmicro_app__1__0_models.AnheiTestNineResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def anhei_test_nine(self) -> dingtalkmicro_app__1__0_models.AnheiTestNineResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.anhei_test_nine_with_options(headers, runtime)
+
+    async def anhei_test_nine_async(self) -> dingtalkmicro_app__1__0_models.AnheiTestNineResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.anhei_test_nine_with_options_async(headers, runtime)
+
     def app_status_manager_test_with_options(
         self,
         request: dingtalkmicro_app__1__0_models.AppStatusManagerTestRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkmicro_app__1__0_models.AppStatusManagerTestResponse:
         UtilClient.validate_model(request)
@@ -1095,14 +1153,112 @@
         self,
         biz_app_id: str,
     ) -> dingtalkmicro_app__1__0_models.GetApaasAppResponse:
         runtime = util_models.RuntimeOptions()
         headers = dingtalkmicro_app__1__0_models.GetApaasAppHeaders()
         return await self.get_apaas_app_with_options_async(biz_app_id, headers, runtime)
 
+    def get_app_resource_use_info_with_options(
+        self,
+        request: dingtalkmicro_app__1__0_models.GetAppResourceUseInfoRequest,
+        headers: dingtalkmicro_app__1__0_models.GetAppResourceUseInfoHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkmicro_app__1__0_models.GetAppResourceUseInfoResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.benefit_code):
+            query['benefitCode'] = request.benefit_code
+        if not UtilClient.is_unset(request.end_time):
+            query['endTime'] = request.end_time
+        if not UtilClient.is_unset(request.period_type):
+            query['periodType'] = request.period_type
+        if not UtilClient.is_unset(request.start_time):
+            query['startTime'] = request.start_time
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetAppResourceUseInfo',
+            version='microApp_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/microApp/resources/useInfos',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='array'
+        )
+        return TeaCore.from_map(
+            dingtalkmicro_app__1__0_models.GetAppResourceUseInfoResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def get_app_resource_use_info_with_options_async(
+        self,
+        request: dingtalkmicro_app__1__0_models.GetAppResourceUseInfoRequest,
+        headers: dingtalkmicro_app__1__0_models.GetAppResourceUseInfoHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkmicro_app__1__0_models.GetAppResourceUseInfoResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.benefit_code):
+            query['benefitCode'] = request.benefit_code
+        if not UtilClient.is_unset(request.end_time):
+            query['endTime'] = request.end_time
+        if not UtilClient.is_unset(request.period_type):
+            query['periodType'] = request.period_type
+        if not UtilClient.is_unset(request.start_time):
+            query['startTime'] = request.start_time
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetAppResourceUseInfo',
+            version='microApp_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/microApp/resources/useInfos',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='array'
+        )
+        return TeaCore.from_map(
+            dingtalkmicro_app__1__0_models.GetAppResourceUseInfoResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def get_app_resource_use_info(
+        self,
+        request: dingtalkmicro_app__1__0_models.GetAppResourceUseInfoRequest,
+    ) -> dingtalkmicro_app__1__0_models.GetAppResourceUseInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkmicro_app__1__0_models.GetAppResourceUseInfoHeaders()
+        return self.get_app_resource_use_info_with_options(request, headers, runtime)
+
+    async def get_app_resource_use_info_async(
+        self,
+        request: dingtalkmicro_app__1__0_models.GetAppResourceUseInfoRequest,
+    ) -> dingtalkmicro_app__1__0_models.GetAppResourceUseInfoResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkmicro_app__1__0_models.GetAppResourceUseInfoHeaders()
+        return await self.get_app_resource_use_info_with_options_async(request, headers, runtime)
+
     def get_app_role_scope_by_role_id_with_options(
         self,
         agent_id: str,
         role_id: str,
         headers: dingtalkmicro_app__1__0_models.GetAppRoleScopeByRoleIdHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkmicro_app__1__0_models.GetAppRoleScopeByRoleIdResponse:
```

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -683,14 +683,85 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AnheiTestBResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class AnheiTestNineResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        return self
+
+
+class AnheiTestNineResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AnheiTestNineResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = AnheiTestNineResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class AppStatusManagerTestRequest(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
         self.request_id = request_id
 
@@ -1630,14 +1701,181 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetApaasAppResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetAppResourceUseInfoHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class GetAppResourceUseInfoRequest(TeaModel):
+    def __init__(
+        self,
+        benefit_code: str = None,
+        end_time: str = None,
+        period_type: str = None,
+        start_time: str = None,
+    ):
+        self.benefit_code = benefit_code
+        self.end_time = end_time
+        self.period_type = period_type
+        self.start_time = start_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.benefit_code is not None:
+            result['benefitCode'] = self.benefit_code
+        if self.end_time is not None:
+            result['endTime'] = self.end_time
+        if self.period_type is not None:
+            result['periodType'] = self.period_type
+        if self.start_time is not None:
+            result['startTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('benefitCode') is not None:
+            self.benefit_code = m.get('benefitCode')
+        if m.get('endTime') is not None:
+            self.end_time = m.get('endTime')
+        if m.get('periodType') is not None:
+            self.period_type = m.get('periodType')
+        if m.get('startTime') is not None:
+            self.start_time = m.get('startTime')
+        return self
+
+
+class GetAppResourceUseInfoResponseBody(TeaModel):
+    def __init__(
+        self,
+        period: str = None,
+        used_num: int = None,
+        quota_num: int = None,
+    ):
+        self.period = period
+        self.used_num = used_num
+        self.quota_num = quota_num
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.period is not None:
+            result['period'] = self.period
+        if self.used_num is not None:
+            result['usedNum'] = self.used_num
+        if self.quota_num is not None:
+            result['quotaNum'] = self.quota_num
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('period') is not None:
+            self.period = m.get('period')
+        if m.get('usedNum') is not None:
+            self.used_num = m.get('usedNum')
+        if m.get('quotaNum') is not None:
+            self.quota_num = m.get('quotaNum')
+        return self
+
+
+class GetAppResourceUseInfoResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: List[GetAppResourceUseInfoResponseBody] = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            for k in self.body:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        result['body'] = []
+        if self.body is not None:
+            for k in self.body:
+                result['body'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        self.body = []
+        if m.get('body') is not None:
+            for k in m.get('body'):
+                temp_model = GetAppResourceUseInfoResponseBody()
+                self.body.append(temp_model.from_map(k))
+        return self
+
+
 class GetAppRoleScopeByRoleIdHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import Dict
 
 
-class RunCallUserHeaders(TeaModel):
+class CountWorkRecordHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -33,92 +33,74 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class RunCallUserRequest(TeaModel):
+class CountWorkRecordRequest(TeaModel):
     def __init__(
         self,
-        authorize_corp_id: str = None,
-        authorize_user_id: str = None,
-        order_id: str = None,
         user_id: str = None,
     ):
-        self.authorize_corp_id = authorize_corp_id
-        self.authorize_user_id = authorize_user_id
-        self.order_id = order_id
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.authorize_corp_id is not None:
-            result['authorizeCorpId'] = self.authorize_corp_id
-        if self.authorize_user_id is not None:
-            result['authorizeUserId'] = self.authorize_user_id
-        if self.order_id is not None:
-            result['orderId'] = self.order_id
         if self.user_id is not None:
             result['userId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('authorizeCorpId') is not None:
-            self.authorize_corp_id = m.get('authorizeCorpId')
-        if m.get('authorizeUserId') is not None:
-            self.authorize_user_id = m.get('authorizeUserId')
-        if m.get('orderId') is not None:
-            self.order_id = m.get('orderId')
         if m.get('userId') is not None:
             self.user_id = m.get('userId')
         return self
 
 
-class RunCallUserResponseBody(TeaModel):
+class CountWorkRecordResponseBody(TeaModel):
     def __init__(
         self,
-        success: str = None,
+        undo_count: int = None,
     ):
-        self.success = success
+        self.undo_count = undo_count
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.success is not None:
-            result['success'] = self.success
+        if self.undo_count is not None:
+            result['undoCount'] = self.undo_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('success') is not None:
-            self.success = m.get('success')
+        if m.get('undoCount') is not None:
+            self.undo_count = m.get('undoCount')
         return self
 
 
-class RunCallUserResponse(TeaModel):
+class CountWorkRecordResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: RunCallUserResponseBody = None,
+        body: CountWorkRecordResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -144,12 +126,12 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = RunCallUserResponseBody()
+            temp_model = CountWorkRecordResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import Dict, List
 
 
-class QueryAppActiveUsersHeaders(TeaModel):
+class WikiWordsDetailHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -33,371 +33,390 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class QueryAppActiveUsersRequest(TeaModel):
+class WikiWordsDetailRequest(TeaModel):
     def __init__(
         self,
-        max_results: int = None,
-        need_position_info: bool = None,
-        next_token: int = None,
+        word_name: str = None,
     ):
-        self.max_results = max_results
-        self.need_position_info = need_position_info
-        self.next_token = next_token
+        self.word_name = word_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.max_results is not None:
-            result['maxResults'] = self.max_results
-        if self.need_position_info is not None:
-            result['needPositionInfo'] = self.need_position_info
-        if self.next_token is not None:
-            result['nextToken'] = self.next_token
+        if self.word_name is not None:
+            result['wordName'] = self.word_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('maxResults') is not None:
-            self.max_results = m.get('maxResults')
-        if m.get('needPositionInfo') is not None:
-            self.need_position_info = m.get('needPositionInfo')
-        if m.get('nextToken') is not None:
-            self.next_token = m.get('nextToken')
+        if m.get('wordName') is not None:
+            self.word_name = m.get('wordName')
         return self
 
 
-class QueryAppActiveUsersResponseBodyList(TeaModel):
+class WikiWordsDetailResponseBodyDataAppLink(TeaModel):
     def __init__(
         self,
-        app_trace_id: str = None,
-        latitude: float = None,
-        longitude: float = None,
-        report_time: int = None,
-        start_time: int = None,
-        user_id: str = None,
+        app_id: int = None,
+        app_name: str = None,
+        icon_link: str = None,
+        pc_link: str = None,
+        phone_link: str = None,
     ):
-        self.app_trace_id = app_trace_id
-        self.latitude = latitude
-        self.longitude = longitude
-        self.report_time = report_time
-        self.start_time = start_time
-        self.user_id = user_id
+        self.app_id = app_id
+        self.app_name = app_name
+        self.icon_link = icon_link
+        self.pc_link = pc_link
+        self.phone_link = phone_link
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.app_trace_id is not None:
-            result['appTraceId'] = self.app_trace_id
-        if self.latitude is not None:
-            result['latitude'] = self.latitude
-        if self.longitude is not None:
-            result['longitude'] = self.longitude
-        if self.report_time is not None:
-            result['reportTime'] = self.report_time
-        if self.start_time is not None:
-            result['startTime'] = self.start_time
-        if self.user_id is not None:
-            result['userId'] = self.user_id
+        if self.app_id is not None:
+            result['appId'] = self.app_id
+        if self.app_name is not None:
+            result['appName'] = self.app_name
+        if self.icon_link is not None:
+            result['iconLink'] = self.icon_link
+        if self.pc_link is not None:
+            result['pcLink'] = self.pc_link
+        if self.phone_link is not None:
+            result['phoneLink'] = self.phone_link
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('appTraceId') is not None:
-            self.app_trace_id = m.get('appTraceId')
-        if m.get('latitude') is not None:
-            self.latitude = m.get('latitude')
-        if m.get('longitude') is not None:
-            self.longitude = m.get('longitude')
-        if m.get('reportTime') is not None:
-            self.report_time = m.get('reportTime')
-        if m.get('startTime') is not None:
-            self.start_time = m.get('startTime')
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
+        if m.get('appId') is not None:
+            self.app_id = m.get('appId')
+        if m.get('appName') is not None:
+            self.app_name = m.get('appName')
+        if m.get('iconLink') is not None:
+            self.icon_link = m.get('iconLink')
+        if m.get('pcLink') is not None:
+            self.pc_link = m.get('pcLink')
+        if m.get('phoneLink') is not None:
+            self.phone_link = m.get('phoneLink')
         return self
 
 
-class QueryAppActiveUsersResponseBody(TeaModel):
+class WikiWordsDetailResponseBodyDataRelatedDoc(TeaModel):
     def __init__(
         self,
-        has_more: bool = None,
-        list: List[QueryAppActiveUsersResponseBodyList] = None,
-        next_token: int = None,
-        total_count: int = None,
+        link: str = None,
+        name: str = None,
+        type: str = None,
     ):
-        self.has_more = has_more
-        self.list = list
-        self.next_token = next_token
-        self.total_count = total_count
-
-    def validate(self):
-        if self.list:
-            for k in self.list:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.has_more is not None:
-            result['hasMore'] = self.has_more
-        result['list'] = []
-        if self.list is not None:
-            for k in self.list:
-                result['list'].append(k.to_map() if k else None)
-        if self.next_token is not None:
-            result['nextToken'] = self.next_token
-        if self.total_count is not None:
-            result['totalCount'] = self.total_count
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('hasMore') is not None:
-            self.has_more = m.get('hasMore')
-        self.list = []
-        if m.get('list') is not None:
-            for k in m.get('list'):
-                temp_model = QueryAppActiveUsersResponseBodyList()
-                self.list.append(temp_model.from_map(k))
-        if m.get('nextToken') is not None:
-            self.next_token = m.get('nextToken')
-        if m.get('totalCount') is not None:
-            self.total_count = m.get('totalCount')
-        return self
-
-
-class QueryAppActiveUsersResponse(TeaModel):
-    def __init__(
-        self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: QueryAppActiveUsersResponseBody = None,
-    ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
-
-    def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
-        if self.body:
-            self.body.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = QueryAppActiveUsersResponseBody()
-            self.body = temp_model.from_map(m['body'])
-        return self
-
-
-class QueryCollectingTraceTaskHeaders(TeaModel):
-    def __init__(
-        self,
-        common_headers: Dict[str, str] = None,
-        x_acs_dingtalk_access_token: str = None,
-    ):
-        self.common_headers = common_headers
-        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+        self.link = link
+        self.name = name
+        self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.common_headers is not None:
-            result['commonHeaders'] = self.common_headers
-        if self.x_acs_dingtalk_access_token is not None:
-            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        if self.link is not None:
+            result['link'] = self.link
+        if self.name is not None:
+            result['name'] = self.name
+        if self.type is not None:
+            result['type'] = self.type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('commonHeaders') is not None:
-            self.common_headers = m.get('commonHeaders')
-        if m.get('x-acs-dingtalk-access-token') is not None:
-            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        if m.get('link') is not None:
+            self.link = m.get('link')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('type') is not None:
+            self.type = m.get('type')
         return self
 
 
-class QueryCollectingTraceTaskRequest(TeaModel):
+class WikiWordsDetailResponseBodyDataRelatedLink(TeaModel):
     def __init__(
         self,
-        user_ids: List[str] = None,
+        link: str = None,
+        name: str = None,
+        type: str = None,
     ):
-        self.user_ids = user_ids
+        self.link = link
+        self.name = name
+        self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.user_ids is not None:
-            result['userIds'] = self.user_ids
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('userIds') is not None:
-            self.user_ids = m.get('userIds')
-        return self
-
-
-class QueryCollectingTraceTaskResponseBodyList(TeaModel):
-    def __init__(
-        self,
-        app_trace_id: str = None,
-        geo_collect_period: int = None,
-        geo_report_period: int = None,
-        geo_report_status: int = None,
-        report_end_time: int = None,
-        report_start_time: int = None,
-        user_id: str = None,
-    ):
-        self.app_trace_id = app_trace_id
-        self.geo_collect_period = geo_collect_period
-        self.geo_report_period = geo_report_period
-        self.geo_report_status = geo_report_status
-        self.report_end_time = report_end_time
-        self.report_start_time = report_start_time
-        self.user_id = user_id
+        if self.link is not None:
+            result['link'] = self.link
+        if self.name is not None:
+            result['name'] = self.name
+        if self.type is not None:
+            result['type'] = self.type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('link') is not None:
+            self.link = m.get('link')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        return self
+
+
+class WikiWordsDetailResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        app_link: List[WikiWordsDetailResponseBodyDataAppLink] = None,
+        approve_name: str = None,
+        contacts: List[str] = None,
+        creator_name: str = None,
+        gmt_create: int = None,
+        gmt_modify: int = None,
+        high_light_word_alias: List[str] = None,
+        im_high_light: bool = None,
+        org_name: str = None,
+        related_doc: List[WikiWordsDetailResponseBodyDataRelatedDoc] = None,
+        related_link: List[WikiWordsDetailResponseBodyDataRelatedLink] = None,
+        sim_high_light: bool = None,
+        simple_word_paraphrase: str = None,
+        tags_list: List[str] = None,
+        updater_name: str = None,
+        uuid: int = None,
+        word_alias: List[str] = None,
+        word_full_name: str = None,
+        word_name: str = None,
+        word_paraphrase: str = None,
+    ):
+        self.app_link = app_link
+        self.approve_name = approve_name
+        self.contacts = contacts
+        self.creator_name = creator_name
+        self.gmt_create = gmt_create
+        self.gmt_modify = gmt_modify
+        self.high_light_word_alias = high_light_word_alias
+        self.im_high_light = im_high_light
+        self.org_name = org_name
+        self.related_doc = related_doc
+        self.related_link = related_link
+        self.sim_high_light = sim_high_light
+        self.simple_word_paraphrase = simple_word_paraphrase
+        self.tags_list = tags_list
+        self.updater_name = updater_name
+        self.uuid = uuid
+        self.word_alias = word_alias
+        self.word_full_name = word_full_name
+        self.word_name = word_name
+        self.word_paraphrase = word_paraphrase
 
     def validate(self):
-        pass
+        if self.app_link:
+            for k in self.app_link:
+                if k:
+                    k.validate()
+        if self.related_doc:
+            for k in self.related_doc:
+                if k:
+                    k.validate()
+        if self.related_link:
+            for k in self.related_link:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.app_trace_id is not None:
-            result['appTraceId'] = self.app_trace_id
-        if self.geo_collect_period is not None:
-            result['geoCollectPeriod'] = self.geo_collect_period
-        if self.geo_report_period is not None:
-            result['geoReportPeriod'] = self.geo_report_period
-        if self.geo_report_status is not None:
-            result['geoReportStatus'] = self.geo_report_status
-        if self.report_end_time is not None:
-            result['reportEndTime'] = self.report_end_time
-        if self.report_start_time is not None:
-            result['reportStartTime'] = self.report_start_time
-        if self.user_id is not None:
-            result['userId'] = self.user_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('appTraceId') is not None:
-            self.app_trace_id = m.get('appTraceId')
-        if m.get('geoCollectPeriod') is not None:
-            self.geo_collect_period = m.get('geoCollectPeriod')
-        if m.get('geoReportPeriod') is not None:
-            self.geo_report_period = m.get('geoReportPeriod')
-        if m.get('geoReportStatus') is not None:
-            self.geo_report_status = m.get('geoReportStatus')
-        if m.get('reportEndTime') is not None:
-            self.report_end_time = m.get('reportEndTime')
-        if m.get('reportStartTime') is not None:
-            self.report_start_time = m.get('reportStartTime')
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
-        return self
-
-
-class QueryCollectingTraceTaskResponseBody(TeaModel):
-    def __init__(
-        self,
-        list: List[QueryCollectingTraceTaskResponseBodyList] = None,
-    ):
-        self.list = list
+        result['appLink'] = []
+        if self.app_link is not None:
+            for k in self.app_link:
+                result['appLink'].append(k.to_map() if k else None)
+        if self.approve_name is not None:
+            result['approveName'] = self.approve_name
+        if self.contacts is not None:
+            result['contacts'] = self.contacts
+        if self.creator_name is not None:
+            result['creatorName'] = self.creator_name
+        if self.gmt_create is not None:
+            result['gmtCreate'] = self.gmt_create
+        if self.gmt_modify is not None:
+            result['gmtModify'] = self.gmt_modify
+        if self.high_light_word_alias is not None:
+            result['highLightWordAlias'] = self.high_light_word_alias
+        if self.im_high_light is not None:
+            result['imHighLight'] = self.im_high_light
+        if self.org_name is not None:
+            result['orgName'] = self.org_name
+        result['relatedDoc'] = []
+        if self.related_doc is not None:
+            for k in self.related_doc:
+                result['relatedDoc'].append(k.to_map() if k else None)
+        result['relatedLink'] = []
+        if self.related_link is not None:
+            for k in self.related_link:
+                result['relatedLink'].append(k.to_map() if k else None)
+        if self.sim_high_light is not None:
+            result['simHighLight'] = self.sim_high_light
+        if self.simple_word_paraphrase is not None:
+            result['simpleWordParaphrase'] = self.simple_word_paraphrase
+        if self.tags_list is not None:
+            result['tagsList'] = self.tags_list
+        if self.updater_name is not None:
+            result['updaterName'] = self.updater_name
+        if self.uuid is not None:
+            result['uuid'] = self.uuid
+        if self.word_alias is not None:
+            result['wordAlias'] = self.word_alias
+        if self.word_full_name is not None:
+            result['wordFullName'] = self.word_full_name
+        if self.word_name is not None:
+            result['wordName'] = self.word_name
+        if self.word_paraphrase is not None:
+            result['wordParaphrase'] = self.word_paraphrase
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.app_link = []
+        if m.get('appLink') is not None:
+            for k in m.get('appLink'):
+                temp_model = WikiWordsDetailResponseBodyDataAppLink()
+                self.app_link.append(temp_model.from_map(k))
+        if m.get('approveName') is not None:
+            self.approve_name = m.get('approveName')
+        if m.get('contacts') is not None:
+            self.contacts = m.get('contacts')
+        if m.get('creatorName') is not None:
+            self.creator_name = m.get('creatorName')
+        if m.get('gmtCreate') is not None:
+            self.gmt_create = m.get('gmtCreate')
+        if m.get('gmtModify') is not None:
+            self.gmt_modify = m.get('gmtModify')
+        if m.get('highLightWordAlias') is not None:
+            self.high_light_word_alias = m.get('highLightWordAlias')
+        if m.get('imHighLight') is not None:
+            self.im_high_light = m.get('imHighLight')
+        if m.get('orgName') is not None:
+            self.org_name = m.get('orgName')
+        self.related_doc = []
+        if m.get('relatedDoc') is not None:
+            for k in m.get('relatedDoc'):
+                temp_model = WikiWordsDetailResponseBodyDataRelatedDoc()
+                self.related_doc.append(temp_model.from_map(k))
+        self.related_link = []
+        if m.get('relatedLink') is not None:
+            for k in m.get('relatedLink'):
+                temp_model = WikiWordsDetailResponseBodyDataRelatedLink()
+                self.related_link.append(temp_model.from_map(k))
+        if m.get('simHighLight') is not None:
+            self.sim_high_light = m.get('simHighLight')
+        if m.get('simpleWordParaphrase') is not None:
+            self.simple_word_paraphrase = m.get('simpleWordParaphrase')
+        if m.get('tagsList') is not None:
+            self.tags_list = m.get('tagsList')
+        if m.get('updaterName') is not None:
+            self.updater_name = m.get('updaterName')
+        if m.get('uuid') is not None:
+            self.uuid = m.get('uuid')
+        if m.get('wordAlias') is not None:
+            self.word_alias = m.get('wordAlias')
+        if m.get('wordFullName') is not None:
+            self.word_full_name = m.get('wordFullName')
+        if m.get('wordName') is not None:
+            self.word_name = m.get('wordName')
+        if m.get('wordParaphrase') is not None:
+            self.word_paraphrase = m.get('wordParaphrase')
+        return self
+
+
+class WikiWordsDetailResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: List[WikiWordsDetailResponseBodyData] = None,
+        err_msg: str = None,
+        success: bool = None,
+    ):
+        self.data = data
+        self.err_msg = err_msg
+        self.success = success
 
     def validate(self):
-        if self.list:
-            for k in self.list:
+        if self.data:
+            for k in self.data:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['list'] = []
-        if self.list is not None:
-            for k in self.list:
-                result['list'].append(k.to_map() if k else None)
+        result['data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['data'].append(k.to_map() if k else None)
+        if self.err_msg is not None:
+            result['errMsg'] = self.err_msg
+        if self.success is not None:
+            result['success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.list = []
-        if m.get('list') is not None:
-            for k in m.get('list'):
-                temp_model = QueryCollectingTraceTaskResponseBodyList()
-                self.list.append(temp_model.from_map(k))
+        self.data = []
+        if m.get('data') is not None:
+            for k in m.get('data'):
+                temp_model = WikiWordsDetailResponseBodyData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('errMsg') is not None:
+            self.err_msg = m.get('errMsg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
         return self
 
 
-class QueryCollectingTraceTaskResponse(TeaModel):
+class WikiWordsDetailResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: QueryCollectingTraceTaskResponseBody = None,
+        body: WikiWordsDetailResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -423,20 +442,20 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = QueryCollectingTraceTaskResponseBody()
+            temp_model = WikiWordsDetailResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class QueryPageTraceDataHeaders(TeaModel):
+class WikiWordsParseHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -461,198 +480,133 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class QueryPageTraceDataRequest(TeaModel):
-    def __init__(
-        self,
-        end_time: int = None,
-        max_results: int = None,
-        next_token: int = None,
-        staff_id: str = None,
-        start_time: int = None,
-        trace_id: str = None,
-    ):
-        self.end_time = end_time
-        self.max_results = max_results
-        self.next_token = next_token
-        self.staff_id = staff_id
-        self.start_time = start_time
-        self.trace_id = trace_id
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.end_time is not None:
-            result['endTime'] = self.end_time
-        if self.max_results is not None:
-            result['maxResults'] = self.max_results
-        if self.next_token is not None:
-            result['nextToken'] = self.next_token
-        if self.staff_id is not None:
-            result['staffId'] = self.staff_id
-        if self.start_time is not None:
-            result['startTime'] = self.start_time
-        if self.trace_id is not None:
-            result['traceId'] = self.trace_id
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('endTime') is not None:
-            self.end_time = m.get('endTime')
-        if m.get('maxResults') is not None:
-            self.max_results = m.get('maxResults')
-        if m.get('nextToken') is not None:
-            self.next_token = m.get('nextToken')
-        if m.get('staffId') is not None:
-            self.staff_id = m.get('staffId')
-        if m.get('startTime') is not None:
-            self.start_time = m.get('startTime')
-        if m.get('traceId') is not None:
-            self.trace_id = m.get('traceId')
-        return self
-
-
-class QueryPageTraceDataResponseBodyListCoordinates(TeaModel):
+class WikiWordsParseRequest(TeaModel):
     def __init__(
         self,
-        latitude: float = None,
-        longitude: float = None,
+        content: str = None,
     ):
-        self.latitude = latitude
-        self.longitude = longitude
+        self.content = content
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.latitude is not None:
-            result['latitude'] = self.latitude
-        if self.longitude is not None:
-            result['longitude'] = self.longitude
+        if self.content is not None:
+            result['content'] = self.content
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('latitude') is not None:
-            self.latitude = m.get('latitude')
-        if m.get('longitude') is not None:
-            self.longitude = m.get('longitude')
+        if m.get('content') is not None:
+            self.content = m.get('content')
         return self
 
 
-class QueryPageTraceDataResponseBodyList(TeaModel):
+class WikiWordsParseResponseBodyData(TeaModel):
     def __init__(
         self,
-        coordinates: QueryPageTraceDataResponseBodyListCoordinates = None,
-        gmt_location: int = None,
-        gmt_upload: int = None,
+        end_index: int = None,
+        start_index: int = None,
+        word_name: str = None,
     ):
-        self.coordinates = coordinates
-        self.gmt_location = gmt_location
-        self.gmt_upload = gmt_upload
+        self.end_index = end_index
+        self.start_index = start_index
+        self.word_name = word_name
 
     def validate(self):
-        if self.coordinates:
-            self.coordinates.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.coordinates is not None:
-            result['coordinates'] = self.coordinates.to_map()
-        if self.gmt_location is not None:
-            result['gmtLocation'] = self.gmt_location
-        if self.gmt_upload is not None:
-            result['gmtUpload'] = self.gmt_upload
+        if self.end_index is not None:
+            result['endIndex'] = self.end_index
+        if self.start_index is not None:
+            result['startIndex'] = self.start_index
+        if self.word_name is not None:
+            result['wordName'] = self.word_name
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('coordinates') is not None:
-            temp_model = QueryPageTraceDataResponseBodyListCoordinates()
-            self.coordinates = temp_model.from_map(m['coordinates'])
-        if m.get('gmtLocation') is not None:
-            self.gmt_location = m.get('gmtLocation')
-        if m.get('gmtUpload') is not None:
-            self.gmt_upload = m.get('gmtUpload')
+        if m.get('endIndex') is not None:
+            self.end_index = m.get('endIndex')
+        if m.get('startIndex') is not None:
+            self.start_index = m.get('startIndex')
+        if m.get('wordName') is not None:
+            self.word_name = m.get('wordName')
         return self
 
 
-class QueryPageTraceDataResponseBody(TeaModel):
+class WikiWordsParseResponseBody(TeaModel):
     def __init__(
         self,
-        has_more: bool = None,
-        list: List[QueryPageTraceDataResponseBodyList] = None,
-        next_token: int = None,
+        data: List[WikiWordsParseResponseBodyData] = None,
+        err_msg: str = None,
+        success: bool = None,
     ):
-        self.has_more = has_more
-        self.list = list
-        self.next_token = next_token
+        self.data = data
+        self.err_msg = err_msg
+        self.success = success
 
     def validate(self):
-        if self.list:
-            for k in self.list:
+        if self.data:
+            for k in self.data:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.has_more is not None:
-            result['hasMore'] = self.has_more
-        result['list'] = []
-        if self.list is not None:
-            for k in self.list:
-                result['list'].append(k.to_map() if k else None)
-        if self.next_token is not None:
-            result['nextToken'] = self.next_token
+        result['data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['data'].append(k.to_map() if k else None)
+        if self.err_msg is not None:
+            result['errMsg'] = self.err_msg
+        if self.success is not None:
+            result['success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('hasMore') is not None:
-            self.has_more = m.get('hasMore')
-        self.list = []
-        if m.get('list') is not None:
-            for k in m.get('list'):
-                temp_model = QueryPageTraceDataResponseBodyList()
-                self.list.append(temp_model.from_map(k))
-        if m.get('nextToken') is not None:
-            self.next_token = m.get('nextToken')
+        self.data = []
+        if m.get('data') is not None:
+            for k in m.get('data'):
+                temp_model = WikiWordsParseResponseBodyData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('errMsg') is not None:
+            self.err_msg = m.get('errMsg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
         return self
 
 
-class QueryPageTraceDataResponse(TeaModel):
+class WikiWordsParseResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: QueryPageTraceDataResponseBody = None,
+        body: WikiWordsParseResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -678,12 +632,12 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = QueryPageTraceDataResponseBody()
+            temp_model = WikiWordsParseResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from Tea.core import TeaCore
 
 from alibabacloud_gateway_spi.client import Client as SPIClient
 from alibabacloud_tea_openapi.client import Client as OpenApiClient
 from alibabacloud_tea_openapi import models as open_api_models
 from alibabacloud_gateway_dingtalk.client import Client as GatewayClientClient
 from alibabacloud_tea_util.client import Client as UtilClient
-from alibabacloud_dingtalk.trip_1_0 import models as dingtalktrip__1__0_models
+from alibabacloud_dingtalk.im_2_0 import models as dingtalkim__2__0_models
 from alibabacloud_tea_util import models as util_models
 from alibabacloud_openapi_util.client import Client as OpenApiUtilClient
 
 
 class Client(OpenApiClient):
     """
     *\
@@ -25,384 +25,470 @@
         super().__init__(config)
         self._client = GatewayClientClient()
         self._spi = self._client
         self._endpoint_rule = ''
         if UtilClient.empty(self._endpoint):
             self._endpoint = 'api.dingtalk.com'
 
-    def sync_business_sign_info_with_options(
+    def close_topbox_with_options(
         self,
-        request: dingtalktrip__1__0_models.SyncBusinessSignInfoRequest,
-        headers: dingtalktrip__1__0_models.SyncBusinessSignInfoHeaders,
+        request: dingtalkim__2__0_models.CloseTopboxRequest,
+        headers: dingtalkim__2__0_models.CloseTopboxHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalktrip__1__0_models.SyncBusinessSignInfoResponse:
+    ) -> dingtalkim__2__0_models.CloseTopboxResponse:
         UtilClient.validate_model(request)
         body = {}
-        if not UtilClient.is_unset(request.biz_type_list):
-            body['bizTypeList'] = request.biz_type_list
-        if not UtilClient.is_unset(request.gmt_org_pay):
-            body['gmtOrgPay'] = request.gmt_org_pay
-        if not UtilClient.is_unset(request.gmt_sign):
-            body['gmtSign'] = request.gmt_sign
-        if not UtilClient.is_unset(request.org_pay_status):
-            body['orgPayStatus'] = request.org_pay_status
-        if not UtilClient.is_unset(request.sign_status):
-            body['signStatus'] = request.sign_status
-        if not UtilClient.is_unset(request.target_corp_id):
-            body['targetCorpId'] = request.target_corp_id
+        if not UtilClient.is_unset(request.conversation_type):
+            body['conversationType'] = request.conversation_type
+        if not UtilClient.is_unset(request.cool_app_code):
+            body['coolAppCode'] = request.cool_app_code
+        if not UtilClient.is_unset(request.group_template_id):
+            body['groupTemplateId'] = request.group_template_id
+        if not UtilClient.is_unset(request.open_conversation_id):
+            body['openConversationId'] = request.open_conversation_id
+        if not UtilClient.is_unset(request.out_track_id):
+            body['outTrackId'] = request.out_track_id
+        if not UtilClient.is_unset(request.robot_code):
+            body['robotCode'] = request.robot_code
+        if not UtilClient.is_unset(request.unoin_id):
+            body['unoinId'] = request.unoin_id
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
-            action='SyncBusinessSignInfo',
-            version='trip_1.0',
+            action='CloseTopbox',
+            version='im_2.0',
             protocol='HTTP',
-            pathname=f'/v1.0/trip/businessSignInfos/sync',
+            pathname=f'/v2.0/im/topBoxes/close',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalktrip__1__0_models.SyncBusinessSignInfoResponse(),
+            dingtalkim__2__0_models.CloseTopboxResponse(),
             self.execute(params, req, runtime)
         )
 
-    async def sync_business_sign_info_with_options_async(
+    async def close_topbox_with_options_async(
         self,
-        request: dingtalktrip__1__0_models.SyncBusinessSignInfoRequest,
-        headers: dingtalktrip__1__0_models.SyncBusinessSignInfoHeaders,
+        request: dingtalkim__2__0_models.CloseTopboxRequest,
+        headers: dingtalkim__2__0_models.CloseTopboxHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalktrip__1__0_models.SyncBusinessSignInfoResponse:
+    ) -> dingtalkim__2__0_models.CloseTopboxResponse:
         UtilClient.validate_model(request)
         body = {}
-        if not UtilClient.is_unset(request.biz_type_list):
-            body['bizTypeList'] = request.biz_type_list
-        if not UtilClient.is_unset(request.gmt_org_pay):
-            body['gmtOrgPay'] = request.gmt_org_pay
-        if not UtilClient.is_unset(request.gmt_sign):
-            body['gmtSign'] = request.gmt_sign
-        if not UtilClient.is_unset(request.org_pay_status):
-            body['orgPayStatus'] = request.org_pay_status
-        if not UtilClient.is_unset(request.sign_status):
-            body['signStatus'] = request.sign_status
-        if not UtilClient.is_unset(request.target_corp_id):
-            body['targetCorpId'] = request.target_corp_id
+        if not UtilClient.is_unset(request.conversation_type):
+            body['conversationType'] = request.conversation_type
+        if not UtilClient.is_unset(request.cool_app_code):
+            body['coolAppCode'] = request.cool_app_code
+        if not UtilClient.is_unset(request.group_template_id):
+            body['groupTemplateId'] = request.group_template_id
+        if not UtilClient.is_unset(request.open_conversation_id):
+            body['openConversationId'] = request.open_conversation_id
+        if not UtilClient.is_unset(request.out_track_id):
+            body['outTrackId'] = request.out_track_id
+        if not UtilClient.is_unset(request.robot_code):
+            body['robotCode'] = request.robot_code
+        if not UtilClient.is_unset(request.unoin_id):
+            body['unoinId'] = request.unoin_id
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
-            action='SyncBusinessSignInfo',
-            version='trip_1.0',
+            action='CloseTopbox',
+            version='im_2.0',
             protocol='HTTP',
-            pathname=f'/v1.0/trip/businessSignInfos/sync',
+            pathname=f'/v2.0/im/topBoxes/close',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalktrip__1__0_models.SyncBusinessSignInfoResponse(),
+            dingtalkim__2__0_models.CloseTopboxResponse(),
             await self.execute_async(params, req, runtime)
         )
 
-    def sync_business_sign_info(
+    def close_topbox(
         self,
-        request: dingtalktrip__1__0_models.SyncBusinessSignInfoRequest,
-    ) -> dingtalktrip__1__0_models.SyncBusinessSignInfoResponse:
+        request: dingtalkim__2__0_models.CloseTopboxRequest,
+    ) -> dingtalkim__2__0_models.CloseTopboxResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalktrip__1__0_models.SyncBusinessSignInfoHeaders()
-        return self.sync_business_sign_info_with_options(request, headers, runtime)
+        headers = dingtalkim__2__0_models.CloseTopboxHeaders()
+        return self.close_topbox_with_options(request, headers, runtime)
 
-    async def sync_business_sign_info_async(
+    async def close_topbox_async(
         self,
-        request: dingtalktrip__1__0_models.SyncBusinessSignInfoRequest,
-    ) -> dingtalktrip__1__0_models.SyncBusinessSignInfoResponse:
+        request: dingtalkim__2__0_models.CloseTopboxRequest,
+    ) -> dingtalkim__2__0_models.CloseTopboxResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalktrip__1__0_models.SyncBusinessSignInfoHeaders()
-        return await self.sync_business_sign_info_with_options_async(request, headers, runtime)
+        headers = dingtalkim__2__0_models.CloseTopboxHeaders()
+        return await self.close_topbox_with_options_async(request, headers, runtime)
 
-    def sync_secret_key_with_options(
+    def create_couple_group_with_options(
         self,
-        request: dingtalktrip__1__0_models.SyncSecretKeyRequest,
-        headers: dingtalktrip__1__0_models.SyncSecretKeyHeaders,
+        request: dingtalkim__2__0_models.CreateCoupleGroupRequest,
+        headers: dingtalkim__2__0_models.CreateCoupleGroupHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalktrip__1__0_models.SyncSecretKeyResponse:
+    ) -> dingtalkim__2__0_models.CreateCoupleGroupResponse:
         UtilClient.validate_model(request)
         body = {}
-        if not UtilClient.is_unset(request.action_type):
-            body['actionType'] = request.action_type
-        if not UtilClient.is_unset(request.secret_string):
-            body['secretString'] = request.secret_string
-        if not UtilClient.is_unset(request.target_corp_id):
-            body['targetCorpId'] = request.target_corp_id
-        if not UtilClient.is_unset(request.trip_app_key):
-            body['tripAppKey'] = request.trip_app_key
-        if not UtilClient.is_unset(request.trip_app_security):
-            body['tripAppSecurity'] = request.trip_app_security
-        if not UtilClient.is_unset(request.trip_corp_id):
-            body['tripCorpId'] = request.trip_corp_id
+        if not UtilClient.is_unset(request.group_template_id):
+            body['groupTemplateId'] = request.group_template_id
+        if not UtilClient.is_unset(request.operator_id):
+            body['operatorId'] = request.operator_id
+        if not UtilClient.is_unset(request.users):
+            body['users'] = request.users
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
-            action='SyncSecretKey',
-            version='trip_1.0',
+            action='CreateCoupleGroup',
+            version='im_2.0',
             protocol='HTTP',
-            pathname=f'/v1.0/trip/secretKeys/sync',
+            pathname=f'/v2.0/im/interconnections/couples/groups',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalktrip__1__0_models.SyncSecretKeyResponse(),
+            dingtalkim__2__0_models.CreateCoupleGroupResponse(),
             self.execute(params, req, runtime)
         )
 
-    async def sync_secret_key_with_options_async(
+    async def create_couple_group_with_options_async(
         self,
-        request: dingtalktrip__1__0_models.SyncSecretKeyRequest,
-        headers: dingtalktrip__1__0_models.SyncSecretKeyHeaders,
+        request: dingtalkim__2__0_models.CreateCoupleGroupRequest,
+        headers: dingtalkim__2__0_models.CreateCoupleGroupHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalktrip__1__0_models.SyncSecretKeyResponse:
+    ) -> dingtalkim__2__0_models.CreateCoupleGroupResponse:
         UtilClient.validate_model(request)
         body = {}
-        if not UtilClient.is_unset(request.action_type):
-            body['actionType'] = request.action_type
-        if not UtilClient.is_unset(request.secret_string):
-            body['secretString'] = request.secret_string
-        if not UtilClient.is_unset(request.target_corp_id):
-            body['targetCorpId'] = request.target_corp_id
-        if not UtilClient.is_unset(request.trip_app_key):
-            body['tripAppKey'] = request.trip_app_key
-        if not UtilClient.is_unset(request.trip_app_security):
-            body['tripAppSecurity'] = request.trip_app_security
-        if not UtilClient.is_unset(request.trip_corp_id):
-            body['tripCorpId'] = request.trip_corp_id
+        if not UtilClient.is_unset(request.group_template_id):
+            body['groupTemplateId'] = request.group_template_id
+        if not UtilClient.is_unset(request.operator_id):
+            body['operatorId'] = request.operator_id
+        if not UtilClient.is_unset(request.users):
+            body['users'] = request.users
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
-            action='SyncSecretKey',
-            version='trip_1.0',
+            action='CreateCoupleGroup',
+            version='im_2.0',
             protocol='HTTP',
-            pathname=f'/v1.0/trip/secretKeys/sync',
+            pathname=f'/v2.0/im/interconnections/couples/groups',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalktrip__1__0_models.SyncSecretKeyResponse(),
+            dingtalkim__2__0_models.CreateCoupleGroupResponse(),
             await self.execute_async(params, req, runtime)
         )
 
-    def sync_secret_key(
+    def create_couple_group(
         self,
-        request: dingtalktrip__1__0_models.SyncSecretKeyRequest,
-    ) -> dingtalktrip__1__0_models.SyncSecretKeyResponse:
+        request: dingtalkim__2__0_models.CreateCoupleGroupRequest,
+    ) -> dingtalkim__2__0_models.CreateCoupleGroupResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalktrip__1__0_models.SyncSecretKeyHeaders()
-        return self.sync_secret_key_with_options(request, headers, runtime)
+        headers = dingtalkim__2__0_models.CreateCoupleGroupHeaders()
+        return self.create_couple_group_with_options(request, headers, runtime)
 
-    async def sync_secret_key_async(
+    async def create_couple_group_async(
         self,
-        request: dingtalktrip__1__0_models.SyncSecretKeyRequest,
-    ) -> dingtalktrip__1__0_models.SyncSecretKeyResponse:
+        request: dingtalkim__2__0_models.CreateCoupleGroupRequest,
+    ) -> dingtalkim__2__0_models.CreateCoupleGroupResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalktrip__1__0_models.SyncSecretKeyHeaders()
-        return await self.sync_secret_key_with_options_async(request, headers, runtime)
+        headers = dingtalkim__2__0_models.CreateCoupleGroupHeaders()
+        return await self.create_couple_group_with_options_async(request, headers, runtime)
 
-    def sync_trip_order_with_options(
+    def create_group_with_options(
         self,
-        request: dingtalktrip__1__0_models.SyncTripOrderRequest,
-        headers: dingtalktrip__1__0_models.SyncTripOrderHeaders,
+        request: dingtalkim__2__0_models.CreateGroupRequest,
+        headers: dingtalkim__2__0_models.CreateGroupHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalktrip__1__0_models.SyncTripOrderResponse:
+    ) -> dingtalkim__2__0_models.CreateGroupResponse:
         UtilClient.validate_model(request)
         body = {}
-        if not UtilClient.is_unset(request.channel_type):
-            body['channelType'] = request.channel_type
-        if not UtilClient.is_unset(request.currency):
-            body['currency'] = request.currency
-        if not UtilClient.is_unset(request.ding_user_id):
-            body['dingUserId'] = request.ding_user_id
-        if not UtilClient.is_unset(request.discount_amount):
-            body['discountAmount'] = request.discount_amount
-        if not UtilClient.is_unset(request.endorse_flag):
-            body['endorseFlag'] = request.endorse_flag
-        if not UtilClient.is_unset(request.event):
-            body['event'] = request.event
-        if not UtilClient.is_unset(request.gmt_order):
-            body['gmtOrder'] = request.gmt_order
-        if not UtilClient.is_unset(request.gmt_pay):
-            body['gmtPay'] = request.gmt_pay
-        if not UtilClient.is_unset(request.gmt_refund):
-            body['gmtRefund'] = request.gmt_refund
-        if not UtilClient.is_unset(request.invoice_apply_url):
-            body['invoiceApplyUrl'] = request.invoice_apply_url
-        if not UtilClient.is_unset(request.journey_biz_no):
-            body['journeyBizNo'] = request.journey_biz_no
-        if not UtilClient.is_unset(request.order_details):
-            body['orderDetails'] = request.order_details
-        if not UtilClient.is_unset(request.order_no):
-            body['orderNo'] = request.order_no
-        if not UtilClient.is_unset(request.order_url):
-            body['orderUrl'] = request.order_url
-        if not UtilClient.is_unset(request.real_amount):
-            body['realAmount'] = request.real_amount
-        if not UtilClient.is_unset(request.refund_amount):
-            body['refundAmount'] = request.refund_amount
-        if not UtilClient.is_unset(request.relative_order_no):
-            body['relativeOrderNo'] = request.relative_order_no
-        if not UtilClient.is_unset(request.source):
-            body['source'] = request.source
-        if not UtilClient.is_unset(request.target_corp_id):
-            body['targetCorpId'] = request.target_corp_id
-        if not UtilClient.is_unset(request.total_amount):
-            body['totalAmount'] = request.total_amount
-        if not UtilClient.is_unset(request.type):
-            body['type'] = request.type
+        if not UtilClient.is_unset(request.group_avatar):
+            body['groupAvatar'] = request.group_avatar
+        if not UtilClient.is_unset(request.group_name):
+            body['groupName'] = request.group_name
+        if not UtilClient.is_unset(request.group_template_id):
+            body['groupTemplateId'] = request.group_template_id
+        if not UtilClient.is_unset(request.operator_id):
+            body['operatorId'] = request.operator_id
+        if not UtilClient.is_unset(request.users):
+            body['users'] = request.users
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
-            action='SyncTripOrder',
-            version='trip_1.0',
+            action='CreateGroup',
+            version='im_2.0',
             protocol='HTTP',
-            pathname=f'/v1.0/trip/tripOrders/sync',
+            pathname=f'/v2.0/im/interconnections/groups',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalktrip__1__0_models.SyncTripOrderResponse(),
+            dingtalkim__2__0_models.CreateGroupResponse(),
             self.execute(params, req, runtime)
         )
 
-    async def sync_trip_order_with_options_async(
+    async def create_group_with_options_async(
         self,
-        request: dingtalktrip__1__0_models.SyncTripOrderRequest,
-        headers: dingtalktrip__1__0_models.SyncTripOrderHeaders,
+        request: dingtalkim__2__0_models.CreateGroupRequest,
+        headers: dingtalkim__2__0_models.CreateGroupHeaders,
         runtime: util_models.RuntimeOptions,
-    ) -> dingtalktrip__1__0_models.SyncTripOrderResponse:
+    ) -> dingtalkim__2__0_models.CreateGroupResponse:
         UtilClient.validate_model(request)
         body = {}
-        if not UtilClient.is_unset(request.channel_type):
-            body['channelType'] = request.channel_type
-        if not UtilClient.is_unset(request.currency):
-            body['currency'] = request.currency
-        if not UtilClient.is_unset(request.ding_user_id):
-            body['dingUserId'] = request.ding_user_id
-        if not UtilClient.is_unset(request.discount_amount):
-            body['discountAmount'] = request.discount_amount
-        if not UtilClient.is_unset(request.endorse_flag):
-            body['endorseFlag'] = request.endorse_flag
-        if not UtilClient.is_unset(request.event):
-            body['event'] = request.event
-        if not UtilClient.is_unset(request.gmt_order):
-            body['gmtOrder'] = request.gmt_order
-        if not UtilClient.is_unset(request.gmt_pay):
-            body['gmtPay'] = request.gmt_pay
-        if not UtilClient.is_unset(request.gmt_refund):
-            body['gmtRefund'] = request.gmt_refund
-        if not UtilClient.is_unset(request.invoice_apply_url):
-            body['invoiceApplyUrl'] = request.invoice_apply_url
-        if not UtilClient.is_unset(request.journey_biz_no):
-            body['journeyBizNo'] = request.journey_biz_no
-        if not UtilClient.is_unset(request.order_details):
-            body['orderDetails'] = request.order_details
-        if not UtilClient.is_unset(request.order_no):
-            body['orderNo'] = request.order_no
-        if not UtilClient.is_unset(request.order_url):
-            body['orderUrl'] = request.order_url
-        if not UtilClient.is_unset(request.real_amount):
-            body['realAmount'] = request.real_amount
-        if not UtilClient.is_unset(request.refund_amount):
-            body['refundAmount'] = request.refund_amount
-        if not UtilClient.is_unset(request.relative_order_no):
-            body['relativeOrderNo'] = request.relative_order_no
-        if not UtilClient.is_unset(request.source):
-            body['source'] = request.source
-        if not UtilClient.is_unset(request.target_corp_id):
-            body['targetCorpId'] = request.target_corp_id
-        if not UtilClient.is_unset(request.total_amount):
-            body['totalAmount'] = request.total_amount
-        if not UtilClient.is_unset(request.type):
-            body['type'] = request.type
+        if not UtilClient.is_unset(request.group_avatar):
+            body['groupAvatar'] = request.group_avatar
+        if not UtilClient.is_unset(request.group_name):
+            body['groupName'] = request.group_name
+        if not UtilClient.is_unset(request.group_template_id):
+            body['groupTemplateId'] = request.group_template_id
+        if not UtilClient.is_unset(request.operator_id):
+            body['operatorId'] = request.operator_id
+        if not UtilClient.is_unset(request.users):
+            body['users'] = request.users
         real_headers = {}
         if not UtilClient.is_unset(headers.common_headers):
             real_headers = headers.common_headers
         if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
             real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
         req = open_api_models.OpenApiRequest(
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
-            action='SyncTripOrder',
-            version='trip_1.0',
+            action='CreateGroup',
+            version='im_2.0',
             protocol='HTTP',
-            pathname=f'/v1.0/trip/tripOrders/sync',
+            pathname=f'/v2.0/im/interconnections/groups',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
-            dingtalktrip__1__0_models.SyncTripOrderResponse(),
+            dingtalkim__2__0_models.CreateGroupResponse(),
             await self.execute_async(params, req, runtime)
         )
 
-    def sync_trip_order(
+    def create_group(
         self,
-        request: dingtalktrip__1__0_models.SyncTripOrderRequest,
-    ) -> dingtalktrip__1__0_models.SyncTripOrderResponse:
+        request: dingtalkim__2__0_models.CreateGroupRequest,
+    ) -> dingtalkim__2__0_models.CreateGroupResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalktrip__1__0_models.SyncTripOrderHeaders()
-        return self.sync_trip_order_with_options(request, headers, runtime)
+        headers = dingtalkim__2__0_models.CreateGroupHeaders()
+        return self.create_group_with_options(request, headers, runtime)
 
-    async def sync_trip_order_async(
+    async def create_group_async(
         self,
-        request: dingtalktrip__1__0_models.SyncTripOrderRequest,
-    ) -> dingtalktrip__1__0_models.SyncTripOrderResponse:
+        request: dingtalkim__2__0_models.CreateGroupRequest,
+    ) -> dingtalkim__2__0_models.CreateGroupResponse:
         runtime = util_models.RuntimeOptions()
-        headers = dingtalktrip__1__0_models.SyncTripOrderHeaders()
-        return await self.sync_trip_order_with_options_async(request, headers, runtime)
+        headers = dingtalkim__2__0_models.CreateGroupHeaders()
+        return await self.create_group_with_options_async(request, headers, runtime)
+
+    def create_topbox_with_options(
+        self,
+        request: dingtalkim__2__0_models.CreateTopboxRequest,
+        headers: dingtalkim__2__0_models.CreateTopboxHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkim__2__0_models.CreateTopboxResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.callback_route_key):
+            body['callbackRouteKey'] = request.callback_route_key
+        if not UtilClient.is_unset(request.card_data):
+            body['cardData'] = request.card_data
+        if not UtilClient.is_unset(request.card_settings):
+            body['cardSettings'] = request.card_settings
+        if not UtilClient.is_unset(request.card_template_id):
+            body['cardTemplateId'] = request.card_template_id
+        if not UtilClient.is_unset(request.conversation_type):
+            body['conversationType'] = request.conversation_type
+        if not UtilClient.is_unset(request.cool_app_code):
+            body['coolAppCode'] = request.cool_app_code
+        if not UtilClient.is_unset(request.expired_time):
+            body['expiredTime'] = request.expired_time
+        if not UtilClient.is_unset(request.group_template_id):
+            body['groupTemplateId'] = request.group_template_id
+        if not UtilClient.is_unset(request.open_conversation_id):
+            body['openConversationId'] = request.open_conversation_id
+        if not UtilClient.is_unset(request.out_track_id):
+            body['outTrackId'] = request.out_track_id
+        if not UtilClient.is_unset(request.platforms):
+            body['platforms'] = request.platforms
+        if not UtilClient.is_unset(request.receiver_union_id_list):
+            body['receiverUnionIdList'] = request.receiver_union_id_list
+        if not UtilClient.is_unset(request.receiver_user_id_list):
+            body['receiverUserIdList'] = request.receiver_user_id_list
+        if not UtilClient.is_unset(request.robot_code):
+            body['robotCode'] = request.robot_code
+        if not UtilClient.is_unset(request.union_id_private_data_map):
+            body['unionIdPrivateDataMap'] = request.union_id_private_data_map
+        if not UtilClient.is_unset(request.unoin_id):
+            body['unoinId'] = request.unoin_id
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
+        if not UtilClient.is_unset(request.user_id_private_data_map):
+            body['userIdPrivateDataMap'] = request.user_id_private_data_map
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateTopbox',
+            version='im_2.0',
+            protocol='HTTP',
+            pathname=f'/v2.0/im/topBoxes',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkim__2__0_models.CreateTopboxResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def create_topbox_with_options_async(
+        self,
+        request: dingtalkim__2__0_models.CreateTopboxRequest,
+        headers: dingtalkim__2__0_models.CreateTopboxHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkim__2__0_models.CreateTopboxResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.callback_route_key):
+            body['callbackRouteKey'] = request.callback_route_key
+        if not UtilClient.is_unset(request.card_data):
+            body['cardData'] = request.card_data
+        if not UtilClient.is_unset(request.card_settings):
+            body['cardSettings'] = request.card_settings
+        if not UtilClient.is_unset(request.card_template_id):
+            body['cardTemplateId'] = request.card_template_id
+        if not UtilClient.is_unset(request.conversation_type):
+            body['conversationType'] = request.conversation_type
+        if not UtilClient.is_unset(request.cool_app_code):
+            body['coolAppCode'] = request.cool_app_code
+        if not UtilClient.is_unset(request.expired_time):
+            body['expiredTime'] = request.expired_time
+        if not UtilClient.is_unset(request.group_template_id):
+            body['groupTemplateId'] = request.group_template_id
+        if not UtilClient.is_unset(request.open_conversation_id):
+            body['openConversationId'] = request.open_conversation_id
+        if not UtilClient.is_unset(request.out_track_id):
+            body['outTrackId'] = request.out_track_id
+        if not UtilClient.is_unset(request.platforms):
+            body['platforms'] = request.platforms
+        if not UtilClient.is_unset(request.receiver_union_id_list):
+            body['receiverUnionIdList'] = request.receiver_union_id_list
+        if not UtilClient.is_unset(request.receiver_user_id_list):
+            body['receiverUserIdList'] = request.receiver_user_id_list
+        if not UtilClient.is_unset(request.robot_code):
+            body['robotCode'] = request.robot_code
+        if not UtilClient.is_unset(request.union_id_private_data_map):
+            body['unionIdPrivateDataMap'] = request.union_id_private_data_map
+        if not UtilClient.is_unset(request.unoin_id):
+            body['unoinId'] = request.unoin_id
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
+        if not UtilClient.is_unset(request.user_id_private_data_map):
+            body['userIdPrivateDataMap'] = request.user_id_private_data_map
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateTopbox',
+            version='im_2.0',
+            protocol='HTTP',
+            pathname=f'/v2.0/im/topBoxes',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkim__2__0_models.CreateTopboxResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def create_topbox(
+        self,
+        request: dingtalkim__2__0_models.CreateTopboxRequest,
+    ) -> dingtalkim__2__0_models.CreateTopboxResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkim__2__0_models.CreateTopboxHeaders()
+        return self.create_topbox_with_options(request, headers, runtime)
+
+    async def create_topbox_async(
+        self,
+        request: dingtalkim__2__0_models.CreateTopboxRequest,
+    ) -> dingtalkim__2__0_models.CreateTopboxResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkim__2__0_models.CreateTopboxHeaders()
+        return await self.create_topbox_with_options_async(request, headers, runtime)
```

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
 from typing import Dict
 
 
-class CountWorkRecordHeaders(TeaModel):
+class SaveOpenExternalLogHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
         self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
@@ -33,74 +33,92 @@
         if m.get('commonHeaders') is not None:
             self.common_headers = m.get('commonHeaders')
         if m.get('x-acs-dingtalk-access-token') is not None:
             self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
         return self
 
 
-class CountWorkRecordRequest(TeaModel):
+class SaveOpenExternalLogRequest(TeaModel):
     def __init__(
         self,
-        user_id: str = None,
+        corp_id: str = None,
+        log_source: str = None,
+        log_type: str = None,
+        open_ext: str = None,
     ):
-        self.user_id = user_id
+        self.corp_id = corp_id
+        self.log_source = log_source
+        self.log_type = log_type
+        self.open_ext = open_ext
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.user_id is not None:
-            result['userId'] = self.user_id
+        if self.corp_id is not None:
+            result['corpId'] = self.corp_id
+        if self.log_source is not None:
+            result['logSource'] = self.log_source
+        if self.log_type is not None:
+            result['logType'] = self.log_type
+        if self.open_ext is not None:
+            result['openExt'] = self.open_ext
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('userId') is not None:
-            self.user_id = m.get('userId')
+        if m.get('corpId') is not None:
+            self.corp_id = m.get('corpId')
+        if m.get('logSource') is not None:
+            self.log_source = m.get('logSource')
+        if m.get('logType') is not None:
+            self.log_type = m.get('logType')
+        if m.get('openExt') is not None:
+            self.open_ext = m.get('openExt')
         return self
 
 
-class CountWorkRecordResponseBody(TeaModel):
+class SaveOpenExternalLogResponseBody(TeaModel):
     def __init__(
         self,
-        undo_count: int = None,
+        success: bool = None,
     ):
-        self.undo_count = undo_count
+        self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.undo_count is not None:
-            result['undoCount'] = self.undo_count
+        if self.success is not None:
+            result['success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('undoCount') is not None:
-            self.undo_count = m.get('undoCount')
+        if m.get('success') is not None:
+            self.success = m.get('success')
         return self
 
 
-class CountWorkRecordResponse(TeaModel):
+class SaveOpenExternalLogResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: CountWorkRecordResponseBody = None,
+        body: SaveOpenExternalLogResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         self.validate_required(self.headers, 'headers')
@@ -126,12 +144,12 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = CountWorkRecordResponseBody()
+            temp_model = SaveOpenExternalLogResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk/yun_shu_1_0/client.py` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.18/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-dingtalk
-Version: 2.0.17
+Name: alibabacloud_dingtalk
+Version: 2.0.18
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.17/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.18/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.17/setup.py` & `alibabacloud_dingtalk-2.0.18/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 26/05/2023
+Created on 31/05/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

