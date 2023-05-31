# Comparing `tmp/zenithlib-1.0.0.tar.gz` & `tmp/zenithlib-1.0.1.tar.gz`

## Comparing `zenithlib-1.0.0.tar` & `zenithlib-1.0.1.tar`

### file list

```diff
@@ -1,49 +1,51 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 zenithlib-1.0.0/.gitattributes
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 zenithlib-1.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     4251 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Code_of_Conduct.md
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 zenithlib-1.0.0/SECURITY.md
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 zenithlib-1.0.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 zenithlib-1.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 zenithlib-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 zenithlib-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 zenithlib-1.0.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 zenithlib-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith/Builder.py
--rw-r--r--   0        0        0    14953 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith/Stylesheet.py
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith/Web.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith/__init__.py
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith/lang/ZenithLang.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith/lang/__init__.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith/lang/langAST.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith/lang/langParser.py
--rw-r--r--   0        0        0     7050 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith/lang/langTranspiler.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith/lang/__testing__/out.html
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith/src/tests.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith-Customs/MaterialButton.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith-Customs/MaterialSlider.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith-Customs/ZenithDecorator.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith-Packages/multiport.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith-Plugins/ToElectron.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zenithlib-1.0.0/Zenith-Plugins/bugRenderer.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/ATTRIBUTES.md
--rw-r--r--   0        0        0    14467 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/ELEMENTS.md
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/README.md
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/STYLESHEETS.md
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/api-reference.md
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/components.md
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/configuration.md
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/contributing.md
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/getting-started.md
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/installation.md
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/routing.md
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/usage.md
--rw-r--r--   0        0        0   205818 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/images/Upscaled-Zenith.png
--rw-r--r--   0        0        0   205818 2020-02-02 00:00:00.000000 zenithlib-1.0.0/docs/images/Zenith.png
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 zenithlib-1.0.0/examples/server.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 zenithlib-1.0.0/scripts/bupload.sh
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 zenithlib-1.0.0/scripts/placeholder.sh
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 zenithlib-1.0.0/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zenithlib-1.0.0/LICENSE
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 zenithlib-1.0.0/README.md
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 zenithlib-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 zenithlib-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 zenithlib-1.0.1/.gitattributes
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 zenithlib-1.0.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     4251 2020-02-02 00:00:00.000000 zenithlib-1.0.1/Code_of_Conduct.md
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 zenithlib-1.0.1/SECURITY.md
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 zenithlib-1.0.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 zenithlib-1.0.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 zenithlib-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 zenithlib-1.0.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 zenithlib-1.0.1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 zenithlib-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 zenithlib-1.0.1/Zenith/Builder.py
+-rw-r--r--   0        0        0    14953 2020-02-02 00:00:00.000000 zenithlib-1.0.1/Zenith/Stylesheet.py
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 zenithlib-1.0.1/Zenith/Web.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 zenithlib-1.0.1/Zenith/__init__.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 zenithlib-1.0.1/Zenith/lang/ZenithLang.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 zenithlib-1.0.1/Zenith/lang/__init__.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 zenithlib-1.0.1/Zenith/lang/langAST.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 zenithlib-1.0.1/Zenith/lang/langParser.py
+-rw-r--r--   0        0        0     7050 2020-02-02 00:00:00.000000 zenithlib-1.0.1/Zenith/lang/langTranspiler.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 zenithlib-1.0.1/Zenith/lang/__testing__/out.html
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 zenithlib-1.0.1/Zenith/modules/ReadFromZenithFile.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 zenithlib-1.0.1/Zenith/modules/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 zenithlib-1.0.1/Zenith-Customs/MaterialButton.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 zenithlib-1.0.1/Zenith-Customs/MaterialSlider.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 zenithlib-1.0.1/Zenith-Customs/ZenithDecorator.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zenithlib-1.0.1/Zenith-Packages/multiport.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zenithlib-1.0.1/Zenith-Plugins/ToElectron.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zenithlib-1.0.1/Zenith-Plugins/bugRenderer.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 zenithlib-1.0.1/docs/ATTRIBUTES.md
+-rw-r--r--   0        0        0    14467 2020-02-02 00:00:00.000000 zenithlib-1.0.1/docs/ELEMENTS.md
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 zenithlib-1.0.1/docs/README.md
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 zenithlib-1.0.1/docs/STYLESHEETS.md
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 zenithlib-1.0.1/docs/api-reference.md
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 zenithlib-1.0.1/docs/components.md
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 zenithlib-1.0.1/docs/configuration.md
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 zenithlib-1.0.1/docs/contributing.md
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 zenithlib-1.0.1/docs/getting-started.md
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 zenithlib-1.0.1/docs/installation.md
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 zenithlib-1.0.1/docs/routing.md
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 zenithlib-1.0.1/docs/usage.md
+-rw-r--r--   0        0        0   205818 2020-02-02 00:00:00.000000 zenithlib-1.0.1/docs/images/Upscaled-Zenith.png
+-rw-r--r--   0        0        0   205818 2020-02-02 00:00:00.000000 zenithlib-1.0.1/docs/images/Zenith.png
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 zenithlib-1.0.1/examples/page.zenith
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 zenithlib-1.0.1/examples/server.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 zenithlib-1.0.1/scripts/bupload.sh
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 zenithlib-1.0.1/scripts/placeholder.sh
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 zenithlib-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zenithlib-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 zenithlib-1.0.1/README.md
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 zenithlib-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 zenithlib-1.0.1/PKG-INFO
```

### Comparing `zenithlib-1.0.0/CONTRIBUTING.md` & `zenithlib-1.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/Code_of_Conduct.md` & `zenithlib-1.0.1/Code_of_Conduct.md`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/SECURITY.md` & `zenithlib-1.0.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/.github/FUNDING.yml` & `zenithlib-1.0.1/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md` & `zenithlib-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md` & `zenithlib-1.0.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/.github/workflows/python-package.yml` & `zenithlib-1.0.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/.github/workflows/python-publish.yml` & `zenithlib-1.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/Zenith/Builder.py` & `zenithlib-1.0.1/Zenith/Builder.py`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/Zenith/Stylesheet.py` & `zenithlib-1.0.1/Zenith/Stylesheet.py`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/Zenith/Web.py` & `zenithlib-1.0.1/Zenith/Web.py`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/Zenith/lang/langAST.py` & `zenithlib-1.0.1/Zenith/lang/langAST.py`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/Zenith/lang/langTranspiler.py` & `zenithlib-1.0.1/Zenith/lang/langTranspiler.py`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/Zenith-Customs/ZenithDecorator.py` & `zenithlib-1.0.1/Zenith-Customs/ZenithDecorator.py`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/docs/ATTRIBUTES.md` & `zenithlib-1.0.1/docs/ATTRIBUTES.md`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/docs/ELEMENTS.md` & `zenithlib-1.0.1/docs/ELEMENTS.md`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/docs/README.md` & `zenithlib-1.0.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/docs/api-reference.md` & `zenithlib-1.0.1/docs/api-reference.md`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/docs/components.md` & `zenithlib-1.0.1/docs/components.md`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/docs/getting-started.md` & `zenithlib-1.0.1/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/docs/routing.md` & `zenithlib-1.0.1/docs/routing.md`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/docs/usage.md` & `zenithlib-1.0.1/docs/usage.md`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/docs/images/Upscaled-Zenith.png` & `zenithlib-1.0.1/docs/images/Upscaled-Zenith.png`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/docs/images/Zenith.png` & `zenithlib-1.0.1/docs/images/Zenith.png`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/.gitignore` & `zenithlib-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/LICENSE` & `zenithlib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/README.md` & `zenithlib-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `zenithlib-1.0.0/pyproject.toml` & `zenithlib-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ZenithLib"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Ryan Rudd", email="rsrudd@gmail.com" },
 ]
 description = "Zenith is a powerful Python framework that revolutionizes web development by enabling declarative and efficient UI components for building interactive and scalable websites."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `zenithlib-1.0.0/PKG-INFO` & `zenithlib-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZenithLib
-Version: 1.0.0
+Version: 1.0.1
 Summary: Zenith is a powerful Python framework that revolutionizes web development by enabling declarative and efficient UI components for building interactive and scalable websites.
 Project-URL: Homepage, https://github.com/Ryan-Rudd/Zenith
 Project-URL: Bug Tracker, https://github.com/Ryan-Rudd/Zenith/issues
 Author-email: Ryan Rudd <rsrudd@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

