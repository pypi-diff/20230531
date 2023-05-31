# Comparing `tmp/satosacontrib.perun-3.3.0.tar.gz` & `tmp/satosacontrib.perun-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satosacontrib.perun-3.3.0.tar", last modified: Fri May 26 07:25:09 2023, max compression
+gzip compressed data, was "satosacontrib.perun-3.4.0.tar", last modified: Wed May 31 07:43:54 2023, max compression
```

## Comparing `satosacontrib.perun-3.3.0.tar` & `satosacontrib.perun-3.4.0.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:25:09.532575 satosacontrib.perun-3.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     1560 2023-05-09 13:18:33.000000 satosacontrib.perun-3.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      246 2023-05-26 07:25:09.532575 satosacontrib.perun-3.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1772 2023-05-26 06:37:05.000000 satosacontrib.perun-3.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:25:09.528576 satosacontrib.perun-3.3.0/satosacontrib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:18:33.000000 satosacontrib.perun-3.3.0/satosacontrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:25:09.528576 satosacontrib.perun-3.3.0/satosacontrib/perun/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:18:33.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:25:09.528576 satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/
--rw-rw-rw-   0 root         (0) root         (0)      727 2023-05-26 06:37:05.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1677 2023-05-09 13:18:33.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/attribute_typing_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     5327 2023-05-09 13:18:33.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/auth_event_logging_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-09 13:18:33.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/cardinality_single_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     3500 2023-05-26 06:37:05.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/compute_eligibility.py
--rw-rw-rw-   0 root         (0) root         (0)     2156 2023-05-24 15:24:28.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/context_attributes_microservice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:25:09.528576 satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/idm/
--rw-rw-rw-   0 root         (0) root         (0)      387 2023-05-10 10:57:23.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/idm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5927 2023-05-10 10:57:23.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/idm/attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    11822 2023-05-10 10:57:23.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/idm/ensure_member.py
--rw-rw-rw-   0 root         (0) root         (0)    11583 2023-05-10 10:57:23.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/idm/entitlement.py
--rw-rw-rw-   0 root         (0) root         (0)     4831 2023-05-10 10:57:23.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/idm/perun_user.py
--rw-rw-rw-   0 root         (0) root         (0)    24791 2023-05-10 10:57:23.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/idm/sp_authorization.py
--rw-rw-rw-   0 root         (0) root         (0)    11491 2023-05-10 10:57:23.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/idm/update_user_ext_source.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2023-05-24 15:24:28.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/is_banned_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     3840 2023-05-09 13:18:33.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/is_eligible_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     2200 2023-05-09 13:18:33.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/multi_idphint_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     1200 2023-05-09 13:18:33.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/nameid_attribute_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     3496 2023-05-09 13:18:33.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/proxystatistics_microservice.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:25:09.528576 satosacontrib.perun-3.3.0/satosacontrib/perun/utils/
--rw-rw-rw-   0 root         (0) root         (0)     2042 2023-05-09 13:18:33.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/utils/AuthEventLoggingDbModels.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2023-05-09 13:18:33.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/utils/ConfigStore.py
--rw-rw-rw-   0 root         (0) root         (0)     4435 2023-05-09 13:18:33.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/utils/CurlConnector.py
--rw-rw-rw-   0 root         (0) root         (0)     1391 2023-05-09 13:18:33.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/utils/CurlConnectorInterface.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-05-09 13:18:33.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/utils/PerunConstants.py
--rw-rw-rw-   0 root         (0) root         (0)     6364 2023-05-10 10:57:23.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/utils/Utils.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:18:33.000000 satosacontrib.perun-3.3.0/satosacontrib/perun/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:25:09.528576 satosacontrib.perun-3.3.0/satosacontrib.perun.egg-info/
--rw-r--r--   0 root         (0) root         (0)      246 2023-05-26 07:25:09.000000 satosacontrib.perun-3.3.0/satosacontrib.perun.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2098 2023-05-26 07:25:09.000000 satosacontrib.perun-3.3.0/satosacontrib.perun.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 07:25:09.000000 satosacontrib.perun-3.3.0/satosacontrib.perun.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      192 2023-05-26 07:25:09.000000 satosacontrib.perun-3.3.0/satosacontrib.perun.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-26 07:25:09.000000 satosacontrib.perun-3.3.0/satosacontrib.perun.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-26 07:25:09.532575 satosacontrib.perun-3.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      624 2023-05-26 06:37:05.000000 satosacontrib.perun-3.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:25:09.532575 satosacontrib.perun-3.3.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:18:33.000000 satosacontrib.perun-3.3.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3496 2023-05-10 13:23:50.000000 satosacontrib.perun-3.3.0/tests/test_auth_event_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     3455 2023-05-24 15:24:28.000000 satosacontrib.perun-3.3.0/tests/test_context_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)     1796 2023-05-24 15:24:28.000000 satosacontrib.perun-3.3.0/tests/test_is_banned.py
--rw-rw-rw-   0 root         (0) root         (0)     7500 2023-05-09 13:18:33.000000 satosacontrib.perun-3.3.0/tests/test_is_eligible_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     2531 2023-05-10 10:57:23.000000 satosacontrib.perun-3.3.0/tests/test_microservice_loader.py
--rw-rw-rw-   0 root         (0) root         (0)     3981 2023-05-10 10:57:23.000000 satosacontrib.perun-3.3.0/tests/test_perun_attributes.py
--rw-rw-rw-   0 root         (0) root         (0)    14517 2023-05-10 10:57:23.000000 satosacontrib.perun-3.3.0/tests/test_perun_ensure_member.py
--rw-rw-rw-   0 root         (0) root         (0)     7117 2023-05-10 10:57:23.000000 satosacontrib.perun-3.3.0/tests/test_perun_entitlement.py
--rw-rw-rw-   0 root         (0) root         (0)     5672 2023-05-10 10:57:23.000000 satosacontrib.perun-3.3.0/tests/test_perun_user_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)    36568 2023-05-10 10:57:23.000000 satosacontrib.perun-3.3.0/tests/test_sp_authorization_microservice.py
--rw-rw-rw-   0 root         (0) root         (0)     7291 2023-05-10 10:57:23.000000 satosacontrib.perun-3.3.0/tests/test_update_ues.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:43:54.971694 satosacontrib.perun-3.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      246 2023-05-31 07:43:54.971694 satosacontrib.perun-3.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2864 2023-05-30 20:33:51.000000 satosacontrib.perun-3.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:43:54.755689 satosacontrib.perun-3.4.0/satosacontrib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:43:54.755689 satosacontrib.perun-3.4.0/satosacontrib/perun/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:43:54.831690 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/
+-rw-rw-rw-   0 root         (0) root         (0)      727 2023-05-26 19:41:47.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/attribute_typing_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     5327 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/auth_event_logging_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/cardinality_single_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3500 2023-05-26 19:41:47.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/compute_eligibility.py
+-rw-rw-rw-   0 root         (0) root         (0)     2156 2023-05-26 19:41:47.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/context_attributes_microservice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:43:54.875692 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/
+-rw-rw-rw-   0 root         (0) root         (0)      474 2023-05-26 19:37:57.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8313 2023-05-30 20:33:51.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/additional_identifiers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5927 2023-05-10 10:57:23.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    11822 2023-05-10 10:57:23.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/ensure_member.py
+-rw-rw-rw-   0 root         (0) root         (0)    11583 2023-05-10 10:57:23.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/entitlement.py
+-rw-rw-rw-   0 root         (0) root         (0)     4831 2023-05-26 19:37:57.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/perun_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    24791 2023-05-10 10:57:23.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/sp_authorization.py
+-rw-rw-rw-   0 root         (0) root         (0)    11491 2023-05-10 10:57:23.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/update_user_ext_source.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2023-05-26 19:41:47.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/is_banned_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3840 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/is_eligible_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     2200 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/multi_idphint_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     1200 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/nameid_attribute_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3496 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/proxystatistics_microservice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:43:54.875692 satosacontrib.perun-3.4.0/satosacontrib/perun/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     2042 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/utils/AuthEventLoggingDbModels.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/utils/ConfigStore.py
+-rw-rw-rw-   0 root         (0) root         (0)     4435 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/utils/CurlConnector.py
+-rw-rw-rw-   0 root         (0) root         (0)     1391 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/utils/CurlConnectorInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/utils/PerunConstants.py
+-rw-rw-rw-   0 root         (0) root         (0)     6719 2023-05-26 19:37:57.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/utils/Utils.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/satosacontrib/perun/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:43:54.755689 satosacontrib.perun-3.4.0/satosacontrib.perun.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      246 2023-05-31 07:43:54.000000 satosacontrib.perun-3.4.0/satosacontrib.perun.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-05-31 07:43:54.000000 satosacontrib.perun-3.4.0/satosacontrib.perun.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 07:43:54.000000 satosacontrib.perun-3.4.0/satosacontrib.perun.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      192 2023-05-31 07:43:54.000000 satosacontrib.perun-3.4.0/satosacontrib.perun.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-31 07:43:54.000000 satosacontrib.perun-3.4.0/satosacontrib.perun.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-31 07:43:54.971694 satosacontrib.perun-3.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      624 2023-05-26 19:41:47.000000 satosacontrib.perun-3.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 07:43:54.963694 satosacontrib.perun-3.4.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10917 2023-05-26 19:37:57.000000 satosacontrib.perun-3.4.0/tests/test_additional_indentifiers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3496 2023-05-10 13:23:50.000000 satosacontrib.perun-3.4.0/tests/test_auth_event_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     3455 2023-05-26 19:41:47.000000 satosacontrib.perun-3.4.0/tests/test_context_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1796 2023-05-26 19:41:47.000000 satosacontrib.perun-3.4.0/tests/test_is_banned.py
+-rw-rw-rw-   0 root         (0) root         (0)     7500 2023-05-09 13:18:33.000000 satosacontrib.perun-3.4.0/tests/test_is_eligible_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     2535 2023-05-26 19:37:57.000000 satosacontrib.perun-3.4.0/tests/test_microservice_loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     3981 2023-05-10 10:57:23.000000 satosacontrib.perun-3.4.0/tests/test_perun_attributes.py
+-rw-rw-rw-   0 root         (0) root         (0)    14517 2023-05-10 10:57:23.000000 satosacontrib.perun-3.4.0/tests/test_perun_ensure_member.py
+-rw-rw-rw-   0 root         (0) root         (0)     7117 2023-05-10 10:57:23.000000 satosacontrib.perun-3.4.0/tests/test_perun_entitlement.py
+-rw-rw-rw-   0 root         (0) root         (0)     5482 2023-05-26 19:37:57.000000 satosacontrib.perun-3.4.0/tests/test_perun_user_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)    36568 2023-05-10 10:57:23.000000 satosacontrib.perun-3.4.0/tests/test_sp_authorization_microservice.py
+-rw-rw-rw-   0 root         (0) root         (0)     7291 2023-05-10 10:57:23.000000 satosacontrib.perun-3.4.0/tests/test_update_ues.py
```

### Comparing `satosacontrib.perun-3.3.0/LICENSE` & `satosacontrib.perun-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/__init__.py` & `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/__init__.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/attribute_typing_microservice.py` & `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/attribute_typing_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/auth_event_logging_microservice.py` & `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/auth_event_logging_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/cardinality_single_microservice.py` & `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/cardinality_single_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/compute_eligibility.py` & `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/compute_eligibility.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/context_attributes_microservice.py` & `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/context_attributes_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/idm/attributes.py` & `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/attributes.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/idm/ensure_member.py` & `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/ensure_member.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/idm/entitlement.py` & `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/entitlement.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/idm/perun_user.py` & `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/perun_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
         self.__perun_user_id_attr = global_config["perun_user_id_attribute"]
         self.__perun_login_attribute = global_config["perun_login_attribute"]
         self.__allowed_requesters = global_config.get("allowed_requesters", {})
         self.__internal_login_attribute = config["internal_login_attribute"]
         self.__internal_extsource_attribute = config["internal_extsource_attribute"]
         self.__proxy_extsource_name = config["proxy_extsource_name"]
-        self.__registration_page_url = config.get("registration_page_url", [])
+        self.__registration_page_url = config.get("registration_page_url", "")
         self.__registration_result_url = config["registration_result_url"]
 
         adapters_manager_cfg = global_config["adapters_manager"]
         attrs_map = ConfigStore.get_attributes_map(global_config["attrs_cfg_path"])
 
         self.__adapters_manager = AdaptersManager(adapters_manager_cfg, attrs_map)
         self.__endpoint = "/process"
```

### Comparing `satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/idm/sp_authorization.py` & `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/sp_authorization.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/idm/update_user_ext_source.py` & `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/idm/update_user_ext_source.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/is_banned_microservice.py` & `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/is_banned_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/is_eligible_microservice.py` & `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/is_eligible_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/multi_idphint_microservice.py` & `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/multi_idphint_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/nameid_attribute_microservice.py` & `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/nameid_attribute_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/satosacontrib/perun/micro_services/proxystatistics_microservice.py` & `satosacontrib.perun-3.4.0/satosacontrib/perun/micro_services/proxystatistics_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/satosacontrib/perun/utils/AuthEventLoggingDbModels.py` & `satosacontrib.perun-3.4.0/satosacontrib/perun/utils/AuthEventLoggingDbModels.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/satosacontrib/perun/utils/ConfigStore.py` & `satosacontrib.perun-3.4.0/satosacontrib/perun/utils/ConfigStore.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/satosacontrib/perun/utils/CurlConnector.py` & `satosacontrib.perun-3.4.0/satosacontrib/perun/utils/CurlConnector.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/satosacontrib/perun/utils/CurlConnectorInterface.py` & `satosacontrib.perun-3.4.0/satosacontrib/perun/utils/CurlConnectorInterface.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/satosacontrib/perun/utils/Utils.py` & `satosacontrib.perun-3.4.0/satosacontrib/perun/utils/Utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import hashlib
 import hmac
 import json
 import logging
 import random
 import string
 import time
 
@@ -169,7 +170,16 @@
             return data.requester not in deny_rules
         logger.debug(
             "Requester '{}' is not allowed for '{}' due to final deny all rule".format(
                 data.requester, target_entity_id
             )
         )
         return False
+
+    @staticmethod
+    def get_hash_function(function_name):
+        hashlib_algs = hashlib.algorithms_available
+        if function_name in hashlib_algs:
+            hash_func = getattr(hashlib, function_name)
+            return hash_func
+        else:
+            raise ValueError(f"Invalid hashing algorithm, supported: {hashlib_algs}")
```

### Comparing `satosacontrib.perun-3.3.0/satosacontrib.perun.egg-info/SOURCES.txt` & `satosacontrib.perun-3.4.0/satosacontrib.perun.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,28 +17,30 @@
 satosacontrib/perun/micro_services/context_attributes_microservice.py
 satosacontrib/perun/micro_services/is_banned_microservice.py
 satosacontrib/perun/micro_services/is_eligible_microservice.py
 satosacontrib/perun/micro_services/multi_idphint_microservice.py
 satosacontrib/perun/micro_services/nameid_attribute_microservice.py
 satosacontrib/perun/micro_services/proxystatistics_microservice.py
 satosacontrib/perun/micro_services/idm/__init__.py
+satosacontrib/perun/micro_services/idm/additional_identifiers.py
 satosacontrib/perun/micro_services/idm/attributes.py
 satosacontrib/perun/micro_services/idm/ensure_member.py
 satosacontrib/perun/micro_services/idm/entitlement.py
 satosacontrib/perun/micro_services/idm/perun_user.py
 satosacontrib/perun/micro_services/idm/sp_authorization.py
 satosacontrib/perun/micro_services/idm/update_user_ext_source.py
 satosacontrib/perun/utils/AuthEventLoggingDbModels.py
 satosacontrib/perun/utils/ConfigStore.py
 satosacontrib/perun/utils/CurlConnector.py
 satosacontrib/perun/utils/CurlConnectorInterface.py
 satosacontrib/perun/utils/PerunConstants.py
 satosacontrib/perun/utils/Utils.py
 satosacontrib/perun/utils/__init__.py
 tests/__init__.py
+tests/test_additional_indentifiers.py
 tests/test_auth_event_logging.py
 tests/test_context_attributes.py
 tests/test_is_banned.py
 tests/test_is_eligible_microservice.py
 tests/test_microservice_loader.py
 tests/test_perun_attributes.py
 tests/test_perun_ensure_member.py
```

### Comparing `satosacontrib.perun-3.3.0/setup.py` & `satosacontrib.perun-3.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     description="Module with satosa micro_services",
     packages=find_packages(),
     install_requires=[
         "setuptools",
         "SATOSA~=8.1",
         "pysaml2~=7.1",
         "requests~=2.28",
-        "perun.connector~=3.3",
+        "perun.connector~=3.7",
         "PyYAML~=6.0",
         "SQLAlchemy~=1.4",
         "jwcrypto~=1.3",
         "natsort~=8.3.1",
         "python-dateutil~=2.8",
         "geoip2~=4.6",
         "user_agents~=2.2",
```

### Comparing `satosacontrib.perun-3.3.0/tests/test_auth_event_logging.py` & `satosacontrib.perun-3.4.0/tests/test_auth_event_logging.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/tests/test_context_attributes.py` & `satosacontrib.perun-3.4.0/tests/test_context_attributes.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/tests/test_is_banned.py` & `satosacontrib.perun-3.4.0/tests/test_is_banned.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/tests/test_is_eligible_microservice.py` & `satosacontrib.perun-3.4.0/tests/test_is_eligible_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/tests/test_microservice_loader.py` & `satosacontrib.perun-3.4.0/tests/test_microservice_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest.mock import patch, MagicMock
 
 from perun.connector.adapters.AdaptersManager import AdaptersManager
 from satosa.context import Context
 from satosa.internal import InternalData
-import satosacontrib.perun.micro_services
+import satosacontrib.perun.micro_services.idm
 
 from satosacontrib.perun.utils.ConfigStore import ConfigStore
 
 
 class TestContext(Context):
     __test__ = False
```

### Comparing `satosacontrib.perun-3.3.0/tests/test_perun_attributes.py` & `satosacontrib.perun-3.4.0/tests/test_perun_attributes.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/tests/test_perun_ensure_member.py` & `satosacontrib.perun-3.4.0/tests/test_perun_ensure_member.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/tests/test_perun_entitlement.py` & `satosacontrib.perun-3.4.0/tests/test_perun_entitlement.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/tests/test_perun_user_microservice.py` & `satosacontrib.perun-3.4.0/tests/test_perun_user_microservice.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,20 +57,17 @@
     data_with_non_existent_user.attributes["example_internal_login"] = []
 
     AdaptersManager.get_perun_user = MagicMock(
         side_effect=AdaptersManagerNotExistsException(
             '"name":"UserExtSourceNotExistsException"'
         )
     )
-    expected_error_message = '"name":"UserExtSourceNotExistsException"'
     PerunUser.handle_user_not_found = MagicMock(return_value=None)
-    with pytest.raises(Exception) as error:
-        MICROSERVICE.process(TestContext(), data_with_non_existent_user)
-        assert str(error.value.args[0]) == expected_error_message
-        PerunUser.handle_user_not_found.assert_called()
+    MICROSERVICE.process(TestContext(), data_with_non_existent_user)
+    PerunUser.handle_user_not_found.assert_called()
 
 
 @patch("perun.connector.adapters.AdaptersManager.AdaptersManager.get_perun_user")
 @patch(
     "perun.connector.adapters.AdaptersManager.AdaptersManager.get_user_attributes"  # noqa
 )
 @patch("satosa.micro_services.base.MicroService.process")
```

### Comparing `satosacontrib.perun-3.3.0/tests/test_sp_authorization_microservice.py` & `satosacontrib.perun-3.4.0/tests/test_sp_authorization_microservice.py`

 * *Files identical despite different names*

### Comparing `satosacontrib.perun-3.3.0/tests/test_update_ues.py` & `satosacontrib.perun-3.4.0/tests/test_update_ues.py`

 * *Files identical despite different names*

