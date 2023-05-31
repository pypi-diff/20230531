# Comparing `tmp/xaiographs-1.0.0.tar.gz` & `tmp/XAIoGraphs-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xaiographs-1.0.0.tar", last modified: Wed May 31 14:26:39 2023, max compression
+gzip compressed data, was "XAIoGraphs-1.0.1.tar", last modified: Wed May 31 14:24:28 2023, max compression
```

## Comparing `xaiographs-1.0.0.tar` & `XAIoGraphs-1.0.1.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.951216 xaiographs-1.0.0/
--rw-r--r--   0 rmg        (503) staff       (20)    34522 2023-05-30 08:46:10.000000 xaiographs-1.0.0/LICENSE
--rw-r--r--   0 rmg        (503) staff       (20)       63 2023-05-30 08:46:10.000000 xaiographs-1.0.0/MANIFEST.in
--rw-r--r--   0 rmg        (503) staff       (20)     5453 2023-05-31 14:26:39.951040 xaiographs-1.0.0/PKG-INFO
--rw-r--r--   0 rmg        (503) staff       (20)     5031 2023-05-31 14:19:12.000000 xaiographs-1.0.0/README.md
--rw-r--r--   0 rmg        (503) staff       (20)        6 2023-05-31 14:26:06.000000 xaiographs-1.0.0/VERSION
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.898396 xaiographs-1.0.0/XAIoGraphs.egg-info/
--rw-r--r--   0 rmg        (503) staff       (20)     5453 2023-05-31 14:26:39.000000 xaiographs-1.0.0/XAIoGraphs.egg-info/PKG-INFO
--rw-r--r--   0 rmg        (503) staff       (20)     6184 2023-05-31 14:26:39.000000 xaiographs-1.0.0/XAIoGraphs.egg-info/SOURCES.txt
--rw-r--r--   0 rmg        (503) staff       (20)        1 2023-05-31 14:26:39.000000 xaiographs-1.0.0/XAIoGraphs.egg-info/dependency_links.txt
--rw-r--r--   0 rmg        (503) staff       (20)      280 2023-05-31 14:26:39.000000 xaiographs-1.0.0/XAIoGraphs.egg-info/entry_points.txt
--rw-r--r--   0 rmg        (503) staff       (20)       75 2023-05-31 14:26:39.000000 xaiographs-1.0.0/XAIoGraphs.egg-info/requires.txt
--rw-r--r--   0 rmg        (503) staff       (20)       11 2023-05-31 14:26:39.000000 xaiographs-1.0.0/XAIoGraphs.egg-info/top_level.txt
--rw-r--r--   0 rmg        (503) staff       (20)       38 2023-05-31 14:26:39.951278 xaiographs-1.0.0/setup.cfg
--rw-r--r--   0 rmg        (503) staff       (20)     2013 2023-05-31 14:26:28.000000 xaiographs-1.0.0/setup.py
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.899367 xaiographs-1.0.0/xaiographs/
--rw-r--r--   0 rmg        (503) staff       (20)     6148 2023-04-03 12:27:00.000000 xaiographs-1.0.0/xaiographs/.DS_Store
--rw-r--r--   0 rmg        (503) staff       (20)      852 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/__init__.py
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.902222 xaiographs-1.0.0/xaiographs/__pycache__/
--rw-r--r--   0 rmg        (503) staff       (20)      316 2023-03-09 13:56:14.000000 xaiographs-1.0.0/xaiographs/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 rmg        (503) staff       (20)     1043 2023-05-30 11:04:13.000000 xaiographs-1.0.0/xaiographs/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rmg        (503) staff       (20)      320 2023-03-02 12:32:11.000000 xaiographs-1.0.0/xaiographs/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 rmg        (503) staff       (20)    63370 2023-03-16 09:06:51.000000 xaiographs-1.0.0/xaiographs/__pycache__/fairness.cpython-37.pyc
--rw-r--r--   0 rmg        (503) staff       (20)    45853 2023-05-30 11:05:09.000000 xaiographs-1.0.0/xaiographs/__pycache__/fairness.cpython-38.pyc
--rw-r--r--   0 rmg        (503) staff       (20)    63378 2023-03-17 11:01:49.000000 xaiographs-1.0.0/xaiographs/__pycache__/fairness.cpython-39.pyc
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.903704 xaiographs-1.0.0/xaiographs/common/
--rw-r--r--   0 rmg        (503) staff       (20)      732 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/common/__init__.py
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.906493 xaiographs-1.0.0/xaiographs/common/__pycache__/
--rw-r--r--   0 rmg        (503) staff       (20)      200 2023-03-09 13:56:23.000000 xaiographs-1.0.0/xaiographs/common/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 rmg        (503) staff       (20)      918 2023-05-30 11:04:37.000000 xaiographs-1.0.0/xaiographs/common/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rmg        (503) staff       (20)      204 2023-03-02 12:32:49.000000 xaiographs-1.0.0/xaiographs/common/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 rmg        (503) staff       (20)      759 2023-03-09 13:56:23.000000 xaiographs-1.0.0/xaiographs/common/__pycache__/constants.cpython-37.pyc
--rw-r--r--   0 rmg        (503) staff       (20)     1482 2023-05-30 11:04:37.000000 xaiographs-1.0.0/xaiographs/common/__pycache__/constants.cpython-38.pyc
--rw-r--r--   0 rmg        (503) staff       (20)      763 2023-03-17 11:01:38.000000 xaiographs-1.0.0/xaiographs/common/__pycache__/constants.cpython-39.pyc
--rw-r--r--   0 rmg        (503) staff       (20)     8927 2023-03-09 13:56:23.000000 xaiographs-1.0.0/xaiographs/common/__pycache__/utils.cpython-37.pyc
--rw-r--r--   0 rmg        (503) staff       (20)     9697 2023-05-30 11:04:37.000000 xaiographs-1.0.0/xaiographs/common/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0 rmg        (503) staff       (20)     8946 2023-03-02 12:32:49.000000 xaiographs-1.0.0/xaiographs/common/__pycache__/utils.cpython-39.pyc
--rwxr-xr-x   0 rmg        (503) staff       (20)     1221 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/common/constants.py
--rwxr-xr-x   0 rmg        (503) staff       (20)     9886 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/common/utils.py
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.907595 xaiographs-1.0.0/xaiographs/datasets/
--rw-r--r--   0 rmg        (503) staff       (20)     6148 2023-04-03 14:11:53.000000 xaiographs-1.0.0/xaiographs/datasets/.DS_Store
--rw-r--r--   0 rmg        (503) staff       (20)     1168 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/datasets/__init__.py
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.911725 xaiographs-1.0.0/xaiographs/datasets/__pycache__/
--rw-r--r--   0 rmg        (503) staff       (20)      333 2023-03-09 15:31:10.000000 xaiographs-1.0.0/xaiographs/datasets/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 rmg        (503) staff       (20)     1367 2023-04-27 15:53:46.000000 xaiographs-1.0.0/xaiographs/datasets/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rmg        (503) staff       (20)      337 2023-03-17 11:01:50.000000 xaiographs-1.0.0/xaiographs/datasets/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 rmg        (503) staff       (20)     9233 2023-03-09 15:31:10.000000 xaiographs-1.0.0/xaiographs/datasets/__pycache__/datasets.cpython-37.pyc
--rw-r--r--   0 rmg        (503) staff       (20)    32863 2023-05-17 08:39:50.000000 xaiographs-1.0.0/xaiographs/datasets/__pycache__/datasets.cpython-38.pyc
--rw-r--r--   0 rmg        (503) staff       (20)     9257 2023-03-17 11:01:50.000000 xaiographs-1.0.0/xaiographs/datasets/__pycache__/datasets.cpython-39.pyc
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.890177 xaiographs-1.0.0/xaiographs/datasets/data/
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.918221 xaiographs-1.0.0/xaiographs/datasets/data/body_performance/
--rw-r--r--   0 rmg        (503) staff       (20)  1021936 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/datasets/data/body_performance/dataset.csv
--rw-r--r--   0 rmg        (503) staff       (20)  1880577 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/datasets/data/body_performance/dataset_discretized.csv
--rw-r--r--   0 rmg        (503) staff       (20)     8367 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/datasets/data/body_performance/target_value_semantics_es.csv
--rw-r--r--   0 rmg        (503) staff       (20)     7207 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/datasets/data/body_performance/target_values_semantics_en.csv
--rw-r--r--   0 rmg        (503) staff       (20)     1857 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/datasets/data/body_performance/values_semantics_en.csv
--rw-r--r--   0 rmg        (503) staff       (20)     2236 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/datasets/data/body_performance/values_semantics_es.csv
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.920537 xaiographs-1.0.0/xaiographs/datasets/data/education_performance/
--rw-r--r--   0 rmg        (503) staff       (20)     9647 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/datasets/data/education_performance/dataset.csv
--rw-r--r--   0 rmg        (503) staff       (20)    37851 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/datasets/data/education_performance/dataset_discretized.csv
--rw-r--r--   0 rmg        (503) staff       (20)    15504 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/datasets/data/education_performance/target_values_semantics_en.csv
--rw-r--r--   0 rmg        (503) staff       (20)    17204 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/datasets/data/education_performance/target_values_semantics_es.csv
--rw-r--r--   0 rmg        (503) staff       (20)     3051 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/datasets/data/education_performance/values_semantics_en.csv
--rw-r--r--   0 rmg        (503) staff       (20)     3402 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/datasets/data/education_performance/values_semantics_es.csv
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.922236 xaiographs-1.0.0/xaiographs/datasets/data/titanic/
--rw-r--r--   0 rmg        (503) staff       (20)    46398 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/datasets/data/titanic/dataset.csv
--rw-r--r--   0 rmg        (503) staff       (20)    84285 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/datasets/data/titanic/dataset_discretized.csv
--rw-r--r--   0 rmg        (503) staff       (20)     1998 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/datasets/data/titanic/target_values_semantics_en.csv
--rw-r--r--   0 rmg        (503) staff       (20)     1995 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/datasets/data/titanic/target_values_semantics_es.csv
--rw-r--r--   0 rmg        (503) staff       (20)      706 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/datasets/data/titanic/values_semantics_en.csv
--rw-r--r--   0 rmg        (503) staff       (20)      743 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/datasets/data/titanic/values_semantics_es.csv
--rw-r--r--   0 rmg        (503) staff       (20)    34149 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/datasets/datasets.py
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.923251 xaiographs-1.0.0/xaiographs/examples/
--rw-r--r--   0 rmg        (503) staff       (20)      732 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/examples/__init__.py
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.924556 xaiographs-1.0.0/xaiographs/examples/__pycache__/
--rw-r--r--   0 rmg        (503) staff       (20)      202 2023-03-09 15:31:10.000000 xaiographs-1.0.0/xaiographs/examples/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 rmg        (503) staff       (20)      206 2023-03-17 11:01:50.000000 xaiographs-1.0.0/xaiographs/examples/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 rmg        (503) staff       (20)     1255 2023-03-09 15:31:10.000000 xaiographs-1.0.0/xaiographs/examples/__pycache__/titanic_example.cpython-37.pyc
--rw-r--r--   0 rmg        (503) staff       (20)     1267 2023-03-17 11:01:50.000000 xaiographs-1.0.0/xaiographs/examples/__pycache__/titanic_example.cpython-39.pyc
--rw-r--r--   0 rmg        (503) staff       (20)     1869 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/examples/body_performance_example.py
--rw-r--r--   0 rmg        (503) staff       (20)     1937 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/examples/education_performance_example.py
--rw-r--r--   0 rmg        (503) staff       (20)     1857 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/examples/titanic_example.py
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.925949 xaiographs-1.0.0/xaiographs/exgraph/
--rw-r--r--   0 rmg        (503) staff       (20)      732 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/exgraph/__init__.py
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.932978 xaiographs-1.0.0/xaiographs/exgraph/__pycache__/
--rw-r--r--   0 rmg        (503) staff       (20)      201 2023-03-09 13:56:14.000000 xaiographs-1.0.0/xaiographs/exgraph/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 rmg        (503) staff       (20)      919 2023-05-30 11:04:13.000000 xaiographs-1.0.0/xaiographs/exgraph/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rmg        (503) staff       (20)      205 2023-03-02 12:32:12.000000 xaiographs-1.0.0/xaiographs/exgraph/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 rmg        (503) staff       (20)    35159 2023-03-24 15:17:34.000000 xaiographs-1.0.0/xaiographs/exgraph/__pycache__/explainer.cpython-37.pyc
--rw-r--r--   0 rmg        (503) staff       (20)    28462 2023-05-30 11:04:13.000000 xaiographs-1.0.0/xaiographs/exgraph/__pycache__/explainer.cpython-38.pyc
--rw-r--r--   0 rmg        (503) staff       (20)    35239 2023-03-17 11:01:30.000000 xaiographs-1.0.0/xaiographs/exgraph/__pycache__/explainer.cpython-39.pyc
--rw-r--r--   0 rmg        (503) staff       (20)    20732 2023-03-09 13:56:23.000000 xaiographs-1.0.0/xaiographs/exgraph/__pycache__/exporter.cpython-37.pyc
--rw-r--r--   0 rmg        (503) staff       (20)    21374 2023-05-30 11:04:37.000000 xaiographs-1.0.0/xaiographs/exgraph/__pycache__/exporter.cpython-38.pyc
--rw-r--r--   0 rmg        (503) staff       (20)    20817 2023-03-17 11:01:38.000000 xaiographs-1.0.0/xaiographs/exgraph/__pycache__/exporter.cpython-39.pyc
--rw-r--r--   0 rmg        (503) staff       (20)    10499 2023-03-09 13:56:23.000000 xaiographs-1.0.0/xaiographs/exgraph/__pycache__/feature_selector.cpython-37.pyc
--rw-r--r--   0 rmg        (503) staff       (20)    11407 2023-05-30 11:04:37.000000 xaiographs-1.0.0/xaiographs/exgraph/__pycache__/feature_selector.cpython-38.pyc
--rw-r--r--   0 rmg        (503) staff       (20)    10563 2023-03-02 12:32:49.000000 xaiographs-1.0.0/xaiographs/exgraph/__pycache__/feature_selector.cpython-39.pyc
--rw-r--r--   0 rmg        (503) staff       (20)     8729 2023-03-24 15:17:42.000000 xaiographs-1.0.0/xaiographs/exgraph/__pycache__/stats_calculator.cpython-37.pyc
--rw-r--r--   0 rmg        (503) staff       (20)     9501 2023-05-30 11:04:37.000000 xaiographs-1.0.0/xaiographs/exgraph/__pycache__/stats_calculator.cpython-38.pyc
--rw-r--r--   0 rmg        (503) staff       (20)     8755 2023-03-17 11:01:38.000000 xaiographs-1.0.0/xaiographs/exgraph/__pycache__/stats_calculator.cpython-39.pyc
--rwxr-xr-x   0 rmg        (503) staff       (20)    34186 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/exgraph/explainer.py
--rwxr-xr-x   0 rmg        (503) staff       (20)    28687 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/exgraph/exporter.py
--rwxr-xr-x   0 rmg        (503) staff       (20)    13210 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/exgraph/feature_selector.py
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.934108 xaiographs-1.0.0/xaiographs/exgraph/importance/
--rw-r--r--   0 rmg        (503) staff       (20)      732 2023-05-30 08:46:10.000000 xaiographs-1.0.0/xaiographs/exgraph/importance/__init__.py
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.937525 xaiographs-1.0.0/xaiographs/exgraph/importance/__pycache__/
--rw-r--r--   0 rmg        (503) staff       (20)      212 2023-03-09 13:56:25.000000 xaiographs-1.0.0/xaiographs/exgraph/importance/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 rmg        (503) staff       (20)      930 2023-05-30 11:04:45.000000 xaiographs-1.0.0/xaiographs/exgraph/importance/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rmg        (503) staff       (20)      216 2023-03-02 12:32:56.000000 xaiographs-1.0.0/xaiographs/exgraph/importance/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 rmg        (503) staff       (20)    16440 2023-03-24 15:17:45.000000 xaiographs-1.0.0/xaiographs/exgraph/importance/__pycache__/importance_calculator.cpython-37.pyc
--rw-r--r--   0 rmg        (503) staff       (20)    17287 2023-05-30 11:04:45.000000 xaiographs-1.0.0/xaiographs/exgraph/importance/__pycache__/importance_calculator.cpython-38.pyc
--rw-r--r--   0 rmg        (503) staff       (20)    16538 2023-03-17 11:01:41.000000 xaiographs-1.0.0/xaiographs/exgraph/importance/__pycache__/importance_calculator.cpython-39.pyc
--rw-r--r--   0 rmg        (503) staff       (20)     1710 2023-03-09 13:56:25.000000 xaiographs-1.0.0/xaiographs/exgraph/importance/__pycache__/importance_calculator_factory.cpython-37.pyc
--rw-r--r--   0 rmg        (503) staff       (20)     2430 2023-05-30 11:04:45.000000 xaiographs-1.0.0/xaiographs/exgraph/importance/__pycache__/importance_calculator_factory.cpython-38.pyc
--rw-r--r--   0 rmg        (503) staff       (20)     1732 2023-03-02 12:32:56.000000 xaiographs-1.0.0/xaiographs/exgraph/importance/__pycache__/importance_calculator_factory.cpython-39.pyc
--rw-r--r--   0 rmg        (503) staff       (20)    21796 2023-05-30 11:04:45.000000 xaiographs-1.0.0/xaiographs/exgraph/importance/__pycache__/lide.cpython-38.pyc
--rwxr-xr-x   0 rmg        (503) staff       (20)    20476 2023-05-30 08:46:11.000000 xaiographs-1.0.0/xaiographs/exgraph/importance/importance_calculator.py
--rwxr-xr-x   0 rmg        (503) staff       (20)     1982 2023-05-30 08:46:11.000000 xaiographs-1.0.0/xaiographs/exgraph/importance/importance_calculator_factory.py
--rwxr-xr-x   0 rmg        (503) staff       (20)    30178 2023-05-30 08:46:11.000000 xaiographs-1.0.0/xaiographs/exgraph/importance/lide.py
--rwxr-xr-x   0 rmg        (503) staff       (20)    12668 2023-05-30 08:46:11.000000 xaiographs-1.0.0/xaiographs/exgraph/stats_calculator.py
--rwxr-xr-x   0 rmg        (503) staff       (20)    57302 2023-05-30 08:46:11.000000 xaiographs-1.0.0/xaiographs/fairness.py
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.937771 xaiographs-1.0.0/xaiographs/viz/
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.946695 xaiographs-1.0.0/xaiographs/viz/frontpiled/
--rw-r--r--   0 rmg        (503) staff       (20)    25566 2023-05-30 08:46:11.000000 xaiographs-1.0.0/xaiographs/viz/frontpiled/3rdpartylicenses.txt
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.948505 xaiographs-1.0.0/xaiographs/viz/frontpiled/assets/
--rw-r--r--   0 rmg        (503) staff       (20)   245235 2023-05-30 08:46:11.000000 xaiographs-1.0.0/xaiographs/viz/frontpiled/assets/20221029_lamb_icon.png
--rw-r--r--   0 rmg        (503) staff       (20)      370 2023-05-30 08:46:11.000000 xaiographs-1.0.0/xaiographs/viz/frontpiled/assets/colors.json
--rw-r--r--   0 rmg        (503) staff       (20)     9327 2023-05-30 08:46:11.000000 xaiographs-1.0.0/xaiographs/viz/frontpiled/assets/empty.png
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.948783 xaiographs-1.0.0/xaiographs/viz/frontpiled/assets/public/
--rw-r--r--   0 rmg        (503) staff       (20)      747 2023-05-30 08:46:11.000000 xaiographs-1.0.0/xaiographs/viz/frontpiled/assets/public/empty.txt
--rw-r--r--   0 rmg        (503) staff       (20)   245235 2023-05-30 08:46:11.000000 xaiographs-1.0.0/xaiographs/viz/frontpiled/favicon.ico
--rw-r--r--   0 rmg        (503) staff       (20)     2178 2023-05-30 08:46:11.000000 xaiographs-1.0.0/xaiographs/viz/frontpiled/index.html
--rw-r--r--   0 rmg        (503) staff       (20)  5595489 2023-05-30 08:46:11.000000 xaiographs-1.0.0/xaiographs/viz/frontpiled/main.9d1d96585d8bd21c.js
--rw-r--r--   0 rmg        (503) staff       (20)    34663 2023-05-30 08:46:11.000000 xaiographs-1.0.0/xaiographs/viz/frontpiled/polyfills.b5ff89bcc5e7cb9f.js
--rw-r--r--   0 rmg        (503) staff       (20)     1819 2023-05-30 08:46:11.000000 xaiographs-1.0.0/xaiographs/viz/frontpiled/runtime.e0dfb29715c1595b.js
--rw-r--r--   0 rmg        (503) staff       (20)    80894 2023-05-30 08:46:11.000000 xaiographs-1.0.0/xaiographs/viz/frontpiled/styles.423eabdc21b5f66a.css
--rwxr-xr-x   0 rmg        (503) staff       (20)     7328 2023-05-30 08:46:11.000000 xaiographs-1.0.0/xaiographs/viz/launcher.py
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.949292 xaiographs-1.0.0/xaiographs/why/
--rw-r--r--   0 rmg        (503) staff       (20)        0 2023-05-30 08:46:11.000000 xaiographs-1.0.0/xaiographs/why/__init__.py
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.950253 xaiographs-1.0.0/xaiographs/why/__pycache__/
--rw-r--r--   0 rmg        (503) staff       (20)      201 2023-05-30 11:05:09.000000 xaiographs-1.0.0/xaiographs/why/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 rmg        (503) staff       (20)    14937 2023-05-30 11:05:09.000000 xaiographs-1.0.0/xaiographs/why/__pycache__/why.cpython-38.pyc
-drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:26:39.950766 xaiographs-1.0.0/xaiographs/why/templates/
--rw-r--r--   0 rmg        (503) staff       (20)      606 2023-05-30 08:46:11.000000 xaiographs-1.0.0/xaiographs/why/templates/why_templates_en.csv
--rw-r--r--   0 rmg        (503) staff       (20)      625 2023-05-30 08:46:11.000000 xaiographs-1.0.0/xaiographs/why/templates/why_templates_es.csv
--rwxr-xr-x   0 rmg        (503) staff       (20)    17247 2023-05-30 08:46:11.000000 xaiographs-1.0.0/xaiographs/why/why.py
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.371745 XAIoGraphs-1.0.1/
+-rw-r--r--   0 rmg        (503) staff       (20)    34522 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/LICENSE
+-rw-r--r--   0 rmg        (503) staff       (20)       63 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/MANIFEST.in
+-rw-r--r--   0 rmg        (503) staff       (20)     5453 2023-05-31 14:24:28.371487 XAIoGraphs-1.0.1/PKG-INFO
+-rw-r--r--   0 rmg        (503) staff       (20)     5031 2023-05-31 14:19:12.000000 XAIoGraphs-1.0.1/README.md
+-rw-r--r--   0 rmg        (503) staff       (20)        6 2023-05-31 14:24:13.000000 XAIoGraphs-1.0.1/VERSION
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.308376 XAIoGraphs-1.0.1/XAIoGraphs.egg-info/
+-rw-r--r--   0 rmg        (503) staff       (20)     5453 2023-05-31 14:24:28.000000 XAIoGraphs-1.0.1/XAIoGraphs.egg-info/PKG-INFO
+-rw-r--r--   0 rmg        (503) staff       (20)     5978 2023-05-31 14:24:28.000000 XAIoGraphs-1.0.1/XAIoGraphs.egg-info/SOURCES.txt
+-rw-r--r--   0 rmg        (503) staff       (20)        1 2023-05-31 14:24:28.000000 XAIoGraphs-1.0.1/XAIoGraphs.egg-info/dependency_links.txt
+-rw-r--r--   0 rmg        (503) staff       (20)      280 2023-05-31 14:24:28.000000 XAIoGraphs-1.0.1/XAIoGraphs.egg-info/entry_points.txt
+-rw-r--r--   0 rmg        (503) staff       (20)       75 2023-05-31 14:24:28.000000 XAIoGraphs-1.0.1/XAIoGraphs.egg-info/requires.txt
+-rw-r--r--   0 rmg        (503) staff       (20)       11 2023-05-31 14:24:28.000000 XAIoGraphs-1.0.1/XAIoGraphs.egg-info/top_level.txt
+-rw-r--r--   0 rmg        (503) staff       (20)       38 2023-05-31 14:24:28.371794 XAIoGraphs-1.0.1/setup.cfg
+-rw-r--r--   0 rmg        (503) staff       (20)     2013 2023-05-31 14:04:54.000000 XAIoGraphs-1.0.1/setup.py
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.309385 XAIoGraphs-1.0.1/xaiographs/
+-rw-r--r--   0 rmg        (503) staff       (20)     6148 2023-04-03 12:27:00.000000 XAIoGraphs-1.0.1/xaiographs/.DS_Store
+-rw-r--r--   0 rmg        (503) staff       (20)      852 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/__init__.py
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.312202 XAIoGraphs-1.0.1/xaiographs/__pycache__/
+-rw-r--r--   0 rmg        (503) staff       (20)      316 2023-03-09 13:56:14.000000 XAIoGraphs-1.0.1/xaiographs/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)     1043 2023-05-30 11:04:13.000000 XAIoGraphs-1.0.1/xaiographs/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)      320 2023-03-02 12:32:11.000000 XAIoGraphs-1.0.1/xaiographs/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)    63370 2023-03-16 09:06:51.000000 XAIoGraphs-1.0.1/xaiographs/__pycache__/fairness.cpython-37.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)    45853 2023-05-30 11:05:09.000000 XAIoGraphs-1.0.1/xaiographs/__pycache__/fairness.cpython-38.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)    63378 2023-03-17 11:01:49.000000 XAIoGraphs-1.0.1/xaiographs/__pycache__/fairness.cpython-39.pyc
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.314081 XAIoGraphs-1.0.1/xaiographs/common/
+-rw-r--r--   0 rmg        (503) staff       (20)      732 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/common/__init__.py
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.318795 XAIoGraphs-1.0.1/xaiographs/common/__pycache__/
+-rw-r--r--   0 rmg        (503) staff       (20)      200 2023-03-09 13:56:23.000000 XAIoGraphs-1.0.1/xaiographs/common/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)      918 2023-05-30 11:04:37.000000 XAIoGraphs-1.0.1/xaiographs/common/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)      204 2023-03-02 12:32:49.000000 XAIoGraphs-1.0.1/xaiographs/common/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)      759 2023-03-09 13:56:23.000000 XAIoGraphs-1.0.1/xaiographs/common/__pycache__/constants.cpython-37.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)     1482 2023-05-30 11:04:37.000000 XAIoGraphs-1.0.1/xaiographs/common/__pycache__/constants.cpython-38.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)      763 2023-03-17 11:01:38.000000 XAIoGraphs-1.0.1/xaiographs/common/__pycache__/constants.cpython-39.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)     8927 2023-03-09 13:56:23.000000 XAIoGraphs-1.0.1/xaiographs/common/__pycache__/utils.cpython-37.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)     9697 2023-05-30 11:04:37.000000 XAIoGraphs-1.0.1/xaiographs/common/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)     8946 2023-03-02 12:32:49.000000 XAIoGraphs-1.0.1/xaiographs/common/__pycache__/utils.cpython-39.pyc
+-rwxr-xr-x   0 rmg        (503) staff       (20)     1221 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/common/constants.py
+-rwxr-xr-x   0 rmg        (503) staff       (20)     9886 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/common/utils.py
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.319913 XAIoGraphs-1.0.1/xaiographs/datasets/
+-rw-r--r--   0 rmg        (503) staff       (20)     6148 2023-04-03 14:11:53.000000 XAIoGraphs-1.0.1/xaiographs/datasets/.DS_Store
+-rw-r--r--   0 rmg        (503) staff       (20)     1168 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/datasets/__init__.py
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.324611 XAIoGraphs-1.0.1/xaiographs/datasets/__pycache__/
+-rw-r--r--   0 rmg        (503) staff       (20)      333 2023-03-09 15:31:10.000000 XAIoGraphs-1.0.1/xaiographs/datasets/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)     1367 2023-04-27 15:53:46.000000 XAIoGraphs-1.0.1/xaiographs/datasets/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)      337 2023-03-17 11:01:50.000000 XAIoGraphs-1.0.1/xaiographs/datasets/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)     9233 2023-03-09 15:31:10.000000 XAIoGraphs-1.0.1/xaiographs/datasets/__pycache__/datasets.cpython-37.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)    32863 2023-05-17 08:39:50.000000 XAIoGraphs-1.0.1/xaiographs/datasets/__pycache__/datasets.cpython-38.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)     9257 2023-03-17 11:01:50.000000 XAIoGraphs-1.0.1/xaiographs/datasets/__pycache__/datasets.cpython-39.pyc
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.300342 XAIoGraphs-1.0.1/xaiographs/datasets/data/
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.331313 XAIoGraphs-1.0.1/xaiographs/datasets/data/body_performance/
+-rw-r--r--   0 rmg        (503) staff       (20)  1021936 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/datasets/data/body_performance/dataset.csv
+-rw-r--r--   0 rmg        (503) staff       (20)  1880577 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/datasets/data/body_performance/dataset_discretized.csv
+-rw-r--r--   0 rmg        (503) staff       (20)     8367 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/datasets/data/body_performance/target_value_semantics_es.csv
+-rw-r--r--   0 rmg        (503) staff       (20)     7207 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/datasets/data/body_performance/target_values_semantics_en.csv
+-rw-r--r--   0 rmg        (503) staff       (20)     1857 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/datasets/data/body_performance/values_semantics_en.csv
+-rw-r--r--   0 rmg        (503) staff       (20)     2236 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/datasets/data/body_performance/values_semantics_es.csv
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.333846 XAIoGraphs-1.0.1/xaiographs/datasets/data/education_performance/
+-rw-r--r--   0 rmg        (503) staff       (20)     9647 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/datasets/data/education_performance/dataset.csv
+-rw-r--r--   0 rmg        (503) staff       (20)    37851 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/datasets/data/education_performance/dataset_discretized.csv
+-rw-r--r--   0 rmg        (503) staff       (20)    15504 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/datasets/data/education_performance/target_values_semantics_en.csv
+-rw-r--r--   0 rmg        (503) staff       (20)    17204 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/datasets/data/education_performance/target_values_semantics_es.csv
+-rw-r--r--   0 rmg        (503) staff       (20)     3051 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/datasets/data/education_performance/values_semantics_en.csv
+-rw-r--r--   0 rmg        (503) staff       (20)     3402 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/datasets/data/education_performance/values_semantics_es.csv
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.335647 XAIoGraphs-1.0.1/xaiographs/datasets/data/titanic/
+-rw-r--r--   0 rmg        (503) staff       (20)    46398 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/datasets/data/titanic/dataset.csv
+-rw-r--r--   0 rmg        (503) staff       (20)    84285 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/datasets/data/titanic/dataset_discretized.csv
+-rw-r--r--   0 rmg        (503) staff       (20)     1998 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/datasets/data/titanic/target_values_semantics_en.csv
+-rw-r--r--   0 rmg        (503) staff       (20)     1995 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/datasets/data/titanic/target_values_semantics_es.csv
+-rw-r--r--   0 rmg        (503) staff       (20)      706 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/datasets/data/titanic/values_semantics_en.csv
+-rw-r--r--   0 rmg        (503) staff       (20)      743 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/datasets/data/titanic/values_semantics_es.csv
+-rw-r--r--   0 rmg        (503) staff       (20)    34149 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/datasets/datasets.py
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.336703 XAIoGraphs-1.0.1/xaiographs/examples/
+-rw-r--r--   0 rmg        (503) staff       (20)      732 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/examples/__init__.py
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.338082 XAIoGraphs-1.0.1/xaiographs/examples/__pycache__/
+-rw-r--r--   0 rmg        (503) staff       (20)      202 2023-03-09 15:31:10.000000 XAIoGraphs-1.0.1/xaiographs/examples/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)      206 2023-03-17 11:01:50.000000 XAIoGraphs-1.0.1/xaiographs/examples/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)     1255 2023-03-09 15:31:10.000000 XAIoGraphs-1.0.1/xaiographs/examples/__pycache__/titanic_example.cpython-37.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)     1267 2023-03-17 11:01:50.000000 XAIoGraphs-1.0.1/xaiographs/examples/__pycache__/titanic_example.cpython-39.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)     1869 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/examples/body_performance_example.py
+-rw-r--r--   0 rmg        (503) staff       (20)     1937 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/examples/education_performance_example.py
+-rw-r--r--   0 rmg        (503) staff       (20)     1857 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/examples/titanic_example.py
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.339555 XAIoGraphs-1.0.1/xaiographs/exgraph/
+-rw-r--r--   0 rmg        (503) staff       (20)      732 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/__init__.py
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.348043 XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/
+-rw-r--r--   0 rmg        (503) staff       (20)      201 2023-03-09 13:56:14.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)      919 2023-05-30 11:04:13.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)      205 2023-03-02 12:32:12.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)    35159 2023-03-24 15:17:34.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/explainer.cpython-37.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)    28462 2023-05-30 11:04:13.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/explainer.cpython-38.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)    35239 2023-03-17 11:01:30.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/explainer.cpython-39.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)    20732 2023-03-09 13:56:23.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/exporter.cpython-37.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)    21374 2023-05-30 11:04:37.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/exporter.cpython-38.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)    20817 2023-03-17 11:01:38.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/exporter.cpython-39.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)    10499 2023-03-09 13:56:23.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/feature_selector.cpython-37.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)    11407 2023-05-30 11:04:37.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/feature_selector.cpython-38.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)    10563 2023-03-02 12:32:49.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/feature_selector.cpython-39.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)     8729 2023-03-24 15:17:42.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/stats_calculator.cpython-37.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)     9501 2023-05-30 11:04:37.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/stats_calculator.cpython-38.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)     8755 2023-03-17 11:01:38.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/stats_calculator.cpython-39.pyc
+-rwxr-xr-x   0 rmg        (503) staff       (20)    34186 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/explainer.py
+-rwxr-xr-x   0 rmg        (503) staff       (20)    28687 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/exporter.py
+-rwxr-xr-x   0 rmg        (503) staff       (20)    13210 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/feature_selector.py
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.353991 XAIoGraphs-1.0.1/xaiographs/exgraph/importance/
+-rw-r--r--   0 rmg        (503) staff       (20)      732 2023-05-30 08:46:10.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/importance/__init__.py
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.357934 XAIoGraphs-1.0.1/xaiographs/exgraph/importance/__pycache__/
+-rw-r--r--   0 rmg        (503) staff       (20)      212 2023-03-09 13:56:25.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/importance/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)      930 2023-05-30 11:04:45.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/importance/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)      216 2023-03-02 12:32:56.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/importance/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)    16440 2023-03-24 15:17:45.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/importance/__pycache__/importance_calculator.cpython-37.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)    17287 2023-05-30 11:04:45.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/importance/__pycache__/importance_calculator.cpython-38.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)    16538 2023-03-17 11:01:41.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/importance/__pycache__/importance_calculator.cpython-39.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)     1710 2023-03-09 13:56:25.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/importance/__pycache__/importance_calculator_factory.cpython-37.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)     2430 2023-05-30 11:04:45.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/importance/__pycache__/importance_calculator_factory.cpython-38.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)     1732 2023-03-02 12:32:56.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/importance/__pycache__/importance_calculator_factory.cpython-39.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)    21796 2023-05-30 11:04:45.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/importance/__pycache__/lide.cpython-38.pyc
+-rwxr-xr-x   0 rmg        (503) staff       (20)    20476 2023-05-30 08:46:11.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/importance/importance_calculator.py
+-rwxr-xr-x   0 rmg        (503) staff       (20)     1982 2023-05-30 08:46:11.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/importance/importance_calculator_factory.py
+-rwxr-xr-x   0 rmg        (503) staff       (20)    30178 2023-05-30 08:46:11.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/importance/lide.py
+-rwxr-xr-x   0 rmg        (503) staff       (20)    12668 2023-05-30 08:46:11.000000 XAIoGraphs-1.0.1/xaiographs/exgraph/stats_calculator.py
+-rwxr-xr-x   0 rmg        (503) staff       (20)    57302 2023-05-30 08:46:11.000000 XAIoGraphs-1.0.1/xaiographs/fairness.py
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.358256 XAIoGraphs-1.0.1/xaiographs/viz/
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.366681 XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/
+-rw-r--r--   0 rmg        (503) staff       (20)    25566 2023-05-30 08:46:11.000000 XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/3rdpartylicenses.txt
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.368634 XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/assets/
+-rw-r--r--   0 rmg        (503) staff       (20)   245235 2023-05-30 08:46:11.000000 XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/assets/20221029_lamb_icon.png
+-rw-r--r--   0 rmg        (503) staff       (20)      370 2023-05-30 08:46:11.000000 XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/assets/colors.json
+-rw-r--r--   0 rmg        (503) staff       (20)     9327 2023-05-30 08:46:11.000000 XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/assets/empty.png
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.368946 XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/assets/public/
+-rw-r--r--   0 rmg        (503) staff       (20)      747 2023-05-30 08:46:11.000000 XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/assets/public/empty.txt
+-rw-r--r--   0 rmg        (503) staff       (20)   245235 2023-05-30 08:46:11.000000 XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/favicon.ico
+-rw-r--r--   0 rmg        (503) staff       (20)     2178 2023-05-30 08:46:11.000000 XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/index.html
+-rw-r--r--   0 rmg        (503) staff       (20)  5595489 2023-05-30 08:46:11.000000 XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/main.9d1d96585d8bd21c.js
+-rw-r--r--   0 rmg        (503) staff       (20)    34663 2023-05-30 08:46:11.000000 XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/polyfills.b5ff89bcc5e7cb9f.js
+-rw-r--r--   0 rmg        (503) staff       (20)     1819 2023-05-30 08:46:11.000000 XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/runtime.e0dfb29715c1595b.js
+-rw-r--r--   0 rmg        (503) staff       (20)    80894 2023-05-30 08:46:11.000000 XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/styles.423eabdc21b5f66a.css
+-rwxr-xr-x   0 rmg        (503) staff       (20)     7328 2023-05-30 08:46:11.000000 XAIoGraphs-1.0.1/xaiographs/viz/launcher.py
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.369584 XAIoGraphs-1.0.1/xaiographs/why/
+-rw-r--r--   0 rmg        (503) staff       (20)        0 2023-05-30 08:46:11.000000 XAIoGraphs-1.0.1/xaiographs/why/__init__.py
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.370642 XAIoGraphs-1.0.1/xaiographs/why/__pycache__/
+-rw-r--r--   0 rmg        (503) staff       (20)      201 2023-05-30 11:05:09.000000 XAIoGraphs-1.0.1/xaiographs/why/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 rmg        (503) staff       (20)    14937 2023-05-30 11:05:09.000000 XAIoGraphs-1.0.1/xaiographs/why/__pycache__/why.cpython-38.pyc
+drwxr-xr-x   0 rmg        (503) staff       (20)        0 2023-05-31 14:24:28.371215 XAIoGraphs-1.0.1/xaiographs/why/templates/
+-rw-r--r--   0 rmg        (503) staff       (20)      606 2023-05-30 08:46:11.000000 XAIoGraphs-1.0.1/xaiographs/why/templates/why_templates_en.csv
+-rw-r--r--   0 rmg        (503) staff       (20)      625 2023-05-30 08:46:11.000000 XAIoGraphs-1.0.1/xaiographs/why/templates/why_templates_es.csv
+-rwxr-xr-x   0 rmg        (503) staff       (20)    17247 2023-05-30 08:46:11.000000 XAIoGraphs-1.0.1/xaiographs/why/why.py
```

### Comparing `xaiographs-1.0.0/LICENSE` & `XAIoGraphs-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/PKG-INFO` & `XAIoGraphs-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xaiographs
-Version: 1.0.0
+Name: XAIoGraphs
+Version: 1.0.1
 Summary: Python library providing Explainability & Fairness AI functionalities
 Home-page: https://github.com/Telefonica/XAIoGraphs
 Author: Telefonica I+D
 Author-email: ricardo.moyagarcia@telefonica.com
 License: AGPL-3.0 license
 Keywords: explainability,fairness,IA,Machine Learning
 Requires-Python: >=3.7
```

### Comparing `xaiographs-1.0.0/README.md` & `XAIoGraphs-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/XAIoGraphs.egg-info/PKG-INFO` & `XAIoGraphs-1.0.1/XAIoGraphs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xaiographs
-Version: 1.0.0
+Name: XAIoGraphs
+Version: 1.0.1
 Summary: Python library providing Explainability & Fairness AI functionalities
 Home-page: https://github.com/Telefonica/XAIoGraphs
 Author: Telefonica I+D
 Author-email: ricardo.moyagarcia@telefonica.com
 License: AGPL-3.0 license
 Keywords: explainability,fairness,IA,Machine Learning
 Requires-Python: >=3.7
```

### Comparing `xaiographs-1.0.0/XAIoGraphs.egg-info/SOURCES.txt` & `XAIoGraphs-1.0.1/XAIoGraphs.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,20 +8,14 @@
 XAIoGraphs.egg-info/dependency_links.txt
 XAIoGraphs.egg-info/entry_points.txt
 XAIoGraphs.egg-info/requires.txt
 XAIoGraphs.egg-info/top_level.txt
 xaiographs/.DS_Store
 xaiographs/__init__.py
 xaiographs/fairness.py
-xaiographs.egg-info/PKG-INFO
-xaiographs.egg-info/SOURCES.txt
-xaiographs.egg-info/dependency_links.txt
-xaiographs.egg-info/entry_points.txt
-xaiographs.egg-info/requires.txt
-xaiographs.egg-info/top_level.txt
 xaiographs/__pycache__/__init__.cpython-37.pyc
 xaiographs/__pycache__/__init__.cpython-38.pyc
 xaiographs/__pycache__/__init__.cpython-39.pyc
 xaiographs/__pycache__/fairness.cpython-37.pyc
 xaiographs/__pycache__/fairness.cpython-38.pyc
 xaiographs/__pycache__/fairness.cpython-39.pyc
 xaiographs/common/__init__.py
```

### Comparing `xaiographs-1.0.0/setup.py` & `XAIoGraphs-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 __VERSION__ = open('VERSION').read().strip()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
-    name='xaiographs',
+    name='XAIoGraphs',
     version=__VERSION__,
     description='Python library providing Explainability & Fairness AI functionalities',
     long_description_content_type="text/markdown",
     long_description=open('README.md', 'r').read(),
     url='https://github.com/Telefonica/XAIoGraphs',
     keywords=['explainability', 'fairness', 'IA', 'Machine Learning'],
     author='Telefonica I+D',
```

### Comparing `xaiographs-1.0.0/xaiographs/.DS_Store` & `XAIoGraphs-1.0.1/xaiographs/.DS_Store`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/__init__.py` & `XAIoGraphs-1.0.1/xaiographs/__init__.py`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/__pycache__/__init__.cpython-38.pyc` & `XAIoGraphs-1.0.1/xaiographs/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/__pycache__/fairness.cpython-37.pyc` & `XAIoGraphs-1.0.1/xaiographs/__pycache__/fairness.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/__pycache__/fairness.cpython-38.pyc` & `XAIoGraphs-1.0.1/xaiographs/__pycache__/fairness.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/__pycache__/fairness.cpython-39.pyc` & `XAIoGraphs-1.0.1/xaiographs/__pycache__/fairness.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/common/__init__.py` & `XAIoGraphs-1.0.1/xaiographs/common/__init__.py`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/common/__pycache__/__init__.cpython-38.pyc` & `XAIoGraphs-1.0.1/xaiographs/common/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/common/__pycache__/constants.cpython-37.pyc` & `XAIoGraphs-1.0.1/xaiographs/common/__pycache__/constants.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/common/__pycache__/constants.cpython-38.pyc` & `XAIoGraphs-1.0.1/xaiographs/common/__pycache__/constants.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/common/__pycache__/constants.cpython-39.pyc` & `XAIoGraphs-1.0.1/xaiographs/common/__pycache__/constants.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/common/__pycache__/utils.cpython-37.pyc` & `XAIoGraphs-1.0.1/xaiographs/common/__pycache__/utils.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/common/__pycache__/utils.cpython-38.pyc` & `XAIoGraphs-1.0.1/xaiographs/common/__pycache__/utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/common/__pycache__/utils.cpython-39.pyc` & `XAIoGraphs-1.0.1/xaiographs/common/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/common/constants.py` & `XAIoGraphs-1.0.1/xaiographs/common/constants.py`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/common/utils.py` & `XAIoGraphs-1.0.1/xaiographs/common/utils.py`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/.DS_Store` & `XAIoGraphs-1.0.1/xaiographs/datasets/.DS_Store`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/__init__.py` & `XAIoGraphs-1.0.1/xaiographs/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/__pycache__/__init__.cpython-38.pyc` & `XAIoGraphs-1.0.1/xaiographs/datasets/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/__pycache__/datasets.cpython-37.pyc` & `XAIoGraphs-1.0.1/xaiographs/datasets/__pycache__/datasets.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/__pycache__/datasets.cpython-38.pyc` & `XAIoGraphs-1.0.1/xaiographs/datasets/__pycache__/datasets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/__pycache__/datasets.cpython-39.pyc` & `XAIoGraphs-1.0.1/xaiographs/datasets/__pycache__/datasets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/data/body_performance/dataset.csv` & `XAIoGraphs-1.0.1/xaiographs/datasets/data/body_performance/dataset.csv`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/data/body_performance/dataset_discretized.csv` & `XAIoGraphs-1.0.1/xaiographs/datasets/data/body_performance/dataset_discretized.csv`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/data/body_performance/target_value_semantics_es.csv` & `XAIoGraphs-1.0.1/xaiographs/datasets/data/body_performance/target_value_semantics_es.csv`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/data/body_performance/target_values_semantics_en.csv` & `XAIoGraphs-1.0.1/xaiographs/datasets/data/body_performance/target_values_semantics_en.csv`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/data/body_performance/values_semantics_en.csv` & `XAIoGraphs-1.0.1/xaiographs/datasets/data/body_performance/values_semantics_en.csv`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/data/body_performance/values_semantics_es.csv` & `XAIoGraphs-1.0.1/xaiographs/datasets/data/body_performance/values_semantics_es.csv`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/data/education_performance/dataset.csv` & `XAIoGraphs-1.0.1/xaiographs/datasets/data/education_performance/dataset.csv`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/data/education_performance/dataset_discretized.csv` & `XAIoGraphs-1.0.1/xaiographs/datasets/data/education_performance/dataset_discretized.csv`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/data/education_performance/target_values_semantics_en.csv` & `XAIoGraphs-1.0.1/xaiographs/datasets/data/education_performance/target_values_semantics_en.csv`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/data/education_performance/target_values_semantics_es.csv` & `XAIoGraphs-1.0.1/xaiographs/datasets/data/education_performance/target_values_semantics_es.csv`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/data/education_performance/values_semantics_en.csv` & `XAIoGraphs-1.0.1/xaiographs/datasets/data/education_performance/values_semantics_en.csv`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/data/education_performance/values_semantics_es.csv` & `XAIoGraphs-1.0.1/xaiographs/datasets/data/education_performance/values_semantics_es.csv`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/data/titanic/dataset.csv` & `XAIoGraphs-1.0.1/xaiographs/datasets/data/titanic/dataset.csv`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/data/titanic/dataset_discretized.csv` & `XAIoGraphs-1.0.1/xaiographs/datasets/data/titanic/dataset_discretized.csv`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/data/titanic/target_values_semantics_en.csv` & `XAIoGraphs-1.0.1/xaiographs/datasets/data/titanic/target_values_semantics_en.csv`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/data/titanic/target_values_semantics_es.csv` & `XAIoGraphs-1.0.1/xaiographs/datasets/data/titanic/target_values_semantics_es.csv`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/data/titanic/values_semantics_en.csv` & `XAIoGraphs-1.0.1/xaiographs/datasets/data/titanic/values_semantics_en.csv`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/data/titanic/values_semantics_es.csv` & `XAIoGraphs-1.0.1/xaiographs/datasets/data/titanic/values_semantics_es.csv`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/datasets/datasets.py` & `XAIoGraphs-1.0.1/xaiographs/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/examples/__init__.py` & `XAIoGraphs-1.0.1/xaiographs/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/examples/__pycache__/titanic_example.cpython-37.pyc` & `XAIoGraphs-1.0.1/xaiographs/examples/__pycache__/titanic_example.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/examples/__pycache__/titanic_example.cpython-39.pyc` & `XAIoGraphs-1.0.1/xaiographs/examples/__pycache__/titanic_example.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/examples/body_performance_example.py` & `XAIoGraphs-1.0.1/xaiographs/examples/body_performance_example.py`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/examples/education_performance_example.py` & `XAIoGraphs-1.0.1/xaiographs/examples/education_performance_example.py`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/examples/titanic_example.py` & `XAIoGraphs-1.0.1/xaiographs/examples/titanic_example.py`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/__init__.py` & `XAIoGraphs-1.0.1/xaiographs/exgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/__pycache__/__init__.cpython-38.pyc` & `XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/__pycache__/explainer.cpython-37.pyc` & `XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/explainer.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/__pycache__/explainer.cpython-38.pyc` & `XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/explainer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/__pycache__/explainer.cpython-39.pyc` & `XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/explainer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/__pycache__/exporter.cpython-37.pyc` & `XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/exporter.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/__pycache__/exporter.cpython-38.pyc` & `XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/exporter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/__pycache__/exporter.cpython-39.pyc` & `XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/exporter.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/__pycache__/feature_selector.cpython-37.pyc` & `XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/feature_selector.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/__pycache__/feature_selector.cpython-38.pyc` & `XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/feature_selector.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/__pycache__/feature_selector.cpython-39.pyc` & `XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/feature_selector.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/__pycache__/stats_calculator.cpython-37.pyc` & `XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/stats_calculator.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/__pycache__/stats_calculator.cpython-38.pyc` & `XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/stats_calculator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/__pycache__/stats_calculator.cpython-39.pyc` & `XAIoGraphs-1.0.1/xaiographs/exgraph/__pycache__/stats_calculator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/explainer.py` & `XAIoGraphs-1.0.1/xaiographs/exgraph/explainer.py`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/exporter.py` & `XAIoGraphs-1.0.1/xaiographs/exgraph/exporter.py`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/feature_selector.py` & `XAIoGraphs-1.0.1/xaiographs/exgraph/feature_selector.py`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/importance/__init__.py` & `XAIoGraphs-1.0.1/xaiographs/exgraph/importance/__init__.py`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/importance/__pycache__/__init__.cpython-38.pyc` & `XAIoGraphs-1.0.1/xaiographs/exgraph/importance/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/importance/__pycache__/importance_calculator.cpython-37.pyc` & `XAIoGraphs-1.0.1/xaiographs/exgraph/importance/__pycache__/importance_calculator.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/importance/__pycache__/importance_calculator.cpython-38.pyc` & `XAIoGraphs-1.0.1/xaiographs/exgraph/importance/__pycache__/importance_calculator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/importance/__pycache__/importance_calculator.cpython-39.pyc` & `XAIoGraphs-1.0.1/xaiographs/exgraph/importance/__pycache__/importance_calculator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/importance/__pycache__/importance_calculator_factory.cpython-37.pyc` & `XAIoGraphs-1.0.1/xaiographs/exgraph/importance/__pycache__/importance_calculator_factory.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/importance/__pycache__/importance_calculator_factory.cpython-38.pyc` & `XAIoGraphs-1.0.1/xaiographs/exgraph/importance/__pycache__/importance_calculator_factory.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/importance/__pycache__/importance_calculator_factory.cpython-39.pyc` & `XAIoGraphs-1.0.1/xaiographs/exgraph/importance/__pycache__/importance_calculator_factory.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/importance/__pycache__/lide.cpython-38.pyc` & `XAIoGraphs-1.0.1/xaiographs/exgraph/importance/__pycache__/lide.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/importance/importance_calculator.py` & `XAIoGraphs-1.0.1/xaiographs/exgraph/importance/importance_calculator.py`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/importance/importance_calculator_factory.py` & `XAIoGraphs-1.0.1/xaiographs/exgraph/importance/importance_calculator_factory.py`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/importance/lide.py` & `XAIoGraphs-1.0.1/xaiographs/exgraph/importance/lide.py`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/exgraph/stats_calculator.py` & `XAIoGraphs-1.0.1/xaiographs/exgraph/stats_calculator.py`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/fairness.py` & `XAIoGraphs-1.0.1/xaiographs/fairness.py`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/viz/frontpiled/3rdpartylicenses.txt` & `XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/3rdpartylicenses.txt`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/viz/frontpiled/assets/20221029_lamb_icon.png` & `XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/assets/20221029_lamb_icon.png`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/viz/frontpiled/assets/empty.png` & `XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/assets/empty.png`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/viz/frontpiled/assets/public/empty.txt` & `XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/assets/public/empty.txt`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/viz/frontpiled/favicon.ico` & `XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/favicon.ico`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/viz/frontpiled/index.html` & `XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/index.html`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/viz/frontpiled/main.9d1d96585d8bd21c.js` & `XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/main.9d1d96585d8bd21c.js`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/viz/frontpiled/polyfills.b5ff89bcc5e7cb9f.js` & `XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/polyfills.b5ff89bcc5e7cb9f.js`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/viz/frontpiled/runtime.e0dfb29715c1595b.js` & `XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/runtime.e0dfb29715c1595b.js`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/viz/frontpiled/styles.423eabdc21b5f66a.css` & `XAIoGraphs-1.0.1/xaiographs/viz/frontpiled/styles.423eabdc21b5f66a.css`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/viz/launcher.py` & `XAIoGraphs-1.0.1/xaiographs/viz/launcher.py`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/why/__pycache__/why.cpython-38.pyc` & `XAIoGraphs-1.0.1/xaiographs/why/__pycache__/why.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/why/templates/why_templates_en.csv` & `XAIoGraphs-1.0.1/xaiographs/why/templates/why_templates_en.csv`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/why/templates/why_templates_es.csv` & `XAIoGraphs-1.0.1/xaiographs/why/templates/why_templates_es.csv`

 * *Files identical despite different names*

### Comparing `xaiographs-1.0.0/xaiographs/why/why.py` & `XAIoGraphs-1.0.1/xaiographs/why/why.py`

 * *Files identical despite different names*

