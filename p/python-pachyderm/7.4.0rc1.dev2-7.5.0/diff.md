# Comparing `tmp/python-pachyderm-7.4.0rc1.dev2.tar.gz` & `tmp/python_pachyderm-7.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-pachyderm-7.4.0rc1.dev2.tar", max compression
+gzip compressed data, was "python_pachyderm-7.5.0.tar", max compression
```

## Comparing `python-pachyderm-7.4.0rc1.dev2.tar` & `python_pachyderm-7.5.0.tar`

### file list

```diff
@@ -1,94 +1,67 @@
--rw-r--r--   0        0        0    10765 2021-11-30 20:22:47.200826 python-pachyderm-7.4.0rc1.dev2/LICENSE
--rw-r--r--   0        0        0     2860 2022-04-11 15:06:43.550359 python-pachyderm-7.4.0rc1.dev2/README.md
--rw-r--r--   0        0        0     1526 2023-02-08 21:31:22.640131 python-pachyderm-7.4.0rc1.dev2/pyproject.toml
--rw-r--r--   0        0        0     3078 2023-02-08 21:31:22.643643 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/__init__.py
--rw-r--r--   0        0        0    18276 2023-01-18 19:38:34.691517 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/client.py
--rw-r--r--   0        0        0      572 2022-04-11 15:06:43.624332 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/errors.py
--rw-r--r--   0        0        0      733 2022-04-11 15:06:43.624433 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/__init__.py
--rw-r--r--   0        0        0     6405 2022-09-23 22:05:41.779841 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/client.py
--rw-r--r--   0        0        0      374 2022-08-11 17:38:47.689371 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/mixin/__init__.py
--rw-r--r--   0        0        0     1039 2023-01-18 19:38:34.691948 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/mixin/admin.py
--rw-r--r--   0        0        0    12974 2022-08-11 17:38:47.689741 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/mixin/auth.py
--rw-r--r--   0        0        0     2873 2022-09-23 22:05:41.779946 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/mixin/debug.py
--rw-r--r--   0        0        0     2373 2022-09-23 22:05:49.012253 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/mixin/enterprise.py
--rw-r--r--   0        0        0      627 2022-08-11 17:38:47.690042 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/mixin/health.py
--rw-r--r--   0        0        0     5916 2022-08-11 17:38:47.690136 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/mixin/identity.py
--rw-r--r--   0        0        0     5826 2023-01-18 19:38:34.692276 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/mixin/license.py
--rw-r--r--   0        0        0    60314 2023-02-08 19:57:46.241015 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/mixin/pfs.py
--rw-r--r--   0        0        0    35309 2023-02-08 19:57:46.241359 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/mixin/pps.py
--rw-r--r--   0        0        0     6517 2022-08-11 17:38:47.690876 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/mixin/transaction.py
--rw-r--r--   0        0        0      687 2022-08-11 17:38:47.690957 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/mixin/version.py
--rw-r--r--   0        0        0     3934 2023-01-18 19:38:34.694763 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/pfs.py
--rw-r--r--   0        0        0      660 2022-04-11 15:06:43.626710 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/proto/__init__.py
--rw-r--r--   0        0        0        0 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/proto/v2/__init__.py
--rw-r--r--   0        0        0     2091 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/proto/v2/admin_v2/__init__.py
--rw-r--r--   0        0        0    44848 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/proto/v2/auth_v2/__init__.py
--rw-r--r--   0        0        0     5803 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/proto/v2/debug_v2/__init__.py
--rw-r--r--   0        0        0    12094 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/proto/v2/enterprise_v2/__init__.py
--rw-r--r--   0        0        0    19648 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/proto/v2/identity_v2/__init__.py
--rw-r--r--   0        0        0    16118 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/proto/v2/license_v2/__init__.py
--rw-r--r--   0        0        0    84365 2023-02-08 19:57:46.241787 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/proto/v2/pfs_v2/__init__.py
--rw-r--r--   0        0        0    84811 2023-02-08 19:57:46.242247 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/proto/v2/pps_v2/__init__.py
--rw-r--r--   0        0        0     1746 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/proto/v2/proxy/__init__.py
--rw-r--r--   0        0        0     1013 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/proto/v2/taskapi/__init__.py
--rw-r--r--   0        0        0    10824 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/proto/v2/transaction_v2/__init__.py
--rw-r--r--   0        0        0     1881 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/proto/v2/versionpb_v2/__init__.py
--rw-r--r--   0        0        0     1277 2022-04-11 15:06:43.629054 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/service.py
--rw-r--r--   0        0        0     5327 2022-08-11 17:38:47.692466 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/util.py
--rw-r--r--   0        0        0     1920 2022-08-11 17:38:47.692702 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/interceptor.py
--rw-r--r--   0        0        0      303 2021-11-30 20:22:47.291056 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/mixin/__init__.py
--rw-r--r--   0        0        0      992 2023-01-18 19:38:34.698155 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/mixin/admin.py
--rw-r--r--   0        0        0    13495 2022-04-11 15:06:43.630063 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/mixin/auth.py
--rw-r--r--   0        0        0     2969 2022-04-11 15:06:43.630235 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/mixin/debug.py
--rw-r--r--   0        0        0     2749 2022-09-23 22:05:49.013729 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/mixin/enterprise.py
--rw-r--r--   0        0        0      682 2022-09-23 22:05:45.598314 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/mixin/health.py
--rw-r--r--   0        0        0     6510 2022-04-11 15:06:43.630843 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/mixin/identity.py
--rw-r--r--   0        0        0     6144 2023-01-18 19:38:34.698330 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/mixin/license.py
--rw-r--r--   0        0        0    58015 2023-02-08 21:14:53.612407 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/mixin/pfs.py
--rw-r--r--   0        0        0    34830 2023-02-08 19:57:46.248788 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/mixin/pps.py
--rw-r--r--   0        0        0     6837 2022-04-11 15:06:43.632185 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/mixin/transaction.py
--rw-r--r--   0        0        0      675 2022-04-11 15:06:43.632353 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/mixin/version.py
--rw-r--r--   0        0        0     3451 2023-01-18 19:38:34.699543 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/pfs.py
--rw-r--r--   0        0        0        0 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/__init__.py
--rw-r--r--   0        0        0        0 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/admin/__init__.py
--rw-r--r--   0        0        0     6334 2023-02-01 20:22:30.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/admin/admin_pb2.py
--rw-r--r--   0        0        0     2776 2023-02-01 20:22:30.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/admin/admin_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/auth/__init__.py
--rw-r--r--   0        0        0   127743 2023-02-01 20:22:30.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/auth/auth_pb2.py
--rw-r--r--   0        0        0    46966 2023-02-01 20:22:30.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/auth/auth_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/debug/__init__.py
--rw-r--r--   0        0        0    15377 2023-02-01 20:22:30.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/debug/debug_pb2.py
--rw-r--r--   0        0        0     6044 2023-02-01 20:22:30.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/debug/debug_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/enterprise/__init__.py
--rw-r--r--   0        0        0    35208 2023-02-01 20:22:30.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/enterprise/enterprise_pb2.py
--rw-r--r--   0        0        0    15946 2023-02-01 20:22:30.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/enterprise/enterprise_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/identity/__init__.py
--rw-r--r--   0        0        0    52022 2023-02-01 20:22:30.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/identity/identity_pb2.py
--rw-r--r--   0        0        0    25893 2023-02-01 20:22:30.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/identity/identity_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/license/__init__.py
--rw-r--r--   0        0        0    44786 2023-02-01 20:22:30.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/license/license_pb2.py
--rw-r--r--   0        0        0    17666 2023-02-01 20:22:30.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/license/license_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/pfs/__init__.py
--rw-r--r--   0        0        0   208740 2023-02-08 19:57:46.249527 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/pfs/pfs_pb2.py
--rw-r--r--   0        0        0    84220 2023-02-01 20:22:30.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/pfs/pfs_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/pps/__init__.py
--rw-r--r--   0        0        0   264354 2023-02-08 19:57:46.250128 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/pps/pps_pb2.py
--rw-r--r--   0        0        0    54338 2023-02-08 19:57:46.250364 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/pps/pps_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/proxy/__init__.py
--rw-r--r--   0        0        0     4268 2023-02-01 20:22:30.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/proxy/proxy_pb2.py
--rw-r--r--   0        0        0     2776 2023-02-01 20:22:30.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/proxy/proxy_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/task/__init__.py
--rw-r--r--   0        0        0     9216 2023-02-01 20:22:30.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/task/task_pb2.py
--rw-r--r--   0        0        0      159 2023-02-01 20:22:30.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/task/task_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/transaction/__init__.py
--rw-r--r--   0        0        0    29890 2023-02-01 20:22:30.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/transaction/transaction_pb2.py
--rw-r--r--   0        0        0    14168 2023-02-01 20:22:30.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/transaction/transaction_pb2_grpc.py
--rw-r--r--   0        0        0        0 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/version/__init__.py
--rw-r--r--   0        0        0        0 2023-02-01 20:22:35.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/version/versionpb/__init__.py
--rw-r--r--   0        0        0     6904 2023-02-01 20:22:30.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/version/versionpb/version_pb2.py
--rw-r--r--   0        0        0     2787 2023-02-01 20:22:30.000000 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/version/versionpb/version_pb2_grpc.py
--rw-r--r--   0        0        0     3496 2022-04-11 15:06:43.633870 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/service.py
--rw-r--r--   0        0        0     4617 2022-04-26 22:35:41.031384 python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/util.py
--rw-r--r--   0        0        0       91 2023-02-08 19:57:46.250531 python-pachyderm-7.4.0rc1.dev2/version.json
--rw-r--r--   0        0        0     5256 2023-02-08 21:31:25.831130 python-pachyderm-7.4.0rc1.dev2/setup.py
--rw-r--r--   0        0        0     4107 2023-02-08 21:31:25.831425 python-pachyderm-7.4.0rc1.dev2/PKG-INFO
+-rw-r--r--   0        0        0    10765 2023-05-19 19:35:24.851765 python_pachyderm-7.5.0/LICENSE
+-rw-r--r--   0        0        0     2860 2023-05-19 19:35:24.851922 python_pachyderm-7.5.0/README.md
+-rw-r--r--   0        0        0     1519 2023-05-31 19:22:57.352678 python_pachyderm-7.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3155 2023-05-31 17:49:06.174530 python_pachyderm-7.5.0/src/python_pachyderm/__init__.py
+-rw-r--r--   0        0        0    19354 2023-05-31 17:49:06.175013 python_pachyderm-7.5.0/src/python_pachyderm/client.py
+-rw-r--r--   0        0        0     1360 2023-05-31 17:49:06.175185 python_pachyderm-7.5.0/src/python_pachyderm/datum_batching.py
+-rw-r--r--   0        0        0      572 2023-05-19 19:35:24.964519 python_pachyderm-7.5.0/src/python_pachyderm/errors.py
+-rw-r--r--   0        0        0     1920 2023-05-19 19:35:24.968392 python_pachyderm-7.5.0/src/python_pachyderm/interceptor.py
+-rw-r--r--   0        0        0      303 2023-05-19 19:35:24.968492 python_pachyderm-7.5.0/src/python_pachyderm/mixin/__init__.py
+-rw-r--r--   0        0        0      992 2023-05-19 19:35:24.968568 python_pachyderm-7.5.0/src/python_pachyderm/mixin/admin.py
+-rw-r--r--   0        0        0    13495 2023-05-19 19:35:24.968632 python_pachyderm-7.5.0/src/python_pachyderm/mixin/auth.py
+-rw-r--r--   0        0        0     4232 2023-05-26 19:37:18.654183 python_pachyderm-7.5.0/src/python_pachyderm/mixin/debug.py
+-rw-r--r--   0        0        0     2749 2023-05-19 19:35:24.968752 python_pachyderm-7.5.0/src/python_pachyderm/mixin/enterprise.py
+-rw-r--r--   0        0        0      682 2023-05-19 19:35:24.968809 python_pachyderm-7.5.0/src/python_pachyderm/mixin/health.py
+-rw-r--r--   0        0        0     6510 2023-05-19 19:35:24.968869 python_pachyderm-7.5.0/src/python_pachyderm/mixin/identity.py
+-rw-r--r--   0        0        0     6144 2023-05-19 19:35:24.968939 python_pachyderm-7.5.0/src/python_pachyderm/mixin/license.py
+-rw-r--r--   0        0        0    59238 2023-05-26 19:37:18.654560 python_pachyderm-7.5.0/src/python_pachyderm/mixin/pfs.py
+-rw-r--r--   0        0        0    35866 2023-05-26 19:37:18.654877 python_pachyderm-7.5.0/src/python_pachyderm/mixin/pps.py
+-rw-r--r--   0        0        0     6837 2023-05-19 19:35:24.969345 python_pachyderm-7.5.0/src/python_pachyderm/mixin/transaction.py
+-rw-r--r--   0        0        0      675 2023-05-19 19:35:24.969408 python_pachyderm-7.5.0/src/python_pachyderm/mixin/version.py
+-rw-r--r--   0        0        0     2829 2023-05-31 17:49:06.175379 python_pachyderm-7.5.0/src/python_pachyderm/mixin/worker.py
+-rw-r--r--   0        0        0     3451 2023-05-19 19:35:24.969494 python_pachyderm-7.5.0/src/python_pachyderm/pfs.py
+-rw-r--r--   0        0        0        0 2023-05-19 20:02:24.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 20:02:24.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/admin/__init__.py
+-rw-r--r--   0        0        0     6334 2023-05-19 20:02:18.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/admin/admin_pb2.py
+-rw-r--r--   0        0        0     2776 2023-05-19 20:02:18.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/admin/admin_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-05-19 20:02:24.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/auth/__init__.py
+-rw-r--r--   0        0        0   128016 2023-05-26 19:23:33.841944 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/auth/auth_pb2.py
+-rw-r--r--   0        0        0    46966 2023-05-19 20:02:18.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/auth/auth_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-05-19 20:02:24.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/debug/__init__.py
+-rw-r--r--   0        0        0    22909 2023-05-26 19:23:33.842454 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/debug/debug_pb2.py
+-rw-r--r--   0        0        0     7848 2023-05-26 19:23:33.842680 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/debug/debug_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-05-19 20:02:24.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/enterprise/__init__.py
+-rw-r--r--   0        0        0    35208 2023-05-19 20:02:18.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/enterprise/enterprise_pb2.py
+-rw-r--r--   0        0        0    15946 2023-05-19 20:02:18.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/enterprise/enterprise_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-05-19 20:02:24.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/identity/__init__.py
+-rw-r--r--   0        0        0    52022 2023-05-19 20:02:18.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/identity/identity_pb2.py
+-rw-r--r--   0        0        0    25893 2023-05-19 20:02:18.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/identity/identity_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-05-19 20:02:24.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/license/__init__.py
+-rw-r--r--   0        0        0    44786 2023-05-19 20:02:18.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/license/license_pb2.py
+-rw-r--r--   0        0        0    17666 2023-05-19 20:02:18.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/license/license_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-05-19 20:02:24.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/pfs/__init__.py
+-rw-r--r--   0        0        0   216577 2023-05-26 19:23:33.843168 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/pfs/pfs_pb2.py
+-rw-r--r--   0        0        0    86039 2023-05-26 19:23:33.843407 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/pfs/pfs_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-05-19 20:02:24.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/pps/__init__.py
+-rw-r--r--   0        0        0   270601 2023-05-26 19:23:33.843745 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/pps/pps_pb2.py
+-rw-r--r--   0        0        0    57841 2023-05-26 19:23:33.844081 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/pps/pps_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-05-19 20:02:24.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/proxy/__init__.py
+-rw-r--r--   0        0        0     4268 2023-05-19 20:02:18.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/proxy/proxy_pb2.py
+-rw-r--r--   0        0        0     2776 2023-05-19 20:02:18.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/proxy/proxy_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-05-19 20:02:24.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/task/__init__.py
+-rw-r--r--   0        0        0     9216 2023-05-19 20:02:18.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/task/task_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-19 20:02:18.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/task/task_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-05-19 20:02:24.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/transaction/__init__.py
+-rw-r--r--   0        0        0    29890 2023-05-19 20:02:18.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/transaction/transaction_pb2.py
+-rw-r--r--   0        0        0    14168 2023-05-19 20:02:18.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/transaction/transaction_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-05-19 20:02:24.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/version/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 20:02:24.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/version/versionpb/__init__.py
+-rw-r--r--   0        0        0     6904 2023-05-19 20:02:18.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/version/versionpb/version_pb2.py
+-rw-r--r--   0        0        0     2787 2023-05-19 20:02:18.000000 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/version/versionpb/version_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2023-05-26 19:23:33.844151 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/worker/__init__.py
+-rw-r--r--   0        0        0     8850 2023-05-26 19:23:33.844256 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/worker/worker_pb2.py
+-rw-r--r--   0        0        0     7003 2023-05-26 19:23:33.844345 python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/worker/worker_pb2_grpc.py
+-rw-r--r--   0        0        0     3722 2023-05-19 19:35:24.974196 python_pachyderm-7.5.0/src/python_pachyderm/service.py
+-rw-r--r--   0        0        0     4617 2023-05-19 19:35:24.974257 python_pachyderm-7.5.0/src/python_pachyderm/util.py
+-rw-r--r--   0        0        0       83 2023-05-26 22:39:46.974357 python_pachyderm-7.5.0/version.json
+-rw-r--r--   0        0        0     4351 1970-01-01 00:00:00.000000 python_pachyderm-7.5.0/PKG-INFO
```

### Comparing `python-pachyderm-7.4.0rc1.dev2/LICENSE` & `python_pachyderm-7.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-pachyderm-7.4.0rc1.dev2/README.md` & `python_pachyderm-7.5.0/README.md`

 * *Files identical despite different names*

### Comparing `python-pachyderm-7.4.0rc1.dev2/pyproject.toml` & `python_pachyderm-7.5.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [tool.poetry]
 name = "python-pachyderm"
-version = "7.4.0-rc.1.dev2"
+version = "7.5.0"
 description = "Python Pachyderm Client"
 authors = ["Pachyderm Integrations <integrations@pachyderm.io>"]
 include = ["version.json"]
 license = "Apache 2.0"
 documentation = "https://python-pachyderm.readthedocs.io/en/stable/"
 readme = 'README.md'
 repository = "https://github.com/pachyderm/python-pachyderm"
 keywords = ["pachyderm"]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
-grpcio = ">=1.38.0"
+python = ">=3.8,<4.0"
+grpcio = ">=1.54.2"
 grpcio-health-checking = ">=1.38.0"
 grpc-interceptor = "^0.13.0"
 importlib-metadata = { version = ">1.5.1", python = "<3.8" }
 protobuf = ">=3.17.1,<4.0.0"
-betterproto = "2.0.0b4"
+python-dotenv = ">=1.0.0"
 
 [tool.poetry.dev-dependencies]
 black = ">=22.6.0"
 certifi = ">=2019.11.28"
 flake8 = ">=3.9.1"
 myst-parser = "0.15.2"
 numpydoc = ">=1.1.0"
```

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/__init__.py` & `python_pachyderm-7.5.0/src/python_pachyderm/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import enum as _enum
 from google.protobuf.internal.enum_type_wrapper import (
     EnumTypeWrapper as _EnumTypeWrapper,
 )
 
 from .mixin.pfs import PFSFile, ModifyFileClient
 from .client import Client, ConfigError, BadClusterDeploymentID
+from .datum_batching import batch_all_datums
 from .util import (
     put_files,
     parse_json_pipeline_spec,
     parse_dict_pipeline_spec,
 )
 from grpc import RpcError
 
@@ -31,20 +32,21 @@
     "put_files",
     "PFSFile",
     "ModifyFileClient",
     "parse_json_pipeline_spec",
     "parse_dict_pipeline_spec",
     "ConfigError",
     "BadClusterDeploymentID",
+    "batch_all_datums",
 ]
 
 __version__ = ""
 try:
     __version__ = metadata.version(__name__)  # type: ignore
-except Exception:
+except FileNotFoundError:
     pass
 
 
 def _import_protos(path):
     """
     Imports items selectively from the auto-generated proto package.
```

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/client.py` & `python_pachyderm-7.5.0/src/python_pachyderm/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from .mixin.health import HealthMixin
 from .mixin.identity import IdentityMixin
 from .mixin.license import LicenseMixin
 from .mixin.pfs import PFSMixin
 from .mixin.pps import PPSMixin
 from .mixin.transaction import TransactionMixin
 from .mixin.version import VersionMixin
+from .mixin.worker import WorkerMixin as _WorkerStub
 from .service import Service, GRPC_CHANNEL_OPTIONS
 
 
 class ConfigError(Exception):
     """Error for issues related to the pachyderm config file."""
 
     def __init__(self, message):
@@ -170,14 +171,15 @@
         self._channel = _apply_metadata_interceptor(channel, self._metadata)
         if not auth_token and os.environ.get("PACH_PYTHON_OIDC_TOKEN"):
             resp = self.authenticate_id_token(os.environ.get("PACH_PYTHON_OIDC_TOKEN"))
             self._auth_token = resp
             self._metadata = self._build_metadata()
             self._channel = _apply_metadata_interceptor(channel, self._metadata)
         super().__init__()  # Initialize all the Mixin classes.
+        self._worker: Optional[_WorkerStub] = None
 
     @classmethod
     def new_in_cluster(
         cls, auth_token: str = None, transaction_id: str = None
     ) -> "Client":
         """Creates a Pachyderm client that operates within a Pachyderm cluster.
 
@@ -470,14 +472,39 @@
             channel=_create_channel(
                 self.address, self.root_certs, options=GRPC_CHANNEL_OPTIONS
             ),
             metadata=self._metadata,
         )
         super().__init__()
 
+    @property
+    def worker(self) -> _WorkerStub:
+        """Access the worker API stub.
+
+        This is dynamically loaded in order to provide a helpful error message
+        to the user if they try to interact with the worker API from outside
+        a worker.
+        """
+        worker_port_env = "PPS_WORKER_GRPC_PORT"
+        if self._worker is None:
+            port = os.environ.get(worker_port_env)
+            if port is None:
+                raise ConnectionError(
+                    f"Cannot connect to the worker since {worker_port_env} is not set. "
+                    "Are you running inside a pipeline?"
+                )
+            # Note: This channel doe not go through the metadata interceptor.
+            channel = _create_channel(
+                address=f"localhost:{port}",
+                root_certs=None,
+                options=GRPC_CHANNEL_OPTIONS,
+            )
+            self._worker = _WorkerStub(channel)
+        return self._worker
+
     def _build_metadata(self):
         metadata = []
         if self._auth_token is not None:
             metadata.append(("authn-token", self._auth_token))
         if self._transaction_id is not None:
             metadata.append(("pach-transaction", self._transaction_id))
         return metadata
```

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/errors.py` & `python_pachyderm-7.5.0/src/python_pachyderm/errors.py`

 * *Files identical despite different names*

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/mixin/admin.py` & `python_pachyderm-7.5.0/src/python_pachyderm/mixin/admin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-from typing import TYPE_CHECKING
+import grpc
+from google.protobuf import empty_pb2
 
-from python_pachyderm.service import Service
-import betterproto.lib.google.protobuf as bp_proto
-
-if TYPE_CHECKING:
-    from python_pachyderm.experimental.service import admin_proto
-
-# bp_to_pb: bp_proto.Empty -> empty_pb2.Empty
+from python_pachyderm.proto.v2.admin import admin_pb2, admin_pb2_grpc
 
 
 class AdminMixin:
     """A mixin for admin-related functionality."""
 
+    _channel: grpc.Channel
+
+    def __init__(self):
+        self.__stub = admin_pb2_grpc.APIStub(self._channel)
+        super().__init__()
+
     # TODO: This method should auto-populate it's message with information about
     #   the version of this package that is making the call. This is to allow
     #   the cluster to emit warnings about incompatible versions.
     #  This is not currently feasible to implement until we have better coupling
     #    with the versions of the core product.
-    def inspect_cluster(self) -> "admin_proto.ClusterInfo":
+    def inspect_cluster(self) -> admin_pb2.ClusterInfo:
         """Inspects a cluster.
 
         Returns
         -------
-        admin_proto.ClusterInfo
+        admin_pb2.ClusterInfo
             A protobuf object with info on the cluster.
         """
-        return self._req(
-            Service.ADMIN,
-            "InspectCluster",
-            req=bp_proto.Empty(),
-        )
+        message = empty_pb2.Empty()
+        return self.__stub.InspectCluster(message)
```

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/mixin/auth.py` & `python_pachyderm-7.5.0/src/python_pachyderm/mixin/auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from typing import Dict, List
-from grpc import RpcError
 
-from python_pachyderm.errors import AuthServiceNotActivated
-from python_pachyderm.service import Service
-from python_pachyderm.experimental.service import auth_proto
+import grpc
 
-# bp_to_pb: OidcConfig -> OIDCConfig
-# bp_to_pb: GetOidcLoginResponse -> GetOIDCLoginResponse
+from python_pachyderm.errors import AuthServiceNotActivated
+from python_pachyderm.proto.v2.auth import auth_pb2, auth_pb2_grpc
 
 
 class AuthMixin:
     """A mixin for auth-related functionality."""
 
+    _channel: grpc.Channel
+
+    def __init__(self):
+        self.__stub = auth_pb2_grpc.APIStub(self._channel)
+        super().__init__()
+
     def activate_auth(self, root_token: str = None) -> str:
         """Activates auth on the cluster. Returns the root token, an
         irrevocable superuser credential that should be stored securely.
 
         Parameters
         ----------
         root_token : str, optional
@@ -23,168 +26,172 @@
             it is safer to not set and let Pachyderm generate one for you.
 
         Returns
         -------
         str
             A token used as the root user login token.
         """
-        return self._req(Service.AUTH, "Activate", root_token=root_token).pach_token
+        message = auth_pb2.ActivateRequest(root_token=root_token)
+        return self.__stub.Activate(message).pach_token
 
     def deactivate_auth(self) -> None:
         """Deactivates auth, removing all ACLs, tokens, and admins from the
         Pachyderm cluster and making all data publicly accessible.
 
         Raises
         ------
         AuthServiceNotActivated
         """
+        message = auth_pb2.DeactivateRequest()
         try:
-            self._req(Service.AUTH, "Deactivate")
-        except RpcError as err:
+            self.__stub.Deactivate(message)
+        except grpc.RpcError as err:
             raise AuthServiceNotActivated.try_from(err)
 
-    def get_auth_configuration(self) -> auth_proto.OidcConfig:
+    def get_auth_configuration(self) -> auth_pb2.OIDCConfig:
         """Gets the auth configuration.
 
         Returns
         -------
-        auth_proto.OidcConfig
+        auth_pb2.OIDCConfig
             A protobuf object with auth configuration information.
         """
-        return self._req(Service.AUTH, "GetConfiguration").configuration
+        message = auth_pb2.GetConfigurationRequest()
+        return self.__stub.GetConfiguration(message).configuration
 
-    def set_auth_configuration(self, configuration: auth_proto.OidcConfig) -> None:
+    def set_auth_configuration(self, configuration: auth_pb2.OIDCConfig) -> None:
         """Sets the auth configuration.
 
         Parameters
         ----------
-        configuration : auth_proto.OidcConfig
+        configuration : auth_pb2.OIDCConfig
             A protobuf object with auth configuration information.
 
         Examples
         --------
-        >>> client.set_auth_configuration(auth_proto.OidcConfig(
+        >>> client.set_auth_configuration(auth_pb2.OIDCConfig(
         ...     issuer="http://localhost:1658",
         ...     client_id="client",
         ...     client_secret="secret",
         ...     redirect_uri="http://test.example.com",
         ... ))
         """
-        self._req(Service.AUTH, "SetConfiguration", configuration=configuration)
+        message = auth_pb2.SetConfigurationRequest(configuration=configuration)
+        self.__stub.SetConfiguration(message)
 
     def get_role_binding(
-        self, resource: auth_proto.Resource
-    ) -> Dict[str, auth_proto.Roles]:
+        self, resource: auth_pb2.Resource
+    ) -> Dict[str, auth_pb2.Roles]:
         """Returns the current set of role bindings to the resource specified.
 
         Parameters
         ----------
-        resource : auth_proto.Resource
+        resource : auth_pb2.Resource
             A protobuf object representing the resource being checked.
 
         Returns
         -------
-        Dict[str, auth_proto.Roles]
+        Dict[str, auth_pb2.Roles]
             A dictionary mapping the principals to the roles they have.
 
         Examples
         --------
-        >>> client.get_role_binding(auth_proto.Resource(type=auth_proto.CLUSTER))
+        >>> client.get_role_binding(auth_pb2.Resource(type=auth_pb2.CLUSTER))
         {
             'robot:someuser': roles {
                 key: "clusterAdmin"
                 value: true
             },
             'pach:root': roles {
                 key: "clusterAdmin"
                 value: true
             }
         }
         ...
-        >>> client.get_role_binding(auth_proto.Resource(type=auth_proto.REPO, name="foobar"))
+        >>> client.get_role_binding(auth_pb2.Resource(type=auth_pb2.REPO, name="foobar"))
         {
             'user:person_a': roles {
                 key: "repoWriter"
                 value: true
             },
             'pach:root': roles {
                 key: "repoOwner"
                 value: true
             }
         }
 
         .. # noqa: W505
         """
-        return self._req(
-            Service.AUTH, "GetRoleBinding", resource=resource
-        ).binding.entries
+        message = auth_pb2.GetRoleBindingRequest(resource=resource)
+        return self.__stub.GetRoleBinding(message).binding.entries
 
     def modify_role_binding(
-        self, resource: auth_proto.Resource, principal: str, roles: List[str] = None
+        self, resource: auth_pb2.Resource, principal: str, roles: List[str] = None
     ) -> None:
         """Sets the roles for a given principal on a resource.
 
         Parameters
         ----------
-        resource : auth_proto.Resource
+        resource : auth_pb2.Resource
             A protobuf object representing the resource to grant the roles on.
         principal : str
             The principal to grant the roles for.
         roles : List[str], optional
             The absolute list of roles for the principtal to have. If roles is
             unset, the principal will have no roles.
 
         Examples
         --------
         You can find some of the built-in roles here:
         https://github.com/pachyderm/pachyderm/blob/master/src/auth/auth.go#L27
 
         >>> client.modify_role_binding(
-        ...     auth_proto.Resource(type=auth_proto.CLUSTER),
+        ...     auth_pb2.Resource(type=auth_pb2.CLUSTER),
         ...     "user:someuser",
         ...     roles=["clusterAdmin"]
         ... )
         >>> client.modify_role_binding(
-        ...     auth_proto.Resource(type=auth_proto.REPO, name="foobar"),
+        ...     auth_pb2.Resource(type=auth_pb2.REPO, name="foobar"),
         ...     "user:someuser",
         ...     roles=["repoWriter"]
         ... )
         """
-        self._req(
-            Service.AUTH,
-            "ModifyRoleBinding",
+        message = auth_pb2.ModifyRoleBindingRequest(
             resource=resource,
             principal=principal,
             roles=roles,
         )
+        self.__stub.ModifyRoleBinding(message)
 
-    def get_oidc_login(self) -> auth_proto.GetOidcLoginResponse:
+    def get_oidc_login(self) -> auth_pb2.GetOIDCLoginResponse:
         """Gets the OIDC login configuration.
 
         Returns
         -------
-        auth_proto.GetOidcLoginResponse
+        auth_pb2.GetOIDCLoginResponse
             A protobuf object with the login configuration information.
         """
-        return self._req(Service.AUTH, "GetOIDCLogin")
+        message = auth_pb2.GetOIDCLoginRequest()
+        return self.__stub.GetOIDCLogin(message)
 
     def authenticate_oidc(self, oidc_state: str) -> str:
         """Authenticates a user to the Pachyderm cluster via OIDC.
 
         Parameters
         ----------
         oidc_state : str
             An OIDC state token.
 
         Returns
         -------
         str
             A token that can be used for making authenticate requests.
         """
-        return self._req(Service.AUTH, "Authenticate", oidc_state=oidc_state).pach_token
+        message = auth_pb2.AuthenticateRequest(oidc_state=oidc_state)
+        return self.__stub.Authenticate(message).pach_token
 
     def authenticate_id_token(self, id_token: str) -> str:
         """Authenticates a user to the Pachyderm cluster using an ID token
         issued by the OIDC provider. The token must include the Pachyderm
         client_id in the set of audiences to be valid.
 
         Parameters
@@ -193,90 +200,90 @@
             The ID token.
 
         Returns
         -------
         str
             A token that can be used for making authenticate requests.
         """
-        return self._req(Service.AUTH, "Authenticate", id_token=id_token).pach_token
+        message = auth_pb2.AuthenticateRequest(id_token=id_token)
+        return self.__stub.Authenticate(message).pach_token
 
     def authorize(
         self,
-        resource: auth_proto.Resource,
-        permissions: List["auth_proto.Permission"] = None,
-    ) -> auth_proto.AuthorizeResponse:
+        resource: auth_pb2.Resource,
+        permissions: List["auth_pb2.Permission"] = None,
+    ) -> auth_pb2.AuthorizeResponse:
         """Tests a list of permissions that the user might have on a resource.
 
         Parameters
         ----------
-        resource : auth_proto.Resource
+        resource : auth_pb2.Resource
             The resource the user wants to test on.
-        permissions : List[auth_proto.Permission], optional
+        permissions : List[auth_pb2.Permission], optional
             The list of permissions the users wants to test.
 
         Returns
         -------
-        auth_proto.AuthorizeResponse
+        auth_pb2.AuthorizeResponse
             A protobuf object that indicates whether the user/principal had all
             the inputted permissions on the resource, which permissions the
             user had, which permissions the user lacked, and the name of the
             principal.
 
         Examples
         --------
         >>> client.authorize(
-        ...     auth_proto.Resource(type=auth_proto.REPO, name="foobar"),
-        ...     [auth_proto.Permission.REPO_READ]
+        ...     auth_pb2.Resource(type=auth_pb2.REPO, name="foobar"),
+        ...     [auth_pb2.Permission.REPO_READ]
         ... )
         authorized: true
         satisfied: REPO_READ
         principal: "pach:root"
         """
-        return self._req(
-            Service.AUTH, "Authorize", resource=resource, permissions=permissions
-        )
+        message = auth_pb2.AuthorizeRequest(resource=resource, permissions=permissions)
+        return self.__stub.Authorize(message)
 
-    def who_am_i(self) -> auth_proto.WhoAmIResponse:
+    def who_am_i(self) -> auth_pb2.WhoAmIResponse:
         """Returns info about the user tied to this `Client`.
 
         Returns
         -------
-        auth_proto.WhoAmIResponse
+        auth_pb2.WhoAmIResponse
             A protobuf object that returns the username and expiration for the
             token used.
         """
-        return self._req(Service.AUTH, "WhoAmI")
+        message = auth_pb2.WhoAmIRequest()
+        return self.__stub.WhoAmI(message)
 
     def get_roles_for_permission(
-        self, permission: auth_proto.Permission
-    ) -> List[auth_proto.Role]:
+        self, permission: auth_pb2.Permission
+    ) -> List[auth_pb2.Role]:
         """Returns a list of all roles that have the specified permission.
 
         Parameters
         ----------
-        permission : auth_proto.Permission
+        permission : auth_pb2.Permission
             The Permission enum to check for.
 
         Returns
         -------
-        List[auth_proto.Role]
+        List[auth_pb2.Role]
             A list of Role protobuf objects that all have the specified
             permission.
 
         Examples
         --------
         All available permissions can be found in auth proto Permissions enum
 
-        >>> roles = client.get_roles_for_permission(auth_proto.Permission.REPO_READ)
+        >>> roles = client.get_roles_for_permission(auth_pb2.Permission.REPO_READ)
 
         .. # noqa: W505
         """
-        return self._req(
-            Service.AUTH, "GetRolesForPermission", permission=permission
-        ).roles
+        message = auth_pb2.GetRolesForPermissionRequest(permission=permission)
+        return self.__stub.GetRolesForPermission(message).roles
 
     def get_robot_token(self, robot: str, ttl: int = None) -> str:
         """Gets a new auth token for a robot user.
 
         Parameters
         ----------
         robot : str
@@ -286,25 +293,27 @@
             token doesn't expire.
 
         Returns
         -------
         str
             The new auth token.
         """
-        return self._req(Service.AUTH, "GetRobotToken", robot=robot, ttl=ttl).token
+        message = auth_pb2.GetRobotTokenRequest(robot=robot, ttl=ttl)
+        return self.__stub.GetRobotToken(message).token
 
     def revoke_auth_token(self, token: str) -> None:
         """Revokes an auth token.
 
         Parameters
         ----------
         token : str
             The Pachyderm token being revoked.
         """
-        self._req(Service.AUTH, "RevokeAuthToken", token=token)
+        message = auth_pb2.RevokeAuthTokenRequest(token=token)
+        self.__stub.RevokeAuthToken(message)
 
     def set_groups_for_user(self, username: str, groups: List[str]) -> None:
         """Sets the group membership for a user.
 
         Parameters
         ----------
         username : str
@@ -314,15 +323,16 @@
 
         Examples
         --------
         >>> client.set_groups_for_user("user:someuser", ["foogroup", "bargroup"])
 
         .. # noqa: W505
         """
-        self._req(Service.AUTH, "SetGroupsForUser", username=username, groups=groups)
+        message = auth_pb2.SetGroupsForUserRequest(username=username, groups=groups)
+        self.__stub.SetGroupsForUser(message)
 
     def modify_members(
         self, group: str, add: List[str] = None, remove: List[str] = None
     ) -> None:
         """Adds and/or removes members of a group.
 
         Parameters
@@ -338,46 +348,43 @@
         --------
         >>> client.modify_members(
         ...     "foogroup",
         ...     add=["user:otheruser"],
         ...     remove=["user:someuser"]
         ... )
         """
-        self._req(
-            Service.AUTH,
-            "ModifyMembers",
-            group=group,
-            add=add,
-            remove=remove,
-        )
+        message = auth_pb2.ModifyMembersRequest(group=group, add=add, remove=remove)
+        self.__stub.ModifyMembers(message)
 
     def get_groups(self) -> List[str]:
         """Gets a list of groups this user belongs to.
 
         Returns
         -------
         List[str]
             List of groups the user belongs to.
         """
-        return self._req(Service.AUTH, "GetGroups").groups
+        message = auth_pb2.GetGroupsRequest()
+        return self.__stub.GetGroups(message).groups
 
     def get_users(self, group: str) -> List[str]:
         """Gets users in a group.
 
         Parameters
         ----------
         group : str
             The group to list users from.
 
         Returns
         -------
         List[str]
             All the users in the specified group.
         """
-        return self._req(Service.AUTH, "GetUsers", group=group).usernames
+        message = auth_pb2.GetUsersRequest(group=group)
+        return self.__stub.GetUsers(message).usernames
 
     def extract_auth_tokens(self):
         """This maps to an internal function that is only used for migration.
         Pachyderm's `extract` and `restore` functionality calls
         `extract_auth_tokens` and `restore_auth_tokens` to move Pachyderm tokens
         between clusters during migration. Currently this function is only used
         for Pachyderm internals, so we're avoiding support for this function in
```

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/mixin/health.py` & `python_pachyderm-7.5.0/src/python_pachyderm/mixin/health.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-from python_pachyderm.service import Service
-from python_pachyderm.experimental.service import health_proto
+import grpc
+from grpc_health.v1 import health_pb2, health_pb2_grpc
 
 
 class HealthMixin:
     """A mixin for health-related functionality."""
 
-    def health_check(self) -> health_proto.HealthCheckResponse:
+    _channel: grpc.Channel
+
+    def __init__(self):
+        self.__stub = health_pb2_grpc.HealthStub(self._channel)
+        super().__init__()
+
+    def health_check(self) -> health_pb2.HealthCheckResponse:
         """Returns a health check indicating if the server can handle
         RPCs.
 
         Returns
         -------
-        health_proto.HealthCheckResponse
+        health_pb2.HealthCheckResponse
             A protobuf object with a status enum indicating server health.
         """
-        return self._req(
-            Service.HEALTH,
-            "Check",
-            req=health_proto.HealthCheckRequest(),
-        )
+        message = health_pb2.HealthCheckRequest()
+        return self.__stub.Check(message)
```

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/mixin/identity.py` & `python_pachyderm-7.5.0/src/python_pachyderm/mixin/identity.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,176 +1,193 @@
 from typing import List
-from grpc import RpcError
 
-from python_pachyderm.errors import AuthServiceNotActivated
-from python_pachyderm.service import Service
-from python_pachyderm.experimental.service import identity_proto
+import grpc
 
-# bp_to_pb: OidcClient -> OIDCClient, IdpConnector -> IDPConnector
+from python_pachyderm.errors import AuthServiceNotActivated
+from python_pachyderm.proto.v2.identity import identity_pb2, identity_pb2_grpc
 
 
 class IdentityMixin:
     """A mixin for identity-related functionality."""
 
+    _channel: grpc.Channel
+
+    def __init__(self):
+        self.__stub = identity_pb2_grpc.APIStub(self._channel)
+        super().__init__()
+
     def set_identity_server_config(
-        self, config: identity_proto.IdentityServerConfig
+        self, config: identity_pb2.IdentityServerConfig
     ) -> None:
         """Configure the embedded identity server.
 
         Parameters
         ----------
-        config : identity_proto.IdentityServerConfig
+        config : identity_pb2.IdentityServerConfig
             A protobuf object that is the configuration for the identity web
             server.
         """
-        self._req(Service.IDENTITY, "SetIdentityServerConfig", config=config)
+        message = identity_pb2.SetIdentityServerConfigRequest(config=config)
+        self.__stub.SetIdentityServerConfig(message)
 
-    def get_identity_server_config(self) -> identity_proto.IdentityServerConfig:
+    def get_identity_server_config(self) -> identity_pb2.IdentityServerConfig:
         """Get the embedded identity server configuration.
 
         Returns
         -------
-        identity_proto.IdentityServerConfig
+        identity_pb2.IdentityServerConfig
             A protobuf object that holds configuration info (issuer and ID
             token expiry) for the identity web server.
         """
-        return self._req(Service.IDENTITY, "GetIdentityServerConfig").config
+        message = identity_pb2.GetIdentityServerConfigRequest()
+        return self.__stub.GetIdentityServerConfig(message).config
 
-    def create_idp_connector(self, connector: identity_proto.IdpConnector) -> None:
+    def create_idp_connector(self, connector: identity_pb2.IDPConnector) -> None:
         """Create an IDP connector in the identity server.
 
         Parameters
         ----------
-        connector : identity_proto.IdpConnector
+        connector : identity_pb2.IDPConnector
             A protobuf object that represents a connection to an identity
             provider.
         """
-        self._req(Service.IDENTITY, "CreateIDPConnector", connector=connector)
+        message = identity_pb2.CreateIDPConnectorRequest(connector=connector)
+        self.__stub.CreateIDPConnector(message)
 
-    def list_idp_connectors(self) -> List[identity_proto.IdpConnector]:
+    def list_idp_connectors(self) -> List[identity_pb2.IDPConnector]:
         """List IDP connectors in the identity server.
 
         Returns
         -------
-        List[identity_proto.IdpConnector]
+        List[identity_pb2.IDPConnector]
             A list of probotuf objects that return info on the connector ID,
             name, type, config version, and configuration of the upstream IDP
             connector.
         """
-        return self._req(Service.IDENTITY, "ListIDPConnectors").connectors
+        message = identity_pb2.ListIDPConnectorsRequest()
+        return self.__stub.ListIDPConnectors(message).connectors
 
-    def update_idp_connector(self, connector: identity_proto.IdpConnector) -> None:
+    def update_idp_connector(self, connector: identity_pb2.IDPConnector) -> None:
         """Update an IDP connector in the identity server.
 
         Parameters
         ----------
-        connector : identity_proto.IdpConnector
+        connector : identity_pb2.IDPConnector
             A protobuf object that represents a connection to an identity
             provider.
         """
-        self._req(Service.IDENTITY, "UpdateIDPConnector", connector=connector)
+        message = identity_pb2.UpdateIDPConnectorRequest(connector=connector)
+        self.__stub.UpdateIDPConnector(message)
 
-    def get_idp_connector(self, id: str) -> identity_proto.IdpConnector:
+    def get_idp_connector(self, id: str) -> identity_pb2.IDPConnector:
         """Get an IDP connector in the identity server.
 
         Parameters
         ----------
         id : str
             The connector ID.
 
         Returns
         -------
-        identity_proto.IdpConnector
+        identity_pb2.IDPConnector
             A protobuf object that returns info on the connector ID, name,
             type, config version, and configuration of the upstream IDP
             connector.
         """
-        return self._req(Service.IDENTITY, "GetIDPConnector", id=id).connector
+        message = identity_pb2.GetIDPConnectorRequest(id=id)
+        return self.__stub.GetIDPConnector(message).connector
 
     def delete_idp_connector(self, id: str) -> None:
         """Delete an IDP connector in the identity server.
 
         Parameters
         ----------
         id : str
             The connector ID.
         """
-        self._req(Service.IDENTITY, "DeleteIDPConnector", id=id)
+        message = identity_pb2.DeleteIDPConnectorRequest(id=id)
+        self.__stub.DeleteIDPConnector(message)
 
     def create_oidc_client(
-        self, client: identity_proto.OidcClient
-    ) -> identity_proto.OidcClient:
+        self, client: identity_pb2.OIDCClient
+    ) -> identity_pb2.OIDCClient:
         """Create an OIDC client in the identity server.
 
         Parameters
         ----------
-        client : identity_proto.OidcClient
+        client : identity_pb2.OIDCClient
             A protobuf object representing an OIDC client.
 
         Returns
         -------
-        identity_proto.OidcClient
+        identity_pb2.OIDCClient
             A protobuf object that returns a client with info on the client ID,
             name, secret, and lists of redirect URIs and trusted peers.
         """
-        return self._req(Service.IDENTITY, "CreateOIDCClient", client=client).client
+        message = identity_pb2.CreateOIDCClientRequest(client=client)
+        return self.__stub.CreateOIDCClient(message).client
 
-    def update_oidc_client(self, client: identity_proto.OidcClient) -> None:
+    def update_oidc_client(self, client: identity_pb2.OIDCClient) -> None:
         """Update an OIDC client in the identity server.
 
         Parameters
         ----------
-        client : identity_proto.OidcClient
+        client : identity_pb2.OIDCClient
             A protobuf object representing an OIDC client.
 
         """
-        return self._req(Service.IDENTITY, "UpdateOIDCClient", client=client)
+        message = identity_pb2.UpdateOIDCClientRequest(client=client)
+        return self.__stub.UpdateOIDCClient(message)
 
-    def get_oidc_client(self, id: str) -> identity_proto.OidcClient:
+    def get_oidc_client(self, id: str) -> identity_pb2.OIDCClient:
         """Get an OIDC client in the identity server.
 
         Parameters
         ----------
         id : str
             The client ID.
 
         Returns
         -------
-        identity_proto.OidcClient
+        identity_pb2.OIDCClient
             A protobuf object that returns a client with info on the client ID,
             name, secret, and lists of redirect URIs and trusted peers.
         """
-        return self._req(Service.IDENTITY, "GetOIDCClient", id=id).client
+        message = identity_pb2.GetOIDCClientRequest(id=id)
+        return self.__stub.GetOIDCClient(message).client
 
     def delete_oidc_client(self, id: str) -> None:
         """Delete an OIDC client in the identity server.
 
         Parameters
         ----------
         id : str
             The client ID.
         """
-        self._req(Service.IDENTITY, "DeleteOIDCClient", id=id)
+        message = identity_pb2.DeleteOIDCClientRequest(id=id)
+        self.__stub.DeleteOIDCClient(message)
 
-    def list_oidc_clients(self) -> List[identity_proto.OidcClient]:
+    def list_oidc_clients(self) -> List[identity_pb2.OIDCClient]:
         """List OIDC clients in the identity server.
 
         Returns
         -------
-        List[identity_proto.OidcClient]
+        List[identity_pb2.OIDCClient]
             A list of protobuf objects that return a client with info on the
             client ID, name, secret, and lists of redirect URIs and trusted
             peers.
         """
-        return self._req(Service.IDENTITY, "ListOIDCClients").clients
+        message = identity_pb2.ListOIDCClientsRequest()
+        return self.__stub.ListOIDCClients(message).clients
 
     def delete_all_identity(self) -> None:
         """Delete all identity service information.
 
         Raises
         ------
         AuthServiceNotActivated
         """
+        message = identity_pb2.DeleteAllRequest()
         try:
-            self._req(Service.IDENTITY, "DeleteAll")
-        except RpcError as err:
+            self.__stub.DeleteAll(message)
+        except grpc.RpcError as err:
             raise AuthServiceNotActivated.try_from(err)
```

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/mixin/license.py` & `python_pachyderm-7.5.0/src/python_pachyderm/mixin/license.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 from typing import List
-from grpc import RpcError
 
-from python_pachyderm.errors import AuthServiceNotActivated
-from python_pachyderm.service import Service
-from python_pachyderm.experimental.service import license_proto, enterprise_proto
+import grpc
 from google.protobuf import timestamp_pb2
-import datetime
 
-# bp_to_pb: datetime.datetime -> timestamp_pb2.Timestamp
+from python_pachyderm.errors import AuthServiceNotActivated
+from python_pachyderm.proto.v2.enterprise import enterprise_pb2
+from python_pachyderm.proto.v2.license import license_pb2, license_pb2_grpc
 
 
 class LicenseMixin:
     """A mixin for license-related functionality."""
 
+    _channel: grpc.Channel
+
+    def __init__(self):
+        self.__stub = license_pb2_grpc.APIStub(self._channel)
+        super().__init__()
+
     def activate_license(
-        self, activation_code: str, expires: datetime.datetime = None
-    ) -> enterprise_proto.TokenInfo:
+        self, activation_code: str, expires: timestamp_pb2.Timestamp = None
+    ) -> enterprise_pb2.TokenInfo:
         """Activates the license service.
 
         Parameters
         ----------
         activation_code : str
             A Pachyderm enterprise activation code. New users can obtain trial
             activation codes.
-        expires : datetime.datetime, optional
+        expires : timestamp_pb2.Timestamp, optional
             A protobuf object indicating when this activation code will expire.
             This should generally not be set and is only applied if it is
             earlier than the signed expiration time of `activation_code`.
 
         Returns
         -------
-        enterprise_proto.TokenInfo
+        enterprise_pb2.TokenInfo
             A protobuf object that has the expiration for the current token.
             Field will be unset if there is no current token.
         """
-        return self._req(
-            Service.LICENSE,
-            "Activate",
-            activation_code=activation_code,
-            expires=expires,
-        ).info
+        message = license_pb2.ActivateRequest(
+            activation_code=activation_code, expires=expires
+        )
+        return self.__stub.Activate(message).info
 
     def add_cluster(
         self,
         id: str,
         address: str,
         secret: str = None,
         user_address: str = None,
         cluster_deployment_id: str = None,
         enterprise_server: bool = False,
-    ) -> license_proto.AddClusterResponse:
+    ) -> license_pb2.AddClusterResponse:
         """Register a cluster with the license service.
 
         Parameters
         ----------
         id : str
             The unique ID to identify the cluster.
         address : str
@@ -66,27 +68,26 @@
         cluster_deployment_id : str, optional
             The deployment ID value generated by each cluster.
         enterprise_server : bool, optional
             Indicates whether the address points to an enterprise server.
 
         Returns
         -------
-        license_proto.AddClusterResponse
+        license_pb2.AddClusterResponse
             A protobuf object that returns the `secret`.
         """
-        return self._req(
-            Service.LICENSE,
-            "AddCluster",
-            id=id,
+        message = license_pb2.AddClusterRequest(
             address=address,
-            secret=secret,
-            user_address=user_address,
             cluster_deployment_id=cluster_deployment_id,
             enterprise_server=enterprise_server,
+            id=id,
+            secret=secret,
+            user_address=user_address,
         )
+        return self.__stub.AddCluster(message)
 
     def update_cluster(
         self,
         id: str,
         address: str,
         user_address: str = None,
         cluster_deployment_id: str = None,
@@ -104,70 +105,74 @@
             The pachd address for users to connect to.
         cluster_deployment_id : str, optional
             The deployment ID value generated by each cluster.
         secret : str, optional
             A shared secret for the cluster to use to authenticate. If not
             specified, a random secret will be generated and returned.
         """
-        self._req(
-            Service.LICENSE,
-            "UpdateCluster",
-            id=id,
+        message = license_pb2.UpdateClusterRequest(
             address=address,
-            user_address=user_address,
             cluster_deployment_id=cluster_deployment_id,
+            id=id,
+            user_address=user_address,
             secret=secret,
         )
+        self.__stub.UpdateCluster(message)
 
     def delete_cluster(self, id: str) -> None:
         """Delete a cluster registered with the license service.
 
         Parameters
         ----------
         id : str
             The unique ID to identify the cluster.
         """
-        self._req(Service.LICENSE, "DeleteCluster", id=id)
+        message = license_pb2.DeleteClusterRequest(id=id)
+        self.__stub.DeleteCluster(message)
 
-    def list_clusters(self) -> List[license_proto.ClusterStatus]:
+    def list_clusters(self) -> List[license_pb2.ClusterStatus]:
         """List clusters registered with the license service.
 
         Returns
         -------
-        List[license_proto.ClusterStatus]
+        List[license_pb2.ClusterStatus]
             A list of protobuf objects that return info on a cluster.
         """
-        return self._req(Service.LICENSE, "ListClusters").clusters
+        message = license_pb2.ListClustersRequest()
+        return self.__stub.ListClusters(message).clusters
 
-    def get_activation_code(self) -> license_proto.GetActivationCodeResponse:
+    def get_activation_code(self) -> license_pb2.GetActivationCodeResponse:
         """Gets the enterprise code used to activate the server.
 
         Returns
         -------
-        license_proto.GetActivationCodeResponse
+        license_pb2.GetActivationCodeResponse
             A protobuf object that returns a state enum, info on the token,
             and the activation code.
         """
-        return self._req(Service.LICENSE, "GetActivationCode")
+        message = license_pb2.GetActivationCodeRequest()
+        return self.__stub.GetActivationCode(message)
 
     def delete_all_license(self) -> None:
         """Remove all clusters and deactivate the license service.
 
         Raises
         ------
         AuthServiceNotActivated
         """
+        message = license_pb2.DeleteAllRequest()
         try:
-            self._req(Service.LICENSE, "DeleteAll")
-        except RpcError as err:
+            self.__stub.DeleteAll(message)
+        except grpc.RpcError as err:
             raise AuthServiceNotActivated.try_from(err)
 
-    def list_user_clusters(self) -> List[license_proto.UserClusterInfo]:
+    def list_user_clusters(self) -> List[license_pb2.UserClusterInfo]:
         """Lists all clusters available to user.
 
         Returns
         -------
-        List[license_proto.UserClusterInfo]
+        List[license_pb2.UserClusterInfo]
             A list of protobuf objects that return info on clusters
             available to the users.
         """
-        return self._req(Service.LICENSE, "ListUserClusters").clusters
+        message = license_pb2.ListUserClustersRequest()
+        return self.__stub.ListUserClusters(message).clusters
```

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/mixin/pfs.py` & `python_pachyderm-7.5.0/src/python_pachyderm/mixin/pfs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,118 @@
 import io
-import re
 import os
-import time
+import re
 import itertools
-import subprocess
-from pathlib import Path
+import tarfile
 from contextlib import contextmanager
 from datetime import datetime
 from typing import Iterator, Union, List, BinaryIO
 
 try:
     from collections.abc import Iterable
 except ImportError:
     from collections import Iterable
 
-from python_pachyderm.mixin.pfs import PFSFile, PFSTarFile
-from python_pachyderm.experimental.pfs import commit_from, Commit, uuid_re
-from python_pachyderm.service import Service, pfs_proto as pfs_proto_pb
-from python_pachyderm.experimental.service import pfs_proto
-from python_pachyderm.experimental.util import check_pachctl
-from google.protobuf import wrappers_pb2, timestamp_pb2
-import betterproto.lib.google.protobuf as bp_proto
-
-# bp_to_pb: bp_proto.Empty -> empty_pb2.Empty
-# bp_to_pb: url -> URL (get_file_tar())
+import grpc
 
+from python_pachyderm.pfs import commit_from, uuid_re, SubcommitType
+from python_pachyderm.proto.v2.pfs import pfs_pb2, pfs_pb2_grpc
+from google.protobuf import empty_pb2, wrappers_pb2, timestamp_pb2
 
 BUFFER_SIZE = 19 * 1024 * 1024
 
 
+class PFSTarFile(tarfile.TarFile):
+    def __iter__(self):
+        for tarinfo in super().__iter__():
+            if os.path.isabs(tarinfo.path):
+                # Hack to prevent extraction to absolute paths.
+                tarinfo.path = tarinfo.path[1:]
+            if tarinfo.mode == 0:
+                # Hack to prevent writing files with no permissions.
+                tarinfo.mode = 0o700
+            yield tarinfo
+
+
+class PFSFile:
+    """File-like objects containing content of a file stored in PFS.
+
+    Examples
+    --------
+    >>> # client.get_file() returns a PFSFile
+    >>> source_file = client.get_file(("montage", "master"), "/montage.png")
+    >>> with open("montage.png", "wb") as dest_file:
+    >>>     shutil.copyfileobj(source_file, dest_file)
+    ...
+    >>> with client.get_file(("montage", "master"), "/montage2.png") as f:
+    >>>     content = f.read()
+    """
+
+    def __init__(self, stream: Iterator[wrappers_pb2.BytesValue]):
+        self._stream = stream
+        self._buffer = bytearray()
+
+        try:
+            first_message = next(self._stream)
+        except grpc.RpcError as err:
+            raise ConnectionError("Error creating the PFSFile") from err
+        self._buffer.extend(first_message.value)
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, type, val, tb):
+        self.close()
+
+    def read(self, size: int = -1) -> bytes:
+        """Reads from the :class:`.PFSFile` buffer.
+
+        Parameters
+        ----------
+        size : int, optional
+            If set, the number of bytes to read from the buffer.
+
+        Returns
+        -------
+        bytes
+            Content from the stream.
+        """
+        try:
+            if size == -1:
+                # Consume the entire stream.
+                for message in self._stream:
+                    self._buffer.extend(message.value)
+                result, self._buffer[:] = self._buffer[:], b""
+                return bytes(result)
+            elif len(self._buffer) < size:
+                for message in self._stream:
+                    self._buffer.extend(message.value)
+                    if len(self._buffer) >= size:
+                        break
+        except grpc.RpcError:
+            pass
+
+        size = min(size, len(self._buffer))
+        result, self._buffer[:size] = self._buffer[:size], b""
+        return bytes(result)
+
+    def close(self) -> None:
+        """Closes the :class:`.PFSFile`."""
+        self._stream.cancel()
+
+
 class PFSMixin:
     """A mixin with pfs-related functionality."""
 
+    _channel: grpc.Channel
+
+    def __init__(self):
+        self.__stub = pfs_pb2_grpc.APIStub(self._channel)
+        super().__init__()
+
     def create_repo(
         self,
         repo_name: str,
         description: str = None,
         update: bool = False,
         project_name: str = None,
     ) -> None:
@@ -52,75 +129,74 @@
         description : str, optional
             Description of the repo.
         update : bool, optional
             Whether to update if the repo already exists.
         project_name : str
             The name of the project.
         """
-        self._req(
-            Service.PFS,
-            "CreateRepo",
-            repo=pfs_proto.Repo(
+        message = pfs_pb2.CreateRepoRequest(
+            description=description,
+            repo=pfs_pb2.Repo(
                 name=repo_name,
                 type="user",
-                project=pfs_proto.Project(name=project_name),
+                project=pfs_pb2.Project(name=project_name),
             ),
-            description=description,
             update=update,
         )
+        self.__stub.CreateRepo(message)
 
     def inspect_repo(
         self, repo_name: str, project_name: str = None
-    ) -> pfs_proto.RepoInfo:
+    ) -> pfs_pb2.RepoInfo:
         """Inspects a repo.
 
         Parameters
         ----------
         repo_name : str
             Name of the repo.
         project_name : str
             The name of the project.
 
         Returns
         -------
-        pfs_proto.RepoInfo
+        pfs_pb2.RepoInfo
             A protobuf object with info on the repo.
         """
-        return self._req(
-            Service.PFS,
-            "InspectRepo",
-            repo=pfs_proto.Repo(
+        message = pfs_pb2.InspectRepoRequest(
+            repo=pfs_pb2.Repo(
                 name=repo_name,
                 type="user",
-                project=pfs_proto.Project(name=project_name),
+                project=pfs_pb2.Project(name=project_name),
             ),
         )
+        return self.__stub.InspectRepo(message)
 
     def list_repo(
-        self, type: str = "user", projects_filter: List[pfs_proto.Project] = None
-    ) -> Iterator[pfs_proto.RepoInfo]:
+        self, type: str = "user", projects_filter: List[pfs_pb2.Project] = None
+    ) -> Iterator[pfs_pb2.RepoInfo]:
         """Lists all repos in PFS.
 
         Parameters
         ----------
         type : str, optional
             The type of repos that should be returned ("user", "meta", "spec").
             If unset, returns all types of repos.
         projects_filter : [Project], optional
             Filters out repos that do not belong in the list,
             while no projects means to list all repos
 
         Returns
         -------
-        Iterator[pfs_proto.RepoInfo]
+        Iterator[pfs_pb2.RepoInfo]
             An iterator of protobuf objects that contain info on a repo.
         """
         if isinstance(projects_filter, Iterable):
-            projects_filter = [pfs_proto.Project(name=p.name) for p in projects_filter]
-        return self._req(Service.PFS, "ListRepo", type=type, projects=projects_filter)
+            projects_filter = [pfs_pb2.Project(name=p.name) for p in projects_filter]
+        message = pfs_pb2.ListRepoRequest(type=type, projects=projects_filter)
+        return self.__stub.ListRepo(message)
 
     def delete_repo(
         self, repo_name: str, force: bool = False, project_name: str = None
     ) -> None:
         """Deletes a repo and reclaims the storage space it was using.
 
         Parameters
@@ -129,28 +205,28 @@
             The name of the repo.
         force : bool, optional
             If set to true, the repo will be removed regardless of errors.
             Use with care.
         project_name : str
             The name of the project.
         """
-        self._req(
-            Service.PFS,
-            "DeleteRepo",
-            repo=pfs_proto.Repo(
+        message = pfs_pb2.DeleteRepoRequest(
+            force=force,
+            repo=pfs_pb2.Repo(
                 name=repo_name,
                 type="user",
-                project=pfs_proto.Project(name=project_name),
+                project=pfs_pb2.Project(name=project_name),
             ),
-            force=force,
         )
+        self.__stub.DeleteRepo(message)
 
     def delete_all_repos(self) -> None:
         """Deletes all repos."""
-        self._req(Service.PFS, "DeleteAll", req=bp_proto.Empty())
+        message = empty_pb2.Empty()
+        self.__stub.DeleteAll(message)
 
     def create_project(
         self, project_name: str, description: str = None, update: bool = False
     ) -> None:
         """Creates a new project with the given name.
 
         Parameters
@@ -158,139 +234,134 @@
         project_name : str
             Name of the project.
         description : str, optional
             Description of the project.
         update : bool, optional
             Whether to update if the project already exists.
         """
-        self._req(
-            Service.PFS,
-            "CreateProject",
-            project=pfs_proto.Project(name=project_name),
+        message = pfs_pb2.CreateProjectRequest(
+            project=pfs_pb2.Project(name=project_name),
             description=description,
             update=update,
         )
+        self.__stub.CreateProject(message)
 
-    def inspect_project(self, project_name: str) -> pfs_proto.ProjectInfo:
+    def inspect_project(self, project_name: str) -> pfs_pb2.ProjectInfo:
         """Inspects a project.
 
         Parameters
         ----------
         project_name : str
             Name of the project.
 
         Returns
         -------
         pfs_proto.ProjectInfo
             A protobuf object with info on the project.
         """
-        return self._req(
-            Service.PFS, "InspectProject", project=pfs_proto.Project(name=project_name)
+        message = pfs_pb2.InspectProjectRequest(
+            project=pfs_pb2.Project(name=project_name)
         )
+        return self.__stub.InspectProject(message)
 
-    def list_project(self) -> Iterator[pfs_proto.ProjectInfo]:
+    def list_project(self) -> Iterator[pfs_pb2.ProjectInfo]:
         """Lists all projects in PFS.
 
         Returns
         -------
         Iterator[pfs_proto.ProjectInfo]
             An iterator of protobuf objects that contain info on a project.
         """
-        return self._req(
-            Service.PFS,
-            "ListProject",
-            req=bp_proto.Empty(),
-        )
+        message = pfs_pb2.ListProjectRequest()
+        return self.__stub.ListProject(message)
 
     def delete_project(self, project_name: str, force: bool = False) -> None:
         """Deletes a project and reclaims the storage space it was using.
 
         Parameters
         ----------
         project_name : str
             The name of the project.
         force : bool, optional
             If set to true, the repo will be removed regardless of errors.
             Use with care.
         """
-        self._req(
-            Service.PFS,
-            "DeleteProject",
+        message = pfs_pb2.DeleteProjectRequest(
             force=force,
-            project=pfs_proto.Project(name=project_name),
+            project=pfs_pb2.Project(name=project_name),
         )
+        self.__stub.DeleteProject(message)
 
     def start_commit(
         self,
         repo_name: str,
         branch: str,
-        parent: Union[str, tuple, dict, Commit, pfs_proto.Commit] = None,
+        parent: Union[str, SubcommitType] = None,
         description: str = None,
         project_name: str = None,
-    ) -> pfs_proto.Commit:
+    ) -> pfs_pb2.Commit:
         """Begins the process of committing data to a repo. Once started you
         can write to the commit with ModifyFile. When all the data has been
         written, you must finish the commit with FinishCommit. NOTE: data is
         not persisted until FinishCommit is called.
 
         Parameters
         ----------
         repo_name : str
             The name of the repo.
         branch_name : str
             A string specifying the branch.
-        parent : Union[str, tuple, dict, Commit, pfs_proto.Commit], optional
+        parent : Union[str, SubcommitType], optional
             A commit specifying the parent of the newly created commit. Upon
             creation, before data is modified, the new commit will appear
             identical to the parent.
         description : str, optional
             A description of the commit.
         project_name : str
             The name of the project.
 
         Returns
         -------
-        pfs_proto.Commit
+        pfs_pb2.Commit
             A protobuf object that represents an open subcommit (commit at the
             repo-level).
 
         Examples
         --------
         >>> c = client.start_commit("foo", "master", ("foo", "staging"))
         """
-        repo = pfs_proto.Repo(
-            name=repo_name, type="user", project=pfs_proto.Project(name=project_name)
+        repo = pfs_pb2.Repo(
+            name=repo_name, type="user", project=pfs_pb2.Project(name=project_name)
         )
         if parent and isinstance(parent, str):
-            parent = pfs_proto.Commit(
+            parent = pfs_pb2.Commit(
                 id=parent,
-                branch=pfs_proto.Branch(repo=repo, name=None),
+                branch=pfs_pb2.Branch(name=None, repo=repo),
             )
-        return self._req(
-            Service.PFS,
-            "StartCommit",
-            parent=commit_from(parent),
-            branch=pfs_proto.Branch(repo=repo, name=branch),
+        message = pfs_pb2.StartCommitRequest(
+            branch=pfs_pb2.Branch(name=branch, repo=repo),
             description=description,
+            parent=commit_from(parent),
         )
+        return self.__stub.StartCommit(message)
 
     def finish_commit(
         self,
-        commit: Union[tuple, dict, Commit, pfs_proto.Commit],
+        commit: SubcommitType,
         description: str = None,
         error: str = None,
         force: bool = False,
     ) -> None:
         """Ends the process of committing data to a repo and persists the
         commit. Once a commit is finished the data becomes immutable and
         future attempts to write to it with ModifyFile will error.
 
         Parameters
         ----------
-        commit : Union[tuple, dict, Commit, pfs_proto.Commit]
+        commit : SubcommitType
             The subcommit (commit at the repo-level) object to close.
         description : str, optional
             A description of the commit. It will overwrite the description set
             in ``start_commit()``.
         error : str, optional
             If set, a message that errors out the commit. Don't use unless you
             want the finish commit request to fail.
@@ -300,59 +371,58 @@
         Examples
         --------
         Commit needs to be open still, either from the result of
         ``start_commit()`` or within scope of ``commit()``
 
         >>> client.start_commit("foo", "master")
         >>> # modify open commit
-        >>> client.finish_commit(("foo", "master))
+        >>> client.finish_commit(("foo", "master"))
         ...
         >>> # same as above
         >>> c = client.start_commit("foo", "master")
         >>> # modify open commit
         >>> client.finish_commit(c)
         """
-        self._req(
-            Service.PFS,
-            "FinishCommit",
+        message = pfs_pb2.FinishCommitRequest(
             commit=commit_from(commit),
             description=description,
             error=error,
             force=force,
         )
+        self.__stub.FinishCommit(message)
 
     @contextmanager
     def commit(
         self,
         repo_name: str,
         branch: str,
-        parent: Union[str, tuple, dict, Commit, pfs_proto.Commit] = None,
+        parent: Union[str, SubcommitType] = None,
         description: str = None,
         project_name: str = None,
-    ) -> Iterator[pfs_proto.Commit]:
+    ) -> Iterator[pfs_pb2.Commit]:
         """A context manager for running operations within a commit.
 
         Parameters
         ----------
         repo_name : str
             The name of the repo.
         branch : str
             A string specifying the branch.
-        parent : Union[str, tuple, dict, Commit, pfs_proto.Commit], optional
+        parent : Union[str, SubcommitType], optional
             A commit specifying the parent of the newly created commit. Upon
             creation, before data is modified, the new commit will appear
             identical to the parent.
         description : str, optional
             A description of the commit.
         project_name : str
             The name of the project.
 
         Yields
         -------
-        pfs_proto.Commit
+        pfs_pb2.Commit
             A protobuf object that represents a commit.
 
         Examples
         --------
         >>> with client.commit("foo", "master") as c:
         >>>     client.delete_file(c, "/dir/delete_me.txt")
         >>>     client.put_file_bytes(c, "/new_file.txt", b"DATA")
@@ -361,116 +431,109 @@
         try:
             yield commit
         finally:
             self.finish_commit(commit)
 
     def inspect_commit(
         self,
-        commit: Union[str, tuple, dict, Commit, pfs_proto.Commit],
-        commit_state: pfs_proto.CommitState = pfs_proto.CommitState.STARTED,
-    ) -> Iterator[pfs_proto.CommitInfo]:
+        commit: Union[str, SubcommitType],
+        commit_state: pfs_pb2.CommitState = pfs_pb2.CommitState.STARTED,
+    ) -> Iterator[pfs_pb2.CommitInfo]:
         """Inspects a commit.
 
         Parameters
         ----------
-        commit : Union[str, tuple, dict, Commit, pfs_proto.Commit]
+        commit : Union[str, SubcommitType]
             The commit to inspect. Can either be a commit ID or a commit object
             that represents a subcommit (commit at the repo-level).
-        commit_state : {pfs_proto.CommitState.STARTED, pfs_proto.CommitState.READY, pfs_proto.CommitState.FINISHING, pfs_proto.CommitState.FINISHED}, optional
+        commit_state : {pfs_pb2.CommitState.STARTED, pfs_pb2.CommitState.READY, pfs_pb2.CommitState.FINISHING, pfs_pb2.CommitState.FINISHED}, optional
             An enum that causes the method to block until the commit is in the
-            specified state. (Default value = ``pfs_proto.CommitState.STARTED``)
+            specified state. (Default value = ``pfs_pb2.CommitState.STARTED``)
 
         Returns
         -------
-        Iterator[pfs_proto.CommitInfo]
+        Iterator[pfs_pb2.CommitInfo]
             An iterator of protobuf objects that contain info on a subcommit
             (commit at the repo-level).
 
         Examples
         --------
         >>> # commit at repo-level
         >>> list(client.inspect_commit(("foo", "master~2")))
         ...
         >>> # an entire commit
-        >>> for commit in client.inspect_commit("467c580611234cdb8cc9758c7aa96087", pfs_proto.CommitState.FINISHED)
+        >>> for commit in client.inspect_commit("467c580611234cdb8cc9758c7aa96087", pfs_pb2.CommitState.FINISHED)
         >>>     print(commit)
 
         .. # noqa: W505
         """
         if not isinstance(commit, str):
-            return iter(
-                [
-                    self._req(
-                        Service.PFS,
-                        "InspectCommit",
-                        commit=commit_from(commit),
-                        wait=commit_state,
-                    )
-                ]
+            message = pfs_pb2.InspectCommitRequest(
+                commit=commit_from(commit), wait=commit_state
             )
+            return iter([self.__stub.InspectCommit(message)])
         elif uuid_re.match(commit):
-            return self._req(
-                Service.PFS,
-                "InspectCommitSet",
-                commit_set=pfs_proto.CommitSet(id=commit),
-                wait=commit_state == pfs_proto.CommitState.FINISHED,
+            message = pfs_pb2.InspectCommitSetRequest(
+                commit_set=pfs_pb2.CommitSet(id=commit),
+                wait=commit_state == pfs_pb2.CommitState.FINISHED,
             )
+            return self.__stub.InspectCommitSet(message)
         raise ValueError(
             "bad argument: commit should either be a commit ID (str) or a commit-like object"
         )
 
     def list_commit(
         self,
         repo_name: str = None,
-        to_commit: Union[tuple, dict, Commit, pfs_proto.Commit] = None,
-        from_commit: Union[tuple, dict, Commit, pfs_proto.Commit] = None,
+        to_commit: SubcommitType = None,
+        from_commit: SubcommitType = None,
         number: int = None,
         reverse: bool = False,
         all: bool = False,
-        origin_kind: pfs_proto.OriginKind = pfs_proto.OriginKind.USER,
+        origin_kind: pfs_pb2.OriginKind = pfs_pb2.OriginKind.USER,
         started_time: datetime = None,
         project_name: str = None,
-    ) -> Union[Iterator[pfs_proto.CommitInfo], Iterator[pfs_proto.CommitSetInfo]]:
+    ) -> Union[Iterator[pfs_pb2.CommitInfo], Iterator[pfs_pb2.CommitSetInfo]]:
         """Lists commits.
 
         Parameters
         ----------
         repo_name : str, optional
             The name of a repo. If set, returns subcommits (commit at
             repo-level) only in this repo.
-        to_commit : Union[tuple, dict, Commit, pfs_proto.Commit], optional
+        to_commit : SubcommitType, optional
             A subcommit (commit at repo-level) that only impacts results if
             `repo_name` is specified. If set, only the ancestors of
             `to_commit`, including `to_commit`, are returned.
-        from_commit : Union[tuple, dict, Commit, pfs_proto.Commit], optional
+        from_commit : SubcommitType, optional
             A subcommit (commit at repo-level) that only impacts results if
             `repo_name` is specified. If set, only the descendants of
             `from_commit`, including `from_commit`, are returned.
         number : int, optional
             The number of subcommits to return. If unset, all subcommits that
             matched the aforementioned criteria are returned. Only impacts
             results if `repo_name` is specified.
         reverse : bool, optional
             If true, returns the subcommits oldest to newest. Only impacts
             results if `repo_name` is specified.
         all : bool, optional
             If true, returns all types of subcommits. Otherwise, alias
             subcommits are excluded. Only impacts results if `repo_name` is
             specified.
-        origin_kind : {pfs_proto.OriginKind.USER, pfs_proto.OriginKind.AUTO, pfs_proto.OriginKind.FSCK, pfs_proto.OriginKind.ALIAS}, optional
+        origin_kind : {pfs_pb2.OriginKind.USER, pfs_pb2.OriginKind.AUTO, pfs_pb2.OriginKind.FSCK, pfs_pb2.OriginKind.ALIAS}, optional
             An enum that specifies how a subcommit originated. Returns only
             subcommits of this enum type. Only impacts results if `repo_name`
             is specified.
         started_time : datetime
         project_name : str, optional
             The name of the project containing the repo.
 
         Returns
         -------
-        Union[Iterator[pfs_proto.CommitInfo], Iterator[pfs_proto.CommitSetInfo]]
+        Union[Iterator[pfs_pb2.CommitInfo], Iterator[pfs_pb2.CommitSetInfo]]
             An iterator of protobuf objects that either contain info on a
             subcommit (commit at the repo-level), if `repo_name` was specified,
             or a commit, if `repo_name` wasn't specified.
 
         Examples
         --------
         >>> # all commits at repo-level
@@ -478,299 +541,314 @@
         >>>     print(c)
         ...
         >>> # all commits
         >>> commits = list(client.list_commit())
 
         .. # noqa: W505
         """
-        project = pfs_proto.Project(name=project_name) if project_name else None
+        project = pfs_pb2.Project(name=project_name) if project_name else None
         if repo_name is not None:
             if started_time is not None:
                 started_time = timestamp_pb2.Timestamp.FromDatetime(started_time)
-            req = pfs_proto.ListCommitRequest(
-                repo=pfs_proto.Repo(
+            message = pfs_pb2.ListCommitRequest(
+                repo=pfs_pb2.Repo(
                     name=repo_name,
                     type="user",
                     project=project,
                 ),
                 number=number,
                 reverse=reverse,
                 all=all,
                 origin_kind=origin_kind,
                 started_time=started_time,
             )
             if to_commit is not None:
-                req.to = commit_from(to_commit)
+                message.to.CopyFrom(commit_from(to_commit))
             if from_commit is not None:
-                req.from_ = commit_from(from_commit)
-            return self._req(Service.PFS, "ListCommit", req=req)
+                getattr(message, "from").CopyFrom(commit_from(from_commit))
+            return self.__stub.ListCommit(message)
         else:
-            return self._req(
-                Service.PFS,
-                "ListCommitSet",
-                project=project,
-            )
+            message = pfs_pb2.ListCommitSetRequest(project=project)
+            return self.__stub.ListCommitSet(message)
 
     def squash_commit(self, commit_id: str) -> None:
         """Squashes a commit into its parent.
 
         Parameters
         ----------
         commit_id : str
             The ID of the commit.
         """
-        self._req(
-            Service.PFS,
-            "SquashCommitSet",
-            commit_set=pfs_proto.CommitSet(id=commit_id),
+        message = pfs_pb2.SquashCommitSetRequest(
+            commit_set=pfs_pb2.CommitSet(id=commit_id)
         )
+        self.__stub.SquashCommitSet(message)
 
     def drop_commit(self, commit_id: str) -> None:
         """
         Drops an entire commit.
 
         Parameters
         ----------
         commit_id : str
             The ID of the commit.
         """
-        self._req(
-            Service.PFS,
-            "DropCommitSet",
-            commit_set=pfs_proto.CommitSet(id=commit_id),
+        message = pfs_pb2.DropCommitSetRequest(
+            commit_set=pfs_pb2.CommitSet(id=commit_id),
         )
+        self.__stub.DropCommitSet(message)
 
     def wait_commit(
-        self, commit: Union[str, tuple, dict, Commit, pfs_proto.Commit]
-    ) -> List[pfs_proto.CommitInfo]:
+        self, commit: Union[str, SubcommitType]
+    ) -> List[pfs_pb2.CommitInfo]:
         """Waits for the specified commit to finish.
 
         Parameters
         ----------
-        commit : Union[str, tuple, dict, Commit, pfs_proto.Commit]
+        commit : Union[str, SubcommitType]
             A commit object to wait on. Can either be an entire commit or a
             subcommit (commit at the repo-level).
 
         Returns
         -------
-        List[pfs_proto.CommitInfo]
+        List[pfs_pb2.CommitInfo]
             A list of protobuf objects that contain info on subcommits (commit
             at the repo-level). These are the individual subcommits this
             function waited on.
 
         Examples
         --------
         >>> # wait for an entire commit to finish
         >>> subcommits = client.wait_commit("467c580611234cdb8cc9758c7aa96087")
         ...
         >>> # wait for a commit to finish at a certain repo
         >>> client.wait_commit(("foo", "master"))
         """
-        return list(self.inspect_commit(commit, pfs_proto.CommitState.FINISHED))
+        return list(self.inspect_commit(commit, pfs_pb2.CommitState.FINISHED))
 
     def subscribe_commit(
         self,
         repo_name: str,
         branch: str,
-        from_commit: Union[str, tuple, dict, Commit, pfs_proto.Commit] = None,
-        state: pfs_proto.CommitState = pfs_proto.CommitState.STARTED,
+        from_commit: Union[str, SubcommitType] = None,
+        state: pfs_pb2.CommitState = pfs_pb2.CommitState.STARTED,
         all: bool = False,
-        origin_kind: pfs_proto.OriginKind = pfs_proto.OriginKind.USER,
+        origin_kind: pfs_pb2.OriginKind = pfs_pb2.OriginKind.USER,
         project_name: str = None,
-    ) -> Iterator[pfs_proto.CommitInfo]:
+    ) -> Iterator[pfs_pb2.CommitInfo]:
         """Returns all commits on the branch and then listens for new commits
         that are created.
 
         Parameters
         ----------
         repo_name : str
             The name of the repo.
         branch : str
             The name of the branch.
-        from_commit : Union[str, tuple, dict, Commit, pfs_proto.Commit], optional
+        from_commit : Union[str, SubcommitType], optional
             Return commits only from this commit and onwards. Can either be an
             entire commit or a subcommit (commit at the repo-level).
-        state : {pfs_proto.CommitState.STARTED, pfs_proto.CommitState.READY, pfs_proto.CommitState.FINISHING, pfs_proto.CommitState.FINISHED}, optional
+        state : {pfs_pb2.CommitState.STARTED, pfs_pb2.CommitState.READY, pfs_pb2.CommitState.FINISHING, pfs_pb2.CommitState.FINISHED}, optional
             Return commits only when they're at least in the specifed enum
-            state. (Default value = ``pfs_proto.CommitState.STARTED``)
+            state. (Default value = ``pfs_pb2.CommitState.STARTED``)
         all : bool, optional
             If true, returns all types of commits. Otherwise, alias commits are
             excluded.
-        origin_kind : {pfs_proto.OriginKind.USER, pfs_proto.OriginKind.AUTO, pfs_proto.OriginKind.FSCK, pfs_proto.OriginKind.ALIAS}, optional
+        origin_kind : {pfs_pb2.OriginKind.USER, pfs_pb2.OriginKind.AUTO, pfs_pb2.OriginKind.FSCK, pfs_pb2.OriginKind.ALIAS}, optional
             An enum that specifies how a commit originated. Returns only
-            commits of this enum type. (Default value = ``pfs_proto.OriginKind.USER``)
+            commits of this enum type. (Default value = ``pfs_pb2.OriginKind.USER``)
         project_name : str
             The name of the project.
 
         Returns
         -------
-        Iterator[pfs_proto.CommitInfo]
+        Iterator[pfs_pb2.CommitInfo]
             An iterator of protobuf objects that contain info on subcommits
             (commits at the repo-level). Use ``next()`` to iterate through as
             the returned stream is potentially endless. Might block your code
             otherwise.
 
         Examples
         --------
-        >>> commits = client.subscribe_commit("foo", "master", state=pfs_proto.CommitState.FINISHED)
+        >>> commits = client.subscribe_commit("foo", "master", state=pfs_pb2.CommitState.FINISHED)
         >>> c = next(commits)
 
         .. # noqa: W505
         """
-        repo = pfs_proto.Repo(
-            name=repo_name, type="user", project=pfs_proto.Project(name=project_name)
+        repo = pfs_pb2.Repo(
+            name=repo_name, type="user", project=pfs_pb2.Project(name=project_name)
         )
-        req = pfs_proto.SubscribeCommitRequest(
+        message = pfs_pb2.SubscribeCommitRequest(
             repo=repo,
             branch=branch,
             state=state,
             all=all,
             origin_kind=origin_kind,
         )
         if from_commit is not None:
             if isinstance(from_commit, str):
-                req.from_ = pfs_proto.Commit(repo=repo, id=from_commit)
+                getattr(message, "from").CopyFrom(
+                    pfs_pb2.Commit(repo=repo, id=from_commit)
+                )
             else:
-                req.from_ = commit_from(from_commit)
-        return self._req(Service.PFS, "SubscribeCommit", req=req)
+                getattr(message, "from").CopyFrom(commit_from(from_commit))
+        return self.__stub.SubscribeCommit(message)
+
+    def find_commits(
+        self, start: SubcommitType, file_path: str, limit: int = 0
+    ) -> Iterator[pfs_pb2.FindCommitsResponse]:
+        """Searches for commits that reference the specified file
+        being modified in a branch.
+
+        Parameters
+        ----------
+        start : SubcommitType
+            The commit where the search should begin.
+        file_path : str
+            The path to the file being queried.
+        limit: int, optional
+            The number of matching commits to return. (default no limit)
+        """
+        message = pfs_pb2.FindCommitsRequest(
+            start=start, file_path=file_path, limit=limit
+        )
+        for item in self.__stub.FinishCommit(message):
+            yield item
 
     def create_branch(
         self,
         repo_name: str,
         branch_name: str,
-        head_commit: Union[tuple, dict, Commit, pfs_proto.Commit] = None,
-        provenance: List[pfs_proto.Branch] = None,
-        trigger: pfs_proto.Trigger = None,
+        head_commit: SubcommitType = None,
+        provenance: List[pfs_pb2.Branch] = None,
+        trigger: pfs_pb2.Trigger = None,
         new_commit: bool = False,
         project_name: str = None,
     ) -> None:
         """Creates a new branch.
 
         Parameters
         ----------
         repo_name : str
             The name of the repo.
         branch_name : str
             The name of the new branch.
-        head_commit : Union[tuple, dict, Commit, pfs_proto.Commit], optional
+        head_commit : SubcommitType, optional
             A subcommit (commit at repo-level) indicating the head of the
             new branch.
-        provenance : List[pfs_proto.Branch], optional
+        provenance : List[pfs_pb2.Branch], optional
             A list of branches to establish provenance with this newly created
             branch.
-        trigger : pfs_proto.Trigger, optional
+        trigger : pfs_pb2.Trigger, optional
             Sets the conditions under which the head of this branch moves.
         new_commit : bool, optional
             If true and `head_commit` is specified, uses a different commit ID
             for head than `head_commit`.
         project_name : str
             The name of the project.
 
         Examples
         --------
         >>> client.create_branch(
         ...     "bar",
         ...     "master",
         ...     provenance=[
-        ...         pfs_proto.Branch(
-        ...             repo=pfs_proto.Repo(name="foo", type="user"), name="master"
+        ...         pfs_pb2.Branch(
+        ...             repo=pfs_pb2.Repo(name="foo", type="user"), name="master"
         ...         )
         ...     ]
         ... )
 
         .. # noqa: W505
         """
-        self._req(
-            Service.PFS,
-            "CreateBranch",
-            branch=pfs_proto.Branch(
+        message = pfs_pb2.CreateBranchRequest(
+            branch=pfs_pb2.Branch(
                 name=branch_name,
-                repo=pfs_proto.Repo(
+                repo=pfs_pb2.Repo(
                     name=repo_name,
                     type="user",
-                    project=pfs_proto.Project(name=project_name),
+                    project=pfs_pb2.Project(name=project_name),
                 ),
             ),
             head=commit_from(head_commit),
+            new_commit_set=new_commit,
             provenance=provenance,
             trigger=trigger,
-            new_commit_set=new_commit,
         )
+        self.__stub.CreateBranch(message)
 
     def inspect_branch(
         self,
         repo_name: str,
         branch_name: str,
         project_name: str = None,
-    ) -> pfs_proto.BranchInfo:
+    ) -> pfs_pb2.BranchInfo:
         """Inspects a branch.
 
         Parameters
         ----------
         repo_name : str
             The name of the repo.
         branch_name : str
             The name of the branch.
         project_name : str
             The name of the project.
 
         Returns
         -------
-        pfs_proto.BranchInfo
+        pfs_pb2.BranchInfo
             A protobuf object with info on a branch.
         """
-        return self._req(
-            Service.PFS,
-            "InspectBranch",
-            branch=pfs_proto.Branch(
+        message = pfs_pb2.InspectBranchRequest(
+            branch=pfs_pb2.Branch(
                 name=branch_name,
-                repo=pfs_proto.Repo(
+                repo=pfs_pb2.Repo(
                     name=repo_name,
                     type="user",
-                    project=pfs_proto.Project(name=project_name),
+                    project=pfs_pb2.Project(name=project_name),
                 ),
             ),
         )
+        return self.__stub.InspectBranch(message)
 
     def list_branch(
         self,
         repo_name: str,
         reverse: bool = False,
         project_name: str = None,
-    ) -> Iterator[pfs_proto.BranchInfo]:
+    ) -> Iterator[pfs_pb2.BranchInfo]:
         """Lists the active branch objects in a repo.
 
         Parameters
         ----------
         repo_name : str
             The name of the repo.
         reverse : bool, optional
             If true, returns branches oldest to newest.
         project_name : str
             The name of the project.
 
         Returns
         -------
-        Iterator[pfs_proto.BranchInfo]
+        Iterator[pfs_pb2.BranchInfo]
             An iterator of protobuf objects that contain info on a branch.
 
         Examples
         --------
         >>> branches = list(client.list_branch("foo"))
         """
-        return self._req(
-            Service.PFS,
-            "ListBranch",
-            repo=pfs_proto.Repo(
+        message = pfs_pb2.ListBranchRequest(
+            repo=pfs_pb2.Repo(
                 name=repo_name,
                 type="user",
-                project=pfs_proto.Project(name=project_name),
+                project=pfs_pb2.Project(name=project_name),
             ),
             reverse=reverse,
         )
+        return self.__stub.ListBranch(message)
 
     def delete_branch(
         self,
         repo_name: str,
         branch_name: str,
         force: bool = False,
         project_name: str = None,
@@ -786,40 +864,37 @@
         branch_name : str
             The name of the branch.
         force : bool, optional
             If true, forces the branch deletion.
         project_name : str
             The name of the project.
         """
-        self._req(
-            Service.PFS,
-            "DeleteBranch",
-            branch=pfs_proto.Branch(
+        message = pfs_pb2.DeleteBranchRequest(
+            branch=pfs_pb2.Branch(
                 name=branch_name,
-                repo=pfs_proto.Repo(
+                repo=pfs_pb2.Repo(
                     name=repo_name,
                     type="user",
-                    project=pfs_proto.Project(name=project_name),
+                    project=pfs_pb2.Project(name=project_name),
                 ),
             ),
             force=force,
         )
+        self.__stub.DeleteBranch(message)
 
     @contextmanager
-    def modify_file_client(
-        self, commit: Union[tuple, dict, Commit, pfs_proto.Commit]
-    ) -> Iterator["ModifyFileClient"]:
+    def modify_file_client(self, commit: SubcommitType) -> Iterator["ModifyFileClient"]:
         """A context manager that gives a :class:`.ModifyFileClient`. When the
         context manager exits, any operations enqueued from the
         :class:`.ModifyFileClient` are executed in a single, atomic
         ModifyFile gRPC call.
 
         Parameters
         ----------
-        commit : Union[tuple, dict, Commit, pfs_proto.Commit]
+        commit : Union[tuple, dict, Commit, pfs_pb2.Commit]
             A subcommit (commit at the repo-level) to modify. If this subcommit
             is opened before ``modify_file_client()`` is called, it will remain
             open after. If ``modify_file_client()`` opens the subcommit, it
             will close when exiting the ``with`` scope.
 
         Yields
         -------
@@ -846,30 +921,31 @@
         >>>     mfc.put_file_from_url(
         ...         "/new_file.txt",
         ...         "https://example.com/data/train/input.txt"
         ...     )
         """
         mfc = ModifyFileClient(commit)
         yield mfc
-        self._req(Service.PFS, "ModifyFile", req=mfc._reqs())
+        messages = mfc._reqs()
+        self.__stub.ModifyFile(messages)
 
     def put_file_bytes(
         self,
-        commit: Union[tuple, dict, Commit, pfs_proto.Commit],
+        commit: SubcommitType,
         path: str,
         value: Union[bytes, BinaryIO],
         datum: str = None,
         append: bool = False,
     ) -> None:
         """Uploads a PFS file from a file-like object, bytestring, or iterator
         of bytestrings.
 
         Parameters
         ----------
-        commit : Union[tuple, dict, Commit, pfs_proto.Commit]
+        commit : SubcommitType
             An open subcommit (commit at the repo-level) to modify.
         path : str
             The path in the repo the file(s) will be written to.
         value : Union[bytes, BinaryIO]
             The file contents as bytes, represented as a file-like object,
             bytestring, or iterator of bystrings.
         datum : str, optional
@@ -900,40 +976,44 @@
                     value,
                     datum=datum,
                     append=append,
                 )
 
     def put_file_url(
         self,
-        commit: Union[tuple, dict, Commit, pfs_proto.Commit],
+        commit: SubcommitType,
         path: str,
         url: str,
         recursive: bool = False,
         datum: str = None,
         append: bool = False,
+        concurrency: int = 0,
     ) -> None:
         """Uploads a PFS file using the content found at a URL. The URL is sent
         to the server which performs the request.
 
         Parameters
         ----------
-        commit : Union[tuple, dict, Commit, pfs_proto.Commit]
+        commit : SubcommitType
             An open subcommit (commit at the repo-level) to modify.
         path : str
             The path in the repo the file(s) will be written to.
         url : str
             The URL of the file to put.
         recursive : bool, optional
             If true, allows for recursive scraping on some types URLs, for
             example on s3:// URLs
         datum : str, optional
             A tag for the added file(s).
         append : bool, optional
             If true, appends the data to the file(s) specified at `path`, if
             they already exist. Otherwise, overwrites them.
+        concurrency : int
+            The maximum number of threads used to complete the request.
+            Defaults to 50.
 
         Examples
         --------
         Commit needs to be open still, either from the result of
         ``start_commit()`` or within scope of ``commit()``
 
         >>> with client.commit("foo", "master") as c:
@@ -946,37 +1026,38 @@
         with self.modify_file_client(commit) as mfc:
             mfc.put_file_from_url(
                 path,
                 url,
                 recursive=recursive,
                 datum=datum,
                 append=append,
+                concurrency=concurrency,
             )
 
     def copy_file(
         self,
-        source_commit: Union[tuple, dict, Commit, pfs_proto.Commit],
+        source_commit: SubcommitType,
         source_path: str,
-        dest_commit: Union[tuple, dict, Commit, pfs_proto.Commit],
+        dest_commit: SubcommitType,
         dest_path: str,
         datum: str = None,
         append: bool = False,
     ) -> None:
         """Efficiently copies files already in PFS. Note that the destination
         repo cannot be an output repo, or the copy operation will silently
         fail.
 
         Parameters
         ----------
-        source_commit : Union[tuple, dict, Commit, pfs_proto.Commit]
+        source_commit : SubcommitType
             The subcommit (commit at the repo-level) which holds the source
             file.
         source_path : str
             The path of the source file.
-        dest_commit : Union[tuple, dict, Commit, pfs_proto.Commit]
+        dest_commit : SubcommitType
             The open subcommit (commit at the repo-level) to which to add the
             file.
         dest_path : str
             The path of the destination file.
         datum : str, optional
             A tag for the added file.
         append : bool, optional
@@ -996,61 +1077,61 @@
         with self.modify_file_client(dest_commit) as mfc:
             mfc.copy_file(
                 source_commit, source_path, dest_path, datum=datum, append=append
             )
 
     def get_file(
         self,
-        commit: Union[tuple, dict, Commit, pfs_proto.Commit],
+        commit: SubcommitType,
         path: str,
         datum: str = None,
         URL: str = None,
         offset: int = 0,
     ) -> PFSFile:
         """Gets a file from PFS.
 
         Parameters
         ----------
-        commit : Union[tuple, dict, Commit, pfs_proto.Commit]
+        commit : SubcommitType
             The subcommit (commit at the repo-level) to get the file from.
         path : str
             The path of the file.
         datum : str, optional
             A tag that filters the files.
         URL : str, optional
             Specifies an object storage URL that the file will be uploaded to.
         offset : int, optional
             Allows file read to begin at `offset` number of bytes.
+
         Returns
         -------
         PFSFile
             The contents of the file in a file-like object.
         """
-        stream = self._req(
-            Service.PFS,
-            "GetFile",
-            file=pfs_proto.File(commit=commit_from(commit), path=path, datum=datum),
+        message = pfs_pb2.GetFileRequest(
+            file=pfs_pb2.File(commit=commit_from(commit), path=path, datum=datum),
             URL=URL,
             offset=offset,
         )
+        stream = self.__stub.GetFile(message)
         return PFSFile(stream)
 
     def get_file_tar(
         self,
-        commit: Union[tuple, dict, Commit, pfs_proto.Commit],
+        commit: SubcommitType,
         path: str,
         datum: str = None,
         URL: str = None,
         offset: int = 0,
     ) -> PFSTarFile:
         """Gets a file from PFS.
 
         Parameters
         ----------
-        commit : Union[tuple, dict, Commit, pfs_proto.Commit]
+        commit : SubcommitType
             The subcommit (commit at the repo-level) to get the file from.
         path : str
             The path of the file.
         datum : str, optional
             A tag that filters the files.
         URL : str, optional
             Specifies an object storage URL that the file will be uploaded to.
@@ -1058,67 +1139,63 @@
             Allows file read to begin at `offset` number of bytes.
 
         Returns
         -------
         PFSFile
             The contents of the file in a file-like object.
         """
-        stream = self._req(
-            Service.PFS,
-            "GetFileTAR",
-            req=pfs_proto.GetFileRequest(
-                file=pfs_proto.File(commit=commit_from(commit), path=path, datum=datum),
-                url=URL,
-                offset=offset,
-            ),
+        message = pfs_pb2.GetFileRequest(
+            file=pfs_pb2.File(commit=commit_from(commit), path=path, datum=datum),
+            URL=URL,
+            offset=offset,
         )
+        stream = self.__stub.GetFileTAR(message)
         return PFSTarFile.open(fileobj=PFSFile(stream), mode="r|*")
 
     def inspect_file(
         self,
-        commit: Union[tuple, dict, Commit, pfs_proto.Commit],
+        commit: SubcommitType,
         path: str,
         datum: str = None,
-    ) -> pfs_proto.FileInfo:
+    ) -> pfs_pb2.FileInfo:
         """Inspects a file.
 
         Parameters
         ----------
-        commit : Union[tuple, dict, Commit, pfs_proto.Commit]
+        commit : SubcommitType
             The subcommit (commit at the repo-level) to inspect the file from.
         path : str
             The path of the file.
         datum : str, optional
             A tag that filters the files.
 
         Returns
         -------
-        pfs_proto.FileInfo
+        pfs_pb2.FileInfo
             A protobuf object that contains info on a file.
         """
-        return self._req(
-            Service.PFS,
-            "InspectFile",
-            file=pfs_proto.File(commit=commit_from(commit), path=path, datum=datum),
+        message = pfs_pb2.InspectFileRequest(
+            file=pfs_pb2.File(commit=commit_from(commit), path=path, datum=datum),
         )
+        return self.__stub.InspectFile(message)
 
     def list_file(
         self,
-        commit: Union[tuple, dict, Commit, pfs_proto.Commit],
+        commit: SubcommitType,
         path: str,
         datum: str = None,
-        pagination_marker: pfs_proto.File = None,
+        pagination_marker: pfs_pb2.File = None,
         number: int = None,
         reverse: bool = False,
-    ) -> Iterator[pfs_proto.FileInfo]:
+    ) -> Iterator[pfs_pb2.FileInfo]:
         """Lists the files in a directory.
 
         Parameters
         ----------
-        commit : Union[tuple, dict, Commit, pfs_proto.Commit]
+        commit : SubcommitType
             The subcommit (commit at the repo-level) to list files from.
         path : str
             The path to the directory.
         datum : str, optional
             A tag that filters the files.
         pagination_marker:
             Marker for pagination. If set, the files that come after the marker
@@ -1128,121 +1205,115 @@
         number : int, optional
             Number of files to return
         reverse : bool, optional
             If true, return files in reverse order
 
         Returns
         -------
-        Iterator[pfs_proto.FileInfo]
+        Iterator[pfs_pb2.FileInfo]
             An iterator of protobuf objects that contain info on files.
 
         Examples
         --------
         >>> files = list(client.list_file(("foo", "master"), "/dir/subdir/"))
         """
-        return self._req(
-            Service.PFS,
-            "ListFile",
-            file=pfs_proto.File(commit=commit_from(commit), path=path, datum=datum),
+        message = pfs_pb2.ListFileRequest(
+            file=pfs_pb2.File(commit=commit_from(commit), path=path, datum=datum),
             paginationMarker=pagination_marker,
             number=number,
             reverse=reverse,
         )
+        return self.__stub.ListFile(message)
 
     def walk_file(
         self,
-        commit: Union[tuple, dict, Commit, pfs_proto.Commit],
+        commit: SubcommitType,
         path: str,
         datum: str = None,
-        pagination_marker: pfs_proto.File = None,
+        pagination_marker: pfs_pb2.File = None,
         number: int = None,
         reverse: bool = False,
-    ) -> Iterator[pfs_proto.FileInfo]:
+    ) -> Iterator[pfs_pb2.FileInfo]:
         """Walks over all descendant files in a directory.
 
         Parameters
         ----------
-        commit : Union[tuple, dict, Commit, pfs_proto.Commit]
+        commit : SubcommitType
             The subcommit (commit at the repo-level) to walk files in.
         path : str
             The path to the directory.
         datum : str, optional
             A tag that filters the files.
         pagination_marker:
             Marker for pagination. If set, the files that come after the marker
             in lexicographical order will be returned. If reverse is also set,
             the files that come before the marker in lexicographical order will
             be returned.
         number : int, optional
             Number of files to return
         reverse : bool, optional
             If true, return files in reverse order
-
         Returns
         -------
-        Iterator[pfs_proto.FileInfo]
+        Iterator[pfs_pb2.FileInfo]
             An iterator of protobuf objects that contain info on files.
 
         Examples
         --------
         >>> files = list(client.walk_file(("foo", "master"), "/dir/subdir/"))
         """
-        return self._req(
-            Service.PFS,
-            "WalkFile",
-            file=pfs_proto.File(commit=commit_from(commit), path=path, datum=datum),
+        message = pfs_pb2.WalkFileRequest(
+            file=pfs_pb2.File(commit=commit_from(commit), path=path, datum=datum),
             paginationMarker=pagination_marker,
             number=number,
             reverse=reverse,
         )
+        return self.__stub.WalkFile(message)
 
     def glob_file(
         self,
-        commit: Union[tuple, dict, Commit, pfs_proto.Commit],
+        commit: SubcommitType,
         pattern: str,
-        path_range: pfs_proto.PathRange = None,
-    ) -> Iterator[pfs_proto.FileInfo]:
+        path_range: pfs_pb2.PathRange = None,
+    ) -> Iterator[pfs_pb2.FileInfo]:
         """Lists files that match a glob pattern.
 
         Parameters
         ----------
-        commit : Union[tuple, dict, Commit, pfs_proto.Commit]
+        commit : SubcommitType
             The subcommit (commit at the repo-level) to query against.
         pattern : str
             A glob pattern.
 
         Returns
         -------
-        Iterator[pfs_proto.FileInfo]
+        Iterator[pfs_pb2.FileInfo]
             An iterator of protobuf objects that contain info on files.
 
         Examples
         --------
         >>> files = list(client.glob_file(("foo", "master"), "/*.txt"))
         """
-        return self._req(
-            Service.PFS,
-            "GlobFile",
+        message = pfs_pb2.GlobFileRequest(
             commit=commit_from(commit),
             pattern=pattern,
             path_range=path_range,
         )
+        return self.__stub.GlobFile(message)
 
-    def delete_file(
-        self, commit: Union[tuple, dict, Commit, pfs_proto.Commit], path: str
-    ) -> None:
+    def delete_file(self, commit: SubcommitType, path: str) -> None:
         """Deletes a file from an open commit. This leaves a tombstone in the
         commit, assuming the file isn't written to later while the commit is
         still open. Attempting to get the file from the finished commit will
         result in a not found error. The file will of course remain intact in
         the commit's parent.
 
         Parameters
         ----------
-        commit : Union[tuple, dict, Commit, pfs_proto.Commit]
+        commit : SubcommitType
             The open subcommit (commit at the repo-level) to delete a file
             from.
         path : str
             The path to the file.
 
         Examples
         --------
@@ -1251,68 +1322,69 @@
 
         >>> with client.commit("bar", "master") as c:
         >>>     client.delete_file(c, "/delete_me.txt")
         """
         with self.modify_file_client(commit) as mfc:
             mfc.delete_file(path)
 
-    def fsck(self, fix: bool = False) -> Iterator[pfs_proto.FsckResponse]:
+    def fsck(self, fix: bool = False) -> Iterator[pfs_pb2.FsckResponse]:
         """Performs a file system consistency check on PFS, ensuring the
         correct provenance relationships are satisfied.
 
         Parameters
         ----------
         fix : bool, optional
             If true, attempts to fix as many problems as possible.
 
         Returns
         -------
-        Iterator[pfs_proto.FsckResponse]
+        Iterator[pfs_pb2.FsckResponse]
             An iterator of protobuf objects that contain info on either what
             error was encountered (and was unable to be fixed, if `fix` is set
             to ``True``) or a fix message (if `fix` is set to ``True``).
 
         Examples
         --------
         >>> for action in client.fsck(True):
         >>>     print(action)
         """
-        return self._req(Service.PFS, "Fsck", fix=fix)
+        message = pfs_pb2.FsckRequest(fix=fix)
+        return self.__stub.Fsck(message)
 
     def diff_file(
         self,
-        new_commit: Union[tuple, dict, Commit, pfs_proto.Commit],
+        new_commit: SubcommitType,
         new_path: str,
-        old_commit: Union[tuple, dict, Commit, pfs_proto.Commit] = None,
+        old_commit: SubcommitType = None,
         old_path: str = None,
         shallow: bool = False,
-    ) -> Iterator[pfs_proto.DiffFileResponse]:
+    ) -> Iterator[pfs_pb2.DiffFileResponse]:
         """Diffs two PFS files (file = commit + path in Pachyderm) and returns
         files that are different. Similar to ``git diff``.
 
         If `old_commit` or `old_path` are not specified, `old_commit` will be
         set to the parent of `new_commit` and `old_path` will be set to
         `new_path`.
 
         Parameters
         ----------
-        new_commit : Union[tuple, dict, Commit, pfs_proto.Commit]
+        new_commit : SubcommitType
             The newer subcommit (commit at the repo-level).
         new_path : str
             The path in `new_commit` to compare with.
-        old_commit : Union[tuple, dict, Commit, pfs_proto.Commit], optional
+        old_commit : SubcommitType, optional
             The older subcommit (commit at the repo-level).
         old_path : str, optional
             The path in `old_commit` to compare with.
         shallow : bool, optional
             Unused.
 
         Returns
         -------
-        Iterator[pfs_proto.DiffFileResponse]
+        Iterator[pfs_pb2.DiffFileResponse]
             An iterator of protobuf objects that contain info on files whose
             content has changed between commits. If a file under one of the
             paths is only in one commit, than the ``DiffFileResponse`` for it
             will only have one ``FileInfo`` set.
 
         Examples
         --------
@@ -1331,35 +1403,32 @@
         ...     "/a/",
         ...     ("foo", "master~2"),
         ...     "/a/"
         ... )
         >>> diff = next(res)
         """
         if old_commit is not None and old_path is not None:
-            old_file = pfs_proto.File(commit=commit_from(old_commit), path=old_path)
+            old_file = pfs_pb2.File(commit=commit_from(old_commit), path=old_path)
         else:
             old_file = None
 
-        return self._req(
-            Service.PFS,
-            "DiffFile",
-            new_file=pfs_proto.File(commit=commit_from(new_commit), path=new_path),
+        message = pfs_pb2.DiffFileRequest(
+            new_file=pfs_pb2.File(commit=commit_from(new_commit), path=new_path),
             old_file=old_file,
             shallow=shallow,
         )
+        return self.__stub.DiffFile(message)
 
-    def path_exists(
-        self, commit: Union[tuple, dict, Commit, pfs_proto.Commit], path: str
-    ) -> bool:
+    def path_exists(self, commit: SubcommitType, path: str) -> bool:
         """Checks whether the path exists in the specified commit, agnostic to
         whether `path` is a file or a directory.
 
         Parameters
         ----------
-        commit : Union[tuple, dict, Commit, pfs_proto.Commit]
+        commit : SubcommitType
             The subcommit (commit at the repo-level) to check in.
         path : str
             The file or directory path in `commit`.
 
         Returns
         -------
         bool
@@ -1376,115 +1445,26 @@
                 return False
             elif invalid_commit_re.match(e.details()):
                 raise ValueError("bad argument: nonexistent commit provided")
             raise e
 
         return True
 
-    def mount(self, mount_dir: str, repos: List[str] = []) -> None:
-        """Mounts Pachyderm repos locally.
-
-        Parameters
-        ----------
-        mount_dir : str
-            The directory to mount repos to. Make sure if this folder already
-            exists that it's empty (including hidden files).
-        repos : List[str], optional
-            The repos to mount. Each repo can only be mounted once, even if
-            multiple branches are passed. If empty, all repos are mounted.
-
-        Notes
-        -----
-        Mounting uses FUSE, which causes some known issues on macOS. For the
-        best experience, we recommend using mount on Linux. We do not support
-        mounting on macOS 1.11 and later.
-
-        Additionally, we recommend using mount in read-only access.
-
-        Examples
-        --------
-        >>> client.mount("dir_a", ["repo1", "repo2@staging"])
-        """
-        check_pachctl()
-        Path(mount_dir).mkdir(parents=True, exist_ok=True)
-
-        subprocess.run(
-            ["sudo", "pachctl", "unmount", mount_dir],
-            stdout=subprocess.DEVNULL,
-            stderr=subprocess.STDOUT,
-        )
-
-        # Check for non-empty mount dir
-        mount_dir_contents = next(os.walk(mount_dir))
-        if mount_dir_contents[1] or mount_dir_contents[2]:
-            raise RuntimeError(
-                f"{mount_dir} must be empty to mount (including hidden files)"
-            )
-
-        # If 0 Pachyderm repos, no need to mount
-        if not list(self.list_repo()):
-            print("no repos in Pachyderm to mount")
-            return
-
-        cmd = ["pachctl", "mount", mount_dir]
-        for r in repos:
-            cmd.append("-r")
-            cmd.append(r)
-
-        subprocess.Popen(cmd, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
-
-        # Ensure mount has finished
-        for _ in range(3):
-            time.sleep(0.25)
-            mounted_repos = next(os.walk(mount_dir))[1]
-
-            if mounted_repos:
-                return
-
-        self.unmount(mount_dir)
-        raise RuntimeError(
-            "mount failed to expose data after three read attempts (0.75s)"
-        )
-
-    def unmount(self, mount_dir: str = None, *, all_mounts: bool = False) -> None:
-        """Unmounts mounted local filesystems with Pachyderm repos.
-
-        Parameters
-        ----------
-        mount_dir : str, optional
-            The mounted directory to unmount.
-        all_mounts : bool, optional
-            If ``True``, unmounts all mounted directories.
-
-        Examples
-        --------
-        >>> client.unmount("dir_a")
-        ...
-        >>> client.unmount(all_mounts=True)
-        """
-        check_pachctl()
-        if mount_dir is not None:
-            subprocess.run(["sudo", "pachctl", "unmount", mount_dir])
-        elif all_mounts:
-            subprocess.run(["sudo", "pachctl", "unmount", "-a"], input=b"y\n")
-        else:
-            print("no repos unmounted, pass arguments or see documentation")
-
 
 class ModifyFileClient:
     """:class:`.ModifyFileClient` puts or deletes PFS files atomically.
     Replaces :class:`.PutFileClient` from python_pachyderm 6.x.
     """
 
-    def __init__(self, commit: Union[tuple, dict, Commit, pfs_proto.Commit]):
+    def __init__(self, commit: SubcommitType):
         self._ops = []
-        self.commit = Commit.from_bp(commit_from(commit)).to_pb()
+        self.commit = commit_from(commit)
 
-    def _reqs(self) -> Iterator[pfs_proto_pb.ModifyFileRequest]:
-        yield pfs_proto_pb.ModifyFileRequest(set_commit=self.commit)
+    def _reqs(self) -> Iterator[pfs_pb2.ModifyFileRequest]:
+        yield pfs_pb2.ModifyFileRequest(set_commit=self.commit)
         for op in self._ops:
             yield from op.reqs()
 
     def put_file_from_filepath(
         self,
         pfs_path: str,
         local_path: str,
@@ -1578,14 +1558,15 @@
     def put_file_from_url(
         self,
         path: str,
         url: str,
         datum: str = None,
         append: bool = False,
         recursive: bool = False,
+        concurrency: int = 0,
     ) -> None:
         """Uploads a PFS File from the content found at a URL. The URL is
         sent to the server which performs the request.
 
         Parameters
         ----------
         path : str
@@ -1596,22 +1577,26 @@
             A tag for the added file.
         append : bool, optional
             If true, appends the content to the file at `path`, if it
             already exists. Otherwise, overwrites the file.
         recursive : bool, optional
             If true, allows for recursive scraping on some types URLs, for
             example on s3:// URLs
+        concurrency : int
+            The maximum number of threads used to complete the request.
+            Defaults to 50.
         """
         self._ops.append(
             _AtomicModifyFileURLOp(
                 path,
                 url,
                 datum=datum,
                 append=append,
                 recursive=recursive,
+                concurrency=concurrency,
             )
         )
 
     def delete_file(self, path: str, datum: str = None) -> None:
         """Deletes a file.
 
         Parameters
@@ -1621,25 +1606,25 @@
         datum : str, optional
             A tag that filters the files.
         """
         self._ops.append(_AtomicDeleteFileOp(path, datum=datum))
 
     def copy_file(
         self,
-        source_commit: Union[tuple, dict, Commit, pfs_proto.Commit],
+        source_commit: SubcommitType,
         source_path: str,
         dest_path: str,
         datum: str = None,
         append: bool = False,
     ) -> None:
         """Copy a file.
 
         Parameters
         ----------
-        source_commit : Union[tuple, dict, Commit, pfs_proto.Commit]
+        source_commit : SubcommitType
             The commit the source file is in.
         source_path : str
             The path to the source file.
         dest_path : str
             The path to the destination file.
         datum : str, optional
             A tag for the added file.
@@ -1682,15 +1667,15 @@
     def __init__(
         self, pfs_path: str, local_path: str, datum: str = None, append: bool = False
     ):
         super().__init__(pfs_path, datum)
         self.local_path = local_path
         self.append = append
 
-    def reqs(self) -> Iterator[pfs_proto_pb.ModifyFileRequest]:
+    def reqs(self) -> Iterator[pfs_pb2.ModifyFileRequest]:
         if not self.append:
             yield _delete_file_req(self.path, self.datum)
         with open(self.local_path, "rb") as f:
             yield _add_file_req(path=self.path, datum=self.datum)
             for _, chunk in enumerate(f):
                 yield _add_file_req(path=self.path, datum=self.datum, chunk=chunk)
 
@@ -1701,15 +1686,15 @@
     def __init__(
         self, path: str, fobj: BinaryIO, datum: str = None, append: bool = False
     ):
         super().__init__(path, datum)
         self.fobj = fobj
         self.append = append
 
-    def reqs(self) -> Iterator[pfs_proto_pb.ModifyFileRequest]:
+    def reqs(self) -> Iterator[pfs_pb2.ModifyFileRequest]:
         if not self.append:
             yield _delete_file_req(self.path, self.datum)
         yield _add_file_req(path=self.path, datum=self.datum)
         for _ in itertools.count():
             chunk = self.fobj.read(BUFFER_SIZE)
             if len(chunk) == 0:
                 return
@@ -1722,59 +1707,62 @@
     def __init__(
         self,
         path: str,
         url: str,
         datum: str = None,
         append: bool = False,
         recursive: bool = False,
+        concurrency: int = 0,
     ):
         super().__init__(path, datum)
         self.url = url
         self.recursive = recursive
         self.append = append
+        self.concurrency = concurrency
 
-    def reqs(self) -> Iterator[pfs_proto_pb.ModifyFileRequest]:
+    def reqs(self) -> Iterator[pfs_pb2.ModifyFileRequest]:
         if not self.append:
             yield _delete_file_req(self.path, self.datum)
-        yield pfs_proto_pb.ModifyFileRequest(
-            add_file=pfs_proto_pb.AddFile(
+        yield pfs_pb2.ModifyFileRequest(
+            add_file=pfs_pb2.AddFile(
                 path=self.path,
                 datum=self.datum,
-                url=pfs_proto_pb.AddFile.URLSource(
+                url=pfs_pb2.AddFile.URLSource(
                     URL=self.url,
                     recursive=self.recursive,
+                    concurrency=self.concurrency,
                 ),
             ),
         )
 
 
 class _AtomicCopyFileOp(_AtomicOp):
     """A `ModifyFile` operation to copy a file."""
 
     def __init__(
         self,
-        source_commit: Union[tuple, dict, Commit, pfs_proto.Commit],
+        source_commit: SubcommitType,
         source_path: str,
         dest_path: str,
         datum: str = None,
         append: bool = False,
     ):
         super().__init__(dest_path, datum)
-        self.source_commit = Commit.from_bp(commit_from(source_commit)).to_pb()
+        self.source_commit = commit_from(source_commit)
         self.source_path = source_path
         self.dest_path = dest_path
         self.append = append
 
-    def reqs(self) -> Iterator[pfs_proto_pb.ModifyFileRequest]:
-        yield pfs_proto_pb.ModifyFileRequest(
-            copy_file=pfs_proto_pb.CopyFile(
+    def reqs(self) -> Iterator[pfs_pb2.ModifyFileRequest]:
+        yield pfs_pb2.ModifyFileRequest(
+            copy_file=pfs_pb2.CopyFile(
                 append=self.append,
                 datum=self.datum,
                 dst=self.dest_path,
-                src=pfs_proto_pb.File(commit=self.source_commit, path=self.source_path),
+                src=pfs_pb2.File(commit=self.source_commit, path=self.source_path),
             ),
         )
 
 
 class _AtomicDeleteFileOp(_AtomicOp):
     """A `ModifyFile` operation to delete a file."""
 
@@ -1782,20 +1770,18 @@
         super().__init__(pfs_path, datum)
 
     def reqs(self):
         yield _delete_file_req(self.path, self.datum)
 
 
 def _add_file_req(path: str, datum: str = None, chunk: bytes = None):
-    return pfs_proto_pb.ModifyFileRequest(
-        add_file=pfs_proto_pb.AddFile(
-            path=path,
-            datum=datum,
-            raw=wrappers_pb2.BytesValue(value=chunk),
+    return pfs_pb2.ModifyFileRequest(
+        add_file=pfs_pb2.AddFile(
+            path=path, datum=datum, raw=wrappers_pb2.BytesValue(value=chunk)
         ),
     )
 
 
 def _delete_file_req(path: str, datum: str = None):
-    return pfs_proto_pb.ModifyFileRequest(
-        delete_file=pfs_proto_pb.DeleteFile(path=path, datum=datum)
+    return pfs_pb2.ModifyFileRequest(
+        delete_file=pfs_pb2.DeleteFile(path=path, datum=datum)
     )
```

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/mixin/pps.py` & `python_pachyderm-7.5.0/src/python_pachyderm/mixin/pps.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 import json
 import base64
-import datetime
+from datetime import timedelta
 from typing import Dict, Iterator, List, Union
 
 try:
     from collections.abc import Iterable
 except ImportError:
     from collections import Iterable
 
-from python_pachyderm.experimental.pfs import commit_from, Commit
-from python_pachyderm.service import Service
-from python_pachyderm.experimental.service import pps_proto, pfs_proto
+import grpc
 from google.protobuf import empty_pb2, duration_pb2
-import betterproto.lib.google.protobuf as bp_proto
 
-# bp_to_pb: bp_proto.Empty -> empty_pb2.Empty
-# bp_to_pb: PfsInput -> PFSInput, datetime.timedelta -> duration_pb2.Duration
+from python_pachyderm.pfs import commit_from, SubcommitType
+from python_pachyderm.proto.v2.pfs import pfs_pb2
+from python_pachyderm.proto.v2.pps import pps_pb2, pps_pb2_grpc
 
 
 class PPSMixin:
     """A mixin for pps-related functionality."""
 
+    _channel: grpc.Channel
+
+    def __init__(self):
+        self.__stub = pps_pb2_grpc.APIStub(self._channel)
+        super().__init__()
+
     def inspect_job(
         self,
         job_id: str,
         pipeline_name: str = None,
         wait: bool = False,
         details: bool = False,
         project_name: str = None,
-    ) -> Iterator[pps_proto.JobInfo]:
+    ) -> Iterator[pps_pb2.JobInfo]:
         """Inspects a job.
 
         Parameters
         ----------
         job_id : str
             The ID of the job.
         pipeline_name : str, optional
@@ -42,76 +46,70 @@
         details : bool, optional
             If true, return worker details.
         project_name : str
             The name of the project.
 
         Returns
         -------
-        Iterator[pps_proto.JobInfo]
+        Iterator[pps_pb2.JobInfo]
             An iterator of protobuf objects that contain info on a subjob
             (jobs at the pipeline-level).
 
         Examples
         --------
         >>> # Look at all subjobs in a job
         >>> subjobs = list(client.inspect_job("467c580611234cdb8cc9758c7aa96087"))
         ...
         >>> # Look at single subjob (job at the pipeline-level)
         >>> subjob = list(client.inspect_job("467c580611234cdb8cc9758c7aa96087", "foo"))[0]
 
         .. # noqa: W505
         """
         if pipeline_name is not None:
-            return iter(
-                [
-                    self._req(
-                        Service.PPS,
-                        "InspectJob",
-                        job=pps_proto.Job(
-                            pipeline=pps_proto.Pipeline(
-                                name=pipeline_name,
-                                project=pfs_proto.Project(name=project_name),
-                            ),
-                            id=job_id,
-                        ),
-                        wait=wait,
-                        details=details,
-                    )
-                ]
+            message = pps_pb2.InspectJobRequest(
+                details=details,
+                job=pps_pb2.Job(
+                    pipeline=pps_pb2.Pipeline(
+                        name=pipeline_name,
+                        project=pfs_pb2.Project(name=project_name),
+                    ),
+                    id=job_id,
+                ),
+                wait=wait,
             )
+            return iter([self.__stub.InspectJob(message)])
         else:
-            return self._req(
-                Service.PPS,
-                "InspectJobSet",
-                job_set=pps_proto.JobSet(id=job_id),
-                wait=wait,
+            message = pps_pb2.InspectJobSetRequest(
                 details=details,
+                job_set=pps_pb2.JobSet(id=job_id),
+                wait=wait,
             )
+            return self.__stub.InspectJobSet(message)
 
     def list_job(
         self,
         pipeline_name: str = None,
-        input_commit: Union[tuple, dict, Commit, pfs_proto.Commit, List] = None,
+        input_commit: SubcommitType = None,
         history: int = 0,
         details: bool = False,
         jqFilter: str = None,
         project_name: str = None,
         projects_filter: List[str] = None,
-        pagination_marker: pfs_proto.File = None,
+        pagination_marker: pfs_pb2.File = None,
         number: int = None,
         reverse: bool = False,
-    ) -> Union[Iterator[pps_proto.JobInfo], Iterator[pps_proto.JobSetInfo]]:
+    ) -> Union[Iterator[pps_pb2.JobInfo], Iterator[pps_pb2.JobSetInfo]]:
         """Lists jobs.
 
         Parameters
         ----------
         pipeline_name : str, optional
             The name of a pipeline. If set, returns subjobs (job at the
             pipeline-level) only from this pipeline.
-        input_commit : Union[tuple, dict, Commit, pfs_proto.Commit, List], optional
+        input_commit : SubcommitType, optional
             A commit or list of commits from the input repo to filter jobs on.
             Only impacts returned results if `pipeline_name` is specified.
         history : int, optional
             Indicates to return jobs from historical versions of
             `pipeline_name`. Semantics are:
 
             - 0: Return jobs from the current version of `pipeline_name`
@@ -139,15 +137,15 @@
         number : int, optional
             Number of files to return
         reverse : bool, optional
             If true, return files in reverse order
 
         Returns
         -------
-        Union[Iterator[pps_proto.JobInfo], Iterator[pps_proto.JobSetInfo]]
+        Union[Iterator[pps_pb2.JobInfo], Iterator[pps_pb2.JobSetInfo]]
             An iterator of protobuf objects that either contain info on a
             subjob (job at the pipeline-level), if `pipeline_name` was
             specified, or a job, if `pipeline_name` wasn't specified.
 
         Examples
         --------
         >>> # List all jobs
@@ -155,46 +153,43 @@
         ...
         >>> # List all jobs at a pipeline-level
         >>> subjobs = list(client.list_job("foo"))
 
         .. # noqa: W505
         """
         if isinstance(projects_filter, Iterable):
-            projects_filter = [pfs_proto.Project(name=p.name) for p in projects_filter]
+            projects_filter = [pfs_pb2.Project(name=p.name) for p in projects_filter]
         if pipeline_name is not None:
             if isinstance(input_commit, list):
                 input_commit = [commit_from(ic) for ic in input_commit]
             elif input_commit is not None:
                 input_commit = [commit_from(input_commit)]
-
-            return self._req(
-                Service.PPS,
-                "ListJob",
-                pipeline=pps_proto.Pipeline(
-                    name=pipeline_name, project=pfs_proto.Project(name=project_name)
-                ),
-                input_commit=input_commit,
-                history=history,
+            message = pps_pb2.ListJobRequest(
                 details=details,
+                history=history,
+                input_commit=input_commit,
                 jqFilter=jqFilter,
+                pipeline=pps_pb2.Pipeline(
+                    name=pipeline_name, project=pfs_pb2.Project(name=project_name)
+                ),
                 projects=projects_filter,
                 paginationMarker=pagination_marker,
                 number=number,
                 reverse=reverse,
             )
+            return self.__stub.ListJob(message)
         else:
-            return self._req(
-                Service.PPS,
-                "ListJobSet",
+            message = pps_pb2.ListJobSetRequest(
                 details=details,
                 projects=projects_filter,
                 paginationMarker=pagination_marker,
                 number=number,
                 reverse=reverse,
             )
+            return self.__stub.ListJobSet(message)
 
     def delete_job(
         self, job_id: str, pipeline_name: str, project_name: str = None
     ) -> None:
         """Deletes a subjob (job at the pipeline-level).
 
         Parameters
@@ -202,24 +197,23 @@
         job_id : str
             The ID of the job.
         pipeline_name : str
             The name of the pipeline.
         project_name : str
             The name of the project.
         """
-        self._req(
-            Service.PPS,
-            "DeleteJob",
-            job=pps_proto.Job(
-                pipeline=pps_proto.Pipeline(
-                    name=pipeline_name, project=pfs_proto.Project(name=project_name)
-                ),
+        message = pps_pb2.DeleteJobRequest(
+            job=pps_pb2.Job(
                 id=job_id,
-            ),
+                pipeline=pps_pb2.Pipeline(
+                    name=pipeline_name, project=pfs_pb2.Project(name=project_name)
+                ),
+            )
         )
+        self.__stub.DeleteJob(message)
 
     def stop_job(
         self,
         job_id: str,
         pipeline_name: str,
         reason: str = None,
         project_name: str = None,
@@ -228,34 +222,34 @@
 
         Parameters
         ----------
         job_id : str
             The ID of the job.
         pipeline_name : str
             The name of the pipeline.
-        project_name : str
-            The name of the project.
         reason : str, optional
             A reason for stopping the job.
+        project_name : str
+            The name of the project.
         """
-        self._req(
-            Service.PPS,
-            "StopJob",
-            job=pps_proto.Job(
-                pipeline=pps_proto.Pipeline(
-                    name=pipeline_name, project=pfs_proto.Project(name=project_name)
-                ),
+        message = pps_pb2.StopJobRequest(
+            job=pps_pb2.Job(
                 id=job_id,
+                pipeline=pps_pb2.Pipeline(
+                    name=pipeline_name,
+                    project=pfs_pb2.Project(name=project_name),
+                ),
             ),
             reason=reason,
         )
+        self.__stub.StopJob(message)
 
     def inspect_datum(
         self, pipeline_name: str, job_id: str, datum_id: str, project_name: str = None
-    ) -> pps_proto.DatumInfo:
+    ) -> pps_pb2.DatumInfo:
         """Inspects a datum.
 
         Parameters
         ----------
         pipeline_name : str
             The name of the pipeline.
         job_id : str
@@ -263,113 +257,105 @@
         datum_id : str
             The ID of the datum.
         project_name : str
             The name of the project.
 
         Returns
         -------
-        pps_proto.DatumInfo
+        pps_pb2.DatumInfo
             A protobuf object with info on the datum.
         """
-        return self._req(
-            Service.PPS,
-            "InspectDatum",
-            datum=pps_proto.Datum(
+        message = pps_pb2.InspectDatumRequest(
+            datum=pps_pb2.Datum(
                 id=datum_id,
-                job=pps_proto.Job(
-                    pipeline=pps_proto.Pipeline(
-                        name=pipeline_name, project=pfs_proto.Project(name=project_name)
-                    ),
+                job=pps_pb2.Job(
                     id=job_id,
+                    pipeline=pps_pb2.Pipeline(
+                        name=pipeline_name, project=pfs_pb2.Project(name=project_name)
+                    ),
                 ),
             ),
         )
+        return self.__stub.InspectDatum(message)
 
     def list_datum(
         self,
         pipeline_name: str = None,
         job_id: str = None,
-        input: pps_proto.Input = None,
+        input: pps_pb2.Input = None,
         project_name: str = None,
-        datum_filter: pps_proto.ListDatumRequestFilter = None,
-        pagination_marker: pfs_proto.File = None,
+        datum_filter: pps_pb2.ListDatumRequest.Filter = None,
+        pagination_marker: pfs_pb2.File = None,
         number: int = None,
         reverse: bool = False,
-    ) -> Iterator[pps_proto.DatumInfo]:
+    ) -> Iterator[pps_pb2.DatumInfo]:
         """Lists datums. Exactly one of (`pipeline_name`, `job_id`) (real) or
         `input` (hypothetical) must be set.
 
         Parameters
         ----------
         pipeline_name : str, optional
             The name of the pipeline.
         job_id : str, optional
             The ID of a job.
-        input : pps_proto.Input, optional
+        input : pps_pb2.Input, optional
             A protobuf object that filters the datums returned. The datums
             listed are ones that would be run if a pipeline was created with
             the provided input.
         project_name : str
             The name of the project.
-        datum_filter: pps_proto.ListDatumRequestFilter
+        datum_filter: pps_proto.ListDatumRequest.adFilter
             Filter restricts returned DatumInfo messages to those which match
             all the filtered attributes.
         pagination_marker:
             Marker for pagination. If set, the files that come after the marker
             in lexicographical order will be returned. If reverse is also set,
             the files that come before the marker in lexicographical order will
             be returned.
         number : int, optional
             Number of files to return
         reverse : bool, optional
             If true, return files in reverse order
 
         Returns
         -------
-        Iterator[pps_proto.DatumInfo]
+        Iterator[pps_pb2.DatumInfo]
             An iterator of protobuf objects that contain info on a datum.
 
         Examples
         --------
         >>> # See hypothetical datums with specified input cross
-        >>> datums = list(client.list_datum(input=pps_proto.Input(
-        ...     pfs=pps_proto.PFSInput(repo="foo", branch="master", glob="/*"),
+        >>> datums = list(client.list_datum(input=pps_pb2.Input(
+        ...     pfs=pps_pb2.PFSInput(repo="foo", branch="master", glob="/*"),
         ...     cross=[
-        ...         pps_proto.Input(pfs=pps_proto.PFSInput(repo="bar", branch="master", glob="/")),
-        ...         pps_proto.Input(pfs=pps_proto.PFSInput(repo="baz", branch="master", glob="/*/*")),
+        ...         pps_pb2.Input(pfs=pps_pb2.PFSInput(repo="bar", branch="master", glob="/")),
+        ...         pps_pb2.Input(pfs=pps_pb2.PFSInput(repo="baz", branch="master", glob="/*/*")),
         ...     ]
         ... )))
 
         .. # noqa: W505
         """
-        kwargs = dict(
+        message = pps_pb2.ListDatumRequest(
             filter=datum_filter,
             paginationMarker=pagination_marker,
             number=number,
             reverse=reverse,
         )
         if pipeline_name is not None and job_id is not None:
-            return self._req(
-                Service.PPS,
-                "ListDatum",
-                job=pps_proto.Job(
-                    pipeline=pps_proto.Pipeline(
-                        name=pipeline_name, project=pfs_proto.Project(name=project_name)
+            message.job.CopyFrom(
+                pps_pb2.Job(
+                    pipeline=pps_pb2.Pipeline(
+                        name=pipeline_name, project=pfs_pb2.Project(name=project_name)
                     ),
                     id=job_id,
-                ),
-                **kwargs,
+                )
             )
         else:
-            return self._req(
-                Service.PPS,
-                "ListDatum",
-                input=input,
-                **kwargs,
-            )
+            message.input.CopyFrom(input)
+        return self.__stub.ListDatum(message)
 
     def restart_datum(
         self,
         pipeline_name: str,
         job_id: str,
         data_filters: List[str] = None,
         project_name: str = None,
@@ -384,129 +370,131 @@
             The ID of the job.
         data_filters : List[str], optional
             A list of paths or hashes of datums that filter which datums are
             restarted.
         project_name : str
             The name of the project.
         """
-        self._req(
-            Service.PPS,
-            "RestartDatum",
-            job=pps_proto.Job(
-                pipeline=pps_proto.Pipeline(
-                    name=pipeline_name, project=pfs_proto.Project(name=project_name)
+        message = pps_pb2.RestartDatumRequest(
+            data_filters=data_filters,
+            job=pps_pb2.Job(
+                pipeline=pps_pb2.Pipeline(
+                    name=pipeline_name, project=pfs_pb2.Project(name=project_name)
                 ),
                 id=job_id,
             ),
-            data_filters=data_filters,
         )
+        self.__stub.RestartDatum(message)
 
     def create_pipeline(
         self,
         pipeline_name: str,
-        transform: pps_proto.Transform,
+        transform: pps_pb2.Transform,
         project_name: str = None,
-        parallelism_spec: pps_proto.ParallelismSpec = None,
-        egress: pps_proto.Egress = None,
+        parallelism_spec: pps_pb2.ParallelismSpec = None,
+        egress: pps_pb2.Egress = None,
         reprocess_spec: str = None,
         update: bool = False,
         output_branch_name: str = None,
         s3_out: bool = False,
-        resource_requests: pps_proto.ResourceSpec = None,
-        resource_limits: pps_proto.ResourceSpec = None,
-        sidecar_resource_limits: pps_proto.ResourceSpec = None,
-        input: pps_proto.Input = None,
+        resource_requests: pps_pb2.ResourceSpec = None,
+        resource_limits: pps_pb2.ResourceSpec = None,
+        sidecar_resource_limits: pps_pb2.ResourceSpec = None,
+        input: pps_pb2.Input = None,
         description: str = None,
         reprocess: bool = False,
-        service: pps_proto.Service = None,
-        datum_set_spec: pps_proto.DatumSetSpec = None,
-        datum_timeout: datetime.timedelta = None,
-        job_timeout: datetime.timedelta = None,
+        service: pps_pb2.Service = None,
+        datum_set_spec: pps_pb2.DatumSetSpec = None,
+        datum_timeout: duration_pb2.Duration = None,
+        job_timeout: duration_pb2.Duration = None,
         salt: str = None,
         datum_tries: int = 3,
-        scheduling_spec: pps_proto.SchedulingSpec = None,
+        scheduling_spec: pps_pb2.SchedulingSpec = None,
         pod_patch: str = None,
-        spout: pps_proto.Spout = None,
-        spec_commit: pfs_proto.Commit = None,
-        metadata: pps_proto.Metadata = None,
+        spout: pps_pb2.Spout = None,
+        spec_commit: pfs_pb2.Commit = None,
+        metadata: pps_pb2.Metadata = None,
         autoscaling: bool = False,
-        tolerations: List[pps_proto.Toleration] = None,
+        tolerations: List[pps_pb2.Toleration] = None,
+        sidecar_resource_requests: pps_pb2.ResourceSpec = None,
     ) -> None:
         """Creates a pipeline.
 
         For info on the params, please refer to the pipeline spec document:
         http://docs.pachyderm.io/en/latest/reference/pipeline_spec.html
 
         Parameters
         ----------
         pipeline_name : str
             The pipeline name.
-        transform : pps_proto.Transform
+        transform : pps_pb2.Transform
             The image and commands run during pipeline execution.
         project_name : str
             The name of the project.
-        parallelism_spec : pps_proto.ParallelismSpec, optional
+        parallelism_spec : pps_pb2.ParallelismSpec, optional
             Specifies how the pipeline is parallelized.
-        egress : pps_proto.Egress, optional
+        egress : pps_pb2.Egress, optional
             An external data store to publish the results of the pipeline to.
         reprocess_spec : str, optional
             Specifies how to handle already-processed datums.
         update : bool, optional
             If true, updates the existing pipeline with new args.
         output_branch_name : str, optional
             The branch name to output results on.
         s3_out : bool, optional
             If true, the output repo is exposed as an S3 gateway bucket.
-        resource_requests : pps_proto.ResourceSpec, optional
+        resource_requests : pps_pb2.ResourceSpec, optional
             The amount of resources that the pipeline workers will consume.
-        resource_limits: pps_proto.ResourceSpec, optional
+        resource_limits: pps_pb2.ResourceSpec, optional
             The upper threshold of allowed resources a given worker can
             consume. If a worker exceeds this value, it will be evicted.
-        sidecar_resource_limits : pps_proto.ResourceSpec, optional
+        sidecar_resource_limits : pps_pb2.ResourceSpec, optional
             The upper threshold of resources allocated to the sidecar
             containers.
-        input : pps_proto.Input, optional
+        input : pps_pb2.Input, optional
             The input repos to the pipeline. Commits to these repos will
             automatically trigger the pipeline to create new jobs to
             process them.
         description : str, optional
             A description of the pipeline.
         reprocess : bool, optional
             If true, forces the pipeline to reprocess all datums. Only has
             meaning if `update` is ``True``.
-        service : pps_proto.Service, optional
+        service : pps_pb2.Service, optional
             Creates a Service pipeline instead of a normal pipeline.
-        datum_set_spec : pps_proto.DatumSetSpec, optional
+        datum_set_spec : pps_pb2.DatumSetSpec, optional
             Specifies how a pipeline should split its datums into datum sets.
-        datum_timeout : datetime.timedelta, optional
+        datum_timeout : duration_pb2.Duration, optional
             The maximum execution time allowed for each datum.
-        job_timeout : datetime.timedelta, optional
+        job_timeout : duration_pb2.Duration, optional
             The maximum execution time allowed for a job.
         salt : str, optional
             A tag for the pipeline.
         datum_tries : int, optional
             The number of times a job attempts to run on a datum when a failure
             occurs.
-        scheduling_spec : pps_proto.SchedulingSpec, optional
+        scheduling_spec : pps_pb2.SchedulingSpec, optional
             Specifies how the pods for a pipeline should be scheduled.
         pod_patch : str, optional
             Allows one to set fields in the pod spec that haven't been
             explicitly exposed in the rest of the pipeline spec.
-        spout : pps_proto.Spout, optional
+        spout : pps_pb2.Spout, optional
             Creates a Spout pipeline instead of a normal pipeline.
-        spec_commit : pfs_proto.Commit, optional
+        spec_commit : pfs_pb2.Commit, optional
             A spec commit to base the pipeline spec from.
-        metadata : pps_proto.Metadata, optional
+        metadata : pps_pb2.Metadata, optional
             Kubernetes labels and annotations to add as metadata to the
             pipeline pods.
         autoscaling : bool, optional
             If true, automatically scales the worker pool based on the datums
             it has to process.
         tolerations: List[pps_pb2.Toleration]
             A list of Kubernetes tolerations to be applied to the worker pod.
+        sidecar_resource_requests : pps_pb2.ResourceSpec, optional
+            The amount of resources that the sidecar containers will consume.
 
         Notes
         -----
         If creating a Spout pipeline, when committing data to the repo, use
         commit methods (``client.commit()``, ``client.start_commit()``, etc.)
         or :class:`.ModifyFileClient` methods (``mfc.put_file_from_bytes``,
         ``mfc.delete_file()``, etc.)
@@ -514,30 +502,28 @@
         For other pipelines, when committing data to the repo, write out to
         ``/pfs/out/``.
 
         Examples
         --------
         >>> client.create_pipeline(
         ...     "foo",
-        ...     transform=pps_proto.Transform(
+        ...     transform=pps_pb2.Transform(
         ...         cmd=["python3", "main.py"],
         ...         image="example/image",
         ...     ),
-        ...     input=pps_proto.Input(pfs=pps_proto.PfsInput(
+        ...     input=pps_pb2.Input(pfs=pps_pb2.PFSInput(
         ...         repo="foo",
         ...         branch="master",
         ...         glob="/*"
         ...     ))
         ... )
         """
-        self._req(
-            Service.PPS,
-            "CreatePipeline",
-            pipeline=pps_proto.Pipeline(
-                name=pipeline_name, project=pfs_proto.Project(name=project_name)
+        message = pps_pb2.CreatePipelineRequest(
+            pipeline=pps_pb2.Pipeline(
+                name=pipeline_name, project=pfs_pb2.Project(name=project_name)
             ),
             transform=transform,
             parallelism_spec=parallelism_spec,
             egress=egress,
             update=update,
             output_branch=output_branch_name,
             s3_out=s3_out,
@@ -558,36 +544,35 @@
             pod_patch=pod_patch,
             spout=spout,
             spec_commit=spec_commit,
             reprocess_spec=reprocess_spec,
             autoscaling=autoscaling,
             tolerations=tolerations,
         )
+        self.__stub.CreatePipeline(message)
 
-    def create_pipeline_from_request(
-        self, req: pps_proto.CreatePipelineRequest
-    ) -> None:
+    def create_pipeline_from_request(self, req: pps_pb2.CreatePipelineRequest) -> None:
         """Creates a pipeline from a ``CreatePipelineRequest`` object. Usually
         used in conjunction with ``util.parse_json_pipeline_spec()`` or
         ``util.parse_dict_pipeline_spec()``.
 
         Parameters
         ----------
-        req : pps_proto.CreatePipelineRequest
+        req : pps_pb2.CreatePipelineRequest
             The ``CreatePipelineRequest`` object.
         """
-        self._req(Service.PPS, "CreatePipeline", req=req)
+        self.__stub.CreatePipeline(req)
 
     def inspect_pipeline(
         self,
         pipeline_name: str,
         history: int = 0,
         details: bool = False,
         project_name: str = None,
-    ) -> Iterator[pps_proto.PipelineInfo]:
+    ) -> Iterator[pps_pb2.PipelineInfo]:
         """.. # noqa: W505
 
         Inspects a pipeline.
 
         Parameters
         ----------
         pipeline_name : str
@@ -604,59 +589,52 @@
         details : bool, optional
             If true, return pipeline details.
         project_name : str
             The name of the project.
 
         Returns
         -------
-        Iterator[pps_proto.PipelineInfo]
+        Iterator[pps_pb2.PipelineInfo]
             An iterator of protobuf objects that contain info on a pipeline.
 
         Examples
         --------
         >>> pipeline = next(client.inspect_pipeline("foo"))
         ...
         >>> for p in client.inspect_pipeline("foo", 2):
         >>>     print(p)
         """
         if history == 0:
-            return iter(
-                [
-                    self._req(
-                        Service.PPS,
-                        "InspectPipeline",
-                        pipeline=pps_proto.Pipeline(
-                            name=pipeline_name,
-                            project=pfs_proto.Project(name=project_name),
-                        ),
-                        details=details,
-                    )
-                ]
+            message = pps_pb2.InspectPipelineRequest(
+                details=details,
+                pipeline=pps_pb2.Pipeline(
+                    name=pipeline_name, project=pfs_pb2.Project(name=project_name)
+                ),
             )
+            return iter([self.__stub.InspectPipeline(message)])
         else:
             # `InspectPipeline` doesn't support history, but `ListPipeline`
             # with a pipeline filter does, so we use that here
-            return self._req(
-                Service.PPS,
-                "ListPipeline",
-                pipeline=pps_proto.Pipeline(
-                    name=pipeline_name, project=pfs_proto.Project(name=project_name)
-                ),
-                history=history,
+            message = pps_pb2.ListPipelineRequest(
                 details=details,
+                history=history,
+                pipeline=pps_pb2.Pipeline(
+                    name=pipeline_name, project=pfs_pb2.Project(name=project_name)
+                ),
             )
+            return self.__stub.ListPipeline(message)
 
     def list_pipeline(
         self,
         history: int = 0,
         details: bool = False,
         jqFilter: str = None,
-        commit_set: pfs_proto.CommitSet = None,
+        commit_set: pfs_pb2.CommitSet = None,
         projects_filter: List[str] = None,
-    ) -> Iterator[pps_proto.PipelineInfo]:
+    ) -> Iterator[pps_pb2.PipelineInfo]:
         """.. # noqa: W505
 
         Lists pipelines.
 
         Parameters
         ----------
         history : int, optional
@@ -675,32 +653,31 @@
         commit_set : pfs_pb2.CommitSet, optional
             If non-nil, will return all the pipeline infos at this commit set
         projects_filter: List[str], optional
             A list of projects to filter jobs on, None means don't filter.
 
         Returns
         -------
-        Iterator[pps_proto.PipelineInfo]
+        Iterator[pps_pb2.PipelineInfo]
             An iterator of protobuf objects that contain info on a pipeline.
 
         Examples
         --------
         >>> pipelines = list(client.list_pipeline())
         """
         if isinstance(projects_filter, Iterable):
-            projects_filter = [pfs_proto.Project(name=p.name) for p in projects_filter]
-        return self._req(
-            Service.PPS,
-            "ListPipeline",
-            history=history,
+            projects_filter = [pfs_pb2.Project(name=p.name) for p in projects_filter]
+        message = pps_pb2.ListPipelineRequest(
             details=details,
+            history=history,
             jqFilter=jqFilter,
             commit_set=commit_set,
             projects=projects_filter,
         )
+        return self.__stub.ListPipeline(message)
 
     def delete_pipeline(
         self,
         pipeline_name: str,
         force: bool = False,
         keep_repo: bool = False,
         project_name: str = None,
@@ -714,88 +691,81 @@
         force : bool, optional
             If true, forces the pipeline deletion.
         keep_repo : bool, optional
             If true, keeps the output repo.
         project_name : str
             The name of the project.
         """
-        self._req(
-            Service.PPS,
-            "DeletePipeline",
-            pipeline=pps_proto.Pipeline(
-                name=pipeline_name, project=pfs_proto.Project(name=project_name)
-            ),
+        message = pps_pb2.DeletePipelineRequest(
             force=force,
             keep_repo=keep_repo,
+            pipeline=pps_pb2.Pipeline(
+                name=pipeline_name, project=pfs_pb2.Project(name=project_name)
+            ),
         )
+        self.__stub.DeletePipeline(message)
 
     def delete_all_pipelines(self) -> None:
         """Deletes all pipelines."""
-        self._req(
-            Service.PPS,
-            "DeleteAll",
-            req=bp_proto.Empty(),
-        )
+        message = empty_pb2.Empty()
+        self.__stub.DeleteAll(message)
 
     def start_pipeline(self, pipeline_name: str, project_name: str = None) -> None:
         """Starts a pipeline.
 
         Parameters
         ----------
         pipeline_name : str
             The name of the pipeline.
         project_name : str
             The name of the project.
         """
-        self._req(
-            Service.PPS,
-            "StartPipeline",
-            pipeline=pps_proto.Pipeline(
-                name=pipeline_name, project=pfs_proto.Project(name=project_name)
+        message = pps_pb2.StartPipelineRequest(
+            pipeline=pps_pb2.Pipeline(
+                name=pipeline_name, project=pfs_pb2.Project(name=project_name)
             ),
         )
+        self.__stub.StartPipeline(message)
 
     def stop_pipeline(self, pipeline_name: str, project_name: str = None) -> None:
         """Stops a pipeline.
 
         Parameters
         ----------
         pipeline_name : str
             The name of the pipeline.
         project_name : str
             The name of the project.
         """
-        self._req(
-            Service.PPS,
-            "StopPipeline",
-            pipeline=pps_proto.Pipeline(
-                name=pipeline_name, project=pfs_proto.Project(name=project_name)
-            ),
+        message = pps_pb2.StopPipelineRequest(
+            pipeline=pps_pb2.Pipeline(
+                name=pipeline_name, project=pfs_pb2.Project(name=project_name)
+            )
         )
+        self.__stub.StopPipeline(message)
 
     def run_cron(self, pipeline_name: str, project_name: str = None) -> None:
         """Triggers a cron pipeline to run now.
 
         For more info on cron pipelines:
         https://docs.pachyderm.com/latest/concepts/pipeline-concepts/pipeline/cron/
 
         Parameters
         ----------
         pipeline_name : str
             The name of the pipeline.
         project_name : str
             The name of the project.
         """
-        self._req(
-            Service.PPS,
-            "RunCron",
-            pipeline=pps_proto.Pipeline(
-                name=pipeline_name, project=pfs_proto.Project(name=project_name)
+        message = pps_pb2.RunCronRequest(
+            pipeline=pps_pb2.Pipeline(
+                name=pipeline_name, project=pfs_pb2.Project(name=project_name)
             ),
         )
+        self.__stub.RunCron(message)
 
     def create_secret(
         self,
         secret_name: str,
         data: Dict[str, Union[str, bytes]],
         labels: Dict[str, str] = None,
         annotations: Dict[str, str] = None,
@@ -817,83 +787,84 @@
 
         encoded_data = {}
         for k, v in data.items():
             if isinstance(v, str):
                 v = v.encode("utf8")
             encoded_data[k] = base64.b64encode(v).decode("utf8")
 
-        f = json.dumps(
+        file = json.dumps(
             {
                 "kind": "Secret",
                 "apiVersion": "v1",
                 "metadata": {
                     "name": secret_name,
                     "labels": labels,
                     "annotations": annotations,
                 },
                 "data": encoded_data,
             }
         ).encode("utf8")
 
-        self._req(Service.PPS, "CreateSecret", file=f)
+        message = pps_pb2.CreateSecretRequest(file=file)
+        self.__stub.CreateSecret(message)
 
     def delete_secret(self, secret_name: str) -> None:
         """Deletes a secret.
 
         Parameters
         ----------
         secret_name : str
             The name of the secret.
         """
-        secret = pps_proto.Secret(name=secret_name)
-        self._req(Service.PPS, "DeleteSecret", secret=secret)
+        message = pps_pb2.DeleteSecretRequest(
+            secret=pps_pb2.Secret(name=secret_name),
+        )
+        self.__stub.DeleteSecret(message)
 
-    def list_secret(self) -> List[pps_proto.SecretInfo]:
+    def list_secret(self) -> List[pps_pb2.SecretInfo]:
         """Lists secrets.
 
         Returns
         -------
-        List[pps_proto.SecretInfo]
+        List[pps_pb2.SecretInfo]
             A list of protobuf objects that contain info on a secret.
         """
+        message = empty_pb2.Empty()
+        return self.__stub.ListSecret(message).secret_info
 
-        return self._req(
-            Service.PPS,
-            "ListSecret",
-            req=bp_proto.Empty(),
-        ).secret_info
-
-    def inspect_secret(self, secret_name: str) -> pps_proto.SecretInfo:
+    def inspect_secret(self, secret_name: str) -> pps_pb2.SecretInfo:
         """Inspects a secret.
 
         Parameters
         ----------
         secret_name : str
             The name of the secret.
 
         Returns
         -------
-        pps_proto.SecretInfo
+        pps_pb2.SecretInfo
             A protobuf object with info on the secret.
         """
-        secret = pps_proto.Secret(name=secret_name)
-        return self._req(Service.PPS, "InspectSecret", secret=secret)
+        message = pps_pb2.InspectSecretRequest(
+            secret=pps_pb2.Secret(name=secret_name),
+        )
+        return self.__stub.InspectSecret(message)
 
     def get_pipeline_logs(
         self,
         pipeline_name: str,
         project_name: str = None,
         data_filters: List[str] = None,
         master: bool = False,
-        datum: pps_proto.Datum = None,
+        datum: pps_pb2.Datum = None,
         follow: bool = False,
         tail: int = 0,
         use_loki_backend: bool = False,
-        since: datetime.timedelta = None,
-    ) -> Iterator[pps_proto.LogMessage]:
+        since: duration_pb2.Duration = None,
+    ) -> Iterator[pps_pb2.LogMessage]:
         """Gets logs for a pipeline.
 
         Parameters
         ----------
         pipeline_name : str
             The name of the pipeline.
         project_name : str
@@ -902,63 +873,62 @@
             A list of the names of input files from which we want processing
             logs. This may contain multiple files, in case `pipeline_name`
             contains multiple inputs. Each filter may be an absolute path of a
             file within a repo, or it may be a hash for that file (to search
             for files at specific versions).
         master : bool, optional
             If true, includes logs from the master
-        datum : pps_proto.Datum, optional
+        datum : pps_pb2.Datum, optional
             Filters log lines for the specified datum.
         follow : bool, optional
             If true, continue to follow new logs as they appear.
         tail : int, optional
             If nonzero, the number of lines from the end of the logs to return.
             Note: tail applies per container, so you will get
             `tail` * <number of pods> total lines back.
         use_loki_backend : bool, optional
             If true, use loki as a backend, rather than Kubernetes, for
             fetching logs. Requires a loki-enabled cluster.
-        since : datetime.timedelta, optional
+        since : duration_pb2.Duration, optional
             Specifies how far in the past to return logs from.
 
         Returns
         -------
-        Iterator[pps_proto.LogMessage]
+        Iterator[pps_pb2.LogMessage]
             An iterator of protobuf objects that contain info on a log from a
             PPS worker. If `follow` is set to ``True``, use ``next()`` to
             iterate through as the returned stream is potentially endless.
             Might block your code otherwise.
         """
-        return self._req(
-            Service.PPS,
-            "GetLogs",
-            pipeline=pps_proto.Pipeline(
-                name=pipeline_name, project=pfs_proto.Project(name=project_name)
+        message = pps_pb2.GetLogsRequest(
+            pipeline=pps_pb2.Pipeline(
+                name=pipeline_name, project=pfs_pb2.Project(name=project_name)
             ),
             data_filters=data_filters,
             master=master,
             datum=datum,
             follow=follow,
             tail=tail,
             use_loki_backend=use_loki_backend,
             since=since,
         )
+        return self.__stub.GetLogs(message)
 
     def get_job_logs(
         self,
         pipeline_name: str,
         job_id: str,
         project_name: str = None,
         data_filters: List[str] = None,
-        datum: pps_proto.Datum = None,
+        datum: pps_pb2.Datum = None,
         follow: bool = False,
         tail: int = 0,
         use_loki_backend: bool = False,
-        since: datetime.timedelta = None,
-    ) -> Iterator[pps_proto.LogMessage]:
+        since: duration_pb2.Duration = None,
+    ) -> Iterator[pps_pb2.LogMessage]:
         """Gets logs for a job.
 
         Parameters
         ----------
         pipeline_name : str
             The name of the pipeline.
         job_id : str
@@ -967,45 +937,65 @@
             The name of the project.
         data_filters : List[str], optional
             A list of the names of input files from which we want processing
             logs. This may contain multiple files, in case `pipeline_name`
             contains multiple inputs. Each filter may be an absolute path of a
             file within a repo, or it may be a hash for that file (to search
             for files at specific versions).
-        datum : pps_proto.Datum, optional
+        datum : pps_pb2.Datum, optional
             Filters log lines for the specified datum.
         follow : bool, optional
             If true, continue to follow new logs as they appear.
         tail : int, optional
             If nonzero, the number of lines from the end of the logs to return.
             Note: tail applies per container, so you will get
             `tail` * <number of pods> total lines back.
         use_loki_backend : bool, optional
             If true, use loki as a backend, rather than Kubernetes, for
             fetching logs. Requires a loki-enabled cluster.
-        since : datetime.timedelta, optional
+        since : duration_pb2.Duration, optional
             Specifies how far in the past to return logs from.
 
         Returns
         -------
-        Iterator[pps_proto.LogMessage]
+        Iterator[pps_pb2.LogMessage]
             An iterator of protobuf objects that contain info on a log from a
             PPS worker. If `follow` is set to ``True``, use ``next()`` to
             iterate through as the returned stream is potentially endless.
             Might block your code otherwise.
         """
-        return self._req(
-            Service.PPS,
-            "GetLogs",
-            job=pps_proto.Job(
-                pipeline=pps_proto.Pipeline(
-                    name=pipeline_name, project=pfs_proto.Project(name=project_name)
+        message = pps_pb2.GetLogsRequest(
+            job=pps_pb2.Job(
+                pipeline=pps_pb2.Pipeline(
+                    name=pipeline_name, project=pfs_pb2.Project(name=project_name)
                 ),
                 id=job_id,
             ),
             data_filters=data_filters,
             datum=datum,
             follow=follow,
             tail=tail,
             use_loki_backend=use_loki_backend,
             since=since,
         )
+        return self.__stub.GetLogs(message)
+
+    def get_kube_events(self, since: duration_pb2.Duration) -> pps_pb2.LokiLogMessage:
+        """Return a stream of Kubernetes events."""
+        message = pps_pb2.LokiRequest(since=since)
+        return self.__stub.GetKubeEvents(message)
+
+    def query_loki(
+        self, query: str, since: duration_pb2.Duration = None
+    ) -> Iterator[pps_pb2.LokiLogMessage]:
+        """Returns a stream of loki log messages given a query string.
+
+        Parameters
+        ----------
+        query : str
+            The Loki query.
+        since : duration_pb2.Duration, optional
+            Return log messages more recent than "since". (default now)
+        """
+        message = pps_pb2.LokiRequest(query=query, since=since)
+        for item in self.__stub.QueryLoki(message):
+            yield item
```

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/mixin/transaction.py` & `python_pachyderm-7.5.0/src/python_pachyderm/mixin/transaction.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,172 +1,180 @@
 from contextlib import contextmanager
 from typing import Iterator, List, Union
 
-from python_pachyderm.service import Service
-from python_pachyderm.experimental.service import transaction_proto
+import grpc
+
+from python_pachyderm.proto.v2.transaction import transaction_pb2, transaction_pb2_grpc
 
 
 def _transaction_from(transaction):
-    if isinstance(transaction, transaction_proto.Transaction):
+    if isinstance(transaction, transaction_pb2.Transaction):
         return transaction
     else:
-        return transaction_proto.Transaction(id=transaction)
+        return transaction_pb2.Transaction(id=transaction)
 
 
 class TransactionMixin:
     """A mixin for transaction-related functionality."""
 
+    _channel: grpc.Channel
+
+    def __init__(self):
+        self.__stub = transaction_pb2_grpc.APIStub(self._channel)
+        super().__init__()
+
     def batch_transaction(
-        self, requests: List[transaction_proto.TransactionRequest]
-    ) -> transaction_proto.TransactionInfo:
+        self, requests: List[transaction_pb2.TransactionRequest]
+    ) -> transaction_pb2.TransactionInfo:
         """Executes a batch transaction.
 
         Parameters
         ----------
-        requests : List[transaction_proto.TransactionRequest]
+        requests : List[transaction_pb2.TransactionRequest]
             A list of ``TransactionRequest`` protobufs. Each protobuf must
             only have one field set.
 
         Returns
         -------
-        transaction_proto.TransactionInfo
+        transaction_pb2.TransactionInfo
             A protobuf object with info on the transaction.
 
         Examples
         --------
         >>> # Deletes one repo and creates a branch in another repo atomically
         >>> client.batch_transaction([
-            transaction_proto.TransactionRequest(delete_repo=pfs_proto.DeleteRepoRequest(repo=pfs_proto.Repo(name="foo"))),
-            transaction_proto.TransactionRequest(create_branch=pfs_proto.CreateBranchRequest(branch=pfs_proto.Branch(
-                repo=pfs_proto.Repo(name="bar", type="user"), name="staging"
+            transaction_pb2.TransactionRequest(delete_repo=pfs_pb2.DeleteRepoRequest(repo=pfs_pb2.Repo(name="foo"))),
+            transaction_pb2.TransactionRequest(create_branch=pfs_pb2.CreateBranchRequest(branch=pfs_pb2.Branch(
+                repo=pfs_pb2.Repo(name="bar", type="user"), name="staging"
             )))
         ])
         """
-        return self._req(Service.TRANSACTION, "BatchTransaction", requests=requests)
+        message = transaction_pb2.BatchTransactionRequest(requests=requests)
+        return self.__stub.BatchTransaction(message)
 
-    def start_transaction(self) -> transaction_proto.Transaction:
+    def start_transaction(self) -> transaction_pb2.Transaction:
         """Starts a transaction.
 
         Returns
         -------
-        transaction_proto.Transaction
+        transaction_pb2.Transaction
             A protobuf object that represents the transaction.
 
         Examples
         --------
         >>> transaction = client.start_transaction()
         >>> # do stuff
         >>> client.finish_transaction(transaction)
         """
-        return self._req(Service.TRANSACTION, "StartTransaction")
+        message = transaction_pb2.StartTransactionRequest()
+        return self.__stub.StartTransaction(message)
 
     def inspect_transaction(
-        self, transaction: Union[str, transaction_proto.Transaction]
-    ) -> transaction_proto.TransactionInfo:
+        self, transaction: Union[str, transaction_pb2.Transaction]
+    ) -> transaction_pb2.TransactionInfo:
         """Inspects a transaction.
 
         Parameters
         ----------
-        transaction : Union[str, transaction_proto.Transaction]
+        transaction : Union[str, transaction_pb2.Transaction]
             The ID or protobuf object representing the transaction.
 
         Returns
         -------
-        transaction_proto.TransactionInfo
+        transaction_pb2.TransactionInfo
             A protobuf object with info on the transaction.
 
         Examples
         --------
         >>> transaction = client.inspect_transaction("6fe754facd9c41e99d04e1037e3be9ee")
         ...
         >>> transaction = client.inspect_transaction(transaction_protobuf)
 
         .. # noqa: W505
         """
-        return self._req(
-            Service.TRANSACTION,
-            "InspectTransaction",
+        message = transaction_pb2.InspectTransactionRequest(
             transaction=_transaction_from(transaction),
         )
+        return self.__stub.InspectTransaction(message)
 
     def delete_transaction(
-        self, transaction: Union[str, transaction_proto.Transaction]
+        self, transaction: Union[str, transaction_pb2.Transaction]
     ) -> None:
         """Deletes a transaction.
 
         Parameters
         ----------
-        transaction : Union[str, transaction_proto.Transaction]
+        transaction : Union[str, transaction_pb2.Transaction]
             The ID or protobuf object representing the transaction.
 
         Examples
         --------
         >>> client.delete_transaction("6fe754facd9c41e99d04e1037e3be9ee")
         ...
         >>> transaction = client.finish_transaction("a3ak09467c580611234cdb8cc9758c7a")
         >>> client.delete_transaction(transaction)
 
         .. # noqa: W505
         """
-        self._req(
-            Service.TRANSACTION,
-            "DeleteTransaction",
+        message = transaction_pb2.DeleteTransactionRequest(
             transaction=_transaction_from(transaction),
         )
+        self.__stub.DeleteTransaction(message)
 
     def delete_all_transactions(self) -> None:
         """Deletes all transactions."""
-        self._req(Service.TRANSACTION, "DeleteAll")
+        message = transaction_pb2.DeleteAllRequest()
+        self.__stub.DeleteAll(message)
 
-    def list_transaction(self) -> List[transaction_proto.TransactionInfo]:
+    def list_transaction(self) -> List[transaction_pb2.TransactionInfo]:
         """Lists unfinished transactions.
 
         Returns
         -------
-        List[transaction_proto.TransactionInfo]
+        List[transaction_pb2.TransactionInfo]
             A list of protobuf objects that contain info on a transaction.
         """
-        return self._req(Service.TRANSACTION, "ListTransaction").transaction_info
+        message = transaction_pb2.ListTransactionRequest()
+        return self.__stub.ListTransaction(message).transaction_info
 
     def finish_transaction(
-        self, transaction: Union[str, transaction_proto.Transaction]
-    ) -> transaction_proto.TransactionInfo:
+        self, transaction: Union[str, transaction_pb2.Transaction]
+    ) -> transaction_pb2.TransactionInfo:
         """Finishes a transaction.
 
         Parameters
         ----------
-        transaction : Union[str, transaction_proto.Transaction]
+        transaction : Union[str, transaction_pb2.Transaction]
             The ID or protobuf object representing the transaction.
 
         Returns
         -------
-        transaction_proto.TransactionInfo
+        transaction_pb2.TransactionInfo
             A protobuf object with info on the transaction.
 
         Examples
         --------
         >>> transaction = client.start_transaction()
         >>> # do stuff
         >>> client.finish_transaction(transaction)
         """
-        return self._req(
-            Service.TRANSACTION,
-            "FinishTransaction",
-            transaction=_transaction_from(transaction),
+        message = transaction_pb2.FinishTransactionRequest(
+            transaction=_transaction_from(transaction)
         )
+        return self.__stub.FinishTransaction(message)
 
     @contextmanager
-    def transaction(self) -> Iterator[transaction_proto.Transaction]:
+    def transaction(self) -> Iterator[transaction_pb2.Transaction]:
         """A context manager for running operations within a transaction. When
         the context manager completes, the transaction will be deleted if an
         error occurred, or otherwise finished.
 
         Yields
         -------
-        transaction_proto.Transaction
+        transaction_pb2.Transaction
             A protobuf object that represents a transaction.
 
         Examples
         --------
         If a pipeline has two input repos, `foo` and `bar`, a transaction is
         useful for adding data to both atomically before the pipeline runs
         even once.
```

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/mixin/version.py` & `python_pachyderm-7.5.0/src/python_pachyderm/mixin/version.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-from python_pachyderm.service import Service
-from python_pachyderm.experimental.service import version_proto
+import grpc
 from google.protobuf import empty_pb2
-import betterproto.lib.google.protobuf as bp_proto
 
-# bp_to_pb: bp_proto.Empty -> empty_pb2.Empty
+from python_pachyderm.proto.v2.version.versionpb import version_pb2, version_pb2_grpc
 
 
 class VersionMixin:
     """A mixin for version-related functionality."""
 
-    def get_remote_version(self) -> version_proto.Version:
+    _channel: grpc.Channel
+
+    def __init__(self):
+        self.__stub = version_pb2_grpc.APIStub(self._channel)
+        super().__init__()
+
+    def get_remote_version(self) -> version_pb2.Version:
         """Gets version of Pachyderm server.
 
         Returns
         -------
-        version_proto.Version
+        version_pb2.Version
             A protobuf object with info on the pachd version.
         """
-        return self._req(
-            Service.VERSION,
-            "GetVersion",
-            req=bp_proto.Empty(),
-        )
+        message = empty_pb2.Empty()
+        return self.__stub.GetVersion(message)
```

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/experimental/util.py` & `python_pachyderm-7.5.0/src/python_pachyderm/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,28 @@
 import os
-from shutil import which
-from subprocess import run
-from typing import Union, TYPE_CHECKING
-
-from python_pachyderm.experimental.service import pps_proto, pfs_proto
-
-if TYPE_CHECKING:
-    # Avoid circular import
-    from python_pachyderm.experimental import Client
-    from python_pachyderm.experimental.pfs import Commit
+from google.protobuf import json_format
+
+from python_pachyderm import Client
+from python_pachyderm.pfs import SubcommitType
+from python_pachyderm.proto.v2.pps import pps_pb2
 
 
 def put_files(
-    client: "Client",
-    source_path: str,
-    commit: Union[tuple, dict, "Commit", pfs_proto.Commit],
-    dest_path: str,
-    **kwargs
+    client: Client, source_path: str, commit: SubcommitType, dest_path: str, **kwargs
 ) -> None:
     """Utility function for inserting files from the local `source_path`
     into Pachyderm. Roughly equivalent to ``pachctl put file [-r]``.
 
     Parameters
     ----------
     client : Client
         A python_pachyderm client instance.
     source_path : str
         The file/directory to recursively insert content from.
-    commit : Union[tuple, dict, Commit, pfs_proto.Commit]
+    commit : SubcommitType
         The open commit to add files to.
     dest_path : str
         The destination path in PFS.
     **kwargs : dict
         Keyword arguments to forward. See
         ``ModifyFileClient.put_file_from_filepath()`` for more details.
 
@@ -39,15 +30,15 @@
     --------
     >>> source_dir = "data/training/"
     >>> with client.commit("repo_name", "master") as commit:
     >>>     python_pachyderm.put_files(client, source_dir, commit, "/training_set/")
     ...
     >>> with client.commit("repo_name", "master") as commit2:
     >>>     python_pachyderm.put_files(client, "metadata/params.csv", commit2, "/hyperparams.csv")
-    >>>     python_pachyderm.put_files(client, "spec.json", commit2, "/")
+    >>>     python_pachyderm.put_files(client, "spec.json", commit2, "/spec.json")
 
     .. # noqa: W505
     """
     with client.modify_file_client(commit) as mfc:
         if os.path.isfile(source_path):
             mfc.put_file_from_filepath(dest_path, source_path, **kwargs)
         elif os.path.isdir(source_path):
@@ -58,26 +49,26 @@
                         dest_path, os.path.relpath(source_filepath, start=source_path)
                     )
                     mfc.put_file_from_filepath(dest_filepath, source_filepath, **kwargs)
         else:
             raise Exception("Please provide an existing directory or file")
 
 
-def parse_json_pipeline_spec(j: str) -> pps_proto.CreatePipelineRequest:
+def parse_json_pipeline_spec(j: str) -> pps_pb2.CreatePipelineRequest:
     """Parses a string of JSON into a `CreatePipelineRequest` protobuf.
 
     Parameters
     ----------
     j : str
         Pipeline spec as a JSON-like string.
 
 
     Returns
     -------
-    pps_proto.CreatePipelineRequest
+    pps_pb2.CreatePipelineRequest
         A protobuf object that contains the spec info necessary to create a
         pipeline.
 
     Examples
     --------
     Useful for going from Pachyderm spec to creating a pipeline. Pachyderm
     spec: https://docs.pachyderm.com/latest/reference/pipeline_spec/
@@ -99,28 +90,28 @@
     ...     }
     ... }'''
     >>> req = python_pachyderm.parse_json_pipeline_spec(spec)
     >>> client.create_pipeline_from_request(req)
 
     .. # noqa: W505
     """
-    return pps_proto.CreatePipelineRequest().from_json(j)
+    return json_format.Parse(j, pps_pb2.CreatePipelineRequest())
 
 
-def parse_dict_pipeline_spec(d: dict) -> pps_proto.CreatePipelineRequest:
+def parse_dict_pipeline_spec(d: dict) -> pps_pb2.CreatePipelineRequest:
     """Parses a dict of serialized JSON into a `CreatePipelineRequest` protobuf.
 
     Parameters
     ----------
     d : dict
         Pipeline spec as a dictionary.
 
     Returns
     -------
-    pps_proto.CreatePipelineRequest
+    pps_pb2.CreatePipelineRequest
         A protobuf object that contains the spec info necessary to create a
         pipeline.
 
     Examples
     --------
     Useful for going from Pachyderm spec to creating a pipeline. Pachyderm
     spec: https://docs.pachyderm.com/latest/reference/pipeline_spec/
@@ -143,25 +134,8 @@
     ... }'''
     >>> req = python_pachyderm.parse_dict_pipeline_spec(json.loads(spec))
     >>> client.create_pipeline_from_request(req)
 
     .. # noqa: W505
     """
 
-    return pps_proto.CreatePipelineRequest().from_dict(d)
-
-
-def check_pachctl() -> None:
-    """Ensures that pachctl is installed and is capable of running
-    mount operations.
-
-    Errors
-    ------
-    FileNotFoundError
-        No pachctl binary present
-    RuntimeError
-        pachctl binary present but cannot run mount operations
-    """
-    if which("pachctl") is None:
-        raise FileNotFoundError("pachctl")
-    if run(["pachctl", "mount", "-h"], capture_output=True).returncode != 0:
-        raise RuntimeError("incompatible pachctl detected")
+    return json_format.ParseDict(d, pps_pb2.CreatePipelineRequest())
```

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/interceptor.py` & `python_pachyderm-7.5.0/src/python_pachyderm/interceptor.py`

 * *Files identical despite different names*

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/mixin/enterprise.py` & `python_pachyderm-7.5.0/src/python_pachyderm/mixin/enterprise.py`

 * *Files identical despite different names*

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/pfs.py` & `python_pachyderm-7.5.0/src/python_pachyderm/pfs.py`

 * *Files identical despite different names*

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/admin/admin_pb2.py` & `python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/admin/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/admin/admin_pb2_grpc.py` & `python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/admin/admin_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/auth/auth_pb2.py` & `python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/auth/auth_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='python_pachyderm/proto/v2/auth/auth.proto',
   package='auth_v2',
   syntax='proto3',
   serialized_options=b'Z*github.com/pachyderm/pachyderm/v2/src/auth',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n)python_pachyderm/proto/v2/auth/auth.proto\x12\x07\x61uth_v2\x1a\x1fgoogle/protobuf/timestamp.proto\"%\n\x0f\x41\x63tivateRequest\x12\x12\n\nroot_token\x18\x01 \x01(\t\"&\n\x10\x41\x63tivateResponse\x12\x12\n\npach_token\x18\x01 \x01(\t\"\x13\n\x11\x44\x65\x61\x63tivateRequest\"\x14\n\x12\x44\x65\x61\x63tivateResponse\",\n\x16RotateRootTokenRequest\x12\x12\n\nroot_token\x18\x01 \x01(\t\"-\n\x17RotateRootTokenResponse\x12\x12\n\nroot_token\x18\x01 \x01(\t\"\xcb\x01\n\nOIDCConfig\x12\x0e\n\x06issuer\x18\x01 \x01(\t\x12\x11\n\tclient_id\x18\x02 \x01(\t\x12\x15\n\rclient_secret\x18\x03 \x01(\t\x12\x14\n\x0credirect_uri\x18\x04 \x01(\t\x12\x0e\n\x06scopes\x18\x05 \x03(\t\x12\x1e\n\x16require_email_verified\x18\x06 \x01(\x08\x12\x18\n\x10localhost_issuer\x18\x07 \x01(\x08\x12#\n\x1buser_accessible_issuer_host\x18\x08 \x01(\t\"\x19\n\x17GetConfigurationRequest\"F\n\x18GetConfigurationResponse\x12*\n\rconfiguration\x18\x01 \x01(\x0b\x32\x13.auth_v2.OIDCConfig\"E\n\x17SetConfigurationRequest\x12*\n\rconfiguration\x18\x01 \x01(\x0b\x32\x13.auth_v2.OIDCConfig\"\x1a\n\x18SetConfigurationResponse\"b\n\tTokenInfo\x12\x0f\n\x07subject\x18\x01 \x01(\t\x12.\n\nexpiration\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0chashed_token\x18\x03 \x01(\t\";\n\x13\x41uthenticateRequest\x12\x12\n\noidc_state\x18\x01 \x01(\t\x12\x10\n\x08id_token\x18\x02 \x01(\t\"*\n\x14\x41uthenticateResponse\x12\x12\n\npach_token\x18\x01 \x01(\t\"\x0f\n\rWhoAmIRequest\"R\n\x0eWhoAmIResponse\x12\x10\n\x08username\x18\x01 \x01(\t\x12.\n\nexpiration\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"G\n\x1cGetRolesForPermissionRequest\x12\'\n\npermission\x18\x01 \x01(\x0e\x32\x13.auth_v2.Permission\"=\n\x1dGetRolesForPermissionResponse\x12\x1c\n\x05roles\x18\x01 \x03(\x0b\x32\r.auth_v2.Role\"_\n\x05Roles\x12(\n\x05roles\x18\x01 \x03(\x0b\x32\x19.auth_v2.Roles.RolesEntry\x1a,\n\nRolesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01\"\x81\x01\n\x0bRoleBinding\x12\x32\n\x07\x65ntries\x18\x01 \x03(\x0b\x32!.auth_v2.RoleBinding.EntriesEntry\x1a>\n\x0c\x45ntriesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.auth_v2.Roles:\x02\x38\x01\"=\n\x08Resource\x12#\n\x04type\x18\x01 \x01(\x0e\x32\x15.auth_v2.ResourceType\x12\x0c\n\x04name\x18\x02 \x01(\t\"k\n\x05Users\x12\x30\n\tusernames\x18\x01 \x03(\x0b\x32\x1d.auth_v2.Users.UsernamesEntry\x1a\x30\n\x0eUsernamesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01\"d\n\x06Groups\x12+\n\x06groups\x18\x01 \x03(\x0b\x32\x1b.auth_v2.Groups.GroupsEntry\x1a-\n\x0bGroupsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01\"m\n\x04Role\x12\x0c\n\x04name\x18\x01 \x01(\t\x12(\n\x0bpermissions\x18\x02 \x03(\x0e\x32\x13.auth_v2.Permission\x12-\n\x0eresource_types\x18\x03 \x03(\x0e\x32\x15.auth_v2.ResourceType\"a\n\x10\x41uthorizeRequest\x12#\n\x08resource\x18\x01 \x01(\x0b\x32\x11.auth_v2.Resource\x12(\n\x0bpermissions\x18\x02 \x03(\x0e\x32\x13.auth_v2.Permission\"\x88\x01\n\x11\x41uthorizeResponse\x12\x12\n\nauthorized\x18\x01 \x01(\x08\x12&\n\tsatisfied\x18\x02 \x03(\x0e\x32\x13.auth_v2.Permission\x12$\n\x07missing\x18\x03 \x03(\x0e\x32\x13.auth_v2.Permission\x12\x11\n\tprincipal\x18\x04 \x01(\t\"<\n\x15GetPermissionsRequest\x12#\n\x08resource\x18\x01 \x01(\x0b\x32\x11.auth_v2.Resource\"[\n!GetPermissionsForPrincipalRequest\x12#\n\x08resource\x18\x01 \x01(\x0b\x32\x11.auth_v2.Resource\x12\x11\n\tprincipal\x18\x02 \x01(\t\"Q\n\x16GetPermissionsResponse\x12(\n\x0bpermissions\x18\x01 \x03(\x0e\x32\x13.auth_v2.Permission\x12\r\n\x05roles\x18\x02 \x03(\t\"a\n\x18ModifyRoleBindingRequest\x12#\n\x08resource\x18\x01 \x01(\x0b\x32\x11.auth_v2.Resource\x12\x11\n\tprincipal\x18\x02 \x01(\t\x12\r\n\x05roles\x18\x03 \x03(\t\"\x1b\n\x19ModifyRoleBindingResponse\"<\n\x15GetRoleBindingRequest\x12#\n\x08resource\x18\x01 \x01(\x0b\x32\x11.auth_v2.Resource\"?\n\x16GetRoleBindingResponse\x12%\n\x07\x62inding\x18\x01 \x01(\x0b\x32\x14.auth_v2.RoleBinding\"C\n\x0bSessionInfo\x12\r\n\x05nonce\x18\x01 \x01(\t\x12\r\n\x05\x65mail\x18\x02 \x01(\t\x12\x16\n\x0e\x63onversion_err\x18\x03 \x01(\x08\"\x15\n\x13GetOIDCLoginRequest\"8\n\x14GetOIDCLoginResponse\x12\x11\n\tlogin_url\x18\x01 \x01(\t\x12\r\n\x05state\x18\x02 \x01(\t\"2\n\x14GetRobotTokenRequest\x12\r\n\x05robot\x18\x01 \x01(\t\x12\x0b\n\x03ttl\x18\x02 \x01(\x03\"&\n\x15GetRobotTokenResponse\x12\r\n\x05token\x18\x01 \x01(\t\"\'\n\x16RevokeAuthTokenRequest\x12\r\n\x05token\x18\x01 \x01(\t\")\n\x17RevokeAuthTokenResponse\x12\x0e\n\x06number\x18\x01 \x01(\x03\";\n\x17SetGroupsForUserRequest\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x0e\n\x06groups\x18\x02 \x03(\t\"\x1a\n\x18SetGroupsForUserResponse\"B\n\x14ModifyMembersRequest\x12\r\n\x05group\x18\x01 \x01(\t\x12\x0b\n\x03\x61\x64\x64\x18\x02 \x03(\t\x12\x0e\n\x06remove\x18\x03 \x03(\t\"\x17\n\x15ModifyMembersResponse\"\x12\n\x10GetGroupsRequest\"1\n\x1cGetGroupsForPrincipalRequest\x12\x11\n\tprincipal\x18\x01 \x01(\t\"#\n\x11GetGroupsResponse\x12\x0e\n\x06groups\x18\x01 \x03(\t\" \n\x0fGetUsersRequest\x12\r\n\x05group\x18\x01 \x01(\t\"%\n\x10GetUsersResponse\x12\x11\n\tusernames\x18\x01 \x03(\t\"\x1a\n\x18\x45xtractAuthTokensRequest\"?\n\x19\x45xtractAuthTokensResponse\x12\"\n\x06tokens\x18\x01 \x03(\x0b\x32\x12.auth_v2.TokenInfo\"<\n\x17RestoreAuthTokenRequest\x12!\n\x05token\x18\x01 \x01(\x0b\x32\x12.auth_v2.TokenInfo\"\x1a\n\x18RestoreAuthTokenResponse\"2\n\x1eRevokeAuthTokensForUserRequest\x12\x10\n\x08username\x18\x01 \x01(\t\"1\n\x1fRevokeAuthTokensForUserResponse\x12\x0e\n\x06number\x18\x01 \x01(\x03\" \n\x1e\x44\x65leteExpiredAuthTokensRequest\"!\n\x1f\x44\x65leteExpiredAuthTokensResponse*\x8d\x10\n\nPermission\x12\x16\n\x12PERMISSION_UNKNOWN\x10\x00\x12\x1b\n\x17\x43LUSTER_MODIFY_BINDINGS\x10\x64\x12\x18\n\x14\x43LUSTER_GET_BINDINGS\x10\x65\x12\x1b\n\x16\x43LUSTER_GET_PACHD_LOGS\x10\x94\x01\x12\x19\n\x15\x43LUSTER_AUTH_ACTIVATE\x10\x66\x12\x1b\n\x17\x43LUSTER_AUTH_DEACTIVATE\x10g\x12\x1b\n\x17\x43LUSTER_AUTH_GET_CONFIG\x10h\x12\x1b\n\x17\x43LUSTER_AUTH_SET_CONFIG\x10i\x12!\n\x1c\x43LUSTER_AUTH_GET_ROBOT_TOKEN\x10\x8b\x01\x12%\n!CLUSTER_AUTH_MODIFY_GROUP_MEMBERS\x10m\x12\x1b\n\x17\x43LUSTER_AUTH_GET_GROUPS\x10n\x12 \n\x1c\x43LUSTER_AUTH_GET_GROUP_USERS\x10o\x12\x1f\n\x1b\x43LUSTER_AUTH_EXTRACT_TOKENS\x10p\x12\x1e\n\x1a\x43LUSTER_AUTH_RESTORE_TOKEN\x10q\x12/\n*CLUSTER_AUTH_GET_PERMISSIONS_FOR_PRINCIPAL\x10\x8d\x01\x12\'\n\"CLUSTER_AUTH_DELETE_EXPIRED_TOKENS\x10\x8c\x01\x12$\n\x1f\x43LUSTER_AUTH_REVOKE_USER_TOKENS\x10\x8e\x01\x12#\n\x1e\x43LUSTER_AUTH_ROTATE_ROOT_TOKEN\x10\x93\x01\x12\x1f\n\x1b\x43LUSTER_ENTERPRISE_ACTIVATE\x10r\x12 \n\x1c\x43LUSTER_ENTERPRISE_HEARTBEAT\x10s\x12\x1f\n\x1b\x43LUSTER_ENTERPRISE_GET_CODE\x10t\x12!\n\x1d\x43LUSTER_ENTERPRISE_DEACTIVATE\x10u\x12\x1d\n\x18\x43LUSTER_ENTERPRISE_PAUSE\x10\x95\x01\x12\x1f\n\x1b\x43LUSTER_IDENTITY_SET_CONFIG\x10v\x12\x1f\n\x1b\x43LUSTER_IDENTITY_GET_CONFIG\x10w\x12\x1f\n\x1b\x43LUSTER_IDENTITY_CREATE_IDP\x10x\x12\x1f\n\x1b\x43LUSTER_IDENTITY_UPDATE_IDP\x10y\x12\x1e\n\x1a\x43LUSTER_IDENTITY_LIST_IDPS\x10z\x12\x1c\n\x18\x43LUSTER_IDENTITY_GET_IDP\x10{\x12\x1f\n\x1b\x43LUSTER_IDENTITY_DELETE_IDP\x10|\x12\'\n#CLUSTER_IDENTITY_CREATE_OIDC_CLIENT\x10}\x12\'\n#CLUSTER_IDENTITY_UPDATE_OIDC_CLIENT\x10~\x12&\n\"CLUSTER_IDENTITY_LIST_OIDC_CLIENTS\x10\x7f\x12%\n CLUSTER_IDENTITY_GET_OIDC_CLIENT\x10\x80\x01\x12(\n#CLUSTER_IDENTITY_DELETE_OIDC_CLIENT\x10\x81\x01\x12\x17\n\x12\x43LUSTER_DEBUG_DUMP\x10\x83\x01\x12\x1d\n\x18\x43LUSTER_LICENSE_ACTIVATE\x10\x84\x01\x12\x1d\n\x18\x43LUSTER_LICENSE_GET_CODE\x10\x85\x01\x12 \n\x1b\x43LUSTER_LICENSE_ADD_CLUSTER\x10\x86\x01\x12#\n\x1e\x43LUSTER_LICENSE_UPDATE_CLUSTER\x10\x87\x01\x12#\n\x1e\x43LUSTER_LICENSE_DELETE_CLUSTER\x10\x88\x01\x12\"\n\x1d\x43LUSTER_LICENSE_LIST_CLUSTERS\x10\x89\x01\x12\x1a\n\x15\x43LUSTER_CREATE_SECRET\x10\x8f\x01\x12\x19\n\x14\x43LUSTER_LIST_SECRETS\x10\x90\x01\x12\x12\n\rSECRET_DELETE\x10\x91\x01\x12\x13\n\x0eSECRET_INSPECT\x10\x92\x01\x12\x17\n\x12\x43LUSTER_DELETE_ALL\x10\x8a\x01\x12\x0e\n\tREPO_READ\x10\xc8\x01\x12\x0f\n\nREPO_WRITE\x10\xc9\x01\x12\x19\n\x14REPO_MODIFY_BINDINGS\x10\xca\x01\x12\x10\n\x0bREPO_DELETE\x10\xcb\x01\x12\x18\n\x13REPO_INSPECT_COMMIT\x10\xcc\x01\x12\x15\n\x10REPO_LIST_COMMIT\x10\xcd\x01\x12\x17\n\x12REPO_DELETE_COMMIT\x10\xce\x01\x12\x17\n\x12REPO_CREATE_BRANCH\x10\xcf\x01\x12\x15\n\x10REPO_LIST_BRANCH\x10\xd0\x01\x12\x17\n\x12REPO_DELETE_BRANCH\x10\xd1\x01\x12\x16\n\x11REPO_INSPECT_FILE\x10\xd2\x01\x12\x13\n\x0eREPO_LIST_FILE\x10\xd3\x01\x12\x1d\n\x18REPO_ADD_PIPELINE_READER\x10\xd4\x01\x12 \n\x1bREPO_REMOVE_PIPELINE_READER\x10\xd5\x01\x12\x1d\n\x18REPO_ADD_PIPELINE_WRITER\x10\xd6\x01\x12\x16\n\x11PIPELINE_LIST_JOB\x10\xad\x02\x12\x13\n\x0ePROJECT_CREATE\x10\x90\x03\x12\x13\n\x0ePROJECT_DELETE\x10\x91\x03\x12\x16\n\x11PROJECT_LIST_REPO\x10\x92\x03\x12\x18\n\x13PROJECT_CREATE_REPO\x10\x93\x03\x12\x1c\n\x17PROJECT_MODIFY_BINDINGS\x10\x94\x03*\\\n\x0cResourceType\x12\x19\n\x15RESOURCE_TYPE_UNKNOWN\x10\x00\x12\x0b\n\x07\x43LUSTER\x10\x01\x12\x08\n\x04REPO\x10\x02\x12\r\n\tSPEC_REPO\x10\x03\x12\x0b\n\x07PROJECT\x10\x04\x32\xf6\x10\n\x03\x41PI\x12\x41\n\x08\x41\x63tivate\x12\x18.auth_v2.ActivateRequest\x1a\x19.auth_v2.ActivateResponse\"\x00\x12G\n\nDeactivate\x12\x1a.auth_v2.DeactivateRequest\x1a\x1b.auth_v2.DeactivateResponse\"\x00\x12Y\n\x10GetConfiguration\x12 .auth_v2.GetConfigurationRequest\x1a!.auth_v2.GetConfigurationResponse\"\x00\x12Y\n\x10SetConfiguration\x12 .auth_v2.SetConfigurationRequest\x1a!.auth_v2.SetConfigurationResponse\"\x00\x12M\n\x0c\x41uthenticate\x12\x1c.auth_v2.AuthenticateRequest\x1a\x1d.auth_v2.AuthenticateResponse\"\x00\x12\x44\n\tAuthorize\x12\x19.auth_v2.AuthorizeRequest\x1a\x1a.auth_v2.AuthorizeResponse\"\x00\x12S\n\x0eGetPermissions\x12\x1e.auth_v2.GetPermissionsRequest\x1a\x1f.auth_v2.GetPermissionsResponse\"\x00\x12k\n\x1aGetPermissionsForPrincipal\x12*.auth_v2.GetPermissionsForPrincipalRequest\x1a\x1f.auth_v2.GetPermissionsResponse\"\x00\x12;\n\x06WhoAmI\x12\x16.auth_v2.WhoAmIRequest\x1a\x17.auth_v2.WhoAmIResponse\"\x00\x12h\n\x15GetRolesForPermission\x12%.auth_v2.GetRolesForPermissionRequest\x1a&.auth_v2.GetRolesForPermissionResponse\"\x00\x12\\\n\x11ModifyRoleBinding\x12!.auth_v2.ModifyRoleBindingRequest\x1a\".auth_v2.ModifyRoleBindingResponse\"\x00\x12S\n\x0eGetRoleBinding\x12\x1e.auth_v2.GetRoleBindingRequest\x1a\x1f.auth_v2.GetRoleBindingResponse\"\x00\x12M\n\x0cGetOIDCLogin\x12\x1c.auth_v2.GetOIDCLoginRequest\x1a\x1d.auth_v2.GetOIDCLoginResponse\"\x00\x12P\n\rGetRobotToken\x12\x1d.auth_v2.GetRobotTokenRequest\x1a\x1e.auth_v2.GetRobotTokenResponse\"\x00\x12V\n\x0fRevokeAuthToken\x12\x1f.auth_v2.RevokeAuthTokenRequest\x1a .auth_v2.RevokeAuthTokenResponse\"\x00\x12n\n\x17RevokeAuthTokensForUser\x12\'.auth_v2.RevokeAuthTokensForUserRequest\x1a(.auth_v2.RevokeAuthTokensForUserResponse\"\x00\x12Y\n\x10SetGroupsForUser\x12 .auth_v2.SetGroupsForUserRequest\x1a!.auth_v2.SetGroupsForUserResponse\"\x00\x12P\n\rModifyMembers\x12\x1d.auth_v2.ModifyMembersRequest\x1a\x1e.auth_v2.ModifyMembersResponse\"\x00\x12\x44\n\tGetGroups\x12\x19.auth_v2.GetGroupsRequest\x1a\x1a.auth_v2.GetGroupsResponse\"\x00\x12\\\n\x15GetGroupsForPrincipal\x12%.auth_v2.GetGroupsForPrincipalRequest\x1a\x1a.auth_v2.GetGroupsResponse\"\x00\x12\x41\n\x08GetUsers\x12\x18.auth_v2.GetUsersRequest\x1a\x19.auth_v2.GetUsersResponse\"\x00\x12\\\n\x11\x45xtractAuthTokens\x12!.auth_v2.ExtractAuthTokensRequest\x1a\".auth_v2.ExtractAuthTokensResponse\"\x00\x12Y\n\x10RestoreAuthToken\x12 .auth_v2.RestoreAuthTokenRequest\x1a!.auth_v2.RestoreAuthTokenResponse\"\x00\x12n\n\x17\x44\x65leteExpiredAuthTokens\x12\'.auth_v2.DeleteExpiredAuthTokensRequest\x1a(.auth_v2.DeleteExpiredAuthTokensResponse\"\x00\x12V\n\x0fRotateRootToken\x12\x1f.auth_v2.RotateRootTokenRequest\x1a .auth_v2.RotateRootTokenResponse\"\x00\x42,Z*github.com/pachyderm/pachyderm/v2/src/authb\x06proto3'
+  serialized_pb=b'\n)python_pachyderm/proto/v2/auth/auth.proto\x12\x07\x61uth_v2\x1a\x1fgoogle/protobuf/timestamp.proto\"%\n\x0f\x41\x63tivateRequest\x12\x12\n\nroot_token\x18\x01 \x01(\t\"&\n\x10\x41\x63tivateResponse\x12\x12\n\npach_token\x18\x01 \x01(\t\"\x13\n\x11\x44\x65\x61\x63tivateRequest\"\x14\n\x12\x44\x65\x61\x63tivateResponse\",\n\x16RotateRootTokenRequest\x12\x12\n\nroot_token\x18\x01 \x01(\t\"-\n\x17RotateRootTokenResponse\x12\x12\n\nroot_token\x18\x01 \x01(\t\"\xcb\x01\n\nOIDCConfig\x12\x0e\n\x06issuer\x18\x01 \x01(\t\x12\x11\n\tclient_id\x18\x02 \x01(\t\x12\x15\n\rclient_secret\x18\x03 \x01(\t\x12\x14\n\x0credirect_uri\x18\x04 \x01(\t\x12\x0e\n\x06scopes\x18\x05 \x03(\t\x12\x1e\n\x16require_email_verified\x18\x06 \x01(\x08\x12\x18\n\x10localhost_issuer\x18\x07 \x01(\x08\x12#\n\x1buser_accessible_issuer_host\x18\x08 \x01(\t\"\x19\n\x17GetConfigurationRequest\"F\n\x18GetConfigurationResponse\x12*\n\rconfiguration\x18\x01 \x01(\x0b\x32\x13.auth_v2.OIDCConfig\"E\n\x17SetConfigurationRequest\x12*\n\rconfiguration\x18\x01 \x01(\x0b\x32\x13.auth_v2.OIDCConfig\"\x1a\n\x18SetConfigurationResponse\"b\n\tTokenInfo\x12\x0f\n\x07subject\x18\x01 \x01(\t\x12.\n\nexpiration\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0chashed_token\x18\x03 \x01(\t\";\n\x13\x41uthenticateRequest\x12\x12\n\noidc_state\x18\x01 \x01(\t\x12\x10\n\x08id_token\x18\x02 \x01(\t\"*\n\x14\x41uthenticateResponse\x12\x12\n\npach_token\x18\x01 \x01(\t\"\x0f\n\rWhoAmIRequest\"R\n\x0eWhoAmIResponse\x12\x10\n\x08username\x18\x01 \x01(\t\x12.\n\nexpiration\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"G\n\x1cGetRolesForPermissionRequest\x12\'\n\npermission\x18\x01 \x01(\x0e\x32\x13.auth_v2.Permission\"=\n\x1dGetRolesForPermissionResponse\x12\x1c\n\x05roles\x18\x01 \x03(\x0b\x32\r.auth_v2.Role\"_\n\x05Roles\x12(\n\x05roles\x18\x01 \x03(\x0b\x32\x19.auth_v2.Roles.RolesEntry\x1a,\n\nRolesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01\"\x81\x01\n\x0bRoleBinding\x12\x32\n\x07\x65ntries\x18\x01 \x03(\x0b\x32!.auth_v2.RoleBinding.EntriesEntry\x1a>\n\x0c\x45ntriesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.auth_v2.Roles:\x02\x38\x01\"=\n\x08Resource\x12#\n\x04type\x18\x01 \x01(\x0e\x32\x15.auth_v2.ResourceType\x12\x0c\n\x04name\x18\x02 \x01(\t\"k\n\x05Users\x12\x30\n\tusernames\x18\x01 \x03(\x0b\x32\x1d.auth_v2.Users.UsernamesEntry\x1a\x30\n\x0eUsernamesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01\"d\n\x06Groups\x12+\n\x06groups\x18\x01 \x03(\x0b\x32\x1b.auth_v2.Groups.GroupsEntry\x1a-\n\x0bGroupsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01\"m\n\x04Role\x12\x0c\n\x04name\x18\x01 \x01(\t\x12(\n\x0bpermissions\x18\x02 \x03(\x0e\x32\x13.auth_v2.Permission\x12-\n\x0eresource_types\x18\x03 \x03(\x0e\x32\x15.auth_v2.ResourceType\"a\n\x10\x41uthorizeRequest\x12#\n\x08resource\x18\x01 \x01(\x0b\x32\x11.auth_v2.Resource\x12(\n\x0bpermissions\x18\x02 \x03(\x0e\x32\x13.auth_v2.Permission\"\x88\x01\n\x11\x41uthorizeResponse\x12\x12\n\nauthorized\x18\x01 \x01(\x08\x12&\n\tsatisfied\x18\x02 \x03(\x0e\x32\x13.auth_v2.Permission\x12$\n\x07missing\x18\x03 \x03(\x0e\x32\x13.auth_v2.Permission\x12\x11\n\tprincipal\x18\x04 \x01(\t\"<\n\x15GetPermissionsRequest\x12#\n\x08resource\x18\x01 \x01(\x0b\x32\x11.auth_v2.Resource\"[\n!GetPermissionsForPrincipalRequest\x12#\n\x08resource\x18\x01 \x01(\x0b\x32\x11.auth_v2.Resource\x12\x11\n\tprincipal\x18\x02 \x01(\t\"Q\n\x16GetPermissionsResponse\x12(\n\x0bpermissions\x18\x01 \x03(\x0e\x32\x13.auth_v2.Permission\x12\r\n\x05roles\x18\x02 \x03(\t\"a\n\x18ModifyRoleBindingRequest\x12#\n\x08resource\x18\x01 \x01(\x0b\x32\x11.auth_v2.Resource\x12\x11\n\tprincipal\x18\x02 \x01(\t\x12\r\n\x05roles\x18\x03 \x03(\t\"\x1b\n\x19ModifyRoleBindingResponse\"<\n\x15GetRoleBindingRequest\x12#\n\x08resource\x18\x01 \x01(\x0b\x32\x11.auth_v2.Resource\"?\n\x16GetRoleBindingResponse\x12%\n\x07\x62inding\x18\x01 \x01(\x0b\x32\x14.auth_v2.RoleBinding\"C\n\x0bSessionInfo\x12\r\n\x05nonce\x18\x01 \x01(\t\x12\r\n\x05\x65mail\x18\x02 \x01(\t\x12\x16\n\x0e\x63onversion_err\x18\x03 \x01(\x08\"\x15\n\x13GetOIDCLoginRequest\"8\n\x14GetOIDCLoginResponse\x12\x11\n\tlogin_url\x18\x01 \x01(\t\x12\r\n\x05state\x18\x02 \x01(\t\"2\n\x14GetRobotTokenRequest\x12\r\n\x05robot\x18\x01 \x01(\t\x12\x0b\n\x03ttl\x18\x02 \x01(\x03\"&\n\x15GetRobotTokenResponse\x12\r\n\x05token\x18\x01 \x01(\t\"\'\n\x16RevokeAuthTokenRequest\x12\r\n\x05token\x18\x01 \x01(\t\")\n\x17RevokeAuthTokenResponse\x12\x0e\n\x06number\x18\x01 \x01(\x03\";\n\x17SetGroupsForUserRequest\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x0e\n\x06groups\x18\x02 \x03(\t\"\x1a\n\x18SetGroupsForUserResponse\"B\n\x14ModifyMembersRequest\x12\r\n\x05group\x18\x01 \x01(\t\x12\x0b\n\x03\x61\x64\x64\x18\x02 \x03(\t\x12\x0e\n\x06remove\x18\x03 \x03(\t\"\x17\n\x15ModifyMembersResponse\"\x12\n\x10GetGroupsRequest\"1\n\x1cGetGroupsForPrincipalRequest\x12\x11\n\tprincipal\x18\x01 \x01(\t\"#\n\x11GetGroupsResponse\x12\x0e\n\x06groups\x18\x01 \x03(\t\" \n\x0fGetUsersRequest\x12\r\n\x05group\x18\x01 \x01(\t\"%\n\x10GetUsersResponse\x12\x11\n\tusernames\x18\x01 \x03(\t\"\x1a\n\x18\x45xtractAuthTokensRequest\"?\n\x19\x45xtractAuthTokensResponse\x12\"\n\x06tokens\x18\x01 \x03(\x0b\x32\x12.auth_v2.TokenInfo\"<\n\x17RestoreAuthTokenRequest\x12!\n\x05token\x18\x01 \x01(\x0b\x32\x12.auth_v2.TokenInfo\"\x1a\n\x18RestoreAuthTokenResponse\"2\n\x1eRevokeAuthTokensForUserRequest\x12\x10\n\x08username\x18\x01 \x01(\t\"1\n\x1fRevokeAuthTokensForUserResponse\x12\x0e\n\x06number\x18\x01 \x01(\x03\" \n\x1e\x44\x65leteExpiredAuthTokensRequest\"!\n\x1f\x44\x65leteExpiredAuthTokensResponse*\xa9\x10\n\nPermission\x12\x16\n\x12PERMISSION_UNKNOWN\x10\x00\x12\x1b\n\x17\x43LUSTER_MODIFY_BINDINGS\x10\x64\x12\x18\n\x14\x43LUSTER_GET_BINDINGS\x10\x65\x12\x1b\n\x16\x43LUSTER_GET_PACHD_LOGS\x10\x94\x01\x12\x1a\n\x15\x43LUSTER_GET_LOKI_LOGS\x10\x96\x01\x12\x19\n\x15\x43LUSTER_AUTH_ACTIVATE\x10\x66\x12\x1b\n\x17\x43LUSTER_AUTH_DEACTIVATE\x10g\x12\x1b\n\x17\x43LUSTER_AUTH_GET_CONFIG\x10h\x12\x1b\n\x17\x43LUSTER_AUTH_SET_CONFIG\x10i\x12!\n\x1c\x43LUSTER_AUTH_GET_ROBOT_TOKEN\x10\x8b\x01\x12%\n!CLUSTER_AUTH_MODIFY_GROUP_MEMBERS\x10m\x12\x1b\n\x17\x43LUSTER_AUTH_GET_GROUPS\x10n\x12 \n\x1c\x43LUSTER_AUTH_GET_GROUP_USERS\x10o\x12\x1f\n\x1b\x43LUSTER_AUTH_EXTRACT_TOKENS\x10p\x12\x1e\n\x1a\x43LUSTER_AUTH_RESTORE_TOKEN\x10q\x12/\n*CLUSTER_AUTH_GET_PERMISSIONS_FOR_PRINCIPAL\x10\x8d\x01\x12\'\n\"CLUSTER_AUTH_DELETE_EXPIRED_TOKENS\x10\x8c\x01\x12$\n\x1f\x43LUSTER_AUTH_REVOKE_USER_TOKENS\x10\x8e\x01\x12#\n\x1e\x43LUSTER_AUTH_ROTATE_ROOT_TOKEN\x10\x93\x01\x12\x1f\n\x1b\x43LUSTER_ENTERPRISE_ACTIVATE\x10r\x12 \n\x1c\x43LUSTER_ENTERPRISE_HEARTBEAT\x10s\x12\x1f\n\x1b\x43LUSTER_ENTERPRISE_GET_CODE\x10t\x12!\n\x1d\x43LUSTER_ENTERPRISE_DEACTIVATE\x10u\x12\x1d\n\x18\x43LUSTER_ENTERPRISE_PAUSE\x10\x95\x01\x12\x1f\n\x1b\x43LUSTER_IDENTITY_SET_CONFIG\x10v\x12\x1f\n\x1b\x43LUSTER_IDENTITY_GET_CONFIG\x10w\x12\x1f\n\x1b\x43LUSTER_IDENTITY_CREATE_IDP\x10x\x12\x1f\n\x1b\x43LUSTER_IDENTITY_UPDATE_IDP\x10y\x12\x1e\n\x1a\x43LUSTER_IDENTITY_LIST_IDPS\x10z\x12\x1c\n\x18\x43LUSTER_IDENTITY_GET_IDP\x10{\x12\x1f\n\x1b\x43LUSTER_IDENTITY_DELETE_IDP\x10|\x12\'\n#CLUSTER_IDENTITY_CREATE_OIDC_CLIENT\x10}\x12\'\n#CLUSTER_IDENTITY_UPDATE_OIDC_CLIENT\x10~\x12&\n\"CLUSTER_IDENTITY_LIST_OIDC_CLIENTS\x10\x7f\x12%\n CLUSTER_IDENTITY_GET_OIDC_CLIENT\x10\x80\x01\x12(\n#CLUSTER_IDENTITY_DELETE_OIDC_CLIENT\x10\x81\x01\x12\x17\n\x12\x43LUSTER_DEBUG_DUMP\x10\x83\x01\x12\x1d\n\x18\x43LUSTER_LICENSE_ACTIVATE\x10\x84\x01\x12\x1d\n\x18\x43LUSTER_LICENSE_GET_CODE\x10\x85\x01\x12 \n\x1b\x43LUSTER_LICENSE_ADD_CLUSTER\x10\x86\x01\x12#\n\x1e\x43LUSTER_LICENSE_UPDATE_CLUSTER\x10\x87\x01\x12#\n\x1e\x43LUSTER_LICENSE_DELETE_CLUSTER\x10\x88\x01\x12\"\n\x1d\x43LUSTER_LICENSE_LIST_CLUSTERS\x10\x89\x01\x12\x1a\n\x15\x43LUSTER_CREATE_SECRET\x10\x8f\x01\x12\x19\n\x14\x43LUSTER_LIST_SECRETS\x10\x90\x01\x12\x12\n\rSECRET_DELETE\x10\x91\x01\x12\x13\n\x0eSECRET_INSPECT\x10\x92\x01\x12\x17\n\x12\x43LUSTER_DELETE_ALL\x10\x8a\x01\x12\x0e\n\tREPO_READ\x10\xc8\x01\x12\x0f\n\nREPO_WRITE\x10\xc9\x01\x12\x19\n\x14REPO_MODIFY_BINDINGS\x10\xca\x01\x12\x10\n\x0bREPO_DELETE\x10\xcb\x01\x12\x18\n\x13REPO_INSPECT_COMMIT\x10\xcc\x01\x12\x15\n\x10REPO_LIST_COMMIT\x10\xcd\x01\x12\x17\n\x12REPO_DELETE_COMMIT\x10\xce\x01\x12\x17\n\x12REPO_CREATE_BRANCH\x10\xcf\x01\x12\x15\n\x10REPO_LIST_BRANCH\x10\xd0\x01\x12\x17\n\x12REPO_DELETE_BRANCH\x10\xd1\x01\x12\x16\n\x11REPO_INSPECT_FILE\x10\xd2\x01\x12\x13\n\x0eREPO_LIST_FILE\x10\xd3\x01\x12\x1d\n\x18REPO_ADD_PIPELINE_READER\x10\xd4\x01\x12 \n\x1bREPO_REMOVE_PIPELINE_READER\x10\xd5\x01\x12\x1d\n\x18REPO_ADD_PIPELINE_WRITER\x10\xd6\x01\x12\x16\n\x11PIPELINE_LIST_JOB\x10\xad\x02\x12\x13\n\x0ePROJECT_CREATE\x10\x90\x03\x12\x13\n\x0ePROJECT_DELETE\x10\x91\x03\x12\x16\n\x11PROJECT_LIST_REPO\x10\x92\x03\x12\x18\n\x13PROJECT_CREATE_REPO\x10\x93\x03\x12\x1c\n\x17PROJECT_MODIFY_BINDINGS\x10\x94\x03*\\\n\x0cResourceType\x12\x19\n\x15RESOURCE_TYPE_UNKNOWN\x10\x00\x12\x0b\n\x07\x43LUSTER\x10\x01\x12\x08\n\x04REPO\x10\x02\x12\r\n\tSPEC_REPO\x10\x03\x12\x0b\n\x07PROJECT\x10\x04\x32\xf6\x10\n\x03\x41PI\x12\x41\n\x08\x41\x63tivate\x12\x18.auth_v2.ActivateRequest\x1a\x19.auth_v2.ActivateResponse\"\x00\x12G\n\nDeactivate\x12\x1a.auth_v2.DeactivateRequest\x1a\x1b.auth_v2.DeactivateResponse\"\x00\x12Y\n\x10GetConfiguration\x12 .auth_v2.GetConfigurationRequest\x1a!.auth_v2.GetConfigurationResponse\"\x00\x12Y\n\x10SetConfiguration\x12 .auth_v2.SetConfigurationRequest\x1a!.auth_v2.SetConfigurationResponse\"\x00\x12M\n\x0c\x41uthenticate\x12\x1c.auth_v2.AuthenticateRequest\x1a\x1d.auth_v2.AuthenticateResponse\"\x00\x12\x44\n\tAuthorize\x12\x19.auth_v2.AuthorizeRequest\x1a\x1a.auth_v2.AuthorizeResponse\"\x00\x12S\n\x0eGetPermissions\x12\x1e.auth_v2.GetPermissionsRequest\x1a\x1f.auth_v2.GetPermissionsResponse\"\x00\x12k\n\x1aGetPermissionsForPrincipal\x12*.auth_v2.GetPermissionsForPrincipalRequest\x1a\x1f.auth_v2.GetPermissionsResponse\"\x00\x12;\n\x06WhoAmI\x12\x16.auth_v2.WhoAmIRequest\x1a\x17.auth_v2.WhoAmIResponse\"\x00\x12h\n\x15GetRolesForPermission\x12%.auth_v2.GetRolesForPermissionRequest\x1a&.auth_v2.GetRolesForPermissionResponse\"\x00\x12\\\n\x11ModifyRoleBinding\x12!.auth_v2.ModifyRoleBindingRequest\x1a\".auth_v2.ModifyRoleBindingResponse\"\x00\x12S\n\x0eGetRoleBinding\x12\x1e.auth_v2.GetRoleBindingRequest\x1a\x1f.auth_v2.GetRoleBindingResponse\"\x00\x12M\n\x0cGetOIDCLogin\x12\x1c.auth_v2.GetOIDCLoginRequest\x1a\x1d.auth_v2.GetOIDCLoginResponse\"\x00\x12P\n\rGetRobotToken\x12\x1d.auth_v2.GetRobotTokenRequest\x1a\x1e.auth_v2.GetRobotTokenResponse\"\x00\x12V\n\x0fRevokeAuthToken\x12\x1f.auth_v2.RevokeAuthTokenRequest\x1a .auth_v2.RevokeAuthTokenResponse\"\x00\x12n\n\x17RevokeAuthTokensForUser\x12\'.auth_v2.RevokeAuthTokensForUserRequest\x1a(.auth_v2.RevokeAuthTokensForUserResponse\"\x00\x12Y\n\x10SetGroupsForUser\x12 .auth_v2.SetGroupsForUserRequest\x1a!.auth_v2.SetGroupsForUserResponse\"\x00\x12P\n\rModifyMembers\x12\x1d.auth_v2.ModifyMembersRequest\x1a\x1e.auth_v2.ModifyMembersResponse\"\x00\x12\x44\n\tGetGroups\x12\x19.auth_v2.GetGroupsRequest\x1a\x1a.auth_v2.GetGroupsResponse\"\x00\x12\\\n\x15GetGroupsForPrincipal\x12%.auth_v2.GetGroupsForPrincipalRequest\x1a\x1a.auth_v2.GetGroupsResponse\"\x00\x12\x41\n\x08GetUsers\x12\x18.auth_v2.GetUsersRequest\x1a\x19.auth_v2.GetUsersResponse\"\x00\x12\\\n\x11\x45xtractAuthTokens\x12!.auth_v2.ExtractAuthTokensRequest\x1a\".auth_v2.ExtractAuthTokensResponse\"\x00\x12Y\n\x10RestoreAuthToken\x12 .auth_v2.RestoreAuthTokenRequest\x1a!.auth_v2.RestoreAuthTokenResponse\"\x00\x12n\n\x17\x44\x65leteExpiredAuthTokens\x12\'.auth_v2.DeleteExpiredAuthTokensRequest\x1a(.auth_v2.DeleteExpiredAuthTokensResponse\"\x00\x12V\n\x0fRotateRootToken\x12\x1f.auth_v2.RotateRootTokenRequest\x1a .auth_v2.RotateRootTokenResponse\"\x00\x42,Z*github.com/pachyderm/pachyderm/v2/src/authb\x06proto3'
   ,
   dependencies=[google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,])
 
 _PERMISSION = _descriptor.EnumDescriptor(
   name='Permission',
   full_name='auth_v2.Permission',
   filename=None,
@@ -49,338 +49,343 @@
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='CLUSTER_GET_PACHD_LOGS', index=3, number=148,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_AUTH_ACTIVATE', index=4, number=102,
+      name='CLUSTER_GET_LOKI_LOGS', index=4, number=150,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_AUTH_DEACTIVATE', index=5, number=103,
+      name='CLUSTER_AUTH_ACTIVATE', index=5, number=102,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_AUTH_GET_CONFIG', index=6, number=104,
+      name='CLUSTER_AUTH_DEACTIVATE', index=6, number=103,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_AUTH_SET_CONFIG', index=7, number=105,
+      name='CLUSTER_AUTH_GET_CONFIG', index=7, number=104,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_AUTH_GET_ROBOT_TOKEN', index=8, number=139,
+      name='CLUSTER_AUTH_SET_CONFIG', index=8, number=105,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_AUTH_MODIFY_GROUP_MEMBERS', index=9, number=109,
+      name='CLUSTER_AUTH_GET_ROBOT_TOKEN', index=9, number=139,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_AUTH_GET_GROUPS', index=10, number=110,
+      name='CLUSTER_AUTH_MODIFY_GROUP_MEMBERS', index=10, number=109,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_AUTH_GET_GROUP_USERS', index=11, number=111,
+      name='CLUSTER_AUTH_GET_GROUPS', index=11, number=110,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_AUTH_EXTRACT_TOKENS', index=12, number=112,
+      name='CLUSTER_AUTH_GET_GROUP_USERS', index=12, number=111,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_AUTH_RESTORE_TOKEN', index=13, number=113,
+      name='CLUSTER_AUTH_EXTRACT_TOKENS', index=13, number=112,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_AUTH_GET_PERMISSIONS_FOR_PRINCIPAL', index=14, number=141,
+      name='CLUSTER_AUTH_RESTORE_TOKEN', index=14, number=113,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_AUTH_DELETE_EXPIRED_TOKENS', index=15, number=140,
+      name='CLUSTER_AUTH_GET_PERMISSIONS_FOR_PRINCIPAL', index=15, number=141,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_AUTH_REVOKE_USER_TOKENS', index=16, number=142,
+      name='CLUSTER_AUTH_DELETE_EXPIRED_TOKENS', index=16, number=140,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_AUTH_ROTATE_ROOT_TOKEN', index=17, number=147,
+      name='CLUSTER_AUTH_REVOKE_USER_TOKENS', index=17, number=142,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_ENTERPRISE_ACTIVATE', index=18, number=114,
+      name='CLUSTER_AUTH_ROTATE_ROOT_TOKEN', index=18, number=147,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_ENTERPRISE_HEARTBEAT', index=19, number=115,
+      name='CLUSTER_ENTERPRISE_ACTIVATE', index=19, number=114,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_ENTERPRISE_GET_CODE', index=20, number=116,
+      name='CLUSTER_ENTERPRISE_HEARTBEAT', index=20, number=115,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_ENTERPRISE_DEACTIVATE', index=21, number=117,
+      name='CLUSTER_ENTERPRISE_GET_CODE', index=21, number=116,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_ENTERPRISE_PAUSE', index=22, number=149,
+      name='CLUSTER_ENTERPRISE_DEACTIVATE', index=22, number=117,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_IDENTITY_SET_CONFIG', index=23, number=118,
+      name='CLUSTER_ENTERPRISE_PAUSE', index=23, number=149,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_IDENTITY_GET_CONFIG', index=24, number=119,
+      name='CLUSTER_IDENTITY_SET_CONFIG', index=24, number=118,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_IDENTITY_CREATE_IDP', index=25, number=120,
+      name='CLUSTER_IDENTITY_GET_CONFIG', index=25, number=119,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_IDENTITY_UPDATE_IDP', index=26, number=121,
+      name='CLUSTER_IDENTITY_CREATE_IDP', index=26, number=120,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_IDENTITY_LIST_IDPS', index=27, number=122,
+      name='CLUSTER_IDENTITY_UPDATE_IDP', index=27, number=121,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_IDENTITY_GET_IDP', index=28, number=123,
+      name='CLUSTER_IDENTITY_LIST_IDPS', index=28, number=122,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_IDENTITY_DELETE_IDP', index=29, number=124,
+      name='CLUSTER_IDENTITY_GET_IDP', index=29, number=123,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_IDENTITY_CREATE_OIDC_CLIENT', index=30, number=125,
+      name='CLUSTER_IDENTITY_DELETE_IDP', index=30, number=124,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_IDENTITY_UPDATE_OIDC_CLIENT', index=31, number=126,
+      name='CLUSTER_IDENTITY_CREATE_OIDC_CLIENT', index=31, number=125,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_IDENTITY_LIST_OIDC_CLIENTS', index=32, number=127,
+      name='CLUSTER_IDENTITY_UPDATE_OIDC_CLIENT', index=32, number=126,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_IDENTITY_GET_OIDC_CLIENT', index=33, number=128,
+      name='CLUSTER_IDENTITY_LIST_OIDC_CLIENTS', index=33, number=127,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_IDENTITY_DELETE_OIDC_CLIENT', index=34, number=129,
+      name='CLUSTER_IDENTITY_GET_OIDC_CLIENT', index=34, number=128,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_DEBUG_DUMP', index=35, number=131,
+      name='CLUSTER_IDENTITY_DELETE_OIDC_CLIENT', index=35, number=129,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_LICENSE_ACTIVATE', index=36, number=132,
+      name='CLUSTER_DEBUG_DUMP', index=36, number=131,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_LICENSE_GET_CODE', index=37, number=133,
+      name='CLUSTER_LICENSE_ACTIVATE', index=37, number=132,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_LICENSE_ADD_CLUSTER', index=38, number=134,
+      name='CLUSTER_LICENSE_GET_CODE', index=38, number=133,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_LICENSE_UPDATE_CLUSTER', index=39, number=135,
+      name='CLUSTER_LICENSE_ADD_CLUSTER', index=39, number=134,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_LICENSE_DELETE_CLUSTER', index=40, number=136,
+      name='CLUSTER_LICENSE_UPDATE_CLUSTER', index=40, number=135,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_LICENSE_LIST_CLUSTERS', index=41, number=137,
+      name='CLUSTER_LICENSE_DELETE_CLUSTER', index=41, number=136,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_CREATE_SECRET', index=42, number=143,
+      name='CLUSTER_LICENSE_LIST_CLUSTERS', index=42, number=137,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_LIST_SECRETS', index=43, number=144,
+      name='CLUSTER_CREATE_SECRET', index=43, number=143,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='SECRET_DELETE', index=44, number=145,
+      name='CLUSTER_LIST_SECRETS', index=44, number=144,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='SECRET_INSPECT', index=45, number=146,
+      name='SECRET_DELETE', index=45, number=145,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='CLUSTER_DELETE_ALL', index=46, number=138,
+      name='SECRET_INSPECT', index=46, number=146,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='REPO_READ', index=47, number=200,
+      name='CLUSTER_DELETE_ALL', index=47, number=138,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='REPO_WRITE', index=48, number=201,
+      name='REPO_READ', index=48, number=200,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='REPO_MODIFY_BINDINGS', index=49, number=202,
+      name='REPO_WRITE', index=49, number=201,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='REPO_DELETE', index=50, number=203,
+      name='REPO_MODIFY_BINDINGS', index=50, number=202,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='REPO_INSPECT_COMMIT', index=51, number=204,
+      name='REPO_DELETE', index=51, number=203,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='REPO_LIST_COMMIT', index=52, number=205,
+      name='REPO_INSPECT_COMMIT', index=52, number=204,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='REPO_DELETE_COMMIT', index=53, number=206,
+      name='REPO_LIST_COMMIT', index=53, number=205,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='REPO_CREATE_BRANCH', index=54, number=207,
+      name='REPO_DELETE_COMMIT', index=54, number=206,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='REPO_LIST_BRANCH', index=55, number=208,
+      name='REPO_CREATE_BRANCH', index=55, number=207,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='REPO_DELETE_BRANCH', index=56, number=209,
+      name='REPO_LIST_BRANCH', index=56, number=208,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='REPO_INSPECT_FILE', index=57, number=210,
+      name='REPO_DELETE_BRANCH', index=57, number=209,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='REPO_LIST_FILE', index=58, number=211,
+      name='REPO_INSPECT_FILE', index=58, number=210,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='REPO_ADD_PIPELINE_READER', index=59, number=212,
+      name='REPO_LIST_FILE', index=59, number=211,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='REPO_REMOVE_PIPELINE_READER', index=60, number=213,
+      name='REPO_ADD_PIPELINE_READER', index=60, number=212,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='REPO_ADD_PIPELINE_WRITER', index=61, number=214,
+      name='REPO_REMOVE_PIPELINE_READER', index=61, number=213,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='PIPELINE_LIST_JOB', index=62, number=301,
+      name='REPO_ADD_PIPELINE_WRITER', index=62, number=214,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='PROJECT_CREATE', index=63, number=400,
+      name='PIPELINE_LIST_JOB', index=63, number=301,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='PROJECT_DELETE', index=64, number=401,
+      name='PROJECT_CREATE', index=64, number=400,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='PROJECT_LIST_REPO', index=65, number=402,
+      name='PROJECT_DELETE', index=65, number=401,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='PROJECT_CREATE_REPO', index=66, number=403,
+      name='PROJECT_LIST_REPO', index=66, number=402,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='PROJECT_MODIFY_BINDINGS', index=67, number=404,
+      name='PROJECT_CREATE_REPO', index=67, number=403,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='PROJECT_MODIFY_BINDINGS', index=68, number=404,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
   serialized_start=3538,
-  serialized_end=5599,
+  serialized_end=5627,
 )
 _sym_db.RegisterEnumDescriptor(_PERMISSION)
 
 Permission = enum_type_wrapper.EnumTypeWrapper(_PERMISSION)
 _RESOURCETYPE = _descriptor.EnumDescriptor(
   name='ResourceType',
   full_name='auth_v2.ResourceType',
@@ -412,24 +417,25 @@
       name='PROJECT', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=5601,
-  serialized_end=5693,
+  serialized_start=5629,
+  serialized_end=5721,
 )
 _sym_db.RegisterEnumDescriptor(_RESOURCETYPE)
 
 ResourceType = enum_type_wrapper.EnumTypeWrapper(_RESOURCETYPE)
 PERMISSION_UNKNOWN = 0
 CLUSTER_MODIFY_BINDINGS = 100
 CLUSTER_GET_BINDINGS = 101
 CLUSTER_GET_PACHD_LOGS = 148
+CLUSTER_GET_LOKI_LOGS = 150
 CLUSTER_AUTH_ACTIVATE = 102
 CLUSTER_AUTH_DEACTIVATE = 103
 CLUSTER_AUTH_GET_CONFIG = 104
 CLUSTER_AUTH_SET_CONFIG = 105
 CLUSTER_AUTH_GET_ROBOT_TOKEN = 139
 CLUSTER_AUTH_MODIFY_GROUP_MEMBERS = 109
 CLUSTER_AUTH_GET_GROUPS = 110
@@ -3110,16 +3116,16 @@
 _API = _descriptor.ServiceDescriptor(
   name='API',
   full_name='auth_v2.API',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=5696,
-  serialized_end=7862,
+  serialized_start=5724,
+  serialized_end=7890,
   methods=[
   _descriptor.MethodDescriptor(
     name='Activate',
     full_name='auth_v2.API.Activate',
     index=0,
     containing_service=None,
     input_type=_ACTIVATEREQUEST,
```

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/auth/auth_pb2_grpc.py` & `python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/auth/auth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/debug/debug_pb2.py` & `python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/debug/debug_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,20 +18,60 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='python_pachyderm/proto/v2/debug/debug.proto',
   package='debug_v2',
   syntax='proto3',
   serialized_options=b'Z+github.com/pachyderm/pachyderm/v2/src/debug',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n+python_pachyderm/proto/v2/debug/debug.proto\x12\x08\x64\x65\x62ug_v2\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\'python_pachyderm/proto/v2/pps/pps.proto\"V\n\x0eProfileRequest\x12\"\n\x07profile\x18\x01 \x01(\x0b\x32\x11.debug_v2.Profile\x12 \n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x10.debug_v2.Filter\"D\n\x07Profile\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\x08\x64uration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\"\x81\x01\n\x06\x46ilter\x12\x0f\n\x05pachd\x18\x01 \x01(\x08H\x00\x12$\n\x08pipeline\x18\x02 \x01(\x0b\x32\x10.pps_v2.PipelineH\x00\x12\"\n\x06worker\x18\x03 \x01(\x0b\x32\x10.debug_v2.WorkerH\x00\x12\x12\n\x08\x64\x61tabase\x18\x04 \x01(\x08H\x00\x42\x08\n\x06\x66ilter\")\n\x06Worker\x12\x0b\n\x03pod\x18\x01 \x01(\t\x12\x12\n\nredirected\x18\x02 \x01(\x08\"1\n\rBinaryRequest\x12 \n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x10.debug_v2.Filter\">\n\x0b\x44umpRequest\x12 \n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x10.debug_v2.Filter\x12\r\n\x05limit\x18\x02 \x01(\x03\x32\xd1\x01\n\x05\x44\x65\x62ug\x12\x44\n\x07Profile\x12\x18.debug_v2.ProfileRequest\x1a\x1b.google.protobuf.BytesValue\"\x00\x30\x01\x12\x42\n\x06\x42inary\x12\x17.debug_v2.BinaryRequest\x1a\x1b.google.protobuf.BytesValue\"\x00\x30\x01\x12>\n\x04\x44ump\x12\x15.debug_v2.DumpRequest\x1a\x1b.google.protobuf.BytesValue\"\x00\x30\x01\x42-Z+github.com/pachyderm/pachyderm/v2/src/debugb\x06proto3'
+  serialized_pb=b'\n+python_pachyderm/proto/v2/debug/debug.proto\x12\x08\x64\x65\x62ug_v2\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\'python_pachyderm/proto/v2/pps/pps.proto\"V\n\x0eProfileRequest\x12\"\n\x07profile\x18\x01 \x01(\x0b\x32\x11.debug_v2.Profile\x12 \n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x10.debug_v2.Filter\"D\n\x07Profile\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\x08\x64uration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\"\x81\x01\n\x06\x46ilter\x12\x0f\n\x05pachd\x18\x01 \x01(\x08H\x00\x12$\n\x08pipeline\x18\x02 \x01(\x0b\x32\x10.pps_v2.PipelineH\x00\x12\"\n\x06worker\x18\x03 \x01(\x0b\x32\x10.debug_v2.WorkerH\x00\x12\x12\n\x08\x64\x61tabase\x18\x04 \x01(\x08H\x00\x42\x08\n\x06\x66ilter\")\n\x06Worker\x12\x0b\n\x03pod\x18\x01 \x01(\t\x12\x12\n\nredirected\x18\x02 \x01(\x08\"1\n\rBinaryRequest\x12 \n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x10.debug_v2.Filter\">\n\x0b\x44umpRequest\x12 \n\x06\x66ilter\x18\x01 \x01(\x0b\x32\x10.debug_v2.Filter\x12\r\n\x05limit\x18\x02 \x01(\x03\"\x90\x02\n\x12SetLogLevelRequest\x12:\n\tpachyderm\x18\x01 \x01(\x0e\x32%.debug_v2.SetLogLevelRequest.LogLevelH\x00\x12\x35\n\x04grpc\x18\x02 \x01(\x0e\x32%.debug_v2.SetLogLevelRequest.LogLevelH\x00\x12+\n\x08\x64uration\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x0f\n\x07recurse\x18\x04 \x01(\x08\"@\n\x08LogLevel\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05\x44\x45\x42UG\x10\x01\x12\x08\n\x04INFO\x10\x02\x12\t\n\x05\x45RROR\x10\x03\x12\x07\n\x03OFF\x10\x04\x42\x07\n\x05level\"B\n\x13SetLogLevelResponse\x12\x15\n\raffected_pods\x18\x01 \x03(\t\x12\x14\n\x0c\x65rrored_pods\x18\x02 \x03(\t2\x9f\x02\n\x05\x44\x65\x62ug\x12\x44\n\x07Profile\x12\x18.debug_v2.ProfileRequest\x1a\x1b.google.protobuf.BytesValue\"\x00\x30\x01\x12\x42\n\x06\x42inary\x12\x17.debug_v2.BinaryRequest\x1a\x1b.google.protobuf.BytesValue\"\x00\x30\x01\x12>\n\x04\x44ump\x12\x15.debug_v2.DumpRequest\x1a\x1b.google.protobuf.BytesValue\"\x00\x30\x01\x12L\n\x0bSetLogLevel\x12\x1c.debug_v2.SetLogLevelRequest\x1a\x1d.debug_v2.SetLogLevelResponse\"\x00\x42-Z+github.com/pachyderm/pachyderm/v2/src/debugb\x06proto3'
   ,
   dependencies=[google_dot_protobuf_dot_wrappers__pb2.DESCRIPTOR,google_dot_protobuf_dot_duration__pb2.DESCRIPTOR,python__pachyderm_dot_proto_dot_v2_dot_pps_dot_pps__pb2.DESCRIPTOR,])
 
 
 
+_SETLOGLEVELREQUEST_LOGLEVEL = _descriptor.EnumDescriptor(
+  name='LogLevel',
+  full_name='debug_v2.SetLogLevelRequest.LogLevel',
+  filename=None,
+  file=DESCRIPTOR,
+  create_key=_descriptor._internal_create_key,
+  values=[
+    _descriptor.EnumValueDescriptor(
+      name='UNKNOWN', index=0, number=0,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='DEBUG', index=1, number=1,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='INFO', index=2, number=2,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='ERROR', index=3, number=3,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='OFF', index=4, number=4,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+  ],
+  containing_type=None,
+  serialized_options=None,
+  serialized_start=810,
+  serialized_end=874,
+)
+_sym_db.RegisterEnumDescriptor(_SETLOGLEVELREQUEST_LOGLEVEL)
+
 
 _PROFILEREQUEST = _descriptor.Descriptor(
   name='ProfileRequest',
   full_name='debug_v2.ProfileRequest',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
@@ -270,14 +310,112 @@
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=546,
   serialized_end=608,
 )
 
+
+_SETLOGLEVELREQUEST = _descriptor.Descriptor(
+  name='SetLogLevelRequest',
+  full_name='debug_v2.SetLogLevelRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='pachyderm', full_name='debug_v2.SetLogLevelRequest.pachyderm', index=0,
+      number=1, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='grpc', full_name='debug_v2.SetLogLevelRequest.grpc', index=1,
+      number=2, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='duration', full_name='debug_v2.SetLogLevelRequest.duration', index=2,
+      number=3, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='recurse', full_name='debug_v2.SetLogLevelRequest.recurse', index=3,
+      number=4, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+    _SETLOGLEVELREQUEST_LOGLEVEL,
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+    _descriptor.OneofDescriptor(
+      name='level', full_name='debug_v2.SetLogLevelRequest.level',
+      index=0, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
+  ],
+  serialized_start=611,
+  serialized_end=883,
+)
+
+
+_SETLOGLEVELRESPONSE = _descriptor.Descriptor(
+  name='SetLogLevelResponse',
+  full_name='debug_v2.SetLogLevelResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='affected_pods', full_name='debug_v2.SetLogLevelResponse.affected_pods', index=0,
+      number=1, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='errored_pods', full_name='debug_v2.SetLogLevelResponse.errored_pods', index=1,
+      number=2, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=885,
+  serialized_end=951,
+)
+
 _PROFILEREQUEST.fields_by_name['profile'].message_type = _PROFILE
 _PROFILEREQUEST.fields_by_name['filter'].message_type = _FILTER
 _PROFILE.fields_by_name['duration'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
 _FILTER.fields_by_name['pipeline'].message_type = python__pachyderm_dot_proto_dot_v2_dot_pps_dot_pps__pb2._PIPELINE
 _FILTER.fields_by_name['worker'].message_type = _WORKER
 _FILTER.oneofs_by_name['filter'].fields.append(
   _FILTER.fields_by_name['pachd'])
@@ -289,20 +427,32 @@
   _FILTER.fields_by_name['worker'])
 _FILTER.fields_by_name['worker'].containing_oneof = _FILTER.oneofs_by_name['filter']
 _FILTER.oneofs_by_name['filter'].fields.append(
   _FILTER.fields_by_name['database'])
 _FILTER.fields_by_name['database'].containing_oneof = _FILTER.oneofs_by_name['filter']
 _BINARYREQUEST.fields_by_name['filter'].message_type = _FILTER
 _DUMPREQUEST.fields_by_name['filter'].message_type = _FILTER
+_SETLOGLEVELREQUEST.fields_by_name['pachyderm'].enum_type = _SETLOGLEVELREQUEST_LOGLEVEL
+_SETLOGLEVELREQUEST.fields_by_name['grpc'].enum_type = _SETLOGLEVELREQUEST_LOGLEVEL
+_SETLOGLEVELREQUEST.fields_by_name['duration'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
+_SETLOGLEVELREQUEST_LOGLEVEL.containing_type = _SETLOGLEVELREQUEST
+_SETLOGLEVELREQUEST.oneofs_by_name['level'].fields.append(
+  _SETLOGLEVELREQUEST.fields_by_name['pachyderm'])
+_SETLOGLEVELREQUEST.fields_by_name['pachyderm'].containing_oneof = _SETLOGLEVELREQUEST.oneofs_by_name['level']
+_SETLOGLEVELREQUEST.oneofs_by_name['level'].fields.append(
+  _SETLOGLEVELREQUEST.fields_by_name['grpc'])
+_SETLOGLEVELREQUEST.fields_by_name['grpc'].containing_oneof = _SETLOGLEVELREQUEST.oneofs_by_name['level']
 DESCRIPTOR.message_types_by_name['ProfileRequest'] = _PROFILEREQUEST
 DESCRIPTOR.message_types_by_name['Profile'] = _PROFILE
 DESCRIPTOR.message_types_by_name['Filter'] = _FILTER
 DESCRIPTOR.message_types_by_name['Worker'] = _WORKER
 DESCRIPTOR.message_types_by_name['BinaryRequest'] = _BINARYREQUEST
 DESCRIPTOR.message_types_by_name['DumpRequest'] = _DUMPREQUEST
+DESCRIPTOR.message_types_by_name['SetLogLevelRequest'] = _SETLOGLEVELREQUEST
+DESCRIPTOR.message_types_by_name['SetLogLevelResponse'] = _SETLOGLEVELRESPONSE
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 ProfileRequest = _reflection.GeneratedProtocolMessageType('ProfileRequest', (_message.Message,), {
   'DESCRIPTOR' : _PROFILEREQUEST,
   '__module__' : 'python_pachyderm.proto.v2.debug.debug_pb2'
   # @@protoc_insertion_point(class_scope:debug_v2.ProfileRequest)
   })
@@ -339,26 +489,40 @@
 DumpRequest = _reflection.GeneratedProtocolMessageType('DumpRequest', (_message.Message,), {
   'DESCRIPTOR' : _DUMPREQUEST,
   '__module__' : 'python_pachyderm.proto.v2.debug.debug_pb2'
   # @@protoc_insertion_point(class_scope:debug_v2.DumpRequest)
   })
 _sym_db.RegisterMessage(DumpRequest)
 
+SetLogLevelRequest = _reflection.GeneratedProtocolMessageType('SetLogLevelRequest', (_message.Message,), {
+  'DESCRIPTOR' : _SETLOGLEVELREQUEST,
+  '__module__' : 'python_pachyderm.proto.v2.debug.debug_pb2'
+  # @@protoc_insertion_point(class_scope:debug_v2.SetLogLevelRequest)
+  })
+_sym_db.RegisterMessage(SetLogLevelRequest)
+
+SetLogLevelResponse = _reflection.GeneratedProtocolMessageType('SetLogLevelResponse', (_message.Message,), {
+  'DESCRIPTOR' : _SETLOGLEVELRESPONSE,
+  '__module__' : 'python_pachyderm.proto.v2.debug.debug_pb2'
+  # @@protoc_insertion_point(class_scope:debug_v2.SetLogLevelResponse)
+  })
+_sym_db.RegisterMessage(SetLogLevelResponse)
+
 
 DESCRIPTOR._options = None
 
 _DEBUG = _descriptor.ServiceDescriptor(
   name='Debug',
   full_name='debug_v2.Debug',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=611,
-  serialized_end=820,
+  serialized_start=954,
+  serialized_end=1241,
   methods=[
   _descriptor.MethodDescriptor(
     name='Profile',
     full_name='debug_v2.Debug.Profile',
     index=0,
     containing_service=None,
     input_type=_PROFILEREQUEST,
@@ -382,13 +546,23 @@
     index=2,
     containing_service=None,
     input_type=_DUMPREQUEST,
     output_type=google_dot_protobuf_dot_wrappers__pb2._BYTESVALUE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
+  _descriptor.MethodDescriptor(
+    name='SetLogLevel',
+    full_name='debug_v2.Debug.SetLogLevel',
+    index=3,
+    containing_service=None,
+    input_type=_SETLOGLEVELREQUEST,
+    output_type=_SETLOGLEVELRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
 ])
 _sym_db.RegisterServiceDescriptor(_DEBUG)
 
 DESCRIPTOR.services_by_name['Debug'] = _DEBUG
 
 # @@protoc_insertion_point(module_scope)
```

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/debug/debug_pb2_grpc.py` & `python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/debug/debug_pb2_grpc.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,14 +26,19 @@
                 response_deserializer=google_dot_protobuf_dot_wrappers__pb2.BytesValue.FromString,
                 )
         self.Dump = channel.unary_stream(
                 '/debug_v2.Debug/Dump',
                 request_serializer=python__pachyderm_dot_proto_dot_v2_dot_debug_dot_debug__pb2.DumpRequest.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_wrappers__pb2.BytesValue.FromString,
                 )
+        self.SetLogLevel = channel.unary_unary(
+                '/debug_v2.Debug/SetLogLevel',
+                request_serializer=python__pachyderm_dot_proto_dot_v2_dot_debug_dot_debug__pb2.SetLogLevelRequest.SerializeToString,
+                response_deserializer=python__pachyderm_dot_proto_dot_v2_dot_debug_dot_debug__pb2.SetLogLevelResponse.FromString,
+                )
 
 
 class DebugServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def Profile(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -49,14 +54,20 @@
 
     def Dump(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def SetLogLevel(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_DebugServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'Profile': grpc.unary_stream_rpc_method_handler(
                     servicer.Profile,
                     request_deserializer=python__pachyderm_dot_proto_dot_v2_dot_debug_dot_debug__pb2.ProfileRequest.FromString,
                     response_serializer=google_dot_protobuf_dot_wrappers__pb2.BytesValue.SerializeToString,
@@ -67,14 +78,19 @@
                     response_serializer=google_dot_protobuf_dot_wrappers__pb2.BytesValue.SerializeToString,
             ),
             'Dump': grpc.unary_stream_rpc_method_handler(
                     servicer.Dump,
                     request_deserializer=python__pachyderm_dot_proto_dot_v2_dot_debug_dot_debug__pb2.DumpRequest.FromString,
                     response_serializer=google_dot_protobuf_dot_wrappers__pb2.BytesValue.SerializeToString,
             ),
+            'SetLogLevel': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetLogLevel,
+                    request_deserializer=python__pachyderm_dot_proto_dot_v2_dot_debug_dot_debug__pb2.SetLogLevelRequest.FromString,
+                    response_serializer=python__pachyderm_dot_proto_dot_v2_dot_debug_dot_debug__pb2.SetLogLevelResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'debug_v2.Debug', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -127,7 +143,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_stream(request, target, '/debug_v2.Debug/Dump',
             python__pachyderm_dot_proto_dot_v2_dot_debug_dot_debug__pb2.DumpRequest.SerializeToString,
             google_dot_protobuf_dot_wrappers__pb2.BytesValue.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def SetLogLevel(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/debug_v2.Debug/SetLogLevel',
+            python__pachyderm_dot_proto_dot_v2_dot_debug_dot_debug__pb2.SetLogLevelRequest.SerializeToString,
+            python__pachyderm_dot_proto_dot_v2_dot_debug_dot_debug__pb2.SetLogLevelResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/enterprise/enterprise_pb2.py` & `python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/enterprise/enterprise_pb2.py`

 * *Files identical despite different names*

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/enterprise/enterprise_pb2_grpc.py` & `python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/enterprise/enterprise_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/identity/identity_pb2.py` & `python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/identity/identity_pb2.py`

 * *Files identical despite different names*

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/identity/identity_pb2_grpc.py` & `python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/identity/identity_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/license/license_pb2.py` & `python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/license/license_pb2.py`

 * *Files identical despite different names*

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/license/license_pb2_grpc.py` & `python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/license/license_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/pfs/pfs_pb2.py` & `python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/pfs/pfs_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='python_pachyderm/proto/v2/pfs/pfs.proto',
   package='pfs_v2',
   syntax='proto3',
   serialized_options=b'Z)github.com/pachyderm/pachyderm/v2/src/pfs',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\'python_pachyderm/proto/v2/pfs/pfs.proto\x12\x06pfs_v2\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x19google/protobuf/any.proto\x1a)python_pachyderm/proto/v2/auth/auth.proto\x1a)python_pachyderm/proto/v2/task/task.proto\"D\n\x04Repo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12 \n\x07project\x18\x03 \x01(\x0b\x32\x0f.pfs_v2.Project\"2\n\x06\x42ranch\x12\x1a\n\x04repo\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.Repo\x12\x0c\n\x04name\x18\x02 \x01(\t\"C\n\x04\x46ile\x12\x1e\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\r\n\x05\x64\x61tum\x18\x03 \x01(\t\"\x9d\x02\n\x08RepoInfo\x12\x1a\n\x04repo\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.Repo\x12+\n\x07\x63reated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x16size_bytes_upper_bound\x18\x03 \x01(\x03\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12 \n\x08\x62ranches\x18\x05 \x03(\x0b\x32\x0e.pfs_v2.Branch\x12\'\n\tauth_info\x18\x06 \x01(\x0b\x32\x14.pfs_v2.RepoAuthInfo\x12)\n\x07\x64\x65tails\x18\x07 \x01(\x0b\x32\x18.pfs_v2.RepoInfo.Details\x1a\x1d\n\x07\x44\x65tails\x12\x12\n\nsize_bytes\x18\x01 \x01(\x03\"G\n\x0cRepoAuthInfo\x12(\n\x0bpermissions\x18\x01 \x03(\x0e\x32\x13.auth_v2.Permission\x12\r\n\x05roles\x18\x02 \x03(\t\"\xdf\x01\n\nBranchInfo\x12\x1e\n\x06\x62ranch\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Branch\x12\x1c\n\x04head\x18\x02 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\"\n\nprovenance\x18\x03 \x03(\x0b\x32\x0e.pfs_v2.Branch\x12\"\n\nsubvenance\x18\x04 \x03(\x0b\x32\x0e.pfs_v2.Branch\x12)\n\x11\x64irect_provenance\x18\x05 \x03(\x0b\x32\x0e.pfs_v2.Branch\x12 \n\x07trigger\x18\x06 \x01(\x0b\x32\x0f.pfs_v2.Trigger\"X\n\x07Trigger\x12\x0e\n\x06\x62ranch\x18\x01 \x01(\t\x12\x0b\n\x03\x61ll\x18\x02 \x01(\x08\x12\x11\n\tcron_spec\x18\x03 \x01(\t\x12\x0c\n\x04size\x18\x04 \x01(\t\x12\x0f\n\x07\x63ommits\x18\x05 \x01(\x03\"0\n\x0c\x43ommitOrigin\x12 \n\x04kind\x18\x01 \x01(\x0e\x32\x12.pfs_v2.OriginKind\"4\n\x06\x43ommit\x12\x1e\n\x06\x62ranch\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Branch\x12\n\n\x02id\x18\x02 \x01(\t\"\xce\x04\n\nCommitInfo\x12\x1e\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12$\n\x06origin\x18\x02 \x01(\x0b\x32\x14.pfs_v2.CommitOrigin\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12%\n\rparent_commit\x18\x04 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12%\n\rchild_commits\x18\x05 \x03(\x0b\x32\x0e.pfs_v2.Commit\x12+\n\x07started\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\tfinishing\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x66inished\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x11\x64irect_provenance\x18\t \x03(\x0b\x32\x0e.pfs_v2.Branch\x12\r\n\x05\x65rror\x18\n \x01(\t\x12\x1e\n\x16size_bytes_upper_bound\x18\x0b \x01(\x03\x12+\n\x07\x64\x65tails\x18\x0c \x01(\x0b\x32\x1a.pfs_v2.CommitInfo.Details\x1a\x85\x01\n\x07\x44\x65tails\x12\x12\n\nsize_bytes\x18\x01 \x01(\x03\x12\x32\n\x0f\x63ompacting_time\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x32\n\x0fvalidating_time\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\"\x17\n\tCommitSet\x12\n\n\x02id\x18\x01 \x01(\t\"[\n\rCommitSetInfo\x12%\n\ncommit_set\x18\x01 \x01(\x0b\x32\x11.pfs_v2.CommitSet\x12#\n\x07\x63ommits\x18\x02 \x03(\x0b\x32\x12.pfs_v2.CommitInfo\"\x9c\x01\n\x08\x46ileInfo\x12\x1a\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.File\x12#\n\tfile_type\x18\x02 \x01(\x0e\x32\x10.pfs_v2.FileType\x12-\n\tcommitted\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nsize_bytes\x18\x04 \x01(\x03\x12\x0c\n\x04hash\x18\x05 \x01(\x0c\"\x17\n\x07Project\x12\x0c\n\x04name\x18\x01 \x01(\t\"D\n\x0bProjectInfo\x12 \n\x07project\x18\x01 \x01(\x0b\x32\x0f.pfs_v2.Project\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\"T\n\x11\x43reateRepoRequest\x12\x1a\n\x04repo\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.Repo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06update\x18\x03 \x01(\x08\"0\n\x12InspectRepoRequest\x12\x1a\n\x04repo\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.Repo\"B\n\x0fListRepoRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12!\n\x08projects\x18\x02 \x03(\x0b\x32\x0f.pfs_v2.Project\">\n\x11\x44\x65leteRepoRequest\x12\x1a\n\x04repo\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.Repo\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"S\n\x12\x44\x65leteReposRequest\x12!\n\x08projects\x18\x01 \x03(\x0b\x32\x0f.pfs_v2.Project\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12\x0b\n\x03\x61ll\x18\x03 \x01(\x08\"2\n\x13\x44\x65leteReposResponse\x12\x1b\n\x05repos\x18\x01 \x03(\x0b\x32\x0c.pfs_v2.Repo\"i\n\x12StartCommitRequest\x12\x1e\n\x06parent\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x1e\n\x06\x62ranch\x18\x03 \x01(\x0b\x32\x0e.pfs_v2.Branch\"h\n\x13\x46inishCommitRequest\x12\x1e\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05\x65rror\x18\x03 \x01(\t\x12\r\n\x05\x66orce\x18\x04 \x01(\x08\"Y\n\x14InspectCommitRequest\x12\x1e\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12!\n\x04wait\x18\x02 \x01(\x0e\x32\x13.pfs_v2.CommitState\"\xf2\x01\n\x11ListCommitRequest\x12\x1a\n\x04repo\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.Repo\x12\x1c\n\x04\x66rom\x18\x02 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x1a\n\x02to\x18\x03 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x0e\n\x06number\x18\x04 \x01(\x03\x12\x0f\n\x07reverse\x18\x05 \x01(\x08\x12\x0b\n\x03\x61ll\x18\x06 \x01(\x08\x12\'\n\x0borigin_kind\x18\x07 \x01(\x0e\x32\x12.pfs_v2.OriginKind\x12\x30\n\x0cstarted_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"N\n\x17InspectCommitSetRequest\x12%\n\ncommit_set\x18\x01 \x01(\x0b\x32\x11.pfs_v2.CommitSet\x12\x0c\n\x04wait\x18\x02 \x01(\x08\"8\n\x14ListCommitSetRequest\x12 \n\x07project\x18\x01 \x01(\x0b\x32\x0f.pfs_v2.Project\"?\n\x16SquashCommitSetRequest\x12%\n\ncommit_set\x18\x01 \x01(\x0b\x32\x11.pfs_v2.CommitSet\"=\n\x14\x44ropCommitSetRequest\x12%\n\ncommit_set\x18\x01 \x01(\x0b\x32\x11.pfs_v2.CommitSet\"\xbc\x01\n\x16SubscribeCommitRequest\x12\x1a\n\x04repo\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.Repo\x12\x0e\n\x06\x62ranch\x18\x02 \x01(\t\x12\x1c\n\x04\x66rom\x18\x03 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\"\n\x05state\x18\x04 \x01(\x0e\x32\x13.pfs_v2.CommitState\x12\x0b\n\x03\x61ll\x18\x05 \x01(\x08\x12\'\n\x0borigin_kind\x18\x06 \x01(\x0e\x32\x12.pfs_v2.OriginKind\"4\n\x12\x43learCommitRequest\x12\x1e\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Commit\"\xb1\x01\n\x13\x43reateBranchRequest\x12\x1c\n\x04head\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x1e\n\x06\x62ranch\x18\x02 \x01(\x0b\x32\x0e.pfs_v2.Branch\x12\"\n\nprovenance\x18\x03 \x03(\x0b\x32\x0e.pfs_v2.Branch\x12 \n\x07trigger\x18\x04 \x01(\x0b\x32\x0f.pfs_v2.Trigger\x12\x16\n\x0enew_commit_set\x18\x05 \x01(\x08\"6\n\x14InspectBranchRequest\x12\x1e\n\x06\x62ranch\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Branch\"@\n\x11ListBranchRequest\x12\x1a\n\x04repo\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.Repo\x12\x0f\n\x07reverse\x18\x02 \x01(\x08\"D\n\x13\x44\x65leteBranchRequest\x12\x1e\n\x06\x62ranch\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Branch\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"]\n\x14\x43reateProjectRequest\x12 \n\x07project\x18\x01 \x01(\x0b\x32\x0f.pfs_v2.Project\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06update\x18\x03 \x01(\x08\"9\n\x15InspectProjectRequest\x12 \n\x07project\x18\x01 \x01(\x0b\x32\x0f.pfs_v2.Project\"\x14\n\x12ListProjectRequest\"G\n\x14\x44\x65leteProjectRequest\x12 \n\x07project\x18\x01 \x01(\x0b\x32\x0f.pfs_v2.Project\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"\xb3\x01\n\x07\x41\x64\x64\x46ile\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\r\n\x05\x64\x61tum\x18\x02 \x01(\t\x12*\n\x03raw\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.BytesValueH\x00\x12(\n\x03url\x18\x04 \x01(\x0b\x32\x19.pfs_v2.AddFile.URLSourceH\x00\x1a+\n\tURLSource\x12\x0b\n\x03URL\x18\x01 \x01(\t\x12\x11\n\trecursive\x18\x02 \x01(\x08\x42\x08\n\x06source\")\n\nDeleteFile\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\r\n\x05\x64\x61tum\x18\x02 \x01(\t\"Q\n\x08\x43opyFile\x12\x0b\n\x03\x64st\x18\x01 \x01(\t\x12\r\n\x05\x64\x61tum\x18\x02 \x01(\t\x12\x19\n\x03src\x18\x03 \x01(\x0b\x32\x0c.pfs_v2.File\x12\x0e\n\x06\x61ppend\x18\x04 \x01(\x08\"\xb8\x01\n\x11ModifyFileRequest\x12$\n\nset_commit\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.CommitH\x00\x12#\n\x08\x61\x64\x64_file\x18\x02 \x01(\x0b\x32\x0f.pfs_v2.AddFileH\x00\x12)\n\x0b\x64\x65lete_file\x18\x03 \x01(\x0b\x32\x12.pfs_v2.DeleteFileH\x00\x12%\n\tcopy_file\x18\x04 \x01(\x0b\x32\x10.pfs_v2.CopyFileH\x00\x42\x06\n\x04\x62ody\"p\n\x0eGetFileRequest\x12\x1a\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.File\x12\x0b\n\x03URL\x18\x02 \x01(\t\x12\x0e\n\x06offset\x18\x03 \x01(\x03\x12%\n\npath_range\x18\x04 \x01(\x0b\x32\x11.pfs_v2.PathRange\"0\n\x12InspectFileRequest\x12\x1a\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.File\"|\n\x0fListFileRequest\x12\x1a\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.File\x12&\n\x10paginationMarker\x18\x03 \x01(\x0b\x32\x0c.pfs_v2.File\x12\x0e\n\x06number\x18\x04 \x01(\x03\x12\x0f\n\x07reverse\x18\x05 \x01(\x08J\x04\x08\x02\x10\x03\"v\n\x0fWalkFileRequest\x12\x1a\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.File\x12&\n\x10paginationMarker\x18\x02 \x01(\x0b\x32\x0c.pfs_v2.File\x12\x0e\n\x06number\x18\x03 \x01(\x03\x12\x0f\n\x07reverse\x18\x04 \x01(\x08\"i\n\x0fGlobFileRequest\x12\x1e\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x0f\n\x07pattern\x18\x02 \x01(\t\x12%\n\npath_range\x18\x03 \x01(\x0b\x32\x11.pfs_v2.PathRange\"b\n\x0f\x44iffFileRequest\x12\x1e\n\x08new_file\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.File\x12\x1e\n\x08old_file\x18\x02 \x01(\x0b\x32\x0c.pfs_v2.File\x12\x0f\n\x07shallow\x18\x03 \x01(\x08\"Z\n\x10\x44iffFileResponse\x12\"\n\x08new_file\x18\x01 \x01(\x0b\x32\x10.pfs_v2.FileInfo\x12\"\n\x08old_file\x18\x02 \x01(\x0b\x32\x10.pfs_v2.FileInfo\"i\n\x0b\x46sckRequest\x12\x0b\n\x03\x66ix\x18\x01 \x01(\x08\x12\'\n\rzombie_target\x18\x02 \x01(\x0b\x32\x0e.pfs_v2.CommitH\x00\x12\x14\n\nzombie_all\x18\x03 \x01(\x08H\x00\x42\x0e\n\x0czombie_check\"*\n\x0c\x46sckResponse\x12\x0b\n\x03\x66ix\x18\x01 \x01(\t\x12\r\n\x05\x65rror\x18\x02 \x01(\t\",\n\x15\x43reateFileSetResponse\x12\x13\n\x0b\x66ile_set_id\x18\x01 \x01(\t\"3\n\x11GetFileSetRequest\x12\x1e\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Commit\"H\n\x11\x41\x64\x64\x46ileSetRequest\x12\x1e\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x13\n\x0b\x66ile_set_id\x18\x02 \x01(\t\"?\n\x13RenewFileSetRequest\x12\x13\n\x0b\x66ile_set_id\x18\x01 \x01(\t\x12\x13\n\x0bttl_seconds\x18\x02 \x01(\x03\"S\n\x15\x43omposeFileSetRequest\x12\x14\n\x0c\x66ile_set_ids\x18\x01 \x03(\t\x12\x13\n\x0bttl_seconds\x18\x02 \x01(\x03\x12\x0f\n\x07\x63ompact\x18\x03 \x01(\x08\"*\n\x13ShardFileSetRequest\x12\x13\n\x0b\x66ile_set_id\x18\x01 \x01(\t\")\n\tPathRange\x12\r\n\x05lower\x18\x01 \x01(\t\x12\r\n\x05upper\x18\x02 \x01(\t\"9\n\x14ShardFileSetResponse\x12!\n\x06shards\x18\x01 \x03(\x0b\x32\x11.pfs_v2.PathRange\"V\n\x13\x43heckStorageRequest\x12\x17\n\x0fread_chunk_data\x18\x01 \x01(\x08\x12\x13\n\x0b\x63hunk_begin\x18\x02 \x01(\x0c\x12\x11\n\tchunk_end\x18\x03 \x01(\x0c\"2\n\x14\x43heckStorageResponse\x12\x1a\n\x12\x63hunk_object_count\x18\x01 \x01(\x03\"f\n\x0fPutCacheRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x14\n\x0c\x66ile_set_ids\x18\x03 \x03(\t\x12\x0b\n\x03tag\x18\x04 \x01(\t\"\x1e\n\x0fGetCacheRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\"7\n\x10GetCacheResponse\x12#\n\x05value\x18\x01 \x01(\x0b\x32\x14.google.protobuf.Any\"\'\n\x11\x43learCacheRequest\x12\x12\n\ntag_prefix\x18\x01 \x01(\t\"\x15\n\x13\x41\x63tivateAuthRequest\"\x16\n\x14\x41\x63tivateAuthResponse\"b\n\x12RunLoadTestRequest\x12\x0c\n\x04spec\x18\x01 \x01(\t\x12\x1e\n\x06\x62ranch\x18\x02 \x01(\x0b\x32\x0e.pfs_v2.Branch\x12\x0c\n\x04seed\x18\x03 \x01(\x03\x12\x10\n\x08state_id\x18\x04 \x01(\t\"\x9f\x01\n\x13RunLoadTestResponse\x12\x0c\n\x04spec\x18\x01 \x01(\t\x12\x1e\n\x06\x62ranch\x18\x02 \x01(\x0b\x32\x0e.pfs_v2.Branch\x12\x0c\n\x04seed\x18\x03 \x01(\x03\x12\r\n\x05\x65rror\x18\x04 \x01(\t\x12+\n\x08\x64uration\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x10\n\x08state_id\x18\x06 \x01(\t\"\"\n\x13ObjectStorageEgress\x12\x0b\n\x03url\x18\x01 \x01(\t\"\xc0\x02\n\x11SQLDatabaseEgress\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x39\n\x0b\x66ile_format\x18\x02 \x01(\x0b\x32$.pfs_v2.SQLDatabaseEgress.FileFormat\x12\x30\n\x06secret\x18\x03 \x01(\x0b\x32 .pfs_v2.SQLDatabaseEgress.Secret\x1a\x8b\x01\n\nFileFormat\x12\x37\n\x04type\x18\x01 \x01(\x0e\x32).pfs_v2.SQLDatabaseEgress.FileFormat.Type\x12\x0f\n\x07\x63olumns\x18\x02 \x03(\t\"3\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03\x43SV\x10\x01\x12\x08\n\x04JSON\x10\x02\x12\x0b\n\x07PARQUET\x10\x03\x1a#\n\x06Secret\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\"\xa3\x01\n\rEgressRequest\x12\x1e\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x35\n\x0eobject_storage\x18\x02 \x01(\x0b\x32\x1b.pfs_v2.ObjectStorageEgressH\x00\x12\x31\n\x0csql_database\x18\x03 \x01(\x0b\x32\x19.pfs_v2.SQLDatabaseEgressH\x00\x42\x08\n\x06target\"\xeb\x02\n\x0e\x45gressResponse\x12\x44\n\x0eobject_storage\x18\x01 \x01(\x0b\x32*.pfs_v2.EgressResponse.ObjectStorageResultH\x00\x12@\n\x0csql_database\x18\x02 \x01(\x0b\x32(.pfs_v2.EgressResponse.SQLDatabaseResultH\x00\x1a,\n\x13ObjectStorageResult\x12\x15\n\rbytes_written\x18\x01 \x01(\x03\x1a\x98\x01\n\x11SQLDatabaseResult\x12O\n\x0crows_written\x18\x01 \x03(\x0b\x32\x39.pfs_v2.EgressResponse.SQLDatabaseResult.RowsWrittenEntry\x1a\x32\n\x10RowsWrittenEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x03:\x02\x38\x01\x42\x08\n\x06result*N\n\nOriginKind\x12\x17\n\x13ORIGIN_KIND_UNKNOWN\x10\x00\x12\x08\n\x04USER\x10\x01\x12\x08\n\x04\x41UTO\x10\x02\x12\x08\n\x04\x46SCK\x10\x03\x12\t\n\x05\x41LIAS\x10\x04*+\n\x08\x46ileType\x12\x0c\n\x08RESERVED\x10\x00\x12\x08\n\x04\x46ILE\x10\x01\x12\x07\n\x03\x44IR\x10\x02*\\\n\x0b\x43ommitState\x12\x18\n\x14\x43OMMIT_STATE_UNKNOWN\x10\x00\x12\x0b\n\x07STARTED\x10\x01\x12\t\n\x05READY\x10\x02\x12\r\n\tFINISHING\x10\x03\x12\x0c\n\x08\x46INISHED\x10\x04*;\n\tDelimiter\x12\x08\n\x04NONE\x10\x00\x12\x08\n\x04JSON\x10\x01\x12\x08\n\x04LINE\x10\x02\x12\x07\n\x03SQL\x10\x03\x12\x07\n\x03\x43SV\x10\x04\x32\xef\x19\n\x03\x41PI\x12\x41\n\nCreateRepo\x12\x19.pfs_v2.CreateRepoRequest\x1a\x16.google.protobuf.Empty\"\x00\x12=\n\x0bInspectRepo\x12\x1a.pfs_v2.InspectRepoRequest\x1a\x10.pfs_v2.RepoInfo\"\x00\x12\x39\n\x08ListRepo\x12\x17.pfs_v2.ListRepoRequest\x1a\x10.pfs_v2.RepoInfo\"\x00\x30\x01\x12\x41\n\nDeleteRepo\x12\x19.pfs_v2.DeleteRepoRequest\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x0b\x44\x65leteRepos\x12\x1a.pfs_v2.DeleteReposRequest\x1a\x1b.pfs_v2.DeleteReposResponse\"\x00\x12;\n\x0bStartCommit\x12\x1a.pfs_v2.StartCommitRequest\x1a\x0e.pfs_v2.Commit\"\x00\x12\x45\n\x0c\x46inishCommit\x12\x1b.pfs_v2.FinishCommitRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x43\n\x0b\x43learCommit\x12\x1a.pfs_v2.ClearCommitRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x43\n\rInspectCommit\x12\x1c.pfs_v2.InspectCommitRequest\x1a\x12.pfs_v2.CommitInfo\"\x00\x12?\n\nListCommit\x12\x19.pfs_v2.ListCommitRequest\x1a\x12.pfs_v2.CommitInfo\"\x00\x30\x01\x12I\n\x0fSubscribeCommit\x12\x1e.pfs_v2.SubscribeCommitRequest\x1a\x12.pfs_v2.CommitInfo\"\x00\x30\x01\x12K\n\x10InspectCommitSet\x12\x1f.pfs_v2.InspectCommitSetRequest\x1a\x12.pfs_v2.CommitInfo\"\x00\x30\x01\x12H\n\rListCommitSet\x12\x1c.pfs_v2.ListCommitSetRequest\x1a\x15.pfs_v2.CommitSetInfo\"\x00\x30\x01\x12K\n\x0fSquashCommitSet\x12\x1e.pfs_v2.SquashCommitSetRequest\x1a\x16.google.protobuf.Empty\"\x00\x12G\n\rDropCommitSet\x12\x1c.pfs_v2.DropCommitSetRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x45\n\x0c\x43reateBranch\x12\x1b.pfs_v2.CreateBranchRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x43\n\rInspectBranch\x12\x1c.pfs_v2.InspectBranchRequest\x1a\x12.pfs_v2.BranchInfo\"\x00\x12?\n\nListBranch\x12\x19.pfs_v2.ListBranchRequest\x1a\x12.pfs_v2.BranchInfo\"\x00\x30\x01\x12\x45\n\x0c\x44\x65leteBranch\x12\x1b.pfs_v2.DeleteBranchRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x43\n\nModifyFile\x12\x19.pfs_v2.ModifyFileRequest\x1a\x16.google.protobuf.Empty\"\x00(\x01\x12\x42\n\x07GetFile\x12\x16.pfs_v2.GetFileRequest\x1a\x1b.google.protobuf.BytesValue\"\x00\x30\x01\x12\x45\n\nGetFileTAR\x12\x16.pfs_v2.GetFileRequest\x1a\x1b.google.protobuf.BytesValue\"\x00\x30\x01\x12=\n\x0bInspectFile\x12\x1a.pfs_v2.InspectFileRequest\x1a\x10.pfs_v2.FileInfo\"\x00\x12\x39\n\x08ListFile\x12\x17.pfs_v2.ListFileRequest\x1a\x10.pfs_v2.FileInfo\"\x00\x30\x01\x12\x39\n\x08WalkFile\x12\x17.pfs_v2.WalkFileRequest\x1a\x10.pfs_v2.FileInfo\"\x00\x30\x01\x12\x39\n\x08GlobFile\x12\x17.pfs_v2.GlobFileRequest\x1a\x10.pfs_v2.FileInfo\"\x00\x30\x01\x12\x41\n\x08\x44iffFile\x12\x17.pfs_v2.DiffFileRequest\x1a\x18.pfs_v2.DiffFileResponse\"\x00\x30\x01\x12K\n\x0c\x41\x63tivateAuth\x12\x1b.pfs_v2.ActivateAuthRequest\x1a\x1c.pfs_v2.ActivateAuthResponse\"\x00\x12=\n\tDeleteAll\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12\x35\n\x04\x46sck\x12\x13.pfs_v2.FsckRequest\x1a\x14.pfs_v2.FsckResponse\"\x00\x30\x01\x12M\n\rCreateFileSet\x12\x19.pfs_v2.ModifyFileRequest\x1a\x1d.pfs_v2.CreateFileSetResponse\"\x00(\x01\x12H\n\nGetFileSet\x12\x19.pfs_v2.GetFileSetRequest\x1a\x1d.pfs_v2.CreateFileSetResponse\"\x00\x12\x41\n\nAddFileSet\x12\x19.pfs_v2.AddFileSetRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x45\n\x0cRenewFileSet\x12\x1b.pfs_v2.RenewFileSetRequest\x1a\x16.google.protobuf.Empty\"\x00\x12P\n\x0e\x43omposeFileSet\x12\x1d.pfs_v2.ComposeFileSetRequest\x1a\x1d.pfs_v2.CreateFileSetResponse\"\x00\x12K\n\x0cShardFileSet\x12\x1b.pfs_v2.ShardFileSetRequest\x1a\x1c.pfs_v2.ShardFileSetResponse\"\x00\x12K\n\x0c\x43heckStorage\x12\x1b.pfs_v2.CheckStorageRequest\x1a\x1c.pfs_v2.CheckStorageResponse\"\x00\x12=\n\x08PutCache\x12\x17.pfs_v2.PutCacheRequest\x1a\x16.google.protobuf.Empty\"\x00\x12?\n\x08GetCache\x12\x17.pfs_v2.GetCacheRequest\x1a\x18.pfs_v2.GetCacheResponse\"\x00\x12\x41\n\nClearCache\x12\x19.pfs_v2.ClearCacheRequest\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x0bRunLoadTest\x12\x1a.pfs_v2.RunLoadTestRequest\x1a\x1b.pfs_v2.RunLoadTestResponse\"\x00\x12K\n\x12RunLoadTestDefault\x12\x16.google.protobuf.Empty\x1a\x1b.pfs_v2.RunLoadTestResponse\"\x00\x12;\n\x08ListTask\x12\x18.taskapi.ListTaskRequest\x1a\x11.taskapi.TaskInfo\"\x00\x30\x01\x12\x39\n\x06\x45gress\x12\x15.pfs_v2.EgressRequest\x1a\x16.pfs_v2.EgressResponse\"\x00\x12G\n\rCreateProject\x12\x1c.pfs_v2.CreateProjectRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x46\n\x0eInspectProject\x12\x1d.pfs_v2.InspectProjectRequest\x1a\x13.pfs_v2.ProjectInfo\"\x00\x12\x42\n\x0bListProject\x12\x1a.pfs_v2.ListProjectRequest\x1a\x13.pfs_v2.ProjectInfo\"\x00\x30\x01\x12G\n\rDeleteProject\x12\x1c.pfs_v2.DeleteProjectRequest\x1a\x16.google.protobuf.Empty\"\x00\x42+Z)github.com/pachyderm/pachyderm/v2/src/pfsb\x06proto3'
+  serialized_pb=b'\n\'python_pachyderm/proto/v2/pfs/pfs.proto\x12\x06pfs_v2\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x19google/protobuf/any.proto\x1a)python_pachyderm/proto/v2/auth/auth.proto\x1a)python_pachyderm/proto/v2/task/task.proto\"D\n\x04Repo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12 \n\x07project\x18\x03 \x01(\x0b\x32\x0f.pfs_v2.Project\"2\n\x06\x42ranch\x12\x1a\n\x04repo\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.Repo\x12\x0c\n\x04name\x18\x02 \x01(\t\"C\n\x04\x46ile\x12\x1e\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\r\n\x05\x64\x61tum\x18\x03 \x01(\t\"\x99\x02\n\x08RepoInfo\x12\x1a\n\x04repo\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.Repo\x12+\n\x07\x63reated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1e\n\x16size_bytes_upper_bound\x18\x03 \x01(\x03\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12 \n\x08\x62ranches\x18\x05 \x03(\x0b\x32\x0e.pfs_v2.Branch\x12#\n\tauth_info\x18\x06 \x01(\x0b\x32\x10.pfs_v2.AuthInfo\x12)\n\x07\x64\x65tails\x18\x07 \x01(\x0b\x32\x18.pfs_v2.RepoInfo.Details\x1a\x1d\n\x07\x44\x65tails\x12\x12\n\nsize_bytes\x18\x01 \x01(\x03\"C\n\x08\x41uthInfo\x12(\n\x0bpermissions\x18\x01 \x03(\x0e\x32\x13.auth_v2.Permission\x12\r\n\x05roles\x18\x02 \x03(\t\"\xdf\x01\n\nBranchInfo\x12\x1e\n\x06\x62ranch\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Branch\x12\x1c\n\x04head\x18\x02 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\"\n\nprovenance\x18\x03 \x03(\x0b\x32\x0e.pfs_v2.Branch\x12\"\n\nsubvenance\x18\x04 \x03(\x0b\x32\x0e.pfs_v2.Branch\x12)\n\x11\x64irect_provenance\x18\x05 \x03(\x0b\x32\x0e.pfs_v2.Branch\x12 \n\x07trigger\x18\x06 \x01(\x0b\x32\x0f.pfs_v2.Trigger\"X\n\x07Trigger\x12\x0e\n\x06\x62ranch\x18\x01 \x01(\t\x12\x0b\n\x03\x61ll\x18\x02 \x01(\x08\x12\x11\n\tcron_spec\x18\x03 \x01(\t\x12\x0c\n\x04size\x18\x04 \x01(\t\x12\x0f\n\x07\x63ommits\x18\x05 \x01(\x03\"0\n\x0c\x43ommitOrigin\x12 \n\x04kind\x18\x01 \x01(\x0e\x32\x12.pfs_v2.OriginKind\"P\n\x06\x43ommit\x12\x1a\n\x04repo\x18\x03 \x01(\x0b\x32\x0c.pfs_v2.Repo\x12\n\n\x02id\x18\x02 \x01(\t\x12\x1e\n\x06\x62ranch\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Branch\"\xd4\x04\n\nCommitInfo\x12\x1e\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12$\n\x06origin\x18\x02 \x01(\x0b\x32\x14.pfs_v2.CommitOrigin\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12%\n\rparent_commit\x18\x04 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12%\n\rchild_commits\x18\x05 \x03(\x0b\x32\x0e.pfs_v2.Commit\x12+\n\x07started\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\tfinishing\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x66inished\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x11\x64irect_provenance\x18\r \x03(\x0b\x32\x0e.pfs_v2.Commit\x12\r\n\x05\x65rror\x18\n \x01(\t\x12\x1e\n\x16size_bytes_upper_bound\x18\x0b \x01(\x03\x12+\n\x07\x64\x65tails\x18\x0c \x01(\x0b\x32\x1a.pfs_v2.CommitInfo.Details\x1a\x85\x01\n\x07\x44\x65tails\x12\x12\n\nsize_bytes\x18\x01 \x01(\x03\x12\x32\n\x0f\x63ompacting_time\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x32\n\x0fvalidating_time\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationJ\x04\x08\t\x10\n\"\x17\n\tCommitSet\x12\n\n\x02id\x18\x01 \x01(\t\"[\n\rCommitSetInfo\x12%\n\ncommit_set\x18\x01 \x01(\x0b\x32\x11.pfs_v2.CommitSet\x12#\n\x07\x63ommits\x18\x02 \x03(\x0b\x32\x12.pfs_v2.CommitInfo\"\x9c\x01\n\x08\x46ileInfo\x12\x1a\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.File\x12#\n\tfile_type\x18\x02 \x01(\x0e\x32\x10.pfs_v2.FileType\x12-\n\tcommitted\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nsize_bytes\x18\x04 \x01(\x03\x12\x0c\n\x04hash\x18\x05 \x01(\x0c\"\x17\n\x07Project\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x99\x01\n\x0bProjectInfo\x12 \n\x07project\x18\x01 \x01(\x0b\x32\x0f.pfs_v2.Project\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12#\n\tauth_info\x18\x03 \x01(\x0b\x32\x10.pfs_v2.AuthInfo\x12.\n\ncreated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"T\n\x11\x43reateRepoRequest\x12\x1a\n\x04repo\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.Repo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06update\x18\x03 \x01(\x08\"0\n\x12InspectRepoRequest\x12\x1a\n\x04repo\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.Repo\"B\n\x0fListRepoRequest\x12\x0c\n\x04type\x18\x01 \x01(\t\x12!\n\x08projects\x18\x02 \x03(\x0b\x32\x0f.pfs_v2.Project\">\n\x11\x44\x65leteRepoRequest\x12\x1a\n\x04repo\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.Repo\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"S\n\x12\x44\x65leteReposRequest\x12!\n\x08projects\x18\x01 \x03(\x0b\x32\x0f.pfs_v2.Project\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12\x0b\n\x03\x61ll\x18\x03 \x01(\x08\"2\n\x13\x44\x65leteReposResponse\x12\x1b\n\x05repos\x18\x01 \x03(\x0b\x32\x0c.pfs_v2.Repo\"i\n\x12StartCommitRequest\x12\x1e\n\x06parent\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x1e\n\x06\x62ranch\x18\x03 \x01(\x0b\x32\x0e.pfs_v2.Branch\"h\n\x13\x46inishCommitRequest\x12\x1e\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05\x65rror\x18\x03 \x01(\t\x12\r\n\x05\x66orce\x18\x04 \x01(\x08\"Y\n\x14InspectCommitRequest\x12\x1e\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12!\n\x04wait\x18\x02 \x01(\x0e\x32\x13.pfs_v2.CommitState\"\xf2\x01\n\x11ListCommitRequest\x12\x1a\n\x04repo\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.Repo\x12\x1c\n\x04\x66rom\x18\x02 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x1a\n\x02to\x18\x03 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x0e\n\x06number\x18\x04 \x01(\x03\x12\x0f\n\x07reverse\x18\x05 \x01(\x08\x12\x0b\n\x03\x61ll\x18\x06 \x01(\x08\x12\'\n\x0borigin_kind\x18\x07 \x01(\x0e\x32\x12.pfs_v2.OriginKind\x12\x30\n\x0cstarted_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"N\n\x17InspectCommitSetRequest\x12%\n\ncommit_set\x18\x01 \x01(\x0b\x32\x11.pfs_v2.CommitSet\x12\x0c\n\x04wait\x18\x02 \x01(\x08\"8\n\x14ListCommitSetRequest\x12 \n\x07project\x18\x01 \x01(\x0b\x32\x0f.pfs_v2.Project\"?\n\x16SquashCommitSetRequest\x12%\n\ncommit_set\x18\x01 \x01(\x0b\x32\x11.pfs_v2.CommitSet\"=\n\x14\x44ropCommitSetRequest\x12%\n\ncommit_set\x18\x01 \x01(\x0b\x32\x11.pfs_v2.CommitSet\"\xbc\x01\n\x16SubscribeCommitRequest\x12\x1a\n\x04repo\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.Repo\x12\x0e\n\x06\x62ranch\x18\x02 \x01(\t\x12\x1c\n\x04\x66rom\x18\x03 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\"\n\x05state\x18\x04 \x01(\x0e\x32\x13.pfs_v2.CommitState\x12\x0b\n\x03\x61ll\x18\x05 \x01(\x08\x12\'\n\x0borigin_kind\x18\x06 \x01(\x0e\x32\x12.pfs_v2.OriginKind\"4\n\x12\x43learCommitRequest\x12\x1e\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Commit\"\xb1\x01\n\x13\x43reateBranchRequest\x12\x1c\n\x04head\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x1e\n\x06\x62ranch\x18\x02 \x01(\x0b\x32\x0e.pfs_v2.Branch\x12\"\n\nprovenance\x18\x03 \x03(\x0b\x32\x0e.pfs_v2.Branch\x12 \n\x07trigger\x18\x04 \x01(\x0b\x32\x0f.pfs_v2.Trigger\x12\x16\n\x0enew_commit_set\x18\x05 \x01(\x08\"U\n\x12\x46indCommitsRequest\x12\x1d\n\x05start\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x11\n\tfile_path\x18\x02 \x01(\t\x12\r\n\x05limit\x18\x03 \x01(\r\"\x91\x01\n\x13\x46indCommitsResponse\x12&\n\x0c\x66ound_commit\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.CommitH\x00\x12.\n\x14last_searched_commit\x18\x02 \x01(\x0b\x32\x0e.pfs_v2.CommitH\x00\x12\x18\n\x10\x63ommits_searched\x18\x03 \x01(\rB\x08\n\x06result\"6\n\x14InspectBranchRequest\x12\x1e\n\x06\x62ranch\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Branch\"@\n\x11ListBranchRequest\x12\x1a\n\x04repo\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.Repo\x12\x0f\n\x07reverse\x18\x02 \x01(\x08\"D\n\x13\x44\x65leteBranchRequest\x12\x1e\n\x06\x62ranch\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Branch\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"]\n\x14\x43reateProjectRequest\x12 \n\x07project\x18\x01 \x01(\x0b\x32\x0f.pfs_v2.Project\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06update\x18\x03 \x01(\x08\"9\n\x15InspectProjectRequest\x12 \n\x07project\x18\x01 \x01(\x0b\x32\x0f.pfs_v2.Project\"\x14\n\x12ListProjectRequest\"G\n\x14\x44\x65leteProjectRequest\x12 \n\x07project\x18\x01 \x01(\x0b\x32\x0f.pfs_v2.Project\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\"\xc8\x01\n\x07\x41\x64\x64\x46ile\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\r\n\x05\x64\x61tum\x18\x02 \x01(\t\x12*\n\x03raw\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.BytesValueH\x00\x12(\n\x03url\x18\x04 \x01(\x0b\x32\x19.pfs_v2.AddFile.URLSourceH\x00\x1a@\n\tURLSource\x12\x0b\n\x03URL\x18\x01 \x01(\t\x12\x11\n\trecursive\x18\x02 \x01(\x08\x12\x13\n\x0b\x63oncurrency\x18\x03 \x01(\rB\x08\n\x06source\")\n\nDeleteFile\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\r\n\x05\x64\x61tum\x18\x02 \x01(\t\"Q\n\x08\x43opyFile\x12\x0b\n\x03\x64st\x18\x01 \x01(\t\x12\r\n\x05\x64\x61tum\x18\x02 \x01(\t\x12\x19\n\x03src\x18\x03 \x01(\x0b\x32\x0c.pfs_v2.File\x12\x0e\n\x06\x61ppend\x18\x04 \x01(\x08\"\xb8\x01\n\x11ModifyFileRequest\x12$\n\nset_commit\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.CommitH\x00\x12#\n\x08\x61\x64\x64_file\x18\x02 \x01(\x0b\x32\x0f.pfs_v2.AddFileH\x00\x12)\n\x0b\x64\x65lete_file\x18\x03 \x01(\x0b\x32\x12.pfs_v2.DeleteFileH\x00\x12%\n\tcopy_file\x18\x04 \x01(\x0b\x32\x10.pfs_v2.CopyFileH\x00\x42\x06\n\x04\x62ody\"p\n\x0eGetFileRequest\x12\x1a\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.File\x12\x0b\n\x03URL\x18\x02 \x01(\t\x12\x0e\n\x06offset\x18\x03 \x01(\x03\x12%\n\npath_range\x18\x04 \x01(\x0b\x32\x11.pfs_v2.PathRange\"0\n\x12InspectFileRequest\x12\x1a\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.File\"|\n\x0fListFileRequest\x12\x1a\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.File\x12&\n\x10paginationMarker\x18\x03 \x01(\x0b\x32\x0c.pfs_v2.File\x12\x0e\n\x06number\x18\x04 \x01(\x03\x12\x0f\n\x07reverse\x18\x05 \x01(\x08J\x04\x08\x02\x10\x03\"v\n\x0fWalkFileRequest\x12\x1a\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.File\x12&\n\x10paginationMarker\x18\x02 \x01(\x0b\x32\x0c.pfs_v2.File\x12\x0e\n\x06number\x18\x03 \x01(\x03\x12\x0f\n\x07reverse\x18\x04 \x01(\x08\"i\n\x0fGlobFileRequest\x12\x1e\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x0f\n\x07pattern\x18\x02 \x01(\t\x12%\n\npath_range\x18\x03 \x01(\x0b\x32\x11.pfs_v2.PathRange\"b\n\x0f\x44iffFileRequest\x12\x1e\n\x08new_file\x18\x01 \x01(\x0b\x32\x0c.pfs_v2.File\x12\x1e\n\x08old_file\x18\x02 \x01(\x0b\x32\x0c.pfs_v2.File\x12\x0f\n\x07shallow\x18\x03 \x01(\x08\"Z\n\x10\x44iffFileResponse\x12\"\n\x08new_file\x18\x01 \x01(\x0b\x32\x10.pfs_v2.FileInfo\x12\"\n\x08old_file\x18\x02 \x01(\x0b\x32\x10.pfs_v2.FileInfo\"i\n\x0b\x46sckRequest\x12\x0b\n\x03\x66ix\x18\x01 \x01(\x08\x12\'\n\rzombie_target\x18\x02 \x01(\x0b\x32\x0e.pfs_v2.CommitH\x00\x12\x14\n\nzombie_all\x18\x03 \x01(\x08H\x00\x42\x0e\n\x0czombie_check\"*\n\x0c\x46sckResponse\x12\x0b\n\x03\x66ix\x18\x01 \x01(\t\x12\r\n\x05\x65rror\x18\x02 \x01(\t\",\n\x15\x43reateFileSetResponse\x12\x13\n\x0b\x66ile_set_id\x18\x01 \x01(\t\"3\n\x11GetFileSetRequest\x12\x1e\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Commit\"H\n\x11\x41\x64\x64\x46ileSetRequest\x12\x1e\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x13\n\x0b\x66ile_set_id\x18\x02 \x01(\t\"?\n\x13RenewFileSetRequest\x12\x13\n\x0b\x66ile_set_id\x18\x01 \x01(\t\x12\x13\n\x0bttl_seconds\x18\x02 \x01(\x03\"S\n\x15\x43omposeFileSetRequest\x12\x14\n\x0c\x66ile_set_ids\x18\x01 \x03(\t\x12\x13\n\x0bttl_seconds\x18\x02 \x01(\x03\x12\x0f\n\x07\x63ompact\x18\x03 \x01(\x08\"*\n\x13ShardFileSetRequest\x12\x13\n\x0b\x66ile_set_id\x18\x01 \x01(\t\")\n\tPathRange\x12\r\n\x05lower\x18\x01 \x01(\t\x12\r\n\x05upper\x18\x02 \x01(\t\"9\n\x14ShardFileSetResponse\x12!\n\x06shards\x18\x01 \x03(\x0b\x32\x11.pfs_v2.PathRange\"V\n\x13\x43heckStorageRequest\x12\x17\n\x0fread_chunk_data\x18\x01 \x01(\x08\x12\x13\n\x0b\x63hunk_begin\x18\x02 \x01(\x0c\x12\x11\n\tchunk_end\x18\x03 \x01(\x0c\"2\n\x14\x43heckStorageResponse\x12\x1a\n\x12\x63hunk_object_count\x18\x01 \x01(\x03\"f\n\x0fPutCacheRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x14\n\x0c\x66ile_set_ids\x18\x03 \x03(\t\x12\x0b\n\x03tag\x18\x04 \x01(\t\"\x1e\n\x0fGetCacheRequest\x12\x0b\n\x03key\x18\x01 \x01(\t\"7\n\x10GetCacheResponse\x12#\n\x05value\x18\x01 \x01(\x0b\x32\x14.google.protobuf.Any\"\'\n\x11\x43learCacheRequest\x12\x12\n\ntag_prefix\x18\x01 \x01(\t\"\x15\n\x13\x41\x63tivateAuthRequest\"\x16\n\x14\x41\x63tivateAuthResponse\"b\n\x12RunLoadTestRequest\x12\x0c\n\x04spec\x18\x01 \x01(\t\x12\x1e\n\x06\x62ranch\x18\x02 \x01(\x0b\x32\x0e.pfs_v2.Branch\x12\x0c\n\x04seed\x18\x03 \x01(\x03\x12\x10\n\x08state_id\x18\x04 \x01(\t\"\x9f\x01\n\x13RunLoadTestResponse\x12\x0c\n\x04spec\x18\x01 \x01(\t\x12\x1e\n\x06\x62ranch\x18\x02 \x01(\x0b\x32\x0e.pfs_v2.Branch\x12\x0c\n\x04seed\x18\x03 \x01(\x03\x12\r\n\x05\x65rror\x18\x04 \x01(\t\x12+\n\x08\x64uration\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x10\n\x08state_id\x18\x06 \x01(\t\"\"\n\x13ObjectStorageEgress\x12\x0b\n\x03url\x18\x01 \x01(\t\"\xc0\x02\n\x11SQLDatabaseEgress\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x39\n\x0b\x66ile_format\x18\x02 \x01(\x0b\x32$.pfs_v2.SQLDatabaseEgress.FileFormat\x12\x30\n\x06secret\x18\x03 \x01(\x0b\x32 .pfs_v2.SQLDatabaseEgress.Secret\x1a\x8b\x01\n\nFileFormat\x12\x37\n\x04type\x18\x01 \x01(\x0e\x32).pfs_v2.SQLDatabaseEgress.FileFormat.Type\x12\x0f\n\x07\x63olumns\x18\x02 \x03(\t\"3\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03\x43SV\x10\x01\x12\x08\n\x04JSON\x10\x02\x12\x0b\n\x07PARQUET\x10\x03\x1a#\n\x06Secret\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\"\xa3\x01\n\rEgressRequest\x12\x1e\n\x06\x63ommit\x18\x01 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x35\n\x0eobject_storage\x18\x02 \x01(\x0b\x32\x1b.pfs_v2.ObjectStorageEgressH\x00\x12\x31\n\x0csql_database\x18\x03 \x01(\x0b\x32\x19.pfs_v2.SQLDatabaseEgressH\x00\x42\x08\n\x06target\"\xeb\x02\n\x0e\x45gressResponse\x12\x44\n\x0eobject_storage\x18\x01 \x01(\x0b\x32*.pfs_v2.EgressResponse.ObjectStorageResultH\x00\x12@\n\x0csql_database\x18\x02 \x01(\x0b\x32(.pfs_v2.EgressResponse.SQLDatabaseResultH\x00\x1a,\n\x13ObjectStorageResult\x12\x15\n\rbytes_written\x18\x01 \x01(\x03\x1a\x98\x01\n\x11SQLDatabaseResult\x12O\n\x0crows_written\x18\x01 \x03(\x0b\x32\x39.pfs_v2.EgressResponse.SQLDatabaseResult.RowsWrittenEntry\x1a\x32\n\x10RowsWrittenEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x03:\x02\x38\x01\x42\x08\n\x06result*C\n\nOriginKind\x12\x17\n\x13ORIGIN_KIND_UNKNOWN\x10\x00\x12\x08\n\x04USER\x10\x01\x12\x08\n\x04\x41UTO\x10\x02\x12\x08\n\x04\x46SCK\x10\x03*+\n\x08\x46ileType\x12\x0c\n\x08RESERVED\x10\x00\x12\x08\n\x04\x46ILE\x10\x01\x12\x07\n\x03\x44IR\x10\x02*\\\n\x0b\x43ommitState\x12\x18\n\x14\x43OMMIT_STATE_UNKNOWN\x10\x00\x12\x0b\n\x07STARTED\x10\x01\x12\t\n\x05READY\x10\x02\x12\r\n\tFINISHING\x10\x03\x12\x0c\n\x08\x46INISHED\x10\x04*;\n\tDelimiter\x12\x08\n\x04NONE\x10\x00\x12\x08\n\x04JSON\x10\x01\x12\x08\n\x04LINE\x10\x02\x12\x07\n\x03SQL\x10\x03\x12\x07\n\x03\x43SV\x10\x04\x32\xbb\x1a\n\x03\x41PI\x12\x41\n\nCreateRepo\x12\x19.pfs_v2.CreateRepoRequest\x1a\x16.google.protobuf.Empty\"\x00\x12=\n\x0bInspectRepo\x12\x1a.pfs_v2.InspectRepoRequest\x1a\x10.pfs_v2.RepoInfo\"\x00\x12\x39\n\x08ListRepo\x12\x17.pfs_v2.ListRepoRequest\x1a\x10.pfs_v2.RepoInfo\"\x00\x30\x01\x12\x41\n\nDeleteRepo\x12\x19.pfs_v2.DeleteRepoRequest\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x0b\x44\x65leteRepos\x12\x1a.pfs_v2.DeleteReposRequest\x1a\x1b.pfs_v2.DeleteReposResponse\"\x00\x12;\n\x0bStartCommit\x12\x1a.pfs_v2.StartCommitRequest\x1a\x0e.pfs_v2.Commit\"\x00\x12\x45\n\x0c\x46inishCommit\x12\x1b.pfs_v2.FinishCommitRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x43\n\x0b\x43learCommit\x12\x1a.pfs_v2.ClearCommitRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x43\n\rInspectCommit\x12\x1c.pfs_v2.InspectCommitRequest\x1a\x12.pfs_v2.CommitInfo\"\x00\x12?\n\nListCommit\x12\x19.pfs_v2.ListCommitRequest\x1a\x12.pfs_v2.CommitInfo\"\x00\x30\x01\x12I\n\x0fSubscribeCommit\x12\x1e.pfs_v2.SubscribeCommitRequest\x1a\x12.pfs_v2.CommitInfo\"\x00\x30\x01\x12K\n\x10InspectCommitSet\x12\x1f.pfs_v2.InspectCommitSetRequest\x1a\x12.pfs_v2.CommitInfo\"\x00\x30\x01\x12H\n\rListCommitSet\x12\x1c.pfs_v2.ListCommitSetRequest\x1a\x15.pfs_v2.CommitSetInfo\"\x00\x30\x01\x12K\n\x0fSquashCommitSet\x12\x1e.pfs_v2.SquashCommitSetRequest\x1a\x16.google.protobuf.Empty\"\x00\x12G\n\rDropCommitSet\x12\x1c.pfs_v2.DropCommitSetRequest\x1a\x16.google.protobuf.Empty\"\x00\x12J\n\x0b\x46indCommits\x12\x1a.pfs_v2.FindCommitsRequest\x1a\x1b.pfs_v2.FindCommitsResponse\"\x00\x30\x01\x12\x45\n\x0c\x43reateBranch\x12\x1b.pfs_v2.CreateBranchRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x43\n\rInspectBranch\x12\x1c.pfs_v2.InspectBranchRequest\x1a\x12.pfs_v2.BranchInfo\"\x00\x12?\n\nListBranch\x12\x19.pfs_v2.ListBranchRequest\x1a\x12.pfs_v2.BranchInfo\"\x00\x30\x01\x12\x45\n\x0c\x44\x65leteBranch\x12\x1b.pfs_v2.DeleteBranchRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x43\n\nModifyFile\x12\x19.pfs_v2.ModifyFileRequest\x1a\x16.google.protobuf.Empty\"\x00(\x01\x12\x42\n\x07GetFile\x12\x16.pfs_v2.GetFileRequest\x1a\x1b.google.protobuf.BytesValue\"\x00\x30\x01\x12\x45\n\nGetFileTAR\x12\x16.pfs_v2.GetFileRequest\x1a\x1b.google.protobuf.BytesValue\"\x00\x30\x01\x12=\n\x0bInspectFile\x12\x1a.pfs_v2.InspectFileRequest\x1a\x10.pfs_v2.FileInfo\"\x00\x12\x39\n\x08ListFile\x12\x17.pfs_v2.ListFileRequest\x1a\x10.pfs_v2.FileInfo\"\x00\x30\x01\x12\x39\n\x08WalkFile\x12\x17.pfs_v2.WalkFileRequest\x1a\x10.pfs_v2.FileInfo\"\x00\x30\x01\x12\x39\n\x08GlobFile\x12\x17.pfs_v2.GlobFileRequest\x1a\x10.pfs_v2.FileInfo\"\x00\x30\x01\x12\x41\n\x08\x44iffFile\x12\x17.pfs_v2.DiffFileRequest\x1a\x18.pfs_v2.DiffFileResponse\"\x00\x30\x01\x12K\n\x0c\x41\x63tivateAuth\x12\x1b.pfs_v2.ActivateAuthRequest\x1a\x1c.pfs_v2.ActivateAuthResponse\"\x00\x12=\n\tDeleteAll\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12\x35\n\x04\x46sck\x12\x13.pfs_v2.FsckRequest\x1a\x14.pfs_v2.FsckResponse\"\x00\x30\x01\x12M\n\rCreateFileSet\x12\x19.pfs_v2.ModifyFileRequest\x1a\x1d.pfs_v2.CreateFileSetResponse\"\x00(\x01\x12H\n\nGetFileSet\x12\x19.pfs_v2.GetFileSetRequest\x1a\x1d.pfs_v2.CreateFileSetResponse\"\x00\x12\x41\n\nAddFileSet\x12\x19.pfs_v2.AddFileSetRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x45\n\x0cRenewFileSet\x12\x1b.pfs_v2.RenewFileSetRequest\x1a\x16.google.protobuf.Empty\"\x00\x12P\n\x0e\x43omposeFileSet\x12\x1d.pfs_v2.ComposeFileSetRequest\x1a\x1d.pfs_v2.CreateFileSetResponse\"\x00\x12K\n\x0cShardFileSet\x12\x1b.pfs_v2.ShardFileSetRequest\x1a\x1c.pfs_v2.ShardFileSetResponse\"\x00\x12K\n\x0c\x43heckStorage\x12\x1b.pfs_v2.CheckStorageRequest\x1a\x1c.pfs_v2.CheckStorageResponse\"\x00\x12=\n\x08PutCache\x12\x17.pfs_v2.PutCacheRequest\x1a\x16.google.protobuf.Empty\"\x00\x12?\n\x08GetCache\x12\x17.pfs_v2.GetCacheRequest\x1a\x18.pfs_v2.GetCacheResponse\"\x00\x12\x41\n\nClearCache\x12\x19.pfs_v2.ClearCacheRequest\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x0bRunLoadTest\x12\x1a.pfs_v2.RunLoadTestRequest\x1a\x1b.pfs_v2.RunLoadTestResponse\"\x00\x12K\n\x12RunLoadTestDefault\x12\x16.google.protobuf.Empty\x1a\x1b.pfs_v2.RunLoadTestResponse\"\x00\x12;\n\x08ListTask\x12\x18.taskapi.ListTaskRequest\x1a\x11.taskapi.TaskInfo\"\x00\x30\x01\x12\x39\n\x06\x45gress\x12\x15.pfs_v2.EgressRequest\x1a\x16.pfs_v2.EgressResponse\"\x00\x12G\n\rCreateProject\x12\x1c.pfs_v2.CreateProjectRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x46\n\x0eInspectProject\x12\x1d.pfs_v2.InspectProjectRequest\x1a\x13.pfs_v2.ProjectInfo\"\x00\x12\x42\n\x0bListProject\x12\x1a.pfs_v2.ListProjectRequest\x1a\x13.pfs_v2.ProjectInfo\"\x00\x30\x01\x12G\n\rDeleteProject\x12\x1c.pfs_v2.DeleteProjectRequest\x1a\x16.google.protobuf.Empty\"\x00\x42+Z)github.com/pachyderm/pachyderm/v2/src/pfsb\x06proto3'
   ,
   dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,google_dot_protobuf_dot_wrappers__pb2.DESCRIPTOR,google_dot_protobuf_dot_duration__pb2.DESCRIPTOR,google_dot_protobuf_dot_any__pb2.DESCRIPTOR,python__pachyderm_dot_proto_dot_v2_dot_auth_dot_auth__pb2.DESCRIPTOR,python__pachyderm_dot_proto_dot_v2_dot_task_dot_task__pb2.DESCRIPTOR,])
 
 _ORIGINKIND = _descriptor.EnumDescriptor(
   name='OriginKind',
   full_name='pfs_v2.OriginKind',
   filename=None,
@@ -54,24 +54,19 @@
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
       name='FSCK', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='ALIAS', index=4, number=4,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=7711,
-  serialized_end=7789,
+  serialized_start=8079,
+  serialized_end=8146,
 )
 _sym_db.RegisterEnumDescriptor(_ORIGINKIND)
 
 OriginKind = enum_type_wrapper.EnumTypeWrapper(_ORIGINKIND)
 _FILETYPE = _descriptor.EnumDescriptor(
   name='FileType',
   full_name='pfs_v2.FileType',
@@ -93,16 +88,16 @@
       name='DIR', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=7791,
-  serialized_end=7834,
+  serialized_start=8148,
+  serialized_end=8191,
 )
 _sym_db.RegisterEnumDescriptor(_FILETYPE)
 
 FileType = enum_type_wrapper.EnumTypeWrapper(_FILETYPE)
 _COMMITSTATE = _descriptor.EnumDescriptor(
   name='CommitState',
   full_name='pfs_v2.CommitState',
@@ -134,16 +129,16 @@
       name='FINISHED', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=7836,
-  serialized_end=7928,
+  serialized_start=8193,
+  serialized_end=8285,
 )
 _sym_db.RegisterEnumDescriptor(_COMMITSTATE)
 
 CommitState = enum_type_wrapper.EnumTypeWrapper(_COMMITSTATE)
 _DELIMITER = _descriptor.EnumDescriptor(
   name='Delimiter',
   full_name='pfs_v2.Delimiter',
@@ -175,25 +170,24 @@
       name='CSV', index=4, number=4,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=7930,
-  serialized_end=7989,
+  serialized_start=8287,
+  serialized_end=8346,
 )
 _sym_db.RegisterEnumDescriptor(_DELIMITER)
 
 Delimiter = enum_type_wrapper.EnumTypeWrapper(_DELIMITER)
 ORIGIN_KIND_UNKNOWN = 0
 USER = 1
 AUTO = 2
 FSCK = 3
-ALIAS = 4
 RESERVED = 0
 FILE = 1
 DIR = 2
 COMMIT_STATE_UNKNOWN = 0
 STARTED = 1
 READY = 2
 FINISHING = 3
@@ -231,16 +225,16 @@
       name='PARQUET', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=7089,
-  serialized_end=7140,
+  serialized_start=7457,
+  serialized_end=7508,
 )
 _sym_db.RegisterEnumDescriptor(_SQLDATABASEEGRESS_FILEFORMAT_TYPE)
 
 
 _REPO = _descriptor.Descriptor(
   name='Repo',
   full_name='pfs_v2.Repo',
@@ -395,16 +389,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=738,
-  serialized_end=767,
+  serialized_start=734,
+  serialized_end=763,
 )
 
 _REPOINFO = _descriptor.Descriptor(
   name='RepoInfo',
   full_name='pfs_v2.RepoInfo',
   filename=None,
   file=DESCRIPTOR,
@@ -469,35 +463,35 @@
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=482,
-  serialized_end=767,
+  serialized_end=763,
 )
 
 
-_REPOAUTHINFO = _descriptor.Descriptor(
-  name='RepoAuthInfo',
-  full_name='pfs_v2.RepoAuthInfo',
+_AUTHINFO = _descriptor.Descriptor(
+  name='AuthInfo',
+  full_name='pfs_v2.AuthInfo',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='permissions', full_name='pfs_v2.RepoAuthInfo.permissions', index=0,
+      name='permissions', full_name='pfs_v2.AuthInfo.permissions', index=0,
       number=1, type=14, cpp_type=8, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='roles', full_name='pfs_v2.RepoAuthInfo.roles', index=1,
+      name='roles', full_name='pfs_v2.AuthInfo.roles', index=1,
       number=2, type=9, cpp_type=9, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -507,16 +501,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=769,
-  serialized_end=840,
+  serialized_start=765,
+  serialized_end=832,
 )
 
 
 _BRANCHINFO = _descriptor.Descriptor(
   name='BranchInfo',
   full_name='pfs_v2.BranchInfo',
   filename=None,
@@ -574,16 +568,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=843,
-  serialized_end=1066,
+  serialized_start=835,
+  serialized_end=1058,
 )
 
 
 _TRIGGER = _descriptor.Descriptor(
   name='Trigger',
   full_name='pfs_v2.Trigger',
   filename=None,
@@ -634,16 +628,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1068,
-  serialized_end=1156,
+  serialized_start=1060,
+  serialized_end=1148,
 )
 
 
 _COMMITORIGIN = _descriptor.Descriptor(
   name='CommitOrigin',
   full_name='pfs_v2.CommitOrigin',
   filename=None,
@@ -666,55 +660,62 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1158,
-  serialized_end=1206,
+  serialized_start=1150,
+  serialized_end=1198,
 )
 
 
 _COMMIT = _descriptor.Descriptor(
   name='Commit',
   full_name='pfs_v2.Commit',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   create_key=_descriptor._internal_create_key,
   fields=[
     _descriptor.FieldDescriptor(
-      name='branch', full_name='pfs_v2.Commit.branch', index=0,
-      number=1, type=11, cpp_type=10, label=1,
+      name='repo', full_name='pfs_v2.Commit.repo', index=0,
+      number=3, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
       name='id', full_name='pfs_v2.Commit.id', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='branch', full_name='pfs_v2.Commit.branch', index=2,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1208,
-  serialized_end=1260,
+  serialized_start=1200,
+  serialized_end=1280,
 )
 
 
 _COMMITINFO_DETAILS = _descriptor.Descriptor(
   name='Details',
   full_name='pfs_v2.CommitInfo.Details',
   filename=None,
@@ -751,16 +752,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1720,
-  serialized_end=1853,
+  serialized_start=1740,
+  serialized_end=1873,
 )
 
 _COMMITINFO = _descriptor.Descriptor(
   name='CommitInfo',
   full_name='pfs_v2.CommitInfo',
   filename=None,
   file=DESCRIPTOR,
@@ -821,15 +822,15 @@
       number=8, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
       name='direct_provenance', full_name='pfs_v2.CommitInfo.direct_provenance', index=8,
-      number=9, type=11, cpp_type=10, label=3,
+      number=13, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
       name='error', full_name='pfs_v2.CommitInfo.error', index=9,
       number=10, type=9, cpp_type=9, label=1,
@@ -859,16 +860,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1263,
-  serialized_end=1853,
+  serialized_start=1283,
+  serialized_end=1879,
 )
 
 
 _COMMITSET = _descriptor.Descriptor(
   name='CommitSet',
   full_name='pfs_v2.CommitSet',
   filename=None,
@@ -891,16 +892,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1855,
-  serialized_end=1878,
+  serialized_start=1881,
+  serialized_end=1904,
 )
 
 
 _COMMITSETINFO = _descriptor.Descriptor(
   name='CommitSetInfo',
   full_name='pfs_v2.CommitSetInfo',
   filename=None,
@@ -930,16 +931,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1880,
-  serialized_end=1971,
+  serialized_start=1906,
+  serialized_end=1997,
 )
 
 
 _FILEINFO = _descriptor.Descriptor(
   name='FileInfo',
   full_name='pfs_v2.FileInfo',
   filename=None,
@@ -990,16 +991,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1974,
-  serialized_end=2130,
+  serialized_start=2000,
+  serialized_end=2156,
 )
 
 
 _PROJECT = _descriptor.Descriptor(
   name='Project',
   full_name='pfs_v2.Project',
   filename=None,
@@ -1022,16 +1023,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2132,
-  serialized_end=2155,
+  serialized_start=2158,
+  serialized_end=2181,
 )
 
 
 _PROJECTINFO = _descriptor.Descriptor(
   name='ProjectInfo',
   full_name='pfs_v2.ProjectInfo',
   filename=None,
@@ -1049,28 +1050,42 @@
     _descriptor.FieldDescriptor(
       name='description', full_name='pfs_v2.ProjectInfo.description', index=1,
       number=2, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='auth_info', full_name='pfs_v2.ProjectInfo.auth_info', index=2,
+      number=3, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='created_at', full_name='pfs_v2.ProjectInfo.created_at', index=3,
+      number=4, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2157,
-  serialized_end=2225,
+  serialized_start=2184,
+  serialized_end=2337,
 )
 
 
 _CREATEREPOREQUEST = _descriptor.Descriptor(
   name='CreateRepoRequest',
   full_name='pfs_v2.CreateRepoRequest',
   filename=None,
@@ -1107,16 +1122,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2227,
-  serialized_end=2311,
+  serialized_start=2339,
+  serialized_end=2423,
 )
 
 
 _INSPECTREPOREQUEST = _descriptor.Descriptor(
   name='InspectRepoRequest',
   full_name='pfs_v2.InspectRepoRequest',
   filename=None,
@@ -1139,16 +1154,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2313,
-  serialized_end=2361,
+  serialized_start=2425,
+  serialized_end=2473,
 )
 
 
 _LISTREPOREQUEST = _descriptor.Descriptor(
   name='ListRepoRequest',
   full_name='pfs_v2.ListRepoRequest',
   filename=None,
@@ -1178,16 +1193,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2363,
-  serialized_end=2429,
+  serialized_start=2475,
+  serialized_end=2541,
 )
 
 
 _DELETEREPOREQUEST = _descriptor.Descriptor(
   name='DeleteRepoRequest',
   full_name='pfs_v2.DeleteRepoRequest',
   filename=None,
@@ -1217,16 +1232,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2431,
-  serialized_end=2493,
+  serialized_start=2543,
+  serialized_end=2605,
 )
 
 
 _DELETEREPOSREQUEST = _descriptor.Descriptor(
   name='DeleteReposRequest',
   full_name='pfs_v2.DeleteReposRequest',
   filename=None,
@@ -1263,16 +1278,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2495,
-  serialized_end=2578,
+  serialized_start=2607,
+  serialized_end=2690,
 )
 
 
 _DELETEREPOSRESPONSE = _descriptor.Descriptor(
   name='DeleteReposResponse',
   full_name='pfs_v2.DeleteReposResponse',
   filename=None,
@@ -1295,16 +1310,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2580,
-  serialized_end=2630,
+  serialized_start=2692,
+  serialized_end=2742,
 )
 
 
 _STARTCOMMITREQUEST = _descriptor.Descriptor(
   name='StartCommitRequest',
   full_name='pfs_v2.StartCommitRequest',
   filename=None,
@@ -1341,16 +1356,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2632,
-  serialized_end=2737,
+  serialized_start=2744,
+  serialized_end=2849,
 )
 
 
 _FINISHCOMMITREQUEST = _descriptor.Descriptor(
   name='FinishCommitRequest',
   full_name='pfs_v2.FinishCommitRequest',
   filename=None,
@@ -1394,16 +1409,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2739,
-  serialized_end=2843,
+  serialized_start=2851,
+  serialized_end=2955,
 )
 
 
 _INSPECTCOMMITREQUEST = _descriptor.Descriptor(
   name='InspectCommitRequest',
   full_name='pfs_v2.InspectCommitRequest',
   filename=None,
@@ -1433,16 +1448,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2845,
-  serialized_end=2934,
+  serialized_start=2957,
+  serialized_end=3046,
 )
 
 
 _LISTCOMMITREQUEST = _descriptor.Descriptor(
   name='ListCommitRequest',
   full_name='pfs_v2.ListCommitRequest',
   filename=None,
@@ -1514,16 +1529,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2937,
-  serialized_end=3179,
+  serialized_start=3049,
+  serialized_end=3291,
 )
 
 
 _INSPECTCOMMITSETREQUEST = _descriptor.Descriptor(
   name='InspectCommitSetRequest',
   full_name='pfs_v2.InspectCommitSetRequest',
   filename=None,
@@ -1553,16 +1568,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3181,
-  serialized_end=3259,
+  serialized_start=3293,
+  serialized_end=3371,
 )
 
 
 _LISTCOMMITSETREQUEST = _descriptor.Descriptor(
   name='ListCommitSetRequest',
   full_name='pfs_v2.ListCommitSetRequest',
   filename=None,
@@ -1585,16 +1600,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3261,
-  serialized_end=3317,
+  serialized_start=3373,
+  serialized_end=3429,
 )
 
 
 _SQUASHCOMMITSETREQUEST = _descriptor.Descriptor(
   name='SquashCommitSetRequest',
   full_name='pfs_v2.SquashCommitSetRequest',
   filename=None,
@@ -1617,16 +1632,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3319,
-  serialized_end=3382,
+  serialized_start=3431,
+  serialized_end=3494,
 )
 
 
 _DROPCOMMITSETREQUEST = _descriptor.Descriptor(
   name='DropCommitSetRequest',
   full_name='pfs_v2.DropCommitSetRequest',
   filename=None,
@@ -1649,16 +1664,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3384,
-  serialized_end=3445,
+  serialized_start=3496,
+  serialized_end=3557,
 )
 
 
 _SUBSCRIBECOMMITREQUEST = _descriptor.Descriptor(
   name='SubscribeCommitRequest',
   full_name='pfs_v2.SubscribeCommitRequest',
   filename=None,
@@ -1716,16 +1731,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3448,
-  serialized_end=3636,
+  serialized_start=3560,
+  serialized_end=3748,
 )
 
 
 _CLEARCOMMITREQUEST = _descriptor.Descriptor(
   name='ClearCommitRequest',
   full_name='pfs_v2.ClearCommitRequest',
   filename=None,
@@ -1748,16 +1763,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3638,
-  serialized_end=3690,
+  serialized_start=3750,
+  serialized_end=3802,
 )
 
 
 _CREATEBRANCHREQUEST = _descriptor.Descriptor(
   name='CreateBranchRequest',
   full_name='pfs_v2.CreateBranchRequest',
   filename=None,
@@ -1808,16 +1823,113 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3693,
-  serialized_end=3870,
+  serialized_start=3805,
+  serialized_end=3982,
+)
+
+
+_FINDCOMMITSREQUEST = _descriptor.Descriptor(
+  name='FindCommitsRequest',
+  full_name='pfs_v2.FindCommitsRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='start', full_name='pfs_v2.FindCommitsRequest.start', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='file_path', full_name='pfs_v2.FindCommitsRequest.file_path', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='limit', full_name='pfs_v2.FindCommitsRequest.limit', index=2,
+      number=3, type=13, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3984,
+  serialized_end=4069,
+)
+
+
+_FINDCOMMITSRESPONSE = _descriptor.Descriptor(
+  name='FindCommitsResponse',
+  full_name='pfs_v2.FindCommitsResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='found_commit', full_name='pfs_v2.FindCommitsResponse.found_commit', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='last_searched_commit', full_name='pfs_v2.FindCommitsResponse.last_searched_commit', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='commits_searched', full_name='pfs_v2.FindCommitsResponse.commits_searched', index=2,
+      number=3, type=13, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+    _descriptor.OneofDescriptor(
+      name='result', full_name='pfs_v2.FindCommitsResponse.result',
+      index=0, containing_type=None,
+      create_key=_descriptor._internal_create_key,
+    fields=[]),
+  ],
+  serialized_start=4072,
+  serialized_end=4217,
 )
 
 
 _INSPECTBRANCHREQUEST = _descriptor.Descriptor(
   name='InspectBranchRequest',
   full_name='pfs_v2.InspectBranchRequest',
   filename=None,
@@ -1840,16 +1952,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3872,
-  serialized_end=3926,
+  serialized_start=4219,
+  serialized_end=4273,
 )
 
 
 _LISTBRANCHREQUEST = _descriptor.Descriptor(
   name='ListBranchRequest',
   full_name='pfs_v2.ListBranchRequest',
   filename=None,
@@ -1879,16 +1991,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3928,
-  serialized_end=3992,
+  serialized_start=4275,
+  serialized_end=4339,
 )
 
 
 _DELETEBRANCHREQUEST = _descriptor.Descriptor(
   name='DeleteBranchRequest',
   full_name='pfs_v2.DeleteBranchRequest',
   filename=None,
@@ -1918,16 +2030,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3994,
-  serialized_end=4062,
+  serialized_start=4341,
+  serialized_end=4409,
 )
 
 
 _CREATEPROJECTREQUEST = _descriptor.Descriptor(
   name='CreateProjectRequest',
   full_name='pfs_v2.CreateProjectRequest',
   filename=None,
@@ -1964,16 +2076,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4064,
-  serialized_end=4157,
+  serialized_start=4411,
+  serialized_end=4504,
 )
 
 
 _INSPECTPROJECTREQUEST = _descriptor.Descriptor(
   name='InspectProjectRequest',
   full_name='pfs_v2.InspectProjectRequest',
   filename=None,
@@ -1996,16 +2108,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4159,
-  serialized_end=4216,
+  serialized_start=4506,
+  serialized_end=4563,
 )
 
 
 _LISTPROJECTREQUEST = _descriptor.Descriptor(
   name='ListProjectRequest',
   full_name='pfs_v2.ListProjectRequest',
   filename=None,
@@ -2021,16 +2133,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4218,
-  serialized_end=4238,
+  serialized_start=4565,
+  serialized_end=4585,
 )
 
 
 _DELETEPROJECTREQUEST = _descriptor.Descriptor(
   name='DeleteProjectRequest',
   full_name='pfs_v2.DeleteProjectRequest',
   filename=None,
@@ -2060,16 +2172,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4240,
-  serialized_end=4311,
+  serialized_start=4587,
+  serialized_end=4658,
 )
 
 
 _ADDFILE_URLSOURCE = _descriptor.Descriptor(
   name='URLSource',
   full_name='pfs_v2.AddFile.URLSource',
   filename=None,
@@ -2087,28 +2199,35 @@
     _descriptor.FieldDescriptor(
       name='recursive', full_name='pfs_v2.AddFile.URLSource.recursive', index=1,
       number=2, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='concurrency', full_name='pfs_v2.AddFile.URLSource.concurrency', index=2,
+      number=3, type=13, cpp_type=3, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4440,
-  serialized_end=4483,
+  serialized_start=4787,
+  serialized_end=4851,
 )
 
 _ADDFILE = _descriptor.Descriptor(
   name='AddFile',
   full_name='pfs_v2.AddFile',
   filename=None,
   file=DESCRIPTOR,
@@ -2156,16 +2275,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='source', full_name='pfs_v2.AddFile.source',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=4314,
-  serialized_end=4493,
+  serialized_start=4661,
+  serialized_end=4861,
 )
 
 
 _DELETEFILE = _descriptor.Descriptor(
   name='DeleteFile',
   full_name='pfs_v2.DeleteFile',
   filename=None,
@@ -2195,16 +2314,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4495,
-  serialized_end=4536,
+  serialized_start=4863,
+  serialized_end=4904,
 )
 
 
 _COPYFILE = _descriptor.Descriptor(
   name='CopyFile',
   full_name='pfs_v2.CopyFile',
   filename=None,
@@ -2248,16 +2367,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4538,
-  serialized_end=4619,
+  serialized_start=4906,
+  serialized_end=4987,
 )
 
 
 _MODIFYFILEREQUEST = _descriptor.Descriptor(
   name='ModifyFileRequest',
   full_name='pfs_v2.ModifyFileRequest',
   filename=None,
@@ -2306,16 +2425,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='body', full_name='pfs_v2.ModifyFileRequest.body',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=4622,
-  serialized_end=4806,
+  serialized_start=4990,
+  serialized_end=5174,
 )
 
 
 _GETFILEREQUEST = _descriptor.Descriptor(
   name='GetFileRequest',
   full_name='pfs_v2.GetFileRequest',
   filename=None,
@@ -2359,16 +2478,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4808,
-  serialized_end=4920,
+  serialized_start=5176,
+  serialized_end=5288,
 )
 
 
 _INSPECTFILEREQUEST = _descriptor.Descriptor(
   name='InspectFileRequest',
   full_name='pfs_v2.InspectFileRequest',
   filename=None,
@@ -2391,16 +2510,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4922,
-  serialized_end=4970,
+  serialized_start=5290,
+  serialized_end=5338,
 )
 
 
 _LISTFILEREQUEST = _descriptor.Descriptor(
   name='ListFileRequest',
   full_name='pfs_v2.ListFileRequest',
   filename=None,
@@ -2444,16 +2563,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4972,
-  serialized_end=5096,
+  serialized_start=5340,
+  serialized_end=5464,
 )
 
 
 _WALKFILEREQUEST = _descriptor.Descriptor(
   name='WalkFileRequest',
   full_name='pfs_v2.WalkFileRequest',
   filename=None,
@@ -2497,16 +2616,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5098,
-  serialized_end=5216,
+  serialized_start=5466,
+  serialized_end=5584,
 )
 
 
 _GLOBFILEREQUEST = _descriptor.Descriptor(
   name='GlobFileRequest',
   full_name='pfs_v2.GlobFileRequest',
   filename=None,
@@ -2543,16 +2662,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5218,
-  serialized_end=5323,
+  serialized_start=5586,
+  serialized_end=5691,
 )
 
 
 _DIFFFILEREQUEST = _descriptor.Descriptor(
   name='DiffFileRequest',
   full_name='pfs_v2.DiffFileRequest',
   filename=None,
@@ -2589,16 +2708,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5325,
-  serialized_end=5423,
+  serialized_start=5693,
+  serialized_end=5791,
 )
 
 
 _DIFFFILERESPONSE = _descriptor.Descriptor(
   name='DiffFileResponse',
   full_name='pfs_v2.DiffFileResponse',
   filename=None,
@@ -2628,16 +2747,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5425,
-  serialized_end=5515,
+  serialized_start=5793,
+  serialized_end=5883,
 )
 
 
 _FSCKREQUEST = _descriptor.Descriptor(
   name='FsckRequest',
   full_name='pfs_v2.FsckRequest',
   filename=None,
@@ -2679,16 +2798,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='zombie_check', full_name='pfs_v2.FsckRequest.zombie_check',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=5517,
-  serialized_end=5622,
+  serialized_start=5885,
+  serialized_end=5990,
 )
 
 
 _FSCKRESPONSE = _descriptor.Descriptor(
   name='FsckResponse',
   full_name='pfs_v2.FsckResponse',
   filename=None,
@@ -2718,16 +2837,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5624,
-  serialized_end=5666,
+  serialized_start=5992,
+  serialized_end=6034,
 )
 
 
 _CREATEFILESETRESPONSE = _descriptor.Descriptor(
   name='CreateFileSetResponse',
   full_name='pfs_v2.CreateFileSetResponse',
   filename=None,
@@ -2750,16 +2869,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5668,
-  serialized_end=5712,
+  serialized_start=6036,
+  serialized_end=6080,
 )
 
 
 _GETFILESETREQUEST = _descriptor.Descriptor(
   name='GetFileSetRequest',
   full_name='pfs_v2.GetFileSetRequest',
   filename=None,
@@ -2782,16 +2901,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5714,
-  serialized_end=5765,
+  serialized_start=6082,
+  serialized_end=6133,
 )
 
 
 _ADDFILESETREQUEST = _descriptor.Descriptor(
   name='AddFileSetRequest',
   full_name='pfs_v2.AddFileSetRequest',
   filename=None,
@@ -2821,16 +2940,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5767,
-  serialized_end=5839,
+  serialized_start=6135,
+  serialized_end=6207,
 )
 
 
 _RENEWFILESETREQUEST = _descriptor.Descriptor(
   name='RenewFileSetRequest',
   full_name='pfs_v2.RenewFileSetRequest',
   filename=None,
@@ -2860,16 +2979,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5841,
-  serialized_end=5904,
+  serialized_start=6209,
+  serialized_end=6272,
 )
 
 
 _COMPOSEFILESETREQUEST = _descriptor.Descriptor(
   name='ComposeFileSetRequest',
   full_name='pfs_v2.ComposeFileSetRequest',
   filename=None,
@@ -2906,16 +3025,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5906,
-  serialized_end=5989,
+  serialized_start=6274,
+  serialized_end=6357,
 )
 
 
 _SHARDFILESETREQUEST = _descriptor.Descriptor(
   name='ShardFileSetRequest',
   full_name='pfs_v2.ShardFileSetRequest',
   filename=None,
@@ -2938,16 +3057,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5991,
-  serialized_end=6033,
+  serialized_start=6359,
+  serialized_end=6401,
 )
 
 
 _PATHRANGE = _descriptor.Descriptor(
   name='PathRange',
   full_name='pfs_v2.PathRange',
   filename=None,
@@ -2977,16 +3096,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6035,
-  serialized_end=6076,
+  serialized_start=6403,
+  serialized_end=6444,
 )
 
 
 _SHARDFILESETRESPONSE = _descriptor.Descriptor(
   name='ShardFileSetResponse',
   full_name='pfs_v2.ShardFileSetResponse',
   filename=None,
@@ -3009,16 +3128,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6078,
-  serialized_end=6135,
+  serialized_start=6446,
+  serialized_end=6503,
 )
 
 
 _CHECKSTORAGEREQUEST = _descriptor.Descriptor(
   name='CheckStorageRequest',
   full_name='pfs_v2.CheckStorageRequest',
   filename=None,
@@ -3055,16 +3174,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6137,
-  serialized_end=6223,
+  serialized_start=6505,
+  serialized_end=6591,
 )
 
 
 _CHECKSTORAGERESPONSE = _descriptor.Descriptor(
   name='CheckStorageResponse',
   full_name='pfs_v2.CheckStorageResponse',
   filename=None,
@@ -3087,16 +3206,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6225,
-  serialized_end=6275,
+  serialized_start=6593,
+  serialized_end=6643,
 )
 
 
 _PUTCACHEREQUEST = _descriptor.Descriptor(
   name='PutCacheRequest',
   full_name='pfs_v2.PutCacheRequest',
   filename=None,
@@ -3140,16 +3259,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6277,
-  serialized_end=6379,
+  serialized_start=6645,
+  serialized_end=6747,
 )
 
 
 _GETCACHEREQUEST = _descriptor.Descriptor(
   name='GetCacheRequest',
   full_name='pfs_v2.GetCacheRequest',
   filename=None,
@@ -3172,16 +3291,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6381,
-  serialized_end=6411,
+  serialized_start=6749,
+  serialized_end=6779,
 )
 
 
 _GETCACHERESPONSE = _descriptor.Descriptor(
   name='GetCacheResponse',
   full_name='pfs_v2.GetCacheResponse',
   filename=None,
@@ -3204,16 +3323,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6413,
-  serialized_end=6468,
+  serialized_start=6781,
+  serialized_end=6836,
 )
 
 
 _CLEARCACHEREQUEST = _descriptor.Descriptor(
   name='ClearCacheRequest',
   full_name='pfs_v2.ClearCacheRequest',
   filename=None,
@@ -3236,16 +3355,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6470,
-  serialized_end=6509,
+  serialized_start=6838,
+  serialized_end=6877,
 )
 
 
 _ACTIVATEAUTHREQUEST = _descriptor.Descriptor(
   name='ActivateAuthRequest',
   full_name='pfs_v2.ActivateAuthRequest',
   filename=None,
@@ -3261,16 +3380,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6511,
-  serialized_end=6532,
+  serialized_start=6879,
+  serialized_end=6900,
 )
 
 
 _ACTIVATEAUTHRESPONSE = _descriptor.Descriptor(
   name='ActivateAuthResponse',
   full_name='pfs_v2.ActivateAuthResponse',
   filename=None,
@@ -3286,16 +3405,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6534,
-  serialized_end=6556,
+  serialized_start=6902,
+  serialized_end=6924,
 )
 
 
 _RUNLOADTESTREQUEST = _descriptor.Descriptor(
   name='RunLoadTestRequest',
   full_name='pfs_v2.RunLoadTestRequest',
   filename=None,
@@ -3339,16 +3458,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6558,
-  serialized_end=6656,
+  serialized_start=6926,
+  serialized_end=7024,
 )
 
 
 _RUNLOADTESTRESPONSE = _descriptor.Descriptor(
   name='RunLoadTestResponse',
   full_name='pfs_v2.RunLoadTestResponse',
   filename=None,
@@ -3406,16 +3525,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6659,
-  serialized_end=6818,
+  serialized_start=7027,
+  serialized_end=7186,
 )
 
 
 _OBJECTSTORAGEEGRESS = _descriptor.Descriptor(
   name='ObjectStorageEgress',
   full_name='pfs_v2.ObjectStorageEgress',
   filename=None,
@@ -3438,16 +3557,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6820,
-  serialized_end=6854,
+  serialized_start=7188,
+  serialized_end=7222,
 )
 
 
 _SQLDATABASEEGRESS_FILEFORMAT = _descriptor.Descriptor(
   name='FileFormat',
   full_name='pfs_v2.SQLDatabaseEgress.FileFormat',
   filename=None,
@@ -3478,16 +3597,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7001,
-  serialized_end=7140,
+  serialized_start=7369,
+  serialized_end=7508,
 )
 
 _SQLDATABASEEGRESS_SECRET = _descriptor.Descriptor(
   name='Secret',
   full_name='pfs_v2.SQLDatabaseEgress.Secret',
   filename=None,
   file=DESCRIPTOR,
@@ -3516,16 +3635,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7142,
-  serialized_end=7177,
+  serialized_start=7510,
+  serialized_end=7545,
 )
 
 _SQLDATABASEEGRESS = _descriptor.Descriptor(
   name='SQLDatabaseEgress',
   full_name='pfs_v2.SQLDatabaseEgress',
   filename=None,
   file=DESCRIPTOR,
@@ -3561,16 +3680,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6857,
-  serialized_end=7177,
+  serialized_start=7225,
+  serialized_end=7545,
 )
 
 
 _EGRESSREQUEST = _descriptor.Descriptor(
   name='EgressRequest',
   full_name='pfs_v2.EgressRequest',
   filename=None,
@@ -3612,16 +3731,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='target', full_name='pfs_v2.EgressRequest.target',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=7180,
-  serialized_end=7343,
+  serialized_start=7548,
+  serialized_end=7711,
 )
 
 
 _EGRESSRESPONSE_OBJECTSTORAGERESULT = _descriptor.Descriptor(
   name='ObjectStorageResult',
   full_name='pfs_v2.EgressResponse.ObjectStorageResult',
   filename=None,
@@ -3644,16 +3763,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7500,
-  serialized_end=7544,
+  serialized_start=7868,
+  serialized_end=7912,
 )
 
 _EGRESSRESPONSE_SQLDATABASERESULT_ROWSWRITTENENTRY = _descriptor.Descriptor(
   name='RowsWrittenEntry',
   full_name='pfs_v2.EgressResponse.SQLDatabaseResult.RowsWrittenEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -3682,16 +3801,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7649,
-  serialized_end=7699,
+  serialized_start=8017,
+  serialized_end=8067,
 )
 
 _EGRESSRESPONSE_SQLDATABASERESULT = _descriptor.Descriptor(
   name='SQLDatabaseResult',
   full_name='pfs_v2.EgressResponse.SQLDatabaseResult',
   filename=None,
   file=DESCRIPTOR,
@@ -3713,16 +3832,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7547,
-  serialized_end=7699,
+  serialized_start=7915,
+  serialized_end=8067,
 )
 
 _EGRESSRESPONSE = _descriptor.Descriptor(
   name='EgressResponse',
   full_name='pfs_v2.EgressResponse',
   filename=None,
   file=DESCRIPTOR,
@@ -3756,54 +3875,57 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='result', full_name='pfs_v2.EgressResponse.result',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=7346,
-  serialized_end=7709,
+  serialized_start=7714,
+  serialized_end=8077,
 )
 
 _REPO.fields_by_name['project'].message_type = _PROJECT
 _BRANCH.fields_by_name['repo'].message_type = _REPO
 _FILE.fields_by_name['commit'].message_type = _COMMIT
 _REPOINFO_DETAILS.containing_type = _REPOINFO
 _REPOINFO.fields_by_name['repo'].message_type = _REPO
 _REPOINFO.fields_by_name['created'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _REPOINFO.fields_by_name['branches'].message_type = _BRANCH
-_REPOINFO.fields_by_name['auth_info'].message_type = _REPOAUTHINFO
+_REPOINFO.fields_by_name['auth_info'].message_type = _AUTHINFO
 _REPOINFO.fields_by_name['details'].message_type = _REPOINFO_DETAILS
-_REPOAUTHINFO.fields_by_name['permissions'].enum_type = python__pachyderm_dot_proto_dot_v2_dot_auth_dot_auth__pb2._PERMISSION
+_AUTHINFO.fields_by_name['permissions'].enum_type = python__pachyderm_dot_proto_dot_v2_dot_auth_dot_auth__pb2._PERMISSION
 _BRANCHINFO.fields_by_name['branch'].message_type = _BRANCH
 _BRANCHINFO.fields_by_name['head'].message_type = _COMMIT
 _BRANCHINFO.fields_by_name['provenance'].message_type = _BRANCH
 _BRANCHINFO.fields_by_name['subvenance'].message_type = _BRANCH
 _BRANCHINFO.fields_by_name['direct_provenance'].message_type = _BRANCH
 _BRANCHINFO.fields_by_name['trigger'].message_type = _TRIGGER
 _COMMITORIGIN.fields_by_name['kind'].enum_type = _ORIGINKIND
+_COMMIT.fields_by_name['repo'].message_type = _REPO
 _COMMIT.fields_by_name['branch'].message_type = _BRANCH
 _COMMITINFO_DETAILS.fields_by_name['compacting_time'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
 _COMMITINFO_DETAILS.fields_by_name['validating_time'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
 _COMMITINFO_DETAILS.containing_type = _COMMITINFO
 _COMMITINFO.fields_by_name['commit'].message_type = _COMMIT
 _COMMITINFO.fields_by_name['origin'].message_type = _COMMITORIGIN
 _COMMITINFO.fields_by_name['parent_commit'].message_type = _COMMIT
 _COMMITINFO.fields_by_name['child_commits'].message_type = _COMMIT
 _COMMITINFO.fields_by_name['started'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _COMMITINFO.fields_by_name['finishing'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _COMMITINFO.fields_by_name['finished'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
-_COMMITINFO.fields_by_name['direct_provenance'].message_type = _BRANCH
+_COMMITINFO.fields_by_name['direct_provenance'].message_type = _COMMIT
 _COMMITINFO.fields_by_name['details'].message_type = _COMMITINFO_DETAILS
 _COMMITSETINFO.fields_by_name['commit_set'].message_type = _COMMITSET
 _COMMITSETINFO.fields_by_name['commits'].message_type = _COMMITINFO
 _FILEINFO.fields_by_name['file'].message_type = _FILE
 _FILEINFO.fields_by_name['file_type'].enum_type = _FILETYPE
 _FILEINFO.fields_by_name['committed'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _PROJECTINFO.fields_by_name['project'].message_type = _PROJECT
+_PROJECTINFO.fields_by_name['auth_info'].message_type = _AUTHINFO
+_PROJECTINFO.fields_by_name['created_at'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _CREATEREPOREQUEST.fields_by_name['repo'].message_type = _REPO
 _INSPECTREPOREQUEST.fields_by_name['repo'].message_type = _REPO
 _LISTREPOREQUEST.fields_by_name['projects'].message_type = _PROJECT
 _DELETEREPOREQUEST.fields_by_name['repo'].message_type = _REPO
 _DELETEREPOSREQUEST.fields_by_name['projects'].message_type = _PROJECT
 _DELETEREPOSRESPONSE.fields_by_name['repos'].message_type = _REPO
 _STARTCOMMITREQUEST.fields_by_name['parent'].message_type = _COMMIT
@@ -3825,14 +3947,23 @@
 _SUBSCRIBECOMMITREQUEST.fields_by_name['state'].enum_type = _COMMITSTATE
 _SUBSCRIBECOMMITREQUEST.fields_by_name['origin_kind'].enum_type = _ORIGINKIND
 _CLEARCOMMITREQUEST.fields_by_name['commit'].message_type = _COMMIT
 _CREATEBRANCHREQUEST.fields_by_name['head'].message_type = _COMMIT
 _CREATEBRANCHREQUEST.fields_by_name['branch'].message_type = _BRANCH
 _CREATEBRANCHREQUEST.fields_by_name['provenance'].message_type = _BRANCH
 _CREATEBRANCHREQUEST.fields_by_name['trigger'].message_type = _TRIGGER
+_FINDCOMMITSREQUEST.fields_by_name['start'].message_type = _COMMIT
+_FINDCOMMITSRESPONSE.fields_by_name['found_commit'].message_type = _COMMIT
+_FINDCOMMITSRESPONSE.fields_by_name['last_searched_commit'].message_type = _COMMIT
+_FINDCOMMITSRESPONSE.oneofs_by_name['result'].fields.append(
+  _FINDCOMMITSRESPONSE.fields_by_name['found_commit'])
+_FINDCOMMITSRESPONSE.fields_by_name['found_commit'].containing_oneof = _FINDCOMMITSRESPONSE.oneofs_by_name['result']
+_FINDCOMMITSRESPONSE.oneofs_by_name['result'].fields.append(
+  _FINDCOMMITSRESPONSE.fields_by_name['last_searched_commit'])
+_FINDCOMMITSRESPONSE.fields_by_name['last_searched_commit'].containing_oneof = _FINDCOMMITSRESPONSE.oneofs_by_name['result']
 _INSPECTBRANCHREQUEST.fields_by_name['branch'].message_type = _BRANCH
 _LISTBRANCHREQUEST.fields_by_name['repo'].message_type = _REPO
 _DELETEBRANCHREQUEST.fields_by_name['branch'].message_type = _BRANCH
 _CREATEPROJECTREQUEST.fields_by_name['project'].message_type = _PROJECT
 _INSPECTPROJECTREQUEST.fields_by_name['project'].message_type = _PROJECT
 _DELETEPROJECTREQUEST.fields_by_name['project'].message_type = _PROJECT
 _ADDFILE_URLSOURCE.containing_type = _ADDFILE
@@ -3916,15 +4047,15 @@
 _EGRESSRESPONSE.oneofs_by_name['result'].fields.append(
   _EGRESSRESPONSE.fields_by_name['sql_database'])
 _EGRESSRESPONSE.fields_by_name['sql_database'].containing_oneof = _EGRESSRESPONSE.oneofs_by_name['result']
 DESCRIPTOR.message_types_by_name['Repo'] = _REPO
 DESCRIPTOR.message_types_by_name['Branch'] = _BRANCH
 DESCRIPTOR.message_types_by_name['File'] = _FILE
 DESCRIPTOR.message_types_by_name['RepoInfo'] = _REPOINFO
-DESCRIPTOR.message_types_by_name['RepoAuthInfo'] = _REPOAUTHINFO
+DESCRIPTOR.message_types_by_name['AuthInfo'] = _AUTHINFO
 DESCRIPTOR.message_types_by_name['BranchInfo'] = _BRANCHINFO
 DESCRIPTOR.message_types_by_name['Trigger'] = _TRIGGER
 DESCRIPTOR.message_types_by_name['CommitOrigin'] = _COMMITORIGIN
 DESCRIPTOR.message_types_by_name['Commit'] = _COMMIT
 DESCRIPTOR.message_types_by_name['CommitInfo'] = _COMMITINFO
 DESCRIPTOR.message_types_by_name['CommitSet'] = _COMMITSET
 DESCRIPTOR.message_types_by_name['CommitSetInfo'] = _COMMITSETINFO
@@ -3944,14 +4075,16 @@
 DESCRIPTOR.message_types_by_name['InspectCommitSetRequest'] = _INSPECTCOMMITSETREQUEST
 DESCRIPTOR.message_types_by_name['ListCommitSetRequest'] = _LISTCOMMITSETREQUEST
 DESCRIPTOR.message_types_by_name['SquashCommitSetRequest'] = _SQUASHCOMMITSETREQUEST
 DESCRIPTOR.message_types_by_name['DropCommitSetRequest'] = _DROPCOMMITSETREQUEST
 DESCRIPTOR.message_types_by_name['SubscribeCommitRequest'] = _SUBSCRIBECOMMITREQUEST
 DESCRIPTOR.message_types_by_name['ClearCommitRequest'] = _CLEARCOMMITREQUEST
 DESCRIPTOR.message_types_by_name['CreateBranchRequest'] = _CREATEBRANCHREQUEST
+DESCRIPTOR.message_types_by_name['FindCommitsRequest'] = _FINDCOMMITSREQUEST
+DESCRIPTOR.message_types_by_name['FindCommitsResponse'] = _FINDCOMMITSRESPONSE
 DESCRIPTOR.message_types_by_name['InspectBranchRequest'] = _INSPECTBRANCHREQUEST
 DESCRIPTOR.message_types_by_name['ListBranchRequest'] = _LISTBRANCHREQUEST
 DESCRIPTOR.message_types_by_name['DeleteBranchRequest'] = _DELETEBRANCHREQUEST
 DESCRIPTOR.message_types_by_name['CreateProjectRequest'] = _CREATEPROJECTREQUEST
 DESCRIPTOR.message_types_by_name['InspectProjectRequest'] = _INSPECTPROJECTREQUEST
 DESCRIPTOR.message_types_by_name['ListProjectRequest'] = _LISTPROJECTREQUEST
 DESCRIPTOR.message_types_by_name['DeleteProjectRequest'] = _DELETEPROJECTREQUEST
@@ -4028,20 +4161,20 @@
   'DESCRIPTOR' : _REPOINFO,
   '__module__' : 'python_pachyderm.proto.v2.pfs.pfs_pb2'
   # @@protoc_insertion_point(class_scope:pfs_v2.RepoInfo)
   })
 _sym_db.RegisterMessage(RepoInfo)
 _sym_db.RegisterMessage(RepoInfo.Details)
 
-RepoAuthInfo = _reflection.GeneratedProtocolMessageType('RepoAuthInfo', (_message.Message,), {
-  'DESCRIPTOR' : _REPOAUTHINFO,
+AuthInfo = _reflection.GeneratedProtocolMessageType('AuthInfo', (_message.Message,), {
+  'DESCRIPTOR' : _AUTHINFO,
   '__module__' : 'python_pachyderm.proto.v2.pfs.pfs_pb2'
-  # @@protoc_insertion_point(class_scope:pfs_v2.RepoAuthInfo)
+  # @@protoc_insertion_point(class_scope:pfs_v2.AuthInfo)
   })
-_sym_db.RegisterMessage(RepoAuthInfo)
+_sym_db.RegisterMessage(AuthInfo)
 
 BranchInfo = _reflection.GeneratedProtocolMessageType('BranchInfo', (_message.Message,), {
   'DESCRIPTOR' : _BRANCHINFO,
   '__module__' : 'python_pachyderm.proto.v2.pfs.pfs_pb2'
   # @@protoc_insertion_point(class_scope:pfs_v2.BranchInfo)
   })
 _sym_db.RegisterMessage(BranchInfo)
@@ -4232,14 +4365,28 @@
 CreateBranchRequest = _reflection.GeneratedProtocolMessageType('CreateBranchRequest', (_message.Message,), {
   'DESCRIPTOR' : _CREATEBRANCHREQUEST,
   '__module__' : 'python_pachyderm.proto.v2.pfs.pfs_pb2'
   # @@protoc_insertion_point(class_scope:pfs_v2.CreateBranchRequest)
   })
 _sym_db.RegisterMessage(CreateBranchRequest)
 
+FindCommitsRequest = _reflection.GeneratedProtocolMessageType('FindCommitsRequest', (_message.Message,), {
+  'DESCRIPTOR' : _FINDCOMMITSREQUEST,
+  '__module__' : 'python_pachyderm.proto.v2.pfs.pfs_pb2'
+  # @@protoc_insertion_point(class_scope:pfs_v2.FindCommitsRequest)
+  })
+_sym_db.RegisterMessage(FindCommitsRequest)
+
+FindCommitsResponse = _reflection.GeneratedProtocolMessageType('FindCommitsResponse', (_message.Message,), {
+  'DESCRIPTOR' : _FINDCOMMITSRESPONSE,
+  '__module__' : 'python_pachyderm.proto.v2.pfs.pfs_pb2'
+  # @@protoc_insertion_point(class_scope:pfs_v2.FindCommitsResponse)
+  })
+_sym_db.RegisterMessage(FindCommitsResponse)
+
 InspectBranchRequest = _reflection.GeneratedProtocolMessageType('InspectBranchRequest', (_message.Message,), {
   'DESCRIPTOR' : _INSPECTBRANCHREQUEST,
   '__module__' : 'python_pachyderm.proto.v2.pfs.pfs_pb2'
   # @@protoc_insertion_point(class_scope:pfs_v2.InspectBranchRequest)
   })
 _sym_db.RegisterMessage(InspectBranchRequest)
 
@@ -4585,16 +4732,16 @@
 _API = _descriptor.ServiceDescriptor(
   name='API',
   full_name='pfs_v2.API',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=7992,
-  serialized_end=11303,
+  serialized_start=8349,
+  serialized_end=11736,
   methods=[
   _descriptor.MethodDescriptor(
     name='CreateRepo',
     full_name='pfs_v2.API.CreateRepo',
     index=0,
     containing_service=None,
     input_type=_CREATEREPOREQUEST,
@@ -4739,337 +4886,347 @@
     containing_service=None,
     input_type=_DROPCOMMITSETREQUEST,
     output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
+    name='FindCommits',
+    full_name='pfs_v2.API.FindCommits',
+    index=15,
+    containing_service=None,
+    input_type=_FINDCOMMITSREQUEST,
+    output_type=_FINDCOMMITSRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
     name='CreateBranch',
     full_name='pfs_v2.API.CreateBranch',
-    index=15,
+    index=16,
     containing_service=None,
     input_type=_CREATEBRANCHREQUEST,
     output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='InspectBranch',
     full_name='pfs_v2.API.InspectBranch',
-    index=16,
+    index=17,
     containing_service=None,
     input_type=_INSPECTBRANCHREQUEST,
     output_type=_BRANCHINFO,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='ListBranch',
     full_name='pfs_v2.API.ListBranch',
-    index=17,
+    index=18,
     containing_service=None,
     input_type=_LISTBRANCHREQUEST,
     output_type=_BRANCHINFO,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='DeleteBranch',
     full_name='pfs_v2.API.DeleteBranch',
-    index=18,
+    index=19,
     containing_service=None,
     input_type=_DELETEBRANCHREQUEST,
     output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='ModifyFile',
     full_name='pfs_v2.API.ModifyFile',
-    index=19,
+    index=20,
     containing_service=None,
     input_type=_MODIFYFILEREQUEST,
     output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='GetFile',
     full_name='pfs_v2.API.GetFile',
-    index=20,
+    index=21,
     containing_service=None,
     input_type=_GETFILEREQUEST,
     output_type=google_dot_protobuf_dot_wrappers__pb2._BYTESVALUE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='GetFileTAR',
     full_name='pfs_v2.API.GetFileTAR',
-    index=21,
+    index=22,
     containing_service=None,
     input_type=_GETFILEREQUEST,
     output_type=google_dot_protobuf_dot_wrappers__pb2._BYTESVALUE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='InspectFile',
     full_name='pfs_v2.API.InspectFile',
-    index=22,
+    index=23,
     containing_service=None,
     input_type=_INSPECTFILEREQUEST,
     output_type=_FILEINFO,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='ListFile',
     full_name='pfs_v2.API.ListFile',
-    index=23,
+    index=24,
     containing_service=None,
     input_type=_LISTFILEREQUEST,
     output_type=_FILEINFO,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='WalkFile',
     full_name='pfs_v2.API.WalkFile',
-    index=24,
+    index=25,
     containing_service=None,
     input_type=_WALKFILEREQUEST,
     output_type=_FILEINFO,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='GlobFile',
     full_name='pfs_v2.API.GlobFile',
-    index=25,
+    index=26,
     containing_service=None,
     input_type=_GLOBFILEREQUEST,
     output_type=_FILEINFO,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='DiffFile',
     full_name='pfs_v2.API.DiffFile',
-    index=26,
+    index=27,
     containing_service=None,
     input_type=_DIFFFILEREQUEST,
     output_type=_DIFFFILERESPONSE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='ActivateAuth',
     full_name='pfs_v2.API.ActivateAuth',
-    index=27,
+    index=28,
     containing_service=None,
     input_type=_ACTIVATEAUTHREQUEST,
     output_type=_ACTIVATEAUTHRESPONSE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='DeleteAll',
     full_name='pfs_v2.API.DeleteAll',
-    index=28,
+    index=29,
     containing_service=None,
     input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
     output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='Fsck',
     full_name='pfs_v2.API.Fsck',
-    index=29,
+    index=30,
     containing_service=None,
     input_type=_FSCKREQUEST,
     output_type=_FSCKRESPONSE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='CreateFileSet',
     full_name='pfs_v2.API.CreateFileSet',
-    index=30,
+    index=31,
     containing_service=None,
     input_type=_MODIFYFILEREQUEST,
     output_type=_CREATEFILESETRESPONSE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='GetFileSet',
     full_name='pfs_v2.API.GetFileSet',
-    index=31,
+    index=32,
     containing_service=None,
     input_type=_GETFILESETREQUEST,
     output_type=_CREATEFILESETRESPONSE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='AddFileSet',
     full_name='pfs_v2.API.AddFileSet',
-    index=32,
+    index=33,
     containing_service=None,
     input_type=_ADDFILESETREQUEST,
     output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='RenewFileSet',
     full_name='pfs_v2.API.RenewFileSet',
-    index=33,
+    index=34,
     containing_service=None,
     input_type=_RENEWFILESETREQUEST,
     output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='ComposeFileSet',
     full_name='pfs_v2.API.ComposeFileSet',
-    index=34,
+    index=35,
     containing_service=None,
     input_type=_COMPOSEFILESETREQUEST,
     output_type=_CREATEFILESETRESPONSE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='ShardFileSet',
     full_name='pfs_v2.API.ShardFileSet',
-    index=35,
+    index=36,
     containing_service=None,
     input_type=_SHARDFILESETREQUEST,
     output_type=_SHARDFILESETRESPONSE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='CheckStorage',
     full_name='pfs_v2.API.CheckStorage',
-    index=36,
+    index=37,
     containing_service=None,
     input_type=_CHECKSTORAGEREQUEST,
     output_type=_CHECKSTORAGERESPONSE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='PutCache',
     full_name='pfs_v2.API.PutCache',
-    index=37,
+    index=38,
     containing_service=None,
     input_type=_PUTCACHEREQUEST,
     output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='GetCache',
     full_name='pfs_v2.API.GetCache',
-    index=38,
+    index=39,
     containing_service=None,
     input_type=_GETCACHEREQUEST,
     output_type=_GETCACHERESPONSE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='ClearCache',
     full_name='pfs_v2.API.ClearCache',
-    index=39,
+    index=40,
     containing_service=None,
     input_type=_CLEARCACHEREQUEST,
     output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='RunLoadTest',
     full_name='pfs_v2.API.RunLoadTest',
-    index=40,
+    index=41,
     containing_service=None,
     input_type=_RUNLOADTESTREQUEST,
     output_type=_RUNLOADTESTRESPONSE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='RunLoadTestDefault',
     full_name='pfs_v2.API.RunLoadTestDefault',
-    index=41,
+    index=42,
     containing_service=None,
     input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
     output_type=_RUNLOADTESTRESPONSE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='ListTask',
     full_name='pfs_v2.API.ListTask',
-    index=42,
+    index=43,
     containing_service=None,
     input_type=python__pachyderm_dot_proto_dot_v2_dot_task_dot_task__pb2._LISTTASKREQUEST,
     output_type=python__pachyderm_dot_proto_dot_v2_dot_task_dot_task__pb2._TASKINFO,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='Egress',
     full_name='pfs_v2.API.Egress',
-    index=43,
+    index=44,
     containing_service=None,
     input_type=_EGRESSREQUEST,
     output_type=_EGRESSRESPONSE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='CreateProject',
     full_name='pfs_v2.API.CreateProject',
-    index=44,
+    index=45,
     containing_service=None,
     input_type=_CREATEPROJECTREQUEST,
     output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='InspectProject',
     full_name='pfs_v2.API.InspectProject',
-    index=45,
+    index=46,
     containing_service=None,
     input_type=_INSPECTPROJECTREQUEST,
     output_type=_PROJECTINFO,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='ListProject',
     full_name='pfs_v2.API.ListProject',
-    index=46,
+    index=47,
     containing_service=None,
     input_type=_LISTPROJECTREQUEST,
     output_type=_PROJECTINFO,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
   _descriptor.MethodDescriptor(
     name='DeleteProject',
     full_name='pfs_v2.API.DeleteProject',
-    index=47,
+    index=48,
     containing_service=None,
     input_type=_DELETEPROJECTREQUEST,
     output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
 ])
```

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/pfs/pfs_pb2_grpc.py` & `python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/pfs/pfs_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,14 +88,19 @@
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
         self.DropCommitSet = channel.unary_unary(
                 '/pfs_v2.API/DropCommitSet',
                 request_serializer=python__pachyderm_dot_proto_dot_v2_dot_pfs_dot_pfs__pb2.DropCommitSetRequest.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
+        self.FindCommits = channel.unary_stream(
+                '/pfs_v2.API/FindCommits',
+                request_serializer=python__pachyderm_dot_proto_dot_v2_dot_pfs_dot_pfs__pb2.FindCommitsRequest.SerializeToString,
+                response_deserializer=python__pachyderm_dot_proto_dot_v2_dot_pfs_dot_pfs__pb2.FindCommitsResponse.FromString,
+                )
         self.CreateBranch = channel.unary_unary(
                 '/pfs_v2.API/CreateBranch',
                 request_serializer=python__pachyderm_dot_proto_dot_v2_dot_pfs_dot_pfs__pb2.CreateBranchRequest.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
         self.InspectBranch = channel.unary_unary(
                 '/pfs_v2.API/InspectBranch',
@@ -368,14 +373,21 @@
     def DropCommitSet(self, request, context):
         """DropCommitSet drops the commits of a CommitSet and all data included in the commits.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def FindCommits(self, request, context):
+        """FindCommits searches for commits that reference a supplied file being modified in a branch.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def CreateBranch(self, request, context):
         """CreateBranch creates a new branch.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -675,14 +687,19 @@
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
             'DropCommitSet': grpc.unary_unary_rpc_method_handler(
                     servicer.DropCommitSet,
                     request_deserializer=python__pachyderm_dot_proto_dot_v2_dot_pfs_dot_pfs__pb2.DropCommitSetRequest.FromString,
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
+            'FindCommits': grpc.unary_stream_rpc_method_handler(
+                    servicer.FindCommits,
+                    request_deserializer=python__pachyderm_dot_proto_dot_v2_dot_pfs_dot_pfs__pb2.FindCommitsRequest.FromString,
+                    response_serializer=python__pachyderm_dot_proto_dot_v2_dot_pfs_dot_pfs__pb2.FindCommitsResponse.SerializeToString,
+            ),
             'CreateBranch': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateBranch,
                     request_deserializer=python__pachyderm_dot_proto_dot_v2_dot_pfs_dot_pfs__pb2.CreateBranchRequest.FromString,
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
             'InspectBranch': grpc.unary_unary_rpc_method_handler(
                     servicer.InspectBranch,
@@ -1106,14 +1123,31 @@
         return grpc.experimental.unary_unary(request, target, '/pfs_v2.API/DropCommitSet',
             python__pachyderm_dot_proto_dot_v2_dot_pfs_dot_pfs__pb2.DropCommitSetRequest.SerializeToString,
             google_dot_protobuf_dot_empty__pb2.Empty.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def FindCommits(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/pfs_v2.API/FindCommits',
+            python__pachyderm_dot_proto_dot_v2_dot_pfs_dot_pfs__pb2.FindCommitsRequest.SerializeToString,
+            python__pachyderm_dot_proto_dot_v2_dot_pfs_dot_pfs__pb2.FindCommitsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def CreateBranch(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/pps/pps_pb2.py` & `python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/pps/pps_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='python_pachyderm/proto/v2/pps/pps.proto',
   package='pps_v2',
   syntax='proto3',
   serialized_options=b'Z)github.com/pachyderm/pachyderm/v2/src/pps',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\'python_pachyderm/proto/v2/pps/pps.proto\x12\x06pps_v2\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\'python_pachyderm/proto/v2/pfs/pfs.proto\x1a)python_pachyderm/proto/v2/task/task.proto\"M\n\x0bSecretMount\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\x12\n\nmount_path\x18\x03 \x01(\t\x12\x0f\n\x07\x65nv_var\x18\x04 \x01(\t\"\xea\x02\n\tTransform\x12\r\n\x05image\x18\x01 \x01(\t\x12\x0b\n\x03\x63md\x18\x02 \x03(\t\x12\x0f\n\x07\x65rr_cmd\x18\x03 \x03(\t\x12\'\n\x03\x65nv\x18\x04 \x03(\x0b\x32\x1a.pps_v2.Transform.EnvEntry\x12$\n\x07secrets\x18\x05 \x03(\x0b\x32\x13.pps_v2.SecretMount\x12\x1a\n\x12image_pull_secrets\x18\x06 \x03(\t\x12\r\n\x05stdin\x18\x07 \x03(\t\x12\x11\n\terr_stdin\x18\x08 \x03(\t\x12\x1a\n\x12\x61\x63\x63\x65pt_return_code\x18\t \x03(\x03\x12\r\n\x05\x64\x65\x62ug\x18\n \x01(\x08\x12\x0c\n\x04user\x18\x0b \x01(\t\x12\x13\n\x0bworking_dir\x18\x0c \x01(\t\x12\x12\n\ndockerfile\x18\r \x01(\t\x12\x15\n\rmemory_volume\x18\x0e \x01(\x08\x1a*\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x17\n\x05TFJob\x12\x0e\n\x06tf_job\x18\x01 \x01(\t\"\x89\x01\n\x06\x45gress\x12\x0b\n\x03URL\x18\x01 \x01(\t\x12\x35\n\x0eobject_storage\x18\x02 \x01(\x0b\x32\x1b.pfs_v2.ObjectStorageEgressH\x00\x12\x31\n\x0csql_database\x18\x03 \x01(\x0b\x32\x19.pfs_v2.SQLDatabaseEgressH\x00\x42\x08\n\x06target\"5\n\x03Job\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\x12\n\n\x02id\x18\x02 \x01(\t\"\xd3\x01\n\x08Metadata\x12\x36\n\x0b\x61nnotations\x18\x01 \x03(\x0b\x32!.pps_v2.Metadata.AnnotationsEntry\x12,\n\x06labels\x18\x02 \x03(\x0b\x32\x1c.pps_v2.Metadata.LabelsEntry\x1a\x32\n\x10\x41nnotationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"Q\n\x07Service\x12\x15\n\rinternal_port\x18\x01 \x01(\x05\x12\x15\n\rexternal_port\x18\x02 \x01(\x05\x12\n\n\x02ip\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\t\")\n\x05Spout\x12 \n\x07service\x18\x01 \x01(\x0b\x32\x0f.pps_v2.Service\"\x80\x02\n\x08PFSInput\x12\x0f\n\x07project\x18\x0e \x01(\t\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04repo\x18\x02 \x01(\t\x12\x11\n\trepo_type\x18\r \x01(\t\x12\x0e\n\x06\x62ranch\x18\x03 \x01(\t\x12\x0e\n\x06\x63ommit\x18\x04 \x01(\t\x12\x0c\n\x04glob\x18\x05 \x01(\t\x12\x0f\n\x07join_on\x18\x06 \x01(\t\x12\x12\n\nouter_join\x18\x07 \x01(\x08\x12\x10\n\x08group_by\x18\x08 \x01(\t\x12\x0c\n\x04lazy\x18\t \x01(\x08\x12\x13\n\x0b\x65mpty_files\x18\n \x01(\x08\x12\n\n\x02s3\x18\x0b \x01(\x08\x12 \n\x07trigger\x18\x0c \x01(\x0b\x32\x0f.pfs_v2.Trigger\"\x94\x01\n\tCronInput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07project\x18\x07 \x01(\t\x12\x0c\n\x04repo\x18\x02 \x01(\t\x12\x0e\n\x06\x63ommit\x18\x03 \x01(\t\x12\x0c\n\x04spec\x18\x04 \x01(\t\x12\x11\n\toverwrite\x18\x05 \x01(\x08\x12)\n\x05start\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xbe\x01\n\x05Input\x12\x1d\n\x03pfs\x18\x01 \x01(\x0b\x32\x10.pps_v2.PFSInput\x12\x1b\n\x04join\x18\x02 \x03(\x0b\x32\r.pps_v2.Input\x12\x1c\n\x05group\x18\x03 \x03(\x0b\x32\r.pps_v2.Input\x12\x1c\n\x05\x63ross\x18\x04 \x03(\x0b\x32\r.pps_v2.Input\x12\x1c\n\x05union\x18\x05 \x03(\x0b\x32\r.pps_v2.Input\x12\x1f\n\x04\x63ron\x18\x06 \x01(\x0b\x32\x11.pps_v2.CronInput\"T\n\x08JobInput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\x06\x63ommit\x18\x02 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x0c\n\x04glob\x18\x03 \x01(\t\x12\x0c\n\x04lazy\x18\x04 \x01(\x08\"#\n\x0fParallelismSpec\x12\x10\n\x08\x63onstant\x18\x01 \x01(\x04\"\'\n\tInputFile\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0c\n\x04hash\x18\x02 \x01(\x0c\"-\n\x05\x44\x61tum\x12\x18\n\x03job\x18\x01 \x01(\x0b\x32\x0b.pps_v2.Job\x12\n\n\x02id\x18\x02 \x01(\t\"\xc4\x01\n\tDatumInfo\x12\x1c\n\x05\x64\x61tum\x18\x01 \x01(\x0b\x32\r.pps_v2.Datum\x12!\n\x05state\x18\x02 \x01(\x0e\x32\x12.pps_v2.DatumState\x12#\n\x05stats\x18\x03 \x01(\x0b\x32\x14.pps_v2.ProcessStats\x12\x1f\n\tpfs_state\x18\x04 \x01(\x0b\x32\x0c.pfs_v2.File\x12\x1e\n\x04\x64\x61ta\x18\x05 \x03(\x0b\x32\x10.pfs_v2.FileInfo\x12\x10\n\x08image_id\x18\x06 \x01(\t\"s\n\tAggregate\x12\r\n\x05\x63ount\x18\x01 \x01(\x03\x12\x0c\n\x04mean\x18\x02 \x01(\x01\x12\x0e\n\x06stddev\x18\x03 \x01(\x01\x12\x18\n\x10\x66ifth_percentile\x18\x04 \x01(\x01\x12\x1f\n\x17ninety_fifth_percentile\x18\x05 \x01(\x01\"\xcf\x01\n\x0cProcessStats\x12\x30\n\rdownload_time\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12/\n\x0cprocess_time\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12.\n\x0bupload_time\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x16\n\x0e\x64ownload_bytes\x18\x04 \x01(\x03\x12\x14\n\x0cupload_bytes\x18\x05 \x01(\x03\"\xe6\x01\n\x15\x41ggregateProcessStats\x12(\n\rdownload_time\x18\x01 \x01(\x0b\x32\x11.pps_v2.Aggregate\x12\'\n\x0cprocess_time\x18\x02 \x01(\x0b\x32\x11.pps_v2.Aggregate\x12&\n\x0bupload_time\x18\x03 \x01(\x0b\x32\x11.pps_v2.Aggregate\x12)\n\x0e\x64ownload_bytes\x18\x04 \x01(\x0b\x32\x11.pps_v2.Aggregate\x12\'\n\x0cupload_bytes\x18\x05 \x01(\x0b\x32\x11.pps_v2.Aggregate\"\\\n\x0cWorkerStatus\x12\x11\n\tworker_id\x18\x01 \x01(\t\x12\x0e\n\x06job_id\x18\x02 \x01(\t\x12)\n\x0c\x64\x61tum_status\x18\x03 \x01(\x0b\x32\x13.pps_v2.DatumStatus\"[\n\x0b\x44\x61tumStatus\x12+\n\x07started\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1f\n\x04\x64\x61ta\x18\x02 \x03(\x0b\x32\x11.pps_v2.InputFile\"W\n\x0cResourceSpec\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x02\x12\x0e\n\x06memory\x18\x02 \x01(\t\x12\x1c\n\x03gpu\x18\x03 \x01(\x0b\x32\x0f.pps_v2.GPUSpec\x12\x0c\n\x04\x64isk\x18\x04 \x01(\t\"\'\n\x07GPUSpec\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06number\x18\x02 \x01(\x03\"L\n\nJobSetInfo\x12\x1f\n\x07job_set\x18\x01 \x01(\x0b\x32\x0e.pps_v2.JobSet\x12\x1d\n\x04jobs\x18\x02 \x03(\x0b\x32\x0f.pps_v2.JobInfo\"\x9c\t\n\x07JobInfo\x12\x18\n\x03job\x18\x01 \x01(\x0b\x32\x0b.pps_v2.Job\x12\x18\n\x10pipeline_version\x18\x02 \x01(\x04\x12%\n\routput_commit\x18\x03 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x0f\n\x07restart\x18\x04 \x01(\x04\x12\x16\n\x0e\x64\x61ta_processed\x18\x05 \x01(\x03\x12\x14\n\x0c\x64\x61ta_skipped\x18\x06 \x01(\x03\x12\x12\n\ndata_total\x18\x07 \x01(\x03\x12\x13\n\x0b\x64\x61ta_failed\x18\x08 \x01(\x03\x12\x16\n\x0e\x64\x61ta_recovered\x18\t \x01(\x03\x12#\n\x05stats\x18\n \x01(\x0b\x32\x14.pps_v2.ProcessStats\x12\x1f\n\x05state\x18\x0b \x01(\x0e\x32\x10.pps_v2.JobState\x12\x0e\n\x06reason\x18\x0c \x01(\t\x12+\n\x07\x63reated\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x07started\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x66inished\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x07\x64\x65tails\x18\x10 \x01(\x0b\x32\x17.pps_v2.JobInfo.Details\x1a\xad\x05\n\x07\x44\x65tails\x12$\n\ttransform\x18\x01 \x01(\x0b\x32\x11.pps_v2.Transform\x12\x31\n\x10parallelism_spec\x18\x02 \x01(\x0b\x32\x17.pps_v2.ParallelismSpec\x12\x1e\n\x06\x65gress\x18\x03 \x01(\x0b\x32\x0e.pps_v2.Egress\x12 \n\x07service\x18\x04 \x01(\x0b\x32\x0f.pps_v2.Service\x12\x1c\n\x05spout\x18\x05 \x01(\x0b\x32\r.pps_v2.Spout\x12+\n\rworker_status\x18\x06 \x03(\x0b\x32\x14.pps_v2.WorkerStatus\x12/\n\x11resource_requests\x18\x07 \x01(\x0b\x32\x14.pps_v2.ResourceSpec\x12-\n\x0fresource_limits\x18\x08 \x01(\x0b\x32\x14.pps_v2.ResourceSpec\x12\x35\n\x17sidecar_resource_limits\x18\t \x01(\x0b\x32\x14.pps_v2.ResourceSpec\x12\x1c\n\x05input\x18\n \x01(\x0b\x32\r.pps_v2.Input\x12\x0c\n\x04salt\x18\x0b \x01(\t\x12,\n\x0e\x64\x61tum_set_spec\x18\x0c \x01(\x0b\x32\x14.pps_v2.DatumSetSpec\x12\x30\n\rdatum_timeout\x18\r \x01(\x0b\x32\x19.google.protobuf.Duration\x12.\n\x0bjob_timeout\x18\x0e \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x13\n\x0b\x64\x61tum_tries\x18\x0f \x01(\x03\x12/\n\x0fscheduling_spec\x18\x10 \x01(\x0b\x32\x16.pps_v2.SchedulingSpec\x12\x10\n\x08pod_spec\x18\x11 \x01(\t\x12\x11\n\tpod_patch\x18\x12 \x01(\t\":\n\x06Worker\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\"\n\x05state\x18\x02 \x01(\x0e\x32\x13.pps_v2.WorkerState\":\n\x08Pipeline\x12 \n\x07project\x18\x02 \x01(\x0b\x32\x0f.pfs_v2.Project\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xb4\x01\n\nToleration\x12\x0b\n\x03key\x18\x01 \x01(\t\x12,\n\x08operator\x18\x02 \x01(\x0e\x32\x1a.pps_v2.TolerationOperator\x12\r\n\x05value\x18\x03 \x01(\t\x12#\n\x06\x65\x66\x66\x65\x63t\x18\x04 \x01(\x0e\x32\x13.pps_v2.TaintEffect\x12\x37\n\x12toleration_seconds\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int64Value\"\xf4\x0b\n\x0cPipelineInfo\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\x12\x0f\n\x07version\x18\x02 \x01(\x04\x12#\n\x0bspec_commit\x18\x03 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x0f\n\x07stopped\x18\x04 \x01(\x08\x12$\n\x05state\x18\x05 \x01(\x0e\x32\x15.pps_v2.PipelineState\x12\x0e\n\x06reason\x18\x06 \x01(\t\x12(\n\x0elast_job_state\x18\x08 \x01(\x0e\x32\x10.pps_v2.JobState\x12\x13\n\x0bparallelism\x18\t \x01(\x04\x12/\n\x04type\x18\n \x01(\x0e\x32!.pps_v2.PipelineInfo.PipelineType\x12\x12\n\nauth_token\x18\x0b \x01(\t\x12-\n\x07\x64\x65tails\x18\x0c \x01(\x0b\x32\x1c.pps_v2.PipelineInfo.Details\x1a\x8d\x08\n\x07\x44\x65tails\x12$\n\ttransform\x18\x01 \x01(\x0b\x32\x11.pps_v2.Transform\x12\x1d\n\x06tf_job\x18\x02 \x01(\x0b\x32\r.pps_v2.TFJob\x12\x31\n\x10parallelism_spec\x18\x03 \x01(\x0b\x32\x17.pps_v2.ParallelismSpec\x12\x1e\n\x06\x65gress\x18\x04 \x01(\x0b\x32\x0e.pps_v2.Egress\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0crecent_error\x18\x06 \x01(\t\x12\x19\n\x11workers_requested\x18\x07 \x01(\x03\x12\x19\n\x11workers_available\x18\x08 \x01(\x03\x12\x15\n\routput_branch\x18\t \x01(\t\x12/\n\x11resource_requests\x18\n \x01(\x0b\x32\x14.pps_v2.ResourceSpec\x12-\n\x0fresource_limits\x18\x0b \x01(\x0b\x32\x14.pps_v2.ResourceSpec\x12\x35\n\x17sidecar_resource_limits\x18\x0c \x01(\x0b\x32\x14.pps_v2.ResourceSpec\x12\x1c\n\x05input\x18\r \x01(\x0b\x32\r.pps_v2.Input\x12\x13\n\x0b\x64\x65scription\x18\x0e \x01(\t\x12\x0c\n\x04salt\x18\x10 \x01(\t\x12\x0e\n\x06reason\x18\x11 \x01(\t\x12 \n\x07service\x18\x13 \x01(\x0b\x32\x0f.pps_v2.Service\x12\x1c\n\x05spout\x18\x14 \x01(\x0b\x32\r.pps_v2.Spout\x12,\n\x0e\x64\x61tum_set_spec\x18\x15 \x01(\x0b\x32\x14.pps_v2.DatumSetSpec\x12\x30\n\rdatum_timeout\x18\x16 \x01(\x0b\x32\x19.google.protobuf.Duration\x12.\n\x0bjob_timeout\x18\x17 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x13\n\x0b\x64\x61tum_tries\x18\x18 \x01(\x03\x12/\n\x0fscheduling_spec\x18\x19 \x01(\x0b\x32\x16.pps_v2.SchedulingSpec\x12\x10\n\x08pod_spec\x18\x1a \x01(\t\x12\x11\n\tpod_patch\x18\x1b \x01(\t\x12\x0e\n\x06s3_out\x18\x1c \x01(\x08\x12\"\n\x08metadata\x18\x1d \x01(\x0b\x32\x10.pps_v2.Metadata\x12\x16\n\x0ereprocess_spec\x18\x1e \x01(\t\x12\x17\n\x0funclaimed_tasks\x18\x1f \x01(\x03\x12\x11\n\tworker_rc\x18  \x01(\t\x12\x13\n\x0b\x61utoscaling\x18! \x01(\x08\x12\'\n\x0btolerations\x18\" \x03(\x0b\x32\x12.pps_v2.Toleration\"z\n\x0cPipelineType\x12\x19\n\x15PIPELINT_TYPE_UNKNOWN\x10\x00\x12\x1b\n\x17PIPELINE_TYPE_TRANSFORM\x10\x01\x12\x17\n\x13PIPELINE_TYPE_SPOUT\x10\x02\x12\x19\n\x15PIPELINE_TYPE_SERVICE\x10\x03J\x04\x08\x07\x10\x08\"<\n\rPipelineInfos\x12+\n\rpipeline_info\x18\x01 \x03(\x0b\x32\x14.pps_v2.PipelineInfo\"\x14\n\x06JobSet\x12\n\n\x02id\x18\x01 \x01(\t\"V\n\x14InspectJobSetRequest\x12\x1f\n\x07job_set\x18\x01 \x01(\x0b\x32\x0e.pps_v2.JobSet\x12\x0c\n\x04wait\x18\x02 \x01(\x08\x12\x0f\n\x07\x64\x65tails\x18\x03 \x01(\x08\"\x9e\x01\n\x11ListJobSetRequest\x12\x0f\n\x07\x64\x65tails\x18\x01 \x01(\x08\x12!\n\x08projects\x18\x02 \x03(\x0b\x32\x0f.pfs_v2.Project\x12\x34\n\x10paginationMarker\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06number\x18\x04 \x01(\x03\x12\x0f\n\x07reverse\x18\x05 \x01(\x08\"L\n\x11InspectJobRequest\x12\x18\n\x03job\x18\x01 \x01(\x0b\x32\x0b.pps_v2.Job\x12\x0c\n\x04wait\x18\x02 \x01(\x08\x12\x0f\n\x07\x64\x65tails\x18\x03 \x01(\x08\"\x88\x02\n\x0eListJobRequest\x12!\n\x08projects\x18\x07 \x03(\x0b\x32\x0f.pfs_v2.Project\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\x12$\n\x0cinput_commit\x18\x02 \x03(\x0b\x32\x0e.pfs_v2.Commit\x12\x0f\n\x07history\x18\x04 \x01(\x03\x12\x0f\n\x07\x64\x65tails\x18\x05 \x01(\x08\x12\x10\n\x08jqFilter\x18\x06 \x01(\t\x12\x34\n\x10paginationMarker\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06number\x18\t \x01(\x03\x12\x0f\n\x07reverse\x18\n \x01(\x08\"J\n\x13SubscribeJobRequest\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\x08\",\n\x10\x44\x65leteJobRequest\x12\x18\n\x03job\x18\x01 \x01(\x0b\x32\x0b.pps_v2.Job\":\n\x0eStopJobRequest\x12\x18\n\x03job\x18\x01 \x01(\x0b\x32\x0b.pps_v2.Job\x12\x0e\n\x06reason\x18\x03 \x01(\t\"\x87\x02\n\x15UpdateJobStateRequest\x12\x18\n\x03job\x18\x01 \x01(\x0b\x32\x0b.pps_v2.Job\x12\x1f\n\x05state\x18\x02 \x01(\x0e\x32\x10.pps_v2.JobState\x12\x0e\n\x06reason\x18\x03 \x01(\t\x12\x0f\n\x07restart\x18\x05 \x01(\x04\x12\x16\n\x0e\x64\x61ta_processed\x18\x06 \x01(\x03\x12\x14\n\x0c\x64\x61ta_skipped\x18\x07 \x01(\x03\x12\x13\n\x0b\x64\x61ta_failed\x18\x08 \x01(\x03\x12\x16\n\x0e\x64\x61ta_recovered\x18\t \x01(\x03\x12\x12\n\ndata_total\x18\n \x01(\x03\x12#\n\x05stats\x18\x0b \x01(\x0b\x32\x14.pps_v2.ProcessStats\"\xf4\x01\n\x0eGetLogsRequest\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\x12\x18\n\x03job\x18\x02 \x01(\x0b\x32\x0b.pps_v2.Job\x12\x14\n\x0c\x64\x61ta_filters\x18\x03 \x03(\t\x12\x1c\n\x05\x64\x61tum\x18\x04 \x01(\x0b\x32\r.pps_v2.Datum\x12\x0e\n\x06master\x18\x05 \x01(\x08\x12\x0e\n\x06\x66ollow\x18\x06 \x01(\x08\x12\x0c\n\x04tail\x18\x07 \x01(\x03\x12\x18\n\x10use_loki_backend\x18\x08 \x01(\x08\x12(\n\x05since\x18\t \x01(\x0b\x32\x19.google.protobuf.Duration\"\xe6\x01\n\nLogMessage\x12\x14\n\x0cproject_name\x18\n \x01(\t\x12\x15\n\rpipeline_name\x18\x01 \x01(\t\x12\x0e\n\x06job_id\x18\x02 \x01(\t\x12\x11\n\tworker_id\x18\x03 \x01(\t\x12\x10\n\x08\x64\x61tum_id\x18\x04 \x01(\t\x12\x0e\n\x06master\x18\x05 \x01(\x08\x12\x1f\n\x04\x64\x61ta\x18\x06 \x03(\x0b\x32\x11.pps_v2.InputFile\x12\x0c\n\x04user\x18\x07 \x01(\x08\x12&\n\x02ts\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07message\x18\t \x01(\t\"E\n\x13RestartDatumRequest\x12\x18\n\x03job\x18\x01 \x01(\x0b\x32\x0b.pps_v2.Job\x12\x14\n\x0c\x64\x61ta_filters\x18\x02 \x03(\t\"3\n\x13InspectDatumRequest\x12\x1c\n\x05\x64\x61tum\x18\x01 \x01(\x0b\x32\r.pps_v2.Datum\"\xe3\x01\n\x10ListDatumRequest\x12\x18\n\x03job\x18\x01 \x01(\x0b\x32\x0b.pps_v2.Job\x12\x1c\n\x05input\x18\x02 \x01(\x0b\x32\r.pps_v2.Input\x12/\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x1f.pps_v2.ListDatumRequest.Filter\x12\x18\n\x10paginationMarker\x18\x04 \x01(\t\x12\x0e\n\x06number\x18\x05 \x01(\x03\x12\x0f\n\x07reverse\x18\x06 \x01(\x08\x1a+\n\x06\x46ilter\x12!\n\x05state\x18\x01 \x03(\x0e\x32\x12.pps_v2.DatumState\"F\n\x0c\x44\x61tumSetSpec\x12\x0e\n\x06number\x18\x01 \x01(\x03\x12\x12\n\nsize_bytes\x18\x02 \x01(\x03\x12\x12\n\nper_worker\x18\x03 \x01(\x03\"\xa3\x01\n\x0eSchedulingSpec\x12?\n\rnode_selector\x18\x01 \x03(\x0b\x32(.pps_v2.SchedulingSpec.NodeSelectorEntry\x12\x1b\n\x13priority_class_name\x18\x02 \x01(\t\x1a\x33\n\x11NodeSelectorEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xcf\x07\n\x15\x43reatePipelineRequest\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\x12\x1d\n\x06tf_job\x18\x02 \x01(\x0b\x32\r.pps_v2.TFJob\x12$\n\ttransform\x18\x03 \x01(\x0b\x32\x11.pps_v2.Transform\x12\x31\n\x10parallelism_spec\x18\x04 \x01(\x0b\x32\x17.pps_v2.ParallelismSpec\x12\x1e\n\x06\x65gress\x18\x05 \x01(\x0b\x32\x0e.pps_v2.Egress\x12\x0e\n\x06update\x18\x06 \x01(\x08\x12\x15\n\routput_branch\x18\x07 \x01(\t\x12\x0e\n\x06s3_out\x18\x08 \x01(\x08\x12/\n\x11resource_requests\x18\t \x01(\x0b\x32\x14.pps_v2.ResourceSpec\x12-\n\x0fresource_limits\x18\n \x01(\x0b\x32\x14.pps_v2.ResourceSpec\x12\x35\n\x17sidecar_resource_limits\x18\x0b \x01(\x0b\x32\x14.pps_v2.ResourceSpec\x12\x1c\n\x05input\x18\x0c \x01(\x0b\x32\r.pps_v2.Input\x12\x13\n\x0b\x64\x65scription\x18\r \x01(\t\x12\x11\n\treprocess\x18\x0f \x01(\x08\x12 \n\x07service\x18\x11 \x01(\x0b\x32\x0f.pps_v2.Service\x12\x1c\n\x05spout\x18\x12 \x01(\x0b\x32\r.pps_v2.Spout\x12,\n\x0e\x64\x61tum_set_spec\x18\x13 \x01(\x0b\x32\x14.pps_v2.DatumSetSpec\x12\x30\n\rdatum_timeout\x18\x14 \x01(\x0b\x32\x19.google.protobuf.Duration\x12.\n\x0bjob_timeout\x18\x15 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x0c\n\x04salt\x18\x16 \x01(\t\x12\x13\n\x0b\x64\x61tum_tries\x18\x17 \x01(\x03\x12/\n\x0fscheduling_spec\x18\x18 \x01(\x0b\x32\x16.pps_v2.SchedulingSpec\x12\x10\n\x08pod_spec\x18\x19 \x01(\t\x12\x11\n\tpod_patch\x18\x1a \x01(\t\x12#\n\x0bspec_commit\x18\x1b \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\"\n\x08metadata\x18\x1c \x01(\x0b\x32\x10.pps_v2.Metadata\x12\x16\n\x0ereprocess_spec\x18\x1d \x01(\t\x12\x13\n\x0b\x61utoscaling\x18\x1e \x01(\x08\x12\'\n\x0btolerations\x18\" \x03(\x0b\x32\x12.pps_v2.Toleration\"M\n\x16InspectPipelineRequest\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\x08\"\xb7\x01\n\x13ListPipelineRequest\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\x12\x0f\n\x07history\x18\x02 \x01(\x03\x12\x0f\n\x07\x64\x65tails\x18\x03 \x01(\x08\x12\x10\n\x08jqFilter\x18\x04 \x01(\t\x12%\n\ncommit_set\x18\x05 \x01(\x0b\x32\x11.pfs_v2.CommitSet\x12!\n\x08projects\x18\x06 \x03(\x0b\x32\x0f.pfs_v2.Project\"n\n\x15\x44\x65letePipelineRequest\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\x12\x0f\n\x03\x61ll\x18\x02 \x01(\x08\x42\x02\x18\x01\x12\r\n\x05\x66orce\x18\x03 \x01(\x08\x12\x11\n\tkeep_repo\x18\x04 \x01(\x08\"j\n\x16\x44\x65letePipelinesRequest\x12!\n\x08projects\x18\x01 \x03(\x0b\x32\x0f.pfs_v2.Project\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12\x11\n\tkeep_repo\x18\x03 \x01(\x08\x12\x0b\n\x03\x61ll\x18\x04 \x01(\x08\">\n\x17\x44\x65letePipelinesResponse\x12#\n\tpipelines\x18\x01 \x03(\x0b\x32\x10.pps_v2.Pipeline\":\n\x14StartPipelineRequest\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\"9\n\x13StopPipelineRequest\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\"l\n\x12RunPipelineRequest\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\x12\"\n\nprovenance\x18\x02 \x03(\x0b\x32\x0e.pfs_v2.Commit\x12\x0e\n\x06job_id\x18\x03 \x01(\t\"4\n\x0eRunCronRequest\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\"#\n\x13\x43reateSecretRequest\x12\x0c\n\x04\x66ile\x18\x01 \x01(\x0c\"5\n\x13\x44\x65leteSecretRequest\x12\x1e\n\x06secret\x18\x01 \x01(\x0b\x32\x0e.pps_v2.Secret\"6\n\x14InspectSecretRequest\x12\x1e\n\x06secret\x18\x01 \x01(\x0b\x32\x0e.pps_v2.Secret\"\x16\n\x06Secret\x12\x0c\n\x04name\x18\x01 \x01(\t\"r\n\nSecretInfo\x12\x1e\n\x06secret\x18\x01 \x01(\x0b\x32\x0e.pps_v2.Secret\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x36\n\x12\x63reation_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"6\n\x0bSecretInfos\x12\'\n\x0bsecret_info\x18\x01 \x03(\x0b\x32\x12.pps_v2.SecretInfo\"\x15\n\x13\x41\x63tivateAuthRequest\"\x16\n\x14\x41\x63tivateAuthResponse\"\x81\x01\n\x12RunLoadTestRequest\x12\x10\n\x08\x64\x61g_spec\x18\x01 \x01(\t\x12\x11\n\tload_spec\x18\x02 \x01(\t\x12\x0c\n\x04seed\x18\x03 \x01(\x03\x12\x13\n\x0bparallelism\x18\x04 \x01(\x03\x12\x11\n\tpod_patch\x18\x05 \x01(\t\x12\x10\n\x08state_id\x18\x06 \x01(\t\"6\n\x13RunLoadTestResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x10\n\x08state_id\x18\x02 \x01(\t\"\x8d\x01\n\x15RenderTemplateRequest\x12\x10\n\x08template\x18\x01 \x01(\t\x12\x35\n\x04\x61rgs\x18\x02 \x03(\x0b\x32\'.pps_v2.RenderTemplateRequest.ArgsEntry\x1a+\n\tArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"T\n\x16RenderTemplateResponse\x12\x0c\n\x04json\x18\x01 \x01(\t\x12,\n\x05specs\x18\x02 \x03(\x0b\x32\x1d.pps_v2.CreatePipelineRequest*\xc1\x01\n\x08JobState\x12\x15\n\x11JOB_STATE_UNKNOWN\x10\x00\x12\x0f\n\x0bJOB_CREATED\x10\x01\x12\x10\n\x0cJOB_STARTING\x10\x02\x12\x0f\n\x0bJOB_RUNNING\x10\x03\x12\x0f\n\x0bJOB_FAILURE\x10\x04\x12\x0f\n\x0bJOB_SUCCESS\x10\x05\x12\x0e\n\nJOB_KILLED\x10\x06\x12\x11\n\rJOB_EGRESSING\x10\x07\x12\x11\n\rJOB_FINISHING\x10\x08\x12\x12\n\x0eJOB_UNRUNNABLE\x10\t*\\\n\nDatumState\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06\x46\x41ILED\x10\x01\x12\x0b\n\x07SUCCESS\x10\x02\x12\x0b\n\x07SKIPPED\x10\x03\x12\x0c\n\x08STARTING\x10\x04\x12\r\n\tRECOVERED\x10\x05*Y\n\x0bWorkerState\x12\x18\n\x14WORKER_STATE_UNKNOWN\x10\x00\x12\x0f\n\x0bPOD_RUNNING\x10\x01\x12\x0f\n\x0bPOD_SUCCESS\x10\x02\x12\x0e\n\nPOD_FAILED\x10\x03*\xc9\x01\n\rPipelineState\x12\x1a\n\x16PIPELINE_STATE_UNKNOWN\x10\x00\x12\x15\n\x11PIPELINE_STARTING\x10\x01\x12\x14\n\x10PIPELINE_RUNNING\x10\x02\x12\x17\n\x13PIPELINE_RESTARTING\x10\x03\x12\x14\n\x10PIPELINE_FAILURE\x10\x04\x12\x13\n\x0fPIPELINE_PAUSED\x10\x05\x12\x14\n\x10PIPELINE_STANDBY\x10\x06\x12\x15\n\x11PIPELINE_CRASHING\x10\x07*6\n\x12TolerationOperator\x12\t\n\x05\x45MPTY\x10\x00\x12\n\n\x06\x45XISTS\x10\x01\x12\t\n\x05\x45QUAL\x10\x02*W\n\x0bTaintEffect\x12\x0f\n\x0b\x41LL_EFFECTS\x10\x00\x12\x0f\n\x0bNO_SCHEDULE\x10\x01\x12\x16\n\x12PREFER_NO_SCHEDULE\x10\x02\x12\x0e\n\nNO_EXECUTE\x10\x03\x32\xde\x10\n\x03\x41PI\x12:\n\nInspectJob\x12\x19.pps_v2.InspectJobRequest\x1a\x0f.pps_v2.JobInfo\"\x00\x12\x42\n\rInspectJobSet\x12\x1c.pps_v2.InspectJobSetRequest\x1a\x0f.pps_v2.JobInfo\"\x00\x30\x01\x12\x36\n\x07ListJob\x12\x16.pps_v2.ListJobRequest\x1a\x0f.pps_v2.JobInfo\"\x00\x30\x01\x12?\n\nListJobSet\x12\x19.pps_v2.ListJobSetRequest\x1a\x12.pps_v2.JobSetInfo\"\x00\x30\x01\x12@\n\x0cSubscribeJob\x12\x1b.pps_v2.SubscribeJobRequest\x1a\x0f.pps_v2.JobInfo\"\x00\x30\x01\x12?\n\tDeleteJob\x12\x18.pps_v2.DeleteJobRequest\x1a\x16.google.protobuf.Empty\"\x00\x12;\n\x07StopJob\x12\x16.pps_v2.StopJobRequest\x1a\x16.google.protobuf.Empty\"\x00\x12@\n\x0cInspectDatum\x12\x1b.pps_v2.InspectDatumRequest\x1a\x11.pps_v2.DatumInfo\"\x00\x12<\n\tListDatum\x12\x18.pps_v2.ListDatumRequest\x1a\x11.pps_v2.DatumInfo\"\x00\x30\x01\x12\x45\n\x0cRestartDatum\x12\x1b.pps_v2.RestartDatumRequest\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\x0e\x43reatePipeline\x12\x1d.pps_v2.CreatePipelineRequest\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\x0fInspectPipeline\x12\x1e.pps_v2.InspectPipelineRequest\x1a\x14.pps_v2.PipelineInfo\"\x00\x12\x45\n\x0cListPipeline\x12\x1b.pps_v2.ListPipelineRequest\x1a\x14.pps_v2.PipelineInfo\"\x00\x30\x01\x12I\n\x0e\x44\x65letePipeline\x12\x1d.pps_v2.DeletePipelineRequest\x1a\x16.google.protobuf.Empty\"\x00\x12T\n\x0f\x44\x65letePipelines\x12\x1e.pps_v2.DeletePipelinesRequest\x1a\x1f.pps_v2.DeletePipelinesResponse\"\x00\x12G\n\rStartPipeline\x12\x1c.pps_v2.StartPipelineRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x45\n\x0cStopPipeline\x12\x1b.pps_v2.StopPipelineRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x43\n\x0bRunPipeline\x12\x1a.pps_v2.RunPipelineRequest\x1a\x16.google.protobuf.Empty\"\x00\x12;\n\x07RunCron\x12\x16.pps_v2.RunCronRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x45\n\x0c\x43reateSecret\x12\x1b.pps_v2.CreateSecretRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x45\n\x0c\x44\x65leteSecret\x12\x1b.pps_v2.DeleteSecretRequest\x1a\x16.google.protobuf.Empty\"\x00\x12;\n\nListSecret\x12\x16.google.protobuf.Empty\x1a\x13.pps_v2.SecretInfos\"\x00\x12\x43\n\rInspectSecret\x12\x1c.pps_v2.InspectSecretRequest\x1a\x12.pps_v2.SecretInfo\"\x00\x12=\n\tDeleteAll\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12\x39\n\x07GetLogs\x12\x16.pps_v2.GetLogsRequest\x1a\x12.pps_v2.LogMessage\"\x00\x30\x01\x12K\n\x0c\x41\x63tivateAuth\x12\x1b.pps_v2.ActivateAuthRequest\x1a\x1c.pps_v2.ActivateAuthResponse\"\x00\x12I\n\x0eUpdateJobState\x12\x1d.pps_v2.UpdateJobStateRequest\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x0bRunLoadTest\x12\x1a.pps_v2.RunLoadTestRequest\x1a\x1b.pps_v2.RunLoadTestResponse\"\x00\x12K\n\x12RunLoadTestDefault\x12\x16.google.protobuf.Empty\x1a\x1b.pps_v2.RunLoadTestResponse\"\x00\x12Q\n\x0eRenderTemplate\x12\x1d.pps_v2.RenderTemplateRequest\x1a\x1e.pps_v2.RenderTemplateResponse\"\x00\x12;\n\x08ListTask\x12\x18.taskapi.ListTaskRequest\x1a\x11.taskapi.TaskInfo\"\x00\x30\x01\x42+Z)github.com/pachyderm/pachyderm/v2/src/ppsb\x06proto3'
+  serialized_pb=b'\n\'python_pachyderm/proto/v2/pps/pps.proto\x12\x06pps_v2\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\'python_pachyderm/proto/v2/pfs/pfs.proto\x1a)python_pachyderm/proto/v2/task/task.proto\"M\n\x0bSecretMount\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\x12\n\nmount_path\x18\x03 \x01(\t\x12\x0f\n\x07\x65nv_var\x18\x04 \x01(\t\"\x82\x03\n\tTransform\x12\r\n\x05image\x18\x01 \x01(\t\x12\x0b\n\x03\x63md\x18\x02 \x03(\t\x12\x0f\n\x07\x65rr_cmd\x18\x03 \x03(\t\x12\'\n\x03\x65nv\x18\x04 \x03(\x0b\x32\x1a.pps_v2.Transform.EnvEntry\x12$\n\x07secrets\x18\x05 \x03(\x0b\x32\x13.pps_v2.SecretMount\x12\x1a\n\x12image_pull_secrets\x18\x06 \x03(\t\x12\r\n\x05stdin\x18\x07 \x03(\t\x12\x11\n\terr_stdin\x18\x08 \x03(\t\x12\x1a\n\x12\x61\x63\x63\x65pt_return_code\x18\t \x03(\x03\x12\r\n\x05\x64\x65\x62ug\x18\n \x01(\x08\x12\x0c\n\x04user\x18\x0b \x01(\t\x12\x13\n\x0bworking_dir\x18\x0c \x01(\t\x12\x12\n\ndockerfile\x18\r \x01(\t\x12\x15\n\rmemory_volume\x18\x0e \x01(\x08\x12\x16\n\x0e\x64\x61tum_batching\x18\x0f \x01(\x08\x1a*\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x17\n\x05TFJob\x12\x0e\n\x06tf_job\x18\x01 \x01(\t\"\x89\x01\n\x06\x45gress\x12\x0b\n\x03URL\x18\x01 \x01(\t\x12\x35\n\x0eobject_storage\x18\x02 \x01(\x0b\x32\x1b.pfs_v2.ObjectStorageEgressH\x00\x12\x31\n\x0csql_database\x18\x03 \x01(\x0b\x32\x19.pfs_v2.SQLDatabaseEgressH\x00\x42\x08\n\x06target\"5\n\x03Job\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\x12\n\n\x02id\x18\x02 \x01(\t\"\xd3\x01\n\x08Metadata\x12\x36\n\x0b\x61nnotations\x18\x01 \x03(\x0b\x32!.pps_v2.Metadata.AnnotationsEntry\x12,\n\x06labels\x18\x02 \x03(\x0b\x32\x1c.pps_v2.Metadata.LabelsEntry\x1a\x32\n\x10\x41nnotationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"Q\n\x07Service\x12\x15\n\rinternal_port\x18\x01 \x01(\x05\x12\x15\n\rexternal_port\x18\x02 \x01(\x05\x12\n\n\x02ip\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\t\")\n\x05Spout\x12 \n\x07service\x18\x01 \x01(\x0b\x32\x0f.pps_v2.Service\"\x80\x02\n\x08PFSInput\x12\x0f\n\x07project\x18\x0e \x01(\t\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04repo\x18\x02 \x01(\t\x12\x11\n\trepo_type\x18\r \x01(\t\x12\x0e\n\x06\x62ranch\x18\x03 \x01(\t\x12\x0e\n\x06\x63ommit\x18\x04 \x01(\t\x12\x0c\n\x04glob\x18\x05 \x01(\t\x12\x0f\n\x07join_on\x18\x06 \x01(\t\x12\x12\n\nouter_join\x18\x07 \x01(\x08\x12\x10\n\x08group_by\x18\x08 \x01(\t\x12\x0c\n\x04lazy\x18\t \x01(\x08\x12\x13\n\x0b\x65mpty_files\x18\n \x01(\x08\x12\n\n\x02s3\x18\x0b \x01(\x08\x12 \n\x07trigger\x18\x0c \x01(\x0b\x32\x0f.pfs_v2.Trigger\"\x94\x01\n\tCronInput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07project\x18\x07 \x01(\t\x12\x0c\n\x04repo\x18\x02 \x01(\t\x12\x0e\n\x06\x63ommit\x18\x03 \x01(\t\x12\x0c\n\x04spec\x18\x04 \x01(\t\x12\x11\n\toverwrite\x18\x05 \x01(\x08\x12)\n\x05start\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xbe\x01\n\x05Input\x12\x1d\n\x03pfs\x18\x01 \x01(\x0b\x32\x10.pps_v2.PFSInput\x12\x1b\n\x04join\x18\x02 \x03(\x0b\x32\r.pps_v2.Input\x12\x1c\n\x05group\x18\x03 \x03(\x0b\x32\r.pps_v2.Input\x12\x1c\n\x05\x63ross\x18\x04 \x03(\x0b\x32\r.pps_v2.Input\x12\x1c\n\x05union\x18\x05 \x03(\x0b\x32\r.pps_v2.Input\x12\x1f\n\x04\x63ron\x18\x06 \x01(\x0b\x32\x11.pps_v2.CronInput\"T\n\x08JobInput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\x06\x63ommit\x18\x02 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x0c\n\x04glob\x18\x03 \x01(\t\x12\x0c\n\x04lazy\x18\x04 \x01(\x08\"#\n\x0fParallelismSpec\x12\x10\n\x08\x63onstant\x18\x01 \x01(\x04\"\'\n\tInputFile\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0c\n\x04hash\x18\x02 \x01(\x0c\"-\n\x05\x44\x61tum\x12\x18\n\x03job\x18\x01 \x01(\x0b\x32\x0b.pps_v2.Job\x12\n\n\x02id\x18\x02 \x01(\t\"\xc4\x01\n\tDatumInfo\x12\x1c\n\x05\x64\x61tum\x18\x01 \x01(\x0b\x32\r.pps_v2.Datum\x12!\n\x05state\x18\x02 \x01(\x0e\x32\x12.pps_v2.DatumState\x12#\n\x05stats\x18\x03 \x01(\x0b\x32\x14.pps_v2.ProcessStats\x12\x1f\n\tpfs_state\x18\x04 \x01(\x0b\x32\x0c.pfs_v2.File\x12\x1e\n\x04\x64\x61ta\x18\x05 \x03(\x0b\x32\x10.pfs_v2.FileInfo\x12\x10\n\x08image_id\x18\x06 \x01(\t\"s\n\tAggregate\x12\r\n\x05\x63ount\x18\x01 \x01(\x03\x12\x0c\n\x04mean\x18\x02 \x01(\x01\x12\x0e\n\x06stddev\x18\x03 \x01(\x01\x12\x18\n\x10\x66ifth_percentile\x18\x04 \x01(\x01\x12\x1f\n\x17ninety_fifth_percentile\x18\x05 \x01(\x01\"\xcf\x01\n\x0cProcessStats\x12\x30\n\rdownload_time\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12/\n\x0cprocess_time\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12.\n\x0bupload_time\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x16\n\x0e\x64ownload_bytes\x18\x04 \x01(\x03\x12\x14\n\x0cupload_bytes\x18\x05 \x01(\x03\"\xe6\x01\n\x15\x41ggregateProcessStats\x12(\n\rdownload_time\x18\x01 \x01(\x0b\x32\x11.pps_v2.Aggregate\x12\'\n\x0cprocess_time\x18\x02 \x01(\x0b\x32\x11.pps_v2.Aggregate\x12&\n\x0bupload_time\x18\x03 \x01(\x0b\x32\x11.pps_v2.Aggregate\x12)\n\x0e\x64ownload_bytes\x18\x04 \x01(\x0b\x32\x11.pps_v2.Aggregate\x12\'\n\x0cupload_bytes\x18\x05 \x01(\x0b\x32\x11.pps_v2.Aggregate\"\\\n\x0cWorkerStatus\x12\x11\n\tworker_id\x18\x01 \x01(\t\x12\x0e\n\x06job_id\x18\x02 \x01(\t\x12)\n\x0c\x64\x61tum_status\x18\x03 \x01(\x0b\x32\x13.pps_v2.DatumStatus\"[\n\x0b\x44\x61tumStatus\x12+\n\x07started\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1f\n\x04\x64\x61ta\x18\x02 \x03(\x0b\x32\x11.pps_v2.InputFile\"W\n\x0cResourceSpec\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x02\x12\x0e\n\x06memory\x18\x02 \x01(\t\x12\x1c\n\x03gpu\x18\x03 \x01(\x0b\x32\x0f.pps_v2.GPUSpec\x12\x0c\n\x04\x64isk\x18\x04 \x01(\t\"\'\n\x07GPUSpec\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0e\n\x06number\x18\x02 \x01(\x03\"L\n\nJobSetInfo\x12\x1f\n\x07job_set\x18\x01 \x01(\x0b\x32\x0e.pps_v2.JobSet\x12\x1d\n\x04jobs\x18\x02 \x03(\x0b\x32\x0f.pps_v2.JobInfo\"\xd5\t\n\x07JobInfo\x12\x18\n\x03job\x18\x01 \x01(\x0b\x32\x0b.pps_v2.Job\x12\x18\n\x10pipeline_version\x18\x02 \x01(\x04\x12%\n\routput_commit\x18\x03 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x0f\n\x07restart\x18\x04 \x01(\x04\x12\x16\n\x0e\x64\x61ta_processed\x18\x05 \x01(\x03\x12\x14\n\x0c\x64\x61ta_skipped\x18\x06 \x01(\x03\x12\x12\n\ndata_total\x18\x07 \x01(\x03\x12\x13\n\x0b\x64\x61ta_failed\x18\x08 \x01(\x03\x12\x16\n\x0e\x64\x61ta_recovered\x18\t \x01(\x03\x12#\n\x05stats\x18\n \x01(\x0b\x32\x14.pps_v2.ProcessStats\x12\x1f\n\x05state\x18\x0b \x01(\x0e\x32\x10.pps_v2.JobState\x12\x0e\n\x06reason\x18\x0c \x01(\t\x12+\n\x07\x63reated\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x07started\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x66inished\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12(\n\x07\x64\x65tails\x18\x10 \x01(\x0b\x32\x17.pps_v2.JobInfo.Details\x1a\xe6\x05\n\x07\x44\x65tails\x12$\n\ttransform\x18\x01 \x01(\x0b\x32\x11.pps_v2.Transform\x12\x31\n\x10parallelism_spec\x18\x02 \x01(\x0b\x32\x17.pps_v2.ParallelismSpec\x12\x1e\n\x06\x65gress\x18\x03 \x01(\x0b\x32\x0e.pps_v2.Egress\x12 \n\x07service\x18\x04 \x01(\x0b\x32\x0f.pps_v2.Service\x12\x1c\n\x05spout\x18\x05 \x01(\x0b\x32\r.pps_v2.Spout\x12+\n\rworker_status\x18\x06 \x03(\x0b\x32\x14.pps_v2.WorkerStatus\x12/\n\x11resource_requests\x18\x07 \x01(\x0b\x32\x14.pps_v2.ResourceSpec\x12-\n\x0fresource_limits\x18\x08 \x01(\x0b\x32\x14.pps_v2.ResourceSpec\x12\x35\n\x17sidecar_resource_limits\x18\t \x01(\x0b\x32\x14.pps_v2.ResourceSpec\x12\x1c\n\x05input\x18\n \x01(\x0b\x32\r.pps_v2.Input\x12\x0c\n\x04salt\x18\x0b \x01(\t\x12,\n\x0e\x64\x61tum_set_spec\x18\x0c \x01(\x0b\x32\x14.pps_v2.DatumSetSpec\x12\x30\n\rdatum_timeout\x18\r \x01(\x0b\x32\x19.google.protobuf.Duration\x12.\n\x0bjob_timeout\x18\x0e \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x13\n\x0b\x64\x61tum_tries\x18\x0f \x01(\x03\x12/\n\x0fscheduling_spec\x18\x10 \x01(\x0b\x32\x16.pps_v2.SchedulingSpec\x12\x10\n\x08pod_spec\x18\x11 \x01(\t\x12\x11\n\tpod_patch\x18\x12 \x01(\t\x12\x37\n\x19sidecar_resource_requests\x18\x13 \x01(\x0b\x32\x14.pps_v2.ResourceSpec\":\n\x06Worker\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\"\n\x05state\x18\x02 \x01(\x0e\x32\x13.pps_v2.WorkerState\":\n\x08Pipeline\x12 \n\x07project\x18\x02 \x01(\x0b\x32\x0f.pfs_v2.Project\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xb4\x01\n\nToleration\x12\x0b\n\x03key\x18\x01 \x01(\t\x12,\n\x08operator\x18\x02 \x01(\x0e\x32\x1a.pps_v2.TolerationOperator\x12\r\n\x05value\x18\x03 \x01(\t\x12#\n\x06\x65\x66\x66\x65\x63t\x18\x04 \x01(\x0e\x32\x13.pps_v2.TaintEffect\x12\x37\n\x12toleration_seconds\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int64Value\"\xad\x0c\n\x0cPipelineInfo\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\x12\x0f\n\x07version\x18\x02 \x01(\x04\x12#\n\x0bspec_commit\x18\x03 \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\x0f\n\x07stopped\x18\x04 \x01(\x08\x12$\n\x05state\x18\x05 \x01(\x0e\x32\x15.pps_v2.PipelineState\x12\x0e\n\x06reason\x18\x06 \x01(\t\x12(\n\x0elast_job_state\x18\x08 \x01(\x0e\x32\x10.pps_v2.JobState\x12\x13\n\x0bparallelism\x18\t \x01(\x04\x12/\n\x04type\x18\n \x01(\x0e\x32!.pps_v2.PipelineInfo.PipelineType\x12\x12\n\nauth_token\x18\x0b \x01(\t\x12-\n\x07\x64\x65tails\x18\x0c \x01(\x0b\x32\x1c.pps_v2.PipelineInfo.Details\x1a\xc6\x08\n\x07\x44\x65tails\x12$\n\ttransform\x18\x01 \x01(\x0b\x32\x11.pps_v2.Transform\x12\x1d\n\x06tf_job\x18\x02 \x01(\x0b\x32\r.pps_v2.TFJob\x12\x31\n\x10parallelism_spec\x18\x03 \x01(\x0b\x32\x17.pps_v2.ParallelismSpec\x12\x1e\n\x06\x65gress\x18\x04 \x01(\x0b\x32\x0e.pps_v2.Egress\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0crecent_error\x18\x06 \x01(\t\x12\x19\n\x11workers_requested\x18\x07 \x01(\x03\x12\x19\n\x11workers_available\x18\x08 \x01(\x03\x12\x15\n\routput_branch\x18\t \x01(\t\x12/\n\x11resource_requests\x18\n \x01(\x0b\x32\x14.pps_v2.ResourceSpec\x12-\n\x0fresource_limits\x18\x0b \x01(\x0b\x32\x14.pps_v2.ResourceSpec\x12\x35\n\x17sidecar_resource_limits\x18\x0c \x01(\x0b\x32\x14.pps_v2.ResourceSpec\x12\x1c\n\x05input\x18\r \x01(\x0b\x32\r.pps_v2.Input\x12\x13\n\x0b\x64\x65scription\x18\x0e \x01(\t\x12\x0c\n\x04salt\x18\x10 \x01(\t\x12\x0e\n\x06reason\x18\x11 \x01(\t\x12 \n\x07service\x18\x13 \x01(\x0b\x32\x0f.pps_v2.Service\x12\x1c\n\x05spout\x18\x14 \x01(\x0b\x32\r.pps_v2.Spout\x12,\n\x0e\x64\x61tum_set_spec\x18\x15 \x01(\x0b\x32\x14.pps_v2.DatumSetSpec\x12\x30\n\rdatum_timeout\x18\x16 \x01(\x0b\x32\x19.google.protobuf.Duration\x12.\n\x0bjob_timeout\x18\x17 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x13\n\x0b\x64\x61tum_tries\x18\x18 \x01(\x03\x12/\n\x0fscheduling_spec\x18\x19 \x01(\x0b\x32\x16.pps_v2.SchedulingSpec\x12\x10\n\x08pod_spec\x18\x1a \x01(\t\x12\x11\n\tpod_patch\x18\x1b \x01(\t\x12\x0e\n\x06s3_out\x18\x1c \x01(\x08\x12\"\n\x08metadata\x18\x1d \x01(\x0b\x32\x10.pps_v2.Metadata\x12\x16\n\x0ereprocess_spec\x18\x1e \x01(\t\x12\x17\n\x0funclaimed_tasks\x18\x1f \x01(\x03\x12\x11\n\tworker_rc\x18  \x01(\t\x12\x13\n\x0b\x61utoscaling\x18! \x01(\x08\x12\'\n\x0btolerations\x18\" \x03(\x0b\x32\x12.pps_v2.Toleration\x12\x37\n\x19sidecar_resource_requests\x18# \x01(\x0b\x32\x14.pps_v2.ResourceSpec\"z\n\x0cPipelineType\x12\x19\n\x15PIPELINT_TYPE_UNKNOWN\x10\x00\x12\x1b\n\x17PIPELINE_TYPE_TRANSFORM\x10\x01\x12\x17\n\x13PIPELINE_TYPE_SPOUT\x10\x02\x12\x19\n\x15PIPELINE_TYPE_SERVICE\x10\x03J\x04\x08\x07\x10\x08\"<\n\rPipelineInfos\x12+\n\rpipeline_info\x18\x01 \x03(\x0b\x32\x14.pps_v2.PipelineInfo\"\x14\n\x06JobSet\x12\n\n\x02id\x18\x01 \x01(\t\"V\n\x14InspectJobSetRequest\x12\x1f\n\x07job_set\x18\x01 \x01(\x0b\x32\x0e.pps_v2.JobSet\x12\x0c\n\x04wait\x18\x02 \x01(\x08\x12\x0f\n\x07\x64\x65tails\x18\x03 \x01(\x08\"\x9e\x01\n\x11ListJobSetRequest\x12\x0f\n\x07\x64\x65tails\x18\x01 \x01(\x08\x12!\n\x08projects\x18\x02 \x03(\x0b\x32\x0f.pfs_v2.Project\x12\x34\n\x10paginationMarker\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06number\x18\x04 \x01(\x03\x12\x0f\n\x07reverse\x18\x05 \x01(\x08\"L\n\x11InspectJobRequest\x12\x18\n\x03job\x18\x01 \x01(\x0b\x32\x0b.pps_v2.Job\x12\x0c\n\x04wait\x18\x02 \x01(\x08\x12\x0f\n\x07\x64\x65tails\x18\x03 \x01(\x08\"\x88\x02\n\x0eListJobRequest\x12!\n\x08projects\x18\x07 \x03(\x0b\x32\x0f.pfs_v2.Project\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\x12$\n\x0cinput_commit\x18\x02 \x03(\x0b\x32\x0e.pfs_v2.Commit\x12\x0f\n\x07history\x18\x04 \x01(\x03\x12\x0f\n\x07\x64\x65tails\x18\x05 \x01(\x08\x12\x10\n\x08jqFilter\x18\x06 \x01(\t\x12\x34\n\x10paginationMarker\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06number\x18\t \x01(\x03\x12\x0f\n\x07reverse\x18\n \x01(\x08\"J\n\x13SubscribeJobRequest\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\x08\",\n\x10\x44\x65leteJobRequest\x12\x18\n\x03job\x18\x01 \x01(\x0b\x32\x0b.pps_v2.Job\":\n\x0eStopJobRequest\x12\x18\n\x03job\x18\x01 \x01(\x0b\x32\x0b.pps_v2.Job\x12\x0e\n\x06reason\x18\x03 \x01(\t\"\x87\x02\n\x15UpdateJobStateRequest\x12\x18\n\x03job\x18\x01 \x01(\x0b\x32\x0b.pps_v2.Job\x12\x1f\n\x05state\x18\x02 \x01(\x0e\x32\x10.pps_v2.JobState\x12\x0e\n\x06reason\x18\x03 \x01(\t\x12\x0f\n\x07restart\x18\x05 \x01(\x04\x12\x16\n\x0e\x64\x61ta_processed\x18\x06 \x01(\x03\x12\x14\n\x0c\x64\x61ta_skipped\x18\x07 \x01(\x03\x12\x13\n\x0b\x64\x61ta_failed\x18\x08 \x01(\x03\x12\x16\n\x0e\x64\x61ta_recovered\x18\t \x01(\x03\x12\x12\n\ndata_total\x18\n \x01(\x03\x12#\n\x05stats\x18\x0b \x01(\x0b\x32\x14.pps_v2.ProcessStats\"\xf4\x01\n\x0eGetLogsRequest\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\x12\x18\n\x03job\x18\x02 \x01(\x0b\x32\x0b.pps_v2.Job\x12\x14\n\x0c\x64\x61ta_filters\x18\x03 \x03(\t\x12\x1c\n\x05\x64\x61tum\x18\x04 \x01(\x0b\x32\r.pps_v2.Datum\x12\x0e\n\x06master\x18\x05 \x01(\x08\x12\x0e\n\x06\x66ollow\x18\x06 \x01(\x08\x12\x0c\n\x04tail\x18\x07 \x01(\x03\x12\x18\n\x10use_loki_backend\x18\x08 \x01(\x08\x12(\n\x05since\x18\t \x01(\x0b\x32\x19.google.protobuf.Duration\"\xe6\x01\n\nLogMessage\x12\x14\n\x0cproject_name\x18\n \x01(\t\x12\x15\n\rpipeline_name\x18\x01 \x01(\t\x12\x0e\n\x06job_id\x18\x02 \x01(\t\x12\x11\n\tworker_id\x18\x03 \x01(\t\x12\x10\n\x08\x64\x61tum_id\x18\x04 \x01(\t\x12\x0e\n\x06master\x18\x05 \x01(\x08\x12\x1f\n\x04\x64\x61ta\x18\x06 \x03(\x0b\x32\x11.pps_v2.InputFile\x12\x0c\n\x04user\x18\x07 \x01(\x08\x12&\n\x02ts\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07message\x18\t \x01(\t\"E\n\x13RestartDatumRequest\x12\x18\n\x03job\x18\x01 \x01(\x0b\x32\x0b.pps_v2.Job\x12\x14\n\x0c\x64\x61ta_filters\x18\x02 \x03(\t\"3\n\x13InspectDatumRequest\x12\x1c\n\x05\x64\x61tum\x18\x01 \x01(\x0b\x32\r.pps_v2.Datum\"\xe3\x01\n\x10ListDatumRequest\x12\x18\n\x03job\x18\x01 \x01(\x0b\x32\x0b.pps_v2.Job\x12\x1c\n\x05input\x18\x02 \x01(\x0b\x32\r.pps_v2.Input\x12/\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x1f.pps_v2.ListDatumRequest.Filter\x12\x18\n\x10paginationMarker\x18\x04 \x01(\t\x12\x0e\n\x06number\x18\x05 \x01(\x03\x12\x0f\n\x07reverse\x18\x06 \x01(\x08\x1a+\n\x06\x46ilter\x12!\n\x05state\x18\x01 \x03(\x0e\x32\x12.pps_v2.DatumState\"F\n\x0c\x44\x61tumSetSpec\x12\x0e\n\x06number\x18\x01 \x01(\x03\x12\x12\n\nsize_bytes\x18\x02 \x01(\x03\x12\x12\n\nper_worker\x18\x03 \x01(\x03\"\xa3\x01\n\x0eSchedulingSpec\x12?\n\rnode_selector\x18\x01 \x03(\x0b\x32(.pps_v2.SchedulingSpec.NodeSelectorEntry\x12\x1b\n\x13priority_class_name\x18\x02 \x01(\t\x1a\x33\n\x11NodeSelectorEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x88\x08\n\x15\x43reatePipelineRequest\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\x12\x1d\n\x06tf_job\x18\x02 \x01(\x0b\x32\r.pps_v2.TFJob\x12$\n\ttransform\x18\x03 \x01(\x0b\x32\x11.pps_v2.Transform\x12\x31\n\x10parallelism_spec\x18\x04 \x01(\x0b\x32\x17.pps_v2.ParallelismSpec\x12\x1e\n\x06\x65gress\x18\x05 \x01(\x0b\x32\x0e.pps_v2.Egress\x12\x0e\n\x06update\x18\x06 \x01(\x08\x12\x15\n\routput_branch\x18\x07 \x01(\t\x12\x0e\n\x06s3_out\x18\x08 \x01(\x08\x12/\n\x11resource_requests\x18\t \x01(\x0b\x32\x14.pps_v2.ResourceSpec\x12-\n\x0fresource_limits\x18\n \x01(\x0b\x32\x14.pps_v2.ResourceSpec\x12\x35\n\x17sidecar_resource_limits\x18\x0b \x01(\x0b\x32\x14.pps_v2.ResourceSpec\x12\x1c\n\x05input\x18\x0c \x01(\x0b\x32\r.pps_v2.Input\x12\x13\n\x0b\x64\x65scription\x18\r \x01(\t\x12\x11\n\treprocess\x18\x0f \x01(\x08\x12 \n\x07service\x18\x11 \x01(\x0b\x32\x0f.pps_v2.Service\x12\x1c\n\x05spout\x18\x12 \x01(\x0b\x32\r.pps_v2.Spout\x12,\n\x0e\x64\x61tum_set_spec\x18\x13 \x01(\x0b\x32\x14.pps_v2.DatumSetSpec\x12\x30\n\rdatum_timeout\x18\x14 \x01(\x0b\x32\x19.google.protobuf.Duration\x12.\n\x0bjob_timeout\x18\x15 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x0c\n\x04salt\x18\x16 \x01(\t\x12\x13\n\x0b\x64\x61tum_tries\x18\x17 \x01(\x03\x12/\n\x0fscheduling_spec\x18\x18 \x01(\x0b\x32\x16.pps_v2.SchedulingSpec\x12\x10\n\x08pod_spec\x18\x19 \x01(\t\x12\x11\n\tpod_patch\x18\x1a \x01(\t\x12#\n\x0bspec_commit\x18\x1b \x01(\x0b\x32\x0e.pfs_v2.Commit\x12\"\n\x08metadata\x18\x1c \x01(\x0b\x32\x10.pps_v2.Metadata\x12\x16\n\x0ereprocess_spec\x18\x1d \x01(\t\x12\x13\n\x0b\x61utoscaling\x18\x1e \x01(\x08\x12\'\n\x0btolerations\x18\" \x03(\x0b\x32\x12.pps_v2.Toleration\x12\x37\n\x19sidecar_resource_requests\x18# \x01(\x0b\x32\x14.pps_v2.ResourceSpec\"M\n\x16InspectPipelineRequest\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\x12\x0f\n\x07\x64\x65tails\x18\x02 \x01(\x08\"\xb7\x01\n\x13ListPipelineRequest\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\x12\x0f\n\x07history\x18\x02 \x01(\x03\x12\x0f\n\x07\x64\x65tails\x18\x03 \x01(\x08\x12\x10\n\x08jqFilter\x18\x04 \x01(\t\x12%\n\ncommit_set\x18\x05 \x01(\x0b\x32\x11.pfs_v2.CommitSet\x12!\n\x08projects\x18\x06 \x03(\x0b\x32\x0f.pfs_v2.Project\"n\n\x15\x44\x65letePipelineRequest\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\x12\x0f\n\x03\x61ll\x18\x02 \x01(\x08\x42\x02\x18\x01\x12\r\n\x05\x66orce\x18\x03 \x01(\x08\x12\x11\n\tkeep_repo\x18\x04 \x01(\x08\"j\n\x16\x44\x65letePipelinesRequest\x12!\n\x08projects\x18\x01 \x03(\x0b\x32\x0f.pfs_v2.Project\x12\r\n\x05\x66orce\x18\x02 \x01(\x08\x12\x11\n\tkeep_repo\x18\x03 \x01(\x08\x12\x0b\n\x03\x61ll\x18\x04 \x01(\x08\">\n\x17\x44\x65letePipelinesResponse\x12#\n\tpipelines\x18\x01 \x03(\x0b\x32\x10.pps_v2.Pipeline\":\n\x14StartPipelineRequest\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\"9\n\x13StopPipelineRequest\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\"l\n\x12RunPipelineRequest\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\x12\"\n\nprovenance\x18\x02 \x03(\x0b\x32\x0e.pfs_v2.Commit\x12\x0e\n\x06job_id\x18\x03 \x01(\t\"4\n\x0eRunCronRequest\x12\"\n\x08pipeline\x18\x01 \x01(\x0b\x32\x10.pps_v2.Pipeline\"#\n\x13\x43reateSecretRequest\x12\x0c\n\x04\x66ile\x18\x01 \x01(\x0c\"5\n\x13\x44\x65leteSecretRequest\x12\x1e\n\x06secret\x18\x01 \x01(\x0b\x32\x0e.pps_v2.Secret\"6\n\x14InspectSecretRequest\x12\x1e\n\x06secret\x18\x01 \x01(\x0b\x32\x0e.pps_v2.Secret\"\x16\n\x06Secret\x12\x0c\n\x04name\x18\x01 \x01(\t\"r\n\nSecretInfo\x12\x1e\n\x06secret\x18\x01 \x01(\x0b\x32\x0e.pps_v2.Secret\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x36\n\x12\x63reation_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"6\n\x0bSecretInfos\x12\'\n\x0bsecret_info\x18\x01 \x03(\x0b\x32\x12.pps_v2.SecretInfo\"\x15\n\x13\x41\x63tivateAuthRequest\"\x16\n\x14\x41\x63tivateAuthResponse\"\x81\x01\n\x12RunLoadTestRequest\x12\x10\n\x08\x64\x61g_spec\x18\x01 \x01(\t\x12\x11\n\tload_spec\x18\x02 \x01(\t\x12\x0c\n\x04seed\x18\x03 \x01(\x03\x12\x13\n\x0bparallelism\x18\x04 \x01(\x03\x12\x11\n\tpod_patch\x18\x05 \x01(\t\x12\x10\n\x08state_id\x18\x06 \x01(\t\"6\n\x13RunLoadTestResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x10\n\x08state_id\x18\x02 \x01(\t\"\x8d\x01\n\x15RenderTemplateRequest\x12\x10\n\x08template\x18\x01 \x01(\t\x12\x35\n\x04\x61rgs\x18\x02 \x03(\x0b\x32\'.pps_v2.RenderTemplateRequest.ArgsEntry\x1a+\n\tArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"T\n\x16RenderTemplateResponse\x12\x0c\n\x04json\x18\x01 \x01(\t\x12,\n\x05specs\x18\x02 \x03(\x0b\x32\x1d.pps_v2.CreatePipelineRequest\"F\n\x0bLokiRequest\x12(\n\x05since\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\r\n\x05query\x18\x02 \x01(\t\"!\n\x0eLokiLogMessage\x12\x0f\n\x07message\x18\x01 \x01(\t*\xc1\x01\n\x08JobState\x12\x15\n\x11JOB_STATE_UNKNOWN\x10\x00\x12\x0f\n\x0bJOB_CREATED\x10\x01\x12\x10\n\x0cJOB_STARTING\x10\x02\x12\x0f\n\x0bJOB_RUNNING\x10\x03\x12\x0f\n\x0bJOB_FAILURE\x10\x04\x12\x0f\n\x0bJOB_SUCCESS\x10\x05\x12\x0e\n\nJOB_KILLED\x10\x06\x12\x11\n\rJOB_EGRESSING\x10\x07\x12\x11\n\rJOB_FINISHING\x10\x08\x12\x12\n\x0eJOB_UNRUNNABLE\x10\t*\\\n\nDatumState\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06\x46\x41ILED\x10\x01\x12\x0b\n\x07SUCCESS\x10\x02\x12\x0b\n\x07SKIPPED\x10\x03\x12\x0c\n\x08STARTING\x10\x04\x12\r\n\tRECOVERED\x10\x05*Y\n\x0bWorkerState\x12\x18\n\x14WORKER_STATE_UNKNOWN\x10\x00\x12\x0f\n\x0bPOD_RUNNING\x10\x01\x12\x0f\n\x0bPOD_SUCCESS\x10\x02\x12\x0e\n\nPOD_FAILED\x10\x03*\xc9\x01\n\rPipelineState\x12\x1a\n\x16PIPELINE_STATE_UNKNOWN\x10\x00\x12\x15\n\x11PIPELINE_STARTING\x10\x01\x12\x14\n\x10PIPELINE_RUNNING\x10\x02\x12\x17\n\x13PIPELINE_RESTARTING\x10\x03\x12\x14\n\x10PIPELINE_FAILURE\x10\x04\x12\x13\n\x0fPIPELINE_PAUSED\x10\x05\x12\x14\n\x10PIPELINE_STANDBY\x10\x06\x12\x15\n\x11PIPELINE_CRASHING\x10\x07*6\n\x12TolerationOperator\x12\t\n\x05\x45MPTY\x10\x00\x12\n\n\x06\x45XISTS\x10\x01\x12\t\n\x05\x45QUAL\x10\x02*W\n\x0bTaintEffect\x12\x0f\n\x0b\x41LL_EFFECTS\x10\x00\x12\x0f\n\x0bNO_SCHEDULE\x10\x01\x12\x16\n\x12PREFER_NO_SCHEDULE\x10\x02\x12\x0e\n\nNO_EXECUTE\x10\x03\x32\xde\x11\n\x03\x41PI\x12:\n\nInspectJob\x12\x19.pps_v2.InspectJobRequest\x1a\x0f.pps_v2.JobInfo\"\x00\x12\x42\n\rInspectJobSet\x12\x1c.pps_v2.InspectJobSetRequest\x1a\x0f.pps_v2.JobInfo\"\x00\x30\x01\x12\x36\n\x07ListJob\x12\x16.pps_v2.ListJobRequest\x1a\x0f.pps_v2.JobInfo\"\x00\x30\x01\x12?\n\nListJobSet\x12\x19.pps_v2.ListJobSetRequest\x1a\x12.pps_v2.JobSetInfo\"\x00\x30\x01\x12@\n\x0cSubscribeJob\x12\x1b.pps_v2.SubscribeJobRequest\x1a\x0f.pps_v2.JobInfo\"\x00\x30\x01\x12?\n\tDeleteJob\x12\x18.pps_v2.DeleteJobRequest\x1a\x16.google.protobuf.Empty\"\x00\x12;\n\x07StopJob\x12\x16.pps_v2.StopJobRequest\x1a\x16.google.protobuf.Empty\"\x00\x12@\n\x0cInspectDatum\x12\x1b.pps_v2.InspectDatumRequest\x1a\x11.pps_v2.DatumInfo\"\x00\x12<\n\tListDatum\x12\x18.pps_v2.ListDatumRequest\x1a\x11.pps_v2.DatumInfo\"\x00\x30\x01\x12\x45\n\x0cRestartDatum\x12\x1b.pps_v2.RestartDatumRequest\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\x0e\x43reatePipeline\x12\x1d.pps_v2.CreatePipelineRequest\x1a\x16.google.protobuf.Empty\"\x00\x12I\n\x0fInspectPipeline\x12\x1e.pps_v2.InspectPipelineRequest\x1a\x14.pps_v2.PipelineInfo\"\x00\x12\x45\n\x0cListPipeline\x12\x1b.pps_v2.ListPipelineRequest\x1a\x14.pps_v2.PipelineInfo\"\x00\x30\x01\x12I\n\x0e\x44\x65letePipeline\x12\x1d.pps_v2.DeletePipelineRequest\x1a\x16.google.protobuf.Empty\"\x00\x12T\n\x0f\x44\x65letePipelines\x12\x1e.pps_v2.DeletePipelinesRequest\x1a\x1f.pps_v2.DeletePipelinesResponse\"\x00\x12G\n\rStartPipeline\x12\x1c.pps_v2.StartPipelineRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x45\n\x0cStopPipeline\x12\x1b.pps_v2.StopPipelineRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x43\n\x0bRunPipeline\x12\x1a.pps_v2.RunPipelineRequest\x1a\x16.google.protobuf.Empty\"\x00\x12;\n\x07RunCron\x12\x16.pps_v2.RunCronRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x45\n\x0c\x43reateSecret\x12\x1b.pps_v2.CreateSecretRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x45\n\x0c\x44\x65leteSecret\x12\x1b.pps_v2.DeleteSecretRequest\x1a\x16.google.protobuf.Empty\"\x00\x12;\n\nListSecret\x12\x16.google.protobuf.Empty\x1a\x13.pps_v2.SecretInfos\"\x00\x12\x43\n\rInspectSecret\x12\x1c.pps_v2.InspectSecretRequest\x1a\x12.pps_v2.SecretInfo\"\x00\x12=\n\tDeleteAll\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x00\x12\x39\n\x07GetLogs\x12\x16.pps_v2.GetLogsRequest\x1a\x12.pps_v2.LogMessage\"\x00\x30\x01\x12K\n\x0c\x41\x63tivateAuth\x12\x1b.pps_v2.ActivateAuthRequest\x1a\x1c.pps_v2.ActivateAuthResponse\"\x00\x12I\n\x0eUpdateJobState\x12\x1d.pps_v2.UpdateJobStateRequest\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x0bRunLoadTest\x12\x1a.pps_v2.RunLoadTestRequest\x1a\x1b.pps_v2.RunLoadTestResponse\"\x00\x12K\n\x12RunLoadTestDefault\x12\x16.google.protobuf.Empty\x1a\x1b.pps_v2.RunLoadTestResponse\"\x00\x12Q\n\x0eRenderTemplate\x12\x1d.pps_v2.RenderTemplateRequest\x1a\x1e.pps_v2.RenderTemplateResponse\"\x00\x12;\n\x08ListTask\x12\x18.taskapi.ListTaskRequest\x1a\x11.taskapi.TaskInfo\"\x00\x30\x01\x12@\n\rGetKubeEvents\x12\x13.pps_v2.LokiRequest\x1a\x16.pps_v2.LokiLogMessage\"\x00\x30\x01\x12<\n\tQueryLoki\x12\x13.pps_v2.LokiRequest\x1a\x16.pps_v2.LokiLogMessage\"\x00\x30\x01\x42+Z)github.com/pachyderm/pachyderm/v2/src/ppsb\x06proto3'
   ,
   dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,google_dot_protobuf_dot_duration__pb2.DESCRIPTOR,google_dot_protobuf_dot_wrappers__pb2.DESCRIPTOR,python__pachyderm_dot_proto_dot_v2_dot_pfs_dot_pfs__pb2.DESCRIPTOR,python__pachyderm_dot_proto_dot_v2_dot_task_dot_task__pb2.DESCRIPTOR,])
 
 _JOBSTATE = _descriptor.EnumDescriptor(
   name='JobState',
   full_name='pps_v2.JobState',
   filename=None,
@@ -86,16 +86,16 @@
       name='JOB_UNRUNNABLE', index=9, number=9,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=11064,
-  serialized_end=11257,
+  serialized_start=11366,
+  serialized_end=11559,
 )
 _sym_db.RegisterEnumDescriptor(_JOBSTATE)
 
 JobState = enum_type_wrapper.EnumTypeWrapper(_JOBSTATE)
 _DATUMSTATE = _descriptor.EnumDescriptor(
   name='DatumState',
   full_name='pps_v2.DatumState',
@@ -132,16 +132,16 @@
       name='RECOVERED', index=5, number=5,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=11259,
-  serialized_end=11351,
+  serialized_start=11561,
+  serialized_end=11653,
 )
 _sym_db.RegisterEnumDescriptor(_DATUMSTATE)
 
 DatumState = enum_type_wrapper.EnumTypeWrapper(_DATUMSTATE)
 _WORKERSTATE = _descriptor.EnumDescriptor(
   name='WorkerState',
   full_name='pps_v2.WorkerState',
@@ -168,16 +168,16 @@
       name='POD_FAILED', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=11353,
-  serialized_end=11442,
+  serialized_start=11655,
+  serialized_end=11744,
 )
 _sym_db.RegisterEnumDescriptor(_WORKERSTATE)
 
 WorkerState = enum_type_wrapper.EnumTypeWrapper(_WORKERSTATE)
 _PIPELINESTATE = _descriptor.EnumDescriptor(
   name='PipelineState',
   full_name='pps_v2.PipelineState',
@@ -224,16 +224,16 @@
       name='PIPELINE_CRASHING', index=7, number=7,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=11445,
-  serialized_end=11646,
+  serialized_start=11747,
+  serialized_end=11948,
 )
 _sym_db.RegisterEnumDescriptor(_PIPELINESTATE)
 
 PipelineState = enum_type_wrapper.EnumTypeWrapper(_PIPELINESTATE)
 _TOLERATIONOPERATOR = _descriptor.EnumDescriptor(
   name='TolerationOperator',
   full_name='pps_v2.TolerationOperator',
@@ -255,16 +255,16 @@
       name='EQUAL', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=11648,
-  serialized_end=11702,
+  serialized_start=11950,
+  serialized_end=12004,
 )
 _sym_db.RegisterEnumDescriptor(_TOLERATIONOPERATOR)
 
 TolerationOperator = enum_type_wrapper.EnumTypeWrapper(_TOLERATIONOPERATOR)
 _TAINTEFFECT = _descriptor.EnumDescriptor(
   name='TaintEffect',
   full_name='pps_v2.TaintEffect',
@@ -291,16 +291,16 @@
       name='NO_EXECUTE', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=11704,
-  serialized_end=11791,
+  serialized_start=12006,
+  serialized_end=12093,
 )
 _sym_db.RegisterEnumDescriptor(_TAINTEFFECT)
 
 TaintEffect = enum_type_wrapper.EnumTypeWrapper(_TAINTEFFECT)
 JOB_STATE_UNKNOWN = 0
 JOB_CREATED = 1
 JOB_STARTING = 2
@@ -364,16 +364,16 @@
       name='PIPELINE_TYPE_SERVICE', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=6116,
-  serialized_end=6238,
+  serialized_start=6254,
+  serialized_end=6376,
 )
 _sym_db.RegisterEnumDescriptor(_PIPELINEINFO_PIPELINETYPE)
 
 
 _SECRETMOUNT = _descriptor.Descriptor(
   name='SecretMount',
   full_name='pps_v2.SecretMount',
@@ -457,16 +457,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=661,
-  serialized_end=703,
+  serialized_start=685,
+  serialized_end=727,
 )
 
 _TRANSFORM = _descriptor.Descriptor(
   name='Transform',
   full_name='pps_v2.Transform',
   filename=None,
   file=DESCRIPTOR,
@@ -567,28 +567,35 @@
     _descriptor.FieldDescriptor(
       name='memory_volume', full_name='pps_v2.Transform.memory_volume', index=13,
       number=14, type=8, cpp_type=7, label=1,
       has_default_value=False, default_value=False,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='datum_batching', full_name='pps_v2.Transform.datum_batching', index=14,
+      number=15, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[_TRANSFORM_ENVENTRY, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=341,
-  serialized_end=703,
+  serialized_end=727,
 )
 
 
 _TFJOB = _descriptor.Descriptor(
   name='TFJob',
   full_name='pps_v2.TFJob',
   filename=None,
@@ -611,16 +618,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=705,
-  serialized_end=728,
+  serialized_start=729,
+  serialized_end=752,
 )
 
 
 _EGRESS = _descriptor.Descriptor(
   name='Egress',
   full_name='pps_v2.Egress',
   filename=None,
@@ -662,16 +669,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='target', full_name='pps_v2.Egress.target',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=731,
-  serialized_end=868,
+  serialized_start=755,
+  serialized_end=892,
 )
 
 
 _JOB = _descriptor.Descriptor(
   name='Job',
   full_name='pps_v2.Job',
   filename=None,
@@ -701,16 +708,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=870,
-  serialized_end=923,
+  serialized_start=894,
+  serialized_end=947,
 )
 
 
 _METADATA_ANNOTATIONSENTRY = _descriptor.Descriptor(
   name='AnnotationsEntry',
   full_name='pps_v2.Metadata.AnnotationsEntry',
   filename=None,
@@ -740,16 +747,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1040,
-  serialized_end=1090,
+  serialized_start=1064,
+  serialized_end=1114,
 )
 
 _METADATA_LABELSENTRY = _descriptor.Descriptor(
   name='LabelsEntry',
   full_name='pps_v2.Metadata.LabelsEntry',
   filename=None,
   file=DESCRIPTOR,
@@ -778,16 +785,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1092,
-  serialized_end=1137,
+  serialized_start=1116,
+  serialized_end=1161,
 )
 
 _METADATA = _descriptor.Descriptor(
   name='Metadata',
   full_name='pps_v2.Metadata',
   filename=None,
   file=DESCRIPTOR,
@@ -816,16 +823,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=926,
-  serialized_end=1137,
+  serialized_start=950,
+  serialized_end=1161,
 )
 
 
 _SERVICE = _descriptor.Descriptor(
   name='Service',
   full_name='pps_v2.Service',
   filename=None,
@@ -869,16 +876,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1139,
-  serialized_end=1220,
+  serialized_start=1163,
+  serialized_end=1244,
 )
 
 
 _SPOUT = _descriptor.Descriptor(
   name='Spout',
   full_name='pps_v2.Spout',
   filename=None,
@@ -901,16 +908,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1222,
-  serialized_end=1263,
+  serialized_start=1246,
+  serialized_end=1287,
 )
 
 
 _PFSINPUT = _descriptor.Descriptor(
   name='PFSInput',
   full_name='pps_v2.PFSInput',
   filename=None,
@@ -1024,16 +1031,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1266,
-  serialized_end=1522,
+  serialized_start=1290,
+  serialized_end=1546,
 )
 
 
 _CRONINPUT = _descriptor.Descriptor(
   name='CronInput',
   full_name='pps_v2.CronInput',
   filename=None,
@@ -1098,16 +1105,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1525,
-  serialized_end=1673,
+  serialized_start=1549,
+  serialized_end=1697,
 )
 
 
 _INPUT = _descriptor.Descriptor(
   name='Input',
   full_name='pps_v2.Input',
   filename=None,
@@ -1165,16 +1172,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1676,
-  serialized_end=1866,
+  serialized_start=1700,
+  serialized_end=1890,
 )
 
 
 _JOBINPUT = _descriptor.Descriptor(
   name='JobInput',
   full_name='pps_v2.JobInput',
   filename=None,
@@ -1218,16 +1225,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1868,
-  serialized_end=1952,
+  serialized_start=1892,
+  serialized_end=1976,
 )
 
 
 _PARALLELISMSPEC = _descriptor.Descriptor(
   name='ParallelismSpec',
   full_name='pps_v2.ParallelismSpec',
   filename=None,
@@ -1250,16 +1257,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1954,
-  serialized_end=1989,
+  serialized_start=1978,
+  serialized_end=2013,
 )
 
 
 _INPUTFILE = _descriptor.Descriptor(
   name='InputFile',
   full_name='pps_v2.InputFile',
   filename=None,
@@ -1289,16 +1296,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1991,
-  serialized_end=2030,
+  serialized_start=2015,
+  serialized_end=2054,
 )
 
 
 _DATUM = _descriptor.Descriptor(
   name='Datum',
   full_name='pps_v2.Datum',
   filename=None,
@@ -1328,16 +1335,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2032,
-  serialized_end=2077,
+  serialized_start=2056,
+  serialized_end=2101,
 )
 
 
 _DATUMINFO = _descriptor.Descriptor(
   name='DatumInfo',
   full_name='pps_v2.DatumInfo',
   filename=None,
@@ -1395,16 +1402,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2080,
-  serialized_end=2276,
+  serialized_start=2104,
+  serialized_end=2300,
 )
 
 
 _AGGREGATE = _descriptor.Descriptor(
   name='Aggregate',
   full_name='pps_v2.Aggregate',
   filename=None,
@@ -1455,16 +1462,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2278,
-  serialized_end=2393,
+  serialized_start=2302,
+  serialized_end=2417,
 )
 
 
 _PROCESSSTATS = _descriptor.Descriptor(
   name='ProcessStats',
   full_name='pps_v2.ProcessStats',
   filename=None,
@@ -1515,16 +1522,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2396,
-  serialized_end=2603,
+  serialized_start=2420,
+  serialized_end=2627,
 )
 
 
 _AGGREGATEPROCESSSTATS = _descriptor.Descriptor(
   name='AggregateProcessStats',
   full_name='pps_v2.AggregateProcessStats',
   filename=None,
@@ -1575,16 +1582,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2606,
-  serialized_end=2836,
+  serialized_start=2630,
+  serialized_end=2860,
 )
 
 
 _WORKERSTATUS = _descriptor.Descriptor(
   name='WorkerStatus',
   full_name='pps_v2.WorkerStatus',
   filename=None,
@@ -1621,16 +1628,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2838,
-  serialized_end=2930,
+  serialized_start=2862,
+  serialized_end=2954,
 )
 
 
 _DATUMSTATUS = _descriptor.Descriptor(
   name='DatumStatus',
   full_name='pps_v2.DatumStatus',
   filename=None,
@@ -1660,16 +1667,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2932,
-  serialized_end=3023,
+  serialized_start=2956,
+  serialized_end=3047,
 )
 
 
 _RESOURCESPEC = _descriptor.Descriptor(
   name='ResourceSpec',
   full_name='pps_v2.ResourceSpec',
   filename=None,
@@ -1713,16 +1720,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3025,
-  serialized_end=3112,
+  serialized_start=3049,
+  serialized_end=3136,
 )
 
 
 _GPUSPEC = _descriptor.Descriptor(
   name='GPUSpec',
   full_name='pps_v2.GPUSpec',
   filename=None,
@@ -1752,16 +1759,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3114,
-  serialized_end=3153,
+  serialized_start=3138,
+  serialized_end=3177,
 )
 
 
 _JOBSETINFO = _descriptor.Descriptor(
   name='JobSetInfo',
   full_name='pps_v2.JobSetInfo',
   filename=None,
@@ -1791,16 +1798,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3155,
-  serialized_end=3231,
+  serialized_start=3179,
+  serialized_end=3255,
 )
 
 
 _JOBINFO_DETAILS = _descriptor.Descriptor(
   name='Details',
   full_name='pps_v2.JobInfo.Details',
   filename=None,
@@ -1930,28 +1937,35 @@
     _descriptor.FieldDescriptor(
       name='pod_patch', full_name='pps_v2.JobInfo.Details.pod_patch', index=17,
       number=18, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='sidecar_resource_requests', full_name='pps_v2.JobInfo.Details.sidecar_resource_requests', index=18,
+      number=19, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3729,
-  serialized_end=4414,
+  serialized_start=3753,
+  serialized_end=4495,
 )
 
 _JOBINFO = _descriptor.Descriptor(
   name='JobInfo',
   full_name='pps_v2.JobInfo',
   filename=None,
   file=DESCRIPTOR,
@@ -2078,16 +2092,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3234,
-  serialized_end=4414,
+  serialized_start=3258,
+  serialized_end=4495,
 )
 
 
 _WORKER = _descriptor.Descriptor(
   name='Worker',
   full_name='pps_v2.Worker',
   filename=None,
@@ -2117,16 +2131,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4416,
-  serialized_end=4474,
+  serialized_start=4497,
+  serialized_end=4555,
 )
 
 
 _PIPELINE = _descriptor.Descriptor(
   name='Pipeline',
   full_name='pps_v2.Pipeline',
   filename=None,
@@ -2156,16 +2170,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4476,
-  serialized_end=4534,
+  serialized_start=4557,
+  serialized_end=4615,
 )
 
 
 _TOLERATION = _descriptor.Descriptor(
   name='Toleration',
   full_name='pps_v2.Toleration',
   filename=None,
@@ -2216,16 +2230,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4537,
-  serialized_end=4717,
+  serialized_start=4618,
+  serialized_end=4798,
 )
 
 
 _PIPELINEINFO_DETAILS = _descriptor.Descriptor(
   name='Details',
   full_name='pps_v2.PipelineInfo.Details',
   filename=None,
@@ -2453,28 +2467,35 @@
     _descriptor.FieldDescriptor(
       name='tolerations', full_name='pps_v2.PipelineInfo.Details.tolerations', index=31,
       number=34, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='sidecar_resource_requests', full_name='pps_v2.PipelineInfo.Details.sidecar_resource_requests', index=32,
+      number=35, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=5077,
-  serialized_end=6114,
+  serialized_start=5158,
+  serialized_end=6252,
 )
 
 _PIPELINEINFO = _descriptor.Descriptor(
   name='PipelineInfo',
   full_name='pps_v2.PipelineInfo',
   filename=None,
   file=DESCRIPTOR,
@@ -2567,16 +2588,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4720,
-  serialized_end=6244,
+  serialized_start=4801,
+  serialized_end=6382,
 )
 
 
 _PIPELINEINFOS = _descriptor.Descriptor(
   name='PipelineInfos',
   full_name='pps_v2.PipelineInfos',
   filename=None,
@@ -2599,16 +2620,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6246,
-  serialized_end=6306,
+  serialized_start=6384,
+  serialized_end=6444,
 )
 
 
 _JOBSET = _descriptor.Descriptor(
   name='JobSet',
   full_name='pps_v2.JobSet',
   filename=None,
@@ -2631,16 +2652,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6308,
-  serialized_end=6328,
+  serialized_start=6446,
+  serialized_end=6466,
 )
 
 
 _INSPECTJOBSETREQUEST = _descriptor.Descriptor(
   name='InspectJobSetRequest',
   full_name='pps_v2.InspectJobSetRequest',
   filename=None,
@@ -2677,16 +2698,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6330,
-  serialized_end=6416,
+  serialized_start=6468,
+  serialized_end=6554,
 )
 
 
 _LISTJOBSETREQUEST = _descriptor.Descriptor(
   name='ListJobSetRequest',
   full_name='pps_v2.ListJobSetRequest',
   filename=None,
@@ -2737,16 +2758,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6419,
-  serialized_end=6577,
+  serialized_start=6557,
+  serialized_end=6715,
 )
 
 
 _INSPECTJOBREQUEST = _descriptor.Descriptor(
   name='InspectJobRequest',
   full_name='pps_v2.InspectJobRequest',
   filename=None,
@@ -2783,16 +2804,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6579,
-  serialized_end=6655,
+  serialized_start=6717,
+  serialized_end=6793,
 )
 
 
 _LISTJOBREQUEST = _descriptor.Descriptor(
   name='ListJobRequest',
   full_name='pps_v2.ListJobRequest',
   filename=None,
@@ -2871,16 +2892,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6658,
-  serialized_end=6922,
+  serialized_start=6796,
+  serialized_end=7060,
 )
 
 
 _SUBSCRIBEJOBREQUEST = _descriptor.Descriptor(
   name='SubscribeJobRequest',
   full_name='pps_v2.SubscribeJobRequest',
   filename=None,
@@ -2910,16 +2931,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=6924,
-  serialized_end=6998,
+  serialized_start=7062,
+  serialized_end=7136,
 )
 
 
 _DELETEJOBREQUEST = _descriptor.Descriptor(
   name='DeleteJobRequest',
   full_name='pps_v2.DeleteJobRequest',
   filename=None,
@@ -2942,16 +2963,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7000,
-  serialized_end=7044,
+  serialized_start=7138,
+  serialized_end=7182,
 )
 
 
 _STOPJOBREQUEST = _descriptor.Descriptor(
   name='StopJobRequest',
   full_name='pps_v2.StopJobRequest',
   filename=None,
@@ -2981,16 +3002,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7046,
-  serialized_end=7104,
+  serialized_start=7184,
+  serialized_end=7242,
 )
 
 
 _UPDATEJOBSTATEREQUEST = _descriptor.Descriptor(
   name='UpdateJobStateRequest',
   full_name='pps_v2.UpdateJobStateRequest',
   filename=None,
@@ -3076,16 +3097,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7107,
-  serialized_end=7370,
+  serialized_start=7245,
+  serialized_end=7508,
 )
 
 
 _GETLOGSREQUEST = _descriptor.Descriptor(
   name='GetLogsRequest',
   full_name='pps_v2.GetLogsRequest',
   filename=None,
@@ -3164,16 +3185,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7373,
-  serialized_end=7617,
+  serialized_start=7511,
+  serialized_end=7755,
 )
 
 
 _LOGMESSAGE = _descriptor.Descriptor(
   name='LogMessage',
   full_name='pps_v2.LogMessage',
   filename=None,
@@ -3259,16 +3280,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7620,
-  serialized_end=7850,
+  serialized_start=7758,
+  serialized_end=7988,
 )
 
 
 _RESTARTDATUMREQUEST = _descriptor.Descriptor(
   name='RestartDatumRequest',
   full_name='pps_v2.RestartDatumRequest',
   filename=None,
@@ -3298,16 +3319,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7852,
-  serialized_end=7921,
+  serialized_start=7990,
+  serialized_end=8059,
 )
 
 
 _INSPECTDATUMREQUEST = _descriptor.Descriptor(
   name='InspectDatumRequest',
   full_name='pps_v2.InspectDatumRequest',
   filename=None,
@@ -3330,16 +3351,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7923,
-  serialized_end=7974,
+  serialized_start=8061,
+  serialized_end=8112,
 )
 
 
 _LISTDATUMREQUEST_FILTER = _descriptor.Descriptor(
   name='Filter',
   full_name='pps_v2.ListDatumRequest.Filter',
   filename=None,
@@ -3362,16 +3383,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8161,
-  serialized_end=8204,
+  serialized_start=8299,
+  serialized_end=8342,
 )
 
 _LISTDATUMREQUEST = _descriptor.Descriptor(
   name='ListDatumRequest',
   full_name='pps_v2.ListDatumRequest',
   filename=None,
   file=DESCRIPTOR,
@@ -3428,16 +3449,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7977,
-  serialized_end=8204,
+  serialized_start=8115,
+  serialized_end=8342,
 )
 
 
 _DATUMSETSPEC = _descriptor.Descriptor(
   name='DatumSetSpec',
   full_name='pps_v2.DatumSetSpec',
   filename=None,
@@ -3474,16 +3495,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8206,
-  serialized_end=8276,
+  serialized_start=8344,
+  serialized_end=8414,
 )
 
 
 _SCHEDULINGSPEC_NODESELECTORENTRY = _descriptor.Descriptor(
   name='NodeSelectorEntry',
   full_name='pps_v2.SchedulingSpec.NodeSelectorEntry',
   filename=None,
@@ -3513,16 +3534,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8391,
-  serialized_end=8442,
+  serialized_start=8529,
+  serialized_end=8580,
 )
 
 _SCHEDULINGSPEC = _descriptor.Descriptor(
   name='SchedulingSpec',
   full_name='pps_v2.SchedulingSpec',
   filename=None,
   file=DESCRIPTOR,
@@ -3551,16 +3572,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8279,
-  serialized_end=8442,
+  serialized_start=8417,
+  serialized_end=8580,
 )
 
 
 _CREATEPIPELINEREQUEST = _descriptor.Descriptor(
   name='CreatePipelineRequest',
   full_name='pps_v2.CreatePipelineRequest',
   filename=None,
@@ -3767,28 +3788,35 @@
     _descriptor.FieldDescriptor(
       name='tolerations', full_name='pps_v2.CreatePipelineRequest.tolerations', index=28,
       number=34, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='sidecar_resource_requests', full_name='pps_v2.CreatePipelineRequest.sidecar_resource_requests', index=29,
+      number=35, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8445,
-  serialized_end=9420,
+  serialized_start=8583,
+  serialized_end=9615,
 )
 
 
 _INSPECTPIPELINEREQUEST = _descriptor.Descriptor(
   name='InspectPipelineRequest',
   full_name='pps_v2.InspectPipelineRequest',
   filename=None,
@@ -3818,16 +3846,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=9422,
-  serialized_end=9499,
+  serialized_start=9617,
+  serialized_end=9694,
 )
 
 
 _LISTPIPELINEREQUEST = _descriptor.Descriptor(
   name='ListPipelineRequest',
   full_name='pps_v2.ListPipelineRequest',
   filename=None,
@@ -3885,16 +3913,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=9502,
-  serialized_end=9685,
+  serialized_start=9697,
+  serialized_end=9880,
 )
 
 
 _DELETEPIPELINEREQUEST = _descriptor.Descriptor(
   name='DeletePipelineRequest',
   full_name='pps_v2.DeletePipelineRequest',
   filename=None,
@@ -3938,16 +3966,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=9687,
-  serialized_end=9797,
+  serialized_start=9882,
+  serialized_end=9992,
 )
 
 
 _DELETEPIPELINESREQUEST = _descriptor.Descriptor(
   name='DeletePipelinesRequest',
   full_name='pps_v2.DeletePipelinesRequest',
   filename=None,
@@ -3991,16 +4019,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=9799,
-  serialized_end=9905,
+  serialized_start=9994,
+  serialized_end=10100,
 )
 
 
 _DELETEPIPELINESRESPONSE = _descriptor.Descriptor(
   name='DeletePipelinesResponse',
   full_name='pps_v2.DeletePipelinesResponse',
   filename=None,
@@ -4023,16 +4051,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=9907,
-  serialized_end=9969,
+  serialized_start=10102,
+  serialized_end=10164,
 )
 
 
 _STARTPIPELINEREQUEST = _descriptor.Descriptor(
   name='StartPipelineRequest',
   full_name='pps_v2.StartPipelineRequest',
   filename=None,
@@ -4055,16 +4083,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=9971,
-  serialized_end=10029,
+  serialized_start=10166,
+  serialized_end=10224,
 )
 
 
 _STOPPIPELINEREQUEST = _descriptor.Descriptor(
   name='StopPipelineRequest',
   full_name='pps_v2.StopPipelineRequest',
   filename=None,
@@ -4087,16 +4115,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10031,
-  serialized_end=10088,
+  serialized_start=10226,
+  serialized_end=10283,
 )
 
 
 _RUNPIPELINEREQUEST = _descriptor.Descriptor(
   name='RunPipelineRequest',
   full_name='pps_v2.RunPipelineRequest',
   filename=None,
@@ -4133,16 +4161,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10090,
-  serialized_end=10198,
+  serialized_start=10285,
+  serialized_end=10393,
 )
 
 
 _RUNCRONREQUEST = _descriptor.Descriptor(
   name='RunCronRequest',
   full_name='pps_v2.RunCronRequest',
   filename=None,
@@ -4165,16 +4193,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10200,
-  serialized_end=10252,
+  serialized_start=10395,
+  serialized_end=10447,
 )
 
 
 _CREATESECRETREQUEST = _descriptor.Descriptor(
   name='CreateSecretRequest',
   full_name='pps_v2.CreateSecretRequest',
   filename=None,
@@ -4197,16 +4225,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10254,
-  serialized_end=10289,
+  serialized_start=10449,
+  serialized_end=10484,
 )
 
 
 _DELETESECRETREQUEST = _descriptor.Descriptor(
   name='DeleteSecretRequest',
   full_name='pps_v2.DeleteSecretRequest',
   filename=None,
@@ -4229,16 +4257,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10291,
-  serialized_end=10344,
+  serialized_start=10486,
+  serialized_end=10539,
 )
 
 
 _INSPECTSECRETREQUEST = _descriptor.Descriptor(
   name='InspectSecretRequest',
   full_name='pps_v2.InspectSecretRequest',
   filename=None,
@@ -4261,16 +4289,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10346,
-  serialized_end=10400,
+  serialized_start=10541,
+  serialized_end=10595,
 )
 
 
 _SECRET = _descriptor.Descriptor(
   name='Secret',
   full_name='pps_v2.Secret',
   filename=None,
@@ -4293,16 +4321,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10402,
-  serialized_end=10424,
+  serialized_start=10597,
+  serialized_end=10619,
 )
 
 
 _SECRETINFO = _descriptor.Descriptor(
   name='SecretInfo',
   full_name='pps_v2.SecretInfo',
   filename=None,
@@ -4339,16 +4367,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10426,
-  serialized_end=10540,
+  serialized_start=10621,
+  serialized_end=10735,
 )
 
 
 _SECRETINFOS = _descriptor.Descriptor(
   name='SecretInfos',
   full_name='pps_v2.SecretInfos',
   filename=None,
@@ -4371,16 +4399,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10542,
-  serialized_end=10596,
+  serialized_start=10737,
+  serialized_end=10791,
 )
 
 
 _ACTIVATEAUTHREQUEST = _descriptor.Descriptor(
   name='ActivateAuthRequest',
   full_name='pps_v2.ActivateAuthRequest',
   filename=None,
@@ -4396,16 +4424,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10598,
-  serialized_end=10619,
+  serialized_start=10793,
+  serialized_end=10814,
 )
 
 
 _ACTIVATEAUTHRESPONSE = _descriptor.Descriptor(
   name='ActivateAuthResponse',
   full_name='pps_v2.ActivateAuthResponse',
   filename=None,
@@ -4421,16 +4449,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10621,
-  serialized_end=10643,
+  serialized_start=10816,
+  serialized_end=10838,
 )
 
 
 _RUNLOADTESTREQUEST = _descriptor.Descriptor(
   name='RunLoadTestRequest',
   full_name='pps_v2.RunLoadTestRequest',
   filename=None,
@@ -4488,16 +4516,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10646,
-  serialized_end=10775,
+  serialized_start=10841,
+  serialized_end=10970,
 )
 
 
 _RUNLOADTESTRESPONSE = _descriptor.Descriptor(
   name='RunLoadTestResponse',
   full_name='pps_v2.RunLoadTestResponse',
   filename=None,
@@ -4527,16 +4555,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10777,
-  serialized_end=10831,
+  serialized_start=10972,
+  serialized_end=11026,
 )
 
 
 _RENDERTEMPLATEREQUEST_ARGSENTRY = _descriptor.Descriptor(
   name='ArgsEntry',
   full_name='pps_v2.RenderTemplateRequest.ArgsEntry',
   filename=None,
@@ -4566,16 +4594,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10932,
-  serialized_end=10975,
+  serialized_start=11127,
+  serialized_end=11170,
 )
 
 _RENDERTEMPLATEREQUEST = _descriptor.Descriptor(
   name='RenderTemplateRequest',
   full_name='pps_v2.RenderTemplateRequest',
   filename=None,
   file=DESCRIPTOR,
@@ -4604,16 +4632,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10834,
-  serialized_end=10975,
+  serialized_start=11029,
+  serialized_end=11170,
 )
 
 
 _RENDERTEMPLATERESPONSE = _descriptor.Descriptor(
   name='RenderTemplateResponse',
   full_name='pps_v2.RenderTemplateResponse',
   filename=None,
@@ -4643,16 +4671,87 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10977,
-  serialized_end=11061,
+  serialized_start=11172,
+  serialized_end=11256,
+)
+
+
+_LOKIREQUEST = _descriptor.Descriptor(
+  name='LokiRequest',
+  full_name='pps_v2.LokiRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='since', full_name='pps_v2.LokiRequest.since', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='query', full_name='pps_v2.LokiRequest.query', index=1,
+      number=2, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=11258,
+  serialized_end=11328,
+)
+
+
+_LOKILOGMESSAGE = _descriptor.Descriptor(
+  name='LokiLogMessage',
+  full_name='pps_v2.LokiLogMessage',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='message', full_name='pps_v2.LokiLogMessage.message', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=11330,
+  serialized_end=11363,
 )
 
 _TRANSFORM_ENVENTRY.containing_type = _TRANSFORM
 _TRANSFORM.fields_by_name['env'].message_type = _TRANSFORM_ENVENTRY
 _TRANSFORM.fields_by_name['secrets'].message_type = _SECRETMOUNT
 _EGRESS.fields_by_name['object_storage'].message_type = python__pachyderm_dot_proto_dot_v2_dot_pfs_dot_pfs__pb2._OBJECTSTORAGEEGRESS
 _EGRESS.fields_by_name['sql_database'].message_type = python__pachyderm_dot_proto_dot_v2_dot_pfs_dot_pfs__pb2._SQLDATABASEEGRESS
@@ -4707,14 +4806,15 @@
 _JOBINFO_DETAILS.fields_by_name['resource_limits'].message_type = _RESOURCESPEC
 _JOBINFO_DETAILS.fields_by_name['sidecar_resource_limits'].message_type = _RESOURCESPEC
 _JOBINFO_DETAILS.fields_by_name['input'].message_type = _INPUT
 _JOBINFO_DETAILS.fields_by_name['datum_set_spec'].message_type = _DATUMSETSPEC
 _JOBINFO_DETAILS.fields_by_name['datum_timeout'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
 _JOBINFO_DETAILS.fields_by_name['job_timeout'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
 _JOBINFO_DETAILS.fields_by_name['scheduling_spec'].message_type = _SCHEDULINGSPEC
+_JOBINFO_DETAILS.fields_by_name['sidecar_resource_requests'].message_type = _RESOURCESPEC
 _JOBINFO_DETAILS.containing_type = _JOBINFO
 _JOBINFO.fields_by_name['job'].message_type = _JOB
 _JOBINFO.fields_by_name['output_commit'].message_type = python__pachyderm_dot_proto_dot_v2_dot_pfs_dot_pfs__pb2._COMMIT
 _JOBINFO.fields_by_name['stats'].message_type = _PROCESSSTATS
 _JOBINFO.fields_by_name['state'].enum_type = _JOBSTATE
 _JOBINFO.fields_by_name['created'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _JOBINFO.fields_by_name['started'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
@@ -4738,14 +4838,15 @@
 _PIPELINEINFO_DETAILS.fields_by_name['spout'].message_type = _SPOUT
 _PIPELINEINFO_DETAILS.fields_by_name['datum_set_spec'].message_type = _DATUMSETSPEC
 _PIPELINEINFO_DETAILS.fields_by_name['datum_timeout'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
 _PIPELINEINFO_DETAILS.fields_by_name['job_timeout'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
 _PIPELINEINFO_DETAILS.fields_by_name['scheduling_spec'].message_type = _SCHEDULINGSPEC
 _PIPELINEINFO_DETAILS.fields_by_name['metadata'].message_type = _METADATA
 _PIPELINEINFO_DETAILS.fields_by_name['tolerations'].message_type = _TOLERATION
+_PIPELINEINFO_DETAILS.fields_by_name['sidecar_resource_requests'].message_type = _RESOURCESPEC
 _PIPELINEINFO_DETAILS.containing_type = _PIPELINEINFO
 _PIPELINEINFO.fields_by_name['pipeline'].message_type = _PIPELINE
 _PIPELINEINFO.fields_by_name['spec_commit'].message_type = python__pachyderm_dot_proto_dot_v2_dot_pfs_dot_pfs__pb2._COMMIT
 _PIPELINEINFO.fields_by_name['state'].enum_type = _PIPELINESTATE
 _PIPELINEINFO.fields_by_name['last_job_state'].enum_type = _JOBSTATE
 _PIPELINEINFO.fields_by_name['type'].enum_type = _PIPELINEINFO_PIPELINETYPE
 _PIPELINEINFO.fields_by_name['details'].message_type = _PIPELINEINFO_DETAILS
@@ -4794,14 +4895,15 @@
 _CREATEPIPELINEREQUEST.fields_by_name['datum_set_spec'].message_type = _DATUMSETSPEC
 _CREATEPIPELINEREQUEST.fields_by_name['datum_timeout'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
 _CREATEPIPELINEREQUEST.fields_by_name['job_timeout'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
 _CREATEPIPELINEREQUEST.fields_by_name['scheduling_spec'].message_type = _SCHEDULINGSPEC
 _CREATEPIPELINEREQUEST.fields_by_name['spec_commit'].message_type = python__pachyderm_dot_proto_dot_v2_dot_pfs_dot_pfs__pb2._COMMIT
 _CREATEPIPELINEREQUEST.fields_by_name['metadata'].message_type = _METADATA
 _CREATEPIPELINEREQUEST.fields_by_name['tolerations'].message_type = _TOLERATION
+_CREATEPIPELINEREQUEST.fields_by_name['sidecar_resource_requests'].message_type = _RESOURCESPEC
 _INSPECTPIPELINEREQUEST.fields_by_name['pipeline'].message_type = _PIPELINE
 _LISTPIPELINEREQUEST.fields_by_name['pipeline'].message_type = _PIPELINE
 _LISTPIPELINEREQUEST.fields_by_name['commit_set'].message_type = python__pachyderm_dot_proto_dot_v2_dot_pfs_dot_pfs__pb2._COMMITSET
 _LISTPIPELINEREQUEST.fields_by_name['projects'].message_type = python__pachyderm_dot_proto_dot_v2_dot_pfs_dot_pfs__pb2._PROJECT
 _DELETEPIPELINEREQUEST.fields_by_name['pipeline'].message_type = _PIPELINE
 _DELETEPIPELINESREQUEST.fields_by_name['projects'].message_type = python__pachyderm_dot_proto_dot_v2_dot_pfs_dot_pfs__pb2._PROJECT
 _DELETEPIPELINESRESPONSE.fields_by_name['pipelines'].message_type = _PIPELINE
@@ -4814,14 +4916,15 @@
 _INSPECTSECRETREQUEST.fields_by_name['secret'].message_type = _SECRET
 _SECRETINFO.fields_by_name['secret'].message_type = _SECRET
 _SECRETINFO.fields_by_name['creation_timestamp'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _SECRETINFOS.fields_by_name['secret_info'].message_type = _SECRETINFO
 _RENDERTEMPLATEREQUEST_ARGSENTRY.containing_type = _RENDERTEMPLATEREQUEST
 _RENDERTEMPLATEREQUEST.fields_by_name['args'].message_type = _RENDERTEMPLATEREQUEST_ARGSENTRY
 _RENDERTEMPLATERESPONSE.fields_by_name['specs'].message_type = _CREATEPIPELINEREQUEST
+_LOKIREQUEST.fields_by_name['since'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
 DESCRIPTOR.message_types_by_name['SecretMount'] = _SECRETMOUNT
 DESCRIPTOR.message_types_by_name['Transform'] = _TRANSFORM
 DESCRIPTOR.message_types_by_name['TFJob'] = _TFJOB
 DESCRIPTOR.message_types_by_name['Egress'] = _EGRESS
 DESCRIPTOR.message_types_by_name['Job'] = _JOB
 DESCRIPTOR.message_types_by_name['Metadata'] = _METADATA
 DESCRIPTOR.message_types_by_name['Service'] = _SERVICE
@@ -4882,14 +4985,16 @@
 DESCRIPTOR.message_types_by_name['SecretInfos'] = _SECRETINFOS
 DESCRIPTOR.message_types_by_name['ActivateAuthRequest'] = _ACTIVATEAUTHREQUEST
 DESCRIPTOR.message_types_by_name['ActivateAuthResponse'] = _ACTIVATEAUTHRESPONSE
 DESCRIPTOR.message_types_by_name['RunLoadTestRequest'] = _RUNLOADTESTREQUEST
 DESCRIPTOR.message_types_by_name['RunLoadTestResponse'] = _RUNLOADTESTRESPONSE
 DESCRIPTOR.message_types_by_name['RenderTemplateRequest'] = _RENDERTEMPLATEREQUEST
 DESCRIPTOR.message_types_by_name['RenderTemplateResponse'] = _RENDERTEMPLATERESPONSE
+DESCRIPTOR.message_types_by_name['LokiRequest'] = _LOKIREQUEST
+DESCRIPTOR.message_types_by_name['LokiLogMessage'] = _LOKILOGMESSAGE
 DESCRIPTOR.enum_types_by_name['JobState'] = _JOBSTATE
 DESCRIPTOR.enum_types_by_name['DatumState'] = _DATUMSTATE
 DESCRIPTOR.enum_types_by_name['WorkerState'] = _WORKERSTATE
 DESCRIPTOR.enum_types_by_name['PipelineState'] = _PIPELINESTATE
 DESCRIPTOR.enum_types_by_name['TolerationOperator'] = _TOLERATIONOPERATOR
 DESCRIPTOR.enum_types_by_name['TaintEffect'] = _TAINTEFFECT
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
@@ -5430,14 +5535,28 @@
 RenderTemplateResponse = _reflection.GeneratedProtocolMessageType('RenderTemplateResponse', (_message.Message,), {
   'DESCRIPTOR' : _RENDERTEMPLATERESPONSE,
   '__module__' : 'python_pachyderm.proto.v2.pps.pps_pb2'
   # @@protoc_insertion_point(class_scope:pps_v2.RenderTemplateResponse)
   })
 _sym_db.RegisterMessage(RenderTemplateResponse)
 
+LokiRequest = _reflection.GeneratedProtocolMessageType('LokiRequest', (_message.Message,), {
+  'DESCRIPTOR' : _LOKIREQUEST,
+  '__module__' : 'python_pachyderm.proto.v2.pps.pps_pb2'
+  # @@protoc_insertion_point(class_scope:pps_v2.LokiRequest)
+  })
+_sym_db.RegisterMessage(LokiRequest)
+
+LokiLogMessage = _reflection.GeneratedProtocolMessageType('LokiLogMessage', (_message.Message,), {
+  'DESCRIPTOR' : _LOKILOGMESSAGE,
+  '__module__' : 'python_pachyderm.proto.v2.pps.pps_pb2'
+  # @@protoc_insertion_point(class_scope:pps_v2.LokiLogMessage)
+  })
+_sym_db.RegisterMessage(LokiLogMessage)
+
 
 DESCRIPTOR._options = None
 _TRANSFORM_ENVENTRY._options = None
 _METADATA_ANNOTATIONSENTRY._options = None
 _METADATA_LABELSENTRY._options = None
 _SCHEDULINGSPEC_NODESELECTORENTRY._options = None
 _DELETEPIPELINEREQUEST.fields_by_name['all']._options = None
@@ -5446,16 +5565,16 @@
 _API = _descriptor.ServiceDescriptor(
   name='API',
   full_name='pps_v2.API',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=11794,
-  serialized_end=13936,
+  serialized_start=12096,
+  serialized_end=14366,
   methods=[
   _descriptor.MethodDescriptor(
     name='InspectJob',
     full_name='pps_v2.API.InspectJob',
     index=0,
     containing_service=None,
     input_type=_INSPECTJOBREQUEST,
@@ -5759,13 +5878,33 @@
     index=30,
     containing_service=None,
     input_type=python__pachyderm_dot_proto_dot_v2_dot_task_dot_task__pb2._LISTTASKREQUEST,
     output_type=python__pachyderm_dot_proto_dot_v2_dot_task_dot_task__pb2._TASKINFO,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
+  _descriptor.MethodDescriptor(
+    name='GetKubeEvents',
+    full_name='pps_v2.API.GetKubeEvents',
+    index=31,
+    containing_service=None,
+    input_type=_LOKIREQUEST,
+    output_type=_LOKILOGMESSAGE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='QueryLoki',
+    full_name='pps_v2.API.QueryLoki',
+    index=32,
+    containing_service=None,
+    input_type=_LOKIREQUEST,
+    output_type=_LOKILOGMESSAGE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
 ])
 _sym_db.RegisterServiceDescriptor(_API)
 
 DESCRIPTOR.services_by_name['API'] = _API
 
 # @@protoc_insertion_point(module_scope)
```

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/pps/pps_pb2_grpc.py` & `python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/pps/pps_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,14 +167,24 @@
                 response_deserializer=python__pachyderm_dot_proto_dot_v2_dot_pps_dot_pps__pb2.RenderTemplateResponse.FromString,
                 )
         self.ListTask = channel.unary_stream(
                 '/pps_v2.API/ListTask',
                 request_serializer=python__pachyderm_dot_proto_dot_v2_dot_task_dot_task__pb2.ListTaskRequest.SerializeToString,
                 response_deserializer=python__pachyderm_dot_proto_dot_v2_dot_task_dot_task__pb2.TaskInfo.FromString,
                 )
+        self.GetKubeEvents = channel.unary_stream(
+                '/pps_v2.API/GetKubeEvents',
+                request_serializer=python__pachyderm_dot_proto_dot_v2_dot_pps_dot_pps__pb2.LokiRequest.SerializeToString,
+                response_deserializer=python__pachyderm_dot_proto_dot_v2_dot_pps_dot_pps__pb2.LokiLogMessage.FromString,
+                )
+        self.QueryLoki = channel.unary_stream(
+                '/pps_v2.API/QueryLoki',
+                request_serializer=python__pachyderm_dot_proto_dot_v2_dot_pps_dot_pps__pb2.LokiRequest.SerializeToString,
+                response_deserializer=python__pachyderm_dot_proto_dot_v2_dot_pps_dot_pps__pb2.LokiLogMessage.FromString,
+                )
 
 
 class APIServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def InspectJob(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -368,14 +378,28 @@
     def ListTask(self, request, context):
         """ListTask lists PPS tasks
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetKubeEvents(self, request, context):
+        """GetKubeEvents returns a stream of kubernetes events
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def QueryLoki(self, request, context):
+        """QueryLoki returns a stream of loki log messages given a query string
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_APIServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'InspectJob': grpc.unary_unary_rpc_method_handler(
                     servicer.InspectJob,
                     request_deserializer=python__pachyderm_dot_proto_dot_v2_dot_pps_dot_pps__pb2.InspectJobRequest.FromString,
                     response_serializer=python__pachyderm_dot_proto_dot_v2_dot_pps_dot_pps__pb2.JobInfo.SerializeToString,
@@ -526,14 +550,24 @@
                     response_serializer=python__pachyderm_dot_proto_dot_v2_dot_pps_dot_pps__pb2.RenderTemplateResponse.SerializeToString,
             ),
             'ListTask': grpc.unary_stream_rpc_method_handler(
                     servicer.ListTask,
                     request_deserializer=python__pachyderm_dot_proto_dot_v2_dot_task_dot_task__pb2.ListTaskRequest.FromString,
                     response_serializer=python__pachyderm_dot_proto_dot_v2_dot_task_dot_task__pb2.TaskInfo.SerializeToString,
             ),
+            'GetKubeEvents': grpc.unary_stream_rpc_method_handler(
+                    servicer.GetKubeEvents,
+                    request_deserializer=python__pachyderm_dot_proto_dot_v2_dot_pps_dot_pps__pb2.LokiRequest.FromString,
+                    response_serializer=python__pachyderm_dot_proto_dot_v2_dot_pps_dot_pps__pb2.LokiLogMessage.SerializeToString,
+            ),
+            'QueryLoki': grpc.unary_stream_rpc_method_handler(
+                    servicer.QueryLoki,
+                    request_deserializer=python__pachyderm_dot_proto_dot_v2_dot_pps_dot_pps__pb2.LokiRequest.FromString,
+                    response_serializer=python__pachyderm_dot_proto_dot_v2_dot_pps_dot_pps__pb2.LokiLogMessage.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'pps_v2.API', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -1062,7 +1096,41 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_stream(request, target, '/pps_v2.API/ListTask',
             python__pachyderm_dot_proto_dot_v2_dot_task_dot_task__pb2.ListTaskRequest.SerializeToString,
             python__pachyderm_dot_proto_dot_v2_dot_task_dot_task__pb2.TaskInfo.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetKubeEvents(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/pps_v2.API/GetKubeEvents',
+            python__pachyderm_dot_proto_dot_v2_dot_pps_dot_pps__pb2.LokiRequest.SerializeToString,
+            python__pachyderm_dot_proto_dot_v2_dot_pps_dot_pps__pb2.LokiLogMessage.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def QueryLoki(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/pps_v2.API/QueryLoki',
+            python__pachyderm_dot_proto_dot_v2_dot_pps_dot_pps__pb2.LokiRequest.SerializeToString,
+            python__pachyderm_dot_proto_dot_v2_dot_pps_dot_pps__pb2.LokiLogMessage.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/proxy/proxy_pb2.py` & `python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/proxy/proxy_pb2.py`

 * *Files identical despite different names*

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/proxy/proxy_pb2_grpc.py` & `python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/proxy/proxy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/task/task_pb2.py` & `python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/task/task_pb2.py`

 * *Files identical despite different names*

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/transaction/transaction_pb2.py` & `python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/transaction/transaction_pb2.py`

 * *Files identical despite different names*

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/transaction/transaction_pb2_grpc.py` & `python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/transaction/transaction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/version/versionpb/version_pb2.py` & `python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/version/versionpb/version_pb2.py`

 * *Files identical despite different names*

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/proto/v2/version/versionpb/version_pb2_grpc.py` & `python_pachyderm-7.5.0/src/python_pachyderm/proto/v2/version/versionpb/version_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `python-pachyderm-7.4.0rc1.dev2/src/python_pachyderm/service.py` & `python_pachyderm-7.5.0/src/python_pachyderm/service.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,16 +23,20 @@
     transaction_pb2_grpc as transaction_grpc,
 )
 from python_pachyderm.proto.v2.version.versionpb import version_pb2 as version_proto
 from python_pachyderm.proto.v2.version.versionpb import version_pb2_grpc as version_grpc
 
 MB = 1024**2
 MAX_RECEIVE_MESSAGE_SIZE = 20 * MB
+PRIMARY_USER_AGENT = "python-pachyderm"
+# SECONDARY_USER_AGENT = "v0.0.0"  # TODO: populate this programmatically
 GRPC_CHANNEL_OPTIONS = [
     ("grpc.max_receive_message_length", MAX_RECEIVE_MESSAGE_SIZE),
+    ("grpc.primary_user_agent", PRIMARY_USER_AGENT),
+    # ("grpc.secondary_user_agent", SECONDARY_USER_AGENT),
 ]
 
 
 class Service(Enum):
     ADMIN = 0
     AUTH = 1
     DEBUG = 2
```

### Comparing `python-pachyderm-7.4.0rc1.dev2/PKG-INFO` & `python_pachyderm-7.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 Metadata-Version: 2.1
 Name: python-pachyderm
-Version: 7.4.0rc1.dev2
+Version: 7.5.0
 Summary: Python Pachyderm Client
 Home-page: https://github.com/pachyderm/python-pachyderm
 License: Apache 2.0
 Keywords: pachyderm
 Author: Pachyderm Integrations
 Author-email: integrations@pachyderm.io
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Dist: betterproto (==2.0.0b4)
 Requires-Dist: grpc-interceptor (>=0.13.0,<0.14.0)
-Requires-Dist: grpcio (>=1.38.0)
+Requires-Dist: grpcio (>=1.54.2)
 Requires-Dist: grpcio-health-checking (>=1.38.0)
-Requires-Dist: importlib-metadata (>1.5.1); python_version < "3.8"
+Requires-Dist: importlib-metadata (>1.5.1) ; python_version < "3.8"
 Requires-Dist: protobuf (>=3.17.1,<4.0.0)
+Requires-Dist: python-dotenv (>=1.0.0)
 Project-URL: Documentation, https://python-pachyderm.readthedocs.io/en/stable/
 Project-URL: Repository, https://github.com/pachyderm/python-pachyderm
 Description-Content-Type: text/markdown
 
 # Python Pachyderm
 
 [![PyPI Package latest release](https://img.shields.io/pypi/v/python-pachyderm.svg)](https://pypi.python.org/pypi/python-pachyderm)
```

