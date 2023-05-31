# Comparing `tmp/rlstack-0.0.0b1.tar.gz` & `tmp/rlstack-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlstack-0.0.0b1.tar", last modified: Mon May 22 21:35:59 2023, max compression
+gzip compressed data, was "rlstack-0.1.0.tar", last modified: Wed May 31 21:48:08 2023, max compression
```

## Comparing `rlstack-0.0.0b1.tar` & `rlstack-0.1.0.tar`

### file list

```diff
@@ -1,76 +1,86 @@
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-22 21:35:59.500000 rlstack-0.0.0b1/
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-22 21:35:59.490000 rlstack-0.0.0b1/.github/
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-22 21:35:59.490000 rlstack-0.0.0b1/.github/workflows/
--rw-r--r--   0 berger    (1000) berger    (1000)      916 2023-04-26 21:08:56.000000 rlstack-0.0.0b1/.github/workflows/build-docs.yml
--rw-r--r--   0 berger    (1000) berger    (1000)      745 2023-04-26 21:09:13.000000 rlstack-0.0.0b1/.github/workflows/test-and-publish.yml
--rw-r--r--   0 berger    (1000) berger    (1000)      551 2023-04-26 21:10:03.000000 rlstack-0.0.0b1/.github/workflows/test.yml
--rw-r--r--   0 berger    (1000) berger    (1000)     1887 2023-04-28 20:49:45.000000 rlstack-0.0.0b1/.gitignore
--rw-r--r--   0 berger    (1000) berger    (1000)      694 2023-05-03 00:17:18.000000 rlstack-0.0.0b1/.pre-commit-config.yaml
--rw-r--r--   0 berger    (1000) berger    (1000)    11357 2023-02-10 22:26:37.000000 rlstack-0.0.0b1/LICENSE
--rw-r--r--   0 berger    (1000) berger    (1000)    25250 2023-05-22 21:35:59.500000 rlstack-0.0.0b1/PKG-INFO
--rw-r--r--   0 berger    (1000) berger    (1000)    11488 2023-05-22 21:28:40.000000 rlstack-0.0.0b1/README.rst
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-22 21:35:59.490000 rlstack-0.0.0b1/docs/
--rw-r--r--   0 berger    (1000) berger    (1000)        0 2023-04-26 22:09:05.000000 rlstack-0.0.0b1/docs/.nojekyll
--rw-r--r--   0 berger    (1000) berger    (1000)      635 2023-04-26 22:09:05.000000 rlstack-0.0.0b1/docs/Makefile
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-22 21:35:59.490000 rlstack-0.0.0b1/docs/_static/
--rw-r--r--   0 berger    (1000) berger    (1000)      480 2023-04-26 22:09:05.000000 rlstack-0.0.0b1/docs/_static/custom.css
--rw-r--r--   0 berger    (1000) berger    (1000)     4234 2023-05-04 01:02:37.000000 rlstack-0.0.0b1/docs/conf.py
--rw-r--r--   0 berger    (1000) berger    (1000)       71 2023-04-26 22:09:05.000000 rlstack-0.0.0b1/docs/index.html
--rw-r--r--   0 berger    (1000) berger    (1000)      188 2023-05-04 20:56:47.000000 rlstack-0.0.0b1/docs/index.rst
--rw-r--r--   0 berger    (1000) berger    (1000)      799 2023-04-26 22:09:05.000000 rlstack-0.0.0b1/docs/make.bat
--rw-r--r--   0 berger    (1000) berger    (1000)       75 2023-04-30 23:31:03.000000 rlstack-0.0.0b1/docs/requirements.txt
--rw-r--r--   0 berger    (1000) berger    (1000)     3760 2023-05-22 21:08:08.000000 rlstack-0.0.0b1/pyproject.toml
--rw-r--r--   0 berger    (1000) berger    (1000)       38 2023-05-22 21:35:59.500000 rlstack-0.0.0b1/setup.cfg
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-22 21:35:59.490000 rlstack-0.0.0b1/src/
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-22 21:35:59.500000 rlstack-0.0.0b1/src/rlstack/
--rw-r--r--   0 berger    (1000) berger    (1000)      644 2023-05-15 21:11:00.000000 rlstack-0.0.0b1/src/rlstack/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)     3826 2023-05-19 02:41:20.000000 rlstack-0.0.0b1/src/rlstack/_utils.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-22 21:35:59.500000 rlstack-0.0.0b1/src/rlstack/algorithms/
--rw-r--r--   0 berger    (1000) berger    (1000)      834 2023-05-15 21:16:46.000000 rlstack-0.0.0b1/src/rlstack/algorithms/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)    27307 2023-05-22 21:09:46.000000 rlstack-0.0.0b1/src/rlstack/algorithms/_feedforward.py
--rw-r--r--   0 berger    (1000) berger    (1000)    29522 2023-05-22 21:09:52.000000 rlstack-0.0.0b1/src/rlstack/algorithms/_recurrent.py
--rw-r--r--   0 berger    (1000) berger    (1000)     4415 2023-05-21 00:35:52.000000 rlstack-0.0.0b1/src/rlstack/conditions.py
--rw-r--r--   0 berger    (1000) berger    (1000)    13633 2023-05-19 02:41:20.000000 rlstack-0.0.0b1/src/rlstack/data.py
--rw-r--r--   0 berger    (1000) berger    (1000)     8491 2023-05-15 21:11:00.000000 rlstack-0.0.0b1/src/rlstack/distributions.py
--rw-r--r--   0 berger    (1000) berger    (1000)     6241 2023-05-18 21:24:54.000000 rlstack-0.0.0b1/src/rlstack/env.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-22 21:35:59.500000 rlstack-0.0.0b1/src/rlstack/models/
--rw-r--r--   0 berger    (1000) berger    (1000)     1126 2023-05-15 21:11:00.000000 rlstack-0.0.0b1/src/rlstack/models/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)    14832 2023-05-22 02:48:58.000000 rlstack-0.0.0b1/src/rlstack/models/_feedforward.py
--rw-r--r--   0 berger    (1000) berger    (1000)    13733 2023-05-15 21:11:00.000000 rlstack-0.0.0b1/src/rlstack/models/_recurrent.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-22 21:35:59.500000 rlstack-0.0.0b1/src/rlstack/nn/
--rw-r--r--   0 berger    (1000) berger    (1000)      568 2023-05-17 21:40:38.000000 rlstack-0.0.0b1/src/rlstack/nn/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)    13184 2023-05-22 21:34:03.000000 rlstack-0.0.0b1/src/rlstack/nn/functional.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-22 21:35:59.500000 rlstack-0.0.0b1/src/rlstack/nn/modules/
--rw-r--r--   0 berger    (1000) berger    (1000)      348 2023-02-08 23:39:43.000000 rlstack-0.0.0b1/src/rlstack/nn/modules/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)     1061 2023-05-02 01:12:30.000000 rlstack-0.0.0b1/src/rlstack/nn/modules/activations.py
--rw-r--r--   0 berger    (1000) berger    (1000)    12168 2023-05-08 01:27:24.000000 rlstack-0.0.0b1/src/rlstack/nn/modules/attention.py
--rw-r--r--   0 berger    (1000) berger    (1000)     1740 2023-05-02 00:38:37.000000 rlstack-0.0.0b1/src/rlstack/nn/modules/embeddings.py
--rw-r--r--   0 berger    (1000) berger    (1000)     1749 2023-02-09 01:31:09.000000 rlstack-0.0.0b1/src/rlstack/nn/modules/mlp.py
--rw-r--r--   0 berger    (1000) berger    (1000)      586 2023-05-04 01:01:58.000000 rlstack-0.0.0b1/src/rlstack/nn/modules/module.py
--rw-r--r--   0 berger    (1000) berger    (1000)     8230 2023-05-08 01:55:09.000000 rlstack-0.0.0b1/src/rlstack/nn/modules/perceiver.py
--rw-r--r--   0 berger    (1000) berger    (1000)     4565 2023-05-02 00:41:33.000000 rlstack-0.0.0b1/src/rlstack/nn/modules/skip.py
--rw-r--r--   0 berger    (1000) berger    (1000)     2791 2023-05-21 20:55:43.000000 rlstack-0.0.0b1/src/rlstack/optimizer.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-22 21:35:59.500000 rlstack-0.0.0b1/src/rlstack/policies/
--rw-r--r--   0 berger    (1000) berger    (1000)      509 2023-05-15 21:17:42.000000 rlstack-0.0.0b1/src/rlstack/policies/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)     8011 2023-05-17 21:01:42.000000 rlstack-0.0.0b1/src/rlstack/policies/_feedforward.py
--rw-r--r--   0 berger    (1000) berger    (1000)     8212 2023-05-17 21:01:42.000000 rlstack-0.0.0b1/src/rlstack/policies/_recurrent.py
--rw-r--r--   0 berger    (1000) berger    (1000)     7532 2023-05-21 15:13:57.000000 rlstack-0.0.0b1/src/rlstack/schedulers.py
--rw-r--r--   0 berger    (1000) berger    (1000)    72012 2023-05-03 00:17:58.000000 rlstack-0.0.0b1/src/rlstack/specs.py
--rw-r--r--   0 berger    (1000) berger    (1000)     4123 2023-05-19 01:58:05.000000 rlstack-0.0.0b1/src/rlstack/trainer.py
--rw-r--r--   0 berger    (1000) berger    (1000)    18447 2023-05-15 21:11:00.000000 rlstack-0.0.0b1/src/rlstack/views.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-22 21:35:59.500000 rlstack-0.0.0b1/src/rlstack.egg-info/
--rw-r--r--   0 berger    (1000) berger    (1000)    25250 2023-05-22 21:35:59.000000 rlstack-0.0.0b1/src/rlstack.egg-info/PKG-INFO
--rw-r--r--   0 berger    (1000) berger    (1000)     1572 2023-05-22 21:35:59.000000 rlstack-0.0.0b1/src/rlstack.egg-info/SOURCES.txt
--rw-r--r--   0 berger    (1000) berger    (1000)        1 2023-05-22 21:35:59.000000 rlstack-0.0.0b1/src/rlstack.egg-info/dependency_links.txt
--rw-r--r--   0 berger    (1000) berger    (1000)      159 2023-05-22 21:35:59.000000 rlstack-0.0.0b1/src/rlstack.egg-info/requires.txt
--rw-r--r--   0 berger    (1000) berger    (1000)        8 2023-05-22 21:35:59.000000 rlstack-0.0.0b1/src/rlstack.egg-info/top_level.txt
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-22 21:35:59.500000 rlstack-0.0.0b1/tests/
--rw-r--r--   0 berger    (1000) berger    (1000)        0 2023-02-10 22:22:48.000000 rlstack-0.0.0b1/tests/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)     1751 2023-05-21 20:54:04.000000 rlstack-0.0.0b1/tests/test_algorithms.py
--rw-r--r--   0 berger    (1000) berger    (1000)     1033 2023-05-21 00:35:52.000000 rlstack-0.0.0b1/tests/test_conditions.py
-drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-22 21:35:59.500000 rlstack-0.0.0b1/tests/test_nn/
--rw-r--r--   0 berger    (1000) berger    (1000)        0 2023-05-21 00:35:52.000000 rlstack-0.0.0b1/tests/test_nn/__init__.py
--rw-r--r--   0 berger    (1000) berger    (1000)     2536 2023-05-21 14:55:57.000000 rlstack-0.0.0b1/tests/test_nn/test_functional.py
--rw-r--r--   0 berger    (1000) berger    (1000)     3124 2023-05-21 00:35:52.000000 rlstack-0.0.0b1/tests/test_policies.py
--rw-r--r--   0 berger    (1000) berger    (1000)     1402 2023-05-21 00:35:52.000000 rlstack-0.0.0b1/tests/test_schedulers.py
--rw-r--r--   0 berger    (1000) berger    (1000)     9988 2023-05-15 21:11:00.000000 rlstack-0.0.0b1/tests/test_views.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.500000 rlstack-0.1.0/
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.480000 rlstack-0.1.0/.github/
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/.github/workflows/
+-rw-r--r--   0 berger    (1000) berger    (1000)      916 2023-04-26 21:08:56.000000 rlstack-0.1.0/.github/workflows/build-docs.yml
+-rw-r--r--   0 berger    (1000) berger    (1000)      745 2023-04-26 21:09:13.000000 rlstack-0.1.0/.github/workflows/test-and-publish.yml
+-rw-r--r--   0 berger    (1000) berger    (1000)      551 2023-04-26 21:10:03.000000 rlstack-0.1.0/.github/workflows/test.yml
+-rw-r--r--   0 berger    (1000) berger    (1000)     1887 2023-04-28 20:49:45.000000 rlstack-0.1.0/.gitignore
+-rw-r--r--   0 berger    (1000) berger    (1000)      694 2023-05-03 00:17:18.000000 rlstack-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 berger    (1000) berger    (1000)    11357 2023-02-10 22:26:37.000000 rlstack-0.1.0/LICENSE
+-rw-r--r--   0 berger    (1000) berger    (1000)    25248 2023-05-31 21:48:08.500000 rlstack-0.1.0/PKG-INFO
+-rw-r--r--   0 berger    (1000) berger    (1000)    11488 2023-05-31 21:17:24.000000 rlstack-0.1.0/README.rst
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/docs/
+-rw-r--r--   0 berger    (1000) berger    (1000)        0 2023-04-26 22:09:05.000000 rlstack-0.1.0/docs/.nojekyll
+-rw-r--r--   0 berger    (1000) berger    (1000)      635 2023-04-26 22:09:05.000000 rlstack-0.1.0/docs/Makefile
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/docs/_static/
+-rw-r--r--   0 berger    (1000) berger    (1000)      480 2023-04-26 22:09:05.000000 rlstack-0.1.0/docs/_static/custom.css
+-rw-r--r--   0 berger    (1000) berger    (1000)     4234 2023-05-04 01:02:37.000000 rlstack-0.1.0/docs/conf.py
+-rw-r--r--   0 berger    (1000) berger    (1000)       71 2023-04-26 22:09:05.000000 rlstack-0.1.0/docs/index.html
+-rw-r--r--   0 berger    (1000) berger    (1000)      188 2023-05-04 20:56:47.000000 rlstack-0.1.0/docs/index.rst
+-rw-r--r--   0 berger    (1000) berger    (1000)      799 2023-04-26 22:09:05.000000 rlstack-0.1.0/docs/make.bat
+-rw-r--r--   0 berger    (1000) berger    (1000)       75 2023-04-30 23:31:03.000000 rlstack-0.1.0/docs/requirements.txt
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.480000 rlstack-0.1.0/examples/
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/examples/algotrading/
+-rw-r--r--   0 berger    (1000) berger    (1000)     2134 2023-05-31 21:17:24.000000 rlstack-0.1.0/examples/algotrading/README.rst
+-rw-r--r--   0 berger    (1000) berger    (1000)     1705 2023-05-31 21:17:24.000000 rlstack-0.1.0/examples/algotrading/__main__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     7276 2023-05-31 21:17:24.000000 rlstack-0.1.0/examples/algotrading/env.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/examples/algotrading/models/
+-rw-r--r--   0 berger    (1000) berger    (1000)      102 2023-05-31 21:17:24.000000 rlstack-0.1.0/examples/algotrading/models/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     3955 2023-05-31 21:42:40.000000 rlstack-0.1.0/examples/algotrading/models/lstm.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     4874 2023-05-31 21:17:24.000000 rlstack-0.1.0/examples/algotrading/models/mlp.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     5613 2023-05-31 21:35:47.000000 rlstack-0.1.0/examples/algotrading/models/transformer.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     3776 2023-05-31 21:17:24.000000 rlstack-0.1.0/pyproject.toml
+-rw-r--r--   0 berger    (1000) berger    (1000)       38 2023-05-31 21:48:08.500000 rlstack-0.1.0/setup.cfg
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.480000 rlstack-0.1.0/src/
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/src/rlstack/
+-rw-r--r--   0 berger    (1000) berger    (1000)      644 2023-05-15 21:11:00.000000 rlstack-0.1.0/src/rlstack/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     4685 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/_utils.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/src/rlstack/algorithms/
+-rw-r--r--   0 berger    (1000) berger    (1000)      834 2023-05-15 21:16:46.000000 rlstack-0.1.0/src/rlstack/algorithms/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    27138 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/algorithms/_feedforward.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    29353 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/algorithms/_recurrent.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     4415 2023-05-21 00:35:52.000000 rlstack-0.1.0/src/rlstack/conditions.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    13633 2023-05-19 02:41:20.000000 rlstack-0.1.0/src/rlstack/data.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     6021 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/distributions.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     6629 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/env.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/src/rlstack/models/
+-rw-r--r--   0 berger    (1000) berger    (1000)     1126 2023-05-15 21:11:00.000000 rlstack-0.1.0/src/rlstack/models/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    14331 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/models/_feedforward.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    13255 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/models/_recurrent.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/src/rlstack/nn/
+-rw-r--r--   0 berger    (1000) berger    (1000)      568 2023-05-17 21:40:38.000000 rlstack-0.1.0/src/rlstack/nn/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    13184 2023-05-22 21:34:03.000000 rlstack-0.1.0/src/rlstack/nn/functional.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/src/rlstack/nn/modules/
+-rw-r--r--   0 berger    (1000) berger    (1000)      348 2023-02-08 23:39:43.000000 rlstack-0.1.0/src/rlstack/nn/modules/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     1061 2023-05-02 01:12:30.000000 rlstack-0.1.0/src/rlstack/nn/modules/activations.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    12068 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/nn/modules/attention.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     1740 2023-05-02 00:38:37.000000 rlstack-0.1.0/src/rlstack/nn/modules/embeddings.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     1749 2023-02-09 01:31:09.000000 rlstack-0.1.0/src/rlstack/nn/modules/mlp.py
+-rw-r--r--   0 berger    (1000) berger    (1000)      586 2023-05-04 01:01:58.000000 rlstack-0.1.0/src/rlstack/nn/modules/module.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     8138 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/nn/modules/perceiver.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     4601 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/nn/modules/skip.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     2791 2023-05-21 20:55:43.000000 rlstack-0.1.0/src/rlstack/optimizer.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/src/rlstack/policies/
+-rw-r--r--   0 berger    (1000) berger    (1000)      509 2023-05-15 21:17:42.000000 rlstack-0.1.0/src/rlstack/policies/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     8036 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/policies/_feedforward.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     8237 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/policies/_recurrent.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     7532 2023-05-21 15:13:57.000000 rlstack-0.1.0/src/rlstack/schedulers.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    72012 2023-05-03 00:17:58.000000 rlstack-0.1.0/src/rlstack/specs.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     4120 2023-05-22 22:09:36.000000 rlstack-0.1.0/src/rlstack/trainer.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    18782 2023-05-31 21:17:24.000000 rlstack-0.1.0/src/rlstack/views.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/src/rlstack.egg-info/
+-rw-r--r--   0 berger    (1000) berger    (1000)    25248 2023-05-31 21:48:08.000000 rlstack-0.1.0/src/rlstack.egg-info/PKG-INFO
+-rw-r--r--   0 berger    (1000) berger    (1000)     1819 2023-05-31 21:48:08.000000 rlstack-0.1.0/src/rlstack.egg-info/SOURCES.txt
+-rw-r--r--   0 berger    (1000) berger    (1000)        1 2023-05-31 21:48:08.000000 rlstack-0.1.0/src/rlstack.egg-info/dependency_links.txt
+-rw-r--r--   0 berger    (1000) berger    (1000)      159 2023-05-31 21:48:08.000000 rlstack-0.1.0/src/rlstack.egg-info/requires.txt
+-rw-r--r--   0 berger    (1000) berger    (1000)        8 2023-05-31 21:48:08.000000 rlstack-0.1.0/src/rlstack.egg-info/top_level.txt
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/tests/
+-rw-r--r--   0 berger    (1000) berger    (1000)        0 2023-02-10 22:22:48.000000 rlstack-0.1.0/tests/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     1751 2023-05-21 20:54:04.000000 rlstack-0.1.0/tests/test_algorithms.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     1033 2023-05-21 00:35:52.000000 rlstack-0.1.0/tests/test_conditions.py
+drwxr-xr-x   0 berger    (1000) berger    (1000)        0 2023-05-31 21:48:08.490000 rlstack-0.1.0/tests/test_nn/
+-rw-r--r--   0 berger    (1000) berger    (1000)        0 2023-05-21 00:35:52.000000 rlstack-0.1.0/tests/test_nn/__init__.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     2536 2023-05-21 14:55:57.000000 rlstack-0.1.0/tests/test_nn/test_functional.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     3124 2023-05-21 00:35:52.000000 rlstack-0.1.0/tests/test_policies.py
+-rw-r--r--   0 berger    (1000) berger    (1000)     1402 2023-05-21 00:35:52.000000 rlstack-0.1.0/tests/test_schedulers.py
+-rw-r--r--   0 berger    (1000) berger    (1000)    12184 2023-05-31 21:17:24.000000 rlstack-0.1.0/tests/test_views.py
```

### Comparing `rlstack-0.0.0b1/.github/workflows/build-docs.yml` & `rlstack-0.1.0/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/.github/workflows/test-and-publish.yml` & `rlstack-0.1.0/.github/workflows/test-and-publish.yml`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/.github/workflows/test.yml` & `rlstack-0.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/.gitignore` & `rlstack-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/.pre-commit-config.yaml` & `rlstack-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/LICENSE` & `rlstack-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/PKG-INFO` & `rlstack-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlstack
-Version: 0.0.0b1
+Version: 0.1.0
 Summary: A minimal RL library for infinite horizon tasks.
 Author: Andrew B.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -275,66 +275,14 @@
 
     from rlstack import Trainer
     from rlstack.env import DiscreteDummyEnv
 
     trainer = Trainer(DiscreteDummyEnv)
     trainer.run()
 
-Why rlstack?
-============
-
-**TL;DR: rlstack focuses on a niche subset of RL that simplifies the overall
-library while allowing fast and fully customizable environments, models, and
-action distributions.**
-
-There are many high quality, open-sourced RL libraries. Most of them take on the
-daunting task of being a monolithic, one-stop-shop for everything RL, attempting to
-support as many algorithms, environments, models, and compute capabilities as possible.
-Naturely, this monolothic goal has some drawbacks:
-
-* The software becomes more dense with each supported feature, making the library
-  all-the-more difficult to customize for a specific use case.
-* The software becomes less performant for a specific use case. RL practitioners
-  typically end up accepting the cost of transitioning to expensive and
-  difficult-to-manage compute clusters to get results faster.
-
-There's a handful of high quality, open-sourced RL libraries that tradeoff feature
-richness to reduce these drawbacks. However, each library still doesn't provide
-enough speed benefit to warrant the switch from a monolithic repo, or is still
-too complex to adapt to a specific use case.
-
-**rlstack** is a niche RL library that finds a goldilocks zone between the
-feature support and speed/complexity tradeoff by making some key assumptions:
-
-* Environments are highly parallelized and their parallelization is entirely
-  managed within the environment. This allows **rlstack** to ignore distributed
-  computing design considerations.
-* Environments are infinite horizon (i.e., they have no terminal conditions).
-  This allows **rlstack** to reset environments at the same, fixed horizon
-  intervals, greatly simplifying environment and algorithm implementations.
-* The only supported ML framework is PyTorch and the only supported algorithm
-  is PPO. This allows **rlstack** to ignore layers upon layers of abstraction,
-  greatly simplifying the overall library implementation.
-
-The end result is a minimal and high throughput library that can train policies
-to solve complex tasks on a single NVIDIA RTX 2080 within minutes.
-
-Unfortunately, this means **rlstack** doesn't support as many use cases as
-a monolithic RL library might. In fact, **rlstack** is probably a bad fit for
-your use case if:
-
-* Your environment isn't parallelizable.
-* Your environment must contain terminal conditions and can't be reformulated
-  as an infinite horizon task.
-* You want to use an ML framework that isn't PyTorch or you want to use an
-  algorithm that isn't a variant of PPO.
-
-However, if **rlstack** does fit your use case, it can do wonders for your
-RL workflow.
-
 Concepts
 ========
 
 **rlstack** is minimal in that it limits the number of interfaces required for
 training a policy with PPO, even for customized policies, without restrictions
 on observation and action specs, custom models, and custom action
 distributions.
@@ -519,14 +467,66 @@
 
     trainer = Trainer(
         DiscreteDummyEnv,
         stop_conditions=[Plateaus("returns/mean", rtol=0.05)],
     )
     trainer.run()
 
+Why rlstack?
+============
+
+**TL;DR: rlstack focuses on a niche subset of RL that simplifies the overall
+library while allowing fast and fully customizable environments, models, and
+action distributions.**
+
+There are many high quality, open-sourced RL libraries. Most of them take on the
+daunting task of being a monolithic, one-stop-shop for everything RL, attempting to
+support as many algorithms, environments, models, and compute capabilities as possible.
+Naturely, this monolothic goal has some drawbacks:
+
+* The software becomes more dense with each supported feature, making the library
+  all-the-more difficult to customize for a specific use case.
+* The software becomes less performant for a specific use case. RL practitioners
+  typically end up accepting the cost of transitioning to expensive and
+  difficult-to-manage compute clusters to get results faster.
+
+There's a handful of high quality, open-sourced RL libraries that tradeoff feature
+richness to reduce these drawbacks. However, each library still doesn't provide
+enough speed benefit to warrant the switch from a monolithic repo, or is still
+too complex to adapt to a specific use case.
+
+**rlstack** is a niche RL library that finds a goldilocks zone between the
+feature support and speed/complexity tradeoff by making some key assumptions:
+
+* Environments are highly parallelized and their parallelization is entirely
+  managed within the environment. This allows **rlstack** to ignore distributed
+  computing design considerations.
+* Environments are infinite horizon (i.e., they have no terminal conditions).
+  This allows **rlstack** to reset environments at the same, fixed horizon
+  intervals, greatly simplifying environment and algorithm implementations.
+* The only supported ML framework is PyTorch and the only supported algorithm
+  is PPO. This allows **rlstack** to ignore layers upon layers of abstraction,
+  greatly simplifying the overall library implementation.
+
+The end result is a minimal and high throughput library that can train policies
+to solve complex tasks on a single NVIDIA RTX 2080 within minutes.
+
+Unfortunately, this means **rlstack** doesn't support as many use cases as
+a monolithic RL library might. In fact, **rlstack** is probably a bad fit for
+your use case if:
+
+* Your environment isn't parallelizable.
+* Your environment must contain terminal conditions and can't be reformulated
+  as an infinite horizon task.
+* You want to use an ML framework that isn't PyTorch or you want to use an
+  algorithm that isn't a variant of PPO.
+
+However, if **rlstack** does fit your use case, it can do wonders for your
+RL workflow.
+
 Related Projects
 ================
 
 * `RL Games`_: RL Games is a high performance RL library built around popular
   environment protocols.
 * `RLlib`_: Ray's RLlib is the industry standard RL library that supports many
   popular RL algorithms. RLlib can scale RL workloads from your laptop all the
```

### Comparing `rlstack-0.0.0b1/README.rst` & `rlstack-0.1.0/README.rst`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -51,66 +51,14 @@
 
     from rlstack import Trainer
     from rlstack.env import DiscreteDummyEnv
 
     trainer = Trainer(DiscreteDummyEnv)
     trainer.run()
 
-Why rlstack?
-============
-
-**TL;DR: rlstack focuses on a niche subset of RL that simplifies the overall
-library while allowing fast and fully customizable environments, models, and
-action distributions.**
-
-There are many high quality, open-sourced RL libraries. Most of them take on the
-daunting task of being a monolithic, one-stop-shop for everything RL, attempting to
-support as many algorithms, environments, models, and compute capabilities as possible.
-Naturely, this monolothic goal has some drawbacks:
-
-* The software becomes more dense with each supported feature, making the library
-  all-the-more difficult to customize for a specific use case.
-* The software becomes less performant for a specific use case. RL practitioners
-  typically end up accepting the cost of transitioning to expensive and
-  difficult-to-manage compute clusters to get results faster.
-
-There's a handful of high quality, open-sourced RL libraries that tradeoff feature
-richness to reduce these drawbacks. However, each library still doesn't provide
-enough speed benefit to warrant the switch from a monolithic repo, or is still
-too complex to adapt to a specific use case.
-
-**rlstack** is a niche RL library that finds a goldilocks zone between the
-feature support and speed/complexity tradeoff by making some key assumptions:
-
-* Environments are highly parallelized and their parallelization is entirely
-  managed within the environment. This allows **rlstack** to ignore distributed
-  computing design considerations.
-* Environments are infinite horizon (i.e., they have no terminal conditions).
-  This allows **rlstack** to reset environments at the same, fixed horizon
-  intervals, greatly simplifying environment and algorithm implementations.
-* The only supported ML framework is PyTorch and the only supported algorithm
-  is PPO. This allows **rlstack** to ignore layers upon layers of abstraction,
-  greatly simplifying the overall library implementation.
-
-The end result is a minimal and high throughput library that can train policies
-to solve complex tasks on a single NVIDIA RTX 2080 within minutes.
-
-Unfortunately, this means **rlstack** doesn't support as many use cases as
-a monolithic RL library might. In fact, **rlstack** is probably a bad fit for
-your use case if:
-
-* Your environment isn't parallelizable.
-* Your environment must contain terminal conditions and can't be reformulated
-  as an infinite horizon task.
-* You want to use an ML framework that isn't PyTorch or you want to use an
-  algorithm that isn't a variant of PPO.
-
-However, if **rlstack** does fit your use case, it can do wonders for your
-RL workflow.
-
 Concepts
 ========
 
 **rlstack** is minimal in that it limits the number of interfaces required for
 training a policy with PPO, even for customized policies, without restrictions
 on observation and action specs, custom models, and custom action
 distributions.
@@ -295,14 +243,66 @@
 
     trainer = Trainer(
         DiscreteDummyEnv,
         stop_conditions=[Plateaus("returns/mean", rtol=0.05)],
     )
     trainer.run()
 
+Why rlstack?
+============
+
+**TL;DR: rlstack focuses on a niche subset of RL that simplifies the overall
+library while allowing fast and fully customizable environments, models, and
+action distributions.**
+
+There are many high quality, open-sourced RL libraries. Most of them take on the
+daunting task of being a monolithic, one-stop-shop for everything RL, attempting to
+support as many algorithms, environments, models, and compute capabilities as possible.
+Naturely, this monolothic goal has some drawbacks:
+
+* The software becomes more dense with each supported feature, making the library
+  all-the-more difficult to customize for a specific use case.
+* The software becomes less performant for a specific use case. RL practitioners
+  typically end up accepting the cost of transitioning to expensive and
+  difficult-to-manage compute clusters to get results faster.
+
+There's a handful of high quality, open-sourced RL libraries that tradeoff feature
+richness to reduce these drawbacks. However, each library still doesn't provide
+enough speed benefit to warrant the switch from a monolithic repo, or is still
+too complex to adapt to a specific use case.
+
+**rlstack** is a niche RL library that finds a goldilocks zone between the
+feature support and speed/complexity tradeoff by making some key assumptions:
+
+* Environments are highly parallelized and their parallelization is entirely
+  managed within the environment. This allows **rlstack** to ignore distributed
+  computing design considerations.
+* Environments are infinite horizon (i.e., they have no terminal conditions).
+  This allows **rlstack** to reset environments at the same, fixed horizon
+  intervals, greatly simplifying environment and algorithm implementations.
+* The only supported ML framework is PyTorch and the only supported algorithm
+  is PPO. This allows **rlstack** to ignore layers upon layers of abstraction,
+  greatly simplifying the overall library implementation.
+
+The end result is a minimal and high throughput library that can train policies
+to solve complex tasks on a single NVIDIA RTX 2080 within minutes.
+
+Unfortunately, this means **rlstack** doesn't support as many use cases as
+a monolithic RL library might. In fact, **rlstack** is probably a bad fit for
+your use case if:
+
+* Your environment isn't parallelizable.
+* Your environment must contain terminal conditions and can't be reformulated
+  as an infinite horizon task.
+* You want to use an ML framework that isn't PyTorch or you want to use an
+  algorithm that isn't a variant of PPO.
+
+However, if **rlstack** does fit your use case, it can do wonders for your
+RL workflow.
+
 Related Projects
 ================
 
 * `RL Games`_: RL Games is a high performance RL library built around popular
   environment protocols.
 * `RLlib`_: Ray's RLlib is the industry standard RL library that supports many
   popular RL algorithms. RLlib can scale RL workloads from your laptop all the
```

### Comparing `rlstack-0.0.0b1/docs/Makefile` & `rlstack-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/docs/conf.py` & `rlstack-0.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/docs/make.bat` & `rlstack-0.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/pyproject.toml` & `rlstack-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     "tox",
     "virtualenv"
 ]
 
 [tool.isort]
 profile = "black"
 src_paths = [
+    "examples",
     "src",
     "tests"
 ]
 
 [tool.mypy]
 ignore_missing_imports = true
 implicit_reexport = true
```

### Comparing `rlstack-0.0.0b1/src/rlstack/__init__.py` & `rlstack-0.1.0/src/rlstack/__init__.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/src/rlstack/_utils.py` & `rlstack-0.1.0/src/rlstack/_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,59 @@
 import time
 from contextlib import contextmanager
 from typing import Callable, Generator, Iterable
 
-from .specs import TensorSpec
+from .specs import CompositeSpec, TensorSpec
 
 
 def assert_1d_spec(spec: TensorSpec, /) -> None:
     """Check if the spec is valid for default models and distributions
     by asserting that it's 1D.
 
     Args:
         spec: Observation or action spec when using default models or
             distributions.
 
     Raises:
         AssertionError: If ``spec`` is not 1D.
 
     """
-    assert spec.shape.numel() == 1, (
+    assert spec.ndim == 1, (
+        f"{spec} is not compatible with default models and distributions. "
         "Default models and distributions do not support tensor specs "
         "that aren't 1D. Tensor specs must have shape ``[N]`` "
         "(where ``N`` is the number of independent elements) to be "
         "compatible with default models and distributions."
     )
 
 
+def assert_nd_spec(spec: TensorSpec, /) -> None:
+    """Check if the spec is at least 1D so it can properly interface with
+    library objects.
+
+    Args:
+        spec: Observation or action spec.
+
+    Raises:
+        AssertionError: If ``spec`` is not at least 1D.
+
+    """
+    match spec:
+        case CompositeSpec():
+            for k in spec:
+                assert_nd_spec(spec[k])
+        case _:
+            assert spec.ndim >= 1, (
+                f"{spec} is not a valid spec. Models and distributions must have specs"
+                " that have a non-empty shape. Tensor specs must have shape ``[N,"
+                " ...]`` (where ``N`` is the number of independent elements and"
+                " ``...`` is any number of additional dimensions)."
+            )
+
+
 @contextmanager
 def profile_ms() -> Generator[Callable[[], float], None, None]:
     """Profiling context manager that returns the time it took for the
     code to execute within the context's scope in milliseconds.
 
     """
     start = time.perf_counter_ns()
```

### Comparing `rlstack-0.0.0b1/src/rlstack/algorithms/__init__.py` & `rlstack-0.1.0/src/rlstack/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/src/rlstack/algorithms/_feedforward.py` & `rlstack-0.1.0/src/rlstack/algorithms/_feedforward.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import torch
 import torch.amp as amp
 import torch.optim as optim
 from tensordict import TensorDict
 from torch.utils.data import DataLoader
 
-from .._utils import StatTracker, profile_ms
+from .._utils import StatTracker, assert_nd_spec, profile_ms
 from ..data import (
     AlgorithmHparams,
     AlgorithmState,
     CollectStats,
     DataKeys,
     Device,
     StepStats,
@@ -240,14 +240,16 @@
         vf_clip_param: float = 5.0,
         dual_clip_param: None | float = None,
         vf_coeff: float = 1.0,
         max_grad_norm: float = 5.0,
         device: Device = "cpu",
     ) -> None:
         self.env = env_cls(num_envs, config=env_config, device=device)
+        assert_nd_spec(self.env.observation_spec)
+        assert_nd_spec(self.env.action_spec)
         self.policy = Policy(
             self.env.observation_spec,
             self.env.action_spec,
             model=model,
             model_cls=model_cls,
             model_config=model_config,
             distribution_cls=distribution_cls,
@@ -255,15 +257,14 @@
         )
         max_horizon = self.env.max_horizon if hasattr(self.env, "max_horizon") else 32
         horizon = min(horizon, max_horizon) if horizon else max_horizon
         self.buffer_spec = CompositeSpec(  # type: ignore[no-untyped-call]
             {
                 DataKeys.OBS: self.env.observation_spec,
                 DataKeys.REWARDS: UnboundedContinuousTensorSpec(1, device=device),
-                DataKeys.FEATURES: self.policy.feature_spec,
                 DataKeys.ACTIONS: self.env.action_spec,
                 DataKeys.LOGP: UnboundedContinuousTensorSpec(1, device=device),
                 DataKeys.VALUES: UnboundedContinuousTensorSpec(1, device=device),
                 DataKeys.ADVANTAGES: UnboundedContinuousTensorSpec(1, device=device),
                 DataKeys.RETURNS: UnboundedContinuousTensorSpec(1, device=device),
             },
         ).to(device)
@@ -361,17 +362,14 @@
                     return_values=True,
                     return_views=False,
                 )
                 out_batch = self.env.step(sample_batch[DataKeys.ACTIONS])
 
                 # Update the buffer using sampled policy data and environment
                 # transition data.
-                self.buffer[DataKeys.FEATURES][:, t, ...] = sample_batch[
-                    DataKeys.FEATURES
-                ]
                 self.buffer[DataKeys.ACTIONS][:, t, ...] = sample_batch[
                     DataKeys.ACTIONS
                 ]
                 self.buffer[DataKeys.LOGP][:, t, ...] = sample_batch[DataKeys.LOGP]
                 self.buffer[DataKeys.VALUES][:, t, ...] = sample_batch[DataKeys.VALUES]
                 self.buffer[DataKeys.REWARDS][:, t, ...] = out_batch[DataKeys.REWARDS]
                 self.buffer[DataKeys.OBS][:, t + 1, ...] = out_batch[DataKeys.OBS]
@@ -385,15 +383,14 @@
                 inplace=False,
                 requires_grad=False,
                 return_actions=False,
                 return_logp=False,
                 return_values=True,
                 return_views=False,
             )
-            self.buffer[DataKeys.FEATURES][:, -1, ...] = sample_batch[DataKeys.FEATURES]
             self.buffer[DataKeys.VALUES][:, -1, ...] = sample_batch[DataKeys.VALUES]
 
             self.state.horizons += 1
             self.state.buffered = True
 
             # Aggregate some metrics.
             rewards = self.buffer[DataKeys.REWARDS][:, :-1, ...]
```

### Comparing `rlstack-0.0.0b1/src/rlstack/algorithms/_recurrent.py` & `rlstack-0.1.0/src/rlstack/algorithms/_recurrent.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import torch
 import torch.amp as amp
 import torch.optim as optim
 from tensordict import TensorDict
 from torch.utils.data import DataLoader
 
-from .._utils import StatTracker, profile_ms
+from .._utils import StatTracker, assert_nd_spec, profile_ms
 from ..data import (
     CollectStats,
     DataKeys,
     Device,
     RecurrentAlgorithmHparams,
     RecurrentAlgorithmState,
     StepStats,
@@ -251,14 +251,16 @@
         vf_clip_param: float = 5.0,
         dual_clip_param: None | float = None,
         vf_coeff: float = 1.0,
         max_grad_norm: float = 5.0,
         device: Device = "cpu",
     ) -> None:
         self.env = env_cls(num_envs, config=env_config, device=device)
+        assert_nd_spec(self.env.observation_spec)
+        assert_nd_spec(self.env.action_spec)
         self.policy = RecurrentPolicy(
             self.env.observation_spec,
             self.env.action_spec,
             model=model,
             model_cls=model_cls,
             model_config=model_config,
             distribution_cls=distribution_cls,
@@ -267,15 +269,14 @@
         max_horizon = self.env.max_horizon if hasattr(self.env, "max_horizon") else 32
         horizon = min(horizon, max_horizon) if horizon else max_horizon
         self.buffer_spec = CompositeSpec(  # type: ignore[no-untyped-call]
             {
                 DataKeys.OBS: self.env.observation_spec,
                 DataKeys.STATES: self.policy.state_spec,
                 DataKeys.REWARDS: UnboundedContinuousTensorSpec(1, device=device),
-                DataKeys.FEATURES: self.policy.feature_spec,
                 DataKeys.ACTIONS: self.env.action_spec,
                 DataKeys.LOGP: UnboundedContinuousTensorSpec(1, device=device),
                 DataKeys.VALUES: UnboundedContinuousTensorSpec(1, device=device),
                 DataKeys.ADVANTAGES: UnboundedContinuousTensorSpec(1, device=device),
                 DataKeys.RETURNS: UnboundedContinuousTensorSpec(1, device=device),
             },
         ).to(device)
@@ -390,17 +391,14 @@
                     return_logp=True,
                     return_values=True,
                 )
                 out_batch = self.env.step(sample_batch[DataKeys.ACTIONS])
 
                 # Update the buffer using sampled policy data and environment
                 # transition data.
-                self.buffer[DataKeys.FEATURES][:, t, ...] = sample_batch[
-                    DataKeys.FEATURES
-                ]
                 self.buffer[DataKeys.ACTIONS][:, t, ...] = sample_batch[
                     DataKeys.ACTIONS
                 ]
                 self.buffer[DataKeys.LOGP][:, t, ...] = sample_batch[DataKeys.LOGP]
                 self.buffer[DataKeys.VALUES][:, t, ...] = sample_batch[DataKeys.VALUES]
                 self.buffer[DataKeys.REWARDS][:, t, ...] = out_batch[DataKeys.REWARDS]
                 self.buffer[DataKeys.OBS][:, t + 1, ...] = out_batch[DataKeys.OBS]
@@ -419,15 +417,14 @@
                 inplace=False,
                 keepdim=False,
                 requires_grad=False,
                 return_actions=False,
                 return_logp=False,
                 return_values=True,
             )
-            self.buffer[DataKeys.FEATURES][:, -1, ...] = sample_batch[DataKeys.FEATURES]
             self.buffer[DataKeys.VALUES][:, -1, ...] = sample_batch[DataKeys.VALUES]
 
             self.state.horizons += 1
             self.state.buffered = True
 
             # Aggregate some metrics.
             rewards = self.buffer[DataKeys.REWARDS][:, 1:-1, ...]
```

### Comparing `rlstack-0.0.0b1/src/rlstack/conditions.py` & `rlstack-0.1.0/src/rlstack/conditions.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/src/rlstack/data.py` & `rlstack-0.1.0/src/rlstack/data.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/src/rlstack/distributions.py` & `rlstack-0.1.0/src/rlstack/distributions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from abc import ABC, abstractmethod
-from copy import deepcopy
 from typing import Any, Generic, TypeVar
 
 import torch
 from tensordict import TensorDict
 
 from ._utils import assert_1d_spec
 from .specs import (
@@ -73,45 +72,14 @@
             case UnboundedContinuousTensorSpec():
                 return Normal
             case _:
                 raise TypeError(
                     f"Action spec {action_spec} has no default distribution support."
                 )
 
-    @staticmethod
-    def default_feature_spec(action_spec: TensorSpec, /) -> TensorSpec:
-        """Return a default feature spec given an action spec.
-
-        Useful for defining feature specs for simple and common action
-        specs. Custom models with complex action specs should define
-        their own custom feature specs as an attribute.
-
-        Args:
-            action_spec: Spec defining the outputs of the policy's action
-                distribution that this model is a component of. Typically
-                passed into the model's ``__init__``.
-
-        Returns:
-            A spec defining the inputs to the policy's action distribution.
-            For simple distributions (e.g., categorical or diagonal gaussian),
-            this returns a spec defining the inputs to those distributions
-            (e.g., logits and mean/scales, respectively). For complex
-            distributions, this returns a copy of the action spec and the model
-            is expected to assign the correct feature spec within its own
-            ``__init__``.
-
-        """
-        match action_spec:
-            case DiscreteTensorSpec():
-                return Categorical.required_feature_spec(action_spec)
-            case UnboundedContinuousTensorSpec():
-                return Normal.required_feature_spec(action_spec)
-            case _:
-                return deepcopy(action_spec)
-
     @abstractmethod
     def deterministic_sample(self) -> torch.Tensor | TensorDict:
         """Draw a deterministic sample from the probability distribution."""
 
     @abstractmethod
     def entropy(self) -> torch.Tensor:
         """Compute the probability distribution's entropy (a measurement
@@ -150,22 +118,14 @@
 
     def entropy(self) -> torch.Tensor:
         return self.dist.entropy().sum(-1, keepdim=True)
 
     def logp(self, samples: torch.Tensor) -> torch.Tensor:
         return self.dist.log_prob(samples).sum(-1, keepdim=True)
 
-    @staticmethod
-    @abstractmethod
-    def required_feature_spec(action_spec: _ActionSpec, /) -> _FeatureSpec:
-        """Define feature spec requirements for the distribution given an
-        action spec.
-
-        """
-
     def sample(self) -> torch.Tensor:
         return self.dist.sample()
 
 
 class Categorical(
     TorchDistributionWrapper[
         CompositeSpec, torch.distributions.Categorical, DiscreteTensorSpec
@@ -173,48 +133,26 @@
 ):
     """Wrapper around the PyTorch categorical (i.e., discrete) distribution."""
 
     def __init__(self, features: TensorDict, model: Any, /) -> None:
         super().__init__(features, model)
         self.dist = torch.distributions.Categorical(logits=features["logits"])  # type: ignore[no-untyped-call]
 
-    @staticmethod
-    def required_feature_spec(action_spec: DiscreteTensorSpec, /) -> CompositeSpec:
-        return CompositeSpec(
-            logits=UnboundedContinuousTensorSpec(
-                shape=torch.Size([action_spec.shape[0], action_spec.space.n]),
-                device=action_spec.device,
-            )
-        )  # type: ignore[no-untyped-call]
-
 
 class Normal(
     TorchDistributionWrapper[
         CompositeSpec, torch.distributions.Normal, UnboundedContinuousTensorSpec
     ]
 ):
     """Wrapper around the PyTorch normal (i.e., gaussian) distribution."""
 
     def __init__(self, features: TensorDict, model: Any) -> None:
         super().__init__(features, model)
         self.dist = torch.distributions.Normal(loc=features["mean"], scale=torch.exp(features["log_std"]))  # type: ignore[no-untyped-call]
 
-    @staticmethod
-    def required_feature_spec(
-        action_spec: UnboundedContinuousTensorSpec, /
-    ) -> CompositeSpec:
-        return CompositeSpec(
-            mean=UnboundedContinuousTensorSpec(
-                shape=action_spec.shape, device=action_spec.device
-            ),
-            log_std=UnboundedContinuousTensorSpec(
-                shape=action_spec.shape, device=action_spec.device
-            ),
-        )  # type: ignore[no-untyped-call]
-
 
 class SquashedNormal(Normal):
     """Squashed normal distribution such that samples are always within [-1, 1]."""
 
     def deterministic_sample(self) -> torch.Tensor:
         return super().deterministic_sample().tanh()
```

### Comparing `rlstack-0.0.0b1/src/rlstack/env.py` & `rlstack-0.1.0/src/rlstack/env.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,59 +1,75 @@
 """Environment protocol definition and helper dummy environment definitions."""
 
-from typing import Any, Generic, Protocol, TypeVar
+from abc import ABC, abstractmethod
+from typing import Any, Generic, TypeVar
 
 import torch
 from tensordict import TensorDict
 
 from .data import DataKeys, Device
 from .specs import DiscreteTensorSpec, TensorSpec, UnboundedContinuousTensorSpec
 
 _ObservationSpec = TypeVar("_ObservationSpec", bound=TensorSpec)
 _ActionSpec = TypeVar("_ActionSpec", bound=TensorSpec)
 
 
-class Env(Protocol):
+class Env(ABC):
     """Protocol defining the IsaacGym -like environments for supporting
     highly parallelized simulation.
 
     Args:
-        num_envs: Number of parallel and independent environment being
+        num_envs: Number of parallel and independent environments being
             simulated by one :class:`Env` instance.
         config: Config detailing simulation options/parameters for the
             environment's initialization.
         device: Device the environment's underlying data should be
             initialized on.
 
     """
 
     #: Spec defining the environment's inputs (and policy's action
     #: distribution's outputs). Used for initializing the policy, the
     #: policy's underlying components, and the learning buffer.
     action_spec: TensorSpec
 
+    #: Environment config passed to the environment at instantiation.
+    #: This could be overwritten by :meth:`Environment.reset`, but it's
+    #: entirely at the developer's discretion.
+    config: dict[str, Any]
+
+    #: Device the environment's states, observations, and rewards reside
+    #: on.
+    device: Device
+
     #: An optional attribute denoting the max number of steps an environment
     #: may take before being reset.
     max_horizon: int
 
+    #: Number of parallel and independent environments being simulated.
+    num_envs: int
+
     #: Spec defining part of the environment's outputs (and policy's
     #: model's outputs). Used for initializing the policy, the
     #: policy's underlying components, and the learning buffer.
     observation_spec: TensorSpec
 
     def __init__(
         self,
         num_envs: int,
         /,
         *,
         config: None | dict[str, Any] = None,
         device: Device = "cpu",
     ) -> None:
-        ...
+        self.num_envs = num_envs
+        self.config = config or {}
+        self.device = device
 
+    @abstractmethod
     def reset(
         self, *, config: None | dict[str, Any] = None
     ) -> torch.Tensor | TensorDict:
         """Reset the environment, applying a new environment config to it and
         returning a new, initial observation from the environment.
 
         Args:
@@ -61,14 +77,15 @@
 
         Returns:
             Initial observation from the reset environment with spec
             :attr:`Env.observation_spec`.
 
         """
 
+    @abstractmethod
     def step(self, action: torch.Tensor | TensorDict) -> TensorDict:
         """Step the environment by applying an action, simulating an environment
         transition, and returning an observation and a reward.
 
         Args:
             action: Action to apply to the environment with tensor spec
                 :attr:`Env.action_spec`.
@@ -114,30 +131,23 @@
         self,
         num_envs: int,
         /,
         *,
         config: None | dict[str, Any] = None,
         device: Device = "cpu",
     ) -> None:
-        if config is None:
-            config = {}
-        self.observation_spec = UnboundedContinuousTensorSpec(1, device=device)
-        self.bounds = config.get("bounds", 100.0)
-        self.state = (
-            -self.bounds * torch.rand(num_envs, device=device).unsqueeze(1)
-            + self.bounds
-        )
+        super().__init__(num_envs, config=config, device=device)
+        self.observation_spec = UnboundedContinuousTensorSpec(1, device=self.device)
+        self.bounds = self.config.get("bounds", 100.0)
 
     def reset(self, *, config: None | dict[str, Any] = None) -> torch.Tensor:
-        if config and "bounds" in config:
-            self.bounds = config["bounds"]
-        self.state = (
-            -self.bounds
-            * torch.rand(self.state.size(0), device=self.state.device).unsqueeze(1)
-            + self.bounds
+        config = config or {}
+        self.bounds = config.get("bounds", self.bounds)
+        self.state = torch.empty(self.num_envs, 1, device=self.device).uniform_(
+            -self.bounds, self.bounds
         )
         return self.state
 
 
 class ContinuousDummyEnv(DummyEnv[UnboundedContinuousTensorSpec]):
     """A continuous version of the dummy environment.
 
@@ -158,16 +168,16 @@
             shape=torch.Size([1]), device=device
         )
 
     def step(self, action: torch.Tensor) -> TensorDict:
         self.state += action
         return TensorDict(
             {DataKeys.OBS: self.state, DataKeys.REWARDS: -self.state.abs()},
-            batch_size=self.state.size(0),
-            device=self.state.device,
+            batch_size=self.num_envs,
+            device=self.device,
         )
 
 
 class DiscreteDummyEnv(DummyEnv[DiscreteTensorSpec]):
     """A discrete version of the dummy environment.
 
     Actions include moving the state left or right one unit. This
@@ -187,10 +197,10 @@
         super().__init__(num_envs, config=config, device=device)
         self.action_spec = DiscreteTensorSpec(2, shape=torch.Size([1]), device=device)
 
     def step(self, action: torch.Tensor) -> TensorDict:
         self.state += 2 * action - 1
         return TensorDict(
             {DataKeys.OBS: self.state, DataKeys.REWARDS: -self.state.abs()},
-            batch_size=self.state.size(0),
-            device=self.state.device,
+            batch_size=self.num_envs,
+            device=self.device,
         )
```

### Comparing `rlstack-0.0.0b1/src/rlstack/models/__init__.py` & `rlstack-0.1.0/src/rlstack/models/__init__.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/src/rlstack/models/_feedforward.py` & `rlstack-0.1.0/src/rlstack/models/_feedforward.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import torch
 import torch.nn as nn
 from tensordict import TensorDict
 from typing_extensions import Self
 
 from .._utils import assert_1d_spec
 from ..data import DataKeys, Device
-from ..distributions import Distribution
 from ..nn import MLP, Module, get_activation
 from ..specs import DiscreteTensorSpec, TensorSpec, UnboundedContinuousTensorSpec
 from ..views import ViewKind, ViewRequirement
 
 _ObservationSpec = TypeVar("_ObservationSpec", bound=TensorSpec)
 _ActionSpec = TypeVar("_ActionSpec", bound=TensorSpec)
 
@@ -41,20 +40,14 @@
     #: this model is a component of. Useful for defining the model as a
     #: function of the action spec.
     action_spec: TensorSpec
 
     #: Model-specific configuration. Passed from the policy and algorithm.
     config: dict[str, Any]
 
-    #: Spec defining the forward pass output. Useful for passing inputs to an
-    #: action distribution or stroing values in the replay buffer. Defaults
-    #: to `action_spec`. This should be overwritten in a model's ``__init__``
-    #: for models that feed into custom action distributions .
-    feature_spec: TensorSpec
-
     #: Spec defining the forward pass input. Useful for validating the forward
     #: pass and for defining the model as a function of the observation spec.
     observation_spec: TensorSpec
 
     #: Requirements on how a tensor batch should be preprocessed by the
     #: policy prior to being passed to the forward pass. Useful for handling
     #: sequence shifting or masking so you don't have to.
@@ -70,16 +63,15 @@
         /,
         **config: Any,
     ) -> None:
         super().__init__()
         self.observation_spec = observation_spec
         self.action_spec = action_spec
         self.config = config
-        self.feature_spec = Distribution.default_feature_spec(action_spec)
-        self.view_requirements = {DataKeys.OBS: ViewRequirement(DataKeys.OBS, shift=0)}
+        self.view_requirements = {DataKeys.OBS: ViewRequirement(shift=0)}
 
     def apply_view_requirements(
         self, batch: TensorDict, /, *, kind: ViewKind = "last"
     ) -> TensorDict:
         """Apply the model's view requirements, reshaping tensors as-needed.
 
         This is usually called by the policy that the model is a component
@@ -108,34 +100,23 @@
 
         """
         batch_sizes = {}
         out = {}
         for key, view_requirement in self.view_requirements.items():
             match kind:
                 case "all":
-                    item = view_requirement.apply_all(batch)
+                    item = view_requirement.apply_all(key, batch)
                 case "last":
-                    item = view_requirement.apply_last(batch)
+                    item = view_requirement.apply_last(key, batch)
             out[key] = item
             B_NEW = item.size(0)
             batch_sizes[key] = B_NEW
         batch_size = next(iter(batch_sizes.values()))
         return TensorDict(out, batch_size=batch_size, device=batch.device)
 
-    @property
-    def burn_size(self) -> int:
-        """Return the model's burn size (also the burn size for all view
-        requirements.
-
-        """
-        burn_sizes = {}
-        for key, view_requirement in self.view_requirements.items():
-            burn_sizes[key] = view_requirement.burn_size
-        return next(iter(burn_sizes.values()))
-
     @staticmethod
     def default_model_cls(
         observation_spec: TensorSpec,
         action_spec: TensorSpec,
         /,
     ) -> type["Model"]:
         """Return a default model class based on the given observation and
@@ -166,14 +147,25 @@
                 )
 
     @property
     def device(self) -> Device:
         """Return the device the model is currently on."""
         return next(self.parameters()).device
 
+    @property
+    def drop_size(self) -> int:
+        """Return the model's drop size (also the drop size for all view
+        requirements).
+
+        """
+        drop_sizes = {}
+        for key, view_requirement in self.view_requirements.items():
+            drop_sizes[key] = view_requirement.drop_size
+        return next(iter(drop_sizes.values()))
+
     @abstractmethod
     def forward(self, batch: TensorDict, /) -> TensorDict:
         """Process a batch of tensors and return features to be fed into an
         action distribution.
 
         Args:
             batch: A tensordict expected to have at least an ``"obs"`` key with any
@@ -199,34 +191,33 @@
 
         Returns:
             The updated model.
 
         """
         self.observation_spec = self.observation_spec.to(device)
         self.action_spec = self.action_spec.to(device)
-        self.feature_spec = self.feature_spec.to(device)
         return super().to(device)
 
     def validate_view_requirements(self) -> None:
         """Helper for validating a model's view requirements.
 
         Raises:
             RuntimeError: If the model's view requirements result in an
                 ambiguous batch size, making training and sampling impossible.
 
         """
-        burn_sizes = {}
+        drop_sizes = {}
         for key, view_requirement in self.view_requirements.items():
-            burn_sizes[key] = view_requirement.burn_size
-        if len(set(burn_sizes.values())) > 1:
+            drop_sizes[key] = view_requirement.drop_size
+        if len(set(drop_sizes.values())) > 1:
             raise RuntimeError(
-                f"""{self} view requirements with burn sizes {burn_sizes}
+                f"""{self} view requirements with drop sizes {drop_sizes}
                 result in an ambiguous batch size. It's recommended you:
                     1) use a view requirement method that does not have sample
-                        burn, allowing view requirements with different sizes
+                        dropping, allowing view requirements with different sizes
                     2) reformulate your model and observation function such
                         that view requirements are not necessary or are
                         handled internal to your environment
 
                 """
             )
 
@@ -387,20 +378,20 @@
             get_activation(activation_fn),
             nn.Linear(hiddens[-1], 1),
         )
         self._value = None
 
     def forward(self, batch: TensorDict, /) -> TensorDict:
         obs = batch[DataKeys.OBS]
-        features = self.feature_model(obs).reshape(
+        logits = self.feature_model(obs).reshape(
             -1, self.action_spec.shape[0], self.action_spec.space.n
         )
         self._value = self.vf_model(obs)
         return TensorDict(
-            {"logits": features},
+            {"logits": logits},
             batch_size=batch.batch_size,
             device=obs.device,
         )
 
     def value_function(self) -> torch.Tensor:
         assert self._value is not None
         return self._value
```

### Comparing `rlstack-0.0.0b1/src/rlstack/models/_recurrent.py` & `rlstack-0.1.0/src/rlstack/models/_recurrent.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import torch
 import torch.nn as nn
 from tensordict import TensorDict
 from typing_extensions import Self
 
 from .._utils import assert_1d_spec
 from ..data import DataKeys, Device
-from ..distributions import Distribution
 from ..nn import Module
 from ..specs import (
     CompositeSpec,
     DiscreteTensorSpec,
     TensorSpec,
     UnboundedContinuousTensorSpec,
 )
@@ -44,20 +43,14 @@
     #: this model is a component of. Useful for defining the model as a
     #: function of the action spec.
     action_spec: TensorSpec
 
     #: Model-specific configuration. Passed from the policy and algorithm.
     config: dict[str, Any]
 
-    #: Spec defining the forward pass output. Useful for passing inputs to an
-    #: action distribution or stroing values in the replay buffer. Defaults
-    #: to `action_spec`. This should be overwritten in a model's ``__init__``
-    #: for models that feed into custom action distributions .
-    feature_spec: TensorSpec
-
     #: Spec defining observations part of the forward pass input. Useful for
     #: validating the forward pass and for defining the model as a function of
     #: the observation spec.
     observation_spec: TensorSpec
 
     #: Spec defining recurrent model states part of the forward pass input
     #: and output. This is expected to be defined in a model's ``__init__``.
@@ -70,15 +63,14 @@
         /,
         **config: Any,
     ) -> None:
         super().__init__()
         self.observation_spec = observation_spec
         self.action_spec = action_spec
         self.config = config
-        self.feature_spec = Distribution.default_feature_spec(action_spec)
 
     @staticmethod
     def default_model_cls(
         observation_spec: TensorSpec,
         action_spec: TensorSpec,
         /,
     ) -> type["RecurrentModel"]:
@@ -139,28 +131,31 @@
             the batch and sequence dimension of the input arguments are
             flattened together for the output features while the returned
             recurrent states maintain the original batch dimension but don't
             have a sequence dimension.
 
         """
 
-    @abstractmethod
     def init_states(self, n: int, /) -> TensorDict:
         """Return initial recurrent states for the model.
 
+        Override this to make your own method for initializing
+        recurrent states.
+
         Args:
             n: Batch size to generate initial recurrent states for.
                 This is typically the number of environments being
                 stepped in parallel.
 
         Returns:
             Recurrent model states that initialize a recurrent
             sequence.
 
         """
+        return self.state_spec.zero([n])
 
     def to(self, device: Device) -> Self:  # type: ignore[override]
         """Helper for changing the device the model is on.
 
         The specs associated with the model aren't updated with the PyTorch
         module's ``to`` method since they aren't PyTorch modules themselves.
 
@@ -169,15 +164,14 @@
 
         Returns:
             The updated model.
 
         """
         self.observation_spec = self.observation_spec.to(device)
         self.action_spec = self.action_spec.to(device)
-        self.feature_spec = self.feature_spec.to(device)
         self.state_spec = self.state_spec.to(device)
         return super().to(device)
 
     @abstractmethod
     def value_function(self) -> torch.Tensor:
         """Return the value function output for the most recent forward pass.
         Note that a :meth`RecurrentModel.forward` call has to be performed
@@ -204,17 +198,14 @@
         observation_spec: _ObservationSpec,
         action_spec: _ActionSpec,
         /,
         **config: Any,
     ) -> None:
         super().__init__(observation_spec, action_spec, **config)
 
-    def init_states(self, n: int) -> TensorDict:
-        return self.state_spec.zero([n])
-
 
 class DefaultContinuousRecurrentModel(
     GenericRecurrentModel[UnboundedContinuousTensorSpec, UnboundedContinuousTensorSpec]
 ):
     """Default recurrent model for 1D continuous observations and action spaces."""
 
     #: Value function estimate set after `forward`.
```

### Comparing `rlstack-0.0.0b1/src/rlstack/nn/__init__.py` & `rlstack-0.1.0/src/rlstack/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/src/rlstack/nn/functional.py` & `rlstack-0.1.0/src/rlstack/nn/functional.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/src/rlstack/nn/modules/activations.py` & `rlstack-0.1.0/src/rlstack/nn/modules/activations.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/src/rlstack/nn/modules/attention.py` & `rlstack-0.1.0/src/rlstack/nn/modules/attention.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,17 +95,14 @@
             of the feedforward network that's after performing attention.
         activation_fn: Activation function ID.
         attention_dropout: Sequence dropout in the attention heads.
         hidden_dropout: Feedforward dropout after performing attention.
         skip_kind: Kind of residual or skip connection to make between
             the output of the multihead attention and the feedforward
             module.
-        fan_in: Whether to apply downsampling within the skip connection
-            when using a ``skip_kind`` that increases hidden feature
-            dimensions.
 
     """
 
     #: Underlying multihead attention mechanism.
     attention: nn.MultiheadAttention
 
     #: Norm for the keys.
@@ -123,24 +120,24 @@
         /,
         num_heads: int = 2,
         hidden_dim: int = 128,
         activation_fn: str = "relu",
         attention_dropout: float = 0.0,
         hidden_dropout: float = 0.0,
         skip_kind: None | str = "cat",
-        fan_in: bool = True,
     ) -> None:
         super().__init__()
         self.q_norm = nn.LayerNorm(embed_dim)
         self.kv_norm = nn.LayerNorm(embed_dim)
         self.attention = nn.MultiheadAttention(
             embed_dim, num_heads, dropout=attention_dropout, batch_first=True
         )
         self.skip_connection = SequentialSkipConnection(
-            embed_dim, kind=skip_kind, fan_in=fan_in
+            embed_dim,
+            kind=skip_kind,
         )
         mlp = torch.nn.Sequential(
             nn.LayerNorm(self.skip_connection.out_features),
             nn.Linear(self.skip_connection.out_features, hidden_dim),
             get_activation(activation_fn),
             nn.Dropout(p=hidden_dropout),
             nn.Linear(hidden_dim, self.skip_connection.out_features),
@@ -214,17 +211,14 @@
             of the feedforward network that's after performing attention.
         activation_fn: Activation function ID.
         attention_dropout: Sequence dropout in the attention heads.
         hidden_dropout: Feedforward dropout after performing attention.
         skip_kind: Kind of residual or skip connection to make between
             the output of the multihead attention and the feedforward
             module.
-        fan_in: Whether to apply downsampling within the skip connection
-            when using a ``skip_kind`` that increases hidden feature
-            dimensions.
 
     """
 
     #: Underlying multihead attention mechanism.
     attention: nn.MultiheadAttention
 
     #: Skip connection for applying special residual connections.
@@ -239,23 +233,23 @@
         /,
         num_heads: int = 2,
         hidden_dim: int = 128,
         activation_fn: str = "relu",
         attention_dropout: float = 0.0,
         hidden_dropout: float = 0.0,
         skip_kind: None | str = "cat",
-        fan_in: bool = True,
     ) -> None:
         super().__init__()
         self.x_norm = nn.LayerNorm(embed_dim)
         self.attention = nn.MultiheadAttention(
             embed_dim, num_heads, dropout=attention_dropout, batch_first=True
         )
         self.skip_connection = SequentialSkipConnection(
-            embed_dim, kind=skip_kind, fan_in=fan_in
+            embed_dim,
+            kind=skip_kind,
         )
         mlp = torch.nn.Sequential(
             nn.LayerNorm(self.skip_connection.out_features),
             nn.Linear(self.skip_connection.out_features, hidden_dim),
             get_activation(activation_fn),
             nn.Dropout(p=hidden_dropout),
             nn.Linear(hidden_dim, self.skip_connection.out_features),
@@ -313,20 +307,32 @@
     Module[[torch.Tensor, None | torch.Tensor, None | torch.Tensor], torch.Tensor]
 ):
     """Stacks of self-attention to iteratively attend over a sequence.
 
     Args:
         module: Self-attention module to repeat.
         num_layers: Number of layers of ``module`` to repeat.
+        share_parameters: Whether to use the same module for each layer.
 
     """
 
-    def __init__(self, module: SelfAttention, num_layers: int, /) -> None:
+    def __init__(
+        self,
+        module: SelfAttention,
+        num_layers: int,
+        /,
+        *,
+        share_parameters: bool = False,
+    ) -> None:
         super().__init__()
-        self.layers = nn.ModuleList([copy.deepcopy(module) for _ in range(num_layers)])
+        if share_parameters:
+            modules = [module for _ in range(num_layers)]
+        else:
+            modules = [copy.deepcopy(module) for _ in range(num_layers)]
+        self.layers = nn.ModuleList(modules)
 
     def forward(
         self,
         x: torch.Tensor,
         key_padding_mask: None | torch.Tensor = None,
         attention_mask: None | torch.Tensor = None,
     ) -> torch.Tensor:
```

### Comparing `rlstack-0.0.0b1/src/rlstack/nn/modules/embeddings.py` & `rlstack-0.1.0/src/rlstack/nn/modules/embeddings.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/src/rlstack/nn/modules/mlp.py` & `rlstack-0.1.0/src/rlstack/nn/modules/mlp.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/src/rlstack/nn/modules/module.py` & `rlstack-0.1.0/src/rlstack/nn/modules/module.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/src/rlstack/nn/modules/perceiver.py` & `rlstack-0.1.0/src/rlstack/nn/modules/perceiver.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,17 +30,16 @@
             of the feedforward networks that're after performing attention.
         activation_fn: Activation function ID.
         attention_dropout: Sequence dropout in the attention heads.
         hidden_dropout: Feedforward dropout after performing attention.
         skip_kind: Kind of residual or skip connection to make between
             outputs of the multihead attentions and the feedforward
             modules.
-        fan_in: Whether to apply downsampling within the skip connection
-            when using a `skip_kind` that increases hidden feature
-            dimensions.
+        share_parameters: Whether to use the same parameters for the layers
+            in the self-attention stack.
 
     .. _`Perceiver`: https://arxiv.org/pdf/2103.03206.pdf
 
     """
 
     def __init__(
         self,
@@ -50,39 +49,38 @@
         num_heads: int = 2,
         hidden_dim: int = 128,
         num_layers: int = 2,
         activation_fn: str = "relu",
         attention_dropout: float = 0.0,
         hidden_dropout: float = 0.0,
         skip_kind: str = "cat",
-        fan_in: bool = True,
+        share_parameters: bool = False,
     ) -> None:
         super().__init__()
         self.cross_attention = CrossAttention(
             embed_dim,
             num_heads=num_heads,
             hidden_dim=hidden_dim,
             activation_fn=activation_fn,
             attention_dropout=attention_dropout,
             hidden_dropout=hidden_dropout,
             skip_kind=skip_kind,
-            fan_in=fan_in,
         )
         self.self_attention = SelfAttentionStack(
             SelfAttention(
                 embed_dim,
                 num_heads=num_heads,
                 hidden_dim=hidden_dim,
                 activation_fn=activation_fn,
                 attention_dropout=attention_dropout,
                 hidden_dropout=hidden_dropout,
                 skip_kind=skip_kind,
-                fan_in=fan_in,
             ),
             num_layers,
+            share_parameters=share_parameters,
         )
 
     def forward(
         self,
         q: torch.Tensor,
         kv: torch.Tensor,
         key_padding_mask: None | torch.Tensor = None,
@@ -136,17 +134,16 @@
             of the feedforward networks that're after performing attention.
         activation_fn: Activation function ID.
         attention_dropout: Sequence dropout in the attention heads.
         hidden_dropout: Feedforward dropout after performing attention.
         skip_kind: Kind of residual or skip connection to make between
             outputs of the multihead attentions and the feedforward
             modules.
-        fan_in: Whether to apply downsampling within the skip connection
-            when using a ``skip_kind`` that increases hidden feature
-            dimensions.
+        share_parameters: Whether to use the same parameters for the layers
+            in the self-attention stack.
 
     .. _`PerceiverIO`: https://arxiv.org/pdf/2107.14795.pdf
 
     """
 
     def __init__(
         self,
@@ -157,40 +154,39 @@
         num_heads: int = 2,
         hidden_dim: int = 128,
         num_layers: int = 2,
         activation_fn: str = "relu",
         attention_dropout: float = 0.0,
         hidden_dropout: float = 0.0,
         skip_kind: str = "cat",
-        fan_in: bool = True,
+        share_parameters: bool = False,
     ) -> None:
         super().__init__()
         self.perceiver_layer = PerceiverLayer(
             embed_dim,
             hidden_dim=hidden_dim,
             num_heads=num_heads,
             num_layers=num_layers,
             activation_fn=activation_fn,
             attention_dropout=attention_dropout,
             hidden_dropout=hidden_dropout,
             skip_kind=skip_kind,
-            fan_in=fan_in,
+            share_parameters=share_parameters,
         )
         self.output_query = nn.Parameter(torch.zeros([output_seq_dim, embed_dim]))
         with torch.no_grad():
             nn.init.xavier_uniform_(self.output_query)
         self.decoder = CrossAttention(
             embed_dim,
             num_heads=num_heads,
             hidden_dim=hidden_dim,
             activation_fn=activation_fn,
             attention_dropout=attention_dropout,
             hidden_dropout=hidden_dropout,
             skip_kind=skip_kind,
-            fan_in=fan_in,
         )
 
     def forward(
         self,
         q: torch.Tensor,
         kv: torch.Tensor,
         key_padding_mask: None | torch.Tensor = None,
```

### Comparing `rlstack-0.0.0b1/src/rlstack/nn/modules/skip.py` & `rlstack-0.1.0/src/rlstack/nn/modules/skip.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,32 +30,29 @@
 
     #: Number of input features for each module.
     _in_features: list[int]
 
     #: Modules associated with the sequential forward passes.
     _layers: nn.ModuleList
 
-    #: Whether to fan-in the outputs of each skip connection automatically.
-    #: The output features of the forward pass will always be ``embed_dim`` in this
-    #: case.
-    fan_in: bool
-
     #: Kind of skip connection. "residual" for a standard residual connection
     #: (summing outputs), "cat" for concatenating outputs, and ``None`` for no
     #: skip connection (reduces to a regular, sequential module).
     kind: None | str
 
-    def __init__(
-        self, embed_dim: int, kind: None | str = "cat", fan_in: bool = True
-    ) -> None:
+    def __init__(self, embed_dim: int, kind: None | str = "cat") -> None:
         super().__init__()
         self._in_features = [embed_dim]
         self._layers = torch.nn.ModuleList([])
         self.kind = kind
-        self.fan_in = fan_in
+        match kind:
+            case "cat":
+                self._layers.append(nn.Linear(self._skip_features, embed_dim))
+            case _:
+                self._layers.append(nn.Identity())
 
     @property
     def _skip_features(self) -> int:
         """Return the number of output features according to the number of input
         features and the kind of skip connection.
 
         """
@@ -65,33 +62,37 @@
             case "cat":
                 return 2 * self._in_features[-1]
             case None:
                 return self._in_features[-1]
         raise ValueError(f"No skip connection type for {self.kind}.")
 
     def append(self, module: nn.Module, /) -> int:
-        """Append `module` to the skip connection.
+        """Append ``module`` to the skip connection.
 
         If :attr:`SequentialSkipConnection.fan_in` is ``True``, then a
         fan-in layer is also appended after ``module`` to reduce the
         number of output features back to the input dimension.
 
         Args:
             module: Module to append and apply a skip connection to.
 
         Returns:
             Number of output features from the sequential skip connection.
 
         """
         self._in_features.append(self._skip_features)
         self._layers.append(module)
-        if self.fan_in:
-            linear = nn.Linear(self._in_features[-1], self._in_features[0])
-            self._in_features.append(linear.out_features)
-            self._layers.append(linear)
+        match self.kind:
+            case "cat":
+                linear = nn.Linear(self._in_features[-1], self._in_features[0])
+                self._in_features.append(linear.out_features)
+                self._layers.append(linear)
+            case _:
+                self._in_features.append(self._in_features[-1])
+                self._layers.append(nn.Identity())
         return self.out_features
 
     def forward(self, x: torch.Tensor, y: torch.Tensor, /) -> torch.Tensor:
         """Perform a sequential skip connection, first applying a skip
         connection to ``x`` and ``y``, and then sequentially applying skip
         connections to the output and the output of the next layer.
 
@@ -103,32 +104,30 @@
             A tensor with shape depending on
             :attr:`SequentialSkipConnection.fan_in` and
             :attr:`SequentialSkipConnection.kind`.
 
         """
         y = skip_connection(x, y, kind=self.kind)
         for i, layer in enumerate(self._layers):
-            if self.fan_in:
-                if not (i % 2):
-                    y = skip_connection(y, layer(y), kind=self.kind)
-                else:
-                    y = layer(y)
-            else:
+            if i % 2:
                 y = skip_connection(y, layer(y), kind=self.kind)
+            else:
+                y = layer(y)
         return y
 
     @property
     def in_features(self) -> int:
         """Return the first number of input features."""
         return self._in_features[0]
 
     @property
     def out_features(self) -> int:
         """Return the number of output features according to the number of input
         features, the kind of skip connection, and whether there's a fan-in
         layer.
 
         """
-        if self.fan_in:
-            return self._in_features[0]
-
-        return self._skip_features
+        match self.kind:
+            case "cat":
+                return self._in_features[0]
+            case _:
+                return self._skip_features
```

### Comparing `rlstack-0.0.0b1/src/rlstack/optimizer.py` & `rlstack-0.1.0/src/rlstack/optimizer.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/src/rlstack/policies/_feedforward.py` & `rlstack-0.1.0/src/rlstack/policies/_feedforward.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,19 +76,14 @@
 
     @property
     def device(self) -> Device:
         """Return the device the policy's model is on."""
         return next(self.model.parameters()).device
 
     @property
-    def feature_spec(self) -> TensorSpec:
-        """Return the feature spec defined in the model."""
-        return self.model.feature_spec
-
-    @property
     def observation_spec(self) -> TensorSpec:
         """Return the observation spec used for constructing the model."""
         return self.model.observation_spec
 
     def sample(
         self,
         batch: TensorDict,
@@ -157,14 +152,18 @@
 
         """
         if DataKeys.VIEWS in batch.keys():
             in_batch = batch[DataKeys.VIEWS]
         else:
             in_batch = self.model.apply_view_requirements(batch, kind=kind)
 
+        training = self.model.training
+        if deterministic and training:
+            self.model.eval()
+
         # This is the same mechanism within `torch.no_grad`
         # for enabling/disabling gradients.
         prev = torch.is_grad_enabled()
         torch.set_grad_enabled(requires_grad)
 
         features = self.model(in_batch)
 
@@ -183,13 +182,17 @@
                 out[DataKeys.LOGP] = dist.logp(actions)
         if return_values:
             out[DataKeys.VALUES] = self.model.value_function()
         if return_views:
             out[DataKeys.VIEWS] = in_batch
 
         torch.set_grad_enabled(prev)
+
+        if deterministic and training:
+            self.model.train()
+
         return out
 
     def to(self, device: Device, /) -> Self:
         """Move the policy and its attributes to ``device``."""
         self.model = self.model.to(device)
         return self
```

### Comparing `rlstack-0.0.0b1/src/rlstack/policies/_recurrent.py` & `rlstack-0.1.0/src/rlstack/policies/_recurrent.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,19 +73,14 @@
         return self.model.action_spec
 
     @property
     def device(self) -> Device:
         """Return the device the policy's model is on."""
         return next(self.model.parameters()).device
 
-    @property
-    def feature_spec(self) -> TensorSpec:
-        """Return the feature spec defined in the model."""
-        return self.model.feature_spec
-
     def init_states(self, n: int, /) -> TensorDict:
         """Return new recurrent states for the policy's model."""
         return self.model.init_states(n)
 
     @property
     def observation_spec(self) -> TensorSpec:
         """Return the observation spec used for constructing the model."""
@@ -150,14 +145,18 @@
             A tensordict containing AT LEAST actions sampled from the policy
             and a tensordict containing updated recurrent states. The returned
             recurrent states will only have shape ``[B, ...]`` WITHOUT a
             time dimension ``T`` since only the last recurrent state of the
             series should be returned.
 
         """
+        training = self.model.training
+        if deterministic and training:
+            self.model.eval()
+
         # This is the same mechanism within `torch.no_grad`
         # for enabling/disabling gradients.
         prev = torch.is_grad_enabled()
         torch.set_grad_enabled(requires_grad)
 
         B, T = batch.batch_size
         states = self.model.init_states(B).reshape(B, 1) if states is None else states
@@ -176,14 +175,18 @@
                 out[DataKeys.LOGP] = dist.logp(actions)
         if return_values:
             out[DataKeys.VALUES] = self.model.value_function()
         if keepdim:
             out = out.reshape(B, T)
 
         torch.set_grad_enabled(prev)
+
+        if deterministic and training:
+            self.model.train()
+
         return out, out_states
 
     @property
     def state_spec(self) -> CompositeSpec:
         """Return the policy's model's state spec for defining recurrent state
         dimensions.
```

### Comparing `rlstack-0.0.0b1/src/rlstack/schedulers.py` & `rlstack-0.1.0/src/rlstack/schedulers.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/src/rlstack/specs.py` & `rlstack-0.1.0/src/rlstack/specs.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/src/rlstack/trainer.py` & `rlstack-0.1.0/src/rlstack/trainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,20 +93,20 @@
                 domain randomization.
 
         Returns:
             The most recent train stats when the training is stopped due
             to a stop condition being satisfied.
 
         """
-        train_stats = self.train(env_config=env_config)
+        train_stats = self.step(env_config=env_config)
         while not any([condition(train_stats) for condition in self.stop_conditions]):
-            train_stats = self.train(env_config=env_config)
+            train_stats = self.step(env_config=env_config)
         return train_stats
 
-    def train(self, *, env_config: None | dict[str, Any] = None) -> TrainStats:
+    def step(self, *, env_config: None | dict[str, Any] = None) -> TrainStats:
         """Run a single training step, collecting environment transitions
         and updating the policy with those transitions.
 
         Args:
             env_config: Environment config override. Useful for scheduling
                 domain randomization.
```

### Comparing `rlstack-0.0.0b1/src/rlstack/views.py` & `rlstack-0.1.0/src/rlstack/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         """Apply the view to the last elements of ``T`` for all ``B`` in a batch
         of size ``[B, T, ...]`` such that the returned batch is of shape
         ``[B, size, ...]``.
 
         """
 
     @staticmethod
-    def burn_size(size: int, /) -> int:
+    def drop_size(size: int, /) -> int:
         """Return the amount of samples along the time or sequence dimension
         that's dropped for each batch element.
 
         This is used to determine batch size reshaping during training to make
         batch components have the same size.
 
         """
@@ -69,16 +69,17 @@
         padded) elements, and key ``"padding_mask"`` corresponding to booleans
         indicating which elements of ``"inputs"`` are padding.
 
     """
     B, T = x.shape[:2]
     pad = size - T
     if pad > 0:
-        padding = torch.zeros_like(x, device=x.device)[:, :pad, ...]
-        x = torch.cat([padding, x], 1)[:, -size:, ...]
+        F = x.shape[2:]
+        padding = torch.zeros(B, pad, *F, device=x.device, dtype=x.dtype)
+        x = torch.cat([padding, x], 1)
         padding_mask = torch.zeros(B, size, device=x.device, dtype=torch.bool)
         padding_mask[:, :pad] = True
     else:
         x = x[:, -size:, ...]
         padding_mask = torch.zeros(B, size, device=x.device, dtype=torch.bool)
     out = TensorDict({}, batch_size=[B, size], device=x.device)
     out[DataKeys.INPUTS] = x
@@ -101,16 +102,17 @@
     Returns:
         A tensordict with key ``"inputs"`` corresponding to the padded (or not
         padded) elements, and key "padding_mask" corresponding to booleans
         indicating which elements of ``"inputs"`` are padding.
 
     """
     B, T = x.shape[:2]
-    pad = RollingWindow.burn_size(size)
-    padding = torch.zeros_like(x)[:, :pad, ...]
+    F = x.shape[2:]
+    pad = RollingWindow.drop_size(size)
+    padding = torch.zeros(B, pad, *F, device=x.device, dtype=x.dtype)
     x = torch.cat([padding, x], 1)
     padding_mask = torch.zeros(B, T + pad, device=x.device, dtype=torch.bool)
     padding_mask[:, :pad] = True
     out = TensorDict({}, batch_size=[B, T + pad], device=x.device)
     out[DataKeys.INPUTS] = x
     out[DataKeys.PADDING_MASK] = padding_mask
     return out
@@ -214,17 +216,17 @@
             return x[:, -size:, ...]
         else:
             B, T = x.shape[:2]
             T_NEW = min(T, size)
             return x.apply(lambda x: x[:, -size:, ...], batch_size=[B, T_NEW])
 
     @staticmethod
-    def burn_size(size: int, /) -> int:
+    def drop_size(size: int, /) -> int:
         """This view doesn't perform any padding or masking and instead
-        burns-off a small amount of samples at the beginning of each
+        drops a small amount of samples at the beginning of each
         sequence in order to create sequences of the same length.
 
         """
         return size - 1
 
 
 class PaddedRollingWindow:
@@ -262,15 +264,15 @@
             ``[B * T, size, ...]``.
 
         """
         if isinstance(x, torch.Tensor):
             return RollingWindow.apply_all(pad_whole_sequence(x, size), size)
         else:
             B_OLD, T_OLD = x.shape[:2]
-            T_NEW = T_OLD + RollingWindow.burn_size(size)
+            T_NEW = T_OLD + RollingWindow.drop_size(size)
             return RollingWindow.apply_all(
                 x.apply(
                     lambda x: pad_whole_sequence(x, size), batch_size=[B_OLD, T_NEW]
                 ),
                 size,
             )
 
@@ -295,17 +297,17 @@
         if isinstance(x, torch.Tensor):
             return pad_last_sequence(x, size)
         else:
             B = x.size(0)
             return x.apply(lambda x: pad_last_sequence(x, size), batch_size=[B, size])
 
     @staticmethod
-    def burn_size(size: int, /) -> int:
+    def drop_size(size: int, /) -> int:
         """This view pads the beginning of each sequence and provides masking
-        to avoid burning-off samples.
+        to avoid dropping-off samples.
 
         """
         return size - size
 
 
 class ViewRequirement:
     """Batch preprocessing for creating overlapping time series or sequential
@@ -315,15 +317,14 @@
     This component is purely for convenience. Its functionality can optionally
     be replicated within an environment's observation function. However, because
     this functionaltiy is fairly common, it's recommended to use this
     component where simple time or sequence shifting is required for
     sequence-based observations.
 
     Args:
-        key: Key to apply the view requirement to for a given batch.
         shift: Number of additional previous samples in the time or sequence
             dimension to include in the view requirement's output.
         method: Method for applying a nonzero shift view requirement.
             Options include:
 
                 - "rolling_window": Create a rolling window over a tensor's
                   time or sequence dimension at the cost of dropping
@@ -332,20 +333,14 @@
                 - "padded_rolling_window": The same as "rolling_window" but
                   pad the beginning of each sequence to avoid dropping
                   samples and provide a mask indicating which element is
                   padding.
 
     """
 
-    #: Key to apply the view requirement to for a given batch. The key
-    #: can be any key that is compatible with a tensordict key.
-    #: E.g., a key can be a tuple of strings such that the item in the
-    #: batch is accessed like ``batch[("obs", "prices")]``.
-    key: str | tuple[str, ...]
-
     #: Method for applying a nonzero shift view requirement. Each method
     #: has its own advantage. Options include:
     #:
     #:  - ``"rolling_window"``: Create a rolling window over a tensor's
     #:      time or sequence dimension. This method is memory-efficient
     #:      and fast, but it drops samples in order for each new batch
     #:      element to have the same sequence size. Only use this method
@@ -361,88 +356,98 @@
     #: to include in the view requirement's output. E.g., if shift is ``1``,
     #: then the last two samples in the time or sequence dimension will be
     #: included for each batch element.
     shift: int
 
     def __init__(
         self,
-        key: str | tuple[str, ...],
-        /,
         *,
         shift: int = 0,
-        method: ViewMethod = "rolling_window",
+        method: ViewMethod = "padded_rolling_window",
     ) -> None:
-        self.key = key
         self.shift = shift
         if shift < 0:
             raise ValueError(f"{self.__class__.__name__} `shift` must be non-negative.")
         match method:
             case "rolling_window":
                 self.method = RollingWindow
             case "padded_rolling_window":
                 self.method = PaddedRollingWindow
 
-    def apply_all(self, batch: TensorDict, /) -> torch.Tensor | TensorDict:
+    def apply_all(
+        self, key: str | tuple[str, ...], batch: TensorDict, /
+    ) -> torch.Tensor | TensorDict:
         """Apply the view to all of the time or sequence elements.
 
         This method expands the elements of ``batch``'s first two dimensions
         together to allow parallel batching of `batch`'s elements in the batch
         and time or sequence dimension together. This method is typically
         used within a training loop and isn't typically used for sampling
         a policy's actions or environment interaction.
 
         Args:
+            key: Key to apply the view requirement to for a given batch. The key
+                can be any key that is compatible with a tensordict key.
+                E.g., a key can be a tuple of strings such that the item in the
+                batch is accessed like ``batch[("obs", "prices")]``.
             batch: Tensor dict of size ``[B, T, ...]`` where ``B`` is the batch
                 dimension, and ``T`` is the time or sequence dimension. ``B`` is
                 typically the number of parallel environments, and ``T`` is
                 typically the number of time steps or observations sampled
                 from each environment.
 
         Returns:
             A tensor or tensordict of size ``[B_NEW, self.shift, ...]``
             where ``B_NEW <= B * T``, depending on the view requirement method
             applied. In the case where :attr:`ViewRequirement.shift` is ``0``,
             the return tensor or tensordict has size ``[B * T, ...]``.
 
         """
-        item = batch[self.key]
+        item = batch[key]
 
         with torch.no_grad():
             if not self.shift:
                 if isinstance(item, torch.Tensor):
                     return item.flatten(end_dim=1)
                 else:
                     return item.reshape(-1)
 
             return self.method.apply_all(item, self.shift + 1)
 
-    def apply_last(self, batch: TensorDict, /) -> torch.Tensor | TensorDict:
+    def apply_last(
+        self, key: str | tuple[str, ...], batch: TensorDict, /
+    ) -> torch.Tensor | TensorDict:
         """Apply the view to just the last time or sequence elements.
 
         This method is typically used for sampling a model's features
         and eventual sampling of a policy's actions for parallel environments.
 
         Args:
+            key: Key to apply the view requirement to for a given batch. The key
+                can be any key that is compatible with a tensordict key.
+                E.g., a key can be a tuple of strings such that the item in the
+                batch is accessed like ``batch[("obs", "prices")]``.
             batch: Tensor dict of size ``[B, T, ...]`` where ``B`` is the batch
                 dimension, and ``T`` is the time or sequence dimension. ``B`` is
                 typically the number of parallel environments, and ``T`` is
                 typically the number of time steps or observations sampled
                 from each environment.
 
         Returns:
             A tensor or tensordict of size ``[B, self.shift + 1, ...]``. In the
             case where :attr:`ViewRequirement.shift` is ``0``, the returned
             tensor or tensordict has size ``[B, ...]``.
 
         """
-        item = batch[self.key]
+        item = batch[key]
 
         with torch.no_grad():
             if not self.shift:
                 return item[:, -1, ...]
 
             return self.method.apply_last(item, self.shift + 1)
 
     @property
-    def burn_size(self) -> int:
-        """Return the burn size of the underlying view requirement method."""
-        return self.method.burn_size(self.shift + 1)
+    def drop_size(self) -> int:
+        """Return the number of samples dropped when using the underlying view requirement method.
+        """
+        return self.method.drop_size(self.shift + 1)
```

### Comparing `rlstack-0.0.0b1/src/rlstack.egg-info/PKG-INFO` & `rlstack-0.1.0/src/rlstack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlstack
-Version: 0.0.0b1
+Version: 0.1.0
 Summary: A minimal RL library for infinite horizon tasks.
 Author: Andrew B.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -275,66 +275,14 @@
 
     from rlstack import Trainer
     from rlstack.env import DiscreteDummyEnv
 
     trainer = Trainer(DiscreteDummyEnv)
     trainer.run()
 
-Why rlstack?
-============
-
-**TL;DR: rlstack focuses on a niche subset of RL that simplifies the overall
-library while allowing fast and fully customizable environments, models, and
-action distributions.**
-
-There are many high quality, open-sourced RL libraries. Most of them take on the
-daunting task of being a monolithic, one-stop-shop for everything RL, attempting to
-support as many algorithms, environments, models, and compute capabilities as possible.
-Naturely, this monolothic goal has some drawbacks:
-
-* The software becomes more dense with each supported feature, making the library
-  all-the-more difficult to customize for a specific use case.
-* The software becomes less performant for a specific use case. RL practitioners
-  typically end up accepting the cost of transitioning to expensive and
-  difficult-to-manage compute clusters to get results faster.
-
-There's a handful of high quality, open-sourced RL libraries that tradeoff feature
-richness to reduce these drawbacks. However, each library still doesn't provide
-enough speed benefit to warrant the switch from a monolithic repo, or is still
-too complex to adapt to a specific use case.
-
-**rlstack** is a niche RL library that finds a goldilocks zone between the
-feature support and speed/complexity tradeoff by making some key assumptions:
-
-* Environments are highly parallelized and their parallelization is entirely
-  managed within the environment. This allows **rlstack** to ignore distributed
-  computing design considerations.
-* Environments are infinite horizon (i.e., they have no terminal conditions).
-  This allows **rlstack** to reset environments at the same, fixed horizon
-  intervals, greatly simplifying environment and algorithm implementations.
-* The only supported ML framework is PyTorch and the only supported algorithm
-  is PPO. This allows **rlstack** to ignore layers upon layers of abstraction,
-  greatly simplifying the overall library implementation.
-
-The end result is a minimal and high throughput library that can train policies
-to solve complex tasks on a single NVIDIA RTX 2080 within minutes.
-
-Unfortunately, this means **rlstack** doesn't support as many use cases as
-a monolithic RL library might. In fact, **rlstack** is probably a bad fit for
-your use case if:
-
-* Your environment isn't parallelizable.
-* Your environment must contain terminal conditions and can't be reformulated
-  as an infinite horizon task.
-* You want to use an ML framework that isn't PyTorch or you want to use an
-  algorithm that isn't a variant of PPO.
-
-However, if **rlstack** does fit your use case, it can do wonders for your
-RL workflow.
-
 Concepts
 ========
 
 **rlstack** is minimal in that it limits the number of interfaces required for
 training a policy with PPO, even for customized policies, without restrictions
 on observation and action specs, custom models, and custom action
 distributions.
@@ -519,14 +467,66 @@
 
     trainer = Trainer(
         DiscreteDummyEnv,
         stop_conditions=[Plateaus("returns/mean", rtol=0.05)],
     )
     trainer.run()
 
+Why rlstack?
+============
+
+**TL;DR: rlstack focuses on a niche subset of RL that simplifies the overall
+library while allowing fast and fully customizable environments, models, and
+action distributions.**
+
+There are many high quality, open-sourced RL libraries. Most of them take on the
+daunting task of being a monolithic, one-stop-shop for everything RL, attempting to
+support as many algorithms, environments, models, and compute capabilities as possible.
+Naturely, this monolothic goal has some drawbacks:
+
+* The software becomes more dense with each supported feature, making the library
+  all-the-more difficult to customize for a specific use case.
+* The software becomes less performant for a specific use case. RL practitioners
+  typically end up accepting the cost of transitioning to expensive and
+  difficult-to-manage compute clusters to get results faster.
+
+There's a handful of high quality, open-sourced RL libraries that tradeoff feature
+richness to reduce these drawbacks. However, each library still doesn't provide
+enough speed benefit to warrant the switch from a monolithic repo, or is still
+too complex to adapt to a specific use case.
+
+**rlstack** is a niche RL library that finds a goldilocks zone between the
+feature support and speed/complexity tradeoff by making some key assumptions:
+
+* Environments are highly parallelized and their parallelization is entirely
+  managed within the environment. This allows **rlstack** to ignore distributed
+  computing design considerations.
+* Environments are infinite horizon (i.e., they have no terminal conditions).
+  This allows **rlstack** to reset environments at the same, fixed horizon
+  intervals, greatly simplifying environment and algorithm implementations.
+* The only supported ML framework is PyTorch and the only supported algorithm
+  is PPO. This allows **rlstack** to ignore layers upon layers of abstraction,
+  greatly simplifying the overall library implementation.
+
+The end result is a minimal and high throughput library that can train policies
+to solve complex tasks on a single NVIDIA RTX 2080 within minutes.
+
+Unfortunately, this means **rlstack** doesn't support as many use cases as
+a monolithic RL library might. In fact, **rlstack** is probably a bad fit for
+your use case if:
+
+* Your environment isn't parallelizable.
+* Your environment must contain terminal conditions and can't be reformulated
+  as an infinite horizon task.
+* You want to use an ML framework that isn't PyTorch or you want to use an
+  algorithm that isn't a variant of PPO.
+
+However, if **rlstack** does fit your use case, it can do wonders for your
+RL workflow.
+
 Related Projects
 ================
 
 * `RL Games`_: RL Games is a high performance RL library built around popular
   environment protocols.
 * `RLlib`_: Ray's RLlib is the industry standard RL library that supports many
   popular RL algorithms. RLlib can scale RL workloads from your laptop all the
```

### Comparing `rlstack-0.0.0b1/src/rlstack.egg-info/SOURCES.txt` & `rlstack-0.1.0/src/rlstack.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -10,14 +10,21 @@
 docs/Makefile
 docs/conf.py
 docs/index.html
 docs/index.rst
 docs/make.bat
 docs/requirements.txt
 docs/_static/custom.css
+examples/algotrading/README.rst
+examples/algotrading/__main__.py
+examples/algotrading/env.py
+examples/algotrading/models/__init__.py
+examples/algotrading/models/lstm.py
+examples/algotrading/models/mlp.py
+examples/algotrading/models/transformer.py
 src/rlstack/__init__.py
 src/rlstack/_utils.py
 src/rlstack/conditions.py
 src/rlstack/data.py
 src/rlstack/distributions.py
 src/rlstack/env.py
 src/rlstack/optimizer.py
```

### Comparing `rlstack-0.0.0b1/tests/test_algorithms.py` & `rlstack-0.1.0/tests/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/tests/test_conditions.py` & `rlstack-0.1.0/tests/test_conditions.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/tests/test_nn/test_functional.py` & `rlstack-0.1.0/tests/test_nn/test_functional.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/tests/test_policies.py` & `rlstack-0.1.0/tests/test_policies.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/tests/test_schedulers.py` & `rlstack-0.1.0/tests/test_schedulers.py`

 * *Files identical despite different names*

### Comparing `rlstack-0.0.0b1/tests/test_views.py` & `rlstack-0.1.0/tests/test_views.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,97 +8,130 @@
     RollingWindow,
     ViewRequirement,
     pad_last_sequence,
     pad_whole_sequence,
     rolling_window,
 )
 
-SIZE = 2
-
 B = 4
 T = 1
+SIZE = 2
 TOTAL = B * T
 INPUTS = torch.tensor([[0, 0], [0, 1], [0, 2], [0, 3]]).float()
 PADDING_MASK = torch.tensor([[1, 0], [1, 0], [1, 0], [1, 0]]).bool()
 PAD_LAST_SEQUENCE_CASE_0 = (
     torch.arange(B * T).reshape(B, T).float(),
     TensorDict(
         {
             DataKeys.INPUTS: INPUTS,
             DataKeys.PADDING_MASK: PADDING_MASK,
         },
         batch_size=[B, SIZE],
     ),
+    SIZE,
 )
 
 B = 2
 T = 2
+SIZE = 2
 TOTAL = B * T * 2
 INPUTS = torch.arange(TOTAL).reshape(B, T, 2).float()
 PADDING_MASK = torch.zeros(B, SIZE).bool()
 PAD_LAST_SEQUENCE_CASE_1 = (
     torch.arange(TOTAL).reshape(B, T, 2).float(),
     TensorDict(
         {
             DataKeys.INPUTS: INPUTS,
             DataKeys.PADDING_MASK: PADDING_MASK,
         },
         batch_size=[B, SIZE],
     ),
+    SIZE,
 )
 
 B = 2
 T = 4
+SIZE = 2
 TOTAL = B * T
 INPUTS = torch.arange(TOTAL).reshape(B, T, 1, 1, 1)[:, -SIZE:, ...].float()
 PADDING_MASK = torch.zeros(B, SIZE).bool()
 PAD_LAST_SEQUENCE_CASE_2 = (
     torch.arange(TOTAL).reshape(B, T, 1, 1, 1).float(),
     TensorDict(
         {
             DataKeys.INPUTS: INPUTS,
             DataKeys.PADDING_MASK: PADDING_MASK,
         },
         batch_size=[B, SIZE],
     ),
+    SIZE,
+)
+
+B = 2
+T = 1
+SIZE = 3
+TOTAL = B * T
+INPUTS = torch.cat(
+    [
+        torch.zeros(B, SIZE - T, 1, 1, 1),
+        torch.arange(TOTAL).reshape(B, T, 1, 1, 1).float(),
+    ],
+    dim=1,
+)
+PADDING_MASK = torch.zeros(B, SIZE).bool()
+PADDING_MASK[:, : SIZE - T] = True
+PAD_LAST_SEQUENCE_CASE_3 = (
+    torch.arange(TOTAL).reshape(B, T, 1, 1, 1).float(),
+    TensorDict(
+        {
+            DataKeys.INPUTS: INPUTS,
+            DataKeys.PADDING_MASK: PADDING_MASK,
+        },
+        batch_size=[B, SIZE],
+    ),
+    SIZE,
 )
 
 
 @pytest.mark.parametrize(
-    "inputs,expected",
+    "inputs,expected,size",
     [
         PAD_LAST_SEQUENCE_CASE_0,
         PAD_LAST_SEQUENCE_CASE_1,
         PAD_LAST_SEQUENCE_CASE_2,
+        PAD_LAST_SEQUENCE_CASE_3,
     ],
 )
 def test_pad_last_sequence(
-    inputs: torch.Tensor, expected: torch.Tensor | TensorDict
+    inputs: torch.Tensor, expected: torch.Tensor | TensorDict, size: int
 ) -> None:
-    assert (pad_last_sequence(inputs, SIZE) == expected).all()
+    assert (pad_last_sequence(inputs, size) == expected).all()
 
 
 B = 4
 T = 1
+SIZE = 2
 TOTAL = B * T
 INPUTS = torch.tensor([[0, 0], [0, 1], [0, 2], [0, 3]]).float()
 PADDING_MASK = torch.tensor([[1, 0], [1, 0], [1, 0], [1, 0]]).bool()
 PAD_WHOLE_SEQUENCE_CASE_0 = (
     torch.arange(TOTAL).reshape(B, T).float(),
     TensorDict(
         {
             DataKeys.INPUTS: INPUTS,
             DataKeys.PADDING_MASK: PADDING_MASK,
         },
         batch_size=[B, T + (SIZE - 1)],
     ),
+    SIZE,
 )
 
 B = 2
 T = 2
+SIZE = 2
 TOTAL = B * T * 2
 INPUTS = torch.cat(
     [torch.zeros(B, (SIZE - 1), 2), torch.arange(TOTAL).reshape(B, T, 2)], dim=1
 ).float()
 PADDING_MASK = torch.zeros(B, T + (SIZE - 1)).bool()
 PADDING_MASK[:, : (SIZE - 1)] = True
 PAD_WHOLE_SEQUENCE_CASE_1 = (
@@ -106,18 +139,20 @@
     TensorDict(
         {
             DataKeys.INPUTS: INPUTS,
             DataKeys.PADDING_MASK: PADDING_MASK,
         },
         batch_size=[B, T + (SIZE - 1)],
     ),
+    SIZE,
 )
 
 B = 2
 T = 4
+SIZE = 2
 TOTAL = B * T
 INPUTS = torch.cat(
     [torch.zeros(B, (SIZE - 1), 1, 1, 1), torch.arange(TOTAL).reshape(B, T, 1, 1, 1)],
     dim=1,
 ).float()
 PADDING_MASK = torch.zeros(B, T + (SIZE - 1)).bool()
 PADDING_MASK[:, : (SIZE - 1)] = True
@@ -126,201 +161,278 @@
     TensorDict(
         {
             DataKeys.INPUTS: INPUTS,
             DataKeys.PADDING_MASK: PADDING_MASK,
         },
         batch_size=[B, T + (SIZE - 1)],
     ),
+    SIZE,
+)
+
+
+B = 2
+T = 1
+SIZE = 3
+TOTAL = B * T
+INPUTS = torch.cat(
+    [torch.zeros(B, (SIZE - 1), 1, 1, 1), torch.arange(TOTAL).reshape(B, T, 1, 1, 1)],
+    dim=1,
+).float()
+PADDING_MASK = torch.zeros(B, T + (SIZE - 1)).bool()
+PADDING_MASK[:, : (SIZE - T)] = True
+PAD_WHOLE_SEQUENCE_CASE_3 = (
+    torch.arange(TOTAL).reshape(B, T, 1, 1, 1).float(),
+    TensorDict(
+        {
+            DataKeys.INPUTS: INPUTS,
+            DataKeys.PADDING_MASK: PADDING_MASK,
+        },
+        batch_size=[B, T + (SIZE - 1)],
+    ),
+    SIZE,
 )
 
 
 @pytest.mark.parametrize(
-    "inputs,expected",
+    "inputs,expected,size",
     [
         PAD_WHOLE_SEQUENCE_CASE_0,
         PAD_WHOLE_SEQUENCE_CASE_1,
         PAD_WHOLE_SEQUENCE_CASE_2,
+        PAD_WHOLE_SEQUENCE_CASE_3,
     ],
 )
 def test_pad_whole_sequence(
-    inputs: torch.Tensor, expected: torch.Tensor | TensorDict
+    inputs: torch.Tensor, expected: torch.Tensor | TensorDict, size: int
 ) -> None:
-    assert (pad_whole_sequence(inputs, SIZE) == expected).all()
+    assert (pad_whole_sequence(inputs, size) == expected).all()
 
 
 B = 2
 T = 1
+SIZE = 2
 TOTAL = B * T
 INPUTS = TensorDict({"x": torch.arange(TOTAL).reshape(B, T).float()}, batch_size=[B, T])
 EXPECTED = TensorDict({}, batch_size=[B, T + SIZE - 1])
 EXPECTED["x"] = TensorDict({}, batch_size=[B, T + SIZE - 1])
-print(INPUTS["x"].shape)
 EXPECTED["x"][DataKeys.INPUTS] = torch.cat(
     [torch.zeros(B, SIZE - 1), INPUTS["x"]], dim=1
 )
 EXPECTED["x"][DataKeys.PADDING_MASK] = torch.zeros(B, T + SIZE - 1).bool()
 EXPECTED["x"][DataKeys.PADDING_MASK][:, : (SIZE - 1)] = True
 PADDED_ROLLING_WINDOW_APPLY_ALL_CASE_0 = (
     INPUTS,
     RollingWindow.apply_all(EXPECTED, SIZE),
+    SIZE,
 )
 
 B = 2
 T = 4
+SIZE = 2
 TOTAL = B * T
 INPUTS = TensorDict(
     {"x": torch.arange(TOTAL).reshape(B, T, 1).float()}, batch_size=[B, T]
 )
 EXPECTED = TensorDict({}, batch_size=[B, T + SIZE - 1])
 EXPECTED["x"] = TensorDict({}, batch_size=[B, T + SIZE - 1])
 EXPECTED["x"][DataKeys.INPUTS] = torch.cat(
     [torch.zeros(B, SIZE - 1, 1), INPUTS["x"]], dim=1
 )
 EXPECTED["x"][DataKeys.PADDING_MASK] = torch.zeros(B, T + SIZE - 1).bool()
 EXPECTED["x"][DataKeys.PADDING_MASK][:, : (SIZE - 1)] = True
 PADDED_ROLLING_WINDOW_APPLY_ALL_CASE_1 = (
     INPUTS,
     RollingWindow.apply_all(EXPECTED, SIZE),
+    SIZE,
 )
 
 
 @pytest.mark.parametrize(
-    "inputs,expected",
+    "inputs,expected,size",
     [
         PADDED_ROLLING_WINDOW_APPLY_ALL_CASE_0,
         PADDED_ROLLING_WINDOW_APPLY_ALL_CASE_1,
     ],
 )
 def test_padded_rolling_window_apply_all(
-    inputs: TensorDict, expected: TensorDict
+    inputs: TensorDict, expected: TensorDict, size: int
 ) -> None:
-    assert (PaddedRollingWindow.apply_all(inputs, SIZE) == expected).all()
+    assert (PaddedRollingWindow.apply_all(inputs, size) == expected).all()
 
 
 B = 2
 T = 1
+SIZE = 2
 TOTAL = B * T
 INPUTS = TensorDict({"x": torch.arange(TOTAL).reshape(B, T).float()}, batch_size=[B, T])
 EXPECTED = TensorDict({}, batch_size=[B, SIZE])
 EXPECTED["x"] = TensorDict({}, batch_size=[B, SIZE])
 EXPECTED["x"][DataKeys.INPUTS] = torch.cat(
     [torch.zeros(B, SIZE - 1), INPUTS["x"]], dim=1
 )
 EXPECTED["x"][DataKeys.PADDING_MASK] = torch.zeros(B, SIZE).bool()
 EXPECTED["x"][DataKeys.PADDING_MASK][:, : (SIZE - 1)] = True
 PADDED_ROLLING_WINDOW_APPLY_LAST_CASE_0 = (
     INPUTS,
     EXPECTED,
+    SIZE,
 )
 
 B = 2
 T = 4
+SIZE = 2
 TOTAL = B * T
 INPUTS = TensorDict(
     {"x": torch.arange(TOTAL).reshape(B, T, 1).float()}, batch_size=[B, T]
 )
 EXPECTED = TensorDict({}, batch_size=[B, SIZE])
 EXPECTED["x"] = TensorDict({}, batch_size=[B, SIZE])
 EXPECTED["x"][DataKeys.INPUTS] = INPUTS["x"][:, -SIZE:, ...]
 EXPECTED["x"][DataKeys.PADDING_MASK] = torch.zeros(B, SIZE).bool()
 PADDED_ROLLING_WINDOW_APPLY_LAST_CASE_1 = (
     INPUTS,
     EXPECTED,
+    SIZE,
+)
+
+B = 2
+T = 1
+SIZE = 3
+TOTAL = B * T
+INPUTS = TensorDict(
+    {"x": torch.arange(TOTAL).reshape(B, T, 1).float()}, batch_size=[B, T], device="cpu"
+)
+EXPECTED = TensorDict({}, batch_size=[B, SIZE], device="cpu")
+EXPECTED["x"] = TensorDict({}, batch_size=[B, SIZE])
+EXPECTED["x"][DataKeys.INPUTS] = torch.cat(
+    [torch.zeros(B, SIZE - T, 1), INPUTS["x"]], dim=1
+)
+EXPECTED["x"][DataKeys.PADDING_MASK] = torch.zeros(B, SIZE).bool()
+EXPECTED["x"][DataKeys.PADDING_MASK][:, : SIZE - T, ...] = True
+PADDED_ROLLING_WINDOW_APPLY_LAST_CASE_2 = (
+    INPUTS,
+    EXPECTED,
+    SIZE,
 )
 
 
 @pytest.mark.parametrize(
-    "inputs,expected",
+    "inputs,expected,size",
     [
         PADDED_ROLLING_WINDOW_APPLY_LAST_CASE_0,
         PADDED_ROLLING_WINDOW_APPLY_LAST_CASE_1,
+        PADDED_ROLLING_WINDOW_APPLY_LAST_CASE_2,
     ],
 )
 def test_padded_rolling_window_apply_last(
-    inputs: TensorDict, expected: TensorDict
+    inputs: TensorDict, expected: TensorDict, size: int
 ) -> None:
-    assert (PaddedRollingWindow.apply_last(inputs, SIZE) == expected).all()
+    assert (PaddedRollingWindow.apply_last(inputs, size) == expected).all()
 
 
+B = 2
+T = 4
+SIZE = 2
+TOTAL = B * T
 ROLLING_WINDOW_CASE_0 = (
-    torch.arange(8).reshape(2, 4).float(),
+    torch.arange(TOTAL).reshape(B, T).float(),
     torch.tensor([[[0, 1], [1, 2], [2, 3]], [[4, 5], [5, 6], [6, 7]]]).float(),
+    SIZE,
 )
 
+B = 2
+T = 4
+SIZE = 2
+TOTAL = B * T
 ROLLING_WINDOW_CASE_1 = (
-    torch.arange(8).reshape(2, 4, 1).float(),
+    torch.arange(TOTAL).reshape(B, T, 1).float(),
     torch.tensor(
         [[[[0], [1]], [[1], [2]], [[2], [3]]], [[[4], [5]], [[5], [6]], [[6], [7]]]]
     ).float(),
+    SIZE,
 )
 
 
 @pytest.mark.parametrize(
-    "inputs,expected",
+    "inputs,expected,size",
     [
         ROLLING_WINDOW_CASE_0,
         ROLLING_WINDOW_CASE_1,
     ],
 )
-def test_rolling_window(inputs: torch.Tensor, expected: torch.Tensor) -> None:
-    assert (rolling_window(inputs, SIZE) == expected).all()
+def test_rolling_window(
+    inputs: torch.Tensor, expected: torch.Tensor, size: int
+) -> None:
+    assert (rolling_window(inputs, size) == expected).all()
 
 
+SIZE = 2
 ROLLING_WINDOW_APPLY_ALL_CASE_0 = (
     ROLLING_WINDOW_CASE_0[0],
     ROLLING_WINDOW_CASE_0[1].reshape(-1, SIZE),
+    SIZE,
 )
 
+SIZE = 2
 ROLLING_WINDOW_APPLY_ALL_CASE_1 = (
     ROLLING_WINDOW_CASE_1[0],
     ROLLING_WINDOW_CASE_1[1].reshape(-1, SIZE, 1),
+    SIZE,
 )
 
 
 @pytest.mark.parametrize(
-    "inputs,expected",
+    "inputs,expected,size",
     [
         ROLLING_WINDOW_APPLY_ALL_CASE_0,
         ROLLING_WINDOW_APPLY_ALL_CASE_1,
     ],
 )
-def test_rolling_window_apply_all(inputs: torch.Tensor, expected: torch.Tensor) -> None:
-    assert (RollingWindow.apply_all(inputs, SIZE) == expected).all()
+def test_rolling_window_apply_all(
+    inputs: torch.Tensor, expected: torch.Tensor, size: int
+) -> None:
+    assert (RollingWindow.apply_all(inputs, size) == expected).all()
 
 
 B = 2
 T = 4
+SIZE = 2
 TOTAL = B * T
 INPUTS = TensorDict({"x": torch.arange(TOTAL).reshape(B, T).float()}, batch_size=[B, T])
 ROLLING_WINDOW_APPLY_LAST_CASE_0 = (
     INPUTS,
     INPUTS[:, -SIZE:, ...],
+    SIZE,
 )
 
 B = 2
 T = 4
+SIZE = 2
 TOTAL = B * T
 INPUTS = TensorDict(
     {"x": torch.arange(TOTAL).reshape(B, T, 1).float()}, batch_size=[B, T]
 )
 ROLLING_WINDOW_APPLY_LAST_CASE_1 = (
     INPUTS,
     INPUTS[:, -SIZE:, ...],
+    SIZE,
 )
 
 
 @pytest.mark.parametrize(
-    "inputs,expected",
+    "inputs,expected,size",
     [
         ROLLING_WINDOW_APPLY_LAST_CASE_0,
         ROLLING_WINDOW_APPLY_LAST_CASE_1,
     ],
 )
-def test_rolling_window_apply_last(inputs: TensorDict, expected: TensorDict) -> None:
-    assert (RollingWindow.apply_last(inputs, SIZE) == expected).all()
+def test_rolling_window_apply_last(
+    inputs: TensorDict, expected: TensorDict, size: int
+) -> None:
+    assert (RollingWindow.apply_last(inputs, size) == expected).all()
 
 
 B = 20
 T = 5
 TOTAL = B * T
 INPUTS = TensorDict({"x": torch.arange(TOTAL).reshape(B, T)}, batch_size=[B, T])
 VIEW_REQUIREMENT_APPLY_ALL_CASE_0 = (INPUTS, INPUTS.reshape(-1))
@@ -345,17 +457,17 @@
         VIEW_REQUIREMENT_APPLY_ALL_CASE_0,
         VIEW_REQUIREMENT_APPLY_ALL_CASE_1,
     ],
 )
 def test_view_requirement_apply_all(
     inputs: TensorDict, expected: torch.Tensor | TensorDict
 ) -> None:
-    view_requirement = ViewRequirement("x", shift=0)
+    view_requirement = ViewRequirement(shift=0)
     out = {}
-    out["x"] = view_requirement.apply_all(inputs)
+    out["x"] = view_requirement.apply_all("x", inputs)
     out_batch = TensorDict(out, batch_size=out["x"].size(0))
     assert (out_batch == expected).all()
 
 
 B = 20
 T = 5
 TOTAL = B * T
@@ -382,12 +494,12 @@
         VIEW_REQUIREMENT_APPLY_LAST_CASE_0,
         VIEW_REQUIREMENT_APPLY_LAST_CASE_1,
     ],
 )
 def test_view_requirement_apply_last(
     inputs: TensorDict, expected: torch.Tensor | TensorDict
 ) -> None:
-    view_requirement = ViewRequirement("x", shift=0)
+    view_requirement = ViewRequirement(shift=0)
     out = {}
-    out["x"] = view_requirement.apply_last(inputs)
+    out["x"] = view_requirement.apply_last("x", inputs)
     out_batch = TensorDict(out, batch_size=out["x"].size(0))
     assert (out_batch == expected).all()
```

