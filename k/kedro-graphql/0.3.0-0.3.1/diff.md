# Comparing `tmp/kedro-graphql-0.3.0.tar.gz` & `tmp/kedro-graphql-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-graphql-0.3.0.tar", last modified: Wed May 24 22:27:35 2023, max compression
+gzip compressed data, was "kedro-graphql-0.3.1.tar", last modified: Wed May 31 01:36:28 2023, max compression
```

## Comparing `kedro-graphql-0.3.0.tar` & `kedro-graphql-0.3.1.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.413492 kedro-graphql-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-05-24 22:27:35.413492 kedro-graphql-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-24 22:27:35.413492 kedro-graphql-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.397492 kedro-graphql-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.401492 kedro-graphql-0.3.0/src/kedro_graphql/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.405492 kedro-graphql-0.3.0/src/kedro_graphql/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/backends/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/celeryapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/celeryconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.405492 kedro-graphql-0.3.0/src/kedro_graphql/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/example/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.405492 kedro-graphql-0.3.0/src/kedro_graphql/logs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/logs/json_log_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/logs/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7523 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/pipeline_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.409492 kedro-graphql-0.3.0/src/kedro_graphql/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.409492 kedro-graphql-0.3.0/src/kedro_graphql/pipelines/example00/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/pipelines/example00/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/pipelines/example00/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/pipelines/example00/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.409492 kedro-graphql-0.3.0/src/kedro_graphql/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/plugins/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/kedro_graphql/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.405492 kedro-graphql-0.3.0/src/kedro_graphql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-05-24 22:27:35.000000 kedro-graphql-0.3.0/src/kedro_graphql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-24 22:27:35.000000 kedro-graphql-0.3.0/src/kedro_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 22:27:35.000000 kedro-graphql-0.3.0/src/kedro_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-24 22:27:35.000000 kedro-graphql-0.3.0/src/kedro_graphql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-24 22:27:35.000000 kedro-graphql-0.3.0/src/kedro_graphql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 22:27:35.000000 kedro-graphql-0.3.0/src/kedro_graphql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.409492 kedro-graphql-0.3.0/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.413492 kedro-graphql-0.3.0/src/tests/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/tests/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:35.413492 kedro-graphql-0.3.0/src/tests/pipelines/example00/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/tests/pipelines/example00/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/tests/pipelines/example00/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/tests/test_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/tests/test_schema_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/tests/test_schema_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-24 22:27:23.000000 kedro-graphql-0.3.0/src/tests/test_schema_subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:36:28.893095 kedro-graphql-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-05-31 01:36:28.893095 kedro-graphql-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-31 01:36:28.893095 kedro-graphql-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:36:28.889095 kedro-graphql-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:36:28.889095 kedro-graphql-0.3.1/src/kedro_graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:36:28.889095 kedro-graphql-0.3.1/src/kedro_graphql/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/backends/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/celeryapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/celeryconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:36:28.889095 kedro-graphql-0.3.1/src/kedro_graphql/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/example/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:36:28.889095 kedro-graphql-0.3.1/src/kedro_graphql/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/logs/json_log_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/logs/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/pipeline_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:36:28.893095 kedro-graphql-0.3.1/src/kedro_graphql/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:36:28.893095 kedro-graphql-0.3.1/src/kedro_graphql/pipelines/example00/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/pipelines/example00/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/pipelines/example00/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/pipelines/example00/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:36:28.893095 kedro-graphql-0.3.1/src/kedro_graphql/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/plugins/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/kedro_graphql/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:36:28.889095 kedro-graphql-0.3.1/src/kedro_graphql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-05-31 01:36:28.000000 kedro-graphql-0.3.1/src/kedro_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-31 01:36:28.000000 kedro-graphql-0.3.1/src/kedro_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 01:36:28.000000 kedro-graphql-0.3.1/src/kedro_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-31 01:36:28.000000 kedro-graphql-0.3.1/src/kedro_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-31 01:36:28.000000 kedro-graphql-0.3.1/src/kedro_graphql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-31 01:36:28.000000 kedro-graphql-0.3.1/src/kedro_graphql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:36:28.893095 kedro-graphql-0.3.1/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:36:28.893095 kedro-graphql-0.3.1/src/tests/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/tests/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:36:28.893095 kedro-graphql-0.3.1/src/tests/pipelines/example00/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/tests/pipelines/example00/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/tests/pipelines/example00/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/tests/test_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/tests/test_schema_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/tests/test_schema_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-31 01:36:16.000000 kedro-graphql-0.3.1/src/tests/test_schema_subscription.py
```

### Comparing `kedro-graphql-0.3.0/LICENSE.txt` & `kedro-graphql-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.0/PKG-INFO` & `kedro-graphql-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: kedro-graphql
-Version: 0.3.0
-Summary: Kedro helps you build production-ready data and analytics pipelines
+Version: 0.3.1
+Summary: A kedro plugin for serving any kedro project as a GraphQL api
 Author: opensean
 License: Apache Software License (Apache 2.0)
 Project-URL: Homepage, https://github.com/opensean/kedro-graphql
 Project-URL: Source, https://github.com/opensean/kedro-graphql
 Keywords: pipelines,machine learning,data pipelines,data science,data engineering
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.11,>=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: TEST
 License-File: LICENSE.txt
 
 # kedro-graphql
 
 ## Overview
 
 Kedro-graphql is a [kedro-plugin](https://docs.kedro.org/en/stable/extend_kedro/plugins.html)
```

### Comparing `kedro-graphql-0.3.0/README.md` & `kedro-graphql-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.0/pyproject.toml` & `kedro-graphql-0.3.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "kedro-graphql"
 authors = [
     {name = "opensean"}
 ]
-description = "Kedro helps you build production-ready data and analytics pipelines"
+description = "A kedro plugin for serving any kedro project as a GraphQL api"
 requires-python = ">=3.10, <3.11"
 keywords = [
     "pipelines",
     "machine learning",
     "data pipelines",
     "data science",
     "data engineering",
@@ -24,19 +24,24 @@
 [project.entry-points."kedro.project_commands"]
 kedro-graphql = "kedro_graphql.commands:commands"
 
 [project.urls]
 Homepage = "https://github.com/opensean/kedro-graphql"
 Source = "https://github.com/opensean/kedro-graphql"
 
+[project.optional-dependencies]
+TEST = ["pandas~=2.0.2"] 
+
 [tool.setuptools.dynamic]
 readme = {file = "README.md", content-type = "text/markdown"}
 version = {attr = "kedro_graphql.__version__"}
 dependencies = {file = "src/requirements.txt"}
 
+
+
 [tool.kedro]
 package_name = "kedro_graphql"
 project_name = "kedro-graphql"
 kedro_init_version = "0.18.4"
 
 [tool.isort]
 profile = "black"
```

### Comparing `kedro-graphql-0.3.0/src/kedro_graphql/__main__.py` & `kedro-graphql-0.3.1/src/kedro_graphql/__main__.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.0/src/kedro_graphql/asgi.py` & `kedro-graphql-0.3.1/src/kedro_graphql/asgi.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.0/src/kedro_graphql/backends/base.py` & `kedro-graphql-0.3.1/src/kedro_graphql/backends/base.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.0/src/kedro_graphql/backends/mongodb.py` & `kedro-graphql-0.3.1/src/kedro_graphql/backends/mongodb.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.0/src/kedro_graphql/commands.py` & `kedro-graphql-0.3.1/src/kedro_graphql/commands.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.0/src/kedro_graphql/config.py` & `kedro-graphql-0.3.1/src/kedro_graphql/config.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.0/src/kedro_graphql/decorators.py` & `kedro-graphql-0.3.1/src/kedro_graphql/decorators.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.0/src/kedro_graphql/events.py` & `kedro-graphql-0.3.1/src/kedro_graphql/events.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.0/src/kedro_graphql/example/app.py` & `kedro-graphql-0.3.1/src/kedro_graphql/example/app.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.0/src/kedro_graphql/logs/json_log_formatter.py` & `kedro-graphql-0.3.1/src/kedro_graphql/logs/json_log_formatter.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.0/src/kedro_graphql/logs/logger.py` & `kedro-graphql-0.3.1/src/kedro_graphql/logs/logger.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.0/src/kedro_graphql/models.py` & `kedro-graphql-0.3.1/src/kedro_graphql/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,20 @@
         """
         Returns serializable dict in format compatible with kedro.
         """
         temp = self.__dict__.copy()
         temp.pop("name")
         if not temp["save_args"]:
             temp.pop("save_args")
+        else:
+            temp["save_args"] = {k:v for p in self.__dict__["save_args"] for k,v in p.serialize().items() }
         if not temp["load_args"]:
             temp.pop("load_args")
+        else:
+            temp["load_args"] = {k:v for p in self.__dict__["save_args"] for k,v in p.serialize().items() }
         return {self.name: temp}
 
     @staticmethod
     def from_dict(payload):
         """
         Return a new DataSet from a dictionary.
```

### Comparing `kedro-graphql-0.3.0/src/kedro_graphql/plugins/plugins.py` & `kedro-graphql-0.3.1/src/kedro_graphql/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.0/src/kedro_graphql/schema.py` & `kedro-graphql-0.3.1/src/kedro_graphql/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from strawberry.tools import merge_types
 from strawberry.types import Info
 from typing import AsyncGenerator, List
 from .celeryapp import app as APP_CELERY
 from .tasks import run_pipeline
 from .models import Parameter, DataSet, Pipeline, PipelineInput, PipelineEvent, PipelineLogMessage, PipelineTemplate, Tag
 from .logs.logger import logger, PipelineLogStream
+from fastapi.encoders import jsonable_encoder
 
 @strawberry.type
 class Query:
     @strawberry.field
     def pipeline_templates(self) -> List[PipelineTemplate]:
         pipes = []
         for k,v in PIPELINES.items():
@@ -24,30 +25,19 @@
 
 
 @strawberry.type
 class Mutation:
     @strawberry.mutation
     def pipeline(self, pipeline: PipelineInput, info: Info) -> Pipeline:
         """
-        - fill in missing values from default catalog?
-        - is validation against template needed, e.g. check DataSet type?
+        - is validation against template needed, e.g. check DataSet type or at least check dataset names
         """
-        if pipeline.tags:
-            tags = [Tag(**vars(t)) for t in pipeline.tags]
-        else:
-            tags = None
-
-        p = Pipeline(
-            name = pipeline.name,
-            inputs = [DataSet(**vars(i)) for i in pipeline.inputs],
-            outputs = [DataSet(**vars(o)) for o in pipeline.outputs],
-            parameters = [Parameter(**vars(p)) for p in pipeline.parameters],
-            tags = tags,
-            task_name = str(run_pipeline),
-        )
+        d = jsonable_encoder(pipeline)
+        p = Pipeline.from_dict(d)
+        p.task_name = str(run_pipeline)
 
         serial = p.serialize()
 
         result = run_pipeline.delay(
             name = serial["name"], 
             inputs = serial["inputs"], 
             outputs = serial["outputs"],
```

### Comparing `kedro-graphql-0.3.0/src/kedro_graphql/settings.py` & `kedro-graphql-0.3.1/src/kedro_graphql/settings.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.0/src/kedro_graphql/tasks.py` & `kedro-graphql-0.3.1/src/kedro_graphql/tasks.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.0/src/kedro_graphql.egg-info/PKG-INFO` & `kedro-graphql-0.3.1/src/kedro_graphql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: kedro-graphql
-Version: 0.3.0
-Summary: Kedro helps you build production-ready data and analytics pipelines
+Version: 0.3.1
+Summary: A kedro plugin for serving any kedro project as a GraphQL api
 Author: opensean
 License: Apache Software License (Apache 2.0)
 Project-URL: Homepage, https://github.com/opensean/kedro-graphql
 Project-URL: Source, https://github.com/opensean/kedro-graphql
 Keywords: pipelines,machine learning,data pipelines,data science,data engineering
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: <3.11,>=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: TEST
 License-File: LICENSE.txt
 
 # kedro-graphql
 
 ## Overview
 
 Kedro-graphql is a [kedro-plugin](https://docs.kedro.org/en/stable/extend_kedro/plugins.html)
```

### Comparing `kedro-graphql-0.3.0/src/kedro_graphql.egg-info/SOURCES.txt` & `kedro-graphql-0.3.1/src/kedro_graphql.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 src/kedro_graphql/pipelines/example00/pipeline.py
 src/kedro_graphql/plugins/__init__.py
 src/kedro_graphql/plugins/plugins.py
 src/tests/__init__.py
 src/tests/conftest.py
 src/tests/test_events.py
 src/tests/test_logs.py
+src/tests/test_models.py
 src/tests/test_run.py
 src/tests/test_schema_mutation.py
 src/tests/test_schema_query.py
 src/tests/test_schema_subscription.py
 src/tests/pipelines/__init__.py
 src/tests/pipelines/example00/__init__.py
 src/tests/pipelines/example00/test_pipeline.py
```

### Comparing `kedro-graphql-0.3.0/src/setup.py` & `kedro-graphql-0.3.1/src/setup.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.0/src/tests/conftest.py` & `kedro-graphql-0.3.1/src/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,14 +73,28 @@
 def mock_text_out(tmp_path):
     #tmp_path.mkdir()
     text_out = tmp_path / "text_out.txt"
     text_out.write_text("good bye")
     return text_out
 
 @pytest.fixture
+def mock_text_in_tsv(tmp_path):
+    #tmp_path.mkdir()
+    text = tmp_path / "text_in.tsv"
+    text.write_text("Some parameter\tOther parameter\tLast parameter\nCONST\t123456\t12.45")
+    return text
+
+@pytest.fixture
+def mock_text_out_tsv(tmp_path):
+    #tmp_path.mkdir()
+    text = tmp_path / "text_out.tsv"
+    text.write_text("Some parameter\tOther parameter\tLast parameter\nCONST\t123456\t12.45")
+    return text
+
+@pytest.fixture
 def mock_pipeline(mock_backend, tmp_path, mock_text_in, mock_text_out):
 
     inputs = [{"name": "text_in", "type": "text.TextDataSet", "filepath": str(mock_text_in)}]
     outputs = [{"name":"text_out", "type": "text.TextDataSet", "filepath": str(mock_text_out)}]
     parameters = [{"name":"example", "value":"hello"}]
     tags = [{"key": "author", "value": "opensean"},{"key":"package", "value":"kedro-graphql"}]
```

### Comparing `kedro-graphql-0.3.0/src/tests/test_events.py` & `kedro-graphql-0.3.1/src/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.0/src/tests/test_logs.py` & `kedro-graphql-0.3.1/src/tests/test_logs.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.0/src/tests/test_run.py` & `kedro-graphql-0.3.1/src/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.0/src/tests/test_schema_query.py` & `kedro-graphql-0.3.1/src/tests/test_schema_query.py`

 * *Files identical despite different names*

### Comparing `kedro-graphql-0.3.0/src/tests/test_schema_subscription.py` & `kedro-graphql-0.3.1/src/tests/test_schema_subscription.py`

 * *Files identical despite different names*

