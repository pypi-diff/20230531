# Comparing `tmp/ip_rotator-1.2.tar.gz` & `tmp/ip_rotator-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ip_rotator-1.2.tar", last modified: Wed May 31 17:28:04 2023, max compression
+gzip compressed data, was "ip_rotator-1.3.tar", last modified: Wed May 31 19:41:25 2023, max compression
```

## Comparing `ip_rotator-1.2.tar` & `ip_rotator-1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:28:04.892886 ip_rotator-1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:28:04.888886 ip_rotator-1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:28:04.888886 ip_rotator-1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-31 17:27:50.000000 ip_rotator-1.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-31 17:27:50.000000 ip_rotator-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-31 17:28:04.892886 ip_rotator-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-31 17:27:50.000000 ip_rotator-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:28:04.888886 ip_rotator-1.2/ip_rotator/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-31 17:27:50.000000 ip_rotator-1.2/ip_rotator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-31 17:27:50.000000 ip_rotator-1.2/ip_rotator/ip_rotator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:28:04.892886 ip_rotator-1.2/ip_rotator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-31 17:28:04.000000 ip_rotator-1.2/ip_rotator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-31 17:28:04.000000 ip_rotator-1.2/ip_rotator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:28:04.000000 ip_rotator-1.2/ip_rotator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-31 17:28:04.000000 ip_rotator-1.2/ip_rotator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 17:28:04.000000 ip_rotator-1.2/ip_rotator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-31 17:27:50.000000 ip_rotator-1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 17:28:04.892886 ip_rotator-1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:28:04.892886 ip_rotator-1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 17:27:50.000000 ip_rotator-1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-31 17:27:50.000000 ip_rotator-1.2/tests/ip_rotator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:41:25.757305 ip_rotator-1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:41:25.757305 ip_rotator-1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:41:25.757305 ip_rotator-1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-31 19:41:13.000000 ip_rotator-1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-31 19:41:13.000000 ip_rotator-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-31 19:41:25.757305 ip_rotator-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-31 19:41:13.000000 ip_rotator-1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:41:25.757305 ip_rotator-1.3/ip_rotator/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-31 19:41:13.000000 ip_rotator-1.3/ip_rotator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-31 19:41:13.000000 ip_rotator-1.3/ip_rotator/ip_rotator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:41:25.757305 ip_rotator-1.3/ip_rotator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-31 19:41:25.000000 ip_rotator-1.3/ip_rotator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-31 19:41:25.000000 ip_rotator-1.3/ip_rotator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:41:25.000000 ip_rotator-1.3/ip_rotator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-31 19:41:25.000000 ip_rotator-1.3/ip_rotator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 19:41:25.000000 ip_rotator-1.3/ip_rotator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-31 19:41:13.000000 ip_rotator-1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 19:41:25.757305 ip_rotator-1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:41:25.757305 ip_rotator-1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:41:13.000000 ip_rotator-1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-31 19:41:13.000000 ip_rotator-1.3/tests/ip_rotator.py
```

### Comparing `ip_rotator-1.2/.github/workflows/python-publish.yml` & `ip_rotator-1.3/.github/workflows/python-publish.yml`

 * *Files 5% similar despite different names*

```diff
@@ -33,7 +33,12 @@
       - name: Build package
         run: python -m build
       - name: Publish package
         uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
+      - name: Publish package 2
+        uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
+        with:
+          user: __token__
+          password: ${{ secrets.PYPI_API_TOKEN_2 }}
```

### Comparing `ip_rotator-1.2/LICENSE` & `ip_rotator-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ip_rotator-1.2/PKG-INFO` & `ip_rotator-1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ip_rotator
-Version: 1.2
-Summary: Hides Your Ip address in https requests
+Version: 1.3
+Summary: Rotate IP In Http Request
 Author-email: Anish <anishshakthivelnadar@gmail.com>
 Project-URL: Homepage, https://github.com/Anish0612/ip_rotator
 Project-URL: Bug Tracker, https://github.com/Anish0612/ip_rotator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `ip_rotator-1.2/README.md` & `ip_rotator-1.3/README.md`

 * *Files identical despite different names*

### Comparing `ip_rotator-1.2/ip_rotator/ip_rotator.py` & `ip_rotator-1.3/ip_rotator/ip_rotator.py`

 * *Files identical despite different names*

### Comparing `ip_rotator-1.2/ip_rotator.egg-info/PKG-INFO` & `ip_rotator-1.3/ip_rotator.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ip-rotator
-Version: 1.2
-Summary: Hides Your Ip address in https requests
+Version: 1.3
+Summary: Rotate IP In Http Request
 Author-email: Anish <anishshakthivelnadar@gmail.com>
 Project-URL: Homepage, https://github.com/Anish0612/ip_rotator
 Project-URL: Bug Tracker, https://github.com/Anish0612/ip_rotator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `ip_rotator-1.2/pyproject.toml` & `ip_rotator-1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "ip_rotator"
 authors = [
   { name="Anish", email="anishshakthivelnadar@gmail.com" },
 ]
-description = "Hides Your Ip address in https requests"
+description = "Rotate IP In Http Request"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `ip_rotator-1.2/tests/ip_rotator.py` & `ip_rotator-1.3/tests/ip_rotator.py`

 * *Files identical despite different names*

