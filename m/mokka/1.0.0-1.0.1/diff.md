# Comparing `tmp/mokka-1.0.0.tar.gz` & `tmp/mokka-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mokka-1.0.0.tar", last modified: Wed May 31 13:24:52 2023, max compression
+gzip compressed data, was "mokka-1.0.1.tar", last modified: Wed May 31 13:49:08 2023, max compression
```

## Comparing `mokka-1.0.0.tar` & `mokka-1.0.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0       72 2023-05-31 11:09:57.056145 mokka-1.0.0/.flake8
--rw-r--r--   0        0        0     1920 2023-05-31 11:48:23.081767 mokka-1.0.0/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      860 2023-05-31 11:09:57.125011 mokka-1.0.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     2110 2023-05-31 11:09:57.074828 mokka-1.0.0/.gitignore
--rw-r--r--   0        0        0      478 2023-05-31 11:09:57.009878 mokka-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    10268 2023-05-31 11:09:57.128240 mokka-1.0.0/COPYING
--rw-r--r--   0        0        0     1752 2023-05-31 12:43:15.244768 mokka-1.0.0/README.md
--rw-r--r--   0        0        0       13 2023-05-31 11:09:57.069806 mokka-1.0.0/docs/.gitignore
--rw-r--r--   0        0        0     1051 2023-05-31 11:09:57.075079 mokka-1.0.0/docs/_templates/package.rst_t
--rw-r--r--   0        0        0      594 2023-05-31 11:09:57.075336 mokka-1.0.0/docs/conf.py
--rw-r--r--   0        0        0      449 2023-05-31 11:09:57.075587 mokka-1.0.0/docs/index.rst
--rwxr-xr-x   0        0        0      130 2023-05-31 11:09:57.075803 mokka-1.0.0/docs/make-docs.sh
--rw-r--r--   0        0        0     3263 2023-05-31 11:09:57.121728 mokka-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1057 2023-05-31 11:09:57.011359 mokka-1.0.0/src/mokka/__init__.py
--rw-r--r--   0        0        0       78 2023-05-31 11:09:57.112618 mokka-1.0.0/src/mokka/channels/__init__.py
--rw-r--r--   0        0        0    39490 2023-05-31 11:09:57.113479 mokka-1.0.0/src/mokka/channels/torch.py
--rw-r--r--   0        0        0       82 2023-05-31 11:09:57.113734 mokka-1.0.0/src/mokka/e2e/__init__.py
--rw-r--r--   0        0        0     3307 2023-05-31 11:09:57.113991 mokka-1.0.0/src/mokka/e2e/torch.py
--rw-r--r--   0        0        0       67 2023-05-31 11:09:57.106505 mokka-1.0.0/src/mokka/equalizers/__init__.py
--rw-r--r--   0        0        0     1205 2023-05-31 11:09:57.106741 mokka-1.0.0/src/mokka/equalizers/torch.py
--rw-r--r--   0        0        0       76 2023-05-31 11:09:57.013015 mokka-1.0.0/src/mokka/functional/__init__.py
--rw-r--r--   0        0        0     3829 2023-05-31 11:09:57.114153 mokka-1.0.0/src/mokka/functional/torch.py
--rw-r--r--   0        0        0       98 2023-05-31 11:09:57.114291 mokka-1.0.0/src/mokka/inft/__init__.py
--rw-r--r--   0        0        0     3968 2023-05-31 11:09:57.114426 mokka-1.0.0/src/mokka/inft/torch.py
--rw-r--r--   0        0        0       49 2023-05-31 11:09:57.098391 mokka-1.0.0/src/mokka/mapping/__init__.py
--rw-r--r--   0        0        0     2241 2023-05-31 11:09:57.062475 mokka-1.0.0/src/mokka/mapping/numpy.py
--rw-r--r--   0        0        0    40640 2023-05-31 11:09:57.066412 mokka-1.0.0/src/mokka/mapping/torch.py
--rw-r--r--   0        0        0      129 2023-05-31 11:09:57.102103 mokka-1.0.0/src/mokka/normalization/__init__.py
--rw-r--r--   0        0        0     1561 2023-05-31 11:09:57.102334 mokka-1.0.0/src/mokka/normalization/torch.py
--rw-r--r--   0        0        0       69 2023-05-31 11:09:57.106982 mokka-1.0.0/src/mokka/pulseshaping/__init__.py
--rw-r--r--   0        0        0     8605 2023-05-31 11:09:57.107138 mokka-1.0.0/src/mokka/pulseshaping/torch.py
--rw-r--r--   0        0        0       70 2023-05-31 11:09:57.107288 mokka-1.0.0/src/mokka/synchronizers/__init__.py
--rw-r--r--   0        0        0       76 2023-05-31 11:09:57.107435 mokka-1.0.0/src/mokka/synchronizers/phase/__init__.py
--rw-r--r--   0        0        0       88 2023-05-31 11:09:57.107577 mokka-1.0.0/src/mokka/synchronizers/phase/torch/__init__.py
--rw-r--r--   0        0        0     9786 2023-05-31 11:09:57.107738 mokka-1.0.0/src/mokka/synchronizers/phase/torch/bps.py
--rw-r--r--   0        0        0     9415 2023-05-31 11:09:57.107929 mokka-1.0.0/src/mokka/utils/__init__.py
--rw-r--r--   0        0        0      166 2023-05-31 11:09:57.016361 mokka-1.0.0/src/mokka/utils/bitops/__init__.py
--rw-r--r--   0        0        0     1461 2023-05-31 11:09:57.108085 mokka-1.0.0/src/mokka/utils/bitops/numpy.py
--rw-r--r--   0        0        0     1360 2023-05-31 11:09:57.016712 mokka-1.0.0/src/mokka/utils/bitops/torch.py
--rw-r--r--   0        0        0      131 2023-05-31 11:09:57.108253 mokka-1.0.0/src/mokka/utils/generators/__init__.py
--rw-r--r--   0        0        0     1220 2023-05-31 11:09:57.108397 mokka-1.0.0/src/mokka/utils/generators/numpy.py
--rw-r--r--   0        0        0       67 2023-05-31 11:09:57.114574 mokka-1.0.0/src/mokka/utils/generators/torch.py
--rw-r--r--   0        0        0       30 2023-05-31 11:09:57.017395 mokka-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0       29 2023-05-31 11:09:57.017564 mokka-1.0.0/tests/mokka/__init__.py
--rw-r--r--   0        0        0     3280 2023-05-31 11:09:57.058432 mokka-1.0.0/tests/mokka/test_channels.py
--rw-r--r--   0        0        0       38 2023-05-31 11:09:57.058567 mokka-1.0.0/tests/mokka/test_e2e.py
--rw-r--r--   0        0        0       52 2023-05-31 11:09:57.058713 mokka-1.0.0/tests/mokka/test_equalizers.py
--rw-r--r--   0        0        0      927 2023-05-31 11:09:57.118003 mokka-1.0.0/tests/mokka/test_functional.py
--rw-r--r--   0        0        0       44 2023-05-31 11:09:57.018725 mokka-1.0.0/tests/mokka/test_import.py
--rw-r--r--   0        0        0     1378 2023-05-31 11:09:57.018890 mokka-1.0.0/tests/mokka/test_mapping.py
--rw-r--r--   0        0        0      900 2023-05-31 11:09:57.019117 mokka-1.0.0/tests/mokka/test_normalization.py
--rw-r--r--   0        0        0       54 2023-05-31 11:09:57.058879 mokka-1.0.0/tests/mokka/test_pulseshaping.py
--rw-r--r--   0        0        0       56 2023-05-31 11:09:57.059049 mokka-1.0.0/tests/mokka/test_synchronizers.py
--rw-r--r--   0        0        0      677 2023-05-31 11:09:57.118286 mokka-1.0.0/tests/mokka/test_utils.py
--rw-r--r--   0        0        0     3019 1970-01-01 00:00:00.000000 mokka-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-05-31 11:09:57.056145 mokka-1.0.1/.flake8
+-rw-r--r--   0        0        0     1920 2023-05-31 11:48:23.081767 mokka-1.0.1/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      860 2023-05-31 11:09:57.125011 mokka-1.0.1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     2110 2023-05-31 11:09:57.074828 mokka-1.0.1/.gitignore
+-rw-r--r--   0        0        0      478 2023-05-31 11:09:57.009878 mokka-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    10268 2023-05-31 11:09:57.128240 mokka-1.0.1/COPYING
+-rw-r--r--   0        0        0     1752 2023-05-31 12:43:15.244768 mokka-1.0.1/README.md
+-rw-r--r--   0        0        0       13 2023-05-31 11:09:57.069806 mokka-1.0.1/docs/.gitignore
+-rw-r--r--   0        0        0     1051 2023-05-31 11:09:57.075079 mokka-1.0.1/docs/_templates/package.rst_t
+-rw-r--r--   0        0        0      594 2023-05-31 11:09:57.075336 mokka-1.0.1/docs/conf.py
+-rw-r--r--   0        0        0      449 2023-05-31 11:09:57.075587 mokka-1.0.1/docs/index.rst
+-rwxr-xr-x   0        0        0      130 2023-05-31 11:09:57.075803 mokka-1.0.1/docs/make-docs.sh
+-rw-r--r--   0        0        0     3506 2023-05-31 13:48:33.571365 mokka-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1057 2023-05-31 13:48:38.404662 mokka-1.0.1/src/mokka/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-31 11:09:57.112618 mokka-1.0.1/src/mokka/channels/__init__.py
+-rw-r--r--   0        0        0    39490 2023-05-31 11:09:57.113479 mokka-1.0.1/src/mokka/channels/torch.py
+-rw-r--r--   0        0        0       82 2023-05-31 11:09:57.113734 mokka-1.0.1/src/mokka/e2e/__init__.py
+-rw-r--r--   0        0        0     3307 2023-05-31 11:09:57.113991 mokka-1.0.1/src/mokka/e2e/torch.py
+-rw-r--r--   0        0        0       67 2023-05-31 11:09:57.106505 mokka-1.0.1/src/mokka/equalizers/__init__.py
+-rw-r--r--   0        0        0     1205 2023-05-31 11:09:57.106741 mokka-1.0.1/src/mokka/equalizers/torch.py
+-rw-r--r--   0        0        0       76 2023-05-31 11:09:57.013015 mokka-1.0.1/src/mokka/functional/__init__.py
+-rw-r--r--   0        0        0     3829 2023-05-31 11:09:57.114153 mokka-1.0.1/src/mokka/functional/torch.py
+-rw-r--r--   0        0        0       98 2023-05-31 11:09:57.114291 mokka-1.0.1/src/mokka/inft/__init__.py
+-rw-r--r--   0        0        0     3968 2023-05-31 11:09:57.114426 mokka-1.0.1/src/mokka/inft/torch.py
+-rw-r--r--   0        0        0       49 2023-05-31 11:09:57.098391 mokka-1.0.1/src/mokka/mapping/__init__.py
+-rw-r--r--   0        0        0     2241 2023-05-31 11:09:57.062475 mokka-1.0.1/src/mokka/mapping/numpy.py
+-rw-r--r--   0        0        0    40640 2023-05-31 11:09:57.066412 mokka-1.0.1/src/mokka/mapping/torch.py
+-rw-r--r--   0        0        0      129 2023-05-31 11:09:57.102103 mokka-1.0.1/src/mokka/normalization/__init__.py
+-rw-r--r--   0        0        0     1561 2023-05-31 11:09:57.102334 mokka-1.0.1/src/mokka/normalization/torch.py
+-rw-r--r--   0        0        0       69 2023-05-31 11:09:57.106982 mokka-1.0.1/src/mokka/pulseshaping/__init__.py
+-rw-r--r--   0        0        0     8605 2023-05-31 11:09:57.107138 mokka-1.0.1/src/mokka/pulseshaping/torch.py
+-rw-r--r--   0        0        0       70 2023-05-31 11:09:57.107288 mokka-1.0.1/src/mokka/synchronizers/__init__.py
+-rw-r--r--   0        0        0       76 2023-05-31 11:09:57.107435 mokka-1.0.1/src/mokka/synchronizers/phase/__init__.py
+-rw-r--r--   0        0        0       88 2023-05-31 11:09:57.107577 mokka-1.0.1/src/mokka/synchronizers/phase/torch/__init__.py
+-rw-r--r--   0        0        0     9786 2023-05-31 11:09:57.107738 mokka-1.0.1/src/mokka/synchronizers/phase/torch/bps.py
+-rw-r--r--   0        0        0     9415 2023-05-31 11:09:57.107929 mokka-1.0.1/src/mokka/utils/__init__.py
+-rw-r--r--   0        0        0      166 2023-05-31 11:09:57.016361 mokka-1.0.1/src/mokka/utils/bitops/__init__.py
+-rw-r--r--   0        0        0     1461 2023-05-31 11:09:57.108085 mokka-1.0.1/src/mokka/utils/bitops/numpy.py
+-rw-r--r--   0        0        0     1360 2023-05-31 11:09:57.016712 mokka-1.0.1/src/mokka/utils/bitops/torch.py
+-rw-r--r--   0        0        0      131 2023-05-31 11:09:57.108253 mokka-1.0.1/src/mokka/utils/generators/__init__.py
+-rw-r--r--   0        0        0     1220 2023-05-31 11:09:57.108397 mokka-1.0.1/src/mokka/utils/generators/numpy.py
+-rw-r--r--   0        0        0       67 2023-05-31 11:09:57.114574 mokka-1.0.1/src/mokka/utils/generators/torch.py
+-rw-r--r--   0        0        0       30 2023-05-31 11:09:57.017395 mokka-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0       29 2023-05-31 11:09:57.017564 mokka-1.0.1/tests/mokka/__init__.py
+-rw-r--r--   0        0        0     3280 2023-05-31 11:09:57.058432 mokka-1.0.1/tests/mokka/test_channels.py
+-rw-r--r--   0        0        0       38 2023-05-31 11:09:57.058567 mokka-1.0.1/tests/mokka/test_e2e.py
+-rw-r--r--   0        0        0       52 2023-05-31 11:09:57.058713 mokka-1.0.1/tests/mokka/test_equalizers.py
+-rw-r--r--   0        0        0      927 2023-05-31 11:09:57.118003 mokka-1.0.1/tests/mokka/test_functional.py
+-rw-r--r--   0        0        0       44 2023-05-31 11:09:57.018725 mokka-1.0.1/tests/mokka/test_import.py
+-rw-r--r--   0        0        0     1378 2023-05-31 11:09:57.018890 mokka-1.0.1/tests/mokka/test_mapping.py
+-rw-r--r--   0        0        0      900 2023-05-31 11:09:57.019117 mokka-1.0.1/tests/mokka/test_normalization.py
+-rw-r--r--   0        0        0       54 2023-05-31 11:09:57.058879 mokka-1.0.1/tests/mokka/test_pulseshaping.py
+-rw-r--r--   0        0        0       56 2023-05-31 11:09:57.059049 mokka-1.0.1/tests/mokka/test_synchronizers.py
+-rw-r--r--   0        0        0      677 2023-05-31 11:09:57.118286 mokka-1.0.1/tests/mokka/test_utils.py
+-rw-r--r--   0        0        0     3178 1970-01-01 00:00:00.000000 mokka-1.0.1/PKG-INFO
```

### Comparing `mokka-1.0.0/.github/workflows/documentation.yml` & `mokka-1.0.1/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/.github/workflows/python-package.yml` & `mokka-1.0.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/.gitignore` & `mokka-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/COPYING` & `mokka-1.0.1/COPYING`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/README.md` & `mokka-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/docs/_templates/package.rst_t` & `mokka-1.0.1/docs/_templates/package.rst_t`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/docs/conf.py` & `mokka-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/pyproject.toml` & `mokka-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -11,26 +11,31 @@
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "COPYING"}
 authors = [
     {name = "Andrej Rode", email = "rode@kit.edu"},
     {name = "Shrinivas Chimmalgi", email="shrinivas.chimmalgi@kit.edu"},
     {name = "Benedikt Geiger", email="benedikt.geiger@kit.edu"},
-    {name = "Laurent Schmalen"}
+    {name = "Laurent Schmalen", email="laurent.schmalen@kit.edu"},
+]
+maintainers = [
+    {name = "Andrej Rode", email = "rode@kit.edu"},
+    {name = "Shrinivas Chimmalgi", email="shrinivas.chimmalgi@kit.edu"},
+    {name = "Benedikt Geiger", email="benedikt.geiger@kit.edu"},
 ]
 
 dependencies = [
   "attrs",
   "numpy",
   "torch",
   "matplotlib",
   "scipy",
   "pyqtgraph",
 ]
-version = "1.0.0"
+version = "1.0.1"
 description = "A machine learning toolbox for communications engineering"
 keywords = ["communications engineering", "machine learning"]
 # dynamic = ["version", "description"]
 
 [project.optional-dependencies]
 torch = [
     "torch",
```

### Comparing `mokka-1.0.0/src/mokka/__init__.py` & `mokka-1.0.1/src/mokka/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 This package implements blocks either for PyTorch or TensorFlow, most
 functionality is implemented exclusively in one of the frameworks.
 In the case of TensorFlow the functions are implemented in conjunction
 with the framework sionna.
 """
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 
 from . import utils  # noqa
 from . import functional  # noqa
 from . import normalization  # noqa
 
 from . import channels  # noqa
```

### Comparing `mokka-1.0.0/src/mokka/channels/torch.py` & `mokka-1.0.1/src/mokka/channels/torch.py`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/src/mokka/e2e/torch.py` & `mokka-1.0.1/src/mokka/e2e/torch.py`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/src/mokka/equalizers/torch.py` & `mokka-1.0.1/src/mokka/equalizers/torch.py`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/src/mokka/functional/torch.py` & `mokka-1.0.1/src/mokka/functional/torch.py`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/src/mokka/inft/torch.py` & `mokka-1.0.1/src/mokka/inft/torch.py`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/src/mokka/mapping/numpy.py` & `mokka-1.0.1/src/mokka/mapping/numpy.py`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/src/mokka/mapping/torch.py` & `mokka-1.0.1/src/mokka/mapping/torch.py`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/src/mokka/normalization/torch.py` & `mokka-1.0.1/src/mokka/normalization/torch.py`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/src/mokka/pulseshaping/torch.py` & `mokka-1.0.1/src/mokka/pulseshaping/torch.py`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/src/mokka/synchronizers/phase/torch/bps.py` & `mokka-1.0.1/src/mokka/synchronizers/phase/torch/bps.py`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/src/mokka/utils/__init__.py` & `mokka-1.0.1/src/mokka/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/src/mokka/utils/bitops/numpy.py` & `mokka-1.0.1/src/mokka/utils/bitops/numpy.py`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/src/mokka/utils/bitops/torch.py` & `mokka-1.0.1/src/mokka/utils/bitops/torch.py`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/src/mokka/utils/generators/numpy.py` & `mokka-1.0.1/src/mokka/utils/generators/numpy.py`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/tests/mokka/test_channels.py` & `mokka-1.0.1/tests/mokka/test_channels.py`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/tests/mokka/test_functional.py` & `mokka-1.0.1/tests/mokka/test_functional.py`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/tests/mokka/test_mapping.py` & `mokka-1.0.1/tests/mokka/test_mapping.py`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/tests/mokka/test_normalization.py` & `mokka-1.0.1/tests/mokka/test_normalization.py`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/tests/mokka/test_utils.py` & `mokka-1.0.1/tests/mokka/test_utils.py`

 * *Files identical despite different names*

### Comparing `mokka-1.0.0/PKG-INFO` & `mokka-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mokka
-Version: 1.0.0
+Version: 1.0.1
 Summary: A machine learning toolbox for communications engineering
 Keywords: communications engineering,machine learning
-Author: Laurent Schmalen
-Author-email: Andrej Rode <rode@kit.edu>, Shrinivas Chimmalgi <shrinivas.chimmalgi@kit.edu>, Benedikt Geiger <benedikt.geiger@kit.edu>
+Author-email: Andrej Rode <rode@kit.edu>, Shrinivas Chimmalgi <shrinivas.chimmalgi@kit.edu>, Benedikt Geiger <benedikt.geiger@kit.edu>, Laurent Schmalen <laurent.schmalen@kit.edu>
+Maintainer-email: Andrej Rode <rode@kit.edu>, Shrinivas Chimmalgi <shrinivas.chimmalgi@kit.edu>, Benedikt Geiger <benedikt.geiger@kit.edu>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: attrs
 Requires-Dist: numpy
 Requires-Dist: torch
 Requires-Dist: matplotlib
 Requires-Dist: scipy
```

