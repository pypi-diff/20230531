# Comparing `tmp/autora-experimentalist-sampler-uncertainty-1.0.0b1.tar.gz` & `tmp/autora-experimentalist-sampler-uncertainty-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-experimentalist-sampler-uncertainty-1.0.0b1.tar", last modified: Wed May 24 17:34:47 2023, max compression
+gzip compressed data, was "autora-experimentalist-sampler-uncertainty-1.0.1.tar", last modified: Wed May 31 18:49:32 2023, max compression
```

## Comparing `autora-experimentalist-sampler-uncertainty-1.0.0b1.tar` & `autora-experimentalist-sampler-uncertainty-1.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.244106 autora-experimentalist-sampler-uncertainty-1.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-24 17:34:35.000000 autora-experimentalist-sampler-uncertainty-1.0.0b1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.240106 autora-experimentalist-sampler-uncertainty-1.0.0b1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.240106 autora-experimentalist-sampler-uncertainty-1.0.0b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-24 17:34:35.000000 autora-experimentalist-sampler-uncertainty-1.0.0b1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-24 17:34:35.000000 autora-experimentalist-sampler-uncertainty-1.0.0b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-24 17:34:35.000000 autora-experimentalist-sampler-uncertainty-1.0.0b1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-24 17:34:47.240106 autora-experimentalist-sampler-uncertainty-1.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-24 17:34:35.000000 autora-experimentalist-sampler-uncertainty-1.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.240106 autora-experimentalist-sampler-uncertainty-1.0.0b1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    58484 2023-05-24 17:34:35.000000 autora-experimentalist-sampler-uncertainty-1.0.0b1/docs/basic-usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-24 17:34:35.000000 autora-experimentalist-sampler-uncertainty-1.0.0b1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.240106 autora-experimentalist-sampler-uncertainty-1.0.0b1/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-24 17:34:35.000000 autora-experimentalist-sampler-uncertainty-1.0.0b1/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-24 17:34:35.000000 autora-experimentalist-sampler-uncertainty-1.0.0b1/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.240106 autora-experimentalist-sampler-uncertainty-1.0.0b1/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-24 17:34:35.000000 autora-experimentalist-sampler-uncertainty-1.0.0b1/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-24 17:34:35.000000 autora-experimentalist-sampler-uncertainty-1.0.0b1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-24 17:34:35.000000 autora-experimentalist-sampler-uncertainty-1.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 17:34:47.244106 autora-experimentalist-sampler-uncertainty-1.0.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.240106 autora-experimentalist-sampler-uncertainty-1.0.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.240106 autora-experimentalist-sampler-uncertainty-1.0.0b1/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.240106 autora-experimentalist-sampler-uncertainty-1.0.0b1/src/autora/experimentalist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.240106 autora-experimentalist-sampler-uncertainty-1.0.0b1/src/autora/experimentalist/sampler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.240106 autora-experimentalist-sampler-uncertainty-1.0.0b1/src/autora/experimentalist/sampler/uncertainty/
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-24 17:34:35.000000 autora-experimentalist-sampler-uncertainty-1.0.0b1/src/autora/experimentalist/sampler/uncertainty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.240106 autora-experimentalist-sampler-uncertainty-1.0.0b1/src/autora_experimentalist_sampler_uncertainty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-05-24 17:34:47.000000 autora-experimentalist-sampler-uncertainty-1.0.0b1/src/autora_experimentalist_sampler_uncertainty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-24 17:34:47.000000 autora-experimentalist-sampler-uncertainty-1.0.0b1/src/autora_experimentalist_sampler_uncertainty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 17:34:47.000000 autora-experimentalist-sampler-uncertainty-1.0.0b1/src/autora_experimentalist_sampler_uncertainty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-24 17:34:47.000000 autora-experimentalist-sampler-uncertainty-1.0.0b1/src/autora_experimentalist_sampler_uncertainty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 17:34:47.000000 autora-experimentalist-sampler-uncertainty-1.0.0b1/src/autora_experimentalist_sampler_uncertainty.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.240106 autora-experimentalist-sampler-uncertainty-1.0.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-24 17:34:35.000000 autora-experimentalist-sampler-uncertainty-1.0.0b1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:35.000000 autora-experimentalist-sampler-uncertainty-1.0.0b1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-24 17:34:35.000000 autora-experimentalist-sampler-uncertainty-1.0.0b1/tests/test_uncertainty_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:49:32.189444 autora-experimentalist-sampler-uncertainty-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 18:49:18.000000 autora-experimentalist-sampler-uncertainty-1.0.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:49:32.185444 autora-experimentalist-sampler-uncertainty-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:49:32.185444 autora-experimentalist-sampler-uncertainty-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-31 18:49:18.000000 autora-experimentalist-sampler-uncertainty-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-31 18:49:18.000000 autora-experimentalist-sampler-uncertainty-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-31 18:49:18.000000 autora-experimentalist-sampler-uncertainty-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-31 18:49:32.189444 autora-experimentalist-sampler-uncertainty-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-31 18:49:18.000000 autora-experimentalist-sampler-uncertainty-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:49:32.189444 autora-experimentalist-sampler-uncertainty-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    58476 2023-05-31 18:49:18.000000 autora-experimentalist-sampler-uncertainty-1.0.1/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-31 18:49:18.000000 autora-experimentalist-sampler-uncertainty-1.0.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:49:32.189444 autora-experimentalist-sampler-uncertainty-1.0.1/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-31 18:49:18.000000 autora-experimentalist-sampler-uncertainty-1.0.1/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-31 18:49:18.000000 autora-experimentalist-sampler-uncertainty-1.0.1/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:49:32.189444 autora-experimentalist-sampler-uncertainty-1.0.1/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-31 18:49:18.000000 autora-experimentalist-sampler-uncertainty-1.0.1/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-31 18:49:18.000000 autora-experimentalist-sampler-uncertainty-1.0.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-31 18:49:18.000000 autora-experimentalist-sampler-uncertainty-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 18:49:32.189444 autora-experimentalist-sampler-uncertainty-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:49:32.185444 autora-experimentalist-sampler-uncertainty-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:49:32.185444 autora-experimentalist-sampler-uncertainty-1.0.1/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:49:32.185444 autora-experimentalist-sampler-uncertainty-1.0.1/src/autora/experimentalist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:49:32.185444 autora-experimentalist-sampler-uncertainty-1.0.1/src/autora/experimentalist/sampler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:49:32.189444 autora-experimentalist-sampler-uncertainty-1.0.1/src/autora/experimentalist/sampler/uncertainty/
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-31 18:49:18.000000 autora-experimentalist-sampler-uncertainty-1.0.1/src/autora/experimentalist/sampler/uncertainty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:49:32.189444 autora-experimentalist-sampler-uncertainty-1.0.1/src/autora_experimentalist_sampler_uncertainty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-31 18:49:32.000000 autora-experimentalist-sampler-uncertainty-1.0.1/src/autora_experimentalist_sampler_uncertainty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-31 18:49:32.000000 autora-experimentalist-sampler-uncertainty-1.0.1/src/autora_experimentalist_sampler_uncertainty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 18:49:32.000000 autora-experimentalist-sampler-uncertainty-1.0.1/src/autora_experimentalist_sampler_uncertainty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-31 18:49:32.000000 autora-experimentalist-sampler-uncertainty-1.0.1/src/autora_experimentalist_sampler_uncertainty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 18:49:32.000000 autora-experimentalist-sampler-uncertainty-1.0.1/src/autora_experimentalist_sampler_uncertainty.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:49:32.189444 autora-experimentalist-sampler-uncertainty-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-31 18:49:18.000000 autora-experimentalist-sampler-uncertainty-1.0.1/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 18:49:18.000000 autora-experimentalist-sampler-uncertainty-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-31 18:49:18.000000 autora-experimentalist-sampler-uncertainty-1.0.1/tests/test_uncertainty_sampler.py
```

### Comparing `autora-experimentalist-sampler-uncertainty-1.0.0b1/.github/workflows/python-publish.yml` & `autora-experimentalist-sampler-uncertainty-1.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-uncertainty-1.0.0b1/.gitignore` & `autora-experimentalist-sampler-uncertainty-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-uncertainty-1.0.0b1/.pre-commit-config.yaml` & `autora-experimentalist-sampler-uncertainty-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-uncertainty-1.0.0b1/PKG-INFO` & `autora-experimentalist-sampler-uncertainty-1.0.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-sampler-uncertainty
-Version: 1.0.0b1
+Version: 1.0.1
 Summary: Sampler based on where the model is least certain.
 Author-email: "Built by Sebastian Musslick, restructured by Chad Williams" <sebastian_musslick@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-sampler-uncertainty
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
@@ -13,36 +13,36 @@
 
 # AutoRA Uncertainty Sampler
 
 The uncertainty sampler identifies experimental conditions $\vec{x}' \in X'$ with respect model uncertainty. Within the uncertainty sampler, there are three methods to determine uncertainty:
 
 ## Least Confident
 $$
-x^* = \operatorname{argmax} \left( 1-P(\hat{y}|x) \right),
+x^* = \text{argmax} \left( 1-P(\hat{y}|x) \right),
 $$
 
-where $\hat{y} = \operatorname{argmax} P(y_i|x)$
+where $\hat{y} = \text{argmax} P(y_i|x)$
 
 ## Margin
 
 $$
-x^* = \operatorname{argmax} \left( P(\hat{y}_1|x) - P(\hat{y}_2|x) \right),
+x^* = \text{argmax} \left( P(\hat{y}_1|x) - P(\hat{y}_2|x) \right),
 $$
 
 where $\hat{y}_1$ and $\hat{y}_2$ are the first and second most probable class labels under the model, respectively.
 
 ## Entropy
 $$ 
-x^* = \operatorname{argmax} \left( - \sum P(y_i|x)\operatorname{log} P(y_i|x) \right)
+x^* = \text{argmax} \left( - \sum P(y_i|x)\text{log} P(y_i|x) \right)
 $$
 
 # Example Code
 
 ```
-from autora.experimentalist.sampler.uncertainty_sampler import uncertainty_sampler
+from autora.experimentalist.sampler.uncertainty import uncertainty_sampler
 from sklearn.linear_model import LogisticRegression
 import numpy as np
 
 #Meta-Setup
 X = np.linspace(start=-3, stop=6, num=10).reshape(-1, 1)
 y = (X**2).reshape(-1)
 n = 5
```

### Comparing `autora-experimentalist-sampler-uncertainty-1.0.0b1/README.md` & `autora-experimentalist-sampler-uncertainty-1.0.1/docs/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AutoRA Uncertainty Sampler
+# Uncertainty Sampler
 
 The uncertainty sampler identifies experimental conditions $\vec{x}' \in X'$ with respect model uncertainty. Within the uncertainty sampler, there are three methods to determine uncertainty:
 
 ## Least Confident
 $$
 x^* = \operatorname{argmax} \left( 1-P(\hat{y}|x) \right),
 $$
@@ -21,23 +21,23 @@
 $$ 
 x^* = \operatorname{argmax} \left( - \sum P(y_i|x)\operatorname{log} P(y_i|x) \right)
 $$
 
 # Example Code
 
 ```
-from autora.experimentalist.sampler.uncertainty_sampler import uncertainty_sampler
+from autora.experimentalist.sampler.uncertainty import uncertainty_sampler
 from sklearn.linear_model import LogisticRegression
 import numpy as np
 
 #Meta-Setup
 X = np.linspace(start=-3, stop=6, num=10).reshape(-1, 1)
 y = (X**2).reshape(-1)
 n = 5
 
 #Theorists
 lr_theorist = LogisticRegression()
 lr_theorist.fit(X,y)
 
 #Sampler
 X_new = uncertainty_sampler(X, lr_theorist, n, measure ="least_confident")
-```
+```
```

### Comparing `autora-experimentalist-sampler-uncertainty-1.0.0b1/docs/basic-usage.ipynb` & `autora-experimentalist-sampler-uncertainty-1.0.1/docs/Basic Usage.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996428571428572%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, 'from autora.experimentalist.sampler.uncertainty import "*

 * *            "uncertainty_sampler')], delete: [3]}}}"}*

```diff
@@ -13,15 +13,15 @@
             "execution_count": 25,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
                 "from sklearn.linear_model import LogisticRegression\n",
-                "from autora.experimentalist.sampler.uncertainty_sampler import uncertainty_sampler"
+                "from autora.experimentalist.sampler.uncertainty import uncertainty_sampler"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "vscode": {
```

### Comparing `autora-experimentalist-sampler-uncertainty-1.0.0b1/mkdocs/base.yml` & `autora-experimentalist-sampler-uncertainty-1.0.1/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-uncertainty-1.0.0b1/pyproject.toml` & `autora-experimentalist-sampler-uncertainty-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-uncertainty-1.0.0b1/src/autora/experimentalist/sampler/uncertainty/__init__.py` & `autora-experimentalist-sampler-uncertainty-1.0.1/src/autora/experimentalist/sampler/uncertainty/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-uncertainty-1.0.0b1/src/autora_experimentalist_sampler_uncertainty.egg-info/PKG-INFO` & `autora-experimentalist-sampler-uncertainty-1.0.1/src/autora_experimentalist_sampler_uncertainty.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-sampler-uncertainty
-Version: 1.0.0b1
+Version: 1.0.1
 Summary: Sampler based on where the model is least certain.
 Author-email: "Built by Sebastian Musslick, restructured by Chad Williams" <sebastian_musslick@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-sampler-uncertainty
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
@@ -13,36 +13,36 @@
 
 # AutoRA Uncertainty Sampler
 
 The uncertainty sampler identifies experimental conditions $\vec{x}' \in X'$ with respect model uncertainty. Within the uncertainty sampler, there are three methods to determine uncertainty:
 
 ## Least Confident
 $$
-x^* = \operatorname{argmax} \left( 1-P(\hat{y}|x) \right),
+x^* = \text{argmax} \left( 1-P(\hat{y}|x) \right),
 $$
 
-where $\hat{y} = \operatorname{argmax} P(y_i|x)$
+where $\hat{y} = \text{argmax} P(y_i|x)$
 
 ## Margin
 
 $$
-x^* = \operatorname{argmax} \left( P(\hat{y}_1|x) - P(\hat{y}_2|x) \right),
+x^* = \text{argmax} \left( P(\hat{y}_1|x) - P(\hat{y}_2|x) \right),
 $$
 
 where $\hat{y}_1$ and $\hat{y}_2$ are the first and second most probable class labels under the model, respectively.
 
 ## Entropy
 $$ 
-x^* = \operatorname{argmax} \left( - \sum P(y_i|x)\operatorname{log} P(y_i|x) \right)
+x^* = \text{argmax} \left( - \sum P(y_i|x)\text{log} P(y_i|x) \right)
 $$
 
 # Example Code
 
 ```
-from autora.experimentalist.sampler.uncertainty_sampler import uncertainty_sampler
+from autora.experimentalist.sampler.uncertainty import uncertainty_sampler
 from sklearn.linear_model import LogisticRegression
 import numpy as np
 
 #Meta-Setup
 X = np.linspace(start=-3, stop=6, num=10).reshape(-1, 1)
 y = (X**2).reshape(-1)
 n = 5
```

### Comparing `autora-experimentalist-sampler-uncertainty-1.0.0b1/src/autora_experimentalist_sampler_uncertainty.egg-info/SOURCES.txt` & `autora-experimentalist-sampler-uncertainty-1.0.1/src/autora_experimentalist_sampler_uncertainty.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
 README.md
 mkdocs.yml
 pyproject.toml
 .github/workflows/python-publish.yml
-docs/basic-usage.ipynb
+docs/Basic Usage.ipynb
 docs/index.md
 docs/quickstart.md
 docs/javascripts/mathjax.js
 mkdocs/base.yml
 src/autora/experimentalist/sampler/uncertainty/__init__.py
 src/autora_experimentalist_sampler_uncertainty.egg-info/PKG-INFO
 src/autora_experimentalist_sampler_uncertainty.egg-info/SOURCES.txt
```

### Comparing `autora-experimentalist-sampler-uncertainty-1.0.0b1/tests/README.md` & `autora-experimentalist-sampler-uncertainty-1.0.1/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-sampler-uncertainty-1.0.0b1/tests/test_uncertainty_sampler.py` & `autora-experimentalist-sampler-uncertainty-1.0.1/tests/test_uncertainty_sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from autora.experimentalist.sampler.uncertainty_sampler import uncertainty_sampler
+from autora.experimentalist.sampler.uncertainty import uncertainty_sampler
 from sklearn.linear_model import LogisticRegression
 import numpy as np
 
 def test_output_dimensions():
     #Meta-Setup
     X = np.linspace(start=-3, stop=6, num=10).reshape(-1, 1)
     y = (X**2).reshape(-1)
```

