# Comparing `tmp/cxbind-0.1.0.tar.gz` & `tmp/cxbind-0.1.1.tar.gz`

## Comparing `cxbind-0.1.0.tar` & `cxbind-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 cxbind-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 cxbind-0.1.0/CMakeLists.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 cxbind-0.1.0/requirements.txt
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cxbind-0.1.0/.procure/__init__.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cxbind-0.1.0/cxbind/__about__.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 cxbind-0.1.0/cxbind/__init__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 cxbind-0.1.0/cxbind/__main__.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cxbind-0.1.0/cxbind/actions.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 cxbind-0.1.0/cxbind/context.py
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 cxbind-0.1.0/cxbind/entry.py
--rw-r--r--   0        0        0    14667 2020-02-02 00:00:00.000000 cxbind-0.1.0/cxbind/generator.py
--rw-r--r--   0        0        0    11776 2020-02-02 00:00:00.000000 cxbind-0.1.0/cxbind/generator_base.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 cxbind-0.1.0/cxbind/runner.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 cxbind-0.1.0/cxbind/yaml.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 cxbind-0.1.0/cxbind/clang/__init__.py
--rw-r--r--   0        0        0   134752 2020-02-02 00:00:00.000000 cxbind-0.1.0/cxbind/clang/cindex.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 cxbind-0.1.0/cxbind/clang/enumerations.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 cxbind-0.1.0/cxbind/cli/__init__.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 cxbind-0.1.0/cxbind/include/cxbind/cxbind.h
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 cxbind-0.1.0/cxbind/share/cmake/cxbind/cxbindConfig.cmake
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 cxbind-0.1.0/cxbind/share/cmake/cxbind/cxbindConfigVersion.cmake
--rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 cxbind-0.1.0/cxbind/share/cmake/cxbind/cxbindTargets.cmake
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 cxbind-0.1.0/cxbind/share/cmake/cxbind/cxbindTools.cmake
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 cxbind-0.1.0/include/cxbind/cxbind.h
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cxbind-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cxbind-0.1.0/tests/test_cxbind.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 cxbind-0.1.0/tools/cxbindConfig.cmake.in
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 cxbind-0.1.0/tools/cxbindTools.cmake
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 cxbind-0.1.0/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 cxbind-0.1.0/LICENSE
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 cxbind-0.1.0/README.md
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 cxbind-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 cxbind-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 cxbind-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 cxbind-0.1.1/CMakeLists.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 cxbind-0.1.1/requirements.txt
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cxbind-0.1.1/.procure/__init__.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cxbind-0.1.1/cxbind/__about__.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 cxbind-0.1.1/cxbind/__init__.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 cxbind-0.1.1/cxbind/__main__.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cxbind-0.1.1/cxbind/actions.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 cxbind-0.1.1/cxbind/context.py
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 cxbind-0.1.1/cxbind/entry.py
+-rw-r--r--   0        0        0    14667 2020-02-02 00:00:00.000000 cxbind-0.1.1/cxbind/generator.py
+-rw-r--r--   0        0        0    11776 2020-02-02 00:00:00.000000 cxbind-0.1.1/cxbind/generator_base.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 cxbind-0.1.1/cxbind/runner.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 cxbind-0.1.1/cxbind/yaml.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 cxbind-0.1.1/cxbind/clang/__init__.py
+-rw-r--r--   0        0        0   134752 2020-02-02 00:00:00.000000 cxbind-0.1.1/cxbind/clang/cindex.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 cxbind-0.1.1/cxbind/clang/enumerations.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 cxbind-0.1.1/cxbind/cli/__init__.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 cxbind-0.1.1/cxbind/include/cxbind/cxbind.h
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 cxbind-0.1.1/cxbind/share/cmake/cxbind/cxbindConfig.cmake
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 cxbind-0.1.1/cxbind/share/cmake/cxbind/cxbindConfigVersion.cmake
+-rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 cxbind-0.1.1/cxbind/share/cmake/cxbind/cxbindTargets.cmake
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 cxbind-0.1.1/cxbind/share/cmake/cxbind/cxbindTools.cmake
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 cxbind-0.1.1/include/cxbind/cxbind.h
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cxbind-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cxbind-0.1.1/tests/test_cxbind.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 cxbind-0.1.1/tools/cxbindConfig.cmake.in
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 cxbind-0.1.1/tools/cxbindTools.cmake
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 cxbind-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 cxbind-0.1.1/LICENSE
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 cxbind-0.1.1/README.md
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 cxbind-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 cxbind-0.1.1/PKG-INFO
```

### Comparing `cxbind-0.1.0/CMakeLists.txt` & `cxbind-0.1.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cxbind-0.1.0/cxbind/__init__.py` & `cxbind-0.1.1/cxbind/__init__.py`

 * *Files identical despite different names*

### Comparing `cxbind-0.1.0/cxbind/actions.py` & `cxbind-0.1.1/cxbind/actions.py`

 * *Files identical despite different names*

### Comparing `cxbind-0.1.0/cxbind/context.py` & `cxbind-0.1.1/cxbind/context.py`

 * *Files identical despite different names*

### Comparing `cxbind-0.1.0/cxbind/entry.py` & `cxbind-0.1.1/cxbind/entry.py`

 * *Files identical despite different names*

### Comparing `cxbind-0.1.0/cxbind/generator.py` & `cxbind-0.1.1/cxbind/generator.py`

 * *Files identical despite different names*

### Comparing `cxbind-0.1.0/cxbind/generator_base.py` & `cxbind-0.1.1/cxbind/generator_base.py`

 * *Files identical despite different names*

### Comparing `cxbind-0.1.0/cxbind/runner.py` & `cxbind-0.1.1/cxbind/runner.py`

 * *Files identical despite different names*

### Comparing `cxbind-0.1.0/cxbind/yaml.py` & `cxbind-0.1.1/cxbind/yaml.py`

 * *Files identical despite different names*

### Comparing `cxbind-0.1.0/cxbind/clang/__init__.py` & `cxbind-0.1.1/cxbind/clang/__init__.py`

 * *Files identical despite different names*

### Comparing `cxbind-0.1.0/cxbind/clang/cindex.py` & `cxbind-0.1.1/cxbind/clang/cindex.py`

 * *Files identical despite different names*

### Comparing `cxbind-0.1.0/cxbind/clang/enumerations.py` & `cxbind-0.1.1/cxbind/clang/enumerations.py`

 * *Files identical despite different names*

### Comparing `cxbind-0.1.0/cxbind/include/cxbind/cxbind.h` & `cxbind-0.1.1/cxbind/include/cxbind/cxbind.h`

 * *Files identical despite different names*

### Comparing `cxbind-0.1.0/cxbind/share/cmake/cxbind/cxbindConfig.cmake` & `cxbind-0.1.1/cxbind/share/cmake/cxbind/cxbindConfig.cmake`

 * *Files identical despite different names*

### Comparing `cxbind-0.1.0/cxbind/share/cmake/cxbind/cxbindConfigVersion.cmake` & `cxbind-0.1.1/cxbind/share/cmake/cxbind/cxbindConfigVersion.cmake`

 * *Files identical despite different names*

### Comparing `cxbind-0.1.0/cxbind/share/cmake/cxbind/cxbindTargets.cmake` & `cxbind-0.1.1/cxbind/share/cmake/cxbind/cxbindTargets.cmake`

 * *Files identical despite different names*

### Comparing `cxbind-0.1.0/include/cxbind/cxbind.h` & `cxbind-0.1.1/include/cxbind/cxbind.h`

 * *Files identical despite different names*

### Comparing `cxbind-0.1.0/tools/cxbindConfig.cmake.in` & `cxbind-0.1.1/tools/cxbindConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `cxbind-0.1.0/.gitignore` & `cxbind-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cxbind-0.1.0/LICENSE` & `cxbind-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cxbind-0.1.0/pyproject.toml` & `cxbind-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cxbind"
-version = "0.1.0"
+version = "0.1.1"
 description = 'pybind11 binding generator'
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = []
 authors = [{ name = "Kurtis Fields", email = "kurtisfields@gmail.com" }]
 classifiers = [
@@ -19,20 +19,18 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 dependencies = [
-    "click ==8.1.3",
-    "toml ==0.10.2",
-    #clang = "^14.0"
+    "click >=8.1.3",
     "Jinja2 ==3.1.2",
-    "loguru ==0.6.0",
-    "pyyaml ==6.0"
+    "loguru >=0.7.0",
+    "pyyaml >=6.0"
 ]
 
 #dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = ["black ~=22.12.0"]
 test = ["pytest ~=7.2.1"]
```

### Comparing `cxbind-0.1.0/PKG-INFO` & `cxbind-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxbind
-Version: 0.1.0
+Version: 0.1.1
 Summary: pybind11 binding generator
 Project-URL: homepage, https://github.com/crunge/cxbind
 Project-URL: documentation, https://crungelab.github.io/cxbind/
 Project-URL: repository, https://github.com/crungelab/cxbind
 Project-URL: changelog, https://github.com/crungelab/cxbind/blob/main/CHANGELOG.md
 Author-email: Kurtis Fields <kurtisfields@gmail.com>
 License: MIT License
@@ -34,19 +34,18 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
-Requires-Dist: click==8.1.3
+Requires-Dist: click>=8.1.3
 Requires-Dist: jinja2==3.1.2
-Requires-Dist: loguru==0.6.0
-Requires-Dist: pyyaml==6.0
-Requires-Dist: toml==0.10.2
+Requires-Dist: loguru>=0.7.0
+Requires-Dist: pyyaml>=6.0
 Provides-Extra: dev
 Requires-Dist: black~=22.12.0; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest~=7.2.1; extra == 'test'
 Description-Content-Type: text/markdown
 
 # CxBind :chains:
```

