# Comparing `tmp/unify-cli-3.4.1.tar.gz` & `tmp/unify-cli-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unify-cli-3.4.1.tar", last modified: Thu May  4 22:06:41 2023, max compression
+gzip compressed data, was "dist/unify-cli-3.5.0.tar", last modified: Wed May 31 06:48:57 2023, max compression
```

## Comparing `unify-cli-3.4.1.tar` & `unify-cli-3.5.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11358 2023-05-04 22:06:15.000000 unify-cli-3.4.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11718 2023-05-04 22:06:41.000000 unify-cli-3.4.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11321 2023-05-04 22:06:15.000000 unify-cli-3.4.1/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-04 22:06:41.000000 unify-cli-3.4.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3218 2023-05-04 22:06:15.000000 unify-cli-3.4.1/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       33 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/_version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/access/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/access/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2677 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/access/commands.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2293 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/ah.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/cluster/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/cluster/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/cluster/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/common/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/common/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1124 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/common/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/dataset/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/dataset/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4854 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/dataset/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/datastream/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/datastream/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4429 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/datastream/commands.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   485294 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/datastream/tags.csv
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/graph/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/graph/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2413 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/graph/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/hierarchy/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/hierarchy/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2474 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/hierarchy/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/org/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/org/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4929 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/org/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/permissions/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/permissions/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2750 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/permissions/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/permissions/rules/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/permissions/rules/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4854 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/permissions/rules/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/permissions/selectors/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/permissions/selectors/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2209 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/permissions/selectors/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/pipeline/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/pipeline/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1677 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/pipeline/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/template/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/template/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1281 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/template/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/user/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/user/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9262 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/user/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      735 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/utils/util_methods.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/workflow/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/workflow/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9700 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/workflow/commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2289 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/data_test.csv
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1408 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/properties.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2040 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/test_asset_access.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3585 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/test_cluster_command.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4264 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/test_datasets_commands.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2520 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/test_graph_commands.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2292 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/test_help.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      209 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/test_helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1462 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/test_org_command.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2536 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/test_pipeline_commands.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1931 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/test_templates_commands.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4049 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/test_user_commands.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4061 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/test_workflow_commands.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/unify_cli.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11718 2023-05-04 22:06:41.000000 unify-cli-3.4.1/unify_cli.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1585 2023-05-04 22:06:41.000000 unify-cli-3.4.1/unify_cli.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-04 22:06:41.000000 unify-cli-3.4.1/unify_cli.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-05-04 22:06:41.000000 unify-cli-3.4.1/unify_cli.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-05-04 22:06:41.000000 unify-cli-3.4.1/unify_cli.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-04 22:06:41.000000 unify-cli-3.4.1/unify_cli.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:57.000000 unify-cli-3.5.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11358 2023-05-31 06:48:32.000000 unify-cli-3.5.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11718 2023-05-31 06:48:57.000000 unify-cli-3.5.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11321 2023-05-31 06:48:32.000000 unify-cli-3.5.0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-31 06:48:57.000000 unify-cli-3.5.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3562 2023-05-31 06:48:32.000000 unify-cli-3.5.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:57.000000 unify-cli-3.5.0/source/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       33 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/_version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:57.000000 unify-cli-3.5.0/source/access/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/access/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2677 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/access/commands.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2293 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/ah.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:57.000000 unify-cli-3.5.0/source/cluster/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/cluster/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/cluster/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:57.000000 unify-cli-3.5.0/source/common/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/common/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1124 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/common/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:57.000000 unify-cli-3.5.0/source/dataset/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/dataset/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4854 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/dataset/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:57.000000 unify-cli-3.5.0/source/datastream/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/datastream/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4429 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/datastream/commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   485294 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/datastream/tags.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:57.000000 unify-cli-3.5.0/source/graph/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/graph/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2413 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/graph/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:57.000000 unify-cli-3.5.0/source/hierarchy/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/hierarchy/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2474 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/hierarchy/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:57.000000 unify-cli-3.5.0/source/org/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/org/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4929 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/org/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:57.000000 unify-cli-3.5.0/source/permissions/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/permissions/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2750 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/permissions/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:57.000000 unify-cli-3.5.0/source/permissions/rules/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/permissions/rules/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4854 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/permissions/rules/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:57.000000 unify-cli-3.5.0/source/permissions/selectors/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/permissions/selectors/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2209 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/permissions/selectors/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:57.000000 unify-cli-3.5.0/source/pipeline/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/pipeline/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1677 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/pipeline/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:57.000000 unify-cli-3.5.0/source/template/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/template/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1281 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/template/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:57.000000 unify-cli-3.5.0/source/user/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/user/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8883 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/user/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:57.000000 unify-cli-3.5.0/source/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      735 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/utils/util_methods.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:57.000000 unify-cli-3.5.0/source/workflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/workflow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9700 2023-05-31 06:48:32.000000 unify-cli-3.5.0/source/workflow/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:57.000000 unify-cli-3.5.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2289 2023-05-31 06:48:32.000000 unify-cli-3.5.0/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2023-05-31 06:48:32.000000 unify-cli-3.5.0/tests/data_test.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1408 2023-05-31 06:48:32.000000 unify-cli-3.5.0/tests/properties.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2040 2023-05-31 06:48:32.000000 unify-cli-3.5.0/tests/test_asset_access.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3585 2023-05-31 06:48:32.000000 unify-cli-3.5.0/tests/test_cluster_command.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4264 2023-05-31 06:48:32.000000 unify-cli-3.5.0/tests/test_datasets_commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2520 2023-05-31 06:48:32.000000 unify-cli-3.5.0/tests/test_graph_commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2292 2023-05-31 06:48:32.000000 unify-cli-3.5.0/tests/test_help.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      209 2023-05-31 06:48:32.000000 unify-cli-3.5.0/tests/test_helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1462 2023-05-31 06:48:32.000000 unify-cli-3.5.0/tests/test_org_command.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2536 2023-05-31 06:48:32.000000 unify-cli-3.5.0/tests/test_pipeline_commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1931 2023-05-31 06:48:32.000000 unify-cli-3.5.0/tests/test_templates_commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4946 2023-05-31 06:48:32.000000 unify-cli-3.5.0/tests/test_user_commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4061 2023-05-31 06:48:32.000000 unify-cli-3.5.0/tests/test_workflow_commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-31 06:48:57.000000 unify-cli-3.5.0/unify_cli.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11718 2023-05-31 06:48:57.000000 unify-cli-3.5.0/unify_cli.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1585 2023-05-31 06:48:57.000000 unify-cli-3.5.0/unify_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-31 06:48:57.000000 unify-cli-3.5.0/unify_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-05-31 06:48:57.000000 unify-cli-3.5.0/unify_cli.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-05-31 06:48:57.000000 unify-cli-3.5.0/unify_cli.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-31 06:48:57.000000 unify-cli-3.5.0/unify_cli.egg-info/top_level.txt
```

### Comparing `unify-cli-3.4.1/LICENSE` & `unify-cli-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/PKG-INFO` & `unify-cli-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unify-cli
-Version: 3.4.1
+Version: 3.5.0
 Summary: Element Unify command line tool
 Home-page: https://github.com/ElementAnalytics/element-unify-cli
 Author: Element Analytics
 Author-email: platform@ean.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3
```

### Comparing `unify-cli-3.4.1/README.md` & `unify-cli-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/setup.py` & `unify-cli-3.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,58 +26,63 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 
 # Some regexes for parsing semver prerelease tags
 GIT_STANDARD_RE = re.compile('^([1-9][0-9]*)-g([0-9a-z]*)$')
-GIT_EXTRA_RE = re.compile('^.*-([1-9][0-9]*)-g([0-9a-z]*)$')
-def pythonSaneVersion():
+GIT_EXTRA_RE = re.compile('^(.*)-([1-9][0-9]*)-g([0-9a-z]*)$')
+GIT_DIRTY_RE = re.compile('^([1-9][0-9]*)-g([0-9a-z]*-dirty)$')
+def pythonSaneVersion(git_describe):
     """
     Creates a version string that python is happy with.
 
     Python doesn't care for semver syntax, so we need to create a valid string from an arbitrary semver
     """
-    def toNum(non_num):
+    def toPep440(non_num):
         commits = 0
-        hashval = 0
+        hashval = None
         # This is probably of the form -NUMBER-SHA_ABBREV so start there
         std_match = GIT_STANDARD_RE.match(non_num)
         if std_match:
             commits = int(std_match.group(1))
-            hashval = int(std_match.group(2), 16)
-            return commits * hashval
+            hashval = std_match.group(2)
+            return f'dev{commits}+git{hashval}'
 
         extra_match = GIT_EXTRA_RE.match(non_num)
         if extra_match:
-            commits = int(extra_match.group(1))
-            hashval = int(extra_match.group(2), 16)
-            return commits * hashval
+            semver_rel_info = extra_match.group(1)
+            commits = int(extra_match.group(2))
+            hashval = extra_match.group(3)
+            return f'dev{commits}+git{hashval}-{semver_rel_info}'
+
+        dirty_match = GIT_DIRTY_RE.match(non_num)
+        if dirty_match:
+            commits = int(dirty_match.group(1))
+            hashval = dirty_match.group(2)
+            return f'dev{commits}+git{hashval}'
 
-        raise Exception(f"Could not parse the prerelease marker from the semver: {non_num}")
-
-
-    git_describe = os.popen('git describe --dirty').read().strip()
+        raise Exception(f'Could not parse the prerelease marker from the semver: {non_num}')
 
     v = semver.Version.parse(git_describe)
 
     prerelease_clean = None
     if v.prerelease:
-        prerelease_clean = f"dev{toNum(v.prerelease)}"
+        prerelease_clean = toPep440(v.prerelease)
 
     cleaned = semver.Version(
             major=v.major,
             minor=v.minor,
             patch=v.patch,
             prerelease=prerelease_clean
         )
 
     return str(cleaned)
 
-version = pythonSaneVersion()
+version = pythonSaneVersion(os.popen('git describe --dirty').read().strip())
 
 setup(
     name='unify-cli',
     version=str(version),
     description="Element Unify command line tool",
     long_description=README,
     long_description_content_type='text/markdown',
```

### Comparing `unify-cli-3.4.1/source/access/commands.py` & `unify-cli-3.5.0/source/access/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/source/ah.py` & `unify-cli-3.5.0/source/ah.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/source/cluster/commands.py` & `unify-cli-3.5.0/source/cluster/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/source/common/commands.py` & `unify-cli-3.5.0/source/common/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/source/dataset/commands.py` & `unify-cli-3.5.0/source/dataset/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/source/datastream/commands.py` & `unify-cli-3.5.0/source/datastream/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/source/datastream/tags.csv` & `unify-cli-3.5.0/source/datastream/tags.csv`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/source/graph/commands.py` & `unify-cli-3.5.0/source/graph/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/source/hierarchy/commands.py` & `unify-cli-3.5.0/source/hierarchy/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/source/org/commands.py` & `unify-cli-3.5.0/source/org/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/source/permissions/commands.py` & `unify-cli-3.5.0/source/permissions/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/source/permissions/rules/commands.py` & `unify-cli-3.5.0/source/permissions/rules/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/source/permissions/selectors/commands.py` & `unify-cli-3.5.0/source/permissions/selectors/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/source/pipeline/commands.py` & `unify-cli-3.5.0/source/pipeline/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/source/template/commands.py` & `unify-cli-3.5.0/source/template/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/source/user/commands.py` & `unify-cli-3.5.0/source/user/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import json
 import uuid
 import string
+import sys
 import secrets
 import random
 import click
 from tabulate import tabulate
 from unify.apimanager import ApiManager
 from unify.apiutils import tabulate_from_json
 from source.common.commands import org_cluster_options, cluster_option
@@ -28,26 +29,14 @@
 MIN_PW_LEN = 12
 
 @click.group()
 def user():
     """Group for the user related commands"""
     pass
 
-
-@user.command('list')
-@cluster_option
-def user_list(remote):
-    try:
-        response = ApiManager(cluster=remote).orgs.retrieve_all_users()
-        click.echo(click.style(tabulate(response, "keys"), blink=False, bold=True, fg='green'))
-    except Exception as err:
-        click.echo(click.style(str(err), blink=False, bold=True, fg='red'))
-        sys.exit(1)
-
-
 @user.command('org-list')
 @org_cluster_options
 def org_user_list(org, remote):
     try:
         response = ApiManager(cluster=remote).orgs.retrieve_all_users_form_org(org)
         click.echo(click.style(tabulate(response, "keys"), blink=False, bold=True, fg='green'))
     except Exception as err:
@@ -133,43 +122,43 @@
 def machine():
     """Sub-Group under user for the machine user related commands"""
     pass
 
 @machine.command('add')
 @org_cluster_options
 @click.option('--name', help='Machine User Name, defaults to "machine-user-${account-id}"', default=None)
-@click.option('--account-id', help="Machine User ID (UUID format)", default=None)
+@click.option('--account-id', help="User ID (e.g. id from `unify user org-list`)", default=None)
 @click.option('--password', help="Password", default=None)
 @click.option('--role', help="User Role", default='Contributor')
-def service_account_add(org, remote, name, account_id, password, role):
+def machine_user_add(org, remote, name, account_id, password, role):
 
     # Create the name, etc if not supplied
     show_generated_data = False
     if account_id is None:
         show_generated_data = True
-        account_id = uuid.uuid4()
+        account_id = str(uuid.uuid4())
     if name is None:
         show_generated_data = True
-        name = f"machine-user-${account_id}"
+        name = f"machine-user-{account_id}"
     if password is None:
         show_generated_data = True
         password = genValidPw(name)
 
     if show_generated_data:
         click.echo('Copy this and save it somewhere safe like a password manager, as you will not be able to retrieve it in the future!')
         click.echo(f'display name: {name}')
         click.echo(f'account_id: {account_id}')
         click.echo(f'password: {password}')
 
     try:
         response = ApiManager(cluster=remote).orgs.invite_machine_user(
             org_id=org,
-            fullname=service_account_name,
-            id=service_account_id,
-            password=service_account_password,
+            id=account_id,
+            password=password,
+            fullname=name,
             role=role
         )
         click.echo(click.style(str(response), bold=True, fg='green'))
     except Exception as err:
         click.echo(click.style(str(err), bold=True, fg='red'))
         sys.exit(1)
```

### Comparing `unify-cli-3.4.1/source/utils/util_methods.py` & `unify-cli-3.5.0/source/utils/util_methods.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/source/workflow/commands.py` & `unify-cli-3.5.0/source/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/tests/__init__.py` & `unify-cli-3.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/tests/properties.py` & `unify-cli-3.5.0/tests/properties.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/tests/test_asset_access.py` & `unify-cli-3.5.0/tests/test_asset_access.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/tests/test_cluster_command.py` & `unify-cli-3.5.0/tests/test_cluster_command.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/tests/test_datasets_commands.py` & `unify-cli-3.5.0/tests/test_datasets_commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/tests/test_graph_commands.py` & `unify-cli-3.5.0/tests/test_graph_commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/tests/test_help.py` & `unify-cli-3.5.0/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/tests/test_org_command.py` & `unify-cli-3.5.0/tests/test_org_command.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/tests/test_pipeline_commands.py` & `unify-cli-3.5.0/tests/test_pipeline_commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/tests/test_templates_commands.py` & `unify-cli-3.5.0/tests/test_templates_commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/tests/test_user_commands.py` & `unify-cli-3.5.0/tests/test_user_commands.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,93 +16,113 @@
 import unittest
 import logging
 from click.testing import CliRunner
 
 from source.cluster.commands import add_cluster
 from source.cluster.commands import disconnect_cluster
 from source.cluster.commands import login
-from source.user.commands import service_account_add, service_account_add_deprecated, genValidPw
+from source.user.commands import machine_user_add as service_account_add, service_account_add_deprecated, genValidPw
 from tests.properties import Properties
 
 from tests import test_org
 from tests import test_pipeline
 
 import logging
 import sys
 
 logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
 
+# Helpers
+def assert_n_times(times, func, *arg_func, last_ex=None):
+    recompute = lambda f: f() if type(f).__name__ == 'function' else f
+
+    if times <= 0:
+        raise last_ex
+
+    try:
+        func(*list(map(recompute, arg_func)))
+    except Exception as e:
+        return assert_n_times(times - 1, func, *arg_func, last_ex=e)
 
+# Test Cases
 class UserTestCases(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         cls.runner = CliRunner()
         cls.cluster_name = str(uuid.uuid4())[:4]
         cls.props = Properties()
 
         params = [
             "--remote", cls.props.api_url,
             "--username", cls.props.user_name,
             "--password", cls.props.user_password,
             "--name", cls.cluster_name,
             "--assetsync", True
-
         ]
 
         cls.runner.invoke(add_cluster, params)
-
         cls.runner.invoke(login, ["--remote", cls.cluster_name])
 
     def test_service_account_add_admin(self):
         name = str(uuid.uuid4())
-        params = [
-            "--remote", self.cluster_name,
-            "--org", test_org,
-            "--service_account_name",name,
-            "--service_account_id", str(uuid.uuid4()),
-            "--service_account_password", genValidPw(name),
-            "--role", 'Admin'
-        ]
-        add_user_result = self.runner.invoke(service_account_add_deprecated, params)
+        def params():
+            return [
+                        "--remote", self.cluster_name,
+                        "--org", test_org,
+                        "--service_account_name",name,
+                        "--service_account_id", str(uuid.uuid4()),
+                        "--service_account_password", genValidPw(name),
+                        "--role", 'Admin'
+                    ]
+
+        def t(params):
+            add_user_result = self.runner.invoke(service_account_add_deprecated, params)
+            self.assertEqual(add_user_result.exit_code, 0, add_user_result.output)
 
-        self.assertEqual(add_user_result.exit_code, 0, add_user_result.output)
+        assert_n_times(2, t, params)
 
 
     def test_service_account_add_contributor(self):
         name = str(uuid.uuid4())
-        params = [
-            "--remote", self.cluster_name,
-            "--org", test_org,
-            "--service_account_name",name,
-            "--service_account_id", str(uuid.uuid4()),
-            "--service_account_password", genValidPw(name),
-            "--role", 'Contributor'
-        ]
 
-        add_user_result = self.runner.invoke(service_account_add_deprecated, params)
+        def params():
+            return [
+                        "--remote", self.cluster_name,
+                        "--org", test_org,
+                        "--service_account_name",name,
+                        "--service_account_id", str(uuid.uuid4()),
+                        "--service_account_password", genValidPw(name),
+                        "--role", 'Contributor'
+                    ]
+
+        def t(params):
+            add_user_result = self.runner.invoke(service_account_add_deprecated, params)
+            self.assertEqual(add_user_result.exit_code, 0, add_user_result.output)
 
-        self.assertEqual(add_user_result.exit_code, 0, add_user_result.output)
+        assert_n_times(2, t, params)
 
     def test_service_account_add_invalid(self):
         name = str(uuid.uuid4())
-        params = [
-            "--remote", self.cluster_name,
-            "--org", test_org,
-            "--service_account_name",name,
-            "--service_account_id", str(uuid.uuid4()),
-            "--service_account_password", genValidPw(name),
-            "--role", str(uuid.uuid4())
-        ]
-
-        add_user_result = self.runner.invoke(service_account_add_deprecated, params)
-
-        logging.debug(add_user_result)
+        def params():
+            return [
+                        "--remote", self.cluster_name,
+                        "--org", test_org,
+                        "--service_account_name",name,
+                        "--service_account_id", str(uuid.uuid4()),
+                        "--service_account_password", genValidPw(name),
+                        "--role", str(uuid.uuid4())
+                    ]
+
+        def t(params):
+            add_user_result = self.runner.invoke(service_account_add_deprecated, params)
+            logging.debug(add_user_result)
+            self.assertNotEquals(add_user_result.exit_code, 0, add_user_result.output)
 
-        self.assertNotEquals(add_user_result.exit_code, 0, add_user_result.output)
+        assert_n_times(2, t, params)
 
     @unittest.skip('Not yet implemented')
     def test_add_admin_fail(self):
         """
         Try to create an admin user by a non-admin user. This should fail as
         users should not be able to grant more permissions than they have.
         """
```

### Comparing `unify-cli-3.4.1/tests/test_workflow_commands.py` & `unify-cli-3.5.0/tests/test_workflow_commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.4.1/unify_cli.egg-info/PKG-INFO` & `unify-cli-3.5.0/unify_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unify-cli
-Version: 3.4.1
+Version: 3.5.0
 Summary: Element Unify command line tool
 Home-page: https://github.com/ElementAnalytics/element-unify-cli
 Author: Element Analytics
 Author-email: platform@ean.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3
```

### Comparing `unify-cli-3.4.1/unify_cli.egg-info/SOURCES.txt` & `unify-cli-3.5.0/unify_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

