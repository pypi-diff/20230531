# Comparing `tmp/edwh_demo_plugin-0.1.0.tar.gz` & `tmp/edwh_demo_plugin-0.1.1.tar.gz`

## Comparing `edwh_demo_plugin-0.1.0.tar` & `edwh_demo_plugin-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 edwh_demo_plugin-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_demo_plugin-0.1.0/src/edwh_demo_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_demo_plugin-0.1.0/src/edwh_demo_plugin/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 edwh_demo_plugin-0.1.0/src/edwh_demo_plugin/demo_plugin.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_demo_plugin-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 edwh_demo_plugin-0.1.0/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_demo_plugin-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 edwh_demo_plugin-0.1.0/README.md
--rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 edwh_demo_plugin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 edwh_demo_plugin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 edwh_demo_plugin-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_demo_plugin-0.1.1/src/edwh_demo_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_demo_plugin-0.1.1/src/edwh_demo_plugin/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 edwh_demo_plugin-0.1.1/src/edwh_demo_plugin/demo_plugin.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_demo_plugin-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 edwh_demo_plugin-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_demo_plugin-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 edwh_demo_plugin-0.1.1/README.md
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 edwh_demo_plugin-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 edwh_demo_plugin-0.1.1/PKG-INFO
```

### Comparing `edwh_demo_plugin-0.1.0/LICENSE.txt` & `edwh_demo_plugin-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_demo_plugin-0.1.0/README.md` & `edwh_demo_plugin-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `edwh_demo_plugin-0.1.0/pyproject.toml` & `edwh_demo_plugin-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 dev = [
     "hatch",
     # "python-semantic-release",
     "black",
 ]
 
 [project.urls]
-Documentation = "https://github.com/educationwarehouse/edwh-demo-plugin#readme"
-Issues = "https://github.com/educationwarehouse/edwh-demo-plugin/issues"
-Source = "https://github.com/educationwarehouse/edwh-demo-plugin"
+Documentation = "https://github.com/educationwarehouse/edwh-demo-tasks-plugin#readme"
+Issues = "https://github.com/educationwarehouse/edwh-demo-tasks-plugin/issues"
+Source = "https://github.com/educationwarehouse/edwh-demo-tasks-plugin"
 
 # https://packaging.python.org/en/latest/guides/creating-and-discovering-plugins/#using-package-metadata
 [project.entry-points."edwh.tasks"]
 demo = "edwh_demo_plugin.demo_plugin"
 
 [tool.hatch.version]
 path = "src/edwh_demo_plugin/__about__.py"
```

### Comparing `edwh_demo_plugin-0.1.0/PKG-INFO` & `edwh_demo_plugin-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: edwh-demo-plugin
-Version: 0.1.0
+Version: 0.1.1
 Summary: Demo project with a plugin to be discovered from the edwh package
-Project-URL: Documentation, https://github.com/educationwarehouse/edwh-demo-plugin#readme
-Project-URL: Issues, https://github.com/educationwarehouse/edwh-demo-plugin/issues
-Project-URL: Source, https://github.com/educationwarehouse/edwh-demo-plugin
+Project-URL: Documentation, https://github.com/educationwarehouse/edwh-demo-tasks-plugin#readme
+Project-URL: Issues, https://github.com/educationwarehouse/edwh-demo-tasks-plugin/issues
+Project-URL: Source, https://github.com/educationwarehouse/edwh-demo-tasks-plugin
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

