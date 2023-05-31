# Comparing `tmp/jupysql-0.7.6.tar.gz` & `tmp/jupysql-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupysql-0.7.6.tar", last modified: Mon May 29 17:52:44 2023, max compression
+gzip compressed data, was "jupysql-0.7.7.tar", last modified: Wed May 31 15:14:54 2023, max compression
```

## Comparing `jupysql-0.7.6.tar` & `jupysql-0.7.7.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:52:44.252600 jupysql-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-05-29 17:52:29.000000 jupysql-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-29 17:52:29.000000 jupysql-0.7.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-29 17:52:44.252600 jupysql-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-29 17:52:29.000000 jupysql-0.7.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-29 17:52:29.000000 jupysql-0.7.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-29 17:52:44.252600 jupysql-0.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-29 17:52:29.000000 jupysql-0.7.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:52:44.248600 jupysql-0.7.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:52:44.252600 jupysql-0.7.6/src/jupysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-29 17:52:44.000000 jupysql-0.7.6/src/jupysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-29 17:52:44.000000 jupysql-0.7.6/src/jupysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:52:44.000000 jupysql-0.7.6/src/jupysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:52:44.000000 jupysql-0.7.6/src/jupysql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-29 17:52:44.000000 jupysql-0.7.6/src/jupysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-29 17:52:44.000000 jupysql-0.7.6/src/jupysql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:52:44.252600 jupysql-0.7.6/src/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/column_guesser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    20230 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/error_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:52:44.252600 jupysql-0.7.6/src/sql/ggplot/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/ggplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/ggplot/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/ggplot/facet_wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:52:44.252600 jupysql-0.7.6/src/sql/ggplot/geom/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/ggplot/geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/ggplot/geom/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/ggplot/geom/geom_boxplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/ggplot/geom/geom_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/ggplot/ggplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)    18030 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/magic_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/magic_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)    16139 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    18194 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/store.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:52:44.252600 jupysql-0.7.6/src/sql/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:52:44.252600 jupysql-0.7.6/src/sql/widgets/table_widget/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/widgets/table_widget/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:52:44.252600 jupysql-0.7.6/src/sql/widgets/table_widget/css/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/widgets/table_widget/css/tableWidget.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:52:44.252600 jupysql-0.7.6/src/sql/widgets/table_widget/js/
--rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/widgets/table_widget/js/tableWidget.js
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/widgets/table_widget/table_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-29 17:52:29.000000 jupysql-0.7.6/src/sql/widgets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:54.096138 jupysql-0.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-05-31 15:14:33.000000 jupysql-0.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-31 15:14:33.000000 jupysql-0.7.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-31 15:14:54.096138 jupysql-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-31 15:14:33.000000 jupysql-0.7.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-31 15:14:33.000000 jupysql-0.7.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-31 15:14:54.096138 jupysql-0.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-31 15:14:33.000000 jupysql-0.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:54.080138 jupysql-0.7.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:54.088138 jupysql-0.7.7/src/jupysql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-31 15:14:53.000000 jupysql-0.7.7/src/jupysql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-31 15:14:53.000000 jupysql-0.7.7/src/jupysql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:14:53.000000 jupysql-0.7.7/src/jupysql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:14:53.000000 jupysql-0.7.7/src/jupysql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-31 15:14:53.000000 jupysql-0.7.7/src/jupysql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-31 15:14:53.000000 jupysql-0.7.7/src/jupysql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:54.092138 jupysql-0.7.7/src/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/column_guesser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21805 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/error_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:54.092138 jupysql-0.7.7/src/sql/ggplot/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/ggplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/ggplot/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/ggplot/facet_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:54.096138 jupysql-0.7.7/src/sql/ggplot/geom/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/ggplot/geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/ggplot/geom/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/ggplot/geom/geom_boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/ggplot/geom/geom_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/ggplot/ggplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18100 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/magic_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/magic_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16139 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18171 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:54.096138 jupysql-0.7.7/src/sql/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:54.096138 jupysql-0.7.7/src/sql/widgets/table_widget/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/widgets/table_widget/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:54.096138 jupysql-0.7.7/src/sql/widgets/table_widget/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/widgets/table_widget/css/tableWidget.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:54.096138 jupysql-0.7.7/src/sql/widgets/table_widget/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/widgets/table_widget/js/tableWidget.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/widgets/table_widget/table_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/widgets/utils.py
```

### Comparing `jupysql-0.7.6/LICENSE` & `jupysql-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.6/PKG-INFO` & `jupysql-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql
-Version: 0.7.6
+Version: 0.7.7
 Summary: Better SQL in Jupyter
 Home-page: https://github.com/ploomber/jupysql
 Author: Ploomber
 Author-email: contact@ploomber.io
 Project-URL: Source, https://github.com/ploomber/jupysql
 Keywords: database ipython postgresql mysql duckdb
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupysql Version: 0.7.6 Summary: Better SQL in
+Metadata-Version: 2.1 Name: jupysql Version: 0.7.7 Summary: Better SQL in
 Jupyter Home-page: https://github.com/ploomber/jupysql Author: Ploomber Author-
 email: contact@ploomber.io Project-URL: Source, https://github.com/ploomber/
 jupysql Keywords: database ipython postgresql mysql duckdb Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Topic ::
 Database Classifier: Topic :: Database :: Front-Ends Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `jupysql-0.7.6/README.md` & `jupysql-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.6/pyproject.toml` & `jupysql-0.7.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.6/setup.py` & `jupysql-0.7.7/setup.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.6/src/jupysql.egg-info/PKG-INFO` & `jupysql-0.7.7/src/jupysql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql
-Version: 0.7.6
+Version: 0.7.7
 Summary: Better SQL in Jupyter
 Home-page: https://github.com/ploomber/jupysql
 Author: Ploomber
 Author-email: contact@ploomber.io
 Project-URL: Source, https://github.com/ploomber/jupysql
 Keywords: database ipython postgresql mysql duckdb
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupysql Version: 0.7.6 Summary: Better SQL in
+Metadata-Version: 2.1 Name: jupysql Version: 0.7.7 Summary: Better SQL in
 Jupyter Home-page: https://github.com/ploomber/jupysql Author: Ploomber Author-
 email: contact@ploomber.io Project-URL: Source, https://github.com/ploomber/
 jupysql Keywords: database ipython postgresql mysql duckdb Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Topic ::
 Database Classifier: Topic :: Database :: Front-Ends Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `jupysql-0.7.6/src/jupysql.egg-info/SOURCES.txt` & `jupysql-0.7.7/src/jupysql.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 src/jupysql.egg-info/top_level.txt
 src/sql/__init__.py
 src/sql/_patch.py
 src/sql/_testing.py
 src/sql/column_guesser.py
 src/sql/command.py
 src/sql/connection.py
+src/sql/display.py
 src/sql/error_message.py
 src/sql/exceptions.py
 src/sql/inspect.py
 src/sql/magic.py
 src/sql/magic_cmd.py
 src/sql/magic_plot.py
 src/sql/parse.py
```

### Comparing `jupysql-0.7.6/src/jupysql.egg-info/requires.txt` & `jupysql-0.7.7/src/jupysql.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.6/src/sql/_patch.py` & `jupysql-0.7.7/src/sql/_patch.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.6/src/sql/_testing.py` & `jupysql-0.7.7/src/sql/_testing.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.6/src/sql/column_guesser.py` & `jupysql-0.7.7/src/sql/column_guesser.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.6/src/sql/command.py` & `jupysql-0.7.7/src/sql/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 class SQLCommand:
     """
     Encapsulates the parsing logic (arguments, SQL code, connection string, etc.)
 
     """
 
     def __init__(self, magic, user_ns, line, cell) -> None:
+        self._line = line
+        self._cell = cell
+
         self.args = parse.magic_args(magic.execute, line)
         # self.args.line (everything that appears after %sql/%%sql in the first line)
         # is split in tokens (delimited by spaces), this checks if we have one arg
         one_arg = len(self.args.line) == 1
 
         is_custom_connection_ = (
             Connection.is_custom_connection(user_ns.get(self.args.line[0], False))
@@ -99,7 +102,13 @@
     @property
     def return_result_var(self):
         """Returns the return_result_var"""
         return self.parsed["return_result_var"]
 
     def _var_expand(self, sql, user_ns, magic):
         return Template(sql).render(user_ns)
+
+    def __repr__(self) -> str:
+        return (
+            f"{type(self).__name__}(line={self._line!r}, cell={self._cell!r}) -> "
+            f"({self.sql!r}, {self.sql_original!r})"
+        )
```

### Comparing `jupysql-0.7.6/src/sql/connection.py` & `jupysql-0.7.7/src/sql/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from sqlalchemy.exc import NoSuchModuleError, OperationalError
 from IPython.core.error import UsageError
 import difflib
 import sqlglot
 
 from sql.store import store
 from sql.telemetry import telemetry
-from sql import exceptions
+from sql import exceptions, display
 from sql.error_message import detail
 from ploomber_core.exceptions import modify_exceptions
 
 PLOOMBER_DOCS_LINK_STR = (
     "Documentation: https://jupysql.ploomber.io/en/latest/connecting.html"
 )
 IS_SQLALCHEMY_ONE = int(sqlalchemy.__version__.split(".")[0]) == 1
@@ -149,43 +149,67 @@
 class Connection:
     """Manages connections to databases
 
     Parameters
     ----------
     engine: sqlalchemy.engine.Engine
         The SQLAlchemy engine to use
+
+    Attributes
+    ----------
+    alias : str or None
+        The alias passed in the constructor
+
+    engine : sqlalchemy.engine.Engine
+        The SQLAlchemy engine passed to the constructor
+
+    name : str
+        A name to identify the connection: {user}@{database_name}
+
+    metadata : Metadata or None
+        An SQLAlchemy Metadata object (if using SQLAlchemy 2, this is None),
+        used to retrieve connection information
+
+    url : str
+        An obfuscated connection string (password hidden)
+
+    dialect : sqlalchemy dialect
+        A SQLAlchemy dialect object
+
+    session : sqlalchemy session
+        A SQLAlchemy session object
     """
 
     # the active connection
     current = None
 
     # all connections
     connections = {}
 
     def __init__(self, engine, alias=None):
-        self.url = engine.url
-        self.name = self.assign_name(engine)
-        self.dialect = self.url.get_dialect()
+        self.alias = alias
         self.engine = engine
+        self.name = self.assign_name(engine)
 
         if IS_SQLALCHEMY_ONE:
             self.metadata = sqlalchemy.MetaData(bind=engine)
+        else:
+            self.metadata = None
 
-        url = (
+        self.url = (
             repr(sqlalchemy.MetaData(bind=engine).bind.url)
             if IS_SQLALCHEMY_ONE
             else repr(engine.url)
         )
 
-        self.session = self._create_session(engine, url)
-
-        self.connections[alias or url] = self
+        self.dialect = engine.url.get_dialect()
+        self.session = self._create_session(engine, self.url)
 
+        self.connections[alias or self.url] = self
         self.connect_args = None
-        self.alias = alias
         Connection.current = self
 
     @classmethod
     def _suggest_fix_no_module_found(module_name):
         DEFAULT_PREFIX = "\n\n"
 
         prefix = DEFAULT_PREFIX
@@ -358,16 +382,15 @@
                     creator=creator,
                     alias=alias,
                 )
 
         else:
             if cls.connections:
                 if displaycon:
-                    # display list of connections
-                    print(cls.connection_list())
+                    cls.display_current_connection()
             elif os.getenv("DATABASE_URL"):
                 cls.current = Connection.from_connect_str(
                     connect_str=os.getenv("DATABASE_URL"),
                     connect_args=connect_args,
                     creator=creator,
                     alias=alias,
                 )
@@ -378,35 +401,61 @@
 
     @classmethod
     def assign_name(cls, engine):
         name = "%s@%s" % (engine.url.username or "", engine.url.database)
         return name
 
     @classmethod
-    def connection_list(cls):
-        """Returns the list of connections, appending '*' to the current one"""
-        result = []
+    def _get_connections(cls):
+        """
+        Return a list of dictionaries
+        """
+        connections = []
+
         for key in sorted(cls.connections):
             conn = cls.connections[key]
 
-            if cls.is_custom_connection(conn):
-                engine_url = conn.url
-            else:
-                engine_url = conn.metadata.bind.url if IS_SQLALCHEMY_ONE else conn.url
+            current = conn == cls.current
 
-            prefix = "* " if conn == cls.current else "  "
+            connections.append(
+                {
+                    "current": current,
+                    "key": key,
+                    "url": conn.url,
+                    "alias": conn.alias,
+                    "connection": conn,
+                }
+            )
 
-            if conn.alias:
-                repr_ = f"{prefix} ({conn.alias}) {engine_url!r}"
-            else:
-                repr_ = f"{prefix} {engine_url!r}"
+        return connections
 
-            result.append(repr_)
+    @classmethod
+    def display_current_connection(cls):
+        for conn in cls._get_connections():
+            if conn["current"]:
+                alias = conn.get("alias")
+                if alias:
+                    display.message(f"Running query in {alias!r}")
+                else:
+                    display.message(f"Running query in {conn['url']!r}")
 
-        return "\n".join(result)
+    @classmethod
+    def connections_table(cls):
+        """Returns the current connections as a table"""
+        connections = cls._get_connections()
+
+        def map_values(d):
+            d["current"] = "*" if d["current"] else ""
+            d["alias"] = d["alias"] if d["alias"] else ""
+            return d
+
+        return display.ConnectionsTable(
+            headers=["current", "url", "alias"],
+            rows_maps=[map_values(c) for c in connections],
+        )
 
     @classmethod
     def close(cls, descriptor):
         if isinstance(descriptor, Connection):
             conn = descriptor
         else:
             conn = cls.connections.get(descriptor) or cls.connections.get(
@@ -422,14 +471,23 @@
             cls.connections.pop(descriptor)
         else:
             cls.connections.pop(
                 str(conn.metadata.bind.url) if IS_SQLALCHEMY_ONE else str(conn.url)
             )
             conn.session.close()
 
+    @classmethod
+    def close_all(cls):
+        """Close all active connections"""
+        connections = Connection.connections.copy()
+        for key, conn in connections.items():
+            conn.close(key)
+
+        cls.connections = {}
+
     def is_custom_connection(conn=None) -> bool:
         """
         Checks if given connection is custom
         """
         is_custom_connection_ = False
 
         if conn is None:
```

### Comparing `jupysql-0.7.6/src/sql/error_message.py` & `jupysql-0.7.7/src/sql/error_message.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.6/src/sql/exceptions.py` & `jupysql-0.7.7/src/sql/exceptions.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.6/src/sql/ggplot/facet_wrap.py` & `jupysql-0.7.7/src/sql/ggplot/facet_wrap.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.6/src/sql/ggplot/geom/geom_histogram.py` & `jupysql-0.7.7/src/sql/ggplot/geom/geom_histogram.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.6/src/sql/ggplot/ggplot.py` & `jupysql-0.7.7/src/sql/ggplot/ggplot.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.6/src/sql/inspect.py` & `jupysql-0.7.7/src/sql/inspect.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.6/src/sql/magic.py` & `jupysql-0.7.7/src/sql/magic.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from IPython.core.magic_arguments import argument, magic_arguments, parse_argstring
 from sqlalchemy.exc import OperationalError, ProgrammingError, DatabaseError
 
 import warnings
 import sql.connection
 import sql.parse
 import sql.run
-from sql import exceptions
+from sql import display, exceptions
 from sql.store import store
 from sql.command import SQLCommand
 from sql.magic_plot import SqlPlotMagic
 from sql.magic_cmd import SqlCmdMagic
 from sql._patch import patch_ipython_usage_error
 from ploomber_core.dependencies import check_installed
 
@@ -332,15 +332,15 @@
             print(
                 "Interactive mode, please interact with below "
                 "widget(s) to control the variable"
             )
             interact(interactive_execute_wrapper, **interactive_dict)
             return
         if args.connections:
-            return sql.connection.Connection.connections
+            return sql.connection.Connection.connections_table()
         elif args.close:
             return sql.connection.Connection.close(args.close)
 
         connect_arg = command.connection
 
         if args.section:
             connect_arg = sql.parse.connection_from_dsn_section(args.section, self)
@@ -370,14 +370,15 @@
             connect_arg,
             displaycon=self.displaycon,
             connect_args=args.connection_arguments,
             creator=args.creator,
             alias=args.alias,
         )
         payload["connection_info"] = conn._get_curr_sqlalchemy_connection_info()
+
         if args.persist_replace and args.append:
             raise exceptions.UsageError(
                 """You cannot simultaneously persist and append data to a dataframe;
                   please choose to utilize either one or the other."""
             )
         if args.persist and args.persist_replace:
             warnings.warn("Please use either --persist or --persist-replace")
@@ -418,15 +419,15 @@
                     + str(args.save.replace("-", "_"))
                     + " instead for the save argument.",
                     FutureWarning,
                 )
             self._store.store(args.save, command.sql_original, with_=args.with_)
 
         if args.no_execute:
-            print("Skipping execution...")
+            display.message("Skipping execution...")
             return
 
         try:
             result = sql.run.run(conn, command.sql, self)
 
             if (
                 result is not None
@@ -533,15 +534,15 @@
             )
         except ValueError:
             raise exceptions.ValueError(
                 f"""Table {table_name!r} already exists. Consider using \
 --persist-replace to drop the table before persisting the data frame"""
             )
 
-        return "Persisted %s" % table_name
+        display.message_success(f"Success! Persisted {table_name} to the database.")
 
 
 def load_ipython_extension(ip):
     """Load the extension in IPython."""
 
     # this fails in both Firefox and Chrome for OS X.
     # I get the error: TypeError: IPython.CodeCell.config_defaults is undefined
```

### Comparing `jupysql-0.7.6/src/sql/magic_cmd.py` & `jupysql-0.7.7/src/sql/magic_cmd.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.6/src/sql/magic_plot.py` & `jupysql-0.7.7/src/sql/magic_plot.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.6/src/sql/parse.py` & `jupysql-0.7.7/src/sql/parse.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.6/src/sql/plot.py` & `jupysql-0.7.7/src/sql/plot.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.6/src/sql/run.py` & `jupysql-0.7.7/src/sql/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from io import StringIO
 import html
 
 import prettytable
 import sqlalchemy
 import sqlparse
 from sql.connection import Connection
-from sql import exceptions
+from sql import exceptions, display
 from .column_guesser import ColumnGuesserMixin
 
 try:
     from pgspecial.main import PGSpecial
 except ModuleNotFoundError:
     PGSpecial = None
 from sqlalchemy.orm import Session
@@ -361,20 +361,17 @@
         if filename:
             outfile.close()
             return CsvResultDescriptor(filename)
         else:
             return outfile.getvalue()
 
 
-def interpret_rowcount(rowcount):
-    if rowcount < 0:
-        result = "Done."
-    else:
-        result = "%d rows affected." % rowcount
-    return result
+def display_affected_rowcount(rowcount):
+    if rowcount > 0:
+        display.message_success(f"{rowcount} rows affected.")
 
 
 class FakeResultProxy(object):
     """A fake class that pretends to behave like the ResultProxy from
     SqlAlchemy.
     """
 
@@ -547,15 +544,15 @@
 
             else:
                 result = conn.session.execute(statement)
                 _commit(conn=conn, config=config, manual_commit=manual_commit)
 
                 if result and config.feedback:
                     if hasattr(result, "rowcount"):
-                        print(interpret_rowcount(result.rowcount))
+                        display_affected_rowcount(result.rowcount)
 
     # bypass ResultSet and use duckdb's native method to return a pandas data frame
     if duckdb_autopandas:
         df = cursor.df()
         conn.close()
         return df
     else:
```

### Comparing `jupysql-0.7.6/src/sql/store.py` & `jupysql-0.7.7/src/sql/store.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,31 +101,39 @@
 
     def __str__(self) -> str:
         """
         We use the ' (backtick symbol) to wrap the CTE alias if the dialect supports
         ` (backtick)
         """
         with_clause_template = Template(
-            """WITH{% for name in with_ %} {{name}} AS ({{saved[name]._query}})\
+            """WITH{% for name in with_ %} {{name}} AS ({{rts(saved[name]._query)}})\
 {{ "," if not loop.last }}{% endfor %}{{query}}"""
         )
         with_clause_template_backtick = Template(
-            """WITH{% for name in with_ %} `{{name}}` AS ({{saved[name]._query}})\
+            """WITH{% for name in with_ %} `{{name}}` AS ({{rts(saved[name]._query)}})\
 {{ "," if not loop.last }}{% endfor %}{{query}}"""
         )
         is_use_backtick = sql.connection.Connection.current.is_use_backtick_template()
         with_all = _get_dependencies(self._store, self._with_)
         template = (
             with_clause_template_backtick if is_use_backtick else with_clause_template
         )
         return template.render(
-            query=self._query, saved=self._store._data, with_=with_all
+            query=self._query,
+            saved=self._store._data,
+            with_=with_all,
+            rts=_remove_trailing_semicolon,
         )
 
 
+def _remove_trailing_semicolon(query):
+    query_ = query.rstrip()
+    return query_[:-1] if query_[-1] == ";" else query
+
+
 def _get_dependencies(store, keys):
     """Get a list of all dependencies to reconstruct the CTEs in keys"""
     # get the dependencies for each key
     deps = _flatten([_get_dependencies_for_key(store, key) for key in keys])
     # remove duplicates but preserve order
     return list(dict.fromkeys(deps + keys))
```

### Comparing `jupysql-0.7.6/src/sql/util.py` & `jupysql-0.7.7/src/sql/util.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.6/src/sql/widgets/table_widget/js/tableWidget.js` & `jupysql-0.7.7/src/sql/widgets/table_widget/js/tableWidget.js`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.6/src/sql/widgets/table_widget/table_widget.py` & `jupysql-0.7.7/src/sql/widgets/table_widget/table_widget.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.6/src/sql/widgets/utils.py` & `jupysql-0.7.7/src/sql/widgets/utils.py`

 * *Files identical despite different names*

