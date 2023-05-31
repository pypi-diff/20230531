# Comparing `tmp/kttools-0.2.1.tar.gz` & `tmp/kttools-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kttools-0.2.1.tar", max compression
+gzip compressed data, was "kttools-0.2.2.tar", max compression
```

## Comparing `kttools-0.2.1.tar` & `kttools-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-04-18 05:39:37.706567 kttools-0.2.1/LICENSE
--rw-r--r--   0        0        0     1538 2023-04-18 05:39:37.706567 kttools-0.2.1/README.rst
--rw-r--r--   0        0        0     1090 2023-04-18 05:39:37.706567 kttools-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      457 2023-04-18 05:39:37.706567 kttools-0.2.1/tools/__init__.py
--rw-r--r--   0        0        0      366 2023-04-18 05:39:37.706567 kttools-0.2.1/tools/sc/__init__.py
--rw-r--r--   0        0        0    12358 2023-04-18 05:39:37.710567 kttools-0.2.1/tools/sc/_sc.py
--rw-r--r--   0        0        0      429 2023-04-18 05:39:37.710567 kttools-0.2.1/tools/tools/__init__.py
--rw-r--r--   0        0        0     8879 2023-04-18 05:39:37.710567 kttools-0.2.1/tools/tools/_tools.py
--rw-r--r--   0        0        0     2611 1970-01-01 00:00:00.000000 kttools-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-30 23:57:36.815537 kttools-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1540 2023-05-30 23:57:36.815537 kttools-0.2.2/README.rst
+-rw-r--r--   0        0        0     1132 2023-05-30 23:57:36.815537 kttools-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      457 2023-05-30 23:57:36.815537 kttools-0.2.2/tools/__init__.py
+-rw-r--r--   0        0        0      449 2023-05-30 23:57:36.815537 kttools-0.2.2/tools/sc/__init__.py
+-rw-r--r--   0        0        0    12358 2023-05-30 23:57:36.815537 kttools-0.2.2/tools/sc/_sc.py
+-rw-r--r--   0        0        0      429 2023-05-30 23:57:36.815537 kttools-0.2.2/tools/tools/__init__.py
+-rw-r--r--   0        0        0     8879 2023-05-30 23:57:36.815537 kttools-0.2.2/tools/tools/_tools.py
+-rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 kttools-0.2.2/PKG-INFO
```

### Comparing `kttools-0.2.1/LICENSE` & `kttools-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kttools-0.2.1/README.rst` & `kttools-0.2.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 ~~~~~~~
 
 .. code:: bash
 
    pip install kttools
 
    # or 
-   pip install git+https://github.com/zktuong/kttools.git
+   pip install git+https://github.com/tuonglab/kttools.git
 
    # or
-   git clone https://github.com/zktuong/kttools.git
+   git clone https://github.com/tuonglab/kttools.git
    cd kttools; pip install -e .
 
 Usage
 ~~~~~
 
 .. code:: python
```

### Comparing `kttools-0.2.1/pyproject.toml` & `kttools-0.2.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "kttools"
-version = "0.2.1"
+version = "0.2.2"
 description = "Kelvin's miscellaneous tools for python"
 authors = ["Zewen Kelvin Tuong <z.tuong@uq.edu.au>"]
 license = "MIT"
 readme = "README.rst"
 classifiers = [
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'Programming Language :: Python :: 3',
 ]
 packages = [{ include = "tools" }]
 
 [tool.poetry.dependencies]
-python = ">=3.8"
-pandas = ">=1.2.4"
-numpy = ">=1.21.6"
-matplotlib = ">=3.5.2"
-scanpy = ">=1.7.1"
-anndata = ">=0.7.6"
+python = ">=3.8,<3.11"
+pandas = ">=1.2.4,<2.0.2"
+numpy = ">=1.21.6,<1.24.4"
+matplotlib = ">=3.5.2,<3.7.2"
+scanpy = ">=1.7.1,<1.9.4"
+anndata = ">=0.7.6,<0.9.2"
 sphinx-autodoc-typehints = { optional = true, version = "*" }
 sphinx_rtd_theme = { optional = true, version = "*" }
 readthedocs-sphinx-ext = { optional = true, version = "*" }
 recommonmark = { optional = true, version = "*" }
 
 [tool.poetry.extras]
 docs = [
```

### Comparing `kttools-0.2.1/tools/sc/_sc.py` & `kttools-0.2.2/tools/sc/_sc.py`

 * *Files identical despite different names*

### Comparing `kttools-0.2.1/tools/tools/_tools.py` & `kttools-0.2.2/tools/tools/_tools.py`

 * *Files identical despite different names*

### Comparing `kttools-0.2.1/PKG-INFO` & `kttools-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: kttools
-Version: 0.2.1
+Version: 0.2.2
 Summary: Kelvin's miscellaneous tools for python
 License: MIT
 Author: Zewen Kelvin Tuong
 Author-email: z.tuong@uq.edu.au
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Provides-Extra: docs
-Requires-Dist: anndata (>=0.7.6)
-Requires-Dist: matplotlib (>=3.5.2)
-Requires-Dist: numpy (>=1.21.6)
-Requires-Dist: pandas (>=1.2.4)
+Requires-Dist: anndata (>=0.7.6,<0.9.2)
+Requires-Dist: matplotlib (>=3.5.2,<3.7.2)
+Requires-Dist: numpy (>=1.21.6,<1.24.4)
+Requires-Dist: pandas (>=1.2.4,<2.0.2)
 Requires-Dist: readthedocs-sphinx-ext ; extra == "docs"
 Requires-Dist: recommonmark ; extra == "docs"
-Requires-Dist: scanpy (>=1.7.1)
+Requires-Dist: scanpy (>=1.7.1,<1.9.4)
 Requires-Dist: sphinx-autodoc-typehints ; extra == "docs"
 Requires-Dist: sphinx_rtd_theme ; extra == "docs"
 Description-Content-Type: text/x-rst
 
 |Docs| |PyPI|
 
 kttools
@@ -38,18 +36,18 @@
 ~~~~~~~
 
 .. code:: bash
 
    pip install kttools
 
    # or 
-   pip install git+https://github.com/zktuong/kttools.git
+   pip install git+https://github.com/tuonglab/kttools.git
 
    # or
-   git clone https://github.com/zktuong/kttools.git
+   git clone https://github.com/tuonglab/kttools.git
    cd kttools; pip install -e .
 
 Usage
 ~~~~~
 
 .. code:: python
```

