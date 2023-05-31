# Comparing `tmp/oarepo-model-builder-ui-4.0.3.tar.gz` & `tmp/oarepo-model-builder-ui-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-ui-4.0.3.tar", last modified: Wed May 31 06:30:26 2023, max compression
+gzip compressed data, was "oarepo-model-builder-ui-4.0.4.tar", last modified: Wed May 31 08:43:51 2023, max compression
```

## Comparing `oarepo-model-builder-ui-4.0.3.tar` & `oarepo-model-builder-ui-4.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:30:26.601968 oarepo-model-builder-ui-4.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-31 06:30:26.601968 oarepo-model-builder-ui-4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:30:26.597967 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:30:26.597967 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/builders/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/builders/i18n_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/builders/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/builders/layout_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:30:26.597967 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:30:26.597967 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/datatypes/components/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/datatypes/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/datatypes/components/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:30:26.601968 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/outputs/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/outputs/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:30:26.601968 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:30:26.597967 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-31 06:30:26.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-31 06:30:26.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 06:30:26.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-31 06:30:26.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-31 06:30:26.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-31 06:30:26.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-31 06:30:26.601968 oarepo-model-builder-ui-4.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:43:51.000558 oarepo-model-builder-ui-4.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-31 08:40:30.000000 oarepo-model-builder-ui-4.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-31 08:43:51.000558 oarepo-model-builder-ui-4.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-31 08:40:30.000000 oarepo-model-builder-ui-4.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:43:51.000558 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 08:40:30.000000 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:43:51.000558 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 08:40:30.000000 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-31 08:40:30.000000 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/builders/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-31 08:40:30.000000 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/builders/i18n_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-31 08:40:30.000000 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/builders/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-31 08:40:30.000000 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/builders/layout_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-31 08:40:30.000000 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:43:51.000558 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 08:40:30.000000 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:43:51.000558 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-31 08:40:30.000000 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/datatypes/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-31 08:40:30.000000 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/datatypes/components/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:43:51.000558 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-31 08:40:30.000000 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/outputs/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-31 08:40:30.000000 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/outputs/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:43:51.000558 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-31 08:40:30.000000 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 08:43:51.000558 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-31 08:43:50.000000 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-31 08:43:50.000000 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 08:43:50.000000 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-31 08:43:50.000000 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-31 08:43:50.000000 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-31 08:43:50.000000 oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 08:40:30.000000 oarepo-model-builder-ui-4.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-31 08:43:51.004558 oarepo-model-builder-ui-4.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 08:40:30.000000 oarepo-model-builder-ui-4.0.4/setup.py
```

### Comparing `oarepo-model-builder-ui-4.0.3/PKG-INFO` & `oarepo-model-builder-ui-4.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-ui
-Version: 4.0.3
+Version: 4.0.4
 Summary: Model builder plugin for oarepo-ui
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 <!--
  Copyright (c) 2022 CESNET
```

### Comparing `oarepo-model-builder-ui-4.0.3/README.md` & `oarepo-model-builder-ui-4.0.4/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/builders/i18n_setup_cfg.py` & `oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/builders/i18n_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/builders/layout.py` & `oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/builders/layout.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/builders/layout_setup_cfg.py` & `oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/builders/layout_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/datatypes/components/model.py` & `oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/datatypes/components/model.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/outputs/i18n.py` & `oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/outputs/i18n.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/outputs/layout.py` & `oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui/outputs/layout.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui.egg-info/PKG-INFO` & `oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-ui
-Version: 4.0.3
+Version: 4.0.4
 Summary: Model builder plugin for oarepo-ui
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 <!--
  Copyright (c) 2022 CESNET
```

### Comparing `oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui.egg-info/SOURCES.txt` & `oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui.egg-info/entry_points.txt` & `oarepo-model-builder-ui-4.0.4/oarepo_model_builder_ui.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.3/setup.cfg` & `oarepo-model-builder-ui-4.0.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-ui
-version = 4.0.3
+version = 4.0.4
 description = Model builder plugin for oarepo-ui
 authors = 
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

