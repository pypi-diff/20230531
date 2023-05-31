# Comparing `tmp/modAL-0.4.0.tar.gz` & `tmp/modAL-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/modAL-0.4.0.tar", last modified: Sun Nov  1 08:44:24 2020, max compression
+gzip compressed data, was "dist/modAL-0.4.1.tar", last modified: Thu Jan  7 09:45:00 2021, max compression
```

## Comparing `modAL-0.4.0.tar` & `modAL-0.4.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 tivadar   (1000) tivadar   (1000)        0 2020-11-01 08:44:24.000000 modAL-0.4.0/
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)      299 2020-11-01 08:44:24.000000 modAL-0.4.0/PKG-INFO
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)    10828 2020-11-01 08:39:18.000000 modAL-0.4.0/README.md
-drwxr-xr-x   0 tivadar   (1000) tivadar   (1000)        0 2020-11-01 08:44:24.000000 modAL-0.4.0/modAL/
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)      128 2019-09-22 08:04:19.000000 modAL-0.4.0/modAL/__init__.py
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)     5560 2020-11-01 08:39:18.000000 modAL-0.4.0/modAL/acquisition.py
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)    10985 2020-11-01 08:39:18.000000 modAL-0.4.0/modAL/batch.py
--rwxr-xr-x   0 tivadar   (1000) tivadar   (1000)      416 2019-09-22 08:04:19.000000 modAL-0.4.0/modAL/cluster.py
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)     1762 2019-09-22 08:04:19.000000 modAL-0.4.0/modAL/density.py
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)     8883 2020-11-01 08:39:18.000000 modAL-0.4.0/modAL/disagreement.py
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)     3071 2020-11-01 08:39:18.000000 modAL-0.4.0/modAL/expected_error.py
-drwxr-xr-x   0 tivadar   (1000) tivadar   (1000)        0 2020-11-01 08:44:24.000000 modAL-0.4.0/modAL/models/
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)      180 2019-09-22 08:04:19.000000 modAL-0.4.0/modAL/models/__init__.py
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)    19706 2020-11-01 08:39:18.000000 modAL-0.4.0/modAL/models/base.py
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)    23061 2020-11-01 08:39:18.000000 modAL-0.4.0/modAL/models/learners.py
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)    10447 2020-11-01 08:39:18.000000 modAL-0.4.0/modAL/multilabel.py
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)     7850 2020-11-01 08:39:18.000000 modAL-0.4.0/modAL/uncertainty.py
-drwxr-xr-x   0 tivadar   (1000) tivadar   (1000)        0 2020-11-01 08:44:24.000000 modAL-0.4.0/modAL/utils/
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)      417 2019-09-22 08:04:19.000000 modAL-0.4.0/modAL/utils/__init__.py
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)     3607 2020-11-01 08:39:18.000000 modAL-0.4.0/modAL/utils/combination.py
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)     4725 2020-11-01 08:39:18.000000 modAL-0.4.0/modAL/utils/data.py
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)     2389 2019-09-22 08:04:19.000000 modAL-0.4.0/modAL/utils/selection.py
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)     1920 2019-09-22 08:04:19.000000 modAL-0.4.0/modAL/utils/validation.py
-drwxr-xr-x   0 tivadar   (1000) tivadar   (1000)        0 2020-11-01 08:44:24.000000 modAL-0.4.0/modAL.egg-info/
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)      299 2020-11-01 08:44:23.000000 modAL-0.4.0/modAL.egg-info/PKG-INFO
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)      540 2020-11-01 08:44:23.000000 modAL-0.4.0/modAL.egg-info/SOURCES.txt
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)        1 2020-11-01 08:44:23.000000 modAL-0.4.0/modAL.egg-info/dependency_links.txt
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)       57 2020-11-01 08:44:23.000000 modAL-0.4.0/modAL.egg-info/requires.txt
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)        6 2020-11-01 08:44:23.000000 modAL-0.4.0/modAL.egg-info/top_level.txt
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)       79 2020-11-01 08:44:24.000000 modAL-0.4.0/setup.cfg
--rw-r--r--   0 tivadar   (1000) tivadar   (1000)      488 2020-11-01 08:39:18.000000 modAL-0.4.0/setup.py
+drwxr-xr-x   0 tivadar   (1000) tivadar   (1000)        0 2021-01-07 09:45:00.000000 modAL-0.4.1/
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)      299 2021-01-07 09:45:00.000000 modAL-0.4.1/PKG-INFO
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)    10828 2020-11-01 08:39:18.000000 modAL-0.4.1/README.md
+drwxr-xr-x   0 tivadar   (1000) tivadar   (1000)        0 2021-01-07 09:45:00.000000 modAL-0.4.1/modAL/
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)      128 2019-09-22 08:04:19.000000 modAL-0.4.1/modAL/__init__.py
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)     5560 2020-11-01 08:39:18.000000 modAL-0.4.1/modAL/acquisition.py
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)    11062 2021-01-07 09:40:55.000000 modAL-0.4.1/modAL/batch.py
+-rwxr-xr-x   0 tivadar   (1000) tivadar   (1000)      416 2019-09-22 08:04:19.000000 modAL-0.4.1/modAL/cluster.py
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)     1762 2019-09-22 08:04:19.000000 modAL-0.4.1/modAL/density.py
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)     8825 2021-01-07 09:40:55.000000 modAL-0.4.1/modAL/disagreement.py
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)     3071 2020-11-01 08:39:18.000000 modAL-0.4.1/modAL/expected_error.py
+drwxr-xr-x   0 tivadar   (1000) tivadar   (1000)        0 2021-01-07 09:45:00.000000 modAL-0.4.1/modAL/models/
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)      180 2019-09-22 08:04:19.000000 modAL-0.4.1/modAL/models/__init__.py
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)    19137 2021-01-07 09:40:55.000000 modAL-0.4.1/modAL/models/base.py
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)    23061 2020-11-01 08:39:18.000000 modAL-0.4.1/modAL/models/learners.py
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)    10447 2020-11-01 08:39:18.000000 modAL-0.4.1/modAL/multilabel.py
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)     7850 2020-11-01 08:39:18.000000 modAL-0.4.1/modAL/uncertainty.py
+drwxr-xr-x   0 tivadar   (1000) tivadar   (1000)        0 2021-01-07 09:45:00.000000 modAL-0.4.1/modAL/utils/
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)      417 2019-09-22 08:04:19.000000 modAL-0.4.1/modAL/utils/__init__.py
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)     3607 2020-11-01 08:39:18.000000 modAL-0.4.1/modAL/utils/combination.py
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)     4725 2020-11-01 08:39:18.000000 modAL-0.4.1/modAL/utils/data.py
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)     2389 2019-09-22 08:04:19.000000 modAL-0.4.1/modAL/utils/selection.py
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)     1920 2019-09-22 08:04:19.000000 modAL-0.4.1/modAL/utils/validation.py
+drwxr-xr-x   0 tivadar   (1000) tivadar   (1000)        0 2021-01-07 09:45:00.000000 modAL-0.4.1/modAL.egg-info/
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)      299 2021-01-07 09:45:00.000000 modAL-0.4.1/modAL.egg-info/PKG-INFO
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)      540 2021-01-07 09:45:00.000000 modAL-0.4.1/modAL.egg-info/SOURCES.txt
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)        1 2021-01-07 09:45:00.000000 modAL-0.4.1/modAL.egg-info/dependency_links.txt
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)       57 2021-01-07 09:45:00.000000 modAL-0.4.1/modAL.egg-info/requires.txt
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)        6 2021-01-07 09:45:00.000000 modAL-0.4.1/modAL.egg-info/top_level.txt
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)       79 2021-01-07 09:45:00.000000 modAL-0.4.1/setup.cfg
+-rw-r--r--   0 tivadar   (1000) tivadar   (1000)      488 2021-01-07 09:40:55.000000 modAL-0.4.1/setup.py
```

### Comparing `modAL-0.4.0/README.md` & `modAL-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `modAL-0.4.0/modAL/acquisition.py` & `modAL-0.4.1/modAL/acquisition.py`

 * *Files identical despite different names*

### Comparing `modAL-0.4.0/modAL/batch.py` & `modAL-0.4.1/modAL/batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from typing import Callable, Optional, Tuple, Union
 
 import numpy as np
 import scipy.sparse as sp
 from sklearn.metrics.pairwise import pairwise_distances, pairwise_distances_argmin_min
 
-from modAL.utils.data import data_vstack, modALinput
+from modAL.utils.data import data_vstack, modALinput, data_shape
 from modAL.models.base import BaseCommittee, BaseLearner
 from modAL.uncertainty import classifier_uncertainty
 
 
 def select_cold_start_instance(X: modALinput,
                                metric: Union[str, Callable],
                                n_jobs: Union[int, None]) -> Tuple[int, modALinput]:
@@ -146,16 +146,18 @@
     # transform unlabeled data if needed
     if classifier.on_transformed:
         unlabeled = classifier.transform_without_estimating(unlabeled)
 
     if classifier.X_training is None:
         best_coldstart_instance_index, labeled = select_cold_start_instance(X=unlabeled, metric=metric, n_jobs=n_jobs)
         instance_index_ranking = [best_coldstart_instance_index]
-    elif classifier.X_training.shape[0] > 0:
-        labeled = classifier.Xt_training[:] if classifier.on_transformed else classifier.X_training[:]
+    elif data_shape(classifier.X_training)[0] > 0:
+        labeled = classifier.transform_without_estimating(
+            classifier.X_training
+        ) if classifier.on_transformed else classifier.X_training[:]
         instance_index_ranking = []
     
     # The maximum number of records to sample.
     ceiling = np.minimum(unlabeled.shape[0], n_instances) - len(instance_index_ranking)
 
     # mask for unlabeled initialized as transparent
     mask = np.ones(unlabeled.shape[0], np.bool)
```

### Comparing `modAL-0.4.0/modAL/density.py` & `modAL-0.4.1/modAL/density.py`

 * *Files identical despite different names*

### Comparing `modAL-0.4.0/modAL/disagreement.py` & `modAL-0.4.1/modAL/disagreement.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,24 +31,22 @@
     n_learners = len(committee)
     try:
         votes = committee.vote(X, **predict_proba_kwargs)
     except NotFittedError:
         return np.zeros(shape=(X.shape[0],))
 
     p_vote = np.zeros(shape=(X.shape[0], len(committee.classes_)))
-    entr = np.zeros(shape=(X.shape[0],))
 
     for vote_idx, vote in enumerate(votes):
         vote_counter = Counter(vote)
 
         for class_idx, class_label in enumerate(committee.classes_):
             p_vote[vote_idx, class_idx] = vote_counter[class_label]/n_learners
 
-        entr[vote_idx] = entropy(p_vote[vote_idx])
-
+    entr = entropy(p_vote, axis=1)
     return entr
 
 
 def consensus_entropy(committee: BaseCommittee, X: modALinput, **predict_proba_kwargs) -> np.ndarray:
     """
     Calculates the consensus entropy for the Committee. First it computes the class probabilties of X for each learner
     in the Committee, then calculates the consensus probability distribution by averaging the individual class
```

### Comparing `modAL-0.4.0/modAL/expected_error.py` & `modAL-0.4.1/modAL/expected_error.py`

 * *Files identical despite different names*

### Comparing `modAL-0.4.0/modAL/models/base.py` & `modAL-0.4.1/modAL/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,19 +62,17 @@
         assert callable(query_strategy), 'query_strategy must be callable'
 
         self.estimator = estimator
         self.query_strategy = query_strategy
         self.on_transformed = on_transformed
 
         self.X_training = X_training
-        self.Xt_training = None
         self.y_training = y_training
         if X_training is not None:
             self._fit_to_known(bootstrap=bootstrap_init, **fit_kwargs)
-            self.Xt_training = self.transform_without_estimating(self.X_training) if self.on_transformed else None
 
         assert isinstance(force_all_finite, bool), 'force_all_finite must be a bool'
         self.force_all_finite = force_all_finite
 
     def _add_training_data(self, X: modALinput, y: modALinput) -> None:
         """
         Adds the new data and label to the known data, but does not retrain the model.
@@ -88,23 +86,18 @@
             classifier has seen.
         """
         check_X_y(X, y, accept_sparse=True, ensure_2d=False, allow_nd=True, multi_output=True, dtype=None,
                   force_all_finite=self.force_all_finite)
 
         if self.X_training is None:
             self.X_training = X
-            self.Xt_training = self.transform_without_estimating(self.X_training) if self.on_transformed else None
             self.y_training = y
         else:
             try:
                 self.X_training = data_vstack((self.X_training, X))
-                self.Xt_training = data_vstack((
-                    self.Xt_training,
-                    self.transform_without_estimating(X)
-                )) if self.on_transformed else None
                 self.y_training = data_vstack((self.y_training, y))
             except ValueError:
                 raise ValueError('the dimensions of the new training data and label must'
                                  'agree with the training data and labels provided so far')
 
     def transform_without_estimating(self, X: modALinput) -> Union[np.ndarray, sp.csr_matrix]:
         """
@@ -209,15 +202,14 @@
 
         Returns:
             self
         """
         check_X_y(X, y, accept_sparse=True, ensure_2d=False, allow_nd=True, multi_output=True, dtype=None,
                   force_all_finite=self.force_all_finite)
         self.X_training, self.y_training = X, y
-        self.Xt_training = self.transform_without_estimating(self.X_training) if self.on_transformed else None
         return self._fit_to_known(bootstrap=bootstrap, **fit_kwargs)
 
     def predict(self, X: modALinput, **predict_kwargs) -> Any:
         """
         Estimator predictions for X. Interface with the predict method of the estimator.
 
         Args:
```

### Comparing `modAL-0.4.0/modAL/models/learners.py` & `modAL-0.4.1/modAL/models/learners.py`

 * *Files identical despite different names*

### Comparing `modAL-0.4.0/modAL/multilabel.py` & `modAL-0.4.1/modAL/multilabel.py`

 * *Files identical despite different names*

### Comparing `modAL-0.4.0/modAL/uncertainty.py` & `modAL-0.4.1/modAL/uncertainty.py`

 * *Files identical despite different names*

### Comparing `modAL-0.4.0/modAL/utils/combination.py` & `modAL-0.4.1/modAL/utils/combination.py`

 * *Files identical despite different names*

### Comparing `modAL-0.4.0/modAL/utils/data.py` & `modAL-0.4.1/modAL/utils/data.py`

 * *Files identical despite different names*

### Comparing `modAL-0.4.0/modAL/utils/selection.py` & `modAL-0.4.1/modAL/utils/selection.py`

 * *Files identical despite different names*

### Comparing `modAL-0.4.0/modAL/utils/validation.py` & `modAL-0.4.1/modAL/utils/validation.py`

 * *Files identical despite different names*

### Comparing `modAL-0.4.0/modAL.egg-info/SOURCES.txt` & `modAL-0.4.1/modAL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

