# Comparing `tmp/ke_airflow_dag_generator-0.0.0.tar.gz` & `tmp/ke_airflow_dag_generator-0.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ke_airflow_dag_generator-0.0.0.tar", max compression
+gzip compressed data, was "ke_airflow_dag_generator-0.1.dev1.tar", max compression
```

## Comparing `ke_airflow_dag_generator-0.0.0.tar` & `ke_airflow_dag_generator-0.1.dev1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     7591 2023-05-29 14:50:37.155063 ke_airflow_dag_generator-0.0.0/README.md
--rw-r--r--   0        0        0      203 2023-05-29 14:50:37.155754 ke_airflow_dag_generator-0.0.0/airflow_dag_generator/__init__.py
--rw-r--r--   0        0        0      491 2023-05-29 14:50:37.156374 ke_airflow_dag_generator-0.0.0/airflow_dag_generator/commons/__init__.py
--rw-r--r--   0        0        0      426 2023-05-30 08:24:01.120469 ke_airflow_dag_generator-0.0.0/airflow_dag_generator/commons/generate_dag.py
--rw-r--r--   0        0        0      305 2023-05-30 08:28:43.959875 ke_airflow_dag_generator-0.0.0/airflow_dag_generator/commons/generate_task.py
--rw-r--r--   0        0        0      349 2023-05-29 14:50:37.156873 ke_airflow_dag_generator-0.0.0/airflow_dag_generator/commons/handlers/__init__.py
--rw-r--r--   0        0        0     1015 2023-05-29 14:50:37.157248 ke_airflow_dag_generator-0.0.0/airflow_dag_generator/commons/handlers/clickhouse_execute_operator.py
--rw-r--r--   0        0        0     1513 2023-05-29 14:50:37.157480 ke_airflow_dag_generator-0.0.0/airflow_dag_generator/commons/handlers/postgres_to_clickhouse_operator.py
--rw-r--r--   0        0        0     1334 2023-05-29 14:50:37.157796 ke_airflow_dag_generator-0.0.0/airflow_dag_generator/commons/handlers/sql_to_file_operator.py
--rw-r--r--   0        0        0     1166 2023-05-29 14:50:37.158135 ke_airflow_dag_generator-0.0.0/airflow_dag_generator/config.py
--rw-r--r--   0        0        0      485 2023-05-29 14:50:37.158446 ke_airflow_dag_generator-0.0.0/airflow_dag_generator/exceptions.py
--rw-r--r--   0        0        0     1497 2023-05-29 14:50:37.158800 ke_airflow_dag_generator-0.0.0/airflow_dag_generator/generate_dag.py
--rw-r--r--   0        0        0     1353 2023-05-29 14:50:37.159144 ke_airflow_dag_generator-0.0.0/airflow_dag_generator/generate_task.py
--rw-r--r--   0        0        0     2377 2023-05-29 14:50:37.159470 ke_airflow_dag_generator-0.0.0/airflow_dag_generator/generate_tasks_graph.py
--rw-r--r--   0        0        0      138 2023-05-29 14:50:37.159800 ke_airflow_dag_generator-0.0.0/airflow_dag_generator/macro/__init__.py
--rw-r--r--   0        0        0      381 2023-05-29 14:50:37.160140 ke_airflow_dag_generator-0.0.0/airflow_dag_generator/macro/hooks.py
--rw-r--r--   0        0        0      695 2023-05-29 14:50:37.160462 ke_airflow_dag_generator-0.0.0/airflow_dag_generator/macro/macro.py
--rw-r--r--   0        0        0       69 2023-05-29 14:50:37.160863 ke_airflow_dag_generator-0.0.0/airflow_dag_generator/res/doc_md.template.md
--rw-r--r--   0        0        0       50 2023-05-29 14:50:37.161166 ke_airflow_dag_generator-0.0.0/airflow_dag_generator/res/task_md.template.md
--rw-r--r--   0        0        0      181 2023-05-29 14:50:37.161488 ke_airflow_dag_generator-0.0.0/airflow_dag_generator/schema/__init__.py
--rw-r--r--   0        0        0      899 2023-05-29 14:50:37.161866 ke_airflow_dag_generator-0.0.0/airflow_dag_generator/schema/base.py
--rw-r--r--   0        0        0     2226 2023-05-29 14:50:37.162224 ke_airflow_dag_generator-0.0.0/airflow_dag_generator/schema/dag.py
--rw-r--r--   0        0        0     1445 2023-05-29 14:50:37.162550 ke_airflow_dag_generator-0.0.0/airflow_dag_generator/schema/task.py
--rw-r--r--   0        0        0      653 2023-05-29 14:50:37.162888 ke_airflow_dag_generator-0.0.0/airflow_dag_generator/schema/task_flow.py
--rw-r--r--   0        0        0      853 2023-05-31 02:49:43.418599 ke_airflow_dag_generator-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     8259 1970-01-01 00:00:00.000000 ke_airflow_dag_generator-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     7591 2023-05-29 14:50:37.155063 ke_airflow_dag_generator-0.1.dev1/README.md
+-rw-r--r--   0        0        0      203 2023-05-29 14:50:37.155754 ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/__init__.py
+-rw-r--r--   0        0        0      491 2023-05-29 14:50:37.156374 ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/commons/__init__.py
+-rw-r--r--   0        0        0      426 2023-05-30 08:24:01.120469 ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/commons/generate_dag.py
+-rw-r--r--   0        0        0      305 2023-05-30 08:28:43.959875 ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/commons/generate_task.py
+-rw-r--r--   0        0        0      349 2023-05-29 14:50:37.156873 ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/commons/handlers/__init__.py
+-rw-r--r--   0        0        0     1015 2023-05-29 14:50:37.157248 ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/commons/handlers/clickhouse_execute_operator.py
+-rw-r--r--   0        0        0     1513 2023-05-29 14:50:37.157480 ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/commons/handlers/postgres_to_clickhouse_operator.py
+-rw-r--r--   0        0        0     1334 2023-05-29 14:50:37.157796 ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/commons/handlers/sql_to_file_operator.py
+-rw-r--r--   0        0        0     1166 2023-05-29 14:50:37.158135 ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/config.py
+-rw-r--r--   0        0        0      485 2023-05-29 14:50:37.158446 ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/exceptions.py
+-rw-r--r--   0        0        0     1497 2023-05-29 14:50:37.158800 ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/generate_dag.py
+-rw-r--r--   0        0        0     1353 2023-05-29 14:50:37.159144 ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/generate_task.py
+-rw-r--r--   0        0        0     2377 2023-05-29 14:50:37.159470 ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/generate_tasks_graph.py
+-rw-r--r--   0        0        0      138 2023-05-29 14:50:37.159800 ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/macro/__init__.py
+-rw-r--r--   0        0        0      381 2023-05-29 14:50:37.160140 ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/macro/hooks.py
+-rw-r--r--   0        0        0      695 2023-05-29 14:50:37.160462 ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/macro/macro.py
+-rw-r--r--   0        0        0       69 2023-05-29 14:50:37.160863 ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/res/doc_md.template.md
+-rw-r--r--   0        0        0       50 2023-05-29 14:50:37.161166 ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/res/task_md.template.md
+-rw-r--r--   0        0        0      181 2023-05-29 14:50:37.161488 ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/schema/__init__.py
+-rw-r--r--   0        0        0      899 2023-05-29 14:50:37.161866 ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/schema/base.py
+-rw-r--r--   0        0        0     2226 2023-05-29 14:50:37.162224 ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/schema/dag.py
+-rw-r--r--   0        0        0     1445 2023-05-29 14:50:37.162550 ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/schema/task.py
+-rw-r--r--   0        0        0      653 2023-05-29 14:50:37.162888 ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/schema/task_flow.py
+-rw-r--r--   0        0        0      856 2023-05-31 02:51:01.968093 ke_airflow_dag_generator-0.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0     8262 1970-01-01 00:00:00.000000 ke_airflow_dag_generator-0.1.dev1/PKG-INFO
```

### Comparing `ke_airflow_dag_generator-0.0.0/README.md` & `ke_airflow_dag_generator-0.1.dev1/README.md`

 * *Files identical despite different names*

### Comparing `ke_airflow_dag_generator-0.0.0/airflow_dag_generator/commons/handlers/clickhouse_execute_operator.py` & `ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/commons/handlers/clickhouse_execute_operator.py`

 * *Files identical despite different names*

### Comparing `ke_airflow_dag_generator-0.0.0/airflow_dag_generator/commons/handlers/postgres_to_clickhouse_operator.py` & `ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/commons/handlers/postgres_to_clickhouse_operator.py`

 * *Files identical despite different names*

### Comparing `ke_airflow_dag_generator-0.0.0/airflow_dag_generator/commons/handlers/sql_to_file_operator.py` & `ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/commons/handlers/sql_to_file_operator.py`

 * *Files identical despite different names*

### Comparing `ke_airflow_dag_generator-0.0.0/airflow_dag_generator/config.py` & `ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/config.py`

 * *Files identical despite different names*

### Comparing `ke_airflow_dag_generator-0.0.0/airflow_dag_generator/generate_dag.py` & `ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/generate_dag.py`

 * *Files identical despite different names*

### Comparing `ke_airflow_dag_generator-0.0.0/airflow_dag_generator/generate_task.py` & `ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/generate_task.py`

 * *Files identical despite different names*

### Comparing `ke_airflow_dag_generator-0.0.0/airflow_dag_generator/generate_tasks_graph.py` & `ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/generate_tasks_graph.py`

 * *Files identical despite different names*

### Comparing `ke_airflow_dag_generator-0.0.0/airflow_dag_generator/macro/macro.py` & `ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/macro/macro.py`

 * *Files identical despite different names*

### Comparing `ke_airflow_dag_generator-0.0.0/airflow_dag_generator/schema/base.py` & `ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/schema/base.py`

 * *Files identical despite different names*

### Comparing `ke_airflow_dag_generator-0.0.0/airflow_dag_generator/schema/dag.py` & `ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/schema/dag.py`

 * *Files identical despite different names*

### Comparing `ke_airflow_dag_generator-0.0.0/airflow_dag_generator/schema/task.py` & `ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/schema/task.py`

 * *Files identical despite different names*

### Comparing `ke_airflow_dag_generator-0.0.0/airflow_dag_generator/schema/task_flow.py` & `ke_airflow_dag_generator-0.1.dev1/airflow_dag_generator/schema/task_flow.py`

 * *Files identical despite different names*

### Comparing `ke_airflow_dag_generator-0.0.0/pyproject.toml` & `ke_airflow_dag_generator-0.1.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ke-airflow-dag-generator"
-version = "0.0.0"
+version = "0.1.dev1"
 description = "Python package that implements generating dag from yaml"
 authors = ["markporoshin <m.poroshin@kazanexpress.tech>"]
 readme = "README.md"
 packages = [{include = "airflow_dag_generator"}]
 
 
 [[tool.poetry.source]]
```

### Comparing `ke_airflow_dag_generator-0.0.0/PKG-INFO` & `ke_airflow_dag_generator-0.1.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ke-airflow-dag-generator
-Version: 0.0.0
+Version: 0.1.dev1
 Summary: Python package that implements generating dag from yaml
 Author: markporoshin
 Author-email: m.poroshin@kazanexpress.tech
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

