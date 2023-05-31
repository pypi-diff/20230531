# Comparing `tmp/openxlab-test-0.0.2.tar.gz` & `tmp/openxlab-test-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openxlab-test-0.0.2.tar", last modified: Wed May 17 09:15:06 2023, max compression
+gzip compressed data, was "openxlab-test-0.0.3.tar", last modified: Wed May 31 11:07:09 2023, max compression
```

## Comparing `openxlab-test-0.0.2.tar` & `openxlab-test-0.0.3.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.685066 openxlab-test-0.0.2/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     4035 2023-05-17 09:15:06.684646 openxlab-test-0.0.2/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3632 2023-05-17 07:32:10.000000 openxlab-test-0.0.2/README.md
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.647626 openxlab-test-0.0.2/openxlab/
--rw-r--r--   0 alvin-pc   (501) staff       (20)       46 2023-04-10 09:49:22.000000 openxlab-test-0.0.2/openxlab/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3207 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/cli.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.649856 openxlab-test-0.0.2/openxlab/config/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 09:49:22.000000 openxlab-test-0.0.2/openxlab/config/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      331 2023-05-17 07:28:28.000000 openxlab-test-0.0.2/openxlab/config/const.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-05-17 09:14:44.000000 openxlab-test-0.0.2/openxlab/config/version.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.650470 openxlab-test-0.0.2/openxlab/demo_cmd/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1057 2023-05-17 07:28:28.000000 openxlab-test-0.0.2/openxlab/demo_cmd/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.651522 openxlab-test-0.0.2/openxlab/model/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      397 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.655874 openxlab-test-0.0.2/openxlab/model/clients/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/clients/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/clients/model_client.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     7757 2023-05-17 08:42:30.000000 openxlab-test-0.0.2/openxlab/model/clients/openapi_client.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      853 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/clients/oss_client.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1877 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/clients/upload_service_client.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.661913 openxlab-test-0.0.2/openxlab/model/commands/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      875 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/commands/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      705 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/commands/create.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1021 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/commands/download.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/commands/inference.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      541 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/commands/init.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      689 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/commands/list.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      536 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/commands/remove.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1105 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/commands/upload.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      765 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/commands/visibility.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.664738 openxlab-test-0.0.2/openxlab/model/common/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/common/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1750 2023-05-17 08:59:13.000000 openxlab-test-0.0.2/openxlab/model/common/constants.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1698 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/common/meta_file_util.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      831 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/common/response_dto.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.671193 openxlab-test-0.0.2/openxlab/model/handler/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        3 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/handler/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/handler/common.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1401 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/handler/create_repository.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     4328 2023-05-17 07:39:55.000000 openxlab-test-0.0.2/openxlab/model/handler/download_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/handler/model_inference.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       56 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/handler/model_list.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1070 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/handler/query_repo_model.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1023 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/handler/remove_repo_or_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1094 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/handler/update_repository.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3711 2023-05-17 07:28:34.000000 openxlab-test-0.0.2/openxlab/model/handler/upload_file.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.671993 openxlab-test-0.0.2/openxlab/types/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 11:25:41.000000 openxlab-test-0.0.2/openxlab/types/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      951 2023-04-10 10:02:47.000000 openxlab-test-0.0.2/openxlab/types/command_type.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.675520 openxlab-test-0.0.2/openxlab/utils/
--rw-r--r--   0 alvin-pc   (501) staff       (20)       20 2023-04-10 10:02:47.000000 openxlab-test-0.0.2/openxlab/utils/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      201 2023-05-17 07:32:10.000000 openxlab-test-0.0.2/openxlab/utils/auth.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      151 2023-05-17 07:32:10.000000 openxlab-test-0.0.2/openxlab/utils/env_util.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 openxlab-test-0.0.2/openxlab/utils/file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      688 2023-05-17 07:28:28.000000 openxlab-test-0.0.2/openxlab/utils/time_util.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.676058 openxlab-test-0.0.2/openxlab/xlab/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      488 2023-05-17 07:28:28.000000 openxlab-test-0.0.2/openxlab/xlab/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.677009 openxlab-test-0.0.2/openxlab/xlab/clients/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:28.000000 openxlab-test-0.0.2/openxlab/xlab/clients/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     2381 2023-05-17 07:32:10.000000 openxlab-test-0.0.2/openxlab/xlab/clients/auth_client.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.678042 openxlab-test-0.0.2/openxlab/xlab/commands/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:28.000000 openxlab-test-0.0.2/openxlab/xlab/commands/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      679 2023-05-17 07:28:28.000000 openxlab-test-0.0.2/openxlab/xlab/commands/config_command.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.679399 openxlab-test-0.0.2/openxlab/xlab/common/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:28.000000 openxlab-test-0.0.2/openxlab/xlab/common/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      851 2023-05-17 07:32:10.000000 openxlab-test-0.0.2/openxlab/xlab/common/response_dto.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.681641 openxlab-test-0.0.2/openxlab/xlab/handler/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-17 07:28:28.000000 openxlab-test-0.0.2/openxlab/xlab/handler/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1802 2023-05-17 07:28:28.000000 openxlab-test-0.0.2/openxlab/xlab/handler/user_config.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3883 2023-05-17 08:34:00.000000 openxlab-test-0.0.2/openxlab/xlab/handler/user_token.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-17 09:15:06.684023 openxlab-test-0.0.2/openxlab_test.egg-info/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     4035 2023-05-17 09:15:06.000000 openxlab-test-0.0.2/openxlab_test.egg-info/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)     2029 2023-05-17 09:15:06.000000 openxlab-test-0.0.2/openxlab_test.egg-info/SOURCES.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-17 09:15:06.000000 openxlab-test-0.0.2/openxlab_test.egg-info/dependency_links.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       53 2023-05-17 09:15:06.000000 openxlab-test-0.0.2/openxlab_test.egg-info/entry_points.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)      117 2023-05-17 09:15:06.000000 openxlab-test-0.0.2/openxlab_test.egg-info/requires.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        9 2023-05-17 09:15:06.000000 openxlab-test-0.0.2/openxlab_test.egg-info/top_level.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1426 2023-05-16 09:43:42.000000 openxlab-test-0.0.2/pyproject.toml
--rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-05-17 09:15:06.685166 openxlab-test-0.0.2/setup.cfg
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1183 2023-05-17 09:14:44.000000 openxlab-test-0.0.2/setup.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:07:09.850460 openxlab-test-0.0.3/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1518 2023-05-31 11:07:09.850081 openxlab-test-0.0.3/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1110 2023-05-30 12:16:34.000000 openxlab-test-0.0.3/README.md
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:07:09.819119 openxlab-test-0.0.3/openxlab/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       46 2023-04-10 09:49:22.000000 openxlab-test-0.0.3/openxlab/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3207 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/cli.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:07:09.820824 openxlab-test-0.0.3/openxlab/config/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 09:49:22.000000 openxlab-test-0.0.3/openxlab/config/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      331 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/config/const.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-05-31 11:07:07.000000 openxlab-test-0.0.3/openxlab/config/version.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:07:09.821165 openxlab-test-0.0.3/openxlab/demo_cmd/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1057 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/demo_cmd/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:07:09.821781 openxlab-test-0.0.3/openxlab/model/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      397 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/model/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:07:09.824262 openxlab-test-0.0.3/openxlab/model/clients/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-test-0.0.3/openxlab/model/clients/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-test-0.0.3/openxlab/model/clients/model_client.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     7755 2023-05-30 09:57:52.000000 openxlab-test-0.0.3/openxlab/model/clients/openapi_client.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      853 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/model/clients/oss_client.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1877 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/model/clients/upload_service_client.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:07:09.830430 openxlab-test-0.0.3/openxlab/model/commands/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      875 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/model/commands/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      705 2023-05-19 05:11:41.000000 openxlab-test-0.0.3/openxlab/model/commands/create.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1049 2023-05-30 09:23:55.000000 openxlab-test-0.0.3/openxlab/model/commands/download.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/model/commands/inference.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      541 2023-05-19 05:11:41.000000 openxlab-test-0.0.3/openxlab/model/commands/init.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      689 2023-05-19 05:11:41.000000 openxlab-test-0.0.3/openxlab/model/commands/list.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      536 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/model/commands/remove.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1105 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/model/commands/upload.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      765 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/model/commands/visibility.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:07:09.832535 openxlab-test-0.0.3/openxlab/model/common/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-test-0.0.3/openxlab/model/common/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1750 2023-05-31 09:40:34.000000 openxlab-test-0.0.3/openxlab/model/common/constants.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1698 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/model/common/meta_file_util.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      831 2023-05-19 05:11:41.000000 openxlab-test-0.0.3/openxlab/model/common/response_dto.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:07:09.838890 openxlab-test-0.0.3/openxlab/model/handler/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        3 2023-05-19 05:11:41.000000 openxlab-test-0.0.3/openxlab/model/handler/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-test-0.0.3/openxlab/model/handler/common.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1401 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/model/handler/create_repository.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     5239 2023-05-31 10:59:28.000000 openxlab-test-0.0.3/openxlab/model/handler/download_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/model/handler/model_inference.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       56 2023-05-19 05:11:41.000000 openxlab-test-0.0.3/openxlab/model/handler/model_list.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1070 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/model/handler/query_repo_model.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1023 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/model/handler/remove_repo_or_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1094 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/model/handler/update_repository.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3711 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/model/handler/upload_file.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:07:09.839714 openxlab-test-0.0.3/openxlab/types/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 11:25:41.000000 openxlab-test-0.0.3/openxlab/types/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      951 2023-04-10 10:02:47.000000 openxlab-test-0.0.3/openxlab/types/command_type.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:07:09.843157 openxlab-test-0.0.3/openxlab/utils/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       20 2023-04-10 10:02:47.000000 openxlab-test-0.0.3/openxlab/utils/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      201 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/utils/auth.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      151 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/utils/env_util.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 openxlab-test-0.0.3/openxlab/utils/file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      688 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/utils/time_util.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:07:09.843679 openxlab-test-0.0.3/openxlab/xlab/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      488 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/xlab/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:07:09.844416 openxlab-test-0.0.3/openxlab/xlab/clients/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/xlab/clients/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     2381 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/xlab/clients/auth_client.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:07:09.845150 openxlab-test-0.0.3/openxlab/xlab/commands/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/xlab/commands/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      679 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/xlab/commands/config_command.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:07:09.845922 openxlab-test-0.0.3/openxlab/xlab/common/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/xlab/common/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      851 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/xlab/common/response_dto.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:07:09.847267 openxlab-test-0.0.3/openxlab/xlab/handler/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/xlab/handler/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1802 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/openxlab/xlab/handler/user_config.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3883 2023-05-31 09:40:20.000000 openxlab-test-0.0.3/openxlab/xlab/handler/user_token.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-31 11:07:09.849616 openxlab-test-0.0.3/openxlab_test.egg-info/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1518 2023-05-31 11:07:09.000000 openxlab-test-0.0.3/openxlab_test.egg-info/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     2029 2023-05-31 11:07:09.000000 openxlab-test-0.0.3/openxlab_test.egg-info/SOURCES.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-31 11:07:09.000000 openxlab-test-0.0.3/openxlab_test.egg-info/dependency_links.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       53 2023-05-31 11:07:09.000000 openxlab-test-0.0.3/openxlab_test.egg-info/entry_points.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      117 2023-05-31 11:07:09.000000 openxlab-test-0.0.3/openxlab_test.egg-info/requires.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        9 2023-05-31 11:07:09.000000 openxlab-test-0.0.3/openxlab_test.egg-info/top_level.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1426 2023-05-19 08:42:18.000000 openxlab-test-0.0.3/pyproject.toml
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-05-31 11:07:09.850573 openxlab-test-0.0.3/setup.cfg
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1188 2023-05-31 11:05:27.000000 openxlab-test-0.0.3/setup.py
```

### Comparing `openxlab-test-0.0.2/openxlab/cli.py` & `openxlab-test-0.0.3/openxlab/cli.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/demo_cmd/__init__.py` & `openxlab-test-0.0.3/openxlab/demo_cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/model/clients/openapi_client.py` & `openxlab-test-0.0.3/openxlab/model/clients/openapi_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,29 +9,28 @@
 
 class OpenapiClient(object):
     def __init__(self, endpoint, token):
         self.endpoint = endpoint
         self.token = token
 
     # def get_dataset_files(self, dataset_name:str, prefix:str):
-    def get_download_url(self, repository, file):
+    def get_download_url(self, username, repository, model_name, filepath):
         """
         get file(model file|meta file|log file|readme file) download url
         """
         client_from = os.environ.get('CLIENT_FROM', '0')
-        payload = {"repositoryName": repository, "fileName": file, "clientFrom": client_from}
+        payload = {"userName": username, "repositoryName": repository, "modelNames": model_name, "filePaths": filepath, "clientFrom": client_from}
         path = paths['file_download_path']
         response_dto = self.http_post_response_dto(path, payload)
         if response_dto.msg_code != '10000':
             raise ValueError(f"Get download url error:{response_dto.msg}, traceId:{response_dto.trace_id}")
         if response_dto.data['msgCode'] != '10000':
             raise ValueError(f"Get download url error:{response_dto.data['msg']}, "
                              f"traceId:{response_dto.data['traceId']}")
-        return response_dto.data['data']['url'], response_dto.data['data']['fileName'], \
-            response_dto.data['data']['hash'], response_dto.data['data']['weightRawSize']
+        return response_dto.data['data']['modelNames'], response_dto.data['data']['filePaths']
 
     def get_metafile_template_download_url(self, file=None):
         """
         get metafile template download url
         """
         payload = {}
         path = paths['meta_file_template_download_path']
@@ -133,26 +132,26 @@
         if response_dto.data['msgCode'] != '10000':
             raise ValueError(f"Get upload signature error:{response_dto.data['msg']}, "
                              f"traceId:{response_dto.data['traceId']}")
         return response_dto.data['data']
 
     def http_post_response_dto(self, path, payload):
         headers = self.http_common_header()
-        print(f"headers:{headers}, body:{payload}")
+        # print(f"headers:{headers}, body:{payload}")
         response = requests.post(f"{self.endpoint}{path}", json=payload, headers=headers)
         response.raise_for_status()
         response_dict = response.json()
         response_dto = ReturnDto.from_camel_case(response_dict)
         return response_dto
 
     def http_common_header(self):
         try:
             jwt = get_jwt()
         except ValueError as e:
-            print(f"Error: {e}")
+            print(f"warning: {e}")
             return
         header_dict = {
             "Content-Type": "application/json",
             "accept": "application/json",
             "Authorization": jwt
         }
         return header_dict
```

### Comparing `openxlab-test-0.0.2/openxlab/model/clients/oss_client.py` & `openxlab-test-0.0.3/openxlab/model/clients/oss_client.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/model/clients/upload_service_client.py` & `openxlab-test-0.0.3/openxlab/model/clients/upload_service_client.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/model/commands/__init__.py` & `openxlab-test-0.0.3/openxlab/model/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/model/commands/create.py` & `openxlab-test-0.0.3/openxlab/model/commands/create.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/model/commands/download.py` & `openxlab-test-0.0.3/openxlab/model/commands/download.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,9 +18,9 @@
                             help='target file to be download.')
         parser.add_argument('-p', '--path', required=False,
                             help='setting download path.')
         parser.add_argument('-o', '--overwrite', action='store_true',
                             help='force overwriting local files.')
 
     def take_action(self, parsed_args: Namespace) -> int:
-        download(parsed_args.model_repo, parsed_args.file, parsed_args.path, parsed_args.overwrite)
+        download(parsed_args.model_repo, model_name=parsed_args.file, output=parsed_args.path, overwrite=parsed_args.overwrite)
         return 0
```

### Comparing `openxlab-test-0.0.2/openxlab/model/commands/init.py` & `openxlab-test-0.0.3/openxlab/model/commands/init.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/model/commands/list.py` & `openxlab-test-0.0.3/openxlab/model/commands/list.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/model/commands/remove.py` & `openxlab-test-0.0.3/openxlab/model/commands/remove.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/model/commands/upload.py` & `openxlab-test-0.0.3/openxlab/model/commands/upload.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/model/commands/visibility.py` & `openxlab-test-0.0.3/openxlab/model/commands/visibility.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/model/common/constants.py` & `openxlab-test-0.0.3/openxlab/model/common/constants.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/model/common/meta_file_util.py` & `openxlab-test-0.0.3/openxlab/model/common/meta_file_util.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/model/common/response_dto.py` & `openxlab-test-0.0.3/openxlab/model/common/response_dto.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/model/handler/create_repository.py` & `openxlab-test-0.0.3/openxlab/model/handler/create_repository.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/model/handler/query_repo_model.py` & `openxlab-test-0.0.3/openxlab/model/handler/query_repo_model.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/model/handler/remove_repo_or_file.py` & `openxlab-test-0.0.3/openxlab/model/handler/remove_repo_or_file.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/model/handler/update_repository.py` & `openxlab-test-0.0.3/openxlab/model/handler/update_repository.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/model/handler/upload_file.py` & `openxlab-test-0.0.3/openxlab/model/handler/upload_file.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/types/command_type.py` & `openxlab-test-0.0.3/openxlab/types/command_type.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/utils/file.py` & `openxlab-test-0.0.3/openxlab/utils/file.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/utils/time_util.py` & `openxlab-test-0.0.3/openxlab/utils/time_util.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/xlab/clients/auth_client.py` & `openxlab-test-0.0.3/openxlab/xlab/clients/auth_client.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/xlab/commands/config_command.py` & `openxlab-test-0.0.3/openxlab/xlab/commands/config_command.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/xlab/common/response_dto.py` & `openxlab-test-0.0.3/openxlab/xlab/common/response_dto.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/xlab/handler/user_config.py` & `openxlab-test-0.0.3/openxlab/xlab/handler/user_config.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab/xlab/handler/user_token.py` & `openxlab-test-0.0.3/openxlab/xlab/handler/user_token.py`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/openxlab_test.egg-info/SOURCES.txt` & `openxlab-test-0.0.3/openxlab_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/pyproject.toml` & `openxlab-test-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openxlab-test-0.0.2/setup.py` & `openxlab-test-0.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import openxlab.utils as utils
 from openxlab.config import version
 
 setup(
     name='openxlab-test',
     version=version.version,
-    description='openxlab',
+    description='openxlab-test',
     long_description= utils.get_file_content("README.md"),
     long_description_content_type='text/markdown',
     author='Openxlab Contributors',
     author_email='myname@example.com',
     keywords='openxlab,  xxxx',
     url='https://github.com/xxx/xxxx',
     packages=find_packages(exclude=('configs', 'tools', 'demo')),
```

