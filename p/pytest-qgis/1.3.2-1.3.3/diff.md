# Comparing `tmp/pytest-qgis-1.3.2.tar.gz` & `tmp/pytest-qgis-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-qgis-1.3.2.tar", last modified: Sun Jun 26 19:32:03 2022, max compression
+gzip compressed data, was "pytest-qgis-1.3.3.tar", last modified: Wed May 31 14:42:19 2023, max compression
```

## Comparing `pytest-qgis-1.3.2.tar` & `pytest-qgis-1.3.3.tar`

### file list

```diff
@@ -1,51 +1,28 @@
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2022-06-26 19:32:03.056440 pytest-qgis-1.3.2/
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2022-06-26 19:32:03.053107 pytest-qgis-1.3.2/.github/
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2022-06-26 19:32:03.056440 pytest-qgis-1.3.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 j         (1000) j         (1000)      609 2021-06-24 10:37:24.000000 pytest-qgis-1.3.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 j         (1000) j         (1000)      685 2021-06-24 10:37:24.000000 pytest-qgis-1.3.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2022-06-26 19:32:03.056440 pytest-qgis-1.3.2/.github/workflows/
--rw-r--r--   0 j         (1000) j         (1000)     1631 2022-06-26 19:21:40.000000 pytest-qgis-1.3.2/.github/workflows/ci.yml
--rw-r--r--   0 j         (1000) j         (1000)      969 2021-11-25 11:44:03.000000 pytest-qgis-1.3.2/.gitignore
--rw-r--r--   0 j         (1000) j         (1000)      962 2022-06-26 19:21:40.000000 pytest-qgis-1.3.2/.pre-commit-config.yaml
--rw-r--r--   0 j         (1000) j         (1000)     2068 2022-06-26 19:23:23.000000 pytest-qgis-1.3.2/CHANGELOG.md
--rw-r--r--   0 j         (1000) j         (1000)    18073 2021-08-02 12:19:15.000000 pytest-qgis-1.3.2/LICENSE
--rw-r--r--   0 j         (1000) j         (1000)     7337 2022-06-26 19:32:03.056440 pytest-qgis-1.3.2/PKG-INFO
--rw-r--r--   0 j         (1000) j         (1000)     6008 2022-06-10 12:16:12.000000 pytest-qgis-1.3.2/README.md
--rw-r--r--   0 j         (1000) j         (1000)       82 2022-01-17 12:01:22.000000 pytest-qgis-1.3.2/changelog-ci-config.json
--rw-r--r--   0 j         (1000) j         (1000)      237 2022-02-17 12:13:26.000000 pytest-qgis-1.3.2/requirements-dev.in
--rw-r--r--   0 j         (1000) j         (1000)     3369 2022-02-17 12:13:26.000000 pytest-qgis-1.3.2/requirements-dev.txt
--rw-r--r--   0 j         (1000) j         (1000)      373 2022-01-14 13:20:33.000000 pytest-qgis-1.3.2/requirements.txt
--rw-r--r--   0 j         (1000) j         (1000)     1953 2022-06-26 19:32:03.059773 pytest-qgis-1.3.2/setup.cfg
--rw-r--r--   0 j         (1000) j         (1000)      821 2021-10-07 08:15:53.000000 pytest-qgis-1.3.2/setup.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2022-06-26 19:32:03.053107 pytest-qgis-1.3.2/src/
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2022-06-26 19:32:03.056440 pytest-qgis-1.3.2/src/pytest_qgis/
--rw-r--r--   0 j         (1000) j         (1000)      834 2021-11-22 12:00:29.000000 pytest-qgis-1.3.2/src/pytest_qgis/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)      757 2022-06-26 19:31:14.000000 pytest-qgis-1.3.2/src/pytest_qgis/_version.py
--rw-r--r--   0 j         (1000) j         (1000)     1550 2021-11-19 11:03:43.000000 pytest-qgis-1.3.2/src/pytest_qgis/mock_qgis_classes.py
--rw-r--r--   0 j         (1000) j         (1000)        0 2021-10-07 07:54:28.000000 pytest-qgis-1.3.2/src/pytest_qgis/py.typed
--rw-r--r--   0 j         (1000) j         (1000)    16098 2022-06-17 08:13:58.000000 pytest-qgis-1.3.2/src/pytest_qgis/pytest_qgis.py
--rw-r--r--   0 j         (1000) j         (1000)     4259 2022-01-18 11:43:45.000000 pytest-qgis-1.3.2/src/pytest_qgis/qgis_bot.py
--rw-r--r--   0 j         (1000) j         (1000)     8502 2022-06-26 19:21:40.000000 pytest-qgis-1.3.2/src/pytest_qgis/qgis_interface.py
--rw-r--r--   0 j         (1000) j         (1000)     6074 2022-06-17 08:13:58.000000 pytest-qgis-1.3.2/src/pytest_qgis/utils.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2022-06-26 19:32:03.056440 pytest-qgis-1.3.2/src/pytest_qgis.egg-info/
--rw-r--r--   0 j         (1000) j         (1000)     7337 2022-06-26 19:32:02.000000 pytest-qgis-1.3.2/src/pytest_qgis.egg-info/PKG-INFO
--rw-r--r--   0 j         (1000) j         (1000)     1012 2022-06-26 19:32:02.000000 pytest-qgis-1.3.2/src/pytest_qgis.egg-info/SOURCES.txt
--rw-r--r--   0 j         (1000) j         (1000)        1 2022-06-26 19:32:02.000000 pytest-qgis-1.3.2/src/pytest_qgis.egg-info/dependency_links.txt
--rw-r--r--   0 j         (1000) j         (1000)       38 2022-06-26 19:32:02.000000 pytest-qgis-1.3.2/src/pytest_qgis.egg-info/entry_points.txt
--rw-r--r--   0 j         (1000) j         (1000)       14 2022-06-26 19:32:02.000000 pytest-qgis-1.3.2/src/pytest_qgis.egg-info/requires.txt
--rw-r--r--   0 j         (1000) j         (1000)       12 2022-06-26 19:32:02.000000 pytest-qgis-1.3.2/src/pytest_qgis.egg-info/top_level.txt
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2022-06-26 19:32:03.056440 pytest-qgis-1.3.2/tests/
--rw-r--r--   0 j         (1000) j         (1000)      733 2021-10-07 08:15:53.000000 pytest-qgis-1.3.2/tests/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)     2015 2022-06-17 09:49:02.000000 pytest-qgis-1.3.2/tests/conftest.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2022-06-26 19:32:03.056440 pytest-qgis-1.3.2/tests/data/
--rw-r--r--   0 j         (1000) j         (1000)   147456 2022-02-17 12:13:26.000000 pytest-qgis-1.3.2/tests/data/db.gpkg
--rw-r--r--   0 j         (1000) j         (1000)     1124 2021-11-25 11:44:03.000000 pytest-qgis-1.3.2/tests/data/small_raster.tif
--rw-r--r--   0 j         (1000) j         (1000)     1964 2022-01-18 11:53:02.000000 pytest-qgis-1.3.2/tests/test_ini.py
--rw-r--r--   0 j         (1000) j         (1000)     3708 2022-06-26 19:21:40.000000 pytest-qgis-1.3.2/tests/test_pytest_qgis.py
--rw-r--r--   0 j         (1000) j         (1000)     2019 2022-02-17 12:13:26.000000 pytest-qgis-1.3.2/tests/test_qgis_bot.py
--rw-r--r--   0 j         (1000) j         (1000)     3962 2022-01-18 11:43:45.000000 pytest-qgis-1.3.2/tests/test_utils.py
--rw-r--r--   0 j         (1000) j         (1000)      918 2022-01-18 11:28:21.000000 pytest-qgis-1.3.2/tests/utils.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2022-06-26 19:32:03.056440 pytest-qgis-1.3.2/tests/visual/
--rw-r--r--   0 j         (1000) j         (1000)      733 2022-01-17 09:25:46.000000 pytest-qgis-1.3.2/tests/visual/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)     1939 2022-06-26 19:21:40.000000 pytest-qgis-1.3.2/tests/visual/test_qgis_ui.py
--rw-r--r--   0 j         (1000) j         (1000)     3930 2022-06-26 19:21:40.000000 pytest-qgis-1.3.2/tests/visual/test_show_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:42:19.171253 pytest-qgis-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-05-31 14:42:19.171253 pytest-qgis-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-31 14:42:19.171253 pytest-qgis-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:42:19.167253 pytest-qgis-1.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:42:19.167253 pytest-qgis-1.3.3/src/pytest_qgis/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/src/pytest_qgis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/src/pytest_qgis/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/src/pytest_qgis/mock_qgis_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/src/pytest_qgis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16281 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/src/pytest_qgis/pytest_qgis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/src/pytest_qgis/qgis_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/src/pytest_qgis/qgis_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/src/pytest_qgis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:42:19.171253 pytest-qgis-1.3.3/src/pytest_qgis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7409 2023-05-31 14:42:19.000000 pytest-qgis-1.3.3/src/pytest_qgis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-31 14:42:19.000000 pytest-qgis-1.3.3/src/pytest_qgis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:42:19.000000 pytest-qgis-1.3.3/src/pytest_qgis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-31 14:42:19.000000 pytest-qgis-1.3.3/src/pytest_qgis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 14:42:19.000000 pytest-qgis-1.3.3/src/pytest_qgis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 14:42:19.000000 pytest-qgis-1.3.3/src/pytest_qgis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:42:19.171253 pytest-qgis-1.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/tests/test_ini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/tests/test_pytest_qgis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/tests/test_qgis_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-31 14:42:10.000000 pytest-qgis-1.3.3/tests/test_utils.py
```

### Comparing `pytest-qgis-1.3.2/LICENSE` & `pytest-qgis-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.2/PKG-INFO` & `pytest-qgis-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: pytest-qgis
-Version: 1.3.2
+Version: 1.3.3
 Summary: A pytest plugin for testing QGIS python plugins
 Home-page: https://github.com/GispoCoding/pytest-qgis
 Author: Joona Laine
 Author-email: info@gispo.fi
 Maintainer: Gispo Ltd.
 Maintainer-email: info@gispo.fi
 License: GNU GPL v2.0
 Keywords: pytest,qgis,QGIS,PyQGIS
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
@@ -127,15 +127,15 @@
 * `create_feature_with_attribute_dialog` method to create a feature with default values using QgsAttributeDialog. This
   ensures that all the default values are honored and for example boolean fields are either true or false, not null.
 * `get_qgs_attribute_dialog_widgets_by_name` function can be used to get dictionary of the `QgsAttributeDialog` widgets.
   Check the test [test_qgis_ui.py::test_attribute_dialog_change](./tests/visual/test_qgis_ui.py) for a usage example.
 
 ## Requirements
 
-This pytest plugin requires QGIS >= 3.10 to work.
+This pytest plugin requires QGIS >= 3.16 to work though it might work with older versions.
 
 ## Installation
 
 Install with `pip`:
 
 ```bash
 pip install pytest-qgis
@@ -156,9 +156,7 @@
 ## Contributing
 
 Contributions are very welcome.
 
 ## License
 
 Distributed under the terms of the `GNU GPL v2.0` license, "pytest-qgis" is free and open source software.
-
-
```

### Comparing `pytest-qgis-1.3.2/README.md` & `pytest-qgis-1.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 * `create_feature_with_attribute_dialog` method to create a feature with default values using QgsAttributeDialog. This
   ensures that all the default values are honored and for example boolean fields are either true or false, not null.
 * `get_qgs_attribute_dialog_widgets_by_name` function can be used to get dictionary of the `QgsAttributeDialog` widgets.
   Check the test [test_qgis_ui.py::test_attribute_dialog_change](./tests/visual/test_qgis_ui.py) for a usage example.
 
 ## Requirements
 
-This pytest plugin requires QGIS >= 3.10 to work.
+This pytest plugin requires QGIS >= 3.16 to work though it might work with older versions.
 
 ## Installation
 
 Install with `pip`:
 
 ```bash
 pip install pytest-qgis
```

### Comparing `pytest-qgis-1.3.2/setup.cfg` & `pytest-qgis-1.3.3/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = pytest-qgis
 author = Joona Laine
 author_email = info@gispo.fi
 maintainer = Gispo Ltd.
 maintainer_email = info@gispo.fi
-version = 1.3.2
+version = 1.3.3
 description = A pytest plugin for testing QGIS python plugins
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = pytest,qgis,QGIS,PyQGIS
 url = https://github.com/GispoCoding/pytest-qgis
 license = GNU GPL v2.0
 classifiers = 
@@ -20,27 +20,28 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.5
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Operating System :: OS Independent
 	License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.5
 install_requires = 
-	pytest>=6.2.3
+	pytest>=6.2.5
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 * = 
 	py.typed
@@ -55,17 +56,17 @@
 [flake8]
 max_line_length = 88
 per-file-ignores = 
 	src/pytest_qgis/pytest_qgis.py:QGS105
 	src/pytest_qgis/qgis_interface.py:N802,N803
 	tests/*:ANN001,ANN201
 extend-ignore = 
-	E203, # whitespace before ':'
-	ANN101, # Missing type annotation for self in method
-	PT004 # fixture '{name}' does not return anything, add leading underscore
+	E203,
+	ANN101,
+	PT004
 
 [isort]
 profile = black
 multi_line_output = 3
 
 [mypy]
 disable_error_code = misc
```

### Comparing `pytest-qgis-1.3.2/setup.py` & `pytest-qgis-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.2/src/pytest_qgis/__init__.py` & `pytest-qgis-1.3.3/src/pytest_qgis/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.2/src/pytest_qgis/_version.py` & `pytest-qgis-1.3.3/src/pytest_qgis/_version.py`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.2/src/pytest_qgis/mock_qgis_classes.py` & `pytest-qgis-1.3.3/src/pytest_qgis/mock_qgis_classes.py`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.2/src/pytest_qgis/pytest_qgis.py` & `pytest-qgis-1.3.3/src/pytest_qgis/pytest_qgis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-#  Copyright (C) 2021 pytest-qgis Contributors.
+#  Copyright (C) 2021-2023 pytest-qgis Contributors.
 #
 #
 #  This file is part of pytest-qgis.
 #
 #  pytest-qgis is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 2 of the License, or
@@ -30,15 +30,15 @@
 from unittest import mock
 
 import pytest
 from _pytest.tmpdir import TempPathFactory
 from qgis.core import Qgis, QgsApplication, QgsProject, QgsRectangle, QgsVectorLayer
 from qgis.gui import QgisInterface as QgisInterfaceOrig
 from qgis.gui import QgsGui, QgsLayerTreeMapCanvasBridge, QgsMapCanvas
-from qgis.PyQt import QtCore, QtWidgets
+from qgis.PyQt import QtCore, QtWidgets, sip
 from qgis.PyQt.QtCore import QCoreApplication
 from qgis.PyQt.QtWidgets import QMainWindow, QMessageBox, QWidget
 
 from pytest_qgis.mock_qgis_classes import MockMessageBar
 from pytest_qgis.qgis_bot import QgisBot
 from pytest_qgis.qgis_interface import QgisInterface
 from pytest_qgis.utils import (
@@ -146,14 +146,16 @@
 
 @pytest.fixture(autouse=True, scope="session")
 def qgis_app(request: "SubRequest") -> QgsApplication:
     yield _APP if not request.config._plugin_settings.qgis_init_disabled else None
 
     if not request.config._plugin_settings.qgis_init_disabled:
         assert _APP
+        if not sip.isdeleted(_CANVAS) and _CANVAS is not None:
+            _CANVAS.deleteLater()
         _APP.exitQgis()
 
 
 @pytest.fixture(scope="session")
 def qgis_parent(qgis_app: QgsApplication) -> QWidget:
     return _PARENT
 
@@ -196,14 +198,15 @@
     Initializes new QGIS project by removing layers and relations etc.
 
     Deprecated: use qgis_new_project instead.
     """
     warnings.warn(
         "new_project fixture will be deprecated. " "Use qgis_new_project instead.",
         PendingDeprecationWarning,
+        stacklevel=2,
     )
     qgis_iface.newProject()
 
 
 @pytest.fixture()
 def qgis_world_map_geopackage(tmp_path: Path) -> Path:
     """
@@ -318,20 +321,22 @@
 def _show_qgis_dlg(common_settings: Settings, qgis_parent: QWidget) -> None:
     if common_settings.gui_enabled and not common_settings.qgis_init_disabled:
         qgis_parent.setWindowTitle("Test QGIS dialog opened by Pytest-qgis")
         qgis_parent.show()
     elif not common_settings.gui_enabled:
         warnings.warn(
             "Cannot show QGIS map because the GUI is not enabled. "
-            "Set qgis_qui_enabled=True in pytest.ini."
+            "Set qgis_qui_enabled=True in pytest.ini.",
+            stacklevel=1,
         )
     elif common_settings.qgis_init_disabled:
         warnings.warn(
             "Cannot show QGIS map because QGIS is not initialized. "
-            "Run the tests without --qgis_disable_init to enable QGIS map."
+            "Run the tests without --qgis_disable_init to enable QGIS map.",
+            stacklevel=1,
         )
 
 
 def _configure_qgis_map(
     qgis_app: QgsApplication,
     qgis_iface: QgisInterface,
     qgis_parent: QWidget,
```

### Comparing `pytest-qgis-1.3.2/src/pytest_qgis/qgis_bot.py` & `pytest-qgis-1.3.3/src/pytest_qgis/qgis_bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     """
 
     def __init__(  # noqa: QGS105 # Iface has to be passed in order to
         # ensure compatibility with all QGIS versions >= 3.10
         self,
         iface: QgisInterface,
     ) -> None:
-
         self._iface = iface
 
     def create_feature_with_attribute_dialog(
         self,
         layer: QgsVectorLayer,
         geometry: QgsGeometry,
         attributes: Optional[Dict[str, Any]] = None,
```

### Comparing `pytest-qgis-1.3.2/src/pytest_qgis/qgis_interface.py` & `pytest-qgis-1.3.3/src/pytest_qgis/qgis_interface.py`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.2/src/pytest_qgis/utils.py` & `pytest-qgis-1.3.3/src/pytest_qgis/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.2/src/pytest_qgis.egg-info/PKG-INFO` & `pytest-qgis-1.3.3/src/pytest_qgis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: pytest-qgis
-Version: 1.3.2
+Version: 1.3.3
 Summary: A pytest plugin for testing QGIS python plugins
 Home-page: https://github.com/GispoCoding/pytest-qgis
 Author: Joona Laine
 Author-email: info@gispo.fi
 Maintainer: Gispo Ltd.
 Maintainer-email: info@gispo.fi
 License: GNU GPL v2.0
 Keywords: pytest,qgis,QGIS,PyQGIS
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
@@ -127,15 +127,15 @@
 * `create_feature_with_attribute_dialog` method to create a feature with default values using QgsAttributeDialog. This
   ensures that all the default values are honored and for example boolean fields are either true or false, not null.
 * `get_qgs_attribute_dialog_widgets_by_name` function can be used to get dictionary of the `QgsAttributeDialog` widgets.
   Check the test [test_qgis_ui.py::test_attribute_dialog_change](./tests/visual/test_qgis_ui.py) for a usage example.
 
 ## Requirements
 
-This pytest plugin requires QGIS >= 3.10 to work.
+This pytest plugin requires QGIS >= 3.16 to work though it might work with older versions.
 
 ## Installation
 
 Install with `pip`:
 
 ```bash
 pip install pytest-qgis
@@ -156,9 +156,7 @@
 ## Contributing
 
 Contributions are very welcome.
 
 ## License
 
 Distributed under the terms of the `GNU GPL v2.0` license, "pytest-qgis" is free and open source software.
-
-
```

### Comparing `pytest-qgis-1.3.2/tests/test_ini.py` & `pytest-qgis-1.3.3/tests/test_ini.py`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.2/tests/test_pytest_qgis.py` & `pytest-qgis-1.3.3/tests/test_pytest_qgis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (C) 2021 pytest-qgis Contributors.
+#  Copyright (C) 2021-2023 pytest-qgis Contributors.
 #
 #
 #  This file is part of pytest-qgis.
 #
 #  pytest-qgis is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 2 of the License, or
@@ -24,15 +24,15 @@
 
 from .utils import QGIS_VERSION
 
 if TYPE_CHECKING:
     pass
 
 # DO not use this directly, this is only meant to be used with
-# replace_iface_with_qgis_iface fixtrure
+# replace_iface_with_qgis_iface fixture
 __iface = None
 
 
 @pytest.fixture()
 def replace_iface_with_qgis_iface(qgis_iface):
     global __iface
     __iface = qgis_iface
@@ -115,7 +115,18 @@
 
 def test_iface_toolbar_qtoolbar(qgis_iface):
     name = "test_bar"
     toolbar: QToolBar = QToolBar(name)
     qgis_iface.addToolBar(toolbar)
     assert toolbar.windowTitle() == name
     assert qgis_iface._toolbars == {name: toolbar}
+
+
+def test_canvas_should_be_released(qgis_canvas, layer_polygon, layer_points):
+    """
+    This test will not assert anything but calling zoom methods of qgis_canvas
+    will cause segmentation faults after test session if
+    the canvas is not released properly.
+    """
+    QgsProject.instance().addMapLayer(layer_polygon)
+    QgsProject.instance().addMapLayer(layer_points)
+    qgis_canvas.zoomToFullExtent()
```

### Comparing `pytest-qgis-1.3.2/tests/test_qgis_bot.py` & `pytest-qgis-1.3.3/tests/test_qgis_bot.py`

 * *Files identical despite different names*

### Comparing `pytest-qgis-1.3.2/tests/test_utils.py` & `pytest-qgis-1.3.3/tests/test_utils.py`

 * *Files identical despite different names*

