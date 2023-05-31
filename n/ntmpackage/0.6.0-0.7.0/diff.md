# Comparing `tmp/ntmpackage-0.6.0.tar.gz` & `tmp/ntmpackage-0.7.0.tar.gz`

## Comparing `ntmpackage-0.6.0.tar` & `ntmpackage-0.7.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/.DS_Store
--rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/ntmpackage/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/ntmpackage/__init__.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/ntmpackage/pkg_1/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/ntmpackage/pkg_1/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/ntmpackage/pkg_1/opt_fwk/__init__.py
--rwxr-xr-x   0        0        0      209 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/ntmpackage/pkg_1/opt_fwk/main1.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/ntmpackage/pkg_2/__init__.py
--rwxr-xr-x   0        0        0      116 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/ntmpackage/pkg_2/main2.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/LICENSE
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/README.md
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ntmpackage-0.7.0/.DS_Store
+-rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 ntmpackage-0.7.0/ntmpackage/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ntmpackage-0.7.0/ntmpackage/__init__.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ntmpackage-0.7.0/ntmpackage/pkg_1/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ntmpackage-0.7.0/ntmpackage/pkg_1/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ntmpackage-0.7.0/ntmpackage/pkg_1/opt_fwk/__init__.py
+-rwxr-xr-x   0        0        0      209 2020-02-02 00:00:00.000000 ntmpackage-0.7.0/ntmpackage/pkg_1/opt_fwk/main1.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ntmpackage-0.7.0/ntmpackage/pkg_2/__init__.py
+-rwxr-xr-x   0        0        0      116 2020-02-02 00:00:00.000000 ntmpackage-0.7.0/ntmpackage/pkg_2/main2.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 ntmpackage-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 ntmpackage-0.7.0/README.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 ntmpackage-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 ntmpackage-0.7.0/PKG-INFO
```

### Comparing `ntmpackage-0.6.0/.DS_Store` & `ntmpackage-0.7.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `ntmpackage-0.6.0/ntmpackage/.DS_Store` & `ntmpackage-0.7.0/ntmpackage/.DS_Store`

 * *Files identical despite different names*

### Comparing `ntmpackage-0.6.0/ntmpackage/pkg_1/.DS_Store` & `ntmpackage-0.7.0/ntmpackage/pkg_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `ntmpackage-0.6.0/LICENSE` & `ntmpackage-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ntmpackage-0.6.0/README.md` & `ntmpackage-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ntmpackage-0.6.0/pyproject.toml` & `ntmpackage-0.7.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ntmpackage"
-version = "0.6.0"
+version = "0.7.0"
 authors = [
   { name="Nara Torres Moreira", email="nara.moreira@astrazeneca.com" },
 ]
 description = "Nara's first package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -17,8 +17,8 @@
 "Homepage" = "https://github.com/AZ-AI/opt-tools"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
-packages = ["ntmpackage/pkg_1/opt_fwk"]
+packages = ["ntmpackage/pkg_1/opt_fwk", "ntmpackage"]
```

### Comparing `ntmpackage-0.6.0/PKG-INFO` & `ntmpackage-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntmpackage
-Version: 0.6.0
+Version: 0.7.0
 Summary: Nara's first package
 Project-URL: Homepage, https://github.com/AZ-AI/opt-tools
 Author-email: Nara Torres Moreira <nara.moreira@astrazeneca.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

