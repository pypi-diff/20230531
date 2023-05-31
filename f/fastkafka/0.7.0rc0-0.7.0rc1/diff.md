# Comparing `tmp/fastkafka-0.7.0rc0.tar.gz` & `tmp/fastkafka-0.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastkafka-0.7.0rc0.tar", last modified: Fri May 26 15:52:52 2023, max compression
+gzip compressed data, was "fastkafka-0.7.0rc1.tar", last modified: Wed May 31 06:50:20 2023, max compression
```

## Comparing `fastkafka-0.7.0rc0.tar` & `fastkafka-0.7.0rc1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-26 15:52:52.288406 fastkafka-0.7.0rc0/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    12621 2023-05-19 13:11:05.000000 fastkafka-0.7.0rc0/CONTRIBUTING.md
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    11357 2023-03-14 07:16:19.000000 fastkafka-0.7.0rc0/LICENSE
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      111 2023-03-14 07:16:19.000000 fastkafka-0.7.0rc0/MANIFEST.in
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    29859 2023-05-26 15:52:52.288406 fastkafka-0.7.0rc0/PKG-INFO
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    28431 2023-05-23 06:49:06.000000 fastkafka-0.7.0rc0/README.md
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-26 15:52:52.284406 fastkafka-0.7.0rc0/fastkafka/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      525 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/__init__.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-26 15:52:52.284406 fastkafka-0.7.0rc0/fastkafka/_application/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_application/__init__.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    32608 2023-05-26 15:49:57.000000 fastkafka-0.7.0rc0/fastkafka/_application/app.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     7773 2023-05-26 15:49:57.000000 fastkafka-0.7.0rc0/fastkafka/_application/tester.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1592 2023-05-26 15:49:57.000000 fastkafka-0.7.0rc0/fastkafka/_cli.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     3879 2023-05-26 15:49:57.000000 fastkafka-0.7.0rc0/fastkafka/_cli_docs.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      852 2023-05-26 15:49:57.000000 fastkafka-0.7.0rc0/fastkafka/_cli_testing.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-26 15:52:52.288406 fastkafka-0.7.0rc0/fastkafka/_components/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_components/__init__.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     3705 2023-05-26 15:49:57.000000 fastkafka-0.7.0rc0/fastkafka/_components/_subprocess.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13315 2023-05-26 15:49:56.000000 fastkafka-0.7.0rc0/fastkafka/_components/aiokafka_consumer_loop.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    16528 2023-05-26 15:49:56.000000 fastkafka-0.7.0rc0/fastkafka/_components/asyncapi.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     2905 2023-05-26 15:49:57.000000 fastkafka-0.7.0rc0/fastkafka/_components/benchmarking.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4695 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_components/docs_dependencies.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-26 15:52:52.288406 fastkafka-0.7.0rc0/fastkafka/_components/encoder/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_components/encoder/__init__.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13910 2023-05-26 15:49:57.000000 fastkafka-0.7.0rc0/fastkafka/_components/encoder/avro.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1630 2023-05-26 15:49:57.000000 fastkafka-0.7.0rc0/fastkafka/_components/encoder/json.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     3450 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_components/helpers.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4432 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_components/logger.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    12567 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_components/meta.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     5432 2023-05-26 15:49:56.000000 fastkafka-0.7.0rc0/fastkafka/_components/producer_decorator.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    11253 2023-05-26 15:49:56.000000 fastkafka-0.7.0rc0/fastkafka/_components/task_streaming.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     5090 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_components/test_dependencies.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    19749 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_docusaurus_helper.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    50531 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_helpers.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    81099 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_modidx.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     6049 2023-05-26 15:49:57.000000 fastkafka-0.7.0rc0/fastkafka/_server.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-26 15:52:52.288406 fastkafka-0.7.0rc0/fastkafka/_testing/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-26 15:49:58.000000 fastkafka-0.7.0rc0/fastkafka/_testing/__init__.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    19995 2023-05-26 15:49:55.000000 fastkafka-0.7.0rc0/fastkafka/_testing/apache_kafka_broker.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    20363 2023-05-26 15:49:55.000000 fastkafka-0.7.0rc0/fastkafka/_testing/in_memory_broker.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    12344 2023-05-26 15:49:56.000000 fastkafka-0.7.0rc0/fastkafka/_testing/local_redpanda_broker.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4592 2023-05-26 15:49:56.000000 fastkafka-0.7.0rc0/fastkafka/_testing/test_utils.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      598 2023-05-26 15:49:57.000000 fastkafka-0.7.0rc0/fastkafka/encoder.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      454 2023-05-26 15:49:56.000000 fastkafka-0.7.0rc0/fastkafka/executors.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      858 2023-05-26 15:49:55.000000 fastkafka-0.7.0rc0/fastkafka/testing.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-26 15:52:52.284406 fastkafka-0.7.0rc0/fastkafka.egg-info/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    29859 2023-05-26 15:52:52.000000 fastkafka-0.7.0rc0/fastkafka.egg-info/PKG-INFO
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1410 2023-05-26 15:52:52.000000 fastkafka-0.7.0rc0/fastkafka.egg-info/SOURCES.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        1 2023-05-26 15:52:52.000000 fastkafka-0.7.0rc0/fastkafka.egg-info/dependency_links.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      146 2023-05-26 15:52:52.000000 fastkafka-0.7.0rc0/fastkafka.egg-info/entry_points.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        1 2023-05-23 12:47:36.000000 fastkafka-0.7.0rc0/fastkafka.egg-info/not-zip-safe
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      643 2023-05-26 15:52:52.000000 fastkafka-0.7.0rc0/fastkafka.egg-info/requires.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)       10 2023-05-26 15:52:52.000000 fastkafka-0.7.0rc0/fastkafka.egg-info/top_level.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1231 2023-05-26 15:49:31.000000 fastkafka-0.7.0rc0/settings.ini
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)       38 2023-05-26 15:52:52.288406 fastkafka-0.7.0rc0/setup.cfg
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     3729 2023-05-23 06:49:06.000000 fastkafka-0.7.0rc0/setup.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 06:50:20.317315 fastkafka-0.7.0rc1/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    12621 2023-05-19 13:11:05.000000 fastkafka-0.7.0rc1/CONTRIBUTING.md
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    11357 2023-03-14 07:16:19.000000 fastkafka-0.7.0rc1/LICENSE
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      111 2023-03-14 07:16:19.000000 fastkafka-0.7.0rc1/MANIFEST.in
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    24097 2023-05-31 06:50:20.317315 fastkafka-0.7.0rc1/PKG-INFO
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    22669 2023-05-31 06:49:07.000000 fastkafka-0.7.0rc1/README.md
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 06:50:20.309315 fastkafka-0.7.0rc1/fastkafka/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      525 2023-05-31 06:37:28.000000 fastkafka-0.7.0rc1/fastkafka/__init__.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 06:50:20.313315 fastkafka-0.7.0rc1/fastkafka/_application/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 06:37:28.000000 fastkafka-0.7.0rc1/fastkafka/_application/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    39065 2023-05-31 06:37:26.000000 fastkafka-0.7.0rc1/fastkafka/_application/app.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    17537 2023-05-31 06:37:26.000000 fastkafka-0.7.0rc1/fastkafka/_application/tester.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     2108 2023-05-31 06:37:26.000000 fastkafka-0.7.0rc1/fastkafka/_cli.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     5110 2023-05-31 06:37:26.000000 fastkafka-0.7.0rc1/fastkafka/_cli_docs.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      996 2023-05-31 06:37:26.000000 fastkafka-0.7.0rc1/fastkafka/_cli_testing.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 06:50:20.313315 fastkafka-0.7.0rc1/fastkafka/_components/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 06:37:28.000000 fastkafka-0.7.0rc1/fastkafka/_components/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4698 2023-05-31 06:37:26.000000 fastkafka-0.7.0rc1/fastkafka/_components/_subprocess.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13315 2023-05-31 06:37:25.000000 fastkafka-0.7.0rc1/fastkafka/_components/aiokafka_consumer_loop.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    18656 2023-05-31 06:37:25.000000 fastkafka-0.7.0rc1/fastkafka/_components/asyncapi.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     2905 2023-05-31 06:37:26.000000 fastkafka-0.7.0rc1/fastkafka/_components/benchmarking.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     6991 2023-05-31 06:37:27.000000 fastkafka-0.7.0rc1/fastkafka/_components/docs_dependencies.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 06:50:20.317315 fastkafka-0.7.0rc1/fastkafka/_components/encoder/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 06:37:28.000000 fastkafka-0.7.0rc1/fastkafka/_components/encoder/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13910 2023-05-31 06:37:26.000000 fastkafka-0.7.0rc1/fastkafka/_components/encoder/avro.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1630 2023-05-31 06:37:26.000000 fastkafka-0.7.0rc1/fastkafka/_components/encoder/json.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4136 2023-05-31 06:37:27.000000 fastkafka-0.7.0rc1/fastkafka/_components/helpers.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4730 2023-05-31 06:37:28.000000 fastkafka-0.7.0rc1/fastkafka/_components/logger.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13150 2023-05-31 06:37:27.000000 fastkafka-0.7.0rc1/fastkafka/_components/meta.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     7403 2023-05-31 06:37:25.000000 fastkafka-0.7.0rc1/fastkafka/_components/producer_decorator.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    11998 2023-05-31 06:37:25.000000 fastkafka-0.7.0rc1/fastkafka/_components/task_streaming.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     7992 2023-05-31 06:37:27.000000 fastkafka-0.7.0rc1/fastkafka/_components/test_dependencies.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    20426 2023-05-31 06:37:27.000000 fastkafka-0.7.0rc1/fastkafka/_docusaurus_helper.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    51550 2023-05-31 06:37:27.000000 fastkafka-0.7.0rc1/fastkafka/_helpers.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    84393 2023-05-31 06:37:28.000000 fastkafka-0.7.0rc1/fastkafka/_modidx.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     8205 2023-05-31 06:37:26.000000 fastkafka-0.7.0rc1/fastkafka/_server.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 06:50:20.317315 fastkafka-0.7.0rc1/fastkafka/_testing/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 06:37:28.000000 fastkafka-0.7.0rc1/fastkafka/_testing/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    22761 2023-05-31 06:37:24.000000 fastkafka-0.7.0rc1/fastkafka/_testing/apache_kafka_broker.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    28873 2023-05-31 06:37:24.000000 fastkafka-0.7.0rc1/fastkafka/_testing/in_memory_broker.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    12344 2023-05-31 06:37:24.000000 fastkafka-0.7.0rc1/fastkafka/_testing/local_redpanda_broker.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4979 2023-05-31 06:37:24.000000 fastkafka-0.7.0rc1/fastkafka/_testing/test_utils.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      598 2023-05-31 06:37:26.000000 fastkafka-0.7.0rc1/fastkafka/encoder.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      454 2023-05-31 06:37:24.000000 fastkafka-0.7.0rc1/fastkafka/executors.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      858 2023-05-31 06:37:24.000000 fastkafka-0.7.0rc1/fastkafka/testing.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 06:50:20.313315 fastkafka-0.7.0rc1/fastkafka.egg-info/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    24097 2023-05-31 06:50:20.000000 fastkafka-0.7.0rc1/fastkafka.egg-info/PKG-INFO
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1410 2023-05-31 06:50:20.000000 fastkafka-0.7.0rc1/fastkafka.egg-info/SOURCES.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        1 2023-05-31 06:50:20.000000 fastkafka-0.7.0rc1/fastkafka.egg-info/dependency_links.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      146 2023-05-31 06:50:20.000000 fastkafka-0.7.0rc1/fastkafka.egg-info/entry_points.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        1 2023-05-23 12:47:36.000000 fastkafka-0.7.0rc1/fastkafka.egg-info/not-zip-safe
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      690 2023-05-31 06:50:20.000000 fastkafka-0.7.0rc1/fastkafka.egg-info/requires.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)       10 2023-05-31 06:50:20.000000 fastkafka-0.7.0rc1/fastkafka.egg-info/top_level.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1231 2023-05-31 06:37:13.000000 fastkafka-0.7.0rc1/settings.ini
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)       38 2023-05-31 06:50:20.317315 fastkafka-0.7.0rc1/setup.cfg
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     3777 2023-05-30 11:33:36.000000 fastkafka-0.7.0rc1/setup.py
```

### Comparing `fastkafka-0.7.0rc0/CONTRIBUTING.md` & `fastkafka-0.7.0rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc0/LICENSE` & `fastkafka-0.7.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc0/PKG-INFO` & `fastkafka-0.7.0rc1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastkafka
-Version: 0.7.0rc0
+Version: 0.7.0rc1
 Summary: FastKafka is a powerful and easy-to-use Python library for building asynchronous web services that interact with Kafka topics. Built on top of FastAPI, Starlette, Pydantic, AIOKafka and AsyncAPI, FastKafka simplifies the process of writing producers and consumers for Kafka topics.
 Home-page: https://github.com/airtai/fastkafka
 Author: airt
 Author-email: info@airt.ai
 License: Apache Software License 2.0
 Project-URL: Bug Tracker, https://github.com/airtai/fastkafka/issues
 Project-URL: CI, https://github.com/airtai/fastkafka/actions
@@ -24,16 +24,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: avro
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
-FastKafka
-================
+# FastKafka
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 <b>Effortless Kafka integration for your web services</b>
 
 ------------------------------------------------------------------------
 
@@ -109,126 +108,81 @@
 
 ``` sh
 pip install fastkafka[test,docs]
 ```
 
 ## Tutorial
 
-You can start an interactive tutorial in Google Colab by clicking the
-button below:
+You can start an interactive and extensive tutorial in Google Colab by
+clicking the button below:
 
 <a href="https://colab.research.google.com/github/airtai/fastkafka/blob/main/nbs/guides/Guide_00_FastKafka_Demo.ipynb" target=”_blank”>
 <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" />
 </a>
 
 ## Writing server code
 
-Here is an example python script using FastKafka that takes data from a
-Kafka topic, makes a prediction using a predictive model, and outputs
-the prediction to another Kafka topic.
-
-### Preparing the demo model
-
-First we will prepare our model using the Iris dataset so that we can
-demonstrate the predictions using FastKafka. The following call
-downloads the dataset and trains the model.
+To demonstrate FastKafka simplicity of using `@produces` and `@consumes`
+decorators, we will focus on a simple app.
 
-We will wrap the model creation into a lifespan of our app so that the
-model is created just before the app is started.
-
-``` python
-from contextlib import asynccontextmanager
-
-from sklearn.datasets import load_iris
-from sklearn.linear_model import LogisticRegression
-
-from fastkafka import FastKafka
-
-ml_models = {}
-
-
-@asynccontextmanager
-async def lifespan(app: FastKafka):
-    # Load the ML model
-    X, y = load_iris(return_X_y=True)
-    ml_models["iris_predictor"] = LogisticRegression(random_state=0, max_iter=500).fit(
-        X, y
-    )
-    yield
-    # Clean up the ML models and release the resources
-    ml_models.clear()
-```
+The app will consume jsons containig positive floats from one topic, log
+them and then produce incremented values to another topic.
 
 ### Messages
 
 FastKafka uses [Pydantic](https://docs.pydantic.dev/) to parse input
 JSON-encoded data into Python objects, making it easy to work with
 structured data in your Kafka-based applications. Pydantic’s
 [`BaseModel`](https://docs.pydantic.dev/usage/models/) class allows you
 to define messages using a declarative syntax, making it easy to specify
 the fields and types of your messages.
 
-This example defines two message classes for use in a FastKafka
-application:
+This example defines one `Data` mesage class. This Class will model the
+consumed and produced data in our app demo, it contains one
+`NonNegativeFloat` field `data` that will be logged and “processed”
+before being produced to another topic.
 
-- The `IrisInputData` class is used to represent input data for a
-  predictive model. It has four fields of type
-  [`NonNegativeFloat`](https://docs.pydantic.dev/usage/types/#constrained-types),
-  which is a subclass of float that only allows non-negative floating
-  point values.
-
-- The `IrisPrediction` class is used to represent the output of the
-  predictive model. It has a single field `species` of type string
-  representing the predicted species.
-
-These message classes will be used to parse and validate incoming data
-in Kafka consumers and producers.
+These message class will be used to parse and validate incoming data in
+Kafka consumers and producers.
 
 ``` python
 from pydantic import BaseModel, Field, NonNegativeFloat
 
 
-class IrisInputData(BaseModel):
-    sepal_length: NonNegativeFloat = Field(
-        ..., example=0.5, description="Sepal length in cm"
-    )
-    sepal_width: NonNegativeFloat = Field(
-        ..., example=0.5, description="Sepal width in cm"
+class Data(BaseModel):
+    data: NonNegativeFloat = Field(
+        ..., example=0.5, description="Float data example"
     )
-    petal_length: NonNegativeFloat = Field(
-        ..., example=0.5, description="Petal length in cm"
-    )
-    petal_width: NonNegativeFloat = Field(
-        ..., example=0.5, description="Petal width in cm"
-    )
-
-
-class IrisPrediction(BaseModel):
-    species: str = Field(..., example="setosa", description="Predicted species")
 ```
 
 ### Application
 
 This example shows how to initialize a FastKafka application.
 
 It starts by defining a dictionary called `kafka_brokers`, which
 contains two entries: `"localhost"` and `"production"`, specifying local
 development and production Kafka brokers. Each entry specifies the URL,
 port, and other details of a Kafka broker. This dictionary is used for
 both generating the documentation and later to run the actual server
 against one of the given kafka broker.
 
 Next, an object of the
-[`FastKafka`](https://fastkafka.airt.ai/docs/api/fastkafka)
+[`FastKafka`](https://fastkafka.airt.ai/docs/api/fastkafka#fastkafka.FastKafka)
 class is initialized with the minimum set of arguments:
 
 - `kafka_brokers`: a dictionary used for generation of documentation
 
+We will also import and create a logger so that we can log the incoming
+data in our consuming function.
+
 ``` python
 from fastkafka import FastKafka
+from fastkafka._components.logger import get_logger
+
+logger = get_logger(__name__)
 
 kafka_brokers = {
     "localhost": {
         "url": "localhost",
         "description": "local development kafka broker",
         "port": 9092,
     },
@@ -238,17 +192,16 @@
         "port": 9092,
         "protocol": "kafka-secure",
         "security": {"type": "plain"},
     },
 }
 
 kafka_app = FastKafka(
-    title="Iris predictions",
+    title="Demo Kafka app",
     kafka_brokers=kafka_brokers,
-    lifespan=lifespan,
 )
 ```
 
 ### Function decorators
 
 FastKafka provides convenient function decorators `@kafka_app.consumes`
 and `@kafka_app.produces` to allow you to delegate the actual process of
@@ -268,75 +221,66 @@
 This following example shows how to use the `@kafka_app.consumes` and
 `@kafka_app.produces` decorators in a FastKafka application:
 
 - The `@kafka_app.consumes` decorator is applied to the `on_input_data`
   function, which specifies that this function should be called whenever
   a message is received on the “input_data” Kafka topic. The
   `on_input_data` function takes a single argument which is expected to
-  be an instance of the `IrisInputData` message class. Specifying the
-  type of the single argument is instructing the Pydantic to use
-  `IrisInputData.parse_raw()` on the consumed message before passing it
-  to the user defined function `on_input_data`.
+  be an instance of the `Data` message class. Specifying the type of the
+  single argument is instructing the Pydantic to use `Data.parse_raw()`
+  on the consumed message before passing it to the user defined function
+  `on_input_data`.
 
-- The `@produces` decorator is applied to the `to_predictions` function,
+- The `@produces` decorator is applied to the `to_output_data` function,
   which specifies that this function should produce a message to the
-  “predictions” Kafka topic whenever it is called. The `to_predictions`
-  function takes a single integer argument `species_class` representing
-  one of three possible strign values predicted by the mdoel. It creates
-  a new `IrisPrediction` message using this value and then returns it.
-  The framework will call the `IrisPrediction.json().encode("utf-8")`
-  function on the returned value and produce it to the specified topic.
+  “output_data” Kafka topic whenever it is called. The `to_output_data`
+  function takes a single float argument `data`. It it increments the
+  data returns it wrapped in a `Data` object. The framework will call
+  the `Data.json().encode("utf-8")` function on the returned value and
+  produce it to the specified topic.
 
 ``` python
 @kafka_app.consumes(topic="input_data", auto_offset_reset="latest")
-async def on_input_data(msg: IrisInputData):
-    species_class = ml_models["iris_predictor"].predict(
-        [[msg.sepal_length, msg.sepal_width, msg.petal_length, msg.petal_width]]
-    )[0]
-
-    to_predictions(species_class)
-
+async def on_input_data(msg: Data):
+    logger.info(f"Got data: {msg.data}")
+    await to_output_data(msg.data)
 
-@kafka_app.produces(topic="predictions")
-def to_predictions(species_class: int) -> IrisPrediction:
-    iris_species = ["setosa", "versicolor", "virginica"]
 
-    prediction = IrisPrediction(species=iris_species[species_class])
-    return prediction
+@kafka_app.produces(topic="output_data")
+async def to_output_data(data: float) -> Data:
+    processed_data = Data(data=data+1.0)
+    return processed_data
 ```
 
 ## Testing the service
 
 The service can be tested using the
-[`Tester`](https://fastkafka.airt.ai/docs/api/fastkafka/testing/Tester)
+[`Tester`](https://fastkafka.airt.ai/docs/api/fastkafka/testing/Tester#fastkafka.testing.Tester)
 instances which internally starts InMemory implementation of Kafka
 broker.
 
 The Tester will redirect your consumes and produces decorated functions
 to the InMemory Kafka broker so that you can quickly test your app
 without the need for a running Kafka broker and all its dependencies.
 
 ``` python
 from fastkafka.testing import Tester
 
-msg = IrisInputData(
-    sepal_length=0.1,
-    sepal_width=0.2,
-    petal_length=0.3,
-    petal_width=0.4,
+msg = Data(
+    data=0.1,
 )
 
 # Start Tester app and create InMemory Kafka broker for testing
 async with Tester(kafka_app) as tester:
     # Send IrisInputData message to input_data topic
     await tester.to_input_data(msg)
 
     # Assert that the kafka_app responded with IrisPrediction in predictions topic
-    await tester.awaited_mocks.on_predictions.assert_awaited_with(
-        IrisPrediction(species="setosa"), timeout=2
+    await tester.awaited_mocks.on_output_data.assert_awaited_with(
+        Data(data=1.1), timeout=2
     )
 ```
 
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._start() called
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._patch_consumers_and_producers(): Patching consumers and producers!
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker starting
     [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
@@ -351,99 +295,66 @@
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer.subscribe(), subscribing to: ['input_data']
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'earliest', 'max_poll_records': 100}
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched start() called()
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched subscribe() called
-    [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer.subscribe(), subscribing to: ['predictions']
+    [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer.subscribe(), subscribing to: ['output_data']
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
-    [INFO] fastkafka._components.aiokafka_consumer_loop: _aiokafka_consumer_loop(): Consumer loop shutting down, waiting for send_stream to drain...
+    [INFO] __main__: Got data: 0.1
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched stop() called
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaProducer patched stop() called
-    [INFO] fastkafka._components.aiokafka_consumer_loop: _aiokafka_consumer_loop(): Consumer loop shutting down, waiting for send_stream to drain...
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched stop() called
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaProducer patched stop() called
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._stop() called
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker stopping
 
 ### Recap
 
-We have created a Iris classification model and encapulated it into our
-fastkafka application. The app will consume the IrisInputData from the
-`input_data` topic and produce the predictions to `predictions` topic.
+We have created a simple fastkafka application. The app will consume the
+`Data` from the `input_data` topic, log it and produce the incremented
+data to `output_data` topic.
 
 To test the app we have:
 
 1.  Created the app
 
 2.  Started our Tester class which mirrors the developed app topics for
     testing purposes
 
-3.  Sent IrisInputData message to `input_data` topic
+3.  Sent Data message to `input_data` topic
 
-4.  Asserted and checked that the developed iris classification service
-    has reacted to IrisInputData message
+4.  Asserted and checked that the developed service has reacted to Data
+    message
 
 ## Running the service
 
 The service can be started using builtin faskafka run CLI command.
 Before we can do that, we will concatenate the code snippets from above
 and save them in a file `"application.py"`
 
 ``` python
 # content of the "application.py" file
 
-from contextlib import asynccontextmanager
-
-from sklearn.datasets import load_iris
-from sklearn.linear_model import LogisticRegression
+from pydantic import BaseModel, Field, NonNegativeFloat
 
 from fastkafka import FastKafka
+from fastkafka._components.logger import get_logger
 
-ml_models = {}
+logger = get_logger(__name__)
 
-
-@asynccontextmanager
-async def lifespan(app: FastKafka):
-    # Load the ML model
-    X, y = load_iris(return_X_y=True)
-    ml_models["iris_predictor"] = LogisticRegression(random_state=0, max_iter=500).fit(
-        X, y
+class Data(BaseModel):
+    data: NonNegativeFloat = Field(
+        ..., example=0.5, description="Float data example"
     )
-    yield
-    # Clean up the ML models and release the resources
-    ml_models.clear()
-
-
-from pydantic import BaseModel, NonNegativeFloat, Field
-
-class IrisInputData(BaseModel):
-    sepal_length: NonNegativeFloat = Field(
-        ..., example=0.5, description="Sepal length in cm"
-    )
-    sepal_width: NonNegativeFloat = Field(
-        ..., example=0.5, description="Sepal width in cm"
-    )
-    petal_length: NonNegativeFloat = Field(
-        ..., example=0.5, description="Petal length in cm"
-    )
-    petal_width: NonNegativeFloat = Field(
-        ..., example=0.5, description="Petal width in cm"
-    )
-
-
-class IrisPrediction(BaseModel):
-    species: str = Field(..., example="setosa", description="Predicted species")
-    
-from fastkafka import FastKafka
 
 kafka_brokers = {
     "localhost": {
         "url": "localhost",
         "description": "local development kafka broker",
         "port": 9092,
     },
@@ -453,179 +364,111 @@
         "port": 9092,
         "protocol": "kafka-secure",
         "security": {"type": "plain"},
     },
 }
 
 kafka_app = FastKafka(
-    title="Iris predictions",
+    title="Demo Kafka app",
     kafka_brokers=kafka_brokers,
-    lifespan=lifespan,
 )
 
 @kafka_app.consumes(topic="input_data", auto_offset_reset="latest")
-async def on_input_data(msg: IrisInputData):
-    species_class = ml_models["iris_predictor"].predict(
-        [[msg.sepal_length, msg.sepal_width, msg.petal_length, msg.petal_width]]
-    )[0]
-
-    to_predictions(species_class)
-
-
-@kafka_app.produces(topic="predictions")
-def to_predictions(species_class: int) -> IrisPrediction:
-    iris_species = ["setosa", "versicolor", "virginica"]
-
-    prediction = IrisPrediction(species=iris_species[species_class])
-    return prediction
-```
-
-To run the service, you will need a running Kafka broker on localhost as
-specified in the `kafka_brokers` parameter above. We can start the Kafka
-broker locally using the
-[`ApacheKafkaBroker`](https://fastkafka.airt.ai/docs/api/fastkafka/testing/ApacheKafkaBroker).
-
-To use
-[`ApacheKafkaBroker`](https://fastkafka.airt.ai/docs/api/fastkafka/testing/ApacheKafkaBroker),
-you need to install JRE and Kafka to your environment. To simplify this
-process, fastkafka comes with a CLI command that does just that, to run
-it, in your terminal execute the following:
-
-``` sh
-fastkafka testing install_deps
-```
-
-Now we can run
-[`ApacheKafkaBroker`](https://fastkafka.airt.ai/docs/api/fastkafka/testing/ApacheKafkaBroker)
-that will start a Kafka broker instance for us.
-
-``` python
-from fastkafka.testing import ApacheKafkaBroker
-
-broker = ApacheKafkaBroker(apply_nest_asyncio=True)
-
-broker.start()
-```
-
-    [INFO] fastkafka._testing.apache_kafka_broker: ApacheKafkaBroker.start(): entering...
-    [WARNING] fastkafka._testing.apache_kafka_broker: ApacheKafkaBroker.start(): (<_UnixSelectorEventLoop running=True closed=False debug=False>) is already running!
-    [WARNING] fastkafka._testing.apache_kafka_broker: ApacheKafkaBroker.start(): calling nest_asyncio.apply()
-    [INFO] fastkafka._components.test_dependencies: Java is already installed.
-    [INFO] fastkafka._components.test_dependencies: But not exported to PATH, exporting...
-    [INFO] fastkafka._components.test_dependencies: Kafka is installed.
-    [INFO] fastkafka._components.test_dependencies: But not exported to PATH, exporting...
-    [INFO] fastkafka._testing.apache_kafka_broker: Starting zookeeper...
-    [INFO] fastkafka._testing.apache_kafka_broker: Starting kafka...
-    [INFO] fastkafka._testing.apache_kafka_broker: Local Kafka broker up and running on 127.0.0.1:9092
-    [INFO] fastkafka._testing.apache_kafka_broker: <class 'fastkafka.testing.ApacheKafkaBroker'>.start(): returning 127.0.0.1:9092
-    [INFO] fastkafka._testing.apache_kafka_broker: ApacheKafkaBroker.start(): exited.
-
-    '127.0.0.1:9092'
-
-Then, we start the FastKafka service by running the following command in
-the folder where the `application.py` file is located:
-
-``` sh
-fastkafka run --num-workers=2 --kafka-broker localhost application:kafka_app
-```
-
-In the above command, we use `--num-workers` option to specify how many
-workers to launch and we use `--kafka-broker` option to specify which
-kafka broker configuration to use from earlier specified `kafka_brokers`
-
-    [801767]: [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
-    [801765]: [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
-    [801767]: [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
-    [801765]: [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
-    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
-    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
-    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
-    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
-    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
-    [801767]: [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
-    [801767]: [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
-    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
-    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
-    [801765]: [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
-    [801765]: [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
-    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
-    [801765]: [ERROR] aiokafka.cluster: Topic input_data not found in cluster metadata
-    [801765]: [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
-    [801767]: [WARNING] aiokafka.cluster: Topic input_data is not available during auto-create initialization
-    [801767]: [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
-    [801767]: [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('192.168.112.2', 9092)
-    [801765]: [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('192.168.112.2', 9092)
-    [801767]: [ERROR] aiokafka: Unable to update metadata from [0]
-    [801765]: [ERROR] aiokafka: Unable to update metadata from [0]
+async def on_input_data(msg: Data):
+    logger.info(f"Got data: {msg.data}")
+    await to_output_data(msg.data)
+
+
+@kafka_app.produces(topic="output_data")
+async def to_output_data(data: float) -> Data:
+    processed_data = Data(data=data+1.0)
+    return processed_data
+```
+
+To run the service, use the FastKafka CLI command and pass the module
+(in this case, the file where the app implementation is located) and the
+app simbol to the command.
+
+`shell fastkafka run --num-workers=1 --kafka-broker localhost application:kafka_app`
+
+After running the command, you should see the following output in your
+command line:
+
+    [7262]: 23-05-22 12:16:07.361 [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
+    [7260]: 23-05-22 12:16:07.361 [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
+    [7260]: 23-05-22 12:16:07.361 [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
+    [7262]: 23-05-22 12:16:07.361 [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
+    [7260]: 23-05-22 12:16:07.388 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
+    [7260]: 23-05-22 12:16:07.388 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
+    [7262]: 23-05-22 12:16:07.389 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
+    [7262]: 23-05-22 12:16:07.389 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
+    [7260]: 23-05-22 12:16:07.396 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
+    [7260]: 23-05-22 12:16:07.396 [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
+    [7260]: 23-05-22 12:16:07.396 [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
+    [7260]: 23-05-22 12:16:07.396 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
+    [7262]: 23-05-22 12:16:07.400 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
+    [7262]: 23-05-22 12:16:07.400 [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
+    [7262]: 23-05-22 12:16:07.401 [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
+    [7262]: 23-05-22 12:16:07.401 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
+    [7262]: 23-05-22 12:16:07.412 [ERROR] aiokafka.cluster: Topic input_data not found in cluster metadata
+    [7262]: 23-05-22 12:16:07.412 [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
+    [7260]: 23-05-22 12:16:07.482 [WARNING] aiokafka.cluster: Topic input_data is not available during auto-create initialization
+    [7260]: 23-05-22 12:16:07.482 [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
+    [7262]: 23-05-22 12:16:12.865 [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('172.18.0.2', 9092)
+    [7262]: 23-05-22 12:16:12.865 [ERROR] aiokafka: Unable to update metadata from [0]
+    [7260]: 23-05-22 12:16:12.866 [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('172.18.0.2', 9092)
+    [7260]: 23-05-22 12:16:12.866 [ERROR] aiokafka: Unable to update metadata from [0]
     ^C
+    [7262]: 23-05-22 12:16:12.978 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
+    [7262]: 23-05-22 12:16:12.979 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
     Starting process cleanup, this may take a few seconds...
-    [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 801765...
-    [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 801767...
-    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: _aiokafka_consumer_loop(): Consumer loop shutting down, waiting for send_stream to drain...
-    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
-    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
-    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: _aiokafka_consumer_loop(): Consumer loop shutting down, waiting for send_stream to drain...
-    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
-    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
-
-You need to interupt running of the cell above by selecting
-`Runtime->Interupt execution` on the toolbar above.
-
-Finally, we can stop the local Kafka Broker:
-
-``` python
-broker.stop()
-```
-
-    [INFO] fastkafka._testing.apache_kafka_broker: ApacheKafkaBroker.stop(): entering...
-    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Terminating the process 801303...
-    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Process 801303 was already terminated.
-    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Terminating the process 800930...
-    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Process 800930 was already terminated.
-    [INFO] fastkafka._testing.apache_kafka_broker: ApacheKafkaBroker.stop(): exited.
+    23-05-22 12:16:12.997 [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 7260...
+    23-05-22 12:16:12.998 [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 7262...
+    [7260]: 23-05-22 12:16:13.035 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
+    [7260]: 23-05-22 12:16:13.035 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
 
 ## Documentation
 
 The kafka app comes with builtin documentation generation using
 [AsyncApi HTML generator](https://www.asyncapi.com/tools/generator).
 
 AsyncApi requires Node.js to be installed and we provide the following
 convenience command line for it:
 
 ``` sh
 fastkafka docs install_deps
 ```
 
-    [INFO] fastkafka._components.docs_dependencies: AsyncAPI generator installed
+    23-05-22 12:17:03.425 [INFO] fastkafka._components.docs_dependencies: AsyncAPI generator installed
 
 To generate the documentation programatically you just need to call the
 folloving command:
 
 ``` sh
 fastkafka docs generate application:kafka_app
 ```
 
-    [INFO] fastkafka._components.asyncapi: New async specifications generated at: '/work/fastkafka/nbs/asyncapi/spec/asyncapi.yml'
-    [INFO] fastkafka._components.asyncapi: Async docs generated at 'asyncapi/docs'
-    [INFO] fastkafka._components.asyncapi: Output of '$ npx -y -p @asyncapi/generator ag asyncapi/spec/asyncapi.yml @asyncapi/html-template -o asyncapi/docs --force-write'
+    23-05-22 12:17:04.268 [INFO] fastkafka._components.asyncapi: New async specifications generated at: '/work/fastkafka/nbs/asyncapi/spec/asyncapi.yml'
+    23-05-22 12:17:13.777 [INFO] fastkafka._components.asyncapi: Async docs generated at 'asyncapi/docs'
+    23-05-22 12:17:13.777 [INFO] fastkafka._components.asyncapi: Output of '$ npx -y -p @asyncapi/generator ag asyncapi/spec/asyncapi.yml @asyncapi/html-template -o asyncapi/docs --force-write'
 
     Done! ✨
     Check out your shiny new generated files at /work/fastkafka/nbs/asyncapi/docs.
 
 . This will generate the *asyncapi* folder in relative path where all
 your documentation will be saved. You can check out the content of it
 with:
 
 ``` sh
 ls -l asyncapi
 ```
 
-    total 8
-    drwxrwxr-x 4 kumaran kumaran 4096 Mar 21 09:14 docs
-    drwxrwxr-x 2 kumaran kumaran 4096 Mar 21 09:14 spec
+    total 2
+    drwxrwxr-x 4 tvrtko tvrtko 5 Mar 29 09:57 docs
+    drwxrwxr-x 2 tvrtko tvrtko 3 Mar 29 09:56 spec
 
 In docs folder you will find the servable static html file of your
 documentation. This can also be served using our `fastkafka docs serve`
 CLI command (more on that in our guides).
 
 In spec folder you will find a asyncapi.yml file containing the async
 API specification of your application.
@@ -633,17 +476,17 @@
 We can locally preview the generated documentation by running the
 following command:
 
 ``` sh
 fastkafka docs serve application:kafka_app
 ```
 
-    [INFO] fastkafka._components.asyncapi: New async specifications generated at: '/work/fastkafka/nbs/asyncapi/spec/asyncapi.yml'
-    [INFO] fastkafka._components.asyncapi: Async docs generated at 'asyncapi/docs'
-    [INFO] fastkafka._components.asyncapi: Output of '$ npx -y -p @asyncapi/generator ag asyncapi/spec/asyncapi.yml @asyncapi/html-template -o asyncapi/docs --force-write'
+    23-05-22 12:17:14.784 [INFO] fastkafka._components.asyncapi: New async specifications generated at: '/work/fastkafka/nbs/asyncapi/spec/asyncapi.yml'
+    23-05-22 12:17:24.450 [INFO] fastkafka._components.asyncapi: Async docs generated at 'asyncapi/docs'
+    23-05-22 12:17:24.450 [INFO] fastkafka._components.asyncapi: Output of '$ npx -y -p @asyncapi/generator ag asyncapi/spec/asyncapi.yml @asyncapi/html-template -o asyncapi/docs --force-write'
 
     Done! ✨
     Check out your shiny new generated files at /work/fastkafka/nbs/asyncapi/docs.
 
 
     Serving documentation on http://127.0.0.1:8000
     ^C
```

### Comparing `fastkafka-0.7.0rc0/README.md` & `fastkafka-0.7.0rc1/fastkafka.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,38 @@
-FastKafka
-================
+Metadata-Version: 2.1
+Name: fastkafka
+Version: 0.7.0rc1
+Summary: FastKafka is a powerful and easy-to-use Python library for building asynchronous web services that interact with Kafka topics. Built on top of FastAPI, Starlette, Pydantic, AIOKafka and AsyncAPI, FastKafka simplifies the process of writing producers and consumers for Kafka topics.
+Home-page: https://github.com/airtai/fastkafka
+Author: airt
+Author-email: info@airt.ai
+License: Apache Software License 2.0
+Project-URL: Bug Tracker, https://github.com/airtai/fastkafka/issues
+Project-URL: CI, https://github.com/airtai/fastkafka/actions
+Project-URL: Documentation, https://fastkafka.airt.ai/
+Project-URL: Tutorial, https://colab.research.google.com/github/airtai/fastkafka/blob/main/nbs/guides/Guide_00_FastKafka_Demo.ipynb
+Keywords: nbdev jupyter notebook python kafka
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: avro
+Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: test
+License-File: LICENSE
+
+# FastKafka
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 <b>Effortless Kafka integration for your web services</b>
 
 ------------------------------------------------------------------------
 
@@ -79,126 +108,81 @@
 
 ``` sh
 pip install fastkafka[test,docs]
 ```
 
 ## Tutorial
 
-You can start an interactive tutorial in Google Colab by clicking the
-button below:
+You can start an interactive and extensive tutorial in Google Colab by
+clicking the button below:
 
 <a href="https://colab.research.google.com/github/airtai/fastkafka/blob/main/nbs/guides/Guide_00_FastKafka_Demo.ipynb" target=”_blank”>
 <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" />
 </a>
 
 ## Writing server code
 
-Here is an example python script using FastKafka that takes data from a
-Kafka topic, makes a prediction using a predictive model, and outputs
-the prediction to another Kafka topic.
-
-### Preparing the demo model
-
-First we will prepare our model using the Iris dataset so that we can
-demonstrate the predictions using FastKafka. The following call
-downloads the dataset and trains the model.
-
-We will wrap the model creation into a lifespan of our app so that the
-model is created just before the app is started.
+To demonstrate FastKafka simplicity of using `@produces` and `@consumes`
+decorators, we will focus on a simple app.
 
-``` python
-from contextlib import asynccontextmanager
-
-from sklearn.datasets import load_iris
-from sklearn.linear_model import LogisticRegression
-
-from fastkafka import FastKafka
-
-ml_models = {}
-
-
-@asynccontextmanager
-async def lifespan(app: FastKafka):
-    # Load the ML model
-    X, y = load_iris(return_X_y=True)
-    ml_models["iris_predictor"] = LogisticRegression(random_state=0, max_iter=500).fit(
-        X, y
-    )
-    yield
-    # Clean up the ML models and release the resources
-    ml_models.clear()
-```
+The app will consume jsons containig positive floats from one topic, log
+them and then produce incremented values to another topic.
 
 ### Messages
 
 FastKafka uses [Pydantic](https://docs.pydantic.dev/) to parse input
 JSON-encoded data into Python objects, making it easy to work with
 structured data in your Kafka-based applications. Pydantic’s
 [`BaseModel`](https://docs.pydantic.dev/usage/models/) class allows you
 to define messages using a declarative syntax, making it easy to specify
 the fields and types of your messages.
 
-This example defines two message classes for use in a FastKafka
-application:
+This example defines one `Data` mesage class. This Class will model the
+consumed and produced data in our app demo, it contains one
+`NonNegativeFloat` field `data` that will be logged and “processed”
+before being produced to another topic.
 
-- The `IrisInputData` class is used to represent input data for a
-  predictive model. It has four fields of type
-  [`NonNegativeFloat`](https://docs.pydantic.dev/usage/types/#constrained-types),
-  which is a subclass of float that only allows non-negative floating
-  point values.
-
-- The `IrisPrediction` class is used to represent the output of the
-  predictive model. It has a single field `species` of type string
-  representing the predicted species.
-
-These message classes will be used to parse and validate incoming data
-in Kafka consumers and producers.
+These message class will be used to parse and validate incoming data in
+Kafka consumers and producers.
 
 ``` python
 from pydantic import BaseModel, Field, NonNegativeFloat
 
 
-class IrisInputData(BaseModel):
-    sepal_length: NonNegativeFloat = Field(
-        ..., example=0.5, description="Sepal length in cm"
-    )
-    sepal_width: NonNegativeFloat = Field(
-        ..., example=0.5, description="Sepal width in cm"
+class Data(BaseModel):
+    data: NonNegativeFloat = Field(
+        ..., example=0.5, description="Float data example"
     )
-    petal_length: NonNegativeFloat = Field(
-        ..., example=0.5, description="Petal length in cm"
-    )
-    petal_width: NonNegativeFloat = Field(
-        ..., example=0.5, description="Petal width in cm"
-    )
-
-
-class IrisPrediction(BaseModel):
-    species: str = Field(..., example="setosa", description="Predicted species")
 ```
 
 ### Application
 
 This example shows how to initialize a FastKafka application.
 
 It starts by defining a dictionary called `kafka_brokers`, which
 contains two entries: `"localhost"` and `"production"`, specifying local
 development and production Kafka brokers. Each entry specifies the URL,
 port, and other details of a Kafka broker. This dictionary is used for
 both generating the documentation and later to run the actual server
 against one of the given kafka broker.
 
 Next, an object of the
-[`FastKafka`](https://fastkafka.airt.ai/docs/api/fastkafka)
+[`FastKafka`](https://fastkafka.airt.ai/docs/api/fastkafka#fastkafka.FastKafka)
 class is initialized with the minimum set of arguments:
 
 - `kafka_brokers`: a dictionary used for generation of documentation
 
+We will also import and create a logger so that we can log the incoming
+data in our consuming function.
+
 ``` python
 from fastkafka import FastKafka
+from fastkafka._components.logger import get_logger
+
+logger = get_logger(__name__)
 
 kafka_brokers = {
     "localhost": {
         "url": "localhost",
         "description": "local development kafka broker",
         "port": 9092,
     },
@@ -208,17 +192,16 @@
         "port": 9092,
         "protocol": "kafka-secure",
         "security": {"type": "plain"},
     },
 }
 
 kafka_app = FastKafka(
-    title="Iris predictions",
+    title="Demo Kafka app",
     kafka_brokers=kafka_brokers,
-    lifespan=lifespan,
 )
 ```
 
 ### Function decorators
 
 FastKafka provides convenient function decorators `@kafka_app.consumes`
 and `@kafka_app.produces` to allow you to delegate the actual process of
@@ -238,75 +221,66 @@
 This following example shows how to use the `@kafka_app.consumes` and
 `@kafka_app.produces` decorators in a FastKafka application:
 
 - The `@kafka_app.consumes` decorator is applied to the `on_input_data`
   function, which specifies that this function should be called whenever
   a message is received on the “input_data” Kafka topic. The
   `on_input_data` function takes a single argument which is expected to
-  be an instance of the `IrisInputData` message class. Specifying the
-  type of the single argument is instructing the Pydantic to use
-  `IrisInputData.parse_raw()` on the consumed message before passing it
-  to the user defined function `on_input_data`.
+  be an instance of the `Data` message class. Specifying the type of the
+  single argument is instructing the Pydantic to use `Data.parse_raw()`
+  on the consumed message before passing it to the user defined function
+  `on_input_data`.
 
-- The `@produces` decorator is applied to the `to_predictions` function,
+- The `@produces` decorator is applied to the `to_output_data` function,
   which specifies that this function should produce a message to the
-  “predictions” Kafka topic whenever it is called. The `to_predictions`
-  function takes a single integer argument `species_class` representing
-  one of three possible strign values predicted by the mdoel. It creates
-  a new `IrisPrediction` message using this value and then returns it.
-  The framework will call the `IrisPrediction.json().encode("utf-8")`
-  function on the returned value and produce it to the specified topic.
+  “output_data” Kafka topic whenever it is called. The `to_output_data`
+  function takes a single float argument `data`. It it increments the
+  data returns it wrapped in a `Data` object. The framework will call
+  the `Data.json().encode("utf-8")` function on the returned value and
+  produce it to the specified topic.
 
 ``` python
 @kafka_app.consumes(topic="input_data", auto_offset_reset="latest")
-async def on_input_data(msg: IrisInputData):
-    species_class = ml_models["iris_predictor"].predict(
-        [[msg.sepal_length, msg.sepal_width, msg.petal_length, msg.petal_width]]
-    )[0]
-
-    to_predictions(species_class)
-
+async def on_input_data(msg: Data):
+    logger.info(f"Got data: {msg.data}")
+    await to_output_data(msg.data)
 
-@kafka_app.produces(topic="predictions")
-def to_predictions(species_class: int) -> IrisPrediction:
-    iris_species = ["setosa", "versicolor", "virginica"]
 
-    prediction = IrisPrediction(species=iris_species[species_class])
-    return prediction
+@kafka_app.produces(topic="output_data")
+async def to_output_data(data: float) -> Data:
+    processed_data = Data(data=data+1.0)
+    return processed_data
 ```
 
 ## Testing the service
 
 The service can be tested using the
-[`Tester`](https://fastkafka.airt.ai/docs/api/fastkafka/testing/Tester)
+[`Tester`](https://fastkafka.airt.ai/docs/api/fastkafka/testing/Tester#fastkafka.testing.Tester)
 instances which internally starts InMemory implementation of Kafka
 broker.
 
 The Tester will redirect your consumes and produces decorated functions
 to the InMemory Kafka broker so that you can quickly test your app
 without the need for a running Kafka broker and all its dependencies.
 
 ``` python
 from fastkafka.testing import Tester
 
-msg = IrisInputData(
-    sepal_length=0.1,
-    sepal_width=0.2,
-    petal_length=0.3,
-    petal_width=0.4,
+msg = Data(
+    data=0.1,
 )
 
 # Start Tester app and create InMemory Kafka broker for testing
 async with Tester(kafka_app) as tester:
     # Send IrisInputData message to input_data topic
     await tester.to_input_data(msg)
 
     # Assert that the kafka_app responded with IrisPrediction in predictions topic
-    await tester.awaited_mocks.on_predictions.assert_awaited_with(
-        IrisPrediction(species="setosa"), timeout=2
+    await tester.awaited_mocks.on_output_data.assert_awaited_with(
+        Data(data=1.1), timeout=2
     )
 ```
 
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._start() called
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._patch_consumers_and_producers(): Patching consumers and producers!
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker starting
     [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
@@ -321,99 +295,66 @@
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer.subscribe(), subscribing to: ['input_data']
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'earliest', 'max_poll_records': 100}
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched start() called()
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched subscribe() called
-    [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer.subscribe(), subscribing to: ['predictions']
+    [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer.subscribe(), subscribing to: ['output_data']
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
-    [INFO] fastkafka._components.aiokafka_consumer_loop: _aiokafka_consumer_loop(): Consumer loop shutting down, waiting for send_stream to drain...
+    [INFO] __main__: Got data: 0.1
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched stop() called
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaProducer patched stop() called
-    [INFO] fastkafka._components.aiokafka_consumer_loop: _aiokafka_consumer_loop(): Consumer loop shutting down, waiting for send_stream to drain...
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaConsumer patched stop() called
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
     [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
     [INFO] fastkafka._testing.in_memory_broker: AIOKafkaProducer patched stop() called
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker._stop() called
     [INFO] fastkafka._testing.in_memory_broker: InMemoryBroker stopping
 
 ### Recap
 
-We have created a Iris classification model and encapulated it into our
-fastkafka application. The app will consume the IrisInputData from the
-`input_data` topic and produce the predictions to `predictions` topic.
+We have created a simple fastkafka application. The app will consume the
+`Data` from the `input_data` topic, log it and produce the incremented
+data to `output_data` topic.
 
 To test the app we have:
 
 1.  Created the app
 
 2.  Started our Tester class which mirrors the developed app topics for
     testing purposes
 
-3.  Sent IrisInputData message to `input_data` topic
+3.  Sent Data message to `input_data` topic
 
-4.  Asserted and checked that the developed iris classification service
-    has reacted to IrisInputData message
+4.  Asserted and checked that the developed service has reacted to Data
+    message
 
 ## Running the service
 
 The service can be started using builtin faskafka run CLI command.
 Before we can do that, we will concatenate the code snippets from above
 and save them in a file `"application.py"`
 
 ``` python
 # content of the "application.py" file
 
-from contextlib import asynccontextmanager
-
-from sklearn.datasets import load_iris
-from sklearn.linear_model import LogisticRegression
+from pydantic import BaseModel, Field, NonNegativeFloat
 
 from fastkafka import FastKafka
+from fastkafka._components.logger import get_logger
 
-ml_models = {}
+logger = get_logger(__name__)
 
-
-@asynccontextmanager
-async def lifespan(app: FastKafka):
-    # Load the ML model
-    X, y = load_iris(return_X_y=True)
-    ml_models["iris_predictor"] = LogisticRegression(random_state=0, max_iter=500).fit(
-        X, y
+class Data(BaseModel):
+    data: NonNegativeFloat = Field(
+        ..., example=0.5, description="Float data example"
     )
-    yield
-    # Clean up the ML models and release the resources
-    ml_models.clear()
-
-
-from pydantic import BaseModel, NonNegativeFloat, Field
-
-class IrisInputData(BaseModel):
-    sepal_length: NonNegativeFloat = Field(
-        ..., example=0.5, description="Sepal length in cm"
-    )
-    sepal_width: NonNegativeFloat = Field(
-        ..., example=0.5, description="Sepal width in cm"
-    )
-    petal_length: NonNegativeFloat = Field(
-        ..., example=0.5, description="Petal length in cm"
-    )
-    petal_width: NonNegativeFloat = Field(
-        ..., example=0.5, description="Petal width in cm"
-    )
-
-
-class IrisPrediction(BaseModel):
-    species: str = Field(..., example="setosa", description="Predicted species")
-    
-from fastkafka import FastKafka
 
 kafka_brokers = {
     "localhost": {
         "url": "localhost",
         "description": "local development kafka broker",
         "port": 9092,
     },
@@ -423,179 +364,111 @@
         "port": 9092,
         "protocol": "kafka-secure",
         "security": {"type": "plain"},
     },
 }
 
 kafka_app = FastKafka(
-    title="Iris predictions",
+    title="Demo Kafka app",
     kafka_brokers=kafka_brokers,
-    lifespan=lifespan,
 )
 
 @kafka_app.consumes(topic="input_data", auto_offset_reset="latest")
-async def on_input_data(msg: IrisInputData):
-    species_class = ml_models["iris_predictor"].predict(
-        [[msg.sepal_length, msg.sepal_width, msg.petal_length, msg.petal_width]]
-    )[0]
-
-    to_predictions(species_class)
-
-
-@kafka_app.produces(topic="predictions")
-def to_predictions(species_class: int) -> IrisPrediction:
-    iris_species = ["setosa", "versicolor", "virginica"]
-
-    prediction = IrisPrediction(species=iris_species[species_class])
-    return prediction
-```
-
-To run the service, you will need a running Kafka broker on localhost as
-specified in the `kafka_brokers` parameter above. We can start the Kafka
-broker locally using the
-[`ApacheKafkaBroker`](https://fastkafka.airt.ai/docs/api/fastkafka/testing/ApacheKafkaBroker).
-
-To use
-[`ApacheKafkaBroker`](https://fastkafka.airt.ai/docs/api/fastkafka/testing/ApacheKafkaBroker),
-you need to install JRE and Kafka to your environment. To simplify this
-process, fastkafka comes with a CLI command that does just that, to run
-it, in your terminal execute the following:
-
-``` sh
-fastkafka testing install_deps
-```
-
-Now we can run
-[`ApacheKafkaBroker`](https://fastkafka.airt.ai/docs/api/fastkafka/testing/ApacheKafkaBroker)
-that will start a Kafka broker instance for us.
-
-``` python
-from fastkafka.testing import ApacheKafkaBroker
-
-broker = ApacheKafkaBroker(apply_nest_asyncio=True)
-
-broker.start()
-```
-
-    [INFO] fastkafka._testing.apache_kafka_broker: ApacheKafkaBroker.start(): entering...
-    [WARNING] fastkafka._testing.apache_kafka_broker: ApacheKafkaBroker.start(): (<_UnixSelectorEventLoop running=True closed=False debug=False>) is already running!
-    [WARNING] fastkafka._testing.apache_kafka_broker: ApacheKafkaBroker.start(): calling nest_asyncio.apply()
-    [INFO] fastkafka._components.test_dependencies: Java is already installed.
-    [INFO] fastkafka._components.test_dependencies: But not exported to PATH, exporting...
-    [INFO] fastkafka._components.test_dependencies: Kafka is installed.
-    [INFO] fastkafka._components.test_dependencies: But not exported to PATH, exporting...
-    [INFO] fastkafka._testing.apache_kafka_broker: Starting zookeeper...
-    [INFO] fastkafka._testing.apache_kafka_broker: Starting kafka...
-    [INFO] fastkafka._testing.apache_kafka_broker: Local Kafka broker up and running on 127.0.0.1:9092
-    [INFO] fastkafka._testing.apache_kafka_broker: <class 'fastkafka.testing.ApacheKafkaBroker'>.start(): returning 127.0.0.1:9092
-    [INFO] fastkafka._testing.apache_kafka_broker: ApacheKafkaBroker.start(): exited.
-
-    '127.0.0.1:9092'
-
-Then, we start the FastKafka service by running the following command in
-the folder where the `application.py` file is located:
-
-``` sh
-fastkafka run --num-workers=2 --kafka-broker localhost application:kafka_app
-```
-
-In the above command, we use `--num-workers` option to specify how many
-workers to launch and we use `--kafka-broker` option to specify which
-kafka broker configuration to use from earlier specified `kafka_brokers`
-
-    [801767]: [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
-    [801765]: [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
-    [801767]: [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
-    [801765]: [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
-    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
-    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
-    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
-    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
-    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
-    [801767]: [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
-    [801767]: [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
-    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
-    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
-    [801765]: [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
-    [801765]: [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
-    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
-    [801765]: [ERROR] aiokafka.cluster: Topic input_data not found in cluster metadata
-    [801765]: [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
-    [801767]: [WARNING] aiokafka.cluster: Topic input_data is not available during auto-create initialization
-    [801767]: [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
-    [801767]: [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('192.168.112.2', 9092)
-    [801765]: [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('192.168.112.2', 9092)
-    [801767]: [ERROR] aiokafka: Unable to update metadata from [0]
-    [801765]: [ERROR] aiokafka: Unable to update metadata from [0]
+async def on_input_data(msg: Data):
+    logger.info(f"Got data: {msg.data}")
+    await to_output_data(msg.data)
+
+
+@kafka_app.produces(topic="output_data")
+async def to_output_data(data: float) -> Data:
+    processed_data = Data(data=data+1.0)
+    return processed_data
+```
+
+To run the service, use the FastKafka CLI command and pass the module
+(in this case, the file where the app implementation is located) and the
+app simbol to the command.
+
+`shell fastkafka run --num-workers=1 --kafka-broker localhost application:kafka_app`
+
+After running the command, you should see the following output in your
+command line:
+
+    [7262]: 23-05-22 12:16:07.361 [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
+    [7260]: 23-05-22 12:16:07.361 [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
+    [7260]: 23-05-22 12:16:07.361 [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
+    [7262]: 23-05-22 12:16:07.361 [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
+    [7260]: 23-05-22 12:16:07.388 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
+    [7260]: 23-05-22 12:16:07.388 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
+    [7262]: 23-05-22 12:16:07.389 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
+    [7262]: 23-05-22 12:16:07.389 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer created using the following parameters: {'bootstrap_servers': 'localhost:9092', 'auto_offset_reset': 'latest', 'max_poll_records': 100}
+    [7260]: 23-05-22 12:16:07.396 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
+    [7260]: 23-05-22 12:16:07.396 [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
+    [7260]: 23-05-22 12:16:07.396 [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
+    [7260]: 23-05-22 12:16:07.396 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
+    [7262]: 23-05-22 12:16:07.400 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer started.
+    [7262]: 23-05-22 12:16:07.400 [INFO] aiokafka.consumer.subscription_state: Updating subscribed topics to: frozenset({'input_data'})
+    [7262]: 23-05-22 12:16:07.401 [INFO] aiokafka.consumer.consumer: Subscribed to topic(s): {'input_data'}
+    [7262]: 23-05-22 12:16:07.401 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer subscribed.
+    [7262]: 23-05-22 12:16:07.412 [ERROR] aiokafka.cluster: Topic input_data not found in cluster metadata
+    [7262]: 23-05-22 12:16:07.412 [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
+    [7260]: 23-05-22 12:16:07.482 [WARNING] aiokafka.cluster: Topic input_data is not available during auto-create initialization
+    [7260]: 23-05-22 12:16:07.482 [INFO] aiokafka.consumer.group_coordinator: Metadata for topic has changed from {} to {'input_data': 0}. 
+    [7262]: 23-05-22 12:16:12.865 [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('172.18.0.2', 9092)
+    [7262]: 23-05-22 12:16:12.865 [ERROR] aiokafka: Unable to update metadata from [0]
+    [7260]: 23-05-22 12:16:12.866 [ERROR] aiokafka: Unable connect to node with id 0: [Errno 111] Connect call failed ('172.18.0.2', 9092)
+    [7260]: 23-05-22 12:16:12.866 [ERROR] aiokafka: Unable to update metadata from [0]
     ^C
+    [7262]: 23-05-22 12:16:12.978 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
+    [7262]: 23-05-22 12:16:12.979 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
     Starting process cleanup, this may take a few seconds...
-    [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 801765...
-    [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 801767...
-    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: _aiokafka_consumer_loop(): Consumer loop shutting down, waiting for send_stream to drain...
-    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
-    [801765]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
-    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: _aiokafka_consumer_loop(): Consumer loop shutting down, waiting for send_stream to drain...
-    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
-    [801767]: [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
-
-You need to interupt running of the cell above by selecting
-`Runtime->Interupt execution` on the toolbar above.
-
-Finally, we can stop the local Kafka Broker:
-
-``` python
-broker.stop()
-```
-
-    [INFO] fastkafka._testing.apache_kafka_broker: ApacheKafkaBroker.stop(): entering...
-    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Terminating the process 801303...
-    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Process 801303 was already terminated.
-    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Terminating the process 800930...
-    [INFO] fastkafka._components._subprocess: terminate_asyncio_process(): Process 800930 was already terminated.
-    [INFO] fastkafka._testing.apache_kafka_broker: ApacheKafkaBroker.stop(): exited.
+    23-05-22 12:16:12.997 [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 7260...
+    23-05-22 12:16:12.998 [INFO] fastkafka._server: terminate_asyncio_process(): Terminating the process 7262...
+    [7260]: 23-05-22 12:16:13.035 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop(): Consumer stopped.
+    [7260]: 23-05-22 12:16:13.035 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() finished.
 
 ## Documentation
 
 The kafka app comes with builtin documentation generation using
 [AsyncApi HTML generator](https://www.asyncapi.com/tools/generator).
 
 AsyncApi requires Node.js to be installed and we provide the following
 convenience command line for it:
 
 ``` sh
 fastkafka docs install_deps
 ```
 
-    [INFO] fastkafka._components.docs_dependencies: AsyncAPI generator installed
+    23-05-22 12:17:03.425 [INFO] fastkafka._components.docs_dependencies: AsyncAPI generator installed
 
 To generate the documentation programatically you just need to call the
 folloving command:
 
 ``` sh
 fastkafka docs generate application:kafka_app
 ```
 
-    [INFO] fastkafka._components.asyncapi: New async specifications generated at: '/work/fastkafka/nbs/asyncapi/spec/asyncapi.yml'
-    [INFO] fastkafka._components.asyncapi: Async docs generated at 'asyncapi/docs'
-    [INFO] fastkafka._components.asyncapi: Output of '$ npx -y -p @asyncapi/generator ag asyncapi/spec/asyncapi.yml @asyncapi/html-template -o asyncapi/docs --force-write'
+    23-05-22 12:17:04.268 [INFO] fastkafka._components.asyncapi: New async specifications generated at: '/work/fastkafka/nbs/asyncapi/spec/asyncapi.yml'
+    23-05-22 12:17:13.777 [INFO] fastkafka._components.asyncapi: Async docs generated at 'asyncapi/docs'
+    23-05-22 12:17:13.777 [INFO] fastkafka._components.asyncapi: Output of '$ npx -y -p @asyncapi/generator ag asyncapi/spec/asyncapi.yml @asyncapi/html-template -o asyncapi/docs --force-write'
 
     Done! ✨
     Check out your shiny new generated files at /work/fastkafka/nbs/asyncapi/docs.
 
 . This will generate the *asyncapi* folder in relative path where all
 your documentation will be saved. You can check out the content of it
 with:
 
 ``` sh
 ls -l asyncapi
 ```
 
-    total 8
-    drwxrwxr-x 4 kumaran kumaran 4096 Mar 21 09:14 docs
-    drwxrwxr-x 2 kumaran kumaran 4096 Mar 21 09:14 spec
+    total 2
+    drwxrwxr-x 4 tvrtko tvrtko 5 Mar 29 09:57 docs
+    drwxrwxr-x 2 tvrtko tvrtko 3 Mar 29 09:56 spec
 
 In docs folder you will find the servable static html file of your
 documentation. This can also be served using our `fastkafka docs serve`
 CLI command (more on that in our guides).
 
 In spec folder you will find a asyncapi.yml file containing the async
 API specification of your application.
@@ -603,17 +476,17 @@
 We can locally preview the generated documentation by running the
 following command:
 
 ``` sh
 fastkafka docs serve application:kafka_app
 ```
 
-    [INFO] fastkafka._components.asyncapi: New async specifications generated at: '/work/fastkafka/nbs/asyncapi/spec/asyncapi.yml'
-    [INFO] fastkafka._components.asyncapi: Async docs generated at 'asyncapi/docs'
-    [INFO] fastkafka._components.asyncapi: Output of '$ npx -y -p @asyncapi/generator ag asyncapi/spec/asyncapi.yml @asyncapi/html-template -o asyncapi/docs --force-write'
+    23-05-22 12:17:14.784 [INFO] fastkafka._components.asyncapi: New async specifications generated at: '/work/fastkafka/nbs/asyncapi/spec/asyncapi.yml'
+    23-05-22 12:17:24.450 [INFO] fastkafka._components.asyncapi: Async docs generated at 'asyncapi/docs'
+    23-05-22 12:17:24.450 [INFO] fastkafka._components.asyncapi: Output of '$ npx -y -p @asyncapi/generator ag asyncapi/spec/asyncapi.yml @asyncapi/html-template -o asyncapi/docs --force-write'
 
     Done! ✨
     Check out your shiny new generated files at /work/fastkafka/nbs/asyncapi/docs.
 
 
     Serving documentation on http://127.0.0.1:8000
     ^C
@@ -670,7 +543,9 @@
 A permissive license whose main conditions require preservation of
 copyright and license notices. Contributors provide an express grant of
 patent rights. Licensed works, modifications, and larger works may be
 distributed under different terms and without source code.
 
 The full text of the license can be found
 [here](https://raw.githubusercontent.com/airtai/fastkafka/main/LICENSE).
+
+
```

### Comparing `fastkafka-0.7.0rc0/fastkafka/__init__.py` & `fastkafka-0.7.0rc1/fastkafka/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.0rc0"
+__version__ = "0.7.0rc1"
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/010_Application_export.ipynb.
 
 # %% auto 0
 __all__ = ['dummy']
 
 # %% ../nbs/010_Application_export.ipynb 1
 from ._application.app import FastKafka
```

### Comparing `fastkafka-0.7.0rc0/fastkafka/_application/app.py` & `fastkafka-0.7.0rc1/fastkafka/_application/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,81 +37,107 @@
     export_async_spec,
 )
 from .._components.benchmarking import _benchmark
 from .._components.logger import get_logger
 from .._components.meta import delegates, export, filter_using_signature, patch
 from .._components.producer_decorator import ProduceCallable, producer_decorator
 from .._components.task_streaming import StreamExecutor
+from .._components.helpers import remove_suffix
 
 # %% ../../nbs/015_FastKafka.ipynb 2
 if TYPE_CHECKING:
     from fastapi import FastAPI
 
 # %% ../../nbs/015_FastKafka.ipynb 4
 logger = get_logger(__name__)
 
 # %% ../../nbs/015_FastKafka.ipynb 9
-@delegates(AIOKafkaConsumer, but=["bootstrap_servers"])
-@delegates(AIOKafkaProducer, but=["bootstrap_servers"], keep=True)
+@delegates(AIOKafkaConsumer, but=["bootstrap_servers_id"])
+@delegates(AIOKafkaProducer, but=["bootstrap_servers_id"], keep=True)
 def _get_kafka_config(
     **kwargs: Any,
 ) -> Dict[str, Any]:
     """Get kafka config"""
     allowed_keys = set(signature(_get_kafka_config).parameters.keys())
     if not set(kwargs.keys()) <= allowed_keys:
         unallowed_keys = ", ".join(
             sorted([f"'{x}'" for x in set(kwargs.keys()).difference(allowed_keys)])
         )
         raise ValueError(f"Unallowed key arguments passed: {unallowed_keys}")
     retval = kwargs.copy()
 
     # todo: check this values
     config_defaults = {
-        "bootstrap_servers": "localhost:9092",
+        "bootstrap_servers_id": "localhost",
         "auto_offset_reset": "earliest",
         "max_poll_records": 100,
-        #         "max_buffer_size": 10_000,
     }
     for key, value in config_defaults.items():
         if key not in retval:
             retval[key] = value
 
     return retval
 
 # %% ../../nbs/015_FastKafka.ipynb 12
-def _get_kafka_brokers(kafka_brokers: Optional[Dict[str, Any]] = None) -> KafkaBrokers:
+def _get_kafka_brokers(
+    kafka_brokers: Optional[Union[Dict[str, Any], KafkaBrokers]] = None
+) -> KafkaBrokers:
     """Get Kafka brokers
 
     Args:
         kafka_brokers: Kafka brokers
 
     """
     if kafka_brokers is None:
         retval: KafkaBrokers = KafkaBrokers(
             brokers={
                 "localhost": KafkaBroker(  # type: ignore
                     url="https://localhost",
                     description="Local (dev) Kafka broker",
                     port="9092",
+                    grouping="localhost",
                 )
             }
         )
     else:
+        if isinstance(kafka_brokers, KafkaBrokers):
+            return kafka_brokers
+
         retval = KafkaBrokers(
             brokers={
-                k: KafkaBroker.parse_raw(
-                    v.json() if hasattr(v, "json") else json.dumps(v)
+                k: (
+                    [
+                        KafkaBroker.parse_raw(
+                            unwrapped_v.json()
+                            if hasattr(unwrapped_v, "json")
+                            else json.dumps(unwrapped_v)
+                        )
+                        for unwrapped_v in v
+                    ]
+                    if isinstance(v, list)
+                    else KafkaBroker.parse_raw(
+                        v.json() if hasattr(v, "json") else json.dumps(v)
+                    )
                 )
                 for k, v in kafka_brokers.items()
             }
         )
 
     return retval
 
 # %% ../../nbs/015_FastKafka.ipynb 14
+def _get_broker_addr_list(
+    brokers: Union[List[KafkaBroker], KafkaBroker]
+) -> Union[str, List[str]]:
+    if isinstance(brokers, list):
+        return [f"{broker.url}:{broker.port}" for broker in brokers]
+    else:
+        return f"{brokers.url}:{brokers.port}"
+
+# %% ../../nbs/015_FastKafka.ipynb 16
 def _get_topic_name(
     topic_callable: Union[ConsumeCallable, ProduceCallable], prefix: str = "on_"
 ) -> str:
     """Get topic name
     Args:
         topic_callable: a function
         prefix: prefix of the name of the function followed by the topic name
@@ -122,29 +148,29 @@
     topic = topic_callable.__name__
     if not topic.startswith(prefix) or len(topic) <= len(prefix):
         raise ValueError(f"Function name '{topic}' must start with {prefix}")
     topic = topic[len(prefix) :]
 
     return topic
 
-# %% ../../nbs/015_FastKafka.ipynb 16
+# %% ../../nbs/015_FastKafka.ipynb 18
 def _get_contact_info(
     name: str = "Author",
     url: str = "https://www.google.com",
     email: str = "noreply@gmail.com",
 ) -> ContactInfo:
     return ContactInfo(name=name, url=url, email=email)  # type: ignore
 
-# %% ../../nbs/015_FastKafka.ipynb 18
+# %% ../../nbs/015_FastKafka.ipynb 20
 I = TypeVar("I", bound=BaseModel)
 O = TypeVar("O", BaseModel, Awaitable[BaseModel])
 
 F = TypeVar("F", bound=Callable)
 
-# %% ../../nbs/015_FastKafka.ipynb 19
+# %% ../../nbs/015_FastKafka.ipynb 21
 @export("fastkafka")
 class FastKafka:
     @delegates(_get_kafka_config)
     def __init__(
         self,
         *,
         title: Optional[str] = None,
@@ -209,14 +235,16 @@
                     "description": "local kafka broker",
                     "port": "9092",
                 }
             }
 
         self._kafka_brokers = _get_kafka_brokers(kafka_brokers)
 
+        self._override_brokers: List[KafkaBrokers] = []
+
         self._root_path = Path(".") if root_path is None else Path(root_path)
 
         self._asyncapi_path = self._root_path / "asyncapi"
         (self._asyncapi_path / "docs").mkdir(exist_ok=True, parents=True)
         (self._asyncapi_path / "spec").mkdir(exist_ok=True, parents=True)
 
         # this is used as default parameters for creating AIOProducer and AIOConsumer objects
@@ -225,20 +253,27 @@
         #
         self._consumers_store: Dict[
             str,
             Tuple[
                 ConsumeCallable,
                 Callable[[bytes, ModelMetaclass], Any],
                 Union[str, StreamExecutor, None],
+                Optional[KafkaBrokers],
                 Dict[str, Any],
             ],
         ] = {}
 
         self._producers_store: Dict[  # type: ignore
-            str, Tuple[ProduceCallable, AIOKafkaProducer, Dict[str, Any]]
+            str,
+            Tuple[
+                ProduceCallable,
+                AIOKafkaProducer,
+                Optional[KafkaBrokers],
+                Dict[str, Any],
+            ],
         ] = {}
 
         self._producers_list: List[AIOKafkaProducer] = []  # type: ignore
 
         self.benchmark_results: Dict[str, Dict[str, Any]] = {}
 
         # background tasks
@@ -264,17 +299,14 @@
         self.mocks = None
         self.awaited_mocks = None
 
     @property
     def is_started(self) -> bool:
         return self._is_started
 
-    def _set_bootstrap_servers(self, bootstrap_servers: str) -> None:
-        self._kafka_config["bootstrap_servers"] = bootstrap_servers
-
     def set_kafka_broker(self, kafka_broker_name: str) -> None:
         """
         Sets the Kafka broker to start FastKafka with
 
         Args:
             kafka_broker_name: The name of the Kafka broker to start FastKafka
 
@@ -286,20 +318,15 @@
         """
 
         if kafka_broker_name not in self._kafka_brokers.brokers:
             raise ValueError(
                 f"Given kafka_broker_name '{kafka_broker_name}' is not found in kafka_brokers, available options are {self._kafka_brokers.brokers.keys()}"
             )
 
-        broker_to_use = self._kafka_brokers.brokers[kafka_broker_name]
-        bootstrap_servers = f"{broker_to_use.url}:{broker_to_use.port}"
-        logger.info(
-            f"set_kafka_broker() : Setting bootstrap_servers value to '{bootstrap_servers}'"
-        )
-        self._set_bootstrap_servers(bootstrap_servers=bootstrap_servers)
+        self._kafka_config["bootstrap_servers_id"] = kafka_broker_name
 
     async def __aenter__(self) -> "FastKafka":
         if self.lifespan is not None:
             self.lifespan_ctx = self.lifespan(self)
             await self.lifespan_ctx.__aenter__()
         await self._start()
         return self
@@ -322,25 +349,28 @@
 
     def consumes(
         self,
         topic: Optional[str] = None,
         decoder: str = "json",
         *,
         prefix: str = "on_",
+        brokers: Optional[KafkaBrokers] = None,
+        description: Optional[str] = None,
         **kwargs: Dict[str, Any],
     ) -> ConsumeCallable:
         raise NotImplementedError
 
-    def produces(  # type: ignore
+    def produces(
         self,
         topic: Optional[str] = None,
         encoder: str = "json",
         *,
         prefix: str = "to_",
-        producer: Optional[AIOKafkaProducer] = None,
+        brokers: Optional[KafkaBrokers] = None,
+        description: Optional[str] = None,
         **kwargs: Dict[str, Any],
     ) -> ProduceCallable:
         raise NotImplementedError
 
     def benchmark(
         self,
         interval: Union[int, timedelta] = 1,
@@ -380,15 +410,15 @@
 
     async def _shutdown_producers(self) -> None:
         raise NotImplementedError
 
     async def _shutdown_bg_tasks(self) -> None:
         raise NotImplementedError
 
-# %% ../../nbs/015_FastKafka.ipynb 26
+# %% ../../nbs/015_FastKafka.ipynb 27
 def _get_decoder_fn(decoder: str) -> Callable[[bytes, ModelMetaclass], Any]:
     """
     Imports and returns decoder function based on input
     """
     if decoder == "json":
         from fastkafka._components.encoder.json import json_decoder
 
@@ -400,24 +430,48 @@
             raise ModuleNotFoundError(
                 "Unable to import avro packages. Please install FastKafka using the command 'fastkafka[avro]'"
             )
         return avro_decoder
     else:
         raise ValueError(f"Unknown decoder - {decoder}")
 
-# %% ../../nbs/015_FastKafka.ipynb 28
+# %% ../../nbs/015_FastKafka.ipynb 29
+def _prepare_and_check_brokers(
+    app: FastKafka, kafka_brokers: Optional[Union[Dict[str, Any], KafkaBrokers]]
+) -> Optional[KafkaBrokers]:
+    if kafka_brokers is not None:
+        prepared_brokers = _get_kafka_brokers(kafka_brokers)
+        if prepared_brokers.brokers.keys() != app._kafka_brokers.brokers.keys():
+            raise ValueError(
+                f"To override application default brokers, you must define all of the broker options. Default defined: {set(app._kafka_brokers.brokers.keys())}, override defined: {set(prepared_brokers.brokers.keys())}"
+            )
+        return prepared_brokers
+    return None
+
+# %% ../../nbs/015_FastKafka.ipynb 30
+def _resolve_key(key: str, dictionary: Dict[str, Any]) -> str:
+    i = 0
+    resolved_key = f"{key}_{i}"
+    while resolved_key in dictionary:
+        i += 1
+        resolved_key = f"{key}_{i}"
+    return resolved_key
+
+# %% ../../nbs/015_FastKafka.ipynb 31
 @patch
 @delegates(AIOKafkaConsumer)
 def consumes(
     self: FastKafka,
     topic: Optional[str] = None,
     decoder: Union[str, Callable[[bytes, ModelMetaclass], Any]] = "json",
     *,
     executor: Union[str, StreamExecutor, None] = None,
+    brokers: Optional[Union[Dict[str, Any], KafkaBrokers]] = None,
     prefix: str = "on_",
+    description: Optional[str] = None,
     **kwargs: Dict[str, Any],
 ) -> Callable[[ConsumeCallable], ConsumeCallable]:
     """Decorator registering the callback called when a message is received in a topic.
 
     This function decorator is also responsible for registering topics for AsyncAPI specificiation and documentation.
 
     Args:
@@ -434,47 +488,67 @@
                 "SequentialExecutor" which will execute the consuming tasks sequentially.
                 If the consuming tasks have high latency it is recommended to use
                 "DynamicTaskExecutor" which will wrap the consuming functions into tasks
                 and run them in on asyncio loop in background. This comes with a cost of
                 increased overhead so use it only in cases when your consume functions have
                 high latency such as database queries or some other type of networking.
         prefix: Prefix stripped from the decorated function to define a topic name
-            if the topic argument is not passed, default: "on_". If the decorated
-            function name is not prefixed with the defined prefix and topic argument
-            is not passed, then this method will throw ValueError
+                if the topic argument is not passed, default: "on_". If the decorated
+                function name is not prefixed with the defined prefix and topic argument
+                is not passed, then this method will throw ValueError
+        brokers: Optional argument specifying multiple broker clusters for consuming
+                messages from different Kafka clusters in FastKafka.
+        description: Optional description of the consuming function async docs.
+                If not provided, consuming function __doc__ attr will be used.
 
     Returns:
         A function returning the same function
 
     Throws:
         ValueError
 
     """
 
     def _decorator(
         on_topic: ConsumeCallable,
         topic: Optional[str] = topic,
         decoder: Union[str, Callable[[bytes, ModelMetaclass], Any]] = decoder,
         executor: Union[str, StreamExecutor, None] = executor,
+        brokers: Optional[Union[Dict[str, Any], KafkaBrokers]] = brokers,
+        description: Optional[str] = description,
         kwargs: Dict[str, Any] = kwargs,
     ) -> ConsumeCallable:
         topic_resolved: str = (
             _get_topic_name(topic_callable=on_topic, prefix=prefix)
             if topic is None
             else topic
         )
 
         decoder_fn = _get_decoder_fn(decoder) if isinstance(decoder, str) else decoder
-        self._consumers_store[topic_resolved] = (on_topic, decoder_fn, executor, kwargs)
+
+        prepared_broker = _prepare_and_check_brokers(self, brokers)
+        if prepared_broker is not None:
+            self._override_brokers.append(prepared_broker.brokers)  # type: ignore
+
+        if description is not None:
+            setattr(on_topic, "description", description)
+
+        self._consumers_store[_resolve_key(topic_resolved, self._consumers_store)] = (
+            on_topic,
+            decoder_fn,
+            executor,
+            prepared_broker,
+            kwargs,
+        )
         setattr(self, on_topic.__name__, on_topic)
         return on_topic
 
     return _decorator
 
-# %% ../../nbs/015_FastKafka.ipynb 30
+# %% ../../nbs/015_FastKafka.ipynb 34
 def _get_encoder_fn(encoder: str) -> Callable[[BaseModel], bytes]:
     """
     Imports and returns encoder function based on input
     """
     if encoder == "json":
         from fastkafka._components.encoder.json import json_encoder
 
@@ -486,23 +560,25 @@
             raise ModuleNotFoundError(
                 "Unable to import avro packages. Please install FastKafka using the command 'fastkafka[avro]'"
             )
         return avro_encoder
     else:
         raise ValueError(f"Unknown encoder - {encoder}")
 
-# %% ../../nbs/015_FastKafka.ipynb 32
+# %% ../../nbs/015_FastKafka.ipynb 36
 @patch
 @delegates(AIOKafkaProducer)
 def produces(
     self: FastKafka,
     topic: Optional[str] = None,
     encoder: Union[str, Callable[[BaseModel], bytes]] = "json",
     *,
     prefix: str = "to_",
+    brokers: Optional[Union[Dict[str, Any], KafkaBrokers]] = None,
+    description: Optional[str] = None,
     **kwargs: Dict[str, Any],
 ) -> Callable[[ProduceCallable], ProduceCallable]:
     """Decorator registering the callback called when delivery report for a produced message is received
 
     This function decorator is also responsible for registering topics for AsyncAPI specificiation and documentation.
 
     Args:
@@ -514,51 +590,80 @@
                 default: json - By default, it uses json encoder to convert
                 pydantic basemodel to json string and then encodes the string to bytes
                 using 'utf-8' encoding. It also accepts custom encoder function.
         prefix: Prefix stripped from the decorated function to define a topic
             name if the topic argument is not passed, default: "to_". If the
             decorated function name is not prefixed with the defined prefix
             and topic argument is not passed, then this method will throw ValueError
+        brokers: Optional argument specifying multiple broker clusters for consuming
+            messages from different Kafka clusters in FastKafka.
+        description: Optional description of the producing function async docs.
+                If not provided, producing function __doc__ attr will be used.
 
     Returns:
         A function returning the same function
 
     Raises:
         ValueError: when needed
     """
 
     def _decorator(
         to_topic: ProduceCallable,
         topic: Optional[str] = topic,
+        brokers: Optional[Union[Dict[str, Any], KafkaBrokers]] = brokers,
+        description: Optional[str] = description,
         kwargs: Dict[str, Any] = kwargs,
     ) -> ProduceCallable:
         topic_resolved: str = (
             _get_topic_name(topic_callable=to_topic, prefix=prefix)
             if topic is None
             else topic
         )
 
-        self._producers_store[topic_resolved] = (to_topic, None, kwargs)
+        topic_key = _resolve_key(topic_resolved, self._producers_store)
+
+        prepared_broker = _prepare_and_check_brokers(self, brokers)
+        if prepared_broker is not None:
+            self._override_brokers.append(prepared_broker.brokers)  # type: ignore
+
+        if description is not None:
+            setattr(to_topic, "description", description)
+
+        self._producers_store[topic_key] = (
+            to_topic,
+            None,
+            prepared_broker,
+            kwargs,
+        )
         encoder_fn = _get_encoder_fn(encoder) if isinstance(encoder, str) else encoder
         decorated = producer_decorator(
-            self._producers_store, to_topic, topic_resolved, encoder_fn=encoder_fn
+            self._producers_store,
+            to_topic,
+            topic_key,
+            encoder_fn=encoder_fn,
         )
         setattr(self, to_topic.__name__, decorated)
         return decorated
 
     return _decorator
 
-# %% ../../nbs/015_FastKafka.ipynb 34
+# %% ../../nbs/015_FastKafka.ipynb 39
 @patch
 def get_topics(self: FastKafka) -> Iterable[str]:
-    produce_topics = set(self._producers_store.keys())
-    consume_topics = set(self._consumers_store.keys())
+    """
+    Get all topics for both producing and consuming.
+
+    Returns:
+        A set of topics for both producing and consuming.
+    """
+    produce_topics = set([remove_suffix(topic) for topic in self._producers_store])
+    consume_topics = set([remove_suffix(topic) for topic in self._consumers_store])
     return consume_topics.union(produce_topics)
 
-# %% ../../nbs/015_FastKafka.ipynb 36
+# %% ../../nbs/015_FastKafka.ipynb 41
 @patch
 def run_in_background(
     self: FastKafka,
 ) -> Callable[
     [Callable[..., Coroutine[Any, Any, Any]]], Callable[..., Coroutine[Any, Any, Any]]
 ]:
     """
@@ -587,77 +692,95 @@
         )
         self._scheduled_bg_tasks.append(bg_task)
 
         return bg_task
 
     return _decorator
 
-# %% ../../nbs/015_FastKafka.ipynb 40
+# %% ../../nbs/015_FastKafka.ipynb 45
 @patch
 def _populate_consumers(
     self: FastKafka,
     is_shutting_down_f: Callable[[], bool],
 ) -> None:
     default_config: Dict[str, Any] = filter_using_signature(
         AIOKafkaConsumer, **self._kafka_config
     )
+
+    bootstrap_server = self._kafka_config["bootstrap_servers_id"]
+
     self._kafka_consumer_tasks = [
         asyncio.create_task(
             aiokafka_consumer_loop(
-                topic=topic,
+                topic="_".join(topic.split("_")[:-1]),
                 decoder_fn=decoder_fn,
                 callback=consumer,
                 msg_type=signature(consumer).parameters["msg"].annotation,
                 is_shutting_down_f=is_shutting_down_f,
                 executor=executor,
-                **{**default_config, **override_config},
+                **{
+                    **default_config,
+                    **override_config,
+                    **{
+                        "bootstrap_servers": _get_broker_addr_list(
+                            kafka_brokers.brokers[bootstrap_server]
+                            if kafka_brokers is not None
+                            else self._kafka_brokers.brokers[bootstrap_server]
+                        )
+                    },
+                },
             )
         )
         for topic, (
             consumer,
             decoder_fn,
             executor,
+            kafka_brokers,
             override_config,
         ) in self._consumers_store.items()
     ]
 
 
 @patch
 async def _shutdown_consumers(
     self: FastKafka,
 ) -> None:
     if self._kafka_consumer_tasks:
         await asyncio.wait(self._kafka_consumer_tasks)
 
-# %% ../../nbs/015_FastKafka.ipynb 42
+# %% ../../nbs/015_FastKafka.ipynb 47
 # TODO: Add passing of vars
 async def _create_producer(  # type: ignore
     *,
     callback: ProduceCallable,
     default_config: Dict[str, Any],
     override_config: Dict[str, Any],
+    bootstrap_servers: Union[str, List[str]],
     producers_list: List[AIOKafkaProducer],
 ) -> AIOKafkaProducer:
     """Creates a producer
 
     Args:
         callback: A callback function that is called when the producer is ready.
         producer: An existing producer to use.
         default_config: A dictionary of default configuration values.
         override_config: A dictionary of configuration values to override.
+        bootstrap_servers: Bootstrap servers to connect the producer to.
         producers_list: A list of producers to add the new producer to.
 
     Returns:
         A producer.
     """
 
     config = {
         **filter_using_signature(AIOKafkaProducer, **default_config),
         **filter_using_signature(AIOKafkaProducer, **override_config),
+        **{"bootstrap_servers": bootstrap_servers},
     }
+
     producer = AIOKafkaProducer(**config)
     logger.info(
         f"_create_producer() : created producer using the config: '{sanitize_kafka_config(**config)}'"
     )
 
     await producer.start()
 
@@ -676,30 +799,39 @@
     Returns:
         None.
 
     Raises:
         None.
     """
     default_config: Dict[str, Any] = self._kafka_config
+    bootstrap_server = default_config["bootstrap_servers_id"]
+
     self._producers_list = []
     self._producers_store.update(
         {
             topic: (
                 callback,
                 await _create_producer(
                     callback=callback,
                     default_config=default_config,
                     override_config=override_config,
+                    bootstrap_servers=_get_broker_addr_list(
+                        kafka_brokers.brokers[bootstrap_server]
+                        if kafka_brokers is not None
+                        else self._kafka_brokers.brokers[bootstrap_server]
+                    ),
                     producers_list=self._producers_list,
                 ),
+                kafka_brokers,
                 override_config,
             )
             for topic, (
                 callback,
                 _,
+                kafka_brokers,
                 override_config,
             ) in self._producers_store.items()
         }
     )
 
 
 @patch
@@ -708,25 +840,27 @@
     # Remove references to stale producers
     self._producers_list = []
     self._producers_store.update(
         {
             topic: (
                 callback,
                 None,
+                kafka_brokers,
                 override_config,
             )
             for topic, (
                 callback,
                 _,
+                kafka_brokers,
                 override_config,
             ) in self._producers_store.items()
         }
     )
 
-# %% ../../nbs/015_FastKafka.ipynb 44
+# %% ../../nbs/015_FastKafka.ipynb 49
 @patch
 async def _populate_bg_tasks(
     self: FastKafka,
 ) -> None:
     def _start_bg_task(task: Callable[..., Coroutine[Any, Any, Any]]) -> asyncio.Task:
         logger.info(
             f"_populate_bg_tasks() : Starting background task '{task.__name__}'"
@@ -754,15 +888,15 @@
             await task
         except asyncio.CancelledError:
             pass
         logger.info(
             f"_shutdown_bg_tasks() : Execution finished for background task '{task.get_name()}'"
         )
 
-# %% ../../nbs/015_FastKafka.ipynb 46
+# %% ../../nbs/015_FastKafka.ipynb 51
 @patch
 async def _start(self: FastKafka) -> None:
     def is_shutting_down_f(self: FastKafka = self) -> bool:
         return self._is_shutting_down
 
     #     self.create_docs()
     await self._populate_producers()
@@ -779,38 +913,69 @@
     await self._shutdown_bg_tasks()
     await self._shutdown_consumers()
     await self._shutdown_producers()
 
     self._is_shutting_down = False
     self._is_started = False
 
-# %% ../../nbs/015_FastKafka.ipynb 52
+# %% ../../nbs/015_FastKafka.ipynb 57
 @patch
 def create_docs(self: FastKafka) -> None:
+    """
+    Create the asyncapi documentation based on the configured consumers and producers.
+
+    This function exports the asyncapi specification based on the configured consumers
+    and producers in the FastKafka instance. It generates the asyncapi documentation by
+    extracting the topics and callbacks from the consumers and producers.
+
+    Note:
+        The asyncapi documentation is saved to the location specified by the `_asyncapi_path`
+        attribute of the FastKafka instance.
+
+    Returns:
+        None
+    """
     export_async_spec(
         consumers={
-            topic: callback
-            for topic, (callback, _, _, _) in self._consumers_store.items()
+            remove_suffix(topic) if topic.endswith("_0") else topic: callback
+            for topic, (callback, _, _, _, _) in self._consumers_store.items()
         },
         producers={
-            topic: callback for topic, (callback, _, _) in self._producers_store.items()
+            remove_suffix(topic) if topic.endswith("_0") else topic: callback
+            for topic, (callback, _, _, _) in self._producers_store.items()
         },
         kafka_brokers=self._kafka_brokers,
         kafka_service_info=self._kafka_service_info,
         asyncapi_path=self._asyncapi_path,
     )
 
-# %% ../../nbs/015_FastKafka.ipynb 56
+# %% ../../nbs/015_FastKafka.ipynb 61
 class AwaitedMock:
+    """
+    Class representing an awaited mock object.
+
+    Args:
+        o: The original object to be wrapped.
+    """
+
     @staticmethod
     def _await_for(f: Callable[..., Any]) -> Callable[..., Any]:
         @delegates(f)
         async def inner(
             *args: Any, f: Callable[..., Any] = f, timeout: int = 60, **kwargs: Any
         ) -> Any:
+            """
+            Decorator to await the execution of a function.
+
+            Args:
+                f: The function to be wrapped.
+
+            Returns:
+                The wrapped function.
+            """
             if inspect.iscoroutinefunction(f):
                 return await asyncio.wait_for(f(*args, **kwargs), timeout=timeout)
             else:
                 t0 = datetime.now()
                 e: Optional[Exception] = None
                 while True:
                     try:
@@ -823,28 +988,34 @@
                         break
 
                 raise e
 
         return inner
 
     def __init__(self, o: Any):
+        """
+        Initializes an instance of AwaitedMock.
+
+        Args:
+            o: The original object to be wrapped.
+        """
         self._o = o
 
         for name in o.__dir__():
             if not name.startswith("_"):
                 f = getattr(o, name)
                 if inspect.ismethod(f):
                     setattr(self, name, self._await_for(f))
 
-# %% ../../nbs/015_FastKafka.ipynb 57
+# %% ../../nbs/015_FastKafka.ipynb 62
 @patch
 def create_mocks(self: FastKafka) -> None:
     """Creates self.mocks as a named tuple mapping a new function obtained by calling the original functions and a mock"""
-    app_methods = [f for f, _, _, _ in self._consumers_store.values()] + [
-        f for f, _, _ in self._producers_store.values()
+    app_methods = [f for f, _, _, _, _ in self._consumers_store.values()] + [
+        f for f, _, _, _ in self._producers_store.values()
     ]
     self.AppMocks = namedtuple(  # type: ignore
         f"{self.__class__.__name__}Mocks", [f.__name__ for f in app_methods]
     )
 
     self.mocks = self.AppMocks(  # type: ignore
         **{
@@ -883,32 +1054,45 @@
 
     self._consumers_store.update(
         {
             name: (
                 add_mock(f, getattr(self.mocks, f.__name__)),
                 decoder_fn,
                 executor,
+                kafka_brokers,
                 kwargs,
             )
-            for name, (f, decoder_fn, executor, kwargs) in self._consumers_store.items()
+            for name, (
+                f,
+                decoder_fn,
+                executor,
+                kafka_brokers,
+                kwargs,
+            ) in self._consumers_store.items()
         }
     )
 
     self._producers_store.update(
         {
             name: (
                 add_mock(f, getattr(self.mocks, f.__name__)),
                 producer,
+                kafka_brokers,
                 kwargs,
             )
-            for name, (f, producer, kwargs) in self._producers_store.items()
+            for name, (
+                f,
+                producer,
+                kafka_brokers,
+                kwargs,
+            ) in self._producers_store.items()
         }
     )
 
-# %% ../../nbs/015_FastKafka.ipynb 62
+# %% ../../nbs/015_FastKafka.ipynb 67
 @patch
 def benchmark(
     self: FastKafka,
     interval: Union[int, timedelta] = 1,
     *,
     sliding_window_size: Optional[int] = None,
 ) -> Callable[[Callable[[I], Optional[O]]], Callable[[I], Optional[O]]]:
@@ -955,15 +1139,15 @@
         if inspect.iscoroutinefunction(func):
             return async_wrapper  # type: ignore
         else:
             return wrapper
 
     return _decorator
 
-# %% ../../nbs/015_FastKafka.ipynb 64
+# %% ../../nbs/015_FastKafka.ipynb 69
 @patch
 def fastapi_lifespan(
     self: FastKafka, kafka_broker_name: str
 ) -> Callable[["FastAPI"], AsyncIterator[None]]:
     """
     Method for managing the lifespan of a FastAPI application with a specific Kafka broker.
```

### Comparing `fastkafka-0.7.0rc0/fastkafka/_cli.py` & `fastkafka-0.7.0rc1/fastkafka/_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,14 +34,25 @@
         help="input in the form of 'path:app', where **path** is the path to a python file and **app** is an object of type **FastKafka**.",
     ),
     kafka_broker: str = typer.Option(
         "localhost",
         help="kafka_broker, one of the keys of the kafka_brokers dictionary passed in the constructor of FastaKafka class.",
     ),
 ) -> None:
+    """
+    Runs FastKafka application.
+
+    Args:
+        num_workers (int): Number of FastKafka instances to run, defaults to the number of CPU cores.
+        app (str): Input in the form of 'path:app', where **path** is the path to a python file and **app** is an object of type **FastKafka**.
+        kafka_broker (str): Kafka broker, one of the keys of the kafka_brokers dictionary passed in the constructor of FastKafka class.
+
+    Raises:
+        typer.Exit: If there is an unexpected internal error.
+    """
     try:
         asyncio.run(
             run_fastkafka_server(
                 num_workers=num_workers, app=app, kafka_broker=kafka_broker
             )
         )
     except Exception as e:
```

### Comparing `fastkafka-0.7.0rc0/fastkafka/_cli_docs.py` & `fastkafka-0.7.0rc1/fastkafka/_cli_docs.py`

 * *Files 24% similar despite different names*

```diff
@@ -29,14 +29,20 @@
 
 # %% ../nbs/024_CLI_Docs.ipynb 9
 @_docs_app.command(
     "install_deps",
     help="Installs dependencies for FastKafka documentation generation",
 )
 def docs_install_deps() -> None:
+    """
+    Installs dependencies for FastKafka documentation generation.
+
+    Raises:
+        typer.Abort: If the user chooses not to install NodeJS and npm locally.
+    """
     try:
         _check_npm_with_local()
     except Exception as e:
         typer.secho(f"Unexpected internal error: {e}", err=True, fg=typer.colors.RED)
         install_confirm = typer.confirm(
             "npm not found or version is too low, do you want us to install the NodeJS and npm locally?"
         )
@@ -57,14 +63,26 @@
         ".", help="root path under which documentation will be created"
     ),
     app: str = typer.Argument(
         ...,
         help="input in the form of 'path:app', where **path** is the path to a python file and **app** is an object of type **FastKafka**.",
     ),
 ) -> None:
+    """
+    Generates documentation for a FastKafka application.
+
+    Args:
+        root_path: The root path under which the documentation will be created.
+            Default is the current directory.
+        app: Input in the form of 'path:app', where **path** is the path to a python
+            file and **app** is an object of type **FastKafka**.
+
+    Raises:
+        typer.Exit: If there is an unexpected internal error.
+    """
     try:
         application = _import_from_string(app)
         application.skip_docs = False
         application.create_docs()
     except Exception as e:
         typer.secho(f"Unexpected internal error: {e}", err=True, fg=typer.colors.RED)
         raise typer.Exit(1)
@@ -81,18 +99,32 @@
     bind: str = typer.Option("127.0.0.1", help="Some info"),
     port: int = typer.Option(8000, help="Some info"),
     app: str = typer.Argument(
         ...,
         help="input in the form of 'path:app', where **path** is the path to a python file and **app** is an object of type **FastKafka**.",
     ),
 ) -> None:
+    """
+    Generates and serves documentation for a FastKafka application.
+
+    Args:
+        root_path: The root path under which the documentation will be created.
+            Default is the current directory.
+        bind: The IP address to bind the server to. Default is '127.0.0.1'.
+        port: The port number to bind the server to. Default is 8000.
+        app: Input in the form of 'path:app', where **path** is the path to a python
+            file and **app** is an object of type **FastKafka**.
+
+    Raises:
+        typer.Exit: If there is an unexpected internal error.
+    """
     try:
         application = _import_from_string(app)
         application.create_docs()
-        with change_dir("asyncapi/docs/"):
+        with change_dir(application._root_path / "asyncapi" / "docs/"):
             server_address = (bind, port)
             handler = SimpleHTTPRequestHandler
 
             d = {"should_stop": False}
 
             def sigint_handler(
                 signal: int, frame: Optional[FrameType], d: Dict[str, bool] = d
```

### Comparing `fastkafka-0.7.0rc0/fastkafka/_cli_testing.py` & `fastkafka-0.7.0rc1/fastkafka/_cli_testing.py`

 * *Files 23% similar despite different names*

```diff
@@ -19,12 +19,18 @@
 
 # %% ../nbs/025_CLI_Testing.ipynb 9
 @_testing_app.command(
     "install_deps",
     help="Installs dependencies for FastKafka app testing",
 )
 def testing_install_deps() -> None:
+    """
+    Installs dependencies for FastKafka app testing.
+
+    Raises:
+        typer.Exit: If there is an unexpected internal error.
+    """
     try:
         _install_testing_deps()
     except Exception as e:
         typer.secho(f"Unexpected internal error: {e}", err=True, fg=typer.colors.RED)
         raise typer.Exit(1)
```

### Comparing `fastkafka-0.7.0rc0/fastkafka/_components/aiokafka_consumer_loop.py` & `fastkafka-0.7.0rc1/fastkafka/_components/aiokafka_consumer_loop.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc0/fastkafka/_components/asyncapi.py` & `fastkafka-0.7.0rc1/fastkafka/_components/asyncapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # %% auto 0
 __all__ = ['logger', 'sec_scheme_name_mapping', 'KafkaMessage', 'SecurityType', 'APIKeyLocation', 'SecuritySchema', 'KafkaBroker',
            'ContactInfo', 'KafkaServiceInfo', 'KafkaBrokers', 'yaml_file_cmp', 'export_async_spec']
 
 # %% ../../nbs/014_AsyncAPI.ipynb 1
 import json
+import platform
 import shutil
 import subprocess  # nosec: B404: Consider possible security implications associated with the subprocess module.
 import tempfile
 from datetime import timedelta
 from enum import Enum
 from pathlib import Path
 from typing import *
@@ -136,15 +137,36 @@
     description: str = Field("Description of the service")
     contact: ContactInfo = Field(
         ...,
     )
 
 # %% ../../nbs/014_AsyncAPI.ipynb 14
 class KafkaBrokers(BaseModel):
-    brokers: Dict[str, KafkaBroker]
+    brokers: Dict[str, Union[List[KafkaBroker], KafkaBroker]]
+
+    def dict(self, *args: Any, **kwarg: Any) -> Dict[str, Any]:
+        """Transcribe brokers into bootstrap server groups"""
+        d = super().dict(*args, **kwarg)
+
+        brokers = {}
+        for k, v in self.brokers.items():
+            if isinstance(v, list):
+                brokers.update(
+                    {f"{k}-bootstrap-server-{i}": u_v.dict() for i, u_v in enumerate(v)}
+                )
+            else:
+                brokers.update({f"{k}": v.dict()})
+        d["brokers"] = brokers
+        d = {k: v for k, v in d.items() if v is not None}
+
+        return d
+
+    def json(self, *args: Any, **kwargs: Any) -> str:
+        """Serialize into JSON using dict()"""
+        return json.dumps(self.dict(), *args, **kwargs)
 
 # %% ../../nbs/014_AsyncAPI.ipynb 17
 # T = TypeVar("T")
 
 
 def _get_msg_cls_for_producer(f: ProduceCallable) -> Type[Any]:
     types = get_type_hints(f)
@@ -188,45 +210,48 @@
     except IndexError:
         raise ValueError(
             f"Consumer function first param must be a BaseModel subclass msg, got {types_list}"
         )
 
 # %% ../../nbs/014_AsyncAPI.ipynb 27
 def _get_topic_dict(
-    f: Callable[[Any], Any], direction: str = "publish"
+    f: Callable[[Any], Any],
+    direction: str = "publish",
 ) -> Dict[str, Any]:
     if not direction in ["publish", "subscribe"]:
         raise ValueError(
             f"direction must be one of ['publish', 'subscribe'], but it is '{direction}'."
         )
 
     #     msg_cls = None
 
     if direction == "publish":
         msg_cls = _get_msg_cls_for_producer(f)
     elif direction == "subscribe":
         msg_cls = _get_msg_cls_for_consumer(f)
 
     msg_schema = {"message": {"$ref": f"#/components/messages/{msg_cls.__name__}"}}
-    if f.__doc__ is not None:
+    if hasattr(f, "description"):
+        msg_schema["description"] = getattr(f, "description")
+    elif f.__doc__ is not None:
         msg_schema["description"] = f.__doc__  # type: ignore
     return {direction: msg_schema}
 
-# %% ../../nbs/014_AsyncAPI.ipynb 30
+# %% ../../nbs/014_AsyncAPI.ipynb 31
 def _get_channels_schema(
     consumers: Dict[str, ConsumeCallable],
     producers: Dict[str, ProduceCallable],
 ) -> Dict[str, Dict[str, Dict[str, Any]]]:
     topics = {}
     for ms, d in zip([consumers, producers], ["subscribe", "publish"]):
         for topic, f in ms.items():  # type: ignore
             topics[topic] = _get_topic_dict(f, d)
     return topics
 
-# %% ../../nbs/014_AsyncAPI.ipynb 32
+# %% ../../nbs/014_AsyncAPI.ipynb 33
 def _get_kafka_msg_classes(
     consumers: Dict[str, ConsumeCallable],
     producers: Dict[str, ProduceCallable],
 ) -> Set[Type[BaseModel]]:
     fc = [_get_msg_cls_for_consumer(consumer) for consumer in consumers.values()]
     fp = [_get_msg_cls_for_producer(producer) for producer in producers.values()]
     return set(fc + fp)
@@ -234,15 +259,15 @@
 
 def _get_kafka_msg_definitions(
     consumers: Dict[str, ConsumeCallable],
     producers: Dict[str, ProduceCallable],
 ) -> Dict[str, Dict[str, Any]]:
     return schema(_get_kafka_msg_classes(consumers, producers))  # type: ignore
 
-# %% ../../nbs/014_AsyncAPI.ipynb 34
+# %% ../../nbs/014_AsyncAPI.ipynb 35
 def _get_example(cls: Type[BaseModel]) -> BaseModel:
     kwargs: Dict[str, Any] = {}
     for k, v in cls.__fields__.items():
         #         try:
         if (
             hasattr(v, "field_info")
             and hasattr(v.field_info, "extra")
@@ -251,15 +276,15 @@
             example = v.field_info.extra["example"]
             kwargs[k] = example
     #         except:
     #             pass
 
     return json.loads(cls(**kwargs).json())  # type: ignore
 
-# %% ../../nbs/014_AsyncAPI.ipynb 36
+# %% ../../nbs/014_AsyncAPI.ipynb 37
 def _add_example_to_msg_definitions(
     msg_cls: Type[BaseModel], msg_schema: Dict[str, Dict[str, Any]]
 ) -> None:
     try:
         example = _get_example(msg_cls)
     except Exception as e:
         example = None
@@ -280,25 +305,30 @@
         {k: {"payload": v} for k, v in msg_schema["definitions"].items()}
         if "definitions" in msg_schema
         else {}
     )
 
     return msg_schema
 
-# %% ../../nbs/014_AsyncAPI.ipynb 38
+# %% ../../nbs/014_AsyncAPI.ipynb 39
 def _get_security_schemes(kafka_brokers: KafkaBrokers) -> Dict[str, Any]:
     security_schemes = {}
-    for key, kafka_broker in kafka_brokers.brokers.items():
+    for key, broker in kafka_brokers.brokers.items():
+        if isinstance(broker, list):
+            kafka_broker = broker[0]
+        else:
+            kafka_broker = broker
+
         if kafka_broker.security is not None:
             security_schemes[f"{key}_default_security"] = json.loads(
                 kafka_broker.security.json()
             )
     return security_schemes
 
-# %% ../../nbs/014_AsyncAPI.ipynb 40
+# %% ../../nbs/014_AsyncAPI.ipynb 41
 def _get_components_schema(
     consumers: Dict[str, ConsumeCallable],
     producers: Dict[str, ProduceCallable],
     kafka_brokers: KafkaBrokers,
 ) -> Dict[str, Any]:
     definitions = _get_msg_definitions_with_examples(consumers, producers)
     msg_classes = [cls.__name__ for cls in _get_kafka_msg_classes(consumers, producers)]
@@ -323,24 +353,24 @@
             for k, v in substitutions.items():
                 if d == k:
                     d = v
         return d
 
     return _sub_values(components)  # type: ignore
 
-# %% ../../nbs/014_AsyncAPI.ipynb 42
+# %% ../../nbs/014_AsyncAPI.ipynb 43
 def _get_servers_schema(kafka_brokers: KafkaBrokers) -> Dict[str, Any]:
     servers = json.loads(kafka_brokers.json(sort_keys=False))["brokers"]
 
     for key, kafka_broker in servers.items():
         if "security" in kafka_broker:
             servers[key]["security"] = [{f"{key}_default_security": []}]
     return servers  # type: ignore
 
-# %% ../../nbs/014_AsyncAPI.ipynb 44
+# %% ../../nbs/014_AsyncAPI.ipynb 45
 def _get_asyncapi_schema(
     consumers: Dict[str, ConsumeCallable],
     producers: Dict[str, ProduceCallable],
     kafka_brokers: KafkaBrokers,
     kafka_service_info: KafkaServiceInfo,
 ) -> Dict[str, Any]:
     #     # we don't use dict because we need custom JSON encoders
@@ -353,31 +383,40 @@
         "asyncapi": "2.5.0",
         "info": info,
         "servers": servers,
         "channels": channels,
         "components": components,
     }
 
-# %% ../../nbs/014_AsyncAPI.ipynb 46
+# %% ../../nbs/014_AsyncAPI.ipynb 47
 def yaml_file_cmp(file_1: Union[Path, str], file_2: Union[Path, str]) -> bool:
+    """Compares two YAML files and returns True if their contents are equal, False otherwise.
+
+    Args:
+        file_1: Path or string representing the first YAML file.
+        file_2: Path or string representing the second YAML file.
+
+    Returns:
+        A boolean indicating whether the contents of the two YAML files are equal.
+    """
     try:
         import yaml
     except Exception as e:
         msg = "Please install docs version of fastkafka using 'pip install fastkafka[docs]' command"
         logger.error(msg)
         raise RuntimeError(msg)
 
     def _read(f: Union[Path, str]) -> Dict[str, Any]:
         with open(f) as stream:
             return yaml.safe_load(stream)  # type: ignore
 
     d = [_read(f) for f in [file_1, file_2]]
     return d[0] == d[1]
 
-# %% ../../nbs/014_AsyncAPI.ipynb 47
+# %% ../../nbs/014_AsyncAPI.ipynb 48
 def _generate_async_spec(
     *,
     consumers: Dict[str, ConsumeCallable],
     producers: Dict[str, ProduceCallable],
     kafka_brokers: KafkaBrokers,
     kafka_service_info: KafkaServiceInfo,
     spec_path: Path,
@@ -413,15 +452,15 @@
             return True
         else:
             logger.info(
                 f"Keeping the old async specifications at: '{spec_path.resolve()}'"
             )
             return False
 
-# %% ../../nbs/014_AsyncAPI.ipynb 49
+# %% ../../nbs/014_AsyncAPI.ipynb 50
 def _generate_async_docs(
     *,
     spec_path: Path,
     docs_path: Path,
 ) -> None:
     _check_npm_with_local()
     cmd = [
@@ -432,43 +471,50 @@
         "ag",
         f"{spec_path}",
         "@asyncapi/html-template",
         "-o",
         f"{docs_path}",
         "--force-write",
     ]
-    p = subprocess.run(  # nosec: B603 subprocess call - check for execution of untrusted input.
-        cmd, stderr=subprocess.STDOUT, stdout=subprocess.PIPE
+    # nosemgrep: python.lang.security.audit.subprocess-shell-true.subprocess-shell-true
+    p = subprocess.run(  # nosec: B602, B603 subprocess call - check for execution of untrusted input.
+        cmd,
+        stderr=subprocess.STDOUT,
+        stdout=subprocess.PIPE,
+        shell=True if platform.system() == "Windows" else False,
     )
     if p.returncode == 0:
         logger.info(f"Async docs generated at '{docs_path}'")
         logger.info(f"Output of '$ {' '.join(cmd)}'{p.stdout.decode()}")
     else:
         logger.error(f"Generation of async docs failed!")
         logger.info(f"Output of '$ {' '.join(cmd)}'{p.stdout.decode()}")
         raise ValueError(
             f"Generation of async docs failed, used '$ {' '.join(cmd)}'{p.stdout.decode()}"
         )
 
-# %% ../../nbs/014_AsyncAPI.ipynb 51
+# %% ../../nbs/014_AsyncAPI.ipynb 52
 def export_async_spec(
     *,
     consumers: Dict[str, ConsumeCallable],
     producers: Dict[str, ProduceCallable],
     kafka_brokers: KafkaBrokers,
     kafka_service_info: KafkaServiceInfo,
     asyncapi_path: Union[Path, str],
     force_rebuild: bool = True,
 ) -> None:
-    """Export async specification to a given path
-
-    Params:
-        path: path where the specification will be exported. If parent subdirectories do not exist, they will be created.
-
+    """Exports the AsyncAPI specification and documentation to the given path.
 
+    Args:
+        consumers: Dictionary of consumer functions, where the keys are the channel names and the values are the consumer functions.
+        producers: Dictionary of producer functions, where the keys are the channel names and the values are the producer functions.
+        kafka_brokers: KafkaBrokers object representing the Kafka brokers configuration.
+        kafka_service_info: KafkaServiceInfo object representing the Kafka service info configuration.
+        asyncapi_path: Path or string representing the base path where the specification and documentation will be exported.
+        force_rebuild: Boolean indicating whether to force a rebuild of the specification file even if it already exists.
     """
     # generate spec file
     spec_path = Path(asyncapi_path) / "spec" / "asyncapi.yml"
     is_spec_built = _generate_async_spec(
         consumers=consumers,
         producers=producers,
         kafka_brokers=kafka_brokers,
```

### Comparing `fastkafka-0.7.0rc0/fastkafka/_components/benchmarking.py` & `fastkafka-0.7.0rc1/fastkafka/_components/benchmarking.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc0/fastkafka/_components/encoder/avro.py` & `fastkafka-0.7.0rc1/fastkafka/_components/encoder/avro.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc0/fastkafka/_components/encoder/json.py` & `fastkafka-0.7.0rc1/fastkafka/_components/encoder/json.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc0/fastkafka/_components/helpers.py` & `fastkafka-0.7.0rc1/fastkafka/_components/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/998_Internal_Helpers.ipynb.
 
 # %% auto 0
-__all__ = ['in_notebook', 'change_dir', 'ImportFromStringError', 'true_after', 'unwrap_list_type']
+__all__ = ['in_notebook', 'change_dir', 'ImportFromStringError', 'true_after', 'unwrap_list_type', 'remove_suffix']
 
 # %% ../../nbs/998_Internal_Helpers.ipynb 2
 def in_notebook() -> bool:
+    """
+    Checks if the code is running in a Jupyter notebook or not.
+
+    Returns:
+        True if running in a Jupyter notebook, False otherwise.
+    """
     try:
         from IPython import get_ipython
 
         if "IPKernelApp" not in get_ipython().config:
             return False
     except ImportError:
         return False
@@ -26,14 +32,23 @@
 from typing import *
 
 import typer
 
 # %% ../../nbs/998_Internal_Helpers.ipynb 6
 @contextlib.contextmanager
 def change_dir(d: str) -> Generator[None, None, None]:
+    """
+    Changes the current working directory temporarily.
+
+    Args:
+        d: The directory to change to.
+
+    Yields:
+        None.
+    """
     curdir = os.getcwd()
     os.chdir(d)
     try:
         yield
     finally:
         os.chdir(curdir)
 
@@ -113,7 +128,20 @@
         - Input: int
           Output: int
     """
     if hasattr(var_type, "__origin__") and var_type.__origin__ == list:
         return var_type.__args__[0]  # type: ignore
     else:
         return var_type
+
+# %% ../../nbs/998_Internal_Helpers.ipynb 14
+def remove_suffix(topic: str) -> str:
+    """
+    Removes the suffix from a string by splitting on underscores and joining all but the last element.
+
+    Args:
+        topic: The string to remove the suffix from.
+
+    Returns:
+        The string without the suffix.
+    """
+    return "_".join(topic.split("_")[:-1])
```

### Comparing `fastkafka-0.7.0rc0/fastkafka/_components/logger.py` & `fastkafka-0.7.0rc1/fastkafka/_components/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -134,14 +134,26 @@
     for logger in loggers:
         logger.setLevel(level)
 
 # %% ../../nbs/Logger.ipynb 18
 def cached_log(
     self: logging.Logger, msg: str, level: int, timeout: Union[int, float] = 5
 ) -> None:
+    """
+    Logs a message with a specified level only once within a given timeout.
+
+    Args:
+        self: The logger instance.
+        msg: The message to log.
+        level: The logging level for the message.
+        timeout: The timeout duration in seconds.
+
+    Returns:
+        None
+    """
     if not hasattr(self, "_timeouted_msgs"):
         self._timeouted_msgs = {}  # type: ignore
 
     if msg not in self._timeouted_msgs or self._timeouted_msgs[msg]():  # type: ignore
         self._timeouted_msgs[msg] = true_after(timeout)  # type: ignore
 
         self.log(level, msg)
```

### Comparing `fastkafka-0.7.0rc0/fastkafka/_components/meta.py` & `fastkafka-0.7.0rc1/fastkafka/_components/meta.py`

 * *Files 3% similar despite different names*

```diff
@@ -320,25 +320,45 @@
     return {k: v for k, v in kwargs.items() if k in param_names}
 
 # %% ../../nbs/096_Meta.ipynb 70
 TorF = TypeVar("TorF", Type, Callable[..., Any])
 
 
 def export(module_name: str) -> Callable[[TorF], TorF]:
+    """
+    Decorator that sets the __module__ attribute of the decorated object to the specified module name.
+
+    Args:
+        module_name: Name of the module to set as __module__ attribute.
+
+    Returns:
+        Decorator function that sets the __module__ attribute of the decorated object.
+    """
+
     def _inner(o: TorF, module_name: str = module_name) -> TorF:
         o.__module__ = module_name
         return o
 
     return _inner
 
 # %% ../../nbs/096_Meta.ipynb 73
 T = TypeVar("T")
 
 
 def classcontextmanager(name: str = "lifecycle") -> Callable[[Type[T]], Type[T]]:
+    """
+    Decorator that adds context manager functionality to a class.
+
+    Args:
+        name: Name of the context manager attribute in the class. Default is "lifecycle".
+
+    Returns:
+        Decorator function that adds context manager functionality to the class.
+    """
+
     def _classcontextmanager(cls: Type[T], name: str = name) -> Type[T]:
         if not hasattr(cls, name):
             raise ValueError
 
         @patch
         def __enter__(self: cls) -> Any:  # type: ignore
             if not hasattr(self, "_lifecycle_ctx"):
```

### Comparing `fastkafka-0.7.0rc0/fastkafka/_components/producer_decorator.py` & `fastkafka-0.7.0rc1/fastkafka/_components/producer_decorator.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from typing import *
 
 from aiokafka import AIOKafkaProducer
 from aiokafka.producer.message_accumulator import BatchBuilder
 from pydantic import BaseModel
 
 from .meta import export
+from .helpers import remove_suffix
 
 # %% ../../nbs/013_ProducerDecorator.ipynb 3
 BaseSubmodel = TypeVar("BaseSubmodel", bound=Union[List[BaseModel], BaseModel])
 BaseSubmodel
 
 
 @dataclass
@@ -40,15 +41,15 @@
     key: Optional[bytes] = None
 
 # %% ../../nbs/013_ProducerDecorator.ipynb 5
 def unwrap_from_kafka_event(var_type: Union[Type, Parameter]) -> Union[Type, Parameter]:
     """
     Unwraps the type from a KafkaEvent.
 
-    Vars:
+    Args:
         var_type: Type to unwrap.
 
     Returns:
         Type: Unwrapped type if the given type is a KafkaEvent, otherwise returns the same type.
 
     Example:
         - Input: KafkaEvent[str]
@@ -83,37 +84,73 @@
 # %% ../../nbs/013_ProducerDecorator.ipynb 14
 async def produce_single(  # type: ignore
     producer: AIOKafkaProducer,
     topic: str,
     encoder_fn: Callable[[BaseModel], bytes],
     wrapped_val: KafkaEvent[BaseModel],
 ) -> ProduceReturnTypes:
+    """
+    Sends a single message to the Kafka producer.
+
+    Args:
+        producer (AIOKafkaProducer): The Kafka producer object.
+        topic (str): The topic to which the message will be sent.
+        encoder_fn (Callable[[BaseModel], bytes]): The encoding function to encode the message.
+        wrapped_val (KafkaEvent[BaseModel]): The wrapped Kafka event containing the message.
+
+    Returns:
+        ProduceReturnTypes: The return value from the decorated function.
+    """
     fut = await producer.send(
         topic, encoder_fn(wrapped_val.message), key=wrapped_val.key
     )
     fut.add_done_callback(release_callback)
 
 # %% ../../nbs/013_ProducerDecorator.ipynb 16
 async def send_batch(  # type: ignore
     producer: AIOKafkaProducer, topic: str, batch: BatchBuilder, key: Optional[bytes]
 ) -> None:
+    """
+    Sends a batch of messages to the Kafka producer.
+
+    Args:
+        producer (AIOKafkaProducer): The Kafka producer object.
+        topic (str): The topic to which the messages will be sent.
+        batch (BatchBuilder): The batch builder object containing the messages.
+        key (Optional[bytes]): The optional key used to identify the batch of messages.
+
+    Returns:
+        None
+    """
     partitions = await producer.partitions_for(topic)
     if key == None:
         partition = random.choice(tuple(partitions))  # nosec
     else:
         partition = producer._partition(topic, None, None, None, key, None)
     await producer.send_batch(batch, topic, partition=partition)
 
 
 async def produce_batch(  # type: ignore
     producer: AIOKafkaProducer,
     topic: str,
     encoder_fn: Callable[[BaseModel], bytes],
     wrapped_val: KafkaEvent[List[BaseModel]],
 ) -> ProduceReturnTypes:
+    """
+    Sends a batch of messages to the Kafka producer.
+
+    Args:
+        producer (AIOKafkaProducer): The Kafka producer object.
+        topic (str): The topic to which the messages will be sent.
+        encoder_fn (Callable[[BaseModel], bytes]): The encoding function to encode the messages.
+        wrapped_val (KafkaEvent[List[BaseModel]]): The wrapped Kafka event containing the list of messages.
+
+    Returns:
+        ProduceReturnTypes: The return value from the decorated function.
+    """
     batch = producer.create_batch()
 
     for message in wrapped_val.message:
         metadata = batch.append(
             key=wrapped_val.key,
             value=encoder_fn(message),
             timestamp=int(time.time() * 1000),
@@ -129,31 +166,46 @@
 
     await send_batch(producer, topic, batch, wrapped_val.key)
 
 # %% ../../nbs/013_ProducerDecorator.ipynb 18
 def producer_decorator(
     producer_store: Dict[str, Any],
     func: ProduceCallable,
-    topic: str,
+    topic_key: str,
     encoder_fn: Callable[[BaseModel], bytes],
 ) -> ProduceCallable:
-    """todo: write documentation"""
+    """
+    Decorator for Kafka producer functions.
+
+    Args:
+        producer_store (Dict[str, Any]): Dictionary to store the Kafka producer objects.
+        func (ProduceCallable): The function to be decorated.
+        topic_key (str): The key used to identify the topic.
+        encoder_fn (Callable[[BaseModel], bytes]): The encoding function to encode the messages.
+
+    Returns:
+        ProduceCallable: The decorated function.
+
+    Raises:
+        ValueError: If the decorated function is synchronous.
+    """
 
     @functools.wraps(func)
     async def _produce_async(
         *args: List[Any],
-        topic: str = topic,
+        topic_key: str = topic_key,
         encoder_fn: Callable[[BaseModel], bytes] = encoder_fn,
         producer_store: Dict[str, Any] = producer_store,
         f: Callable[..., Awaitable[ProduceReturnTypes]] = func,  # type: ignore
         **kwargs: Any,
     ) -> ProduceReturnTypes:
         return_val = await f(*args, **kwargs)
         wrapped_val = _wrap_in_event(return_val)
-        _, producer, _ = producer_store[topic]
+        _, producer, _, _ = producer_store[topic_key]
+        topic = remove_suffix(topic_key)
 
         if isinstance(wrapped_val.message, list):
             await produce_batch(producer, topic, encoder_fn, wrapped_val)
         else:
             await produce_single(producer, topic, encoder_fn, wrapped_val)
         return return_val
```

### Comparing `fastkafka-0.7.0rc0/fastkafka/_components/task_streaming.py` & `fastkafka-0.7.0rc1/fastkafka/_components/task_streaming.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,24 @@
 # %% ../../nbs/006_TaskStreaming.ipynb 10
 class TaskPool:
     def __init__(
         self,
         size: int = 100_000,
         on_error: Optional[Callable[[BaseException], None]] = None,
     ):
+        """
+        Initializes a TaskPool instance.
+
+        Args:
+            size: The size of the task pool. Defaults to 100,000.
+            on_error: Optional callback function to handle task errors. Defaults to None.
+
+        Returns:
+            None
+        """
         self.size = size
         self.pool: Set[Task] = set()
         self.on_error = on_error
         self.finished = False
 
     async def add(self, item: Task) -> None:
         """
@@ -104,14 +114,20 @@
             logger.warning(f"{e=}")
 
         return _log_error
 
 # %% ../../nbs/006_TaskStreaming.ipynb 14
 class ExceptionMonitor:
     def __init__(self) -> None:
+        """
+        Initializes an ExceptionMonitor instance.
+
+        Returns:
+            None
+        """
         self.exceptions: List[Exception] = []
         self.exception_found = False
 
     def on_error(self, e: Exception) -> None:
         """
         Handles an error by storing the exception.
 
@@ -149,14 +165,25 @@
     async def run(  # type: ignore
         self,
         *,
         is_shutting_down_f: Callable[[], bool],
         generator: Callable[[], Awaitable[ConsumerRecord]],
         processor: Callable[[ConsumerRecord], Awaitable[None]],
     ) -> None:
+        """
+        Abstract method for running the stream executor.
+
+        Args:
+            is_shutting_down_f: Function to check if the executor is shutting down.
+            generator: Generator function for retrieving consumer records.
+            processor: Processor function for processing consumer records.
+
+        Returns:
+            None
+        """
         pass
 
 # %% ../../nbs/006_TaskStreaming.ipynb 20
 def _process_items_task(  # type: ignore
     processor: Callable[[ConsumerRecord], Awaitable[None]], task_pool: TaskPool
 ) -> Callable[
     [
```

### Comparing `fastkafka-0.7.0rc0/fastkafka/_components/test_dependencies.py` & `fastkafka-0.7.0rc1/fastkafka/_components/test_dependencies.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/098_Test_Dependencies.ipynb.
 
 # %% auto 0
 __all__ = ['logger', 'kafka_version', 'kafka_fname', 'kafka_url', 'local_path', 'tgz_path', 'kafka_path', 'check_java',
            'check_kafka', 'generate_app_src', 'generate_app_in_tmp']
 
 # %% ../../nbs/098_Test_Dependencies.ipynb 2
+import platform
 import shutil
 import tarfile
 from contextlib import contextmanager
-from os import environ
+from os import environ, rename
+from os.path import expanduser
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import *
 
 from .helpers import change_dir, in_notebook
 from .logger import get_logger
 
@@ -22,75 +24,126 @@
     from tqdm import tqdm
 
 # %% ../../nbs/098_Test_Dependencies.ipynb 4
 logger = get_logger(__name__)
 
 # %% ../../nbs/098_Test_Dependencies.ipynb 6
 def check_java(*, potential_jdk_path: Optional[List[Path]] = None) -> bool:
+    """Checks if JDK 11 is installed on the machine and exports it to PATH if necessary.
+
+    Args:
+        potential_jdk_path: Optional. List of potential paths where JDK 11 may be installed.
+                            If not provided, it defaults to searching for JDK 11 in the user's home directory.
+
+    Returns:
+        bool: True if JDK 11 is installed and exported to PATH, False otherwise.
+    """
     if potential_jdk_path is None:
-        potential_jdk_path = list(Path(environ["HOME"] + "/.jdk").glob("jdk-11*"))
+        potential_jdk_path = list(Path(expanduser("~") + "/.jdk").glob("jdk-11*"))
 
     if potential_jdk_path != []:
         logger.info("Java is already installed.")
         if not shutil.which("java"):
             logger.info("But not exported to PATH, exporting...")
-            environ["PATH"] = environ["PATH"] + f":{potential_jdk_path[0]}/bin"
+            env_path_separator = ";" if platform.system() == "Windows" else ":"
+            environ["PATH"] = (
+                environ["PATH"] + f"{env_path_separator}{potential_jdk_path[0]/ 'bin'}"
+            )
         return True
     return False
 
 # %% ../../nbs/098_Test_Dependencies.ipynb 8
 def _install_java() -> None:
     """Checks if jdk-11 is installed on the machine and installs it if not
+
     Returns:
        None
+
+    Raises:
+        RuntimeError: If JDK 11 installation fails.
     """
     try:
         import jdk
     except Exception as e:
         msg = "Please install test version of fastkafka using 'pip install fastkafka[test]' command"
         logger.error(msg)
         raise RuntimeError(msg)
 
     if not check_java():
         logger.info("Installing Java...")
         logger.info(" - installing jdk...")
-        jdk_bin_path = jdk.install("11")
+        jdk_bin_path = Path(jdk.install("11"))
         logger.info(f" - jdk path: {jdk_bin_path}")
-        environ["PATH"] = environ["PATH"] + f":{jdk_bin_path}/bin"
+        env_path_separator = ";" if platform.system() == "Windows" else ":"
+        environ["PATH"] = (
+            environ["PATH"] + f"{env_path_separator}{jdk_bin_path / 'bin'}"
+        )
         logger.info("Java installed.")
 
 # %% ../../nbs/098_Test_Dependencies.ipynb 10
 # ToDo: move it somewhere
 kafka_version = "3.3.2"
 kafka_fname = f"kafka_2.13-{kafka_version}"
 kafka_url = f"https://dlcdn.apache.org/kafka/{kafka_version}/{kafka_fname}.tgz"
-local_path = Path(environ["HOME"]) / ".local"
+local_path = (
+    Path(expanduser("~")).parent / "Public"
+    if platform.system() == "Windows"
+    else Path(expanduser("~")) / ".local"
+)
 tgz_path = local_path / f"{kafka_fname}.tgz"
-kafka_path = local_path / f"{kafka_fname}"
+kafka_path = (
+    local_path / "kafka"
+    if platform.system() == "Windows"
+    else local_path / f"{kafka_fname}"
+)
 
 
 def check_kafka(kafka_path: Path = kafka_path) -> bool:
+    """Checks if Kafka is installed on the machine and exports it to PATH if necessary.
+
+    Args:
+        kafka_path: Path to the Kafka installation directory. Defaults to the global variable `kafka_path`.
+
+    Returns:
+        bool: True if Kafka is installed and exported to PATH, False otherwise.
+    """
     if (kafka_path / "bin").exists():
         logger.info("Kafka is installed.")
         if not shutil.which("kafka-server-start.sh"):
             logger.info("But not exported to PATH, exporting...")
-            environ["PATH"] = environ["PATH"] + f":{kafka_path}/bin"
+            kafka_binary_path = (
+                f";{kafka_path / 'bin' / 'windows'}"
+                if platform.system() == "Windows"
+                else f":{kafka_path / 'bin'}"
+            )
+            environ["PATH"] = environ["PATH"] + kafka_binary_path
         return True
     return False
 
 # %% ../../nbs/098_Test_Dependencies.ipynb 11
 def _install_kafka(
     *,
     kafka_url: str = kafka_url,
     local_path: Path = local_path,
     tgz_path: Path = tgz_path,
+    kafka_path: Path = kafka_path,
 ) -> None:
-    """Checks if kafka is installed on the machine and installs it if not
+    """Checks if Kafka is installed on the machine and installs it if not.
+
+    Args:
+        kafka_url: URL to download the Kafka installation package. Defaults to the global variable `kafka_url`.
+        local_path: Path where the Kafka installation package will be stored. Defaults to the global variable `local_path`.
+        tgz_path: Path where the Kafka installation package will be extracted. Defaults to the global variable `tgz_path`.
+        kafka_path: Path where Kafka will be installed. Defaults to the global variable `kafka_path`.
+
     Returns:
        None
+
+    Raises:
+        RuntimeError: If Kafka installation fails.
     """
     try:
         import requests
     except Exception as e:
         msg = "Please install test version of fastkafka using 'pip install fastkafka[test]' command"
         logger.error(msg)
         raise RuntimeError(msg)
@@ -112,24 +165,45 @@
             for data in tqdm(response.iter_content(chunk_size=128), total=total):
                 f.write(data)
 
         with tarfile.open(tgz_path) as tar:
             for tarinfo in tar:
                 tar.extract(tarinfo, local_path)
 
-        environ["PATH"] = environ["PATH"] + f":{kafka_path}/bin"
+        if platform.system() == "Windows":
+            rename(local_path / f"{kafka_fname}", kafka_path)
+
+        kafka_binary_path = (
+            f";{kafka_path / 'bin' / 'windows'}"
+            if platform.system() == "Windows"
+            else f":{kafka_path / 'bin'}"
+        )
+        environ["PATH"] = environ["PATH"] + kafka_binary_path
         logger.info(f"Kafka installed in {kafka_path}.")
 
 # %% ../../nbs/098_Test_Dependencies.ipynb 13
 def _install_testing_deps() -> None:
+    """Installs Java and Kafka dependencies required for testing.
+
+    Raises:
+        RuntimeError: If Java or Kafka installation fails.
+    """
     _install_java()
     _install_kafka()
 
 # %% ../../nbs/098_Test_Dependencies.ipynb 15
 def generate_app_src(out_path: Union[Path, str]) -> None:
+    """Generates the source code for the test application based on a Jupyter notebook.
+
+    Args:
+        out_path: Path where the generated source code will be saved.
+
+    Raises:
+        ValueError: If the Jupyter notebook file does not exist.
+    """
     import nbformat
     from nbconvert import PythonExporter
 
     path = Path("099_Test_Service.ipynb")
     if not path.exists():
         path = Path("..") / "099_Test_Service.ipynb"
     if not path.exists():
@@ -142,13 +216,18 @@
 
     with open(out_path, "w") as f:
         f.write(source)
 
 # %% ../../nbs/098_Test_Dependencies.ipynb 17
 @contextmanager
 def generate_app_in_tmp() -> Generator[str, None, None]:
+    """Context manager that generates the test application source code in a temporary directory.
+
+    Yields:
+        str: Import statement for the generated test application.
+    """
     with TemporaryDirectory() as d:
         src_path = Path(d) / "main.py"
         generate_app_src(src_path)
         with change_dir(d):
             import_str = f"{src_path.stem}:kafka_app"
             yield import_str
```

### Comparing `fastkafka-0.7.0rc0/fastkafka/_docusaurus_helper.py` & `fastkafka-0.7.0rc1/fastkafka/_docusaurus_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -453,14 +453,31 @@
 
 # %% ../nbs/096_Docusaurus_Helper.ipynb 66
 def generate_sidebar(
     summary_file: str = "./docusaurus/docs/SUMMARY.md",
     summary: str = "",
     target: str = "./docusaurus/sidebars.js",
 ) -> None:
+    """
+    Generate a sidebar js file for a Docusaurus documentation site based on a SUMMARY.md file.
+
+    Args:
+        summary_file: The path to the SUMMARY.md file containing the documentation structure.
+            Default is "./docusaurus/docs/SUMMARY.md".
+        summary: An optional summary string.
+            Default is an empty string.
+        target: The path to the target sidebar js file to be generated.
+            Default is "./docusaurus/sidebars.js".
+
+    Returns:
+        None: The function does not return any value directly, but it generates a sidebar file.
+
+    Raises:
+        FileNotFoundError: If the specified `summary_file` does not exist.
+    """
     with open(summary_file, "r") as stream, open(target, "w") as target_stream:
         summary_contents = stream.read()
 
         guides_summary = _get_section_from_markdown(summary_contents, "Guides")
         parsed_guides = _parse_section(guides_summary)  # type: ignore
 
         api_summary = _get_section_from_markdown(summary_contents, "API")
```

### Comparing `fastkafka-0.7.0rc0/fastkafka/_helpers.py` & `fastkafka-0.7.0rc1/fastkafka/_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -830,14 +830,26 @@
             ),
         )
 
 # %% ../nbs/999_Helpers.ipynb 23
 def get_collapsible_admonition(
     code_block: str, *, name: Optional[str] = None
 ) -> Markdown:
+    """
+    Generate a collapsible admonition containing a code block as an example.
+
+    Args:
+        code_block: The code block to be included in the example.
+        name: Optional name or title for the example.
+            Default is None.
+
+    Returns:
+        A Markdown object representing the collapsible admonition
+        with the provided code block.
+    """
     alt_name = "" if name is None else name
     intro = f'This example contains the content of the file "{alt_name}":'
     return Markdown(
         f"??? Example \n\n    {intro}\n\n"
         + textwrap.indent(f"```python\n{code_block}\n```", prefix="    ")
     )
 
@@ -857,14 +869,31 @@
 """
     )
 
 # %% ../nbs/999_Helpers.ipynb 27
 async def wait_for_get_url(
     url: str, timeout: Optional[int] = None, **kwargs: Dict[str, Any]
 ) -> aiohttp.ClientResponse:
+    """
+    Asynchronously wait for a GET request to a specified URL with an optional timeout.
+
+    Args:
+        url: The URL to send the GET request to.
+        timeout: Optional maximum number of seconds to wait
+            for a response. If not provided, there is no timeout. Default is None.
+        **kwargs: Additional keyword arguments to be passed to the tqdm progress bar,
+            if a timeout is provided.
+
+    Returns:
+        The aiohttp.ClientResponse response object for the GET request.
+
+    Raises:
+        TimeoutError: If the timeout is reached and the URL couldn't be fetched within
+            the specified time.
+    """
     t0 = datetime.now()
     if timeout is not None:
         pbar = tqdm(total=timeout, **kwargs)
     try:
         async with aiohttp.ClientSession() as session:
             while True:
                 try:
```

### Comparing `fastkafka-0.7.0rc0/fastkafka/_modidx.py` & `fastkafka-0.7.0rc1/fastkafka/_modidx.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,14 @@
                                                                                                'fastkafka/_application/app.py'),
                                             'fastkafka._application.app.FastKafka._populate_bg_tasks': ( 'fastkafka.html#fastkafka._populate_bg_tasks',
                                                                                                          'fastkafka/_application/app.py'),
                                             'fastkafka._application.app.FastKafka._populate_consumers': ( 'fastkafka.html#fastkafka._populate_consumers',
                                                                                                           'fastkafka/_application/app.py'),
                                             'fastkafka._application.app.FastKafka._populate_producers': ( 'fastkafka.html#fastkafka._populate_producers',
                                                                                                           'fastkafka/_application/app.py'),
-                                            'fastkafka._application.app.FastKafka._set_bootstrap_servers': ( 'fastkafka.html#fastkafka._set_bootstrap_servers',
-                                                                                                             'fastkafka/_application/app.py'),
                                             'fastkafka._application.app.FastKafka._shutdown_bg_tasks': ( 'fastkafka.html#fastkafka._shutdown_bg_tasks',
                                                                                                          'fastkafka/_application/app.py'),
                                             'fastkafka._application.app.FastKafka._shutdown_consumers': ( 'fastkafka.html#fastkafka._shutdown_consumers',
                                                                                                           'fastkafka/_application/app.py'),
                                             'fastkafka._application.app.FastKafka._shutdown_producers': ( 'fastkafka.html#fastkafka._shutdown_producers',
                                                                                                           'fastkafka/_application/app.py'),
                                             'fastkafka._application.app.FastKafka._start': ( 'fastkafka.html#fastkafka._start',
@@ -55,50 +53,70 @@
                                                                                                'fastkafka/_application/app.py'),
                                             'fastkafka._application.app.FastKafka.run_in_background': ( 'fastkafka.html#fastkafka.run_in_background',
                                                                                                         'fastkafka/_application/app.py'),
                                             'fastkafka._application.app.FastKafka.set_kafka_broker': ( 'fastkafka.html#fastkafka.set_kafka_broker',
                                                                                                        'fastkafka/_application/app.py'),
                                             'fastkafka._application.app._create_producer': ( 'fastkafka.html#_create_producer',
                                                                                              'fastkafka/_application/app.py'),
+                                            'fastkafka._application.app._get_broker_addr_list': ( 'fastkafka.html#_get_broker_addr_list',
+                                                                                                  'fastkafka/_application/app.py'),
                                             'fastkafka._application.app._get_contact_info': ( 'fastkafka.html#_get_contact_info',
                                                                                               'fastkafka/_application/app.py'),
                                             'fastkafka._application.app._get_decoder_fn': ( 'fastkafka.html#_get_decoder_fn',
                                                                                             'fastkafka/_application/app.py'),
                                             'fastkafka._application.app._get_encoder_fn': ( 'fastkafka.html#_get_encoder_fn',
                                                                                             'fastkafka/_application/app.py'),
                                             'fastkafka._application.app._get_kafka_brokers': ( 'fastkafka.html#_get_kafka_brokers',
                                                                                                'fastkafka/_application/app.py'),
                                             'fastkafka._application.app._get_kafka_config': ( 'fastkafka.html#_get_kafka_config',
                                                                                               'fastkafka/_application/app.py'),
                                             'fastkafka._application.app._get_topic_name': ( 'fastkafka.html#_get_topic_name',
-                                                                                            'fastkafka/_application/app.py')},
-            'fastkafka._application.tester': { 'fastkafka._application.tester.Tester': ( 'tester.html#tester',
+                                                                                            'fastkafka/_application/app.py'),
+                                            'fastkafka._application.app._prepare_and_check_brokers': ( 'fastkafka.html#_prepare_and_check_brokers',
+                                                                                                       'fastkafka/_application/app.py'),
+                                            'fastkafka._application.app._resolve_key': ( 'fastkafka.html#_resolve_key',
+                                                                                         'fastkafka/_application/app.py')},
+            'fastkafka._application.tester': { 'fastkafka._application.tester.AmbiguousWarning': ( 'tester.html#ambiguouswarning',
+                                                                                                   'fastkafka/_application/tester.py'),
+                                               'fastkafka._application.tester.AmbiguousWarning.__call__': ( 'tester.html#ambiguouswarning.__call__',
+                                                                                                            'fastkafka/_application/tester.py'),
+                                               'fastkafka._application.tester.AmbiguousWarning.__getattribute__': ( 'tester.html#ambiguouswarning.__getattribute__',
+                                                                                                                    'fastkafka/_application/tester.py'),
+                                               'fastkafka._application.tester.AmbiguousWarning.__init__': ( 'tester.html#ambiguouswarning.__init__',
+                                                                                                            'fastkafka/_application/tester.py'),
+                                               'fastkafka._application.tester.Tester': ( 'tester.html#tester',
                                                                                          'fastkafka/_application/tester.py'),
                                                'fastkafka._application.tester.Tester.__aenter__': ( 'tester.html#tester.__aenter__',
                                                                                                     'fastkafka/_application/tester.py'),
                                                'fastkafka._application.tester.Tester.__aexit__': ( 'tester.html#tester.__aexit__',
                                                                                                    'fastkafka/_application/tester.py'),
                                                'fastkafka._application.tester.Tester.__init__': ( 'tester.html#tester.__init__',
                                                                                                   'fastkafka/_application/tester.py'),
+                                               'fastkafka._application.tester.Tester._arrange_mirrors': ( 'tester.html#tester._arrange_mirrors',
+                                                                                                          'fastkafka/_application/tester.py'),
                                                'fastkafka._application.tester.Tester._create_ctx': ( 'tester.html#tester._create_ctx',
                                                                                                      'fastkafka/_application/tester.py'),
+                                               'fastkafka._application.tester.Tester._create_mirrors': ( 'tester.html#tester._create_mirrors',
+                                                                                                         'fastkafka/_application/tester.py'),
                                                'fastkafka._application.tester.Tester._start_tester': ( 'tester.html#tester._start_tester',
                                                                                                        'fastkafka/_application/tester.py'),
                                                'fastkafka._application.tester.Tester._stop_tester': ( 'tester.html#tester._stop_tester',
                                                                                                       'fastkafka/_application/tester.py'),
-                                               'fastkafka._application.tester.Tester.create_mirrors': ( 'tester.html#tester.create_mirrors',
-                                                                                                        'fastkafka/_application/tester.py'),
                                                'fastkafka._application.tester.Tester.using_local_kafka': ( 'tester.html#tester.using_local_kafka',
                                                                                                            'fastkafka/_application/tester.py'),
                                                'fastkafka._application.tester.Tester.using_local_redpanda': ( 'tester.html#tester.using_local_redpanda',
                                                                                                               'fastkafka/_application/tester.py'),
+                                               'fastkafka._application.tester._get_broker_spec': ( 'tester.html#_get_broker_spec',
+                                                                                                   'fastkafka/_application/tester.py'),
                                                'fastkafka._application.tester.mirror_consumer': ( 'tester.html#mirror_consumer',
                                                                                                   'fastkafka/_application/tester.py'),
                                                'fastkafka._application.tester.mirror_producer': ( 'tester.html#mirror_producer',
-                                                                                                  'fastkafka/_application/tester.py')},
+                                                                                                  'fastkafka/_application/tester.py'),
+                                               'fastkafka._application.tester.set_sugar': ( 'tester.html#set_sugar',
+                                                                                            'fastkafka/_application/tester.py')},
             'fastkafka._components.aiokafka_consumer_loop': { 'fastkafka._components.aiokafka_consumer_loop.EventMetadata': ( 'consumerloop.html#eventmetadata',
                                                                                                                               'fastkafka/_components/aiokafka_consumer_loop.py'),
                                                               'fastkafka._components.aiokafka_consumer_loop.EventMetadata.create_event_metadata': ( 'consumerloop.html#eventmetadata.create_event_metadata',
                                                                                                                                                     'fastkafka/_components/aiokafka_consumer_loop.py'),
                                                               'fastkafka._components.aiokafka_consumer_loop._aiokafka_consumer_loop': ( 'consumerloop.html#_aiokafka_consumer_loop',
                                                                                                                                         'fastkafka/_components/aiokafka_consumer_loop.py'),
                                                               'fastkafka._components.aiokafka_consumer_loop._callback_parameters_wrapper': ( 'consumerloop.html#_callback_parameters_wrapper',
@@ -121,14 +139,18 @@
                                                                                                 'fastkafka/_components/asyncapi.py'),
                                                 'fastkafka._components.asyncapi.KafkaBroker.dict': ( 'asyncapi.html#kafkabroker.dict',
                                                                                                      'fastkafka/_components/asyncapi.py'),
                                                 'fastkafka._components.asyncapi.KafkaBroker.json': ( 'asyncapi.html#kafkabroker.json',
                                                                                                      'fastkafka/_components/asyncapi.py'),
                                                 'fastkafka._components.asyncapi.KafkaBrokers': ( 'asyncapi.html#kafkabrokers',
                                                                                                  'fastkafka/_components/asyncapi.py'),
+                                                'fastkafka._components.asyncapi.KafkaBrokers.dict': ( 'asyncapi.html#kafkabrokers.dict',
+                                                                                                      'fastkafka/_components/asyncapi.py'),
+                                                'fastkafka._components.asyncapi.KafkaBrokers.json': ( 'asyncapi.html#kafkabrokers.json',
+                                                                                                      'fastkafka/_components/asyncapi.py'),
                                                 'fastkafka._components.asyncapi.KafkaMessage': ( 'asyncapi.html#kafkamessage',
                                                                                                  'fastkafka/_components/asyncapi.py'),
                                                 'fastkafka._components.asyncapi.KafkaMessage.Config': ( 'asyncapi.html#kafkamessage.config',
                                                                                                         'fastkafka/_components/asyncapi.py'),
                                                 'fastkafka._components.asyncapi.KafkaServiceInfo': ( 'asyncapi.html#kafkaserviceinfo',
                                                                                                      'fastkafka/_components/asyncapi.py'),
                                                 'fastkafka._components.asyncapi.SecuritySchema': ( 'asyncapi.html#securityschema',
@@ -209,14 +231,16 @@
                                                                                                         'fastkafka/_components/helpers.py'),
                                                'fastkafka._components.helpers._import_from_string': ( 'internal_helpers.html#_import_from_string',
                                                                                                       'fastkafka/_components/helpers.py'),
                                                'fastkafka._components.helpers.change_dir': ( 'internal_helpers.html#change_dir',
                                                                                              'fastkafka/_components/helpers.py'),
                                                'fastkafka._components.helpers.in_notebook': ( 'internal_helpers.html#in_notebook',
                                                                                               'fastkafka/_components/helpers.py'),
+                                               'fastkafka._components.helpers.remove_suffix': ( 'internal_helpers.html#remove_suffix',
+                                                                                                'fastkafka/_components/helpers.py'),
                                                'fastkafka._components.helpers.true_after': ( 'internal_helpers.html#true_after',
                                                                                              'fastkafka/_components/helpers.py'),
                                                'fastkafka._components.helpers.unwrap_list_type': ( 'internal_helpers.html#unwrap_list_type',
                                                                                                    'fastkafka/_components/helpers.py')},
             'fastkafka._components.logger': { 'fastkafka._components.logger.cached_log': ( 'logger.html#cached_log',
                                                                                            'fastkafka/_components/logger.py'),
                                               'fastkafka._components.logger.get_default_logger_configuration': ( 'logger.html#get_default_logger_configuration',
```

### Comparing `fastkafka-0.7.0rc0/fastkafka/_server.py` & `fastkafka-0.7.0rc1/fastkafka/_server.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,87 +3,120 @@
 # %% auto 0
 __all__ = ['logger', 'ServerProcess', 'run_fastkafka_server_process', 'terminate_asyncio_process', 'run_fastkafka_server',
            'run_in_process']
 
 # %% ../nbs/021_FastKafkaServer.ipynb 1
 import asyncio
 import multiprocessing
+import platform
 import signal
 import threading
 from contextlib import contextmanager
 from typing import *
+from types import FrameType
 
 import asyncer
 import typer
 
 from ._components.helpers import _import_from_string
 from ._components.logger import get_logger
 
 # %% ../nbs/021_FastKafkaServer.ipynb 5
 logger = get_logger(__name__, level=20)
 
 # %% ../nbs/021_FastKafkaServer.ipynb 7
 class ServerProcess:
     def __init__(self, app: str, kafka_broker_name: str):
+        """
+        Represents a server process for running the FastKafka application.
+
+        Args:
+            app (str): Input in the form of 'path:app', where **path** is the path to a python file and **app** is an object of type **FastKafka**.
+            kafka_broker_name (str): The name of the Kafka broker, one of the keys of the kafka_brokers dictionary passed in the constructor of FastKafka class.
+        """
         self.app = app
         self.should_exit = False
         self.kafka_broker_name = kafka_broker_name
 
     def run(self) -> None:
+        """
+        Runs the FastKafka application server process.
+        """
         return asyncio.run(self._serve())
 
     async def _serve(self) -> None:
+        """
+        Internal method that runs the FastKafka application server.
+        """
         self._install_signal_handlers()
 
         self.application = _import_from_string(self.app)
         self.application.set_kafka_broker(self.kafka_broker_name)
 
         async with self.application:
             await self._main_loop()
 
     def _install_signal_handlers(self) -> None:
+        """
+        Installs signal handlers for handling termination signals.
+        """
         if threading.current_thread() is not threading.main_thread():
             raise RuntimeError()
 
         loop = asyncio.get_event_loop()
 
         HANDLED_SIGNALS = (
             signal.SIGINT,  # Unix signal 2. Sent by Ctrl+C.
             signal.SIGTERM,  # Unix signal 15. Sent by `kill <pid>`.
         )
 
+        def handle_windows_exit(signum: int, frame: Optional[FrameType]) -> None:
+            self.should_exit = True
+
         def handle_exit(sig: int) -> None:
             self.should_exit = True
 
         for sig in HANDLED_SIGNALS:
-            loop.add_signal_handler(sig, handle_exit, sig)
+            if platform.system() == "Windows":
+                signal.signal(sig, handle_windows_exit)
+            else:
+                loop.add_signal_handler(sig, handle_exit, sig)
 
     async def _main_loop(self) -> None:
+        """
+        Main loop for the FastKafka application server process.
+        """
         while not self.should_exit:
             await asyncio.sleep(0.1)
 
 # %% ../nbs/021_FastKafkaServer.ipynb 8
 _app = typer.Typer()
 
 
 @_app.command()
 def run_fastkafka_server_process(
     app: str = typer.Argument(
         ...,
-        help="input in the form of 'path:app', where **path** is the path to a python file and **app** is an object of type **FastKafka**.",
+        help="Input in the form of 'path:app', where **path** is the path to a python file and **app** is an object of type **FastKafka**.",
     ),
     kafka_broker: str = typer.Option(
         ...,
-        help="kafka_broker, one of the keys of the kafka_brokers dictionary passed in the constructor of FastaKafka class.",
+        help="Kafka broker, one of the keys of the kafka_brokers dictionary passed in the constructor of FastKafka class.",
     ),
 ) -> None:
     ServerProcess(app, kafka_broker).run()
 
 # %% ../nbs/021_FastKafkaServer.ipynb 10
 async def terminate_asyncio_process(p: asyncio.subprocess.Process) -> None:
+    """
+    Terminates an asyncio process.
+
+    Args:
+        p (asyncio.subprocess.Process): The process to terminate.
+    """
     logger.info(f"terminate_asyncio_process(): Terminating the process {p.pid}...")
     # Check if SIGINT already propagated to process
     try:
         await asyncio.wait_for(p.wait(), 1)
         logger.info(
             f"terminate_asyncio_process(): Process {p.pid} was already terminated."
         )
@@ -105,28 +138,44 @@
     logger.warning(f"Killing the process {p.pid}...")
     p.kill()
     await p.wait()
     logger.warning(f"terminate_asyncio_process(): Process {p.pid} killed!")
 
 # %% ../nbs/021_FastKafkaServer.ipynb 12
 async def run_fastkafka_server(num_workers: int, app: str, kafka_broker: str) -> None:
+    """
+    Runs the FastKafka server with multiple worker processes.
+
+    Args:
+        num_workers (int): Number of FastKafka instances to run.
+        app (str): Input in the form of 'path:app', where **path** is the path to a python file and **app** is an object of type **FastKafka**.
+        kafka_broker (str): Kafka broker, one of the keys of the kafka_brokers dictionary passed in the constructor of FastKafka class.
+    """
     loop = asyncio.get_event_loop()
 
     HANDLED_SIGNALS = (
         signal.SIGINT,  # Unix signal 2. Sent by Ctrl+C.
         signal.SIGTERM,  # Unix signal 15. Sent by `kill <pid>`.
     )
 
     d = {"should_exit": False}
 
+    def handle_windows_exit(
+        signum: int, frame: Optional[FrameType], d: Dict[str, bool] = d
+    ) -> None:
+        d["should_exit"] = True
+
     def handle_exit(sig: int, d: Dict[str, bool] = d) -> None:
         d["should_exit"] = True
 
     for sig in HANDLED_SIGNALS:
-        loop.add_signal_handler(sig, handle_exit, sig)
+        if platform.system() == "Windows":
+            signal.signal(sig, handle_windows_exit)
+        else:
+            loop.add_signal_handler(sig, handle_exit, sig)
 
     async with asyncer.create_task_group() as tg:
         args = [
             "run_fastkafka_server_process",
             "--kafka-broker",
             kafka_broker,
             app,
@@ -178,14 +227,23 @@
         raise typer.Exit(1)
 
 # %% ../nbs/021_FastKafkaServer.ipynb 13
 @contextmanager
 def run_in_process(
     target: Callable[..., Any]
 ) -> Generator[multiprocessing.Process, None, None]:
+    """
+    Runs the target function in a separate process.
+
+    Args:
+        target (Callable[..., Any]): The function to run in a separate process.
+
+    Yields:
+        Generator[multiprocessing.Process, None, None]: A generator that yields the process object.
+    """
     p = multiprocessing.Process(target=target)
     try:
         p.start()
         yield p
     except Exception as e:
         print(f"Exception raised {e=}")
     finally:
```

### Comparing `fastkafka-0.7.0rc0/fastkafka/_testing/apache_kafka_broker.py` & `fastkafka-0.7.0rc1/fastkafka/_testing/apache_kafka_broker.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 # %% auto 0
 __all__ = ['logger', 'get_zookeeper_config_string', 'get_kafka_config_string', 'ApacheKafkaBroker', 'run_and_match',
            'get_free_port', 'write_config_and_run']
 
 # %% ../../nbs/002_ApacheKafkaBroker.ipynb 1
 import asyncio
 import re
+import platform
 import socket
 from datetime import datetime, timedelta
+from os import environ
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import *
 
 import asyncer
 import nest_asyncio
 
@@ -42,16 +44,18 @@
     Args:
         data_dir: Path to the directory where the zookeepeer instance will save data
         zookeeper_port: Port for clients (Kafka brokes) to connect
     Returns:
         Zookeeper configuration string.
 
     """
-
-    zookeeper_config = f"""dataDir={data_dir}/zookeeper
+    zookeeper_data_dir = str((Path(data_dir) / "zookeeper").resolve())
+    if platform.system() == "Windows":
+        zookeeper_data_dir = zookeeper_data_dir.replace("\\", "/")
+    zookeeper_config = f"""dataDir={zookeeper_data_dir}
 clientPort={zookeeper_port}
 maxClientCnxns=0
 admin.enableServer=false
 """
 
     return zookeeper_config
 
@@ -66,15 +70,17 @@
         data_dir: Path to the directory where the kafka broker instance will save data
         zookeeper_port: Port on which the zookeeper instance is running
         listener_port: Port on which the clients (producers and consumers) can connect
     Returns:
         Kafka broker configuration string.
 
     """
-
+    kafka_logs_dir = str((Path(data_dir) / "kafka_logs").resolve())
+    if platform.system() == "Windows":
+        kafka_logs_dir = kafka_logs_dir.replace("\\", "/")
     kafka_config = f"""broker.id=0
 
 ############################# Socket Server Settings #############################
 
 # The address the socket server listens on. If not configured, the host name will be equal to the value of
 # java.net.InetAddress.getCanonicalHostName(), with PLAINTEXT listener name, and port 9092.
 #   FORMAT:
@@ -105,15 +111,15 @@
 # The maximum size of a request that the socket server will accept (protection against OOM)
 socket.request.max.bytes=104857600
 
 
 ############################# Log Basics #############################
 
 # A comma separated list of directories under which to store log files
-log.dirs={data_dir}/kafka_logs
+log.dirs={kafka_logs_dir}
 
 # The default number of log partitions per topic. More partitions allow greater
 # parallelism for consumption, but this will also result in more files across
 # the brokers.
 num.partitions=1
 
 # The number of threads per data directory to be used for log recovery at startup and flushing at shutdown.
@@ -291,31 +297,53 @@
 
     async def __aexit__(self, *args: Any, **kwargs: Any) -> None:
         await self._stop()
 
 # %% ../../nbs/002_ApacheKafkaBroker.ipynb 14
 @patch(cls_method=True)  # type: ignore
 def _check_deps(cls: ApacheKafkaBroker) -> None:
+    """Checks the dependencies required to run Apache KafkaBroker.
+
+    Raises:
+        RuntimeError: If JDK installation or Kafka installation is not found.
+    """
     if not check_java():
         raise RuntimeError(
             "JDK installation not found! Please install JDK manually or run 'fastkafka testing install_deps'."
         )
     if not check_kafka():
         raise RuntimeError(
             "Kafka installation not found! Please install Kafka tools manually or run 'fastkafka testing install_deps'."
         )
 
-# %% ../../nbs/002_ApacheKafkaBroker.ipynb 16
+# %% ../../nbs/002_ApacheKafkaBroker.ipynb 17
 async def run_and_match(
     *args: str,
     capture: str = "stdout",
     timeout: int = 5,
     pattern: str,
     num_to_match: int = 1,
 ) -> asyncio.subprocess.Process:
+    """Runs a command asynchronously and matches the output against a pattern.
+
+    Args:
+        *args: Command-line arguments for the subprocess.
+        capture: Which output to capture ("stdout" or "stderr").
+        timeout: Timeout in seconds for reading the output.
+        pattern: Regular expression pattern to match in the output.
+        num_to_match: Number of matches to wait for.
+
+    Returns:
+        The subprocess process object.
+
+    Raises:
+        ValueError: If the capture parameter has an unsupported value.
+        TimeoutError: If the process times out.
+        RuntimeError: If the process returns a non-zero return code.
+    """
     # Create the subprocess; redirect the standard output
     # into a pipe.
     matched = 0
     proc = await asyncio.create_subprocess_exec(
         *args,
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.PIPE,
@@ -354,26 +382,41 @@
                     f"stdout={dstdout}, stderr={dstderr}, returncode={proc.returncode}"
                 )
 
     await terminate_asyncio_process(proc)
 
     raise TimeoutError()
 
-# %% ../../nbs/002_ApacheKafkaBroker.ipynb 19
+# %% ../../nbs/002_ApacheKafkaBroker.ipynb 20
 def get_free_port() -> str:
+    """Gets a port number which is available and free in the system.
+
+    Returns:
+        The free port number as a string.
+    """
     s = socket.socket()
     s.bind(("127.0.0.1", 0))
     port = str(s.getsockname()[1])
     s.close()
     return port
 
 
 async def write_config_and_run(
     config: str, config_path: Union[str, Path], run_cmd: str
 ) -> asyncio.subprocess.Process:
+    """Writes the configuration to a file, and runs a command using the configuration.
+
+    Args:
+        config: The configuration string.
+        config_path: Path to the configuration file.
+        run_cmd: The command to run.
+
+    Returns:
+        The subprocess process object.
+    """
     with open(config_path, "w") as f:
         f.write(config)
 
     return await asyncio.create_subprocess_exec(
         run_cmd,
         config_path,
         stdout=asyncio.subprocess.PIPE,
@@ -381,23 +424,37 @@
     )
 
 
 @patch
 def get_service_config_string(
     self: ApacheKafkaBroker, service: str, *, data_dir: Path
 ) -> str:
+    """Gets the configuration string for a service.
+
+    Args:
+        service: Name of the service ("kafka" or "zookeeper").
+        data_dir: Path to the directory where the service will save data.
+
+    Returns:
+        The service configuration string.
+    """
     service_kwargs = getattr(self, f"{service}_kwargs")
     if service == "kafka":
         return get_kafka_config_string(data_dir=data_dir, **service_kwargs)
     else:
         return get_zookeeper_config_string(data_dir=data_dir, **service_kwargs)
 
 
 @patch
 async def _start_service(self: ApacheKafkaBroker, service: str = "kafka") -> None:
+    """Starts a service (kafka or zookeeper) asynchronously.
+
+    Args:
+        service: Name of the service ("kafka" or "zookeeper").
+    """
     logger.info(f"Starting {service}...")
 
     if self.temporary_directory_path is None:
         raise ValueError(
             "ApacheKafkaBroker._start_service(): self.temporary_directory_path is None, did you initialise it?"
         )
 
@@ -412,61 +469,68 @@
             f.write(
                 self.get_service_config_string(
                     service, data_dir=self.temporary_directory_path
                 )
             )
 
         try:
+            script_extension = "bat" if platform.system() == "Windows" else "sh"
+            service_start_script = f"{service}-server-start.{script_extension}"
             service_task = await run_and_match(
-                f"{service}-server-start.sh",
+                service_start_script,
                 str(service_config_path),
                 pattern="INFO \[KafkaServer id=0\] started"
                 if service == "kafka"
                 else "INFO Snapshot taken",
                 timeout=30,
             )
         except Exception as e:
             print(e)
             logger.info(
-                f"{service} startup falied, generating a new port and retrying..."
+                f"{service} startup failed, generating a new port and retrying..."
             )
             port = get_free_port()
             if service == "zookeeper":
                 self.zookeeper_kwargs["zookeeper_port"] = port
                 self.kafka_kwargs["zookeeper_port"] = port
             else:
                 self.kafka_kwargs["listener_port"] = port
 
-            logger.info(f"port={port}")
+            logger.info(f"{service} new port={port}")
         else:
             setattr(self, f"{service}_task", service_task)
             return
 
     raise ValueError(f"Could not start {service} with params: {configs_tried}")
 
 
 @patch
 async def _start_kafka(self: ApacheKafkaBroker) -> None:
+    """Starts a local Kafka broker asynchronously."""
     return await self._start_service("kafka")
 
 
 @patch
 async def _start_zookeeper(self: ApacheKafkaBroker) -> None:
+    """Starts a local ZooKeeper instance asynchronously."""
     return await self._start_service("zookeeper")
 
 
 @patch
 async def _create_topics(self: ApacheKafkaBroker) -> None:
+    """Creates missing topics in a local Kafka broker asynchronously."""
     listener_port = self.kafka_kwargs.get("listener_port", 9092)
     bootstrap_server = f"127.0.0.1:{listener_port}"
 
+    script_extension = "bat" if platform.system() == "Windows" else "sh"
+    topics_script = f"kafka-topics.{script_extension}"
     async with asyncer.create_task_group() as tg:
         processes = [
             tg.soonify(asyncio.create_subprocess_exec)(
-                "kafka-topics.sh",
+                topics_script,
                 "--create",
                 f"--topic={topic}",
                 f"--bootstrap-server={bootstrap_server}",
                 stdout=asyncio.subprocess.PIPE,
                 stdin=asyncio.subprocess.PIPE,
             )
             for topic in self.topics
@@ -480,14 +544,19 @@
             raise ValueError("Could not create missing topics!")
     except asyncio.TimeoutError as _:
         raise ValueError("Timed out while creating missing topics!")
 
 
 @patch
 async def _start(self: ApacheKafkaBroker) -> str:
+    """Starts a local Kafka broker and ZooKeeper instance asynchronously.
+
+    Returns:
+        The Kafka broker bootstrap server address in string format: host:port.
+    """
     self._check_deps()
 
     self.temporary_directory = TemporaryDirectory()
     self.temporary_directory_path = Path(self.temporary_directory.__enter__())
 
     await self._start_zookeeper()
     await self._start_kafka()
@@ -501,25 +570,27 @@
     self._is_started = True
 
     return bootstrap_server
 
 
 @patch
 async def _stop(self: ApacheKafkaBroker) -> None:
+    """Stops a local Kafka broker and ZooKeeper instance asynchronously."""
     await terminate_asyncio_process(self.kafka_task)  # type: ignore
     await terminate_asyncio_process(self.zookeeper_task)  # type: ignore
     self.temporary_directory.__exit__(None, None, None)  # type: ignore
     self._is_started = False
 
-# %% ../../nbs/002_ApacheKafkaBroker.ipynb 22
+# %% ../../nbs/002_ApacheKafkaBroker.ipynb 23
 @patch
 def start(self: ApacheKafkaBroker) -> str:
-    """Starts a local kafka broker and zookeeper instance synchronously
+    """Starts a local Kafka broker and ZooKeeper instance synchronously.
+
     Returns:
-       Kafka broker bootstrap server address in string format: add:port
+        The Kafka broker bootstrap server address in string format: host:port.
     """
     logger.info(f"{self.__class__.__name__}.start(): entering...")
     try:
         # get or create loop
         try:
             loop = asyncio.get_event_loop()
         except RuntimeError as e:
```

### Comparing `fastkafka-0.7.0rc0/fastkafka/_testing/in_memory_broker.py` & `fastkafka-0.7.0rc1/fastkafka/_testing/in_memory_broker.py`

 * *Files 23% similar despite different names*

```diff
@@ -44,19 +44,36 @@
     serialized_key_size = 0
     serialized_value_size = 0
     headers: Sequence[Tuple[str, bytes]] = field(default_factory=list)
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 7
 class KafkaPartition:
     def __init__(self, *, partition: int, topic: str):
+        """
+        Initialize a KafkaPartition object.
+
+        Args:
+            partition: The partition number.
+            topic: The topic name.
+        """
         self.partition = partition
         self.topic = topic
         self.messages: List[KafkaRecord] = list()
 
     def write(self, value: bytes, key: Optional[bytes] = None) -> RecordMetadata:  # type: ignore
+        """
+        Write a Kafka record to the partition.
+
+        Args:
+            value: The value of the record.
+            key: The key of the record.
+
+        Returns:
+            The record metadata.
+        """
         record = KafkaRecord(
             topic=self.topic,
             partition=self.partition,
             value=value,
             key=key,
             offset=len(self.messages),
         )
@@ -69,90 +86,193 @@
             timestamp_type=0,
             log_start_offset=0,
         )
         self.messages.append(record)
         return record_meta
 
     def read(self, offset: int) -> Tuple[List[KafkaRecord], int]:
+        """
+        Read Kafka records from the partition starting from the given offset.
+
+        Args:
+            offset: The starting offset.
+
+        Returns:
+            A tuple containing the list of records and the current offset.
+        """
         return self.messages[offset:], len(self.messages)
 
     def latest_offset(self) -> int:
+        """
+        Get the latest offset of the partition.
+
+        Returns:
+            The latest offset.
+        """
         return len(self.messages)
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 11
 class KafkaTopic:
     def __init__(self, topic: str, num_partitions: int = 1):
+        """
+        Initialize a KafkaTopic object.
+
+        Args:
+            topic: The topic name.
+            num_partitions: The number of partitions in the topic (default: 1).
+        """
         self.topic = topic
         self.num_partitions = num_partitions
         self.partitions: List[KafkaPartition] = [
             KafkaPartition(topic=topic, partition=partition_index)
             for partition_index in range(num_partitions)
         ]
 
     def read(  # type: ignore
         self, partition: int, offset: int
     ) -> Tuple[TopicPartition, List[KafkaRecord], int]:
+        """
+        Read records from the specified partition and offset.
+
+        Args:
+            partition: The partition index.
+            offset: The offset from which to start reading.
+
+        Returns:
+            A tuple containing the topic partition, list of Kafka records, and the new offset.
+        """
         topic_partition = TopicPartition(topic=self.topic, partition=partition)
         records, offset = self.partitions[partition].read(offset)
         return topic_partition, records, offset
 
     def write_with_partition(  # type: ignore
         self,
         value: bytes,
         partition: int,
     ) -> RecordMetadata:
+        """
+        Write a record with a specified partition.
+
+        Args:
+            value: The value of the record.
+            partition: The partition to write the record to.
+
+        Returns:
+            The metadata of the written record.
+        """
         return self.partitions[partition].write(value)
 
     def write_with_key(self, value: bytes, key: bytes) -> RecordMetadata:  # type: ignore
+        """
+        Write a record with a specified key.
+
+        Args:
+            value: The value of the record.
+            key: The key of the record.
+
+        Returns:
+            The metadata of the written record.
+        """
         partition = int(hashlib.sha256(key).hexdigest(), 16) % self.num_partitions
         return self.partitions[partition].write(value, key=key)
 
     def write(  # type: ignore
         self,
         value: bytes,
         *,
         key: Optional[bytes] = None,
         partition: Optional[int] = None,
     ) -> RecordMetadata:
+        """
+        Write a record to the topic.
+
+        Args:
+            value: The value of the record.
+            key: The key of the record (optional).
+            partition: The partition to write the record to (optional).
+
+        Returns:
+            The metadata of the written record.
+        """
         if partition is not None:
             return self.write_with_partition(value, partition)
 
         if key is not None:
             return self.write_with_key(value, key)
 
         partition = random.randint(0, self.num_partitions - 1)  # nosec
         return self.write_with_partition(value, partition)
 
     def latest_offset(self, partition: int) -> int:
+        """
+        Get the latest offset of a partition.
+
+        Args:
+            partition: The partition index.
+
+        Returns:
+            The latest offset of the partition.
+        """
         return self.partitions[partition].latest_offset()
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 17
 def split_list(list_to_split: List[Any], split_size: int) -> List[List[Any]]:
+    """
+    Split a list into smaller lists of a specified size.
+
+    Args:
+        list_to_split: The list to split.
+        split_size: The size of each split.
+
+    Returns:
+        A list of smaller lists.
+    """
     return [
         list_to_split[start_index : start_index + split_size]
         for start_index in range(0, len(list_to_split), split_size)
     ]
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 19
 class GroupMetadata:
     def __init__(self, num_partitions: int):
+        """
+        Initialize a GroupMetadata object.
+
+        Args:
+            num_partitions: The number of partitions in the group.
+        """
         self.num_partitions = num_partitions
         self.partitions_offsets: Dict[int, int] = {}
         self.consumer_ids: List[uuid.UUID] = list()
         self.partition_assignments: Dict[uuid.UUID, List[int]] = {}
 
     def subscribe(self, consumer_id: uuid.UUID) -> None:
+        """
+        Subscribe a consumer to the group.
+
+        Args:
+            consumer_id: The ID of the consumer.
+        """
         self.consumer_ids.append(consumer_id)
         self.rebalance()
 
     def unsubscribe(self, consumer_id: uuid.UUID) -> None:
+        """
+        Unsubscribe a consumer from the group.
+
+        Args:
+            consumer_id: The ID of the consumer.
+        """
         self.consumer_ids.remove(consumer_id)
         self.rebalance()
 
     def rebalance(self) -> None:
+        """
+        Rebalance the group's partition assignments.
+        """
         if len(self.consumer_ids) == 0:
             self.partition_assignments = {}
         else:
             partitions_per_actor = self.num_partitions // len(self.consumer_ids)
             if self.num_partitions % len(self.consumer_ids) != 0:
                 partitions_per_actor += 1
             self.assign_partitions(partitions_per_actor)
@@ -165,22 +285,38 @@
             self.consumer_ids[i]: partition_split
             for i, partition_split in enumerate(partitions_split)
         }
 
     def get_partitions(
         self, consumer_id: uuid.UUID
     ) -> Tuple[List[int], Dict[int, Optional[int]]]:
+        """
+        Get the partition assignments and offsets for a consumer.
+
+        Args:
+            consumer_id: The ID of the consumer.
+
+        Returns:
+            A tuple containing the partition assignments and offsets.
+        """
         partition_assignments = self.partition_assignments.get(consumer_id, [])
         partition_offsets_assignments = {
             partition: self.partitions_offsets.get(partition, None)
             for partition in partition_assignments
         }
         return partition_assignments, partition_offsets_assignments
 
     def set_offset(self, partition: int, offset: int) -> None:
+        """
+        Set the offset for a partition.
+
+        Args:
+            partition: The partition index.
+            offset: The offset to set.
+        """
         self.partitions_offsets[partition] = offset
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 22
 @classcontextmanager()
 class InMemoryBroker:
     def __init__(
         self,
@@ -191,14 +327,20 @@
         self.topic_groups: Dict[Tuple[str, str, str], GroupMetadata] = {}
         self.is_started: bool = False
 
     def connect(self) -> uuid.UUID:
         return uuid.uuid4()
 
     def dissconnect(self, consumer_id: uuid.UUID) -> None:
+        """
+        Disconnect a consumer from the broker.
+
+        Args:
+            consumer_id: The ID of the consumer.
+        """
         pass
 
     def subscribe(
         self, bootstrap_server: str, topic: str, group: str, consumer_id: uuid.UUID
     ) -> None:
         raise NotImplementedError()
 
@@ -227,34 +369,58 @@
         key: Optional[bytes] = None,
         partition: Optional[int] = None,
     ) -> RecordMetadata:
         raise NotImplementedError()
 
     @contextmanager
     def lifecycle(self) -> Iterator["InMemoryBroker"]:
+        """
+        Context manager for the lifecycle of the in-memory broker.
+
+        Yields:
+            An instance of the in-memory broker.
+        """
         raise NotImplementedError()
 
     async def _start(self) -> str:
+        """
+        Start the in-memory broker.
+
+        Returns:
+            The address of the broker.
+        """
         logger.info("InMemoryBroker._start() called")
         self.__enter__()  # type: ignore
         return "localbroker:0"
 
     async def _stop(self) -> None:
+        """
+        Stop the in-memory broker.
+        """
         logger.info("InMemoryBroker._stop() called")
         self.__exit__(None, None, None)  # type: ignore
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 23
 @patch
 def subscribe(
     self: InMemoryBroker,
     bootstrap_server: str,
     topic: str,
     group: str,
     consumer_id: uuid.UUID,
 ) -> None:
+    """
+    Subscribe a consumer to a topic group.
+
+    Args:
+        bootstrap_server: The bootstrap server address.
+        topic: The topic to subscribe to.
+        group: The group to join.
+        consumer_id: The ID of the consumer.
+    """
     if (bootstrap_server, topic) not in self.topics:
         self.topics[(bootstrap_server, topic)] = KafkaTopic(
             topic=topic, num_partitions=self.num_partitions
         )
 
     group_meta = self.topic_groups.get(
         (bootstrap_server, topic, group), GroupMetadata(self.num_partitions)
@@ -267,27 +433,49 @@
 def unsubscribe(
     self: InMemoryBroker,
     bootstrap_server: str,
     topic: str,
     group: str,
     consumer_id: uuid.UUID,
 ) -> None:
+    """
+    Unsubscribe a consumer from a topic group.
+
+    Args:
+        bootstrap_server: The bootstrap server address.
+        topic: The topic to unsubscribe from.
+        group: The group to leave.
+        consumer_id: The ID of the consumer.
+    """
     self.topic_groups[(bootstrap_server, topic, group)].unsubscribe(consumer_id)
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 25
 @patch
 def write(  # type: ignore
     self: InMemoryBroker,
     *,
     bootstrap_server: str,
     topic: str,
     value: bytes,
     key: Optional[bytes] = None,
     partition: Optional[int] = None,
 ) -> RecordMetadata:
+    """
+    Write a message to a topic.
+
+    Args:
+        bootstrap_server: The bootstrap server address.
+        topic: The topic to write the message to.
+        value: The value of the message.
+        key: The key associated with the message.
+        partition: The partition ID to write the message to.
+
+    Returns:
+        The metadata of the written message.
+    """
     if (bootstrap_server, topic) not in self.topics:
         self.topics[(bootstrap_server, topic)] = KafkaTopic(
             topic=topic, num_partitions=self.num_partitions
         )
 
     return self.topics[(bootstrap_server, topic)].write(
         value, key=key, partition=partition
@@ -300,14 +488,27 @@
     *,
     bootstrap_server: str,
     topic: str,
     group: str,
     consumer_id: uuid.UUID,
     auto_offset_reset: str,
 ) -> Dict[TopicPartition, List[KafkaRecord]]:
+    """
+    Read messages from a topic group.
+
+    Args:
+        bootstrap_server: The bootstrap server address.
+        topic: The topic to read messages from.
+        group: The group to read messages for.
+        consumer_id: The ID of the consumer.
+        auto_offset_reset: The strategy to use when the consumer does not have a valid offset for the group.
+
+    Returns:
+        A dictionary containing the messages retrieved from each topic partition.
+    """
     group_meta = self.topic_groups[(bootstrap_server, topic, group)]
     partitions, offsets = group_meta.get_partitions(consumer_id)
 
     if len(partitions) == 0:
         return {}
 
     partitions_data = {}
@@ -346,15 +547,20 @@
         self._bootstrap_servers = ""
 
     @delegates(AIOKafkaConsumer)
     def __call__(self, **kwargs: Any) -> "InMemoryConsumer":
         defaults = _get_default_kwargs_from_sig(InMemoryConsumer.__call__, **kwargs)
         consume_copy = InMemoryConsumer(self.broker)
         consume_copy._auto_offset_reset = defaults["auto_offset_reset"]
-        consume_copy._bootstrap_servers = defaults["bootstrap_servers"]
+        consume_copy._bootstrap_servers = (
+            "".join(defaults["bootstrap_servers"])
+            if isinstance(defaults["bootstrap_servers"], list)
+            else defaults["bootstrap_servers"]
+        )
+
         consume_copy._group_id = (
             defaults["group_id"]
             if defaults["group_id"] is not None
             else "".join(random.choices(string.ascii_letters, k=10))  # nosec
         )
         return consume_copy
 
@@ -376,25 +582,40 @@
     ) -> Dict[TopicPartition, List[ConsumerRecord]]:
         raise NotImplementedError()
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 37
 @patch
 @delegates(AIOKafkaConsumer.start)
 async def start(self: InMemoryConsumer, **kwargs: Any) -> None:
+    """
+    Start consuming messages from the connected broker.
+
+    Raises:
+        RuntimeError: If start() has already been called without calling stop() first.
+    """
     logger.info("AIOKafkaConsumer patched start() called()")
     if self._id is not None:
         raise RuntimeError(
             "Consumer start() already called! Run consumer stop() before running start() again"
         )
     self._id = self.broker.connect()
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 40
 @patch  # type: ignore
 @delegates(AIOKafkaConsumer.subscribe)
 def subscribe(self: InMemoryConsumer, topics: List[str], **kwargs: Any) -> None:
+    """
+    Subscribe to a list of topics for consuming messages.
+
+    Args:
+        topics: A list of topics to subscribe to.
+
+    Raises:
+        RuntimeError: If start() has not been called before calling subscribe().
+    """
     logger.info("AIOKafkaConsumer patched subscribe() called")
     if self._id is None:
         raise RuntimeError("Consumer start() not called! Run consumer start() first")
     logger.info(f"AIOKafkaConsumer.subscribe(), subscribing to: {topics}")
     for topic in topics:
         self.broker.subscribe(
             bootstrap_server=self._bootstrap_servers,
@@ -404,14 +625,20 @@
         )
         self._topics.append(topic)
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 43
 @patch
 @delegates(AIOKafkaConsumer.stop)
 async def stop(self: InMemoryConsumer, **kwargs: Any) -> None:
+    """
+    Stop consuming messages from the connected broker.
+
+    Raises:
+        RuntimeError: If start() has not been called before calling stop().
+    """
     logger.info("AIOKafkaConsumer patched stop() called")
     if self._id is None:
         raise RuntimeError("Consumer start() not called! Run consumer start() first")
     for topic in self._topics:
         self.broker.unsubscribe(
             bootstrap_server=self._bootstrap_servers,
             topic=topic,
@@ -421,14 +648,23 @@
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 46
 @patch
 @delegates(AIOKafkaConsumer.getmany)
 async def getmany(  # type: ignore
     self: InMemoryConsumer, **kwargs: Any
 ) -> Dict[TopicPartition, List[ConsumerRecord]]:
+    """
+    Retrieve messages from the subscribed topics.
+
+    Returns:
+        A dictionary containing the retrieved messages from each topic partition.
+
+    Raises:
+        RuntimeError: If start() has not been called before calling getmany().
+    """
     await asyncio.sleep(0)
     for topic in self._topics:
         return self.broker.read(
             bootstrap_server=self._bootstrap_servers,
             topic=topic,
             consumer_id=self._id,  # type: ignore
             group=self._group_id,  # type: ignore
@@ -442,15 +678,19 @@
         self.id: Optional[uuid.UUID] = None
         self._bootstrap_servers = ""
 
     @delegates(AIOKafkaProducer)
     def __call__(self, **kwargs: Any) -> "InMemoryProducer":
         defaults = _get_default_kwargs_from_sig(InMemoryConsumer.__call__, **kwargs)
         producer_copy = InMemoryProducer(self.broker)
-        producer_copy._bootstrap_servers = defaults["bootstrap_servers"]
+        producer_copy._bootstrap_servers = (
+            "".join(defaults["bootstrap_servers"])
+            if isinstance(defaults["bootstrap_servers"], list)
+            else defaults["bootstrap_servers"]
+        )
         return producer_copy
 
     @delegates(AIOKafkaProducer.start)
     async def start(self, **kwargs: Any) -> None:
         raise NotImplementedError()
 
     @delegates(AIOKafkaProducer.stop)
@@ -485,25 +725,37 @@
     async def send_batch(self, batch: "MockBatch", topic: str, partition: Any) -> None:
         raise NotImplementedError()
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 52
 @patch  # type: ignore
 @delegates(AIOKafkaProducer.start)
 async def start(self: InMemoryProducer, **kwargs: Any) -> None:
+    """
+    Start the in-memory producer.
+
+    Raises:
+        RuntimeError: If start() has already been called without calling stop() first.
+    """
     logger.info("AIOKafkaProducer patched start() called()")
     if self.id is not None:
         raise RuntimeError(
             "Producer start() already called! Run producer stop() before running start() again"
         )
     self.id = self.broker.connect()
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 55
 @patch  # type: ignore
 @delegates(AIOKafkaProducer.stop)
 async def stop(self: InMemoryProducer, **kwargs: Any) -> None:
+    """
+    Stop the in-memory producer.
+
+    Raises:
+        RuntimeError: If start() has not been called before calling stop().
+    """
     logger.info("AIOKafkaProducer patched stop() called")
     if self.id is None:
         raise RuntimeError("Producer start() not called! Run producer start() first")
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 58
 @patch
 @delegates(AIOKafkaProducer.send)
@@ -511,14 +763,30 @@
     self: InMemoryProducer,
     topic: str,
     msg: bytes,
     key: Optional[bytes] = None,
     partition: Optional[int] = None,
     **kwargs: Any,
 ):  # asyncio.Task[RecordMetadata]
+    """
+    Send a message to the specified topic.
+
+    Args:
+        topic: The topic to send the message to.
+        msg: The message to send.
+        key: The key associated with the message (optional).
+        partition: The partition to send the message to (optional).
+        **kwargs: Additional arguments to be passed to AIOKafkaProducer.send().
+
+    Returns:
+        A task that resolves to the RecordMetadata of the sent message.
+
+    Raises:
+        RuntimeError: If start() has not been called before calling send().
+    """
     if self.id is None:
         raise RuntimeError("Producer start() not called! Run producer start() first")
 
     record = self.broker.write(
         bootstrap_server=self._bootstrap_servers,
         topic=topic,
         value=msg,
@@ -531,38 +799,71 @@
 
     return asyncio.create_task(_f())
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 60
 @patch
 @delegates(AIOKafkaProducer.partitions_for)
 async def partitions_for(self: InMemoryProducer, topic: str) -> List[int]:
+    """
+    Retrieve the list of partitions for the specified topic.
+
+    Args:
+        topic: The topic to get the partitions for.
+
+    Returns:
+        A list of partition IDs.
+    """
     return [i for i in range(self.broker.num_partitions)]
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 62
 @patch
 @delegates(AIOKafkaProducer._partition)
 def _partition(
     self: InMemoryProducer,
     topic: str,
     arg1: Any,
     arg2: Any,
     arg3: Any,
     key: bytes,
     arg4: Any,
 ) -> int:
+    """
+    Determine the partition to which the message should be sent.
+
+    Args:
+        topic: The topic to send the message to.
+        arg1, arg2, arg3, arg4: Additional arguments passed to the original AIOKafkaProducer._partition().
+
+    Returns:
+        The partition ID.
+    """
     return int(hashlib.sha256(key).hexdigest(), 16) % self.broker.num_partitions
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 64
 class MockBatch:
     def __init__(self) -> None:
+        """
+        Initialize an instance of MockBatch.
+        """
         self._batch: List[Tuple] = list()
 
     def append(  # type: ignore
         self, key: Optional[bytes], value: bytes, timestamp: int
     ) -> RecordMetadata:
+        """
+        Append a message to the batch.
+
+        Args:
+            key: The key associated with the message (optional).
+            value: The value of the message.
+            timestamp: The timestamp of the message.
+
+        Returns:
+            The RecordMetadata of the appended message.
+        """
         self._batch.append((key, value))
         return RecordMetadata(
             topic="",
             partition=0,
             topic_partition=None,
             offset=0,
             timestamp=timestamp,
@@ -570,35 +871,55 @@
             log_start_offset=0,
         )
 
 
 @patch
 @delegates(AIOKafkaProducer.create_batch)
 def create_batch(self: InMemoryProducer) -> "MockBatch":
+    """
+    Create a mock batch for the in-memory producer.
+
+    Returns:
+        A MockBatch instance.
+    """
     return MockBatch()
 
 
 @patch
 @delegates(AIOKafkaProducer.send_batch)
 async def send_batch(
     self: InMemoryProducer, batch: "MockBatch", topic: str, partition: Any
 ) -> None:
+    """
+    Send a batch of messages to the specified topic and partition.
+
+    Args:
+        batch: The MockBatch containing the messages to send.
+        topic: The topic to send the batch of messages to.
+        partition: The partition to send the batch of messages to.
+    """
     for record in batch._batch:
         self.broker.write(
             bootstrap_server=self._bootstrap_servers,
             topic=topic,
             value=record[1],
             key=record[0],
             partition=partition,
         )
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 68
 @patch
 @contextmanager
 def lifecycle(self: InMemoryBroker) -> Iterator[InMemoryBroker]:
+    """
+    Context manager for the lifecycle of the in-memory broker.
+
+    Yields:
+        An instance of the in-memory broker.
+    """
     logger.info(
         "InMemoryBroker._patch_consumers_and_producers(): Patching consumers and producers!"
     )
     try:
         logger.info("InMemoryBroker starting")
 
         old_consumer_app = fastkafka._application.app.AIOKafkaConsumer
```

### Comparing `fastkafka-0.7.0rc0/fastkafka/_testing/local_redpanda_broker.py` & `fastkafka-0.7.0rc1/fastkafka/_testing/local_redpanda_broker.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc0/fastkafka/_testing/test_utils.py` & `fastkafka-0.7.0rc1/fastkafka/_testing/test_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -63,24 +63,28 @@
     script_file: Optional[str] = None,
     cmd: Optional[str] = None,
     cancel_after: int = 10,
     app_name: str = "app",
     kafka_app_name: str = "kafka_app",
     generate_docs: bool = False,
 ) -> Tuple[int, bytes]:
-    """Run script and cancel after predefined time
+    """
+    Runs a script and cancels it after a predefined time.
 
     Args:
-        script: a python source code to be executed in a separate subprocess
-        script_file: name of the script where script source will be saved
-        cmd: command to execute. If None, it will be set to 'python3 -m {Path(script_file).stem}'
-        cancel_after: number of seconds before sending SIGTERM signal
+        script: A python source code to be executed in a separate subprocess.
+        script_file: Name of the script where script source will be saved.
+        cmd: Command to execute. If None, it will be set to 'python3 -m {Path(script_file).stem}'.
+        cancel_after: Number of seconds before sending SIGTERM signal.
+        app_name: Name of the app.
+        kafka_app_name: Name of the Kafka app.
+        generate_docs: Flag indicating whether to generate docs.
 
     Returns:
-        A tuple containing exit code and combined stdout and stderr as a binary string
+        A tuple containing the exit code and combined stdout and stderr as a binary string.
     """
     if script_file is None:
         script_file = "script.py"
 
     if cmd is None:
         cmd = f"python3 -m {Path(script_file).stem}"
 
@@ -111,14 +115,24 @@
         proc.terminate()
         output, _ = proc.communicate()
 
         return (proc.returncode, output)
 
 # %% ../../nbs/004_Test_Utils.ipynb 14
 async def display_docs(docs_path: str, port: int = 4000) -> None:
+    """
+    Serves the documentation using an HTTP server.
+
+    Args:
+        docs_path: Path to the documentation.
+        port: Port number for the HTTP server. Defaults to 4000.
+
+    Returns:
+        None
+    """
     with change_dir(docs_path):
         process = await asyncio.create_subprocess_exec(
             "python3",
             "-m",
             "http.server",
             f"{port}",
             stdout=asyncio.subprocess.PIPE,
```

### Comparing `fastkafka-0.7.0rc0/fastkafka/encoder.py` & `fastkafka-0.7.0rc1/fastkafka/encoder.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc0/fastkafka/testing.py` & `fastkafka-0.7.0rc1/fastkafka/testing.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc0/fastkafka.egg-info/SOURCES.txt` & `fastkafka-0.7.0rc1/fastkafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc0/settings.ini` & `fastkafka-0.7.0rc1/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = fastkafka
 lib_name = %(repo)s
-version = 0.7.0rc0
+version = 0.7.0rc1
 min_python = 3.8
 license = apache2
 
 
 ### nbdev ###
 doc_path = _docs
 lib_path = fastkafka
```

### Comparing `fastkafka-0.7.0rc0/setup.py` & `fastkafka-0.7.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     "anyio>=3.0",
     "aiokafka>=0.8.0",
     "asyncer>=0.0.2",
     "tqdm>=4.62",
     "docstring-parser>=0.15",
     "typer>=0.7.0",
     "nest-asyncio>=1.5.6",
+    "psutil>=5.9.5;platform_system=='Windows'",
 ]
 avro_requirements = [
     "fastavro>=1.7.3"
 ]
 test_requirements = [
     "install-jdk==0.3.0",
     "ipywidgets>=8.0,<=8.0.4",
```

