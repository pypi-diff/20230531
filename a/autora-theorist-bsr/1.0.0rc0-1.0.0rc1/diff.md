# Comparing `tmp/autora-theorist-bsr-1.0.0rc0.tar.gz` & `tmp/autora-theorist-bsr-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-theorist-bsr-1.0.0rc0.tar", last modified: Wed May 10 11:34:45 2023, max compression
+gzip compressed data, was "autora-theorist-bsr-1.0.0rc1.tar", last modified: Thu May 25 16:18:16 2023, max compression
```

## Comparing `autora-theorist-bsr-1.0.0rc0.tar` & `autora-theorist-bsr-1.0.0rc1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:34:45.866334 autora-theorist-bsr-1.0.0rc0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:34:45.854334 autora-theorist-bsr-1.0.0rc0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:34:45.858334 autora-theorist-bsr-1.0.0rc0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-10 11:34:31.000000 autora-theorist-bsr-1.0.0rc0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-10 11:34:31.000000 autora-theorist-bsr-1.0.0rc0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-10 11:34:31.000000 autora-theorist-bsr-1.0.0rc0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-10 11:34:45.866334 autora-theorist-bsr-1.0.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-10 11:34:31.000000 autora-theorist-bsr-1.0.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:34:45.858334 autora-theorist-bsr-1.0.0rc0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    32362 2023-05-10 11:34:31.000000 autora-theorist-bsr-1.0.0rc0/docs/basic-usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-10 11:34:31.000000 autora-theorist-bsr-1.0.0rc0/docs/how-it-works.md
--rw-r--r--   0 runner    (1001) docker     (123)    17622 2023-05-10 11:34:31.000000 autora-theorist-bsr-1.0.0rc0/docs/img.png
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-10 11:34:31.000000 autora-theorist-bsr-1.0.0rc0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:34:45.858334 autora-theorist-bsr-1.0.0rc0/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-10 11:34:31.000000 autora-theorist-bsr-1.0.0rc0/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-10 11:34:31.000000 autora-theorist-bsr-1.0.0rc0/docs/meta-parameters.md
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-10 11:34:31.000000 autora-theorist-bsr-1.0.0rc0/docs/quick-start.md
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-10 11:34:31.000000 autora-theorist-bsr-1.0.0rc0/docs/search-space.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:34:45.862334 autora-theorist-bsr-1.0.0rc0/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-10 11:34:31.000000 autora-theorist-bsr-1.0.0rc0/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-10 11:34:31.000000 autora-theorist-bsr-1.0.0rc0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-10 11:34:31.000000 autora-theorist-bsr-1.0.0rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 11:34:45.866334 autora-theorist-bsr-1.0.0rc0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:34:45.858334 autora-theorist-bsr-1.0.0rc0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:34:45.858334 autora-theorist-bsr-1.0.0rc0/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:34:45.858334 autora-theorist-bsr-1.0.0rc0/src/autora/theorist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:34:45.862334 autora-theorist-bsr-1.0.0rc0/src/autora/theorist/bsr/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 11:34:31.000000 autora-theorist-bsr-1.0.0rc0/src/autora/theorist/bsr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32217 2023-05-10 11:34:32.000000 autora-theorist-bsr-1.0.0rc0/src/autora/theorist/bsr/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-10 11:34:32.000000 autora-theorist-bsr-1.0.0rc0/src/autora/theorist/bsr/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-05-10 11:34:32.000000 autora-theorist-bsr-1.0.0rc0/src/autora/theorist/bsr/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-10 11:34:32.000000 autora-theorist-bsr-1.0.0rc0/src/autora/theorist/bsr/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-10 11:34:32.000000 autora-theorist-bsr-1.0.0rc0/src/autora/theorist/bsr/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-05-10 11:34:32.000000 autora-theorist-bsr-1.0.0rc0/src/autora/theorist/bsr/regressor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:34:45.862334 autora-theorist-bsr-1.0.0rc0/src/autora_theorist_bsr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-10 11:34:45.000000 autora-theorist-bsr-1.0.0rc0/src/autora_theorist_bsr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-10 11:34:45.000000 autora-theorist-bsr-1.0.0rc0/src/autora_theorist_bsr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 11:34:45.000000 autora-theorist-bsr-1.0.0rc0/src/autora_theorist_bsr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 11:34:45.000000 autora-theorist-bsr-1.0.0rc0/src/autora_theorist_bsr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 11:34:45.000000 autora-theorist-bsr-1.0.0rc0/src/autora_theorist_bsr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:34:45.866334 autora-theorist-bsr-1.0.0rc0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-10 11:34:32.000000 autora-theorist-bsr-1.0.0rc0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 11:34:32.000000 autora-theorist-bsr-1.0.0rc0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-10 11:34:32.000000 autora-theorist-bsr-1.0.0rc0/tests/test_bsr_mcmc_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-10 11:34:32.000000 autora-theorist-bsr-1.0.0rc0/tests/test_bsr_node_and_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-10 11:34:32.000000 autora-theorist-bsr-1.0.0rc0/tests/test_bsr_tree_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:18:16.776187 autora-theorist-bsr-1.0.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:18:16.768186 autora-theorist-bsr-1.0.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:18:16.772186 autora-theorist-bsr-1.0.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-25 16:18:16.776187 autora-theorist-bsr-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:18:16.772186 autora-theorist-bsr-1.0.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    32342 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/docs/how-it-works.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17622 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/docs/img.png
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:18:16.772186 autora-theorist-bsr-1.0.0rc1/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/docs/meta-parameters.md
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/docs/search-space.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:18:16.772186 autora-theorist-bsr-1.0.0rc1/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 16:18:16.776187 autora-theorist-bsr-1.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:18:16.768186 autora-theorist-bsr-1.0.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:18:16.768186 autora-theorist-bsr-1.0.0rc1/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:18:16.768186 autora-theorist-bsr-1.0.0rc1/src/autora/theorist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:18:16.772186 autora-theorist-bsr-1.0.0rc1/src/autora/theorist/bsr/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/src/autora/theorist/bsr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32217 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/src/autora/theorist/bsr/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/src/autora/theorist/bsr/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/src/autora/theorist/bsr/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/src/autora/theorist/bsr/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/src/autora/theorist/bsr/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/src/autora/theorist/bsr/regressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:18:16.772186 autora-theorist-bsr-1.0.0rc1/src/autora_theorist_bsr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-25 16:18:16.000000 autora-theorist-bsr-1.0.0rc1/src/autora_theorist_bsr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-25 16:18:16.000000 autora-theorist-bsr-1.0.0rc1/src/autora_theorist_bsr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:18:16.000000 autora-theorist-bsr-1.0.0rc1/src/autora_theorist_bsr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-25 16:18:16.000000 autora-theorist-bsr-1.0.0rc1/src/autora_theorist_bsr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-25 16:18:16.000000 autora-theorist-bsr-1.0.0rc1/src/autora_theorist_bsr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:18:16.776187 autora-theorist-bsr-1.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/tests/test_bsr_mcmc_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/tests/test_bsr_node_and_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-25 16:18:05.000000 autora-theorist-bsr-1.0.0rc1/tests/test_bsr_tree_operation.py
```

### Comparing `autora-theorist-bsr-1.0.0rc0/.github/workflows/python-publish.yml` & `autora-theorist-bsr-1.0.0rc1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0rc0/.gitignore` & `autora-theorist-bsr-1.0.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0rc0/.pre-commit-config.yaml` & `autora-theorist-bsr-1.0.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0rc0/docs/basic-usage.ipynb` & `autora-theorist-bsr-1.0.0rc1/docs/Basic Usage.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9969866071428571%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Basic Usage\\n')], delete: [2, 1, 0]}, 'attachments': "*

 * *            "OrderedDict()}, 11: {'outputs': {0: {'data': {'text/plain': ['<Figure size 640x480 "*

 * *            "with 1 Axes>']}}}}}"}*

```diff
@@ -1,18 +1,17 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false
             },
             "source": [
-                "# Bayesian Symbolic Regression (BSR)\n",
-                "\n",
-                "## Basic Example\n",
+                "# Basic Usage\n",
                 "\n",
                 "The following simple example shows out-of-the-box functionality of BSR."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -126,15 +125,17 @@
             "metadata": {
                 "collapsed": false
             },
             "outputs": [
                 {
                     "data": {
                         "image/png": "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adWqlbnzzjuz7SvIP3p/8/b6OnfubB566KFc31+8eLGxWq3Z/sC++uqrJioqymRkZPik7QXhq8/vww8/NBERESYzM9O9r6g+v3bt2pn777/fve1wOEz16tVNQkJCjuVvueUW06dPn2z72rdvb+655x5jTMF+JwPJ0+v7u6ysLFOuXDnz9ttvu/cNGjTIXH/99b5uqtc8vcb8/r4Wt89w6tSpply5cubkyZPufcH2GZ5XkL8Djz32mGnatGm2fbfeeqvp0aOHe7uwP7OC0GOjQtizZw8pKSl0797dvS86Opr27duTmJgIQGJiIuXLl+fSSy91l+nevTtWq5W1a9cGtL2+aMv69etJSkpiyJAhF7x3//33U7lyZdq1a8ebb75ZoGXNfakw1/fee+9RuXJlmjVrxqhRo7ItWZGYmEjz5s2JiYlx7+vRowfp6els3brV9xeSC1/9W0pLSyMqKoqwsOwTbAf68zt37hzr16/P9vtjtVrp3r27+/fn7xITE7OVB9dncb58QX4nA8Wb6/u706dPk5mZScWKFbPtX7VqFVWrVqVRo0bcd999HD161KdtLyhvr/HkyZPUqVOHWrVqcf3112f7PSpun+Ebb7xB//79KVOmTLb9wfIZeiq/30Ff/MwKwm/LA5QEKSkpANm+1M5vn38vJSWFqlWrZns/LCyMihUrussEii/a8sYbb9CkSRM6duyYbf/TTz/NVVddRenSpVm6dCn/+te/OHnyJA8++KDP2p8fb6/vtttuo06dOlSvXp1Nmzbx+OOPs3PnTj7++GP3cXP6jM+/Fyi++PyOHDnChAkTuPvuu7PtL4rP78iRIzgcjhx/tjt27MixTm6fxV9/387vy61MoHhzfX/3+OOPU7169WxfBD179uSmm26iXr167N69myeeeIJevXqRmJiIzWbz6TXkx5trbNSoEW+++SYtWrQgLS2NKVOm0LFjR7Zu3UrNmjWL1Wf4/fffs2XLFt54441s+4PpM/RUbr+D6enpnDlzht9//73Q/+4LotiHl5EjRzJp0qQ8y2zfvp3GjRsHqEW+V9BrLKwzZ84wZ84cnnzyyQve++u+1q1bc+rUKSZPnuyTLz9/X99fv8ibN29OtWrV6NatG7t376ZBgwZeH7egAvX5paen06dPHy655BKeeuqpbO/58/MT7zz33HPMnTuXVatWZevQ2r9/f/d/N2/enBYtWtCgQQNWrVpFt27diqKpHomLiyMuLs693bFjR5o0acKsWbOYMGFCEbbM99544w2aN29Ou3btsu0P9c8wGBT78DJixIh8F4isX7++V8eOjY0FIDU1lWrVqrn3p6am0qpVK3eZ3377LVu9rKwsjh075q5fWAW9xsK25X//+x+nT59m4MCB+ZZt3749EyZMICMjo9DrXwTq+s5r3749AMnJyTRo0IDY2NgLesqnpqYC+OQzDMT1nThxgp49e1KuXDk++eQTwsPD8yzvy88vN5UrV8Zms7l/luelpqbmej2xsbF5li/I72SgeHN9502ZMoXnnnuOL7/8khYtWuRZtn79+lSuXJnk5OSAf/EV5hrPCw8Pp3Xr1iQnJwPF5zM8deoUc+fO5emnn873PEX5GXoqt9/BqKgoSpUqhc1mK/S/iQLxWe+ZYsTTDrtTpkxx70tLS8uxw+66devcZb744osi7bDrbVs6d+58wSiV3DzzzDOmQoUKXrfVG776Wa9Zs8YA5scffzTG/Nlh96895WfNmmWioqLM2bNnfXcB+fD2+tLS0kyHDh1M586dzalTpwp0rkB9fu3atTPDhg1zbzscDlOjRo08O+z27ds32764uLgLOuzm9TsZSJ5enzHGTJo0yURFRZnExMQCnWP//v3GYrGYBQsWFLq93vDmGv8qKyvLNGrUyDz88MPGmOLxGRrj+h6x2+3myJEj+Z6jqD/D8yhgh91mzZpl2zdgwIALOuwW5t9EgdrqsyMVA7/88ovZuHGjeyjwxo0bzcaNG7MNCW7UqJH5+OOP3dvPPfecKV++vFmwYIHZtGmTuf7663McKt26dWuzdu1as2bNGnPRRRcV6VDpvNry66+/mkaNGpm1a9dmq7dr1y5jsVjM559/fsExP/30U/P666+bzZs3m127dplXXnnFlC5d2owdO9bv1/N3nl5fcnKyefrpp826devMnj17zIIFC0z9+vXNlVde6a5zfqj0NddcY5KSksySJUtMlSpVimyotCfXl5aWZtq3b2+aN29ukpOTsw3NzMrKMsYU7ec3d+5cY7fbzezZs822bdvM3XffbcqXL+8e2XX77bebkSNHust/8803JiwszEyZMsVs377djBs3Lseh0vn9TgaKp9f33HPPmYiICPO///0v22d1/m/QiRMnzCOPPGISExPNnj17zJdffmnatGljLrroooAG6cJc4/jx480XX3xhdu/ebdavX2/69+9vIiMjzdatW91lQvkzPO+KK64wt9566wX7g+0zPHHihPu7DjAvvvii2bhxo/nll1+MMcaMHDnS3H777e7y54dKP/roo2b79u1mxowZOQ6Vzutn5gsKL38xaNAgA1zwWrlypbsMf8yHcZ7T6TRPPvmkiYmJMXa73XTr1s3s3Lkz23GPHj1qBgwYYMqWLWuioqLMHXfckS0QBVJ+bdmzZ88F12yMMaNGjTK1atUyDofjgmN+/vnnplWrVqZs2bKmTJkypmXLlmbmzJk5lvU3T69v37595sorrzQVK1Y0drvdNGzY0Dz66KPZ5nkxxpi9e/eaXr16mVKlSpnKlSubESNGZBtqHCieXt/KlStz/DcNmD179hhjiv7zmz59uqldu7aJiIgw7dq1M9999537vc6dO5tBgwZlK//hhx+aiy++2ERERJimTZuaRYsWZXu/IL+TgeTJ9dWpUyfHz2rcuHHGGGNOnz5trrnmGlOlShUTHh5u6tSpY4YOHerTLwVveHKNw4cPd5eNiYkxvXv3Nhs2bMh2vFD+DI0xZseOHQYwS5cuveBYwfYZ5vY34vw1DRo0yHTu3PmCOq1atTIRERGmfv362b4Tz8vrZ+YLFmMCPJ5VREREpBA0z4uIiIiEFIUXERERCSkKLyIiIhJSFF5EREQkpCi8iIiISEhReBEREZGQovAiIiIiIUXhRUREREKKwouIiIiEFIUXERERCSkKLyIiIhJSFF5EREQkpPw/JsGtlRuQKZsAAAAASUVORK5CYII=",
-                        "text/plain": "<Figure size 640x480 with 1 Axes>"
+                        "text/plain": [
+                            "<Figure size 640x480 with 1 Axes>"
+                        ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "# plot out the ground truth versus predicted responses\n",
```

### Comparing `autora-theorist-bsr-1.0.0rc0/docs/how-it-works.md` & `autora-theorist-bsr-1.0.0rc1/docs/how-it-works.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# Bayesian Symbolic Regression
-
-## How it works
+# How It Works
 
 Bayesian Symbolic Regression (BSR) has the following features:
 
 1. It models equations as expression trees, with root and intermediate tree nodes representing operators (e.g. `*` for a binary node and `sin` for a unary node) and leaf nodes representing features in the data. BSR then defines the search space as the union of the following three parts:
     - Tree structure (T): this represents the structure of the expression tree (e.g. how to recursively construct the tree and when to stop by using leaf nodes), and also specifies the assignment of operators to non-leaf nodes.
     - Leaf nodes (M): this assigns features to leaf nodes that are already defined from part **T**.
     - Operator parameters ($\Theta$): this uses a vector $\Theta$ to collect additional parameters for certain operators which require them (e.g. a linear operator `ln` with intercept and slope params).
```

### Comparing `autora-theorist-bsr-1.0.0rc0/docs/img.png` & `autora-theorist-bsr-1.0.0rc1/docs/img.png`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0rc0/docs/index.md` & `autora-theorist-bsr-1.0.0rc1/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0rc0/docs/meta-parameters.md` & `autora-theorist-bsr-1.0.0rc1/docs/meta-parameters.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# Bayesian Symbolic Regression
-
-## Meta-Parameters
+# Meta-Parameters
 
 Meta-Parameters are used to control the search space and the model configuration. In BSR, they are mainly defined in the theorist constructor (see `bsr.py`). Below is a basic overview of these parameters. Note, there are additional algorithm-irrelevant configurations that can be customized in the constructor; please refer to code documentation for their details.
 
 - `tree_num`: the number of expression trees to use in the linear mixture (final prediction model); also denoted by `K` in BSR.
 - `iter_num`: the number of RJ-MCMC steps to execute (note: this can also be understood as the number of `K`-samples to take in the fitting process).
 - `val`: the number of validation steps to execute following each iteration.
 - `beta`: the hyperparameter that controls growth of a new expression tree. This needs to be < 0, and in general, smaller values of `beta` correspond to deeper expression trees.
```

### Comparing `autora-theorist-bsr-1.0.0rc0/docs/search-space.md` & `autora-theorist-bsr-1.0.0rc1/docs/search-space.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# Bayesian Symbolic Regression
-
-## Search space
+# Search Space
 
 The following are built-in operators which constitute the search space:
 
 - **\+**: The output of the computation $x_j$ is the sum over its inputs $x_i, x_{ii}$: $x_j = x_i + x_{ii}$.
 - **\-**: The output of the computation $x_j$ is the respective difference between its inputs $x_i, x_{ii}$: $x_j = x_i - x_{ii}$.
 - __\*__: The output of the computation $x_j$ is the product over its two inputs $x_i, x_{ii}$: $x_j = x_i * x_{ii}$.
 - **exp**: The output of the computation $x_j$ is the natural exponential function applied to its input $x_i$: $x_j = \exp(x_i)$.
```

### Comparing `autora-theorist-bsr-1.0.0rc0/mkdocs/base.yml` & `autora-theorist-bsr-1.0.0rc1/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0rc0/pyproject.toml` & `autora-theorist-bsr-1.0.0rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 [project]
 name = "autora-theorist-bsr"
 description = "Bayesian Symbolic Regression theorist for AutoRA"
 authors = [
     { name = "Sida (Star) Li", email = "listar2000@uchicago.edu" },
-    { name = "Ben Andrew", email = "benwallaceandrew@gmail.com" },
 ]
 dynamic = ["version"]
 
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.8,<4"
```

### Comparing `autora-theorist-bsr-1.0.0rc0/src/autora/theorist/bsr/funcs.py` & `autora-theorist-bsr-1.0.0rc1/src/autora/theorist/bsr/funcs.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0rc0/src/autora/theorist/bsr/misc.py` & `autora-theorist-bsr-1.0.0rc1/src/autora/theorist/bsr/misc.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0rc0/src/autora/theorist/bsr/node.py` & `autora-theorist-bsr-1.0.0rc1/src/autora/theorist/bsr/node.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0rc0/src/autora/theorist/bsr/operation.py` & `autora-theorist-bsr-1.0.0rc1/src/autora/theorist/bsr/operation.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0rc0/src/autora/theorist/bsr/prior.py` & `autora-theorist-bsr-1.0.0rc1/src/autora/theorist/bsr/prior.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0rc0/src/autora/theorist/bsr/regressor.py` & `autora-theorist-bsr-1.0.0rc1/src/autora/theorist/bsr/regressor.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0rc0/src/autora_theorist_bsr.egg-info/SOURCES.txt` & `autora-theorist-bsr-1.0.0rc1/src/autora_theorist_bsr.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 .gitignore
 .pre-commit-config.yaml
 README.md
 mkdocs.yml
 pyproject.toml
 .github/workflows/python-publish.yml
-docs/basic-usage.ipynb
+docs/Basic Usage.ipynb
 docs/how-it-works.md
 docs/img.png
 docs/index.md
 docs/meta-parameters.md
-docs/quick-start.md
+docs/quickstart.md
 docs/search-space.md
 docs/javascripts/mathjax.js
 mkdocs/base.yml
 src/autora/theorist/bsr/__init__.py
 src/autora/theorist/bsr/funcs.py
 src/autora/theorist/bsr/misc.py
 src/autora/theorist/bsr/node.py
```

### Comparing `autora-theorist-bsr-1.0.0rc0/tests/README.md` & `autora-theorist-bsr-1.0.0rc1/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0rc0/tests/test_bsr_mcmc_actions.py` & `autora-theorist-bsr-1.0.0rc1/tests/test_bsr_mcmc_actions.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0rc0/tests/test_bsr_node_and_operator.py` & `autora-theorist-bsr-1.0.0rc1/tests/test_bsr_node_and_operator.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-bsr-1.0.0rc0/tests/test_bsr_tree_operation.py` & `autora-theorist-bsr-1.0.0rc1/tests/test_bsr_tree_operation.py`

 * *Files identical despite different names*
