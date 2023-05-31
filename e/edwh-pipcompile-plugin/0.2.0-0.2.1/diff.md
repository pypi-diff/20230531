# Comparing `tmp/edwh_pipcompile_plugin-0.2.0.tar.gz` & `tmp/edwh_pipcompile_plugin-0.2.1.tar.gz`

## Comparing `edwh_pipcompile_plugin-0.2.0.tar` & `edwh_pipcompile_plugin-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,10 @@
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/requirements-dev.in
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/requirements-dev.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/src/edwh_pipcompile_plugin/__about__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/src/edwh_pipcompile_plugin/__init__.py
--rw-r--r--   0        0        0    10672 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/src/edwh_pipcompile_plugin/pipcompile_plugin.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/README.md
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.1/src/edwh_pipcompile_plugin/__about__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.1/src/edwh_pipcompile_plugin/__init__.py
+-rw-r--r--   0        0        0    10612 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.1/src/edwh_pipcompile_plugin/pipcompile_plugin.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.1/README.md
+-rw-r--r--   0        0        0     4050 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 edwh_pipcompile_plugin-0.2.1/PKG-INFO
```

### Comparing `edwh_pipcompile_plugin-0.2.0/CHANGELOG.md` & `edwh_pipcompile_plugin-0.2.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.2.1 (2023-05-31)
+
+
 ## v0.2.0 (2023-05-08)
 ### Feature
 * Import main tasks to __init__ so this plugin can be used as a library ([`61611cf`](https://github.com/educationwarehouse/edwh-pipcompile-plugin/commit/61611cf0f795221615e4e802bf8209280b1ef854))
 
 ## v0.1.9 (2023-05-04)
 ### Fix
 * **compile:** Reverting change ([`6651cd7`](https://github.com/educationwarehouse/edwh-pipcompile-plugin/commit/6651cd77a07dfe9a7befee5bea39bfeff61ae061))
```

### Comparing `edwh_pipcompile_plugin-0.2.0/src/edwh_pipcompile_plugin/pipcompile_plugin.py` & `edwh_pipcompile_plugin-0.2.1/src/edwh_pipcompile_plugin/pipcompile_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,19 +185,15 @@
     """
 
     if directory and str(directory).endswith(".in"):
         # already one file!
         yield str(directory)
         return
 
-    if directory:
-        _glob = f"{directory}/*.in"
-    else:
-        _glob = "*.in"
-
+    _glob = f"{directory}/*.in" if directory else "*.in"
     yield from glob.glob(_glob)
 
 
 def extract_package_info(package: str) -> tuple[str, str, str]:
     """
     From a possibly pinned package string (e.g. edwh-ghost==0.01)
     extract the package info as a tuple of name, operator, version
@@ -332,17 +328,15 @@
                 )
                 continue
 
             if force or (operator and version):
                 with open(file, "w") as f:
                     f.write(reg.sub(package, contents))
             elif dep_version := dependency[0][2]:
-                warn(
-                    f"{package} is pinned to {dep_version} in {file}. Use --force to upgrade anyway."
-                )
+                warn(f"{package} is pinned to {dep_version} in {file}. Use --force to upgrade anyway.")
                 continue
             # arg = f'--upgrade-package "{package}"'
             args["upgrade-package"] = package
 
             success(f"Upgrading {package} in {file}")
         else:
             success(f"Upgrading all in {file}")
@@ -370,18 +364,17 @@
         pypi_server (str): which server to get files from?
 
     Examples:
         pip.remove . black
         pip.remove . --package black
     """
     _package, *_ = extract_package_info(package)
-    files = _find_infiles(Path(path))
 
-    if not files:
-        files = _find_infiles()
+    # first try with path, then without
+    files = _find_infiles(Path(path)) or _find_infiles()
 
     for file in files:
         with open(file, "r") as f:
             contents = f.read()
 
         reg = compile_package_re(_package)
         if not reg.search(contents):
```

### Comparing `edwh_pipcompile_plugin-0.2.0/LICENSE.txt` & `edwh_pipcompile_plugin-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.2.0/README.md` & `edwh_pipcompile_plugin-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `edwh_pipcompile_plugin-0.2.0/pyproject.toml` & `edwh_pipcompile_plugin-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,24 @@
   { name = "Remco Boerma", email = "remco.b@educationwarehouse.nl" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ['invoke', "pip-tools"]
 
 [project.optional-dependencies]
 dev = [
   "hatch",
-  "python-semantic-release",
+  # "python-semantic-release",
   "black",
 ]
 
 [project.urls]
 Documentation = "https://github.com/educationwarehouse/edwh-pipcompile-plugin#readme"
 Issues = "https://github.com/educationwarehouse/edwh-pipcompile-plugin/issues"
 Source = "https://github.com/educationwarehouse/edwh-pipcompile-plugin"
@@ -73,15 +74,15 @@
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
 
 [[tool.hatch.envs.all.matrix]]
-python = ["3.10", "3.11"]
+python = ["3.10", "3.11", "3.12"]
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
   "black>=23.1.0",
   "mypy>=1.0.0",
   "ruff>=0.0.243",
```

### Comparing `edwh_pipcompile_plugin-0.2.0/PKG-INFO` & `edwh_pipcompile_plugin-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: edwh-pipcompile-plugin
-Version: 0.2.0
+Version: 0.2.1
 Summary: Plugin that integrates `pip-tools` with `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-pipcompile-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-pipcompile-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-pipcompile-plugin
 Author-email: Robin van der Noord <robin.vdn@educationwarehouse.nl>, Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: invoke
 Requires-Dist: pip-tools
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
-Requires-Dist: python-semantic-release; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # edwh-pipcompile-plugin
 
 [![PyPI - Version](https://img.shields.io/pypi/v/edwh-pipcompile-plugin.svg)](https://pypi.org/project/edwh-pipcompile-plugin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/edwh-pipcompile-plugin.svg)](https://pypi.org/project/edwh-pipcompile-plugin)
```

