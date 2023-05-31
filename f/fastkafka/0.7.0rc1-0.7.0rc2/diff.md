# Comparing `tmp/fastkafka-0.7.0rc1.tar.gz` & `tmp/fastkafka-0.7.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastkafka-0.7.0rc1.tar", last modified: Wed May 31 06:50:20 2023, max compression
+gzip compressed data, was "fastkafka-0.7.0rc2.tar", last modified: Wed May 31 15:08:03 2023, max compression
```

## Comparing `fastkafka-0.7.0rc1.tar` & `fastkafka-0.7.0rc2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 06:50:20.317315 fastkafka-0.7.0rc1/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    12621 2023-05-19 13:11:05.000000 fastkafka-0.7.0rc1/CONTRIBUTING.md
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    11357 2023-03-14 07:16:19.000000 fastkafka-0.7.0rc1/LICENSE
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      111 2023-03-14 07:16:19.000000 fastkafka-0.7.0rc1/MANIFEST.in
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    24097 2023-05-31 06:50:20.317315 fastkafka-0.7.0rc1/PKG-INFO
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    22669 2023-05-31 06:49:07.000000 fastkafka-0.7.0rc1/README.md
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 06:50:20.309315 fastkafka-0.7.0rc1/fastkafka/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      525 2023-05-31 06:37:28.000000 fastkafka-0.7.0rc1/fastkafka/__init__.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 06:50:20.313315 fastkafka-0.7.0rc1/fastkafka/_application/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 06:37:28.000000 fastkafka-0.7.0rc1/fastkafka/_application/__init__.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    39065 2023-05-31 06:37:26.000000 fastkafka-0.7.0rc1/fastkafka/_application/app.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    17537 2023-05-31 06:37:26.000000 fastkafka-0.7.0rc1/fastkafka/_application/tester.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     2108 2023-05-31 06:37:26.000000 fastkafka-0.7.0rc1/fastkafka/_cli.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     5110 2023-05-31 06:37:26.000000 fastkafka-0.7.0rc1/fastkafka/_cli_docs.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      996 2023-05-31 06:37:26.000000 fastkafka-0.7.0rc1/fastkafka/_cli_testing.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 06:50:20.313315 fastkafka-0.7.0rc1/fastkafka/_components/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 06:37:28.000000 fastkafka-0.7.0rc1/fastkafka/_components/__init__.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4698 2023-05-31 06:37:26.000000 fastkafka-0.7.0rc1/fastkafka/_components/_subprocess.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13315 2023-05-31 06:37:25.000000 fastkafka-0.7.0rc1/fastkafka/_components/aiokafka_consumer_loop.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    18656 2023-05-31 06:37:25.000000 fastkafka-0.7.0rc1/fastkafka/_components/asyncapi.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     2905 2023-05-31 06:37:26.000000 fastkafka-0.7.0rc1/fastkafka/_components/benchmarking.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     6991 2023-05-31 06:37:27.000000 fastkafka-0.7.0rc1/fastkafka/_components/docs_dependencies.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 06:50:20.317315 fastkafka-0.7.0rc1/fastkafka/_components/encoder/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 06:37:28.000000 fastkafka-0.7.0rc1/fastkafka/_components/encoder/__init__.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13910 2023-05-31 06:37:26.000000 fastkafka-0.7.0rc1/fastkafka/_components/encoder/avro.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1630 2023-05-31 06:37:26.000000 fastkafka-0.7.0rc1/fastkafka/_components/encoder/json.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4136 2023-05-31 06:37:27.000000 fastkafka-0.7.0rc1/fastkafka/_components/helpers.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4730 2023-05-31 06:37:28.000000 fastkafka-0.7.0rc1/fastkafka/_components/logger.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13150 2023-05-31 06:37:27.000000 fastkafka-0.7.0rc1/fastkafka/_components/meta.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     7403 2023-05-31 06:37:25.000000 fastkafka-0.7.0rc1/fastkafka/_components/producer_decorator.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    11998 2023-05-31 06:37:25.000000 fastkafka-0.7.0rc1/fastkafka/_components/task_streaming.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     7992 2023-05-31 06:37:27.000000 fastkafka-0.7.0rc1/fastkafka/_components/test_dependencies.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    20426 2023-05-31 06:37:27.000000 fastkafka-0.7.0rc1/fastkafka/_docusaurus_helper.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    51550 2023-05-31 06:37:27.000000 fastkafka-0.7.0rc1/fastkafka/_helpers.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    84393 2023-05-31 06:37:28.000000 fastkafka-0.7.0rc1/fastkafka/_modidx.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     8205 2023-05-31 06:37:26.000000 fastkafka-0.7.0rc1/fastkafka/_server.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 06:50:20.317315 fastkafka-0.7.0rc1/fastkafka/_testing/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 06:37:28.000000 fastkafka-0.7.0rc1/fastkafka/_testing/__init__.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    22761 2023-05-31 06:37:24.000000 fastkafka-0.7.0rc1/fastkafka/_testing/apache_kafka_broker.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    28873 2023-05-31 06:37:24.000000 fastkafka-0.7.0rc1/fastkafka/_testing/in_memory_broker.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    12344 2023-05-31 06:37:24.000000 fastkafka-0.7.0rc1/fastkafka/_testing/local_redpanda_broker.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4979 2023-05-31 06:37:24.000000 fastkafka-0.7.0rc1/fastkafka/_testing/test_utils.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      598 2023-05-31 06:37:26.000000 fastkafka-0.7.0rc1/fastkafka/encoder.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      454 2023-05-31 06:37:24.000000 fastkafka-0.7.0rc1/fastkafka/executors.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      858 2023-05-31 06:37:24.000000 fastkafka-0.7.0rc1/fastkafka/testing.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 06:50:20.313315 fastkafka-0.7.0rc1/fastkafka.egg-info/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    24097 2023-05-31 06:50:20.000000 fastkafka-0.7.0rc1/fastkafka.egg-info/PKG-INFO
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1410 2023-05-31 06:50:20.000000 fastkafka-0.7.0rc1/fastkafka.egg-info/SOURCES.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        1 2023-05-31 06:50:20.000000 fastkafka-0.7.0rc1/fastkafka.egg-info/dependency_links.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      146 2023-05-31 06:50:20.000000 fastkafka-0.7.0rc1/fastkafka.egg-info/entry_points.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        1 2023-05-23 12:47:36.000000 fastkafka-0.7.0rc1/fastkafka.egg-info/not-zip-safe
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      690 2023-05-31 06:50:20.000000 fastkafka-0.7.0rc1/fastkafka.egg-info/requires.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)       10 2023-05-31 06:50:20.000000 fastkafka-0.7.0rc1/fastkafka.egg-info/top_level.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1231 2023-05-31 06:37:13.000000 fastkafka-0.7.0rc1/settings.ini
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)       38 2023-05-31 06:50:20.317315 fastkafka-0.7.0rc1/setup.cfg
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     3777 2023-05-30 11:33:36.000000 fastkafka-0.7.0rc1/setup.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 15:08:03.870864 fastkafka-0.7.0rc2/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    12621 2023-05-19 13:11:05.000000 fastkafka-0.7.0rc2/CONTRIBUTING.md
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    11357 2023-03-14 07:16:19.000000 fastkafka-0.7.0rc2/LICENSE
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      111 2023-03-14 07:16:19.000000 fastkafka-0.7.0rc2/MANIFEST.in
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    24678 2023-05-31 15:08:03.870864 fastkafka-0.7.0rc2/PKG-INFO
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    23250 2023-05-31 15:05:16.000000 fastkafka-0.7.0rc2/README.md
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 15:08:03.862865 fastkafka-0.7.0rc2/fastkafka/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      525 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/__init__.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 15:08:03.866865 fastkafka-0.7.0rc2/fastkafka/_application/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/_application/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    39065 2023-05-31 15:02:33.000000 fastkafka-0.7.0rc2/fastkafka/_application/app.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    17537 2023-05-31 15:02:34.000000 fastkafka-0.7.0rc2/fastkafka/_application/tester.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     2108 2023-05-31 15:02:34.000000 fastkafka-0.7.0rc2/fastkafka/_cli.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     5622 2023-05-31 15:02:34.000000 fastkafka-0.7.0rc2/fastkafka/_cli_docs.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      996 2023-05-31 15:02:34.000000 fastkafka-0.7.0rc2/fastkafka/_cli_testing.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 15:08:03.870864 fastkafka-0.7.0rc2/fastkafka/_components/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/_components/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4698 2023-05-31 15:02:34.000000 fastkafka-0.7.0rc2/fastkafka/_components/_subprocess.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13315 2023-05-31 15:02:33.000000 fastkafka-0.7.0rc2/fastkafka/_components/aiokafka_consumer_loop.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    18656 2023-05-31 15:02:33.000000 fastkafka-0.7.0rc2/fastkafka/_components/asyncapi.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     2905 2023-05-31 15:02:34.000000 fastkafka-0.7.0rc2/fastkafka/_components/benchmarking.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     6991 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/_components/docs_dependencies.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 15:08:03.870864 fastkafka-0.7.0rc2/fastkafka/_components/encoder/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/_components/encoder/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13910 2023-05-31 15:02:34.000000 fastkafka-0.7.0rc2/fastkafka/_components/encoder/avro.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1630 2023-05-31 15:02:34.000000 fastkafka-0.7.0rc2/fastkafka/_components/encoder/json.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4136 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/_components/helpers.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4730 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/_components/logger.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13150 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/_components/meta.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     7403 2023-05-31 15:02:33.000000 fastkafka-0.7.0rc2/fastkafka/_components/producer_decorator.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    11998 2023-05-31 15:02:32.000000 fastkafka-0.7.0rc2/fastkafka/_components/task_streaming.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     7992 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/_components/test_dependencies.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    20426 2023-05-31 15:02:34.000000 fastkafka-0.7.0rc2/fastkafka/_docusaurus_helper.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    51550 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/_helpers.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    84393 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/_modidx.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     8205 2023-05-31 15:02:34.000000 fastkafka-0.7.0rc2/fastkafka/_server.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 15:08:03.870864 fastkafka-0.7.0rc2/fastkafka/_testing/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/_testing/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    22761 2023-05-31 15:02:32.000000 fastkafka-0.7.0rc2/fastkafka/_testing/apache_kafka_broker.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    28873 2023-05-31 15:02:32.000000 fastkafka-0.7.0rc2/fastkafka/_testing/in_memory_broker.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    12344 2023-05-31 15:02:32.000000 fastkafka-0.7.0rc2/fastkafka/_testing/local_redpanda_broker.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4979 2023-05-31 15:02:32.000000 fastkafka-0.7.0rc2/fastkafka/_testing/test_utils.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      598 2023-05-31 15:02:34.000000 fastkafka-0.7.0rc2/fastkafka/encoder.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      454 2023-05-31 15:02:32.000000 fastkafka-0.7.0rc2/fastkafka/executors.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      858 2023-05-31 15:02:32.000000 fastkafka-0.7.0rc2/fastkafka/testing.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 15:08:03.866865 fastkafka-0.7.0rc2/fastkafka.egg-info/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    24678 2023-05-31 15:08:03.000000 fastkafka-0.7.0rc2/fastkafka.egg-info/PKG-INFO
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1410 2023-05-31 15:08:03.000000 fastkafka-0.7.0rc2/fastkafka.egg-info/SOURCES.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        1 2023-05-31 15:08:03.000000 fastkafka-0.7.0rc2/fastkafka.egg-info/dependency_links.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      146 2023-05-31 15:08:03.000000 fastkafka-0.7.0rc2/fastkafka.egg-info/entry_points.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        1 2023-05-23 12:47:36.000000 fastkafka-0.7.0rc2/fastkafka.egg-info/not-zip-safe
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      690 2023-05-31 15:08:03.000000 fastkafka-0.7.0rc2/fastkafka.egg-info/requires.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)       10 2023-05-31 15:08:03.000000 fastkafka-0.7.0rc2/fastkafka.egg-info/top_level.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1231 2023-05-31 14:46:47.000000 fastkafka-0.7.0rc2/settings.ini
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)       38 2023-05-31 15:08:03.870864 fastkafka-0.7.0rc2/setup.cfg
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     3777 2023-05-30 11:33:36.000000 fastkafka-0.7.0rc2/setup.py
```

### Comparing `fastkafka-0.7.0rc1/CONTRIBUTING.md` & `fastkafka-0.7.0rc2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/LICENSE` & `fastkafka-0.7.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/PKG-INFO` & `fastkafka-0.7.0rc2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastkafka
-Version: 0.7.0rc1
+Version: 0.7.0rc2
 Summary: FastKafka is a powerful and easy-to-use Python library for building asynchronous web services that interact with Kafka topics. Built on top of FastAPI, Starlette, Pydantic, AIOKafka and AsyncAPI, FastKafka simplifies the process of writing producers and consumers for Kafka topics.
 Home-page: https://github.com/airtai/fastkafka
 Author: airt
 Author-email: info@airt.ai
 License: Apache Software License 2.0
 Project-URL: Bug Tracker, https://github.com/airtai/fastkafka/issues
 Project-URL: CI, https://github.com/airtai/fastkafka/actions
@@ -108,19 +108,19 @@
 
 ``` sh
 pip install fastkafka[test,docs]
 ```
 
 ## Tutorial
 
-You can start an interactive and extensive tutorial in Google Colab by
-clicking the button below:
+You can start an interactive tutorial in Google Colab by clicking the
+button below:
 
-<a href="https://colab.research.google.com/github/airtai/fastkafka/blob/main/nbs/guides/Guide_00_FastKafka_Demo.ipynb" target=”_blank”>
-<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" />
+<a href="https://colab.research.google.com/github/airtai/fastkafka/blob/main/nbs/index.ipynb" target=”_blank”>
+<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab" />
 </a>
 
 ## Writing server code
 
 To demonstrate FastKafka simplicity of using `@produces` and `@consumes`
 decorators, we will focus on a simple app.
 
@@ -171,18 +171,18 @@
 
 - `kafka_brokers`: a dictionary used for generation of documentation
 
 We will also import and create a logger so that we can log the incoming
 data in our consuming function.
 
 ``` python
+from logging import getLogger
 from fastkafka import FastKafka
-from fastkafka._components.logger import get_logger
 
-logger = get_logger(__name__)
+logger = getLogger("Demo Kafka app")
 
 kafka_brokers = {
     "localhost": {
         "url": "localhost",
         "description": "local development kafka broker",
         "port": 9092,
     },
@@ -267,18 +267,18 @@
 
 msg = Data(
     data=0.1,
 )
 
 # Start Tester app and create InMemory Kafka broker for testing
 async with Tester(kafka_app) as tester:
-    # Send IrisInputData message to input_data topic
+    # Send Data message to input_data topic
     await tester.to_input_data(msg)
 
-    # Assert that the kafka_app responded with IrisPrediction in predictions topic
+    # Assert that the kafka_app responded with incremented data in output_data topic
     await tester.awaited_mocks.on_output_data.assert_awaited_with(
         Data(data=1.1), timeout=2
     )
 ```
 
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._start() called
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._patch_consumers_and_producers(): Patching consumers and producers!
@@ -297,15 +297,15 @@
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'earliest', 'max_poll_records': 100}
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched start() called()
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched subscribe() called
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer.subscribe(), subscribing to: ['output_data']
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
-    [INFO] __main__: Got data: 0.1
+    [INFO] Demo Kafka app: Got data: 0.1
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched stop() called
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaProducer patched stop() called
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched stop() called
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
@@ -389,86 +389,87 @@
 app simbol to the command.
 
 `shell fastkafka run --num-workers=1 --kafka-broker localhost application:kafka_app`
 
 After running the command, you should see the following output in your
 command line:
 
-    [7262]: 23-05-22 12:16:07.361 [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
-    [7260]: 23-05-22 12:16:07.361 [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
-    [7260]: 23-05-22 12:16:07.361 [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
-    [7262]: 23-05-22 12:16:07.361 [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
-    [7260]: 23-05-22 12:16:07.388 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
-    [7260]: 23-05-22 12:16:07.388 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
-    [7262]: 23-05-22 12:16:07.389 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
-    [7262]: 23-05-22 12:16:07.389 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
-    [7260]: 23-05-22 12:16:07.396 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
-    [7260]: 23-05-22 12:16:07.396 [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
-    [7260]: 23-05-22 12:16:07.396 [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
-    [7260]: 23-05-22 12:16:07.396 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
-    [7262]: 23-05-22 12:16:07.400 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
-    [7262]: 23-05-22 12:16:07.400 [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
-    [7262]: 23-05-22 12:16:07.401 [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
-    [7262]: 23-05-22 12:16:07.401 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
-    [7262]: 23-05-22 12:16:07.412 [ERROR] aiokafka.cluster: Topic input_data not found in cluster metadata
-    [7262]: 23-05-22 12:16:07.412 [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
-    [7260]: 23-05-22 12:16:07.482 [WARNING] aiokafka.cluster: Topic input_data is not available during auto-create initialization
-    [7260]: 23-05-22 12:16:07.482 [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
-    [7262]: 23-05-22 12:16:12.865 [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('172.18.0.2', 9092)
-    [7262]: 23-05-22 12:16:12.865 [ERROR] aiokafka: Unable to update metadata from [0]
-    [7260]: 23-05-22 12:16:12.866 [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('172.18.0.2', 9092)
-    [7260]: 23-05-22 12:16:12.866 [ERROR] aiokafka: Unable to update metadata from [0]
-    ^C
-    [7262]: 23-05-22 12:16:12.978 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
-    [7262]: 23-05-22 12:16:12.979 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
+    [1504]: 23-05-31 11:36:45.874 [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
+    [1504]: 23-05-31 11:36:45.875 [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
+    [1504]: 23-05-31 11:36:45.937 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
+    [1504]: 23-05-31 11:36:45.937 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
+    [1504]: 23-05-31 11:36:45.956 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
+    [1504]: 23-05-31 11:36:45.956 [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
+    [1504]: 23-05-31 11:36:45.956 [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
+    [1504]: 23-05-31 11:36:45.956 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
+    [1506]: 23-05-31 11:36:45.993 [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
+    [1506]: 23-05-31 11:36:45.994 [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
+    [1506]: 23-05-31 11:36:46.014 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
+    [1506]: 23-05-31 11:36:46.015 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
+    [1506]: 23-05-31 11:36:46.040 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
+    [1506]: 23-05-31 11:36:46.042 [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
+    [1506]: 23-05-31 11:36:46.043 [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
+    [1506]: 23-05-31 11:36:46.043 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
+    [1506]: 23-05-31 11:36:46.068 [ERROR] aiokafka.cluster: Topic input_data not found in cluster metadata
+    [1506]: 23-05-31 11:36:46.070 [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
+    [1504]: 23-05-31 11:36:46.131 [WARNING] aiokafka.cluster: Topic input_data is not available during auto-create initialization
+    [1504]: 23-05-31 11:36:46.132 [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
+    [1506]: 23-05-31 11:37:00.237 [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('172.28.0.12', 9092)
+    [1506]: 23-05-31 11:37:00.237 [ERROR] aiokafka: Unable to update metadata from [0]
+    [1504]: 23-05-31 11:37:00.238 [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('172.28.0.12', 9092)
+    [1504]: 23-05-31 11:37:00.238 [ERROR] aiokafka: Unable to update metadata from [0]
+    [1506]: 23-05-31 11:37:00.294 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
+    [1506]: 23-05-31 11:37:00.294 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
     Starting process cleanup, this may take a few seconds...
-    23-05-22 12:16:12.997 [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 7260...
-    23-05-22 12:16:12.998 [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 7262...
-    [7260]: 23-05-22 12:16:13.035 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
-    [7260]: 23-05-22 12:16:13.035 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
+    23-05-31 11:37:00.345 [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 1504...
+    23-05-31 11:37:00.345 [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 1506...
+    [1504]: 23-05-31 11:37:00.347 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
+    [1504]: 23-05-31 11:37:00.347 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
+    23-05-31 11:37:00.607 [INFO] fastkafka._server: terminate_asyncio_process(): Process 1506 was already terminated.
+    23-05-31 11:37:00.822 [INFO] fastkafka._server: terminate_asyncio_process(): Process 1504 was already terminated.
 
 ## Documentation
 
 The kafka app comes with builtin documentation generation using
 [AsyncApi HTML generator](https://www.asyncapi.com/tools/generator).
 
 AsyncApi requires Node.js to be installed and we provide the following
 convenience command line for it:
 
 ``` sh
 fastkafka docs install_deps
 ```
 
-    23-05-22 12:17:03.425 [INFO] fastkafka._components.docs_dependencies: AsyncAPI generator installed
+    23-05-31 11:38:24.128 [INFO] fastkafka._components.docs_dependencies: AsyncAPI generator installed
 
 To generate the documentation programatically you just need to call the
-folloving command:
+following command:
 
 ``` sh
 fastkafka docs generate application:kafka_app
 ```
 
-    23-05-22 12:17:04.268 [INFO] fastkafka._components.asyncapi: New async specifications generated at: '/work/fastkafka/nbs/asyncapi/spec/asyncapi.yml'
-    23-05-22 12:17:13.777 [INFO] fastkafka._components.asyncapi: Async docs generated at 'asyncapi/docs'
-    23-05-22 12:17:13.777 [INFO] fastkafka._components.asyncapi: Output of '$ npx -y -p @asyncapi/generator ag asyncapi/spec/asyncapi.yml @asyncapi/html-template -o asyncapi/docs --force-write'
+    23-05-31 11:38:25.113 [INFO] fastkafka._components.asyncapi: Old async specifications at '/content/asyncapi/spec/asyncapi.yml' does not exist.
+    23-05-31 11:38:25.118 [INFO] fastkafka._components.asyncapi: New async specifications generated at: '/content/asyncapi/spec/asyncapi.yml'
+    23-05-31 11:38:43.455 [INFO] fastkafka._components.asyncapi: Async docs generated at 'asyncapi/docs'
+    23-05-31 11:38:43.455 [INFO] fastkafka._components.asyncapi: Output of '$ npx -y -p @asyncapi/generator ag asyncapi/spec/asyncapi.yml @asyncapi/html-template -o asyncapi/docs --force-write'
 
     Done! ✨
-    Check out your shiny new generated files at /work/fastkafka/nbs/asyncapi/docs.
+    Check out your shiny new generated files at /content/asyncapi/docs.
 
-. This will generate the *asyncapi* folder in relative path where all
-your documentation will be saved. You can check out the content of it
-with:
+This will generate the *asyncapi* folder in relative path where all your
+documentation will be saved. You can check out the content of it with:
 
 ``` sh
 ls -l asyncapi
 ```
 
-    total 2
-    drwxrwxr-x 4 tvrtko tvrtko 5 Mar 29 09:57 docs
-    drwxrwxr-x 2 tvrtko tvrtko 3 Mar 29 09:56 spec
+    total 8
+    drwxr-xr-x 4 root root 4096 May 31 11:38 docs
+    drwxr-xr-x 2 root root 4096 May 31 11:38 spec
 
 In docs folder you will find the servable static html file of your
 documentation. This can also be served using our `fastkafka docs serve`
 CLI command (more on that in our guides).
 
 In spec folder you will find a asyncapi.yml file containing the async
 API specification of your application.
@@ -476,24 +477,27 @@
 We can locally preview the generated documentation by running the
 following command:
 
 ``` sh
 fastkafka docs serve application:kafka_app
 ```
 
-    23-05-22 12:17:14.784 [INFO] fastkafka._components.asyncapi: New async specifications generated at: '/work/fastkafka/nbs/asyncapi/spec/asyncapi.yml'
-    23-05-22 12:17:24.450 [INFO] fastkafka._components.asyncapi: Async docs generated at 'asyncapi/docs'
-    23-05-22 12:17:24.450 [INFO] fastkafka._components.asyncapi: Output of '$ npx -y -p @asyncapi/generator ag asyncapi/spec/asyncapi.yml @asyncapi/html-template -o asyncapi/docs --force-write'
+    23-05-31 11:38:45.250 [INFO] fastkafka._components.asyncapi: New async specifications generated at: '/content/asyncapi/spec/asyncapi.yml'
+    23-05-31 11:39:04.410 [INFO] fastkafka._components.asyncapi: Async docs generated at 'asyncapi/docs'
+    23-05-31 11:39:04.411 [INFO] fastkafka._components.asyncapi: Output of '$ npx -y -p @asyncapi/generator ag asyncapi/spec/asyncapi.yml @asyncapi/html-template -o asyncapi/docs --force-write'
 
     Done! ✨
-    Check out your shiny new generated files at /work/fastkafka/nbs/asyncapi/docs.
+    Check out your shiny new generated files at /content/asyncapi/docs.
 
 
     Serving documentation on http://127.0.0.1:8000
-    ^C
+    127.0.0.1 - - [31/May/2023 11:39:14] "GET / HTTP/1.1" 200 -
+    127.0.0.1 - - [31/May/2023 11:39:14] "GET /css/global.min.css HTTP/1.1" 200 -
+    127.0.0.1 - - [31/May/2023 11:39:14] "GET /js/asyncapi-ui.min.js HTTP/1.1" 200 -
+    127.0.0.1 - - [31/May/2023 11:39:14] "GET /css/asyncapi.min.css HTTP/1.1" 200 -
     Interupting serving of documentation and cleaning up...
 
 From the parameters passed to the application constructor, we get the
 documentation bellow:
 
 ``` python
 from fastkafka import FastKafka
@@ -510,15 +514,15 @@
         "port": 9092,
         "protocol": "kafka-secure",
         "security": {"type": "plain"},
     },
 }
 
 kafka_app = FastKafka(
-    title="Iris predictions",
+    title="Demo Kafka app",
     kafka_brokers=kafka_brokers,
 )
 ```
 
 ![Kafka_servers](https://raw.githubusercontent.com/airtai/fastkafka/main/nbs/images/screenshot-kafka-servers.png)
 
 The following documentation snippet are for the consumer as specified in
```

### Comparing `fastkafka-0.7.0rc1/README.md` & `fastkafka-0.7.0rc2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -78,19 +78,19 @@
 
 ``` sh
 pip install fastkafka[test,docs]
 ```
 
 ## Tutorial
 
-You can start an interactive and extensive tutorial in Google Colab by
-clicking the button below:
+You can start an interactive tutorial in Google Colab by clicking the
+button below:
 
-<a href="https://colab.research.google.com/github/airtai/fastkafka/blob/main/nbs/guides/Guide_00_FastKafka_Demo.ipynb" target=”_blank”>
-<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" />
+<a href="https://colab.research.google.com/github/airtai/fastkafka/blob/main/nbs/index.ipynb" target=”_blank”>
+<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab" />
 </a>
 
 ## Writing server code
 
 To demonstrate FastKafka simplicity of using `@produces` and `@consumes`
 decorators, we will focus on a simple app.
 
@@ -141,18 +141,18 @@
 
 - `kafka_brokers`: a dictionary used for generation of documentation
 
 We will also import and create a logger so that we can log the incoming
 data in our consuming function.
 
 ``` python
+from logging import getLogger
 from fastkafka import FastKafka
-from fastkafka._components.logger import get_logger
 
-logger = get_logger(__name__)
+logger = getLogger("Demo Kafka app")
 
 kafka_brokers = {
     "localhost": {
         "url": "localhost",
         "description": "local development kafka broker",
         "port": 9092,
     },
@@ -237,18 +237,18 @@
 
 msg = Data(
     data=0.1,
 )
 
 # Start Tester app and create InMemory Kafka broker for testing
 async with Tester(kafka_app) as tester:
-    # Send IrisInputData message to input_data topic
+    # Send Data message to input_data topic
     await tester.to_input_data(msg)
 
-    # Assert that the kafka_app responded with IrisPrediction in predictions topic
+    # Assert that the kafka_app responded with incremented data in output_data topic
     await tester.awaited_mocks.on_output_data.assert_awaited_with(
         Data(data=1.1), timeout=2
     )
 ```
 
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._start() called
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._patch_consumers_and_producers(): Patching consumers and producers!
@@ -267,15 +267,15 @@
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'earliest', 'max_poll_records': 100}
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched start() called()
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched subscribe() called
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer.subscribe(), subscribing to: ['output_data']
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
-    [INFO] __main__: Got data: 0.1
+    [INFO] Demo Kafka app: Got data: 0.1
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched stop() called
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaProducer patched stop() called
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched stop() called
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
@@ -359,86 +359,87 @@
 app simbol to the command.
 
 `shell fastkafka run --num-workers=1 --kafka-broker localhost application:kafka_app`
 
 After running the command, you should see the following output in your
 command line:
 
-    [7262]: 23-05-22 12:16:07.361 [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
-    [7260]: 23-05-22 12:16:07.361 [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
-    [7260]: 23-05-22 12:16:07.361 [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
-    [7262]: 23-05-22 12:16:07.361 [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
-    [7260]: 23-05-22 12:16:07.388 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
-    [7260]: 23-05-22 12:16:07.388 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
-    [7262]: 23-05-22 12:16:07.389 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
-    [7262]: 23-05-22 12:16:07.389 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
-    [7260]: 23-05-22 12:16:07.396 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
-    [7260]: 23-05-22 12:16:07.396 [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
-    [7260]: 23-05-22 12:16:07.396 [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
-    [7260]: 23-05-22 12:16:07.396 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
-    [7262]: 23-05-22 12:16:07.400 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
-    [7262]: 23-05-22 12:16:07.400 [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
-    [7262]: 23-05-22 12:16:07.401 [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
-    [7262]: 23-05-22 12:16:07.401 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
-    [7262]: 23-05-22 12:16:07.412 [ERROR] aiokafka.cluster: Topic input_data not found in cluster metadata
-    [7262]: 23-05-22 12:16:07.412 [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
-    [7260]: 23-05-22 12:16:07.482 [WARNING] aiokafka.cluster: Topic input_data is not available during auto-create initialization
-    [7260]: 23-05-22 12:16:07.482 [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
-    [7262]: 23-05-22 12:16:12.865 [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('172.18.0.2', 9092)
-    [7262]: 23-05-22 12:16:12.865 [ERROR] aiokafka: Unable to update metadata from [0]
-    [7260]: 23-05-22 12:16:12.866 [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('172.18.0.2', 9092)
-    [7260]: 23-05-22 12:16:12.866 [ERROR] aiokafka: Unable to update metadata from [0]
-    ^C
-    [7262]: 23-05-22 12:16:12.978 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
-    [7262]: 23-05-22 12:16:12.979 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
+    [1504]: 23-05-31 11:36:45.874 [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
+    [1504]: 23-05-31 11:36:45.875 [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
+    [1504]: 23-05-31 11:36:45.937 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
+    [1504]: 23-05-31 11:36:45.937 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
+    [1504]: 23-05-31 11:36:45.956 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
+    [1504]: 23-05-31 11:36:45.956 [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
+    [1504]: 23-05-31 11:36:45.956 [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
+    [1504]: 23-05-31 11:36:45.956 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
+    [1506]: 23-05-31 11:36:45.993 [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
+    [1506]: 23-05-31 11:36:45.994 [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
+    [1506]: 23-05-31 11:36:46.014 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
+    [1506]: 23-05-31 11:36:46.015 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
+    [1506]: 23-05-31 11:36:46.040 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
+    [1506]: 23-05-31 11:36:46.042 [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
+    [1506]: 23-05-31 11:36:46.043 [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
+    [1506]: 23-05-31 11:36:46.043 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
+    [1506]: 23-05-31 11:36:46.068 [ERROR] aiokafka.cluster: Topic input_data not found in cluster metadata
+    [1506]: 23-05-31 11:36:46.070 [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
+    [1504]: 23-05-31 11:36:46.131 [WARNING] aiokafka.cluster: Topic input_data is not available during auto-create initialization
+    [1504]: 23-05-31 11:36:46.132 [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
+    [1506]: 23-05-31 11:37:00.237 [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('172.28.0.12', 9092)
+    [1506]: 23-05-31 11:37:00.237 [ERROR] aiokafka: Unable to update metadata from [0]
+    [1504]: 23-05-31 11:37:00.238 [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('172.28.0.12', 9092)
+    [1504]: 23-05-31 11:37:00.238 [ERROR] aiokafka: Unable to update metadata from [0]
+    [1506]: 23-05-31 11:37:00.294 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
+    [1506]: 23-05-31 11:37:00.294 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
     Starting process cleanup, this may take a few seconds...
-    23-05-22 12:16:12.997 [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 7260...
-    23-05-22 12:16:12.998 [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 7262...
-    [7260]: 23-05-22 12:16:13.035 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
-    [7260]: 23-05-22 12:16:13.035 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
+    23-05-31 11:37:00.345 [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 1504...
+    23-05-31 11:37:00.345 [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 1506...
+    [1504]: 23-05-31 11:37:00.347 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
+    [1504]: 23-05-31 11:37:00.347 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
+    23-05-31 11:37:00.607 [INFO] fastkafka._server: terminate_asyncio_process(): Process 1506 was already terminated.
+    23-05-31 11:37:00.822 [INFO] fastkafka._server: terminate_asyncio_process(): Process 1504 was already terminated.
 
 ## Documentation
 
 The kafka app comes with builtin documentation generation using
 [AsyncApi HTML generator](https://www.asyncapi.com/tools/generator).
 
 AsyncApi requires Node.js to be installed and we provide the following
 convenience command line for it:
 
 ``` sh
 fastkafka docs install_deps
 ```
 
-    23-05-22 12:17:03.425 [INFO] fastkafka._components.docs_dependencies: AsyncAPI generator installed
+    23-05-31 11:38:24.128 [INFO] fastkafka._components.docs_dependencies: AsyncAPI generator installed
 
 To generate the documentation programatically you just need to call the
-folloving command:
+following command:
 
 ``` sh
 fastkafka docs generate application:kafka_app
 ```
 
-    23-05-22 12:17:04.268 [INFO] fastkafka._components.asyncapi: New async specifications generated at: '/work/fastkafka/nbs/asyncapi/spec/asyncapi.yml'
-    23-05-22 12:17:13.777 [INFO] fastkafka._components.asyncapi: Async docs generated at 'asyncapi/docs'
-    23-05-22 12:17:13.777 [INFO] fastkafka._components.asyncapi: Output of '$ npx -y -p @asyncapi/generator ag asyncapi/spec/asyncapi.yml @asyncapi/html-template -o asyncapi/docs --force-write'
+    23-05-31 11:38:25.113 [INFO] fastkafka._components.asyncapi: Old async specifications at '/content/asyncapi/spec/asyncapi.yml' does not exist.
+    23-05-31 11:38:25.118 [INFO] fastkafka._components.asyncapi: New async specifications generated at: '/content/asyncapi/spec/asyncapi.yml'
+    23-05-31 11:38:43.455 [INFO] fastkafka._components.asyncapi: Async docs generated at 'asyncapi/docs'
+    23-05-31 11:38:43.455 [INFO] fastkafka._components.asyncapi: Output of '$ npx -y -p @asyncapi/generator ag asyncapi/spec/asyncapi.yml @asyncapi/html-template -o asyncapi/docs --force-write'
 
     Done! ✨
-    Check out your shiny new generated files at /work/fastkafka/nbs/asyncapi/docs.
+    Check out your shiny new generated files at /content/asyncapi/docs.
 
-. This will generate the *asyncapi* folder in relative path where all
-your documentation will be saved. You can check out the content of it
-with:
+This will generate the *asyncapi* folder in relative path where all your
+documentation will be saved. You can check out the content of it with:
 
 ``` sh
 ls -l asyncapi
 ```
 
-    total 2
-    drwxrwxr-x 4 tvrtko tvrtko 5 Mar 29 09:57 docs
-    drwxrwxr-x 2 tvrtko tvrtko 3 Mar 29 09:56 spec
+    total 8
+    drwxr-xr-x 4 root root 4096 May 31 11:38 docs
+    drwxr-xr-x 2 root root 4096 May 31 11:38 spec
 
 In docs folder you will find the servable static html file of your
 documentation. This can also be served using our `fastkafka docs serve`
 CLI command (more on that in our guides).
 
 In spec folder you will find a asyncapi.yml file containing the async
 API specification of your application.
@@ -446,24 +447,27 @@
 We can locally preview the generated documentation by running the
 following command:
 
 ``` sh
 fastkafka docs serve application:kafka_app
 ```
 
-    23-05-22 12:17:14.784 [INFO] fastkafka._components.asyncapi: New async specifications generated at: '/work/fastkafka/nbs/asyncapi/spec/asyncapi.yml'
-    23-05-22 12:17:24.450 [INFO] fastkafka._components.asyncapi: Async docs generated at 'asyncapi/docs'
-    23-05-22 12:17:24.450 [INFO] fastkafka._components.asyncapi: Output of '$ npx -y -p @asyncapi/generator ag asyncapi/spec/asyncapi.yml @asyncapi/html-template -o asyncapi/docs --force-write'
+    23-05-31 11:38:45.250 [INFO] fastkafka._components.asyncapi: New async specifications generated at: '/content/asyncapi/spec/asyncapi.yml'
+    23-05-31 11:39:04.410 [INFO] fastkafka._components.asyncapi: Async docs generated at 'asyncapi/docs'
+    23-05-31 11:39:04.411 [INFO] fastkafka._components.asyncapi: Output of '$ npx -y -p @asyncapi/generator ag asyncapi/spec/asyncapi.yml @asyncapi/html-template -o asyncapi/docs --force-write'
 
     Done! ✨
-    Check out your shiny new generated files at /work/fastkafka/nbs/asyncapi/docs.
+    Check out your shiny new generated files at /content/asyncapi/docs.
 
 
     Serving documentation on http://127.0.0.1:8000
-    ^C
+    127.0.0.1 - - [31/May/2023 11:39:14] "GET / HTTP/1.1" 200 -
+    127.0.0.1 - - [31/May/2023 11:39:14] "GET /css/global.min.css HTTP/1.1" 200 -
+    127.0.0.1 - - [31/May/2023 11:39:14] "GET /js/asyncapi-ui.min.js HTTP/1.1" 200 -
+    127.0.0.1 - - [31/May/2023 11:39:14] "GET /css/asyncapi.min.css HTTP/1.1" 200 -
     Interupting serving of documentation and cleaning up...
 
 From the parameters passed to the application constructor, we get the
 documentation bellow:
 
 ``` python
 from fastkafka import FastKafka
@@ -480,15 +484,15 @@
         "port": 9092,
         "protocol": "kafka-secure",
         "security": {"type": "plain"},
     },
 }
 
 kafka_app = FastKafka(
-    title="Iris predictions",
+    title="Demo Kafka app",
     kafka_brokers=kafka_brokers,
 )
 ```
 
 ![Kafka_servers](https://raw.githubusercontent.com/airtai/fastkafka/main/nbs/images/screenshot-kafka-servers.png)
 
 The following documentation snippet are for the consumer as specified in
```

### Comparing `fastkafka-0.7.0rc1/fastkafka/__init__.py` & `fastkafka-0.7.0rc2/fastkafka/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.0rc1"
+__version__ = "0.7.0rc2"
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/010_Application_export.ipynb.
 
 # %% auto 0
 __all__ = ['dummy']
 
 # %% ../nbs/010_Application_export.ipynb 1
 from ._application.app import FastKafka
```

### Comparing `fastkafka-0.7.0rc1/fastkafka/_application/app.py` & `fastkafka-0.7.0rc2/fastkafka/_application/app.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_application/tester.py` & `fastkafka-0.7.0rc2/fastkafka/_application/tester.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_cli.py` & `fastkafka-0.7.0rc2/fastkafka/_cli.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_cli_docs.py` & `fastkafka-0.7.0rc2/fastkafka/_cli_docs.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 __all__ = ['logger', 'docs_install_deps', 'generate_docs', 'serve_docs']
 
 # %% ../nbs/024_CLI_Docs.ipynb 1
 import asyncio
 import signal
 import socketserver
 from http.server import SimpleHTTPRequestHandler
+from pathlib import Path
 from types import FrameType
 from typing import *
 
 import typer
 
 from fastkafka._components.docs_dependencies import (
     _check_npm_with_local,
@@ -55,16 +56,18 @@
 
 
 @_docs_app.command(
     "generate",
     help="Generates documentation for a FastKafka application",
 )
 def generate_docs(
-    root_path: str = typer.Option(
-        ".", help="root path under which documentation will be created"
+    root_path: Optional[str] = typer.Option(
+        default=None,
+        help="root path under which documentation will be created; default is current directory",
+        show_default=False,
     ),
     app: str = typer.Argument(
         ...,
         help="input in the form of 'path:app', where **path** is the path to a python file and **app** is an object of type **FastKafka**.",
     ),
 ) -> None:
     """
@@ -77,28 +80,34 @@
             file and **app** is an object of type **FastKafka**.
 
     Raises:
         typer.Exit: If there is an unexpected internal error.
     """
     try:
         application = _import_from_string(app)
+        if root_path is not None:
+            application._root_path = Path(root_path)
+            application._asyncapi_path = application._root_path / "asyncapi"
+
         application.skip_docs = False
         application.create_docs()
     except Exception as e:
         typer.secho(f"Unexpected internal error: {e}", err=True, fg=typer.colors.RED)
         raise typer.Exit(1)
 
 
 @_docs_app.command(
     "serve",
     help="Generates and serves documentation for a FastKafka application",
 )
 def serve_docs(
     root_path: str = typer.Option(
-        ".", help="root path under which documentation will be created"
+        default=None,
+        help="root path under which documentation will be created; default is current directory",
+        show_default=False,
     ),
     bind: str = typer.Option("127.0.0.1", help="Some info"),
     port: int = typer.Option(8000, help="Some info"),
     app: str = typer.Argument(
         ...,
         help="input in the form of 'path:app', where **path** is the path to a python file and **app** is an object of type **FastKafka**.",
     ),
@@ -115,16 +124,20 @@
             file and **app** is an object of type **FastKafka**.
 
     Raises:
         typer.Exit: If there is an unexpected internal error.
     """
     try:
         application = _import_from_string(app)
+        if root_path is not None:
+            application._root_path = Path(root_path)
+            application._asyncapi_path = application._root_path / "asyncapi"
+
         application.create_docs()
-        with change_dir(application._root_path / "asyncapi" / "docs/"):
+        with change_dir(str(application._asyncapi_path / "docs")):
             server_address = (bind, port)
             handler = SimpleHTTPRequestHandler
 
             d = {"should_stop": False}
 
             def sigint_handler(
                 signal: int, frame: Optional[FrameType], d: Dict[str, bool] = d
```

### Comparing `fastkafka-0.7.0rc1/fastkafka/_cli_testing.py` & `fastkafka-0.7.0rc2/fastkafka/_cli_testing.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_components/_subprocess.py` & `fastkafka-0.7.0rc2/fastkafka/_components/_subprocess.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_components/aiokafka_consumer_loop.py` & `fastkafka-0.7.0rc2/fastkafka/_components/aiokafka_consumer_loop.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_components/asyncapi.py` & `fastkafka-0.7.0rc2/fastkafka/_components/asyncapi.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_components/benchmarking.py` & `fastkafka-0.7.0rc2/fastkafka/_components/benchmarking.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_components/docs_dependencies.py` & `fastkafka-0.7.0rc2/fastkafka/_components/docs_dependencies.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_components/encoder/avro.py` & `fastkafka-0.7.0rc2/fastkafka/_components/encoder/avro.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_components/encoder/json.py` & `fastkafka-0.7.0rc2/fastkafka/_components/encoder/json.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_components/helpers.py` & `fastkafka-0.7.0rc2/fastkafka/_components/helpers.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_components/logger.py` & `fastkafka-0.7.0rc2/fastkafka/_components/logger.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_components/meta.py` & `fastkafka-0.7.0rc2/fastkafka/_components/meta.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_components/producer_decorator.py` & `fastkafka-0.7.0rc2/fastkafka/_components/producer_decorator.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_components/task_streaming.py` & `fastkafka-0.7.0rc2/fastkafka/_components/task_streaming.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_components/test_dependencies.py` & `fastkafka-0.7.0rc2/fastkafka/_components/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_docusaurus_helper.py` & `fastkafka-0.7.0rc2/fastkafka/_docusaurus_helper.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_helpers.py` & `fastkafka-0.7.0rc2/fastkafka/_helpers.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_modidx.py` & `fastkafka-0.7.0rc2/fastkafka/_modidx.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_server.py` & `fastkafka-0.7.0rc2/fastkafka/_server.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_testing/apache_kafka_broker.py` & `fastkafka-0.7.0rc2/fastkafka/_testing/apache_kafka_broker.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_testing/in_memory_broker.py` & `fastkafka-0.7.0rc2/fastkafka/_testing/in_memory_broker.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_testing/local_redpanda_broker.py` & `fastkafka-0.7.0rc2/fastkafka/_testing/local_redpanda_broker.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/_testing/test_utils.py` & `fastkafka-0.7.0rc2/fastkafka/_testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/encoder.py` & `fastkafka-0.7.0rc2/fastkafka/encoder.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka/testing.py` & `fastkafka-0.7.0rc2/fastkafka/testing.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka.egg-info/PKG-INFO` & `fastkafka-0.7.0rc2/fastkafka.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastkafka
-Version: 0.7.0rc1
+Version: 0.7.0rc2
 Summary: FastKafka is a powerful and easy-to-use Python library for building asynchronous web services that interact with Kafka topics. Built on top of FastAPI, Starlette, Pydantic, AIOKafka and AsyncAPI, FastKafka simplifies the process of writing producers and consumers for Kafka topics.
 Home-page: https://github.com/airtai/fastkafka
 Author: airt
 Author-email: info@airt.ai
 License: Apache Software License 2.0
 Project-URL: Bug Tracker, https://github.com/airtai/fastkafka/issues
 Project-URL: CI, https://github.com/airtai/fastkafka/actions
@@ -108,19 +108,19 @@
 
 ``` sh
 pip install fastkafka[test,docs]
 ```
 
 ## Tutorial
 
-You can start an interactive and extensive tutorial in Google Colab by
-clicking the button below:
+You can start an interactive tutorial in Google Colab by clicking the
+button below:
 
-<a href="https://colab.research.google.com/github/airtai/fastkafka/blob/main/nbs/guides/Guide_00_FastKafka_Demo.ipynb" target=”_blank”>
-<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" />
+<a href="https://colab.research.google.com/github/airtai/fastkafka/blob/main/nbs/index.ipynb" target=”_blank”>
+<img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open in Colab" />
 </a>
 
 ## Writing server code
 
 To demonstrate FastKafka simplicity of using `@produces` and `@consumes`
 decorators, we will focus on a simple app.
 
@@ -171,18 +171,18 @@
 
 - `kafka_brokers`: a dictionary used for generation of documentation
 
 We will also import and create a logger so that we can log the incoming
 data in our consuming function.
 
 ``` python
+from logging import getLogger
 from fastkafka import FastKafka
-from fastkafka._components.logger import get_logger
 
-logger = get_logger(__name__)
+logger = getLogger("Demo Kafka app")
 
 kafka_brokers = {
     "localhost": {
         "url": "localhost",
         "description": "local development kafka broker",
         "port": 9092,
     },
@@ -267,18 +267,18 @@
 
 msg = Data(
     data=0.1,
 )
 
 # Start Tester app and create InMemory Kafka broker for testing
 async with Tester(kafka_app) as tester:
-    # Send IrisInputData message to input_data topic
+    # Send Data message to input_data topic
     await tester.to_input_data(msg)
 
-    # Assert that the kafka_app responded with IrisPrediction in predictions topic
+    # Assert that the kafka_app responded with incremented data in output_data topic
     await tester.awaited_mocks.on_output_data.assert_awaited_with(
         Data(data=1.1), timeout=2
     )
 ```
 
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._start() called
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._patch_consumers_and_producers(): Patching consumers and producers!
@@ -297,15 +297,15 @@
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'earliest', 'max_poll_records': 100}
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched start() called()
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched subscribe() called
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer.subscribe(), subscribing to: ['output_data']
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
-    [INFO] __main__: Got data: 0.1
+    [INFO] Demo Kafka app: Got data: 0.1
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched stop() called
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaProducer patched stop() called
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched stop() called
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
@@ -389,86 +389,87 @@
 app simbol to the command.
 
 `shell fastkafka run --num-workers=1 --kafka-broker localhost application:kafka_app`
 
 After running the command, you should see the following output in your
 command line:
 
-    [7262]: 23-05-22 12:16:07.361 [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
-    [7260]: 23-05-22 12:16:07.361 [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
-    [7260]: 23-05-22 12:16:07.361 [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
-    [7262]: 23-05-22 12:16:07.361 [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
-    [7260]: 23-05-22 12:16:07.388 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
-    [7260]: 23-05-22 12:16:07.388 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
-    [7262]: 23-05-22 12:16:07.389 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
-    [7262]: 23-05-22 12:16:07.389 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
-    [7260]: 23-05-22 12:16:07.396 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
-    [7260]: 23-05-22 12:16:07.396 [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
-    [7260]: 23-05-22 12:16:07.396 [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
-    [7260]: 23-05-22 12:16:07.396 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
-    [7262]: 23-05-22 12:16:07.400 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
-    [7262]: 23-05-22 12:16:07.400 [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
-    [7262]: 23-05-22 12:16:07.401 [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
-    [7262]: 23-05-22 12:16:07.401 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
-    [7262]: 23-05-22 12:16:07.412 [ERROR] aiokafka.cluster: Topic input_data not found in cluster metadata
-    [7262]: 23-05-22 12:16:07.412 [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
-    [7260]: 23-05-22 12:16:07.482 [WARNING] aiokafka.cluster: Topic input_data is not available during auto-create initialization
-    [7260]: 23-05-22 12:16:07.482 [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
-    [7262]: 23-05-22 12:16:12.865 [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('172.18.0.2', 9092)
-    [7262]: 23-05-22 12:16:12.865 [ERROR] aiokafka: Unable to update metadata from [0]
-    [7260]: 23-05-22 12:16:12.866 [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('172.18.0.2', 9092)
-    [7260]: 23-05-22 12:16:12.866 [ERROR] aiokafka: Unable to update metadata from [0]
-    ^C
-    [7262]: 23-05-22 12:16:12.978 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
-    [7262]: 23-05-22 12:16:12.979 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
+    [1504]: 23-05-31 11:36:45.874 [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
+    [1504]: 23-05-31 11:36:45.875 [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
+    [1504]: 23-05-31 11:36:45.937 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
+    [1504]: 23-05-31 11:36:45.937 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
+    [1504]: 23-05-31 11:36:45.956 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
+    [1504]: 23-05-31 11:36:45.956 [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
+    [1504]: 23-05-31 11:36:45.956 [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
+    [1504]: 23-05-31 11:36:45.956 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
+    [1506]: 23-05-31 11:36:45.993 [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
+    [1506]: 23-05-31 11:36:45.994 [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
+    [1506]: 23-05-31 11:36:46.014 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
+    [1506]: 23-05-31 11:36:46.015 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
+    [1506]: 23-05-31 11:36:46.040 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
+    [1506]: 23-05-31 11:36:46.042 [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
+    [1506]: 23-05-31 11:36:46.043 [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
+    [1506]: 23-05-31 11:36:46.043 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
+    [1506]: 23-05-31 11:36:46.068 [ERROR] aiokafka.cluster: Topic input_data not found in cluster metadata
+    [1506]: 23-05-31 11:36:46.070 [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
+    [1504]: 23-05-31 11:36:46.131 [WARNING] aiokafka.cluster: Topic input_data is not available during auto-create initialization
+    [1504]: 23-05-31 11:36:46.132 [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
+    [1506]: 23-05-31 11:37:00.237 [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('172.28.0.12', 9092)
+    [1506]: 23-05-31 11:37:00.237 [ERROR] aiokafka: Unable to update metadata from [0]
+    [1504]: 23-05-31 11:37:00.238 [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('172.28.0.12', 9092)
+    [1504]: 23-05-31 11:37:00.238 [ERROR] aiokafka: Unable to update metadata from [0]
+    [1506]: 23-05-31 11:37:00.294 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
+    [1506]: 23-05-31 11:37:00.294 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
     Starting process cleanup, this may take a few seconds...
-    23-05-22 12:16:12.997 [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 7260...
-    23-05-22 12:16:12.998 [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 7262...
-    [7260]: 23-05-22 12:16:13.035 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
-    [7260]: 23-05-22 12:16:13.035 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
+    23-05-31 11:37:00.345 [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 1504...
+    23-05-31 11:37:00.345 [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 1506...
+    [1504]: 23-05-31 11:37:00.347 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
+    [1504]: 23-05-31 11:37:00.347 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
+    23-05-31 11:37:00.607 [INFO] fastkafka._server: terminate_asyncio_process(): Process 1506 was already terminated.
+    23-05-31 11:37:00.822 [INFO] fastkafka._server: terminate_asyncio_process(): Process 1504 was already terminated.
 
 ## Documentation
 
 The kafka app comes with builtin documentation generation using
 [AsyncApi HTML generator](https://www.asyncapi.com/tools/generator).
 
 AsyncApi requires Node.js to be installed and we provide the following
 convenience command line for it:
 
 ``` sh
 fastkafka docs install_deps
 ```
 
-    23-05-22 12:17:03.425 [INFO] fastkafka._components.docs_dependencies: AsyncAPI generator installed
+    23-05-31 11:38:24.128 [INFO] fastkafka._components.docs_dependencies: AsyncAPI generator installed
 
 To generate the documentation programatically you just need to call the
-folloving command:
+following command:
 
 ``` sh
 fastkafka docs generate application:kafka_app
 ```
 
-    23-05-22 12:17:04.268 [INFO] fastkafka._components.asyncapi: New async specifications generated at: '/work/fastkafka/nbs/asyncapi/spec/asyncapi.yml'
-    23-05-22 12:17:13.777 [INFO] fastkafka._components.asyncapi: Async docs generated at 'asyncapi/docs'
-    23-05-22 12:17:13.777 [INFO] fastkafka._components.asyncapi: Output of '$ npx -y -p @asyncapi/generator ag asyncapi/spec/asyncapi.yml @asyncapi/html-template -o asyncapi/docs --force-write'
+    23-05-31 11:38:25.113 [INFO] fastkafka._components.asyncapi: Old async specifications at '/content/asyncapi/spec/asyncapi.yml' does not exist.
+    23-05-31 11:38:25.118 [INFO] fastkafka._components.asyncapi: New async specifications generated at: '/content/asyncapi/spec/asyncapi.yml'
+    23-05-31 11:38:43.455 [INFO] fastkafka._components.asyncapi: Async docs generated at 'asyncapi/docs'
+    23-05-31 11:38:43.455 [INFO] fastkafka._components.asyncapi: Output of '$ npx -y -p @asyncapi/generator ag asyncapi/spec/asyncapi.yml @asyncapi/html-template -o asyncapi/docs --force-write'
 
     Done! ✨
-    Check out your shiny new generated files at /work/fastkafka/nbs/asyncapi/docs.
+    Check out your shiny new generated files at /content/asyncapi/docs.
 
-. This will generate the *asyncapi* folder in relative path where all
-your documentation will be saved. You can check out the content of it
-with:
+This will generate the *asyncapi* folder in relative path where all your
+documentation will be saved. You can check out the content of it with:
 
 ``` sh
 ls -l asyncapi
 ```
 
-    total 2
-    drwxrwxr-x 4 tvrtko tvrtko 5 Mar 29 09:57 docs
-    drwxrwxr-x 2 tvrtko tvrtko 3 Mar 29 09:56 spec
+    total 8
+    drwxr-xr-x 4 root root 4096 May 31 11:38 docs
+    drwxr-xr-x 2 root root 4096 May 31 11:38 spec
 
 In docs folder you will find the servable static html file of your
 documentation. This can also be served using our `fastkafka docs serve`
 CLI command (more on that in our guides).
 
 In spec folder you will find a asyncapi.yml file containing the async
 API specification of your application.
@@ -476,24 +477,27 @@
 We can locally preview the generated documentation by running the
 following command:
 
 ``` sh
 fastkafka docs serve application:kafka_app
 ```
 
-    23-05-22 12:17:14.784 [INFO] fastkafka._components.asyncapi: New async specifications generated at: '/work/fastkafka/nbs/asyncapi/spec/asyncapi.yml'
-    23-05-22 12:17:24.450 [INFO] fastkafka._components.asyncapi: Async docs generated at 'asyncapi/docs'
-    23-05-22 12:17:24.450 [INFO] fastkafka._components.asyncapi: Output of '$ npx -y -p @asyncapi/generator ag asyncapi/spec/asyncapi.yml @asyncapi/html-template -o asyncapi/docs --force-write'
+    23-05-31 11:38:45.250 [INFO] fastkafka._components.asyncapi: New async specifications generated at: '/content/asyncapi/spec/asyncapi.yml'
+    23-05-31 11:39:04.410 [INFO] fastkafka._components.asyncapi: Async docs generated at 'asyncapi/docs'
+    23-05-31 11:39:04.411 [INFO] fastkafka._components.asyncapi: Output of '$ npx -y -p @asyncapi/generator ag asyncapi/spec/asyncapi.yml @asyncapi/html-template -o asyncapi/docs --force-write'
 
     Done! ✨
-    Check out your shiny new generated files at /work/fastkafka/nbs/asyncapi/docs.
+    Check out your shiny new generated files at /content/asyncapi/docs.
 
 
     Serving documentation on http://127.0.0.1:8000
-    ^C
+    127.0.0.1 - - [31/May/2023 11:39:14] "GET / HTTP/1.1" 200 -
+    127.0.0.1 - - [31/May/2023 11:39:14] "GET /css/global.min.css HTTP/1.1" 200 -
+    127.0.0.1 - - [31/May/2023 11:39:14] "GET /js/asyncapi-ui.min.js HTTP/1.1" 200 -
+    127.0.0.1 - - [31/May/2023 11:39:14] "GET /css/asyncapi.min.css HTTP/1.1" 200 -
     Interupting serving of documentation and cleaning up...
 
 From the parameters passed to the application constructor, we get the
 documentation bellow:
 
 ``` python
 from fastkafka import FastKafka
@@ -510,15 +514,15 @@
         "port": 9092,
         "protocol": "kafka-secure",
         "security": {"type": "plain"},
     },
 }
 
 kafka_app = FastKafka(
-    title="Iris predictions",
+    title="Demo Kafka app",
     kafka_brokers=kafka_brokers,
 )
 ```
 
 ![Kafka_servers](https://raw.githubusercontent.com/airtai/fastkafka/main/nbs/images/screenshot-kafka-servers.png)
 
 The following documentation snippet are for the consumer as specified in
```

### Comparing `fastkafka-0.7.0rc1/fastkafka.egg-info/SOURCES.txt` & `fastkafka-0.7.0rc2/fastkafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/fastkafka.egg-info/requires.txt` & `fastkafka-0.7.0rc2/fastkafka.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc1/settings.ini` & `fastkafka-0.7.0rc2/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = fastkafka
 lib_name = %(repo)s
-version = 0.7.0rc1
+version = 0.7.0rc2
 min_python = 3.8
 license = apache2
 
 
 ### nbdev ###
 doc_path = _docs
 lib_path = fastkafka
```

### Comparing `fastkafka-0.7.0rc1/setup.py` & `fastkafka-0.7.0rc2/setup.py`

 * *Files identical despite different names*

