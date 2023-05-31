# Comparing `tmp/ip_rotator-1.0.1.tar.gz` & `tmp/ip_rotator-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ip_rotator-1.0.1.tar", last modified: Tue Dec 20 15:11:32 2022, max compression
+gzip compressed data, was "ip_rotator-1.2.tar", last modified: Wed May 31 17:28:04 2023, max compression
```

## Comparing `ip_rotator-1.0.1.tar` & `ip_rotator-1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:11:32.483890 ip_rotator-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:11:32.479890 ip_rotator-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:11:32.483890 ip_rotator-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2022-12-20 15:11:11.000000 ip_rotator-1.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2022-12-20 15:11:11.000000 ip_rotator-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2022-12-20 15:11:32.483890 ip_rotator-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2022-12-20 15:11:11.000000 ip_rotator-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:11:32.483890 ip_rotator-1.0.1/ip_rotator/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2022-12-20 15:11:11.000000 ip_rotator-1.0.1/ip_rotator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2022-12-20 15:11:11.000000 ip_rotator-1.0.1/ip_rotator/ip_rotator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:11:32.483890 ip_rotator-1.0.1/ip_rotator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2022-12-20 15:11:32.000000 ip_rotator-1.0.1/ip_rotator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2022-12-20 15:11:32.000000 ip_rotator-1.0.1/ip_rotator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 15:11:32.000000 ip_rotator-1.0.1/ip_rotator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2022-12-20 15:11:32.000000 ip_rotator-1.0.1/ip_rotator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-20 15:11:32.000000 ip_rotator-1.0.1/ip_rotator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      717 2022-12-20 15:11:11.000000 ip_rotator-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 15:11:32.483890 ip_rotator-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:11:32.483890 ip_rotator-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 15:11:11.000000 ip_rotator-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2022-12-20 15:11:11.000000 ip_rotator-1.0.1/tests/ip_rotator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:28:04.892886 ip_rotator-1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:28:04.888886 ip_rotator-1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:28:04.888886 ip_rotator-1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-31 17:27:50.000000 ip_rotator-1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-31 17:27:50.000000 ip_rotator-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-31 17:28:04.892886 ip_rotator-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-31 17:27:50.000000 ip_rotator-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:28:04.888886 ip_rotator-1.2/ip_rotator/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-31 17:27:50.000000 ip_rotator-1.2/ip_rotator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-31 17:27:50.000000 ip_rotator-1.2/ip_rotator/ip_rotator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:28:04.892886 ip_rotator-1.2/ip_rotator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-31 17:28:04.000000 ip_rotator-1.2/ip_rotator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-31 17:28:04.000000 ip_rotator-1.2/ip_rotator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:28:04.000000 ip_rotator-1.2/ip_rotator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-31 17:28:04.000000 ip_rotator-1.2/ip_rotator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 17:28:04.000000 ip_rotator-1.2/ip_rotator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-31 17:27:50.000000 ip_rotator-1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 17:28:04.892886 ip_rotator-1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:28:04.892886 ip_rotator-1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:27:50.000000 ip_rotator-1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-31 17:27:50.000000 ip_rotator-1.2/tests/ip_rotator.py
```

### Comparing `ip_rotator-1.0.1/.github/workflows/python-publish.yml` & `ip_rotator-1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ip_rotator-1.0.1/LICENSE` & `ip_rotator-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ip_rotator-1.0.1/PKG-INFO` & `ip_rotator-1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ip_rotator
-Version: 1.0.1
+Version: 1.2
 Summary: Hides Your Ip address in https requests
 Author-email: Anish <anishshakthivelnadar@gmail.com>
 Project-URL: Homepage, https://github.com/Anish0612/ip_rotator
 Project-URL: Bug Tracker, https://github.com/Anish0612/ip_rotator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ip_rotator-1.0.1/README.md` & `ip_rotator-1.2/README.md`

 * *Files identical despite different names*

### Comparing `ip_rotator-1.0.1/ip_rotator/ip_rotator.py` & `ip_rotator-1.2/ip_rotator/ip_rotator.py`

 * *Files identical despite different names*

### Comparing `ip_rotator-1.0.1/ip_rotator.egg-info/PKG-INFO` & `ip_rotator-1.2/ip_rotator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ip-rotator
-Version: 1.0.1
+Version: 1.2
 Summary: Hides Your Ip address in https requests
 Author-email: Anish <anishshakthivelnadar@gmail.com>
 Project-URL: Homepage, https://github.com/Anish0612/ip_rotator
 Project-URL: Bug Tracker, https://github.com/Anish0612/ip_rotator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ip_rotator-1.0.1/pyproject.toml` & `ip_rotator-1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ip_rotator-1.0.1/tests/ip_rotator.py` & `ip_rotator-1.2/tests/ip_rotator.py`

 * *Files identical despite different names*

