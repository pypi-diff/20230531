# Comparing `tmp/datature-1.0.1.tar.gz` & `tmp/datature-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Puppeteer/Puppeteer/pypi/puppeteer/dist/.tmp-9vsg8_24/datature-1.0.1.tar", last modified: Wed Apr 26 10:54:28 2023, max compression
+gzip compressed data, was "/home/runner/work/Puppeteer/Puppeteer/pypi/puppeteer/dist/.tmp-78ndph57/datature-1.0.2.tar", last modified: Wed May 31 09:04:42 2023, max compression
```

## Comparing `datature-1.0.1.tar` & `datature-1.0.2.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-04-26 10:54:17.000000 datature-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 10:54:17.000000 datature-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-26 10:54:28.000000 datature-1.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/datature/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-26 10:54:17.000000 datature-1.0.1/datature/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/datature/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:17.000000 datature-1.0.1/datature/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-26 10:54:17.000000 datature-1.0.1/datature/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-26 10:54:17.000000 datature-1.0.1/datature/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-04-26 10:54:17.000000 datature-1.0.1/datature/cli/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-26 10:54:17.000000 datature-1.0.1/datature/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-26 10:54:17.000000 datature-1.0.1/datature/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/datature/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:17.000000 datature-1.0.1/datature/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-04-26 10:54:17.000000 datature-1.0.1/datature/http/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-26 10:54:17.000000 datature-1.0.1/datature/http/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-26 10:54:17.000000 datature-1.0.1/datature/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-26 10:54:17.000000 datature-1.0.1/datature/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/datature/processor/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-26 10:54:17.000000 datature-1.0.1/datature/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-26 10:54:17.000000 datature-1.0.1/datature/processor/base_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-26 10:54:17.000000 datature-1.0.1/datature/processor/dicom_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-26 10:54:17.000000 datature-1.0.1/datature/processor/nii_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/datature/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15163 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/artifact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/datature/rest/asset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/asset/__int__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/asset/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/asset/upload_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    14570 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/datature/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:17.000000 datature-1.0.1/datature/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-26 10:54:17.000000 datature-1.0.1/datature/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/datature.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-26 10:54:28.000000 datature-1.0.1/datature.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-26 10:54:28.000000 datature-1.0.1/datature.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 10:54:28.000000 datature-1.0.1/datature.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 10:54:28.000000 datature-1.0.1/datature.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-26 10:54:28.000000 datature-1.0.1/datature.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-26 10:54:28.000000 datature-1.0.1/datature.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-26 10:54:17.000000 datature-1.0.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-26 10:54:17.000000 datature-1.0.1/docs/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-26 10:54:17.000000 datature-1.0.1/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 10:54:28.000000 datature-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-26 10:54:17.000000 datature-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:17.000000 datature-1.0.1/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/test/fixture/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:17.000000 datature-1.0.1/test/fixture/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/test/fixture/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:17.000000 datature-1.0.1/test/fixture/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-26 10:54:17.000000 datature-1.0.1/test/fixture/data/error_fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-26 10:54:17.000000 datature-1.0.1/test/fixture/data/operation_fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-26 10:54:17.000000 datature-1.0.1/test/fixture/data/upload_session_fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-26 10:54:17.000000 datature-1.0.1/test/fixture/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/test/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:17.000000 datature-1.0.1/test/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-26 10:54:17.000000 datature-1.0.1/test/http/test_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-26 10:54:17.000000 datature-1.0.1/test/http/test_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/test/rest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:17.000000 datature-1.0.1/test/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-04-26 10:54:17.000000 datature-1.0.1/test/rest/test_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-26 10:54:17.000000 datature-1.0.1/test/rest/test_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-26 10:54:17.000000 datature-1.0.1/test/rest/test_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-04-26 10:54:17.000000 datature-1.0.1/test/rest/test_asset_upload_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-26 10:54:17.000000 datature-1.0.1/test/rest/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-26 10:54:17.000000 datature-1.0.1/test/rest/test_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-26 10:54:17.000000 datature-1.0.1/test/rest/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-26 10:54:17.000000 datature-1.0.1/test/rest/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-26 10:54:17.000000 datature-1.0.1/test/rest/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-26 10:54:17.000000 datature-1.0.1/test/rest/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 10:54:17.000000 datature-1.0.1/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-26 10:54:17.000000 datature-1.0.1/test/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-05-31 09:04:27.000000 datature-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-31 09:04:27.000000 datature-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-31 09:04:42.000000 datature-1.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/datature/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-31 09:04:27.000000 datature-1.0.2/datature/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/datature/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:27.000000 datature-1.0.2/datature/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-05-31 09:04:27.000000 datature-1.0.2/datature/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-05-31 09:04:27.000000 datature-1.0.2/datature/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-05-31 09:04:27.000000 datature-1.0.2/datature/cli/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-31 09:04:27.000000 datature-1.0.2/datature/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-31 09:04:27.000000 datature-1.0.2/datature/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/datature/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:27.000000 datature-1.0.2/datature/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-31 09:04:27.000000 datature-1.0.2/datature/http/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-31 09:04:27.000000 datature-1.0.2/datature/http/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-31 09:04:27.000000 datature-1.0.2/datature/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-31 09:04:27.000000 datature-1.0.2/datature/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/datature/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-31 09:04:27.000000 datature-1.0.2/datature/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-31 09:04:27.000000 datature-1.0.2/datature/processor/base_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-31 09:04:27.000000 datature-1.0.2/datature/processor/dicom_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-31 09:04:27.000000 datature-1.0.2/datature/processor/nii_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/datature/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15223 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/artifact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/datature/rest/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/asset/__int__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/asset/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/asset/upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14570 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-31 09:04:27.000000 datature-1.0.2/datature/rest/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/datature/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:27.000000 datature-1.0.2/datature/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-31 09:04:27.000000 datature-1.0.2/datature/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/datature.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-31 09:04:42.000000 datature-1.0.2/datature.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-31 09:04:42.000000 datature-1.0.2/datature.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:04:42.000000 datature-1.0.2/datature.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-31 09:04:42.000000 datature-1.0.2/datature.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-31 09:04:42.000000 datature-1.0.2/datature.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-31 09:04:42.000000 datature-1.0.2/datature.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-31 09:04:27.000000 datature-1.0.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-31 09:04:27.000000 datature-1.0.2/docs/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-31 09:04:27.000000 datature-1.0.2/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 09:04:42.000000 datature-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-31 09:04:27.000000 datature-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:27.000000 datature-1.0.2/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/test/fixture/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:27.000000 datature-1.0.2/test/fixture/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/test/fixture/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:27.000000 datature-1.0.2/test/fixture/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-31 09:04:27.000000 datature-1.0.2/test/fixture/data/error_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-31 09:04:27.000000 datature-1.0.2/test/fixture/data/operation_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-31 09:04:27.000000 datature-1.0.2/test/fixture/data/upload_session_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-31 09:04:27.000000 datature-1.0.2/test/fixture/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/test/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:27.000000 datature-1.0.2/test/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-31 09:04:27.000000 datature-1.0.2/test/http/test_requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-31 09:04:27.000000 datature-1.0.2/test/http/test_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:42.000000 datature-1.0.2/test/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:04:27.000000 datature-1.0.2/test/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-05-31 09:04:27.000000 datature-1.0.2/test/rest/test_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-31 09:04:27.000000 datature-1.0.2/test/rest/test_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-31 09:04:27.000000 datature-1.0.2/test/rest/test_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-05-31 09:04:27.000000 datature-1.0.2/test/rest/test_asset_upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-31 09:04:27.000000 datature-1.0.2/test/rest/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-31 09:04:27.000000 datature-1.0.2/test/rest/test_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-31 09:04:27.000000 datature-1.0.2/test/rest/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-31 09:04:27.000000 datature-1.0.2/test/rest/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-31 09:04:27.000000 datature-1.0.2/test/rest/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-31 09:04:27.000000 datature-1.0.2/test/rest/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-31 09:04:27.000000 datature-1.0.2/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 09:04:27.000000 datature-1.0.2/test/test_logger.py
```

### Comparing `datature-1.0.1/LICENSE` & `datature-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/PKG-INFO` & `datature-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datature
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python bindings for the Datature API
 Author: Raighne Weng
 Author-email: raighne@datature.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `datature-1.0.1/datature/__init__.py` & `datature-1.0.2/datature/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   __init__.py
 @Author  :   Raighne.Weng
-@Version :   1.0.0
+@Version :   1.0.2
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   init module, include global configuration
 '''
 
 # Global Configuration
 API_BASE_URL = "https://api.datature.io/v1"
-SDK_VERSION = "1.0.1"
+SDK_VERSION = "1.0.2"
 
 # Constant environment
 OPERATION_LOOPING_TIMES = 20
 ASSET_UPLOAD_BATCH_SIZE = 5000
 SHOW_PROGRESS = False
 OPERATION_LOOPING_DELAY_SECONDS = 5
 HTTP_TIMEOUT_SECONDS = 120
```

### Comparing `datature-1.0.1/datature/cli/commands.py` & `datature-1.0.2/datature/cli/commands.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/datature/cli/config.py` & `datature-1.0.2/datature/cli/config.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/datature/cli/functions.py` & `datature-1.0.2/datature/cli/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,25 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   functions.py
 @Author  :   Raighne.Weng
-@Version :   0.7.6
+@Version :   1.0.2
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   CLI functions
 '''
 
 import os
 import re
 import sys
 import time
-from os.path import basename, exists, isfile, join
+from os.path import basename, exists, join
 from pathlib import Path
 from typing import Optional
 
 import inquirer
 import requests
 from halo import Halo
 from alive_progress import alive_bar
@@ -259,18 +259,14 @@
         questions = [
             inquirer.Path("path_result",
                           message=messages.ANNOTATION_FOLDER_MESSAGE),
         ]
         answer = inquirer.prompt(questions, raise_keyboard_interrupt=True)
         path = answer.get("path_result")
 
-    if not isfile(path):
-        print(messages.PATH_NOT_EXISTS_MESSAGE)
-        sys.exit(1)
-
     if not annotation_format:
         questions = [
             inquirer.List(
                 "annotation_format",
                 message=messages.ANNOTATION_FORMAT_MESSAGE,
                 choices=[format.value for format in AnnotationFormat],
             ),
```

### Comparing `datature-1.0.1/datature/cli/main.py` & `datature-1.0.2/datature/cli/main.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/datature/error.py` & `datature-1.0.2/datature/error.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/datature/http/requester.py` & `datature-1.0.2/datature/http/requester.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/datature/http/resource.py` & `datature-1.0.2/datature/http/resource.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/datature/logger.py` & `datature-1.0.2/datature/logger.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/datature/messages.py` & `datature-1.0.2/datature/messages.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/datature/processor/__init__.py` & `datature-1.0.2/datature/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/datature/processor/base_processor.py` & `datature-1.0.2/datature/processor/base_processor.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/datature/processor/dicom_processor.py` & `datature-1.0.2/datature/processor/dicom_processor.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/datature/processor/nii_processor.py` & `datature-1.0.2/datature/processor/nii_processor.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/datature/rest/__init__.py` & `datature-1.0.2/datature/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/datature/rest/annotation.py` & `datature-1.0.2/datature/rest/annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,26 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   annotation.py
 @Author  :   Raighne.Weng
-@Version :   0.1.0
+@Version :   1.0.2
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Datature Annotation API
 '''
 
-from os.path import exists
-
-from datature.error import Error
+from datature.utils import utils
 from datature.http.resource import RESTResource
 from datature.rest.operation import Operation
-from datature.rest.types import (
-    AnnotationExportOptions,
-    AnnotationFormat,
-    AnnotationMetadata,
-)
+from datature.rest.types import (AnnotationExportOptions, AnnotationFormat,
+                                 AnnotationMetadata)
+
 
 
 class Annotation(RESTResource):
     """Datature Annotation API Resource."""
 
     @classmethod
     def list(cls, asset_id: str) -> dict:
@@ -311,15 +307,15 @@
     def upload(cls,
                annotation_format: AnnotationFormat,
                file_path: str,
                background=False) -> dict:
         """Uploads annotations to project.
 
         :param annotation_format: The annotation format for bounding boxes or polygons as a string.
-        :param file_path: The file path containing the annotation metadata to be uploaded. The file contents should match the annotation format specified.
+        :param file_path: The file path or folder containing the annotation metadata to be uploaded. The file contents should match the annotation format specified.
         :param background: Signal to complete the annotation upload process in the background. Defaults to False.
         :return: A dictionary containing the operation metadata of the annotation upload with the following structure:
 
                 .. code-block:: json
                         {
                             "id": "op_508fc5d1-e908-486d-9e7b-1dca99b80024",
                             "object": "operation",
@@ -348,27 +344,26 @@
                         import datature
 
                         datature.secret_key = "5aa41e8ba........"
 
                         datature.Annotation.upload("csv_fourcorner",
                                                 "Your file path")
         """
-        file_exists = exists(file_path)
-
-        if not file_exists:
-            raise Error("Could not find the Asset file")
-
-        with open(file_path, "rb") as file:
-            files = [('files', file)]
+        upload_paths = utils.find_all_annotations_files(file_path, annotation_format)
 
-            response = cls.request(
-                "POST",
-                "/annotation/import",
-                query={"format": annotation_format},
-                request_files=files,
-            )
+        upload_list =[]
+        for upload_path in upload_paths:
+            with open(upload_path, "rb") as file:
+                upload_list.append(('files', (file.name, file.read(), 'application/octet-stream')))
+
+        response = cls.request(
+            "POST",
+            "/annotation/import",
+            query={"format": annotation_format},
+            request_files=upload_list,
+        )
 
-            if background:
-                return response
+        if background:
+            return response
 
-            op_link = response["op_link"]
-            return Operation.loop_retrieve(op_link)
+        op_link = response["op_link"]
+        return Operation.loop_retrieve(op_link)
```

### Comparing `datature-1.0.1/datature/rest/artifact.py` & `datature-1.0.2/datature/rest/artifact.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/datature/rest/asset/asset.py` & `datature-1.0.2/datature/rest/asset/asset.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/datature/rest/asset/upload_session.py` & `datature-1.0.2/datature/rest/asset/upload_session.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/datature/rest/deploy.py` & `datature-1.0.2/datature/rest/deploy.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/datature/rest/operation.py` & `datature-1.0.2/datature/rest/operation.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/datature/rest/project.py` & `datature-1.0.2/datature/rest/project.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/datature/rest/run.py` & `datature-1.0.2/datature/rest/run.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/datature/rest/tag.py` & `datature-1.0.2/datature/rest/tag.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/datature/rest/types.py` & `datature-1.0.2/datature/rest/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   ████
 ██    ██   Datature
   ██  ██   Powering Breakthrough AI
     ██
 
 @File    :   types.py
 @Author  :   Raighne.Weng
-@Version :   0.7.2
+@Version :   1.0.2
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Types for Datature API resources.
 '''
 
 from enum import Enum
 from dataclasses import dataclass
@@ -83,34 +83,38 @@
     status: str
     custom_metadata: object
 
 class AnnotationFormat(Enum):
     """Annotation CSV Format.
 
     Bounding Box Options:
+        coco
         csv_fourcorner
         csv_widthheight
-        coco
         pascal_voc
-        yolo_keras_pytorch
         yolo_darknet
+        yolo_keras_pytorch
+        createml
+        tfrecord
 
     Polygon Options:
         polygon_single
         polygon_coco
     """
 
+    COCO = "coco"
     CSV_FOURCORNER = "csv_fourcorner"
     CSV_WIDTHHEIGHT = "csv_widthheight"
-    COCO = "coco"
     PASCAL_VOC = "pascal_voc"
-    YOLO_KERAS_PYTORCH = "yolo_keras_pytorch"
     YOLO_DARKNET = "yolo_darknet"
-    POLYGON_SINGLE = "polygon_single"
+    YOLO_KERAS_PYTORCH = "yolo_keras_pytorch"
+    CREATEML = "createml"
+    TFRECORD = "tfrecord"
     POLYGON_COCO = "polygon_coco"
+    POLYGON_SINGLE = "polygon_single"
 
 
 @dataclass
 class DeploymentMetadata:
     """Deployment Settings Metadata.
 
     :param name: The name of the deployment instance.
```

### Comparing `datature-1.0.1/datature/rest/workflow.py` & `datature-1.0.2/datature/rest/workflow.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/datature.egg-info/PKG-INFO` & `datature-1.0.2/datature.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datature
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python bindings for the Datature API
 Author: Raighne Weng
 Author-email: raighne@datature.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `datature-1.0.1/datature.egg-info/SOURCES.txt` & `datature-1.0.2/datature.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/docs/source/conf.py` & `datature-1.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/docs/upload.py` & `datature-1.0.2/docs/upload.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/readme.md` & `datature-1.0.2/readme.md`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/setup.py` & `datature-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/test/fixture/data/error_fixture.py` & `datature-1.0.2/test/fixture/data/error_fixture.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/test/fixture/data/operation_fixture.py` & `datature-1.0.2/test/fixture/data/operation_fixture.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/test/fixture/data/upload_session_fixture.py` & `datature-1.0.2/test/fixture/data/upload_session_fixture.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/test/fixture/mock.py` & `datature-1.0.2/test/fixture/mock.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/test/http/test_requester.py` & `datature-1.0.2/test/http/test_requester.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/test/http/test_resource.py` & `datature-1.0.2/test/http/test_resource.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/test/rest/test_annotation.py` & `datature-1.0.2/test/rest/test_annotation.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/test/rest/test_artifact.py` & `datature-1.0.2/test/rest/test_artifact.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/test/rest/test_asset.py` & `datature-1.0.2/test/rest/test_asset.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/test/rest/test_asset_upload_session.py` & `datature-1.0.2/test/rest/test_asset_upload_session.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/test/rest/test_deploy.py` & `datature-1.0.2/test/rest/test_deploy.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/test/rest/test_operation.py` & `datature-1.0.2/test/rest/test_operation.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/test/rest/test_project.py` & `datature-1.0.2/test/rest/test_project.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/test/rest/test_run.py` & `datature-1.0.2/test/rest/test_run.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/test/rest/test_tag.py` & `datature-1.0.2/test/rest/test_tag.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/test/rest/test_workflow.py` & `datature-1.0.2/test/rest/test_workflow.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/test/test_error.py` & `datature-1.0.2/test/test_error.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.1/test/test_logger.py` & `datature-1.0.2/test/test_logger.py`

 * *Files identical despite different names*

