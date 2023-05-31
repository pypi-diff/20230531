# Comparing `tmp/je_api_testka_dev-0.0.91.tar.gz` & `tmp/je_api_testka_dev-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_api_testka_dev-0.0.91.tar", last modified: Wed May 31 05:43:00 2023, max compression
+gzip compressed data, was "je_api_testka_dev-0.0.92.tar", last modified: Wed May 31 06:07:50 2023, max compression
```

## Comparing `je_api_testka_dev-0.0.91.tar` & `je_api_testka_dev-0.0.92.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.734224 je_api_testka_dev-0.0.91/
--rw-rw-rw-   0        0        0     3074 2023-05-31 05:43:00.732269 je_api_testka_dev-0.0.91/PKG-INFO
--rw-rw-rw-   0        0        0     2270 2023-05-30 02:10:25.000000 je_api_testka_dev-0.0.91/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.517528 je_api_testka_dev-0.0.91/je_api_testka/
--rw-rw-rw-   0        0        0     2957 2023-05-31 05:32:44.000000 je_api_testka_dev-0.0.91/je_api_testka/__init__.py
--rw-rw-rw-   0        0        0     2349 2023-04-25 09:07:47.000000 je_api_testka_dev-0.0.91/je_api_testka/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.534587 je_api_testka_dev-0.0.91/je_api_testka/requests_wrapper/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/requests_wrapper/__init__.py
--rw-rw-rw-   0        0        0     5026 2023-04-18 02:35:49.000000 je_api_testka_dev-0.0.91/je_api_testka/requests_wrapper/request_method.py
--rw-rw-rw-   0        0        0     2615 2023-04-18 02:35:49.000000 je_api_testka_dev-0.0.91/je_api_testka/requests_wrapper/requests_http_method_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.539741 je_api_testka_dev-0.0.91/je_api_testka/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.547743 je_api_testka_dev-0.0.91/je_api_testka/utils/assert_result/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/assert_result/__init__.py
--rw-rw-rw-   0        0        0      942 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/assert_result/result_check.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.554788 je_api_testka_dev-0.0.91/je_api_testka/utils/callback/
--rw-rw-rw-   0        0        0        0 2023-03-31 09:04:52.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/callback/__init__.py
--rw-rw-rw-   0        0        0     3497 2023-05-29 03:22:33.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/callback/callback_function_executor.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.569791 je_api_testka_dev-0.0.91/je_api_testka/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     3393 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0     2392 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.576789 je_api_testka_dev-0.0.91/je_api_testka/utils/executor/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/executor/__init__.py
--rw-rw-rw-   0        0        0     5456 2023-05-29 03:21:49.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/executor/action_executor.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.585807 je_api_testka_dev-0.0.91/je_api_testka/utils/file_process/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0      709 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.599287 je_api_testka_dev-0.0.91/je_api_testka/utils/generate_report/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/generate_report/__init__.py
--rw-rw-rw-   0        0        0     9028 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/generate_report/html_report_generate.py
--rw-rw-rw-   0        0        0     4017 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/generate_report/json_report.py
--rw-rw-rw-   0        0        0     1688 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/generate_report/xml_report.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.611527 je_api_testka_dev-0.0.91/je_api_testka/utils/get_data_strcture/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/get_data_strcture/__init__.py
--rw-rw-rw-   0        0        0     1588 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/get_data_strcture/get_api_data.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.615527 je_api_testka_dev-0.0.91/je_api_testka/utils/json/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/json/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.621564 je_api_testka_dev-0.0.91/je_api_testka/utils/json/json_file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/json/json_file/__init__.py
--rw-rw-rw-   0        0        0     1353 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/json/json_file/json_file.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.628528 je_api_testka_dev-0.0.91/je_api_testka/utils/json/json_format/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/json/json_format/__init__.py
--rw-rw-rw-   0        0        0     1300 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/json/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.635529 je_api_testka_dev-0.0.91/je_api_testka/utils/mock_server/
--rw-rw-rw-   0        0        0        0 2023-04-21 01:03:22.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/mock_server/__init__.py
--rw-rw-rw-   0        0        0     1479 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/mock_server/flask_mock_server.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.639524 je_api_testka_dev-0.0.91/je_api_testka/utils/package_manager/
--rw-rw-rw-   0        0        0        0 2023-04-06 01:01:22.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/package_manager/__init__.py
--rw-rw-rw-   0        0        0     3346 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.645553 je_api_testka_dev-0.0.91/je_api_testka/utils/project/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/project/__init__.py
--rw-rw-rw-   0        0        0     2982 2023-04-18 02:25:34.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/project/create_project_structure.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.659557 je_api_testka_dev-0.0.91/je_api_testka/utils/project/template/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/project/template/__init__.py
--rw-rw-rw-   0        0        0      633 2023-04-17 08:42:18.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/project/template/template_executor.py
--rw-rw-rw-   0        0        0      633 2023-04-17 08:52:06.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/project/template/template_keyword.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.667198 je_api_testka_dev-0.0.91/je_api_testka/utils/scheduler/
--rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/scheduler/__init__.py
--rw-rw-rw-   0        0        0     5280 2023-05-31 05:41:42.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/scheduler/extend_apscheduler.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.673198 je_api_testka_dev-0.0.91/je_api_testka/utils/socket_server/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/socket_server/__init__.py
--rw-rw-rw-   0        0        0     2490 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/socket_server/api_testka_socket_server.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.679311 je_api_testka_dev-0.0.91/je_api_testka/utils/test_record/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/test_record/__init__.py
--rw-rw-rw-   0        0        0      389 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/test_record/test_record_class.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.683201 je_api_testka_dev-0.0.91/je_api_testka/utils/xml/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/xml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.688822 je_api_testka_dev-0.0.91/je_api_testka/utils/xml/change_xml_structure/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/xml/change_xml_structure/__init__.py
--rw-rw-rw-   0        0        0     2513 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.699011 je_api_testka_dev-0.0.91/je_api_testka/utils/xml/xml_file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/xml/xml_file/__init__.py
--rw-rw-rw-   0        0        0     2424 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/xml/xml_file/xml_file.py
-drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.729232 je_api_testka_dev-0.0.91/je_api_testka_dev.egg-info/
--rw-rw-rw-   0        0        0     3074 2023-05-31 05:43:00.000000 je_api_testka_dev-0.0.91/je_api_testka_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2549 2023-05-31 05:43:00.000000 je_api_testka_dev-0.0.91/je_api_testka_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 05:43:00.000000 je_api_testka_dev-0.0.91/je_api_testka_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-31 05:43:00.000000 je_api_testka_dev-0.0.91/je_api_testka_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-31 05:43:00.000000 je_api_testka_dev-0.0.91/je_api_testka_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1170 2023-05-31 05:42:36.000000 je_api_testka_dev-0.0.91/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 05:43:00.734224 je_api_testka_dev-0.0.91/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.667583 je_api_testka_dev-0.0.92/
+-rw-rw-rw-   0        0        0     3074 2023-05-31 06:07:50.666583 je_api_testka_dev-0.0.92/PKG-INFO
+-rw-rw-rw-   0        0        0     2270 2023-05-30 02:10:25.000000 je_api_testka_dev-0.0.92/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.479880 je_api_testka_dev-0.0.92/je_api_testka/
+-rw-rw-rw-   0        0        0     2957 2023-05-31 05:32:44.000000 je_api_testka_dev-0.0.92/je_api_testka/__init__.py
+-rw-rw-rw-   0        0        0     2349 2023-04-25 09:07:47.000000 je_api_testka_dev-0.0.92/je_api_testka/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.487907 je_api_testka_dev-0.0.92/je_api_testka/requests_wrapper/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/requests_wrapper/__init__.py
+-rw-rw-rw-   0        0        0     5026 2023-04-18 02:35:49.000000 je_api_testka_dev-0.0.92/je_api_testka/requests_wrapper/request_method.py
+-rw-rw-rw-   0        0        0     2615 2023-04-18 02:35:49.000000 je_api_testka_dev-0.0.92/je_api_testka/requests_wrapper/requests_http_method_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.491905 je_api_testka_dev-0.0.92/je_api_testka/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.496966 je_api_testka_dev-0.0.92/je_api_testka/utils/assert_result/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/assert_result/__init__.py
+-rw-rw-rw-   0        0        0      942 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/assert_result/result_check.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.502905 je_api_testka_dev-0.0.92/je_api_testka/utils/callback/
+-rw-rw-rw-   0        0        0        0 2023-03-31 09:04:52.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/callback/__init__.py
+-rw-rw-rw-   0        0        0     3497 2023-05-29 03:22:33.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/callback/callback_function_executor.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.512681 je_api_testka_dev-0.0.92/je_api_testka/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     3393 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0     2392 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.521729 je_api_testka_dev-0.0.92/je_api_testka/utils/executor/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/executor/__init__.py
+-rw-rw-rw-   0        0        0     5456 2023-05-29 03:21:49.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/executor/action_executor.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.526858 je_api_testka_dev-0.0.92/je_api_testka/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0      709 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.539047 je_api_testka_dev-0.0.92/je_api_testka/utils/generate_report/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/generate_report/__init__.py
+-rw-rw-rw-   0        0        0     9028 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/generate_report/html_report_generate.py
+-rw-rw-rw-   0        0        0     4017 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/generate_report/json_report.py
+-rw-rw-rw-   0        0        0     1688 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/generate_report/xml_report.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.545046 je_api_testka_dev-0.0.92/je_api_testka/utils/get_data_strcture/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/get_data_strcture/__init__.py
+-rw-rw-rw-   0        0        0     1588 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/get_data_strcture/get_api_data.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.548046 je_api_testka_dev-0.0.92/je_api_testka/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/json/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.553132 je_api_testka_dev-0.0.92/je_api_testka/utils/json/json_file/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/json/json_file/__init__.py
+-rw-rw-rw-   0        0        0     1353 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/json/json_file/json_file.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.559050 je_api_testka_dev-0.0.92/je_api_testka/utils/json/json_format/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/json/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1300 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/json/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.565056 je_api_testka_dev-0.0.92/je_api_testka/utils/mock_server/
+-rw-rw-rw-   0        0        0        0 2023-04-21 01:03:22.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/mock_server/__init__.py
+-rw-rw-rw-   0        0        0     1479 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/mock_server/flask_mock_server.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.570140 je_api_testka_dev-0.0.92/je_api_testka/utils/package_manager/
+-rw-rw-rw-   0        0        0        0 2023-04-06 01:01:22.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/package_manager/__init__.py
+-rw-rw-rw-   0        0        0     3346 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/package_manager/package_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.576051 je_api_testka_dev-0.0.92/je_api_testka/utils/project/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/project/__init__.py
+-rw-rw-rw-   0        0        0     2982 2023-04-18 02:25:34.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/project/create_project_structure.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.585618 je_api_testka_dev-0.0.92/je_api_testka/utils/project/template/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/project/template/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-04-17 08:42:18.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/project/template/template_executor.py
+-rw-rw-rw-   0        0        0      633 2023-04-17 08:52:06.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/project/template/template_keyword.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.596571 je_api_testka_dev-0.0.92/je_api_testka/utils/scheduler/
+-rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/scheduler/__init__.py
+-rw-rw-rw-   0        0        0     6250 2023-05-31 06:04:47.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/scheduler/extend_apscheduler.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.602574 je_api_testka_dev-0.0.92/je_api_testka/utils/socket_server/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/socket_server/__init__.py
+-rw-rw-rw-   0        0        0     2490 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/socket_server/api_testka_socket_server.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.609577 je_api_testka_dev-0.0.92/je_api_testka/utils/test_record/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/test_record/__init__.py
+-rw-rw-rw-   0        0        0      389 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/test_record/test_record_class.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.612659 je_api_testka_dev-0.0.92/je_api_testka/utils/xml/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/xml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.618572 je_api_testka_dev-0.0.92/je_api_testka/utils/xml/change_xml_structure/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/xml/change_xml_structure/__init__.py
+-rw-rw-rw-   0        0        0     2513 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.626672 je_api_testka_dev-0.0.92/je_api_testka/utils/xml/xml_file/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/xml/xml_file/__init__.py
+-rw-rw-rw-   0        0        0     2424 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.92/je_api_testka/utils/xml/xml_file/xml_file.py
+drwxrwxrwx   0        0        0        0 2023-05-31 06:07:50.662573 je_api_testka_dev-0.0.92/je_api_testka_dev.egg-info/
+-rw-rw-rw-   0        0        0     3074 2023-05-31 06:07:50.000000 je_api_testka_dev-0.0.92/je_api_testka_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2549 2023-05-31 06:07:50.000000 je_api_testka_dev-0.0.92/je_api_testka_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 06:07:50.000000 je_api_testka_dev-0.0.92/je_api_testka_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-31 06:07:50.000000 je_api_testka_dev-0.0.92/je_api_testka_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-31 06:07:50.000000 je_api_testka_dev-0.0.92/je_api_testka_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1170 2023-05-31 06:07:28.000000 je_api_testka_dev-0.0.92/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 06:07:50.668581 je_api_testka_dev-0.0.92/setup.cfg
```

### Comparing `je_api_testka_dev-0.0.91/PKG-INFO` & `je_api_testka_dev-0.0.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je_api_testka_dev
-Version: 0.0.91
+Version: 0.0.92
 Summary: Requests Automation Framework
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/APITestka
 Project-URL: Documentation, https://apitestka.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/APITestka
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_api_testka_dev-0.0.91/README.md` & `je_api_testka_dev-0.0.92/README.md`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/__init__.py` & `je_api_testka_dev-0.0.92/je_api_testka/__init__.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/__main__.py` & `je_api_testka_dev-0.0.92/je_api_testka/__main__.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/requests_wrapper/request_method.py` & `je_api_testka_dev-0.0.92/je_api_testka/requests_wrapper/request_method.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/requests_wrapper/requests_http_method_wrapper.py` & `je_api_testka_dev-0.0.92/je_api_testka/requests_wrapper/requests_http_method_wrapper.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/utils/assert_result/result_check.py` & `je_api_testka_dev-0.0.92/je_api_testka/utils/assert_result/result_check.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/utils/callback/callback_function_executor.py` & `je_api_testka_dev-0.0.92/je_api_testka/utils/callback/callback_function_executor.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/utils/exception/exception_tags.py` & `je_api_testka_dev-0.0.92/je_api_testka/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/utils/exception/exceptions.py` & `je_api_testka_dev-0.0.92/je_api_testka/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/utils/executor/action_executor.py` & `je_api_testka_dev-0.0.92/je_api_testka/utils/executor/action_executor.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/utils/file_process/get_dir_file_list.py` & `je_api_testka_dev-0.0.92/je_api_testka/utils/file_process/get_dir_file_list.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/utils/generate_report/html_report_generate.py` & `je_api_testka_dev-0.0.92/je_api_testka/utils/generate_report/html_report_generate.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/utils/generate_report/json_report.py` & `je_api_testka_dev-0.0.92/je_api_testka/utils/generate_report/json_report.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/utils/generate_report/xml_report.py` & `je_api_testka_dev-0.0.92/je_api_testka/utils/generate_report/xml_report.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/utils/get_data_strcture/get_api_data.py` & `je_api_testka_dev-0.0.92/je_api_testka/utils/get_data_strcture/get_api_data.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/utils/json/json_file/json_file.py` & `je_api_testka_dev-0.0.92/je_api_testka/utils/json/json_file/json_file.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/utils/json/json_format/json_process.py` & `je_api_testka_dev-0.0.92/je_api_testka/utils/json/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/utils/mock_server/flask_mock_server.py` & `je_api_testka_dev-0.0.92/je_api_testka/utils/mock_server/flask_mock_server.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/utils/package_manager/package_manager_class.py` & `je_api_testka_dev-0.0.92/je_api_testka/utils/package_manager/package_manager_class.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/utils/project/create_project_structure.py` & `je_api_testka_dev-0.0.92/je_api_testka/utils/project/create_project_structure.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/utils/project/template/template_executor.py` & `je_api_testka_dev-0.0.92/je_api_testka/utils/project/template/template_executor.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/utils/project/template/template_keyword.py` & `je_api_testka_dev-0.0.92/je_api_testka/utils/project/template/template_keyword.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/utils/scheduler/extend_apscheduler.py` & `je_api_testka_dev-0.0.92/je_api_testka/utils/scheduler/extend_apscheduler.py`

 * *Files 20% similar despite different names*

```diff
@@ -44,52 +44,80 @@
         self._background_schedulers.start(*args, **kwargs)
 
     def start_all_scheduler(self, *args, **kwargs):
         self._blocking_schedulers.start(*args, **kwargs)
         self._background_schedulers.start(*args, **kwargs)
 
     def add_interval_blocking_secondly(
-            self, function: Callable, id: str = None, args: list = None, kwargs: dict = None, seconds: int = 1):
-        self.add_blocking_job(func=function, trigger="interval", id=id, args=args, kwargs=kwargs, seconds=seconds)
+            self, function: Callable, id: str = None, args: list = None,
+            kwargs: dict = None, seconds: int = 1, **trigger_args):
+        self.add_blocking_job(
+            func=function, trigger="interval", id=id, args=args, kwargs=kwargs, seconds=seconds, **trigger_args)
 
     def add_interval_blocking_minutely(
-            self, function: Callable, id: str = None, args: list = None, kwargs: dict = None, minutes: int = 1):
-        self.add_blocking_job(func=function, trigger="interval", id=id, args=args, kwargs=kwargs, minutes=minutes)
+            self, function: Callable, id: str = None, args: list = None,
+            kwargs: dict = None, minutes: int = 1, **trigger_args):
+        self.add_blocking_job(
+            func=function, trigger="interval", id=id, args=args, kwargs=kwargs, minutes=minutes, **trigger_args)
 
     def add_interval_blocking_hourly(
-            self, function: Callable, id: str = None, args: list = None, kwargs: dict = None, hours: int = 1):
-        self.add_blocking_job(func=function, trigger="interval", id=id, args=args, kwargs=kwargs, hours=hours)
+            self, function: Callable, id: str = None, args: list = None,
+            kwargs: dict = None, hours: int = 1, **trigger_args):
+        self.add_blocking_job(
+            func=function, trigger="interval", id=id, args=args, kwargs=kwargs, hours=hours, **trigger_args)
 
     def add_interval_blocking_daily(
-            self, function: Callable, id: str = None, args: list = None, kwargs: dict = None, days: int = 1):
-        self.add_blocking_job(func=function, trigger="interval", id=id, args=args, kwargs=kwargs, days=days)
+            self, function: Callable, id: str = None, args: list = None,
+            kwargs: dict = None, days: int = 1, **trigger_args):
+        self.add_blocking_job(
+            func=function, trigger="interval", id=id, args=args, kwargs=kwargs, days=days, **trigger_args)
 
     def add_interval_blocking_weekly(
-            self, function: Callable, id: str = None, args: list = None, kwargs: dict = None, weeks: int = 1):
-        self.add_blocking_job(func=function, trigger="interval", id=id, args=args, kwargs=kwargs, weeks=weeks)
+            self, function: Callable, id: str = None, args: list = None,
+            kwargs: dict = None, weeks: int = 1, **trigger_args):
+        self.add_blocking_job(
+            func=function, trigger="interval", id=id, args=args, kwargs=kwargs, weeks=weeks, **trigger_args)
 
     def add_interval_nonblocking_secondly(
-            self, function: Callable, id: str = None, args: list = None, kwargs: dict = None, seconds: int = 1):
-        self.add_nonblocking_job(func=function, trigger="interval", id=id, args=args, kwargs=kwargs, seconds=seconds)
+            self, function: Callable, id: str = None, args: list = None,
+            kwargs: dict = None, seconds: int = 1, **trigger_args):
+        self.add_nonblocking_job(
+            func=function, trigger="interval", id=id, args=args, kwargs=kwargs, seconds=seconds, **trigger_args)
 
     def add_interval_nonblocking_minutely(
-            self, function: Callable, id: str = None, args: list = None, kwargs: dict = None, minutes: int = 1):
-        self.add_nonblocking_job(func=function, trigger="interval", id=id, args=args, kwargs=kwargs, minutes=minutes)
+            self, function: Callable, id: str = None, args: list = None,
+            kwargs: dict = None, minutes: int = 1, **trigger_args):
+        self.add_nonblocking_job(
+            func=function, trigger="interval", id=id, args=args, kwargs=kwargs, minutes=minutes, **trigger_args)
 
     def add_interval_nonblocking_hourly(
-            self, function: Callable, id: str = None, args: list = None, kwargs: dict = None, hours: int = 1):
-        self.add_nonblocking_job(func=function, trigger="interval", id=id, args=args, kwargs=kwargs, hours=hours)
+            self, function: Callable, id: str = None, args: list = None,
+            kwargs: dict = None, hours: int = 1, **trigger_args):
+        self.add_nonblocking_job(
+            func=function, trigger="interval", id=id, args=args, kwargs=kwargs, hours=hours, **trigger_args)
 
     def add_interval_nonblocking_daily(
-            self, function: Callable, id: str = None, args: list = None, kwargs: dict = None, days: int = 1):
-        self.add_nonblocking_job(func=function, trigger="interval", id=id, args=args, kwargs=kwargs, days=days)
+            self, function: Callable, id: str = None, args: list = None,
+            kwargs: dict = None, days: int = 1, **trigger_args):
+        self.add_nonblocking_job(
+            func=function, trigger="interval", id=id, args=args, kwargs=kwargs, days=days, **trigger_args)
 
     def add_interval_nonblocking_weekly(
-            self, function: Callable, id: str = None, args: list = None, kwargs: dict = None, weeks: int = 1):
-        self.add_nonblocking_job(func=function, trigger="interval", id=id, args=args, kwargs=kwargs, weeks=weeks)
+            self, function: Callable, id: str = None, args: list = None,
+            kwargs: dict = None, weeks: int = 1, **trigger_args):
+        self.add_nonblocking_job(
+            func=function, trigger="interval", id=id, args=args, kwargs=kwargs, weeks=weeks, **trigger_args)
+
+    def add_cron_blocking(
+            self, function: Callable, id: str = None, **trigger_args):
+        self.add_blocking_job(func=function, id=id, trigger="cron", **trigger_args)
+
+    def add_cron_nonblocking(
+            self, function: Callable, id: str = None, **trigger_args):
+        self.add_nonblocking_job(func=function, id=id, trigger="cron", **trigger_args)
 
     def remove_blocking_job(self, id: str, jobstore: str = 'default'):
         self._blocking_schedulers.remove_job(job_id=id, jobstore=jobstore)
 
     def remove_nonblocking_job(self, id: str, jobstore: str = 'default'):
         self._background_schedulers.remove_job(job_id=id, jobstore=jobstore)
```

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/utils/socket_server/api_testka_socket_server.py` & `je_api_testka_dev-0.0.92/je_api_testka/utils/socket_server/api_testka_socket_server.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py` & `je_api_testka_dev-0.0.92/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka/utils/xml/xml_file/xml_file.py` & `je_api_testka_dev-0.0.92/je_api_testka/utils/xml/xml_file/xml_file.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/je_api_testka_dev.egg-info/PKG-INFO` & `je_api_testka_dev-0.0.92/je_api_testka_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je-api-testka-dev
-Version: 0.0.91
+Version: 0.0.92
 Summary: Requests Automation Framework
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/APITestka
 Project-URL: Documentation, https://apitestka.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/APITestka
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `je_api_testka_dev-0.0.91/je_api_testka_dev.egg-info/SOURCES.txt` & `je_api_testka_dev-0.0.92/je_api_testka_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.91/pyproject.toml` & `je_api_testka_dev-0.0.92/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "je_api_testka_dev"
-version = "0.0.91"
+version = "0.0.92"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 description = "Requests Automation Framework"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 dependencies = [
```

