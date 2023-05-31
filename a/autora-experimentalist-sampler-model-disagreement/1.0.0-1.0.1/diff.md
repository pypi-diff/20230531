# Comparing `tmp/autora-experimentalist-sampler-model-disagreement-1.0.0.tar.gz` & `tmp/autora-experimentalist-sampler-model-disagreement-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-experimentalist-sampler-model-disagreement-1.0.0.tar", last modified: Wed May 31 18:14:06 2023, max compression
+gzip compressed data, was "autora-experimentalist-sampler-model-disagreement-1.0.1.tar", last modified: Wed May 31 18:18:22 2023, max compression
```

## Comparing `autora-experimentalist-sampler-model-disagreement-1.0.0.tar` & `autora-experimentalist-sampler-model-disagreement-1.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:14:06.954318 autora-experimentalist-sampler-model-disagreement-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 18:13:47.000000 autora-experimentalist-sampler-model-disagreement-1.0.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:14:06.942318 autora-experimentalist-sampler-model-disagreement-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:14:06.946318 autora-experimentalist-sampler-model-disagreement-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-31 18:13:47.000000 autora-experimentalist-sampler-model-disagreement-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-31 18:13:47.000000 autora-experimentalist-sampler-model-disagreement-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-31 18:13:47.000000 autora-experimentalist-sampler-model-disagreement-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-31 18:14:06.950318 autora-experimentalist-sampler-model-disagreement-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-31 18:13:47.000000 autora-experimentalist-sampler-model-disagreement-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:14:06.950318 autora-experimentalist-sampler-model-disagreement-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   154072 2023-05-31 18:13:47.000000 autora-experimentalist-sampler-model-disagreement-1.0.0/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-31 18:13:47.000000 autora-experimentalist-sampler-model-disagreement-1.0.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:14:06.950318 autora-experimentalist-sampler-model-disagreement-1.0.0/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-31 18:13:47.000000 autora-experimentalist-sampler-model-disagreement-1.0.0/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-31 18:13:47.000000 autora-experimentalist-sampler-model-disagreement-1.0.0/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:14:06.950318 autora-experimentalist-sampler-model-disagreement-1.0.0/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-31 18:13:47.000000 autora-experimentalist-sampler-model-disagreement-1.0.0/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-31 18:13:47.000000 autora-experimentalist-sampler-model-disagreement-1.0.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-31 18:13:47.000000 autora-experimentalist-sampler-model-disagreement-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 18:14:06.954318 autora-experimentalist-sampler-model-disagreement-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:14:06.946318 autora-experimentalist-sampler-model-disagreement-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:14:06.946318 autora-experimentalist-sampler-model-disagreement-1.0.0/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:14:06.946318 autora-experimentalist-sampler-model-disagreement-1.0.0/src/autora/experimentalist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:14:06.946318 autora-experimentalist-sampler-model-disagreement-1.0.0/src/autora/experimentalist/sampler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:14:06.950318 autora-experimentalist-sampler-model-disagreement-1.0.0/src/autora/experimentalist/sampler/model_disagreement/
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-31 18:13:47.000000 autora-experimentalist-sampler-model-disagreement-1.0.0/src/autora/experimentalist/sampler/model_disagreement/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:14:06.950318 autora-experimentalist-sampler-model-disagreement-1.0.0/src/autora_experimentalist_sampler_model_disagreement.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-31 18:14:06.000000 autora-experimentalist-sampler-model-disagreement-1.0.0/src/autora_experimentalist_sampler_model_disagreement.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-31 18:14:06.000000 autora-experimentalist-sampler-model-disagreement-1.0.0/src/autora_experimentalist_sampler_model_disagreement.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 18:14:06.000000 autora-experimentalist-sampler-model-disagreement-1.0.0/src/autora_experimentalist_sampler_model_disagreement.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-31 18:14:06.000000 autora-experimentalist-sampler-model-disagreement-1.0.0/src/autora_experimentalist_sampler_model_disagreement.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 18:14:06.000000 autora-experimentalist-sampler-model-disagreement-1.0.0/src/autora_experimentalist_sampler_model_disagreement.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:14:06.950318 autora-experimentalist-sampler-model-disagreement-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-31 18:13:47.000000 autora-experimentalist-sampler-model-disagreement-1.0.0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 18:13:47.000000 autora-experimentalist-sampler-model-disagreement-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-31 18:13:47.000000 autora-experimentalist-sampler-model-disagreement-1.0.0/tests/test_model_disagreement_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.092282 autora-experimentalist-sampler-model-disagreement-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.088282 autora-experimentalist-sampler-model-disagreement-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.088282 autora-experimentalist-sampler-model-disagreement-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-31 18:18:22.092282 autora-experimentalist-sampler-model-disagreement-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.088282 autora-experimentalist-sampler-model-disagreement-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   154072 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.088282 autora-experimentalist-sampler-model-disagreement-1.0.1/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.088282 autora-experimentalist-sampler-model-disagreement-1.0.1/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 18:18:22.092282 autora-experimentalist-sampler-model-disagreement-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.088282 autora-experimentalist-sampler-model-disagreement-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.088282 autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.088282 autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora/experimentalist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.088282 autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora/experimentalist/sampler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.088282 autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora/experimentalist/sampler/model_disagreement/
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora/experimentalist/sampler/model_disagreement/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.092282 autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora_experimentalist_sampler_model_disagreement.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-31 18:18:22.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora_experimentalist_sampler_model_disagreement.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-31 18:18:22.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora_experimentalist_sampler_model_disagreement.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 18:18:22.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora_experimentalist_sampler_model_disagreement.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-31 18:18:22.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora_experimentalist_sampler_model_disagreement.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 18:18:22.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora_experimentalist_sampler_model_disagreement.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:22.092282 autora-experimentalist-sampler-model-disagreement-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-31 18:18:10.000000 autora-experimentalist-sampler-model-disagreement-1.0.1/tests/test_model_disagreement_sampler.py
```

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.0/.github/workflows/python-publish.yml` & `autora-experimentalist-sampler-model-disagreement-1.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.0/.gitignore` & `autora-experimentalist-sampler-model-disagreement-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.0/.pre-commit-config.yaml` & `autora-experimentalist-sampler-model-disagreement-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.0/PKG-INFO` & `autora-experimentalist-sampler-model-disagreement-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-sampler-model-disagreement
-Version: 1.0.0
+Version: 1.0.1
 Summary: Compares weaknesses in multiple models
 Author-email: "Built by Sebastian Musslick, re-factored by Chad Williams" <sebastian_musslick@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-sampler-model-disagreement
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
@@ -19,15 +19,15 @@
 $$
 \underset{\vec{x}'}{\arg\max}~(P_{M_{1}}(\hat{y}, \vec{x}') - P_{M_{2}}(\hat{y}, \vec{x}'))^2
 $$
 
 # Example Code
 
 ```
-from autora.experimentalist.sampler.model_disagreement_sampler import model_disagreement_sampler
+from autora.experimentalist.sampler.model_disagreement import model_disagreement_sampler
 from autora.theorist.bms import BMSRegressor; BMSRegressor()
 from autora.theorist.darts import DARTSRegressor; DARTSRegressor()
 import numpy as np
 
 #Meta-Setup
 X = np.linspace(start=-3, stop=6, num=10).reshape(-1, 1)
 y = (X**2).reshape(-1, 1)
```

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.0/README.md` & `autora-experimentalist-sampler-model-disagreement-1.0.1/docs/index.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# AutoRA Model Disagreement Sampler
+# Model Disagreement Sampler
 
 The model disagreement sampler identifies experimental conditions $\vec{x}' \in X'$ with respect to
 a pairwise distance metric between theorist models, $P_{M_{i}}(\hat{y}, \vec{x}')$:
 
 $$
 \underset{\vec{x}'}{\arg\max}~(P_{M_{1}}(\hat{y}, \vec{x}') - P_{M_{2}}(\hat{y}, \vec{x}'))^2
 $$
 
 # Example Code
 
 ```
-from autora.experimentalist.sampler.model_disagreement_sampler import model_disagreement_sampler
+from autora.experimentalist.sampler.model_disagreement import model_disagreement_sampler
 from autora.theorist.bms import BMSRegressor; BMSRegressor()
 from autora.theorist.darts import DARTSRegressor; DARTSRegressor()
 import numpy as np
 
 #Meta-Setup
 X = np.linspace(start=-3, stop=6, num=10).reshape(-1, 1)
 y = (X**2).reshape(-1, 1)
@@ -24,8 +24,8 @@
 bms_theorist = BMSRegressor()
 darts_theorist = DARTSRegressor()
 bms_theorist.fit(X,y)
 darts_theorist.fit(X,y)
 
 #Sampler
 X_new = model_disagreement_sampler(X, [bms_theorist, darts_theorist], n)
-```
+```
```

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.0/docs/Basic Usage.ipynb` & `autora-experimentalist-sampler-model-disagreement-1.0.1/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.0/docs/index.md` & `autora-experimentalist-sampler-model-disagreement-1.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Model Disagreement Sampler
+# AutoRA Model Disagreement Sampler
 
 The model disagreement sampler identifies experimental conditions $\vec{x}' \in X'$ with respect to
 a pairwise distance metric between theorist models, $P_{M_{i}}(\hat{y}, \vec{x}')$:
 
 $$
 \underset{\vec{x}'}{\arg\max}~(P_{M_{1}}(\hat{y}, \vec{x}') - P_{M_{2}}(\hat{y}, \vec{x}'))^2
 $$
 
 # Example Code
 
 ```
-from autora.experimentalist.sampler.model_disagreement_sampler import model_disagreement_sampler
+from autora.experimentalist.sampler.model_disagreement import model_disagreement_sampler
 from autora.theorist.bms import BMSRegressor; BMSRegressor()
 from autora.theorist.darts import DARTSRegressor; DARTSRegressor()
 import numpy as np
 
 #Meta-Setup
 X = np.linspace(start=-3, stop=6, num=10).reshape(-1, 1)
 y = (X**2).reshape(-1, 1)
@@ -24,8 +24,8 @@
 bms_theorist = BMSRegressor()
 darts_theorist = DARTSRegressor()
 bms_theorist.fit(X,y)
 darts_theorist.fit(X,y)
 
 #Sampler
 X_new = model_disagreement_sampler(X, [bms_theorist, darts_theorist], n)
-```
+```
```

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.0/mkdocs/base.yml` & `autora-experimentalist-sampler-model-disagreement-1.0.1/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.0/pyproject.toml` & `autora-experimentalist-sampler-model-disagreement-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.0/src/autora/experimentalist/sampler/model_disagreement/__init__.py` & `autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora/experimentalist/sampler/model_disagreement/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.0/src/autora_experimentalist_sampler_model_disagreement.egg-info/PKG-INFO` & `autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora_experimentalist_sampler_model_disagreement.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-sampler-model-disagreement
-Version: 1.0.0
+Version: 1.0.1
 Summary: Compares weaknesses in multiple models
 Author-email: "Built by Sebastian Musslick, re-factored by Chad Williams" <sebastian_musslick@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-sampler-model-disagreement
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
@@ -19,15 +19,15 @@
 $$
 \underset{\vec{x}'}{\arg\max}~(P_{M_{1}}(\hat{y}, \vec{x}') - P_{M_{2}}(\hat{y}, \vec{x}'))^2
 $$
 
 # Example Code
 
 ```
-from autora.experimentalist.sampler.model_disagreement_sampler import model_disagreement_sampler
+from autora.experimentalist.sampler.model_disagreement import model_disagreement_sampler
 from autora.theorist.bms import BMSRegressor; BMSRegressor()
 from autora.theorist.darts import DARTSRegressor; DARTSRegressor()
 import numpy as np
 
 #Meta-Setup
 X = np.linspace(start=-3, stop=6, num=10).reshape(-1, 1)
 y = (X**2).reshape(-1, 1)
```

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.0/src/autora_experimentalist_sampler_model_disagreement.egg-info/SOURCES.txt` & `autora-experimentalist-sampler-model-disagreement-1.0.1/src/autora_experimentalist_sampler_model_disagreement.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.0/tests/README.md` & `autora-experimentalist-sampler-model-disagreement-1.0.1/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-model-disagreement-1.0.0/tests/test_model_disagreement_sampler.py` & `autora-experimentalist-sampler-model-disagreement-1.0.1/tests/test_model_disagreement_sampler.py`

 * *Files identical despite different names*

