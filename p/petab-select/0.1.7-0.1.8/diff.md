# Comparing `tmp/petab_select-0.1.7.tar.gz` & `tmp/petab_select-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petab_select-0.1.7.tar", last modified: Tue May  9 18:46:03 2023, max compression
+gzip compressed data, was "petab_select-0.1.8.tar", last modified: Wed May 31 15:56:37 2023, max compression
```

## Comparing `petab_select-0.1.7.tar` & `petab_select-0.1.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-05-09 18:46:03.076553 petab_select-0.1.7/
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     1602 2021-08-31 13:20:42.000000 petab_select-0.1.7/LICENSE
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     9746 2023-05-09 18:46:03.076553 petab_select-0.1.7/PKG-INFO
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     9256 2023-04-13 16:12:57.000000 petab_select-0.1.7/README.md
-drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-05-09 18:46:03.076553 petab_select-0.1.7/petab_select/
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      263 2023-04-13 08:28:52.000000 petab_select-0.1.7/petab_select/__init__.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    51673 2023-05-09 18:43:32.000000 petab_select-0.1.7/petab_select/candidate_space.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    13247 2022-09-30 16:40:04.000000 petab_select-0.1.7/petab_select/cli.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     4460 2022-09-30 16:40:04.000000 petab_select-0.1.7/petab_select/constants.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     7225 2022-09-30 16:40:04.000000 petab_select-0.1.7/petab_select/criteria.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     2443 2021-11-02 20:14:39.000000 petab_select-0.1.7/petab_select/descriptors.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     1076 2022-09-30 16:40:04.000000 petab_select-0.1.7/petab_select/handlers.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     2438 2022-09-30 16:40:04.000000 petab_select-0.1.7/petab_select/misc.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    25976 2023-05-09 10:52:56.000000 petab_select-0.1.7/petab_select/model.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    11415 2022-09-30 16:40:04.000000 petab_select-0.1.7/petab_select/model_space.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    38364 2022-09-30 16:40:04.000000 petab_select-0.1.7/petab_select/model_subspace.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     2254 2022-09-30 16:40:04.000000 petab_select-0.1.7/petab_select/petab.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     8571 2023-04-13 08:28:52.000000 petab_select-0.1.7/petab_select/problem.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    10246 2023-05-09 18:43:32.000000 petab_select-0.1.7/petab_select/ui.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      295 2021-11-03 18:08:02.000000 petab_select-0.1.7/petab_select/validators.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)       80 2023-05-09 18:45:22.000000 petab_select-0.1.7/petab_select/version.py
-drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-05-09 18:46:03.076553 petab_select-0.1.7/petab_select.egg-info/
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     9746 2023-05-09 18:46:03.000000 petab_select-0.1.7/petab_select.egg-info/PKG-INFO
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      658 2023-05-09 18:46:03.000000 petab_select-0.1.7/petab_select.egg-info/SOURCES.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)        1 2023-05-09 18:46:03.000000 petab_select-0.1.7/petab_select.egg-info/dependency_links.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)       54 2023-05-09 18:46:03.000000 petab_select-0.1.7/petab_select.egg-info/entry_points.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      136 2023-05-09 18:46:03.000000 petab_select-0.1.7/petab_select.egg-info/requires.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)       13 2023-05-09 18:46:03.000000 petab_select-0.1.7/petab_select.egg-info/top_level.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      281 2022-09-30 16:40:04.000000 petab_select-0.1.7/pyproject.toml
--rw-rw-r--   0 dilan     (1001) dilan     (1001)       38 2023-05-09 18:46:03.076553 petab_select-0.1.7/setup.cfg
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     2961 2023-04-13 16:12:57.000000 petab_select-0.1.7/setup.py
+drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-05-31 15:56:37.946644 petab_select-0.1.8/
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     1602 2021-08-31 13:20:42.000000 petab_select-0.1.8/LICENSE
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     9746 2023-05-31 15:56:37.946644 petab_select-0.1.8/PKG-INFO
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     9256 2023-04-13 16:12:57.000000 petab_select-0.1.8/README.md
+drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-05-31 15:56:37.946644 petab_select-0.1.8/petab_select/
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      263 2023-04-13 08:28:52.000000 petab_select-0.1.8/petab_select/__init__.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    52003 2023-05-31 15:52:41.000000 petab_select-0.1.8/petab_select/candidate_space.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    13247 2022-09-30 16:40:04.000000 petab_select-0.1.8/petab_select/cli.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     4460 2022-09-30 16:40:04.000000 petab_select-0.1.8/petab_select/constants.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     7225 2022-09-30 16:40:04.000000 petab_select-0.1.8/petab_select/criteria.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     2443 2021-11-02 20:14:39.000000 petab_select-0.1.8/petab_select/descriptors.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     1076 2022-09-30 16:40:04.000000 petab_select-0.1.8/petab_select/handlers.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     2438 2022-09-30 16:40:04.000000 petab_select-0.1.8/petab_select/misc.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    25976 2023-05-09 10:52:56.000000 petab_select-0.1.8/petab_select/model.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    11415 2022-09-30 16:40:04.000000 petab_select-0.1.8/petab_select/model_space.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    38364 2022-09-30 16:40:04.000000 petab_select-0.1.8/petab_select/model_subspace.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     2254 2022-09-30 16:40:04.000000 petab_select-0.1.8/petab_select/petab.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     8571 2023-04-13 08:28:52.000000 petab_select-0.1.8/petab_select/problem.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    10226 2023-05-31 15:52:41.000000 petab_select-0.1.8/petab_select/ui.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      295 2021-11-03 18:08:02.000000 petab_select-0.1.8/petab_select/validators.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)       80 2023-05-31 15:52:51.000000 petab_select-0.1.8/petab_select/version.py
+drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-05-31 15:56:37.946644 petab_select-0.1.8/petab_select.egg-info/
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     9746 2023-05-31 15:56:37.000000 petab_select-0.1.8/petab_select.egg-info/PKG-INFO
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      658 2023-05-31 15:56:37.000000 petab_select-0.1.8/petab_select.egg-info/SOURCES.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)        1 2023-05-31 15:56:37.000000 petab_select-0.1.8/petab_select.egg-info/dependency_links.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)       54 2023-05-31 15:56:37.000000 petab_select-0.1.8/petab_select.egg-info/entry_points.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      136 2023-05-31 15:56:37.000000 petab_select-0.1.8/petab_select.egg-info/requires.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)       13 2023-05-31 15:56:37.000000 petab_select-0.1.8/petab_select.egg-info/top_level.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      281 2022-09-30 16:40:04.000000 petab_select-0.1.8/pyproject.toml
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)       38 2023-05-31 15:56:37.946644 petab_select-0.1.8/setup.cfg
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     2961 2023-04-13 16:12:57.000000 petab_select-0.1.8/setup.py
```

### Comparing `petab_select-0.1.7/LICENSE` & `petab_select-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.7/PKG-INFO` & `petab_select-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petab_select
-Version: 0.1.7
+Version: 0.1.8
 Summary: PEtab Select: an extension to PEtab for model selection.
 Home-page: https://github.com/PEtab-dev/petab_select
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `petab_select-0.1.7/README.md` & `petab_select-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.7/petab_select/candidate_space.py` & `petab_select-0.1.8/petab_select/candidate_space.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,16 @@
     Attributes:
         distances:
             The distances of all candidate models from the initial model.
             FIXME change list to int? Is storage of more than one value
             useful?
         predecessor_model:
             The model used for comparison, e.g. for stepwise methods.
+        previous_predecessor_model:
+            The previous predecessor model.
         models:
             The current set of candidate models.
         exclusions:
             A list of model hashes. Models that match a hash in `exclusions` will not
             be accepted into the candidate space. The hashes of models that are accepted
             are added to `exclusions`.
         limit:
@@ -80,14 +82,15 @@
     def __init__(
         self,
         # TODO add MODEL_TYPE = Union[str, Model], str for VIRTUAL_INITIAL_MODEL
         predecessor_model: Optional[Model] = None,
         exclusions: Optional[List[Any]] = None,
         limit: TYPE_LIMIT = np.inf,
         summary_tsv: TYPE_PATH = None,
+        previous_predecessor_model: Optional[Model] = None,
     ):
         self.limit = LimitHandler(
             current=self.n_accepted,
             limit=limit,
         )
         # Each candidate class specifies this as a class attribute.
         if self.governing_method is None:
@@ -95,14 +98,18 @@
         self.reset(predecessor_model=predecessor_model, exclusions=exclusions)
 
         self.summary_tsv = summary_tsv
         if self.summary_tsv is not None:
             self.summary_tsv = Path(self.summary_tsv)
             self._setup_summary_tsv()
 
+        self.previous_predecessor_model = previous_predecessor_model
+        if self.previous_predecessor_model is None:
+            self.previous_predecessor_model = self.predecessor_model
+
     def write_summary_tsv(self, row):
         if self.summary_tsv is None:
             return
 
         # Format single values to be valid rows
         if not isinstance(row, list):
             row = [
@@ -136,15 +143,14 @@
     def read_arguments_from_yaml_dict(cls, yaml_dict):
         kwargs = copy.deepcopy(yaml_dict)
 
         predecessor_model = None
         if (
             predecessor_model_yaml := kwargs.pop(PREDECESSOR_MODEL, None)
         ) is not None:
-
             predecessor_model = Model.from_yaml(predecessor_model_yaml)
 
         return {
             **kwargs,
             PREDECESSOR_MODEL: predecessor_model,
         }
```

### Comparing `petab_select-0.1.7/petab_select/cli.py` & `petab_select-0.1.8/petab_select/cli.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.7/petab_select/constants.py` & `petab_select-0.1.8/petab_select/constants.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.7/petab_select/criteria.py` & `petab_select-0.1.8/petab_select/criteria.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.7/petab_select/descriptors.py` & `petab_select-0.1.8/petab_select/descriptors.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.7/petab_select/handlers.py` & `petab_select-0.1.8/petab_select/handlers.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.7/petab_select/misc.py` & `petab_select-0.1.8/petab_select/misc.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.7/petab_select/model.py` & `petab_select-0.1.8/petab_select/model.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.7/petab_select/model_space.py` & `petab_select-0.1.8/petab_select/model_space.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.7/petab_select/model_subspace.py` & `petab_select-0.1.8/petab_select/model_subspace.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.7/petab_select/petab.py` & `petab_select-0.1.8/petab_select/petab.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.7/petab_select/problem.py` & `petab_select-0.1.8/petab_select/problem.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.7/petab_select/ui.py` & `petab_select-0.1.8/petab_select/ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from .model import Model, default_compare
 from .problem import Problem
 
 
 def candidates(
     problem: Problem,
     candidate_space: Optional[CandidateSpace] = None,
-    previous_predecessor_model: Optional[Model] = None,
     limit: Union[float, int] = np.inf,
     limit_sent: Union[float, int] = np.inf,
     calibrated_models: Optional[Dict[str, Model]] = None,
     newly_calibrated_models: Optional[Dict[str, Model]] = None,
     excluded_models: Optional[List[Model]] = None,
     excluded_model_hashes: Optional[List[str]] = None,
     criterion: Optional[Criterion] = None,
@@ -37,18 +36,14 @@
 
     Args:
         problem:
             A PEtab Select problem.
         candidate_space:
             The candidate space. Defaults to a new candidate space based on the method
             defined in the problem.
-        previous_predecessor_model:
-            The previous predecessor model for a compatible method. This is
-            used as the predecessor model for the current iteration, if a
-            better model doesn't exist in the candidate space models.
         limit:
             The maximum number of models to add to the candidate space.
         limit_sent:
             The maximum number of models sent to the candidate space (which are possibly
             rejected and excluded).
         calibrated_models:
             All calibrated models in the model selection.
@@ -88,30 +83,30 @@
         candidate_space = problem.new_candidate_space(limit=limit)
     candidate_space.exclude_hashes(calibrated_models)
 
     # Set the predecessor model to the previous predecessor model.
     # Set the new predecessor_model from the initial model or
     # by calling ui.best to find the best model to jump to if
     # this is not the first step of the search.
-    predecessor_model = previous_predecessor_model
+    predecessor_model = candidate_space.previous_predecessor_model
     if newly_calibrated_models:
         predecessor_model = problem.get_best(
             newly_calibrated_models.values(),
             criterion=criterion,
         )
         # If the new predecessor model isn't better than the previous one,
         # keep the previous one.
         # If FAMoS jumped this will not be useful, since the jumped-to model
         # can be expected to be worse than the jumped-from model, in general.
         if not default_compare(
-            model0=previous_predecessor_model,
+            model0=candidate_space.previous_predecessor_model,
             model1=predecessor_model,
             criterion=criterion,
         ):
-            predecessor_model = previous_predecessor_model
+            predecessor_model = candidate_space.previous_predecessor_model
 
         try:
             candidate_space.update_after_calibration(
                 calibrated_models=calibrated_models,
                 newly_calibrated_models=newly_calibrated_models,
                 criterion=criterion,
             )
@@ -149,18 +144,20 @@
     )
     if do_search:
         problem.model_space.search(candidate_space, limit=limit_sent)
 
     write_summary_tsv(
         problem=problem,
         candidate_space=candidate_space,
-        previous_predecessor_model=previous_predecessor_model,
+        previous_predecessor_model=candidate_space.previous_predecessor_model,
         predecessor_model=predecessor_model,
     )
 
+    candidate_space.previous_predecessor_model = predecessor_model
+
     return candidate_space
 
 
 def model_to_petab(
     model: Model,
     output_path: Optional[TYPE_PATH] = None,
 ) -> Dict[str, Union[petab.Problem, TYPE_PATH]]:
@@ -262,16 +259,18 @@
 
     diff_candidates_parameter_ids = []
     for candidate_model in candidate_space.models:
         candidate_parameter_ids = set(
             candidate_model.get_estimated_parameter_ids_all()
         )
         diff_candidates_parameter_ids.append(
-            candidate_parameter_ids.symmetric_difference(
-                predecessor_parameter_ids
+            list(
+                candidate_parameter_ids.symmetric_difference(
+                    predecessor_parameter_ids
+                )
             )
         )
 
     # FIXME remove once MostDistantCandidateSpace exists...
     method = candidate_space.method
     if (
         candidate_space.governing_method == Method.FAMOS
@@ -282,13 +281,16 @@
             if sum(1 for _ in f) > 1:
                 method = Method.MOST_DISTANT
 
     candidate_space.write_summary_tsv(
         [
             method,
             len(candidate_space.models),
-            diff_parameter_ids,
+            sorted(diff_parameter_ids),
             predecessor_criterion,
-            predecessor_parameter_ids,
-            diff_candidates_parameter_ids,
+            sorted(predecessor_parameter_ids),
+            sorted(
+                diff_candidates_parameter_ids,
+                key=lambda x: [x[i] for i in range(len(x))],
+            ),
         ]
     )
```

### Comparing `petab_select-0.1.7/petab_select.egg-info/PKG-INFO` & `petab_select-0.1.8/petab_select.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petab-select
-Version: 0.1.7
+Version: 0.1.8
 Summary: PEtab Select: an extension to PEtab for model selection.
 Home-page: https://github.com/PEtab-dev/petab_select
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `petab_select-0.1.7/petab_select.egg-info/SOURCES.txt` & `petab_select-0.1.8/petab_select.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.7/setup.py` & `petab_select-0.1.8/setup.py`

 * *Files identical despite different names*

