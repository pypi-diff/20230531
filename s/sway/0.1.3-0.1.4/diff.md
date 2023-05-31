# Comparing `tmp/sway-0.1.3.tar.gz` & `tmp/sway-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sway-0.1.3.tar", max compression
+gzip compressed data, was "sway-0.1.4.tar", max compression
```

## Comparing `sway-0.1.3.tar` & `sway-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      536 2023-05-28 18:21:43.172898 sway-0.1.3/README.md
--rw-r--r--   0        0        0      472 2023-05-28 18:37:50.474302 sway-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-28 18:15:05.590094 sway-0.1.3/sway/__init__.py
--rw-r--r--   0        0        0      120 2023-05-28 18:15:05.590559 sway-0.1.3/sway/__main__.py
--rw-r--r--   0        0        0        0 2023-05-27 19:01:22.081688 sway-0.1.3/sway/commands/__init__.py
--rw-r--r--   0        0        0     2295 2023-05-28 18:15:05.590839 sway-0.1.3/sway/commands/branch.py
--rw-r--r--   0        0        0        0 2023-05-27 19:01:22.082089 sway-0.1.3/sway/commands/build.py
--rw-r--r--   0        0        0     3493 2023-05-28 18:15:05.591100 sway-0.1.3/sway/commands/config.py
--rw-r--r--   0        0        0     1854 2023-05-28 18:15:05.591358 sway-0.1.3/sway/main.py
--rw-r--r--   0        0        0        0 2023-05-27 19:01:22.082574 sway-0.1.3/sway/utils/__init__.py
--rw-r--r--   0        0        0      894 2023-05-28 18:15:05.591692 sway-0.1.3/sway/utils/yaml.py
--rw-r--r--   0        0        0     1107 1970-01-01 00:00:00.000000 sway-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      959 2023-05-31 19:15:42.520283 sway-0.1.4/README.md
+-rw-r--r--   0        0        0      472 2023-05-31 19:16:30.248641 sway-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-28 18:15:05.590094 sway-0.1.4/sway/__init__.py
+-rw-r--r--   0        0        0      120 2023-05-28 18:15:05.590559 sway-0.1.4/sway/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-27 19:01:22.081688 sway-0.1.4/sway/commands/__init__.py
+-rw-r--r--   0        0        0     2295 2023-05-28 18:15:05.590839 sway-0.1.4/sway/commands/branch.py
+-rw-r--r--   0        0        0     1335 2023-05-31 19:11:54.088762 sway-0.1.4/sway/commands/build.py
+-rw-r--r--   0        0        0     3493 2023-05-28 18:15:05.591100 sway-0.1.4/sway/commands/config.py
+-rw-r--r--   0        0        0     2813 2023-05-31 19:11:54.088963 sway-0.1.4/sway/main.py
+-rw-r--r--   0        0        0        0 2023-05-27 19:01:22.082574 sway-0.1.4/sway/utils/__init__.py
+-rw-r--r--   0        0        0      108 2023-05-30 09:29:07.991862 sway-0.1.4/sway/utils/config.py
+-rw-r--r--   0        0        0      894 2023-05-28 18:15:05.591692 sway-0.1.4/sway/utils/yaml.py
+-rw-r--r--   0        0        0     1530 1970-01-01 00:00:00.000000 sway-0.1.4/PKG-INFO
```

### Comparing `sway-0.1.3/sway/commands/branch.py` & `sway-0.1.4/sway/commands/branch.py`

 * *Files identical despite different names*

### Comparing `sway-0.1.3/sway/commands/config.py` & `sway-0.1.4/sway/commands/config.py`

 * *Files identical despite different names*

### Comparing `sway-0.1.3/sway/utils/yaml.py` & `sway-0.1.4/sway/utils/yaml.py`

 * *Files identical despite different names*

