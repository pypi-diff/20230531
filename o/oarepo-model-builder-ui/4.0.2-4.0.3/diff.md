# Comparing `tmp/oarepo-model-builder-ui-4.0.2.tar.gz` & `tmp/oarepo-model-builder-ui-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-ui-4.0.2.tar", last modified: Tue May 30 20:35:15 2023, max compression
+gzip compressed data, was "oarepo-model-builder-ui-4.0.3.tar", last modified: Wed May 31 06:30:26 2023, max compression
```

## Comparing `oarepo-model-builder-ui-4.0.2.tar` & `oarepo-model-builder-ui-4.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:35:15.401019 oarepo-model-builder-ui-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-30 20:35:15.401019 oarepo-model-builder-ui-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:35:15.401019 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:35:15.401019 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/builders/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/builders/i18n_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/builders/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/builders/layout_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:35:15.401019 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:35:15.401019 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/datatypes/components/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/datatypes/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/datatypes/components/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:35:15.401019 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/outputs/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/outputs/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:35:15.401019 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:35:15.401019 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-30 20:35:15.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-30 20:35:15.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 20:35:15.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-30 20:35:15.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 20:35:15.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-30 20:35:15.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-30 20:35:15.405020 oarepo-model-builder-ui-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:30:26.601968 oarepo-model-builder-ui-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-31 06:30:26.601968 oarepo-model-builder-ui-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:30:26.597967 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:30:26.597967 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/builders/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/builders/i18n_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/builders/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/builders/layout_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:30:26.597967 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:30:26.597967 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/datatypes/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/datatypes/components/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:30:26.601968 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/outputs/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/outputs/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:30:26.601968 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:30:26.597967 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-31 06:30:26.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-31 06:30:26.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 06:30:26.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-31 06:30:26.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-31 06:30:26.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-31 06:30:26.000000 oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-31 06:30:26.601968 oarepo-model-builder-ui-4.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 06:27:32.000000 oarepo-model-builder-ui-4.0.3/setup.py
```

### Comparing `oarepo-model-builder-ui-4.0.2/PKG-INFO` & `oarepo-model-builder-ui-4.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-ui
-Version: 4.0.2
+Version: 4.0.3
 Summary: Model builder plugin for oarepo-ui
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 <!--
  Copyright (c) 2022 CESNET
```

### Comparing `oarepo-model-builder-ui-4.0.2/README.md` & `oarepo-model-builder-ui-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/builders/i18n.py` & `oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/builders/i18n.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/builders/i18n_setup_cfg.py` & `oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/builders/i18n_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/builders/layout.py` & `oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/builders/layout.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/builders/layout_setup_cfg.py` & `oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/builders/layout_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/datatypes/components/__init__.py` & `oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/datatypes/components/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/datatypes/components/model.py` & `oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/datatypes/components/model.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/outputs/i18n.py` & `oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/outputs/i18n.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/outputs/layout.py` & `oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui/outputs/layout.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui.egg-info/PKG-INFO` & `oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-ui
-Version: 4.0.2
+Version: 4.0.3
 Summary: Model builder plugin for oarepo-ui
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 <!--
  Copyright (c) 2022 CESNET
```

### Comparing `oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui.egg-info/SOURCES.txt` & `oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui.egg-info/entry_points.txt` & `oarepo-model-builder-ui-4.0.3/oarepo_model_builder_ui.egg-info/entry_points.txt`

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 [oarepo_model_builder.outputs]
 po = oarepo_model_builder_ui.outputs.i18n:POOutput
 
 [oarepo_model_builder.validation.settings]
 ui-settings = oarepo_model_builder_ui.validation:UISettingsSchema
 
 [oarepo_model_builder.validation.ui.model]
-ui-model = oarepo_model_builder.ui.datatypes.components.model:UISchema
+ui-model = oarepo_model_builder_ui.datatypes.components.model:UISchema
```

### Comparing `oarepo-model-builder-ui-4.0.2/setup.cfg` & `oarepo-model-builder-ui-4.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-ui
-version = 4.0.2
+version = 4.0.3
 description = Model builder plugin for oarepo-ui
 authors = 
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
@@ -27,15 +27,15 @@
 [options.package_data]
 * = *.json, *.rst, *.md, *.json5, *.jinja2
 
 [options.entry_points]
 oarepo_model_builder.validation.settings = 
 	ui-settings = oarepo_model_builder_ui.validation:UISettingsSchema
 oarepo_model_builder.validation.ui.model = 
-	ui-model = oarepo_model_builder.ui.datatypes.components.model:UISchema
+	ui-model = oarepo_model_builder_ui.datatypes.components.model:UISchema
 oarepo_model_builder.datatypes.components = 
 	ui-components = oarepo_model_builder_ui.datatypes.components:components
 oarepo_model_builder.builders.record = 
 	4000-oarepo-i18n = oarepo_model_builder_ui.builders.i18n:InvenioI18nBuilder
 	4010-oarepo-i18n-setup = oarepo_model_builder_ui.builders.i18n_setup_cfg:InvenioI18NSetupCfgBuilder
 	4020-oarepo-ui-layout = oarepo_model_builder_ui.builders.layout:InvenioLayoutBuilder
 	4030-oarepo-ui-layout-setup = oarepo_model_builder_ui.builders.layout_setup_cfg:InvenioLayoutSetupCfgBuilder
```

