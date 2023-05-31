# Comparing `tmp/aind_metadata_service-0.4.3.tar.gz` & `tmp/aind_metadata_service-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_metadata_service-0.4.3.tar", last modified: Wed May 24 21:12:00 2023, max compression
+gzip compressed data, was "aind_metadata_service-0.4.4.tar", last modified: Wed May 31 17:01:37 2023, max compression
```

## Comparing `aind_metadata_service-0.4.3.tar` & `aind_metadata_service-0.4.4.tar`

### file list

```diff
@@ -1,121 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.579331 aind_metadata_service-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.567331 aind_metadata_service-0.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.571331 aind_metadata_service-0.4.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.571331 aind_metadata_service-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-24 21:12:00.579331 aind_metadata_service-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.571331 aind_metadata_service-0.4.3/doc_template/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.571331 aind_metadata_service-0.4.3/doc_template/source/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/doc_template/source/aind_metadata_service.labtracks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/doc_template/source/aind_metadata_service.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/doc_template/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 21:12:00.579331 aind_metadata_service-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.567331 aind_metadata_service-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.571331 aind_metadata_service-0.4.3/src/aind_metadata_service/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 21:11:44.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.571331 aind_metadata_service-0.4.3/src/aind_metadata_service/labtracks/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/labtracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13540 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/labtracks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/labtracks/query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/response_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.571331 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.571331 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2019/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2019/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66133 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2019/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    41586 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2019/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2019/procedures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.571331 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2023/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2023/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19552 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2023/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    35167 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2023/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.571331 aind_metadata_service-0.4.3/src/aind_metadata_service.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-24 21:12:00.000000 aind_metadata_service-0.4.3/src/aind_metadata_service.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-05-24 21:12:00.000000 aind_metadata_service-0.4.3/src/aind_metadata_service.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 21:12:00.000000 aind_metadata_service-0.4.3/src/aind_metadata_service.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-24 21:12:00.000000 aind_metadata_service-0.4.3/src/aind_metadata_service.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 21:12:00.000000 aind_metadata_service-0.4.3/src/aind_metadata_service.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.575331 aind_metadata_service-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.575331 aind_metadata_service-0.4.3/tests/labtracks/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/labtracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/labtracks/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/labtracks/test_query_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/labtracks/test_response_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.567331 aind_metadata_service-0.4.3/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.575331 aind_metadata_service-0.4.3/tests/resources/json_responses/
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/json_responses/combined.json
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/json_responses/mapped_las_procedure.json
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/json_responses/mapped_sp_procedure.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.567331 aind_metadata_service-0.4.3/tests/resources/sharepoint/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.567331 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.575331 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item12.json
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.575331 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item1.json
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item12.json
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item2.json
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item3.json
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item4.json
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item5.json
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item6.json
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item7.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.567331 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.579331 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item13.json
--rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json
--rw-r--r--   0 runner    (1001) docker     (123)     9620 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json
--rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.579331 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item10.json
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item11.json
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item13.json
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item14.json
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item15.json
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item16.json
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item17.json
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item8.json
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item9.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.579331 aind_metadata_service-0.4.3/tests/sharepoint/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/sharepoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.579331 aind_metadata_service-0.4.3/tests/sharepoint/nsb2019/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/sharepoint/nsb2019/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/sharepoint/nsb2019/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/sharepoint/nsb2019/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 21:12:00.579331 aind_metadata_service-0.4.3/tests/sharepoint/nsb2023/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/sharepoint/nsb2023/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/sharepoint/nsb2023/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/sharepoint/nsb2023/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/sharepoint/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-05-24 21:11:43.000000 aind_metadata_service-0.4.3/tests/test_response_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.901626 aind_metadata_service-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.877625 aind_metadata_service-0.4.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.885625 aind_metadata_service-0.4.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.885625 aind_metadata_service-0.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-31 17:01:37.901626 aind_metadata_service-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.885625 aind_metadata_service-0.4.4/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.885625 aind_metadata_service-0.4.4/doc_template/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/doc_template/source/aind_metadata_service.labtracks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/doc_template/source/aind_metadata_service.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/doc_template/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 17:01:37.901626 aind_metadata_service-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.881625 aind_metadata_service-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.889625 aind_metadata_service-0.4.4/src/aind_metadata_service/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-31 17:01:18.000000 aind_metadata_service-0.4.4/src/aind_metadata_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/src/aind_metadata_service/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.889625 aind_metadata_service-0.4.4/src/aind_metadata_service/labtracks/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/src/aind_metadata_service/labtracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13540 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/src/aind_metadata_service/labtracks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/src/aind_metadata_service/labtracks/query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/src/aind_metadata_service/response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/src/aind_metadata_service/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.889625 aind_metadata_service-0.4.4/src/aind_metadata_service/sharepoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/src/aind_metadata_service/sharepoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/src/aind_metadata_service/sharepoint/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.889625 aind_metadata_service-0.4.4/src/aind_metadata_service/sharepoint/nsb2019/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/src/aind_metadata_service/sharepoint/nsb2019/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66133 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/src/aind_metadata_service/sharepoint/nsb2019/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41586 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/src/aind_metadata_service/sharepoint/nsb2019/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/src/aind_metadata_service/sharepoint/nsb2019/procedures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.889625 aind_metadata_service-0.4.4/src/aind_metadata_service/sharepoint/nsb2023/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/src/aind_metadata_service/sharepoint/nsb2023/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113119 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/src/aind_metadata_service/sharepoint/nsb2023/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57053 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/src/aind_metadata_service/sharepoint/nsb2023/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/src/aind_metadata_service/sharepoint/nsb2023/procedures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.889625 aind_metadata_service-0.4.4/src/aind_metadata_service.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-31 17:01:37.000000 aind_metadata_service-0.4.4/src/aind_metadata_service.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-31 17:01:37.000000 aind_metadata_service-0.4.4/src/aind_metadata_service.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:01:37.000000 aind_metadata_service-0.4.4/src/aind_metadata_service.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-31 17:01:37.000000 aind_metadata_service-0.4.4/src/aind_metadata_service.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 17:01:37.000000 aind_metadata_service-0.4.4/src/aind_metadata_service.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.889625 aind_metadata_service-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.889625 aind_metadata_service-0.4.4/tests/labtracks/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/labtracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/labtracks/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/labtracks/test_query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/labtracks/test_response_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.881625 aind_metadata_service-0.4.4/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.893625 aind_metadata_service-0.4.4/tests/resources/json_responses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/json_responses/combined.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/json_responses/mapped_las_procedure.json
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/json_responses/mapped_sp_procedure.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.885625 aind_metadata_service-0.4.4/tests/resources/sharepoint/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.885625 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.893625 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/mapped/
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item12.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.897626 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/raw/list_item1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/raw/list_item12.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/raw/list_item2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/raw/list_item3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/raw/list_item4.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/raw/list_item5.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/raw/list_item6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/raw/list_item7.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.885625 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.897626 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/mapped/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item13.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9617 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item9.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.897626 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/raw/list_item10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/raw/list_item11.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/raw/list_item13.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/raw/list_item14.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/raw/list_item15.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/raw/list_item16.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/raw/list_item17.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/raw/list_item8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/raw/list_item9.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.901626 aind_metadata_service-0.4.4/tests/sharepoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/sharepoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.901626 aind_metadata_service-0.4.4/tests/sharepoint/nsb2019/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/sharepoint/nsb2019/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/sharepoint/nsb2019/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/sharepoint/nsb2019/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:01:37.901626 aind_metadata_service-0.4.4/tests/sharepoint/nsb2023/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/sharepoint/nsb2023/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/sharepoint/nsb2023/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/sharepoint/nsb2023/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/sharepoint/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-05-31 17:01:17.000000 aind_metadata_service-0.4.4/tests/test_response_handle.py
```

### Comparing `aind_metadata_service-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_metadata_service-0.4.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_metadata_service-0.4.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/.github/ISSUE_TEMPLATE/user-story.md` & `aind_metadata_service-0.4.4/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/.github/workflows/ci.yml` & `aind_metadata_service-0.4.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/.github/workflows/publish.yml` & `aind_metadata_service-0.4.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/.gitignore` & `aind_metadata_service-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/Dockerfile` & `aind_metadata_service-0.4.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/LICENSE` & `aind_metadata_service-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/PKG-INFO` & `aind_metadata_service-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_metadata_service
-Version: 0.4.3
+Version: 0.4.4
 Summary: REST service to retrive metadata from databases.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_metadata_service-0.4.3/README.md` & `aind_metadata_service-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/doc_template/Makefile` & `aind_metadata_service-0.4.4/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/doc_template/make.bat` & `aind_metadata_service-0.4.4/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/doc_template/source/aind_metadata_service.labtracks.rst` & `aind_metadata_service-0.4.4/doc_template/source/aind_metadata_service.labtracks.rst`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/doc_template/source/conf.py` & `aind_metadata_service-0.4.4/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/pyproject.toml` & `aind_metadata_service-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/src/aind_metadata_service/client.py` & `aind_metadata_service-0.4.4/src/aind_metadata_service/client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/src/aind_metadata_service/labtracks/client.py` & `aind_metadata_service-0.4.4/src/aind_metadata_service/labtracks/client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/src/aind_metadata_service/labtracks/query_builder.py` & `aind_metadata_service-0.4.4/src/aind_metadata_service/labtracks/query_builder.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/src/aind_metadata_service/response_handler.py` & `aind_metadata_service-0.4.4/src/aind_metadata_service/response_handler.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/src/aind_metadata_service/server.py` & `aind_metadata_service-0.4.4/src/aind_metadata_service/server.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/client.py` & `aind_metadata_service-0.4.4/src/aind_metadata_service/sharepoint/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,16 +2,20 @@
 
 from aind_data_schema.procedures import Procedures
 from fastapi.responses import JSONResponse
 from office365.runtime.auth.client_credential import ClientCredential
 from office365.sharepoint.client_context import ClientContext
 
 from aind_metadata_service.response_handler import Responses
-from aind_metadata_service.sharepoint.nsb2019.procedures import NSB2019Mapping
-from aind_metadata_service.sharepoint.nsb2023.mapping import NSB2023Mapping
+from aind_metadata_service.sharepoint.nsb2019.procedures import (
+    NSB2019Procedures,
+)
+from aind_metadata_service.sharepoint.nsb2023.procedures import (
+    NSB2023Procedures,
+)
 
 
 class SharePointClient:
     """This class contains the api to connect to SharePoint db."""
 
     def __init__(
         self,
@@ -58,16 +62,16 @@
         JSONResponse
           A response
 
         """
         # TODO: Add try to handle internal server error response.
         subject_procedures = []
         nsb_ctx = self.nsb_client_context
-        nsb_2019_mapper = NSB2019Mapping()
-        nsb_2023_mapper = NSB2023Mapping()
+        nsb_2019_mapper = NSB2019Procedures()
+        nsb_2023_mapper = NSB2023Procedures()
         procedures2019 = nsb_2019_mapper.get_procedures_from_sharepoint(
             subject_id=subject_id,
             client_context=nsb_ctx,
             list_title=self.nsb_list_title_2019,
         )
         procedures2023 = nsb_2023_mapper.get_procedures_from_sharepoint(
             subject_id=subject_id,
```

### Comparing `aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2019/mapping.py` & `aind_metadata_service-0.4.4/src/aind_metadata_service/sharepoint/nsb2019/mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2019/models.py` & `aind_metadata_service-0.4.4/src/aind_metadata_service/sharepoint/nsb2019/models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/src/aind_metadata_service/sharepoint/nsb2019/procedures.py` & `aind_metadata_service-0.4.4/src/aind_metadata_service/sharepoint/nsb2019/procedures.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from aind_data_schema.procedures import SubjectProcedure
 from office365.sharepoint.client_context import ClientContext
 
 from aind_metadata_service.sharepoint.nsb2019.mapping import MappedNSBList
 from aind_metadata_service.sharepoint.nsb2019.models import NSBList
 
 
-class NSB2019Mapping:
+class NSB2019Procedures:
     """Provides methods to retrieve procedure information from sharepoint,
     parses the response into an intermediate data model, and maps that model
     into AIND Procedures model."""
 
     _view_title = "New Request"
 
     def get_procedures_from_sharepoint(
```

### Comparing `aind_metadata_service-0.4.3/src/aind_metadata_service.egg-info/PKG-INFO` & `aind_metadata_service-0.4.4/src/aind_metadata_service.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-metadata-service
-Version: 0.4.3
+Version: 0.4.4
 Summary: REST service to retrive metadata from databases.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `aind_metadata_service-0.4.3/src/aind_metadata_service.egg-info/SOURCES.txt` & `aind_metadata_service-0.4.4/src/aind_metadata_service.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 src/aind_metadata_service/sharepoint/nsb2019/__init__.py
 src/aind_metadata_service/sharepoint/nsb2019/mapping.py
 src/aind_metadata_service/sharepoint/nsb2019/models.py
 src/aind_metadata_service/sharepoint/nsb2019/procedures.py
 src/aind_metadata_service/sharepoint/nsb2023/__init__.py
 src/aind_metadata_service/sharepoint/nsb2023/mapping.py
 src/aind_metadata_service/sharepoint/nsb2023/models.py
+src/aind_metadata_service/sharepoint/nsb2023/procedures.py
 tests/__init__.py
 tests/test_client.py
 tests/test_response_handle.py
 tests/labtracks/__init__.py
 tests/labtracks/test_client.py
 tests/labtracks/test_query_builder.py
 tests/labtracks/test_response_handler.py
```

### Comparing `aind_metadata_service-0.4.3/tests/labtracks/test_client.py` & `aind_metadata_service-0.4.4/tests/labtracks/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/labtracks/test_query_builder.py` & `aind_metadata_service-0.4.4/tests/labtracks/test_query_builder.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/labtracks/test_response_handler.py` & `aind_metadata_service-0.4.4/tests/labtracks/test_response_handler.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/json_responses/combined.json` & `aind_metadata_service-0.4.4/tests/resources/json_responses/combined.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/json_responses/mapped_las_procedure.json` & `aind_metadata_service-0.4.4/tests/resources/json_responses/mapped_las_procedure.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/json_responses/mapped_sp_procedure.json` & `aind_metadata_service-0.4.4/tests/resources/json_responses/mapped_sp_procedure.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item1.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item2.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item3.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item4.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item5.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item6.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/mapped/mapped_list_item7.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item1.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/raw/list_item1.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item12.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/raw/list_item12.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item2.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/raw/list_item2.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item3.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/raw/list_item3.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item4.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/raw/list_item4.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item5.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/raw/list_item5.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item6.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/raw/list_item6.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2019/raw/list_item7.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2019/raw/list_item7.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item10.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item11.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9844081844081843%*

 * *Differences: {'0': "{'headframe_type': 'Motor Ctx', 'headframe_part_number': '0160-100-51', 'well_part_number': "*

 * *      "'Rev A', 'well_type': 'Scientifica (CAM)'}",*

 * * '2': "{'probes': {'stereotactic_coordinate_dv': None}}",*

 * * '4': "{'probes': {'stereotactic_coordinate_dv': None}}",*

 * * '6': "{'probes': {'stereotactic_coordinate_dv': None}}",*

 * * '8': "{'probes': {'stereotactic_coordinate_dv': None}}"}*

```diff
@@ -7,23 +7,23 @@
             "type": "isoflurane"
         },
         "animal_weight_post": 28.2,
         "animal_weight_prior": 25.2,
         "end_date": "2022-01-03",
         "experimenter_full_name": "NSB-187",
         "headframe_material": null,
-        "headframe_part_number": "0160-100-46",
-        "headframe_type": "Frontal Ctx",
+        "headframe_part_number": "0160-100-51",
+        "headframe_type": "Motor Ctx",
         "iacuc_protocol": "2103",
         "notes": null,
         "procedure_type": "Headframe",
         "start_date": "2022-01-03",
         "weight_unit": "gram",
-        "well_part_number": "0160-055-08",
-        "well_type": "WHC NP"
+        "well_part_number": "Rev A",
+        "well_type": "Scientifica (CAM)"
     },
     {
         "alternating_current": null,
         "anaesthesia": {
             "duration": 90.0,
             "duration_unit": "minute",
             "level": 2.0,
@@ -78,15 +78,15 @@
             "bregma_to_lambda_distance": null,
             "bregma_to_lambda_unit": "millimeter",
             "core_diameter_unit": "\u03bcm",
             "ferrule_material": null,
             "name": "Probe A",
             "notes": null,
             "stereotactic_coordinate_ap": null,
-            "stereotactic_coordinate_dv": -2.95,
+            "stereotactic_coordinate_dv": null,
             "stereotactic_coordinate_ml": null,
             "stereotactic_coordinate_reference": "Bregma",
             "stereotactic_coordinate_unit": "millimeter"
         },
         "procedure_type": "Fiber implant",
         "start_date": "2022-01-03",
         "weight_unit": "gram"
@@ -147,15 +147,15 @@
             "bregma_to_lambda_distance": null,
             "bregma_to_lambda_unit": "millimeter",
             "core_diameter_unit": "\u03bcm",
             "ferrule_material": null,
             "name": "Probe B",
             "notes": null,
             "stereotactic_coordinate_ap": null,
-            "stereotactic_coordinate_dv": -1.05,
+            "stereotactic_coordinate_dv": null,
             "stereotactic_coordinate_ml": null,
             "stereotactic_coordinate_reference": "Bregma",
             "stereotactic_coordinate_unit": "millimeter"
         },
         "procedure_type": "Fiber implant",
         "start_date": "2022-01-03",
         "weight_unit": "gram"
@@ -187,15 +187,15 @@
         "injection_duration": null,
         "injection_duration_unit": "minute",
         "injection_hemisphere": "Left",
         "injection_materials": null,
         "instrument_id": null,
         "notes": null,
         "procedure_type": "Iontophoresis injection",
-        "recovery_time": 25,
+        "recovery_time": 25.0,
         "start_date": "2022-01-03",
         "targeted_structure": null,
         "weight_unit": "gram",
         "workstation_id": null
     },
     {
         "anaesthesia": {
@@ -216,15 +216,15 @@
             "bregma_to_lambda_distance": null,
             "bregma_to_lambda_unit": "millimeter",
             "core_diameter_unit": "\u03bcm",
             "ferrule_material": null,
             "name": "Probe C",
             "notes": null,
             "stereotactic_coordinate_ap": null,
-            "stereotactic_coordinate_dv": -1.85,
+            "stereotactic_coordinate_dv": null,
             "stereotactic_coordinate_ml": null,
             "stereotactic_coordinate_reference": "Bregma",
             "stereotactic_coordinate_unit": "millimeter"
         },
         "procedure_type": "Fiber implant",
         "start_date": "2022-01-03",
         "weight_unit": "gram"
@@ -256,15 +256,15 @@
         "injection_duration": null,
         "injection_duration_unit": "minute",
         "injection_hemisphere": "Right",
         "injection_materials": null,
         "instrument_id": null,
         "notes": null,
         "procedure_type": "Iontophoresis injection",
-        "recovery_time": 25,
+        "recovery_time": 25.0,
         "start_date": "2022-01-03",
         "targeted_structure": null,
         "weight_unit": "gram",
         "workstation_id": null
     },
     {
         "anaesthesia": {
@@ -285,15 +285,15 @@
             "bregma_to_lambda_distance": null,
             "bregma_to_lambda_unit": "millimeter",
             "core_diameter_unit": "\u03bcm",
             "ferrule_material": null,
             "name": "Probe D",
             "notes": null,
             "stereotactic_coordinate_ap": null,
-            "stereotactic_coordinate_dv": -1.8,
+            "stereotactic_coordinate_dv": null,
             "stereotactic_coordinate_ml": null,
             "stereotactic_coordinate_reference": "Bregma",
             "stereotactic_coordinate_unit": "millimeter"
         },
         "procedure_type": "Fiber implant",
         "start_date": "2022-01-03",
         "weight_unit": "gram"
```

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item15.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item14.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9844081844081843%*

 * *Differences: {'0': "{'headframe_type': 'Frontal Ctx', 'headframe_part_number': '0160-100-46', "*

 * *      "'well_part_number': '0160-055-08', 'well_type': 'WHC NP'}",*

 * * '2': "{'probes': {'stereotactic_coordinate_dv': None}}",*

 * * '4': "{'probes': {'stereotactic_coordinate_dv': None}}",*

 * * '6': "{'probes': {'stereotactic_coordinate_dv': None}}",*

 * * '8': "{'probes': {'stereotactic_coordinate_dv': None}}"}*

```diff
@@ -7,23 +7,23 @@
             "type": "isoflurane"
         },
         "animal_weight_post": 28.2,
         "animal_weight_prior": 25.2,
         "end_date": "2022-01-03",
         "experimenter_full_name": "NSB-187",
         "headframe_material": null,
-        "headframe_part_number": "0160-100-51",
-        "headframe_type": "Motor Ctx",
+        "headframe_part_number": "0160-100-46",
+        "headframe_type": "Frontal Ctx",
         "iacuc_protocol": "2103",
         "notes": null,
         "procedure_type": "Headframe",
         "start_date": "2022-01-03",
         "weight_unit": "gram",
-        "well_part_number": "Rev A",
-        "well_type": "Scientifica (CAM)"
+        "well_part_number": "0160-055-08",
+        "well_type": "WHC NP"
     },
     {
         "alternating_current": null,
         "anaesthesia": {
             "duration": 90.0,
             "duration_unit": "minute",
             "level": 2.0,
@@ -78,15 +78,15 @@
             "bregma_to_lambda_distance": null,
             "bregma_to_lambda_unit": "millimeter",
             "core_diameter_unit": "\u03bcm",
             "ferrule_material": null,
             "name": "Probe A",
             "notes": null,
             "stereotactic_coordinate_ap": null,
-            "stereotactic_coordinate_dv": -2.95,
+            "stereotactic_coordinate_dv": null,
             "stereotactic_coordinate_ml": null,
             "stereotactic_coordinate_reference": "Bregma",
             "stereotactic_coordinate_unit": "millimeter"
         },
         "procedure_type": "Fiber implant",
         "start_date": "2022-01-03",
         "weight_unit": "gram"
@@ -147,15 +147,15 @@
             "bregma_to_lambda_distance": null,
             "bregma_to_lambda_unit": "millimeter",
             "core_diameter_unit": "\u03bcm",
             "ferrule_material": null,
             "name": "Probe B",
             "notes": null,
             "stereotactic_coordinate_ap": null,
-            "stereotactic_coordinate_dv": -1.05,
+            "stereotactic_coordinate_dv": null,
             "stereotactic_coordinate_ml": null,
             "stereotactic_coordinate_reference": "Bregma",
             "stereotactic_coordinate_unit": "millimeter"
         },
         "procedure_type": "Fiber implant",
         "start_date": "2022-01-03",
         "weight_unit": "gram"
@@ -216,15 +216,15 @@
             "bregma_to_lambda_distance": null,
             "bregma_to_lambda_unit": "millimeter",
             "core_diameter_unit": "\u03bcm",
             "ferrule_material": null,
             "name": "Probe C",
             "notes": null,
             "stereotactic_coordinate_ap": null,
-            "stereotactic_coordinate_dv": -1.85,
+            "stereotactic_coordinate_dv": null,
             "stereotactic_coordinate_ml": null,
             "stereotactic_coordinate_reference": "Bregma",
             "stereotactic_coordinate_unit": "millimeter"
         },
         "procedure_type": "Fiber implant",
         "start_date": "2022-01-03",
         "weight_unit": "gram"
@@ -285,15 +285,15 @@
             "bregma_to_lambda_distance": null,
             "bregma_to_lambda_unit": "millimeter",
             "core_diameter_unit": "\u03bcm",
             "ferrule_material": null,
             "name": "Probe D",
             "notes": null,
             "stereotactic_coordinate_ap": null,
-            "stereotactic_coordinate_dv": -1.8,
+            "stereotactic_coordinate_dv": null,
             "stereotactic_coordinate_ml": null,
             "stereotactic_coordinate_reference": "Bregma",
             "stereotactic_coordinate_unit": "millimeter"
         },
         "procedure_type": "Fiber implant",
         "start_date": "2022-01-03",
         "weight_unit": "gram"
```

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item16.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992229992229993%*

 * *Differences: {'2': "{'probes': {'stereotactic_coordinate_dv': None}}",*

 * * '4': "{'probes': {'stereotactic_coordinate_dv': None}}",*

 * * '6': "{'probes': {'stereotactic_coordinate_dv': None}}",*

 * * '8': "{'probes': {'stereotactic_coordinate_dv': None}}"}*

```diff
@@ -78,15 +78,15 @@
             "bregma_to_lambda_distance": null,
             "bregma_to_lambda_unit": "millimeter",
             "core_diameter_unit": "\u03bcm",
             "ferrule_material": null,
             "name": "Probe A",
             "notes": null,
             "stereotactic_coordinate_ap": null,
-            "stereotactic_coordinate_dv": -2.95,
+            "stereotactic_coordinate_dv": null,
             "stereotactic_coordinate_ml": null,
             "stereotactic_coordinate_reference": "Bregma",
             "stereotactic_coordinate_unit": "millimeter"
         },
         "procedure_type": "Fiber implant",
         "start_date": null,
         "weight_unit": "gram"
@@ -147,15 +147,15 @@
             "bregma_to_lambda_distance": null,
             "bregma_to_lambda_unit": "millimeter",
             "core_diameter_unit": "\u03bcm",
             "ferrule_material": null,
             "name": "Probe B",
             "notes": null,
             "stereotactic_coordinate_ap": null,
-            "stereotactic_coordinate_dv": -1.05,
+            "stereotactic_coordinate_dv": null,
             "stereotactic_coordinate_ml": null,
             "stereotactic_coordinate_reference": "Bregma",
             "stereotactic_coordinate_unit": "millimeter"
         },
         "procedure_type": "Fiber implant",
         "start_date": "2022-01-03",
         "weight_unit": "gram"
@@ -216,15 +216,15 @@
             "bregma_to_lambda_distance": null,
             "bregma_to_lambda_unit": "millimeter",
             "core_diameter_unit": "\u03bcm",
             "ferrule_material": null,
             "name": "Probe C",
             "notes": null,
             "stereotactic_coordinate_ap": null,
-            "stereotactic_coordinate_dv": -1.85,
+            "stereotactic_coordinate_dv": null,
             "stereotactic_coordinate_ml": null,
             "stereotactic_coordinate_reference": "Bregma",
             "stereotactic_coordinate_unit": "millimeter"
         },
         "procedure_type": "Fiber implant",
         "start_date": null,
         "weight_unit": "gram"
@@ -285,15 +285,15 @@
             "bregma_to_lambda_distance": null,
             "bregma_to_lambda_unit": "millimeter",
             "core_diameter_unit": "\u03bcm",
             "ferrule_material": null,
             "name": "Probe D",
             "notes": null,
             "stereotactic_coordinate_ap": null,
-            "stereotactic_coordinate_dv": -1.8,
+            "stereotactic_coordinate_dv": null,
             "stereotactic_coordinate_ml": null,
             "stereotactic_coordinate_reference": "Bregma",
             "stereotactic_coordinate_unit": "millimeter"
         },
         "procedure_type": "Fiber implant",
         "start_date": null,
         "weight_unit": "gram"
```

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item17.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992229992229993%*

 * *Differences: {'2': "{'probes': {'stereotactic_coordinate_dv': None}}",*

 * * '4': "{'probes': {'stereotactic_coordinate_dv': None}}",*

 * * '6': "{'probes': {'stereotactic_coordinate_dv': None}}",*

 * * '8': "{'probes': {'stereotactic_coordinate_dv': None}}"}*

```diff
@@ -78,15 +78,15 @@
             "bregma_to_lambda_distance": null,
             "bregma_to_lambda_unit": "millimeter",
             "core_diameter_unit": "\u03bcm",
             "ferrule_material": null,
             "name": "Probe A",
             "notes": null,
             "stereotactic_coordinate_ap": null,
-            "stereotactic_coordinate_dv": -2.95,
+            "stereotactic_coordinate_dv": null,
             "stereotactic_coordinate_ml": null,
             "stereotactic_coordinate_reference": "Bregma",
             "stereotactic_coordinate_unit": "millimeter"
         },
         "procedure_type": "Fiber implant",
         "start_date": null,
         "weight_unit": "gram"
@@ -147,15 +147,15 @@
             "bregma_to_lambda_distance": null,
             "bregma_to_lambda_unit": "millimeter",
             "core_diameter_unit": "\u03bcm",
             "ferrule_material": null,
             "name": "Probe B",
             "notes": null,
             "stereotactic_coordinate_ap": null,
-            "stereotactic_coordinate_dv": -1.05,
+            "stereotactic_coordinate_dv": null,
             "stereotactic_coordinate_ml": null,
             "stereotactic_coordinate_reference": "Bregma",
             "stereotactic_coordinate_unit": "millimeter"
         },
         "procedure_type": "Fiber implant",
         "start_date": "2022-01-03",
         "weight_unit": "gram"
@@ -216,15 +216,15 @@
             "bregma_to_lambda_distance": null,
             "bregma_to_lambda_unit": "millimeter",
             "core_diameter_unit": "\u03bcm",
             "ferrule_material": null,
             "name": "Probe C",
             "notes": null,
             "stereotactic_coordinate_ap": null,
-            "stereotactic_coordinate_dv": -1.85,
+            "stereotactic_coordinate_dv": null,
             "stereotactic_coordinate_ml": null,
             "stereotactic_coordinate_reference": "Bregma",
             "stereotactic_coordinate_unit": "millimeter"
         },
         "procedure_type": "Fiber implant",
         "start_date": null,
         "weight_unit": "gram"
@@ -285,15 +285,15 @@
             "bregma_to_lambda_distance": null,
             "bregma_to_lambda_unit": "millimeter",
             "core_diameter_unit": "\u03bcm",
             "ferrule_material": null,
             "name": "Probe D",
             "notes": null,
             "stereotactic_coordinate_ap": null,
-            "stereotactic_coordinate_dv": -1.8,
+            "stereotactic_coordinate_dv": null,
             "stereotactic_coordinate_ml": null,
             "stereotactic_coordinate_reference": "Bregma",
             "stereotactic_coordinate_unit": "millimeter"
         },
         "procedure_type": "Fiber implant",
         "start_date": null,
         "weight_unit": "gram"
```

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/mapped/mapped_list_item8.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item10.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/raw/list_item10.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item11.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/raw/list_item11.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item13.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/raw/list_item13.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item14.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/raw/list_item14.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965753424657534%*

 * *Differences: {"'FirstInjectionIsoDuration'": '1.5'}*

```diff
@@ -50,15 +50,15 @@
     "Fiber_x0020_Implant2_x0020_Lengt": "2.5 mm",
     "Fiber_x0020_Implant3_x0020_D_x00": "-1.85",
     "Fiber_x0020_Implant3_x0020_Lengt": null,
     "Fiber_x0020_Implant4_x0020_D_x00": "-1.8",
     "Fiber_x0020_Implant4_x0020_Lengt": "Select...",
     "FileSystemObjectType": 0,
     "FirstInjRecovery": "25",
-    "FirstInjectionIsoDuration": "1.5",
+    "FirstInjectionIsoDuration": 1.5,
     "FirstInjectionWeightAfter": "28.2",
     "FirstInjectionWeightBefor": "25.2",
     "GUID": "cda0b241-be4f-4a14-a7ef-75a01939036a",
     "HPIsoLevel": "2",
     "HPRecovery": "25",
     "HPSurgeonComments": "Went very well",
     "Headpost": "Frontal Ctx",
```

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item15.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/raw/list_item15.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965753424657534%*

 * *Differences: {"'Round1InjIsolevel'": 'None'}*

```diff
@@ -119,15 +119,15 @@
     "PIStringId": "166",
     "PedigreeName": "Gad2-IRES-Cre;Slc32a1-T2A-FlpO;Ai210-hyg",
     "Procedure": "HP Only",
     "Procedure_x0020_Family": "Headpost Only",
     "Procedure_x0020_Slots": "Single surgical session",
     "Procedure_x0020_T2": "Select...",
     "Project_x0020_ID_x0020__x0028_te": "121-01-012-10 Learning mFISH",
-    "Round1InjIsolevel": "Select...",
+    "Round1InjIsolevel": null,
     "ServerRedirectedEmbedUri": null,
     "ServerRedirectedEmbedUrl": "",
     "Sex": "Male",
     "SurgeryStatus": "Ready for Feedback",
     "TEST_x0020_1st_x0020_Round_x0020Id": null,
     "TEST_x0020_1st_x0020_Round_x0020StringId": null,
     "Test1Id": 2846,
```

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item16.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/raw/list_item16.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965753424657534%*

 * *Differences: {"'Round1InjIsolevel'": 'None'}*

```diff
@@ -119,15 +119,15 @@
     "PIStringId": "166",
     "PedigreeName": "Gad2-IRES-Cre;Slc32a1-T2A-FlpO;Ai210-hyg",
     "Procedure": "HP Transcranial",
     "Procedure_x0020_Family": "Headpost Only",
     "Procedure_x0020_Slots": "Single surgical session",
     "Procedure_x0020_T2": "Select...",
     "Project_x0020_ID_x0020__x0028_te": "121-01-012-10 Learning mFISH",
-    "Round1InjIsolevel": "Select...",
+    "Round1InjIsolevel": null,
     "ServerRedirectedEmbedUri": null,
     "ServerRedirectedEmbedUrl": "",
     "Sex": "Male",
     "SurgeryStatus": "Ready for Feedback",
     "TEST_x0020_1st_x0020_Round_x0020Id": null,
     "TEST_x0020_1st_x0020_Round_x0020StringId": null,
     "Test1Id": 2846,
```

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item17.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/raw/list_item17.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965753424657534%*

 * *Differences: {"'Round1InjIsolevel'": 'None'}*

```diff
@@ -119,15 +119,15 @@
     "PIStringId": "166",
     "PedigreeName": "Gad2-IRES-Cre;Slc32a1-T2A-FlpO;Ai210-hyg",
     "Procedure": "HP Transcranial",
     "Procedure_x0020_Family": "Headpost Only",
     "Procedure_x0020_Slots": "Single surgical session",
     "Procedure_x0020_T2": "Select...",
     "Project_x0020_ID_x0020__x0028_te": "121-01-012-10 Learning mFISH",
-    "Round1InjIsolevel": "Select...",
+    "Round1InjIsolevel": null,
     "ServerRedirectedEmbedUri": null,
     "ServerRedirectedEmbedUrl": "",
     "Sex": "Male",
     "SurgeryStatus": "Ready for Feedback",
     "TEST_x0020_1st_x0020_Round_x0020Id": null,
     "TEST_x0020_1st_x0020_Round_x0020StringId": null,
     "Test1Id": 2846,
```

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item8.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/raw/list_item8.json`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/resources/sharepoint/nsb2023/raw/list_item9.json` & `aind_metadata_service-0.4.4/tests/resources/sharepoint/nsb2023/raw/list_item9.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965753424657534%*

 * *Differences: {"'Procedure'": "'Frontal Ctx 2P'"}*

```diff
@@ -114,15 +114,15 @@
     "Modified": "2023-01-03T19:46:31Z",
     "NanojectNumberInj10": "Select...",
     "NanojectNumberInj2": "Select...",
     "OData__UIVersionString": "1",
     "PIId": 166,
     "PIStringId": "166",
     "PedigreeName": "Gad2-IRES-Cre;Slc32a1-T2A-FlpO;Ai210-hyg",
-    "Procedure": "Frontal Ctx 2P (with Headpost)",
+    "Procedure": "Frontal Ctx 2P",
     "Procedure_x0020_Family": "Injection",
     "Procedure_x0020_Slots": "Initial surgery with follow up session",
     "Procedure_x0020_T2": "Select...",
     "Project_x0020_ID_x0020__x0028_te": "121-01-012-10 Learning mFISH",
     "Round1InjIsolevel": "2",
     "ServerRedirectedEmbedUri": null,
     "ServerRedirectedEmbedUrl": "",
```

### Comparing `aind_metadata_service-0.4.3/tests/sharepoint/nsb2019/test_mapping.py` & `aind_metadata_service-0.4.4/tests/sharepoint/nsb2019/test_mapping.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/sharepoint/nsb2019/test_models.py` & `aind_metadata_service-0.4.4/tests/sharepoint/nsb2019/test_models.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/sharepoint/nsb2023/test_mapping.py` & `aind_metadata_service-0.4.4/tests/sharepoint/nsb2023/test_mapping.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,18 +5,24 @@
 import os
 from copy import deepcopy
 from pathlib import Path
 from typing import List, Tuple
 from unittest import TestCase
 from unittest import main as unittest_main
 
-from aind_data_schema.procedures import CraniotomyType, InjectionMaterial
+from aind_data_schema.procedures import BrainInjection, CraniotomyType
 
-from aind_metadata_service.sharepoint.nsb2023.mapping import NSB2023Mapping
-from aind_metadata_service.sharepoint.nsb2023.models import NSBList2023
+from aind_metadata_service.sharepoint.nsb2023.mapping import (
+    BurrHoleInfo,
+    HeadPost,
+    HeadPostInfo,
+    HeadPostType,
+    MappedNSBList,
+)
+from aind_metadata_service.sharepoint.nsb2023.models import NSBList
 
 if os.getenv("LOG_LEVEL"):  # pragma: no cover
     logging.basicConfig(level=os.getenv("LOG_LEVEL"))
 
 TEST_DIR = Path(os.path.dirname(os.path.realpath(__file__))) / ".." / ".."
 DIR_RAW = TEST_DIR / "resources" / "sharepoint" / "nsb2023" / "raw"
 DIR_MAP = TEST_DIR / "resources" / "sharepoint" / "nsb2023" / "mapped"
@@ -58,73 +64,99 @@
         """Checks that raw data is parsed correctly"""
         for list_item in self.list_items:
             raw_data = list_item[0]
             expected_mapped_data = list(list_item[1])
             expected_mapped_data.sort(key=lambda x: str(x))
             raw_file_name = list_item[2]
             logging.debug(f"Processing file: {raw_file_name}")
-            nsb_model = NSBList2023.parse_obj(raw_data)
-            mapper = NSB2023Mapping()
-            mapped_procedure = mapper.map_nsb_model(nsb_model)
+            nsb_model = NSBList.parse_obj(raw_data)
+            mapper = MappedNSBList(nsb=nsb_model)
+            mapped_procedures = mapper.get_procedures()
             mapped_procedure_json = [
-                json.loads(p.json()) for p in mapped_procedure
+                json.loads(p.json()) for p in mapped_procedures
             ]
             mapped_procedure_json.sort(key=lambda x: str(x))
             self.assertEqual(expected_mapped_data, mapped_procedure_json)
 
+    def test_properties(self):
+        """Tests that the properties are parsed correctly."""
+        list_item = self.list_items[0]
+        raw_data = deepcopy(list_item[0])
+        nsb_model = NSBList.parse_obj(raw_data)
+        mapped_model = MappedNSBList(nsb=nsb_model)
+        props = []
+        for k in dir(mapped_model.__class__):
+            cls = mapped_model.__class__
+            attr = getattr(cls, k)
+            if isinstance(attr, property):
+                props.append(getattr(mapped_model, k))
+        self.assertEqual(144, len(props))
+
+    def test_parse_basic_float_str(self):
+        """Tests parsing of basic float strings"""
+        self.assertEqual(MappedNSBList._parse_basic_float_str("0.25"), 0.25)
+        self.assertIsNone(MappedNSBList._parse_basic_float_str("abc"))
+
     def test_craniotomy_edge_case(self):
         """Tests other craniotomy cases"""
 
         # Check WHC type
         list_item = self.list_items[2]
         raw_data = deepcopy(list_item[0])
         raw_data["Procedure"] = "WHC NP"
         raw_data["CraniotomyType"] = "WHC"
-        nsb_model1 = NSBList2023.parse_obj(raw_data)
-        mapper = NSB2023Mapping()
-        mapped_procedure1 = mapper.map_nsb_model(nsb_model1)
+        nsb_model1 = NSBList.parse_obj(raw_data)
+        mapper = MappedNSBList(nsb=nsb_model1)
+        mapped_procedure1 = mapper.get_procedures()
         mapped_procedure1.sort(key=lambda x: str(x))
         cran_proc1 = mapped_procedure1[0]
         self.assertEqual(
             CraniotomyType.WHC, getattr(cran_proc1, "craniotomy_type")
         )
 
         # Check OTHER type
         raw_data["Procedure"] = "WHC NP"
-        raw_data["CraniotomyType"] = "Other"
-        nsb_model2 = NSBList2023.parse_obj(raw_data)
-        mapped_procedure2 = mapper.map_nsb_model(nsb_model2)
+        raw_data["CraniotomyType"] = "Select..."
+        nsb_model2 = NSBList.parse_obj(raw_data)
+        mapper = MappedNSBList(nsb=nsb_model2)
+        mapped_procedure2 = mapper.get_procedures()
         mapped_procedure2.sort(key=lambda x: str(x))
         cran_proc2 = mapped_procedure2[0]
-        self.assertEqual(
-            CraniotomyType.OTHER, getattr(cran_proc2, "craniotomy_type")
+        self.assertIsNone(getattr(cran_proc2, "craniotomy_type"))
+
+    def test_headpost_edge_case(self):
+        """Test edge case for HeadPostInfo class constructor"""
+        hp_info = HeadPostInfo.from_hp_and_hp_type(
+            hp=HeadPost.VISUAL_CTX, hp_type=HeadPostType.MESOSCOPE
+        )
+        exp_hp_info = HeadPostInfo(
+            headframe_type=HeadPost.VISUAL_CTX.value,
+            headframe_part_number="0160-100-10",
+            well_type=HeadPostType.MESOSCOPE.value,
+            well_part_number="0160-200-20",
         )
+        self.assertEqual(exp_hp_info, hp_info)
 
     def test_injection_edge_case(self):
         """Tests the case where there is an INJ procedure, but the inj types
         are malformed. It should create generic BrainInjection objects."""
         list_item = self.list_items[3]
         raw_data = deepcopy(list_item[0])
         raw_data["Inj1Type"] = "Select..."
-        raw_data["ImplantIDCoverslipType"] = "3.5"
-        nsb_model = NSBList2023.parse_obj(raw_data)
-        mapper = NSB2023Mapping()
-        mapped_procedure = mapper.map_nsb_model(nsb_model)
-        mapped_virus_strain = mapper._map_virus_strain_to_materials("abc-def")
-        mapped_virus_strain_none = mapper._map_virus_strain_to_materials(None)
-        mapped_coordinate_ref = mapper._map_ap_info_to_coord_reference(None)
-        self.assertEqual(
-            InjectionMaterial.construct(full_genome_name="abc-def"),
-            mapped_virus_strain,
-        )
-        self.assertIsNone(mapped_virus_strain_none)
-        self.assertIsNone(mapped_coordinate_ref)
-        self.assertIsNotNone(mapped_procedure)
+        nsb_model = NSBList.parse_obj(raw_data)
+        mapper = MappedNSBList(nsb=nsb_model)
+        mapped_procedure = mapper.get_procedures()
+        proc_types = [type(p) for p in mapped_procedure]
+        self.assertTrue(BrainInjection in proc_types)
 
     def test_burr_hole_to_probe_edge_case(self):
-        """Tests edge case where burr hole number is 5"""
-        mapper = NSB2023Mapping()
+        """Tests edge case where burr hole number greater than 4"""
+        list_item = self.list_items[2]
+        raw_data = deepcopy(list_item[0])
+        nsb_model = NSBList.parse_obj(raw_data)
+        mapper = MappedNSBList(nsb=nsb_model)
         self.assertIsNone(mapper._map_burr_hole_number_to_probe(5))
+        self.assertEqual(BurrHoleInfo(), mapper.burr_hole_info(5))
 
 
 if __name__ == "__main__":
     unittest_main()
```

### Comparing `aind_metadata_service-0.4.3/tests/sharepoint/test_client.py` & `aind_metadata_service-0.4.4/tests/sharepoint/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/test_client.py` & `aind_metadata_service-0.4.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `aind_metadata_service-0.4.3/tests/test_response_handle.py` & `aind_metadata_service-0.4.4/tests/test_response_handle.py`

 * *Files identical despite different names*

