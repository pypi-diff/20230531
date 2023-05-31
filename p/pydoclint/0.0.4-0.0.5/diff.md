# Comparing `tmp/pydoclint-0.0.4.tar.gz` & `tmp/pydoclint-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydoclint-0.0.4.tar", last modified: Sat May 27 10:28:49 2023, max compression
+gzip compressed data, was "pydoclint-0.0.5.tar", last modified: Wed May 31 10:43:11 2023, max compression
```

## Comparing `pydoclint-0.0.4.tar` & `pydoclint-0.0.5.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:28:49.309871 pydoclint-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-27 10:28:34.000000 pydoclint-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-05-27 10:28:49.309871 pydoclint-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-05-27 10:28:34.000000 pydoclint-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:28:49.301870 pydoclint-0.0.4/pydoclint/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/flake8_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:28:49.305871 pydoclint-0.0.4/pydoclint/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/astTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/internal_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/method_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/return_yield_raise.py
--rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/unparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/violation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/utils/walk.py
--rw-r--r--   0 runner    (1001) docker     (123)    16937 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pydoclint/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:28:49.305871 pydoclint-0.0.4/pydoclint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-05-27 10:28:49.000000 pydoclint-0.0.4/pydoclint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-27 10:28:49.000000 pydoclint-0.0.4/pydoclint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 10:28:49.000000 pydoclint-0.0.4/pydoclint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-27 10:28:49.000000 pydoclint-0.0.4/pydoclint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-27 10:28:49.000000 pydoclint-0.0.4/pydoclint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 10:28:49.000000 pydoclint-0.0.4/pydoclint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-27 10:28:34.000000 pydoclint-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-27 10:28:49.309871 pydoclint-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-27 10:28:34.000000 pydoclint-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:28:49.309871 pydoclint-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    23976 2023-05-27 10:28:34.000000 pydoclint-0.0.4/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:43:11.884906 pydoclint-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-31 10:42:55.000000 pydoclint-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-05-31 10:43:11.884906 pydoclint-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-05-31 10:42:55.000000 pydoclint-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:43:11.880906 pydoclint-0.0.5/pydoclint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/flake8_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/parse_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:43:11.884906 pydoclint-0.0.5/pydoclint/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/astTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/internal_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/method_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/return_yield_raise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21587 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/unparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/violation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/utils/walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pydoclint/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:43:11.880906 pydoclint-0.0.5/pydoclint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-05-31 10:43:11.000000 pydoclint-0.0.5/pydoclint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-31 10:43:11.000000 pydoclint-0.0.5/pydoclint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 10:43:11.000000 pydoclint-0.0.5/pydoclint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-31 10:43:11.000000 pydoclint-0.0.5/pydoclint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 10:43:11.000000 pydoclint-0.0.5/pydoclint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 10:43:11.000000 pydoclint-0.0.5/pydoclint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-31 10:42:55.000000 pydoclint-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-31 10:43:11.884906 pydoclint-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 10:42:55.000000 pydoclint-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:43:11.884906 pydoclint-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    25662 2023-05-31 10:42:55.000000 pydoclint-0.0.5/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-31 10:42:55.000000 pydoclint-0.0.5/tests/test_parse_config.py
```

### Comparing `pydoclint-0.0.4/LICENSE` & `pydoclint-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.4/PKG-INFO` & `pydoclint-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: pydoclint
-Version: 0.0.4
-Summary: A linter to check arguments in Python docstrings
-Home-page: https://github.com/jsh9/pydoclint
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pydoclint
 
 A Python docstring linter to check whether a docstring's sections (arguments,
 returns, raises, ...) match the function signature or function implementation.
 
 It runs really fast. In fact, it is at least ~1,475 times faster than
 [darglint](https://github.com/terrencepreilly/darglint) (another linter of the
@@ -72,24 +59,74 @@
 other built-in _flake8_ linters on your code.
 
 ### 2.3. Native vs _flake8_
 
 Should I use _pydoclint_ as a native command line tool or a _flake8_ plugin?
 Here's comparison:
 
-|                 | Pros                                       | Cons                                                          |
-| --------------- | ------------------------------------------ | ------------------------------------------------------------- |
-| Native tool     | Slightly faster                            | No per-line or project-wide omission support right now [*]    |
-| _flake8_ plugin | Supports per-line or project-wide omission | Slightly slower because other flake8 plugins are run together |
+|                 | Pros                                     | Cons                                                          |
+| --------------- | ---------------------------------------- | ------------------------------------------------------------- |
+| Native tool     | Slightly faster                          | No inline or project-wide omission support right now [*]      |
+| _flake8_ plugin | Supports inline or project-wide omission | Slightly slower because other flake8 plugins are run together |
 
 \*) This feature may be added in the near future
 
+### 2.4. Configuration
+
+Here is how to configure _pydoclint_. For detailed explanations of all options,
+see [Section 4](#4-configuration-options) below.
+
+#### 2.4.1. Setting options inline
+
+- Native:
+
+  ```bash
+  pydoclint --check-arg-order=False <FILE_OR_FOLDER_PATH>
+  ```
+
+- Flake8:
+
+  ```bash
+  flake8 --check-arg-order=False <FILE_OR_FOLDER_PATH>
+  ```
+
+#### 2.4.2. Setting options in a configuration file
+
+- Native:
+
+  - In a `.toml` file somewhere in your project folder, add a section like this
+    (put in the config that you need):
+
+    ```toml
+    [tool.pydoclint]
+    style = 'google'
+    exclude = '\.git|\.tox|tests/data|some_script\.py'
+    require-return-section-when-returning-none = true
+    ```
+
+  - Then, specify the path of the `.toml` file in your command:
+
+    ```bash
+    pydoclint --config=path/to/my/config.toml <FILE_OR_FOLDER_PATH>
+    ```
+
+- Flake8:
+  - In your flake8 config file (see
+    [flake8's official doc](https://flake8.pycqa.org/en/latest/user/configuration.html#configuration-locations)),
+    add the config you need under the section `[flake8]`
+
 ## 3. Style violation codes
 
-`pydoclint` currently has the following style violation codes:
+_pydoclint_ currently has the following style violation codes:
+
+### 3.0. `DOC0xx`: Docstring parsing issues
+
+| Code     | Explanation                              |
+| -------- | ---------------------------------------- |
+| `DOC001` | Potential formatting errors in docstring |
 
 ### 3.1. `DOC1xx`: Violations about input arguments
 
 | Code     | Explanation                                                                                                                                          |
 | -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `DOC101` | Docstring contains fewer arguments than in function signature                                                                                        |
 | `DOC102` | Docstring contains more arguments than in function signature                                                                                         |
@@ -110,14 +147,17 @@
 ### 3.2. `DOC2xx`: Violations about return argument(s)
 
 | Code     | Explanation                                                                                          |
 | -------- | ---------------------------------------------------------------------------------------------------- |
 | `DOC201` | Function/method does not have a return section in docstring                                          |
 | `DOC202` | Function/method has a return section in docstring, but there are no return statements or annotations |
 
+Note on `DOC201`: Methods with `@property` as its last decorator do not need to
+have a return section.
+
 ### 3.3. `DOC3xx`: Violations about class docstring and class constructor
 
 | Code     | Explanation                                                                                             |
 | -------- | ------------------------------------------------------------------------------------------------------- |
 | `DOC301` | `__init__()` should not have a docstring; please combine it with the docstring of the class             |
 | `DOC302` | The class docstring does not need a "Returns" section, because `__init__()` cannot return anything      |
 | `DOC303` | The `__init__()` docstring does not need a "Returns" section, because it cannot return anything         |
@@ -193,15 +233,15 @@
 ```
 
 ### 4.4. `--check-type-hint` (shortform: `-th`, default: `True`)
 
 If `True`, the type hints in the docstring and in the Python code need to
 exactly match.
 
-To turn this optoin on/off, do this:
+To turn this option on/off, do this:
 
 ```
 pydoclint --check-type-hint=False <FILE_OR_FOLDER>
 ```
 
 or
 
@@ -210,15 +250,15 @@
 ```
 
 ### 4.5. `--check-arg-order` (shortform: `-ao`, default: `True`)
 
 If `True`, the input argument order in the docstring needs to match that in the
 function signature.
 
-To turn this optoin on/off, do this:
+To turn this option on/off, do this:
 
 ```
 pydoclint --check-arg-order=False <FILE_OR_FOLDER>
 ```
 
 or
 
@@ -227,15 +267,15 @@
 ```
 
 ### 4.6. `--skip-checking-short-docstrings` (shortform: `-scsd`, default: `True`)
 
 If `True`, `pydoclint` won't check functions that have only a short description
 in their docstring.
 
-To turn this optoin on/off, do this:
+To turn this option on/off, do this:
 
 ```
 pydoclint --skip-checking-short-docstrings=False <FILE_OR_FOLDER>
 ```
 
 or
 
@@ -250,7 +290,13 @@
 docstring (or vice versa).
 
 ### 4.8. `--allow-init-docstring` (shortform: `-aid`, default: `False`)
 
 If it is set to `True`, having a docstring for class constructors
 (`__init__()`) is allowed, and the arguments are expected to be documented
 under `__init__()` rather than in the class docstring.
+
+### 4.9. `--require-return-section-when-returning-none` (shortform: `-rrs`, default: `False`)
+
+If `False`, a "return" section is not necessary in the docstring if the
+function implicitly returns `None` (for example, doesn't have a return
+statement, or has `-> None` as the return annotation).
```

### Comparing `pydoclint-0.0.4/README.md` & `pydoclint-0.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: pydoclint
+Version: 0.0.5
+Summary: A linter to check arguments in Python docstrings
+Home-page: https://github.com/jsh9/pydoclint
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pydoclint
 
 A Python docstring linter to check whether a docstring's sections (arguments,
 returns, raises, ...) match the function signature or function implementation.
 
 It runs really fast. In fact, it is at least ~1,475 times faster than
 [darglint](https://github.com/terrencepreilly/darglint) (another linter of the
@@ -59,24 +72,74 @@
 other built-in _flake8_ linters on your code.
 
 ### 2.3. Native vs _flake8_
 
 Should I use _pydoclint_ as a native command line tool or a _flake8_ plugin?
 Here's comparison:
 
-|                 | Pros                                       | Cons                                                          |
-| --------------- | ------------------------------------------ | ------------------------------------------------------------- |
-| Native tool     | Slightly faster                            | No per-line or project-wide omission support right now [*]    |
-| _flake8_ plugin | Supports per-line or project-wide omission | Slightly slower because other flake8 plugins are run together |
+|                 | Pros                                     | Cons                                                          |
+| --------------- | ---------------------------------------- | ------------------------------------------------------------- |
+| Native tool     | Slightly faster                          | No inline or project-wide omission support right now [*]      |
+| _flake8_ plugin | Supports inline or project-wide omission | Slightly slower because other flake8 plugins are run together |
 
 \*) This feature may be added in the near future
 
+### 2.4. Configuration
+
+Here is how to configure _pydoclint_. For detailed explanations of all options,
+see [Section 4](#4-configuration-options) below.
+
+#### 2.4.1. Setting options inline
+
+- Native:
+
+  ```bash
+  pydoclint --check-arg-order=False <FILE_OR_FOLDER_PATH>
+  ```
+
+- Flake8:
+
+  ```bash
+  flake8 --check-arg-order=False <FILE_OR_FOLDER_PATH>
+  ```
+
+#### 2.4.2. Setting options in a configuration file
+
+- Native:
+
+  - In a `.toml` file somewhere in your project folder, add a section like this
+    (put in the config that you need):
+
+    ```toml
+    [tool.pydoclint]
+    style = 'google'
+    exclude = '\.git|\.tox|tests/data|some_script\.py'
+    require-return-section-when-returning-none = true
+    ```
+
+  - Then, specify the path of the `.toml` file in your command:
+
+    ```bash
+    pydoclint --config=path/to/my/config.toml <FILE_OR_FOLDER_PATH>
+    ```
+
+- Flake8:
+  - In your flake8 config file (see
+    [flake8's official doc](https://flake8.pycqa.org/en/latest/user/configuration.html#configuration-locations)),
+    add the config you need under the section `[flake8]`
+
 ## 3. Style violation codes
 
-`pydoclint` currently has the following style violation codes:
+_pydoclint_ currently has the following style violation codes:
+
+### 3.0. `DOC0xx`: Docstring parsing issues
+
+| Code     | Explanation                              |
+| -------- | ---------------------------------------- |
+| `DOC001` | Potential formatting errors in docstring |
 
 ### 3.1. `DOC1xx`: Violations about input arguments
 
 | Code     | Explanation                                                                                                                                          |
 | -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `DOC101` | Docstring contains fewer arguments than in function signature                                                                                        |
 | `DOC102` | Docstring contains more arguments than in function signature                                                                                         |
@@ -97,14 +160,17 @@
 ### 3.2. `DOC2xx`: Violations about return argument(s)
 
 | Code     | Explanation                                                                                          |
 | -------- | ---------------------------------------------------------------------------------------------------- |
 | `DOC201` | Function/method does not have a return section in docstring                                          |
 | `DOC202` | Function/method has a return section in docstring, but there are no return statements or annotations |
 
+Note on `DOC201`: Methods with `@property` as its last decorator do not need to
+have a return section.
+
 ### 3.3. `DOC3xx`: Violations about class docstring and class constructor
 
 | Code     | Explanation                                                                                             |
 | -------- | ------------------------------------------------------------------------------------------------------- |
 | `DOC301` | `__init__()` should not have a docstring; please combine it with the docstring of the class             |
 | `DOC302` | The class docstring does not need a "Returns" section, because `__init__()` cannot return anything      |
 | `DOC303` | The `__init__()` docstring does not need a "Returns" section, because it cannot return anything         |
@@ -180,15 +246,15 @@
 ```
 
 ### 4.4. `--check-type-hint` (shortform: `-th`, default: `True`)
 
 If `True`, the type hints in the docstring and in the Python code need to
 exactly match.
 
-To turn this optoin on/off, do this:
+To turn this option on/off, do this:
 
 ```
 pydoclint --check-type-hint=False <FILE_OR_FOLDER>
 ```
 
 or
 
@@ -197,15 +263,15 @@
 ```
 
 ### 4.5. `--check-arg-order` (shortform: `-ao`, default: `True`)
 
 If `True`, the input argument order in the docstring needs to match that in the
 function signature.
 
-To turn this optoin on/off, do this:
+To turn this option on/off, do this:
 
 ```
 pydoclint --check-arg-order=False <FILE_OR_FOLDER>
 ```
 
 or
 
@@ -214,15 +280,15 @@
 ```
 
 ### 4.6. `--skip-checking-short-docstrings` (shortform: `-scsd`, default: `True`)
 
 If `True`, `pydoclint` won't check functions that have only a short description
 in their docstring.
 
-To turn this optoin on/off, do this:
+To turn this option on/off, do this:
 
 ```
 pydoclint --skip-checking-short-docstrings=False <FILE_OR_FOLDER>
 ```
 
 or
 
@@ -237,7 +303,13 @@
 docstring (or vice versa).
 
 ### 4.8. `--allow-init-docstring` (shortform: `-aid`, default: `False`)
 
 If it is set to `True`, having a docstring for class constructors
 (`__init__()`) is allowed, and the arguments are expected to be documented
 under `__init__()` rather than in the class docstring.
+
+### 4.9. `--require-return-section-when-returning-none` (shortform: `-rrs`, default: `False`)
+
+If `False`, a "return" section is not necessary in the docstring if the
+function implicitly returns `None` (for example, doesn't have a return
+statement, or has `-> None` as the return annotation).
```

### Comparing `pydoclint-0.0.4/pydoclint/main.py` & `pydoclint-0.0.5/pydoclint/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import ast
 import re
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple
 
 import click
 
+from pydoclint.parse_config import (
+    injectDefaultOptionsFromUserSpecifiedTomlFilePath,
+)
 from pydoclint.utils.violation import Violation
 from pydoclint.visitor import Visitor
 
 
 def validateStyleValue(
         context: click.Context,
         param: click.Parameter,
@@ -19,17 +22,15 @@
         raise click.BadParameter('"--style" must be "numpy" or "google"')
 
     return value
 
 
 @click.command(
     context_settings={'help_option_names': ['-h', '--help']},
-    # While Click does set this field automatically using the docstring, mypyc
-    # (annoyingly) strips them, so we need to set it here too.
-    help='Yes',
+    help='Pydoclint, a linter for Python docstring styles',
 )
 @click.option(
     '-s',
     '--src',
     type=str,
     help='The source code to check',
 )
@@ -95,39 +96,71 @@
     '-aid',
     '--allow-init-docstring',
     type=bool,
     show_default=True,
     default=False,
     help='If True, allow both __init__() and the class def to have docstrings',
 )
+@click.option(
+    '-rrs',
+    '--require-return-section-when-returning-none',
+    type=bool,
+    show_default=True,
+    default=False,
+    help=(
+        'If False, a return section is not needed in docstring if'
+        ' the function body does not have a "return" statement and'
+        ' the return type annotation is "-> None".'
+    ),
+)
 @click.argument(
     'paths',
     nargs=-1,
     type=click.Path(
         exists=True,
         file_okay=True,
         dir_okay=True,
         readable=True,
         allow_dash=True,
     ),
     is_eager=True,
 )
+@click.option(
+    '--config',
+    type=click.Path(
+        exists=True,
+        file_okay=True,
+        dir_okay=False,
+        readable=True,
+        allow_dash=False,
+        path_type=str,
+    ),
+    is_eager=True,
+    callback=injectDefaultOptionsFromUserSpecifiedTomlFilePath,
+    help=(
+        'The full path of the .toml config file that contains the config'
+        ' options; note that the command line options take precedence'
+        ' over the .toml file'
+    ),
+)
 @click.pass_context
-def main(
+def main(  # noqa: C901
         ctx: click.Context,
         quiet: bool,
         exclude: str,
         style: str,
         src: Optional[str],
         paths: Tuple[str, ...],
         check_type_hint: bool,
         check_arg_order: bool,
         skip_checking_short_docstrings: bool,
         skip_checking_raises: bool,
         allow_init_docstring: bool,
+        require_return_section_when_returning_none: bool,
+        config: Optional[str],
 ) -> None:
     """Command-line entry point of pydoclint"""
     ctx.ensure_object(dict)
 
     if paths and src is not None:
         click.echo(
             main.get_usage(ctx)
@@ -147,14 +180,15 @@
         style=style,
         paths=paths,
         checkTypeHint=check_type_hint,
         checkArgOrder=check_arg_order,
         skipCheckingShortDocstrings=skip_checking_short_docstrings,
         skipCheckingRaises=skip_checking_raises,
         allowInitDocstring=allow_init_docstring,
+        requireReturnSectionWhenReturningNone=require_return_section_when_returning_none,
     )
 
     violationCounter: int = 0
     if len(violationsInAllFiles) > 0:
         counter = 0
         for filename, violationsInThisFile in violationsInAllFiles.items():
             counter += 1
@@ -191,14 +225,15 @@
         paths: Tuple[str, ...],
         style: str = 'numpy',
         checkTypeHint: bool = True,
         checkArgOrder: bool = True,
         skipCheckingShortDocstrings: bool = True,
         skipCheckingRaises: bool = False,
         allowInitDocstring: bool = False,
+        requireReturnSectionWhenReturningNone: bool = False,
         quiet: bool = False,
         exclude: str = '',
 ) -> Dict[str, List[Violation]]:
     filenames: List[Path] = []
 
     if not quiet:
         skipMsg = f'Skipping files that match this pattern: {exclude}'
@@ -226,40 +261,43 @@
             filename,
             style=style,
             checkTypeHint=checkTypeHint,
             checkArgOrder=checkArgOrder,
             skipCheckingShortDocstrings=skipCheckingShortDocstrings,
             skipCheckingRaises=skipCheckingRaises,
             allowInitDocstring=allowInitDocstring,
+            requireReturnSectionWhenReturningNone=requireReturnSectionWhenReturningNone,
         )
         allViolations[filename.as_posix()] = violationsInThisFile
 
     return allViolations
 
 
 def _checkFile(
         filename: Path,
         style: str = 'numpy',
         checkTypeHint: bool = True,
         checkArgOrder: bool = True,
         skipCheckingShortDocstrings: bool = True,
         skipCheckingRaises: bool = False,
         allowInitDocstring: bool = False,
+        requireReturnSectionWhenReturningNone: bool = False,
 ) -> List[Violation]:
     with open(filename) as fp:
         src: str = ''.join(fp.readlines())
 
     tree: ast.Module = ast.parse(src)
     visitor = Visitor(
         style=style,
         checkTypeHint=checkTypeHint,
         checkArgOrder=checkArgOrder,
         skipCheckingShortDocstrings=skipCheckingShortDocstrings,
         skipCheckingRaises=skipCheckingRaises,
         allowInitDocstring=allowInitDocstring,
+        requireReturnSectionWhenReturningNone=requireReturnSectionWhenReturningNone,
     )
     visitor.visit(tree)
     return visitor.violations
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pydoclint-0.0.4/pydoclint/utils/annotation.py` & `pydoclint-0.0.5/pydoclint/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.4/pydoclint/utils/arg.py` & `pydoclint-0.0.5/pydoclint/utils/arg.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.4/pydoclint/utils/doc.py` & `pydoclint-0.0.5/pydoclint/utils/doc.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.4/pydoclint/utils/generic.py` & `pydoclint-0.0.5/pydoclint/utils/generic.py`

 * *Files 13% similar despite different names*

```diff
@@ -118,7 +118,18 @@
 
 def getNodeName(node: ast.AST) -> str:
     """Get the name of an AST node"""
     if node is None:
         return ''
 
     return node.name if 'name' in node.__dict__ else ''
+
+
+def isPropertyMethod(node: FuncOrAsyncFuncDef) -> bool:
+    """Check whether a function has `@property` as its last decorator"""
+    return (
+        isinstance(node.decorator_list, list)
+        and len(node.decorator_list) > 0
+        and isinstance(node.decorator_list[-1], ast.Name)
+        and hasattr(node.decorator_list[-1], 'id')
+        and node.decorator_list[-1].id == 'property'
+    )
```

### Comparing `pydoclint-0.0.4/pydoclint/utils/return_yield_raise.py` & `pydoclint-0.0.5/pydoclint/utils/return_yield_raise.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 
 
 def hasReturnAnnotation(node: FuncOrAsyncFuncDef) -> bool:
     """Check whether the function node has a return type annotation"""
     return node.returns is not None
 
 
+def isReturnAnnotationNone(node: FuncOrAsyncFuncDef) -> bool:
+    """Check whether the return type annotation if `None`"""
+    return _isNone(node.returns)
+
+
 def hasGeneratorAsReturnAnnotation(node: FuncOrAsyncFuncDef) -> bool:
     """Check whether the function node has a 'Generator' return annotation"""
     if node.returns is None:
         return False
 
     returnAnnotation: str = unparseAnnotation(node.returns)
     return returnAnnotation.startswith('Generator')
@@ -70,7 +75,11 @@
                 if thisId == parentId:
                     return True
 
             if isinstance(parent, BlockType):
                 return True
 
     return False
+
+
+def _isNone(node: ast.AST) -> bool:
+    return isinstance(node, ast.Constant) and node.value is None
```

### Comparing `pydoclint-0.0.4/pydoclint/utils/unparser.py` & `pydoclint-0.0.5/pydoclint/utils/unparser.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.4/pydoclint/utils/violation.py` & `pydoclint-0.0.5/pydoclint/utils/violation.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.4/pydoclint/utils/walk.py` & `pydoclint-0.0.5/pydoclint/utils/walk.py`

 * *Files identical despite different names*

### Comparing `pydoclint-0.0.4/pydoclint/visitor.py` & `pydoclint-0.0.5/pydoclint/visitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 from pydoclint.utils.astTypes import FuncOrAsyncFuncDef
 from pydoclint.utils.doc import Doc
 from pydoclint.utils.generic import (
     collectFuncArgs,
     detectMethodType,
     generateMsgPrefix,
     getDocstring,
+    isPropertyMethod,
 )
 from pydoclint.utils.internal_error import InternalError
 from pydoclint.utils.method_type import MethodType
 from pydoclint.utils.return_yield_raise import (
     hasGeneratorAsReturnAnnotation,
     hasRaiseStatements,
     hasReturnAnnotation,
     hasReturnStatements,
     hasYieldStatements,
+    isReturnAnnotationNone,
 )
 from pydoclint.utils.violation import Violation
 
 
 class Visitor(ast.NodeVisitor):
     """A class to recursively visit all the nodes in a parsed module"""
 
@@ -29,21 +31,25 @@
             self,
             style: str = 'numpy',
             checkTypeHint: bool = True,
             checkArgOrder: bool = True,
             skipCheckingShortDocstrings: bool = True,
             skipCheckingRaises: bool = False,
             allowInitDocstring: bool = False,
+            requireReturnSectionWhenReturningNone: bool = False,
     ) -> None:
         self.style: str = style
         self.checkTypeHint: bool = checkTypeHint
         self.checkArgOrder: bool = checkArgOrder
         self.skipCheckingShortDocstrings: bool = skipCheckingShortDocstrings
         self.skipCheckingRaises: bool = skipCheckingRaises
         self.allowInitDocstring: bool = allowInitDocstring
+        self.requireReturnSectionWhenReturningNone: bool = (
+            requireReturnSectionWhenReturningNone
+        )
 
         self.parent: Optional[ast.AST] = None  # keep track of parent node
         self.violations: List[Violation] = []
 
     def visit_ClassDef(self, node: ast.ClassDef):  # noqa: D102
         currentParent = self.parent  # keep aside
         self.parent = node
@@ -370,17 +376,16 @@
                         msgPrefix=msgPrefix,
                         msgPostfix=' '.join(msgPostfixParts),
                     )
                 )
 
         return violations
 
-    @classmethod
     def checkReturns(
-            cls,
+            self,
             node: FuncOrAsyncFuncDef,
             parent: ast.AST,
             doc: Doc,
     ) -> List[Violation]:
         """Check return statement & return type annotation of this function"""
         lineNum: int = node.lineno
         msgPrefix = generateMsgPrefix(node, parent, appendColon=False)
@@ -391,20 +396,23 @@
         hasReturnStmt: bool = hasReturnStatements(node)
         hasReturnAnno: bool = hasReturnAnnotation(node)
         hasGenAsRetAnno: bool = hasGeneratorAsReturnAnnotation(node)
 
         docstringHasReturnSection: bool = doc.hasReturnsSection
 
         violations: List[Violation] = []
-        if not docstringHasReturnSection:
+        if not docstringHasReturnSection and not isPropertyMethod(node):
             if hasReturnStmt or (hasReturnAnno and not hasGenAsRetAnno):
                 # If "Generator[...]" is put in the return type annotation,
                 # we don't need a "Returns" section in the docstring. Instead,
                 # we need a "Yields" section.
-                violations.append(v201)
+                if self.requireReturnSectionWhenReturningNone:
+                    violations.append(v201)
+                elif not isReturnAnnotationNone(node):
+                    violations.append(v201)
 
         if docstringHasReturnSection and not (hasReturnStmt or hasReturnAnno):
             violations.append(v202)
 
         return violations
 
     @classmethod
```

### Comparing `pydoclint-0.0.4/pydoclint.egg-info/PKG-INFO` & `pydoclint-0.0.5/pydoclint.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydoclint
-Version: 0.0.4
+Version: 0.0.5
 Summary: A linter to check arguments in Python docstrings
 Home-page: https://github.com/jsh9/pydoclint
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
@@ -72,24 +72,74 @@
 other built-in _flake8_ linters on your code.
 
 ### 2.3. Native vs _flake8_
 
 Should I use _pydoclint_ as a native command line tool or a _flake8_ plugin?
 Here's comparison:
 
-|                 | Pros                                       | Cons                                                          |
-| --------------- | ------------------------------------------ | ------------------------------------------------------------- |
-| Native tool     | Slightly faster                            | No per-line or project-wide omission support right now [*]    |
-| _flake8_ plugin | Supports per-line or project-wide omission | Slightly slower because other flake8 plugins are run together |
+|                 | Pros                                     | Cons                                                          |
+| --------------- | ---------------------------------------- | ------------------------------------------------------------- |
+| Native tool     | Slightly faster                          | No inline or project-wide omission support right now [*]      |
+| _flake8_ plugin | Supports inline or project-wide omission | Slightly slower because other flake8 plugins are run together |
 
 \*) This feature may be added in the near future
 
+### 2.4. Configuration
+
+Here is how to configure _pydoclint_. For detailed explanations of all options,
+see [Section 4](#4-configuration-options) below.
+
+#### 2.4.1. Setting options inline
+
+- Native:
+
+  ```bash
+  pydoclint --check-arg-order=False <FILE_OR_FOLDER_PATH>
+  ```
+
+- Flake8:
+
+  ```bash
+  flake8 --check-arg-order=False <FILE_OR_FOLDER_PATH>
+  ```
+
+#### 2.4.2. Setting options in a configuration file
+
+- Native:
+
+  - In a `.toml` file somewhere in your project folder, add a section like this
+    (put in the config that you need):
+
+    ```toml
+    [tool.pydoclint]
+    style = 'google'
+    exclude = '\.git|\.tox|tests/data|some_script\.py'
+    require-return-section-when-returning-none = true
+    ```
+
+  - Then, specify the path of the `.toml` file in your command:
+
+    ```bash
+    pydoclint --config=path/to/my/config.toml <FILE_OR_FOLDER_PATH>
+    ```
+
+- Flake8:
+  - In your flake8 config file (see
+    [flake8's official doc](https://flake8.pycqa.org/en/latest/user/configuration.html#configuration-locations)),
+    add the config you need under the section `[flake8]`
+
 ## 3. Style violation codes
 
-`pydoclint` currently has the following style violation codes:
+_pydoclint_ currently has the following style violation codes:
+
+### 3.0. `DOC0xx`: Docstring parsing issues
+
+| Code     | Explanation                              |
+| -------- | ---------------------------------------- |
+| `DOC001` | Potential formatting errors in docstring |
 
 ### 3.1. `DOC1xx`: Violations about input arguments
 
 | Code     | Explanation                                                                                                                                          |
 | -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `DOC101` | Docstring contains fewer arguments than in function signature                                                                                        |
 | `DOC102` | Docstring contains more arguments than in function signature                                                                                         |
@@ -110,14 +160,17 @@
 ### 3.2. `DOC2xx`: Violations about return argument(s)
 
 | Code     | Explanation                                                                                          |
 | -------- | ---------------------------------------------------------------------------------------------------- |
 | `DOC201` | Function/method does not have a return section in docstring                                          |
 | `DOC202` | Function/method has a return section in docstring, but there are no return statements or annotations |
 
+Note on `DOC201`: Methods with `@property` as its last decorator do not need to
+have a return section.
+
 ### 3.3. `DOC3xx`: Violations about class docstring and class constructor
 
 | Code     | Explanation                                                                                             |
 | -------- | ------------------------------------------------------------------------------------------------------- |
 | `DOC301` | `__init__()` should not have a docstring; please combine it with the docstring of the class             |
 | `DOC302` | The class docstring does not need a "Returns" section, because `__init__()` cannot return anything      |
 | `DOC303` | The `__init__()` docstring does not need a "Returns" section, because it cannot return anything         |
@@ -193,15 +246,15 @@
 ```
 
 ### 4.4. `--check-type-hint` (shortform: `-th`, default: `True`)
 
 If `True`, the type hints in the docstring and in the Python code need to
 exactly match.
 
-To turn this optoin on/off, do this:
+To turn this option on/off, do this:
 
 ```
 pydoclint --check-type-hint=False <FILE_OR_FOLDER>
 ```
 
 or
 
@@ -210,15 +263,15 @@
 ```
 
 ### 4.5. `--check-arg-order` (shortform: `-ao`, default: `True`)
 
 If `True`, the input argument order in the docstring needs to match that in the
 function signature.
 
-To turn this optoin on/off, do this:
+To turn this option on/off, do this:
 
 ```
 pydoclint --check-arg-order=False <FILE_OR_FOLDER>
 ```
 
 or
 
@@ -227,15 +280,15 @@
 ```
 
 ### 4.6. `--skip-checking-short-docstrings` (shortform: `-scsd`, default: `True`)
 
 If `True`, `pydoclint` won't check functions that have only a short description
 in their docstring.
 
-To turn this optoin on/off, do this:
+To turn this option on/off, do this:
 
 ```
 pydoclint --skip-checking-short-docstrings=False <FILE_OR_FOLDER>
 ```
 
 or
 
@@ -250,7 +303,13 @@
 docstring (or vice versa).
 
 ### 4.8. `--allow-init-docstring` (shortform: `-aid`, default: `False`)
 
 If it is set to `True`, having a docstring for class constructors
 (`__init__()`) is allowed, and the arguments are expected to be documented
 under `__init__()` rather than in the class docstring.
+
+### 4.9. `--require-return-section-when-returning-none` (shortform: `-rrs`, default: `False`)
+
+If `False`, a "return" section is not necessary in the docstring if the
+function implicitly returns `None` (for example, doesn't have a return
+statement, or has `-> None` as the return annotation).
```

### Comparing `pydoclint-0.0.4/setup.cfg` & `pydoclint-0.0.5/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pydoclint
-version = 0.0.4
+version = 0.0.5
 description = A linter to check arguments in Python docstrings
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jsh9/pydoclint
 license = MIT
 license_file = LICENSE
 classifiers = 
@@ -15,14 +15,15 @@
 [options]
 packages = find:
 install_requires = 
 	flake8>=4
 	click>=8.0.0
 	numpydoc>=1.5.0
 	docstring_parser>=0.15
+	tomli>=2.0.1; python_version<'3.11'
 python_requires = >=3.8
 
 [options.packages.find]
 exclude = 
 	tests*
 	testing*
```

### Comparing `pydoclint-0.0.4/tests/test_main.py` & `pydoclint-0.0.5/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,14 +221,15 @@
         ),
     ),
 )
 def testReturns(style: str, filename: str) -> None:
     violations = _checkFile(
         filename=DATA_DIR / f'{style}/returns/{filename}',
         skipCheckingShortDocstrings=False,
+        requireReturnSectionWhenReturningNone=True,
         style=style,
     )
 
     expectedViolations: List[str] = [
         'DOC201: Method `MyClass.func1_3` does not have a return section in '
         'docstring ',
         'DOC201: Method `MyClass.func1_5` does not have a return section in '
@@ -485,14 +486,62 @@
         'docstring. Error message: The section Parameters appears twice in  Some '
         'class  Parameters ----------     arg1     arg2  Parameters ----------     '
         'arg3     arg4'
     ]
     assert list(map(str, violations)) == expected
 
 
+@pytest.mark.parametrize(
+    'style, rrs',
+    itertools.product(
+        ['numpy', 'google'],
+        [False, True],
+    ),
+)
+def testNoReturnSection(
+        style: str,
+        rrs: bool,
+) -> None:
+    violations = _checkFile(
+        filename=DATA_DIR / f'{style}/no_return_section/cases.py',
+        style=style,
+        requireReturnSectionWhenReturningNone=rrs,
+    )
+    expected_lookup = {
+        True: [
+            'DOC201: Function `func1` does not have a return section in docstring ',
+            'DOC201: Function `func2` does not have a return section in docstring ',
+            'DOC201: Function `func3` does not have a return section in docstring ',
+            'DOC201: Function `func4` does not have a return section in docstring ',
+            'DOC201: Function `func5` does not have a return section in docstring ',
+        ],
+        False: [
+            'DOC201: Function `func2` does not have a return section in docstring ',
+            'DOC201: Function `func3` does not have a return section in docstring ',
+            'DOC201: Function `func4` does not have a return section in docstring ',
+            'DOC201: Function `func5` does not have a return section in docstring ',
+        ],
+    }
+    assert list(map(str, violations)) == expected_lookup[rrs]
+
+
+@pytest.mark.parametrize(
+    'style',
+    ['numpy', 'google'],
+)
+def testPropertyMethod(style: str) -> None:
+    violations = _checkFile(
+        filename=DATA_DIR / f'{style}/property_method/cases.py',
+        style=style,
+        skipCheckingShortDocstrings=True,
+    )
+    expected = []
+    assert list(map(str, violations)) == expected
+
+
 def testPlayground() -> None:
     """
     This is a placeholder test for testing the `playground.py` file.
 
     When you want to quickly test something, you can add contents into
     tests/data/playground.py and run this test function.
     """
```

