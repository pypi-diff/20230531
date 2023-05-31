# Comparing `tmp/autora-experimentalist-sampler-nearest-value-1.0.0.tar.gz` & `tmp/autora-experimentalist-sampler-nearest-value-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-experimentalist-sampler-nearest-value-1.0.0.tar", last modified: Wed May 31 18:25:02 2023, max compression
+gzip compressed data, was "autora-experimentalist-sampler-nearest-value-1.0.1.tar", last modified: Wed May 31 18:33:17 2023, max compression
```

## Comparing `autora-experimentalist-sampler-nearest-value-1.0.0.tar` & `autora-experimentalist-sampler-nearest-value-1.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:25:02.569929 autora-experimentalist-sampler-nearest-value-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 18:24:50.000000 autora-experimentalist-sampler-nearest-value-1.0.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:25:02.565929 autora-experimentalist-sampler-nearest-value-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:25:02.565929 autora-experimentalist-sampler-nearest-value-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-31 18:24:50.000000 autora-experimentalist-sampler-nearest-value-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-31 18:24:50.000000 autora-experimentalist-sampler-nearest-value-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-31 18:24:50.000000 autora-experimentalist-sampler-nearest-value-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 18:25:02.569929 autora-experimentalist-sampler-nearest-value-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-31 18:24:50.000000 autora-experimentalist-sampler-nearest-value-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:25:02.565929 autora-experimentalist-sampler-nearest-value-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    35694 2023-05-31 18:24:50.000000 autora-experimentalist-sampler-nearest-value-1.0.0/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-31 18:24:50.000000 autora-experimentalist-sampler-nearest-value-1.0.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:25:02.569929 autora-experimentalist-sampler-nearest-value-1.0.0/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-31 18:24:50.000000 autora-experimentalist-sampler-nearest-value-1.0.0/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-31 18:24:50.000000 autora-experimentalist-sampler-nearest-value-1.0.0/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:25:02.569929 autora-experimentalist-sampler-nearest-value-1.0.0/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-31 18:24:50.000000 autora-experimentalist-sampler-nearest-value-1.0.0/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-31 18:24:50.000000 autora-experimentalist-sampler-nearest-value-1.0.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-31 18:24:50.000000 autora-experimentalist-sampler-nearest-value-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 18:25:02.569929 autora-experimentalist-sampler-nearest-value-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:25:02.565929 autora-experimentalist-sampler-nearest-value-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:25:02.565929 autora-experimentalist-sampler-nearest-value-1.0.0/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:25:02.565929 autora-experimentalist-sampler-nearest-value-1.0.0/src/autora/experimentalist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:25:02.565929 autora-experimentalist-sampler-nearest-value-1.0.0/src/autora/experimentalist/sampler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:25:02.569929 autora-experimentalist-sampler-nearest-value-1.0.0/src/autora/experimentalist/sampler/nearest_value/
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-31 18:24:50.000000 autora-experimentalist-sampler-nearest-value-1.0.0/src/autora/experimentalist/sampler/nearest_value/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:25:02.569929 autora-experimentalist-sampler-nearest-value-1.0.0/src/autora_experimentalist_sampler_nearest_value.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 18:25:02.000000 autora-experimentalist-sampler-nearest-value-1.0.0/src/autora_experimentalist_sampler_nearest_value.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-31 18:25:02.000000 autora-experimentalist-sampler-nearest-value-1.0.0/src/autora_experimentalist_sampler_nearest_value.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 18:25:02.000000 autora-experimentalist-sampler-nearest-value-1.0.0/src/autora_experimentalist_sampler_nearest_value.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-31 18:25:02.000000 autora-experimentalist-sampler-nearest-value-1.0.0/src/autora_experimentalist_sampler_nearest_value.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 18:25:02.000000 autora-experimentalist-sampler-nearest-value-1.0.0/src/autora_experimentalist_sampler_nearest_value.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:25:02.569929 autora-experimentalist-sampler-nearest-value-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-31 18:24:50.000000 autora-experimentalist-sampler-nearest-value-1.0.0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 18:24:50.000000 autora-experimentalist-sampler-nearest-value-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-31 18:24:50.000000 autora-experimentalist-sampler-nearest-value-1.0.0/tests/test_nearest_value_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:33:17.841422 autora-experimentalist-sampler-nearest-value-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 18:33:05.000000 autora-experimentalist-sampler-nearest-value-1.0.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:33:17.837422 autora-experimentalist-sampler-nearest-value-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:33:17.837422 autora-experimentalist-sampler-nearest-value-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-31 18:33:05.000000 autora-experimentalist-sampler-nearest-value-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-31 18:33:05.000000 autora-experimentalist-sampler-nearest-value-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-31 18:33:05.000000 autora-experimentalist-sampler-nearest-value-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 18:33:17.841422 autora-experimentalist-sampler-nearest-value-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-31 18:33:05.000000 autora-experimentalist-sampler-nearest-value-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:33:17.837422 autora-experimentalist-sampler-nearest-value-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    35694 2023-05-31 18:33:05.000000 autora-experimentalist-sampler-nearest-value-1.0.1/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-31 18:33:05.000000 autora-experimentalist-sampler-nearest-value-1.0.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:33:17.837422 autora-experimentalist-sampler-nearest-value-1.0.1/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-31 18:33:05.000000 autora-experimentalist-sampler-nearest-value-1.0.1/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-31 18:33:05.000000 autora-experimentalist-sampler-nearest-value-1.0.1/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:33:17.837422 autora-experimentalist-sampler-nearest-value-1.0.1/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-31 18:33:05.000000 autora-experimentalist-sampler-nearest-value-1.0.1/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-31 18:33:05.000000 autora-experimentalist-sampler-nearest-value-1.0.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-31 18:33:05.000000 autora-experimentalist-sampler-nearest-value-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 18:33:17.841422 autora-experimentalist-sampler-nearest-value-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:33:17.837422 autora-experimentalist-sampler-nearest-value-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:33:17.837422 autora-experimentalist-sampler-nearest-value-1.0.1/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:33:17.837422 autora-experimentalist-sampler-nearest-value-1.0.1/src/autora/experimentalist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:33:17.837422 autora-experimentalist-sampler-nearest-value-1.0.1/src/autora/experimentalist/sampler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:33:17.841422 autora-experimentalist-sampler-nearest-value-1.0.1/src/autora/experimentalist/sampler/nearest_value/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-31 18:33:05.000000 autora-experimentalist-sampler-nearest-value-1.0.1/src/autora/experimentalist/sampler/nearest_value/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:33:17.841422 autora-experimentalist-sampler-nearest-value-1.0.1/src/autora_experimentalist_sampler_nearest_value.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 18:33:17.000000 autora-experimentalist-sampler-nearest-value-1.0.1/src/autora_experimentalist_sampler_nearest_value.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-31 18:33:17.000000 autora-experimentalist-sampler-nearest-value-1.0.1/src/autora_experimentalist_sampler_nearest_value.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 18:33:17.000000 autora-experimentalist-sampler-nearest-value-1.0.1/src/autora_experimentalist_sampler_nearest_value.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-31 18:33:17.000000 autora-experimentalist-sampler-nearest-value-1.0.1/src/autora_experimentalist_sampler_nearest_value.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 18:33:17.000000 autora-experimentalist-sampler-nearest-value-1.0.1/src/autora_experimentalist_sampler_nearest_value.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:33:17.841422 autora-experimentalist-sampler-nearest-value-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-31 18:33:05.000000 autora-experimentalist-sampler-nearest-value-1.0.1/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 18:33:05.000000 autora-experimentalist-sampler-nearest-value-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-31 18:33:05.000000 autora-experimentalist-sampler-nearest-value-1.0.1/tests/test_nearest_value_sampler.py
```

### Comparing `autora-experimentalist-sampler-nearest-value-1.0.0/.github/workflows/python-publish.yml` & `autora-experimentalist-sampler-nearest-value-1.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-nearest-value-1.0.0/.gitignore` & `autora-experimentalist-sampler-nearest-value-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-nearest-value-1.0.0/.pre-commit-config.yaml` & `autora-experimentalist-sampler-nearest-value-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-nearest-value-1.0.0/PKG-INFO` & `autora-experimentalist-sampler-nearest-value-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-sampler-nearest-value
-Version: 1.0.0
+Version: 1.0.1
 Summary: A sampler which returns the nearest values between the input samples and the allowed values, without replacement.
 Author-email: "Built by Sebastian Musslick, restructured by Chad Williams" <sebastian_musslick@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-sampler-nearest-value
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-experimentalist-sampler-nearest-value-1.0.0/docs/Basic Usage.ipynb` & `autora-experimentalist-sampler-nearest-value-1.0.1/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-nearest-value-1.0.0/mkdocs/base.yml` & `autora-experimentalist-sampler-nearest-value-1.0.1/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-nearest-value-1.0.0/pyproject.toml` & `autora-experimentalist-sampler-nearest-value-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-nearest-value-1.0.0/src/autora/experimentalist/sampler/nearest_value/__init__.py` & `autora-experimentalist-sampler-nearest-value-1.0.1/src/autora/experimentalist/sampler/nearest_value/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-nearest-value-1.0.0/src/autora_experimentalist_sampler_nearest_value.egg-info/PKG-INFO` & `autora-experimentalist-sampler-nearest-value-1.0.1/src/autora_experimentalist_sampler_nearest_value.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-sampler-nearest-value
-Version: 1.0.0
+Version: 1.0.1
 Summary: A sampler which returns the nearest values between the input samples and the allowed values, without replacement.
 Author-email: "Built by Sebastian Musslick, restructured by Chad Williams" <sebastian_musslick@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-sampler-nearest-value
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-experimentalist-sampler-nearest-value-1.0.0/src/autora_experimentalist_sampler_nearest_value.egg-info/SOURCES.txt` & `autora-experimentalist-sampler-nearest-value-1.0.1/src/autora_experimentalist_sampler_nearest_value.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-nearest-value-1.0.0/tests/README.md` & `autora-experimentalist-sampler-nearest-value-1.0.1/tests/README.md`

 * *Files identical despite different names*

