# Comparing `tmp/auto-test-common-1.0.1.tar.gz` & `tmp/auto-test-common-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-test-common-1.0.1.tar", last modified: Wed May 31 01:41:16 2023, max compression
+gzip compressed data, was "auto-test-common-1.0.2.tar", last modified: Wed May 31 02:36:09 2023, max compression
```

## Comparing `auto-test-common-1.0.1.tar` & `auto-test-common-1.0.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 01:41:16.071056 auto-test-common-1.0.1/
--rw-r--r--   0 edz        (502) staff       (20)      447 2023-05-31 01:41:16.071189 auto-test-common-1.0.1/PKG-INFO
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 01:41:16.041473 auto-test-common-1.0.1/auto_test_common.egg-info/
--rw-r--r--   0 edz        (502) staff       (20)      447 2023-05-31 01:41:15.000000 auto-test-common-1.0.1/auto_test_common.egg-info/PKG-INFO
--rw-r--r--   0 edz        (502) staff       (20)     1505 2023-05-31 01:41:15.000000 auto-test-common-1.0.1/auto_test_common.egg-info/SOURCES.txt
--rw-r--r--   0 edz        (502) staff       (20)        1 2023-05-31 01:41:15.000000 auto-test-common-1.0.1/auto_test_common.egg-info/dependency_links.txt
--rw-r--r--   0 edz        (502) staff       (20)       56 2023-05-31 01:41:15.000000 auto-test-common-1.0.1/auto_test_common.egg-info/entry_points.txt
--rw-r--r--   0 edz        (502) staff       (20)      571 2023-05-31 01:41:15.000000 auto-test-common-1.0.1/auto_test_common.egg-info/requires.txt
--rw-r--r--   0 edz        (502) staff       (20)        7 2023-05-31 01:41:15.000000 auto-test-common-1.0.1/auto_test_common.egg-info/top_level.txt
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 01:41:16.041926 auto-test-common-1.0.1/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-1.0.1/common/__init__.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 01:41:16.043989 auto-test-common-1.0.1/common/autotest/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-1.0.1/common/autotest/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     8490 2023-05-09 01:49:15.000000 auto-test-common-1.0.1/common/autotest/base_requests.py
--rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 auto-test-common-1.0.1/common/autotest/handle_allure.py
--rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 auto-test-common-1.0.1/common/autotest/handle_assert.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 01:41:16.046414 auto-test-common-1.0.1/common/common/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-1.0.1/common/common/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 auto-test-common-1.0.1/common/common/api_driver.py
--rw-r--r--   0 edz        (502) staff       (20)     3612 2023-05-30 05:55:54.000000 auto-test-common-1.0.1/common/common/constant.py
--rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-1.0.1/common/common/test.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 01:41:16.047267 auto-test-common-1.0.1/common/config/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.1/common/config/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 auto-test-common-1.0.1/common/config/config.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 01:41:16.049119 auto-test-common-1.0.1/common/data/
--rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-1.0.1/common/data/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    17370 2023-05-24 07:32:32.000000 auto-test-common-1.0.1/common/data/data_process.py
--rw-r--r--   0 edz        (502) staff       (20)     8641 2023-05-30 08:45:37.000000 auto-test-common-1.0.1/common/data/handle_common.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 01:41:16.053262 auto-test-common-1.0.1/common/db/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.1/common/db/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-1.0.1/common/db/handle_db.py
--rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-1.0.1/common/db/handle_db_batch.py
--rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-1.0.1/common/db/handle_mysqldb.py
--rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-1.0.1/common/db/handle_oracle.py
--rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-1.0.1/common/db/handle_sqlserver.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 01:41:16.058823 auto-test-common-1.0.1/common/file/
--rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 auto-test-common-1.0.1/common/file/ReadFile.py
--rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-1.0.1/common/file/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)    11426 2023-05-31 01:20:03.000000 auto-test-common-1.0.1/common/file/handle_excel.py
--rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-1.0.1/common/file/handle_file.py
--rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-1.0.1/common/file/handle_reques.py
--rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 auto-test-common-1.0.1/common/file/handle_system.py
--rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:00.000000 auto-test-common-1.0.1/common/file/handle_yaml.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 01:41:16.059909 auto-test-common-1.0.1/common/mq/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.1/common/mq/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-1.0.1/common/mq/handle_rabbit.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 01:41:16.064001 auto-test-common-1.0.1/common/plat/
--rw-r--r--   0 edz        (502) staff       (20)     3543 2023-05-31 01:13:42.000000 auto-test-common-1.0.1/common/plat/ATF_platform.py
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-1.0.1/common/plat/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-1.0.1/common/plat/jenkin_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     7851 2023-05-30 02:15:47.000000 auto-test-common-1.0.1/common/plat/jira_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     8129 2023-05-30 07:56:22.000000 auto-test-common-1.0.1/common/plat/mysql_platform.py
--rw-r--r--   0 edz        (502) staff       (20)     8826 2023-05-31 01:13:42.000000 auto-test-common-1.0.1/common/plat/service_platform.py
-drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 01:41:16.070717 auto-test-common-1.0.1/common/plugin/
--rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-1.0.1/common/plugin/__init__.py
--rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 auto-test-common-1.0.1/common/plugin/allure_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 auto-test-common-1.0.1/common/plugin/assert_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     8163 2023-05-24 06:58:41.000000 auto-test-common-1.0.1/common/plugin/atf_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)     6768 2023-05-15 07:47:06.000000 auto-test-common-1.0.1/common/plugin/data_bus.py
--rw-r--r--   0 edz        (502) staff       (20)     3654 2023-05-27 02:43:55.000000 auto-test-common-1.0.1/common/plugin/data_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    12175 2023-05-29 05:53:50.000000 auto-test-common-1.0.1/common/plugin/file_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-1.0.1/common/plugin/hooks_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)    13093 2023-01-16 07:46:00.000000 auto-test-common-1.0.1/common/plugin/pytest_playwright.py
--rw-r--r--   0 edz        (502) staff       (20)    17706 2023-05-31 01:26:33.000000 auto-test-common-1.0.1/common/plugin/pytest_plugin.py
--rw-r--r--   0 edz        (502) staff       (20)      443 2023-05-31 01:41:16.071827 auto-test-common-1.0.1/setup.cfg
--rw-r--r--   0 edz        (502) staff       (20)     1686 2023-05-23 02:48:09.000000 auto-test-common-1.0.1/setup.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.650002 auto-test-common-1.0.2/
+-rw-r--r--   0 edz        (502) staff       (20)      447 2023-05-31 02:36:09.650150 auto-test-common-1.0.2/PKG-INFO
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.617980 auto-test-common-1.0.2/auto_test_common.egg-info/
+-rw-r--r--   0 edz        (502) staff       (20)      447 2023-05-31 02:36:09.000000 auto-test-common-1.0.2/auto_test_common.egg-info/PKG-INFO
+-rw-r--r--   0 edz        (502) staff       (20)     1505 2023-05-31 02:36:09.000000 auto-test-common-1.0.2/auto_test_common.egg-info/SOURCES.txt
+-rw-r--r--   0 edz        (502) staff       (20)        1 2023-05-31 02:36:09.000000 auto-test-common-1.0.2/auto_test_common.egg-info/dependency_links.txt
+-rw-r--r--   0 edz        (502) staff       (20)       56 2023-05-31 02:36:09.000000 auto-test-common-1.0.2/auto_test_common.egg-info/entry_points.txt
+-rw-r--r--   0 edz        (502) staff       (20)      571 2023-05-31 02:36:09.000000 auto-test-common-1.0.2/auto_test_common.egg-info/requires.txt
+-rw-r--r--   0 edz        (502) staff       (20)        7 2023-05-31 02:36:09.000000 auto-test-common-1.0.2/auto_test_common.egg-info/top_level.txt
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.618414 auto-test-common-1.0.2/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:32:00.000000 auto-test-common-1.0.2/common/__init__.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.620716 auto-test-common-1.0.2/common/autotest/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:59:00.000000 auto-test-common-1.0.2/common/autotest/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     8490 2023-05-09 01:49:15.000000 auto-test-common-1.0.2/common/autotest/base_requests.py
+-rw-r--r--   0 edz        (502) staff       (20)     6429 2023-03-22 09:11:00.000000 auto-test-common-1.0.2/common/autotest/handle_allure.py
+-rw-r--r--   0 edz        (502) staff       (20)    10703 2023-04-14 00:29:00.000000 auto-test-common-1.0.2/common/autotest/handle_assert.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.623235 auto-test-common-1.0.2/common/common/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 03:00:00.000000 auto-test-common-1.0.2/common/common/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2126 2023-04-23 02:46:40.000000 auto-test-common-1.0.2/common/common/api_driver.py
+-rw-r--r--   0 edz        (502) staff       (20)     3612 2023-05-30 05:55:54.000000 auto-test-common-1.0.2/common/common/constant.py
+-rw-r--r--   0 edz        (502) staff       (20)     1763 2023-04-14 00:29:00.000000 auto-test-common-1.0.2/common/common/test.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.624222 auto-test-common-1.0.2/common/config/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.2/common/config/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2429 2022-12-01 00:35:00.000000 auto-test-common-1.0.2/common/config/config.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.626770 auto-test-common-1.0.2/common/data/
+-rw-r--r--   0 edz        (502) staff       (20)       28 2022-03-29 12:15:00.000000 auto-test-common-1.0.2/common/data/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    17370 2023-05-24 07:32:32.000000 auto-test-common-1.0.2/common/data/data_process.py
+-rw-r--r--   0 edz        (502) staff       (20)     8641 2023-05-30 08:45:37.000000 auto-test-common-1.0.2/common/data/handle_common.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.631475 auto-test-common-1.0.2/common/db/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.2/common/db/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     3592 2023-05-15 07:43:20.000000 auto-test-common-1.0.2/common/db/handle_db.py
+-rw-r--r--   0 edz        (502) staff       (20)     1345 2022-12-13 01:35:00.000000 auto-test-common-1.0.2/common/db/handle_db_batch.py
+-rw-r--r--   0 edz        (502) staff       (20)     1223 2023-04-14 00:29:00.000000 auto-test-common-1.0.2/common/db/handle_mysqldb.py
+-rw-r--r--   0 edz        (502) staff       (20)     1533 2023-04-14 00:29:00.000000 auto-test-common-1.0.2/common/db/handle_oracle.py
+-rw-r--r--   0 edz        (502) staff       (20)     1665 2023-04-14 00:29:00.000000 auto-test-common-1.0.2/common/db/handle_sqlserver.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.637407 auto-test-common-1.0.2/common/file/
+-rw-r--r--   0 edz        (502) staff       (20)     4508 2023-04-14 00:29:00.000000 auto-test-common-1.0.2/common/file/ReadFile.py
+-rw-r--r--   0 edz        (502) staff       (20)       41 2022-03-29 11:09:00.000000 auto-test-common-1.0.2/common/file/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)    11426 2023-05-31 01:20:03.000000 auto-test-common-1.0.2/common/file/handle_excel.py
+-rw-r--r--   0 edz        (502) staff       (20)     2265 2023-05-25 07:52:43.000000 auto-test-common-1.0.2/common/file/handle_file.py
+-rw-r--r--   0 edz        (502) staff       (20)     1364 2023-04-14 00:29:00.000000 auto-test-common-1.0.2/common/file/handle_reques.py
+-rw-r--r--   0 edz        (502) staff       (20)     2201 2022-10-24 01:09:00.000000 auto-test-common-1.0.2/common/file/handle_system.py
+-rw-r--r--   0 edz        (502) staff       (20)     1000 2023-04-14 00:29:00.000000 auto-test-common-1.0.2/common/file/handle_yaml.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.638580 auto-test-common-1.0.2/common/mq/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-29 02:29:00.000000 auto-test-common-1.0.2/common/mq/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     2059 2023-04-14 00:29:00.000000 auto-test-common-1.0.2/common/mq/handle_rabbit.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.642858 auto-test-common-1.0.2/common/plat/
+-rw-r--r--   0 edz        (502) staff       (20)     3543 2023-05-31 01:13:42.000000 auto-test-common-1.0.2/common/plat/ATF_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-04-16 11:02:00.000000 auto-test-common-1.0.2/common/plat/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1384 2022-04-27 12:06:00.000000 auto-test-common-1.0.2/common/plat/jenkin_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     7851 2023-05-30 02:15:47.000000 auto-test-common-1.0.2/common/plat/jira_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     8129 2023-05-30 07:56:22.000000 auto-test-common-1.0.2/common/plat/mysql_platform.py
+-rw-r--r--   0 edz        (502) staff       (20)     8826 2023-05-31 01:13:42.000000 auto-test-common-1.0.2/common/plat/service_platform.py
+drwxr-xr-x   0 edz        (502) staff       (20)        0 2023-05-31 02:36:09.649588 auto-test-common-1.0.2/common/plugin/
+-rw-r--r--   0 edz        (502) staff       (20)        0 2022-03-31 18:00:00.000000 auto-test-common-1.0.2/common/plugin/__init__.py
+-rw-r--r--   0 edz        (502) staff       (20)     1330 2023-01-16 07:33:00.000000 auto-test-common-1.0.2/common/plugin/allure_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     2054 2022-07-28 02:48:00.000000 auto-test-common-1.0.2/common/plugin/assert_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     8348 2023-05-31 02:31:39.000000 auto-test-common-1.0.2/common/plugin/atf_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)     6768 2023-05-15 07:47:06.000000 auto-test-common-1.0.2/common/plugin/data_bus.py
+-rw-r--r--   0 edz        (502) staff       (20)     3654 2023-05-27 02:43:55.000000 auto-test-common-1.0.2/common/plugin/data_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    12175 2023-05-29 05:53:50.000000 auto-test-common-1.0.2/common/plugin/file_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      904 2022-03-31 14:08:00.000000 auto-test-common-1.0.2/common/plugin/hooks_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)    13093 2023-01-16 07:46:00.000000 auto-test-common-1.0.2/common/plugin/pytest_playwright.py
+-rw-r--r--   0 edz        (502) staff       (20)    17708 2023-05-31 02:35:10.000000 auto-test-common-1.0.2/common/plugin/pytest_plugin.py
+-rw-r--r--   0 edz        (502) staff       (20)      443 2023-05-31 02:36:09.650855 auto-test-common-1.0.2/setup.cfg
+-rw-r--r--   0 edz        (502) staff       (20)     1686 2023-05-23 02:48:09.000000 auto-test-common-1.0.2/setup.py
```

### Comparing `auto-test-common-1.0.1/auto_test_common.egg-info/SOURCES.txt` & `auto-test-common-1.0.2/auto_test_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/auto_test_common.egg-info/requires.txt` & `auto-test-common-1.0.2/auto_test_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/autotest/base_requests.py` & `auto-test-common-1.0.2/common/autotest/base_requests.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/autotest/handle_allure.py` & `auto-test-common-1.0.2/common/autotest/handle_allure.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/autotest/handle_assert.py` & `auto-test-common-1.0.2/common/autotest/handle_assert.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/common/api_driver.py` & `auto-test-common-1.0.2/common/common/api_driver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/common/constant.py` & `auto-test-common-1.0.2/common/common/constant.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/common/test.py` & `auto-test-common-1.0.2/common/common/test.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/config/config.py` & `auto-test-common-1.0.2/common/config/config.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/data/data_process.py` & `auto-test-common-1.0.2/common/data/data_process.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/data/handle_common.py` & `auto-test-common-1.0.2/common/data/handle_common.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/db/handle_db.py` & `auto-test-common-1.0.2/common/db/handle_db.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/db/handle_db_batch.py` & `auto-test-common-1.0.2/common/db/handle_db_batch.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/db/handle_mysqldb.py` & `auto-test-common-1.0.2/common/db/handle_mysqldb.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/db/handle_oracle.py` & `auto-test-common-1.0.2/common/db/handle_oracle.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/db/handle_sqlserver.py` & `auto-test-common-1.0.2/common/db/handle_sqlserver.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/file/ReadFile.py` & `auto-test-common-1.0.2/common/file/ReadFile.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/file/handle_excel.py` & `auto-test-common-1.0.2/common/file/handle_excel.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/file/handle_file.py` & `auto-test-common-1.0.2/common/file/handle_file.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/file/handle_reques.py` & `auto-test-common-1.0.2/common/file/handle_reques.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/file/handle_system.py` & `auto-test-common-1.0.2/common/file/handle_system.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/file/handle_yaml.py` & `auto-test-common-1.0.2/common/file/handle_yaml.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/mq/handle_rabbit.py` & `auto-test-common-1.0.2/common/mq/handle_rabbit.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/plat/ATF_platform.py` & `auto-test-common-1.0.2/common/plat/ATF_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/plat/jenkin_platform.py` & `auto-test-common-1.0.2/common/plat/jenkin_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/plat/jira_platform.py` & `auto-test-common-1.0.2/common/plat/jira_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/plat/mysql_platform.py` & `auto-test-common-1.0.2/common/plat/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/plat/service_platform.py` & `auto-test-common-1.0.2/common/plat/service_platform.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/plugin/allure_plugin.py` & `auto-test-common-1.0.2/common/plugin/allure_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/plugin/assert_plugin.py` & `auto-test-common-1.0.2/common/plugin/assert_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/plugin/atf_plugin.py` & `auto-test-common-1.0.2/common/plugin/atf_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,14 +158,20 @@
 
 
 
 
 
 
 
+if __name__ == '__main__':
+    _summary=FilePlugin.load_json("aa.json")
+    print( DataProcess.getDate(int(str(DataPlugin.get_data_jpath(_summary, "$.time.start")).strip()) / 1000))
+
+
+
```

### Comparing `auto-test-common-1.0.1/common/plugin/data_bus.py` & `auto-test-common-1.0.2/common/plugin/data_bus.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/plugin/data_plugin.py` & `auto-test-common-1.0.2/common/plugin/data_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/plugin/file_plugin.py` & `auto-test-common-1.0.2/common/plugin/file_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/plugin/hooks_plugin.py` & `auto-test-common-1.0.2/common/plugin/hooks_plugin.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/plugin/pytest_playwright.py` & `auto-test-common-1.0.2/common/plugin/pytest_playwright.py`

 * *Files identical despite different names*

### Comparing `auto-test-common-1.0.1/common/plugin/pytest_plugin.py` & `auto-test-common-1.0.2/common/plugin/pytest_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         if get_system_key(Constant.ALLURE_PATH) is not None:
             ALLURE_PATH = get_system_key(Constant.ALLURE_PATH)
         else:
             ALLURE_PATH = ''
         if DataProcess.isNotNull(get_system_key(Constant.RUN_TYPE)) == False:
             os.system(f'{ALLURE_PATH}allure generate {TEST_TARGET_RESULTS_PATH} -o {TEST_TARGET_REPORT_PATH} --clean')
             logger.success('Allure测试报告已生成')
-        ATFPlugin.sendResult()
+        # ATFPlugin.sendResult()
 
     @classmethod
     def change_allure_title(cls,report_html_path: str = TEST_TARGET_REPORT_PATH):
         """
         修改Allure标题
         :param name: 
         :param report_html_path:
```

### Comparing `auto-test-common-1.0.1/setup.py` & `auto-test-common-1.0.2/setup.py`

 * *Files identical despite different names*

