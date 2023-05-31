# Comparing `tmp/zenithlib-0.1.0.tar.gz` & `tmp/zenithlib-0.1.1.tar.gz`

## Comparing `zenithlib-0.1.0.tar` & `zenithlib-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 zenithlib-0.1.0/.gitattributes
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 zenithlib-0.1.0/Zenith/Builder.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 zenithlib-0.1.0/Zenith/Stylesheet.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 zenithlib-0.1.0/Zenith/Web.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 zenithlib-0.1.0/Zenith/__init__.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 zenithlib-0.1.0/Zenith/lang/ZenithLang.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 zenithlib-0.1.0/Zenith/lang/__init__.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 zenithlib-0.1.0/Zenith/lang/langAST.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 zenithlib-0.1.0/Zenith/lang/langParser.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 zenithlib-0.1.0/Zenith/lang/langTranspiler.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 zenithlib-0.1.0/Zenith/lang/__testing__/out.html
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 zenithlib-0.1.0/Zenith/src/tests.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 zenithlib-0.1.0/examples/server.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 zenithlib-0.1.0/scripts/bupload.sh
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 zenithlib-0.1.0/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zenithlib-0.1.0/LICENSE
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 zenithlib-0.1.0/README.md
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 zenithlib-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 zenithlib-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 zenithlib-0.1.1/.gitattributes
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 zenithlib-0.1.1/Zenith/Builder.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 zenithlib-0.1.1/Zenith/Stylesheet.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 zenithlib-0.1.1/Zenith/Web.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 zenithlib-0.1.1/Zenith/__init__.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 zenithlib-0.1.1/Zenith/lang/ZenithLang.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 zenithlib-0.1.1/Zenith/lang/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 zenithlib-0.1.1/Zenith/lang/langAST.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 zenithlib-0.1.1/Zenith/lang/langParser.py
+-rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 zenithlib-0.1.1/Zenith/lang/langTranspiler.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 zenithlib-0.1.1/Zenith/lang/__testing__/out.html
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 zenithlib-0.1.1/Zenith/src/tests.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 zenithlib-0.1.1/docs/README.md
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 zenithlib-0.1.1/docs/STYLESHEETS.md
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 zenithlib-0.1.1/examples/server.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 zenithlib-0.1.1/scripts/bupload.sh
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 zenithlib-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zenithlib-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 zenithlib-0.1.1/README.md
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 zenithlib-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 zenithlib-0.1.1/PKG-INFO
```

### Comparing `zenithlib-0.1.0/Zenith/Builder.py` & `zenithlib-0.1.1/Zenith/Builder.py`

 * *Files identical despite different names*

### Comparing `zenithlib-0.1.0/Zenith/Web.py` & `zenithlib-0.1.1/Zenith/Web.py`

 * *Files identical despite different names*

### Comparing `zenithlib-0.1.0/Zenith/lang/langAST.py` & `zenithlib-0.1.1/Zenith/lang/langAST.py`

 * *Files identical despite different names*

### Comparing `zenithlib-0.1.0/.gitignore` & `zenithlib-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `zenithlib-0.1.0/LICENSE` & `zenithlib-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zenithlib-0.1.0/pyproject.toml` & `zenithlib-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ZenithLib"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Ryan Rudd", email="rsrudd@gmail.com" },
 ]
 description = "Zenith is a powerful Python framework that revolutionizes web development by enabling declarative and efficient UI components for building interactive and scalable websites."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

