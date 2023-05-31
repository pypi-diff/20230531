# Comparing `tmp/robotframework-jupyterlibrary-0.4.2.tar.gz` & `tmp/robotframework_jupyterlibrary-0.5.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-jupyterlibrary-0.4.2.tar", last modified: Sun Jan  1 15:33:49 2023, max compression
+gzip compressed data, was "robotframework_jupyterlibrary-0.5.0a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `robotframework-jupyterlibrary-0.4.2.tar` & `robotframework_jupyterlibrary-0.5.0a0.tar`

### file list

```diff
@@ -1,45 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:33:49.213118 robotframework-jupyterlibrary-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-01-01 15:33:49.213118 robotframework-jupyterlibrary-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-01-01 15:33:49.213118 robotframework-jupyterlibrary-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:33:49.209118 robotframework-jupyterlibrary-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:33:49.209118 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:33:49.209118 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:33:49.209118 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/jupyterlab/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/jupyterlab/Commands.resource
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/jupyterlab/Icons.resource
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/jupyterlab/Launcher.resource
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/jupyterlab/Notebook.resource
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/jupyterlab/Output.resource
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/jupyterlab/PageInfo.resource
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/jupyterlab/Selectors.resource
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/jupyterlab/Settings.resource
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/jupyterlab/Shell.resource
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/jupyterlab/Shortcuts.resource
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/jupyterlab/Sidebar.resource
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:33:49.209118 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/notebook/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/notebook/Commands.resource
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/notebook/Notebook.resource
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/notebook/Output.resource
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/notebook/Selectors.resource
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/notebook/Tree.resource
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:33:49.209118 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/common/CodeMirror.resource
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:33:49.213118 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/keywords/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/keywords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/keywords/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/keywords/webelements.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-01-01 15:32:33.000000 robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/magic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-01 15:33:49.213118 robotframework-jupyterlibrary-0.4.2/src/robotframework_jupyterlibrary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-01-01 15:33:49.000000 robotframework-jupyterlibrary-0.4.2/src/robotframework_jupyterlibrary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-01-01 15:33:49.000000 robotframework-jupyterlibrary-0.4.2/src/robotframework_jupyterlibrary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-01 15:33:49.000000 robotframework-jupyterlibrary-0.4.2/src/robotframework_jupyterlibrary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-01 15:33:49.000000 robotframework-jupyterlibrary-0.4.2/src/robotframework_jupyterlibrary.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-01 15:33:49.000000 robotframework-jupyterlibrary-0.4.2/src/robotframework_jupyterlibrary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-01 15:33:49.000000 robotframework-jupyterlibrary-0.4.2/src/robotframework_jupyterlibrary.egg-info/top_level.txt
+-rw-r--r--   0        0        0       25 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.binder/apt.txt
+-rw-r--r--   0        0        0       52 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.binder/labex.txt
+-rw-r--r--   0        0        0      382 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.binder/postBuild
+-rw-r--r--   0        0        0     2573 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      739 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/ISSUE_TEMPLATE/docs.md
+-rw-r--r--   0        0        0      572 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      903 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/ISSUE_TEMPLATE/release.md
+-rw-r--r--   0        0        0      310 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/env_specs/_base.yml
+-rw-r--r--   0        0        0      172 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/env_specs/docs.yml
+-rw-r--r--   0        0        0      339 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/env_specs/lab3.yml
+-rw-r--r--   0        0        0      268 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/env_specs/lab4.yml
+-rw-r--r--   0        0        0      122 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/env_specs/lint.yml
+-rw-r--r--   0        0        0      257 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/env_specs/meta.yml
+-rw-r--r--   0        0        0      122 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/env_specs/py3.11.yml
+-rw-r--r--   0        0        0      155 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/env_specs/py3.8.yml
+-rw-r--r--   0        0        0       56 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/env_specs/test-py3.7.yml
+-rw-r--r--   0        0        0      116 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/env_specs/test.yml
+-rw-r--r--   0        0        0    16815 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/docs/linux-64/conda.lock
+-rw-r--r--   0        0        0    16034 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/docs/osx-64/conda.lock
+-rw-r--r--   0        0        0    15961 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/docs/win-64/conda.lock
+-rw-r--r--   0        0        0    10412 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/lint/linux-64/conda.lock
+-rw-r--r--   0        0        0     9531 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/lint/osx-64/conda.lock
+-rw-r--r--   0        0        0     9688 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/lint/win-64/conda.lock
+-rw-r--r--   0        0        0    19331 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/meta/linux-64/conda.lock
+-rw-r--r--   0        0        0    18146 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/meta/osx-64/conda.lock
+-rw-r--r--   0        0        0    18114 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/meta/win-64/conda.lock
+-rw-r--r--   0        0        0    19865 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/linux-64/py3.11/lab3/conda.lock
+-rw-r--r--   0        0        0    18584 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/linux-64/py3.11/lab4/conda.lock
+-rw-r--r--   0        0        0    19058 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/linux-64/py3.8/lab3/conda.lock
+-rw-r--r--   0        0        0    17778 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/linux-64/py3.8/lab4/conda.lock
+-rw-r--r--   0        0        0    19323 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/osx-64/py3.11/lab3/conda.lock
+-rw-r--r--   0        0        0    18046 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/osx-64/py3.11/lab4/conda.lock
+-rw-r--r--   0        0        0    18514 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/osx-64/py3.8/lab3/conda.lock
+-rw-r--r--   0        0        0    17238 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/osx-64/py3.8/lab4/conda.lock
+-rw-r--r--   0        0        0    19110 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/win-64/py3.11/lab3/conda.lock
+-rw-r--r--   0        0        0    17833 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/win-64/py3.11/lab4/conda.lock
+-rw-r--r--   0        0        0    18301 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/win-64/py3.8/lab3/conda.lock
+-rw-r--r--   0        0        0    17025 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/locks/test/win-64/py3.8/lab4/conda.lock
+-rw-r--r--   0        0        0      912 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/pull_request_template.md
+-rw-r--r--   0        0        0      994 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/recipe/meta.yaml.in
+-rw-r--r--   0        0        0     5766 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      190 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.gitignore
+-rw-r--r--   0        0        0      313 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/.readthedocs.yml
+-rw-r--r--   0        0        0     3358 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1506 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/LICENSE
+-rw-r--r--   0        0        0     3858 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/README.md
+-rw-r--r--   0        0        0       27 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/_scripts/__init__.py
+-rw-r--r--   0        0        0     4888 2023-05-31 18:21:30.288637 robotframework_jupyterlibrary-0.5.0a0/_scripts/atest.py
+-rw-r--r--   0        0        0      905 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/_scripts/combine.py
+-rw-r--r--   0        0        0     1082 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/_scripts/lint.py
+-rw-r--r--   0        0        0     2426 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/_scripts/lock.py
+-rw-r--r--   0        0        0     9650 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/_scripts/project.py
+-rw-r--r--   0        0        0     1324 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/_scripts/reporter.py
+-rw-r--r--   0        0        0      222 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/00_smoke/00_import.robot
+-rw-r--r--   0        0        0     3128 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/01_server/00_basic.robot
+-rw-r--r--   0        0        0      546 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/__init__.robot
+-rw-r--r--   0        0        0     1100 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/classic/10_notebook.robot
+-rw-r--r--   0        0        0      418 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/classic/__init__.robot
+-rw-r--r--   0        0        0      590 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/lab/00_shell.robot
+-rw-r--r--   0        0        0     2495 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/lab/10_notebook.robot
+-rw-r--r--   0        0        0     1565 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/lab/20_magic.robot
+-rw-r--r--   0        0        0      866 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/lab/30_settings.robot
+-rw-r--r--   0        0        0     2408 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/lab/__init__.robot
+-rw-r--r--   0        0        0     1035 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/notebook/10_notebook.robot
+-rw-r--r--   0        0        0      468 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/atest/notebook/__init__.robot
+-rw-r--r--   0        0        0    10986 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/CI.ipynb
+-rw-r--r--   0        0        0     7065 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/HISTORY.ipynb
+-rw-r--r--   0        0        0     3808 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/INSTALL.ipynb
+-rw-r--r--   0        0        0     3750 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/KEYWORDS.ipynb
+-rw-r--r--   0        0        0     2163 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/LIMITS.ipynb
+-rw-r--r--   0        0        0     5020 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/MAGIC.ipynb
+-rw-r--r--   0        0        0     2387 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/WHY.ipynb
+-rw-r--r--   0        0        0     1175 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/_static/anvil.svg
+-rw-r--r--   0        0        0     1654 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/_static/css/custom.css
+-rw-r--r--   0        0        0     6452 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/_static/fonts/OCRA.woff2
+-rw-r--r--   0        0        0     9212 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/conf.py
+-rw-r--r--   0        0        0      881 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/index.ipynb
+-rw-r--r--   0        0        0    17571 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/docs/rtd.yml
+-rw-r--r--   0        0        0    17991 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/dodo.py
+-rw-r--r--   0        0        0      313 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/package.json
+-rw-r--r--   0        0        0     3008 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/pyproject.toml
+-rw-r--r--   0        0        0      391 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/__init__.py
+-rw-r--r--   0        0        0      131 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/_version.py
+-rw-r--r--   0        0        0      485 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/README.md
+-rw-r--r--   0        0        0      593 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/classic/Commands.resource
+-rw-r--r--   0        0        0     1140 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/classic/Notebook.resource
+-rw-r--r--   0        0        0     1946 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/classic/Output.resource
+-rw-r--r--   0        0        0     1708 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/classic/Selectors.resource
+-rw-r--r--   0        0        0     1735 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/classic/Tree.resource
+-rw-r--r--   0        0        0     2028 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Commands.resource
+-rw-r--r--   0        0        0     2068 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Icons.resource
+-rw-r--r--   0        0        0     1146 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Launcher.resource
+-rw-r--r--   0        0        0     2609 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Notebook.resource
+-rw-r--r--   0        0        0     2087 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Output.resource
+-rw-r--r--   0        0        0     2679 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/PageInfo.resource
+-rw-r--r--   0        0        0     3864 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Selectors.resource
+-rw-r--r--   0        0        0     3133 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Settings.resource
+-rw-r--r--   0        0        0     4412 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Shell.resource
+-rw-r--r--   0        0        0      705 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Shortcuts.resource
+-rw-r--r--   0        0        0      712 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Sidebar.resource
+-rw-r--r--   0        0        0     1219 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Version.resource
+-rw-r--r--   0        0        0      587 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/notebook/Commands.resource
+-rw-r--r--   0        0        0     1207 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/notebook/Notebook.resource
+-rw-r--r--   0        0        0     1891 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/notebook/Output.resource
+-rw-r--r--   0        0        0     2394 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/notebook/Selectors.resource
+-rw-r--r--   0        0        0     1974 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/notebook/Tree.resource
+-rw-r--r--   0        0        0     3556 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/common/CodeMirror.resource
+-rw-r--r--   0        0        0      450 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/common/Lumino.resource
+-rw-r--r--   0        0        0       94 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/constants.py
+-rw-r--r--   0        0        0     2586 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/core.py
+-rw-r--r--   0        0        0       75 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/keywords/__init__.py
+-rw-r--r--   0        0        0    13479 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/keywords/server.py
+-rw-r--r--   0        0        0     1224 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/keywords/webelements.py
+-rw-r--r--   0        0        0     6948 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/magic.py
+-rw-r--r--   0        0        0      342 2023-05-31 18:21:30.292637 robotframework_jupyterlibrary-0.5.0a0/yarn.lock
+-rw-r--r--   0        0        0     5824 1970-01-01 00:00:00.000000 robotframework_jupyterlibrary-0.5.0a0/PKG-INFO
```

### Comparing `robotframework-jupyterlibrary-0.4.2/LICENSE` & `robotframework_jupyterlibrary-0.5.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-jupyterlibrary-0.4.2/PKG-INFO` & `robotframework_jupyterlibrary-0.5.0a0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 Metadata-Version: 2.1
 Name: robotframework-jupyterlibrary
-Version: 0.4.2
-Summary: A Robot Framework library for automating (testing of) Jupyter end-user applications and extensions
-Home-page: https://github.com/robots-from-jupyter/robotframework-jupyterlibrary
-Author: Robots from Jupyter
-Author-email: nick.bollweg@gmail.com
-License: BSD-3-Clause
-Project-URL: Bug Tracker, https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/issues
-Project-URL: Changelog, https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/blob/master/docs/HISTORY.ipynb
-Project-URL: CI, https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/actions
-Project-URL: Documentation, https://robotframework-jupyterlibrary.readthedocs.io/en/stable
-Project-URL: Releases, https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/releases
-Project-URL: Source Code, https://github.com/robots-from-jupyter/robotframework-jupyterlibrary
+Version: 0.5.0a0
+Summary: A Robot Framework library for automating (testing of) Jupyter end-user applications and extensions.
 Keywords: Interactive,Jupyter,notebook,Testing,Web
+Author-email: JupyterLibrary contributors <robots-from-jupyter@googlegroups.com>
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab
-Classifier: Framework :: Jupyter :: JupyterLab :: 1
-Classifier: Framework :: Jupyter :: JupyterLab :: 2
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
+Classifier: Framework :: Jupyter :: JupyterLab :: 4
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
-Description-Content-Type: text/markdown
-License-File: LICENSE
+Requires-Dist: robotframework >=5
+Requires-Dist: robotframework-seleniumlibrary >=5
+Requires-Dist: robotframwork-tidy ; extra == "tidy"
+Requires-Dist: ipywidgets ; extra == "widgets"
+Project-URL: Bug Tracker, https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/issues
+Project-URL: CI, https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/actions
+Project-URL: Changelog, https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/blob/main/docs/HISTORY.ipynb
+Project-URL: Documentation, https://robotframework-jupyterlibrary.readthedocs.io/en/stable
+Project-URL: Releases, https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/releases
+Project-URL: Source Code, https://github.com/robots-from-jupyter/robotframework-jupyterlibrary
+Provides-Extra: tidy
+Provides-Extra: widgets
 
 # robotframework-jupyterlibrary
 
 > A [Robot Framework] library for automating (testing of) [Jupyter] end-user
 > applications and extensions
 
 [robot framework]: http://robotframework.org
@@ -92,34 +93,44 @@
 
 JupyterLibrary is Free Software under the [BSD-3-Clause License][license]. It contains
 code from a number of other projects:
 
 - [Jyve] ([BSD-3-Clause][jyve-license])
   - Initial implementations of robot keywords
 
+Some of its testing approaches (only distribtued in source form, not e.g. wheels) are
+also derived from other tools:
+
+- [ipyforcegraph][ipfg] ([BSD-3-Clause][ipfg-license])
+  - Initial implementation of [kernel-under-test coverage][kernel-cov] instrumentation
+
 [license]:
-  https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/blob/master/LICENSE
+  https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/blob/main/LICENSE
 [acceptance tests]:
-  https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/tree/master/atest
+  https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/tree/main/atest
 [miniforge]: https://github.com/conda-forge/miniforge/releases
 [binder-badge]: https://mybinder.org/badge_logo.svg
 [binder]:
-  https://mybinder.org/v2/gh/robots-from-jupyter/robotframework-jupyterlibrary/master?urlpath=lab/tree/docs/MAGIC.ipynb
+  https://mybinder.org/v2/gh/robots-from-jupyter/robotframework-jupyterlibrary/main?urlpath=lab/tree/docs/MAGIC.ipynb
 [workflow-badge]:
   https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/workflows/CI/badge.svg
 [workflow]:
-  https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/actions?query=workflow%3ACI+branch%3Amaster
+  https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/actions?query=workflow%3ACI+branch%3Amain
 [docs-badge]:
   https://readthedocs.org/projects/robotframework-jupyterlibrary/badge/?version=stable
 [pip-badge]: https://img.shields.io/pypi/v/robotframework-jupyterlibrary.svg
 [pip]: https://pypi.org/project/robotframework-jupyterlibrary
 [conda-forge]:
   https://github.com/conda-forge/robotframework-jupyterlibrary-feedstock#installing-robotframework-jupyterlibrary
 [conda-forge-badge]:
   https://img.shields.io/conda/vn/conda-forge/robotframework-jupyterlibrary.svg
 [docs]: https://robotframework-jupyterlibrary.readthedocs.io
+[ipfg]: https://github.com/jupyrdf/ipyforcegraph
+[ipfg-license]: https://github.com/jupyrdf/ipyforcegraph/blob/main/LICENSE.txt
 [jyve]: https://github.com/deathbeds/jyve
 [jyve-license]: https://github.com/deathbeds/jyve/blob/master/LICENSE
+[kernel-cov]: https://github.com/jupyrdf/ipyforcegraph/pull/89
 [magics]: https://robotframework-jupyterlibrary.readthedocs.io/en/stable/MAGIC.html
 [keywords]: https://robotframework-jupyterlibrary.readthedocs.io/en/stable/KEYWORDS.html
 [contributing]:
-  https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/blob/master/CONTRIBUTING.md
+  https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/blob/main/CONTRIBUTING.md
+
```

### Comparing `robotframework-jupyterlibrary-0.4.2/README.md` & `robotframework_jupyterlibrary-0.5.0a0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -57,34 +57,43 @@
 
 JupyterLibrary is Free Software under the [BSD-3-Clause License][license]. It contains
 code from a number of other projects:
 
 - [Jyve] ([BSD-3-Clause][jyve-license])
   - Initial implementations of robot keywords
 
+Some of its testing approaches (only distribtued in source form, not e.g. wheels) are
+also derived from other tools:
+
+- [ipyforcegraph][ipfg] ([BSD-3-Clause][ipfg-license])
+  - Initial implementation of [kernel-under-test coverage][kernel-cov] instrumentation
+
 [license]:
-  https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/blob/master/LICENSE
+  https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/blob/main/LICENSE
 [acceptance tests]:
-  https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/tree/master/atest
+  https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/tree/main/atest
 [miniforge]: https://github.com/conda-forge/miniforge/releases
 [binder-badge]: https://mybinder.org/badge_logo.svg
 [binder]:
-  https://mybinder.org/v2/gh/robots-from-jupyter/robotframework-jupyterlibrary/master?urlpath=lab/tree/docs/MAGIC.ipynb
+  https://mybinder.org/v2/gh/robots-from-jupyter/robotframework-jupyterlibrary/main?urlpath=lab/tree/docs/MAGIC.ipynb
 [workflow-badge]:
   https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/workflows/CI/badge.svg
 [workflow]:
-  https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/actions?query=workflow%3ACI+branch%3Amaster
+  https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/actions?query=workflow%3ACI+branch%3Amain
 [docs-badge]:
   https://readthedocs.org/projects/robotframework-jupyterlibrary/badge/?version=stable
 [pip-badge]: https://img.shields.io/pypi/v/robotframework-jupyterlibrary.svg
 [pip]: https://pypi.org/project/robotframework-jupyterlibrary
 [conda-forge]:
   https://github.com/conda-forge/robotframework-jupyterlibrary-feedstock#installing-robotframework-jupyterlibrary
 [conda-forge-badge]:
   https://img.shields.io/conda/vn/conda-forge/robotframework-jupyterlibrary.svg
 [docs]: https://robotframework-jupyterlibrary.readthedocs.io
+[ipfg]: https://github.com/jupyrdf/ipyforcegraph
+[ipfg-license]: https://github.com/jupyrdf/ipyforcegraph/blob/main/LICENSE.txt
 [jyve]: https://github.com/deathbeds/jyve
 [jyve-license]: https://github.com/deathbeds/jyve/blob/master/LICENSE
+[kernel-cov]: https://github.com/jupyrdf/ipyforcegraph/pull/89
 [magics]: https://robotframework-jupyterlibrary.readthedocs.io/en/stable/MAGIC.html
 [keywords]: https://robotframework-jupyterlibrary.readthedocs.io/en/stable/KEYWORDS.html
 [contributing]:
-  https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/blob/master/CONTRIBUTING.md
+  https://github.com/robots-from-jupyter/robotframework-jupyterlibrary/blob/main/CONTRIBUTING.md
```

### Comparing `robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/jupyterlab/Commands.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Commands.resource`

 * *Files 9% similar despite different names*

```diff
@@ -11,28 +11,28 @@
     ...    [https://jupyterlab.readthedocs.io/en/stable/user/commands.html|Command Palette]
     ...    to run a ``command`` and ``accept`` any resulting dialogs, then ``close``
     ...    the Command Palette.
     [Arguments]    ${command}    ${accept}=${True}    ${close}=${True}
     Maybe Accept A JupyterLab Prompt
     Open Command Palette With Hotkeys
     Input Text    css:${JLAB CSS CMD INPUT}    ${command}
-    Wait Until Page Contains Element    css:${JLAB CSS CMD ITEM}
+    Wait Until Element Is Visible    css:${JLAB CSS CMD ITEM}
     Click Element    css:${JLAB CSS CMD ITEM}
     Run Keyword If    ${accept}    Maybe Accept A JupyterLab Prompt
     Run Keyword If    ${close}    Maybe Close JupyterLab Sidebar
 
 Open Command Palette With Hotkeys
     [Documentation]
     ...    Open the JupyterLab Command Palette with the platform-specific keyboard
     ...    shortcuts. Note that the JupyterLab 3 modal command palette is flaky.
     ...    Enabling the sidebar-based mechanism may help, see:
     ...    - [#Set JupyterLab Plugin Settings|Set JupyterLab Plugin Settings]
     ${accel} =    Get ACCEL Key
     Press Keys    id:main    ${accel}+SHIFT+c
-    Wait Until Page Contains Element    css:${JLAB CSS CMD INPUT}
+    Wait Until Element Is Visible    css:${JLAB CSS CMD INPUT}
     Run Keyword And Ignore Error    Click Element    css:${JLAB CSS CMD INPUT}
 
 Reset JupyterLab And Close
     [Documentation]    Try to clean up after doing some things to the JupyterLab
     ...    open in the current browser, then close the browser.
     Execute JupyterLab Command    Reset Application State
     Close Browser
```

### Comparing `robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/jupyterlab/Icons.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Icons.resource`

 * *Files identical despite different names*

### Comparing `robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/jupyterlab/Launcher.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Launcher.resource`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 Launch A New JupyterLab Document
     [Documentation]    Use the JupyterLab launcher to launch a document of ``category``
     ...    Notebook or Console with the given ``kernel``, and wait until the loading
     ...    animation is complete.
     [Arguments]    ${kernel}=Python 3    ${category}=Notebook    ${timeout}=10s    ${sleep}=0.5s
     ${launcher} =    Get WebElements    xpath:${JLAB XP LAUNCHER}
     Run Keyword If    not ${launcher.__len__()}    Execute JupyterLab Command    New Launcher
-    Wait Until Page Contains Element    xpath:${JLAB XP CARD}    timeout=${timeout}
+    Wait Until Element Is Visible    xpath:${JLAB XP CARD}    timeout=${timeout}
     Click Element    xpath:${JLAB XP CARD}\[starts-with(@title, '${kernel}')][@data-category='${category}']
     Run Keyword And Ignore Error
-    ...    Wait Until Page Contains Element    css:${JLAB CSS SPINNER}
+    ...    Wait Until Element Is Visible    css:${JLAB CSS SPINNER}
     Run Keyword And Ignore Error
-    ...    Wait Until Page Does Not Contain Element    css:${JLAB CSS SPINNER}
+    ...    Wait Until Element Is Not Visible    css:${JLAB CSS SPINNER}
     Wait Until Page Contains Element    css:${JLAB CSS ACTIVE INPUT}
     Sleep    ${sleep}
```

### Comparing `robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/jupyterlab/Notebook.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Notebook.resource`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     [Documentation]    Add a ``code`` cell to the ``n`` th notebook on the page and run it.
     ...    ``code`` is a list of strings to set as lines in the code editor.
     ...    ``n`` is the 1-based index of the notebook, usually in order of opening.
     [Arguments]    @{code}    ${n}=1
     ${add icon} =    Get JupyterLab Icon XPath    add
     ${nb} =    Get WebElement    xpath://div${JLAB XP NB FRAG}\[${n}]
     # rely on main area widgets all having ids
-    ${nbid} =    Get Element Attribute    ${nb}    id
+    ${nbid} =    JupyterLibrary.Get Element Attribute    ${nb}    id
     ${icon} =    Get WebElement Relative To    ${nb}    xpath:div${JLAB XP NB TOOLBAR FRAG}//${add icon}
     Click Element    ${icon}
     Sleep    0.1s
     ${cell} =    Get WebElement Relative To    ${nb}
     ...    css:${JLAB CSS ACTIVE INPUT.replace('''${JLAB CSS ACTIVE DOC}''', '')}
     Click Element    ${cell}
     Set CodeMirror Value    \#${nbid}${JLAB CSS ACTIVE INPUT}    @{code}
```

### Comparing `robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/jupyterlab/Output.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Output.resource`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Resource            JupyterLibrary/clients/jupyterlab/Selectors.resource
 
 
 *** Keywords ***
 Current JupyterLab Cell Output Should Contain
     [Documentation]    Check the current active Notebook cell for the ``expected`` text.
     [Arguments]    ${expected}
-    Wait Until Page Contains Element    css:${JLAB CSS ACTIVE OUTPUT CHILDREN}
+    Wait Until Element Is Visible    css:${JLAB CSS ACTIVE OUTPUT CHILDREN}
     Element Should Contain    css:${JLAB CSS ACTIVE OUTPUT CHILDREN}    ${expected}
 
 Screenshot Each Output Of Active JupyterLab Cell
     [Documentation]    Capture all of the outputs of the current _Cell_ as screenshots
     ...    with a ``prefix`` (may include folders).
     [Arguments]    ${prefix}
     ${outputs} =    Get WebElements    css:${JLAB CSS ACTIVE OUTPUT CHILDREN} ${JLAB CSS OUTPUT} > *
```

### Comparing `robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/jupyterlab/PageInfo.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/PageInfo.resource`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     ${result} =    Set Variable If    ${key.__len__()}    ${pageInfo.get("${key}")}    ${pageInfo}
     [Return]    ${result}
 
 Update JupyterLab PageInfo Cache
     [Documentation]    Update the cached JupyterLab ``pageInfo``. _Not usually needed._
     ${sel} =    Set Variable    xpath://${JLAB XP PAGEINFO}
     Wait Until Page Contains Element    ${sel}
-    ${txt} =    Get Element Attribute    ${sel}    innerHTML
+    ${txt} =    JupyterLibrary.Get Element Attribute    ${sel}    innerHTML
     ${pageInfo} =    JSON.Loads    ${txt}
     Set Suite Variable    ${JLAB PAGEINFO CACHE}    ${pageInfo}    children=${True}
 
 Tag With JupyterLab Metadata
     [Documentation]    Tag the current test (or suite) with ``keys`` from the
     ...    JupyterLab ``pageInfo``.
     ...    The default ``keys``: ``appName`` ``appVersion`` ``buildAvailable``
@@ -49,8 +49,9 @@
 
 Get JupyterLab Application Version Info
     [Documentation]    Get the version of the application ``2.3.0.rc1`` as a list of
     ...    strings from ``pageInfo``, e.g. ``["2", "3", "1", "rc1"]``. Optionally ``clear``
     ...    the cached info first.
     [Arguments]    ${clear}=${False}
     ${version} =    Get JupyterLab Page Info    appVersion    clear=${clear}
-    [Return]    ${version.split(".")}
+    ${version_info} =    Set Variable    ${version.split(".")}
+    [Return]    ${version_info}
```

#### html2text {}

```diff
@@ -10,21 +10,21 @@
 {key}=${EMPTY} ${clear}=${False} ${pageInfo} = Get Variable Value ${JLAB
 PAGEINFO CACHE} ${EMPTY} Run Keyword If ${clear} or not ${pageInfo.__len__()}
 Update JupyterLab PageInfo Cache ${pageInfo} = Set Variable ${JLAB PAGEINFO
 CACHE} ${result} = Set Variable If ${key.__len__()} ${pageInfo.get("${key}")} $
 {pageInfo} [Return] ${result} Update JupyterLab PageInfo Cache [Documentation]
 Update the cached JupyterLab ``pageInfo``. _Not usually needed._ ${sel} = Set
 Variable xpath://${JLAB XP PAGEINFO} Wait Until Page Contains Element ${sel} $
-{txt} = Get Element Attribute ${sel} innerHTML ${pageInfo} = JSON.Loads ${txt}
-Set Suite Variable ${JLAB PAGEINFO CACHE} ${pageInfo} children=${True} Tag With
-JupyterLab Metadata [Documentation] Tag the current test (or suite) with
-``keys`` from the ... JupyterLab ``pageInfo``. ... The default ``keys``:
-``appName`` ``appVersion`` ``buildAvailable`` ... ``buildCheck``
-``notebookVersion`` ``devMode`` [Arguments] ${keys}=${JLAB DEFAULT PAGEINFO
-TAGS} ${clear}=${False} ${info} = Get JupyterLab Page Info clear=${clear} FOR $
-{key} IN @{keys} ${val} = Set Variable ${info.get("${key}")} Set Tags
-jupyterlab:${key}:${val} END Get JupyterLab Application Version Info
-[Documentation] Get the version of the application ``2.3.0.rc1`` as a list of
-... strings from ``pageInfo``, e.g. ``["2", "3", "1", "rc1"]``. Optionally
-``clear`` ... the cached info first. [Arguments] ${clear}=${False} ${version} =
-Get JupyterLab Page Info appVersion clear=${clear} [Return] ${version.split
-(".")}
+{txt} = JupyterLibrary.Get Element Attribute ${sel} innerHTML ${pageInfo} =
+JSON.Loads ${txt} Set Suite Variable ${JLAB PAGEINFO CACHE} ${pageInfo}
+children=${True} Tag With JupyterLab Metadata [Documentation] Tag the current
+test (or suite) with ``keys`` from the ... JupyterLab ``pageInfo``. ... The
+default ``keys``: ``appName`` ``appVersion`` ``buildAvailable`` ...
+``buildCheck`` ``notebookVersion`` ``devMode`` [Arguments] ${keys}=${JLAB
+DEFAULT PAGEINFO TAGS} ${clear}=${False} ${info} = Get JupyterLab Page Info
+clear=${clear} FOR ${key} IN @{keys} ${val} = Set Variable ${info.get("$
+{key}")} Set Tags jupyterlab:${key}:${val} END Get JupyterLab Application
+Version Info [Documentation] Get the version of the application ``2.3.0.rc1``
+as a list of ... strings from ``pageInfo``, e.g. ``["2", "3", "1", "rc1"]``.
+Optionally ``clear`` ... the cached info first. [Arguments] ${clear}=${False} $
+{version} = Get JupyterLab Page Info appVersion clear=${clear} ${version_info}
+= Set Variable ${version.split(".")} [Return] ${version_info}
```

### Comparing `robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/jupyterlab/Selectors.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Selectors.resource`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,71 @@
 *** Settings ***
 Documentation       Common selectors for JupyterLab elements
 
+Resource            JupyterLibrary/common/CodeMirror.resource
+Resource            JupyterLibrary/common/Lumino.resource
+
 
 *** Variables ***
 # robocop: disable=line-too-long
-# css selectors
-${JLAB CSS ACCEPT}                      .jp-mod-accept
-${JLAB CSS ACTIVE DOC}                  .jp-Document:not(.jp-mod-hidden)
-${JLAB CSS ACTIVE DOC CELLS}            ${JLAB CSS ACTIVE DOC} .jp-Cell
-${JLAB CSS ACTIVE CELL}                 ${JLAB CSS ACTIVE DOC} .jp-Cell.jp-mod-active
-${JLAB CSS ACTIVE INPUT}                ${JLAB CSS ACTIVE CELL} .CodeMirror
-${JLAB CSS ACTIVE OUTPUT CHILDREN}      ${JLAB CSS ACTIVE CELL} .jp-OutputArea-child
+# top-level mod utility classes
+${JLAB CSS MOD ACTIVE}                  .jp-mod-active
+${JLAB CSS MOD ACCEPT}                  .jp-mod-accept
+${JLAB CSS MOD HIDDEN}                  .jp-mod-hidden
+
+# deprecated
+${JLAB CSS ACCEPT}                      ${JLAB CSS MOD ACCEPT}    # deprecated
+
+# css atom element selectors
+${JLAB CSS CELL}                        .jp-Cell
+${JLAB CSS OUTPUT MARKDOWN}             .jp-MarkdownOutput
+
+# app and utility
+${JLAB CSS DOC}                         .jp-Document
+${JLAB CSS SIDEBAR}                     .jp-SideBar
+${JLAB CSS SPINNER}                     .jp-Spinner
+
+# component selectors
+${JLAB CSS NB TOOLBAR}                  .jp-NotebookPanel-toolbar
 ${JLAB CSS OUTPUT}                      .jp-OutputArea-output
-${JLAB CSS ACTIVE CELL MARKDOWN}        ${JLAB CSS ACTIVE CELL} .jp-MarkdownOutput:not(.jp-mod-hidden)
-${JLAB CSS ACTIVE SIDEBAR}              .jp-SideBar .p-TabBar-tab.p-mod-current
+${JLAB CSS OUTPUT CHILD}                .jp-OutputArea-child
+
+# compounds
+${JLAB CSS ACTIVE DOC}                  ${JLAB CSS DOC}:not(${JLAB CSS MOD HIDDEN})
+${JLAB CSS ACTIVE DOC CELLS}            ${JLAB CSS ACTIVE DOC} ${JLAB CSS CELL}
+${JLAB CSS ACTIVE CELL}                 ${JLAB CSS ACTIVE DOC} ${JLAB CSS CELL}${JLAB CSS MOD ACTIVE}
+${JLAB CSS ACTIVE OUTPUT CHILDREN}      ${JLAB CSS ACTIVE CELL} ${JLAB CSS OUTPUT CHILD}
+${JLAB CSS ACTIVE CELL MARKDOWN}        ${JLAB CSS ACTIVE CELL} ${JLAB CSS OUTPUT MARKDOWN}:not(${JLAB CSS MOD HIDDEN})
+${JLAB CSS ACTIVE SIDEBAR}              ${JLAB CSS SIDEBAR} ${LM CSS TAB}${LM CSS MOD CURRENT}
 ${JLAB CSS BUSY KERNEL}                 .jp-Toolbar-kernelStatus.jp-FilledCircleIcon
-${JLAB CSS CMD INPUT}                   .p-CommandPalette-input
-${JLAB CSS CMD ITEM}                    .p-CommandPalette-item
-${JLAB CSS NB TOOLBAR}                  .jp-NotebookPanel-toolbar
-${JLAB CSS SIDEBAR TAB}                 .jp-SideBar .p-TabBar-tab
-${JLAB CSS SPINNER}                     .jp-Spinner
+${JLAB CSS CMD INPUT}                   ${LM CSS CMD INPUT}
+${JLAB CSS CMD ITEM}                    ${LM CSS CMD ITEM}
+${JLAB CSS SIDEBAR TAB}                 ${JLAB CSS SIDEBAR} ${LM CSS TAB}
+
+# overloaded by version
+${JLAB CSS ACTIVE INPUT}                ${JLAB CSS ACTIVE CELL} .CodeMirror
+
 # magic ids
 ${JLAB ID SPLASH}                       jupyterlab-splash
 # magic strings
 ${JLAB TEXT BUSY PROMPT}                In [*]:
 # xpath selectors
 ${JLAB XP LAUNCHER}                     //div[contains(@class, 'jp-Launcher-body')]
 ${JLAB XP CARD}                         //div[contains(@class, 'jp-LauncherCard')]
 ${JLAB XP DOCK}                         //div[@id='jp-main-dock-panel']
-${JLAB XP MENU ITEM}                    //li[contains(@class, 'p-Menu-item')]
-${JLAB XP MENU ITEM LABEL}              //div[contains(@class, 'p-Menu-itemLabel')]
-${JLAB XP MENU ITEM VISIBLE}            ${JLAB XP MENU ITEM}\[not(contains(@class,'p-mod-hidden'))]
-${JLAB XP MENU ITEM LABEL VISIBLE}      ${JLAB XP MENU ITEM VISIBLE}/div[contains(@class, 'p-Menu-itemLabel')]
-${JLAB XP MENU LABEL}                   //div[contains(@class, 'p-MenuBar-itemLabel')]
+${JLAB XP MENU ITEM}                    //li[contains(@class, 'lm-Menu-item')]
+${JLAB XP MENU ITEM LABEL}              //div[contains(@class, 'lm-Menu-itemLabel')]
+${JLAB XP MENU ITEM VISIBLE}            ${JLAB XP MENU ITEM}\[not(contains(@class,'lm-mod-hidden'))]
+${JLAB XP MENU ITEM LABEL VISIBLE}      ${JLAB XP MENU ITEM VISIBLE}/div[contains(@class, 'lm-Menu-itemLabel')]
+${JLAB XP MENU LABEL}                   //div[contains(@class, 'lm-MenuBar-itemLabel')]
 ${JLAB XP TOP}                          //div[@id='jp-top-panel']
 ${JLAB XP MAIN AREA FRAG}               [contains(@class, 'jp-MainAreaWidget')]
 ${JLAB XP NB FRAG}                      ${JLAB XP MAIN AREA FRAG}\[contains(@class, 'jp-NotebookPanel')]
 ${JLAB XP NB TOOLBAR FRAG}              [contains(@class, 'jp-NotebookPanel-toolbar')]
 ${JLAB XP NB TOOLBAR}                   //div${JLAB XP NB TOOLBAR FRAG}
 ${JLAB XP BUSY KERNEL}
 ...                                     //*[local-name() = 'div' and contains(@class, 'jp-FilledCircleIcon' or (local-name() = 'svg' and contains(@data-icon, 'ui-components:circle-filled')))]
 # dock panel
 ${JLAB XP DOCK PANEL}                   //*[@id = 'jp-main-dock-panel']
 ${JLAB XP DOCK TAB}
-...                                     ${JLAB XP DOCK PANEL}//ul[contains(@class, 'p-TabBar-content')]/li[contains(@class, 'p-TabBar-tab')]
-${JLAB XP DOCK TAB LABEL}               ${JLAB XP DOCK TAB}/div[contains(@class, 'p-TabBar-tabLabel')]
+...                                     ${JLAB XP DOCK PANEL}//ul[contains(@class, 'lm-TabBar-content')]/li[contains(@class, 'lm-TabBar-tab')]
+${JLAB XP DOCK TAB LABEL}               ${JLAB XP DOCK TAB}/div[contains(@class, 'lm-TabBar-tabLabel')]
```

### Comparing `robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/jupyterlab/Settings.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Settings.resource`

 * *Files identical despite different names*

### Comparing `robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/jupyterlab/Shell.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Shell.resource`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 *** Settings ***
 Documentation       Application shell keywords for JupyterLab
 
 Resource            JupyterLibrary/clients/jupyterlab/Selectors.resource
 Resource            JupyterLibrary/clients/jupyterlab/PageInfo.resource
+Resource            JupyterLibrary/clients/jupyterlab/Version.resource
 
 
 *** Keywords ***
 # robocop: disable=too-many-arguments
 
 Open JupyterLab
     [Documentation]    Open JupyterLab, served from the given (or most-recently-started)
@@ -21,44 +22,47 @@
     ...    &{configuration}
     ${nbserver_url} =    Run Keyword If    not "${url}"    Get Jupyter Server URL    ${nbserver}
     ${token} =    Run Keyword If    not "${url}"    Get Jupyter Server Token    ${nbserver}
     ${final_url} =    Set Variable If    "${url}"    ${url}    ${nbserver_url}lab?token=${token}
     Open Browser    url=${final_url}    browser=${browser}    &{configuration}
     Maybe Wait For JupyterLab Splash Screen
     Tag With JupyterLab Metadata    ${pageinfo tags}    clear=${clear}
+    LOG    ${JLAB CSS ACTIVE INPUT}
+    Update Globals For JupyterLab Version
+    LOG    ${JLAB CSS ACTIVE INPUT}
 
 Wait For JupyterLab Splash Screen
     [Documentation]    Wait for the JupyterLab splash animation, waiting ``timeout``
     ...    for the splash screen to appear/disappear, then ``sleep``.
     [Arguments]    ${timeout}=10s    ${sleep}=2s
-    Wait Until Page Contains Element    css:#${JLAB ID SPLASH}    timeout=${timeout}
+    Wait Until Element Is Visible    css:#${JLAB ID SPLASH}    timeout=${timeout}
     Wait Until Page Does Not Contain Element    css:#${JLAB ID SPLASH}    timeout=${timeout}
     Sleep    ${sleep}
 
 Maybe Wait For JupyterLab Splash Screen
     [Documentation]    Wait for the JupyterLab splash animation, waiting ``timeout``
     ...    for the splash screen to appear/disappear, then ``sleep``. Ignore errors.
     [Arguments]    ${timeout}=10s    ${sleep}=2s
     Run Keyword And Ignore Error    Wait For JupyterLab Splash Screen    ${timeout}    ${sleep}
 
 Click JupyterLab Menu
     [Documentation]    Click a top-level JupyterLab menu bar item by ``label``,
     ...    e.g. _File_, _Help_, etc.
     [Arguments]    ${label}
     ${xpath} =    Set Variable    ${JLAB XP TOP}${JLAB XP MENU LABEL}\[text() = '${label}']
-    Wait Until Page Contains Element    ${xpath}
+    Wait Until Element Is Visible    ${xpath}
     Mouse Over    ${xpath}
     Click Element    ${xpath}
     Run Keyword And Ignore Error    Mouse Over    ${xpath}
 
 Click JupyterLab Menu Item
     [Documentation]    Click a currently-visible JupyterLab menu item by ``label``.
     [Arguments]    ${label}
     ${item} =    Set Variable    ${JLAB XP MENU ITEM LABEL VISIBLE}\[text() = '${label}']
-    Wait Until Page Contains Element    ${item}
+    Wait Until Element Is Visible    ${item}
     Mouse Over    ${item}
     Click Element    ${item}
     Run Keyword And Ignore Error    Mouse Over    ${item}
 
 Open With JupyterLab Menu
     [Documentation]    Click into a ``menu``, then a series of ``submenus``.
     [Arguments]    ${menu}    @{submenus}
```

### Comparing `robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/jupyterlab/Shortcuts.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Shortcuts.resource`

 * *Files identical despite different names*

### Comparing `robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/jupyterlab/Sidebar.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/jupyterlab/Sidebar.resource`

 * *Files identical despite different names*

### Comparing `robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/notebook/Commands.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/classic/Commands.resource`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 *** Settings ***
 Documentation       Command keywords for Jupyter Classic
 
-Resource            JupyterLibrary/clients/notebook/Selectors.resource
+Resource            JupyterLibrary/clients/classic/Selectors.resource
 
 
 *** Keywords ***
 Execute Notebook Classic Command
     [Documentation]    Use the Notebook Classic Command Pop-up
     ...    to run a command and ``accept`` any resulting dialogs, then ``close``
     ...    the Command Palette.
```

### Comparing `robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/notebook/Notebook.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/classic/Notebook.resource`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 *** Settings ***
 Documentation       Notebook keywords for Jupyter Classic
 
-Resource            JupyterLibrary/clients/notebook/Selectors.resource
+Resource            JupyterLibrary/clients/classic/Selectors.resource
 Resource            JupyterLibrary/common/CodeMirror.resource
 
 
 *** Keywords ***
 Add And Run Notebook Classic Code Cell
     [Documentation]    Add a ``code`` cell to the currently active notebook and run it.
     [Arguments]    ${code}=print("hello world")
```

### Comparing `robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/notebook/Output.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/classic/Output.resource`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 *** Settings ***
 Documentation       Keywords for outputs in Jupyter Classic
 
-Resource            JupyterLibrary/clients/notebook/Selectors.resource
+Resource            JupyterLibrary/clients/classic/Selectors.resource
 
 
 *** Keywords ***
 Current Notebook Classic Cell Output Should Contain
     [Documentation]    Check whether the currently-selected cell's output contains the given text
     [Arguments]    ${expected}
     Wait Until Element Contains    css:${JNC CSS ACTIVE OUTPUT}    ${expected}
```

### Comparing `robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/notebook/Selectors.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/classic/Selectors.resource`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 *** Variables ***
 ${JNC CSS TREE LIST}                    \#notebook_list
 ${JNC CSS TREE LIST ITEM}               ${JNC CSS TREE LIST} .list_item
 ${JNC CSS TREE NEW BUTTON}              \#new-dropdown-button
 ${JNC CSS TREE NEW MENU}                \#new-menu
 ${JNC CSS NB KERNEL ICON}               \#kernel_indicator_icon
 ${JNC CSS NB KERNEL IDLE}               .kernel_idle_icon
-${JNC CSS NB KERNEL BUSY}               .kernel_budy_icon
+${JNC CSS NB KERNEL BUSY}               .kernel_busy_icon
 ${JNC TEXT BUSY PROMPT}                 In [*]:
 ${JNC CSS CMD BUTTON}                   button[data-jupyter-action="jupyter-notebook:show-command-palette"]
 ${JNC CSS CMD PALETTE}                  .modal.cmd-palette.in
 ${JNC CSS CMD INPUT}                    ${JNC CSS CMD PALETTE}    input[type="search"]
 ${JNC CSS CMD ITEM}                     ${JNC CSS CMD PALETTE}    .typeahead-result li > a
 ${JNC CSS NB TOOLBAR}                   \#maintoolbar-container
 ${JNC CSS ICON ADD}                     .fa-plus
```

### Comparing `robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/clients/notebook/Tree.resource` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/clients/classic/Tree.resource`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 *** Settings ***
 Documentation       Keywords for working with the Jupyter Notebook Clasic web application
 ...                 You should have already started a Jupyter Server, such as with
 ...                 *Wait For New Jupyter Server To Be Ready*.
 
-Resource            JupyterLibrary/clients/notebook/Selectors.resource
+Resource            JupyterLibrary/clients/classic/Selectors.resource
 
 
 *** Keywords ***
 Open Notebook Classic
     [Documentation]    Open Jupyter Notebook Classic, served from the given (or most-recently-started)
     ...    ``nbserver`` in a ``browser`` (or ``headlessfirefox``) or ``url``,
     ...    then wait for the splash screen.
     ...    Extra ``configuration`` is passed on to SeleniumLibrary's *Open Browser*.
     [Arguments]    ${browser}=headlessfirefox    ${nbserver}=${None}    ${url}=${EMPTY}    &{configuration}
     ${nbserver_url} =    Run Keyword If    not "${url}"    Get Jupyter Server URL    ${nbserver}
     ${token} =    Run Keyword If    not "${url}"    Get Jupyter Server Token    ${nbserver}
     ${final_url} =    Set Variable If    "${url}"    ${url}    ${nbserver_url}tree?token=${token}
     Open Browser    url=${final_url}    browser=${browser}    &{configuration}
-    Wait Until Page Contains Element    css:${JNC CSS TREE LIST ITEM}
+    Wait Until Element Is Visible    css:${JNC CSS TREE LIST ITEM}
 
 Launch A New Notebook Classic Notebook
     [Documentation]    Use the Jupyter Notebook Classic tree to launch a
     ...    Notebook with the given ``kernel``
     [Arguments]    ${kernel}=Python 3
     Click Element    css:${JNC CSS TREE NEW BUTTON}
-    Wait Until Page Contains Element    css:${JNC CSS TREE NEW MENU}
+    Wait Until Element Is Visible    css:${JNC CSS TREE NEW MENU}
     Click Element    css:${JNC CSS TREE NEW MENU} a[title*="${kernel}"]
     Switch Window    NEW
-    Wait Until Page Contains Element    css:${JNC CSS NB KERNEL ICON}${JNC CSS NB KERNEL IDLE}    timeout=30s
+    Wait Until Element Is Visible    css:${JNC CSS NB KERNEL ICON}${JNC CSS NB KERNEL IDLE}    timeout=30s
```

### Comparing `robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/core.py` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-""" Core library entrypoint for JupyterLibrary
-
-    We <3 Python3, but for the time being, this module should also run in Python2
-"""
-from glob import glob
-from os.path import basename, dirname, isdir, join
+"""Core library entrypoint for JupyterLibrary."""
+from pathlib import Path
 
 from robot.libraries.BuiltIn import BuiltIn
 from SeleniumLibrary import SeleniumLibrary
 from SeleniumLibrary.utils.librarylistener import LibraryListener
 
 from .keywords import server, webelements
 
+HERE = Path(__file__).parent
 
-CLIENTS = [
-    client for client in glob(join(dirname(__file__), "clients", "*")) if isdir(client)
-]
+CLIENTS = [client for client in sorted(HERE.glob("clients/*")) if client.is_dir()]
 
-COMMON = list(glob(join(dirname(__file__), "common", "*.resource")))
+COMMON = sorted(HERE.glob("common/*.resource"))
 
 component_classes = [
     webelements.WebElementKeywords,
     server.ServerKeywords,
 ]
 
 
+class JupyterLibraryListener(LibraryListener):
+
+    """Custom listener to do per-suite imports of resource files."""
+
+    ROBOT_LISTENER_API_VERSION = 2
+
+    def start_suite(self, name, attrs):
+        """Handle dynamic imports at suite startup."""
+        super().start_suite(name, attrs)
+        resources = []
+
+        for common in COMMON:
+            resources += [f"JupyterLibrary/common/{common.name}"]
+
+        for client in CLIENTS:
+            for path in sorted(client.rglob("*.resource")):
+                resources += [
+                    f"JupyterLibrary/{path.relative_to(HERE).as_posix()}",
+                ]
+
+        for resource in resources:
+            BuiltIn().import_resource(resource)
+
+
 class JupyterLibrary(SeleniumLibrary):
+
     """JupyterLibrary is a Jupyter testing library for Robot Framework."""
 
     def __init__(
         self,
         timeout=5.0,
         implicit_wait=0.0,
         run_on_failure="Capture Page Screenshot",
         screenshot_root_directory=None,
         **kwargs,
-    ):
-        """JupyterLibrary can be imported with several optional arguments.
+    ) -> None:
+        """Instantiate a stateful ``JupyterLibrary`` instance.
+
+        JupyterLibrary can be imported with several optional arguments.
         - ``timeout``:
           Default value for `timeouts` used with ``Wait ...`` keywords.
         - ``implicit_wait``:
           Default value for `implicit wait` used when locating elements.
         - ``run_on_failure``:
           Default action for the `run-on-failure functionality`.
         - ``screenshot_root_directory``:
           Location where possible screenshots are created. If not given,
           the directory where the log file is written is used.
         """
-        super(JupyterLibrary, self).__init__(
+        super().__init__(
             timeout=timeout,
             implicit_wait=implicit_wait,
             run_on_failure=run_on_failure,
             screenshot_root_directory=screenshot_root_directory,
             **kwargs,
         )
         self.add_library_components(
-            [Component(self) for Component in component_classes]
+            [Component(self) for Component in component_classes],
         )
         self.ROBOT_LIBRARY_LISTENER = JupyterLibraryListener()
-
-
-class JupyterLibraryListener(LibraryListener):
-    """Custom listener to do per-suite imports of resource files"""
-
-    ROBOT_LISTENER_API_VERSION = 2
-
-    def start_suite(self, name, attrs):
-        super(JupyterLibraryListener, self).start_suite(name, attrs)
-        resources = []
-
-        for common in COMMON:
-            resources += [f"JupyterLibrary/common/{basename(common)}"]
-
-        for client in CLIENTS:
-            for path in glob(join(client, "*.resource")):
-                resources += [
-                    f"JupyterLibrary/clients/{basename(client)}/{basename(path)}"
-                ]
-
-        for resource in resources:
-            BuiltIn().import_resource(resource)
```

### Comparing `robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/keywords/server.py` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/keywords/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,42 @@
+"""A library component for managing Jupyter servers."""
 import os
 import shutil
 import socket
+import subprocess
 import tempfile
-import typing
 import time
-import subprocess
-from os.path import join
+import typing
+from pathlib import Path
+from urllib.request import urlopen
 from uuid import uuid4
 
 from robot.libraries.BuiltIn import BuiltIn
 from SeleniumLibrary.base import LibraryComponent, keyword
-from urllib.request import urlopen
 
 
 class ServerKeywords(LibraryComponent):
-    _handles = []
-    _tmpdirs = {}
-    _notebook_dirs = {}
-    _ports = {}
-    _base_urls = {}
-    _tokens = {}
 
-    _app_name = None
+    """A component that extends the core with Jupyter server management."""
+
+    _handles: typing.List[subprocess.Popen] = []
+    _tmpdirs: typing.Dict[subprocess.Popen, str] = {}
+    _notebook_dirs: typing.Dict[subprocess.Popen, str] = {}
+    _ports: typing.Dict[subprocess.Popen, int] = {}
+    _base_urls: typing.Dict[subprocess.Popen, str] = {}
+    _tokens: typing.Dict[subprocess.Popen, str] = {}
+
+    _app_name: typing.Optional[str] = None
 
     @keyword
     def set_default_jupyter_app_name(
-        self, app_name: typing.Optional[str] = None
+        self,
+        app_name: typing.Optional[str] = None,
     ) -> typing.Optional[str]:
-        """Set the current ``traitlets.Configurable`` Jupyter Server application,
-        returning the previous value.
+        """Set the current ``traitlets.Configurable`` Jupyter Server application, returning the previous value.
 
         A value of ``None`` (the default) will try to detect the app based on
         command name, such as:
 
         - ``jupyter-notebook`` is configured with ``NotebookApp``
         - ``jupyter-lab`` and most other are configured with ``ServerApp``
 
@@ -43,18 +47,18 @@
         """
         old_app_name = self.app_name
         self.app_name = app_name
         return old_app_name
 
     @keyword
     def get_jupyter_app_name(
-        self, command: typing.Optional[str] = None
+        self,
+        command: typing.Optional[str] = None,
     ) -> typing.Optional[str]:
-        """Get the current ``traitlets.Configurable`` Jupyter Server application,
-        optionally for a specific CLI command.
+        """Get the current ``traitlets.Configurable`` Jupyter Server application, optionally for a specific CLI command.
 
         See [#Set Default Jupyter App Name] for more.
         """
         app_name = os.environ.get("JUPYTER_LIBRARY_APP")
 
         if self._app_name is not None:
             app_name = self._app_name
@@ -72,144 +76,158 @@
         notebook_dir: typing.Optional[str] = None,
         token: typing.Optional[str] = None,
         *args,
         **config,
     ) -> subprocess.Popen:
         """Start a Jupyter server. All arguments are optional.
 
-        | = argument =     | = default =           | = notes =                          |
-        | ``command``      | ``jupyter-notebook``  | e.g. ``jupyter-lab``               |
-        | ``port``         | an unused port        |                                    |
-        | ``base_url``     | ``/@rf/``             |                                    |
-        | ``notebook_dir`` | a temporary directory |                                    |
-        | ``token``        | a random ``uuid4``    |                                    |
-        | ``*args``        |                       | extra server arguments             |
-        | ``**config``     |                       | extra process arguments            |
-        | ``app_name``     | ``None`` (detect)     | e.g. ``NotebookApp``, `ServerApp`` |
+        | = argument =     | = default =           | = notes =                               |
+        | ``command``      | ``jupyter-notebook``  | e.g. ``jupyter-lab``                    |
+        | ``port``         | an unused port        |                                         |
+        | ``base_url``     | ``/@rf/``             |                                         |
+        | ``notebook_dir`` | a temporary directory |                                         |
+        | ``token``        | a random ``uuid4``    |                                         |
+        | ``*args``        |                       | extra server arguments                  |
+        | ``**config``     |                       | extra process arguments                 |
+        | ``app_name``     | ``None`` (detect)     | e.g. ``NotebookApp``, `ServerApp``      |
+        | ``extra_args``   | ``[]``                | extra arguments beyond ```token``, etc. |
 
         If not configured, the ``%{HOME}`` environment variable and current
         working directory will be set to avoid leaking configuration
         between between runs (or the test instance) itself. These
         directories will be cleaned up after the server process is
         [#Terminate All Jupyter Servers|terminated].
 
         The ``app_name`` argument is as described for the [#Get Jupyter App Name|app name],
         with the default being to autodetect from the command and environment.
+
+        ``extra_args`` are passed to ``Start Process`` before the ``token``
         """
         app_name = (
             config.pop("app_name", None)
             or config.get("env:JUPYTER_LIBRARY_APP")
             or self.get_jupyter_app_name(command)
         )
         port = port or self.get_unused_port()
         token = str(uuid4()) if token is None else token
 
         BuiltIn().import_library("Process")
         plib = BuiltIn().get_library_instance("Process")
 
-        tmpdir = tempfile.mkdtemp()
+        tmp_path = Path(tempfile.mkdtemp())
 
         if "env:HOME" not in config:
-            home_dir = join(tmpdir, "home")
-            os.mkdir(home_dir)
-            config["env:HOME"] = home_dir
+            home_dir = tmp_path / "home"
+            home_dir.mkdir()
+            config["env:HOME"] = str(home_dir)
 
         if "stdout" not in config:
-            config["stdout"] = join(tmpdir, "server.log")
+            config["stdout"] = str(tmp_path / "server.log")
 
         if "stderr" not in config:
             config["stderr"] = "STDOUT"
 
         if notebook_dir is None:
-            notebook_dir = join(tmpdir, "notebooks")
-            os.mkdir(notebook_dir)
-            config["cwd"] = notebook_dir
+            notebook_dir = tmp_path / "notebooks"
+            notebook_dir.mkdir()
+            config["cwd"] = str(notebook_dir)
 
         args = args or self.build_jupyter_server_arguments(
-            port, base_url, token, app_name
+            port,
+            base_url,
+            token,
+            app_name,
         )
 
-        handle = plib.start_process(command, *args, **config)
+        extra_args = config.pop("extra_args", [])
+
+        handle = plib.start_process(command, *extra_args, *args, **config)
 
         self._handles += [handle]
-        self._tmpdirs[handle] = tmpdir
-        self._notebook_dirs[handle] = notebook_dir
+        self._tmpdirs[handle] = str(tmp_path)
+        self._notebook_dirs[handle] = str(notebook_dir)
         self._ports[handle] = port
         self._base_urls[handle] = base_url
         self._tokens[handle] = token
 
         return handle
 
     @keyword
     def build_jupyter_server_arguments(
         self,
         port: int,
         base_url: str,
         token: str,
         app_name: typing.Optional[str] = None,
-    ) -> typing.List[str]:
+    ) -> typing.Tuple[str]:
         """Build Some default Jupyter application arguments.
 
         If the ``app_name`` is not provided, it will be detected based on the rules
-        in [#Get Jupyter App Name]."""
+        in [#Get Jupyter App Name].
+        """
         app_name = app_name or self.get_jupyter_app_name()
-        return [
+        return (
             "--no-browser",
             "--debug",
             f"--port={port}",
             f"--{app_name}.token={token}",
             f"--{app_name}.base_url={base_url}",
-        ]
+        )
 
     @keyword
     def copy_files_to_jupyter_directory(self, *sources: str, **kwargs) -> None:
         """Copy some files into the (temporary) jupyter server root.
 
         | = argument = | = default =                       |
         | ``nbserver`` | the most-recently launched server |
         """
         nbserver = kwargs.get("nbserver", self._handles[-1])
         notebook_dir = self._notebook_dirs[nbserver]
         BuiltIn().import_library("OperatingSystem")
         osli = BuiltIn().get_library_instance("OperatingSystem")
-        return osli.copy_files(*(list(sources) + [notebook_dir]))
+        return osli.copy_files(*sorted(sources), notebook_dir)
 
     @keyword
     def copy_files_from_jupyter_directory(self, *src_and_dest: str, **kwargs) -> None:
-        """Copy some files from the (temporary) jupyter server root
+        """Copy some files from the (temporary) jupyter server root.
 
         | = argument = | = default =                       |
         | ``nbserver`` | the most-recently launched server |
 
         Patterns will have the notebook directory prepended
         """
         nbserver = kwargs.get("nbserver", self._handles[-1])
-        notebook_dir = self._notebook_dirs[nbserver]
+        notebook_dir = Path(self._notebook_dirs[nbserver])
         BuiltIn().import_library("OperatingSystem")
         osli = BuiltIn().get_library_instance("OperatingSystem")
-        sources = [join(notebook_dir, src) for src in src_and_dest[:-1]]
+        sources = [str(notebook_dir / src) for src in src_and_dest[:-1]]
         dest = src_and_dest[-1]
-        return osli.copy_files(*sources + [dest])
+        return osli.copy_files(*sources, dest)
 
     @keyword
     def get_jupyter_directory(
-        self, nbserver: typing.Optional[subprocess.Popen] = None
+        self,
+        nbserver: typing.Optional[subprocess.Popen] = None,
     ) -> str:
-        """
+        """Get the Jupyter contents directory.
+
         | = argument = | = default =                       |
         | ``nbserver`` | the most-recently launched server |
         """
         nbserver = nbserver if nbserver is not None else self._handles[-1]
+
         return self._notebook_dirs[nbserver]
 
     @keyword
     def wait_for_jupyter_server_to_be_ready(
-        self, *nbservers: subprocess.Popen, **kwargs
+        self,
+        *nbservers: subprocess.Popen,
+        **kwargs,
     ) -> int:
-        """Wait for the most-recently started Jupyter server to be ready"""
+        """Wait for the most-recently started Jupyter server to be ready."""
         interval = float(kwargs.get("interval", 0.5))
         retries = int(kwargs.get("retries", 60))
 
         if not nbservers:
             if not self._handles:
                 return 0
             nbservers = [self._handles[-1]]
@@ -224,99 +242,145 @@
                 for nbh in nbservers:
                     urlopen(self.get_jupyter_server_url(nbh))
                     ready += 1
             except Exception as _error:
                 time.sleep(interval)
                 error = _error
 
-        assert ready == len(nbservers), (
-            f"Only {ready} of {len(nbservers)} servers were ready after "
-            f"{interval * retries}s. Last error: {type(error)} {error}"
-        )
+        if ready != len(nbservers):
+            message = (
+                f"Only {ready} of {len(nbservers)} servers were ready after "
+                f"{interval * retries}s. Last error: {type(error)} {error}"
+            )
+            raise RuntimeError(message)
         return ready
 
     @keyword
     def get_jupyter_server_url(
-        self, nbserver: typing.Optional[subprocess.Popen] = None
+        self,
+        nbserver: typing.Optional[subprocess.Popen] = None,
     ) -> str:
-        """Get the given (or most recently-launched) server's URL"""
+        """Get the given (or most recently-launched) server's URL."""
         nbh = nbserver or self._handles[-1]
         return f"http://127.0.0.1:{self._ports[nbh]}{self._base_urls[nbh]}"
 
     @keyword
     def get_jupyter_server_token(
-        self, nbserver: typing.Optional[subprocess.Popen] = None
+        self,
+        nbserver: typing.Optional[subprocess.Popen] = None,
     ) -> str:
-        """Get the given (or most recently-launched) server's token"""
+        """Get the given (or most recently-launched) server's token."""
         nbh = nbserver or self._handles[-1]
         return self._tokens[nbh]
 
     @keyword
     def wait_for_new_jupyter_server_to_be_ready(
-        self, command: typing.Optional[str] = None, *args, **config
+        self,
+        command: typing.Optional[str] = None,
+        *args,
+        **config,
     ) -> subprocess.Popen:
-        """Get the given (or most recently-launched) server's token. See
-        [#Start New Jupyter Server|Start New Jupyter Server]
+        """Get the given (or most recently-launched) server's token.
+
+        See [#Start New Jupyter Server|Start New Jupyter Server].
         """
         handle = self.start_new_jupyter_server(command, *args, **config)
         self.wait_for_jupyter_server_to_be_ready(handle)
         return handle
 
     @keyword
-    def terminate_all_jupyter_servers(self, timeout: str = "6s") -> int:
-        """Close all Jupyter servers started by
-        [#Start New Jupyter Server|Start New Jupyter Server],
-        waiting ``timeout`` to ensure all files/processes are freed before
+    def shut_down_jupyter_server(self, nbserver=None) -> int:
+        """Gracefully shut down a Jupyter server started by [#Start New Jupyter Server|Start New Jupyter Server].
+
+        If no ``handle`` is given, the last-started server will be shut down.
+        """
+        nbh = nbserver or self._handles[-1]
+        url = self.get_jupyter_server_url(nbh)
+        token = self.get_jupyter_server_token(nbh)
+
+        try:
+            urlopen(f"{url}api/shutdown?token={token}", data=[])
+        except Exception as err:
+            BuiltIn().log(err)
+            return 0
+
+        self._ports.pop(nbh)
+        self._base_urls.pop(nbh)
+        self._tokens.pop(nbh)
+
+        return 1
+
+    @keyword
+    def clean_up_jupyter_server_files(self, nbserver=None) -> int:
+        """Clean up the files owned by a started by [#Start New Jupyter Server|Jupyter Server].
+
+        If no ``handle`` is given, the last-started server will be terminated.
+        """
+        nbh = nbserver or self._handles[-1]
+
+        shutil.rmtree(self._tmpdirs[nbh], ignore_errors=True)
+
+        self._tmpdirs.pop(nbh)
+
+    @keyword
+    def terminate_jupyter_server(self, nbserver=None) -> int:
+        """Close a Jupyter server started by [#Start New Jupyter Server|Start New Jupyter Server].
+
+        If no ``nbserver`` is given, the last-started server will be terminated.
+
+        Waiting ``timeout`` to ensure all files/processes are freed before
         cleaning up temporary directories, if any.
         """
         plib = BuiltIn().get_library_instance("Process")
 
-        self.wait_for_jupyter_server_to_be_ready()
+        nbh = nbserver or self._handles[-1]
+
+        plib.terminate_process(nbh)
+
+        self._handles.remove(nbh)
+
+        return 1
 
-        terminated = 0
-        shutdown = 0
+    @keyword
+    def terminate_all_jupyter_servers(self, timeout: str = "6s") -> int:
+        """Close all Jupyter servers started by [#Start New Jupyter Server|Start New Jupyter Server].
+
+        Waiting ``timeout`` after termination to ensure all files/processes are freed before
+        cleaning up temporary directories.
+        """
+        was_shutdown = []
+        was_terminated = []
         for nbh in self._handles:
-            url = self.get_jupyter_server_url(nbh)
-            token = self.get_jupyter_server_token(nbh)
             try:
-                urlopen(f"{url}api/shutdown?token={token}", data=[])
-                shutdown += 1
+                self.shut_down_jupyter_server(nbh)
+                was_shutdown += [nbh]
             except Exception as err:
                 BuiltIn().log(err)
 
-        if shutdown:
-            for nbh in self._handles:
-                try:
-                    plib.terminate_process(nbh)
-                    terminated += 1
-                except Exception as err:
-                    BuiltIn().log(err)
-            if self._handles:
-                BuiltIn().sleep(timeout)
-            for nbh in self._handles:
-                try:
-                    plib.terminate_process(nbh, kill=True)
-                except Exception as err:
-                    BuiltIn().log(err)
-
-        # give processes a mo to shutdown
-        if terminated or shutdown and self._tmpdirs:
-            for nbh in self._handles:
-                shutil.rmtree(self._tmpdirs[nbh])
-
-        self._handles = []
-        self._tmpdirs = {}
-        self._notebook_dirs = {}
-        self._ports = {}
-        self._base_urls = {}
-        self._tokens = {}
+        handles = list(self._handles)
+
+        for nbh in handles:
+            try:
+                self.terminate_jupyter_server(nbh)
+                was_terminated += [nbh]
+            except Exception as err:
+                BuiltIn().log(err)
+
+        if was_shutdown or was_terminated:
+            BuiltIn().sleep(timeout)
+
+        tmpdir_handles = list(self._tmpdirs)
+
+        for nbh in tmpdir_handles:
+            self.clean_up_jupyter_server_files(nbh)
 
-        return terminated
+        return len(was_terminated)
 
     @keyword
     def get_unused_port(self) -> int:
+        """Find an unused network port (could still create race conditions)."""
         s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         s.bind(("localhost", 0))
         s.listen(1)
         port = s.getsockname()[1]
         s.close()
         return port
```

### Comparing `robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/keywords/webelements.py` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/keywords/webelements.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,36 @@
-"""Handle working with WebElements
-"""
+"""Handle working with WebElements."""
 
 from typing import List, Union
 
 from selenium.webdriver.remote.webelement import WebElement
 from SeleniumLibrary.base import LibraryComponent, keyword
 
 
 class WebElementKeywords(LibraryComponent):
+
+    """A component for working with WebElements."""
+
     @keyword(name="Get WebElement Relative To")
     def get_webelement_relative_to(
-        self, element: WebElement, locator: Union[WebElement, str]
+        self,
+        element: WebElement,
+        locator: Union[WebElement, str],
     ) -> WebElement:
-        """Returns the first WebElement relative to ``element`` matching the given ``locator``.
+        """Get the first WebElement relative to ``element`` matching the given ``locator``.
+
         See the `Locating elements` section for details about the locator
         syntax.
         """
         return self.element_finder.find_element(locator=locator, parent=element)
 
     @keyword(name="Get WebElements Relative To")
     def get_webelements_relative_to(
-        self, element: WebElement, locator: Union[WebElement, str]
+        self,
+        element: WebElement,
+        locator: Union[WebElement, str],
     ) -> List[WebElement]:
-        """Returns a list of WebElement objects relative to ``element` matching the ``locator``.
-        See the `Locating elements` section for details about the locator
-        syntax.
+        """Get a list of WebElement objects relative to ``element` matching the ``locator``.
+
+        See the `Locating elements` section for details about the locator syntax.
         """
         return self.element_finder.find_elements(locator=locator, parent=element)
```

### Comparing `robotframework-jupyterlibrary-0.4.2/src/JupyterLibrary/magic.py` & `robotframework_jupyterlibrary-0.5.0a0/src/JupyterLibrary/magic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,62 +1,66 @@
-""" a lightweight robot runner
+"""a lightweight robot runner.
 
 Install once (per notebook/kernel):
 
     %reload_ext JupyterLibrary
 """
-from pathlib import Path
-from hashlib import sha256
+import contextlib
 import shutil
 import tempfile
+from hashlib import sha256
+from pathlib import Path
 
-from pygments import highlight
-from pygments.formatters.html import HtmlFormatter
-from pygments.lexers.robotframework import RobotFrameworkLexer
-from pygments.styles import get_all_styles
-
+import robot
 from IPython import get_ipython
-from IPython.display import (
-    display,
-    HTML,
-    Markdown,
-)
 from IPython.core import magic_arguments
 from IPython.core.magic import (
     Magics,
-    magics_class,
     cell_magic,
+    magics_class,
 )
-
-import robot
+from IPython.display import (
+    HTML,
+    Markdown,
+    display,
+)
+from pygments import highlight
+from pygments.formatters.html import HtmlFormatter
+from pygments.lexers.robotframework import RobotFrameworkLexer
+from pygments.styles import get_all_styles
 
 HAS_CORE_TIDY = False
+HAS_WIDGETS = False
+
 try:
     from robot.tidy import Tidy
 
     HAS_CORE_TIDY = True
 except ImportError:
     pass
 
 
 try:
     import ipywidgets
-except:
-    ipywidgets = None
+
+    HAS_WIDGETS = True
+except ImportError:
+    pass
 
 
-ENC = dict(encoding="utf-8")
+ENC = {"encoding": "utf-8"}
 
 
 @magics_class
 class RobotMagics(Magics):
-    """
-    Run Robot Framework code
+
+    """Run Robot Framework code.
 
     Example:
+    -------
         %%robot --
         *** Tasks ***
         Just Log Something
             Log    Something
     """
 
     PRETTY_CLASS = "robot-magic"
@@ -66,15 +70,18 @@
     @magic_arguments.argument(
         "-o",
         "--output-dir",
         default=None,
         help="""Name of directory to update (default:cwd/_robot_magic_) """,
     )
     @magic_arguments.argument(
-        "-e", "--execute", default=True, help="""run the robot test"""
+        "-e",
+        "--execute",
+        default=True,
+        help="""run the robot test""",
     )
     @magic_arguments.argument(
         "-p",
         "--pretty",
         default=True,
         help=(
             """print out syntax highlighted, tidied source. """
@@ -102,37 +109,38 @@
     @magic_arguments.argument(
         "-n",
         "--name",
         default=None,
         help="name of the suite. default: Untitled_<hash>",
     )
     def robot(self, line, cell):
-        """run some Robot Framework code"""
+        """Run some Robot Framework code."""
         line = f" {line} "
 
         m = sha256()
         m.update(line.encode("utf-8"))
         m.update(cell.encode("utf-8"))
 
         content_hash = str(m.hexdigest())[:12]
 
         args = magic_arguments.parse_argstring(self.robot, line)
 
-        if ipywidgets and args.gui.lower() in ["widget", "w", "widgets"]:
-            self.widget(args, cell, content_hash)
+        if HAS_WIDGETS and args.gui.lower() in ["widget", "w", "widgets"]:
+            self.widget(args, cell)
         else:
             if args.pretty and HAS_CORE_TIDY:
                 html = self.pretty_core(args, cell)
                 if args.gui == "display":
                     display(html)
 
             if args.execute:
                 self.execute(args, cell, content_hash)
 
-    def widget(self, args, cell, content_hash):
+    def widget(self, args, cell):
+        """Display a widget of files built during a run."""
         log = ipywidgets.HTML()
         titles = ["Log"]
         children = [log]
         tabs = ipywidgets.Tab(children)
         tabs.titles = titles
 
         if args.pretty:
@@ -141,16 +149,16 @@
             with out:
                 display(self.pretty(args, cell))
 
             tabs.children = [*tabs.children, out]
             tabs.titles = [*tabs.titles, "Pretty"]
         display(tabs)
 
-    def execute(self, args, cell, content_hash):
-        """run a cell in the outputdir, in a directory named after the content hash"""
+    def execute(self, args, cell: str, content_hash: str):
+        """Run a cell in the outputdir, in a directory named after the content hash."""
         ip = get_ipython()
         if args.output_dir:
             outputdir = Path(args.output_dir).resolve() / "_robot_magic_" / content_hash
         else:
             outputdir = Path.cwd() / "_robot_magic_" / content_hash
         display(Markdown(f"- _🤖 making files in_ `{outputdir}`"))
         if outputdir.exists():
@@ -166,87 +174,79 @@
 
         display(Markdown("- _🤖 running!_"))
         stdout_file = outputdir / "stdout.txt"
         stderr_file = outputdir / "stderr.txt"
 
         robot_args = ip.user_ns[args.arg] if args.arg else {}
 
-        with open(stdout_file, "w+") as stdout:
-            with open(stderr_file, "w+") as stderr:
-                try:
-                    rc = robot.run(
-                        robot_file,
-                        outputdir=outputdir,
-                        stderr=stderr,
-                        stdout=stdout,
-                        **robot_args,
-                    )
-                except SystemExit:
-                    pass
+        with contextlib.suppress(SystemExit), stdout_file.open(
+            "w+",
+        ) as stdout, stderr_file.open(
+            "w+",
+        ) as stderr:
+            rc = robot.run(
+                robot_file,
+                outputdir=outputdir,
+                stderr=stderr,
+                stdout=stdout,
+                **robot_args,
+            )
 
         if args.gui == "display":
             for outfile in [stdout_file, stderr_file]:
                 display(
                     HTML(
-                        f"""
-                        <ul><li>
+                        f"""<ul><li>
                             <code>{outfile.name}</code>
                             <code><pre>{outfile.read_text(**ENC) or "empty"}</pre></code>
-                        </li></ul>
-                        """
-                    )
+                        </li></ul>""",
+                    ),
                 )
             files = [
                 f"""<li>
                     <a href="{p.relative_to(Path.cwd()).as_posix()}"
                             data-commandlinker-command="filebrowser:open"
                             data-commandlinker-args="{{}}">
                         {p.relative_to(outputdir).as_posix()}
                     </a>
-                </li>
-                """
+                </li>"""
                 for p in sorted(outputdir.rglob("*"))
             ]
             display(
                 HTML(
-                    f"""
-                    <ul><li><details>
+                    f"""<ul><li><details>
                     <summary>{len(files)} Files</summary>
                     <ul>
                     {"".join(files)}
                     </ul>
-                    </li></ul>
-                    """
-                )
+                    </li></ul>""",
+                ),
             )
             display(Markdown(f"- _🤖 returned {rc}_"))
 
         if rc:
-            raise RuntimeError(f"robot returned {rc}")
+            msg = f"robot returned {rc}"
+            raise RuntimeError(msg)
 
     def pretty_core(self, args, cell):
-        """pretty-print the robot text"""
+        """pretty-print the robot text."""
         tidier = Tidy()
 
         with tempfile.TemporaryDirectory() as td:
             tdp = Path(td)
             it = tdp / "ugly.robot"
             it.write_text(cell, **ENC)
             tidier.inplace(str(it))
             cell = it.read_text(**ENC)
 
         lexer = RobotFrameworkLexer()
         formatter = HtmlFormatter(cssclass=self.PRETTY_CLASS, style=args.style)
         css = formatter.get_style_defs(f".{self.PRETTY_CLASS}")
         highlighted = highlight(cell, lexer, formatter)
-        html = HTML(
-            f"""
-            <ul><li>
+        return HTML(
+            f"""<ul><li>
             <details>
                 <summary>Formatted Robot Code</summary>
                 <style>{css}</style>{highlighted}
             </details>
-            </li></ul>
-        """
+            </li></ul>""",
         )
-
-        return html
```

