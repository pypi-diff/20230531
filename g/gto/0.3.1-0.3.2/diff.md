# Comparing `tmp/gto-0.3.1.tar.gz` & `tmp/gto-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gto-0.3.1.tar", last modified: Wed May 24 10:47:07 2023, max compression
+gzip compressed data, was "gto-0.3.2.tar", last modified: Wed May 31 09:42:12 2023, max compression
```

## Comparing `gto-0.3.1.tar` & `gto-0.3.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:47:07.986599 gto-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-24 10:46:54.000000 gto-0.3.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:47:07.962599 gto-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:47:07.970599 gto-0.3.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-24 10:46:54.000000 gto-0.3.1/.github/ISSUE_TEMPLATE/epic-or-story.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:47:07.970599 gto-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-24 10:46:54.000000 gto-0.3.1/.github/workflows/check-test-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-24 10:46:54.000000 gto-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-24 10:46:54.000000 gto-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20057 2023-05-24 10:46:54.000000 gto-0.3.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-24 10:46:54.000000 gto-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-24 10:47:07.986599 gto-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-24 10:46:54.000000 gto-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:47:07.978599 gto-0.3.1/gto/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-24 10:46:54.000000 gto-0.3.1/gto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 10:47:07.000000 gto-0.3.1/gto/_gto_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-24 10:46:54.000000 gto-0.3.1/gto/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-05-24 10:46:54.000000 gto-0.3.1/gto/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-05-24 10:46:54.000000 gto-0.3.1/gto/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    25158 2023-05-24 10:46:54.000000 gto-0.3.1/gto/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-24 10:46:54.000000 gto-0.3.1/gto/commit_message_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-24 10:46:54.000000 gto-0.3.1/gto/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-24 10:46:54.000000 gto-0.3.1/gto/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-24 10:46:54.000000 gto-0.3.1/gto/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-24 10:46:54.000000 gto-0.3.1/gto/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-05-24 10:46:54.000000 gto-0.3.1/gto/git_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-05-24 10:46:54.000000 gto-0.3.1/gto/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-24 10:46:54.000000 gto-0.3.1/gto/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-05-24 10:46:54.000000 gto-0.3.1/gto/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-05-24 10:46:54.000000 gto-0.3.1/gto/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-24 10:46:54.000000 gto-0.3.1/gto/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-24 10:46:54.000000 gto-0.3.1/gto/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-24 10:46:54.000000 gto-0.3.1/gto/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:47:07.978599 gto-0.3.1/gto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-24 10:47:07.000000 gto-0.3.1/gto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-24 10:47:07.000000 gto-0.3.1/gto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 10:47:07.000000 gto-0.3.1/gto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-24 10:47:07.000000 gto-0.3.1/gto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 10:47:07.000000 gto-0.3.1/gto.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-24 10:47:07.000000 gto-0.3.1/gto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-24 10:47:07.000000 gto-0.3.1/gto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-24 10:46:54.000000 gto-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-24 10:46:54.000000 gto-0.3.1/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-24 10:47:07.986599 gto-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-24 10:46:54.000000 gto-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:47:07.986599 gto-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 10:46:54.000000 gto-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-24 10:46:54.000000 gto-0.3.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:47:07.986599 gto-0.3.1/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-24 10:46:54.000000 gto-0.3.1/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-24 10:46:54.000000 gto-0.3.1/tests/resources/sample_remote_repo_expected_history_churn.json
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-24 10:46:54.000000 gto-0.3.1/tests/resources/sample_remote_repo_expected_registry.json
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-24 10:46:54.000000 gto-0.3.1/tests/skip_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    21477 2023-05-24 10:46:54.000000 gto-0.3.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-05-24 10:46:54.000000 gto-0.3.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-24 10:46:54.000000 gto-0.3.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-24 10:46:54.000000 gto-0.3.1/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-05-24 10:46:54.000000 gto-0.3.1/tests/test_git_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-24 10:46:54.000000 gto-0.3.1/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)    19732 2023-05-24 10:46:54.000000 gto-0.3.1/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-24 10:46:54.000000 gto-0.3.1/tests/test_showcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-24 10:46:54.000000 gto-0.3.1/tests/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-24 10:46:54.000000 gto-0.3.1/tests/test_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-24 10:46:54.000000 gto-0.3.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:42:12.420599 gto-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-31 09:41:55.000000 gto-0.3.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:42:12.404599 gto-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:42:12.408599 gto-0.3.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-31 09:41:55.000000 gto-0.3.2/.github/ISSUE_TEMPLATE/epic-or-story.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:42:12.408599 gto-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-31 09:41:55.000000 gto-0.3.2/.github/workflows/check-test-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-31 09:41:55.000000 gto-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-31 09:41:55.000000 gto-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20057 2023-05-31 09:41:55.000000 gto-0.3.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-31 09:41:55.000000 gto-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-31 09:42:12.420599 gto-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-31 09:41:55.000000 gto-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:42:12.412599 gto-0.3.2/gto/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-31 09:41:55.000000 gto-0.3.2/gto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 09:42:12.000000 gto-0.3.2/gto/_gto_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-31 09:41:55.000000 gto-0.3.2/gto/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-05-31 09:41:55.000000 gto-0.3.2/gto/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-05-31 09:41:55.000000 gto-0.3.2/gto/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25182 2023-05-31 09:41:55.000000 gto-0.3.2/gto/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-31 09:41:55.000000 gto-0.3.2/gto/commit_message_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-31 09:41:55.000000 gto-0.3.2/gto/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-31 09:41:55.000000 gto-0.3.2/gto/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-31 09:41:55.000000 gto-0.3.2/gto/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-31 09:41:55.000000 gto-0.3.2/gto/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-05-31 09:41:55.000000 gto-0.3.2/gto/git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-05-31 09:41:55.000000 gto-0.3.2/gto/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-31 09:41:55.000000 gto-0.3.2/gto/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-05-31 09:41:55.000000 gto-0.3.2/gto/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11221 2023-05-31 09:41:55.000000 gto-0.3.2/gto/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-31 09:41:55.000000 gto-0.3.2/gto/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-31 09:41:55.000000 gto-0.3.2/gto/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-31 09:41:55.000000 gto-0.3.2/gto/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:42:12.416599 gto-0.3.2/gto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-31 09:42:12.000000 gto-0.3.2/gto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-31 09:42:12.000000 gto-0.3.2/gto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:42:12.000000 gto-0.3.2/gto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-31 09:42:12.000000 gto-0.3.2/gto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 09:42:12.000000 gto-0.3.2/gto.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-31 09:42:12.000000 gto-0.3.2/gto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 09:42:12.000000 gto-0.3.2/gto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-31 09:41:55.000000 gto-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-31 09:41:55.000000 gto-0.3.2/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-31 09:42:12.420599 gto-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-31 09:41:55.000000 gto-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:42:12.416599 gto-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 09:41:55.000000 gto-0.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-31 09:41:55.000000 gto-0.3.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 09:42:12.420599 gto-0.3.2/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-31 09:41:55.000000 gto-0.3.2/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-31 09:41:55.000000 gto-0.3.2/tests/resources/sample_remote_repo_expected_history_churn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-31 09:41:55.000000 gto-0.3.2/tests/resources/sample_remote_repo_expected_registry.json
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-31 09:41:55.000000 gto-0.3.2/tests/skip_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22113 2023-05-31 09:41:55.000000 gto-0.3.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-05-31 09:41:55.000000 gto-0.3.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-31 09:41:55.000000 gto-0.3.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-31 09:41:55.000000 gto-0.3.2/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-05-31 09:41:55.000000 gto-0.3.2/tests/test_git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-31 09:41:55.000000 gto-0.3.2/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19732 2023-05-31 09:41:55.000000 gto-0.3.2/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-05-31 09:41:55.000000 gto-0.3.2/tests/test_showcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-31 09:41:55.000000 gto-0.3.2/tests/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-31 09:41:55.000000 gto-0.3.2/tests/test_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-31 09:41:55.000000 gto-0.3.2/tests/utils.py
```

### Comparing `gto-0.3.1/.github/ISSUE_TEMPLATE/epic-or-story.md` & `gto-0.3.2/.github/ISSUE_TEMPLATE/epic-or-story.md`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/.github/workflows/check-test-release.yml` & `gto-0.3.2/.github/workflows/check-test-release.yml`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/.gitignore` & `gto-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/.pre-commit-config.yaml` & `gto-0.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/.pylintrc` & `gto-0.3.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/LICENSE` & `gto-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/PKG-INFO` & `gto-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gto
-Version: 0.3.1
+Version: 0.3.2
 Summary: Version and deploy your models following GitOps principles
 Download-URL: https://github.com/iterative/gto
 Author: Alexander Guschin
 Author-email: aguschin@iterative.ai
 License: Apache License 2.0
 Keywords: git repo repository artifact registry developer-tools collaboration
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `gto-0.3.1/README.md` & `gto-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/gto/api.py` & `gto-0.3.2/gto/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     parse_shortcut,
 )
 from gto.exceptions import NoRepo, NotImplementedInGTO, WrongArgs
 from gto.git_utils import is_url_of_remote_repo
 from gto.index import Artifact, FileIndexManager, RepoIndexManager
 from gto.registry import GitRegistry
 from gto.tag import parse_name as parse_tag_name
+from gto.utils import resolve_ref
 
 
 def _is_gto_repo(repo: Union[str, Repo]):
     """Check if repo is a gto repo"""
     try:
         with GitRegistry.from_repo(repo) as reg:
             return reg.is_gto_repo()
@@ -370,61 +371,90 @@
                 + [d["stage"][name] for name in stages],
             ),
         )
         for name, d in sorted(models_state.items())
     ], "keys"
 
 
+def _get_versions(
+    artifact,
+    deprecated,
+    registered_only,
+    assignments_per_version,
+    versions_per_stage,
+    sort,
+):
+    versions = []
+    stages = artifact.get_vstages(
+        registered_only=registered_only,
+        assignments_per_version=assignments_per_version,
+        versions_per_stage=versions_per_stage,
+        sort=sort,
+    )
+    for v in artifact.get_versions(
+        active_only=not deprecated,
+        include_non_explicit=not registered_only,
+        include_discovered=True,
+    ):
+        v = v.dict_state()
+        v["stages"] = [
+            vstage.dict_state()
+            for vstages in stages.values()
+            for vstage in vstages
+            if vstage.version == v["version"]
+        ]
+        if artifact.is_active or deprecated:
+            versions.append(v)
+    return versions
+
+
 def _show_versions(  # pylint: disable=too-many-locals
     repo: Union[str, Repo],
     name: str,
+    ref: Optional[str] = None,
     raw: bool = False,
     registered_only=False,
     deprecated=False,
-    assignments_per_version: int = None,
-    versions_per_stage: int = None,
-    sort: VersionSort = None,
+    assignments_per_version=ASSIGNMENTS_PER_VERSION,
+    versions_per_stage=VERSIONS_PER_STAGE,
+    sort=VersionSort.Timestamp,
     table: bool = False,
     truncate_hexsha: bool = False,
 ):
     """List versions of artifact"""
 
+    if isinstance(repo, str):
+        repo = Repo(repo)
+
     def format_hexsha(hexsha):
         return hexsha[:7] if truncate_hexsha and is_hexsha(hexsha) else hexsha
 
     shortcut = parse_shortcut(name)
+    if shortcut.shortcut and ref:
+        raise WrongArgs("Cannot specify both shortcut and ref")
 
     with GitRegistry.from_repo(repo=repo) as reg:
         if raw:
             return reg.find_artifact(shortcut.name).versions
 
         artifact = reg.find_artifact(shortcut.name)
-    stages = artifact.get_vstages(
-        registered_only=registered_only,
-        assignments_per_version=assignments_per_version,
-        versions_per_stage=versions_per_stage,
-        sort=sort,
+
+    versions = _get_versions(
+        artifact,
+        deprecated,
+        registered_only,
+        assignments_per_version,
+        versions_per_stage,
+        sort,
     )
-    versions = []
-    for v in artifact.get_versions(
-        active_only=not deprecated,
-        include_non_explicit=not registered_only,
-        include_discovered=True,
-    ):
-        v = v.dict_state()
-        v["stages"] = [
-            vstage.dict_state()
-            for vstages in stages.values()
-            for vstage in vstages
-            if vstage.version == v["version"]
-        ]
-        if artifact.is_active or deprecated:
-            versions.append(v)
+    if ref:
+        ref_hexsha = resolve_ref(repo, ref).hexsha
+        versions = [v for v in versions if v["commit_hexsha"] == ref_hexsha]
 
-    if shortcut.latest:
+    elif shortcut.latest:
         versions = versions[:1]
     elif shortcut.version:
         versions = [v for v in versions if shortcut.version == v["version"]]
     elif shortcut.stage:
         versions = [
             v for v in versions for a in v["stages"] if shortcut.stage == a["stage"]
         ]
```

### Comparing `gto-0.3.1/gto/base.py` & `gto-0.3.2/gto/base.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/gto/cli.py` & `gto-0.3.2/gto/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,15 +371,15 @@
     help="Print output in table format",
     show_default=True,
 )
 option_push_tag = Option(
     False,
     "--push",
     is_flag=True,
-    help="Push created tag automatically (experimental)",
+    help="Push created git tag to `origin` (done automatically for remote repo)",
 )
 option_commit = Option(
     False,
     "--commit",
     is_flag=True,
     help="Automatically commit changes due to this command (experimental)",
 )
```

### Comparing `gto-0.3.1/gto/config.py` & `gto-0.3.2/gto/config.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/gto/constants.py` & `gto-0.3.2/gto/constants.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/gto/exceptions.py` & `gto-0.3.2/gto/exceptions.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/gto/ext.py` & `gto-0.3.2/gto/ext.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/gto/git_utils.py` & `gto-0.3.2/gto/git_utils.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/gto/index.py` & `gto-0.3.2/gto/index.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/gto/log.py` & `gto-0.3.2/gto/log.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/gto/registry.py` & `gto-0.3.2/gto/registry.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/gto/tag.py` & `gto-0.3.2/gto/tag.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/gto/ui.py` & `gto-0.3.2/gto/ui.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/gto/utils.py` & `gto-0.3.2/gto/utils.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/gto/versions.py` & `gto-0.3.2/gto/versions.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/gto.egg-info/PKG-INFO` & `gto-0.3.2/gto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gto
-Version: 0.3.1
+Version: 0.3.2
 Summary: Version and deploy your models following GitOps principles
 Download-URL: https://github.com/iterative/gto
 Author: Alexander Guschin
 Author-email: aguschin@iterative.ai
 License: Apache License 2.0
 Keywords: git repo repository artifact registry developer-tools collaboration
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `gto-0.3.1/gto.egg-info/SOURCES.txt` & `gto-0.3.2/gto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/setup.cfg` & `gto-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/setup.py` & `gto-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/tests/conftest.py` & `gto-0.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/tests/resources/__init__.py` & `gto-0.3.2/tests/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/tests/resources/sample_remote_repo_expected_history_churn.json` & `gto-0.3.2/tests/resources/sample_remote_repo_expected_history_churn.json`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/tests/resources/sample_remote_repo_expected_registry.json` & `gto-0.3.2/tests/resources/sample_remote_repo_expected_registry.json`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/tests/skip_presets.py` & `gto-0.3.2/tests/skip_presets.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/tests/test_api.py` & `gto-0.3.2/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import git
 import pytest
 from freezegun import freeze_time
 
 import gto
 import tests.resources
 from gto.api import show
-from gto.exceptions import WrongArgs
+from gto.exceptions import RefNotFound, WrongArgs
 from gto.index import RepoIndexManager
 from gto.tag import find
 from gto.versions import SemVer
 from tests.skip_presets import skip_for_windows
 from tests.utils import (
     check_obj,
     convert_objects_to_str_in_json_serializable_object,
@@ -118,20 +118,39 @@
     assert latest.version == vname2
     assert latest.message == message
     assert latest.author == author
     assert latest.author_email == author_email
 
     assert len(gto.api.show(repo.working_dir, name, deprecated=False)) == 2
 
+    # test _show_versions
+    assert (
+        gto.api._show_versions(repo.working_dir, name, ref="HEAD")[0]["ref"]
+        == f"{name}@v1.0.1"
+    )
+    assert (
+        gto.api._show_versions(repo.working_dir, name, ref="HEAD^1")[0]["ref"]
+        == f"{name}@v1.0.0"
+    )
+    assert (
+        gto.api._show_versions(repo.working_dir, name, ref=repo.commit().hexsha)[0][
+            "ref"
+        ]
+        == f"{name}@v1.0.1"
+    )
+    with pytest.raises(RefNotFound):
+        gto.api._show_versions(repo.working_dir, name, ref="HEAD^2")
+
     gto.api.deregister(repo=repo.working_dir, name=name, version=vname2)
     latest = gto.api.find_latest_version(repo.working_dir, name)
     assert latest.version == vname1
 
     assert len(gto.api.show(repo.working_dir, name, deprecated=False)) == 1
     assert len(gto.api.show(repo.working_dir, name, deprecated=True)) == 2
+    assert len(gto.api._show_versions(repo.working_dir, name, ref="HEAD")) == 0
 
 
 def test_assign(repo_with_artifact: Tuple[git.Repo, str]):
     repo, name = repo_with_artifact
     stage = "staging"
     repo.create_tag("v1.0.0")
     repo.create_tag("wrong-tag-unrelated")
```

### Comparing `gto-0.3.1/tests/test_cli.py` & `gto-0.3.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/tests/test_config.py` & `gto-0.3.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/tests/test_constants.py` & `gto-0.3.2/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/tests/test_git_utils.py` & `gto-0.3.2/tests/test_git_utils.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/tests/test_index.py` & `gto-0.3.2/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/tests/test_registry.py` & `gto-0.3.2/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/tests/test_showcase.py` & `gto-0.3.2/tests/test_showcase.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/tests/test_tag.py` & `gto-0.3.2/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/tests/test_versions.py` & `gto-0.3.2/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `gto-0.3.1/tests/utils.py` & `gto-0.3.2/tests/utils.py`

 * *Files identical despite different names*

