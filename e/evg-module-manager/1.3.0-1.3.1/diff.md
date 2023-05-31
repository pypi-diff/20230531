# Comparing `tmp/evg_module_manager-1.3.0.tar.gz` & `tmp/evg_module_manager-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evg_module_manager-1.3.0.tar", max compression
+gzip compressed data, was "evg_module_manager-1.3.1.tar", max compression
```

## Comparing `evg_module_manager-1.3.0.tar` & `evg_module_manager-1.3.1.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0    11337 2022-10-20 00:47:42.875216 evg_module_manager-1.3.0/LICENSE
--rw-r--r--   0        0        0     7017 2022-10-20 00:47:42.875216 evg_module_manager-1.3.0/README.md
--rw-r--r--   0        0        0     1815 2022-10-20 00:47:42.943216 evg_module_manager-1.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-10-20 00:47:42.943216 evg_module_manager-1.3.0/src/emm/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 00:47:42.943216 evg_module_manager-1.3.0/src/emm/cli/__init__.py
--rw-r--r--   0        0        0     2967 2022-10-20 00:47:42.943216 evg_module_manager-1.3.0/src/emm/cli/evg_cli.py
--rw-r--r--   0        0        0    12567 2022-10-20 00:47:42.943216 evg_module_manager-1.3.0/src/emm/cli/git_cli.py
--rw-r--r--   0        0        0        0 2022-10-20 00:47:42.943216 evg_module_manager-1.3.0/src/emm/clients/__init__.py
--rw-r--r--   0        0        0     5293 2022-10-20 00:47:42.943216 evg_module_manager-1.3.0/src/emm/clients/evg_cli_service.py
--rw-r--r--   0        0        0     3369 2022-10-20 00:47:42.943216 evg_module_manager-1.3.0/src/emm/clients/evg_service.py
--rw-r--r--   0        0        0    11653 2022-10-20 00:47:42.943216 evg_module_manager-1.3.0/src/emm/clients/git_proxy.py
--rw-r--r--   0        0        0     2829 2022-10-20 00:47:42.943216 evg_module_manager-1.3.0/src/emm/clients/github_service.py
--rw-r--r--   0        0        0    11605 2022-10-20 00:47:42.943216 evg_module_manager-1.3.0/src/emm/emm_cli.py
--rw-r--r--   0        0        0        0 2022-10-20 00:47:42.943216 evg_module_manager-1.3.0/src/emm/models/__init__.py
--rw-r--r--   0        0        0     1445 2022-10-20 00:47:42.943216 evg_module_manager-1.3.0/src/emm/models/repository.py
--rw-r--r--   0        0        0     1770 2022-10-20 00:47:42.943216 evg_module_manager-1.3.0/src/emm/options.py
--rw-r--r--   0        0        0        0 2022-10-20 00:47:42.943216 evg_module_manager-1.3.0/src/emm/services/__init__.py
--rw-r--r--   0        0        0     1644 2022-10-20 00:47:42.943216 evg_module_manager-1.3.0/src/emm/services/file_service.py
--rw-r--r--   0        0        0     5073 2022-10-20 00:47:42.943216 evg_module_manager-1.3.0/src/emm/services/git_branch_service.py
--rw-r--r--   0        0        0     6588 2022-10-20 00:47:42.943216 evg_module_manager-1.3.0/src/emm/services/git_commit_service.py
--rw-r--r--   0        0        0     9597 2022-10-20 00:47:42.943216 evg_module_manager-1.3.0/src/emm/services/modules_service.py
--rw-r--r--   0        0        0     2610 2022-10-20 00:47:42.943216 evg_module_manager-1.3.0/src/emm/services/patch_service.py
--rw-r--r--   0        0        0     5764 2022-10-20 00:47:42.943216 evg_module_manager-1.3.0/src/emm/services/pull_request_service.py
--rw-r--r--   0        0        0     2239 2022-10-20 00:47:42.943216 evg_module_manager-1.3.0/src/emm/services/validation_service.py
--rw-r--r--   0        0        0     8357 1970-01-01 00:00:00.000000 evg_module_manager-1.3.0/setup.py
--rw-r--r--   0        0        0     8200 1970-01-01 00:00:00.000000 evg_module_manager-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-05-31 08:18:33.116995 evg_module_manager-1.3.1/LICENSE
+-rw-r--r--   0        0        0     7017 2023-05-31 08:18:33.116995 evg_module_manager-1.3.1/README.md
+-rw-r--r--   0        0        0     1856 2023-05-31 08:18:33.204996 evg_module_manager-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-31 08:18:33.204996 evg_module_manager-1.3.1/src/emm/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:18:33.204996 evg_module_manager-1.3.1/src/emm/cli/__init__.py
+-rw-r--r--   0        0        0     2967 2023-05-31 08:18:33.208996 evg_module_manager-1.3.1/src/emm/cli/evg_cli.py
+-rw-r--r--   0        0        0    12567 2023-05-31 08:18:33.208996 evg_module_manager-1.3.1/src/emm/cli/git_cli.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:18:33.208996 evg_module_manager-1.3.1/src/emm/clients/__init__.py
+-rw-r--r--   0        0        0     5293 2023-05-31 08:18:33.208996 evg_module_manager-1.3.1/src/emm/clients/evg_cli_service.py
+-rw-r--r--   0        0        0     3369 2023-05-31 08:18:33.208996 evg_module_manager-1.3.1/src/emm/clients/evg_service.py
+-rw-r--r--   0        0        0    11653 2023-05-31 08:18:33.208996 evg_module_manager-1.3.1/src/emm/clients/git_proxy.py
+-rw-r--r--   0        0        0     2829 2023-05-31 08:18:33.208996 evg_module_manager-1.3.1/src/emm/clients/github_service.py
+-rw-r--r--   0        0        0    11605 2023-05-31 08:18:33.208996 evg_module_manager-1.3.1/src/emm/emm_cli.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:18:33.208996 evg_module_manager-1.3.1/src/emm/models/__init__.py
+-rw-r--r--   0        0        0     1445 2023-05-31 08:18:33.208996 evg_module_manager-1.3.1/src/emm/models/repository.py
+-rw-r--r--   0        0        0     1770 2023-05-31 08:18:33.208996 evg_module_manager-1.3.1/src/emm/options.py
+-rw-r--r--   0        0        0        0 2023-05-31 08:18:33.208996 evg_module_manager-1.3.1/src/emm/services/__init__.py
+-rw-r--r--   0        0        0     1644 2023-05-31 08:18:33.208996 evg_module_manager-1.3.1/src/emm/services/file_service.py
+-rw-r--r--   0        0        0     5073 2023-05-31 08:18:33.208996 evg_module_manager-1.3.1/src/emm/services/git_branch_service.py
+-rw-r--r--   0        0        0     6588 2023-05-31 08:18:33.208996 evg_module_manager-1.3.1/src/emm/services/git_commit_service.py
+-rw-r--r--   0        0        0     9597 2023-05-31 08:18:33.208996 evg_module_manager-1.3.1/src/emm/services/modules_service.py
+-rw-r--r--   0        0        0     2610 2023-05-31 08:18:33.208996 evg_module_manager-1.3.1/src/emm/services/patch_service.py
+-rw-r--r--   0        0        0     5764 2023-05-31 08:18:33.208996 evg_module_manager-1.3.1/src/emm/services/pull_request_service.py
+-rw-r--r--   0        0        0     2239 2023-05-31 08:18:33.208996 evg_module_manager-1.3.1/src/emm/services/validation_service.py
+-rw-r--r--   0        0        0     8235 1970-01-01 00:00:00.000000 evg_module_manager-1.3.1/PKG-INFO
```

### Comparing `evg_module_manager-1.3.0/LICENSE` & `evg_module_manager-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `evg_module_manager-1.3.0/README.md` & `evg_module_manager-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `evg_module_manager-1.3.0/pyproject.toml` & `evg_module_manager-1.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "evg-module-manager"
-version = "1.3.0"
+version = "1.3.1"
 description = "Manage Evergreen modules locally."
 authors = ["Dev Prod DAG <dev-prod-dag@mongodb.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/evergreen-ci/evg-module-manager"
 documentation = "https://evergreen-ci.github.io/evg-module-manager/"
 packages = [
@@ -22,29 +22,31 @@
 Inject = "^4.3.1"
 structlog = "^21.1.0"
 PyYAML = "^5.4.1"
 xdg = "^5.1.1"
 pydantic = "^1.8.2"
 rich = "^10.9.0"
 "shrub.py" = "^3.0.1"
+urllib3 = "1.26.15"
 
-[tool.poetry.dev-dependencies]
-pytest = "^6.2"
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.0"
 black = "^22.3"
 pytest-black = "^0.3"
 pytest-cov = "^2.8"
 pytest-flake8 = "^1.0"
 pytest-mypy = "^0.8"
 mypy = "^0.910"
-pytest-pydocstyle = "^2.0"
+pytest-pydocstyle = "^2.3"
 pre-commit = "^2.6"
 pytest-isort = "^2.0"
 flake8-bugbear = "^21.4"
 types-PyYAML = "^5.4.10"
 flake8 = "3.9.2"
+py = "^1.11.0"
 
 [tool.black]
 line-length = 100
 target-version = ['py39']
 
 [tool.isort]
 multi_line_output = 3
```

### Comparing `evg_module_manager-1.3.0/src/emm/cli/evg_cli.py` & `evg_module_manager-1.3.1/src/emm/cli/evg_cli.py`

 * *Files identical despite different names*

### Comparing `evg_module_manager-1.3.0/src/emm/cli/git_cli.py` & `evg_module_manager-1.3.1/src/emm/cli/git_cli.py`

 * *Files identical despite different names*

### Comparing `evg_module_manager-1.3.0/src/emm/clients/evg_cli_service.py` & `evg_module_manager-1.3.1/src/emm/clients/evg_cli_service.py`

 * *Files identical despite different names*

### Comparing `evg_module_manager-1.3.0/src/emm/clients/evg_service.py` & `evg_module_manager-1.3.1/src/emm/clients/evg_service.py`

 * *Files identical despite different names*

### Comparing `evg_module_manager-1.3.0/src/emm/clients/git_proxy.py` & `evg_module_manager-1.3.1/src/emm/clients/git_proxy.py`

 * *Files identical despite different names*

### Comparing `evg_module_manager-1.3.0/src/emm/clients/github_service.py` & `evg_module_manager-1.3.1/src/emm/clients/github_service.py`

 * *Files identical despite different names*

### Comparing `evg_module_manager-1.3.0/src/emm/emm_cli.py` & `evg_module_manager-1.3.1/src/emm/emm_cli.py`

 * *Files identical despite different names*

### Comparing `evg_module_manager-1.3.0/src/emm/models/repository.py` & `evg_module_manager-1.3.1/src/emm/models/repository.py`

 * *Files identical despite different names*

### Comparing `evg_module_manager-1.3.0/src/emm/options.py` & `evg_module_manager-1.3.1/src/emm/options.py`

 * *Files identical despite different names*

### Comparing `evg_module_manager-1.3.0/src/emm/services/file_service.py` & `evg_module_manager-1.3.1/src/emm/services/file_service.py`

 * *Files identical despite different names*

### Comparing `evg_module_manager-1.3.0/src/emm/services/git_branch_service.py` & `evg_module_manager-1.3.1/src/emm/services/git_branch_service.py`

 * *Files identical despite different names*

### Comparing `evg_module_manager-1.3.0/src/emm/services/git_commit_service.py` & `evg_module_manager-1.3.1/src/emm/services/git_commit_service.py`

 * *Files identical despite different names*

### Comparing `evg_module_manager-1.3.0/src/emm/services/modules_service.py` & `evg_module_manager-1.3.1/src/emm/services/modules_service.py`

 * *Files identical despite different names*

### Comparing `evg_module_manager-1.3.0/src/emm/services/patch_service.py` & `evg_module_manager-1.3.1/src/emm/services/patch_service.py`

 * *Files identical despite different names*

### Comparing `evg_module_manager-1.3.0/src/emm/services/pull_request_service.py` & `evg_module_manager-1.3.1/src/emm/services/pull_request_service.py`

 * *Files identical despite different names*

### Comparing `evg_module_manager-1.3.0/src/emm/services/validation_service.py` & `evg_module_manager-1.3.1/src/emm/services/validation_service.py`

 * *Files identical despite different names*

### Comparing `evg_module_manager-1.3.0/setup.py` & `evg_module_manager-1.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,229 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: evg-module-manager
+Version: 1.3.1
+Summary: Manage Evergreen modules locally.
+Home-page: https://github.com/evergreen-ci/evg-module-manager
+License: Apache-2.0
+Author: Dev Prod DAG
+Author-email: dev-prod-dag@mongodb.com
+Requires-Python: >=3.7.1,<4.0.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Inject (>=4.3.1,<5.0.0)
+Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
+Requires-Dist: click (>=8,<9)
+Requires-Dist: evergreen.py (>=3.2.7,<4.0.0)
+Requires-Dist: plumbum (>=1.7.0,<2.0.0)
+Requires-Dist: pydantic (>=1.8.2,<2.0.0)
+Requires-Dist: rich (>=10.9.0,<11.0.0)
+Requires-Dist: shrub.py (>=3.0.1,<4.0.0)
+Requires-Dist: structlog (>=21.1.0,<22.0.0)
+Requires-Dist: urllib3 (==1.26.15)
+Requires-Dist: xdg (>=5.1.1,<6.0.0)
+Project-URL: Documentation, https://evergreen-ci.github.io/evg-module-manager/
+Project-URL: Repository, https://github.com/evergreen-ci/evg-module-manager
+Description-Content-Type: text/markdown
+
+# Evergreen Module Manager
+
+Manage Evergreen modules in your local environment.
+
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/evg-module-manager) [![PyPI](https://img.shields.io/pypi/v/evg-module-manager.svg)](https://pypi.org/project/evg-module-manager/) [![Documentation](https://img.shields.io/badge/Docs-Available-green)](https://evergreen-ci.github.io/evg-module-manager/)
+## Table of contents
+
+1. [Description](#description)
+2. [Getting Help](#getting-help)
+3. [Documentation](#documentation)
+4. [Dependencies](#dependencies)
+5. [Installation](#installation)
+6. [Usage](#usage)
+7. [Contributor's Guide](#contributors-guide)
+    - [Setting up a local development environment](#setting-up-a-local-development-environment)
+    - [linting/formatting](#lintingformatting)
+    - [Running tests](#running-tests)
+    - [Automatically running checks on commit](#automatically-running-checks-on-commit)
+    - [Versioning](#versioning)
+    - [Code Review](#code-review)
+    - [Deployment](#deployment)
+8. [Resources](#resources)
+
+## Description
+
+The evg-module-manager is a tool to help improve the local workflows of working with modules in
+your evergreen projects. It will help you keep any modules defined in your local project in sync.
+It supports the following functionality:
+
+* List what modules are defined in the local project.
+* List what modules are currently active in your local repo.
+* Clone a module repository.
+* Enable/disable modules in your local repo.
+* Create an evergreen patch build that includes changes from the local patch build and all enabled
+  modules.
+* Submit a changes to the commit-queue that includes changes from the local patch build and all
+  enabled modules.
+
+## Getting Help
+
+### What's the right channel to ask my question?
+If you have a question about evg-module-manager, please mention @dag-on-call in the
+slack channel [#evergreen-users](https://mongodb.slack.com/messages/#evergreen-users/)
+or email us at
+dev-prod-dag@mongodb.com.
+
+### How can I request a change/report a bug in evg-module-manager?
+Create a [DAG ticket](https://jira.mongodb.org/projects/DAG).
+
+### What should I include in my ticket or #evergreen-users question?
+Since #evergreen-users questions are interrupts,
+please include as much information as possible.
+This can help avoid long information-gathering threads.
+
+Please include the following in any created tickets:
+* **Motivation for Request**
+  * Provide us the motivation for this change.
+* **Context**
+  * Provide some background context for this issue.
+* **Description**
+  * Provide some description on how this issue happened.
+
+## Documentation
+
+Read the documentation [here](https://evergreen-ci.github.io/evg-module-manager/).
+
+## Dependencies
+
+* Python 3.7 or later
+* git
+* evergreen command line tool
+* [Evergreen config file](https://github.com/evergreen-ci/evergreen/wiki/Using-the-Command-Line-Tool#downloading-the-command-line-tool)
+* [github CLI](https://cli.github.com/)
+
+See [Usage Prerequisites](https://github.com/evergreen-ci/evg-module-manager/blob/main/docs/usage.md#prerequities)
+for more details.
+
+## Installation
+
+We strongly recommend using a tool like [pipx](https://pypa.github.io/pipx/) to install
+this tool. This will isolate the dependencies and ensure they don't conflict with other tools.
+
+```bash
+$ pipx install evg-module-manager
+```
+
+### Debugging installation issues
+
+A common issue that arises during installation is pipx failing to install emm and printing out the following error:
+```bash
+$ pipx install evg-module-manager
+Fatal error from pip prevented installation. Full pip output in file:
+    /home/ubuntu/.local/pipx/logs/cmd_2022-03-31_13.24.42_pip_errors.log
+ 
+Some possibly relevant errors from pip install:
+    ERROR: Could not find a version that satisfies the requirement evg-module-manager (from versions: none)
+    ERROR: No matching distribution found for evg-module-manager
+ 
+Error installing evg-module-manager.
+```
+
+This error indicates that pipx could not find a version of emm that was built to support the version of Python installed on your machine.
+Make sure to check that your version of Python matches the requirements called out in the [Dependencies](#dependencies) section. You
+can check the version of Python that is on your computer by running
+```bash
+$ python --version
+```
+
+If you are running into the issue above but are sure that the correct version of Python is installed on your computer,
+you can explicitly specify a path to the correct Python version during installation.
+
+```bash
+$ which python3.9
+/usr/bin/python3.9
+$ pipx install evg-module-manager --python /usr/bin/python3.9
+```
+
+## Usage
+
+See the [documentation](https://evergreen-ci.github.io/evg-module-manager/) for details about using this tool.
+
+```bash
+Usage: evg-module-manager [OPTIONS] COMMAND [ARGS]...
+
+  Evergreen Module Manager is a tool help simplify the local workflows of evergreen modules.
+
+Options:
+  --modules-dir PATH      Directory to store module repositories [default='..']
+  --evg-config-file PATH  Path to file with evergreen auth configuration
+                          [default='/Users/dbradf/.evergreen.yml']
+  --evg-project TEXT      Name of Evergreen project [default='mongodb-mongo-master']
+  --help                  Show this message and exit.
+
+Commands:
+  disable       Disable the specified module in the current repo.
+  enable        Enable the specified module in the current repo.
+  evg           Perform evergreen actions against the base repo and enabled modules.
+  git           Perform git actions against the base repo and enabled modules.
+  list-modules  List the modules available for the current repo.
+  pull-request  Create a Github pull request for changes in the base repository and any...
+```
+
+## Contributor's Guide
+
+### Setting up a local development environment
+
+This project uses [poetry](https://python-poetry.org/) for setting up a local environment.
+
+```bash
+git clone ...
+cd evg-module-manager
+poetry install
+```
+
+### linting/formatting
+
+This project uses [black](https://black.readthedocs.io/en/stable/) and
+[isort](https://pycqa.github.io/isort/) for formatting.
+
+```bash
+poetry run black src tests
+poetry run isort src tests
+```
+
+### Running tests
+
+This project uses [pytest](https://docs.pytest.org/en/6.2.x/) for testing.
+
+```bash
+poetry run pytest
+```
+
+### Automatically running checks on commit
+
+This project has [pre-commit](https://pre-commit.com/) configured. Pre-commit will run
+configured checks at git commit time. To enable pre-commit on your local repository run:
+
+```bash
+poetry run pre-commit install
+```
+
+### Versioning
+
+This project uses [semver](https://semver.org/) for versioning.
+
+Please include a description what is added for each new version in `CHANGELOG.md`.
+
+### Code Review
+
+Please open a Github Pull Request for code review.
 
-package_dir = \
-{'': 'src'}
+### Deployment
 
-packages = \
-['emm', 'emm.cli', 'emm.clients', 'emm.models', 'emm.services']
+Deployment to pypi is automatically triggered on merges to main.
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Inject>=4.3.1,<5.0.0',
- 'PyYAML>=5.4.1,<6.0.0',
- 'click>=8,<9',
- 'evergreen.py>=3.2.7,<4.0.0',
- 'plumbum>=1.7.0,<2.0.0',
- 'pydantic>=1.8.2,<2.0.0',
- 'rich>=10.9.0,<11.0.0',
- 'shrub.py>=3.0.1,<4.0.0',
- 'structlog>=21.1.0,<22.0.0',
- 'xdg>=5.1.1,<6.0.0']
-
-entry_points = \
-{'console_scripts': ['evg-module-manager = emm.emm_cli:cli']}
-
-setup_kwargs = {
-    'name': 'evg-module-manager',
-    'version': '1.3.0',
-    'description': 'Manage Evergreen modules locally.',
-    'long_description': "# Evergreen Module Manager\n\nManage Evergreen modules in your local environment.\n\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/evg-module-manager) [![PyPI](https://img.shields.io/pypi/v/evg-module-manager.svg)](https://pypi.org/project/evg-module-manager/) [![Documentation](https://img.shields.io/badge/Docs-Available-green)](https://evergreen-ci.github.io/evg-module-manager/)\n## Table of contents\n\n1. [Description](#description)\n2. [Getting Help](#getting-help)\n3. [Documentation](#documentation)\n4. [Dependencies](#dependencies)\n5. [Installation](#installation)\n6. [Usage](#usage)\n7. [Contributor's Guide](#contributors-guide)\n    - [Setting up a local development environment](#setting-up-a-local-development-environment)\n    - [linting/formatting](#lintingformatting)\n    - [Running tests](#running-tests)\n    - [Automatically running checks on commit](#automatically-running-checks-on-commit)\n    - [Versioning](#versioning)\n    - [Code Review](#code-review)\n    - [Deployment](#deployment)\n8. [Resources](#resources)\n\n## Description\n\nThe evg-module-manager is a tool to help improve the local workflows of working with modules in\nyour evergreen projects. It will help you keep any modules defined in your local project in sync.\nIt supports the following functionality:\n\n* List what modules are defined in the local project.\n* List what modules are currently active in your local repo.\n* Clone a module repository.\n* Enable/disable modules in your local repo.\n* Create an evergreen patch build that includes changes from the local patch build and all enabled\n  modules.\n* Submit a changes to the commit-queue that includes changes from the local patch build and all\n  enabled modules.\n\n## Getting Help\n\n### What's the right channel to ask my question?\nIf you have a question about evg-module-manager, please mention @dag-on-call in the\nslack channel [#evergreen-users](https://mongodb.slack.com/messages/#evergreen-users/)\nor email us at\ndev-prod-dag@mongodb.com.\n\n### How can I request a change/report a bug in evg-module-manager?\nCreate a [DAG ticket](https://jira.mongodb.org/projects/DAG).\n\n### What should I include in my ticket or #evergreen-users question?\nSince #evergreen-users questions are interrupts,\nplease include as much information as possible.\nThis can help avoid long information-gathering threads.\n\nPlease include the following in any created tickets:\n* **Motivation for Request**\n  * Provide us the motivation for this change.\n* **Context**\n  * Provide some background context for this issue.\n* **Description**\n  * Provide some description on how this issue happened.\n\n## Documentation\n\nRead the documentation [here](https://evergreen-ci.github.io/evg-module-manager/).\n\n## Dependencies\n\n* Python 3.7 or later\n* git\n* evergreen command line tool\n* [Evergreen config file](https://github.com/evergreen-ci/evergreen/wiki/Using-the-Command-Line-Tool#downloading-the-command-line-tool)\n* [github CLI](https://cli.github.com/)\n\nSee [Usage Prerequisites](https://github.com/evergreen-ci/evg-module-manager/blob/main/docs/usage.md#prerequities)\nfor more details.\n\n## Installation\n\nWe strongly recommend using a tool like [pipx](https://pypa.github.io/pipx/) to install\nthis tool. This will isolate the dependencies and ensure they don't conflict with other tools.\n\n```bash\n$ pipx install evg-module-manager\n```\n\n### Debugging installation issues\n\nA common issue that arises during installation is pipx failing to install emm and printing out the following error:\n```bash\n$ pipx install evg-module-manager\nFatal error from pip prevented installation. Full pip output in file:\n    /home/ubuntu/.local/pipx/logs/cmd_2022-03-31_13.24.42_pip_errors.log\n \nSome possibly relevant errors from pip install:\n    ERROR: Could not find a version that satisfies the requirement evg-module-manager (from versions: none)\n    ERROR: No matching distribution found for evg-module-manager\n \nError installing evg-module-manager.\n```\n\nThis error indicates that pipx could not find a version of emm that was built to support the version of Python installed on your machine.\nMake sure to check that your version of Python matches the requirements called out in the [Dependencies](#dependencies) section. You\ncan check the version of Python that is on your computer by running\n```bash\n$ python --version\n```\n\nIf you are running into the issue above but are sure that the correct version of Python is installed on your computer,\nyou can explicitly specify a path to the correct Python version during installation.\n\n```bash\n$ which python3.9\n/usr/bin/python3.9\n$ pipx install evg-module-manager --python /usr/bin/python3.9\n```\n\n## Usage\n\nSee the [documentation](https://evergreen-ci.github.io/evg-module-manager/) for details about using this tool.\n\n```bash\nUsage: evg-module-manager [OPTIONS] COMMAND [ARGS]...\n\n  Evergreen Module Manager is a tool help simplify the local workflows of evergreen modules.\n\nOptions:\n  --modules-dir PATH      Directory to store module repositories [default='..']\n  --evg-config-file PATH  Path to file with evergreen auth configuration\n                          [default='/Users/dbradf/.evergreen.yml']\n  --evg-project TEXT      Name of Evergreen project [default='mongodb-mongo-master']\n  --help                  Show this message and exit.\n\nCommands:\n  disable       Disable the specified module in the current repo.\n  enable        Enable the specified module in the current repo.\n  evg           Perform evergreen actions against the base repo and enabled modules.\n  git           Perform git actions against the base repo and enabled modules.\n  list-modules  List the modules available for the current repo.\n  pull-request  Create a Github pull request for changes in the base repository and any...\n```\n\n## Contributor's Guide\n\n### Setting up a local development environment\n\nThis project uses [poetry](https://python-poetry.org/) for setting up a local environment.\n\n```bash\ngit clone ...\ncd evg-module-manager\npoetry install\n```\n\n### linting/formatting\n\nThis project uses [black](https://black.readthedocs.io/en/stable/) and\n[isort](https://pycqa.github.io/isort/) for formatting.\n\n```bash\npoetry run black src tests\npoetry run isort src tests\n```\n\n### Running tests\n\nThis project uses [pytest](https://docs.pytest.org/en/6.2.x/) for testing.\n\n```bash\npoetry run pytest\n```\n\n### Automatically running checks on commit\n\nThis project has [pre-commit](https://pre-commit.com/) configured. Pre-commit will run\nconfigured checks at git commit time. To enable pre-commit on your local repository run:\n\n```bash\npoetry run pre-commit install\n```\n\n### Versioning\n\nThis project uses [semver](https://semver.org/) for versioning.\n\nPlease include a description what is added for each new version in `CHANGELOG.md`.\n\n### Code Review\n\nPlease open a Github Pull Request for code review.\n\n### Deployment\n\nDeployment to pypi is automatically triggered on merges to main.\n\n## Resources\n\n* [Evergreen REST documentation](https://github.com/evergreen-ci/evergreen/wiki/REST-V2-Usage)\n",
-    'author': 'Dev Prod DAG',
-    'author_email': 'dev-prod-dag@mongodb.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/evergreen-ci/evg-module-manager',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.1,<4.0.0',
-}
+## Resources
 
+* [Evergreen REST documentation](https://github.com/evergreen-ci/evergreen/wiki/REST-V2-Usage)
 
-setup(**setup_kwargs)
```

