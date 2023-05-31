# Comparing `tmp/je_api_testka_dev-0.0.90.tar.gz` & `tmp/je_api_testka_dev-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "je_api_testka_dev-0.0.90.tar", last modified: Mon May 29 03:22:56 2023, max compression
+gzip compressed data, was "je_api_testka_dev-0.0.91.tar", last modified: Wed May 31 05:43:00 2023, max compression
```

## Comparing `je_api_testka_dev-0.0.90.tar` & `je_api_testka_dev-0.0.91.tar`

### file list

```diff
@@ -1,79 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.861945 je_api_testka_dev-0.0.90/
--rw-rw-rw-   0        0        0     3330 2023-05-29 03:22:56.860978 je_api_testka_dev-0.0.90/PKG-INFO
--rw-rw-rw-   0        0        0     2526 2023-05-24 09:54:01.000000 je_api_testka_dev-0.0.90/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.674218 je_api_testka_dev-0.0.90/je_api_testka/
--rw-rw-rw-   0        0        0     2845 2023-04-21 07:30:34.000000 je_api_testka_dev-0.0.90/je_api_testka/__init__.py
--rw-rw-rw-   0        0        0     2349 2023-04-25 09:07:47.000000 je_api_testka_dev-0.0.90/je_api_testka/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.685744 je_api_testka_dev-0.0.90/je_api_testka/requests_wrapper/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.90/je_api_testka/requests_wrapper/__init__.py
--rw-rw-rw-   0        0        0     5026 2023-04-18 02:35:49.000000 je_api_testka_dev-0.0.90/je_api_testka/requests_wrapper/request_method.py
--rw-rw-rw-   0        0        0     2615 2023-04-18 02:35:49.000000 je_api_testka_dev-0.0.90/je_api_testka/requests_wrapper/requests_http_method_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.689250 je_api_testka_dev-0.0.90/je_api_testka/utils/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.696763 je_api_testka_dev-0.0.90/je_api_testka/utils/assert_result/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/assert_result/__init__.py
--rw-rw-rw-   0        0        0      942 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/assert_result/result_check.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.706415 je_api_testka_dev-0.0.90/je_api_testka/utils/callback/
--rw-rw-rw-   0        0        0        0 2023-03-31 09:04:52.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/callback/__init__.py
--rw-rw-rw-   0        0        0     3497 2023-05-29 03:22:33.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/callback/callback_function_executor.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.716929 je_api_testka_dev-0.0.90/je_api_testka/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/exception/__init__.py
--rw-rw-rw-   0        0        0     3393 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0     2392 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.729222 je_api_testka_dev-0.0.90/je_api_testka/utils/executor/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/executor/__init__.py
--rw-rw-rw-   0        0        0     5456 2023-05-29 03:21:49.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/executor/action_executor.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.735239 je_api_testka_dev-0.0.90/je_api_testka/utils/file_process/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/file_process/__init__.py
--rw-rw-rw-   0        0        0      709 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/file_process/get_dir_file_list.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.749318 je_api_testka_dev-0.0.90/je_api_testka/utils/generate_report/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/generate_report/__init__.py
--rw-rw-rw-   0        0        0     9028 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/generate_report/html_report_generate.py
--rw-rw-rw-   0        0        0     4017 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/generate_report/json_report.py
--rw-rw-rw-   0        0        0     1688 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/generate_report/xml_report.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.755378 je_api_testka_dev-0.0.90/je_api_testka/utils/get_data_strcture/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/get_data_strcture/__init__.py
--rw-rw-rw-   0        0        0     1588 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/get_data_strcture/get_api_data.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.758891 je_api_testka_dev-0.0.90/je_api_testka/utils/json/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/json/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.764912 je_api_testka_dev-0.0.90/je_api_testka/utils/json/json_file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/json/json_file/__init__.py
--rw-rw-rw-   0        0        0     1353 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/json/json_file/json_file.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.771988 je_api_testka_dev-0.0.90/je_api_testka/utils/json/json_format/
--rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/json/json_format/__init__.py
--rw-rw-rw-   0        0        0     1300 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/json/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.778034 je_api_testka_dev-0.0.90/je_api_testka/utils/mock_server/
--rw-rw-rw-   0        0        0        0 2023-04-21 01:03:22.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/mock_server/__init__.py
--rw-rw-rw-   0        0        0     1479 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/mock_server/flask_mock_server.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.784266 je_api_testka_dev-0.0.90/je_api_testka/utils/package_manager/
--rw-rw-rw-   0        0        0        0 2023-04-06 01:01:22.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/package_manager/__init__.py
--rw-rw-rw-   0        0        0     3346 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/package_manager/package_manager_class.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.792348 je_api_testka_dev-0.0.90/je_api_testka/utils/project/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/project/__init__.py
--rw-rw-rw-   0        0        0     2982 2023-04-18 02:25:34.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/project/create_project_structure.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.801857 je_api_testka_dev-0.0.90/je_api_testka/utils/project/template/
--rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/project/template/__init__.py
--rw-rw-rw-   0        0        0      633 2023-04-17 08:42:18.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/project/template/template_executor.py
--rw-rw-rw-   0        0        0      633 2023-04-17 08:52:06.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/project/template/template_keyword.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.809079 je_api_testka_dev-0.0.90/je_api_testka/utils/socket_server/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/socket_server/__init__.py
--rw-rw-rw-   0        0        0     2490 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/socket_server/api_testka_socket_server.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.815241 je_api_testka_dev-0.0.90/je_api_testka/utils/test_record/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/test_record/__init__.py
--rw-rw-rw-   0        0        0      389 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/test_record/test_record_class.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.817220 je_api_testka_dev-0.0.90/je_api_testka/utils/xml/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/xml/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.824743 je_api_testka_dev-0.0.90/je_api_testka/utils/xml/change_xml_structure/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/xml/change_xml_structure/__init__.py
--rw-rw-rw-   0        0        0     2513 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.830280 je_api_testka_dev-0.0.90/je_api_testka/utils/xml/xml_file/
--rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/xml/xml_file/__init__.py
--rw-rw-rw-   0        0        0     2424 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.90/je_api_testka/utils/xml/xml_file/xml_file.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:22:56.857429 je_api_testka_dev-0.0.90/je_api_testka_dev.egg-info/
--rw-rw-rw-   0        0        0     3330 2023-05-29 03:22:56.000000 je_api_testka_dev-0.0.90/je_api_testka_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2455 2023-05-29 03:22:56.000000 je_api_testka_dev-0.0.90/je_api_testka_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 03:22:56.000000 je_api_testka_dev-0.0.90/je_api_testka_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-29 03:22:56.000000 je_api_testka_dev-0.0.90/je_api_testka_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-29 03:22:56.000000 je_api_testka_dev-0.0.90/je_api_testka_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1150 2023-05-29 03:22:33.000000 je_api_testka_dev-0.0.90/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 03:22:56.863019 je_api_testka_dev-0.0.90/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.734224 je_api_testka_dev-0.0.91/
+-rw-rw-rw-   0        0        0     3074 2023-05-31 05:43:00.732269 je_api_testka_dev-0.0.91/PKG-INFO
+-rw-rw-rw-   0        0        0     2270 2023-05-30 02:10:25.000000 je_api_testka_dev-0.0.91/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.517528 je_api_testka_dev-0.0.91/je_api_testka/
+-rw-rw-rw-   0        0        0     2957 2023-05-31 05:32:44.000000 je_api_testka_dev-0.0.91/je_api_testka/__init__.py
+-rw-rw-rw-   0        0        0     2349 2023-04-25 09:07:47.000000 je_api_testka_dev-0.0.91/je_api_testka/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.534587 je_api_testka_dev-0.0.91/je_api_testka/requests_wrapper/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/requests_wrapper/__init__.py
+-rw-rw-rw-   0        0        0     5026 2023-04-18 02:35:49.000000 je_api_testka_dev-0.0.91/je_api_testka/requests_wrapper/request_method.py
+-rw-rw-rw-   0        0        0     2615 2023-04-18 02:35:49.000000 je_api_testka_dev-0.0.91/je_api_testka/requests_wrapper/requests_http_method_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.539741 je_api_testka_dev-0.0.91/je_api_testka/utils/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.547743 je_api_testka_dev-0.0.91/je_api_testka/utils/assert_result/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/assert_result/__init__.py
+-rw-rw-rw-   0        0        0      942 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/assert_result/result_check.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.554788 je_api_testka_dev-0.0.91/je_api_testka/utils/callback/
+-rw-rw-rw-   0        0        0        0 2023-03-31 09:04:52.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/callback/__init__.py
+-rw-rw-rw-   0        0        0     3497 2023-05-29 03:22:33.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/callback/callback_function_executor.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.569791 je_api_testka_dev-0.0.91/je_api_testka/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0     3393 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0     2392 2023-04-21 01:54:17.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.576789 je_api_testka_dev-0.0.91/je_api_testka/utils/executor/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/executor/__init__.py
+-rw-rw-rw-   0        0        0     5456 2023-05-29 03:21:49.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/executor/action_executor.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.585807 je_api_testka_dev-0.0.91/je_api_testka/utils/file_process/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/file_process/__init__.py
+-rw-rw-rw-   0        0        0      709 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/file_process/get_dir_file_list.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.599287 je_api_testka_dev-0.0.91/je_api_testka/utils/generate_report/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/generate_report/__init__.py
+-rw-rw-rw-   0        0        0     9028 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/generate_report/html_report_generate.py
+-rw-rw-rw-   0        0        0     4017 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/generate_report/json_report.py
+-rw-rw-rw-   0        0        0     1688 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/generate_report/xml_report.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.611527 je_api_testka_dev-0.0.91/je_api_testka/utils/get_data_strcture/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/get_data_strcture/__init__.py
+-rw-rw-rw-   0        0        0     1588 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/get_data_strcture/get_api_data.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.615527 je_api_testka_dev-0.0.91/je_api_testka/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/json/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.621564 je_api_testka_dev-0.0.91/je_api_testka/utils/json/json_file/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/json/json_file/__init__.py
+-rw-rw-rw-   0        0        0     1353 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/json/json_file/json_file.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.628528 je_api_testka_dev-0.0.91/je_api_testka/utils/json/json_format/
+-rw-rw-rw-   0        0        0        2 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/json/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1300 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/json/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.635529 je_api_testka_dev-0.0.91/je_api_testka/utils/mock_server/
+-rw-rw-rw-   0        0        0        0 2023-04-21 01:03:22.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/mock_server/__init__.py
+-rw-rw-rw-   0        0        0     1479 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/mock_server/flask_mock_server.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.639524 je_api_testka_dev-0.0.91/je_api_testka/utils/package_manager/
+-rw-rw-rw-   0        0        0        0 2023-04-06 01:01:22.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/package_manager/__init__.py
+-rw-rw-rw-   0        0        0     3346 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/package_manager/package_manager_class.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.645553 je_api_testka_dev-0.0.91/je_api_testka/utils/project/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/project/__init__.py
+-rw-rw-rw-   0        0        0     2982 2023-04-18 02:25:34.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/project/create_project_structure.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.659557 je_api_testka_dev-0.0.91/je_api_testka/utils/project/template/
+-rw-rw-rw-   0        0        0        0 2023-04-10 03:26:08.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/project/template/__init__.py
+-rw-rw-rw-   0        0        0      633 2023-04-17 08:42:18.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/project/template/template_executor.py
+-rw-rw-rw-   0        0        0      633 2023-04-17 08:52:06.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/project/template/template_keyword.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.667198 je_api_testka_dev-0.0.91/je_api_testka/utils/scheduler/
+-rw-rw-rw-   0        0        0        0 2023-05-31 01:17:46.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/scheduler/__init__.py
+-rw-rw-rw-   0        0        0     5280 2023-05-31 05:41:42.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/scheduler/extend_apscheduler.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.673198 je_api_testka_dev-0.0.91/je_api_testka/utils/socket_server/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/socket_server/__init__.py
+-rw-rw-rw-   0        0        0     2490 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/socket_server/api_testka_socket_server.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.679311 je_api_testka_dev-0.0.91/je_api_testka/utils/test_record/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/test_record/__init__.py
+-rw-rw-rw-   0        0        0      389 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/test_record/test_record_class.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.683201 je_api_testka_dev-0.0.91/je_api_testka/utils/xml/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/xml/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.688822 je_api_testka_dev-0.0.91/je_api_testka/utils/xml/change_xml_structure/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/xml/change_xml_structure/__init__.py
+-rw-rw-rw-   0        0        0     2513 2023-05-22 01:11:00.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.699011 je_api_testka_dev-0.0.91/je_api_testka/utils/xml/xml_file/
+-rw-rw-rw-   0        0        0        0 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/xml/xml_file/__init__.py
+-rw-rw-rw-   0        0        0     2424 2023-03-28 03:04:09.000000 je_api_testka_dev-0.0.91/je_api_testka/utils/xml/xml_file/xml_file.py
+drwxrwxrwx   0        0        0        0 2023-05-31 05:43:00.729232 je_api_testka_dev-0.0.91/je_api_testka_dev.egg-info/
+-rw-rw-rw-   0        0        0     3074 2023-05-31 05:43:00.000000 je_api_testka_dev-0.0.91/je_api_testka_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2549 2023-05-31 05:43:00.000000 je_api_testka_dev-0.0.91/je_api_testka_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 05:43:00.000000 je_api_testka_dev-0.0.91/je_api_testka_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-05-31 05:43:00.000000 je_api_testka_dev-0.0.91/je_api_testka_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-31 05:43:00.000000 je_api_testka_dev-0.0.91/je_api_testka_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1170 2023-05-31 05:42:36.000000 je_api_testka_dev-0.0.91/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 05:43:00.734224 je_api_testka_dev-0.0.91/setup.cfg
```

### Comparing `je_api_testka_dev-0.0.90/PKG-INFO` & `je_api_testka_dev-0.0.91/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je_api_testka_dev
-Version: 0.0.90
+Version: 0.0.91
 Summary: Requests Automation Framework
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/APITestka
 Project-URL: Documentation, https://apitestka.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/APITestka
 Classifier: Programming Language :: Python :: 3.8
@@ -32,35 +32,30 @@
 
 ### Documentation
 
 [![Documentation Status](https://readthedocs.org/projects/apitestka/badge/?version=latest)](https://apitestka.readthedocs.io/en/latest/?badge=latest)
 
 ---
 > Project Kanban \
-> https://github.com/orgs/Intergration-Automation-Testing/projects/2 \
-> Simple way to automation requests HTTP/S & Soap \
-> Wrapper for Requests package, designed for those with experience using Requests. \
-> Send HTTP/S and SOAP requests with a simple line of code or keyword. \
-> Detailed information on Requests and Responses. \
-> Solves problems such as:
->> * Detailed reports on Requests and Responses.
->> * Automation for SOAP protocol.
->> * Data comparison for each Request.
->> * API request in pure CLI mode.
----
-### Features
+> https://github.com/orgs/Integration-Automation/projects/2/views/1 \
+> * API requests automation.
+> * Data comparison for each Request.
+> * API request in pure CLI mode.
+> * Detailed reports on Requests and Responses.
+> * HTTP/HTTPS support.
+> * SOAP/XML support.
+> * JSON support.
+> * Generate JSON/HTML/XML report.
+> * APITestka script.
+> * 1 sec / thousands requests.
+> * OS Independent.
+> * Mockserver support.
+> * Remote Automation support.
+> * Project & Template support.
 
->* HTTP Method requests
->* Get response data body etc...
->* Action file and executor
->* result compare
->* xml to json and json to xml
->* Soap test
->* Generate HTML Report
->* CLI with action file
 
 ---
 
 
 ## install
 > pip install je_api_testka
```

### Comparing `je_api_testka_dev-0.0.90/README.md` & `je_api_testka_dev-0.0.91/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -13,35 +13,30 @@
 
 ### Documentation
 
 [![Documentation Status](https://readthedocs.org/projects/apitestka/badge/?version=latest)](https://apitestka.readthedocs.io/en/latest/?badge=latest)
 
 ---
 > Project Kanban \
-> https://github.com/orgs/Intergration-Automation-Testing/projects/2 \
-> Simple way to automation requests HTTP/S & Soap \
-> Wrapper for Requests package, designed for those with experience using Requests. \
-> Send HTTP/S and SOAP requests with a simple line of code or keyword. \
-> Detailed information on Requests and Responses. \
-> Solves problems such as:
->> * Detailed reports on Requests and Responses.
->> * Automation for SOAP protocol.
->> * Data comparison for each Request.
->> * API request in pure CLI mode.
----
-### Features
+> https://github.com/orgs/Integration-Automation/projects/2/views/1 \
+> * API requests automation.
+> * Data comparison for each Request.
+> * API request in pure CLI mode.
+> * Detailed reports on Requests and Responses.
+> * HTTP/HTTPS support.
+> * SOAP/XML support.
+> * JSON support.
+> * Generate JSON/HTML/XML report.
+> * APITestka script.
+> * 1 sec / thousands requests.
+> * OS Independent.
+> * Mockserver support.
+> * Remote Automation support.
+> * Project & Template support.
 
->* HTTP Method requests
->* Get response data body etc...
->* Action file and executor
->* result compare
->* xml to json and json to xml
->* Soap test
->* Generate HTML Report
->* CLI with action file
 
 ---
 
 
 ## install
 > pip install je_api_testka
```

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/__init__.py` & `je_api_testka_dev-0.0.91/je_api_testka/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,20 +32,22 @@
 # xml
 from je_api_testka.utils.xml.xml_file.xml_file import XMLParser
 from je_api_testka.utils.xml.xml_file.xml_file import reformat_xml_file
 # Mock server
 from je_api_testka.utils.mock_server.flask_mock_server import flask_mock_server_instance
 # Flask
 from flask import request, redirect
+# Scheduler
+from je_api_testka.utils.scheduler.extend_apscheduler import SchedulerManager
 
 __all__ = ["test_api_method",
            "add_command_to_executor",
            "execute_action", "execute_files", "executor",
            "get_dir_files_as_list",
            "generate_html", "generate_html_report", "read_action_json",
            "write_action_json", "reformat_json", "generate_json", "generate_json_report",
            "start_apitestka_socket_server",
            "test_record_instance", "dict_to_elements_tree", "elements_tree_to_dict",
            "XMLParser", "reformat_xml_file", "generate_xml", "generate_xml_report",
            "callback_executor", "create_project_dir", "flask_mock_server_instance",
-           "request", "redirect"
+           "request", "redirect", "SchedulerManager"
            ]
```

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/__main__.py` & `je_api_testka_dev-0.0.91/je_api_testka/__main__.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/requests_wrapper/request_method.py` & `je_api_testka_dev-0.0.91/je_api_testka/requests_wrapper/request_method.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/requests_wrapper/requests_http_method_wrapper.py` & `je_api_testka_dev-0.0.91/je_api_testka/requests_wrapper/requests_http_method_wrapper.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/utils/assert_result/result_check.py` & `je_api_testka_dev-0.0.91/je_api_testka/utils/assert_result/result_check.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/utils/callback/callback_function_executor.py` & `je_api_testka_dev-0.0.91/je_api_testka/utils/callback/callback_function_executor.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/utils/exception/exception_tags.py` & `je_api_testka_dev-0.0.91/je_api_testka/utils/exception/exception_tags.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/utils/exception/exceptions.py` & `je_api_testka_dev-0.0.91/je_api_testka/utils/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/utils/executor/action_executor.py` & `je_api_testka_dev-0.0.91/je_api_testka/utils/executor/action_executor.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/utils/file_process/get_dir_file_list.py` & `je_api_testka_dev-0.0.91/je_api_testka/utils/file_process/get_dir_file_list.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/utils/generate_report/html_report_generate.py` & `je_api_testka_dev-0.0.91/je_api_testka/utils/generate_report/html_report_generate.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/utils/generate_report/json_report.py` & `je_api_testka_dev-0.0.91/je_api_testka/utils/generate_report/json_report.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/utils/generate_report/xml_report.py` & `je_api_testka_dev-0.0.91/je_api_testka/utils/generate_report/xml_report.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/utils/get_data_strcture/get_api_data.py` & `je_api_testka_dev-0.0.91/je_api_testka/utils/get_data_strcture/get_api_data.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/utils/json/json_file/json_file.py` & `je_api_testka_dev-0.0.91/je_api_testka/utils/json/json_file/json_file.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/utils/json/json_format/json_process.py` & `je_api_testka_dev-0.0.91/je_api_testka/utils/json/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/utils/mock_server/flask_mock_server.py` & `je_api_testka_dev-0.0.91/je_api_testka/utils/mock_server/flask_mock_server.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/utils/package_manager/package_manager_class.py` & `je_api_testka_dev-0.0.91/je_api_testka/utils/package_manager/package_manager_class.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/utils/project/create_project_structure.py` & `je_api_testka_dev-0.0.91/je_api_testka/utils/project/create_project_structure.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/utils/project/template/template_executor.py` & `je_api_testka_dev-0.0.91/je_api_testka/utils/project/template/template_executor.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/utils/project/template/template_keyword.py` & `je_api_testka_dev-0.0.91/je_api_testka/utils/project/template/template_keyword.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/utils/socket_server/api_testka_socket_server.py` & `je_api_testka_dev-0.0.91/je_api_testka/utils/socket_server/api_testka_socket_server.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py` & `je_api_testka_dev-0.0.91/je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.90/je_api_testka/utils/xml/xml_file/xml_file.py` & `je_api_testka_dev-0.0.91/je_api_testka/utils/xml/xml_file/xml_file.py`

 * *Files identical despite different names*

### Comparing `je_api_testka_dev-0.0.90/je_api_testka_dev.egg-info/PKG-INFO` & `je_api_testka_dev-0.0.91/je_api_testka_dev.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: je-api-testka-dev
-Version: 0.0.90
+Version: 0.0.91
 Summary: Requests Automation Framework
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/APITestka
 Project-URL: Documentation, https://apitestka.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/APITestka
 Classifier: Programming Language :: Python :: 3.8
@@ -32,35 +32,30 @@
 
 ### Documentation
 
 [![Documentation Status](https://readthedocs.org/projects/apitestka/badge/?version=latest)](https://apitestka.readthedocs.io/en/latest/?badge=latest)
 
 ---
 > Project Kanban \
-> https://github.com/orgs/Intergration-Automation-Testing/projects/2 \
-> Simple way to automation requests HTTP/S & Soap \
-> Wrapper for Requests package, designed for those with experience using Requests. \
-> Send HTTP/S and SOAP requests with a simple line of code or keyword. \
-> Detailed information on Requests and Responses. \
-> Solves problems such as:
->> * Detailed reports on Requests and Responses.
->> * Automation for SOAP protocol.
->> * Data comparison for each Request.
->> * API request in pure CLI mode.
----
-### Features
+> https://github.com/orgs/Integration-Automation/projects/2/views/1 \
+> * API requests automation.
+> * Data comparison for each Request.
+> * API request in pure CLI mode.
+> * Detailed reports on Requests and Responses.
+> * HTTP/HTTPS support.
+> * SOAP/XML support.
+> * JSON support.
+> * Generate JSON/HTML/XML report.
+> * APITestka script.
+> * 1 sec / thousands requests.
+> * OS Independent.
+> * Mockserver support.
+> * Remote Automation support.
+> * Project & Template support.
 
->* HTTP Method requests
->* Get response data body etc...
->* Action file and executor
->* result compare
->* xml to json and json to xml
->* Soap test
->* Generate HTML Report
->* CLI with action file
 
 ---
 
 
 ## install
 > pip install je_api_testka
```

### Comparing `je_api_testka_dev-0.0.90/je_api_testka_dev.egg-info/SOURCES.txt` & `je_api_testka_dev-0.0.91/je_api_testka_dev.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 je_api_testka/utils/package_manager/__init__.py
 je_api_testka/utils/package_manager/package_manager_class.py
 je_api_testka/utils/project/__init__.py
 je_api_testka/utils/project/create_project_structure.py
 je_api_testka/utils/project/template/__init__.py
 je_api_testka/utils/project/template/template_executor.py
 je_api_testka/utils/project/template/template_keyword.py
+je_api_testka/utils/scheduler/__init__.py
+je_api_testka/utils/scheduler/extend_apscheduler.py
 je_api_testka/utils/socket_server/__init__.py
 je_api_testka/utils/socket_server/api_testka_socket_server.py
 je_api_testka/utils/test_record/__init__.py
 je_api_testka/utils/test_record/test_record_class.py
 je_api_testka/utils/xml/__init__.py
 je_api_testka/utils/xml/change_xml_structure/__init__.py
 je_api_testka/utils/xml/change_xml_structure/change_xml_structure.py
```

### Comparing `je_api_testka_dev-0.0.90/pyproject.toml` & `je_api_testka_dev-0.0.91/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 # This is dev version
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "je_api_testka_dev"
-version = "0.0.90"
+version = "0.0.91"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 description = "Requests Automation Framework"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 dependencies = [
     "requests",
-    "Flask"
+    "Flask",
+    "APScheduler"
 ]
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Development Status :: 2 - Pre-Alpha",
     "Environment :: Win32 (MS Windows)",
     "Environment :: MacOS X",
     "Environment :: X11 Applications",
```

