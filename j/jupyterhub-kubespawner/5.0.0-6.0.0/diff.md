# Comparing `tmp/jupyterhub_kubespawner-5.0.0.tar.gz` & `tmp/jupyterhub_kubespawner-6.0.0.tar.gz`

## Comparing `jupyterhub_kubespawner-5.0.0.tar` & `jupyterhub_kubespawner-6.0.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/.flake8
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/.readthedocs.yaml
--rw-r--r--   0        0        0     7235 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/MANIFEST.in
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/RELEASE.md
--rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/jupyterhub_config.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/.github/dependabot.yaml
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/.github/workflows/test.yaml
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/Makefile
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/make.bat
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/requirements.txt
--rw-r--r--   0        0        0    66490 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/source/changelog.md
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/source/conf.py
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/source/index.md
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/source/objects.md
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/source/reflector.md
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/source/spawner.md
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/source/ssl.md
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/source/utils.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/docs/source/_static/.gitkeep
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/kubespawner/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/kubespawner/_version.py
--rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/kubespawner/clients.py
--rw-r--r--   0        0        0    37969 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/kubespawner/objects.py
--rw-r--r--   0        0        0    22353 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/kubespawner/proxy.py
--rw-r--r--   0        0        0    16100 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/kubespawner/reflector.py
--rw-r--r--   0        0        0   125371 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/kubespawner/spawner.py
--rw-r--r--   0        0        0     8415 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/kubespawner/utils.py
--rw-r--r--   0        0        0    20490 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/tests/conftest.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/tests/jupyterhub_config.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/tests/test_clients.py
--rw-r--r--   0        0        0   102281 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/tests/test_objects.py
--rw-r--r--   0        0        0    46364 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/tests/test_spawner.py
--rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/tests/test_utils.py
--rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/.gitignore
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/LICENSE
--rw-r--r--   0        0        0     5414 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/README.md
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/pyproject.toml
--rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/.flake8
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     7235 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/MANIFEST.in
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/RELEASE.md
+-rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/jupyterhub_config.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/.github/dependabot.yaml
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/docs/Makefile
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/docs/make.bat
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/docs/requirements.txt
+-rw-r--r--   0        0        0    69220 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/docs/source/changelog.md
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/docs/source/conf.py
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/docs/source/index.md
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/docs/source/objects.md
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/docs/source/reflector.md
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/docs/source/spawner.md
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/docs/source/ssl.md
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/docs/source/utils.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/docs/source/_static/.gitkeep
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/kubespawner/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/kubespawner/_version.py
+-rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/kubespawner/clients.py
+-rw-r--r--   0        0        0    37969 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/kubespawner/objects.py
+-rw-r--r--   0        0        0    22365 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/kubespawner/proxy.py
+-rw-r--r--   0        0        0    16100 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/kubespawner/reflector.py
+-rw-r--r--   0        0        0   124127 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/kubespawner/spawner.py
+-rw-r--r--   0        0        0     8415 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/kubespawner/utils.py
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/kubespawner/templates/form.html
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/kubespawner/templates/style.css
+-rw-r--r--   0        0        0    20490 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/tests/jupyterhub_config.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/tests/test_clients.py
+-rw-r--r--   0        0        0   102281 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/tests/test_objects.py
+-rw-r--r--   0        0        0    46364 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/tests/test_spawner.py
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/tests/test_utils.py
+-rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/.gitignore
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/LICENSE
+-rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/README.md
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8117 2020-02-02 00:00:00.000000 jupyterhub_kubespawner-6.0.0/PKG-INFO
```

### Comparing `jupyterhub_kubespawner-5.0.0/.pre-commit-config.yaml` & `jupyterhub_kubespawner-6.0.0/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # - Run on all files:   pre-commit run --all-files
 # - Register git hooks: pre-commit install --install-hooks
 #
 repos:
   # Autoformat: Python code, syntax patterns are modernized
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.3.2
     hooks:
       - id: pyupgrade
         args:
           - --py37-plus
 
   # Autoformat: Python code
   - repo: https://github.com/pycqa/isort
@@ -27,17 +27,19 @@
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
   # Autoformat: markdown, yaml
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.6
+    rev: v3.0.0-alpha.9-for-vscode
     hooks:
       - id: prettier
+        # Don't run prettier on our jinja2 template files. We run djlint instead
+        exclude: "kubespawner/templates/.*\\.html"
 
   # Misc...
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     # ref: https://github.com/pre-commit/pre-commit-hooks#hooks-available
     hooks:
       # Autoformat: Makes sure files end in a newline and only a newline.
@@ -55,10 +57,21 @@
 
   # Lint: Python code
   - repo: https://github.com/PyCQA/flake8
     rev: "6.0.0"
     hooks:
       - id: flake8
 
+  # Lint our jinja2 templates
+  - repo: https://github.com/Riverside-Healthcare/djLint
+    rev: v1.24.0
+    hooks:
+      - id: djlint-jinja
+        files: "kubespawner/templates/.*\\.html"
+        types_or:
+          - html
+        args:
+          - --reformat
+
 # pre-commit.ci config reference: https://pre-commit.ci/#configuration
 ci:
   autoupdate_schedule: monthly
```

### Comparing `jupyterhub_kubespawner-5.0.0/CONTRIBUTING.md` & `jupyterhub_kubespawner-6.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyterhub_kubespawner-5.0.0/RELEASE.md` & `jupyterhub_kubespawner-6.0.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterhub_kubespawner-5.0.0/jupyterhub_config.py` & `jupyterhub_kubespawner-6.0.0/jupyterhub_config.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_kubespawner-5.0.0/.github/dependabot.yaml` & `jupyterhub_kubespawner-6.0.0/.github/dependabot.yaml`

 * *Files identical despite different names*

### Comparing `jupyterhub_kubespawner-5.0.0/.github/workflows/publish.yaml` & `jupyterhub_kubespawner-6.0.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `jupyterhub_kubespawner-5.0.0/.github/workflows/test.yaml` & `jupyterhub_kubespawner-6.0.0/.github/workflows/test.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 on:
   pull_request:
     paths-ignore:
       - "docs/**"
       - "**.md"
       - ".github/workflows/*"
-      - "!.github/workflows/test-chart.yaml"
+      - "!.github/workflows/test.yaml"
   push:
     paths-ignore:
       - "docs/**"
       - "**.md"
       - ".github/workflows/*"
-      - "!.github/workflows/test-chart.yaml"
+      - "!.github/workflows/test.yaml"
     branches-ignore:
       - "dependabot/**"
       - "pre-commit-ci-update-config"
   workflow_dispatch:
 
 jobs:
   run-pytest:
@@ -35,20 +35,23 @@
         # gain meaning on how job steps use them.
         #
         # k3s-channel:        https://update.k3s.io/v1-release/channels
         # kubernetes_asyncio:  https://github.com/tomplus/kubernetes_asyncio/tags
         #
         include:
           # Tests with oldest supported Python, jupyterhub, k8s, and k8s client
+          #
+          # NOTE: If lower bounds are updated, also update our test for the
+          #       lower bounds in pyproject.toml.
+          #
           - python: "3.7"
-            k3s: v1.23
+            k3s: v1.24
             test_dependencies: >-
-              jupyterhub==1.3.0
-              kubernetes_asyncio==23.6.0
-              traitlets==4.3.2
+              jupyterhub==4.0.0
+              kubernetes_asyncio==24.2.3
 
           # Test with modern python and k8s versions
           - python: "3.9"
             k3s: stable
           - python: "3.10"
             k3s: latest
```

### Comparing `jupyterhub_kubespawner-5.0.0/docs/Makefile` & `jupyterhub_kubespawner-6.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyterhub_kubespawner-5.0.0/docs/make.bat` & `jupyterhub_kubespawner-6.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyterhub_kubespawner-5.0.0/docs/source/changelog.md` & `jupyterhub_kubespawner-6.0.0/docs/source/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,56 @@
 # Changes in KubeSpawner
 
 <!-- PR summaries generated using github-activity CLI, see RELEASE.md for details -->
 
 ## [Unreleased]
 
+#### Breaking changes
+
+- JupyterHub 4 is now required by KubeSpawner.
+  [#726](https://github.com/jupyterhub/kubespawner/pull/726)
+- Versions of K8s older than 1.24 are no longer supported, KubeSpawner may still
+  work but this is not guaranteed.
+  [#726](https://github.com/jupyterhub/kubespawner/pull/726)
+
+## 6.0
+
+### [6.0.0] - 2023-05-31
+
+#### Breaking changes
+
+- Versions of K8s older than 1.24 are no longer officially supported,
+  KubeSpawner still likely works but this is not guaranteed through tests.
+  [#726](https://github.com/jupyterhub/kubespawner/pull/726)
+- `jupyterhub` 4+ and `kubernetes_asyncio` 24.2.3+ is now required.
+  [#726](https://github.com/jupyterhub/kubespawner/pull/726)
+
+#### New features added
+
+- Allow building more complex profile_list templates [#724](https://github.com/jupyterhub/kubespawner/pull/724) ([@yuvipanda](https://github.com/yuvipanda))
+
+#### Bugs fixed
+
+- [KubeIngressProxy] Do not try to escape None [#731](https://github.com/jupyterhub/kubespawner/pull/731) ([@dolfinus](https://github.com/dolfinus))
+- Select profile if any of its choices are interacted with [#729](https://github.com/jupyterhub/kubespawner/pull/729) ([@batpad](https://github.com/batpad))
+
+#### Maintenance and upkeep improvements
+
+- Require jupyterhub 4+, currently latest kubernetes_asyncio, and stop testing k8s 1.23 [#726](https://github.com/jupyterhub/kubespawner/pull/726) ([@consideRatio](https://github.com/consideRatio))
+
+#### Documentation improvements
+
+- Update Readme badges & requirements [#733](https://github.com/jupyterhub/kubespawner/pull/733) ([@dolfinus](https://github.com/dolfinus))
+
+#### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyterhub/kubespawner/graphs/contributors?from=2023-04-18&to=2023-05-30&type=c))
+
+[@batpad](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Abatpad+updated%3A2023-04-18..2023-05-30&type=Issues) | [@consideRatio](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3AconsideRatio+updated%3A2023-04-18..2023-05-30&type=Issues) | [@dolfinus](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Adolfinus+updated%3A2023-04-18..2023-05-30&type=Issues) | [@manics](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Amanics+updated%3A2023-04-18..2023-05-30&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Apre-commit-ci+updated%3A2023-04-18..2023-05-30&type=Issues) | [@yuvipanda](https://github.com/search?q=repo%3Ajupyterhub%2Fkubespawner+involves%3Ayuvipanda+updated%3A2023-04-18..2023-05-30&type=Issues)
+
 ## 5.0
 
 ### [5.0.0] - 2023-04-19
 
 #### Breaking changes
 
 - Versions of K8s older than 1.23 are no longer supported, KubeSpawner may still
@@ -730,15 +773,16 @@
 - Require Python >= 3.5
 - Expose lots more Kubernetes options
 - Support configuration profiles via :attr:`.KubeSpawner.profile_list`
 - Support Kubernetes events for the progress API in JupyterHub 0.9.
 - Update Kubernetes Python client to 6.0 (supporting Kubernetes 1.10 APIs)
 - Numerous bugfixes
 
-[unreleased]: https://github.com/jupyterhub/kubespawner/compare/5.0.0...HEAD
+[unreleased]: https://github.com/jupyterhub/kubespawner/compare/6.0.0...HEAD
+[6.0.0]: https://github.com/jupyterhub/kubespawner/compare/5.0.0...6.0.0
 [5.0.0]: https://github.com/jupyterhub/kubespawner/compare/4.3.0...5.0.0
 [4.3.0]: https://github.com/jupyterhub/kubespawner/compare/4.2.0...4.3.0
 [4.2.0]: https://github.com/jupyterhub/kubespawner/compare/4.1.0...4.2.0
 [4.1.0]: https://github.com/jupyterhub/kubespawner/compare/4.0.0...4.1.0
 [4.0.0]: https://github.com/jupyterhub/kubespawner/compare/3.0.2...4.0.0
 [3.0.2]: https://github.com/jupyterhub/kubespawner/compare/3.0.1...3.0.2
 [3.0.1]: https://github.com/jupyterhub/kubespawner/compare/3.0.0...3.0.1
```

### Comparing `jupyterhub_kubespawner-5.0.0/docs/source/conf.py` & `jupyterhub_kubespawner-6.0.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_kubespawner-5.0.0/docs/source/index.md` & `jupyterhub_kubespawner-6.0.0/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `jupyterhub_kubespawner-5.0.0/kubespawner/clients.py` & `jupyterhub_kubespawner-6.0.0/kubespawner/clients.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_kubespawner-5.0.0/kubespawner/objects.py` & `jupyterhub_kubespawner-6.0.0/kubespawner/objects.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_kubespawner-5.0.0/kubespawner/proxy.py` & `jupyterhub_kubespawner-6.0.0/kubespawner/proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,20 +345,20 @@
             raw_servername, safe=safe_chars, escape_char='-'
         ).lower()
 
         hub_namespace = self._namespace_default()
         if hub_namespace == "default":
             hub_namespace = "user"
 
-        raw_username = data.get('user')
+        raw_username = data.get('user') or ''
         safe_username = escapism.escape(
             raw_username, safe=safe_chars, escape_char='-'
         ).lower()
 
-        raw_servicename = data.get('services')
+        raw_servicename = data.get('services') or ''
         safe_servicename = escapism.escape(
             raw_servicename, safe=safe_chars, escape_char='-'
         ).lower()
 
         raw_routespec = routespec
         safe_routespec = self._safe_name_for_routespec(routespec)
```

### Comparing `jupyterhub_kubespawner-5.0.0/kubespawner/reflector.py` & `jupyterhub_kubespawner-6.0.0/kubespawner/reflector.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_kubespawner-5.0.0/kubespawner/spawner.py` & `jupyterhub_kubespawner-6.0.0/kubespawner/spawner.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import sys
 import warnings
 from functools import partial
 from typing import Optional, Tuple, Type
 from urllib.parse import urlparse
 
 import escapism
-from jinja2 import BaseLoader, Environment
+from jinja2 import ChoiceLoader, Environment, FileSystemLoader, PackageLoader
 from jupyterhub.spawner import Spawner
 from jupyterhub.traitlets import Callable, Command
 from jupyterhub.utils import exponential_backoff, maybe_future
 from kubernetes_asyncio import client
 from kubernetes_asyncio.client.rest import ApiException
 from slugify import slugify
 from traitlets import (
@@ -1470,91 +1470,49 @@
         help="""
         Whether to delete pods that have stopped themselves.
         Set to False to leave stopped pods in the completed state,
         allowing for easier debugging of why they may have stopped.
         """,
     )
 
-    profile_form_template = Unicode(
-        """
-        <style>
-            /*
-                .profile divs holds two div tags: one for a radio button, and one
-                for the profile's content.
-            */
-            #kubespawner-profiles-list .profile {
-                display: flex;
-                flex-direction: row;
-                font-weight: normal;
-                border-bottom: 1px solid #ccc;
-                padding-bottom: 12px;
-            }
-
-            #kubespawner-profiles-list .profile .radio {
-                padding: 12px;
-            }
-
-            /* .option divs holds a label and a select tag */
-            #kubespawner-profiles-list .profile .option {
-                display: flex;
-                flex-direction: row;
-                align-items: center;
-                padding-bottom: 12px;
-            }
+    additional_profile_form_template_paths = List(
+        default=[],
+        help="""
+        Additional paths to search for jinja2 templates when rendering profile_form.
 
-            #kubespawner-profiles-list .profile .option label {
-                font-weight: normal;
-                margin-right: 8px;
-                min-width: 96px;
-            }
-        </style>
+        These directories will be searched before the default `templates/` directory
+        shipped with kubespawner with the default template.
 
-        <div class='form-group' id='kubespawner-profiles-list'>
-            {%- for profile in profile_list %}
-            {#- Wrap everything in a <label> so clicking anywhere selects the option #}
-            <label for='profile-item-{{ profile.slug }}' class='profile'>
-                <div class='radio'>
-                    <input type='radio' name='profile' id='profile-item-{{ profile.slug }}' value='{{ profile.slug }}' {% if profile.default %}checked{% endif %} />
-                </div>
-                <div>
-                    <h3>{{ profile.display_name }}</h3>
-
-                    {%- if profile.description %}
-                    <p>{{ profile.description }}</p>
-                    {%- endif %}
-
-                    {%- if profile.profile_options %}
-                    <div>
-                        {%- for k, option in profile.profile_options.items() %}
-                        <div class='option'>
-                            <label for='profile-option-{{profile.slug}}-{{k}}'>{{option.display_name}}</label>
-                            <select name="profile-option-{{profile.slug}}-{{k}}" class="form-control">
-                                {%- for k, choice in option['choices'].items() %}
-                                <option value="{{ k }}" {% if choice.default %}selected{%endif %}>{{ choice.display_name }}</option>
-                                {%- endfor %}
-                            </select>
-                        </div>
-                        {%- endfor %}
-                    </div>
-                    {%- endif %}
-                </div>
-            </label>
-            {%- endfor %}
-        </div>
+        Any file named `form.html` in these directories will be used to render the
+        profile options form.
         """,
         config=True,
+    )
+
+    profile_form_template = Unicode(
+        "",
+        config=True,
         help="""
-        Jinja2 template for constructing profile list shown to user.
+        Literal Jinja2 template for constructing profile list shown to user.
 
         Used when `profile_list` is set.
 
         The contents of `profile_list` are passed in to the template.
         This should be used to construct the contents of a HTML form. When
         posted, this form is expected to have an item with name `profile` and
         the value the index of the profile in `profile_list`.
+
+        When this traitlet is not set, the default template `form.html` from the
+        directory `kubespawner/templates` is used. Admins can override this by
+        setting the `additional_profile_form_template_paths` config to a directory
+        with jinja2 templates, and any file named `form.html` in there will be used
+        instead of the default.
+
+        Using additional_profile_form_template_paths is recommended instead of
+        this.
         """,
     )
 
     profile_list = Union(
         trait_types=[List(trait=Dict()), Callable()],
         config=True,
         help="""
@@ -2947,17 +2905,29 @@
     def _env_keep_default(self):
         return []
 
     _profile_list = None
 
     def _render_options_form(self, profile_list):
         self._profile_list = self._init_profile_list(profile_list)
-        profile_form_template = Environment(loader=BaseLoader).from_string(
-            self.profile_form_template
+
+        loader = ChoiceLoader(
+            [
+                FileSystemLoader(self.additional_profile_form_template_paths),
+                PackageLoader("kubespawner", "templates"),
+            ]
         )
+
+        env = Environment(loader=loader)
+        if self.profile_form_template != "":
+            # Admin has custom set the profile_form_template as a templated string
+            # so we use that directly
+            profile_form_template = env.from_string(self.profile_form_template)
+        else:
+            profile_form_template = env.get_template("form.html")
         return profile_form_template.render(profile_list=self._profile_list)
 
     async def _render_options_form_dynamically(self, current_spawner):
         profile_list = await maybe_future(self.profile_list(current_spawner))
         profile_list = self._init_profile_list(profile_list)
         return self._render_options_form(profile_list)
```

### Comparing `jupyterhub_kubespawner-5.0.0/kubespawner/utils.py` & `jupyterhub_kubespawner-6.0.0/kubespawner/utils.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_kubespawner-5.0.0/tests/conftest.py` & `jupyterhub_kubespawner-6.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_kubespawner-5.0.0/tests/jupyterhub_config.py` & `jupyterhub_kubespawner-6.0.0/tests/jupyterhub_config.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_kubespawner-5.0.0/tests/test_clients.py` & `jupyterhub_kubespawner-6.0.0/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_kubespawner-5.0.0/tests/test_objects.py` & `jupyterhub_kubespawner-6.0.0/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_kubespawner-5.0.0/tests/test_spawner.py` & `jupyterhub_kubespawner-6.0.0/tests/test_spawner.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_kubespawner-5.0.0/tests/test_utils.py` & `jupyterhub_kubespawner-6.0.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `jupyterhub_kubespawner-5.0.0/.gitignore` & `jupyterhub_kubespawner-6.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterhub_kubespawner-5.0.0/LICENSE` & `jupyterhub_kubespawner-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterhub_kubespawner-5.0.0/README.md` & `jupyterhub_kubespawner-6.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # [kubespawner](https://github.com/jupyterhub/kubespawner) (jupyterhub-kubespawner @ PyPI)
 
 [![Latest PyPI version](https://img.shields.io/pypi/v/jupyterhub-kubespawner?logo=pypi)](https://pypi.python.org/pypi/jupyterhub-kubespawner)
 [![Latest conda-forge version](https://img.shields.io/conda/vn/conda-forge/jupyterhub-kubespawner?logo=conda-forge)](https://anaconda.org/conda-forge/jupyterhub-kubespawner)
 [![Documentation status](https://img.shields.io/readthedocs/jupyterhub-kubespawner?logo=read-the-docs)](https://jupyterhub-kubespawner.readthedocs.io/en/latest/?badge=latest)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/jupyterhub/kubespawner/test.yaml?logo=github&label=tests)](https://github.com/jupyterhub/kubespawner/actions)
 [![Code coverage](https://codecov.io/gh/jupyterhub/kubespawner/branch/main/graph/badge.svg)](https://codecov.io/gh/jupyterhub/kubespawner)
-[![](https://img.shields.io/pypi/v/jupyterhub-kubespawner.svg?logo=pypi)](https://pypi.python.org/pypi/jupyterhub-kubespawner)
 
 The _kubespawner_ (also known as JupyterHub Kubernetes Spawner) enables JupyterHub to spawn
 single-user notebook servers on a [Kubernetes](https://kubernetes.io/)
 cluster.
 
 See the [KubeSpawner documentation](https://jupyterhub-kubespawner.readthedocs.io) for more
 information about features and usage. In particular, here is [a list of all the spawner options](https://jupyterhub-kubespawner.readthedocs.io/en/latest/spawner.html#module-kubespawner.spawner).
@@ -53,17 +52,21 @@
   [multiple clouds at the same time](https://kubernetes.io/docs/user-guide/federation/).
 
 In general, Kubernetes provides a ton of well thought out, useful features -
 and you can use all of them along with this spawner.
 
 ## Requirements
 
+### JupyterHub
+
+Requires JupyterHub 4.0+
+
 ### Kubernetes
 
-Everything should work from Kubernetes v1.6+.
+Everything should work from Kubernetes v1.24+.
 
 The [Kube DNS addon](https://kubernetes.io/docs/user-guide/connecting-applications/#dns)
 is not strictly required - the spawner uses
 [environment variable](https://kubernetes.io/docs/user-guide/connecting-applications/#environment-variables)
 based discovery instead. Your kubernetes cluster will need to be configured to
 support the types of volumes you want to use.
```

### Comparing `jupyterhub_kubespawner-5.0.0/pyproject.toml` & `jupyterhub_kubespawner-6.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -25,19 +25,19 @@
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     # NOTE: If lower bounds are updated, also update our test for the lower
     #       bounds in .github/workflows/test.yaml.
     "escapism",
     "jinja2",
-    "jupyterhub>=1.3.0",
-    "kubernetes_asyncio>=23.6.0",
+    "jupyterhub>=4.0.0",
+    "kubernetes_asyncio>=24.2.3",
     "python-slugify",
     "pyYAML",
-    "traitlets>=4.3.2",
+    "traitlets",
     "urllib3",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = [
     "kubernetes>=11",
@@ -47,14 +47,21 @@
 ]
 
 [project.urls]
 Documentation = "https://jupyterhub-kubespawner.readthedocs.io"
 Source = "https://github.com/jupyterhub/kubespawner"
 Issues = "https://github.com/jupyterhub/kubespawner/issues"
 
+# Explicitly include our profile_list templates, as hatch doesn't
+# respect MANIFEST.in.
+# Documentation: https://hatch.pypa.io/latest/config/build/#artifacts
+[tool.hatch.build]
+artifacts = [
+    "kubespawner/templates/*"
+]
 
 # black is used for autoformatting Python code
 #
 # ref: https://black.readthedocs.io/en/stable/
 #
 [tool.black]
 skip-string-normalization = true
@@ -99,15 +106,15 @@
 #
 # ref: https://github.com/your-tools/tbump#readme
 #
 [tool.tbump]
 github_url = "https://github.com/jupyterhub/kubespawner"
 
 [tool.tbump.version]
-current = "5.0.0"
+current = "6.0.0"
 regex = '''
     (?P<major>\d+)
     \.
     (?P<minor>\d+)
     \.
     (?P<patch>\d+)
     (?P<pre>((a|b|rc)\d+)|)
@@ -117,7 +124,15 @@
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
 tag_template = "{new_version}"
 
 [[tool.tbump.file]]
 src = "kubespawner/_version.py"
+
+# djlint is used for autoformatting jinja templates
+#
+# ref: https://www.djlint.com/docs/formatter/
+#
+[tool.djlint]
+indent = 2
+profile = "jinja"
```

### Comparing `jupyterhub_kubespawner-5.0.0/PKG-INFO` & `jupyterhub_kubespawner-6.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterhub-kubespawner
-Version: 5.0.0
+Version: 6.0.0
 Summary: JupyterHub Spawner for Kubernetes
 Project-URL: Documentation, https://jupyterhub-kubespawner.readthedocs.io
 Project-URL: Source, https://github.com/jupyterhub/kubespawner
 Project-URL: Issues, https://github.com/jupyterhub/kubespawner/issues
 Author-email: Jupyter Contributors <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
@@ -38,19 +38,19 @@
 License-File: LICENSE
 Keywords: jupyterhub,spawner
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: escapism
 Requires-Dist: jinja2
-Requires-Dist: jupyterhub>=1.3.0
-Requires-Dist: kubernetes-asyncio>=23.6.0
+Requires-Dist: jupyterhub>=4.0.0
+Requires-Dist: kubernetes-asyncio>=24.2.3
 Requires-Dist: python-slugify
 Requires-Dist: pyyaml
-Requires-Dist: traitlets>=4.3.2
+Requires-Dist: traitlets
 Requires-Dist: urllib3
 Provides-Extra: test
 Requires-Dist: kubernetes>=11; extra == 'test'
 Requires-Dist: pytest-asyncio>=0.17; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest>=5.4; extra == 'test'
 Description-Content-Type: text/markdown
@@ -58,15 +58,14 @@
 # [kubespawner](https://github.com/jupyterhub/kubespawner) (jupyterhub-kubespawner @ PyPI)
 
 [![Latest PyPI version](https://img.shields.io/pypi/v/jupyterhub-kubespawner?logo=pypi)](https://pypi.python.org/pypi/jupyterhub-kubespawner)
 [![Latest conda-forge version](https://img.shields.io/conda/vn/conda-forge/jupyterhub-kubespawner?logo=conda-forge)](https://anaconda.org/conda-forge/jupyterhub-kubespawner)
 [![Documentation status](https://img.shields.io/readthedocs/jupyterhub-kubespawner?logo=read-the-docs)](https://jupyterhub-kubespawner.readthedocs.io/en/latest/?badge=latest)
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/jupyterhub/kubespawner/test.yaml?logo=github&label=tests)](https://github.com/jupyterhub/kubespawner/actions)
 [![Code coverage](https://codecov.io/gh/jupyterhub/kubespawner/branch/main/graph/badge.svg)](https://codecov.io/gh/jupyterhub/kubespawner)
-[![](https://img.shields.io/pypi/v/jupyterhub-kubespawner.svg?logo=pypi)](https://pypi.python.org/pypi/jupyterhub-kubespawner)
 
 The _kubespawner_ (also known as JupyterHub Kubernetes Spawner) enables JupyterHub to spawn
 single-user notebook servers on a [Kubernetes](https://kubernetes.io/)
 cluster.
 
 See the [KubeSpawner documentation](https://jupyterhub-kubespawner.readthedocs.io) for more
 information about features and usage. In particular, here is [a list of all the spawner options](https://jupyterhub-kubespawner.readthedocs.io/en/latest/spawner.html#module-kubespawner.spawner).
@@ -110,17 +109,21 @@
   [multiple clouds at the same time](https://kubernetes.io/docs/user-guide/federation/).
 
 In general, Kubernetes provides a ton of well thought out, useful features -
 and you can use all of them along with this spawner.
 
 ## Requirements
 
+### JupyterHub
+
+Requires JupyterHub 4.0+
+
 ### Kubernetes
 
-Everything should work from Kubernetes v1.6+.
+Everything should work from Kubernetes v1.24+.
 
 The [Kube DNS addon](https://kubernetes.io/docs/user-guide/connecting-applications/#dns)
 is not strictly required - the spawner uses
 [environment variable](https://kubernetes.io/docs/user-guide/connecting-applications/#environment-variables)
 based discovery instead. Your kubernetes cluster will need to be configured to
 support the types of volumes you want to use.
```

