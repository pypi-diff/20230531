# Comparing `tmp/schemamodels-0.6.1.tar.gz` & `tmp/schemamodels-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schemamodels-0.6.1.tar", max compression
+gzip compressed data, was "schemamodels-0.7.0.tar", max compression
```

## Comparing `schemamodels-0.6.1.tar` & `schemamodels-0.7.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     2724 2022-12-04 23:32:10.320277 schemamodels-0.6.1/README.md
--rw-r--r--   0        0        0      534 2022-12-08 00:19:36.151972 schemamodels-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     4128 2022-12-08 00:16:40.387973 schemamodels-0.6.1/schemamodels/__init__.py
--rw-r--r--   0        0        0      754 2022-12-08 00:16:40.387973 schemamodels-0.6.1/schemamodels/bases.py
--rw-r--r--   0        0        0        0 2022-12-02 06:38:42.495836 schemamodels-0.6.1/schemamodels/dynamic.py
--rw-r--r--   0        0        0      202 2022-12-05 02:58:35.791952 schemamodels-0.6.1/schemamodels/exceptions.py
--rw-r--r--   0        0        0     3384 2022-12-08 00:20:13.107205 schemamodels-0.6.1/setup.py
--rw-r--r--   0        0        0     3302 2022-12-08 00:20:13.107402 schemamodels-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    32473 2023-05-31 03:33:36.221264 schemamodels-0.7.0/LICENSE
+drwxr-xr-x   0        0        0        0 2023-05-31 03:33:36.221264 schemamodels-0.7.0/LICENSES/
+-rw-r--r--   0        0        0     3135 2023-05-31 03:42:04.157758 schemamodels-0.7.0/README.md
+-rw-r--r--   0        0        0      573 2023-05-31 03:39:42.815743 schemamodels-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     8206 2023-05-31 03:33:36.225264 schemamodels-0.7.0/schemamodels/__init__.py
+-rw-r--r--   0        0        0      848 2023-05-31 03:33:36.225264 schemamodels-0.7.0/schemamodels/bases.py
+-rw-r--r--   0        0        0       93 2023-05-31 03:33:36.225264 schemamodels-0.7.0/schemamodels/dynamic.py
+-rw-r--r--   0        0        0      410 2023-05-31 03:33:36.225264 schemamodels-0.7.0/schemamodels/exceptions.py
+-rw-r--r--   0        0        0     3755 1970-01-01 00:00:00.000000 schemamodels-0.7.0/PKG-INFO
```

### Comparing `schemamodels-0.6.1/README.md` & `schemamodels-0.7.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-# Schema Models
-
-![PyPI](https://img.shields.io/pypi/v/schemamodels?style=for-the-badge) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/schemamodels?style=for-the-badge)
+<!--
+SPDX-FileCopyrightText: 2023 Civic Hacker, LLC
 
-Dynamically created data classes from JSON schemas
+SPDX-License-Identifier: GPL-3.0-or-later
+-->
 
+# Schema Models
 
-Use this library to quickly turn a JSON Schema into a Python dataclass that you can immediately consume.
+![PyPI](https://img.shields.io/pypi/v/schemamodels?style=for-the-badge) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/schemamodels?style=for-the-badge)
+[![REUSE status](https://api.reuse.software/badge/git.fsfe.org/reuse/api)](https://api.reuse.software/info/git.fsfe.org/reuse/api)
 
+Use this library to turn a JSON Schema into a plain 'ol Python dataclass.
 
 ## Installation
 
 Install this package using the usual suspects.
 
 ```
 pip install schemamodels
 ```
 
 ## Usage
 
-Assuming you have a JSON schema like:
+This library **only** supports JSON schemas of `type: object`:
 
 ```json
     {
         "$id": "https://schema.dev/fake-schema.schema.json",
         "$schema": "http://json-schema.org/draft-07/schema#",
         "title": "fake-schema",
         "description": "Blue Blah",
@@ -59,27 +62,34 @@
 your_data_instance = FakeSchema(property_a=2334)  # OK
 
 with pytest.raises(exceptions.ValueTypeViolation):
   your_data_instance = FakeSchema(property_a="hello")
 
 ```
 
-## Rationale
+## Why this library exists
 
 ### The JSON Schema can come from anywhere
 
-Regardless of where the JSON schema originated, it only needs to be valid for the Draft version you care about. There are a number of libraries better suited validating a JSON Schema document. A user of this library would obtain a JSON Schema document using their prefered method (filesystem, remote), then pass it to this library.
+Regardless of where your JSON schema originated, it only needs to be valid for the Draft version you care about. There are a number of libraries better suited validating a JSON Schema document. A user of this library would obtain a JSON Schema document using their prefered method (filesystem, remote), then pass it to this library.
 
 
 ### Just-enough validation
 
-At this time, I'm not interested in validating a JSON Schema. However, there are some basic checks I'd like to have performed _every time_ create a new instance of a object that's designed to _hold_ my data. Also, questions about the quality of the data is out of scope.
+Use this library, if there are some basic checks you'd like performed _every time_ create a new instance data class. Also, questions about the quality of the data is out of scope.
 
 I want to have the confidence that the data has a structure the adhears to the rules provided by a JSON Schema.
 
 I want to be sure that the dictionary exported by these data classes would pass validation checks. The specific tool used to validate an instance of data against the original JSON Schema shouldn't matter.
 
 ### I'm tired of writing Python classes by hand
 
-While I like using Python-classes to write Python declaratively, I think letting JSON Schema drive the data models creates an opportunity to automate.
+While I like using classes to write Python declaratively, I think letting JSON Schema drive the data models creates an opportunity to automate.
 
 When I have a valid JSON Schema, I can create a new Python dataclass with one line of code.
+
+
+## License
+
+This codebase is licensed under the GPLv3+ and therefore the use, inclusion, modification, and distribution of this software is governed by the GPL.
+
+If you are planning to use schemamodels in a commercial product or wish to opt-out of the obligations of the GPL, please reach out to license@civichacker.com.
```

### Comparing `schemamodels-0.6.1/pyproject.toml` & `schemamodels-0.7.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [tool.poetry]
 name = "schemamodels"
-version = "0.6.1"
+version = "0.7.0"
 description = "Dynamically create useful data classes from JSON schemas"
 authors = ["'Jurnell Cockhren' <jurnell@civichacker.com>"]
-license = "LGPL-3.0-or-later"
+license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
-ipython = "^8.7.0"
+ipython = "^8.10.0"
 jsonschema = "^4.17.3"
 vulture = "^2.6"
 flake8 = { version = "^6.0.0", python = ">=3.8.1" }
+pytest-cov = "^4.0.0"
+reuse = "^1.1.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `schemamodels-0.6.1/setup.py` & `schemamodels-0.7.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,112 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: schemamodels
+Version: 0.7.0
+Summary: Dynamically create useful data classes from JSON schemas
+License: GPL-3.0-or-later
+Author: 'Jurnell Cockhren'
+Author-email: jurnell@civichacker.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
 
-packages = \
-['schemamodels']
+<!--
+SPDX-FileCopyrightText: 2023 Civic Hacker, LLC
 
-package_data = \
-{'': ['*']}
+SPDX-License-Identifier: GPL-3.0-or-later
+-->
 
-setup_kwargs = {
-    'name': 'schemamodels',
-    'version': '0.6.1',
-    'description': 'Dynamically create useful data classes from JSON schemas',
-    'long_description': '# Schema Models\n\n![PyPI](https://img.shields.io/pypi/v/schemamodels?style=for-the-badge) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/schemamodels?style=for-the-badge)\n\nDynamically created data classes from JSON schemas\n\n\nUse this library to quickly turn a JSON Schema into a Python dataclass that you can immediately consume.\n\n\n## Installation\n\nInstall this package using the usual suspects.\n\n```\npip install schemamodels\n```\n\n## Usage\n\nAssuming you have a JSON schema like:\n\n```json\n    {\n        "$id": "https://schema.dev/fake-schema.schema.json",\n        "$schema": "http://json-schema.org/draft-07/schema#",\n        "title": "fake-schema",\n        "description": "Blue Blah",\n        "type": "object",\n        "properties": {\n            "property_a": {\n              "default": 5,\n              "type": "integer"\n            },\n            "property_b": {\n              "type": "string"\n            }\n        }\n    }\n```\n\n```python\nfrom schemamodels import SchemaModelFactory\n\nschema_string = \'..\'\nmy_json_schema = json.loads(schema_string)\n\nfactory = SchemaModelFactory()\nfactory.register(my_json_schema)\n```\n\n\nUse your new dataclass\n\n```python\nfrom schemamodels import exceptions\nfrom schemamodels.dynamic import FakeSchema\n\nyour_data_instance = FakeSchema(property_a=2334)  # OK\n\nwith pytest.raises(exceptions.ValueTypeViolation):\n  your_data_instance = FakeSchema(property_a="hello")\n\n```\n\n## Rationale\n\n### The JSON Schema can come from anywhere\n\nRegardless of where the JSON schema originated, it only needs to be valid for the Draft version you care about. There are a number of libraries better suited validating a JSON Schema document. A user of this library would obtain a JSON Schema document using their prefered method (filesystem, remote), then pass it to this library.\n\n\n### Just-enough validation\n\nAt this time, I\'m not interested in validating a JSON Schema. However, there are some basic checks I\'d like to have performed _every time_ create a new instance of a object that\'s designed to _hold_ my data. Also, questions about the quality of the data is out of scope.\n\nI want to have the confidence that the data has a structure the adhears to the rules provided by a JSON Schema.\n\nI want to be sure that the dictionary exported by these data classes would pass validation checks. The specific tool used to validate an instance of data against the original JSON Schema shouldn\'t matter.\n\n### I\'m tired of writing Python classes by hand\n\nWhile I like using Python-classes to write Python declaratively, I think letting JSON Schema drive the data models creates an opportunity to automate.\n\nWhen I have a valid JSON Schema, I can create a new Python dataclass with one line of code.\n',
-    'author': "'Jurnell Cockhren'",
-    'author_email': 'jurnell@civichacker.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.8,<4.0',
-}
+# Schema Models
 
+![PyPI](https://img.shields.io/pypi/v/schemamodels?style=for-the-badge) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/schemamodels?style=for-the-badge)
+[![REUSE status](https://api.reuse.software/badge/git.fsfe.org/reuse/api)](https://api.reuse.software/info/git.fsfe.org/reuse/api)
+
+Use this library to turn a JSON Schema into a plain 'ol Python dataclass.
+
+## Installation
+
+Install this package using the usual suspects.
+
+```
+pip install schemamodels
+```
+
+## Usage
+
+This library **only** supports JSON schemas of `type: object`:
+
+```json
+    {
+        "$id": "https://schema.dev/fake-schema.schema.json",
+        "$schema": "http://json-schema.org/draft-07/schema#",
+        "title": "fake-schema",
+        "description": "Blue Blah",
+        "type": "object",
+        "properties": {
+            "property_a": {
+              "default": 5,
+              "type": "integer"
+            },
+            "property_b": {
+              "type": "string"
+            }
+        }
+    }
+```
+
+```python
+from schemamodels import SchemaModelFactory
+
+schema_string = '..'
+my_json_schema = json.loads(schema_string)
+
+factory = SchemaModelFactory()
+factory.register(my_json_schema)
+```
+
+
+Use your new dataclass
+
+```python
+from schemamodels import exceptions
+from schemamodels.dynamic import FakeSchema
+
+your_data_instance = FakeSchema(property_a=2334)  # OK
+
+with pytest.raises(exceptions.ValueTypeViolation):
+  your_data_instance = FakeSchema(property_a="hello")
+
+```
+
+## Why this library exists
+
+### The JSON Schema can come from anywhere
+
+Regardless of where your JSON schema originated, it only needs to be valid for the Draft version you care about. There are a number of libraries better suited validating a JSON Schema document. A user of this library would obtain a JSON Schema document using their prefered method (filesystem, remote), then pass it to this library.
+
+
+### Just-enough validation
+
+Use this library, if there are some basic checks you'd like performed _every time_ create a new instance data class. Also, questions about the quality of the data is out of scope.
+
+I want to have the confidence that the data has a structure the adhears to the rules provided by a JSON Schema.
+
+I want to be sure that the dictionary exported by these data classes would pass validation checks. The specific tool used to validate an instance of data against the original JSON Schema shouldn't matter.
+
+### I'm tired of writing Python classes by hand
+
+While I like using classes to write Python declaratively, I think letting JSON Schema drive the data models creates an opportunity to automate.
+
+When I have a valid JSON Schema, I can create a new Python dataclass with one line of code.
+
+
+## License
+
+This codebase is licensed under the GPLv3+ and therefore the use, inclusion, modification, and distribution of this software is governed by the GPL.
+
+If you are planning to use schemamodels in a commercial product or wish to opt-out of the obligations of the GPL, please reach out to license@civichacker.com.
 
-setup(**setup_kwargs)
```

