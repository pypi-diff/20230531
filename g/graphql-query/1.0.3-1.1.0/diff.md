# Comparing `tmp/graphql_query-1.0.3.tar.gz` & `tmp/graphql_query-1.1.0.tar.gz`

## Comparing `graphql_query-1.0.3.tar` & `graphql_query-1.1.0.tar`

### file list

```diff
@@ -1,62 +1,64 @@
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 graphql_query-1.0.3/.editorconfig
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 graphql_query-1.0.3/CONTRIBUTING.md
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 graphql_query-1.0.3/Makefile
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 graphql_query-1.0.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 graphql_query-1.0.3/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 graphql_query-1.0.3/.github/workflows/check.yaml
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 graphql_query-1.0.3/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 graphql_query-1.0.3/.github/workflows/static.yaml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 graphql_query-1.0.3/docs/Makefile
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 graphql_query-1.0.3/docs/make.bat
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 graphql_query-1.0.3/docs/source/api.rst
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 graphql_query-1.0.3/docs/source/conf.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 graphql_query-1.0.3/docs/source/examples.rst
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 graphql_query-1.0.3/docs/source/index.rst
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 graphql_query-1.0.3/docs/source/intro.rst
--rw-r--r--   0        0        0    12568 2020-02-02 00:00:00.000000 graphql_query-1.0.3/docs/source/usage.rst
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 graphql_query-1.0.3/docs/source/examples/list_of_objects.rst
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 graphql_query-1.0.3/docs/source/examples/with_gql.rst
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 graphql_query-1.0.3/graphql_query/__info__.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 graphql_query-1.0.3/graphql_query/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 graphql_query-1.0.3/graphql_query/__version__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 graphql_query-1.0.3/graphql_query/py.typed
--rw-r--r--   0        0        0    20405 2020-02-02 00:00:00.000000 graphql_query-1.0.3/graphql_query/types.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 graphql_query-1.0.3/graphql_query/templates/argument_key_argument.jinja2
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 graphql_query-1.0.3/graphql_query/templates/argument_key_arguments.jinja2
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 graphql_query-1.0.3/graphql_query/templates/argument_key_objects.jinja2
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 graphql_query-1.0.3/graphql_query/templates/argument_key_value.jinja2
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 graphql_query-1.0.3/graphql_query/templates/argument_key_values.jinja2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 graphql_query-1.0.3/graphql_query/templates/argument_key_variable.jinja2
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 graphql_query-1.0.3/graphql_query/templates/directive.jinja2
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 graphql_query-1.0.3/graphql_query/templates/field.jinja2
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 graphql_query-1.0.3/graphql_query/templates/fragment.jinja2
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 graphql_query-1.0.3/graphql_query/templates/inline_fragment.jinja2
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 graphql_query-1.0.3/graphql_query/templates/operation.jinja2
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 graphql_query-1.0.3/graphql_query/templates/query.jinja2
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 graphql_query-1.0.3/graphql_query/templates/variable.jinja2
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 graphql_query-1.0.3/requirements/requirements-dev.txt
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 graphql_query-1.0.3/requirements/requirements-docs.txt
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 graphql_query-1.0.3/requirements/requirements-test.txt
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 graphql_query-1.0.3/requirements/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.0.3/tests/__init__.py
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 graphql_query-1.0.3/tests/data.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 graphql_query-1.0.3/tests/test_directive.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 graphql_query-1.0.3/tests/test_exist_templates.py
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 graphql_query-1.0.3/tests/test_field.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 graphql_query-1.0.3/tests/test_fragment.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 graphql_query-1.0.3/tests/test_graphql2python_query.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 graphql_query-1.0.3/tests/test_inline_fragment.py
--rw-r--r--   0        0        0    14373 2020-02-02 00:00:00.000000 graphql_query-1.0.3/tests/test_operation.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 graphql_query-1.0.3/tests/test_query.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.0.3/tests/arguments/__init__.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 graphql_query-1.0.3/tests/arguments/data_arguments.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 graphql_query-1.0.3/tests/arguments/test_arguments.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.0.3/tests/test_argument/__init__.py
--rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 graphql_query-1.0.3/tests/test_argument/test_argument.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.0.3/tests/test_variable/__init__.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 graphql_query-1.0.3/tests/test_variable/test_variable.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 graphql_query-1.0.3/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 graphql_query-1.0.3/LICENSE
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 graphql_query-1.0.3/README.md
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 graphql_query-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 graphql_query-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 graphql_query-1.1.0/.editorconfig
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 graphql_query-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 graphql_query-1.1.0/Makefile
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 graphql_query-1.1.0/SECURITY.md
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 graphql_query-1.1.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 graphql_query-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 graphql_query-1.1.0/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 graphql_query-1.1.0/.github/workflows/check.yaml
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 graphql_query-1.1.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 graphql_query-1.1.0/.github/workflows/static.yaml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 graphql_query-1.1.0/docs/Makefile
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 graphql_query-1.1.0/docs/make.bat
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 graphql_query-1.1.0/docs/source/api.rst
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 graphql_query-1.1.0/docs/source/conf.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 graphql_query-1.1.0/docs/source/examples.rst
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 graphql_query-1.1.0/docs/source/index.rst
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 graphql_query-1.1.0/docs/source/intro.rst
+-rw-r--r--   0        0        0    12568 2020-02-02 00:00:00.000000 graphql_query-1.1.0/docs/source/usage.rst
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 graphql_query-1.1.0/docs/source/examples/list_of_objects.rst
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 graphql_query-1.1.0/docs/source/examples/with_gql.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/__info__.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/__version__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/py.typed
+-rw-r--r--   0        0        0    18575 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/types.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/argument_key_argument.jinja2
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/argument_key_arguments.jinja2
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/argument_key_objects.jinja2
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/argument_key_value.jinja2
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/argument_key_values.jinja2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/argument_key_variable.jinja2
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/directive.jinja2
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/field.jinja2
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/fragment.jinja2
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/inline_fragment.jinja2
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/operation.jinja2
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/query.jinja2
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/variable.jinja2
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 graphql_query-1.1.0/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 graphql_query-1.1.0/requirements/requirements-docs.txt
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 graphql_query-1.1.0/requirements/requirements-test.txt
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 graphql_query-1.1.0/requirements/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/data.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_directive.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_exist_templates.py
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_field.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_fragment.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_graphql2python_query.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_inline_fragment.py
+-rw-r--r--   0        0        0    14256 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_operation.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_query.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/arguments/__init__.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/arguments/data_arguments.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/arguments/test_arguments.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_argument/__init__.py
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_argument/test_argument.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_variable/__init__.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_variable/test_variable.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 graphql_query-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 graphql_query-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 graphql_query-1.1.0/README.md
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 graphql_query-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 graphql_query-1.1.0/PKG-INFO
```

### Comparing `graphql_query-1.0.3/CONTRIBUTING.md` & `graphql_query-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/Makefile` & `graphql_query-1.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/.github/ISSUE_TEMPLATE/bug_report.md` & `graphql_query-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/.github/workflows/check.yaml` & `graphql_query-1.1.0/.github/workflows/check.yaml`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/.github/workflows/static.yaml` & `graphql_query-1.1.0/.github/workflows/static.yaml`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/docs/Makefile` & `graphql_query-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/docs/make.bat` & `graphql_query-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/docs/source/conf.py` & `graphql_query-1.1.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'graphql_query'
 copyright = '2022-2023, Denis A. Artyushin'
 author = 'Denis A. Artyushin'
-version = '1.0.3'
+version = '1.1.0'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinxarg.ext',
     'sphinx.ext.autodoc',
```

### Comparing `graphql_query-1.0.3/docs/source/index.rst` & `graphql_query-1.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/docs/source/usage.rst` & `graphql_query-1.1.0/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/docs/source/examples/list_of_objects.rst` & `graphql_query-1.1.0/docs/source/examples/list_of_objects.rst`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/docs/source/examples/with_gql.rst` & `graphql_query-1.1.0/docs/source/examples/with_gql.rst`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/graphql_query/__init__.py` & `graphql_query-1.1.0/graphql_query/__init__.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/graphql_query/types.py` & `graphql_query-1.1.0/graphql_query/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import os
 import sys
 from pathlib import Path
 from typing import Any, List, Optional, Union
 
-from graphql import assert_name
 from jinja2 import Environment, FileSystemLoader, Template
 from pydantic import BaseModel
 from pydantic import Field as PydanticField
-from pydantic import validator
 
 if sys.version_info >= (3, 10):
     from typing import TypeGuard
 else:
     # Use TypeGuard from typing_extensions for python <= 3.9
     from typing_extensions import TypeGuard
 
@@ -93,18 +91,14 @@
 
     name: str
     type: str
     default: Optional[str] = PydanticField(default=None)
 
     _template: Template = template_env.get_template("variable.jinja2")
 
-    @validator("name")
-    def graphql_variable_name(cls, name: str) -> str:
-        return assert_name(name)
-
     def render(self) -> str:
         return self._template.render(name=self.name, type=self.type, default=self.default)
 
 
 class Argument(_GraphQL2PythonQuery):
     """GraphQL argument type.
 
@@ -181,18 +175,14 @@
     _template_key_value: Template = template_env.get_template("argument_key_value.jinja2")
     _template_key_values: Template = template_env.get_template("argument_key_values.jinja2")
     _template_key_argument: Template = template_env.get_template("argument_key_argument.jinja2")
     _template_key_variable: Template = template_env.get_template("argument_key_variable.jinja2")
     _template_key_arguments: Template = template_env.get_template("argument_key_arguments.jinja2")
     _template_key_objects: Template = template_env.get_template("argument_key_objects.jinja2")
 
-    @validator("name")
-    def graphql_argument_name(cls, name: str) -> str:
-        return assert_name(name)
-
     @staticmethod
     def _check_is_list_of_str(values: List[Any]) -> TypeGuard[List[str]]:
         return all(isinstance(value, str) for value in values)
 
     @staticmethod
     def _check_is_list_of_arguments(values: List[Any]) -> TypeGuard[List['Argument']]:
         return all(isinstance(value, Argument) for value in values)
@@ -293,18 +283,14 @@
     """
 
     name: str
     arguments: List[Argument] = PydanticField(default_factory=list)
 
     _template_directive: Template = template_env.get_template("directive.jinja2")
 
-    @validator("name")
-    def graphql_directive_name(cls, name: str) -> str:
-        return assert_name(name)
-
     def render(self) -> str:
         return self._template_directive.render(
             name=self.name, arguments=[self._line_shift(argument.render()) for argument in self.arguments]
         )
 
 
 class Field(_GraphQL2PythonQuery):
@@ -363,24 +349,14 @@
     arguments: List[Argument] = PydanticField(default_factory=list)
     fields: List[Union[str, 'Field', 'InlineFragment', 'Fragment']] = PydanticField(default_factory=list)
     directives: List[Directive] = PydanticField(default_factory=list)
     typename: bool = PydanticField(default=False, description="Add meta field `__typename` to sub-fields.")
 
     _template: Template = template_env.get_template("field.jinja2")
 
-    @validator("name")
-    def graphql_field_name(cls, name: str) -> str:
-        return assert_name(name)
-
-    @validator("alias")
-    def graphql_field_alias(cls, alias: Optional[str]) -> Optional[str]:
-        if alias is not None:
-            return assert_name(alias)
-        return alias
-
     def render(self) -> str:
         return self._template.render(
             name=self.name,
             alias=self.alias,
             arguments=[self._line_shift(argument.render()) for argument in self.arguments],
             fields=[self._render_field(field) for field in self.fields],
             directives=[directive.render() for directive in self.directives],
@@ -427,22 +403,14 @@
     type: str
     arguments: List[Argument] = PydanticField(default_factory=list)
     fields: List[Union[str, 'Field', 'InlineFragment', 'Fragment']] = PydanticField(default_factory=list)
     typename: bool = PydanticField(default=False, description="Add meta field `__typename` to sub-fields.")
 
     _template: Template = template_env.get_template("inline_fragment.jinja2")
 
-    @validator("fields")
-    def graphql_inline_fragment_fields(
-        cls, fields: List[Union[str, 'Field', 'InlineFragment', 'Fragment']]
-    ) -> List[Union[str, 'Field', 'InlineFragment', 'Fragment']]:
-        if len(fields) == 0:
-            raise ValueError("empty fields for this inline fragment")
-        return fields
-
     def render(self) -> str:
         return self._template.render(
             type=self.type,
             arguments=[self._line_shift(argument.render()) for argument in self.arguments],
             fields=[self._render_field(field) for field in self.fields],
             typename=self.typename,
         )
@@ -495,18 +463,14 @@
     name: str
     type: str
     fields: List[Union[str, 'Field', 'InlineFragment', 'Fragment']] = PydanticField(default_factory=list)
     typename: bool = PydanticField(default=False, description="Add meta field `__typename` to sub-fields")
 
     _template: Template = template_env.get_template("fragment.jinja2")
 
-    @validator("name")
-    def graphql_fragment_name(cls, name: str) -> str:
-        return assert_name(name)
-
     def render(self) -> str:
         return self._template.render(
             name=self.name,
             type=self.type,
             fields=[self._render_field(field) for field in self.fields],
             typename=self.typename,
         )
@@ -554,24 +518,14 @@
     alias: Optional[str] = PydanticField(default=None)
     arguments: List[Argument] = PydanticField(default_factory=list)
     typename: bool = PydanticField(default=False, description="Add meta field `__typename` to the query.")
     fields: List[Union[str, 'Field', 'InlineFragment', 'Fragment']] = PydanticField(default_factory=list)
 
     _template: Template = template_env.get_template("query.jinja2")
 
-    @validator("name")
-    def graphql_query_name(cls, name: str) -> str:
-        return assert_name(name)
-
-    @validator("alias")
-    def graphql_alias_alias(cls, alias: Optional[str]) -> Optional[str]:
-        if alias is not None:
-            return assert_name(alias)
-        return alias
-
     def render(self) -> str:
         return self._template.render(
             name=self.name,
             alias=self.alias,
             arguments=[self._line_shift(argument.render()) for argument in self.arguments],
             typename=self.typename,
             fields=[self._render_field(field) for field in self.fields],
@@ -635,26 +589,14 @@
     fragments: List[Fragment] = PydanticField(
         default_factory=list, description="https://graphql.org/learn/queries/#fragments"
     )
 
     _template: Template = template_env.get_template("operation.jinja2")
     _supported_types = ["query", "mutation", "subscription"]
 
-    @validator("name")
-    def graphql_operation_name(cls, name: Optional[str]) -> Optional[str]:
-        if name is not None:
-            return assert_name(name)
-        return name
-
-    @validator("queries")
-    def graphql_queries(cls, queries: List[Query]) -> List[Query]:
-        if len(queries) == 0:
-            raise ValueError("empty queries list for this operation")
-        return queries
-
     def render(self) -> str:
         return self._template.render(
             type=self.type,
             name=self.name,
             variables=[self._line_shift(variable.render()) for variable in self.variables],
             queries=[self._line_shift(query.render()) for query in self.queries],
             fragments=[fragment.render() for fragment in self.fragments],
```

### Comparing `graphql_query-1.0.3/requirements/requirements-dev.txt` & `graphql_query-1.1.0/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/requirements/requirements-docs.txt` & `graphql_query-1.1.0/requirements/requirements-docs.txt`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/requirements/requirements-test.txt` & `graphql_query-1.1.0/requirements/requirements-test.txt`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/tests/data.py` & `graphql_query-1.1.0/tests/data.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/tests/test_directive.py` & `graphql_query-1.1.0/tests/test_directive.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/tests/test_exist_templates.py` & `graphql_query-1.1.0/tests/test_exist_templates.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/tests/test_field.py` & `graphql_query-1.1.0/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/tests/test_fragment.py` & `graphql_query-1.1.0/tests/test_fragment.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/tests/test_inline_fragment.py` & `graphql_query-1.1.0/tests/test_inline_fragment.py`

 * *Files 15% similar despite different names*

```diff
@@ -47,12 +47,7 @@
     arguments: List[Argument],
     fields: List[Union[str, Field, InlineFragment, Fragment]],
     typename: bool,
     result: str,
 ):
     fragment = InlineFragment(type=type, arguments=arguments, fields=fields, typename=typename)
     assert fragment.render() == result
-
-
-def test_empty_fields():
-    with pytest.raises(ValueError):
-        _ = InlineFragment(type="Type", fields=[])
```

### Comparing `graphql_query-1.0.3/tests/test_operation.py` & `graphql_query-1.1.0/tests/test_operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -477,12 +477,7 @@
     queries: List[Query],
     fragments: List[Fragment],
     result: str,
 ):
     operation = Operation(type=type, name=name, variables=variables, queries=queries, fragments=fragments)
 
     assert operation.render() == result
-
-
-def test_empty_queries_list():
-    with pytest.raises(ValueError):
-        _ = Operation(type="query", queries=[])
```

### Comparing `graphql_query-1.0.3/tests/test_query.py` & `graphql_query-1.1.0/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/tests/arguments/data_arguments.py` & `graphql_query-1.1.0/tests/arguments/data_arguments.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/tests/test_argument/test_argument.py` & `graphql_query-1.1.0/tests/test_argument/test_argument.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/tests/test_variable/test_variable.py` & `graphql_query-1.1.0/tests/test_variable/test_variable.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/.gitignore` & `graphql_query-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/LICENSE` & `graphql_query-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/README.md` & `graphql_query-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `graphql_query-1.0.3/pyproject.toml` & `graphql_query-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     "Framework :: Pydantic",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 requires-python = ">=3.7"
 dependencies = [
     "pydantic>=1.10, <1.11",
     "jinja2>=3.1, <3.2",
-    "graphql-core>=3.2, <3.3",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/denisart/graphql-query"
 Documentation = "https://denisart.github.io/graphql-query/"
 Source = "https://github.com/denisart/graphql-query"
```

### Comparing `graphql_query-1.0.3/PKG-INFO` & `graphql_query-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphql_query
-Version: 1.0.3
+Version: 1.1.0
 Summary: Complete GraphQL query string generation for python.
 Project-URL: Homepage, https://github.com/denisart/graphql-query
 Project-URL: Documentation, https://denisart.github.io/graphql-query/
 Project-URL: Source, https://github.com/denisart/graphql-query
 Author-email: "Denis A. Artyushin" <artyushinden@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -22,15 +22,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
-Requires-Dist: graphql-core<3.3,>=3.2
 Requires-Dist: jinja2<3.2,>=3.1
 Requires-Dist: pydantic<1.11,>=1.10
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pylint-pydantic; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
```

