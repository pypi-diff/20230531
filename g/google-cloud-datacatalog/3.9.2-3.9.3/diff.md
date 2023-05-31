# Comparing `tmp/google-cloud-datacatalog-3.9.2.tar.gz` & `tmp/google-cloud-datacatalog-3.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-datacatalog-3.9.2.tar", last modified: Mon Oct  3 23:50:07 2022, max compression
+gzip compressed data, was "google-cloud-datacatalog-3.9.3.tar", last modified: Mon Oct 10 16:57:05 2022, max compression
```

## Comparing `google-cloud-datacatalog-3.9.2.tar` & `google-cloud-datacatalog-3.9.3.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.277808 google-cloud-datacatalog-3.9.2/
--rw-rw-r--   0 root         (0)     1003    11358 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4682 2022-10-03 23:50:07.277808 google-cloud-datacatalog-3.9.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3777 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.253805 google-cloud-datacatalog-3.9.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.253805 google-cloud-datacatalog-3.9.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.257806 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog/
--rw-rw-r--   0 root         (0)     1003     7310 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog/__init__.py
--rw-rw-r--   0 root         (0)     1003       85 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.257806 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/
--rw-rw-r--   0 root         (0)     1003     6485 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    13251 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       85 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.257806 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.257806 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/data_catalog/
--rw-rw-r--   0 root         (0)     1003      757 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/data_catalog/__init__.py
--rw-rw-r--   0 root         (0)     1003   174730 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/data_catalog/async_client.py
--rw-rw-r--   0 root         (0)     1003   189722 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/data_catalog/client.py
--rw-rw-r--   0 root         (0)     1003    20630 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/data_catalog/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.257806 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/data_catalog/transports/
--rw-rw-r--   0 root         (0)     1003     1166 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/data_catalog/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    22564 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/data_catalog/transports/base.py
--rw-rw-r--   0 root         (0)     1003    55750 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/data_catalog/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    56907 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/data_catalog/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.261806 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager/
--rw-rw-r--   0 root         (0)     1003      777 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager/__init__.py
--rw-rw-r--   0 root         (0)     1003    70306 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager/async_client.py
--rw-rw-r--   0 root         (0)     1003    81493 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager/client.py
--rw-rw-r--   0 root         (0)     1003    10983 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.261806 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager/transports/
--rw-rw-r--   0 root         (0)     1003     1211 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11750 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager/transports/base.py
--rw-rw-r--   0 root         (0)     1003    26332 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    26886 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.261806 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/
--rw-rw-r--   0 root         (0)     1003      829 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/__init__.py
--rw-rw-r--   0 root         (0)     1003    22031 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/async_client.py
--rw-rw-r--   0 root         (0)     1003    31189 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.261806 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/transports/
--rw-rw-r--   0 root         (0)     1003     1336 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7367 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15699 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15976 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.265807 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/
--rw-rw-r--   0 root         (0)     1003     5854 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3330 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/bigquery.py
--rw-rw-r--   0 root         (0)     1003     1683 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/common.py
--rw-rw-r--   0 root         (0)     1003     3930 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/data_source.py
--rw-rw-r--   0 root         (0)     1003    56954 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/datacatalog.py
--rw-rw-r--   0 root         (0)     1003     4732 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/dataplex_spec.py
--rw-rw-r--   0 root         (0)     1003     3842 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/gcs_fileset_spec.py
--rw-rw-r--   0 root         (0)     1003     4269 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/physical_schema.py
--rw-rw-r--   0 root         (0)     1003    14166 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/policytagmanager.py
--rw-rw-r--   0 root         (0)     1003     8345 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/policytagmanagerserialization.py
--rw-rw-r--   0 root         (0)     1003     2883 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/schema.py
--rw-rw-r--   0 root         (0)     1003     5283 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/search.py
--rw-rw-r--   0 root         (0)     1003     4799 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/table_spec.py
--rw-rw-r--   0 root         (0)     1003    14254 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/tags.py
--rw-rw-r--   0 root         (0)     1003     2139 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/timestamps.py
--rw-rw-r--   0 root         (0)     1003     3127 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/usage.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.265807 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/
--rw-rw-r--   0 root         (0)     1003     4912 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    11681 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       85 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.265807 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.265807 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/data_catalog/
--rw-rw-r--   0 root         (0)     1003      757 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/data_catalog/__init__.py
--rw-rw-r--   0 root         (0)     1003   155963 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/data_catalog/async_client.py
--rw-rw-r--   0 root         (0)     1003   167967 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/data_catalog/client.py
--rw-rw-r--   0 root         (0)     1003    20795 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/data_catalog/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.265807 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/data_catalog/transports/
--rw-rw-r--   0 root         (0)     1003     1166 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/data_catalog/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    21535 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/data_catalog/transports/base.py
--rw-rw-r--   0 root         (0)     1003    47954 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/data_catalog/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    48936 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/data_catalog/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.269807 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/
--rw-rw-r--   0 root         (0)     1003      777 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/__init__.py
--rw-rw-r--   0 root         (0)     1003    69744 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/async_client.py
--rw-rw-r--   0 root         (0)     1003    80931 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/client.py
--rw-rw-r--   0 root         (0)     1003    11068 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.269807 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/transports/
--rw-rw-r--   0 root         (0)     1003     1211 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11755 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/transports/base.py
--rw-rw-r--   0 root         (0)     1003    25795 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    26349 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.269807 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/
--rw-rw-r--   0 root         (0)     1003      829 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/__init__.py
--rw-rw-r--   0 root         (0)     1003    17398 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/async_client.py
--rw-rw-r--   0 root         (0)     1003    26324 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.269807 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/transports/
--rw-rw-r--   0 root         (0)     1003     1336 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6883 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13616 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13871 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.273807 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     4274 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     1022 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/types/common.py
--rw-rw-r--   0 root         (0)     1003    39496 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/types/datacatalog.py
--rw-rw-r--   0 root         (0)     1003     3868 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/types/gcs_fileset_spec.py
--rw-rw-r--   0 root         (0)     1003    13770 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/types/policytagmanager.py
--rw-rw-r--   0 root         (0)     1003     6239 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/types/policytagmanagerserialization.py
--rw-rw-r--   0 root         (0)     1003     2525 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/types/schema.py
--rw-rw-r--   0 root         (0)     1003     2853 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/types/search.py
--rw-rw-r--   0 root         (0)     1003     4507 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/types/table_spec.py
--rw-rw-r--   0 root         (0)     1003    12510 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/types/tags.py
--rw-rw-r--   0 root         (0)     1003     1886 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/types/timestamps.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.273807 google-cloud-datacatalog-3.9.2/google_cloud_datacatalog.egg-info/
--rw-r--r--   0 root         (0)     1003     4682 2022-10-03 23:50:07.000000 google-cloud-datacatalog-3.9.2/google_cloud_datacatalog.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     6430 2022-10-03 23:50:07.000000 google-cloud-datacatalog-3.9.2/google_cloud_datacatalog.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-03 23:50:07.000000 google-cloud-datacatalog-3.9.2/google_cloud_datacatalog.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-10-03 23:50:07.000000 google-cloud-datacatalog-3.9.2/google_cloud_datacatalog.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-10-03 23:50:07.000000 google-cloud-datacatalog-3.9.2/google_cloud_datacatalog.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      221 2022-10-03 23:50:07.000000 google-cloud-datacatalog-3.9.2/google_cloud_datacatalog.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-10-03 23:50:07.000000 google-cloud-datacatalog-3.9.2/google_cloud_datacatalog.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.273807 google-cloud-datacatalog-3.9.2/scripts/
--rw-rw-r--   0 root         (0)     1003     8619 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/scripts/fixup_datacatalog_v1_keywords.py
--rw-rw-r--   0 root         (0)     1003     8226 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/scripts/fixup_datacatalog_v1beta1_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2022-10-03 23:50:07.277808 google-cloud-datacatalog-3.9.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2850 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.273807 google-cloud-datacatalog-3.9.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.273807 google-cloud-datacatalog-3.9.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.273807 google-cloud-datacatalog-3.9.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.277808 google-cloud-datacatalog-3.9.2/tests/unit/gapic/datacatalog_v1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/tests/unit/gapic/datacatalog_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   349973 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/tests/unit/gapic/datacatalog_v1/test_data_catalog.py
--rw-rw-r--   0 root         (0)     1003   174233 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/tests/unit/gapic/datacatalog_v1/test_policy_tag_manager.py
--rw-rw-r--   0 root         (0)     1003    71686 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/tests/unit/gapic/datacatalog_v1/test_policy_tag_manager_serialization.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-10-03 23:50:07.277808 google-cloud-datacatalog-3.9.2/tests/unit/gapic/datacatalog_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/tests/unit/gapic/datacatalog_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003   308765 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/tests/unit/gapic/datacatalog_v1beta1/test_data_catalog.py
--rw-rw-r--   0 root         (0)     1003   173701 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/tests/unit/gapic/datacatalog_v1beta1/test_policy_tag_manager.py
--rw-rw-r--   0 root         (0)     1003    65009 2022-10-03 23:46:30.000000 google-cloud-datacatalog-3.9.2/tests/unit/gapic/datacatalog_v1beta1/test_policy_tag_manager_serialization.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.340708 google-cloud-datacatalog-3.9.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4682 2022-10-10 16:57:05.340708 google-cloud-datacatalog-3.9.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3777 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.304708 google-cloud-datacatalog-3.9.3/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.304708 google-cloud-datacatalog-3.9.3/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.308708 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog/
+-rw-rw-r--   0 root         (0)     1003     7310 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog/__init__.py
+-rw-rw-r--   0 root         (0)     1003       85 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.308708 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/
+-rw-rw-r--   0 root         (0)     1003     6485 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13251 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       85 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.308708 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.312708 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/data_catalog/
+-rw-rw-r--   0 root         (0)     1003      757 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/data_catalog/__init__.py
+-rw-rw-r--   0 root         (0)     1003   174730 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/data_catalog/async_client.py
+-rw-rw-r--   0 root         (0)     1003   189722 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/data_catalog/client.py
+-rw-rw-r--   0 root         (0)     1003    20630 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/data_catalog/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.312708 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/data_catalog/transports/
+-rw-rw-r--   0 root         (0)     1003     1166 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/data_catalog/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22564 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/data_catalog/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    55750 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/data_catalog/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    56907 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/data_catalog/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.316708 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager/
+-rw-rw-r--   0 root         (0)     1003      777 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager/__init__.py
+-rw-rw-r--   0 root         (0)     1003    70306 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager/async_client.py
+-rw-rw-r--   0 root         (0)     1003    81493 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager/client.py
+-rw-rw-r--   0 root         (0)     1003    10983 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.316708 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager/transports/
+-rw-rw-r--   0 root         (0)     1003     1211 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11750 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    26332 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    26886 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.316708 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/
+-rw-rw-r--   0 root         (0)     1003      829 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22031 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/async_client.py
+-rw-rw-r--   0 root         (0)     1003    31189 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.316708 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/transports/
+-rw-rw-r--   0 root         (0)     1003     1336 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7367 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15699 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15976 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.320708 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/
+-rw-rw-r--   0 root         (0)     1003     5854 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3330 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/bigquery.py
+-rw-rw-r--   0 root         (0)     1003     1683 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003     3930 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/data_source.py
+-rw-rw-r--   0 root         (0)     1003    56954 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/datacatalog.py
+-rw-rw-r--   0 root         (0)     1003     4732 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/dataplex_spec.py
+-rw-rw-r--   0 root         (0)     1003     3842 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/gcs_fileset_spec.py
+-rw-rw-r--   0 root         (0)     1003     4269 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/physical_schema.py
+-rw-rw-r--   0 root         (0)     1003    14166 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/policytagmanager.py
+-rw-rw-r--   0 root         (0)     1003     8345 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/policytagmanagerserialization.py
+-rw-rw-r--   0 root         (0)     1003     2883 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/schema.py
+-rw-rw-r--   0 root         (0)     1003     5283 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/search.py
+-rw-rw-r--   0 root         (0)     1003     4799 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/table_spec.py
+-rw-rw-r--   0 root         (0)     1003    14254 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/tags.py
+-rw-rw-r--   0 root         (0)     1003     2139 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/timestamps.py
+-rw-rw-r--   0 root         (0)     1003     3127 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/usage.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.320708 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     4912 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11681 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       85 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.320708 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.324708 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/data_catalog/
+-rw-rw-r--   0 root         (0)     1003      757 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/data_catalog/__init__.py
+-rw-rw-r--   0 root         (0)     1003   155963 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/data_catalog/async_client.py
+-rw-rw-r--   0 root         (0)     1003   167967 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/data_catalog/client.py
+-rw-rw-r--   0 root         (0)     1003    20795 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/data_catalog/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.324708 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/data_catalog/transports/
+-rw-rw-r--   0 root         (0)     1003     1166 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/data_catalog/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21535 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/data_catalog/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    47954 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/data_catalog/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    48936 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/data_catalog/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.328708 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/
+-rw-rw-r--   0 root         (0)     1003      777 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/__init__.py
+-rw-rw-r--   0 root         (0)     1003    69744 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/async_client.py
+-rw-rw-r--   0 root         (0)     1003    80931 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/client.py
+-rw-rw-r--   0 root         (0)     1003    11068 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.328708 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/transports/
+-rw-rw-r--   0 root         (0)     1003     1211 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11755 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    25795 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    26349 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.328708 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/
+-rw-rw-r--   0 root         (0)     1003      829 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17398 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/async_client.py
+-rw-rw-r--   0 root         (0)     1003    26324 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.328708 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/transports/
+-rw-rw-r--   0 root         (0)     1003     1336 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6883 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13616 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13871 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.332708 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     4274 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1022 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/types/common.py
+-rw-rw-r--   0 root         (0)     1003    39496 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/types/datacatalog.py
+-rw-rw-r--   0 root         (0)     1003     3868 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/types/gcs_fileset_spec.py
+-rw-rw-r--   0 root         (0)     1003    13770 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/types/policytagmanager.py
+-rw-rw-r--   0 root         (0)     1003     6239 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/types/policytagmanagerserialization.py
+-rw-rw-r--   0 root         (0)     1003     2525 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/types/schema.py
+-rw-rw-r--   0 root         (0)     1003     2853 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/types/search.py
+-rw-rw-r--   0 root         (0)     1003     4507 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/types/table_spec.py
+-rw-rw-r--   0 root         (0)     1003    12510 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/types/tags.py
+-rw-rw-r--   0 root         (0)     1003     1886 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/types/timestamps.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.332708 google-cloud-datacatalog-3.9.3/google_cloud_datacatalog.egg-info/
+-rw-r--r--   0 root         (0)     1003     4682 2022-10-10 16:57:05.000000 google-cloud-datacatalog-3.9.3/google_cloud_datacatalog.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     6430 2022-10-10 16:57:05.000000 google-cloud-datacatalog-3.9.3/google_cloud_datacatalog.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:57:05.000000 google-cloud-datacatalog-3.9.3/google_cloud_datacatalog.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-10-10 16:57:05.000000 google-cloud-datacatalog-3.9.3/google_cloud_datacatalog.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-10-10 16:57:05.000000 google-cloud-datacatalog-3.9.3/google_cloud_datacatalog.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      293 2022-10-10 16:57:05.000000 google-cloud-datacatalog-3.9.3/google_cloud_datacatalog.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-10-10 16:57:05.000000 google-cloud-datacatalog-3.9.3/google_cloud_datacatalog.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.332708 google-cloud-datacatalog-3.9.3/scripts/
+-rw-rw-r--   0 root         (0)     1003     8619 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/scripts/fixup_datacatalog_v1_keywords.py
+-rw-rw-r--   0 root         (0)     1003     8226 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/scripts/fixup_datacatalog_v1beta1_keywords.py
+-rw-rw-r--   0 root         (0)     1003       67 2022-10-10 16:57:05.340708 google-cloud-datacatalog-3.9.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2919 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.332708 google-cloud-datacatalog-3.9.3/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.332708 google-cloud-datacatalog-3.9.3/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.332708 google-cloud-datacatalog-3.9.3/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.336708 google-cloud-datacatalog-3.9.3/tests/unit/gapic/datacatalog_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/tests/unit/gapic/datacatalog_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   349973 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/tests/unit/gapic/datacatalog_v1/test_data_catalog.py
+-rw-rw-r--   0 root         (0)     1003   174233 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/tests/unit/gapic/datacatalog_v1/test_policy_tag_manager.py
+-rw-rw-r--   0 root         (0)     1003    71686 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/tests/unit/gapic/datacatalog_v1/test_policy_tag_manager_serialization.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-10-10 16:57:05.340708 google-cloud-datacatalog-3.9.3/tests/unit/gapic/datacatalog_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/tests/unit/gapic/datacatalog_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   308765 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/tests/unit/gapic/datacatalog_v1beta1/test_data_catalog.py
+-rw-rw-r--   0 root         (0)     1003   173701 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/tests/unit/gapic/datacatalog_v1beta1/test_policy_tag_manager.py
+-rw-rw-r--   0 root         (0)     1003    65009 2022-10-10 16:53:01.000000 google-cloud-datacatalog-3.9.3/tests/unit/gapic/datacatalog_v1beta1/test_policy_tag_manager_serialization.py
```

### Comparing `google-cloud-datacatalog-3.9.2/LICENSE` & `google-cloud-datacatalog-3.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/MANIFEST.in` & `google-cloud-datacatalog-3.9.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/PKG-INFO` & `google-cloud-datacatalog-3.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-datacatalog
-Version: 3.9.2
+Version: 3.9.3
 Summary: Google Cloud Data Catalog API API client library
 Home-page: https://github.com/googleapis/python-datacatalog
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-datacatalog-3.9.2/README.rst` & `google-cloud-datacatalog-3.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog/__init__.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/__init__.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/gapic_metadata.json` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/__init__.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/data_catalog/__init__.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/data_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/data_catalog/async_client.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/data_catalog/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/data_catalog/client.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/data_catalog/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/data_catalog/pagers.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/data_catalog/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/data_catalog/transports/__init__.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/data_catalog/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/data_catalog/transports/base.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/data_catalog/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/data_catalog/transports/grpc.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/data_catalog/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/data_catalog/transports/grpc_asyncio.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/data_catalog/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager/__init__.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager/async_client.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager/client.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager/pagers.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager/transports/__init__.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager/transports/base.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager/transports/grpc.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager/transports/grpc_asyncio.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/__init__.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/async_client.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/client.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/transports/__init__.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/transports/base.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/transports/grpc.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/transports/grpc_asyncio.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/services/policy_tag_manager_serialization/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/__init__.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/bigquery.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/bigquery.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/common.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/data_source.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/data_source.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/datacatalog.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/datacatalog.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/dataplex_spec.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/dataplex_spec.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/gcs_fileset_spec.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/gcs_fileset_spec.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/physical_schema.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/physical_schema.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/policytagmanager.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/policytagmanager.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/policytagmanagerserialization.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/policytagmanagerserialization.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/schema.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/schema.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/search.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/search.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/table_spec.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/table_spec.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/tags.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/tags.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/timestamps.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/timestamps.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1/types/usage.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1/types/usage.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/__init__.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/gapic_metadata.json` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/__init__.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/data_catalog/__init__.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/data_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/data_catalog/async_client.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/data_catalog/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/data_catalog/client.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/data_catalog/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/data_catalog/pagers.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/data_catalog/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/data_catalog/transports/__init__.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/data_catalog/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/data_catalog/transports/base.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/data_catalog/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/data_catalog/transports/grpc.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/data_catalog/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/data_catalog/transports/grpc_asyncio.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/data_catalog/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/__init__.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/async_client.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/client.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/pagers.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/transports/__init__.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/transports/base.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/transports/grpc.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/transports/grpc_asyncio.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/__init__.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/async_client.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/client.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/transports/__init__.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/transports/base.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/transports/grpc.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/transports/grpc_asyncio.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/services/policy_tag_manager_serialization/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/types/__init__.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/types/common.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/types/datacatalog.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/types/datacatalog.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/types/gcs_fileset_spec.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/types/gcs_fileset_spec.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/types/policytagmanager.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/types/policytagmanager.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/types/policytagmanagerserialization.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/types/policytagmanagerserialization.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/types/schema.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/types/schema.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/types/search.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/types/search.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/types/table_spec.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/types/table_spec.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/types/tags.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/types/tags.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google/cloud/datacatalog_v1beta1/types/timestamps.py` & `google-cloud-datacatalog-3.9.3/google/cloud/datacatalog_v1beta1/types/timestamps.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/google_cloud_datacatalog.egg-info/PKG-INFO` & `google-cloud-datacatalog-3.9.3/google_cloud_datacatalog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-datacatalog
-Version: 3.9.2
+Version: 3.9.3
 Summary: Google Cloud Data Catalog API API client library
 Home-page: https://github.com/googleapis/python-datacatalog
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-datacatalog-3.9.2/google_cloud_datacatalog.egg-info/SOURCES.txt` & `google-cloud-datacatalog-3.9.3/google_cloud_datacatalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/scripts/fixup_datacatalog_v1_keywords.py` & `google-cloud-datacatalog-3.9.3/scripts/fixup_datacatalog_v1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/scripts/fixup_datacatalog_v1beta1_keywords.py` & `google-cloud-datacatalog-3.9.3/scripts/fixup_datacatalog_v1beta1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/setup.py` & `google-cloud-datacatalog-3.9.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 import io
 import os
 
 import setuptools
 
 name = "google-cloud-datacatalog"
 description = "Google Cloud Data Catalog API API client library"
-version = "3.9.2"
+version = "3.9.3"
 # Should be one of:
 # 'Development Status :: 3 - Alpha'
 # 'Development Status :: 4 - Beta'
 # 'Development Status :: 5 - Production/Stable'
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
     "google-api-core[grpc] >= 1.32.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*",
     "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
     "proto-plus >= 1.22.0, <2.0.0dev",
-    "protobuf >= 3.20.2, <5.0.0dev",
+    "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
 
 extras = {"libcst": "libcst >= 0.2.5"}
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
```

### Comparing `google-cloud-datacatalog-3.9.2/tests/__init__.py` & `google-cloud-datacatalog-3.9.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/tests/unit/__init__.py` & `google-cloud-datacatalog-3.9.3/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/tests/unit/gapic/__init__.py` & `google-cloud-datacatalog-3.9.3/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/tests/unit/gapic/datacatalog_v1/__init__.py` & `google-cloud-datacatalog-3.9.3/tests/unit/gapic/datacatalog_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/tests/unit/gapic/datacatalog_v1/test_data_catalog.py` & `google-cloud-datacatalog-3.9.3/tests/unit/gapic/datacatalog_v1/test_data_catalog.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/tests/unit/gapic/datacatalog_v1/test_policy_tag_manager.py` & `google-cloud-datacatalog-3.9.3/tests/unit/gapic/datacatalog_v1/test_policy_tag_manager.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/tests/unit/gapic/datacatalog_v1/test_policy_tag_manager_serialization.py` & `google-cloud-datacatalog-3.9.3/tests/unit/gapic/datacatalog_v1/test_policy_tag_manager_serialization.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/tests/unit/gapic/datacatalog_v1beta1/__init__.py` & `google-cloud-datacatalog-3.9.3/tests/unit/gapic/datacatalog_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/tests/unit/gapic/datacatalog_v1beta1/test_data_catalog.py` & `google-cloud-datacatalog-3.9.3/tests/unit/gapic/datacatalog_v1beta1/test_data_catalog.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/tests/unit/gapic/datacatalog_v1beta1/test_policy_tag_manager.py` & `google-cloud-datacatalog-3.9.3/tests/unit/gapic/datacatalog_v1beta1/test_policy_tag_manager.py`

 * *Files identical despite different names*

### Comparing `google-cloud-datacatalog-3.9.2/tests/unit/gapic/datacatalog_v1beta1/test_policy_tag_manager_serialization.py` & `google-cloud-datacatalog-3.9.3/tests/unit/gapic/datacatalog_v1beta1/test_policy_tag_manager_serialization.py`

 * *Files identical despite different names*

