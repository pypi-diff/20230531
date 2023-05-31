# Comparing `tmp/talisman-interfaces-0.3.3.tar.gz` & `tmp/talisman-interfaces-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talisman-interfaces-0.3.3.tar", last modified: Wed May 24 09:54:00 2023, max compression
+gzip compressed data, was "talisman-interfaces-0.4.0.tar", last modified: Wed Apr 12 08:26:31 2023, max compression
```

## Comparing `talisman-interfaces-0.3.3.tar` & `talisman-interfaces-0.4.0.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:54:00.837344 talisman-interfaces-0.3.3/
--rw-r--r--   0 root         (0) root         (0)      698 2023-05-24 09:54:00.837344 talisman-interfaces-0.3.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:53:57.000000 talisman-interfaces-0.3.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)        5 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/VERSION
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 09:54:00.837344 talisman-interfaces-0.3.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1301 2023-05-10 13:39:53.000000 talisman-interfaces-0.3.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:54:00.825344 talisman-interfaces-0.3.3/talisman_interfaces.egg-info/
--rw-r--r--   0 root         (0) root         (0)      698 2023-05-24 09:54:00.000000 talisman-interfaces-0.3.3/talisman_interfaces.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1873 2023-05-24 09:54:00.000000 talisman-interfaces-0.3.3/talisman_interfaces.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 09:54:00.000000 talisman-interfaces-0.3.3/talisman_interfaces.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-05-24 09:54:00.000000 talisman-interfaces-0.3.3/talisman_interfaces.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-24 09:54:00.000000 talisman-interfaces-0.3.3/talisman_interfaces.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:54:00.825344 talisman-interfaces-0.3.3/tp_interfaces/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:53:57.000000 talisman-interfaces-0.3.3/tp_interfaces/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:54:00.825344 talisman-interfaces-0.3.3/tp_interfaces/abstract/
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/abstract/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:54:00.825344 talisman-interfaces-0.3.3/tp_interfaces/abstract/configuration/
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/abstract/configuration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/abstract/configuration/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:54:00.829344 talisman-interfaces-0.3.3/tp_interfaces/abstract/model/
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/abstract/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/abstract/model/composite.py
--rw-rw-rw-   0 root         (0) root         (0)      339 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/abstract/model/constructable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:54:00.829344 talisman-interfaces-0.3.3/tp_interfaces/abstract/model/merge/
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/abstract/model/merge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      733 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/abstract/model/merge/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1384 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/abstract/model/model.py
--rw-rw-rw-   0 root         (0) root         (0)      765 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/abstract/model/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:54:00.829344 talisman-interfaces-0.3.3/tp_interfaces/abstract/processor/
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/abstract/processor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2317 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/abstract/processor/category.py
--rw-rw-rw-   0 root         (0) root         (0)     1353 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/abstract/processor/processor.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/abstract/processor/trainer.py
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/abstract/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:54:00.833344 talisman-interfaces-0.3.3/tp_interfaces/abstract/updatable/
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/abstract/updatable/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1249 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/abstract/updatable/model.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/abstract/updatable/update.py
--rw-rw-rw-   0 root         (0) root         (0)     1296 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/abstract/updatable/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:54:00.833344 talisman-interfaces-0.3.3/tp_interfaces/helpers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:53:57.000000 talisman-interfaces-0.3.3/tp_interfaces/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1332 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/helpers/batch.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/helpers/io.py
--rw-rw-rw-   0 root         (0) root         (0)     1197 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/helpers/tar_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:54:00.833344 talisman-interfaces-0.3.3/tp_interfaces/knowledge_base/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:53:57.000000 talisman-interfaces-0.3.3/tp_interfaces/knowledge_base/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1601 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/knowledge_base/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2960 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/knowledge_base/kb_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1145 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/knowledge_base/manager.py
--rw-rw-rw-   0 root         (0) root         (0)     1385 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/knowledge_base/stub_kb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:54:00.837344 talisman-interfaces-0.3.3/tp_interfaces/logging/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:53:57.000000 talisman-interfaces-0.3.3/tp_interfaces/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1694 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/logging/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:54:00.837344 talisman-interfaces-0.3.3/tp_interfaces/processors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:53:57.000000 talisman-interfaces-0.3.3/tp_interfaces/processors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3855 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/processors/composite.py
--rw-rw-rw-   0 root         (0) root         (0)     2807 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/processors/updatable_composite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:54:00.837344 talisman-interfaces-0.3.3/tp_interfaces/readers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:53:57.000000 talisman-interfaces-0.3.3/tp_interfaces/readers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/readers/abstract.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:54:00.837344 talisman-interfaces-0.3.3/tp_interfaces/serializers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:53:57.000000 talisman-interfaces-0.3.3/tp_interfaces/serializers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/serializers/abstract.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 09:54:00.837344 talisman-interfaces-0.3.3/tp_interfaces/trainer_cache/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-24 09:53:57.000000 talisman-interfaces-0.3.3/tp_interfaces/trainer_cache/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3970 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/trainer_cache/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2554 2023-05-10 10:50:11.000000 talisman-interfaces-0.3.3/tp_interfaces/trainer_cache/manipulations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.673859 talisman-interfaces-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)      698 2023-04-12 08:26:31.673859 talisman-interfaces-0.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:29.000000 talisman-interfaces-0.4.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-04-11 11:40:07.000000 talisman-interfaces-0.4.0/VERSION
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 08:26:31.673859 talisman-interfaces-0.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1269 2023-04-11 11:40:07.000000 talisman-interfaces-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/talisman_interfaces.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      698 2023-04-12 08:26:31.000000 talisman-interfaces-0.4.0/talisman_interfaces.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-04-12 08:26:31.000000 talisman-interfaces-0.4.0/talisman_interfaces.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 08:26:31.000000 talisman-interfaces-0.4.0/talisman_interfaces.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-04-12 08:26:31.000000 talisman-interfaces-0.4.0/talisman_interfaces.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-12 08:26:31.000000 talisman-interfaces-0.4.0/talisman_interfaces.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:29.000000 talisman-interfaces-0.4.0/tp_interfaces/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/abstract/
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-04-03 07:21:48.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/abstract/configuration/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-04-03 07:21:48.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/configuration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/configuration/factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/abstract/model/
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-04 13:33:04.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/model/composite.py
+-rw-rw-rw-   0 root         (0) root         (0)      339 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/model/constructable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/abstract/model/merge/
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-03 07:21:48.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/model/merge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      733 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/model/merge/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1384 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/model/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      765 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/model/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/abstract/processor/
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-04-03 07:21:48.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/processor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2688 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/processor/category.py
+-rw-rw-rw-   0 root         (0) root         (0)     1638 2023-04-11 11:40:07.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/processor/processor.py
+-rw-rw-rw-   0 root         (0) root         (0)      911 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/processor/trainer.py
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/abstract/updatable/
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-04-03 07:21:48.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/updatable/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1249 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/updatable/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/updatable/update.py
+-rw-rw-rw-   0 root         (0) root         (0)     1296 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/abstract/updatable/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:29.000000 talisman-interfaces-0.4.0/tp_interfaces/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1332 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/helpers/batch.py
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/helpers/io.py
+-rw-rw-rw-   0 root         (0) root         (0)     1197 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/helpers/tar_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/knowledge_base/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:29.000000 talisman-interfaces-0.4.0/tp_interfaces/knowledge_base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7608 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/knowledge_base/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3482 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/knowledge_base/kb_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1145 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/knowledge_base/manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     7744 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/knowledge_base/readers.py
+-rw-rw-rw-   0 root         (0) root         (0)     3540 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/knowledge_base/stub_kb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/logging/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:29.000000 talisman-interfaces-0.4.0/tp_interfaces/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1694 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/logging/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/processors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:29.000000 talisman-interfaces-0.4.0/tp_interfaces/processors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4100 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/processors/composite.py
+-rw-rw-rw-   0 root         (0) root         (0)     2807 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/processors/updatable_composite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.669859 talisman-interfaces-0.4.0/tp_interfaces/readers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:29.000000 talisman-interfaces-0.4.0/tp_interfaces/readers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1486 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/readers/abstract.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.673859 talisman-interfaces-0.4.0/tp_interfaces/serializers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:29.000000 talisman-interfaces-0.4.0/tp_interfaces/serializers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/serializers/abstract.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 08:26:31.673859 talisman-interfaces-0.4.0/tp_interfaces/trainer_cache/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-12 08:26:29.000000 talisman-interfaces-0.4.0/tp_interfaces/trainer_cache/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3970 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/trainer_cache/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2554 2023-04-05 16:40:00.000000 talisman-interfaces-0.4.0/tp_interfaces/trainer_cache/manipulations.py
```

### Comparing `talisman-interfaces-0.3.3/PKG-INFO` & `talisman-interfaces-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-interfaces
-Version: 0.3.3
+Version: 0.4.0
 Summary: Talisman Processor base interfaces
 Author: ISPRAS Talisman NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `talisman-interfaces-0.3.3/setup.py` & `talisman-interfaces-0.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,16 +14,15 @@
     long_description_content_type="text/markdown",
     author='ISPRAS Talisman NLP team',
     author_email='modis@ispras.ru',
     maintainer='Vladimir Mayorov',
     maintainer_email='vmayorov@ispras.ru',
     packages=find_packages(include=['tp_interfaces', 'tp_interfaces.*']),
     install_requires=[
-        'talisman-dm~=1.0.0a7', 'pydantic>=1.9.0', 'more-itertools>=8.12.0',
-        'jsonpath-ng~=1.5.3'
+        'talisman-dm~=0.7.1', 'pydantic>=1.9.0', 'more-itertools>=8.12.0'
     ],
     extras_require={
         'dvc': ['dvc[s3]>=2.8.1']
     },
     data_files=[('', ['VERSION'])],
     python_requires='>=3.6',
     license='Apache Software License',
```

### Comparing `talisman-interfaces-0.3.3/talisman_interfaces.egg-info/PKG-INFO` & `talisman-interfaces-0.4.0/talisman_interfaces.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-interfaces
-Version: 0.3.3
+Version: 0.4.0
 Summary: Talisman Processor base interfaces
 Author: ISPRAS Talisman NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `talisman-interfaces-0.3.3/talisman_interfaces.egg-info/SOURCES.txt` & `talisman-interfaces-0.4.0/talisman_interfaces.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 tp_interfaces/helpers/batch.py
 tp_interfaces/helpers/io.py
 tp_interfaces/helpers/tar_model.py
 tp_interfaces/knowledge_base/__init__.py
 tp_interfaces/knowledge_base/interfaces.py
 tp_interfaces/knowledge_base/kb_schema.py
 tp_interfaces/knowledge_base/manager.py
+tp_interfaces/knowledge_base/readers.py
 tp_interfaces/knowledge_base/stub_kb.py
 tp_interfaces/logging/__init__.py
 tp_interfaces/logging/context.py
 tp_interfaces/processors/__init__.py
 tp_interfaces/processors/composite.py
 tp_interfaces/processors/updatable_composite.py
 tp_interfaces/readers/__init__.py
```

### Comparing `talisman-interfaces-0.3.3/tp_interfaces/abstract/__init__.py` & `talisman-interfaces-0.4.0/tp_interfaces/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.3/tp_interfaces/abstract/model/merge/models.py` & `talisman-interfaces-0.4.0/tp_interfaces/abstract/model/merge/models.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.3/tp_interfaces/abstract/model/model.py` & `talisman-interfaces-0.4.0/tp_interfaces/abstract/model/model.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.3/tp_interfaces/abstract/model/wrapper.py` & `talisman-interfaces-0.4.0/tp_interfaces/abstract/model/wrapper.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.3/tp_interfaces/abstract/processor/category.py` & `talisman-interfaces-0.4.0/tp_interfaces/abstract/processor/category.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 from collections import defaultdict
 from typing import Callable, Dict, Generic, List, Optional, Sequence, Tuple, Type, TypeVar
 
-from tdm import TalismanDocument
+from tdm.abstract.datamodel import AbstractTreeDocumentContent
+from tdm.datamodel import TalismanDocument
 
 from tp_interfaces.abstract.model import AbstractCompositeModel
 from tp_interfaces.abstract.schema import ImmutableBaseModel
 from .processor import AbstractDocumentProcessor
 
+_DocumentContent = TypeVar('_DocumentContent', bound=AbstractTreeDocumentContent)
 _Config = TypeVar('_Config', bound=ImmutableBaseModel)
 _Category = TypeVar('_Category')
 
 
 class AbstractCategoryAwareDocumentProcessor(
-    AbstractCompositeModel[AbstractDocumentProcessor[_Config]],
-    AbstractDocumentProcessor[_Config], Generic[_Config, _Category]
+    AbstractCompositeModel[AbstractDocumentProcessor[_Config, _DocumentContent]],
+    AbstractDocumentProcessor[_Config, _DocumentContent], Generic[_Config, _DocumentContent, _Category]
 ):
     def __init__(self,
-                 category2processor: Dict[_Category, AbstractDocumentProcessor[_Config]],
-                 categorizer: Callable[[TalismanDocument], _Category],
-                 default_processor: Optional[AbstractDocumentProcessor[_Config]] = None
+                 category2processor: Dict[_Category, AbstractDocumentProcessor[_Config, _DocumentContent]],
+                 categorizer: Callable[[TalismanDocument[_DocumentContent]], _Category],
+                 default_processor: Optional[AbstractDocumentProcessor[_Config, _DocumentContent]] = None
                  ):
         self._category2processor = dict(category2processor)
         super().__init__(self._category2processor.values())
-        self._models: Tuple[AbstractDocumentProcessor[_Config], ...]
+        self._models: Tuple[AbstractDocumentProcessor[_Config, _DocumentContent], ...]
         self._categorizer = categorizer
         self._default = default_processor
 
-    def process_doc(self, document: TalismanDocument, config: _Config) -> TalismanDocument:
+    def process_doc(self, document: TalismanDocument[_DocumentContent], config: _Config) -> TalismanDocument[_DocumentContent]:
         return self.process_docs([document], config)[0]
 
-    def process_docs(self, documents: Sequence[TalismanDocument], config: _Config) \
-            -> Tuple[TalismanDocument, ...]:
+    def process_docs(self, documents: Sequence[TalismanDocument[_DocumentContent]], config: _Config) \
+            -> Tuple[TalismanDocument[_DocumentContent], ...]:
         category2doc = defaultdict(dict)
-        processed_docs: List[Optional[TalismanDocument]] = [None] * len(documents)
+        processed_docs: List[Optional[TalismanDocument[_DocumentContent]]] = [None] * len(documents)
 
         for i, doc in enumerate(documents):
             category = self._categorizer(doc)
             category2doc[category].update({i: doc})
 
         for category, docs in category2doc.items():
             processor = self._category2processor.get(category, self._default)
```

### Comparing `talisman-interfaces-0.3.3/tp_interfaces/abstract/processor/trainer.py` & `talisman-interfaces-0.4.0/tp_interfaces/abstract/processor/trainer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Dict, Generic, Optional, TypeVar
 
-from tp_interfaces.abstract.model.model import Picklable
 from .processor import AbstractDocumentProcessor
+from ..model.model import Picklable
 
 DEFAULT_CACHE_DIR = Path('trainer_cache')
 
 
 class Cache(Picklable):
     pass
```

### Comparing `talisman-interfaces-0.3.3/tp_interfaces/abstract/updatable/model.py` & `talisman-interfaces-0.4.0/tp_interfaces/abstract/updatable/model.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.3/tp_interfaces/abstract/updatable/wrapper.py` & `talisman-interfaces-0.4.0/tp_interfaces/abstract/updatable/wrapper.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.3/tp_interfaces/helpers/batch.py` & `talisman-interfaces-0.4.0/tp_interfaces/helpers/batch.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.3/tp_interfaces/helpers/io.py` & `talisman-interfaces-0.4.0/tp_interfaces/helpers/io.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.3/tp_interfaces/helpers/tar_model.py` & `talisman-interfaces-0.4.0/tp_interfaces/helpers/tar_model.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.3/tp_interfaces/knowledge_base/interfaces.py` & `talisman-interfaces-0.4.0/tp_interfaces/readers/abstract.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,39 @@
 from abc import ABCMeta, abstractmethod
-from contextlib import AbstractContextManager
-from typing import Generic, Tuple, Type, TypeVar
+from typing import Callable, Dict, Generic, Iterator, Optional, Type, TypeVar, Union
 
-from tdm import TalismanDocument
-from tdm.datamodel.directives import CreateConceptDirective
-from tdm.datamodel.facts import ConceptFact
+from tdm.abstract.datamodel import AbstractFact, AbstractTreeDocumentContent, FactStatus
+from tdm.datamodel import TalismanDocument, TalismanSpan
+from tdm.datamodel.fact import ConceptFact, ValueFact
 
-from tp_interfaces.abstract import ImmutableBaseModel
-from tp_interfaces.knowledge_base.kb_schema import KBSchema
+EntityFactType = Union[Type[ConceptFact], Type[ValueFact]]
+Label2FactType = Dict[str, EntityFactType]
 
-_DMBConfigInterface = TypeVar('_DMBConfigInterface', bound=ImmutableBaseModel)
+_Content = TypeVar('_Content', bound=AbstractTreeDocumentContent)
 
 
-class LoaderKB(AbstractContextManager, metaclass=ABCMeta):
+class AbstractReader(Generic[_Content], metaclass=ABCMeta):
     @abstractmethod
-    def bind_facts_and_load_docs(self, docs: Tuple[TalismanDocument, ...]):
+    def read(self) -> Iterator[TalismanDocument[_Content]]:
         pass
 
-    @property
-    @abstractmethod
-    def schema(self) -> KBSchema:
-        pass
 
-    @abstractmethod
-    def refresh_schema(self):
-        pass
+_AbstractConfigurableReader = TypeVar('_AbstractConfigurableReader', bound='AbstractConfigurableReader')
+
 
+class AbstractConfigurableReader(AbstractReader, Generic[_Content], metaclass=ABCMeta):
     @classmethod
     @abstractmethod
-    def from_config(cls, config: dict) -> 'LoaderKB':
+    def from_config(cls: _AbstractConfigurableReader, config) -> _AbstractConfigurableReader:
         pass
 
 
-class DisambiguationKB(AbstractContextManager, Generic[_DMBConfigInterface], metaclass=ABCMeta):
-    @abstractmethod
-    def get_candidates(self, doc: TalismanDocument, config: _DMBConfigInterface
-                       ) -> Tuple[Tuple[ConceptFact, ...], Tuple[CreateConceptDirective, ...]]:
-        pass
+def label_span2fact(default_type: EntityFactType,
+                    label2facttype: Optional[Label2FactType] = None,
+                    status: FactStatus = FactStatus.APPROVED) \
+        -> Callable[[str, TalismanSpan], AbstractFact]:
+    mapping = dict(label2facttype) if label2facttype is not None else {}
 
-    @property
-    @abstractmethod
-    def config_type(self) -> Type[_DMBConfigInterface]:
-        pass
+    def create_fact(label: str, span: TalismanSpan) -> AbstractFact:
+        return mapping.get(label, default_type)(None, status, label, tuple(), [span])
 
-    @classmethod
-    @abstractmethod
-    def from_config(cls, config: dict) -> 'DisambiguationKB':
-        pass
-
-
-class KB(LoaderKB, DisambiguationKB, Generic[_DMBConfigInterface], metaclass=ABCMeta):
-    @classmethod
-    @abstractmethod
-    def from_config(cls, config: dict) -> 'KB':
-        pass
+    return create_fact
```

### Comparing `talisman-interfaces-0.3.3/tp_interfaces/knowledge_base/manager.py` & `talisman-interfaces-0.4.0/tp_interfaces/knowledge_base/manager.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.3/tp_interfaces/logging/context.py` & `talisman-interfaces-0.4.0/tp_interfaces/logging/context.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.3/tp_interfaces/processors/composite.py` & `talisman-interfaces-0.4.0/tp_interfaces/processors/composite.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import operator
 from operator import attrgetter
 from typing import Iterable, Optional, Sequence, Tuple, Type, TypeVar
 
 from pydantic import BaseModel, create_model
-from tdm import TalismanDocument
+from tdm.abstract.datamodel import AbstractTreeDocumentContent
+from tdm.datamodel import TalismanDocument
 
 from tp_interfaces.abstract import AbstractCompositeModel, AbstractDocumentProcessor, ImmutableBaseModel
 from tp_interfaces.abstract.model.merge import MergeModel
 
+_DocumentContent = TypeVar('_DocumentContent', bound=AbstractTreeDocumentContent)
 _Config = TypeVar('_Config', bound=BaseModel)
 
 
 class SequentialConfig(ImmutableBaseModel):
     pass
 
 
 class SequentialDocumentProcessor(
     AbstractCompositeModel[AbstractDocumentProcessor],
-    AbstractDocumentProcessor[SequentialConfig]
+    AbstractDocumentProcessor[SequentialConfig, _DocumentContent]
 ):
 
     def __init__(self, processors: Iterable[Tuple[str, AbstractDocumentProcessor]]):
         processors = tuple(processors)
         AbstractCompositeModel[AbstractDocumentProcessor].__init__(self, map(operator.itemgetter(1), processors))
         AbstractDocumentProcessor.__init__(self)
 
@@ -45,22 +47,22 @@
         else:
             if any(not name for name in config_types):
                 raise ValueError(f"empty model name couldn't be processed")
             self._config_type = create_model('RuntimeSequentialConfig', **config_types, __base__=SequentialConfig)
 
         self._config_extractors = tuple(config_extractors)
 
-    def process_doc(self, document: TalismanDocument, config: _Config) -> TalismanDocument:
+    def process_doc(self, document: TalismanDocument[_DocumentContent], config: _Config) -> TalismanDocument[_DocumentContent]:
         return self.process_docs([document], config)[0]
 
     def process_docs(
             self,
-            documents: Sequence[TalismanDocument],
+            documents: Sequence[TalismanDocument[_DocumentContent]],
             config: SequentialConfig
-    ) -> Tuple[TalismanDocument, ...]:
+    ) -> Tuple[TalismanDocument[_DocumentContent], ...]:
         for processor, config_extractor in zip(self._models, self._config_extractors):
             documents = processor.process_docs(documents, config_extractor(config))
         return documents
 
     @property
     def config_type(self) -> Type[SequentialConfig]:
         return self._config_type
```

### Comparing `talisman-interfaces-0.3.3/tp_interfaces/processors/updatable_composite.py` & `talisman-interfaces-0.4.0/tp_interfaces/processors/updatable_composite.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.3/tp_interfaces/trainer_cache/base.py` & `talisman-interfaces-0.4.0/tp_interfaces/trainer_cache/base.py`

 * *Files identical despite different names*

### Comparing `talisman-interfaces-0.3.3/tp_interfaces/trainer_cache/manipulations.py` & `talisman-interfaces-0.4.0/tp_interfaces/trainer_cache/manipulations.py`

 * *Files identical despite different names*

