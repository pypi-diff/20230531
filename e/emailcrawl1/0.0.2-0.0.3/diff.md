# Comparing `tmp/emailcrawl1-0.0.2.tar.gz` & `tmp/emailcrawl1-0.0.3.tar.gz`

## Comparing `emailcrawl1-0.0.2.tar` & `emailcrawl1-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 emailcrawl1-0.0.2/src/emailcrawl1/__init__.py
--rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 emailcrawl1-0.0.2/src/emailcrawl1/emailcrawl1.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 emailcrawl1-0.0.2/README.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 emailcrawl1-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 emailcrawl1-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 emailcrawl1-0.0.3/src/emailcrawl1/__init__.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 emailcrawl1-0.0.3/src/emailcrawl1/emailcrawl1.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 emailcrawl1-0.0.3/README.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 emailcrawl1-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 emailcrawl1-0.0.3/PKG-INFO
```

### Comparing `emailcrawl1-0.0.2/src/emailcrawl1/emailcrawl1.py` & `emailcrawl1-0.0.3/src/emailcrawl1/emailcrawl1.py`

 * *Files identical despite different names*

### Comparing `emailcrawl1-0.0.2/pyproject.toml` & `emailcrawl1-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
-requires = ["hatchling","requests-html","bs4","pandas"]
+requires = ["hatchling","requests_html","bs4","pandas"]
 build-backend = "hatchling.build"
 [project]
 name = "emailcrawl1"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Raghav", email="raghavgarg121212@gmail.com" },
 ]
 description = "Scrap emails from website"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `emailcrawl1-0.0.2/PKG-INFO` & `emailcrawl1-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emailcrawl1
-Version: 0.0.2
+Version: 0.0.3
 Summary: Scrap emails from website
 Project-URL: Homepage, https://github.com/Raghavgarg12/Python-Projects/tree/main/Web%20Crawling
 Author-email: Raghav <raghavgarg121212@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

