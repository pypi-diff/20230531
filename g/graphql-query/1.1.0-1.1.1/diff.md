# Comparing `tmp/graphql_query-1.1.0.tar.gz` & `tmp/graphql_query-1.1.1.tar.gz`

## Comparing `graphql_query-1.1.0.tar` & `graphql_query-1.1.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 graphql_query-1.1.0/.editorconfig
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 graphql_query-1.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 graphql_query-1.1.0/Makefile
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 graphql_query-1.1.0/SECURITY.md
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 graphql_query-1.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 graphql_query-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 graphql_query-1.1.0/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 graphql_query-1.1.0/.github/workflows/check.yaml
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 graphql_query-1.1.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 graphql_query-1.1.0/.github/workflows/static.yaml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 graphql_query-1.1.0/docs/Makefile
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 graphql_query-1.1.0/docs/make.bat
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 graphql_query-1.1.0/docs/source/api.rst
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 graphql_query-1.1.0/docs/source/conf.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 graphql_query-1.1.0/docs/source/examples.rst
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 graphql_query-1.1.0/docs/source/index.rst
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 graphql_query-1.1.0/docs/source/intro.rst
--rw-r--r--   0        0        0    12568 2020-02-02 00:00:00.000000 graphql_query-1.1.0/docs/source/usage.rst
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 graphql_query-1.1.0/docs/source/examples/list_of_objects.rst
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 graphql_query-1.1.0/docs/source/examples/with_gql.rst
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/__info__.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/__version__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/py.typed
--rw-r--r--   0        0        0    18575 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/types.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/argument_key_argument.jinja2
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/argument_key_arguments.jinja2
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/argument_key_objects.jinja2
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/argument_key_value.jinja2
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/argument_key_values.jinja2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/argument_key_variable.jinja2
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/directive.jinja2
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/field.jinja2
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/fragment.jinja2
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/inline_fragment.jinja2
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/operation.jinja2
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/query.jinja2
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 graphql_query-1.1.0/graphql_query/templates/variable.jinja2
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 graphql_query-1.1.0/requirements/requirements-dev.txt
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 graphql_query-1.1.0/requirements/requirements-docs.txt
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 graphql_query-1.1.0/requirements/requirements-test.txt
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 graphql_query-1.1.0/requirements/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/data.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_directive.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_exist_templates.py
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_field.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_fragment.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_graphql2python_query.py
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_inline_fragment.py
--rw-r--r--   0        0        0    14256 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_operation.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_query.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/arguments/__init__.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/arguments/data_arguments.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/arguments/test_arguments.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_argument/__init__.py
--rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_argument/test_argument.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_variable/__init__.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 graphql_query-1.1.0/tests/test_variable/test_variable.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 graphql_query-1.1.0/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 graphql_query-1.1.0/LICENSE
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 graphql_query-1.1.0/README.md
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 graphql_query-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 graphql_query-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 graphql_query-1.1.1/.editorconfig
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 graphql_query-1.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 graphql_query-1.1.1/Makefile
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 graphql_query-1.1.1/SECURITY.md
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 graphql_query-1.1.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 graphql_query-1.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 graphql_query-1.1.1/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 graphql_query-1.1.1/.github/workflows/check.yaml
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 graphql_query-1.1.1/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 graphql_query-1.1.1/.github/workflows/static.yaml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 graphql_query-1.1.1/docs/Makefile
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 graphql_query-1.1.1/docs/make.bat
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 graphql_query-1.1.1/docs/source/api.rst
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 graphql_query-1.1.1/docs/source/conf.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 graphql_query-1.1.1/docs/source/examples.rst
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 graphql_query-1.1.1/docs/source/index.rst
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 graphql_query-1.1.1/docs/source/intro.rst
+-rw-r--r--   0        0        0    12568 2020-02-02 00:00:00.000000 graphql_query-1.1.1/docs/source/usage.rst
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 graphql_query-1.1.1/docs/source/examples/list_of_objects.rst
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 graphql_query-1.1.1/docs/source/examples/with_gql.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/__info__.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/__version__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/py.typed
+-rw-r--r--   0        0        0    18575 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/types.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/argument_key_argument.jinja2
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/argument_key_arguments.jinja2
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/argument_key_objects.jinja2
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/argument_key_value.jinja2
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/argument_key_values.jinja2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/argument_key_variable.jinja2
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/directive.jinja2
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/field.jinja2
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/fragment.jinja2
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/inline_fragment.jinja2
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/operation.jinja2
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/query.jinja2
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 graphql_query-1.1.1/graphql_query/templates/variable.jinja2
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 graphql_query-1.1.1/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 graphql_query-1.1.1/requirements/requirements-docs.txt
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 graphql_query-1.1.1/requirements/requirements-test.txt
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 graphql_query-1.1.1/requirements/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/data.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_directive.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_exist_templates.py
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_field.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_fragment.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_graphql2python_query.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_inline_fragment.py
+-rw-r--r--   0        0        0    14256 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_operation.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_query.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/arguments/__init__.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/arguments/data_arguments.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/arguments/test_arguments.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_argument/__init__.py
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_argument/test_argument.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_variable/__init__.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 graphql_query-1.1.1/tests/test_variable/test_variable.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 graphql_query-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 graphql_query-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 graphql_query-1.1.1/README.md
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 graphql_query-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 graphql_query-1.1.1/PKG-INFO
```

### Comparing `graphql_query-1.1.0/CONTRIBUTING.md` & `graphql_query-1.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/Makefile` & `graphql_query-1.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `graphql_query-1.1.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/.github/workflows/check.yaml` & `graphql_query-1.1.1/.github/workflows/check.yaml`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/.github/workflows/static.yaml` & `graphql_query-1.1.1/.github/workflows/static.yaml`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/docs/Makefile` & `graphql_query-1.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/docs/make.bat` & `graphql_query-1.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/docs/source/conf.py` & `graphql_query-1.1.1/docs/source/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'graphql_query'
 copyright = '2022-2023, Denis A. Artyushin'
 author = 'Denis A. Artyushin'
-version = '1.1.0'
+version = '1.1.1'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinxarg.ext',
     'sphinx.ext.autodoc',
```

### Comparing `graphql_query-1.1.0/docs/source/index.rst` & `graphql_query-1.1.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/docs/source/usage.rst` & `graphql_query-1.1.1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/docs/source/examples/list_of_objects.rst` & `graphql_query-1.1.1/docs/source/examples/list_of_objects.rst`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/docs/source/examples/with_gql.rst` & `graphql_query-1.1.1/docs/source/examples/with_gql.rst`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/graphql_query/__init__.py` & `graphql_query-1.1.1/graphql_query/__init__.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/graphql_query/types.py` & `graphql_query-1.1.1/graphql_query/types.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/requirements/requirements-dev.txt` & `graphql_query-1.1.1/requirements/requirements-dev.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,67 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --extra=dev --output-file=requirements/requirements-dev.txt --resolver=backtracking pyproject.toml
 #
-astroid==2.15.0
+astroid==2.15.5
     # via pylint
-black==23.1.0
+black==23.3.0
     # via graphql_query (pyproject.toml)
 click==8.1.3
     # via black
 dill==0.3.6
     # via pylint
-graphql-core==3.2.3
-    # via graphql_query (pyproject.toml)
 isort==5.12.0
     # via pylint
 jinja2==3.1.2
     # via graphql_query (pyproject.toml)
 lazy-object-proxy==1.9.0
     # via astroid
 markupsafe==2.1.2
     # via jinja2
 mccabe==0.7.0
     # via pylint
-mypy==1.1.1
+mypy==1.3.0
     # via graphql_query (pyproject.toml)
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-packaging==23.0
+packaging==23.1
     # via black
 pathspec==0.11.1
     # via black
-platformdirs==3.1.1
+platformdirs==3.5.1
     # via
     #   black
     #   pylint
-pydantic==1.10.6
+pydantic==1.10.8
     # via
     #   graphql_query (pyproject.toml)
     #   pylint-pydantic
-pylint==2.17.0
+pylint==2.17.4
     # via
     #   pylint-plugin-utils
     #   pylint-pydantic
-pylint-plugin-utils==0.7
+pylint-plugin-utils==0.8.2
     # via pylint-pydantic
 pylint-pydantic==0.1.8
     # via graphql_query (pyproject.toml)
-ruff==0.0.257
+ruff==0.0.270
     # via graphql_query (pyproject.toml)
 tomli==2.0.1
     # via
     #   black
     #   mypy
     #   pylint
-tomlkit==0.11.6
+tomlkit==0.11.8
     # via pylint
-typing-extensions==4.5.0
+typing-extensions==4.6.2
     # via
     #   astroid
     #   mypy
     #   pydantic
 wheel==0.40.0
     # via graphql_query (pyproject.toml)
 wrapt==1.15.0
```

### Comparing `graphql_query-1.1.0/requirements/requirements-docs.txt` & `graphql_query-1.1.1/requirements/requirements-docs.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,70 +4,68 @@
 #
 #    pip-compile --extra=docs --output-file=requirements/requirements-docs.txt --resolver=backtracking pyproject.toml
 #
 alabaster==0.7.13
     # via sphinx
 babel==2.12.1
     # via sphinx
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via cryptography
 charset-normalizer==3.1.0
     # via requests
-cryptography==39.0.2
+cryptography==41.0.0
     # via pyjwt
 docutils==0.18.1
     # via
     #   sphinx
     #   sphinx-rtd-theme
-github3-py==3.2.0
+github3-py==4.0.1
     # via sphinxcontrib-github
-graphql-core==3.2.3
-    # via graphql_query (pyproject.toml)
 idna==3.4
     # via requests
 imagesize==1.4.1
     # via sphinx
 jinja2==3.1.2
     # via
     #   graphql_query (pyproject.toml)
     #   sphinx
 markupsafe==2.1.2
     # via jinja2
-packaging==23.0
+packaging==23.1
     # via sphinx
 pycparser==2.21
     # via cffi
-pydantic==1.10.6
+pydantic==1.10.8
     # via graphql_query (pyproject.toml)
-pygments==2.14.0
+pygments==2.15.1
     # via sphinx
-pyjwt[crypto]==2.6.0
+pyjwt[crypto]==2.7.0
     # via github3-py
 python-dateutil==2.8.2
     # via github3-py
-requests==2.28.2
+requests==2.31.0
     # via
     #   github3-py
     #   sphinx
 six==1.16.0
     # via python-dateutil
 snowballstemmer==2.2.0
     # via sphinx
-sphinx==6.1.3
+sphinx==6.2.1
     # via
     #   graphql_query (pyproject.toml)
     #   sphinx-argparse
     #   sphinx-rtd-theme
     #   sphinxcontrib-github
     #   sphinxcontrib-jquery
 sphinx-argparse==0.4.0
     # via graphql_query (pyproject.toml)
-sphinx-rtd-theme==1.2.0
+sphinx-rtd-theme==1.2.1
     # via graphql_query (pyproject.toml)
 sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
 sphinxcontrib-github==0.1.3
     # via graphql_query (pyproject.toml)
@@ -77,13 +75,13 @@
     # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
-typing-extensions==4.5.0
+typing-extensions==4.6.2
     # via pydantic
 uritemplate==4.1.1
     # via github3-py
-urllib3==1.26.15
+urllib3==2.0.2
     # via requests
```

### Comparing `graphql_query-1.1.0/requirements/requirements-test.txt` & `graphql_query-1.1.1/requirements/requirements-test.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --extra=test --output-file=requirements/requirements-test.txt --resolver=backtracking pyproject.toml
 #
-attrs==22.2.0
-    # via pytest
-coverage[toml]==7.2.2
+coverage[toml]==7.2.7
     # via pytest-cov
 exceptiongroup==1.1.1
     # via pytest
-graphql-core==3.2.3
-    # via graphql_query (pyproject.toml)
 iniconfig==2.0.0
     # via pytest
 jinja2==3.1.2
     # via graphql_query (pyproject.toml)
 markupsafe==2.1.2
     # via jinja2
-packaging==23.0
+packaging==23.1
     # via pytest
 pluggy==1.0.0
     # via pytest
-pydantic==1.10.6
+pydantic==1.10.8
     # via graphql_query (pyproject.toml)
-pytest==7.2.2
+pytest==7.3.1
     # via
     #   graphql_query (pyproject.toml)
     #   pytest-cov
     #   pytest-mock
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via graphql_query (pyproject.toml)
 pytest-mock==3.10.0
     # via graphql_query (pyproject.toml)
 tomli==2.0.1
     # via
     #   coverage
     #   pytest
-typing-extensions==4.5.0
+typing-extensions==4.6.2
     # via pydantic
```

### Comparing `graphql_query-1.1.0/tests/data.py` & `graphql_query-1.1.1/tests/data.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/tests/test_directive.py` & `graphql_query-1.1.1/tests/test_directive.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/tests/test_exist_templates.py` & `graphql_query-1.1.1/tests/test_exist_templates.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/tests/test_field.py` & `graphql_query-1.1.1/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/tests/test_fragment.py` & `graphql_query-1.1.1/tests/test_fragment.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/tests/test_inline_fragment.py` & `graphql_query-1.1.1/tests/test_inline_fragment.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/tests/test_operation.py` & `graphql_query-1.1.1/tests/test_operation.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/tests/test_query.py` & `graphql_query-1.1.1/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/tests/arguments/data_arguments.py` & `graphql_query-1.1.1/tests/arguments/data_arguments.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/tests/test_argument/test_argument.py` & `graphql_query-1.1.1/tests/test_argument/test_argument.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/tests/test_variable/test_variable.py` & `graphql_query-1.1.1/tests/test_variable/test_variable.py`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/.gitignore` & `graphql_query-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/LICENSE` & `graphql_query-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/README.md` & `graphql_query-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/pyproject.toml` & `graphql_query-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `graphql_query-1.1.0/PKG-INFO` & `graphql_query-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphql_query
-Version: 1.1.0
+Version: 1.1.1
 Summary: Complete GraphQL query string generation for python.
 Project-URL: Homepage, https://github.com/denisart/graphql-query
 Project-URL: Documentation, https://denisart.github.io/graphql-query/
 Project-URL: Source, https://github.com/denisart/graphql-query
 Author-email: "Denis A. Artyushin" <artyushinden@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

