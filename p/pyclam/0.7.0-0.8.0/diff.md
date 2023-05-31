# Comparing `tmp/pyclam-0.7.0.tar.gz` & `tmp/pyclam-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyclam-0.7.0.tar", last modified: Wed Jun  1 03:22:11 2022, max compression
+gzip compressed data, was "pyclam-0.8.0.tar", last modified: Wed May 31 17:17:18 2023, max compression
```

## Comparing `pyclam-0.7.0.tar` & `pyclam-0.8.0.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 03:22:11.618459 pyclam-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-06-01 03:21:41.000000 pyclam-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2851 2022-06-01 03:22:11.618459 pyclam-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2475 2022-06-01 03:21:41.000000 pyclam-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 03:22:11.614458 pyclam-0.7.0/pyclam/
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-06-01 03:21:41.000000 pyclam-0.7.0/pyclam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 03:22:11.618459 pyclam-0.7.0/pyclam/anomaly_detection/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-06-01 03:21:41.000000 pyclam-0.7.0/pyclam/anomaly_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10261 2022-06-01 03:21:41.000000 pyclam-0.7.0/pyclam/anomaly_detection/chaoda.py
--rw-r--r--   0 runner    (1001) docker     (121)     7407 2022-06-01 03:21:41.000000 pyclam-0.7.0/pyclam/anomaly_detection/datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)     2083 2022-06-01 03:21:41.000000 pyclam-0.7.0/pyclam/anomaly_detection/graph_selectors.py
--rw-r--r--   0 runner    (1001) docker     (121)     9968 2022-06-01 03:21:41.000000 pyclam-0.7.0/pyclam/anomaly_detection/individual_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (121)     4405 2022-06-01 03:21:41.000000 pyclam-0.7.0/pyclam/anomaly_detection/meta_ml_models.py
--rw-r--r--   0 runner    (1001) docker     (121)    12071 2022-06-01 03:21:41.000000 pyclam-0.7.0/pyclam/anomaly_detection/pretrained_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 03:22:11.618459 pyclam-0.7.0/pyclam/classification/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-06-01 03:21:41.000000 pyclam-0.7.0/pyclam/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1911 2022-06-01 03:21:41.000000 pyclam-0.7.0/pyclam/classification/classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 03:22:11.618459 pyclam-0.7.0/pyclam/core/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-06-01 03:21:41.000000 pyclam-0.7.0/pyclam/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14210 2022-06-01 03:21:41.000000 pyclam-0.7.0/pyclam/core/criterion.py
--rw-r--r--   0 runner    (1001) docker     (121)    48846 2022-06-01 03:21:41.000000 pyclam-0.7.0/pyclam/core/manifold.py
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-06-01 03:21:41.000000 pyclam-0.7.0/pyclam/core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 03:22:11.618459 pyclam-0.7.0/pyclam/search/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-06-01 03:21:41.000000 pyclam-0.7.0/pyclam/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10383 2022-06-01 03:21:41.000000 pyclam-0.7.0/pyclam/search/cakes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 03:22:11.618459 pyclam-0.7.0/pyclam/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-06-01 03:21:41.000000 pyclam-0.7.0/pyclam/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-06-01 03:21:41.000000 pyclam-0.7.0/pyclam/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-06-01 03:21:41.000000 pyclam-0.7.0/pyclam/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4917 2022-06-01 03:21:41.000000 pyclam-0.7.0/pyclam/utils/synthetic_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 03:22:11.614458 pyclam-0.7.0/pyclam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2851 2022-06-01 03:22:10.000000 pyclam-0.7.0/pyclam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-06-01 03:22:11.000000 pyclam-0.7.0/pyclam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-01 03:22:11.000000 pyclam-0.7.0/pyclam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-06-01 03:22:11.000000 pyclam-0.7.0/pyclam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-06-01 03:22:11.000000 pyclam-0.7.0/pyclam.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-01 03:22:11.618459 pyclam-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-06-01 03:21:41.000000 pyclam-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:17:18.227154 pyclam-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-31 17:16:51.000000 pyclam-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-31 17:17:18.223154 pyclam-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-31 17:16:51.000000 pyclam-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:17:18.219154 pyclam-0.8.0/pyclam/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:17:18.223154 pyclam-0.8.0/pyclam/anomaly_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/anomaly_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/anomaly_detection/anomaly_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/anomaly_detection/anomaly_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/anomaly_detection/chaoda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/anomaly_detection/graph_scorers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/anomaly_detection/meta_ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12071 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/anomaly_detection/pretrained_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10060 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/anomaly_detection/training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:17:18.223154 pyclam-0.8.0/pyclam/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/classification/classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:17:18.223154 pyclam-0.8.0/pyclam/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/core/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/core/cluster_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13299 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/core/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/core/graph_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/core/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/core/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:17:18.223154 pyclam-0.8.0/pyclam/search/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/search/cakes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:17:18.223154 pyclam-0.8.0/pyclam/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-31 17:16:51.000000 pyclam-0.8.0/pyclam/utils/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 17:17:18.219154 pyclam-0.8.0/pyclam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-31 17:17:18.000000 pyclam-0.8.0/pyclam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-31 17:17:18.000000 pyclam-0.8.0/pyclam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 17:17:18.000000 pyclam-0.8.0/pyclam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 17:17:18.000000 pyclam-0.8.0/pyclam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 17:17:18.000000 pyclam-0.8.0/pyclam.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 17:17:18.227154 pyclam-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-31 17:16:51.000000 pyclam-0.8.0/setup.py
```

### Comparing `pyclam-0.7.0/LICENSE` & `pyclam-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclam-0.7.0/PKG-INFO` & `pyclam-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyclam
-Version: 0.7.0
+Version: 0.8.0
 Summary: Clustered Learning of Approximate Manifolds
 Home-page: https://github.com/URI-ABD/clam
-Author: Najib Ishaq <nishaq@zoho.com>; Tom Howard <info@tomhoward.codes>; Noah Daniels <noah_daniels@uri.edu>
+Author: Najib Ishaq <najib_ishaq@zoho.com>; Tom Howard <info@tomhoward.codes>; Noah Daniels <noah_daniels@uri.edu>; Morgan Prior <morgan_prior@uri.edu>; Isaac Chen <ijchen@uri.edu>; Oliver McLaughlin <olwmcjp@gmail.com>
 Author-email: 
 License: MIT
 Requires-Python: >=3.9,<3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # URI-ABD: Clustered Learning of Approximate Manifolds
@@ -36,15 +36,15 @@
 
 ### Python Scripting
 
 ```python
 from pyclam import criterion
 from pyclam import Manifold
 from pyclam.search import CAKES
-from pyclam.utils import synthetic_datasets
+from tests import synthetic_datasets
 
 # Get the data.
 data, _ = synthetic_datasets.bullseye()
 # data is a numpy.ndarray in this case but it could just as easily be a numpy.memmap if your data does fit in RAM.
 # We used numpy memmaps for the research, though they impose file-IO costs.
 
 search = CAKES(data, 'euclidean')
@@ -52,18 +52,18 @@
 # TODO: Provide link to CHESS paper
 
 search.build(max_depth=10)
 # Build the search tree to depth of 10.
 # This method can be called again with a higher depth, if needed.
 
 query, radius = data[0], 0.5
-rnn_results = search.rnn(query, radius)
+rnn_results = search.rnn_search(query, radius)
 # This is how we perform rho-nearest neighbors search with radius 0.5 around the query.
 
-knn_results = search.knn(query, 10)
+knn_results = search.knn_search(query, 10)
 # This is how to perform k-nearest neighbors search for the 10 nearest neighbors of query.
 
 # TODO: Provide snippets for using CHAODA
 
 # You can also directly use the Manifold functionality provided by CLAM.
 
 manifold = Manifold(data, 'euclidean')
```

### Comparing `pyclam-0.7.0/README.md` & `pyclam-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ### Python Scripting
 
 ```python
 from pyclam import criterion
 from pyclam import Manifold
 from pyclam.search import CAKES
-from pyclam.utils import synthetic_datasets
+from tests import synthetic_datasets
 
 # Get the data.
 data, _ = synthetic_datasets.bullseye()
 # data is a numpy.ndarray in this case but it could just as easily be a numpy.memmap if your data does fit in RAM.
 # We used numpy memmaps for the research, though they impose file-IO costs.
 
 search = CAKES(data, 'euclidean')
@@ -40,18 +40,18 @@
 # TODO: Provide link to CHESS paper
 
 search.build(max_depth=10)
 # Build the search tree to depth of 10.
 # This method can be called again with a higher depth, if needed.
 
 query, radius = data[0], 0.5
-rnn_results = search.rnn(query, radius)
+rnn_results = search.rnn_search(query, radius)
 # This is how we perform rho-nearest neighbors search with radius 0.5 around the query.
 
-knn_results = search.knn(query, 10)
+knn_results = search.knn_search(query, 10)
 # This is how to perform k-nearest neighbors search for the 10 nearest neighbors of query.
 
 # TODO: Provide snippets for using CHAODA
 
 # You can also directly use the Manifold functionality provided by CLAM.
 
 manifold = Manifold(data, 'euclidean')
```

### Comparing `pyclam-0.7.0/pyclam/anomaly_detection/chaoda.py` & `pyclam-0.8.0/pyclam/anomaly_detection/chaoda.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,240 +1,285 @@
-""" This module provides the CHAODA algorithms implemented on top of CLAM.
-"""
-import logging
+import inspect
+import math
 import typing
 
 import numpy
 
-from . import graph_selectors
-from . import individual_algorithms
+from . import graph_scorers
+from . import pretrained_models
 from .. import core
 from .. import search
 from .. import utils
-from ..core import criterion
+from ..core import cluster_criteria
+from ..core import graph_criteria
 from ..utils import constants
+from ..utils import helpers
 
-logger = logging.getLogger(__name__)
-logger.setLevel(constants.LOG_LEVEL)
+logger = helpers.make_logger(__name__)
 
 VotingMode = typing.Literal[
     'mean',
     'product',
     'median',
     'min',
     'max',
     'p25',
     'p75',
 ]
 
+DEFAULT_GRAPH_CRITERIA = [
+    graph_criteria.MetaMLSelect(function, min_depth=4)
+    for _, function in inspect.getmembers(pretrained_models, inspect.isfunction)
+]
+
+DEFAULT_GRAPH_SCORERS: list[graph_scorers.GraphScorer] = [
+    graph_scorers.ClusterCardinality(),
+    graph_scorers.ComponentCardinality(),
+    graph_scorers.VertexDegree(),
+    graph_scorers.ParentCardinality(depth_weight=lambda d: 1 / (d ** 0.5)),
+    graph_scorers.GraphNeighborhood(eccentricity_fraction=0.25),
+    graph_scorers.StationaryProbabilities(steps=16),
+]
+
 
 class CHAODA:
     # TODO: Allow weights for each method in ensemble. Perhaps with an Ensembler class?
 
     def __init__(
-            self, *,
-            metrics: typing.Optional[list[str]] = None,  # TODO: convert this to a metric class to allow for custom metrics from users.
-            partition_criteria: typing.Optional[list[criterion.ClusterCriterion]] = None,
-            selector_scorers: typing.Optional[list[tuple[graph_selectors.GraphSelector, list[individual_algorithms.GraphScorer]]]] = None,
-            normalization_mode: str = 'gaussian',
+            self,
+            metric_spaces: list[core.Space],
+            *,
+            partition_criteria: typing.Optional[list[cluster_criteria.ClusterCriterion]] = None,
+            selector_scorers: typing.Optional[list[tuple[graph_criteria.GraphCriterion, list[graph_scorers.GraphScorer]]]] = None,
+            normalization_mode: helpers.NormalizationMode = 'gaussian',
             use_speed_threshold: bool = True,
             voting_mode: VotingMode = 'mean',
     ):
         """ Creates and initializes a CHAODA object.
 
         Args:
-            metrics: list of distance metrics to use for constructing manifolds.
-            partition_criteria: list of criteria for partitioning clusters when building trees in the manifolds.
+            metric_spaces: A list of metric spaces to use for anomaly detection.
+                All metric spaces should have the same `Dataset` object.
+            partition_criteria: list of criteria for partitioning clusters when
+                building trees.
             selector_scorers: list of 2-tuples whose items are
-                - a trained meta-ml model for selecting a graph from a manifold.
+                - a trained meta-ml model for selecting a graph.
                 - a list of individual algorithms to run on that graph.
-            normalization_mode: What normalization mode to use. Must be one of 'linear', 'gaussian', or 'sigmoid'.
-            use_speed_threshold: number of clusters above which to skip the slow methods.
-            voting_mode: voting method to use to aggregate scores in the ensemble
-        """
-        self.metrics: list[str] = metrics or ['euclidean', 'cityblock']
-        self.partition_criteria: list[criterion.ClusterCriterion] = partition_criteria or [
-            criterion.MaxDepth(25),
-            criterion.MinPoints(1),
+            normalization_mode: What normalization mode to use. Must be one of
+                - 'linear',
+                - 'gaussian', or
+                - 'sigmoid'.
+            use_speed_threshold: Whether to skip slow graph scorers.
+            voting_mode: to use to aggregate scores for the ensemble.
+        """
+        for i, l in enumerate(metric_spaces):
+            for j, r in enumerate(metric_spaces[i + 1:], start=i + 1):
+                if not l.data == r.data:
+                    raise ValueError(f'Metric spaces {l.name} and {r.name} had different datasets.')
+
+        self.__metric_spaces = metric_spaces
+
+        self.__partition_criteria: list[cluster_criteria.ClusterCriterion] = partition_criteria or [
+            cluster_criteria.MinPoints(int(math.log2(self.__metric_spaces[0].data.cardinality))),
+        ]
+
+        self.__selector_scorers: list[tuple[graph_criteria.GraphCriterion, list[graph_scorers.GraphScorer]]] = selector_scorers or [
+            (c, [s for s in DEFAULT_GRAPH_SCORERS if s.name in c.name])
+            for c in DEFAULT_GRAPH_CRITERIA
         ]
 
-        self.selector_scorers: list[tuple[graph_selectors.GraphSelector, list[individual_algorithms.GraphScorer]]] = selector_scorers or list()
-        if len(self.selector_scorers) == 0:
-            for selector in graph_selectors.DEFAULT_SELECTORS:
-                scorers = [
-                    scorer for scorer in individual_algorithms.DEFAULT_SCORERS
-                    if scorer.name == selector.scorer_name
-                ]
-                self.selector_scorers.append((selector, scorers))
-
-        self.normalization_mode = normalization_mode
-        self.use_speed_threshold = use_speed_threshold
-        self.voting_mode = voting_mode
-
-        self.bowls = [
-            SingleMetricChaoda(metric, self.partition_criteria, self.selector_scorers, self.normalization_mode, self.use_speed_threshold)
-            for metric in self.metrics
+        self.__normalization_mode = normalization_mode
+        self.__use_speed_threshold = use_speed_threshold
+        self.__voting_mode = voting_mode
+
+        self.__bowls = [
+            SingleSpaceChaoda(
+                metric_space,
+                self.__partition_criteria,
+                self.__selector_scorers,
+                self.__normalization_mode,
+                self.__use_speed_threshold,
+            )
+            for metric_space in self.__metric_spaces
         ]
 
         self.__scores: typing.Union[numpy.ndarray, utils.Unset] = constants.UNSET
 
-    def fit(self, data: numpy.ndarray, *, indices: typing.Optional[list[int]] = None) -> 'CHAODA':
-        indices = indices or list(range(data.shape[0]))
-        self.bowls = [bowl.fit(data, indices) for bowl in self.bowls]
-        individual_scores = numpy.stack([bowl.scores for bowl in self.bowls])
+    def build(self) -> 'CHAODA':
+        self.__bowls = [bowl.build() for bowl in self.__bowls]
+        individual_scores = numpy.concatenate([bowl.scores for bowl in self.__bowls])
         self.__scores = self.__vote(individual_scores)
         return self
 
     def __vote(self, scores: numpy.ndarray) -> numpy.ndarray:
         """ Vote among individual scores for ensemble score.
         """
-        if self.voting_mode == 'mean':
+        if self.__voting_mode == 'mean':
             scores = numpy.mean(scores, axis=0)
-        elif self.voting_mode == 'product':
+        elif self.__voting_mode == 'product':
             scores = numpy.product(scores, axis=0)
-        elif self.voting_mode == 'median':
+        elif self.__voting_mode == 'median':
             scores = numpy.median(scores, axis=0)
-        elif self.voting_mode == 'min':
+        elif self.__voting_mode == 'min':
             scores = numpy.min(scores, axis=0)
-        elif self.voting_mode == 'max':
+        elif self.__voting_mode == 'max':
             scores = numpy.max(scores, axis=0)
-        elif self.voting_mode == 'p25':
+        elif self.__voting_mode == 'p25':
             scores = numpy.percentile(scores, 25, axis=0)
-        elif self.voting_mode == 'p75':
+        else:  # self.__voting_mode == 'p75'
             scores = numpy.percentile(scores, 75, axis=0)
-        else:
-            # TODO: Investigate other voting methods.
-            raise NotImplementedError(f'voting mode {self.voting_mode} is not implemented. Try one of {VotingMode}.')
 
         return scores
 
     @property
     def scores(self) -> numpy.ndarray:
-        if isinstance(self.__scores, utils.Unset):
-            raise ValueError(f'Please call the `fit` method before fetching anomaly scores.')
+        if self.__scores is constants.UNSET:
+            raise ValueError(f'Please call the `fit` method before using this property.')
         return self.__scores
 
-    def fit_predict(self, data: numpy.ndarray, *, indices: typing.Optional[list[int]] = None) -> numpy.ndarray:
-        self.fit(data, indices=indices)
-        return self.scores
+    def fit_predict(self) -> numpy.ndarray:
+        self.build()
+        return self.__scores
 
-    def predict_single(self, query: numpy.array) -> float:
+    def predict_single(self, query) -> float:
         """ Predict the anomaly score for a single query.
         """
         scores = list()
-        for bowl in self.bowls:
-            searcher = search.CAKES.from_manifold(bowl.manifold)
-
+        for bowl in self.__bowls:
             for cluster_scores in bowl.cluster_scores_list:
-                hits = list(searcher.tree_search_history(query, radius=0)[0].keys())
+                hits = set(bowl.searcher.tree_search_history(query, 0.)[0].keys())
 
-                intersection = [cluster for cluster in hits if cluster in cluster_scores]
+                intersection = hits.intersection(set(cluster_scores.keys()))
                 if len(intersection) > 0:
-                    individual_scores = [cluster_scores[cluster] for cluster in intersection]
+                    score = self.__vote(numpy.asarray([cluster_scores[c] for c in intersection], dtype=numpy.float32))
                 else:
-                    individual_scores = [1.]
+                    score = 1.
+                scores.append(1. if numpy.isnan(score) else float(score))
 
-                scores.append(self.__vote(numpy.asarray(individual_scores, dtype=numpy.float32)))
+        final_score = self.__vote(numpy.asarray(scores, dtype=numpy.float32))
+        return float(final_score)
 
-        score = self.__vote(numpy.asarray(scores, dtype=numpy.float32))
-        return float(score)
-
-    def predict(self, queries: numpy.array) -> numpy.array:
-        """ Predict the anomaly score for a 2d array of queries.
+    def predict(self, queries: core.Dataset) -> numpy.ndarray:
+        """ Predict the anomaly scores for a 2d array of queries.
         """
         scores = list()
-        for i in range(queries.shape[0]):
+        for i in range(queries.cardinality):
             logger.info(f'Predicting anomaly score for query {i} ...')
             scores.append(self.predict_single(queries[i]))
-        return numpy.array(scores, dtype=numpy.float32)
+        return numpy.asarray(scores, dtype=numpy.float32)
+
+
+class SingleSpaceChaoda:
+    """ This class is a single-metric-space version of CHAODA. This is intended
+    to be used from the CHAODA class. This class has almost no input validation.
 
+    This class does not vote among scores to form an ensemble.
+    """
 
-class SingleMetricChaoda:
-    # TODO: metric argument and type: replace with a Metric class
     def __init__(
             self,
-            metric: str,
-            partition_criteria: list[criterion.ClusterCriterion],
-            selectors_scorers: list[tuple[graph_selectors.GraphSelector, list[individual_algorithms.GraphScorer]]],
-            normalization_mode: str,
+            metric_space: core.Space,
+            partition_criteria: list[cluster_criteria.ClusterCriterion],
+            selectors_scorers: list[tuple[graph_criteria.GraphCriterion, list[graph_scorers.GraphScorer]]],
+            normalization_mode: helpers.NormalizationMode,
             use_speed_threshold: bool,
     ):
-        """ This class is a single-metric version of CHAODA. This is intended to
-         be used from the CHAODA class. All input validation should be done in
-         CHAODA and not here.
+        """ Creates single-metric-space version of chaoda.
 
         Args:
-            metric: name of the metric used.
-            partition_criteria:
+            metric_space: The metric space to use.
+            partition_criteria: A list of criteria to use for partitioning
+                clusters.
             selectors_scorers: list of 2-tuples whose items are
-                - a trained meta-ml model for selecting clusters to build graphs.
+                - a trained meta-ml model for selecting clusters to build
+                  graphs.
                 - a list of individual algorithms for predicting anomaly scores
                   from that graph.
-            normalization_mode: method to use to normalize anomaly scores from different scoring algorithms.
-            use_speed_threshold: Whether to only run the fast algorithms in the ensemble.
+            normalization_mode: method to use to normalize anomaly scores from
+                different scoring algorithms.
+            use_speed_threshold: Whether to only run the fast algorithms in the
+                ensemble.
         """
 
-        self.metric = metric
-        self.partition_criteria = partition_criteria
-        self.selectors_scorers = selectors_scorers
-        self.normalization_mode = normalization_mode
-        self.use_speed_threshold = use_speed_threshold
-
-        self.__manifold: typing.Union[core.Manifold, utils.Unset] = constants.UNSET
-        self.__cluster_scores_list: typing.Union[list[individual_algorithms.ClusterScores], utils.Unset] = constants.UNSET
+        self.__metric_space = metric_space
+        self.__partition_criteria = partition_criteria
+        self.__selectors = [s for s, _ in selectors_scorers]
+        self.__scorers = [s for _, s in selectors_scorers]
+        self.__normalization_mode = normalization_mode
+        self.__use_speed_threshold = use_speed_threshold
+
+        self.__root: typing.Union[core.Cluster, utils.Unset] = constants.UNSET
+        self.__graphs: typing.Union[list[core.Graph], utils.Unset] = constants.UNSET
+        self.__cluster_scores_list: typing.Union[list[graph_scorers.ClusterScores], utils.Unset] = constants.UNSET
         self.__scores: typing.Union[numpy.ndarray, utils.Unset] = constants.UNSET
+        self.__searcher: typing.Union[search.CAKES, utils.Unset] = constants.UNSET
 
     @property
-    def manifold(self) -> core.Manifold:
-        if isinstance(self.__manifold, utils.Unset):
-            raise ValueError(f'Please call the `fit` method before fetching the manifold.')
-        return self.__manifold
+    def root(self) -> core.Cluster:
+        if self.__root is constants.UNSET:
+            raise ValueError(f'Please call the `fit` method before using this property.')
+        return self.__root
 
     @property
     def scores(self) -> numpy.ndarray:
-        if isinstance(self.__scores, utils.Unset):
-            raise ValueError(f'Please call the `fit` method before fetching anomaly scores.')
+        if self.__scores is constants.UNSET:
+            raise ValueError(f'Please call the `fit` method before using this property.')
         return self.__scores
 
     @property
-    def cluster_scores_list(self) -> list[individual_algorithms.ClusterScores]:
-        if isinstance(self.__cluster_scores_list, utils.Unset):
-            raise ValueError(f'Please call the `fit` method before fetching dict of cluster scores.')
+    def cluster_scores_list(self) -> list[graph_scorers.ClusterScores]:
+        if self.__cluster_scores_list is constants.UNSET:
+            raise ValueError(f'Please call the `fit` method before using this property.')
         return self.__cluster_scores_list
 
-    def fit(self, data: numpy.ndarray, indices: list[int]) -> 'SingleMetricChaoda':
-        """ Build a Manifold on the given data, create optimal Graphs, and predict anomaly scores for each Graph.
-
-        Args:
-            data: A 2d array where rows are instances and columns are features.
-            indices: A list of indices of rows from data on which to fit the model.
+    @property
+    def searcher(self) -> search.CAKES:
+        if self.__searcher is constants.UNSET:
+            raise ValueError(f'Please call the `fit` method before using this property.')
+        return self.__searcher
+
+    def build(self) -> 'SingleSpaceChaoda':
+        """ Build a Manifold on the given data, create optimal Graphs, and
+         predict anomaly scores for each Graph.
         """
-        self.__manifold = core.Manifold(data, self.metric, indices).build(*self.partition_criteria)
-        self.__manifold.layers[-1].build_edges()
-
-        graphs_scorers = [
-            (core.Graph(*selector(self.__manifold.root)).build_edges(), scorers)
-            for selector, scorers in self.selectors_scorers
+        self.__root = (
+            core.Cluster.new_root(self.__metric_space)
+                .build()
+                .iterative_partition(self.__partition_criteria)
+                .normalize_ratios(mode=self.__normalization_mode)
+        )
+        self.__searcher = search.CAKES.from_root(self.__root)
+
+        self.__graphs = [
+            core.Graph(selector(self.__root)).build()
+            for selector in self.__selectors
         ]
 
-        if self.use_speed_threshold:
+        if self.__use_speed_threshold:
             individual_scores = [
-                method(graph)
-                for graph, scorers in graphs_scorers
+                method(g)
+                for g, scorers in zip(self.__graphs, self.__scorers)
                 for method in scorers
-                if method.should_be_fast(graph)
+                if method.should_be_fast(g)
             ]
             if len(individual_scores) == 0:
-                uniform_cluster_scores = {self.__manifold.root: .5}
-                uniform_scores = 0.5 * numpy.ones(shape=(len(indices,)))
+                uniform_cluster_scores = {self.__root: .5}
+                uniform_scores = 0.5 * numpy.ones(shape=(self.__root.cardinality, ))
                 individual_scores.append((uniform_cluster_scores, uniform_scores))
         else:
             individual_scores = [
-                method(graph)
-                for graph, scorers in graphs_scorers
+                method(g)
+                for g, scorers in zip(self.__graphs, self.__scorers)
                 for method in scorers
             ]
 
-        [cluster_scores, scores] = list(zip(*individual_scores))
-        self.__scores = numpy.stack(scores)
-        self.__cluster_scores_list = cluster_scores
+        self.__scores = numpy.stack([s for _, s in individual_scores])
+        self.__cluster_scores_list = [d for d, _ in individual_scores]
+
         return self
+
+
+__all__ = [
+    'VotingMode',
+    'CHAODA',
+    'SingleSpaceChaoda',
+]
```

### Comparing `pyclam-0.7.0/pyclam/anomaly_detection/individual_algorithms.py` & `pyclam-0.8.0/pyclam/anomaly_detection/graph_scorers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 import abc
-import logging
 import typing
 
 import numpy
 
 from .. import core
 from ..utils import constants
 from ..utils import helpers
 
-logger = logging.getLogger(__name__)
-logger.setLevel(constants.LOG_LEVEL)
+logger = helpers.make_logger(__name__)
 
 ClusterScores = dict[core.Cluster, float]
-DatumScores = dict[int, float]
+InstanceScores = dict[int, float]
 
 # TODO: Look at DSD (diffusion-state-distance) as a possible individual-method.
+# TODO: Specialize `should_be_fast` for each algorithm based on complexity analysis and graph properties.
 
 
 class GraphScorer(abc.ABC):
 
-    def __init__(self):
-        self.__cluster_scores: ClusterScores = dict()
-        self.__datum_scores: list[float] = list()
-
-    def __call__(self, graph: core.Graph) -> tuple[ClusterScores, numpy.ndarray]:
-        """ Use this scorer to generate normalized anomaly scores for the given graph.
+    def __call__(self, g: core.Graph) -> tuple[ClusterScores, numpy.ndarray]:
+        """ Use this scorer to generate normalized anomaly scores.
         """
-        logger.info(f'Running method {self.name} on a graph with {graph.cardinality} clusters.')
-        self.__cluster_scores = self.score_graph(graph)
-        self.__normalize_scores()
-        self.__inherit_scores(graph.manifold.argpoints)
-        self.__individual_scores = numpy.asarray(self.__datum_scores, dtype=numpy.float32)
-        return self.__cluster_scores, self.__individual_scores
+        logger.info(f'Running method {self.name} on a graph with {g.vertex_cardinality} clusters.')
 
-    @property
-    def cluster_scores(self) -> ClusterScores:
-        return self.__cluster_scores
+        cluster_scores = self.score_graph(g)
+        if self.normalize_on_clusters:
+            cluster_scores = self.__normalize_scores(cluster_scores)
+
+        instance_scores = self.inherit_scores(cluster_scores)
+        if not self.normalize_on_clusters:
+            instance_scores = self.__normalize_scores(instance_scores)
 
-    @property
-    def individual_scores(self) -> numpy.ndarray:
-        return self.__individual_scores
+        scores_array = self.ordered_scores(g, instance_scores)
+        return cluster_scores, scores_array
+
+    @abc.abstractmethod
+    def __hash__(self):
+        """ A way to uniquely identify each `GraphScorer` object.
+        """
+        pass
 
     @property
     @abc.abstractmethod
     def name(self) -> str:
         """ Full name of the algorithm.
         """
         pass
@@ -51,251 +50,289 @@
     @property
     @abc.abstractmethod
     def short_name(self) -> str:
         """ Abbreviated name of the algorithm.
         """
         pass
 
+    @property
     @abc.abstractmethod
-    def score_graph(self, graph: core.Graph) -> ClusterScores:
-        """ The method with which to assign anomaly scores to Clusters in the
-         Graph. This should return a dictionary whose keys are Clusters in the
-         Graph and whose values are the anomaly scores (before normalization).
+    def normalize_on_clusters(self) -> bool:
+        """ Whether to normalize scores for clusters or for instances.
         """
         pass
 
-    @staticmethod
-    def should_be_fast(graph: core.Graph) -> bool:
-        """ Whether this algorithm is expected to run in a reasonably short
-         time on the given Graph. This method should make a quick estimate.
+    @property
+    @abc.abstractmethod
+    def normalization_mode(self) -> helpers.NormalizationMode:
+        """ What normalization method to use.
         """
-        # TODO: Specialize this for each algorithm based on complexity analysis and graph properties.
-        return graph.cardinality <= 128
+        pass
 
-    def __normalize_scores(self):
-        if len(self.__cluster_scores) == 0:
-            raise ValueError(f'This scoring method needs to be called on a Graph before scores can be normalized.')
-
-        scores = numpy.asarray(list(self.__cluster_scores.values()), dtype=numpy.float32)
-        scores = helpers.normalize(scores, mode='gaussian')
-        self.__cluster_scores = {cluster: score for cluster, score in zip(self.__cluster_scores.keys(), map(float, scores))}
-        return
-
-    def __inherit_scores(self, manifold_indices: list[int]):
-        if len(self.__cluster_scores) == 0:
-            raise ValueError(f'This scoring method needs to be called on a Graph before scores can be assigned from Clusters to Instances.')
+    @abc.abstractmethod
+    def score_graph(self, g: core.Graph) -> ClusterScores:
+        """ The method with which to assign anomaly scores to `Clusters` in the
+        `Graph`. This should return a dictionary whose keys are `Clusters` in
+        the `Graph` and whose values are the pre-normalization anomaly scores.
+        """
+        pass
 
-        scores = {index: score for cluster, score in self.__cluster_scores.items() for index in cluster.argpoints}
+    @abc.abstractmethod
+    def should_be_fast(self, g: core.Graph) -> bool:
+        """ Whether this algorithm is expected to run in a reasonably short
+        time on the given `Graph`. This method should make a quick estimate.
+        """
+        pass
 
-        self.__datum_scores = [scores[i] for i in manifold_indices]
-        return
+    def __normalize_scores(
+            self,
+            scores: typing.Union[ClusterScores, InstanceScores],
+    ) -> typing.Union[ClusterScores, InstanceScores]:
+        [keys, scores] = list(zip(*scores.items()))
+        scores = helpers.normalize(numpy.asarray(scores, dtype=numpy.float32), mode=self.normalization_mode)
+        return {c: s for c, s in zip(keys, map(float, scores))}
 
     @staticmethod
-    def score_subsumed(
-            subsumer_scores: ClusterScores,
-            subsumer_subsumed: dict[core.Cluster, set[core.Cluster]],
-    ) -> ClusterScores:
-        """ Given scores for subsumer Clusters and a mapping between
-         subsumer-subsumed Clusters, assigns the scores from the subsumer
-         to each subsumed. If a Cluster is subsumed by multiple Clusters, the
-         highest score from among the subsumers is assigned to the subsumed.
-
-         Cluster A is subsumed by Cluster B if the volume of A lies entirely
-          inside B.
-
-        Args:
-            subsumer_scores: dict of scores of Clusters that are not subsumed by any
-             other cluster.
-            subsumer_subsumed: dict where the key is a subsumer Cluster and the
-             value is a set of subsumed Clusters.
-
-        Side effects:
-            - modifies subsumer_scores
+    def inherit_scores(scores: ClusterScores) -> InstanceScores:
+        return {i: s for c, s in scores.items() for i in c.indices}
 
-        Returns:
-            Anomaly scores for each Cluster.
-        """
-        for subsumer, subsumed_set in subsumer_subsumed.items():
-            for subsumed in subsumed_set:
-                if subsumed in subsumer_scores:
-                    subsumer_scores[subsumed] = max(subsumer_scores[subsumed], subsumer_scores[subsumer])
-                else:
-                    subsumer_scores[subsumed] = subsumer_scores[subsumer]
-        return subsumer_scores
+    @staticmethod
+    def ordered_scores(g: core.Graph, scores: InstanceScores) -> numpy.ndarray:
+        [indices, scores] = list(zip(*sorted(scores.items())))
+        assert set(indices) == {i for c in g.clusters for i in c.indices}
+        return numpy.asarray(scores, dtype=numpy.float32)
 
 
 class ClusterCardinality(GraphScorer):
 
+    def __hash__(self):
+        return hash(self.name)
+
     @property
     def name(self) -> str:
         return 'cluster_cardinality'
 
     @property
     def short_name(self) -> str:
         return 'cc'
 
-    def score_graph(self, graph: core.Graph) -> ClusterScores:
-        return {cluster: cluster.cardinality for cluster in graph.clusters}
+    @property
+    def normalize_on_clusters(self) -> bool:
+        return True
+
+    @property
+    def normalization_mode(self) -> helpers.NormalizationMode:
+        return 'gaussian'
+
+    def should_be_fast(self, _) -> bool:
+        return True
+
+    def score_graph(self, g: core.Graph) -> ClusterScores:
+        return {c: -c.cardinality for c in g.clusters}
 
 
 class ComponentCardinality(GraphScorer):
 
+    def __hash__(self):
+        return hash(self.name)
+
     @property
     def name(self) -> str:
         return 'component_cardinality'
 
     @property
     def short_name(self) -> str:
         return 'sc'
 
-    def score_graph(self, graph: core.Graph) -> ClusterScores:
+    @property
+    def normalize_on_clusters(self) -> bool:
+        return True
+
+    @property
+    def normalization_mode(self) -> helpers.NormalizationMode:
+        return 'gaussian'
+
+    def should_be_fast(self, _) -> bool:
+        return True
+
+    def score_graph(self, g: core.Graph) -> ClusterScores:
         return {
-            cluster: component.cardinality
-            for component in graph.components
-            for cluster in component.clusters
+            c: -component.vertex_cardinality
+            for component in g.components
+            for c in component.clusters
         }
 
 
 class VertexDegree(GraphScorer):
 
+    def __hash__(self):
+        return hash(self.name)
+
     @property
     def name(self) -> str:
         return 'vertex_degree'
 
     @property
     def short_name(self) -> str:
         return 'vd'
 
-    def score_graph(self, graph: core.Graph) -> ClusterScores:
-        return {cluster: graph.vertex_degree(cluster) for cluster in graph.clusters}
+    @property
+    def normalize_on_clusters(self) -> bool:
+        return True
+
+    @property
+    def normalization_mode(self) -> helpers.NormalizationMode:
+        return 'gaussian'
+
+    def should_be_fast(self, _) -> bool:
+        return True
+
+    def score_graph(self, g: core.Graph) -> ClusterScores:
+        return {c: -g.vertex_degree(c) for c in g.clusters}
 
 
 class ParentCardinality(GraphScorer):
 
-    def __init__(self, weight: typing.Callable[[int], float] = None):
-        super().__init__()
-        self.weight = (lambda d: 1 / (d ** 0.5)) if weight is None else weight
+    def __init__(self, depth_weight: typing.Callable[[int], float]):
+        self.weight = depth_weight
+
+    def __hash__(self):
+        return hash(self.name)
 
     @property
     def name(self) -> str:
         return 'parent_cardinality'
 
     @property
     def short_name(self) -> str:
         return 'pc'
 
-    def score_graph(self, graph: core.Graph) -> ClusterScores:
+    @property
+    def normalize_on_clusters(self) -> bool:
+        return True
+
+    @property
+    def normalization_mode(self) -> helpers.NormalizationMode:
+        return 'gaussian'
 
-        scores = {cluster: 0 for cluster in graph.clusters}
+    def should_be_fast(self, _) -> bool:
+        return True
 
-        for cluster in graph.clusters:
-            ancestry = graph.manifold.ancestry(cluster)
+    def score_graph(self, g: core.Graph) -> ClusterScores:
+
+        scores = {c: 0 for c in g.clusters}
+
+        for c in g.clusters:
+            ancestry = c.ancestry
             for i in range(1, len(ancestry)):
-                scores[cluster] += (self.weight(i) * ancestry[i - 1].cardinality / ancestry[i].cardinality)
+                scores[c] += (self.weight(i) * ancestry[i - 1].cardinality / ancestry[i].cardinality)
 
-        return {cluster: -scores[cluster] for cluster in graph.clusters}
+        return {c: scores[c] for c in g.clusters}
 
 
 class GraphNeighborhood(GraphScorer):
 
-    def __init__(self, eccentricity_fraction: float = 0.25):
+    def __init__(self, eccentricity_fraction: float):
         if not (0 < eccentricity_fraction <= 1):
             raise ValueError(f'eccentricity fraction must be in the (0, 1] range. Got {eccentricity_fraction:.2e} instead.')
 
-        super().__init__()
         self.eccentricity_fraction = eccentricity_fraction
 
+    def __hash__(self):
+        return hash(self.name)
+
     @property
     def name(self) -> str:
         return 'graph_neighborhood'
 
     @property
     def short_name(self) -> str:
         return 'gn'
 
-    @staticmethod
-    def __neighborhood_sizes(start: core.Cluster, steps: int, pruned_graph: core.Graph) -> list[int]:
-        """ Returns the number of clusters in the frontier at each step in a
-         breadth-first traversal of the graph.
-        """
-        visited: set[core.Cluster] = set()
-        frontier: set[core.Cluster] = {start}
-        frontier_sizes = [1]
-
-        for _ in range(steps):
-            if len(frontier) > 0:
-                visited.update(frontier)
-                frontier = {
-                    neighbor for cluster in frontier
-                    for neighbor in pruned_graph.neighbors(cluster)
-                    if neighbor not in visited
-                }
-                frontier_sizes.append(len(frontier))
-            else:
-                break
+    @property
+    def normalize_on_clusters(self) -> bool:
+        return True
+
+    @property
+    def normalization_mode(self) -> helpers.NormalizationMode:
+        return 'gaussian'
 
-        return frontier_sizes
+    def should_be_fast(self, g: core.Graph) -> bool:
+        return g.vertex_cardinality < 256
 
-    def score_graph(self, graph: core.Graph) -> ClusterScores:
+    def num_steps(self, g: core.Graph, c: core.Cluster) -> int:
+        return int(g.eccentricity(c) * self.eccentricity_fraction) + 1
 
-        pruned_graph, subsumer_subsumed = graph.pruned_graph
+    def score_graph(self, g: core.Graph) -> ClusterScores:
 
         step_sizes: dict[core.Cluster, list[int]] = {
-            cluster: self.__neighborhood_sizes(
-                start=cluster,
-                steps=int(pruned_graph.eccentricity(cluster) * self.eccentricity_fraction),
-                pruned_graph=pruned_graph,
-            )
-            for cluster in pruned_graph.clusters
+            c: g.frontier_sizes(c)[:self.num_steps(g, c)]
+            for c in g.clusters
         }
-        subsumer_scores = {cluster: -float(sum(sizes)) for cluster, sizes in step_sizes.items()}
+        scores = {c: -float(sum(sizes)) for c, sizes in step_sizes.items()}
 
-        return self.score_subsumed(subsumer_scores, subsumer_subsumed)
+        return scores
 
 
 class StationaryProbabilities(GraphScorer):
 
-    def __init__(self, steps: int = 16):
-        super().__init__()
+    def __init__(self, steps: int):
         self.steps = steps
 
+    def __hash__(self):
+        return hash(self.name)
+
     @property
     def name(self) -> str:
         return 'stationary_probabilities'
 
     @property
     def short_name(self) -> str:
         return 'sp'
 
-    def score_graph(self, graph: core.Graph) -> ClusterScores:
+    @property
+    def normalize_on_clusters(self) -> bool:
+        return True
+
+    @property
+    def normalization_mode(self) -> helpers.NormalizationMode:
+        return 'gaussian'
+
+    def should_be_fast(self, g: core.Graph) -> bool:
+        return True
+
+    def score_graph(self, g: core.Graph) -> ClusterScores:
 
-        pruned_graph, subsumer_subsumed = graph.pruned_graph
-        subsumer_scores = dict()
+        scores = dict()
 
-        for component in pruned_graph.components:
+        for component in g.components:
 
-            if component.cardinality > 1:
-                clusters, matrix = component.as_matrix
-                matrix = matrix / numpy.sum(matrix, axis=1)[:, None]
+            if component.vertex_cardinality > 1:
+                clusters, matrix = component.distance_matrix
 
+                # TODO: Figure out how to go until convergence.
+                sums = numpy.sum(matrix, axis=1)[:, None] + constants.EPSILON
+                matrix = matrix / sums
                 for _ in range(self.steps):
-                    # TODO: Go until convergence. For now, matrix ^ (2 ^ 16) ought to be enough.
                     matrix = numpy.linalg.matrix_power(matrix, 2)
 
-                subsumer_scores.update({cluster: score for cluster, score in zip(clusters, numpy.sum(matrix, axis=0))})
+                scores.update({c: s for c, s in zip(clusters, numpy.sum(matrix, axis=0))})
 
             else:  # Component with only one Cluster means that the Cluster is anomalous.
-                subsumer_scores.update({cluster: 0 for cluster in component.clusters})
+                scores.update({c: 0 for c in component.clusters})
 
-        subsumer_scores = {cluster: -score for cluster, score in subsumer_scores.items()}
+        scores = {c: -s for c, s in scores.items()}
 
-        return self.score_subsumed(subsumer_scores, subsumer_subsumed)
+        return scores
 
 
-DEFAULT_SCORERS = [
-    ClusterCardinality(),
-    ComponentCardinality(),
-    VertexDegree(),
-    ParentCardinality(),
-    GraphNeighborhood(),
-    StationaryProbabilities(),
+__all__ = [
+    'ClusterScores',
+    'InstanceScores',
+    'GraphScorer',
+    'ClusterCardinality',
+    'ComponentCardinality',
+    'VertexDegree',
+    'ParentCardinality',
+    'GraphNeighborhood',
+    'StationaryProbabilities',
 ]
```

### Comparing `pyclam-0.7.0/pyclam/anomaly_detection/meta_ml_models.py` & `pyclam-0.8.0/pyclam/anomaly_detection/meta_ml.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import abc
-import logging
 
 import numpy
 from sklearn import linear_model
 from sklearn import tree
 
-from ..core import Manifold
 from ..utils import constants
+from ..utils import helpers
 
-logger = logging.getLogger(__name__)
-logger.setLevel(constants.LOG_LEVEL)
+logger = helpers.make_logger(__name__)
 
 
 class MetaMLModel(abc.ABC):
 
     def __init__(self, model_class, **kwargs):
         """ Creates a model and initializes it with the given key-word arguments.
         """
@@ -21,28 +19,33 @@
 
     @property
     @abc.abstractmethod
     def name(self) -> str:
         pass
 
     @abc.abstractmethod
-    def fit(self, *args, **kwargs):
+    def fit(self, *args, **kwargs) -> 'MetaMLModel':
         """ Fits the model.
         """
         pass
 
     @abc.abstractmethod
+    def predict(self, ratios: numpy.ndarray) -> float:
+        """ Predicts using the underlying model.
+        """
+        pass
+
+    @abc.abstractmethod
     def extract_python(self, *args, **kwargs) -> tuple[list[str], str]:
         """ Extracts the scoring function as a string which can be written to disk.
 
         The scoring function should have the following signature:
 
         ```
-        def helpful_function_name(ratios: numpy.ndarray) -> float:
-            ...
+        helpful_function_name(ratios: numpy.ndarray) -> float
         ```
 
         where `ratios` is a 1d array of floats with 6 elements. These ratios are
         `cluster_ratios` from Manifold.
 
         Returns:
             A 2-tuple whose items are:
@@ -50,40 +53,43 @@
             - a string containing the code for the scoring function in Python.
         """
         pass
 
 
 class MetaDT(MetaMLModel):
 
-    def __init__(self, max_depth: int = 3):
-        super().__init__(tree.DecisionTreeRegressor, max_depth=max_depth)
+    def __init__(self):
+        super().__init__(tree.DecisionTreeRegressor, max_depth=3)
 
     @property
     def name(self) -> str:
         return 'dt'
 
-    def fit(self, data: numpy.ndarray, scores: numpy.ndarray):
+    def fit(self, data: numpy.ndarray, scores: numpy.ndarray) -> 'MetaDT':
         logger.info(f'Fitting meta-model {self.name} on data with shape {data.shape} ...')
-        self.model.fit(data, scores)
-        return
+        self.model = self.model.fit(data, scores)
+        return self
+
+    def predict(self, ratios: numpy.ndarray) -> float:
+        return self.model.predict(ratios)
 
     def extract_python(self, metric: str, method: str) -> tuple[list[str], str]:
         # noinspection PyProtectedMember
         undefined_feature = tree._tree.TREE_UNDEFINED
 
         feature_names = [
-            Manifold.RATIO_NAMES[i] if i != undefined_feature else "undefined!"
+            constants.RATIO_NAMES[i] if i != undefined_feature else "undefined!"
             for i in self.model.tree_.feature
         ]
 
         # start function definition
         function_name = f'{self.name}_{metric}_{method}'
         code_lines: list[str] = [
             f'def {function_name}(ratios: numpy.ndarray) -> float:',
-            f'    {", ".join(Manifold.RATIO_NAMES)} = tuple(ratios)',
+            f'    {", ".join(constants.RATIO_NAMES)} = tuple(ratios)',
         ]
 
         def extract_lines(node_index: int, indent: str):
             if self.model.tree_.feature[node_index] != undefined_feature:  # internal node
 
                 feature: str = feature_names[node_index]
                 threshold: float = self.model.tree_.threshold[node_index]
@@ -110,24 +116,27 @@
 
         return imports, code
 
 
 class MetaLR(MetaMLModel):
 
     def __init__(self):
-        super().__init__(linear_model.LinearRegression)
+        super().__init__(linear_model.LinearRegression, fit_intercept=False)
 
     @property
     def name(self) -> str:
         return 'lr'
 
-    def fit(self, data: numpy.ndarray, scores: numpy.ndarray):
+    def fit(self, data: numpy.ndarray, scores: numpy.ndarray) -> 'MetaLR':
         logger.info(f'Fitting meta-model {self.name} on data with shape {data.shape} ...')
-        self.model.fit(data, scores)
-        return
+        self.model = self.model.fit(data, scores)
+        return self
+
+    def predict(self, ratios: numpy.ndarray) -> float:
+        return self.model.predict(ratios)
 
     def extract_python(self, metric: str, method: str) -> tuple[list[str], str]:
         imports = ['import numpy']
 
         function_name = f'{self.name}_{metric}_{method}'
         coefficients = [f'{float(c):.6e}' for c in self.model.coef_]
         code = '\n'.join([
@@ -135,7 +144,14 @@
             f'    return float(numpy.dot(numpy.asarray(',
             f'        a=[{", ".join(coefficients)}],',
             f'        dtype=float,',
             f'    ), ratios))'
         ])
 
         return imports, code
+
+
+__all__ = [
+    'MetaMLModel',
+    'MetaDT',
+    'MetaLR',
+]
```

### Comparing `pyclam-0.7.0/pyclam/anomaly_detection/pretrained_models.py` & `pyclam-0.8.0/pyclam/anomaly_detection/pretrained_models.py`

 * *Files identical despite different names*

### Comparing `pyclam-0.7.0/pyclam/classification/classifier.py` & `pyclam-0.8.0/pyclam/classification/classifier.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,99 @@
-import logging
+import operator
 import typing
 
 import numpy
 
+from .. import core
 from ..anomaly_detection import CHAODA
-from ..utils import constants
+from ..utils import helpers
 
-logger = logging.getLogger(__name__)
-logger.setLevel(constants.LOG_LEVEL)
+logger = helpers.make_logger(__name__)
 
 
 class Classifier:
 
-    def __init__(self, **kwargs):
+    def __init__(
+            self,
+            labels: numpy.ndarray,
+            metric_spaces: list[core.Space],
+            **kwargs,
+    ):
         """ Creates and initializes a CLAM Classifier.
 
-        See CHAODA for the list of input arguments.
+        Args:
+            metric_spaces: See `CHAODA`.
+            labels: 1d array of labels. dtype must be numpy.uint.
+            kwargs: These are the same as the kwargs for `CHAODA`.
         """
-        self.kwargs = kwargs
-
-        self._bowls: typing.Dict[int, CHAODA] = dict()
+        if not labels.dtype == numpy.uint:
+            raise ValueError(f'labels must have dtype {numpy.uint}. Got {labels.dtype} instead.')
 
-    def fit(self, data: numpy.ndarray, labels: typing.List[int]) -> 'Classifier':
-        """ Fits the Classifier to the data.
-
-        Args:
-            data: 2d array where the rows are instances and the columns are features.
-            labels: List of enumerated labels for each row of data.
+        self.__metric_spaces = metric_spaces
+        self.__labels = list(map(int, labels))
+        self.__unique_labels = list(set(self.__labels))
+        self.__kwargs = kwargs
+        self.__bowls: typing.Dict[int, CHAODA] = dict()
+
+    @property
+    def labels(self) -> list[int]:
+        return self.__labels
+
+    @property
+    def unique_labels(self) -> list[int]:
+        return self.__unique_labels
 
-        Returns:
-            the fitted Classifier.
+    def build(self) -> 'Classifier':
+        """ Fits the Classifier to the data and returns the fitted object.
         """
-        labels = numpy.array(labels)
-        unique_labels = numpy.unique(labels)
-        for label in unique_labels:
-            indices = list(numpy.argwhere(labels == label))
-
+        for label in self.__unique_labels:
             logger.info(f'Fitting CHAODA object for label {label} ...')
-            bowl = CHAODA(**self.kwargs)
-            bowl = bowl.fit(data, indices=indices)
-            self._bowls[label] = bowl
+
+            indices = [i for i, l in enumerate(self.__labels) if l == label]
+            metric_spaces = [s.subset(indices, f'{s.data.name}__{label}') for s in self.__metric_spaces]
+
+            self.__bowls[label] = CHAODA(metric_spaces, **self.__kwargs).build()
 
         return self
 
-    def predict_single(self, query: numpy.ndarray) -> int:
+    def rank_single(self, query) -> list[tuple[int, float]]:
+        """ Predicts the class rankings for a single query. Lower scores are
+        better.
+        """
+        label_scores = list()
+        for label, bowl in self.__bowls.items():
+            score = bowl.predict_single(query)
+            label_scores.append((label, score))
+
+        return label_scores
+
+    def rank(self, queries: core.Dataset) -> list[list[tuple[int, float]]]:
+        """ Predicts the class rankings for a set of queries. Lower scores are
+        better.
+        """
+        label_scores = list()
+        for i in range(queries.cardinality):
+            logger.info(f'Predicting class for query {i} ...')
+            label_scores.append(self.rank_single(queries[i]))
+        return label_scores
+
+    def predict_single(self, query) -> tuple[int, float]:
         """ Predicts the label for a single query.
         """
-        labels = list(self._bowls.keys())
-        scores = numpy.array(list(bowl.predict_single(query) for bowl in self._bowls.values()), dtype=numpy.float32)
-        min_index = numpy.argmin(scores)
-        return labels[min_index]
+        label_scores = self.rank_single(query)
+        best_label, best_score = min(label_scores, key=operator.itemgetter(1))
+        return best_label, best_score
 
-    def predict(self, queries: numpy.ndarray) -> typing.List[int]:
+    def predict(self, queries: core.Dataset) -> tuple[list[int], list[float]]:
         """ Predicts the label for a set of queries.
         """
-        labels = list()
-        for i in range(queries.shape[0]):
-            logger.info(f'Predicting class for query {i} ...')
-            labels.append(self.predict_single(queries[i]))
-        return labels
+        label_scores = list()
+        for i in range(queries.cardinality):
+            logger.info(f'Predicting class for query {i + 1}/{queries.cardinality} ...')
+            label_scores.append(self.predict_single(queries[i]))
+        [labels, scores] = list(zip(*label_scores))
+        return labels, scores
+
+
+__all__ = [
+    'Classifier',
+]
```

### Comparing `pyclam-0.7.0/pyclam/utils/helpers.py` & `pyclam-0.8.0/pyclam/utils/helpers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,58 @@
+import logging
+import typing
+
 import numpy
 from scipy.special import erf
 
 from . import constants
 
+NormalizationMode = typing.Literal[
+    'linear',
+    'gaussian',
+    'sigmoid',
+]
+
+
+def make_logger(name: str):
+    logger = logging.getLogger(name)
+    logger.setLevel(constants.LOG_LEVEL)
+    return logger
 
-def catch_normalization_mode(mode: str) -> None:
-    """ Make sure that the normalization mode is allowed. """
-    modes: list[str] = ['linear', 'gaussian', 'sigmoid']
-    if mode not in modes:
-        raise ValueError(f'Normalization method {mode} is undefined. Must by one of {modes}.')
-    else:
-        return
 
+def next_ema(ratio: float, ema: float) -> float:
+    return constants.EMA_ALPHA * ratio + (1 - constants.EMA_ALPHA) * ema
 
-def normalize(values, mode: str):
+
+def normalize(values: numpy.ndarray, mode: NormalizationMode):
     """ Normalizes each column in values into a [0, 1] range.
 
-    :param values: A 1-d or 2-d array of values to normalize.
-    :param mode: Normalization mode to use. Must be one of 'linear', 'gaussian', or 'sigmoid'.
-    :return: array of normalized values.
+    Args:
+        values: A 1-d or 2-d array of values to normalize.
+        mode: Normalization mode to use. Must be one of:
+         - 'linear',
+         - 'gaussian', or
+         - 'sigmoid'.
+
+    Returns:
+        array of normalized values.
     """
     squeeze = False
     if len(values.shape) == 1:
         squeeze = True
         values = numpy.expand_dims(values, axis=1)
 
     if mode == 'linear':
         min_v, max_v = numpy.min(values, axis=0), numpy.max(values, axis=0)
-        for i in range(values.shape[1]):
-            if min_v[i] == max_v[i]:
-                max_v[i] += 1
-                values[:, i] = min_v[i] + 0.5
-        values = (values - min_v) / (max_v - min_v)
+        values = (values - min_v) / (max_v - min_v + constants.EPSILON)
     else:
-        mu = numpy.mean(values, axis=0)
-        sigma = numpy.std(values, axis=0)
-
-        for i in range(values.shape[1]):
-            if sigma[i] < constants.EPSILON:
-                values[:, i] = 0.5
-            else:
-                if mode == 'gaussian':
-                    values[:, i] = (1 + erf((values[:, i] - mu[i]) / (sigma[i] * numpy.sqrt(2)))) / 2
-                else:
-                    values[:, i] = 1 / (1 + numpy.exp(-(values[:, i] - mu[i]) / sigma[i]))
+        means = numpy.mean(values, axis=0)
+        sds = numpy.std(values, axis=0) + constants.EPSILON
+        if mode == 'gaussian':
+            values = (1 + erf((values - means) / (sds * numpy.sqrt(2)))) / 2
+        else:
+            values = 1 / (1 + numpy.exp(-(values - means) / sds))
 
     values = values.clip(constants.EPSILON, 1)
     if squeeze:
         values = numpy.squeeze(values)
     return values
```

### Comparing `pyclam-0.7.0/pyclam.egg-info/PKG-INFO` & `pyclam-0.8.0/pyclam.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyclam
-Version: 0.7.0
+Version: 0.8.0
 Summary: Clustered Learning of Approximate Manifolds
 Home-page: https://github.com/URI-ABD/clam
-Author: Najib Ishaq <nishaq@zoho.com>; Tom Howard <info@tomhoward.codes>; Noah Daniels <noah_daniels@uri.edu>
+Author: Najib Ishaq <najib_ishaq@zoho.com>; Tom Howard <info@tomhoward.codes>; Noah Daniels <noah_daniels@uri.edu>; Morgan Prior <morgan_prior@uri.edu>; Isaac Chen <ijchen@uri.edu>; Oliver McLaughlin <olwmcjp@gmail.com>
 Author-email: 
 License: MIT
 Requires-Python: >=3.9,<3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # URI-ABD: Clustered Learning of Approximate Manifolds
@@ -36,15 +36,15 @@
 
 ### Python Scripting
 
 ```python
 from pyclam import criterion
 from pyclam import Manifold
 from pyclam.search import CAKES
-from pyclam.utils import synthetic_datasets
+from tests import synthetic_datasets
 
 # Get the data.
 data, _ = synthetic_datasets.bullseye()
 # data is a numpy.ndarray in this case but it could just as easily be a numpy.memmap if your data does fit in RAM.
 # We used numpy memmaps for the research, though they impose file-IO costs.
 
 search = CAKES(data, 'euclidean')
@@ -52,18 +52,18 @@
 # TODO: Provide link to CHESS paper
 
 search.build(max_depth=10)
 # Build the search tree to depth of 10.
 # This method can be called again with a higher depth, if needed.
 
 query, radius = data[0], 0.5
-rnn_results = search.rnn(query, radius)
+rnn_results = search.rnn_search(query, radius)
 # This is how we perform rho-nearest neighbors search with radius 0.5 around the query.
 
-knn_results = search.knn(query, 10)
+knn_results = search.knn_search(query, 10)
 # This is how to perform k-nearest neighbors search for the 10 nearest neighbors of query.
 
 # TODO: Provide snippets for using CHAODA
 
 # You can also directly use the Manifold functionality provided by CLAM.
 
 manifold = Manifold(data, 'euclidean')
```

### Comparing `pyclam-0.7.0/pyclam.egg-info/SOURCES.txt` & `pyclam-0.8.0/pyclam.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,25 +4,29 @@
 pyclam/__init__.py
 pyclam.egg-info/PKG-INFO
 pyclam.egg-info/SOURCES.txt
 pyclam.egg-info/dependency_links.txt
 pyclam.egg-info/requires.txt
 pyclam.egg-info/top_level.txt
 pyclam/anomaly_detection/__init__.py
+pyclam/anomaly_detection/anomaly_dataset.py
+pyclam/anomaly_detection/anomaly_space.py
 pyclam/anomaly_detection/chaoda.py
-pyclam/anomaly_detection/datasets.py
-pyclam/anomaly_detection/graph_selectors.py
-pyclam/anomaly_detection/individual_algorithms.py
-pyclam/anomaly_detection/meta_ml_models.py
+pyclam/anomaly_detection/graph_scorers.py
+pyclam/anomaly_detection/meta_ml.py
 pyclam/anomaly_detection/pretrained_models.py
+pyclam/anomaly_detection/training.py
 pyclam/classification/__init__.py
 pyclam/classification/classifier.py
 pyclam/core/__init__.py
-pyclam/core/criterion.py
-pyclam/core/manifold.py
-pyclam/core/types.py
+pyclam/core/cluster.py
+pyclam/core/cluster_criteria.py
+pyclam/core/dataset.py
+pyclam/core/graph.py
+pyclam/core/graph_criteria.py
+pyclam/core/metric.py
+pyclam/core/space.py
 pyclam/search/__init__.py
 pyclam/search/cakes.py
 pyclam/utils/__init__.py
 pyclam/utils/constants.py
-pyclam/utils/helpers.py
-pyclam/utils/synthetic_datasets.py
+pyclam/utils/helpers.py
```

### Comparing `pyclam-0.7.0/setup.py` & `pyclam-0.8.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,10 +14,10 @@
     url='https://github.com/URI-ABD/clam',
     license='MIT',
     author='; '.join(cargo['package']['authors']),
     author_email='',
     description='Clustered Learning of Approximate Manifolds',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    install_requires=['numpy>=1.22,<1.23', 'scipy>=1.8,<1.9', 'toml>=0.10,<0.11', 'scikit-learn>=1.1,<1.2', 'h5py>=3.7,<3.8'],
+    install_requires=['numpy>=1.22,<1.23', 'scipy>=1.8,<1.9', 'toml>=0.10,<0.11', 'scikit-learn>=1.1,<1.2'],
     python_requires='>=3.9,<3.11',
 )
```

