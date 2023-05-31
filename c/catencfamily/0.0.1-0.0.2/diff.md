# Comparing `tmp/catencfamily-0.0.1.tar.gz` & `tmp/catencfamily-0.0.2.tar.gz`

## Comparing `catencfamily-0.0.1.tar` & `catencfamily-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 catencfamily-0.0.1/0.1.0
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 catencfamily-0.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.1/src/catfamilyenc/__init__.py
--rw-r--r--   0        0        0    87907 2020-02-02 00:00:00.000000 catencfamily-0.0.1/src/catfamilyenc/catencfamily.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.1/LICENSE
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 catencfamily-0.0.1/README.md
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 catencfamily-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 catencfamily-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 catencfamily-0.0.2/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.2/src/catfamilyenc/__init__.py
+-rw-r--r--   0        0        0    87907 2020-02-02 00:00:00.000000 catencfamily-0.0.2/src/catfamilyenc/catencfamily.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 catencfamily-0.0.2/README.md
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 catencfamily-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 catencfamily-0.0.2/PKG-INFO
```

### Comparing `catencfamily-0.0.1/requirements.txt` & `catencfamily-0.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.1/src/catfamilyenc/catencfamily.py` & `catencfamily-0.0.2/src/catfamilyenc/catencfamily.py`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.1/LICENSE` & `catencfamily-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.1/pyproject.toml` & `catencfamily-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -21,8 +21,8 @@
   "numpy",
   "networkx",
   "cdlib",
   "matplotlib",
   "pathlib",
 ]
 [project.urls]
-"Homepage" = "https://github.com/harnalashok/catfamilyencoders/tree/main"
+"Homepage" = "https://github.com/harnalashok/CatEncodersFamily"
```

### Comparing `catencfamily-0.0.1/PKG-INFO` & `catencfamily-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.1
+Version: 0.0.2
 Summary: A class to generate a family of categorical encoders using network analysis
-Project-URL: Homepage, https://github.com/harnalashok/catfamilyencoders/tree/main
+Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: cdlib
@@ -14,8 +14,30 @@
 Requires-Dist: networkx
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pathlib
 Requires-Dist: scikit-learn
 Description-Content-Type: text/markdown
 
-A class to encode categorical features in multiple but related ways using network analysis. Together the family of multiple encodings serve as a numerical vector for every level of a categorical feature. The class transforms a group of categorical features into corresponding numerical features which can then be used either in unsupervised learning or predictive analytics. To assist in unsupervised learning, it has methods to save a categorical feature as network graphs and plot them. The class has methods to extract unit vectors for every level of a categorical feature to help, for example, in understanding relationshsips between various levels. Extracted numerical vectors can directly be used in plotting, for example, in tensorflow's Embedding Projector. Class provides methods to get categories encoded for large datasets; one can also take a sample of data at a time, have categories encoded, then take another sample and have categories similarly encoded. After a number of iterations, take either a mean or median to get final category-wise vectors. As the encodings are calculated using a group of network analysis operations, the family of encodings is extensible. The class provides one way, but a limited one to extend it.
+# catencfamily
+
+The module provides a way to encode categorical features in multiple but related ways using network analysis. Together, the family of multiple encodings serve as a numerical vector for every level of a categorical feature. The class transforms a group of categorical features into corresponding numerical features which can then be used either in unsupervised learning or in predictive analytics. To assist in unsupervised learning, it has methods to save a categorical feature as network graphs and plot them. The class has methods to extract unit vectors for every level of a categorical feature to help, for example, in understanding relationshsips between various levels. Extracted numerical vectors can directly be used in plotting, for example, in tensorflow's Embedding Projector. Class provides methods to get categories encoded for large datasets; one can, for example, take a sample of data at a time, have categories encoded, then take another sample and have categories similarly encoded. After a number of iterations, take either a mean or median to get final category-wise vectors. As the encodings are calculated using a group of network analysis operations, the family of encodings is extensible. The class provides one way, but a limited one to extend it.
+
+## Installation
+
+<code>pip install catencfamily</code>
+
+### Requirements
+<pre><code>
+python >= 3.7
+pandas
+numpy
+networkx
+cdlib
+scikit-learn
+matplotlib
+pathlib
+
+
+## License
+
+_MIT License. Any contribution is welcome!
```

