# Comparing `tmp/spine_engine-0.21.0.tar.gz` & `tmp/spine_engine-0.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spine_engine-0.21.0.tar", last modified: Fri Mar 24 10:33:04 2023, max compression
+gzip compressed data, was "spine_engine-0.22.0.tar", last modified: Wed May 31 12:35:46 2023, max compression
```

## Comparing `spine_engine-0.21.0.tar` & `spine_engine-0.22.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 10:33:04.441169 spine_engine-0.21.0/
--rw-rw-rw-   0        0        0    35823 2022-10-07 09:11:46.000000 spine_engine-0.21.0/COPYING
--rw-rw-rw-   0        0        0     7815 2022-10-07 09:11:46.000000 spine_engine-0.21.0/COPYING.LESSER
--rw-rw-rw-   0        0        0     2851 2023-03-24 10:33:04.441169 spine_engine-0.21.0/PKG-INFO
--rw-rw-rw-   0        0        0     1938 2023-01-24 14:04:25.000000 spine_engine-0.21.0/README.md
--rw-rw-rw-   0        0        0       84 2022-10-07 09:11:46.000000 spine_engine-0.21.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-24 10:33:04.441169 spine_engine-0.21.0/setup.cfg
--rw-rw-rw-   0        0        0     2792 2023-01-24 08:36:40.000000 spine_engine-0.21.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-24 10:33:03.957922 spine_engine-0.21.0/spine_engine/
--rw-rw-rw-   0        0        0     1143 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/__init__.py
--rw-rw-rw-   0        0        0     1875 2023-02-15 13:10:53.000000 spine_engine-0.21.0/spine_engine/config.py
--rw-rw-rw-   0        0        0     1294 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/exception.py
-drwxrwxrwx   0        0        0        0 2023-03-24 10:33:04.091274 spine_engine-0.21.0/spine_engine/execution_managers/
--rw-rw-rw-   0        0        0      977 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/execution_managers/__init__.py
--rw-rw-rw-   0        0        0    17413 2023-03-10 11:07:33.000000 spine_engine-0.21.0/spine_engine/execution_managers/conda_kernel_spec_manager.py
--rw-rw-rw-   0        0        0     1882 2022-10-07 09:11:46.000000 spine_engine-0.21.0/spine_engine/execution_managers/conda_kernel_spec_runner.py
--rw-rw-rw-   0        0        0     1675 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/execution_managers/execution_manager_base.py
--rw-rw-rw-   0        0        0    10162 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/execution_managers/kernel_execution_manager.py
--rw-rw-rw-   0        0        0    30489 2023-03-15 13:29:29.000000 spine_engine-0.21.0/spine_engine/execution_managers/persistent_execution_manager.py
--rw-rw-rw-   0        0        0     3594 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/execution_managers/process_execution_manager.py
--rw-rw-rw-   0        0        0     3355 2022-10-07 09:11:46.000000 spine_engine-0.21.0/spine_engine/execution_managers/spine_repl.jl
--rw-rw-rw-   0        0        0     3850 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/execution_managers/spine_repl.py
--rw-rw-rw-   0        0        0     3393 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/load_project_items.py
-drwxrwxrwx   0        0        0        0 2023-03-24 10:33:04.140964 spine_engine-0.21.0/spine_engine/multithread_executor/
--rw-rw-rw-   0        0        0      977 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/multithread_executor/__init__.py
--rw-rw-rw-   0        0        0     2727 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/multithread_executor/executor.py
--rw-rw-rw-   0        0        0    16685 2023-03-10 11:07:33.000000 spine_engine-0.21.0/spine_engine/multithread_executor/multithread.py
--rw-rw-rw-   0        0        0     4196 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/multithread_executor/thread_executor.py
-drwxrwxrwx   0        0        0        0 2023-03-24 10:33:04.207885 spine_engine-0.21.0/spine_engine/project_item/
--rw-rw-rw-   0        0        0     1096 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/project_item/__init__.py
--rw-rw-rw-   0        0        0    26399 2023-02-15 13:10:53.000000 spine_engine-0.21.0/spine_engine/project_item/connection.py
--rw-rw-rw-   0        0        0     9040 2023-01-13 07:06:05.000000 spine_engine-0.21.0/spine_engine/project_item/executable_item_base.py
--rw-rw-rw-   0        0        0     1536 2023-02-06 07:38:36.000000 spine_engine-0.21.0/spine_engine/project_item/project_item_info.py
--rw-rw-rw-   0        0        0    14440 2023-03-08 11:18:08.000000 spine_engine-0.21.0/spine_engine/project_item/project_item_resource.py
--rw-rw-rw-   0        0        0     4447 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/project_item/project_item_specification.py
--rw-rw-rw-   0        0        0     1805 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/project_item/project_item_specification_factory.py
--rw-rw-rw-   0        0        0     2934 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/project_item_loader.py
-drwxrwxrwx   0        0        0        0 2023-03-24 10:33:04.307911 spine_engine-0.21.0/spine_engine/server/
--rw-rw-rw-   0        0        0     1132 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/server/__init__.py
--rw-rw-rw-   0        0        0     3551 2023-03-10 11:07:33.000000 spine_engine-0.21.0/spine_engine/server/certificate_creator.py
--rw-rw-rw-   0        0        0    19446 2022-11-18 09:21:11.000000 spine_engine-0.21.0/spine_engine/server/engine_server.py
--rw-rw-rw-   0        0        0     4545 2023-03-15 13:29:29.000000 spine_engine-0.21.0/spine_engine/server/persistent_execution_service.py
--rw-rw-rw-   0        0        0     2208 2022-11-08 06:30:00.000000 spine_engine-0.21.0/spine_engine/server/ping_service.py
--rw-rw-rw-   0        0        0     5795 2022-11-08 06:30:00.000000 spine_engine-0.21.0/spine_engine/server/project_extractor_service.py
--rw-rw-rw-   0        0        0     2682 2022-11-18 09:21:11.000000 spine_engine-0.21.0/spine_engine/server/project_remover_service.py
--rw-rw-rw-   0        0        0     3865 2022-11-08 06:30:00.000000 spine_engine-0.21.0/spine_engine/server/project_retriever_service.py
--rw-rw-rw-   0        0        0    12444 2023-03-10 11:07:33.000000 spine_engine-0.21.0/spine_engine/server/remote_execution_service.py
--rw-rw-rw-   0        0        0     5830 2023-03-10 11:07:33.000000 spine_engine-0.21.0/spine_engine/server/request.py
--rw-rw-rw-   0        0        0     1734 2022-11-08 06:30:00.000000 spine_engine-0.21.0/spine_engine/server/service_base.py
--rw-rw-rw-   0        0        0     2508 2022-11-08 06:30:00.000000 spine_engine-0.21.0/spine_engine/server/start_server.py
-drwxrwxrwx   0        0        0        0 2023-03-24 10:33:04.357680 spine_engine-0.21.0/spine_engine/server/util/
--rw-rw-rw-   0        0        0     1148 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/server/util/__init__.py
--rw-rw-rw-   0        0        0     6414 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/server/util/event_data_converter.py
--rw-rw-rw-   0        0        0     5438 2022-11-08 06:30:00.000000 spine_engine-0.21.0/spine_engine/server/util/server_message.py
--rw-rw-rw-   0        0        0     3676 2023-03-10 11:07:33.000000 spine_engine-0.21.0/spine_engine/server/util/zip_handler.py
--rw-rw-rw-   0        0        0     1722 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/shared_memory_io_manager.py
--rw-rw-rw-   0        0        0    40214 2023-03-10 11:07:33.000000 spine_engine-0.21.0/spine_engine/spine_engine.py
-drwxrwxrwx   0        0        0        0 2023-03-24 10:33:04.407963 spine_engine-0.21.0/spine_engine/utils/
--rw-rw-rw-   0        0        0      977 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/utils/__init__.py
--rw-rw-rw-   0        0        0     2115 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/utils/command_line_arguments.py
--rw-rw-rw-   0        0        0     3782 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/utils/execution_resources.py
--rw-rw-rw-   0        0        0    11260 2023-03-01 14:44:57.000000 spine_engine-0.21.0/spine_engine/utils/helpers.py
--rw-rw-rw-   0        0        0     5444 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/utils/queue_logger.py
--rw-rw-rw-   0        0        0     3923 2022-11-03 13:43:21.000000 spine_engine-0.21.0/spine_engine/utils/returning_process.py
--rw-rw-rw-   0        0        0     5154 2023-03-10 11:07:33.000000 spine_engine-0.21.0/spine_engine/utils/serialization.py
--rw-rw-rw-   0        0        0     1001 2023-03-24 10:32:58.000000 spine_engine-0.21.0/spine_engine/version.py
-drwxrwxrwx   0        0        0        0 2023-03-24 10:33:03.991217 spine_engine-0.21.0/spine_engine.egg-info/
--rw-rw-rw-   0        0        0     2851 2023-03-24 10:33:03.000000 spine_engine-0.21.0/spine_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2533 2023-03-24 10:33:03.000000 spine_engine-0.21.0/spine_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 10:33:03.000000 spine_engine-0.21.0/spine_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-10-07 10:28:55.000000 spine_engine-0.21.0/spine_engine.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      147 2023-03-24 10:33:03.000000 spine_engine-0.21.0/spine_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-24 10:33:03.000000 spine_engine-0.21.0/spine_engine.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-24 10:33:04.441169 spine_engine-0.21.0/tests/
--rw-rw-rw-   0        0        0     2393 2022-11-03 13:43:21.000000 spine_engine-0.21.0/tests/test_load_project_items.py
--rw-rw-rw-   0        0        0    51405 2023-03-01 14:44:57.000000 spine_engine-0.21.0/tests/test_spine_engine.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:35:46.832330 spine_engine-0.22.0/
+-rw-rw-rw-   0        0        0    35823 2022-10-07 09:11:46.000000 spine_engine-0.22.0/COPYING
+-rw-rw-rw-   0        0        0     7815 2022-10-07 09:11:46.000000 spine_engine-0.22.0/COPYING.LESSER
+-rw-rw-rw-   0        0        0     2552 2023-05-31 12:35:46.831332 spine_engine-0.22.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1938 2023-01-24 14:04:25.000000 spine_engine-0.22.0/README.md
+-rw-rw-rw-   0        0        0       84 2022-10-07 09:11:46.000000 spine_engine-0.22.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 12:35:46.832330 spine_engine-0.22.0/setup.cfg
+-rw-rw-rw-   0        0        0     2745 2023-05-31 12:33:27.000000 spine_engine-0.22.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:35:46.318624 spine_engine-0.22.0/spine_engine/
+-rw-rw-rw-   0        0        0     1143 2022-11-03 13:43:21.000000 spine_engine-0.22.0/spine_engine/__init__.py
+-rw-rw-rw-   0        0        0     1826 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/config.py
+-rw-rw-rw-   0        0        0     1244 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/exception.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:35:46.438029 spine_engine-0.22.0/spine_engine/execution_managers/
+-rw-rw-rw-   0        0        0      977 2022-11-03 13:43:21.000000 spine_engine-0.22.0/spine_engine/execution_managers/__init__.py
+-rw-rw-rw-   0        0        0    17413 2023-03-10 11:07:33.000000 spine_engine-0.22.0/spine_engine/execution_managers/conda_kernel_spec_manager.py
+-rw-rw-rw-   0        0        0     1882 2022-10-07 09:11:46.000000 spine_engine-0.22.0/spine_engine/execution_managers/conda_kernel_spec_runner.py
+-rw-rw-rw-   0        0        0     1628 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/execution_managers/execution_manager_base.py
+-rw-rw-rw-   0        0        0    13433 2023-05-02 10:55:41.000000 spine_engine-0.22.0/spine_engine/execution_managers/kernel_execution_manager.py
+-rw-rw-rw-   0        0        0    30972 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/execution_managers/persistent_execution_manager.py
+-rw-rw-rw-   0        0        0     3547 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/execution_managers/process_execution_manager.py
+-rw-rw-rw-   0        0        0     3355 2022-10-07 09:11:46.000000 spine_engine-0.22.0/spine_engine/execution_managers/spine_repl.jl
+-rw-rw-rw-   0        0        0     3850 2022-11-03 13:43:21.000000 spine_engine-0.22.0/spine_engine/execution_managers/spine_repl.py
+-rw-rw-rw-   0        0        0     3345 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/load_project_items.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:35:46.472496 spine_engine-0.22.0/spine_engine/multithread_executor/
+-rw-rw-rw-   0        0        0      977 2022-11-03 13:43:21.000000 spine_engine-0.22.0/spine_engine/multithread_executor/__init__.py
+-rw-rw-rw-   0        0        0     2682 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/multithread_executor/executor.py
+-rw-rw-rw-   0        0        0    16640 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/multithread_executor/multithread.py
+-rw-rw-rw-   0        0        0     4196 2022-11-03 13:43:21.000000 spine_engine-0.22.0/spine_engine/multithread_executor/thread_executor.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:35:46.556216 spine_engine-0.22.0/spine_engine/project_item/
+-rw-rw-rw-   0        0        0     1049 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/project_item/__init__.py
+-rw-rw-rw-   0        0        0    26349 2023-05-22 08:51:20.000000 spine_engine-0.22.0/spine_engine/project_item/connection.py
+-rw-rw-rw-   0        0        0     8990 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/project_item/executable_item_base.py
+-rw-rw-rw-   0        0        0     1487 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/project_item/project_item_info.py
+-rw-rw-rw-   0        0        0    14394 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/project_item/project_item_resource.py
+-rw-rw-rw-   0        0        0     4401 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/project_item/project_item_specification.py
+-rw-rw-rw-   0        0        0     1757 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/project_item/project_item_specification_factory.py
+-rw-rw-rw-   0        0        0     2886 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/project_item_loader.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:35:46.693766 spine_engine-0.22.0/spine_engine/server/
+-rw-rw-rw-   0        0        0     1057 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/server/__init__.py
+-rw-rw-rw-   0        0        0     3497 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/server/certificate_creator.py
+-rw-rw-rw-   0        0        0    20054 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/server/engine_server.py
+-rw-rw-rw-   0        0        0     4494 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/server/persistent_execution_service.py
+-rw-rw-rw-   0        0        0     2133 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/server/ping_service.py
+-rw-rw-rw-   0        0        0     5744 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/server/project_extractor_service.py
+-rw-rw-rw-   0        0        0     2630 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/server/project_remover_service.py
+-rw-rw-rw-   0        0        0     3813 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/server/project_retriever_service.py
+-rw-rw-rw-   0        0        0    12509 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/server/remote_execution_service.py
+-rw-rw-rw-   0        0        0     5757 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/server/request.py
+-rw-rw-rw-   0        0        0     1683 2023-04-19 13:04:17.000000 spine_engine-0.22.0/spine_engine/server/service_base.py
+-rw-rw-rw-   0        0        0     2457 2023-04-19 13:04:18.000000 spine_engine-0.22.0/spine_engine/server/start_server.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:35:46.737506 spine_engine-0.22.0/spine_engine/server/util/
+-rw-rw-rw-   0        0        0     1073 2023-04-19 13:04:18.000000 spine_engine-0.22.0/spine_engine/server/util/__init__.py
+-rw-rw-rw-   0        0        0     6339 2023-04-19 13:04:18.000000 spine_engine-0.22.0/spine_engine/server/util/event_data_converter.py
+-rw-rw-rw-   0        0        0     5363 2023-04-19 13:04:18.000000 spine_engine-0.22.0/spine_engine/server/util/server_message.py
+-rw-rw-rw-   0        0        0     3601 2023-04-19 13:04:18.000000 spine_engine-0.22.0/spine_engine/server/util/zip_handler.py
+-rw-rw-rw-   0        0        0     1673 2023-04-19 13:04:18.000000 spine_engine-0.22.0/spine_engine/shared_memory_io_manager.py
+-rw-rw-rw-   0        0        0    42548 2023-05-31 12:24:59.000000 spine_engine-0.22.0/spine_engine/spine_engine.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:35:46.803296 spine_engine-0.22.0/spine_engine/utils/
+-rw-rw-rw-   0        0        0      977 2022-11-03 13:43:21.000000 spine_engine-0.22.0/spine_engine/utils/__init__.py
+-rw-rw-rw-   0        0        0     2064 2023-04-19 13:04:18.000000 spine_engine-0.22.0/spine_engine/utils/command_line_arguments.py
+-rw-rw-rw-   0        0        0     3732 2023-04-19 13:04:18.000000 spine_engine-0.22.0/spine_engine/utils/execution_resources.py
+-rw-rw-rw-   0        0        0    13377 2023-05-02 10:55:42.000000 spine_engine-0.22.0/spine_engine/utils/helpers.py
+-rw-rw-rw-   0        0        0     5398 2023-04-19 13:04:18.000000 spine_engine-0.22.0/spine_engine/utils/queue_logger.py
+-rw-rw-rw-   0        0        0     3876 2023-04-19 13:04:18.000000 spine_engine-0.22.0/spine_engine/utils/returning_process.py
+-rw-rw-rw-   0        0        0     5103 2023-04-19 13:04:18.000000 spine_engine-0.22.0/spine_engine/utils/serialization.py
+-rw-rw-rw-   0        0        0     1001 2023-05-31 12:35:35.000000 spine_engine-0.22.0/spine_engine/version.py
+drwxrwxrwx   0        0        0        0 2023-05-31 12:35:46.339284 spine_engine-0.22.0/spine_engine.egg-info/
+-rw-rw-rw-   0        0        0     2552 2023-05-31 12:35:45.000000 spine_engine-0.22.0/spine_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2533 2023-05-31 12:35:46.000000 spine_engine-0.22.0/spine_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 12:35:45.000000 spine_engine-0.22.0/spine_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-10-07 10:28:55.000000 spine_engine-0.22.0/spine_engine.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      147 2023-05-31 12:35:45.000000 spine_engine-0.22.0/spine_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-31 12:35:45.000000 spine_engine-0.22.0/spine_engine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 12:35:46.826553 spine_engine-0.22.0/tests/
+-rw-rw-rw-   0        0        0     2345 2023-04-19 13:04:18.000000 spine_engine-0.22.0/tests/test_load_project_items.py
+-rw-rw-rw-   0        0        0    51148 2023-05-02 10:55:42.000000 spine_engine-0.22.0/tests/test_spine_engine.py
```

### Comparing `spine_engine-0.21.0/COPYING` & `spine_engine-0.22.0/COPYING`

 * *Files identical despite different names*

### Comparing `spine_engine-0.21.0/COPYING.LESSER` & `spine_engine-0.22.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `spine_engine-0.21.0/PKG-INFO` & `spine_engine-0.22.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,40 @@
-Metadata-Version: 2.1
-Name: spine_engine
-Version: 0.21.0
-Summary: A package to run Spine workflows.
-Home-page: https://github.com/spine-tools/spine-engine
-Author: Spine Project consortium
-Author-email: spine_info@vtt.fi
-License: LGPL-3.0-or-later
-Project-URL: Issue Tracker, https://github.com/spine-tools/spine-engine/issues
-Description: # Spine Engine
-        
-        [![Python](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)](https://www.python.org/downloads/release/python-379/)
-        [![Unit tests](https://github.com/spine-tools/spine-engine/workflows/Unit%20tests/badge.svg)](https://github.com/spine-tools/spine-engine/actions?query=workflow%3A"Unit+tests")
-        [![codecov](https://codecov.io/gh/spine-tools/spine-engine/branch/master/graph/badge.svg)](https://codecov.io/gh/spine-tools/spine-engine)
-        [![PyPI version](https://badge.fury.io/py/spine-engine.svg)](https://badge.fury.io/py/spine-engine)
-        
-        A Python package to coordinate the execution of [Spine Toolbox](https://github.com/spine-tools/Spine-Toolbox) workflows.
-        
-        ## License
-        
-        Spine Engine is released under the GNU Lesser General Public License (LGPL) license. All accompanying
-        documentation and manual are released under the [Creative Commons BY-SA 4.0 license](https://creativecommons.org/licenses/by-sa/4.0/).
-        
-        ## Getting started
-        
-        ### Installation
-        
-        To install Spine Engine into an existing Python environment, run
-        
-            $ pip install spine_engine
-        
-        ### Dependencies
-        
-        Spine Engine installation will install [dagster](https://dagster.readthedocs.io/en/master/index.html).
-        
-        &nbsp;
-        <hr>
-        <center>
-        <table width=500px frame="none">
-        <tr>
-        <td valign="middle" width=100px>
-        <img src=fig/eu-emblem-low-res.jpg alt="EU emblem" width=100%></td>
-        <td valign="middle">This project has received funding from European Climate, Infrastructure and Environment Executive Agency under the European Union’s HORIZON Research and Innovation Actions under grant agreement N°101095998.</td>
-        <tr>
-        <td valign="middle" width=100px>
-        <img src=fig/eu-emblem-low-res.jpg alt="EU emblem" width=100%></td>
-        <td valign="middle">This project has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement No 774629.</td>
-        </table>
-        </center>
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
+# Spine Engine
+
+[![Python](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)](https://www.python.org/downloads/release/python-379/)
+[![Unit tests](https://github.com/spine-tools/spine-engine/workflows/Unit%20tests/badge.svg)](https://github.com/spine-tools/spine-engine/actions?query=workflow%3A"Unit+tests")
+[![codecov](https://codecov.io/gh/spine-tools/spine-engine/branch/master/graph/badge.svg)](https://codecov.io/gh/spine-tools/spine-engine)
+[![PyPI version](https://badge.fury.io/py/spine-engine.svg)](https://badge.fury.io/py/spine-engine)
+
+A Python package to coordinate the execution of [Spine Toolbox](https://github.com/spine-tools/Spine-Toolbox) workflows.
+
+## License
+
+Spine Engine is released under the GNU Lesser General Public License (LGPL) license. All accompanying
+documentation and manual are released under the [Creative Commons BY-SA 4.0 license](https://creativecommons.org/licenses/by-sa/4.0/).
+
+## Getting started
+
+### Installation
+
+To install Spine Engine into an existing Python environment, run
+
+    $ pip install spine_engine
+
+### Dependencies
+
+Spine Engine installation will install [dagster](https://dagster.readthedocs.io/en/master/index.html).
+
+&nbsp;
+<hr>
+<center>
+<table width=500px frame="none">
+<tr>
+<td valign="middle" width=100px>
+<img src=fig/eu-emblem-low-res.jpg alt="EU emblem" width=100%></td>
+<td valign="middle">This project has received funding from European Climate, Infrastructure and Environment Executive Agency under the European Union’s HORIZON Research and Innovation Actions under grant agreement N°101095998.</td>
+<tr>
+<td valign="middle" width=100px>
+<img src=fig/eu-emblem-low-res.jpg alt="EU emblem" width=100%></td>
+<td valign="middle">This project has received funding from the European Union’s Horizon 2020 research and innovation programme under grant agreement No 774629.</td>
+</table>
+</center>
```

#### html2text {}

```diff
@@ -1,31 +1,22 @@
-Metadata-Version: 2.1 Name: spine_engine Version: 0.21.0 Summary: A package to
-run Spine workflows. Home-page: https://github.com/spine-tools/spine-engine
-Author: Spine Project consortium Author-email: spine_info@vtt.fi License: LGPL-
-3.0-or-later Project-URL: Issue Tracker, https://github.com/spine-tools/spine-
-engine/issues Description: # Spine Engine [![Python](https://img.shields.io/
-badge/python-3.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)](https://
-www.python.org/downloads/release/python-379/) [![Unit tests](https://
-github.com/spine-tools/spine-engine/workflows/Unit%20tests/badge.svg)](https://
-github.com/spine-tools/spine-engine/actions?query=workflow%3A"Unit+tests") [!
-[codecov](https://codecov.io/gh/spine-tools/spine-engine/branch/master/graph/
-badge.svg)](https://codecov.io/gh/spine-tools/spine-engine) [![PyPI version]
-(https://badge.fury.io/py/spine-engine.svg)](https://badge.fury.io/py/spine-
-engine) A Python package to coordinate the execution of [Spine Toolbox](https:/
-/github.com/spine-tools/Spine-Toolbox) workflows. ## License Spine Engine is
-released under the GNU Lesser General Public License (LGPL) license. All
-accompanying documentation and manual are released under the [Creative Commons
-BY-SA 4.0 license](https://creativecommons.org/licenses/by-sa/4.0/). ## Getting
-started ### Installation To install Spine Engine into an existing Python
-environment, run $ pip install spine_engine ### Dependencies Spine Engine
-installation will install [dagster](https://dagster.readthedocs.io/en/master/
-index.html).  
+# Spine Engine [![Python](https://img.shields.io/badge/python-
+3.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)](https://www.python.org/
+downloads/release/python-379/) [![Unit tests](https://github.com/spine-tools/
+spine-engine/workflows/Unit%20tests/badge.svg)](https://github.com/spine-tools/
+spine-engine/actions?query=workflow%3A"Unit+tests") [![codecov](https://
+codecov.io/gh/spine-tools/spine-engine/branch/master/graph/badge.svg)](https://
+codecov.io/gh/spine-tools/spine-engine) [![PyPI version](https://badge.fury.io/
+py/spine-engine.svg)](https://badge.fury.io/py/spine-engine) A Python package
+to coordinate the execution of [Spine Toolbox](https://github.com/spine-tools/
+Spine-Toolbox) workflows. ## License Spine Engine is released under the GNU
+Lesser General Public License (LGPL) license. All accompanying documentation
+and manual are released under the [Creative Commons BY-SA 4.0 license](https://
+creativecommons.org/licenses/by-sa/4.0/). ## Getting started ### Installation
+To install Spine Engine into an existing Python environment, run $ pip install
+spine_engine ### Dependencies Spine Engine installation will install [dagster]
+(https://dagster.readthedocs.io/en/master/index.html).  
 ===============================================================================
 [EU     This project has received funding from European Climate, Infrastructure and
 emblem] Environment Executive Agency under the European Unionâs HORIZON Research and
         Innovation Actions under grant agreement NÂ°101095998.
 [EU     This project has received funding from the European Unionâs Horizon 2020
 emblem] research and innovation programme under grant agreement No 774629.
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent Description-Content-Type: text/
-markdown
```

### Comparing `spine_engine-0.21.0/setup.py` & `spine_engine-0.22.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Setup script for Python's setuptools.
 
-:authors: M. Marin (KTH)
-:date:   20.11.2019
 """
 
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf8") as readme_file:
     readme = readme_file.read()
 
@@ -27,15 +25,15 @@
 
 install_requires = [
     "dagster>=0.12.6, <0.12.9",  # dagster >= 0.12.9 requires alembic that is incompatible with spinedb_api
     "protobuf<3.21.0",  # https://developers.google.com/protocol-buffers/docs/news/2022-05-06#python-updates
     "networkx>2.5.1",
     "datapackage>=1.15.2, <1.16",
     "jupyter_client<7.0",
-    "spinedb_api>=0.24.0",
+    "spinedb_api>=0.29.0",
     "pyzmq >=21.0",
     "markupsafe < 2.1",  # dagster 0.12.8 requires Jinja2<3.0, which tries to import soft_unicode, which has been removed in markupsafe 2.1
 ]
 
 setup(
     name="spine_engine",
     version=version["__version__"],
```

### Comparing `spine_engine-0.21.0/spine_engine/__init__.py` & `spine_engine-0.22.0/spine_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.21.0/spine_engine/config.py` & `spine_engine-0.22.0/spine_engine/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Application constants.
 
-:author: P. Savolainen (VTT)
-:date:   2.1.2018
 """
 
 import os
 import sys
 
 _on_windows = sys.platform == "win32"
```

### Comparing `spine_engine-0.21.0/spine_engine/exception.py` & `spine_engine-0.22.0/spine_engine/exception.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 """
 Contains Engine's exceptions.
 
-:authors: A. Soininen (VTT)
-:date:    30.6.2021
 """
 
 
 class EngineInitFailed(Exception):
     """Raised when :class:`SpineEngine` initialization fails."""
```

### Comparing `spine_engine-0.21.0/spine_engine/execution_managers/__init__.py` & `spine_engine-0.22.0/spine_engine/execution_managers/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.21.0/spine_engine/execution_managers/conda_kernel_spec_manager.py` & `spine_engine-0.22.0/spine_engine/execution_managers/conda_kernel_spec_manager.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.21.0/spine_engine/execution_managers/conda_kernel_spec_runner.py` & `spine_engine-0.22.0/spine_engine/execution_managers/conda_kernel_spec_runner.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.21.0/spine_engine/execution_managers/execution_manager_base.py` & `spine_engine-0.22.0/spine_engine/execution_managers/execution_manager_base.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains the ExecutionManagerBase class.
 
-:authors: M. Marin (KTH)
-:date:   12.10.2020
 """
 
 
 class ExecutionManagerBase:
     """Base class for all tool instance execution managers."""
 
     def __init__(self, logger):
```

### Comparing `spine_engine-0.21.0/spine_engine/execution_managers/kernel_execution_manager.py` & `spine_engine-0.22.0/spine_engine/execution_managers/kernel_execution_manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,52 +8,80 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains the KernelExecutionManager class and subclasses, and some convenience functions.
 
-:authors: M. Marin (KTH)
-:date:   12.10.2020
 """
 
 import os
 import sys
 import subprocess
+import uuid
 from jupyter_client.manager import KernelManager
 from jupyter_client.kernelspec import NoSuchKernel
 from ..utils.helpers import Singleton
 from .execution_manager_base import ExecutionManagerBase
 from spine_engine.execution_managers.conda_kernel_spec_manager import CondaKernelSpecManager
 
 
+class GroupedKernelManager(KernelManager):
+    """Kernel Manager that supports group ID's."""
+
+    def __init__(self, *args, **kwargs):
+        group_id = kwargs.pop("group_id", "")
+        super().__init__(*args, **kwargs)
+        self._group_id = group_id
+        self._is_busy = False
+
+    def group_id(self):
+        """Returns the group ID of this kernel manager."""
+        return self._group_id
+
+    def set_busy(self, f):
+        """Sets km busy. This is set according to the
+        status messages received from the IOPUB channel."""
+        self._is_busy = f
+
+    def is_busy(self):
+        """Returns whether km is busy or not."""
+        return self._is_busy
+
+
 class _KernelManagerFactory(metaclass=Singleton):
     _kernel_managers = {}
-    """Maps tuples (kernel name, group id) to associated KernelManager."""
+    """Maps filter_id (str) to associated KernelManager"""
     _key_by_connection_file = {}
-    """Maps connection file string to tuple (kernel_name, group_id). Mostly for fast lookup in ``restart_kernel()``"""
+    """Maps connection file path to filter_id (str)"""
 
-    def _make_kernel_manager(self, kernel_name, group_id, server_ip):
-        """Creates a new kernel manager for given kernel and group id if none exists, and returns it.
+    def _make_kernel_manager(self, kernel_name, group_id, server_ip, filter_id):
+        """Creates a new kernel manager if necessary or returns an existing one.
 
         Args:
-            kernel_name (str): the kernel
-            group_id (str): item group that will execute using this kernel
+            kernel_name (str): The kernel
+            group_id (str): Item group that will execute using this kernel
             server_ip (str): Engine Server IP address. '127.0.0.1' when execution happens locally
+            filter_id (str): Filter Id
 
         Returns:
-            KernelManager
+            GroupedKernelManager
         """
-        if group_id is None:
-            # Execute in isolation
-            return KernelManager(kernel_name=kernel_name, ip=server_ip)
-        key = (kernel_name, group_id)
-        if key not in self._kernel_managers:
-            self._kernel_managers[key] = KernelManager(kernel_name=kernel_name, ip=server_ip)
-        return self._kernel_managers[key]
+        if not filter_id == "":
+            group_id = filter_id  # Ignore group ID in case filter ID exists
+        for k in self._kernel_managers:
+            # Reuse kernel manager if using same group id and kernel and it's idle
+            km = self._kernel_managers[k]
+            if km.group_id() == group_id and km.kernel_name == kernel_name:
+                if not km.is_busy():
+                    return km
+        key = uuid.uuid4().hex
+        # Spawn a new kernel manager
+        km = self._kernel_managers[key] = GroupedKernelManager(kernel_name=kernel_name, ip=server_ip, group_id=group_id)
+        return km
 
     def new_kernel_manager(self, kernel_name, group_id, logger, extra_switches=None, environment="", **kwargs):
         """Creates a new kernel manager for given kernel and group id if none exists.
         Starts the kernel if not started, and returns it.
 
         Args:
             kernel_name (str): the kernel
@@ -64,88 +92,150 @@
             environment (str): "conda" to launch a Conda kernel spec. "" for a regular kernel spec
             `**kwargs`: optional. Keyword arguments passed to ``KernelManager.start_kernel()``
 
         Returns:
             KernelManager
         """
         server_ip = kwargs.pop("server_ip", "")
-        km = self._make_kernel_manager(kernel_name, group_id, server_ip)
+        filter_id = logger.msg_kernel_execution.filter_id
+        km = self._make_kernel_manager(kernel_name, group_id, server_ip, filter_id)
         conda_exe = kwargs.pop("conda_exe", "")
         if environment == "conda":
             try:
                 km.kernel_spec_manager = CondaKernelSpecManager(conda_exe=conda_exe)
             except Exception as err:
                 logger.msg_kernel_execution.emit(msg=dict(type="conda_not_found", error=err))
                 raise RuntimeError
-        msg_head = dict(kernel_name=kernel_name)
+        msg = dict(kernel_name=kernel_name)
         if not km.is_alive():
             try:
                 if not km.kernel_spec:
                     # Happens when a conda kernel spec with the requested name cannot be dynamically created
                     # i.e. the conda environment does not exist
-                    msg = dict(type="kernel_spec_not_found", **msg_head)
+                    msg["type"] = "kernel_spec_not_found"
                     logger.msg_kernel_execution.emit(msg)
                     raise RuntimeError
             except NoSuchKernel:
-                msg = dict(type="kernel_spec_not_found", **msg_head)
+                msg["type"] = "kernel_spec_not_found"
                 logger.msg_kernel_execution.emit(msg)
                 raise RuntimeError
             # Check that kernel spec executable is referring to a file that actually exists
             exe_path = km.kernel_spec.argv[0]
             if not os.path.exists(exe_path) and os.path.isabs(exe_path):
-                msg_head["kernel_exe_path"] = exe_path
-                msg = dict(type="kernel_spec_exe_not_found", **msg_head)
+                msg["type"] = "kernel_spec_exe_not_found"
+                msg["kernel_exe_path"] = exe_path
                 logger.msg_kernel_execution.emit(msg)
                 raise RuntimeError
             if extra_switches:
                 # Insert switches right after the julia program
                 km.kernel_spec.argv[1:1] = extra_switches
             km.start_kernel(**kwargs)
-            self._key_by_connection_file[km.connection_file] = (kernel_name, group_id)
-        msg = dict(type="kernel_started", connection_file=km.connection_file, **msg_head)
+            key = self.get_kernel_manager_key(km)
+            if not key:
+                raise RuntimeError  # Logic error
+            self._key_by_connection_file[km.connection_file] = key
+        msg["type"] = "kernel_started"
+        msg["connection_file"] = km.connection_file
         logger.msg_kernel_execution.emit(msg)
         return km
 
+    def get_kernel_manager_key(self, km):
+        """Returns the key of the given kernel manager stored in this factory.
+
+        Args:
+            km (GroupedKernelManager): Kernel managers
+
+        Returns:
+            str: Kernel Manager's 32 character key
+        """
+        for key, kernman in self._kernel_managers.items():
+            if kernman == km:
+                return key
+        return None
+
     def get_kernel_manager(self, connection_file):
         """Returns a kernel manager for given connection file if any.
 
         Args:
             connection_file (str): path of connection file
 
         Returns:
-            KernelManager or None
+            GroupedKernelManager or None
         """
-        key = self._key_by_connection_file.get(connection_file)
-        return self._kernel_managers.get(key)
+        key = self._key_by_connection_file.get(connection_file, None)
+        return self._kernel_managers.get(key, None)
 
     def pop_kernel_manager(self, connection_file):
         """Returns a kernel manager for given connection file if any.
         It also removes it from cache.
 
         Args:
             connection_file (str): path of connection file
 
         Returns:
-            KernelManager or None
+            GroupedKernelManager or None
         """
         key = self._key_by_connection_file.pop(connection_file, None)
         return self._kernel_managers.pop(key, None)
 
+    def shutdown_kernel_manager(self, connection_file):
+        """Pops a kernel manager from factory and shuts it down.
+
+        Args:
+            connection_file (str): path of connection file
+
+        Returns:
+            bool: True if operation succeeded, False otherwise
+        """
+        km = self.pop_kernel_manager(connection_file)
+        if not km:  # Just to be safe
+            return
+        if km.is_alive():
+            km.shutdown_kernel(now=True)
+        return
+
+    def kill_kernel_managers(self):
+        """Shuts down all kernel managers stored in the factory."""
+        while True:
+            try:
+                key, km = self._kernel_managers.popitem()
+                if km.is_alive():
+                    km.shutdown_kernel(now=True)
+            except KeyError:
+                break
+        self._key_by_connection_file.clear()
+
+    def n_kernel_managers(self):
+        """Returns the number of open kernel managers stored in the factory."""
+        return len(self._kernel_managers)
+
 
 _kernel_manager_factory = _KernelManagerFactory()
 
 
 def get_kernel_manager(connection_file):
     return _kernel_manager_factory.get_kernel_manager(connection_file)
 
 
 def pop_kernel_manager(connection_file):
     return _kernel_manager_factory.pop_kernel_manager(connection_file)
 
 
+def n_kernel_managers():
+    return _kernel_manager_factory.n_kernel_managers()
+
+
+def kill_all_kernel_managers():
+    _kernel_manager_factory.kill_kernel_managers()
+
+
+def shutdown_kernel_manager(connection_file):
+    return _kernel_manager_factory.shutdown_kernel_manager(connection_file)
+
+
 class KernelExecutionManager(ExecutionManagerBase):
     def __init__(
         self,
         logger,
         kernel_name,
         *commands,
         group_id=None,
@@ -166,16 +256,16 @@
             environment (str): "conda" to launch a Conda kernel spec. "" for a regular kernel spec.
             **kwargs (optional): Keyword arguments passed to ``KernelManager.start_kernel()``
         """
         super().__init__(logger)
         self._msg_head = dict(kernel_name=kernel_name)
         self._commands = commands
         self._cmd_failed = False
-        kwargs["stdout"] = open(os.devnull, 'w')
-        kwargs["stderr"] = open(os.devnull, 'w')
+        self.std_out = kwargs["stdout"] = open(os.devnull, 'w')
+        self.std_err = kwargs["stderr"] = open(os.devnull, 'w')
         # Don't show console when frozen
         kwargs["creationflags"] = subprocess.CREATE_NO_WINDOW if sys.platform == "win32" else 0
         self._kernel_manager = _kernel_manager_factory.new_kernel_manager(
             kernel_name, group_id, logger, extra_switches=extra_switches, environment=environment, **kwargs
         )
         self._kernel_client = self._kernel_manager.client() if self._kernel_manager is not None else None
         self._startup_timeout = startup_timeout
@@ -208,15 +298,23 @@
             reply = self._kernel_client.execute_interactive(cmd, output_hook=self._output_hook)
             st = reply["content"]["status"]
             if st != "ok":
                 return False  # This happens when execute_request fails
         return True
 
     def _output_hook(self, msg):
-        """Catches messages from the IOPUB (PUB/SUB) channel and handle case when message type is 'error'.
-        'error' msg is a response to an execute_input msg."""
+        """Catches messages from the IOPUB (PUB/SUB) channel and
+        handles 'error' and 'status message tyoe cases. 'error'
+        msg is a response to an execute_input msg."""
         if msg["header"]["msg_type"] == "error":
             self._cmd_failed = True
+        elif msg["header"]["msg_type"] == "status":
+            # Set kernel manager busy if execution is starting or in progress
+            exec_state = msg["content"]["execution_state"]
+            if exec_state == "busy" or exec_state == "starting":
+                self._kernel_manager.set_busy(True)
+            else:  # exec_state == 'idle'
+                self._kernel_manager.set_busy(False)
 
     def stop_execution(self):
         if self._kernel_manager is not None:
             self._kernel_manager.interrupt_kernel()
```

### Comparing `spine_engine-0.21.0/spine_engine/execution_managers/persistent_execution_manager.py` & `spine_engine-0.22.0/spine_engine/execution_managers/persistent_execution_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains PersistentManagerBase, PersistentExecutionManagerBase classes and subclasses,
 as well as some convenience functions.
 
-:authors: M. Marin (KTH)
-:date:   12.10.2020
 """
 import uuid
 import socket
 import socketserver
 import sys
 import os
 import signal
@@ -399,27 +397,40 @@
         self.set_running_until_completion(False)
         self._start_persistent()
         self._wait()
         yield from self.drain_queue()
 
     def interrupt_persistent(self):
         """Interrupts the persistent process."""
-        threading.Thread(target=self._do_interrupt_persistent).start()
+        queue = Queue()
+        thread = threading.Thread(target=self._do_interrupt_persistent, args=(queue,))
+        thread.start()
+        # Wait till the process becomes idle, then put None to the queue
         self._wait()
+        queue.put(None)
+        thread.join()
 
-    def _do_interrupt_persistent(self):
+    def _do_interrupt_persistent(self, queue):
         persistent = self._persistent  # Make local copy; other threads may set self._persistent to None while sleeping.
         if persistent is None:
             return
-        if sys.platform == "win32":
-            p = Process(target=_send_ctrl_c, args=(persistent.pid,))
-            p.start()
-            p.join()
-        else:
-            persistent.send_signal(signal.SIGINT)
+        while True:
+            if sys.platform == "win32":
+                p = Process(target=_send_ctrl_c, args=(persistent.pid,))
+                p.start()
+                p.join()
+            else:
+                persistent.send_signal(signal.SIGINT)
+            try:
+                # Wait 2 seconds to get an item from the queue, which means the process has become idle...
+                # Otherwise just keep interrupting it
+                queue.get(timeout=2)
+                break
+            except Empty:
+                pass
         self.set_running_until_completion(False)
 
     def is_persistent_alive(self):
         """Whether the persistent is still alive and ready to receive commands.
 
         Returns:
             bool
```

### Comparing `spine_engine-0.21.0/spine_engine/execution_managers/process_execution_manager.py` & `spine_engine-0.22.0/spine_engine/execution_managers/process_execution_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains the ProcessExecutionManager class.
 
-:authors: M. Marin (KTH)
-:date:   12.10.2020
 """
 
 import sys
 import subprocess
 from threading import Thread
 from .execution_manager_base import ExecutionManagerBase
 from ..utils.execution_resources import one_shot_process_semaphore
```

### Comparing `spine_engine-0.21.0/spine_engine/execution_managers/spine_repl.jl` & `spine_engine-0.22.0/spine_engine/execution_managers/spine_repl.jl`

 * *Files identical despite different names*

### Comparing `spine_engine-0.21.0/spine_engine/execution_managers/spine_repl.py` & `spine_engine-0.22.0/spine_engine/execution_managers/spine_repl.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.21.0/spine_engine/load_project_items.py` & `spine_engine-0.22.0/spine_engine/load_project_items.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Functions to load project item modules.
 
-:author: A. Soininen (VTT)
-:date:   29.4.2020
 """
 import pathlib
 import importlib
 import importlib.util
 
 
 def load_item_specification_factories(items_package_name):
```

### Comparing `spine_engine-0.21.0/spine_engine/multithread_executor/__init__.py` & `spine_engine-0.22.0/spine_engine/multithread_executor/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.21.0/spine_engine/multithread_executor/executor.py` & `spine_engine-0.22.0/spine_engine/multithread_executor/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Module contains multithread_executor.
 
-:author: M. Marin (KTH)
-:date:   1.11.2020
 """
 
 from dagster.core.definitions.executor import Int, Field, RetryMode, check, executor, get_retries_config
 
 
 @executor(
     name="multithread",
```

### Comparing `spine_engine-0.21.0/spine_engine/multithread_executor/multithread.py` & `spine_engine-0.22.0/spine_engine/multithread_executor/multithread.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Module contains MultithreadExecutor.
 
-:author: M. Marin (KTH)
-:date:   1.11.2020
 """
 
 import os
 import sys
 from dagster import check
 from dagster.core.execution.api import (
     create_execution_plan,
```

### Comparing `spine_engine-0.21.0/spine_engine/multithread_executor/thread_executor.py` & `spine_engine-0.22.0/spine_engine/multithread_executor/thread_executor.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.21.0/spine_engine/project_item/__init__.py` & `spine_engine-0.22.0/spine_engine/project_item/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,10 +8,8 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 This subpackage contains base classes for project items.
 
-:authors: M. Marin (KTH)
-:date:    8.10.2020
 """
```

### Comparing `spine_engine-0.21.0/spine_engine/project_item/connection.py` & `spine_engine-0.22.0/spine_engine/project_item/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 """
 Provides connection classes for linking project items.
 
-:authors: A. Soininen (VTT)
-:date:    12.2.2021
 """
 from dataclasses import asdict, dataclass, field
 import os
 import subprocess
 import tempfile
 from contextlib import ExitStack
 from datapackage import Package
```

### Comparing `spine_engine-0.21.0/spine_engine/project_item/executable_item_base.py` & `spine_engine-0.22.0/spine_engine/project_item/executable_item_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains ExecutableItem, a project item's counterpart in execution as well as support utilities.
 
-:authors: A. Soininen (VTT)
-:date:    30.3.2020
 """
 from hashlib import sha1
 from pathlib import Path
 from ..utils.helpers import ExecutionDirection, ItemExecutionFinishState, shorten
 
 
 class ExecutableItemBase:
```

### Comparing `spine_engine-0.21.0/spine_engine/project_item/project_item_info.py` & `spine_engine-0.22.0/spine_engine/project_item/project_item_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 """
 Provides the ProjectItemInfo class.
 
-:authors: A. Soininen (VTT)
-:date:   29.4.2020
 """
 
 
 class ProjectItemInfo:
     @staticmethod
     def item_category():
         """
```

### Comparing `spine_engine-0.21.0/spine_engine/project_item/project_item_resource.py` & `spine_engine-0.22.0/spine_engine/project_item/project_item_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Provides the ProjectItemResource class.
 
-:authors: M. Marin (KTH)
-:date:   29.4.2020
 """
 import copy
 import uuid
 from contextlib import contextmanager
 from pathlib import Path
 from urllib.parse import urlparse
 from urllib.request import url2pathname
```

### Comparing `spine_engine-0.21.0/spine_engine/project_item/project_item_specification.py` & `spine_engine-0.22.0/spine_engine/project_item/project_item_specification.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains project item specification class.
 
-:authors: M. Marin (KTH)
-:date:    7.5.2020
 """
 import json
 
 from spine_engine.utils.helpers import shorten, gather_leaf_data
 
 
 class ProjectItemSpecification:
```

### Comparing `spine_engine-0.21.0/spine_engine/project_item/project_item_specification_factory.py` & `spine_engine-0.22.0/spine_engine/project_item/project_item_specification_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains project item specification factory.
 
-:authors: A. Soininen (VTT)
-:date:   6.5.2020
 """
 
 
 class ProjectItemSpecificationFactory:
     """A factory to make project item specifications."""
 
     @staticmethod
```

### Comparing `spine_engine-0.21.0/spine_engine/project_item_loader.py` & `spine_engine-0.22.0/spine_engine/project_item_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains :class:`ProjectItemLoader`.
 
-:author: A. Soininen (VTT)
-:date:   11.2.2021
 """
 from multiprocessing import Lock
 from .load_project_items import load_executable_item_classes, load_item_specification_factories
 from .utils.helpers import Singleton
 
 
 class ProjectItemLoader(metaclass=Singleton):
```

### Comparing `spine_engine-0.21.0/spine_engine/server/__init__.py` & `spine_engine-0.22.0/spine_engine/version.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,8 @@
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser
 # General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your
 # option) any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
-
-"""
-This package contains Remote Server classes of the Spine Engine.
-
-:authors: P. Pääkkönen (VTT), P. Savolainen (VTT)
-:date:    18.8.2021
-"""
+__version__ = "0.22.0"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spine_engine-0.21.0/spine_engine/server/certificate_creator.py` & `spine_engine-0.22.0/spine_engine/server/certificate_creator.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 ######################################################################################################################
 
 """
 The function of this class can be used for generation of keys for enabling security 
 of the remote spine_server. The code has been copied based on an example at (by Chris Laws):
 https://github.com/zeromq/pyzmq/blob/main/examples/security/generate_certificates.py
 
-:authors: P. Pääkkönen (VTT)
-:date:   15.09.2021
 """
 
 import os
 import sys
 import shutil
 import zmq.auth
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spine_engine-0.21.0/spine_engine/server/engine_server.py` & `spine_engine-0.22.0/spine_engine/server/engine_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains EngineServer class for running a Zero-MQ server with Spine Engine.
-:authors: P. Pääkkönen (VTT), P. Savolainen (VTT)
-:date:   19.08.2021
 """
 import json.decoder
 import os
 import queue
 import time
 import threading
 import ipaddress
@@ -152,14 +150,24 @@
                             print(f"Worker for job_id:{request.request_id()} not found")
                             msg = f"Stopping DAG execution failed. Worker for job_id:{request.request_id()} not found."
                             self.send_init_failed_reply(frontend, request.connection_id(), msg)
                             continue
                         worker.stop_engine()
                         request.send_response(frontend, ("server_status_msg", "DAG worker stopped"))
                         continue
+                    elif request.cmd() == "answer_prompt":
+                        worker = workers.get(request.request_id(), None)  # Get DAG execution worker based on job Id
+                        if not worker:
+                            print(f"Worker for job_id:{request.request_id()} not found")
+                            msg = f"Answering prompt failed. Worker for job_id:{request.request_id()} not found."
+                            self.send_init_failed_reply(frontend, request.connection_id(), msg)
+                            continue
+                        item_name, accepted = request.data()
+                        worker.answer_prompt(item_name, accepted)
+                        continue
                     elif request.cmd() == "retrieve_project":
                         project_dir = project_dirs.get(request.request_id(), None)  # Get project dir based on job_id
                         if not project_dir:
                             print(f"Project for job_id:{request.request_id()} not found")
                             msg = (
                                 f"Retrieving project for job_id {request.request_id()} failed. "
                                 f"Project directory not found."
@@ -249,17 +257,15 @@
 
         Returns:
             None if something went wrong or a new Request instance
         """
         b_json_str_server_msg = msg[1]  # binary string
         if len(b_json_str_server_msg) <= 10:  # Message size too small
             print(f"User data frame too small [{len(msg[1])}]. msg:{msg}")
-            self.send_init_failed_reply(
-                socket, msg[0], f"User data frame too small " f"- Malformed message sent to server."
-            )
+            self.send_init_failed_reply(socket, msg[0], "User data frame too small. Malformed message sent to server.")
             return None
         try:
             json_str_server_msg = b_json_str_server_msg.decode("utf-8")  # json string
         except UnicodeDecodeError as e:
             print(f"Decoding received msg '{msg[1]} ' failed. \nUnicodeDecodeError: {e}")
             self.send_init_failed_reply(
                 socket, msg[0], f"UnicodeDecodeError: {e}. " f"- Malformed message sent to server."
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spine_engine-0.21.0/spine_engine/server/persistent_execution_service.py` & `spine_engine-0.22.0/spine_engine/server/persistent_execution_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains a class for remote persistent execution manager related actions.
-:authors: P. Savolainen (VTT)
-:date:   26.9.2022
 """
 
 import threading
 import json
 import zmq
 from spine_engine.server.service_base import ServiceBase
```

### Comparing `spine_engine-0.21.0/spine_engine/server/ping_service.py` & `spine_engine-0.22.0/spine_engine/server/ping_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains a class for handling ping requests.
-:authors: P. Pääkkönen (VTT), P. Savolainen (VTT)
-:date:   13.09.2021
 """
 
 import threading
 import json
 import zmq
 from spine_engine.server.service_base import ServiceBase
 from spine_engine.server.util.server_message import ServerMessage
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spine_engine-0.21.0/spine_engine/server/project_extractor_service.py` & `spine_engine-0.22.0/spine_engine/server/project_extractor_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains a class for extracting a project ZIP file into a new directory on server.
-:authors: P. Savolainen (VTT)
-:date:   29.8.2022
 """
 
 import os
 import json
 import threading
 import uuid
 import zmq
```

### Comparing `spine_engine-0.21.0/spine_engine/server/project_remover_service.py` & `spine_engine-0.22.0/spine_engine/server/project_remover_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains a class for sending a finished project back to client.
-:authors: P. Savolainen (VTT)
-:date:   13.09.2021
 """
 
 import os
 import shutil
 import threading
 import zmq
 from spine_engine.server.service_base import ServiceBase
```

### Comparing `spine_engine-0.21.0/spine_engine/server/project_retriever_service.py` & `spine_engine-0.22.0/spine_engine/server/project_retriever_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains a class for sending a finished project back to client.
-:authors: P. Savolainen (VTT)
-:date:   13.09.2021
 """
 
 import os
 import shutil
 import threading
 import json
 import zmq
```

### Comparing `spine_engine-0.21.0/spine_engine/server/remote_execution_service.py` & `spine_engine-0.22.0/spine_engine/server/remote_execution_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains RemoteExecutionService class that executes a single DAG on the Spine Engine Server.
-:authors: P. Pääkkönen (VTT), P. Savolainen (VTT)
-:date:   24.08.2021
 """
 
 import os
 import threading
 import zmq
 from spine_engine import SpineEngine
 from spine_engine.utils.helpers import get_file_size
@@ -153,14 +151,18 @@
             self.worker_socket, ("remote_execution_event", "completed"), (self.job_id, "completed")
         )
 
     def stop_engine(self):
         """Stops DAG execution."""
         self.engine.stop()
 
+    def answer_prompt(self, item_name, accepted):
+        """Answers prompt."""
+        self.engine.answer_prompt(item_name, accepted)
+
     def close(self):
         """Cleans up sockets after worker is finished."""
         super().close()
         self.push_socket.close()
 
     @staticmethod
     def convert_input(input_data, local_project_dir):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spine_engine-0.21.0/spine_engine/server/request.py` & `spine_engine-0.22.0/spine_engine/server/request.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains a class for client requests received at server.
-:author: P. Pääkkönen (VTT), P. Savolainen (VTT)
-:date:   19.8.2021
 """
 
 import json
 from spine_engine.server.util.server_message import ServerMessage
 
 
 class Request:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spine_engine-0.21.0/spine_engine/server/service_base.py` & `spine_engine-0.22.0/spine_engine/server/service_base.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains a base class for different services provided by the Spine Engine Server.
-:authors: P. Savolainen (VTT)
-:date:   30.9.2021
 """
 
 import zmq
 
 
 class ServiceBase:
     """Service base class."""
```

### Comparing `spine_engine-0.21.0/spine_engine/server/start_server.py` & `spine_engine-0.22.0/spine_engine/server/start_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Start script for Spine Engine Server.
 
-:author: P. Savolainen (VTT)
-:date:   01.09.2021
 """
 
 import sys
 import time
 from spine_engine.server.engine_server import EngineServer, ServerSecurityModel
```

### Comparing `spine_engine-0.21.0/spine_engine/server/util/__init__.py` & `spine_engine-0.22.0/spine_engine/server/util/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,10 +8,8 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 This package contains utility classes of remote server part of the Spine Engine.
 
-:authors: P. Pääkkönen (VTT), P. Savolainen (VTT)
-:date:    23.8.2021
 """
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spine_engine-0.21.0/spine_engine/server/util/event_data_converter.py` & `spine_engine-0.22.0/spine_engine/server/util/event_data_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains static methods for converting event and data information to JSON format and back.
-:authors: P. Pääkkönen (VTT), P. Savolainen (VTT)
-:date:   27.08.2021
 """
 
 import base64
 import json
 from spine_engine.spine_engine import ItemExecutionFinishState
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spine_engine-0.21.0/spine_engine/server/util/server_message.py` & `spine_engine-0.22.0/spine_engine/server/util/server_message.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains a helper class for JSON-based messages exchanged between server and clients.
-:authors: P. Pääkkönen (VTT), P. Savolainen (VTT)
-:date:   23.08.2021
 """
 
 import json
 
 
 class ServerMessage:
     """Class for communicating requests and replies between the client and the server."""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spine_engine-0.21.0/spine_engine/server/util/zip_handler.py` & `spine_engine-0.22.0/spine_engine/server/util/zip_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains static methods for handling ZIP files.
-:authors: P. Pääkkönen (VTT), P. Savolainen (VTT)
-:date:   23.08.2021
 """
 
 import os
 import shutil
 from zipfile import ZipFile
 from spine_engine.utils.helpers import get_file_size
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `spine_engine-0.21.0/spine_engine/shared_memory_io_manager.py` & `spine_engine-0.22.0/spine_engine/shared_memory_io_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 """
 Contains Engine's IO manager.
 
-:authors: A. Soininen (VTT)
-:date:    6.7.2021
 """
 from dagster import IOManager, io_manager
 
 
 @io_manager
 def shared_memory_io_manager(init_context):
     return SharedMemoryIOManager()
```

### Comparing `spine_engine-0.21.0/spine_engine/spine_engine.py` & `spine_engine-0.22.0/spine_engine/spine_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Contains the SpineEngine class for running Spine Toolbox DAGs.
 
-:authors: M. Marin (KTH)
-:date:   20.11.2019
 """
 
 from enum import Enum, unique
 import os
 import threading
 import multiprocessing as mp
 from itertools import product
@@ -49,14 +47,16 @@
 from .utils.helpers import (
     AppSettings,
     inverted,
     create_timestamp,
     make_dag,
     ExecutionDirection as ED,
     ItemExecutionFinishState,
+    dag_edges,
+    make_connections,
 )
 from .utils.execution_resources import one_shot_process_semaphore, persistent_process_semaphore
 from .utils.queue_logger import QueueLogger
 from .project_item_loader import ProjectItemLoader
 from .multithread_executor.executor import multithread_executor
 from .project_item.connection import Connection, Jump
 from .shared_memory_io_manager import shared_memory_io_manager
@@ -106,94 +106,145 @@
             specifications (dict(str,list(dict))): A mapping from item type to list of specification dicts.
             connections (list of dict): List of connection dicts
             jumps (list of dict, optional): List of jump dicts
             items_module_name (str): name of the Python module that contains project items
             settings (dict): Toolbox execution settings.
             project_dir (str): Path to project directory.
             execution_permits (dict(str,bool)): A mapping from item name to a boolean value, False indicating that
-                the item is not executed, only its resources are collected.
+                the item is not executed
             debug (bool): Whether debug mode is active or not.
 
         Raises:
-            EngineInitFailed: raised if initialization failed
+            EngineInitFailed: Raised if initialization fails
         """
         super().__init__()
         self._queue = mp.Queue()
         if items is None:
             items = {}
         self._items = items
-        if connections is None:
-            connections = []
-        self._connections = list(map(Connection.from_dict, connections))
+        if execution_permits is None:
+            execution_permits = {}
+        self._execution_permits = execution_permits
+        connections = list(map(Connection.from_dict, connections))  # Deserialize connections
+        self._connections = make_connections(connections, self._execution_permits)
         self._connections_by_source = dict()
         self._connections_by_destination = dict()
-        node_successors = {item_name: list() for item_name in self._items}
-        for connection in self._connections:
-            if not connection.ready_to_execute():
-                notifications = " ".join(connection.notifications())
-                raise EngineInitFailed(f"Link {connection.name} is not ready for execution. {notifications}")
-            source, destination = connection.source, connection.destination
-            self._connections_by_source.setdefault(source, list()).append(connection)
-            self._connections_by_destination.setdefault(destination, list()).append(connection)
-            successors = node_successors.get(source)
-            if successors is not None:
-                successors.append(destination)
+        self._validate_and_sort_connections()
+        edges = dag_edges(self._connections)  # Mapping of a source node (item) to a list of destination nodes (items)
+        self._check_write_index()
         self._settings = AppSettings(settings if settings is not None else {})
         _set_resource_limits(self._settings, SpineEngine._resource_limit_lock)
         enable_persistent_process_creation()
         self._project_dir = project_dir
         project_item_loader = ProjectItemLoader()
         self._executable_item_classes = project_item_loader.load_executable_item_classes(items_module_name)
         if specifications is None:
             specifications = {}
         self._item_specifications = self._make_item_specifications(
             specifications, project_item_loader, items_module_name
         )
-        self._solid_names = {item_name: str(i) for i, item_name in enumerate(items)}
-        self._item_names = {solid_name: item_name for item_name, solid_name in self._solid_names.items()}
-        if execution_permits is None:
-            execution_permits = {}
-        self._execution_permits = {self._solid_names[name]: permits for name, permits in execution_permits.items()}
-        self._dag = make_dag(node_successors)
+        self._dag = make_dag(edges, self._execution_permits)
         _validate_dag(self._dag)
+        self._dag_nodes = list(self._dag)  # Names of permitted items and their neighbors
         if jumps is None:
             jumps = []
         self._jumps = list(map(Jump.from_dict, jumps))
         validate_jumps(self._jumps, self._dag)
         for x in self._connections + self._jumps:
             x.make_logger(self._queue)
         for x in self._jumps:
             x.set_engine(self)
+        # Mapping of item name to solid name
+        self._solids_by_items = {item_name: str(i) for i, item_name in enumerate(self._dag_nodes)}
+        # Mapping of solid name to item name
+        self._items_by_solids = {solid_name: item_name for item_name, solid_name in self._solids_by_items.items()}
+        # Same as edges but item names are swapped to solid names
         self._back_injectors = {
-            self._solid_names[key]: [self._solid_names[x] for x in value] for key, value in node_successors.items()
+            self._solids_by_items[key]: [self._solids_by_items[x] for x in value] for key, value in edges.items()
         }
         self._forth_injectors = inverted(self._back_injectors)
         self._pipeline = self._make_pipeline()
         self._state = SpineEngineState.SLEEPING
         self._debug = debug
         self._running_items = []
         self._prompt_queues = {}
         self._answered_prompts = {}
         self.resources_per_item = {}  # Tuples of (forward resources, backward resources) from last execution
         self._timestamp = create_timestamp()
         self._db_server_manager_queue = None
         self._thread = threading.Thread(target=self.run)
         self._event_stream = self._get_event_stream()
-        self._multiprocess_manager = mp.Manager()
+
+    def _descendants(self, name):
+        """Yields descendant item names.
+
+        Args:
+            name (str): name of the project item whose descendants to collect
+
+        Yields:
+            str: descendant name
+        """
+        for c in self._connections_by_source.get(name, ()):
+            yield c.destination
+            yield from self._descendants(c.destination)
+
+    def _check_write_index(self):
+        """Checks if write indexes are valid."""
+        conflicting_by_item = {}
+        for item_name in self._items:
+            conflicting = {}
+            descendants = self._descendants(item_name)
+            for conn in self._connections_by_source.get(item_name, ()):
+                sibling_connections = [
+                    x for x in self._connections_by_destination.get(conn.destination, []) if x != conn
+                ]
+                conflicting.update(
+                    {
+                        c.source: c.destination
+                        for c in sibling_connections
+                        if c.write_index < conn.write_index and c.source in descendants
+                    }
+                )
+            if conflicting:
+                conflicting_by_item[item_name] = conflicting
+        rows = []
+        for item_name, conflicting in conflicting_by_item.items():
+            row = []
+            for other_item_name, dest in conflicting.items():
+                row.append(f"{other_item_name}, but {other_item_name} is set to write ealier to {dest}")
+            if row:
+                rows.append(f"Item {item_name} cannot execute because it is a dependency to " + ", ".join(row))
+        msg = "\n".join(rows)
+        if msg:
+            raise EngineInitFailed(msg)
+
+    def _validate_and_sort_connections(self):
+        """Checks and sorts Connections by source and destination.
+
+        Raises:
+            EngineInitFailed: If connection is not ready
+        """
+        for connection in self._connections:
+            if not connection.ready_to_execute():
+                notifications = " ".join(connection.notifications())
+                raise EngineInitFailed(f"Link {connection.name} is not ready for execution. {notifications}")
+            source, destination = connection.source, connection.destination
+            self._connections_by_source.setdefault(source, list()).append(connection)
+            self._connections_by_destination.setdefault(destination, list()).append(connection)
 
     def _make_item_specifications(self, specifications, project_item_loader, items_module_name):
         """Instantiates item specifications.
 
         Args:
             specifications (dict): A mapping from item type to list of specification dicts.
             project_item_loader (ProjectItemLoader): loader instance
             items_module_name (str): name of the Python module that contains the project items
 
         Returns:
-            dict: mapping from item type to a dict that maps specification names to specification instances
+            dict: Mapping from item type to a dict that maps specification names to specification instances
         """
         specification_factories = project_item_loader.load_item_specification_factories(items_module_name)
         item_specifications = {}
         for item_type, spec_dicts in specifications.items():
             factory = specification_factories.get(item_type)
             if factory is None:
                 continue
@@ -219,19 +270,19 @@
         executable_item_class = self._executable_item_classes[item_type]
         return executable_item_class.from_dict(
             item_dict, item_name, self._project_dir, self._settings, self._item_specifications, logger
         )
 
     def get_event(self):
         """Returns the next event in the stream. Calling this after receiving the event of type "dag_exec_finished"
-        will raise StopIterationError.
-        """
+        will raise StopIterationError."""
         return next(self._event_stream)
 
     def state(self):
+        """Returns Spine Engine state."""
         return self._state
 
     def _get_event_stream(self):
         """Yields events (event_type, event_data).
 
         TODO: Describe the events in depth.
 
@@ -247,49 +298,49 @@
         self._thread.join()
 
     def answer_prompt(self, item_name, accepted):
         """Answers the prompt for the specified item, either accepting or rejecting it."""
         self._prompt_queues[item_name].put(accepted)
 
     def wait(self):
+        """Waits until engine execution has finished."""
         if self._thread.is_alive():
             self._thread.join()
-        self._multiprocess_manager.shutdown()
 
     def run(self):
-        """Runs this engine."""
+        """Starts db server manager the engine."""
         with db_server_manager() as self._db_server_manager_queue:
             self._do_run()
 
     def _do_run(self):
+        """Runs this engine."""
         self._state = SpineEngineState.RUNNING
         run_config = {
             "loggers": {"console": {"config": {"log_level": "CRITICAL"}}},
             "execution": {"multithread": {"config": {}}},
         }
         for event in execute_pipeline_iterator(self._pipeline, run_config=run_config):
             self._process_event(event)
         if self._state == SpineEngineState.RUNNING:
             self._state = SpineEngineState.COMPLETED
         self._queue.put(("dag_exec_finished", str(self._state)))
 
     def _process_event(self, event):
-        """
-        Processes events from a pipeline.
+        """Processes events from a pipeline.
 
         Args:
             event (DagsterEvent): an event
         """
         if event.event_type == DagsterEventType.STEP_START:
             direction, _, solid_name = event.solid_name.partition("_")
-            item_name = self._item_names[solid_name]
+            item_name = self._items_by_solids[solid_name]
             self._queue.put(('exec_started', {"item_name": item_name, "direction": direction}))
         elif event.event_type == DagsterEventType.STEP_FAILURE and self._state != SpineEngineState.USER_STOPPED:
             direction, _, solid_name = event.solid_name.partition("_")
-            item_name = self._item_names[solid_name]
+            item_name = self._items_by_solids[solid_name]
             self._state = SpineEngineState.FAILED
             self._queue.put(
                 (
                     'exec_finished',
                     {
                         "item_name": item_name,
                         "direction": direction,
@@ -304,16 +355,16 @@
                 print("".join(error.stack + [error.message]))
                 print("(reported by SpineEngine in debug mode)")
         elif event.event_type == DagsterEventType.STEP_SUCCESS:
             # Notify Toolbox here when BACKWARD execution has finished
             direction, _, solid_name = event.solid_name.partition("_")
             if direction != "BACKWARD":
                 return
-            item_name = self._item_names[solid_name]
-            if not self._execution_permits[solid_name]:
+            item_name = self._items_by_solids[solid_name]
+            if not self._execution_permits[item_name]:
                 item_finish_state = ItemExecutionFinishState.EXCLUDED
             else:
                 item_finish_state = ItemExecutionFinishState.SUCCESS
             self._queue.put(
                 (
                     'exec_finished',
                     {
@@ -325,15 +376,15 @@
                 )
             )
         elif event.event_type == DagsterEventType.ASSET_MATERIALIZATION:
             # Notify Toolbox here when FORWARD execution has finished
             direction, _, solid_name = event.solid_name.partition("_")
             if direction != "FORWARD":
                 return
-            item_name = self._item_names[solid_name]
+            item_name = self._items_by_solids[solid_name]
             state_value = event.asset_key.path[0]
             item_finish_state = ItemExecutionFinishState[state_value]
             self._queue.put(
                 (
                     'exec_finished',
                     {
                         "item_name": item_name,
@@ -349,37 +400,37 @@
         self._state = SpineEngineState.USER_STOPPED
         disable_persistent_process_creation()
         for item in self._running_items:
             self._stop_item(item)
         self._queue.put(("dag_exec_finished", str(self._state)))
 
     def _stop_item(self, item):
+        """Stops given project item."""
         item.stop_execution()
         self._queue.put(
             (
                 'exec_finished',
                 {
                     "item_name": item.name,
                     "direction": str(ED.FORWARD),
                     "state": str(self._state),
                     "item_state": ItemExecutionFinishState.STOPPED,
                 },
             )
         )
 
     def _make_pipeline(self):
-        """
-        Returns a _JumpPipelineDefinition for executing this engine.
+        """Returns a _JumpPipelineDefinition for executing this engine.
 
         Returns:
             _JumpPipelineDefinition
         """
         solid_defs = [
             make_solid_def(item_name)
-            for item_name in self._items
+            for item_name in self._dag_nodes
             for make_solid_def in (self._make_forward_solid_def, self._make_backward_solid_def)
         ]
         dependencies = self._make_dependencies()
         mode_defs = [
             ModeDefinition(
                 executor_defs=default_executors + [multithread_executor],
                 resource_defs={"io_manager": shared_memory_io_manager},
@@ -397,17 +448,17 @@
             dict
         """
         for jump in self._jumps:
             src, dst = jump.source, jump.destination
             jump.item_names = {dst, src}
             for path in nx.all_simple_paths(self._dag, dst, src):
                 jump.item_names.update(path)
-            jump.solid_names = {f"{ED.FORWARD}_{self._solid_names[n]}" for n in jump.item_names}
-            jump.source_solid = f"{ED.FORWARD}_{self._solid_names[src]}"
-            jump.destination_solid = f"{ED.BACKWARD}_{self._solid_names[dst]}"
+            jump.solid_names = {f"{ED.FORWARD}_{self._solids_by_items[n]}" for n in jump.item_names}
+            jump.source_solid = f"{ED.FORWARD}_{self._solids_by_items[src]}"
+            jump.destination_solid = f"{ED.BACKWARD}_{self._solids_by_items[dst]}"
 
     def _make_backward_solid_def(self, item_name):
         """Returns a SolidDefinition for executing the given item in the backward sweep.
 
         Args:
             item_name (str): The project item that gets executed by the solid.
         """
@@ -422,15 +473,15 @@
             for r in resources:
                 r.metadata["db_server_manager_queue"] = self._db_server_manager_queue
             yield Output(value=resources, output_name=f"{ED.BACKWARD}_output")
 
         input_defs = []
         output_defs = [OutputDefinition(name=f"{ED.BACKWARD}_output")]
         return SolidDefinition(
-            name=f"{ED.BACKWARD}_{self._solid_names[item_name]}",
+            name=f"{ED.BACKWARD}_{self._solids_by_items[item_name]}",
             input_defs=input_defs,
             compute_fn=compute_fn,
             output_defs=output_defs,
         )
 
     def _make_forward_solid_def(self, item_name):
         """Returns a SolidDefinition for executing the given item.
@@ -464,22 +515,22 @@
             if output_resource_stacks:
                 yield Output(value=output_resource_stacks, output_name=f"{ED.FORWARD}_output")
             for conn in self._connections_by_source.get(item_name, []):
                 conn.visit_source()
 
         input_defs = [
             InputDefinition(name=f"{ED.FORWARD}_input_from_{inj}")
-            for inj in self._forth_injectors.get(self._solid_names[item_name], [])
+            for inj in self._forth_injectors.get(self._solids_by_items[item_name], [])
         ] + [
             InputDefinition(name=f"{ED.BACKWARD}_input_from_{inj}")
-            for inj in self._back_injectors.get(self._solid_names[item_name], [])
+            for inj in self._back_injectors.get(self._solids_by_items[item_name], [])
         ]
         output_defs = [OutputDefinition(name=f"{ED.FORWARD}_output")]
         return SolidDefinition(
-            name=f"{ED.FORWARD}_{self._solid_names[item_name]}",
+            name=f"{ED.FORWARD}_{self._solids_by_items[item_name]}",
             input_defs=input_defs,
             compute_fn=compute_fn,
             output_defs=output_defs,
         )
 
     def _execute_item(self, context, item_name, forward_resource_stacks, backward_resources):
         """Executes the given item using the given forward resource stacks and backward resources.
@@ -501,38 +552,39 @@
 
         Returns:
             ItemExecutionFinishState
             list(tuple(ProjectItemResource))
         """
         item = self.make_item(item_name, ED.NONE)
         if not item.ready_to_execute(self._settings):
-            if not self._execution_permits[self._solid_names[item_name]]:
+            if not self._execution_permits[item_name]:
                 return ItemExecutionFinishState.EXCLUDED, []
             context.log.error(f"compute_fn() FAILURE with '{item_name}', not ready for forward execution")
             return ItemExecutionFinishState.FAILURE, []
         success = [ItemExecutionFinishState.NEVER_FINISHED]
         output_resources_list = []
         threads = []
         resources_iterator = self._filtered_resources_iterator(
             item_name, forward_resource_stacks, backward_resources, self._timestamp
         )
-        item_lock = self._multiprocess_manager.Lock()
-        for flt_fwd_resources, flt_bwd_resources, filter_id in resources_iterator:
-            self.resources_per_item[item_name] = (flt_fwd_resources, flt_bwd_resources)
-            item = self.make_item(item_name, ED.FORWARD)
-            item.filter_id = filter_id
-            thread = threading.Thread(
-                target=self._execute_item_filtered,
-                args=(item, flt_fwd_resources, flt_bwd_resources, output_resources_list, item_lock, success),
-            )
-            threads.append(thread)
-        for thread in threads:
-            thread.start()
-        for thread in threads:
-            thread.join()
+        with mp.Manager() as multiprocess_manager:
+            item_lock = multiprocess_manager.Lock()
+            for flt_fwd_resources, flt_bwd_resources, filter_id in resources_iterator:
+                self.resources_per_item[item_name] = (flt_fwd_resources, flt_bwd_resources)
+                item = self.make_item(item_name, ED.FORWARD)
+                item.filter_id = filter_id
+                thread = threading.Thread(
+                    target=self._execute_item_filtered,
+                    args=(item, flt_fwd_resources, flt_bwd_resources, output_resources_list, item_lock, success),
+                )
+                threads.append(thread)
+            for thread in threads:
+                thread.start()
+            for thread in threads:
+                thread.join()
         if success[0] == ItemExecutionFinishState.FAILURE:
             context.log.error(f"compute_fn() FAILURE with {item_name}, failed to execute")
             raise Failure()
         for resources in output_resources_list:
             for connection in self._connections_by_source.get(item_name, []):
                 connection.receive_resources_from_source(resources)
         return success[0], output_resources_list
@@ -548,15 +600,15 @@
             filtered_backward_resources (list(ProjectItemResource))
             output_resources_list (list(list(ProjectItemResource))): A list to append the output resources
                 generated by the item.
             item_lock (mp.Lock): Shared lock for parallel executions.
             success (list): A list of one element, to write the outcome of the execution.
         """
         self._running_items.append(item)
-        if self._execution_permits[self._solid_names[item.name]]:
+        if self._execution_permits[item.name]:
             item_finish_state = item.execute(filtered_forward_resources, filtered_backward_resources, item_lock)
             item.finish_execution(item_finish_state)
         else:
             item.exclude_execution(filtered_forward_resources, filtered_backward_resources, item_lock)
             item_finish_state = ItemExecutionFinishState.EXCLUDED
         filter_stack = sum((r.metadata.get("filter_stack", ()) for r in filtered_forward_resources), ())
         output_resources = item.output_resources(ED.FORWARD)
@@ -703,15 +755,15 @@
         resources_by_provider = {}
         for r in resources:
             resources_by_provider.setdefault(r.provider_name, list()).append(r)
         for c in connections:
             resources_from_destination = resources_by_provider.get(c.destination)
             if resources_from_destination is None:
                 continue
-            if self._execution_permits[self._solid_names[item_name]]:
+            if self._execution_permits[item_name]:
                 c.clean_up_backward_resources(resources_from_destination)
             sibling_connections = [x for x in self._connections_by_destination.get(c.destination, []) if x != c]
             resources_by_provider[c.destination] = c.convert_backward_resources(
                 resources_from_destination, sibling_connections
             )
         return [r for resources in resources_by_provider.values() for r in resources]
```

### Comparing `spine_engine-0.21.0/spine_engine/utils/__init__.py` & `spine_engine-0.22.0/spine_engine/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `spine_engine-0.21.0/spine_engine/utils/command_line_arguments.py` & `spine_engine-0.22.0/spine_engine/utils/command_line_arguments.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Split command line arguments.
 
-:authors: P. Savolainen (VTT)
-:date:   10.1.2018
 """
 
 
 def split_cmdline_args(arg_string):
     """
     Splits a string of command line arguments into a list of tokens.
```

### Comparing `spine_engine-0.21.0/spine_engine/utils/execution_resources.py` & `spine_engine-0.22.0/spine_engine/utils/execution_resources.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Utilities for managing execution resources such as processes.
 
-:authors: A. Soininen (VTT)
-:date:    9.11.2021
 """
 import threading
 
 
 class ResourceSemaphore:
     """A bit more flexible semaphore than the one found in the standard threading module."""
```

### Comparing `spine_engine-0.21.0/spine_engine/utils/helpers.py` & `spine_engine-0.22.0/spine_engine/utils/helpers.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,27 +8,24 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Helpers functions and classes.
 
-:authors: M. Marin (KTH)
-:date:   20.11.2019
 """
 import os
 import sys
 import datetime
 import time
 import json
 from pathlib import Path
 from enum import Enum, auto, unique
 import networkx
 from jupyter_client.kernelspec import find_kernel_specs
-
 from spinedb_api.spine_io.gdx_utils import find_gams_directory
 from ..config import PYTHON_EXECUTABLE, JULIA_EXECUTABLE, GAMS_EXECUTABLE, EMBEDDED_PYTHON
 
 
 @unique
 class ExecutionDirection(Enum):
     FORWARD = auto()
@@ -246,30 +243,87 @@
         julia = resolve_executable_from_path(JULIA_EXECUTABLE)
         if julia == "":
             return None
     project = settings.value("appSettings/juliaProjectPath", defaultValue="")
     return julia, project
 
 
-def make_dag(node_successors):
-    """Builds a DAG from node successors.
+def make_connections(connections, execution_permits):
+    """Returns a list of Connections based on permitted
+    items. Creates Connections only for connections that
+    are coming from permitted items or leaving from
+    permitted items.
+
+    Args:
+        connections (list(Connection): Serialized connections in the DAG
+        execution_permits (dict):
+
+    Returns:
+        list: List of permitted Connections or an empty list if the DAG contains no connections
+    """
+    if not connections:
+        return list()
+    # List of item names that are permitted, i.e. selected for execution
+    permitted_items = [n for n, n_permitted in execution_permits.items() if n_permitted]
+    connections = connections_to_selected_items(connections, permitted_items)
+    return connections
+
+
+def connections_to_selected_items(connections, selected_items):
+    """Returns a list of Connections that have a permitted item
+    as its source or destination item.
+
+    Args:
+        connections (list(Connection): List of Connections
+        selected_items (list): List of project item names
+
+    returns:
+        list(Connection): Connections allowed in the current DAG
+    """
+    return [conn for conn in connections if conn.source in selected_items or conn.destination in selected_items]
+
+
+def dag_edges(connections):
+    """Collects DAG edges based on Connection instances.
+
+    Args:
+        connections (list(Connection): Connections
+
+    Returns:
+        dict: DAG edges. Mapping of source item (node) to a list of destination items (nodes)
+    """
+    edges = dict()
+    for connection in connections:
+        source, destination = connection.source, connection.destination
+        edges.setdefault(source, list()).append(destination)
+    return edges
+
+
+def make_dag(edges, permitted_nodes=None):
+    """Builds a DAG from edges or if no edges exist, from permitted_nodes.
 
     Args:
-        node_successors (dict): mapping from item name to list of its successors' names
+        edges (dict): Mapping from item name to list of its successors' names
+        permitted_nodes (dict, optional): Mapping from item name to boolean value indicating if item is selected
 
     Returns:
-        DiGraph: directed acyclic graph
+        DiGraph: Directed acyclic graph
     """
     graph = networkx.DiGraph()
-    graph.add_nodes_from(node_successors)
-    for node, successors in node_successors.items():
-        if successors is None:
-            continue
-        for successor in successors:
-            graph.add_edge(node, successor)
+    if not edges:
+        # Make a single node DAG with no edges
+        nodes = [node_name for node_name, permitted in permitted_nodes.items() if permitted]
+        graph.add_nodes_from(nodes)
+    else:
+        graph.add_nodes_from(edges)
+        for node, successors in edges.items():
+            if successors is None:
+                continue
+            for successor in successors:
+                graph.add_edge(node, successor)
     return graph
 
 
 def write_filter_id_file(filter_id, path):
     """Writes filter id to disk.
 
     Args:
```

### Comparing `spine_engine-0.21.0/spine_engine/utils/queue_logger.py` & `spine_engine-0.22.0/spine_engine/utils/queue_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 The QueueLogger class.
 
-:authors: M. Marin (KTH)
-:date:   3.11.2020
 """
 
 
 class _Message:
     def __init__(self, queue, event_type, msg_type, item_name):
         self._queue = queue
         self._event_type = event_type
```

### Comparing `spine_engine-0.21.0/spine_engine/utils/returning_process.py` & `spine_engine-0.22.0/spine_engine/utils/returning_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 The ReturningProcess class.
 
-:authors: M. Marin (KTH)
-:date:    3.11.2020
 """
 
 import multiprocessing as mp
 import threading
 from contextlib import contextmanager
 from enum import Enum, auto, unique
 from .execution_resources import one_shot_process_semaphore
```

### Comparing `spine_engine-0.21.0/spine_engine/utils/serialization.py` & `spine_engine-0.22.0/spine_engine/utils/serialization.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Functions to (de)serialize stuff.
 
-:authors: P. Savolainen (VTT)
-:date:   10.1.2018
 """
 
 import os
 import sys
 import urllib
 from pathlib import Path
 from urllib.parse import urljoin
```

### Comparing `spine_engine-0.21.0/spine_engine/version.py` & `spine_engine-0.22.0/spine_engine/server/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,8 +4,12 @@
 # Spine Engine is free software: you can redistribute it and/or modify it under the terms of the GNU Lesser
 # General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your
 # option) any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Lesser General
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
-__version__ = "0.21.0"
+
+"""
+This package contains Remote Server classes of the Spine Engine.
+
+"""
```

### Comparing `spine_engine-0.21.0/spine_engine.egg-info/SOURCES.txt` & `spine_engine-0.22.0/spine_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spine_engine-0.21.0/tests/test_load_project_items.py` & `spine_engine-0.22.0/tests/test_load_project_items.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 # Public License for more details. You should have received a copy of the GNU Lesser General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 ######################################################################################################################
 
 """
 Unit tests for `load_project_items` module.
 
-:author: A. Soininen (VTT)
-:date:   11.2.2021
 """
 import os.path
 import unittest
 import sys
 from spine_engine.load_project_items import load_executable_item_classes, load_item_specification_factories
 from spine_engine.project_item.executable_item_base import ExecutableItemBase
 from spine_engine.project_item.project_item_specification_factory import ProjectItemSpecificationFactory
```

### Comparing `spine_engine-0.21.0/tests/test_spine_engine.py` & `spine_engine-0.22.0/tests/test_spine_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 
 """
 Unit tests for `spine_engine` module.
 
 Inspired from tests for spinetoolbox.ExecutionInstance and spinetoolbox.ResourceMap,
 and intended to supersede them.
 
-:author: M. Marin (KTH)
-:date:   11.9.2019
 """
 import os.path
 import sys
 from tempfile import TemporaryDirectory
 import unittest
 from unittest.mock import MagicMock, NonCallableMagicMock, call, patch
 
@@ -701,33 +699,29 @@
 
     def test_self_jump_succeeds(self):
         mock_item = self._mock_item("item", resources_forward=[], resources_backward=[])
         items = {"item": mock_item}
         connections = []
         jumps = [Jump("item", "bottom", "item", "top", self._LOOP_TWICE).to_dict()]
         execution_permits = {"item": True}
-        with patch("spine_engine.spine_engine.mp.Manager") as mock_multiprocessing_manager:
-            mock_lock = object()
+        mock_lock = object()
 
-            class MockLockConstructor:
-                def Lock(self):
-                    return mock_lock
-
-            mock_multiprocessing_manager.return_value = MockLockConstructor()
-            engine = SpineEngine(
-                items=items,
-                connections=connections,
-                jumps=jumps,
-                execution_permits=execution_permits,
-                items_module_name="items_module",
-            )
-            engine.make_item = lambda name, direction: engine._items[name]
-            engine.run()
-            self.assertEqual(mock_item.execute.call_args_list, 2 * [call([], [], mock_lock)])
-            self.assertEqual(engine.state(), SpineEngineState.COMPLETED)
+        engine = SpineEngine(
+            items=items,
+            connections=connections,
+            jumps=jumps,
+            execution_permits=execution_permits,
+            items_module_name="items_module",
+        )
+        engine.make_item = lambda name, direction: engine._items[name]
+        engine.run()
+        lock_1 = mock_item.execute.call_args_list[0].args[-1]
+        lock_2 = mock_item.execute.call_args_list[1].args[-1]
+        self.assertEqual(mock_item.execute.call_args_list, [call([], [], lock_1), call([], [], lock_2)])
+        self.assertEqual(engine.state(), SpineEngineState.COMPLETED)
 
     @unittest.skip("Hangs because something's not right in SpineDBServer")
     def test_jump_resources_get_passed_correctly(self):
         resource_fw_a = _make_url_resource("db:///fw_a")
         resource_bw_a = _make_url_resource("db:///bw_a")
         item_a = self._mock_item("a", resources_forward=[resource_fw_a], resources_backward=[resource_bw_a])
         resource_fw_b = _make_url_resource("db:///fw_b")
@@ -821,16 +815,16 @@
                     self.assertEqual(clear_filter_configs(resource.url), expected_resource.url)
                     for key, value in expected_resource.metadata.items():
                         self.assertEqual(resource.metadata[key], value)
 
 
 class TestValidateSingleJump(unittest.TestCase):
     def test_bug(self):
-        node_successors = {"a": ["b"], "b": ["c"], "c": "d"}
-        dag = make_dag(node_successors)
+        edges = {"a": ["b"], "b": ["c"], "c": "d"}
+        dag = make_dag(edges)
         jumps = [Jump("b", "top", "a", "top"), Jump("d", "top", "c", "top")]
         jump_to_check = jumps[0]
         try:
             validate_single_jump(jump_to_check, jumps, dag)
         except EngineInitFailed:
             self.fail("validate_single_jump shouldn't have raised")
```

