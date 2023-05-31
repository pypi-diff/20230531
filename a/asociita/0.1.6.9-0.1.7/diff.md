# Comparing `tmp/asociita-0.1.6.9.tar.gz` & `tmp/asociita-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asociita-0.1.6.9.tar", max compression
+gzip compressed data, was "asociita-0.1.7.tar", max compression
```

## Comparing `asociita-0.1.6.9.tar` & `asociita-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0        0 2023-04-07 16:31:28.755226 asociita-0.1.6.9/asociita/__init__.py
--rw-r--r--   0        0        0     3959 2023-05-20 16:17:12.712011 asociita-0.1.6.9/asociita/components/archiver/archive_manager.py
--rw-r--r--   0        0        0     4768 2023-05-18 12:35:56.518494 asociita-0.1.6.9/asociita/components/evaluator/evaluation_manager.py
--rw-r--r--   0        0        0    13585 2023-05-04 12:29:03.864051 asociita-0.1.6.9/asociita/components/evaluator/mr_evaluator.py
--rw-r--r--   0        0        0    10175 2023-05-03 13:58:58.211507 asociita-0.1.6.9/asociita/components/evaluator/or_evaluator.py
--rw-r--r--   0        0        0     4497 2023-04-17 14:01:29.838168 asociita-0.1.6.9/asociita/components/nodes/federated_node.py
--rw-r--r--   0        0        0     7400 2023-05-20 16:22:57.462290 asociita-0.1.6.9/asociita/components/orchestrator/evaluator_orchestrator.py
--rw-r--r--   0        0        0     6202 2023-05-20 16:45:47.898655 asociita-0.1.6.9/asociita/components/orchestrator/fedopt_orchestrator.py
--rw-r--r--   0        0        0    11300 2023-05-29 14:02:15.655724 asociita-0.1.6.9/asociita/components/orchestrator/generic_orchestrator.py
--rw-r--r--   0        0        0     2190 2023-05-22 09:43:29.422557 asociita-0.1.6.9/asociita/datasets/fetch_data.py
--rw-r--r--   0        0        0     2699 2023-05-22 14:23:05.141330 asociita-0.1.6.9/asociita/datasets/load_cifar.py
--rw-r--r--   0        0        0     2654 2023-05-22 14:12:53.922859 asociita-0.1.6.9/asociita/datasets/load_mnist.py
--rw-r--r--   0        0        0     6874 2023-05-22 14:12:25.240855 asociita-0.1.6.9/asociita/datasets/shard_splits.py
--rw-r--r--   0        0        0     4661 2023-05-22 14:08:01.227174 asociita-0.1.6.9/asociita/datasets/shard_transformation.py
--rw-r--r--   0        0        0      329 2023-05-19 09:42:13.494113 asociita-0.1.6.9/asociita/exceptions/settingexception.py
--rw-r--r--   0        0        0      701 2023-05-20 18:16:28.662467 asociita-0.1.6.9/asociita/models/pytorch/cifar10.py
--rw-r--r--   0        0        0    15195 2023-05-29 14:02:15.656751 asociita-0.1.6.9/asociita/models/pytorch/federated_model.py
--rw-r--r--   0        0        0      966 2023-05-12 12:18:20.228520 asociita-0.1.6.9/asociita/models/pytorch/mnist.py
--rw-r--r--   0        0        0     6068 2023-04-26 13:48:40.502010 asociita-0.1.6.9/asociita/utils/computations.py
--rw-r--r--   0        0        0      633 2023-05-12 12:12:31.672198 asociita-0.1.6.9/asociita/utils/custom_transformations.py
--rw-r--r--   0        0        0     4756 2023-05-17 12:51:14.070551 asociita-0.1.6.9/asociita/utils/handlers.py
--rw-r--r--   0        0        0      585 2023-05-22 14:29:57.943413 asociita-0.1.6.9/asociita/utils/helpers.py
--rw-r--r--   0        0        0     1843 2023-04-14 15:47:01.523825 asociita-0.1.6.9/asociita/utils/loggers.py
--rw-r--r--   0        0        0     4192 2023-05-29 14:02:15.657751 asociita-0.1.6.9/asociita/utils/optimizers.py
--rw-r--r--   0        0        0     4176 2023-04-19 13:27:23.001147 asociita-0.1.6.9/asociita/utils/orchestrations.py
--rw-r--r--   0        0        0     1059 2023-05-03 14:04:40.497199 asociita-0.1.6.9/asociita/utils/showcase.py
--rw-r--r--   0        0        0     1084 2023-04-07 16:30:34.501923 asociita-0.1.6.9/LICENSE
--rw-r--r--   0        0        0      705 2023-05-29 14:05:01.254994 asociita-0.1.6.9/pyproject.toml
--rw-r--r--   0        0        0     2862 2023-04-18 20:10:20.511705 asociita-0.1.6.9/README.md
--rw-r--r--   0        0        0     4024 1970-01-01 00:00:00.000000 asociita-0.1.6.9/setup.py
--rw-r--r--   0        0        0     3767 1970-01-01 00:00:00.000000 asociita-0.1.6.9/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-29 08:30:33.477904 asociita-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2812 2023-05-29 08:30:33.477904 asociita-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 08:30:33.477904 asociita-0.1.7/asociita/__init__.py
+-rw-r--r--   0        0        0     3881 2023-05-29 08:30:33.477904 asociita-0.1.7/asociita/components/archiver/archive_manager.py
+-rw-r--r--   0        0        0     4650 2023-05-29 08:30:33.477904 asociita-0.1.7/asociita/components/evaluator/evaluation_manager.py
+-rw-r--r--   0        0        0    13324 2023-05-29 08:30:33.477904 asociita-0.1.7/asociita/components/evaluator/mr_evaluator.py
+-rw-r--r--   0        0        0     9972 2023-05-29 08:30:33.477904 asociita-0.1.7/asociita/components/evaluator/or_evaluator.py
+-rw-r--r--   0        0        0     4370 2023-05-31 10:46:23.372156 asociita-0.1.7/asociita/components/nodes/federated_node.py
+-rw-r--r--   0        0        0     7266 2023-05-29 08:30:33.477904 asociita-0.1.7/asociita/components/orchestrator/evaluator_orchestrator.py
+-rw-r--r--   0        0        0     6083 2023-05-29 08:30:33.477904 asociita-0.1.7/asociita/components/orchestrator/fedopt_orchestrator.py
+-rw-r--r--   0        0        0    11069 2023-05-29 11:25:00.192088 asociita-0.1.7/asociita/components/orchestrator/generic_orchestrator.py
+-rw-r--r--   0        0        0     2635 2023-05-30 14:56:02.584171 asociita-0.1.7/asociita/datasets/fetch_data.py
+-rw-r--r--   0        0        0     2639 2023-05-29 08:30:33.477904 asociita-0.1.7/asociita/datasets/load_cifar.py
+-rw-r--r--   0        0        0     2612 2023-05-30 14:56:14.419772 asociita-0.1.7/asociita/datasets/load_fmnist.py
+-rw-r--r--   0        0        0     2595 2023-05-29 08:30:33.477904 asociita-0.1.7/asociita/datasets/load_mnist.py
+-rw-r--r--   0        0        0     6766 2023-05-30 09:52:26.729788 asociita-0.1.7/asociita/datasets/shard_splits.py
+-rw-r--r--   0        0        0     5962 2023-05-30 10:15:28.967345 asociita-0.1.7/asociita/datasets/shard_transformation.py
+-rw-r--r--   0        0        0      322 2023-05-29 08:30:33.477904 asociita-0.1.7/asociita/exceptions/settingexception.py
+-rw-r--r--   0        0        0      679 2023-05-29 08:30:33.481904 asociita-0.1.7/asociita/models/pytorch/cifar10.py
+-rw-r--r--   0        0        0    14810 2023-05-31 12:16:49.573243 asociita-0.1.7/asociita/models/pytorch/federated_model.py
+-rw-r--r--   0        0        0      934 2023-05-31 13:26:40.943955 asociita-0.1.7/asociita/models/pytorch/mnist.py
+-rw-r--r--   0        0        0     5918 2023-05-29 08:30:33.481904 asociita-0.1.7/asociita/utils/computations.py
+-rw-r--r--   0        0        0      613 2023-05-29 08:30:33.481904 asociita-0.1.7/asociita/utils/custom_transformations.py
+-rw-r--r--   0        0        0     4648 2023-05-29 08:30:33.481904 asociita-0.1.7/asociita/utils/handlers.py
+-rw-r--r--   0        0        0      572 2023-05-29 08:30:33.481904 asociita-0.1.7/asociita/utils/helpers.py
+-rw-r--r--   0        0        0     1796 2023-05-29 08:30:33.481904 asociita-0.1.7/asociita/utils/loggers.py
+-rw-r--r--   0        0        0     7792 2023-05-31 13:15:18.590875 asociita-0.1.7/asociita/utils/optimizers.py
+-rw-r--r--   0        0        0     4073 2023-05-29 08:30:33.481904 asociita-0.1.7/asociita/utils/orchestrations.py
+-rw-r--r--   0        0        0     1026 2023-05-29 08:30:33.481904 asociita-0.1.7/asociita/utils/showcase.py
+-rw-r--r--   0        0        0      678 2023-05-31 13:27:28.274363 asociita-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 asociita-0.1.7/PKG-INFO
```

### Comparing `asociita-0.1.6.9/asociita/components/archiver/archive_manager.py` & `asociita-0.1.7/asociita/components/archiver/archive_manager.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-from asociita.exceptions.settingexception import ArchiverSettingsException
-from asociita.models.pytorch.federated_model import FederatedModel
-from asociita.utils.handlers import Handler
-import os
-
-class Archive_Manager():
-    def __init__(self,
-                 archive_manager: dict,
-                 logger) -> None:
-        try:
-            # Modes
-            self.orchestrator_metrics = archive_manager["orchestrator"]
-            self.clients_on_central = archive_manager["clients_on_central"]
-            self.central_on_local = archive_manager["central_on_local"]
-            self.save_results = archive_manager["save_results"]
-            if self.save_results:
-                self.only_log = False
-            else:
-                self.only_log = archive_manager["log_results"]
-            
-            self.save_orchestrator_model = archive_manager["save_orchestrator_model"]
-
-            
-            # Paths and filenames for preserving metrics
-            self.metrics_savepath = archive_manager["metrics_savepath"]
-            self.orchestrator_metrics_file = archive_manager["orchestrator_filename"]
-            self.clients_on_central_file = archive_manager["clients_on_central_filename"]
-            self.central_on_local_file = archive_manager["central_on_local_filename"]
-
-            # Paths for preserving models
-            self.orchestrator_save_path = archive_manager["orchestrator_model_save_path"]
-            self.nodes_save_path = archive_manager["nodes_model_save_path"]
-
-        except ArchiverSettingsException:
-            raise ArchiverSettingsException
-        
-        self.logger = logger
-    
-    def archive_training_results(self,
-                        iteration: int,
-                        central_model: FederatedModel,
-                        nodes: list[FederatedModel]
-    ):
-        if self.orchestrator_metrics:
-            if self.save_results:
-                Handler.save_model_metrics(iteration=iteration,
-                                           model = central_model,
-                                           logger = self.logger,
-                                           saving_path = self.metrics_savepath,
-                                           log_to_screen = True,
-                                           file_name=self.orchestrator_metrics_file)
-            elif self.only_log:
-                Handler.log_model_metrics(iteration=iteration,
-                                          model=central_model,
-                                          logger = self.logger)
-            if self.save_orchestrator_model:
-                central_model.store_model_on_disk(iteration = iteration,
-                                                path = self.orchestrator_save_path)
-        
-        if self.central_on_local:
-            if self.save_results:
-                for node in nodes:
-                    Handler.save_model_metrics(iteration = iteration,
-                                               model = node.model,
-                                               logger = self.logger,
-                                               saving_path = self.metrics_savepath,
-                                               log_to_screen = True,
-                                               file_name=self.central_on_local_file) # PRESERVING METRICS FUNCTION -> CHANGE IF NEEDED
-            elif self.only_log:
-                for node in nodes:
-                    Handler.log_model_metrics(iteration = iteration,
-                                              model = node.model,
-                                              logger = self.logger)
-                
-                if self.nodes_save_path:
-                    for node in nodes:
-                        node.store_model_on_disk(iteration = iteration,
-                                                 path = self.nodes_save_path)
+from asociita.exceptions.settingexception import ArchiverSettingsException
+from asociita.models.pytorch.federated_model import FederatedModel
+from asociita.utils.handlers import Handler
+import os
+
+class Archive_Manager():
+    def __init__(self,
+                 archive_manager: dict,
+                 logger) -> None:
+        try:
+            # Modes
+            self.orchestrator_metrics = archive_manager["orchestrator"]
+            self.clients_on_central = archive_manager["clients_on_central"]
+            self.central_on_local = archive_manager["central_on_local"]
+            self.save_results = archive_manager["save_results"]
+            if self.save_results:
+                self.only_log = False
+            else:
+                self.only_log = archive_manager["log_results"]
+            
+            self.save_orchestrator_model = archive_manager["save_orchestrator_model"]
+
+            
+            # Paths and filenames for preserving metrics
+            self.metrics_savepath = archive_manager["metrics_savepath"]
+            self.orchestrator_metrics_file = archive_manager["orchestrator_filename"]
+            self.clients_on_central_file = archive_manager["clients_on_central_filename"]
+            self.central_on_local_file = archive_manager["central_on_local_filename"]
+
+            # Paths for preserving models
+            self.orchestrator_save_path = archive_manager["orchestrator_model_save_path"]
+            self.nodes_save_path = archive_manager["nodes_model_save_path"]
+
+        except ArchiverSettingsException:
+            raise ArchiverSettingsException
+        
+        self.logger = logger
+    
+    def archive_training_results(self,
+                        iteration: int,
+                        central_model: FederatedModel,
+                        nodes: list[FederatedModel]
+    ):
+        if self.orchestrator_metrics:
+            if self.save_results:
+                Handler.save_model_metrics(iteration=iteration,
+                                           model = central_model,
+                                           logger = self.logger,
+                                           saving_path = self.metrics_savepath,
+                                           log_to_screen = True,
+                                           file_name=self.orchestrator_metrics_file)
+            elif self.only_log:
+                Handler.log_model_metrics(iteration=iteration,
+                                          model=central_model,
+                                          logger = self.logger)
+            if self.save_orchestrator_model:
+                central_model.store_model_on_disk(iteration = iteration,
+                                                path = self.orchestrator_save_path)
+        
+        if self.central_on_local:
+            if self.save_results:
+                for node in nodes:
+                    Handler.save_model_metrics(iteration = iteration,
+                                               model = node.model,
+                                               logger = self.logger,
+                                               saving_path = self.metrics_savepath,
+                                               log_to_screen = True,
+                                               file_name=self.central_on_local_file) # PRESERVING METRICS FUNCTION -> CHANGE IF NEEDED
+            elif self.only_log:
+                for node in nodes:
+                    Handler.log_model_metrics(iteration = iteration,
+                                              model = node.model,
+                                              logger = self.logger)
+                
+                if self.nodes_save_path:
+                    for node in nodes:
+                        node.store_model_on_disk(iteration = iteration,
+                                                 path = self.nodes_save_path)
```

### Comparing `asociita-0.1.6.9/asociita/components/evaluator/evaluation_manager.py` & `asociita-0.1.7/asociita/components/evaluator/evaluation_manager.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-from asociita.components.evaluator.or_evaluator import OR_Evaluator
-from asociita.models.pytorch.federated_model import FederatedModel
-import os
-import csv
-
-
-class Evaluation_Manager():
-    def __init__(self,
-                settings: dict,
-                model: FederatedModel) -> None:
-        """Manages the process of evaluation. Creates an instance of 
-        Evaluation_Manager object, that controls all the instances
-        that perform evaluation.
-        
-        -------------
-        Args
-            settings (dict): dictionary object cotaining all the settings of the Evaluation_Manager.
-       -------------
-         Returns
-            None"""
-
-        self.settings = settings
-        # Sets up the flag for each available method of evaluation.
-        if settings['evaluation'].get("Shapley_OR"):
-            self.flag_shap_or = True
-        else:
-            self.flag_shap_or = False
-        
-        if settings['evaluation'].get("LOO_OR"):
-            self.flag_loo_or = True
-        else:
-            self.flag_loo_or = False
-
-        # Initialized an instance of the OR_Evaluator (One_Round Evaluator) if a flag is passed.
-        if self.flag_shap_or or self.flag_loo_or:
-            self.or_evaluator = OR_Evaluator(settings=settings,
-                                             model=model)
-    
-
-    def track_gradients(self,
-                        gradients: dict):
-        """Tracks the models' gradinets for the One Round Evaluator.
-        Specifically, reconstruct gradients for every possible coalition
-        of interest.
-        
-        -------------
-        Args
-            gradients (dict): Dictionary mapping each node to its respective gradients.
-       -------------
-         Returns
-            None"""
-        if self.flag_shap_or:
-            self.or_evaluator.track_shapley(gradients=gradients)
-        elif self.flag_loo_or: # This is called ONLY when we don't calculate Shapley, but we calculate LOO
-            self.or_evaluator.track_loo(gradients=gradients)
-    
-
-    def calculate_results(self,
-                          map_results:bool = True) -> dict[str:dict] | None:
-        """Calculate results for each contribution analysis method. 
-        
-        -------------
-        Args
-            map_results (bool): If set to true, the method will map results
-                of the evaluation to each node and will return an additionall
-                dictionary of the format: {node_id: {method:score, method:score}}
-       -------------
-         Returns
-            results | None"""
-        results = {}
-        if map_results:
-            mapped_results = {node: {'node_number': node} for node in self.settings['nodes']}
-        
-        if self.flag_shap_or:
-            self.or_evaluator.calculate_shaply()
-            results["Shapley_OneRound"] = self.or_evaluator.shapley_values
-            if map_results:
-                for node, result in zip(mapped_results, results['Shapley_OneRound'].values()):
-                    mapped_results[node]["shapley_one_round"] = result
-
-        
-        if self.flag_loo_or:
-            self.or_evaluator.calculate_loo()
-            results["LOO_OneRound"] = self.or_evaluator.loo_values
-            if map_results:
-                for node, result in zip(mapped_results, results['LOO_OneRound'].values()):
-                    mapped_results[node]['leave_one_out_one_round'] = result
-        
-        if mapped_results:
-            return (results, mapped_results)
-        else:
-            return results
-
-
-    def save_results(self,
-                     path: str,
-                     mapped_results: str,
-                     file_name: str = 'contribution_results') -> None:
-        """Preserves metrics of every contribution index calculated by the manager
-        in a csv file.
-        -------------
-        Args
-            path (str): a path to the directory in which the file should be saved.
-            mapped_results: results mapped to each note, stored in a dictionary
-                of a format {node_id: {method:score, method:score}
-            file_name (str): a proper filename with .csv ending. Default is
-                "contribution.results.csv
-       -------------
-         Returns
-            results | None"""
-        file_name = 'contribution_results.csv'
-        path = os.path.join(path, file_name)
-        with open(path, 'w', newline='') as csvfile:
-            header = [column_name for column_name in mapped_results[0].keys()]
-            writer = csv.DictWriter(csvfile, fieldnames=header)
-
-            writer.writeheader()
-            for row in mapped_results.values():
+from asociita.components.evaluator.or_evaluator import OR_Evaluator
+from asociita.models.pytorch.federated_model import FederatedModel
+import os
+import csv
+
+
+class Evaluation_Manager():
+    def __init__(self,
+                settings: dict,
+                model: FederatedModel) -> None:
+        """Manages the process of evaluation. Creates an instance of 
+        Evaluation_Manager object, that controls all the instances
+        that perform evaluation.
+        
+        -------------
+        Args
+            settings (dict): dictionary object cotaining all the settings of the Evaluation_Manager.
+       -------------
+         Returns
+            None"""
+
+        self.settings = settings
+        # Sets up the flag for each available method of evaluation.
+        if settings['evaluation'].get("Shapley_OR"):
+            self.flag_shap_or = True
+        else:
+            self.flag_shap_or = False
+        
+        if settings['evaluation'].get("LOO_OR"):
+            self.flag_loo_or = True
+        else:
+            self.flag_loo_or = False
+
+        # Initialized an instance of the OR_Evaluator (One_Round Evaluator) if a flag is passed.
+        if self.flag_shap_or or self.flag_loo_or:
+            self.or_evaluator = OR_Evaluator(settings=settings,
+                                             model=model)
+    
+
+    def track_gradients(self,
+                        gradients: dict):
+        """Tracks the models' gradinets for the One Round Evaluator.
+        Specifically, reconstruct gradients for every possible coalition
+        of interest.
+        
+        -------------
+        Args
+            gradients (dict): Dictionary mapping each node to its respective gradients.
+       -------------
+         Returns
+            None"""
+        if self.flag_shap_or:
+            self.or_evaluator.track_shapley(gradients=gradients)
+        elif self.flag_loo_or: # This is called ONLY when we don't calculate Shapley, but we calculate LOO
+            self.or_evaluator.track_loo(gradients=gradients)
+    
+
+    def calculate_results(self,
+                          map_results:bool = True) -> dict[str:dict] | None:
+        """Calculate results for each contribution analysis method. 
+        
+        -------------
+        Args
+            map_results (bool): If set to true, the method will map results
+                of the evaluation to each node and will return an additionall
+                dictionary of the format: {node_id: {method:score, method:score}}
+       -------------
+         Returns
+            results | None"""
+        results = {}
+        if map_results:
+            mapped_results = {node: {'node_number': node} for node in self.settings['nodes']}
+        
+        if self.flag_shap_or:
+            self.or_evaluator.calculate_shaply()
+            results["Shapley_OneRound"] = self.or_evaluator.shapley_values
+            if map_results:
+                for node, result in zip(mapped_results, results['Shapley_OneRound'].values()):
+                    mapped_results[node]["shapley_one_round"] = result
+
+        
+        if self.flag_loo_or:
+            self.or_evaluator.calculate_loo()
+            results["LOO_OneRound"] = self.or_evaluator.loo_values
+            if map_results:
+                for node, result in zip(mapped_results, results['LOO_OneRound'].values()):
+                    mapped_results[node]['leave_one_out_one_round'] = result
+        
+        if mapped_results:
+            return (results, mapped_results)
+        else:
+            return results
+
+
+    def save_results(self,
+                     path: str,
+                     mapped_results: str,
+                     file_name: str = 'contribution_results') -> None:
+        """Preserves metrics of every contribution index calculated by the manager
+        in a csv file.
+        -------------
+        Args
+            path (str): a path to the directory in which the file should be saved.
+            mapped_results: results mapped to each note, stored in a dictionary
+                of a format {node_id: {method:score, method:score}
+            file_name (str): a proper filename with .csv ending. Default is
+                "contribution.results.csv
+       -------------
+         Returns
+            results | None"""
+        file_name = 'contribution_results.csv'
+        path = os.path.join(path, file_name)
+        with open(path, 'w', newline='') as csvfile:
+            header = [column_name for column_name in mapped_results[0].keys()]
+            writer = csv.DictWriter(csvfile, fieldnames=header)
+
+            writer.writeheader()
+            for row in mapped_results.values():
                 writer.writerow(row)
```

### Comparing `asociita-0.1.6.9/asociita/components/evaluator/mr_evaluator.py` & `asociita-0.1.7/asociita/components/evaluator/mr_evaluator.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,261 +1,261 @@
-# LIBRARY MODULES IMPORT
-from asociita.utils.computations import Subsets
-from asociita.models.pytorch.federated_model import FederatedModel
-from asociita.utils.computations import Aggregators
-from asociita.utils.optimizers import Optimizers
-from copy import deepcopy
-# ADDITIONAL IMPORTS
-import math
-
-
-class MR_Evaluator():
-    def __init__(self,
-                 settings: dict,
-                 model: FederatedModel) -> None:
-        """A multi_round evaluator that calculates partial values each round
-          and then aggregates to compute the final metric.
-        -------------
-        Args
-            settings (dict): dictionary object cotaining all the settings of the orchestrator.
-            model (FederatedModel): a primary (initial) model that will be deep-copied for each coalition.
-       -------------
-         Returns
-            None"""
-        self.settings = settings
-        self.evaluation = settings['evaluation']
-        self.rounds = settings['orchestrator']['iterations']
-        self.recorded_values = {} # Maps every coalition to it's value, implemented to decrease the complexity.
-        self.shapley_mr_recon = None
-        
-        # Creates coalitions for Shapley, if so indicated in the settings.
-        if self.evaluation.get("Shapley_OR"):
-            self.shapley_values = {node:float(0) for node in settings['nodes']} # Final dict (of Shapley evaluation)
-            self.partial_shapley = {round: {node:float(0) for node in settings['nodes']} for round in range(self.rounds)} # Partial shapley values
-            self.shapley_mr_recon = Subsets.form_superset(settings['nodes'], return_dict=False)
-            self.shapley_mr_recon = {tuple(coalition) : deepcopy(model) for 
-                                     coalition in self.shapley_or_recon}
-        
-        # Creates coalition for Leave-one-out, if so indicated in the settings.
-        if self.evaluation.get("LOO_OR"):
-            self.loo_values = {node:float(0) for node in settings['nodes']} # Final list (of LOO evaluation)
-            self.loo_values = {round: {node:float(0) for node in settings['nodes']} for round in range(self.rounds)} # Partial LOO values.
-            if self.shapley_or_recon: # If we already have coalition for shapleys values, we can use model of those
-                self.loo_mr_recon = {coalition: model for coalition, model in self.shapley_or_recon.items()
-                                     if len(coalition) >= (settings["number_of_nodes"] - 1)}
-            else:
-                self.loo_mr_recon = Subsets.form_loo_set(settings['nodes'], return_dict=False) # Else we have to create a new one.
-                self.loo_mr_recon = {tuple(coaliton) : deepcopy(model) for
-                                     coaliton in self.loo_or_recon}
-
-
-    def track_shapley(self,
-                      gradients: dict):
-        """A method that allows to collect gradients from the t-th round of the training and
-        update all the models in every coalition of interest.
-        
-        -------------
-        Args
-            gradients (dict): Dictionary mapping each node to its respective gradients.
-       -------------
-         Returns
-            None"""
-        
-        # Establishing gradients for all possible coalitions in N
-        delta_s = Subsets.form_superset(self.settings["nodes"], return_dict=True)
-        for coalition in delta_s:
-            specific_gradients = {}
-            for member in coalition:
-                specific_gradients[member] = gradients[member]
-            delta_s[coalition] = Aggregators.compute_average(specific_gradients)
-        
-        # Upadting models of all possible coalitions in N
-        for coalition in self.shapley_mr_recon:
-            model_s_t = self.shapley_mr_recon[coalition]
-            delta_s_t = delta_s[coalition]
-            updated_weights = Optimizers.SimpleFedopt(weights=model_s_t.get_weights(),
-                                                                       delta=delta_s_t,
-                                                                       learning_rate=0.99)
-            self.shapley_mr_recon[coalition].update_weights(updated_weights)
-    
-
-    def calculate_partial_shapley(self,
-                                round: int):
-        N = self.settings['number_of_nodes']
-        operation_counter = 1
-        number_of_operations = 2 ** N - 1
-        for node in self.partial_shapley[round]:
-            shapley_value = float(0)
-            subsets = Subsets.select_subsets(coalitions=self.shapley_or_recon,
-                                            searched_node=node)
-            for subset in subsets.keys():
-                subset_without_i = tuple(sorted(subset))
-                subset_with_i = tuple(sorted(subset + (node, )))
-
-                if subset_without_i in self.recorded_values:
-                    score_without_i = self.recorded_values[subset_without_i]
-                else:
-                    print(f"{operation_counter} of {number_of_operations}: forming and evaluating subset {subset_without_i}")
-                    model_without_i = self.shapley_or_recon[subset_without_i]
-                    score_without_i = model_without_i.evaluate_model()[1]
-                    self.recorded_values[subset_without_i] = score_without_i
-                    print(f"Coalition of {subset_without_i} scored {self.recorded_values[subset_without_i]}")
-                    operation_counter += 1
-
-                if subset_with_i in self.recorded_values:
-                    score_with_i = self.recorded_values[subset_with_i]
-                else:
-                    print(f"{operation_counter} of {number_of_operations}: forming and evaluating subset {subset_with_i}")
-                    model_with_i = self.shapley_or_recon[subset_with_i]
-                    score_with_i = model_with_i.evaluate_model()[1]
-                    self.recorded_values[subset_with_i] = score_with_i
-                    print(f"Coalition of {subset_with_i} scored {self.recorded_values[subset_with_i]}")
-                    operation_counter += 1
-                
-                summand = (score_with_i - score_without_i) /  math.comb((N-1), len(subset))
-                shapley_value += summand
-
-            # One last summand - empty set
-            score_without_i = float(0) # since v(empty_set) = 0
-            subset_with_i = (node, )
-            if subset_with_i in self.recorded_values:
-                    score_with_i = self.recorded_values[subset_with_i]
-            else:
-                print(f"{operation_counter} of {number_of_operations}: forming and evaluating subset {subset_with_i}")
-                model_with_i = self.shapley_or_recon[subset_with_i]
-                score_with_i = model_with_i.evaluate_model()[1]
-                self.recorded_values[subset_with_i] = score_with_i
-                print(f"Coalition of {subset_with_i} scored {self.recorded_values[subset_with_i]}")
-                operation_counter += 1
-            
-            summand = (score_with_i - score_without_i) /  math.comb((N-1), len(subset))
-            shapley_value += summand
-            
-            self.shapley_values[node] = (shapley_value / self.settings['number_of_nodes'])
-    
-
-    def track_loo(self,
-                   gradients: dict):
-        """A method that allows to collect gradients from the t-th round of the training and
-        update all the models in every coalition of interest. Note that it should be called
-        ONLY when we DO NOT track Shapley values. Otherwise, models used for LOO evaluation
-        will be a shallow copy of some of the models used for Shapley valuation and SHOULD NOT
-        be updated again.
-        
-        -------------
-        Args
-            gradients (dict): Dictionary mapping each node to its respective gradients.
-       -------------
-         Returns
-            None"""
-        
-        # Establishing gradients for all possible coalitions in N
-        delta_s = {coalition: float(0) for coalition in self.loo_or_recon.keys()}
-        for coalition in delta_s:
-            specific_gradients = {}
-            for member in coalition:
-                specific_gradients[member] = gradients[member]
-            delta_s[coalition] = Aggregators.compute_average(specific_gradients)
-        
-        # Upadting models of all possible coalitions in N
-        for coalition in self.loo_or_recon:
-            model_s_t = self.loo_or_recon[coalition]
-            delta_s_t = delta_s[coalition]
-            updated_weights = Optimizers.SimpleFedopt(weights=model_s_t.get_weights(),
-                                                      delta=delta_s_t,
-                                                      learning_rate=0.99)
-            self.loo_or_recon[coalition].update_weights(updated_weights)
-
-    def calculate_shaply(self):
-        """Calculates Shapley values.
-        -------------
-        Args
-            None
-       -------------
-         Returns
-            None"""
-        N = self.settings['number_of_nodes']
-        operation_counter = 1
-        number_of_operations = 2 ** N - 1
-        for node in self.shapley_values:
-            shapley_value = float(0)
-            subsets = Subsets.select_subsets(coalitions=self.shapley_or_recon,
-                                            searched_node=node)
-            for subset in subsets.keys():
-                subset_without_i = tuple(sorted(subset))
-                subset_with_i = tuple(sorted(subset + (node, )))
-
-                if subset_without_i in self.recorded_values:
-                    score_without_i = self.recorded_values[subset_without_i]
-                else:
-                    print(f"{operation_counter} of {number_of_operations}: forming and evaluating subset {subset_without_i}")
-                    model_without_i = self.shapley_or_recon[subset_without_i]
-                    score_without_i = model_without_i.evaluate_model()[1]
-                    self.recorded_values[subset_without_i] = score_without_i
-                    print(f"Coalition of {subset_without_i} scored {self.recorded_values[subset_without_i]}")
-                    operation_counter += 1
-
-                if subset_with_i in self.recorded_values:
-                    score_with_i = self.recorded_values[subset_with_i]
-                else:
-                    print(f"{operation_counter} of {number_of_operations}: forming and evaluating subset {subset_with_i}")
-                    model_with_i = self.shapley_or_recon[subset_with_i]
-                    score_with_i = model_with_i.evaluate_model()[1]
-                    self.recorded_values[subset_with_i] = score_with_i
-                    print(f"Coalition of {subset_with_i} scored {self.recorded_values[subset_with_i]}")
-                    operation_counter += 1
-                
-                summand = (score_with_i - score_without_i) /  math.comb((N-1), len(subset))
-                shapley_value += summand
-
-            # One last summand - empty set
-            score_without_i = float(0) # since v(empty_set) = 0
-            subset_with_i = (node, )
-            if subset_with_i in self.recorded_values:
-                    score_with_i = self.recorded_values[subset_with_i]
-            else:
-                print(f"{operation_counter} of {number_of_operations}: forming and evaluating subset {subset_with_i}")
-                model_with_i = self.shapley_or_recon[subset_with_i]
-                score_with_i = model_with_i.evaluate_model()[1]
-                self.recorded_values[subset_with_i] = score_with_i
-                print(f"Coalition of {subset_with_i} scored {self.recorded_values[subset_with_i]}")
-                operation_counter += 1
-            
-            summand = (score_with_i - score_without_i) /  math.comb((N-1), len(subset))
-            shapley_value += summand
-            
-            self.shapley_values[node] = (shapley_value / self.settings['number_of_nodes'])
-    
-
-    def calculate_loo(self):
-        """Calculates Leave-one-out values.
-        -------------
-        Args
-            None
-       -------------
-         Returns
-            None"""
-        
-        all_nodes = deepcopy(self.settings['nodes'])
-        general_subset = tuple(self.settings['nodes'])
-        if general_subset in self.recorded_values:
-            general_score = self.recorded_values[general_subset]
-        else:
-            print(f"Forming and evaluating subset {general_subset}")
-            general_model = self.loo_or_recon[general_subset]
-            general_score = general_model.evaluate_model()[1]
-            self.recorded_values[general_subset] = general_score
-        
-        for node in self.loo_values:
-            subset_without_i = deepcopy(all_nodes)
-            subset_without_i.remove(node)
-            subset_without_i = tuple(sorted(subset_without_i))
-            if subset_without_i in self.recorded_values:
-                score_without_i = self.recorded_values[subset_without_i]
-            else:
-                print(f"Forming and evaluating subset {subset_without_i}")
-                model_without_i = self.loo_or_recon[subset_without_i]
-                score_without_i = model_without_i.evaluate_model()[1]
-                self.recorded_values[subset_without_i] = score_without_i
-            
-            self.loo_values[node] = general_score - score_without_i
-            
+# LIBRARY MODULES IMPORT
+from asociita.utils.computations import Subsets
+from asociita.models.pytorch.federated_model import FederatedModel
+from asociita.utils.computations import Aggregators
+from asociita.utils.optimizers import Optimizers
+from copy import deepcopy
+# ADDITIONAL IMPORTS
+import math
+
+
+class MR_Evaluator():
+    def __init__(self,
+                 settings: dict,
+                 model: FederatedModel) -> None:
+        """A multi_round evaluator that calculates partial values each round
+          and then aggregates to compute the final metric.
+        -------------
+        Args
+            settings (dict): dictionary object cotaining all the settings of the orchestrator.
+            model (FederatedModel): a primary (initial) model that will be deep-copied for each coalition.
+       -------------
+         Returns
+            None"""
+        self.settings = settings
+        self.evaluation = settings['evaluation']
+        self.rounds = settings['orchestrator']['iterations']
+        self.recorded_values = {} # Maps every coalition to it's value, implemented to decrease the complexity.
+        self.shapley_mr_recon = None
+        
+        # Creates coalitions for Shapley, if so indicated in the settings.
+        if self.evaluation.get("Shapley_OR"):
+            self.shapley_values = {node:float(0) for node in settings['nodes']} # Final dict (of Shapley evaluation)
+            self.partial_shapley = {round: {node:float(0) for node in settings['nodes']} for round in range(self.rounds)} # Partial shapley values
+            self.shapley_mr_recon = Subsets.form_superset(settings['nodes'], return_dict=False)
+            self.shapley_mr_recon = {tuple(coalition) : deepcopy(model) for 
+                                     coalition in self.shapley_or_recon}
+        
+        # Creates coalition for Leave-one-out, if so indicated in the settings.
+        if self.evaluation.get("LOO_OR"):
+            self.loo_values = {node:float(0) for node in settings['nodes']} # Final list (of LOO evaluation)
+            self.loo_values = {round: {node:float(0) for node in settings['nodes']} for round in range(self.rounds)} # Partial LOO values.
+            if self.shapley_or_recon: # If we already have coalition for shapleys values, we can use model of those
+                self.loo_mr_recon = {coalition: model for coalition, model in self.shapley_or_recon.items()
+                                     if len(coalition) >= (settings["number_of_nodes"] - 1)}
+            else:
+                self.loo_mr_recon = Subsets.form_loo_set(settings['nodes'], return_dict=False) # Else we have to create a new one.
+                self.loo_mr_recon = {tuple(coaliton) : deepcopy(model) for
+                                     coaliton in self.loo_or_recon}
+
+
+    def track_shapley(self,
+                      gradients: dict):
+        """A method that allows to collect gradients from the t-th round of the training and
+        update all the models in every coalition of interest.
+        
+        -------------
+        Args
+            gradients (dict): Dictionary mapping each node to its respective gradients.
+       -------------
+         Returns
+            None"""
+        
+        # Establishing gradients for all possible coalitions in N
+        delta_s = Subsets.form_superset(self.settings["nodes"], return_dict=True)
+        for coalition in delta_s:
+            specific_gradients = {}
+            for member in coalition:
+                specific_gradients[member] = gradients[member]
+            delta_s[coalition] = Aggregators.compute_average(specific_gradients)
+        
+        # Upadting models of all possible coalitions in N
+        for coalition in self.shapley_mr_recon:
+            model_s_t = self.shapley_mr_recon[coalition]
+            delta_s_t = delta_s[coalition]
+            updated_weights = Optimizers.SimpleFedopt(weights=model_s_t.get_weights(),
+                                                                       delta=delta_s_t,
+                                                                       learning_rate=0.99)
+            self.shapley_mr_recon[coalition].update_weights(updated_weights)
+    
+
+    def calculate_partial_shapley(self,
+                                round: int):
+        N = self.settings['number_of_nodes']
+        operation_counter = 1
+        number_of_operations = 2 ** N - 1
+        for node in self.partial_shapley[round]:
+            shapley_value = float(0)
+            subsets = Subsets.select_subsets(coalitions=self.shapley_or_recon,
+                                            searched_node=node)
+            for subset in subsets.keys():
+                subset_without_i = tuple(sorted(subset))
+                subset_with_i = tuple(sorted(subset + (node, )))
+
+                if subset_without_i in self.recorded_values:
+                    score_without_i = self.recorded_values[subset_without_i]
+                else:
+                    print(f"{operation_counter} of {number_of_operations}: forming and evaluating subset {subset_without_i}")
+                    model_without_i = self.shapley_or_recon[subset_without_i]
+                    score_without_i = model_without_i.evaluate_model()[1]
+                    self.recorded_values[subset_without_i] = score_without_i
+                    print(f"Coalition of {subset_without_i} scored {self.recorded_values[subset_without_i]}")
+                    operation_counter += 1
+
+                if subset_with_i in self.recorded_values:
+                    score_with_i = self.recorded_values[subset_with_i]
+                else:
+                    print(f"{operation_counter} of {number_of_operations}: forming and evaluating subset {subset_with_i}")
+                    model_with_i = self.shapley_or_recon[subset_with_i]
+                    score_with_i = model_with_i.evaluate_model()[1]
+                    self.recorded_values[subset_with_i] = score_with_i
+                    print(f"Coalition of {subset_with_i} scored {self.recorded_values[subset_with_i]}")
+                    operation_counter += 1
+                
+                summand = (score_with_i - score_without_i) /  math.comb((N-1), len(subset))
+                shapley_value += summand
+
+            # One last summand - empty set
+            score_without_i = float(0) # since v(empty_set) = 0
+            subset_with_i = (node, )
+            if subset_with_i in self.recorded_values:
+                    score_with_i = self.recorded_values[subset_with_i]
+            else:
+                print(f"{operation_counter} of {number_of_operations}: forming and evaluating subset {subset_with_i}")
+                model_with_i = self.shapley_or_recon[subset_with_i]
+                score_with_i = model_with_i.evaluate_model()[1]
+                self.recorded_values[subset_with_i] = score_with_i
+                print(f"Coalition of {subset_with_i} scored {self.recorded_values[subset_with_i]}")
+                operation_counter += 1
+            
+            summand = (score_with_i - score_without_i) /  math.comb((N-1), len(subset))
+            shapley_value += summand
+            
+            self.shapley_values[node] = (shapley_value / self.settings['number_of_nodes'])
+    
+
+    def track_loo(self,
+                   gradients: dict):
+        """A method that allows to collect gradients from the t-th round of the training and
+        update all the models in every coalition of interest. Note that it should be called
+        ONLY when we DO NOT track Shapley values. Otherwise, models used for LOO evaluation
+        will be a shallow copy of some of the models used for Shapley valuation and SHOULD NOT
+        be updated again.
+        
+        -------------
+        Args
+            gradients (dict): Dictionary mapping each node to its respective gradients.
+       -------------
+         Returns
+            None"""
+        
+        # Establishing gradients for all possible coalitions in N
+        delta_s = {coalition: float(0) for coalition in self.loo_or_recon.keys()}
+        for coalition in delta_s:
+            specific_gradients = {}
+            for member in coalition:
+                specific_gradients[member] = gradients[member]
+            delta_s[coalition] = Aggregators.compute_average(specific_gradients)
+        
+        # Upadting models of all possible coalitions in N
+        for coalition in self.loo_or_recon:
+            model_s_t = self.loo_or_recon[coalition]
+            delta_s_t = delta_s[coalition]
+            updated_weights = Optimizers.SimpleFedopt(weights=model_s_t.get_weights(),
+                                                      delta=delta_s_t,
+                                                      learning_rate=0.99)
+            self.loo_or_recon[coalition].update_weights(updated_weights)
+
+    def calculate_shaply(self):
+        """Calculates Shapley values.
+        -------------
+        Args
+            None
+       -------------
+         Returns
+            None"""
+        N = self.settings['number_of_nodes']
+        operation_counter = 1
+        number_of_operations = 2 ** N - 1
+        for node in self.shapley_values:
+            shapley_value = float(0)
+            subsets = Subsets.select_subsets(coalitions=self.shapley_or_recon,
+                                            searched_node=node)
+            for subset in subsets.keys():
+                subset_without_i = tuple(sorted(subset))
+                subset_with_i = tuple(sorted(subset + (node, )))
+
+                if subset_without_i in self.recorded_values:
+                    score_without_i = self.recorded_values[subset_without_i]
+                else:
+                    print(f"{operation_counter} of {number_of_operations}: forming and evaluating subset {subset_without_i}")
+                    model_without_i = self.shapley_or_recon[subset_without_i]
+                    score_without_i = model_without_i.evaluate_model()[1]
+                    self.recorded_values[subset_without_i] = score_without_i
+                    print(f"Coalition of {subset_without_i} scored {self.recorded_values[subset_without_i]}")
+                    operation_counter += 1
+
+                if subset_with_i in self.recorded_values:
+                    score_with_i = self.recorded_values[subset_with_i]
+                else:
+                    print(f"{operation_counter} of {number_of_operations}: forming and evaluating subset {subset_with_i}")
+                    model_with_i = self.shapley_or_recon[subset_with_i]
+                    score_with_i = model_with_i.evaluate_model()[1]
+                    self.recorded_values[subset_with_i] = score_with_i
+                    print(f"Coalition of {subset_with_i} scored {self.recorded_values[subset_with_i]}")
+                    operation_counter += 1
+                
+                summand = (score_with_i - score_without_i) /  math.comb((N-1), len(subset))
+                shapley_value += summand
+
+            # One last summand - empty set
+            score_without_i = float(0) # since v(empty_set) = 0
+            subset_with_i = (node, )
+            if subset_with_i in self.recorded_values:
+                    score_with_i = self.recorded_values[subset_with_i]
+            else:
+                print(f"{operation_counter} of {number_of_operations}: forming and evaluating subset {subset_with_i}")
+                model_with_i = self.shapley_or_recon[subset_with_i]
+                score_with_i = model_with_i.evaluate_model()[1]
+                self.recorded_values[subset_with_i] = score_with_i
+                print(f"Coalition of {subset_with_i} scored {self.recorded_values[subset_with_i]}")
+                operation_counter += 1
+            
+            summand = (score_with_i - score_without_i) /  math.comb((N-1), len(subset))
+            shapley_value += summand
+            
+            self.shapley_values[node] = (shapley_value / self.settings['number_of_nodes'])
+    
+
+    def calculate_loo(self):
+        """Calculates Leave-one-out values.
+        -------------
+        Args
+            None
+       -------------
+         Returns
+            None"""
+        
+        all_nodes = deepcopy(self.settings['nodes'])
+        general_subset = tuple(self.settings['nodes'])
+        if general_subset in self.recorded_values:
+            general_score = self.recorded_values[general_subset]
+        else:
+            print(f"Forming and evaluating subset {general_subset}")
+            general_model = self.loo_or_recon[general_subset]
+            general_score = general_model.evaluate_model()[1]
+            self.recorded_values[general_subset] = general_score
+        
+        for node in self.loo_values:
+            subset_without_i = deepcopy(all_nodes)
+            subset_without_i.remove(node)
+            subset_without_i = tuple(sorted(subset_without_i))
+            if subset_without_i in self.recorded_values:
+                score_without_i = self.recorded_values[subset_without_i]
+            else:
+                print(f"Forming and evaluating subset {subset_without_i}")
+                model_without_i = self.loo_or_recon[subset_without_i]
+                score_without_i = model_without_i.evaluate_model()[1]
+                self.recorded_values[subset_without_i] = score_without_i
+            
+            self.loo_values[node] = general_score - score_without_i
+
```

### Comparing `asociita-0.1.6.9/asociita/components/evaluator/or_evaluator.py` & `asociita-0.1.7/asociita/components/evaluator/or_evaluator.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,203 +1,203 @@
-# LIBRARY MODULES IMPORT
-from asociita.utils.computations import Subsets
-from asociita.models.pytorch.federated_model import FederatedModel
-from asociita.utils.computations import Aggregators
-from asociita.utils.optimizers import Optimizers
-from copy import deepcopy
-# ADDITIONAL IMPORTS
-import math
-
-
-class OR_Evaluator():
-    def __init__(self,
-                 settings: dict,
-                 model: FederatedModel) -> None:
-        """A one_round evaluator that firstly collects all the models reconstructed
-        from gradients, and then perform an evaluation according to the chosen metric.
-        -------------
-        Args
-            settings (dict): dictionary object cotaining all the settings of the orchestrator.
-            model (FederatedModel): a primary (initial) model that will be deep-copied for each coalition.
-       -------------
-         Returns
-            None"""
-        self.settings = settings
-        self.evaluation = settings['evaluation']
-        self.recorded_values = {} # Maps every coalition to it's value, implemented to decrease the complexity.
-        self.shapley_or_recon = None
-        
-        # Creates coalitions for Shapley, if so indicated in the settings.
-        if self.evaluation.get("Shapley_OR"):
-            self.shapley_values = {node:float(0) for node in settings['nodes']} # Final list (of Shapley evaluation)
-            self.shapley_or_recon = Subsets.form_superset(settings['nodes'], return_dict=False)
-            self.shapley_or_recon = {tuple(coalition) : deepcopy(model) for 
-                                     coalition in self.shapley_or_recon}
-        
-        # Creates coalition for Leave-one-out, if so indicated in the settings.
-        if self.evaluation.get("LOO_OR"):
-            self.loo_values = {node:float(0) for node in settings['nodes']} # Final list (of LOO evaluation)
-            if self.shapley_or_recon: # If we already have coalition for shapleys values, we can use model of those
-                self.loo_or_recon = {coalition: model for coalition, model in self.shapley_or_recon.items()
-                                     if len(coalition) >= (settings["number_of_nodes"] - 1)}
-            else:
-                self.loo_or_recon = Subsets.form_loo_set(settings['nodes'], return_dict=False) # Else we have to create a new one.
-                self.loo_or_recon = {tuple(coaliton) : deepcopy(model) for
-                                     coaliton in self.loo_or_recon}
-
-
-    def track_shapley(self,
-                      gradients: dict):
-        """A method that allows to collect gradients from the t-th round of the training and
-        update all the models in every coalition of interest.
-        
-        -------------
-        Args
-            gradients (dict): Dictionary mapping each node to its respective gradients.
-       -------------
-         Returns
-            None"""
-        
-        # Establishing gradients for all possible coalitions in N
-        delta_s = Subsets.form_superset(self.settings["nodes"], return_dict=True)
-        for coalition in delta_s:
-            specific_gradients = {}
-            for member in coalition:
-                specific_gradients[member] = gradients[member]
-            delta_s[coalition] = Aggregators.compute_average(specific_gradients)
-        
-        # Upadting models of all possible coalitions in N
-        for coalition in self.shapley_or_recon:
-            model_s_t = self.shapley_or_recon[coalition]
-            delta_s_t = delta_s[coalition]
-            updated_weights = Optimizers.SimpleFedopt(weights=model_s_t.get_weights(),
-                                                                       delta=delta_s_t,
-                                                                       learning_rate=0.99)
-            self.shapley_or_recon[coalition].update_weights(updated_weights)
-    
-
-    def track_loo(self,
-                   gradients: dict):
-        """A method that allows to collect gradients from the t-th round of the training and
-        update all the models in every coalition of interest. Note that it should be called
-        ONLY when we DO NOT track Shapley values. Otherwise, models used for LOO evaluation
-        will be a shallow copy of some of the models used for Shapley valuation and SHOULD NOT
-        be updated again.
-        
-        -------------
-        Args
-            gradients (dict): Dictionary mapping each node to its respective gradients.
-       -------------
-         Returns
-            None"""
-        
-        # Establishing gradients for all possible coalitions in N
-        delta_s = {coalition: float(0) for coalition in self.loo_or_recon.keys()}
-        for coalition in delta_s:
-            specific_gradients = {}
-            for member in coalition:
-                specific_gradients[member] = gradients[member]
-            delta_s[coalition] = Aggregators.compute_average(specific_gradients)
-        
-        # Upadting models of all possible coalitions in N
-        for coalition in self.loo_or_recon:
-            model_s_t = self.loo_or_recon[coalition]
-            delta_s_t = delta_s[coalition]
-            updated_weights = Optimizers.SimpleFedopt(weights=model_s_t.get_weights(),
-                                                      delta=delta_s_t,
-                                                      learning_rate=0.99)
-            self.loo_or_recon[coalition].update_weights(updated_weights)
-
-    def calculate_shaply(self):
-        """Calculates Shapley values.
-        -------------
-        Args
-            None
-       -------------
-         Returns
-            None"""
-        N = self.settings['number_of_nodes']
-        operation_counter = 1
-        number_of_operations = 2 ** N - 1
-        for node in self.shapley_values:
-            shapley_value = float(0)
-            subsets = Subsets.select_subsets(coalitions=self.shapley_or_recon,
-                                            searched_node=node)
-            for subset in subsets.keys():
-                subset_without_i = tuple(sorted(subset))
-                subset_with_i = tuple(sorted(subset + (node, )))
-
-                if subset_without_i in self.recorded_values:
-                    score_without_i = self.recorded_values[subset_without_i]
-                else:
-                    print(f"{operation_counter} of {number_of_operations}: forming and evaluating subset {subset_without_i}")
-                    model_without_i = self.shapley_or_recon[subset_without_i]
-                    score_without_i = model_without_i.evaluate_model()[1]
-                    self.recorded_values[subset_without_i] = score_without_i
-                    print(f"Coalition of {subset_without_i} scored {self.recorded_values[subset_without_i]}")
-                    operation_counter += 1
-
-                if subset_with_i in self.recorded_values:
-                    score_with_i = self.recorded_values[subset_with_i]
-                else:
-                    print(f"{operation_counter} of {number_of_operations}: forming and evaluating subset {subset_with_i}")
-                    model_with_i = self.shapley_or_recon[subset_with_i]
-                    score_with_i = model_with_i.evaluate_model()[1]
-                    self.recorded_values[subset_with_i] = score_with_i
-                    print(f"Coalition of {subset_with_i} scored {self.recorded_values[subset_with_i]}")
-                    operation_counter += 1
-                
-                summand = (score_with_i - score_without_i) /  math.comb((N-1), len(subset))
-                shapley_value += summand
-
-            # One last summand - empty set
-            score_without_i = float(0) # since v(empty_set) = 0
-            subset_with_i = (node, )
-            if subset_with_i in self.recorded_values:
-                    score_with_i = self.recorded_values[subset_with_i]
-            else:
-                print(f"{operation_counter} of {number_of_operations}: forming and evaluating subset {subset_with_i}")
-                model_with_i = self.shapley_or_recon[subset_with_i]
-                score_with_i = model_with_i.evaluate_model()[1]
-                self.recorded_values[subset_with_i] = score_with_i
-                print(f"Coalition of {subset_with_i} scored {self.recorded_values[subset_with_i]}")
-                operation_counter += 1
-            
-            summand = (score_with_i - score_without_i) /  math.comb((N-1), len(subset))
-            shapley_value += summand
-            
-            self.shapley_values[node] = (shapley_value / self.settings['number_of_nodes'])
-    
-
-    def calculate_loo(self):
-        """Calculates Leave-one-out values.
-        -------------
-        Args
-            None
-       -------------
-         Returns
-            None"""
-        
-        all_nodes = deepcopy(self.settings['nodes'])
-        general_subset = tuple(self.settings['nodes'])
-        if general_subset in self.recorded_values:
-            general_score = self.recorded_values[general_subset]
-        else:
-            print(f"Forming and evaluating subset {general_subset}")
-            general_model = self.loo_or_recon[general_subset]
-            general_score = general_model.evaluate_model()[1]
-            self.recorded_values[general_subset] = general_score
-        
-        for node in self.loo_values:
-            subset_without_i = deepcopy(all_nodes)
-            subset_without_i.remove(node)
-            subset_without_i = tuple(sorted(subset_without_i))
-            if subset_without_i in self.recorded_values:
-                score_without_i = self.recorded_values[subset_without_i]
-            else:
-                print(f"Forming and evaluating subset {subset_without_i}")
-                model_without_i = self.loo_or_recon[subset_without_i]
-                score_without_i = model_without_i.evaluate_model()[1]
-                self.recorded_values[subset_without_i] = score_without_i
-            
-            self.loo_values[node] = general_score - score_without_i
-            
+# LIBRARY MODULES IMPORT
+from asociita.utils.computations import Subsets
+from asociita.models.pytorch.federated_model import FederatedModel
+from asociita.utils.computations import Aggregators
+from asociita.utils.optimizers import Optimizers
+from copy import deepcopy
+# ADDITIONAL IMPORTS
+import math
+
+
+class OR_Evaluator():
+    def __init__(self,
+                 settings: dict,
+                 model: FederatedModel) -> None:
+        """A one_round evaluator that firstly collects all the models reconstructed
+        from gradients, and then perform an evaluation according to the chosen metric.
+        -------------
+        Args
+            settings (dict): dictionary object cotaining all the settings of the orchestrator.
+            model (FederatedModel): a primary (initial) model that will be deep-copied for each coalition.
+       -------------
+         Returns
+            None"""
+        self.settings = settings
+        self.evaluation = settings['evaluation']
+        self.recorded_values = {} # Maps every coalition to it's value, implemented to decrease the complexity.
+        self.shapley_or_recon = None
+        
+        # Creates coalitions for Shapley, if so indicated in the settings.
+        if self.evaluation.get("Shapley_OR"):
+            self.shapley_values = {node:float(0) for node in settings['nodes']} # Final list (of Shapley evaluation)
+            self.shapley_or_recon = Subsets.form_superset(settings['nodes'], return_dict=False)
+            self.shapley_or_recon = {tuple(coalition) : deepcopy(model) for 
+                                     coalition in self.shapley_or_recon}
+        
+        # Creates coalition for Leave-one-out, if so indicated in the settings.
+        if self.evaluation.get("LOO_OR"):
+            self.loo_values = {node:float(0) for node in settings['nodes']} # Final list (of LOO evaluation)
+            if self.shapley_or_recon: # If we already have coalition for shapleys values, we can use model of those
+                self.loo_or_recon = {coalition: model for coalition, model in self.shapley_or_recon.items()
+                                     if len(coalition) >= (settings["number_of_nodes"] - 1)}
+            else:
+                self.loo_or_recon = Subsets.form_loo_set(settings['nodes'], return_dict=False) # Else we have to create a new one.
+                self.loo_or_recon = {tuple(coaliton) : deepcopy(model) for
+                                     coaliton in self.loo_or_recon}
+
+
+    def track_shapley(self,
+                      gradients: dict):
+        """A method that allows to collect gradients from the t-th round of the training and
+        update all the models in every coalition of interest.
+        
+        -------------
+        Args
+            gradients (dict): Dictionary mapping each node to its respective gradients.
+       -------------
+         Returns
+            None"""
+        
+        # Establishing gradients for all possible coalitions in N
+        delta_s = Subsets.form_superset(self.settings["nodes"], return_dict=True)
+        for coalition in delta_s:
+            specific_gradients = {}
+            for member in coalition:
+                specific_gradients[member] = gradients[member]
+            delta_s[coalition] = Aggregators.compute_average(specific_gradients)
+        
+        # Upadting models of all possible coalitions in N
+        for coalition in self.shapley_or_recon:
+            model_s_t = self.shapley_or_recon[coalition]
+            delta_s_t = delta_s[coalition]
+            updated_weights = Optimizers.SimpleFedopt(weights=model_s_t.get_weights(),
+                                                                       delta=delta_s_t,
+                                                                       learning_rate=0.99)
+            self.shapley_or_recon[coalition].update_weights(updated_weights)
+    
+
+    def track_loo(self,
+                   gradients: dict):
+        """A method that allows to collect gradients from the t-th round of the training and
+        update all the models in every coalition of interest. Note that it should be called
+        ONLY when we DO NOT track Shapley values. Otherwise, models used for LOO evaluation
+        will be a shallow copy of some of the models used for Shapley valuation and SHOULD NOT
+        be updated again.
+        
+        -------------
+        Args
+            gradients (dict): Dictionary mapping each node to its respective gradients.
+       -------------
+         Returns
+            None"""
+        
+        # Establishing gradients for all possible coalitions in N
+        delta_s = {coalition: float(0) for coalition in self.loo_or_recon.keys()}
+        for coalition in delta_s:
+            specific_gradients = {}
+            for member in coalition:
+                specific_gradients[member] = gradients[member]
+            delta_s[coalition] = Aggregators.compute_average(specific_gradients)
+        
+        # Upadting models of all possible coalitions in N
+        for coalition in self.loo_or_recon:
+            model_s_t = self.loo_or_recon[coalition]
+            delta_s_t = delta_s[coalition]
+            updated_weights = Optimizers.SimpleFedopt(weights=model_s_t.get_weights(),
+                                                      delta=delta_s_t,
+                                                      learning_rate=0.99)
+            self.loo_or_recon[coalition].update_weights(updated_weights)
+
+    def calculate_shaply(self):
+        """Calculates Shapley values.
+        -------------
+        Args
+            None
+       -------------
+         Returns
+            None"""
+        N = self.settings['number_of_nodes']
+        operation_counter = 1
+        number_of_operations = 2 ** N - 1
+        for node in self.shapley_values:
+            shapley_value = float(0)
+            subsets = Subsets.select_subsets(coalitions=self.shapley_or_recon,
+                                            searched_node=node)
+            for subset in subsets.keys():
+                subset_without_i = tuple(sorted(subset))
+                subset_with_i = tuple(sorted(subset + (node, )))
+
+                if subset_without_i in self.recorded_values:
+                    score_without_i = self.recorded_values[subset_without_i]
+                else:
+                    print(f"{operation_counter} of {number_of_operations}: forming and evaluating subset {subset_without_i}")
+                    model_without_i = self.shapley_or_recon[subset_without_i]
+                    score_without_i = model_without_i.evaluate_model()[1]
+                    self.recorded_values[subset_without_i] = score_without_i
+                    print(f"Coalition of {subset_without_i} scored {self.recorded_values[subset_without_i]}")
+                    operation_counter += 1
+
+                if subset_with_i in self.recorded_values:
+                    score_with_i = self.recorded_values[subset_with_i]
+                else:
+                    print(f"{operation_counter} of {number_of_operations}: forming and evaluating subset {subset_with_i}")
+                    model_with_i = self.shapley_or_recon[subset_with_i]
+                    score_with_i = model_with_i.evaluate_model()[1]
+                    self.recorded_values[subset_with_i] = score_with_i
+                    print(f"Coalition of {subset_with_i} scored {self.recorded_values[subset_with_i]}")
+                    operation_counter += 1
+                
+                summand = (score_with_i - score_without_i) /  math.comb((N-1), len(subset))
+                shapley_value += summand
+
+            # One last summand - empty set
+            score_without_i = float(0) # since v(empty_set) = 0
+            subset_with_i = (node, )
+            if subset_with_i in self.recorded_values:
+                    score_with_i = self.recorded_values[subset_with_i]
+            else:
+                print(f"{operation_counter} of {number_of_operations}: forming and evaluating subset {subset_with_i}")
+                model_with_i = self.shapley_or_recon[subset_with_i]
+                score_with_i = model_with_i.evaluate_model()[1]
+                self.recorded_values[subset_with_i] = score_with_i
+                print(f"Coalition of {subset_with_i} scored {self.recorded_values[subset_with_i]}")
+                operation_counter += 1
+            
+            summand = (score_with_i - score_without_i) /  math.comb((N-1), len(subset))
+            shapley_value += summand
+            
+            self.shapley_values[node] = (shapley_value / self.settings['number_of_nodes'])
+    
+
+    def calculate_loo(self):
+        """Calculates Leave-one-out values.
+        -------------
+        Args
+            None
+       -------------
+         Returns
+            None"""
+        
+        all_nodes = deepcopy(self.settings['nodes'])
+        general_subset = tuple(self.settings['nodes'])
+        if general_subset in self.recorded_values:
+            general_score = self.recorded_values[general_subset]
+        else:
+            print(f"Forming and evaluating subset {general_subset}")
+            general_model = self.loo_or_recon[general_subset]
+            general_score = general_model.evaluate_model()[1]
+            self.recorded_values[general_subset] = general_score
+        
+        for node in self.loo_values:
+            subset_without_i = deepcopy(all_nodes)
+            subset_without_i.remove(node)
+            subset_without_i = tuple(sorted(subset_without_i))
+            if subset_without_i in self.recorded_values:
+                score_without_i = self.recorded_values[subset_without_i]
+            else:
+                print(f"Forming and evaluating subset {subset_without_i}")
+                model_without_i = self.loo_or_recon[subset_without_i]
+                score_without_i = model_without_i.evaluate_model()[1]
+                self.recorded_values[subset_without_i] = score_without_i
+            
+            self.loo_values[node] = general_score - score_without_i
+
```

### Comparing `asociita-0.1.6.9/asociita/components/nodes/federated_node.py` & `asociita-0.1.7/asociita/components/nodes/federated_node.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-from typing import Any
-from datasets import arrow_dataset
-from asociita.models.pytorch.federated_model import FederatedModel
-from asociita.utils.loggers import Loggers
-
-node_logger = Loggers.node_logger()
-
-class FederatedNode:
-    def __init__(self, 
-                 node_id: int,
-                 settings: dict) -> None:
-        """An abstract object representing a single node in the federated training.
-        ------------
-        Arguments:
-            node_id (int): an int identifier of a node
-            settings (dict): a dictionary containing settings for the node
-        ------------
-        Returns:
-            None"""
-        self.state = 1 # Attribute controlling the state of the object.
-                         # 0 - initialized, resting
-                         # 1 - initialized, in run-time
-        
-        self.node_id = node_id
-        self.model = None
-        self.train_data = None
-        self.test_data = None
-        self.settings = settings
-        self.state = 0
-
-
-    def prepare_node(self, 
-                     model: Any, 
-                     data: arrow_dataset.Dataset):
-       """Prepares node for the training, given the passed model 
-       and dataset.
-       ------------
-       Arguments:
-            model (Any): compiled or pre-compiled model to be trained
-            dataset (list[datasets.arrow_dataset.Dataset, 
-                        datasets.arrow_dataset.Dataset]): a list[train_data, test_data]
-                        wrapped in a pre-compiled HuggingFace object.
-        ------------
-        Returns:
-            None"""
-       
-       self.state = 1
-       self.train_data = data[0]
-       self.test_data = data[1]
-       
-       self.model = FederatedModel(
-           settings=self.settings["model_settings"],
-           net = model,
-           local_dataset = data,
-           node_name=self.node_id
-       )
-
-       if self.model != None and self.train_data != None \
-        and self.test_data != None:
-           self.state = 0
-       else:
-           # TODO: LOGGING INFO
-           pass
-    
-
-    def train_local_model(
-        self,
-        mode: str
-    ) -> tuple[list[float], list[float], list[float]]:
-        """This function starts the server phase of the federated learning.
-        In particular, it trains the model locally and then sends the weights.
-        Then the updated weights are received and used to update
-        the local model.
-        -------------
-        Args:
-        node (FederatedNode object): Node that we want to train.
-        mode (str): Mode of the training. 
-            Mode = 'weights': Node will return model's weights.
-            Mode = 'gradients': Node will return model's gradients.
-        -------------
-        Returns:
-            Tuple[List[float], List[float], List[float]]: _description_
-        """
-        node_logger.info(f"Starting training on node {self.node_id}")
-        loss_list: list[float] = []
-        accuracy_list: list[float] = []
-
-        local_epochs = self.settings['local_epochs']
-
-        if mode == 'gradients':
-            self.model.preserve_initial_model()
-        
-        for _ in range(local_epochs):
-            metrics = self.local_training()
-            loss_list.append(metrics["loss"])
-            accuracy_list.append(metrics["accuracy"])
-        
-        node_logger.debug(f"Results of training on node {self.node_id}: {accuracy_list}")
-        if mode == 'weights:':
-            return (
-                self.node_id,
-                self.model.get_weights()
-                )
-        elif mode == 'gradients':
-            return (
-                self.node_id,
-                self.model.get_gradients()
-            )
-        else:
-            node_logger.warning("No mode was provided, returning only node's weights")
-            return (
-                self.node_id,
-                self.model.get_weights()
-                )
-
-    def local_training(
-        self,
-    ) -> dict[int, int]:
-        """Helper method for performing one epoch of local training.
-        Performs one round of Federated Training and pack the
-        results (metrics) into the appropiate data structure.
-        Args:
-            self
-        Returns
-        -------
-            dict[int, int]: metrics from the training.
-        """
-        loss, accuracy = self.model.train()
+from typing import Any
+from datasets import arrow_dataset
+from asociita.models.pytorch.federated_model import FederatedModel
+from asociita.utils.loggers import Loggers
+
+node_logger = Loggers.node_logger()
+
+class FederatedNode:
+    def __init__(self, 
+                 node_id: int,
+                 settings: dict) -> None:
+        """An abstract object representing a single node in the federated training.
+        ------------
+        Arguments:
+            node_id (int): an int identifier of a node
+            settings (dict): a dictionary containing settings for the node
+        ------------
+        Returns:
+            None"""
+        self.state = 1 # Attribute controlling the state of the object.
+                         # 0 - initialized, resting
+                         # 1 - initialized, in run-time
+        
+        self.node_id = node_id
+        self.model = None
+        self.train_data = None
+        self.test_data = None
+        self.settings = settings
+        self.state = 0
+
+
+    def prepare_node(self, 
+                     model: Any, 
+                     data: arrow_dataset.Dataset):
+       """Prepares node for the training, given the passed model 
+       and dataset.
+       ------------
+       Arguments:
+            model (Any): compiled or pre-compiled model to be trained
+            dataset (list[datasets.arrow_dataset.Dataset, 
+                        datasets.arrow_dataset.Dataset]): a list[train_data, test_data]
+                        wrapped in a pre-compiled HuggingFace object.
+        ------------
+        Returns:
+            None"""
+       
+       self.state = 1
+       self.train_data = data[0]
+       self.test_data = data[1]
+       
+       self.model = FederatedModel(
+           settings=self.settings["model_settings"],
+           net = model,
+           local_dataset = data,
+           node_name=self.node_id
+       )
+
+       if self.model != None and self.train_data != None \
+        and self.test_data != None:
+           self.state = 0
+       else:
+           # TODO: LOGGING INFO
+           pass
+    
+
+    def train_local_model(
+        self,
+        mode: str
+    ) -> tuple[list[float], list[float], list[float]]:
+        """This function starts the server phase of the federated learning.
+        In particular, it trains the model locally and then sends the weights.
+        Then the updated weights are received and used to update
+        the local model.
+        -------------
+        Args:
+        node (FederatedNode object): Node that we want to train.
+        mode (str): Mode of the training. 
+            Mode = 'weights': Node will return model's weights.
+            Mode = 'gradients': Node will return model's gradients.
+        -------------
+        Returns:
+            Tuple[List[float], List[float], List[float]]: _description_
+        """
+        node_logger.info(f"Starting training on node {self.node_id}")
+        loss_list: list[float] = []
+        accuracy_list: list[float] = []
+
+        local_epochs = self.settings['local_epochs']
+
+        if mode == 'gradients':
+            self.model.preserve_initial_model()
+        
+        for _ in range(local_epochs):
+            metrics = self.local_training()
+            loss_list.append(metrics["loss"])
+            accuracy_list.append(metrics["accuracy"])
+        
+        node_logger.debug(f"Results of training on node {self.node_id}: {accuracy_list}")
+        if mode == 'weights:':
+            return (
+                self.node_id,
+                self.model.get_weights()
+                )
+        elif mode == 'gradients':
+            return (
+                self.node_id,
+                self.model.get_gradients()
+            )
+        else:
+            node_logger.warning("No mode was provided, returning only model's weights")
+            return (
+                self.node_id,
+                self.model.get_weights()
+                )
+
+    def local_training(
+        self,
+    ) -> dict[int, int]:
+        """Helper method for performing one epoch of local training.
+        Performs one round of Federated Training and pack the
+        results (metrics) into the appropiate data structure.
+        Args:
+            self
+        Returns
+        -------
+            dict[int, int]: metrics from the training.
+        """
+        loss, accuracy = self.model.train()
         return {"loss": loss, "accuracy": accuracy}
```

### Comparing `asociita-0.1.6.9/asociita/components/orchestrator/evaluator_orchestrator.py` & `asociita-0.1.7/asociita/components/orchestrator/evaluator_orchestrator.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-# PARENT CLASS IMPORT
-from asociita.components.orchestrator.generic_orchestrator import Orchestrator # Parent class import
-# LIBRARY MODULES IMPORT
-from asociita.utils.orchestrations import create_nodes, sample_nodes, train_nodes
-from asociita.utils.computations import Aggregators
-from asociita.utils.handlers import Handler
-from asociita.utils.loggers import Loggers
-from asociita.utils.orchestrations import create_nodes, sample_nodes, train_nodes
-from asociita.utils.optimizers import Optimizers
-from asociita.components.evaluator.evaluation_manager import Evaluation_Manager
-from asociita.components.archiver.archive_manager import Archive_Manager
-# ADDITIONAL IMPORTS
-import datasets, copy
-from multiprocessing import Pool, Manager
-
-
-orchestrator_logger = Loggers.orchestrator_logger()
-
-
-class Evaluator_Orchestrator(Orchestrator):
-    def __init__(self, settings: dict) -> None:
-        """Orchestrator is a central object necessary for performing the simulation.
-        It connects the nodes, maintain the knowledge about their state and manages the
-        multithread pool. generic_orchestrator.orchestrator is a parent to all more
-        specific orchestrators. Evaluator_Orchestrator additionally performs a 
-        evaluation of the clients contribution, according to the passed settings.
-        
-        -------------
-        Args
-            settings (dict): dictionary object cotaining all the settings of the orchestrator.
-       -------------
-         Returns
-            None"""
-        super().__init__(settings)
-    
-
-    def train_protocol(self,
-                nodes_data: list[datasets.arrow_dataset.Dataset, 
-                datasets.arrow_dataset.Dataset]) -> None:
-        """"Performs a full federated training according to the initialized
-        settings. The train_protocol of the fedopt.orchestrator.Fedopt_Orchestrator
-        follows a popular FedAvg generalisation, FedOpt. Instead of weights from each
-        clients, it aggregates gradients (understood as a difference between the weights
-        of a model after all t epochs of the local training) and aggregates according to 
-        provided rule.
-        SOURCE: Adaptive Federated Optimization, S.J. Reddi et al.
-
-        -------------
-        Args:
-            nodes_data(list[..., ....]): list containing train set and test set
-                wrapped in a hugging facr arrow_dataset.Dataset containers.
-        -------------
-        Returns:
-            None"""
-        
-        # 1. SETTINGS -> CHANGE IF NEEDED
-        # GENERAL SETTINGS
-        iterations = self.settings['iterations'] # Number of iterations of the Fed training, int.
-        nodes_number = self.settings['number_of_nodes'] # Number of nodes prepared for sampling, int.
-        local_warm_start = self.settings["local_warm_start"] # Local warm start for pre-trained models - not implemented yet.
-        nodes = self.settings["nodes"] # List of nodes, list[int]
-        sample_size = self.settings["sample_size"] # Size of the sample, int.
-        # OPTIMIZER SETTINGS
-        optimizer_settings = self.settings["optimizer"] # Dict containing instructions for the optimizer, dict.
-        optimizer_name = optimizer_settings["name"] # Name of the optimizer, e.g. FedAdagard, dict.
-        
-
-        # 2. SET-UP PHASE -> CHANGE IF NEEDED
-        # SETTING-UP EVALUATION MANAGER
-        evaluation_maanger = Evaluation_Manager(settings=self.settings,
-                                                model=self.central_model)
-        archive_manager = Archive_Manager(archive_manager = self.settings['archiver'],
-                                          logger = orchestrator_logger)
-        self.metrics_save_path = self.settings['metrics_save_path']
-
-        # CREATING FEDERATED NODES
-        nodes_green = create_nodes(nodes, self.node_settings)
-        # CREATING LOCAL MODELS (that will be loaded onto nodes)
-        model_list = self.model_initialization(nodes_number=nodes_number,
-                                               model=self.central_net)
-        # INITIALIZING ALL THE NODES
-        nodes_green = self.nodes_initialization(nodes_list=nodes_green,
-                                                model_list=model_list,
-                                                data_list=nodes_data,
-                                                nodes_number=nodes_number)
-        # SETTING UP THE OPTIMIZER
-        Optim = Optimizers(weights = self.central_model.get_weights())
-
-
-        # 3. TRAINING PHASE ----- FEDOPT
-        with Manager() as manager:
-            # create the shared queue
-            queue = manager.Queue()
-            # create the pool of workers
-            with Pool(sample_size) as pool:
-                for iteration in range(iterations):
-                    orchestrator_logger.info(f"Iteration {iteration}")
-                    gradients = {}
-                    # Sampling nodes and asynchronously apply the function
-                    sampled_nodes = sample_nodes(nodes_green, 
-                                                 sample_size=sample_size,
-                                                 orchestrator_logger=orchestrator_logger) # SAMPLING FUNCTION -> CHANGE IF NEEDED
-                    results = [pool.apply_async(train_nodes, (node, 'gradients')) for node in sampled_nodes]
-                    # consume the results
-                    for result in results:
-                        node_id, model_gradients = result.get()
-                        gradients[node_id] = copy.deepcopy(model_gradients)
-                    
-                    # Computing the average of gradients
-                    grad_avg = Aggregators.compute_average(gradients) # AGGREGATING FUNCTION -> CHANGE IF NEEDED
-                    updated_weights = Optim.fed_optimize(optimizer=optimizer_name,
-                                                         settings=optimizer_settings,
-                                                         weights=self.central_model.get_weights(),
-                                                         delta=grad_avg)
-                    # TRACKING GRADIENTS FOR EVALUATION
-                    evaluation_maanger.track_gradients(gradients=gradients) # TRACKING FUNCTION -> CHANGE IF NEEDED
-                    ### WEIGHTS UPDATE
-                    # Updating the nodes
-                    for node in nodes_green:
-                        node.model.update_weights(updated_weights)
-                    # Upadting the orchestrator
-                    self.central_model.update_weights(updated_weights)                 
-                    archive_manager.archive_training_results(iteration = iteration,
-                                                             central_model=self.central_model,
-                                                             nodes=nodes_green)
-        # 4. FINALIZING PHASE
-        # EVALUATING THE RESULTS
-        evaluation_results, mapped_results = evaluation_maanger.calculate_results()
-        
-        # FINAL MESSAGES
-        print(evaluation_results)
-        print(mapped_results)
-        evaluation_maanger.save_results(path = self.metrics_save_path,
-                                        mapped_results=mapped_results)
+# PARENT CLASS IMPORT
+from asociita.components.orchestrator.generic_orchestrator import Orchestrator # Parent class import
+# LIBRARY MODULES IMPORT
+from asociita.utils.orchestrations import create_nodes, sample_nodes, train_nodes
+from asociita.utils.computations import Aggregators
+from asociita.utils.handlers import Handler
+from asociita.utils.loggers import Loggers
+from asociita.utils.orchestrations import create_nodes, sample_nodes, train_nodes
+from asociita.utils.optimizers import Optimizers
+from asociita.components.evaluator.evaluation_manager import Evaluation_Manager
+from asociita.components.archiver.archive_manager import Archive_Manager
+# ADDITIONAL IMPORTS
+import datasets, copy
+from multiprocessing import Pool, Manager
+
+
+orchestrator_logger = Loggers.orchestrator_logger()
+
+
+class Evaluator_Orchestrator(Orchestrator):
+    def __init__(self, settings: dict) -> None:
+        """Orchestrator is a central object necessary for performing the simulation.
+        It connects the nodes, maintain the knowledge about their state and manages the
+        multithread pool. generic_orchestrator.orchestrator is a parent to all more
+        specific orchestrators. Evaluator_Orchestrator additionally performs a 
+        evaluation of the clients contribution, according to the passed settings.
+        
+        -------------
+        Args
+            settings (dict): dictionary object cotaining all the settings of the orchestrator.
+       -------------
+         Returns
+            None"""
+        super().__init__(settings)
+    
+
+    def train_protocol(self,
+                nodes_data: list[datasets.arrow_dataset.Dataset, 
+                datasets.arrow_dataset.Dataset]) -> None:
+        """"Performs a full federated training according to the initialized
+        settings. The train_protocol of the fedopt.orchestrator.Fedopt_Orchestrator
+        follows a popular FedAvg generalisation, FedOpt. Instead of weights from each
+        clients, it aggregates gradients (understood as a difference between the weights
+        of a model after all t epochs of the local training) and aggregates according to 
+        provided rule.
+        SOURCE: Adaptive Federated Optimization, S.J. Reddi et al.
+
+        -------------
+        Args:
+            nodes_data(list[..., ....]): list containing train set and test set
+                wrapped in a hugging facr arrow_dataset.Dataset containers.
+        -------------
+        Returns:
+            None"""
+        
+        # 1. SETTINGS -> CHANGE IF NEEDED
+        # GENERAL SETTINGS
+        iterations = self.settings['iterations'] # Number of iterations of the Fed training, int.
+        nodes_number = self.settings['number_of_nodes'] # Number of nodes prepared for sampling, int.
+        local_warm_start = self.settings["local_warm_start"] # Local warm start for pre-trained models - not implemented yet.
+        nodes = self.settings["nodes"] # List of nodes, list[int]
+        sample_size = self.settings["sample_size"] # Size of the sample, int.
+        # OPTIMIZER SETTINGS
+        optimizer_settings = self.settings["optimizer"] # Dict containing instructions for the optimizer, dict.
+        optimizer_name = optimizer_settings["name"] # Name of the optimizer, e.g. FedAdagard, dict.
+        
+
+        # 2. SET-UP PHASE -> CHANGE IF NEEDED
+        # SETTING-UP EVALUATION MANAGER
+        evaluation_maanger = Evaluation_Manager(settings=self.settings,
+                                                model=self.central_model)
+        archive_manager = Archive_Manager(archive_manager = self.settings['archiver'],
+                                          logger = orchestrator_logger)
+        self.metrics_save_path = self.settings['metrics_save_path']
+
+        # CREATING FEDERATED NODES
+        nodes_green = create_nodes(nodes, self.node_settings)
+        # CREATING LOCAL MODELS (that will be loaded onto nodes)
+        model_list = self.model_initialization(nodes_number=nodes_number,
+                                               model=self.central_net)
+        # INITIALIZING ALL THE NODES
+        nodes_green = self.nodes_initialization(nodes_list=nodes_green,
+                                                model_list=model_list,
+                                                data_list=nodes_data,
+                                                nodes_number=nodes_number)
+        # SETTING UP THE OPTIMIZER
+        Optim = Optimizers(weights = self.central_model.get_weights())
+
+
+        # 3. TRAINING PHASE ----- FEDOPT
+        with Manager() as manager:
+            # create the shared queue
+            queue = manager.Queue()
+            # create the pool of workers
+            with Pool(sample_size) as pool:
+                for iteration in range(iterations):
+                    orchestrator_logger.info(f"Iteration {iteration}")
+                    gradients = {}
+                    # Sampling nodes and asynchronously apply the function
+                    sampled_nodes = sample_nodes(nodes_green, 
+                                                 sample_size=sample_size,
+                                                 orchestrator_logger=orchestrator_logger) # SAMPLING FUNCTION -> CHANGE IF NEEDED
+                    results = [pool.apply_async(train_nodes, (node, 'gradients')) for node in sampled_nodes]
+                    # consume the results
+                    for result in results:
+                        node_id, model_gradients = result.get()
+                        gradients[node_id] = copy.deepcopy(model_gradients)
+                    
+                    # Computing the average of gradients
+                    grad_avg = Aggregators.compute_average(gradients) # AGGREGATING FUNCTION -> CHANGE IF NEEDED
+                    updated_weights = Optim.fed_optimize(optimizer=optimizer_name,
+                                                         settings=optimizer_settings,
+                                                         weights=self.central_model.get_weights(),
+                                                         delta=grad_avg)
+                    # TRACKING GRADIENTS FOR EVALUATION
+                    evaluation_maanger.track_gradients(gradients=gradients) # TRACKING FUNCTION -> CHANGE IF NEEDED
+                    ### WEIGHTS UPDATE
+                    # Updating the nodes
+                    for node in nodes_green:
+                        node.model.update_weights(updated_weights)
+                    # Upadting the orchestrator
+                    self.central_model.update_weights(updated_weights)                 
+                    archive_manager.archive_training_results(iteration = iteration,
+                                                             central_model=self.central_model,
+                                                             nodes=nodes_green)
+        # 4. FINALIZING PHASE
+        # EVALUATING THE RESULTS
+        evaluation_results, mapped_results = evaluation_maanger.calculate_results()
+        
+        # FINAL MESSAGES
+        print(evaluation_results)
+        print(mapped_results)
+        evaluation_maanger.save_results(path = self.metrics_save_path,
+                                        mapped_results=mapped_results)
         orchestrator_logger.critical("Training complete")
```

### Comparing `asociita-0.1.6.9/asociita/components/orchestrator/fedopt_orchestrator.py` & `asociita-0.1.7/asociita/components/orchestrator/fedopt_orchestrator.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-from asociita.components.orchestrator.generic_orchestrator import Orchestrator # Parent class import
-import datasets, copy
-from typing import Any, Union
-from asociita.components.nodes.federated_node import FederatedNode
-from asociita.models.pytorch.federated_model import FederatedModel
-from asociita.utils.computations import Aggregators
-from asociita.utils.handlers import Handler
-from asociita.utils.loggers import Loggers
-from asociita.utils.orchestrations import prepare_nodes, create_nodes, check_health, sample_nodes, train_nodes
-from asociita.utils.optimizers import Optimizers
-from asociita.components.archiver.archive_manager import Archive_Manager
-from multiprocessing import Pool, Manager
-from torch import nn
-
-orchestrator_logger = Loggers.orchestrator_logger()
-
-
-class Fedopt_Orchestrator(Orchestrator):
-    def __init__(self, settings: dict) -> None:
-        """Orchestrator is a central object necessary for performing the simulation.
-        It connects the nodes, maintain the knowledge about their state and manages the
-        multithread pool. generic_orchestrator.orchestrator is a parent to all more
-        specific orchestrators.
-        
-        -------------
-        Args
-            settings (dict): dictionary object cotaining all the settings of the orchestrator.
-       -------------
-         Returns
-            None"""
-        super().__init__(settings)
-    
-
-    def train_protocol(self,
-                nodes_data: list[datasets.arrow_dataset.Dataset, 
-                datasets.arrow_dataset.Dataset]) -> None:
-        """"Performs a full federated training according to the initialized
-        settings. The train_protocol of the fedopt.orchestrator.Fedopt_Orchestrator
-        follows a popular FedAvg generalisation, FedOpt. Instead of weights from each
-        clients, it aggregates gradients (understood as a difference between the weights
-        of a model after all t epochs of the local training) and aggregates according to 
-        provided rule.
-        SOURCE: Adaptive Federated Optimization, S.J. Reddi et al.
-
-        -------------
-        Args:
-            nodes_data(list[..., ....]): list containing train set and test set
-                wrapped in a hugging facr arrow_dataset.Dataset containers.
-        -------------
-        Returns:
-            None"""
-        
-        # SETTINGS -> CHANGE IF NEEDED
-        # GENERAL SETTINGS
-        iterations = self.settings['iterations']
-        nodes_number = self.settings['number_of_nodes']
-        local_warm_start = self.settings["local_warm_start"]
-        nodes = self.settings["nodes"]
-        sample_size = self.settings["sample_size"]
-        archive_manager = Archive_Manager(archive_manager = self.settings['archiver'],
-                                          logger = orchestrator_logger)
-
-        # OPTIMIZER SETTINGS
-        optimizer_settings = self.settings["optimizer"]
-        optimizer_name = optimizer_settings["name"]
-        
-        # CREATING FEDERATED NODES
-        nodes_green = create_nodes(nodes, self.node_settings) # Exterior method / function, can override in childr.
-
-
-        # CREATING LOCAL MODELS (that will be loaded onto nodes)
-        model_list = self.model_initialization(nodes_number=nodes_number,
-                                               model=self.central_net) # Exterior method / function, can overide in childr.
-        
-        # INITIALIZING ALL THE NODES
-        nodes_green = self.nodes_initialization(nodes_list=nodes_green, # Exterion method / function, can overide in child.
-                                                model_list=model_list,
-                                                data_list=nodes_data,
-                                                nodes_number=nodes_number)
-        
-        Optim = Optimizers(weights = self.central_model.get_weights()) # Setting up the Optim.
-        
-        # TRAINING PHASE ----- FEDOPT
-        with Manager() as manager:
-            # create the shared queue
-            queue = manager.Queue()
-
-            # create the pool of workers
-            with Pool(sample_size) as pool:
-                for iteration in range(iterations):
-                    orchestrator_logger.info(f"Iteration {iteration}")
-                    gradients = {}
-                    
-                    # Sampling nodes and asynchronously apply the function
-                    sampled_nodes = sample_nodes(nodes_green, 
-                                                 sample_size=sample_size,
-                                                 orchestrator_logger=orchestrator_logger) # SAMPLING FUNCTION -> CHANGE IF NEEDED
-                    results = [pool.apply_async(train_nodes, (node, 'gradients')) for node in sampled_nodes]
-                    # consume the results
-                    for result in results:
-                        node_id, model_gradients = result.get()
-                        gradients[node_id] = copy.deepcopy(model_gradients)
-                    
-                    # Computing the average of gradients
-                    grad_avg = Aggregators.compute_average(gradients) # AGGREGATING FUNCTION -> CHANGE IF NEEDED
-                    updated_weights = Optim.fed_optimize(optimizer=optimizer_name,
-                                                         settings=optimizer_settings,
-                                                         weights=self.central_model.get_weights(),
-                                                         delta=grad_avg)
-                    # Updating the nodes
-                    for node in nodes_green:
-                        node.model.update_weights(updated_weights)
-                    # Upadting the orchestrator
-                    self.central_model.update_weights(updated_weights)
-
-                    archive_manager.archive_training_results(iteration = iteration,
-                                                             central_model=self.central_model,
-                                                             nodes=nodes_green)
-        
+from asociita.components.orchestrator.generic_orchestrator import Orchestrator # Parent class import
+import datasets, copy
+from typing import Any, Union
+from asociita.components.nodes.federated_node import FederatedNode
+from asociita.models.pytorch.federated_model import FederatedModel
+from asociita.utils.computations import Aggregators
+from asociita.utils.handlers import Handler
+from asociita.utils.loggers import Loggers
+from asociita.utils.orchestrations import prepare_nodes, create_nodes, check_health, sample_nodes, train_nodes
+from asociita.utils.optimizers import Optimizers
+from asociita.components.archiver.archive_manager import Archive_Manager
+from multiprocessing import Pool, Manager
+from torch import nn
+
+orchestrator_logger = Loggers.orchestrator_logger()
+
+
+class Fedopt_Orchestrator(Orchestrator):
+    def __init__(self, settings: dict) -> None:
+        """Orchestrator is a central object necessary for performing the simulation.
+        It connects the nodes, maintain the knowledge about their state and manages the
+        multithread pool. generic_orchestrator.orchestrator is a parent to all more
+        specific orchestrators.
+        
+        -------------
+        Args
+            settings (dict): dictionary object cotaining all the settings of the orchestrator.
+       -------------
+         Returns
+            None"""
+        super().__init__(settings)
+    
+
+    def train_protocol(self,
+                nodes_data: list[datasets.arrow_dataset.Dataset, 
+                datasets.arrow_dataset.Dataset]) -> None:
+        """"Performs a full federated training according to the initialized
+        settings. The train_protocol of the fedopt.orchestrator.Fedopt_Orchestrator
+        follows a popular FedAvg generalisation, FedOpt. Instead of weights from each
+        clients, it aggregates gradients (understood as a difference between the weights
+        of a model after all t epochs of the local training) and aggregates according to 
+        provided rule.
+        SOURCE: Adaptive Federated Optimization, S.J. Reddi et al.
+
+        -------------
+        Args:
+            nodes_data(list[..., ....]): list containing train set and test set
+                wrapped in a hugging facr arrow_dataset.Dataset containers.
+        -------------
+        Returns:
+            None"""
+        
+        # SETTINGS -> CHANGE IF NEEDED
+        # GENERAL SETTINGS
+        iterations = self.settings['iterations']
+        nodes_number = self.settings['number_of_nodes']
+        local_warm_start = self.settings["local_warm_start"]
+        nodes = self.settings["nodes"]
+        sample_size = self.settings["sample_size"]
+        archive_manager = Archive_Manager(archive_manager = self.settings['archiver'],
+                                          logger = orchestrator_logger)
+
+        # OPTIMIZER SETTINGS
+        optimizer_settings = self.settings["optimizer"]
+        optimizer_name = optimizer_settings["name"]
+        
+        # CREATING FEDERATED NODES
+        nodes_green = create_nodes(nodes, self.node_settings) # Exterior method / function, can override in childr.
+
+
+        # CREATING LOCAL MODELS (that will be loaded onto nodes)
+        model_list = self.model_initialization(nodes_number=nodes_number,
+                                               model=self.central_net) # Exterior method / function, can overide in childr.
+        
+        # INITIALIZING ALL THE NODES
+        nodes_green = self.nodes_initialization(nodes_list=nodes_green, # Exterion method / function, can overide in child.
+                                                model_list=model_list,
+                                                data_list=nodes_data,
+                                                nodes_number=nodes_number)
+        
+        Optim = Optimizers(weights = self.central_model.get_weights()) # Setting up the Optim.
+        
+        # TRAINING PHASE ----- FEDOPT
+        with Manager() as manager:
+            # create the shared queue
+            queue = manager.Queue()
+
+            # create the pool of workers
+            with Pool(sample_size) as pool:
+                for iteration in range(iterations):
+                    orchestrator_logger.info(f"Iteration {iteration}")
+                    gradients = {}
+                    
+                    # Sampling nodes and asynchronously apply the function
+                    sampled_nodes = sample_nodes(nodes_green, 
+                                                 sample_size=sample_size,
+                                                 orchestrator_logger=orchestrator_logger) # SAMPLING FUNCTION -> CHANGE IF NEEDED
+                    results = [pool.apply_async(train_nodes, (node, 'gradients')) for node in sampled_nodes]
+                    # consume the results
+                    for result in results:
+                        node_id, model_gradients = result.get()
+                        gradients[node_id] = copy.deepcopy(model_gradients)
+                    
+                    # Computing the average of gradients
+                    grad_avg = Aggregators.compute_average(gradients) # AGGREGATING FUNCTION -> CHANGE IF NEEDED
+                    updated_weights = Optim.fed_optimize(optimizer=optimizer_name,
+                                                         settings=optimizer_settings,
+                                                         weights=self.central_model.get_weights(),
+                                                         delta=grad_avg)
+                    # Updating the nodes
+                    for node in nodes_green:
+                        node.model.update_weights(updated_weights)
+                    # Upadting the orchestrator
+                    self.central_model.update_weights(updated_weights)
+
+                    archive_manager.archive_training_results(iteration = iteration,
+                                                             central_model=self.central_model,
+                                                             nodes=nodes_green)
+        
         orchestrator_logger.critical("Training complete")
```

### Comparing `asociita-0.1.6.9/asociita/components/orchestrator/generic_orchestrator.py` & `asociita-0.1.7/asociita/components/orchestrator/generic_orchestrator.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,231 +1,231 @@
-import datasets, copy
-from typing import Any, Union
-from asociita.components.nodes.federated_node import FederatedNode
-from asociita.models.pytorch.federated_model import FederatedModel
-from asociita.utils.computations import Aggregators
-from asociita.utils.handlers import Handler
-from asociita.utils.loggers import Loggers
-from asociita.utils.orchestrations import prepare_nodes, create_nodes, check_health, sample_nodes, train_nodes
-from asociita.components.archiver.archive_manager import Archive_Manager
-from multiprocessing import Pool, Manager
-from torch import nn
-
-
-orchestrator_logger = Loggers.orchestrator_logger()
-from multiprocessing import set_start_method
-set_start_method("spawn", force=True)
-
-class Orchestrator():
-    def __init__(self, 
-                 settings: dict) -> None:
-        """Orchestrator is a central object necessary for performing the simulation.
-        It connects the nodes, maintain the knowledge about their state and manages the
-        multithread pool. generic_orchestrator.orchestrator is a parent to all more
-        specific orchestrators.
-        
-        -------------
-        Args
-            settings (dict): dictionary object cotaining all the settings of the orchestrator.
-       -------------
-         Returns
-            None"""
-        self.settings = settings["orchestrator"] # Settings attribute (dict)
-        self.node_settings = settings["nodes"]
-        self.model = None
-        if self.settings.get('training_metrics'):
-            self.training_metrics_filename = self.settings['training_metrics']
-        else:
-            self.training_metrics_filename = 'training_metrics.csv'
-        if self.settings.get('nodes_metrics'):
-            self.nodes_metrics_filename = self.settings['nodes_metrics']
-        else:
-            self.nodes_metrics_filename = 'nodes_metrics.csv'
-    
-
-    def prepare_orchestrator(self, 
-                             model: Any,
-                             validation_data: datasets.arrow_dataset.Dataset,
-                             ) -> None:
-        """Loads the global model and validation data that will be used by the Orchestrator.
-        
-        -------------
-        Args
-        validation_data (datasets.arrow_dataset.Dataset): 
-            Validation dataset that will be used by the Orchestrator.
-        model (Any): Compiled or pre-compiled model that will 
-            be used by the instance of the class.
-        -------------
-        Returns
-            None"""
-        self.validation_data = [validation_data]
-        self.central_net = model
-        self.central_model = FederatedModel(settings = self.node_settings["model_settings"],
-                                        net=model,
-                                        local_dataset=self.validation_data,
-                                        node_name='orchestrator')
-    
-
-    def model_initialization(self,
-                             nodes_number: int,
-                             model: Union[nn.Module, list[nn.Module]],
-                             local_warm_start: bool = False,
-                             ) -> list[nn.Module]:
-        """Creates a list of neural nets (not FederatedModels!) that will be
-        passed onto the nodes and converted into FederatedModels. If local_warm_start
-        is set to True, the method call should be passed a list of models which
-        length is equall to the number of nodes.
-        
-        -------------
-        Args:
-            nodes_number (int): number of nodes that will participate in the
-                training.
-            model (Union[nn.Module, list]): a neural net schematic (if warm
-                start is set to False) or a number of different neural net schematics
-                (if warm start is set to True) that will prepared for the nodes to be
-                loaded as FederatedModels.
-            local_warm_start (bool): A boolean value for switching on/off the warm start
-                utility.
-        -------------
-        Returns:
-            tuple(node_id: str, weights)
-        """
-        if local_warm_start == True:
-            raise("Beginning the training with different local models not implemented yet.")
-        else:
-            model_list = [copy.deepcopy(model) for _ in range(nodes_number)]
-
-        return model_list
-
-
-    def nodes_initialization(self,
-                             nodes_list: list[FederatedNode],
-                             model_list: list[nn.Module],
-                             data_list: list[datasets.arrow_dataset.Dataset, 
-                                    datasets.arrow_dataset.Dataset],
-                             nodes_number: int) -> list[FederatedNode]:
-        """Prepare instances of a FederatedNode object for a participation in 
-        the Federated Training.  Contrary to the  create nodes function, 
-        it accepts only already initialized instances of the FederatedNode
-        object.
-        
-        -------------
-        Args:
-            nodess_list (list[FederatedNode]): list containing all the initialized
-                FederatedNode instances.
-            model_list (list[nn.Module]): list containing all the initialized 
-                nn.Module objects. Note that conversion from nn.Module into the
-                FederatedModel will occur at the local node level.
-            data_list (list[..., ....]): list containing train set and test set
-                wrapped in a hugging facr arrow_dataset.Dataset containers.
-            nodes_number (int): Number of nodes that will participate in the training.
-        -------------
-        Returns:
-            list[FederatedNode]"""
-        
-        results = []
-        for node, model, dataset in zip(nodes_list, model_list, data_list):
-            node.prepare_node(model, dataset)
-            results.append(node)
-        nodes_green = []
-        for result in results:
-            if check_health(result,
-                            orchestrator_logger=orchestrator_logger):
-                nodes_green.append(result)
-        return nodes_green # Returning initialized nodes
-
-        
-        # # create the manager
-        # with Manager() as manager:
-        #     # create the shared queue
-        #     queue = manager.Queue()
-        #     # create a pool of workers
-        #     with Pool(nodes_number) as pool:
-        #         # asynchronously apply the function
-        #         results = [
-        #             pool.apply_async(prepare_nodes, (node, model, dataset, queue))
-        #             for node, model, dataset in zip(nodes_list, model_list, data_list)
-        #         ]
-        #         # consume the results
-        #         # Define a list of healthy nodes
-        #         nodes_green = []
-        #         for result in results:
-        #             # query for results
-        #             _ = result.get()
-        #             updated_node = queue.get()
-        #             # Adds to list only if the node is healthy
-        #             if check_health(updated_node,
-        #                             orchestrator_logger=orchestrator_logger):
-        #                 nodes_green.append(updated_node)
-        # return nodes_green # Returning initialized nodes
-
-    def train_protocol(self,
-                nodes_data: list[datasets.arrow_dataset.Dataset, 
-                datasets.arrow_dataset.Dataset]) -> None:
-        """Performs a full federated training according to the initialized
-        settings. The train_protocol of the generic_orchestrator.Orchestrator
-        follows a classic FedAvg algorithm - it averages the local weights
-        and aggregates them taking a weighted average.
-        SOURCE: Communication-Efficient Learning of Deep Networks from Decentralized Data, H.B. McMahan et al.
-
-        -------------
-        Args:
-            nodes_data(list[..., ....]): list containing train set and test set
-                wrapped in a hugging facr arrow_dataset.Dataset containers.
-        -------------
-        Returns:
-            None"""
-        
-        # SETTINGS -> CHANGE IF NEEDED
-        iterations = self.settings['iterations']
-        nodes_number = self.settings['number_of_nodes']
-        local_warm_start = self.settings["local_warm_start"]
-        nodes = self.settings["nodes"]
-        sample_size = self.settings["sample_size"]
-        archive_manager = Archive_Manager(archive_manager = self.settings['archiver'],
-                                          logger = orchestrator_logger)
-
-        # CREATING FEDERATED NODES
-        nodes_green = create_nodes(nodes, self.node_settings) # Exterior method / function, can override in childr.
-
-
-        # CREATING LOCAL MODELS (that will be loaded onto nodes)
-        model_list = self.model_initialization(nodes_number=nodes_number,
-                                               model=self.central_net) # Exterior method / function, can overide in childr.
-        
-        # INITIALIZING ALL THE NODES
-        nodes_green = self.nodes_initialization(nodes_list=nodes_green, # Exterion method / function, can overide in child.
-                                                model_list=model_list,
-                                                data_list=nodes_data,
-                                                nodes_number=nodes_number)
-            
-        # TRAINING PHASE ----- FEDAVG
-        with Manager() as manager:
-            queue = manager.Queue() # creates a shared queue
-            # create the pool of workers
-            with Pool(sample_size) as pool: 
-                for iteration in range(iterations):
-                    orchestrator_logger.info(f"Iteration {iteration}")
-                    weights = {}
-                    # Sampling nodes and asynchronously apply the function
-                    sampled_nodes = sample_nodes(nodes_green, 
-                                                 sample_size=sample_size, 
-                                                 orchestrator_logger=orchestrator_logger) # SAMPLING FUNCTION -> CHANGE IF NEEDED
-                    results = [pool.apply_async(train_nodes, (node,)) for node in sampled_nodes]
-                    # consume the results
-                    for result in results:
-                        node_id, model_weights = result.get()
-                        weights[node_id] = copy.deepcopy(model_weights)
-                    # Computing the average
-                    avg = Aggregators.compute_average(weights) # AGGREGATING FUNCTION -> CHANGE IF NEEDED
-                    # Updating the nodes
-                    for node in nodes_green:
-                        node.model.update_weights(avg)
-                    # Upadting the orchestrator
-                    self.central_model.update_weights(avg)
-
-                    archive_manager.archive_training_results(iteration = iteration,
-                                                             central_model=self.central_model,
-                                                             nodes=nodes_green)
-
-        orchestrator_logger.critical("Training complete")
-                    
+import datasets, copy
+from typing import Any, Union
+from asociita.components.nodes.federated_node import FederatedNode
+from asociita.models.pytorch.federated_model import FederatedModel
+from asociita.utils.computations import Aggregators
+from asociita.utils.handlers import Handler
+from asociita.utils.loggers import Loggers
+from asociita.utils.orchestrations import prepare_nodes, create_nodes, check_health, sample_nodes, train_nodes
+from asociita.components.archiver.archive_manager import Archive_Manager
+from multiprocessing import Pool, Manager
+from torch import nn
+
+
+orchestrator_logger = Loggers.orchestrator_logger()
+from multiprocessing import set_start_method
+set_start_method("spawn", force=True)
+
+class Orchestrator():
+    def __init__(self, 
+                 settings: dict) -> None:
+        """Orchestrator is a central object necessary for performing the simulation.
+        It connects the nodes, maintain the knowledge about their state and manages the
+        multithread pool. generic_orchestrator.orchestrator is a parent to all more
+        specific orchestrators.
+        
+        -------------
+        Args
+            settings (dict): dictionary object cotaining all the settings of the orchestrator.
+       -------------
+         Returns
+            None"""
+        self.settings = settings["orchestrator"] # Settings attribute (dict)
+        self.node_settings = settings["nodes"]
+        self.model = None
+        if self.settings.get('training_metrics'):
+            self.training_metrics_filename = self.settings['training_metrics']
+        else:
+            self.training_metrics_filename = 'training_metrics.csv'
+        if self.settings.get('nodes_metrics'):
+            self.nodes_metrics_filename = self.settings['nodes_metrics']
+        else:
+            self.nodes_metrics_filename = 'nodes_metrics.csv'
+    
+
+    def prepare_orchestrator(self, 
+                             model: Any,
+                             validation_data: datasets.arrow_dataset.Dataset,
+                             ) -> None:
+        """Loads the global model and validation data that will be used by the Orchestrator.
+        
+        -------------
+        Args
+        validation_data (datasets.arrow_dataset.Dataset): 
+            Validation dataset that will be used by the Orchestrator.
+        model (Any): Compiled or pre-compiled model that will 
+            be used by the instance of the class.
+        -------------
+        Returns
+            None"""
+        self.validation_data = [validation_data]
+        self.central_net = model
+        self.central_model = FederatedModel(settings = self.node_settings["model_settings"],
+                                        net=model,
+                                        local_dataset=self.validation_data,
+                                        node_name='orchestrator')
+    
+
+    def model_initialization(self,
+                             nodes_number: int,
+                             model: Union[nn.Module, list[nn.Module]],
+                             local_warm_start: bool = False,
+                             ) -> list[nn.Module]:
+        """Creates a list of neural nets (not FederatedModels!) that will be
+        passed onto the nodes and converted into FederatedModels. If local_warm_start
+        is set to True, the method call should be passed a list of models which
+        length is equall to the number of nodes.
+        
+        -------------
+        Args:
+            nodes_number (int): number of nodes that will participate in the
+                training.
+            model (Union[nn.Module, list]): a neural net schematic (if warm
+                start is set to False) or a number of different neural net schematics
+                (if warm start is set to True) that will prepared for the nodes to be
+                loaded as FederatedModels.
+            local_warm_start (bool): A boolean value for switching on/off the warm start
+                utility.
+        -------------
+        Returns:
+            tuple(node_id: str, weights)
+        """
+        if local_warm_start == True:
+            raise("Beginning the training with different local models not implemented yet.")
+        else:
+            model_list = [copy.deepcopy(model) for _ in range(nodes_number)]
+
+        return model_list
+
+
+    def nodes_initialization(self,
+                             nodes_list: list[FederatedNode],
+                             model_list: list[nn.Module],
+                             data_list: list[datasets.arrow_dataset.Dataset, 
+                                    datasets.arrow_dataset.Dataset],
+                             nodes_number: int) -> list[FederatedNode]:
+        """Prepare instances of a FederatedNode object for a participation in 
+        the Federated Training.  Contrary to the  create nodes function, 
+        it accepts only already initialized instances of the FederatedNode
+        object.
+        
+        -------------
+        Args:
+            nodess_list (list[FederatedNode]): list containing all the initialized
+                FederatedNode instances.
+            model_list (list[nn.Module]): list containing all the initialized 
+                nn.Module objects. Note that conversion from nn.Module into the
+                FederatedModel will occur at the local node level.
+            data_list (list[..., ....]): list containing train set and test set
+                wrapped in a hugging facr arrow_dataset.Dataset containers.
+            nodes_number (int): Number of nodes that will participate in the training.
+        -------------
+        Returns:
+            list[FederatedNode]"""
+        
+        results = []
+        for node, model, dataset in zip(nodes_list, model_list, data_list):
+            node.prepare_node(model, dataset)
+            results.append(node)
+        nodes_green = []
+        for result in results:
+            if check_health(result,
+                            orchestrator_logger=orchestrator_logger):
+                nodes_green.append(result)
+        return nodes_green # Returning initialized nodes
+
+        
+        # # create the manager
+        # with Manager() as manager:
+        #     # create the shared queue
+        #     queue = manager.Queue()
+        #     # create a pool of workers
+        #     with Pool(nodes_number) as pool:
+        #         # asynchronously apply the function
+        #         results = [
+        #             pool.apply_async(prepare_nodes, (node, model, dataset, queue))
+        #             for node, model, dataset in zip(nodes_list, model_list, data_list)
+        #         ]
+        #         # consume the results
+        #         # Define a list of healthy nodes
+        #         nodes_green = []
+        #         for result in results:
+        #             # query for results
+        #             _ = result.get()
+        #             updated_node = queue.get()
+        #             # Adds to list only if the node is healthy
+        #             if check_health(updated_node,
+        #                             orchestrator_logger=orchestrator_logger):
+        #                 nodes_green.append(updated_node)
+        # return nodes_green # Returning initialized nodes
+
+    def train_protocol(self,
+                nodes_data: list[datasets.arrow_dataset.Dataset, 
+                datasets.arrow_dataset.Dataset]) -> None:
+        """Performs a full federated training according to the initialized
+        settings. The train_protocol of the generic_orchestrator.Orchestrator
+        follows a classic FedAvg algorithm - it averages the local weights
+        and aggregates them taking a weighted average.
+        SOURCE: Communication-Efficient Learning of Deep Networks from Decentralized Data, H.B. McMahan et al.
+
+        -------------
+        Args:
+            nodes_data(list[..., ....]): list containing train set and test set
+                wrapped in a hugging facr arrow_dataset.Dataset containers.
+        -------------
+        Returns:
+            None"""
+        
+        # SETTINGS -> CHANGE IF NEEDED
+        iterations = self.settings['iterations']
+        nodes_number = self.settings['number_of_nodes']
+        local_warm_start = self.settings["local_warm_start"]
+        nodes = self.settings["nodes"]
+        sample_size = self.settings["sample_size"]
+        archive_manager = Archive_Manager(archive_manager = self.settings['archiver'],
+                                          logger = orchestrator_logger)
+
+        # CREATING FEDERATED NODES
+        nodes_green = create_nodes(nodes, self.node_settings) # Exterior method / function, can override in childr.
+
+
+        # CREATING LOCAL MODELS (that will be loaded onto nodes)
+        model_list = self.model_initialization(nodes_number=nodes_number,
+                                               model=self.central_net) # Exterior method / function, can overide in childr.
+        
+        # INITIALIZING ALL THE NODES
+        nodes_green = self.nodes_initialization(nodes_list=nodes_green, # Exterion method / function, can overide in child.
+                                                model_list=model_list,
+                                                data_list=nodes_data,
+                                                nodes_number=nodes_number)
+            
+        # TRAINING PHASE ----- FEDAVG
+        with Manager() as manager:
+            queue = manager.Queue() # creates a shared queue
+            # create the pool of workers
+            with Pool(sample_size) as pool: 
+                for iteration in range(iterations):
+                    orchestrator_logger.info(f"Iteration {iteration}")
+                    weights = {}
+                    # Sampling nodes and asynchronously apply the function
+                    sampled_nodes = sample_nodes(nodes_green, 
+                                                 sample_size=sample_size, 
+                                                 orchestrator_logger=orchestrator_logger) # SAMPLING FUNCTION -> CHANGE IF NEEDED
+                    results = [pool.apply_async(train_nodes, (node,)) for node in sampled_nodes]
+                    # consume the results
+                    for result in results:
+                        node_id, model_weights = result.get()
+                        weights[node_id] = copy.deepcopy(model_weights)
+                    # Computing the average
+                    avg = Aggregators.compute_average(weights) # AGGREGATING FUNCTION -> CHANGE IF NEEDED
+                    # Updating the nodes
+                    for node in nodes_green:
+                        node.model.update_weights(avg)
+                    # Upadting the orchestrator
+                    self.central_model.update_weights(avg)
+
+                    archive_manager.archive_training_results(iteration = iteration,
+                                                             central_model=self.central_model,
+                                                             nodes=nodes_green)
+
+        orchestrator_logger.critical("Training complete")
+
```

### Comparing `asociita-0.1.6.9/asociita/datasets/fetch_data.py` & `asociita-0.1.7/asociita/datasets/fetch_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,67 @@
-import logging
-import datasets
-from asociita.datasets.load_mnist import load_mnist
-from asociita.datasets.load_cifar import load_cifar
-import pickle
-import os
-
-def load_data(settings:dict) -> list[datasets.arrow_dataset.Dataset,
-                                       list[list[list[datasets.arrow_dataset.Dataset]]]]:
-    """Loads the MNIST dataset, splits it into the number of shards, pre-process selected
-    shards (subsets) and returns in a following format:
-    list[   
-        "Orchestrator Data"[
-            Dataset
-            ],   
-        "Agents Data"[
-            "Agent N"[
-                "Train Data"[
-                Dataset
-                ],
-                "Test Data"[
-                Dataset
-                ]
-            ]]]
-    Where all 'Datasets' are an instances of hugging face container datasets.arrow_dataset.Dataset
-    ---------
-    Args:
-        settings (dict) : A dictionary containing all the dataset settings.
-    Returns:
-        list[datasets.arrow_dataset.Dataset,
-                                       list[list[list[datasets.arrow_dataset.Dataset]]]]"""
-    
-    dataset_name = settings['dataset_name']
-    if dataset_name == 'mnist':
-        loaded_dataset = load_mnist(settings=settings)
-        if settings['save_dataset'] == True:
-            dataset_name = f"MNIST_{settings['shards']}_dataset"
-            path = os.path.join(settings['save_path'], dataset_name)
-            with open(path, 'wb') as file:
-                pickle.dump(loaded_dataset, file)
-            return loaded_dataset
-        else:
-            return loaded_dataset
-    elif dataset_name == 'cifar10':
-        loaded_dataset = load_cifar(settings=settings)
-        if settings['save_dataset'] == True:
-            dataset_name = f"MNIST_{settings['shards']}_dataset"
-            path = os.path.join(settings['save_path'], dataset_name)
-            with open(path, 'wb') as file:
-                pickle.dump(loaded_dataset, file)
-            return loaded_dataset
-        else:
-            return loaded_dataset
-    else:
-        logging.warning("Wrong name of the dataset. Please provide a valid name.")
+import logging
+import datasets
+from asociita.datasets.load_mnist import load_mnist
+from asociita.datasets.load_cifar import load_cifar
+from asociita.datasets.load_fmnist import load_fmnist
+import pickle
+import os
+
+def load_data(settings:dict) -> list[datasets.arrow_dataset.Dataset,
+                                       list[list[list[datasets.arrow_dataset.Dataset]]]]:
+    """Loads the MNIST dataset, splits it into the number of shards, pre-process selected
+    shards (subsets) and returns in a following format:
+    list[   
+        "Orchestrator Data"[
+            Dataset
+            ],   
+        "Agents Data"[
+            "Agent N"[
+                "Train Data"[
+                Dataset
+                ],
+                "Test Data"[
+                Dataset
+                ]
+            ]]]
+    Where all 'Datasets' are an instances of hugging face container datasets.arrow_dataset.Dataset
+    ---------
+    Args:
+        settings (dict) : A dictionary containing all the dataset settings.
+    Returns:
+        list[datasets.arrow_dataset.Dataset,
+                                       list[list[list[datasets.arrow_dataset.Dataset]]]]"""
+    
+    dataset_name = settings['dataset_name']
+    if dataset_name == 'mnist':
+        loaded_dataset = load_mnist(settings=settings)
+        if settings['save_dataset'] == True:
+            dataset_name = f"MNIST_{settings['shards']}_dataset"
+            path = os.path.join(settings['save_path'], dataset_name)
+            with open(path, 'wb') as file:
+                pickle.dump(loaded_dataset, file)
+            return loaded_dataset
+        else:
+            return loaded_dataset
+    elif dataset_name == 'cifar10':
+        loaded_dataset = load_cifar(settings=settings)
+        if settings['save_dataset'] == True:
+            dataset_name = f"MNIST_{settings['shards']}_dataset"
+            path = os.path.join(settings['save_path'], dataset_name)
+            with open(path, 'wb') as file:
+                pickle.dump(loaded_dataset, file)
+            return loaded_dataset
+        else:
+            return loaded_dataset
+    elif dataset_name == 'fmnist':
+        loaded_dataset = load_fmnist(settings=settings)
+        if settings['save_dataset'] == True:
+            dataset_name = f"FMNIST_{settings['shards']}_dataset"
+            path = os.path.join(settings['save_path'], dataset_name)
+            with open(path, 'wb') as file:
+                pickle.dump(loaded_dataset, file)
+            return loaded_dataset
+        else:
+            return loaded_dataset
+    else:
+        logging.warning("Wrong name of the dataset. Please provide a valid name.")
```

### Comparing `asociita-0.1.6.9/asociita/datasets/load_cifar.py` & `asociita-0.1.7/asociita/datasets/load_cifar.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import datasets
-from datasets import load_dataset
-from asociita.datasets.shard_splits import Shard_Splits
-from asociita.utils.showcase import save_random
-from asociita.utils.handlers import Handler
-import copy
-import pandas as pd
-import numpy as np
-
-def load_cifar(settings: dict) -> list[datasets.arrow_dataset.Dataset,
-                                       list[list[list[datasets.arrow_dataset.Dataset]]]]:
-    """Loads the CIFAR dataset, splits it into the number of shards, pre-process selected
-    shards (subsets) and returns in a following format:
-    list[   
-        "Orchestrator Data"[
-            Dataset
-            ],   
-        "Agents Data"[
-            "Agent N"[
-                "Train Data"[
-                Dataset
-                ],
-                "Test Data"[
-                Dataset
-                ]
-            ]]]
-    Where all 'Datasets' are an instances of hugging face container datasets.arrow_dataset.Dataset
-    ---------
-    Args:
-        settings (dict) : A dictionary containing all the dataset settings.
-    Returns:
-        list[datasets.arrow_dataset.Dataset,
-                                       list[list[list[datasets.arrow_dataset.Dataset]]]]"""
-    
-    # Using the 'test' data as a orchestrator validaiton set.
-    orchestrator_data = load_dataset('cifar10', split='test')
-    # Using the 'train' data as a dataset reserved for agents
-    dataset = load_dataset('cifar10', split='train')
-
-    orchestrator_data = orchestrator_data.rename_column('img', 'image')
-    dataset = dataset.rename_column('img', 'image')
-
-    # Type: Random Uniform (Sharding) -> Same size, random distribution
-    if settings['split_type'] == 'random_uniform':
-        return [orchestrator_data, Shard_Splits.random_uniform(dataset=dataset, settings=settings)]
-    
-    # Type: Uniform with Imbalanced Classes -> Samze size, different (random) distributions with heavy imbalance on selected clients
-    if settings['split_type'] == 'random_imbalanced':
-        return [orchestrator_data, Shard_Splits.random_imbalanced(dataset=dataset, settings=settings)]
-
-    # Type: Same Dataset -> One dataset copied n times.
-    elif settings['split_type'] == 'replicate_same_dataset':
-        return [orchestrator_data, Shard_Splits.replicate_same_dataset(dataset=dataset, settings=settings)]
-    
-    # Type: Blocks - One dataset copied inside one block (cluster)
-    elif settings['split_type'] == 'split_in_blocks':
-        return [orchestrator_data, Shard_Splits.replicate_same_dataset(dataset=dataset, settings=settings)]
-    
-    else:
-        raise "Unable to generate the dataset. Provided split-type does not exist."
+import datasets
+from datasets import load_dataset
+from asociita.datasets.shard_splits import Shard_Splits
+from asociita.utils.showcase import save_random
+from asociita.utils.handlers import Handler
+import copy
+import pandas as pd
+import numpy as np
+
+def load_cifar(settings: dict) -> list[datasets.arrow_dataset.Dataset,
+                                       list[list[list[datasets.arrow_dataset.Dataset]]]]:
+    """Loads the CIFAR dataset, splits it into the number of shards, pre-process selected
+    shards (subsets) and returns in a following format:
+    list[   
+        "Orchestrator Data"[
+            Dataset
+            ],   
+        "Agents Data"[
+            "Agent N"[
+                "Train Data"[
+                Dataset
+                ],
+                "Test Data"[
+                Dataset
+                ]
+            ]]]
+    Where all 'Datasets' are an instances of hugging face container datasets.arrow_dataset.Dataset
+    ---------
+    Args:
+        settings (dict) : A dictionary containing all the dataset settings.
+    Returns:
+        list[datasets.arrow_dataset.Dataset,
+                                       list[list[list[datasets.arrow_dataset.Dataset]]]]"""
+    
+    # Using the 'test' data as a orchestrator validaiton set.
+    orchestrator_data = load_dataset('cifar10', split='test')
+    # Using the 'train' data as a dataset reserved for agents
+    dataset = load_dataset('cifar10', split='train')
+
+    orchestrator_data = orchestrator_data.rename_column('img', 'image')
+    dataset = dataset.rename_column('img', 'image')
+
+    # Type: Random Uniform (Sharding) -> Same size, random distribution
+    if settings['split_type'] == 'random_uniform':
+        return [orchestrator_data, Shard_Splits.random_uniform(dataset=dataset, settings=settings)]
+    
+    # Type: Uniform with Imbalanced Classes -> Samze size, different (random) distributions with heavy imbalance on selected clients
+    if settings['split_type'] == 'random_imbalanced':
+        return [orchestrator_data, Shard_Splits.random_imbalanced(dataset=dataset, settings=settings)]
+
+    # Type: Same Dataset -> One dataset copied n times.
+    elif settings['split_type'] == 'replicate_same_dataset':
+        return [orchestrator_data, Shard_Splits.replicate_same_dataset(dataset=dataset, settings=settings)]
+    
+    # Type: Blocks - One dataset copied inside one block (cluster)
+    elif settings['split_type'] == 'split_in_blocks':
+        return [orchestrator_data, Shard_Splits.replicate_same_dataset(dataset=dataset, settings=settings)]
+    
+    else:
+        raise "Unable to generate the dataset. Provided split-type does not exist."
```

### Comparing `asociita-0.1.6.9/asociita/datasets/load_mnist.py` & `asociita-0.1.7/asociita/datasets/load_fmnist.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-import datasets
-from datasets import load_dataset
-from asociita.datasets.shard_transformation import Shard_Transformation
-from asociita.datasets.shard_splits import Shard_Splits
-from asociita.utils.showcase import save_random
-from asociita.utils.handlers import Handler
-import copy
-import pandas as pd
-import numpy as np
-
-def load_mnist(settings: dict) -> list[datasets.arrow_dataset.Dataset,
-                                       list[list[list[datasets.arrow_dataset.Dataset]]]]:
-    """Loads the MNIST dataset, splits it into the number of shards, pre-process selected
-    shards (subsets) and returns in a following format:
-    list[   
-        "Orchestrator Data"[
-            Dataset
-            ],   
-        "Agents Data"[
-            "Agent N"[
-                "Train Data"[
-                Dataset
-                ],
-                "Test Data"[
-                Dataset
-                ]
-            ]]]
-    Where all 'Datasets' are an instances of hugging face container datasets.arrow_dataset.Dataset
-    ---------
-    Args:
-        settings (dict) : A dictionary containing all the dataset settings.
-    Returns:
-        list[datasets.arrow_dataset.Dataset,
-                                       list[list[list[datasets.arrow_dataset.Dataset]]]]"""
-    
-    # Using the 'test' data as a orchestrator validaiton set.
-    orchestrator_data = load_dataset('mnist', split='test')
-    # Using the 'train' data as a dataset reserved for agents
-    dataset = load_dataset('mnist', split='train')
-
-    # Type: Random Uniform (Sharding) -> Same size, random distribution
-    if settings['split_type'] == 'random_uniform':
-        return [orchestrator_data, Shard_Splits.random_uniform(dataset=dataset, settings=settings)]
-    
-    # Type: Uniform with Imbalanced Classes -> Samze size, different (random) distributions with heavy imbalance on selected clients
-    if settings['split_type'] == 'random_imbalanced':
-        return [orchestrator_data, Shard_Splits.random_imbalanced(dataset=dataset, settings=settings)]
-
-    # Type: Same Dataset -> One dataset copied n times.
-    elif settings['split_type'] == 'replicate_same_dataset':
-        return [orchestrator_data, Shard_Splits.replicate_same_dataset(dataset=dataset, settings=settings)]
-    
-    # Type: Blocks - One dataset copied inside one block (cluster)
-    elif settings['split_type'] == 'split_in_blocks':
-        return [orchestrator_data, Shard_Splits.replicate_same_dataset(dataset=dataset, settings=settings)]
-    
-    else:
-        raise "Unable to generate the dataset. Provided split-type does not exist."
-            
+import datasets
+from datasets import load_dataset
+from asociita.datasets.shard_transformation import Shard_Transformation
+from asociita.datasets.shard_splits import Shard_Splits
+from asociita.utils.showcase import save_random
+from asociita.utils.handlers import Handler
+import copy
+import pandas as pd
+import numpy as np
+
+def load_fmnist(settings: dict) -> list[datasets.arrow_dataset.Dataset,
+                                       list[list[list[datasets.arrow_dataset.Dataset]]]]:
+    """Loads the MNIST dataset, splits it into the number of shards, pre-process selected
+    shards (subsets) and returns in a following format:
+    list[   
+        "Orchestrator Data"[
+            Dataset
+            ],   
+        "Agents Data"[
+            "Agent N"[
+                "Train Data"[
+                Dataset
+                ],
+                "Test Data"[
+                Dataset
+                ]
+            ]]]
+    Where all 'Datasets' are an instances of hugging face container datasets.arrow_dataset.Dataset
+    ---------
+    Args:
+        settings (dict) : A dictionary containing all the dataset settings.
+    Returns:
+        list[datasets.arrow_dataset.Dataset,
+                                       list[list[list[datasets.arrow_dataset.Dataset]]]]"""
+    
+    # Using the 'test' data as a orchestrator validaiton set.
+    orchestrator_data = load_dataset('fashion_mnist', split='test')
+    # Using the 'train' data as a dataset reserved for agents
+    dataset = load_dataset('fashion_mnist', split='train')
+
+    # Type: Random Uniform (Sharding) -> Same size, random distribution
+    if settings['split_type'] == 'random_uniform':
+        return [orchestrator_data, Shard_Splits.random_uniform(dataset=dataset, settings=settings)]
+    
+    # Type: Uniform with Imbalanced Classes -> Samze size, different (random) distributions with heavy imbalance on selected clients
+    if settings['split_type'] == 'random_imbalanced':
+        return [orchestrator_data, Shard_Splits.random_imbalanced(dataset=dataset, settings=settings)]
+
+    # Type: Same Dataset -> One dataset copied n times.
+    elif settings['split_type'] == 'replicate_same_dataset':
+        return [orchestrator_data, Shard_Splits.replicate_same_dataset(dataset=dataset, settings=settings)]
+    
+    # Type: Blocks - One dataset copied inside one block (cluster)
+    elif settings['split_type'] == 'split_in_blocks':
+        return [orchestrator_data, Shard_Splits.replicate_same_dataset(dataset=dataset, settings=settings)]
+    
+    else:
+        raise "Unable to generate the dataset. Provided split-type does not exist."
+
```

### Comparing `asociita-0.1.6.9/asociita/datasets/shard_splits.py` & `asociita-0.1.7/asociita/datasets/shard_splits.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-import datasets
-from datasets import load_dataset
-from asociita.datasets.shard_transformation import Shard_Transformation
-from asociita.utils.handlers import Handler
-from asociita.utils.showcase import save_random
-import copy
-
-
-
-class Shard_Splits:
-    """a common class for creating various splits among the clients"""
-
-    @staticmethod
-    def random_uniform(dataset: datasets.arrow_dataset.Dataset,
-                       settings: dict):
-        nodes_data = []
-        for shard in range(settings['shards']): # Each shard corresponds to one
-            agent_data = dataset.shard(num_shards=settings['shards'], index=shard)
-            
-            # Shard transformation
-            if shard in settings['transformations'].keys():
-                if settings['save_transformations']:
-                    original_imgs = copy.deepcopy(agent_data['image'])
-                agent_data = Shard_Transformation.transform(agent_data, preferences=settings['transformations'][shard]) # CALL SHARD_TRANSFORMATION CLASS
-                if settings['save_transformations']:
-                    save_random(original_imgs, agent_data['image'], settings['transformations'][shard])
-
-            # In-shard split between test and train data.
-            agent_data = agent_data.train_test_split(test_size=settings["local_test_size"])
-            nodes_data.append([agent_data['train'], agent_data['test']])
-        return nodes_data
-    
-
-    @staticmethod
-    def random_imbalanced(dataset: datasets.arrow_dataset.Dataset,
-                          settings: dict):
-        nodes_data = []
-        no_agents = settings['agents']
-        imbalanced_agents = settings['imbalanced_clients']
-        agents = [agent for agent in range(no_agents)]
-        pandas_df = dataset.to_pandas().drop('image', axis=1)
-        labels = sorted(pandas_df.label.unique())
-
-        save_distribution = False
-        print_distribution = False
-        
-        if settings.get('save_distribution'):
-            distribution_blueprint = []
-            save_distribution = True
-        if settings.get('print_distribution'):
-            print_distribution = True
-        if settings.get('custom_sample_size'):
-            sample_size = settings['custom_sample_size']
-        else:
-            sample_size = int(len(dataset) / no_agents)
-    
-
-        # I) Sampling dominant clients
-        for agent in agents:
-            if agent in imbalanced_agents:
-                # 1. Sampling indexes
-                sampling_weights = {key: (1 - imbalanced_agents[agent][1]) / (len(labels) - 1) for key in labels}
-                sampling_weights[imbalanced_agents[agent][0]] = imbalanced_agents[agent][1]
-                
-                # Additional step, checking the availability of every label TODO
-                # required_samples = (np.array(list(sampling_weights.values())) * sample_size).astype('int')
-                # counts = pandas_df['label'].value_counts()[pandas_df['label'].value_counts() > required_samples]
-                
-                # 2. Apllying weights
-                pandas_df["weights"] = pandas_df['label'].apply(lambda x: sampling_weights[x])
-                sample = pandas_df.sample(n = sample_size, weights='weights', random_state=42)
-                
-                counts = sample['label'].value_counts().sort_index()
-                if print_distribution:
-                    print(f"Distribution of client {agent} is : {counts}")
-                if save_distribution:
-                    ag = counts.to_dict()
-                    distribution = {'agent':agent}
-                    distribution.update(ag)
-                    distribution_blueprint.append(distribution)
-                # 3. Selecting indexes and performing test - train split.
-                sampled_data = dataset.filter(lambda filter, idx: idx in list(sample.index), with_indices=True)
-                agent_data = sampled_data.train_test_split(test_size=settings["local_test_size"])
-                nodes_data.append([agent_data['train'], agent_data['test']])
-                
-                # 4. Removing samples indexes
-                pandas_df.drop(sample.index, inplace=True)
-            else:
-                nodes_data.append([]) # Inserting placeholder to preserve in-list order.
-
-
-        # II) Sampling balanced clients
-        for agent in agents:
-            if agent not in imbalanced_agents:
-                # 1. Sampling indexes
-                sample = pandas_df.sample(n = sample_size, random_state=42)
-                counts = sample['label'].value_counts().sort_index()
-                if print_distribution:
-                    print(f"Distribution of client {agent} is : {counts}")
-                if save_distribution:
-                    ag = counts.to_dict()
-                    distribution = {'agent':agent}
-                    distribution.update(ag)
-                    distribution_blueprint.append(distribution)
-                # 2. Selecting indexes and performing test - train split.
-                sampled_data = dataset.filter(lambda filter, idx: idx in list(sample.index), with_indices=True)
-                agent_data = sampled_data.train_test_split(test_size=settings["local_test_size"])
-                nodes_data[agent] = ([agent_data['train'], agent_data['test']])
-                # 3. Removing samples indexes
-                pandas_df.drop(sample.index, inplace=True)
-        
-        if save_distribution:
-            Handler.save_csv_file(file = distribution_blueprint,
-                                  saving_path=settings['save_path'],
-                                  file_name='distribution_blueprint.csv')
-        return nodes_data
-
-    @staticmethod
-    def replicate_same_dataset(dataset: datasets.arrow_dataset.Dataset,
-                               settings: dict):
-        nodes_data = []
-        agent_data = dataset.shard(num_shards=1, index=0)
-        agent_data = agent_data.train_test_split(test_size=settings["local_test_size"])
-        for _ in range(settings['agents']):
-            nodes_data.append([copy.deepcopy(agent_data['train']), copy.deepcopy(agent_data['test'])])
-        
-        return nodes_data
-    
-
-    @staticmethod
-    def split_in_blocks(dataset: datasets.arrow_dataset.Dataset,
-                        settings: dict):
-        nodes_data = []
-        for shard in range(settings['shards']):
-            agent_data = dataset.shard(num_shards=settings['shards'], index=shard)
-            agent_data = agent_data.train_test_split(test_size=settings["local_test_size"])
-            for _ in range((int(settings['agents'] / settings['shards']))):
-                nodes_data.append([copy.deepcopy(agent_data['train']), copy.deepcopy(agent_data['test'])])
+import datasets
+from datasets import load_dataset
+from asociita.datasets.shard_transformation import Shard_Transformation
+from asociita.utils.handlers import Handler
+from asociita.utils.showcase import save_random
+import copy
+
+
+
+class Shard_Splits:
+    """a common class for creating various splits among the clients"""
+
+    @staticmethod
+    def random_uniform(dataset: datasets.arrow_dataset.Dataset,
+                       settings: dict):
+        nodes_data = []
+        for shard in range(settings['shards']): # Each shard corresponds to one agent.
+            agent_data = dataset.shard(num_shards=settings['shards'], index=shard)
+            
+            # Shard transformation
+            if shard in settings['transformations'].keys():
+                if settings['save_transformations']:
+                    original_imgs = copy.deepcopy(agent_data['image'])
+                agent_data = Shard_Transformation.transform(agent_data, preferences=settings['transformations'][shard]) # CALL SHARD_TRANSFORMATION CLASS
+                if settings['save_transformations']:
+                    save_random(original_imgs, agent_data['image'], settings['transformations'][shard]["transformation_type"])
+
+            # In-shard split between test and train data.
+            agent_data = agent_data.train_test_split(test_size=settings["local_test_size"])
+            nodes_data.append([agent_data['train'], agent_data['test']])
+        return nodes_data
+    
+
+    @staticmethod
+    def random_imbalanced(dataset: datasets.arrow_dataset.Dataset,
+                          settings: dict):
+        nodes_data = []
+        no_agents = settings['agents']
+        imbalanced_agents = settings['imbalanced_clients']
+        agents = [agent for agent in range(no_agents)]
+        pandas_df = dataset.to_pandas().drop('image', axis=1)
+        labels = sorted(pandas_df.label.unique())
+
+        save_distribution = False
+        print_distribution = False
+        
+        if settings.get('save_distribution'):
+            distribution_blueprint = []
+            save_distribution = True
+        if settings.get('print_distribution'):
+            print_distribution = True
+        if settings.get('custom_sample_size'):
+            sample_size = settings['custom_sample_size']
+        else:
+            sample_size = int(len(dataset) / no_agents)
+    
+
+        # I) Sampling dominant clients
+        for agent in agents:
+            if agent in imbalanced_agents:
+                # 1. Sampling indexes
+                sampling_weights = {key: (1 - imbalanced_agents[agent][1]) / (len(labels) - 1) for key in labels}
+                sampling_weights[imbalanced_agents[agent][0]] = imbalanced_agents[agent][1]
+                
+                # Additional step, checking the availability of every label TODO
+                # required_samples = (np.array(list(sampling_weights.values())) * sample_size).astype('int')
+                # counts = pandas_df['label'].value_counts()[pandas_df['label'].value_counts() > required_samples]
+                
+                # 2. Apllying weights
+                pandas_df["weights"] = pandas_df['label'].apply(lambda x: sampling_weights[x])
+                sample = pandas_df.sample(n = sample_size, weights='weights', random_state=42)
+                
+                counts = sample['label'].value_counts().sort_index()
+                if print_distribution:
+                    print(f"Distribution of client {agent} is : {counts}")
+                if save_distribution:
+                    ag = counts.to_dict()
+                    distribution = {'agent':agent}
+                    distribution.update(ag)
+                    distribution_blueprint.append(distribution)
+                # 3. Selecting indexes and performing test - train split.
+                sampled_data = dataset.filter(lambda filter, idx: idx in list(sample.index), with_indices=True)
+                agent_data = sampled_data.train_test_split(test_size=settings["local_test_size"])
+                nodes_data.append([agent_data['train'], agent_data['test']])
+                
+                # 4. Removing samples indexes
+                pandas_df.drop(sample.index, inplace=True)
+            else:
+                nodes_data.append([]) # Inserting placeholder to preserve in-list order.
+
+
+        # II) Sampling balanced clients
+        for agent in agents:
+            if agent not in imbalanced_agents:
+                # 1. Sampling indexes
+                sample = pandas_df.sample(n = sample_size, random_state=42)
+                counts = sample['label'].value_counts().sort_index()
+                if print_distribution:
+                    print(f"Distribution of client {agent} is : {counts}")
+                if save_distribution:
+                    ag = counts.to_dict()
+                    distribution = {'agent':agent}
+                    distribution.update(ag)
+                    distribution_blueprint.append(distribution)
+                # 2. Selecting indexes and performing test - train split.
+                sampled_data = dataset.filter(lambda filter, idx: idx in list(sample.index), with_indices=True)
+                agent_data = sampled_data.train_test_split(test_size=settings["local_test_size"])
+                nodes_data[agent] = ([agent_data['train'], agent_data['test']])
+                # 3. Removing samples indexes
+                pandas_df.drop(sample.index, inplace=True)
+        
+        if save_distribution:
+            Handler.save_csv_file(file = distribution_blueprint,
+                                  saving_path=settings['save_path'],
+                                  file_name='distribution_blueprint.csv')
+        return nodes_data
+
+    @staticmethod
+    def replicate_same_dataset(dataset: datasets.arrow_dataset.Dataset,
+                               settings: dict):
+        nodes_data = []
+        agent_data = dataset.shard(num_shards=1, index=0)
+        agent_data = agent_data.train_test_split(test_size=settings["local_test_size"])
+        for _ in range(settings['agents']):
+            nodes_data.append([copy.deepcopy(agent_data['train']), copy.deepcopy(agent_data['test'])])
+        
+        return nodes_data
+    
+
+    @staticmethod
+    def split_in_blocks(dataset: datasets.arrow_dataset.Dataset,
+                        settings: dict):
+        nodes_data = []
+        for shard in range(settings['shards']):
+            agent_data = dataset.shard(num_shards=settings['shards'], index=shard)
+            agent_data = agent_data.train_test_split(test_size=settings["local_test_size"])
+            for _ in range((int(settings['agents'] / settings['shards']))):
+                nodes_data.append([copy.deepcopy(agent_data['train']), copy.deepcopy(agent_data['test'])])
         return nodes_data
```

### Comparing `asociita-0.1.6.9/asociita/models/pytorch/cifar10.py` & `asociita-0.1.7/asociita/models/pytorch/cifar10.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-
-class CifarNet(nn.Module):
-    def __init__(self):
-        super().__init__()
-        self.conv1 = nn.Conv2d(3, 6, 5)
-        self.pool = nn.MaxPool2d(2, 2)
-        self.conv2 = nn.Conv2d(6, 16, 5)
-        self.fc1 = nn.Linear(16 * 5 * 5, 120)
-        self.fc2 = nn.Linear(120, 84)
-        self.fc3 = nn.Linear(84, 10)
-
-    def forward(self, x):
-        x = self.pool(F.relu(self.conv1(x)))
-        x = self.pool(F.relu(self.conv2(x)))
-        x = torch.flatten(x, 1) # flatten all dimensions except batch
-        x = F.relu(self.fc1(x))
-        x = F.relu(self.fc2(x))
-        x = self.fc3(x)
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+
+class CifarNet(nn.Module):
+    def __init__(self):
+        super().__init__()
+        self.conv1 = nn.Conv2d(3, 6, 5)
+        self.pool = nn.MaxPool2d(2, 2)
+        self.conv2 = nn.Conv2d(6, 16, 5)
+        self.fc1 = nn.Linear(16 * 5 * 5, 120)
+        self.fc2 = nn.Linear(120, 84)
+        self.fc3 = nn.Linear(84, 10)
+
+    def forward(self, x):
+        x = self.pool(F.relu(self.conv1(x)))
+        x = self.pool(F.relu(self.conv2(x)))
+        x = torch.flatten(x, 1) # flatten all dimensions except batch
+        x = F.relu(self.fc1(x))
+        x = F.relu(self.fc2(x))
+        x = self.fc3(x)
         return x
```

### Comparing `asociita-0.1.6.9/asociita/models/pytorch/federated_model.py` & `asociita-0.1.7/asociita/models/pytorch/federated_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,387 +1,387 @@
-# Libraries imports
-import sys, warnings, torch, gc, copy
-import numpy as np
-from datasets import arrow_dataset
-from collections import OrderedDict
-# Modules imports
-from collections import Counter
-from typing import Any, Generic, Mapping, TypeVar, Union
-#from sklearn.metrics import confusion_matrix, f1_score, precision_score, recall_score
-from torch import nn, optim
-from torchvision import transforms
-from sklearn.metrics import f1_score, recall_score, confusion_matrix, precision_score
-import os
-
-from asociita.utils.loggers import Loggers
-
-model_logger = Loggers.model_logger()
-
-class FederatedModel:
-    """This class is used to encapsulate the (PyTorch) federated model that
-    we will train. It accepts only the PyTorch models and 
-    provides a utility functions to initialize the model, 
-    retrieve the weights or perform an indicated number of traning
-    epochs.
-    """
-    def __init__(
-        self,
-        settings: dict,
-        net: nn.Module,
-        local_dataset: list[arrow_dataset.Dataset, arrow_dataset.Dataset] |
-                                list[arrow_dataset.Dataset],
-        node_name: int
-    ) -> None:
-        """Initialize the Federated Model. This model will be attached to a 
-        specific client and will wait for further instructions.
-        -------------
-        Args:
-            settings (dict): Settings for this run.
-            net (nn.Module): Neural Network architecture that we want to use.
-            local_dataset (list[...]): local dataset that will be used with this set.
-            node_name (int): identifier for the node that uses this container.
-            features_name (int): name of key used to retrieve features, e.g. 'image'.
-        -------------
-        Returns:
-            None
-        """
-        self.device = None
-        self.initial_model = None
-        self.optimizer: optim.Optimizer = None
-        
-        # Checks for all the necessary elements:
-        assert settings, "Could not find settings, please ensure that a valid dictionary containing settings was passed in a function call."
-        assert net, "Could not find net object, please ensure that a valid nn.Module was passed in a function call."
-        assert local_dataset, "Could not find local dataset that should be used with that model. Pleasure ensure that local dataset was passed in a function call."
-        
-        self.net = copy.deepcopy(net)
-        self.settings = settings
-        self.node_name = node_name
-
-        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-        self.net.to(self.device)
-        model_logger.info(f"Node {node_name} will use {self.device} as a device.")
-
-        # If both, train and test data were provided
-        if len(local_dataset) == 2:
-            self.trainloader, self.testloader = self.prepare_data(local_dataset)
-        # If only a test dataset was provided.
-        elif len(local_dataset) == 1:
-            self.testloader = self.prepare_data(local_dataset, only_test=True)
-        else:
-            raise "The provided dataset object seem to be wrong. Please provide list[train_set, test_set] or list[test_set]"
-
-        # List containing all the parameters to update
-        params_to_update = []
-        for _, param in self.net.named_parameters():
-            if param.requires_grad is True:
-                params_to_update.append(param)
-
-        # Choosing an optimizer based on settings
-        if self.settings['optimizer'] == "Adam":
-            raise "Using Adam Optimizer has not been implemented yet."
-            # TODO #self.optimizer = torch.optim.Adam(...
-        elif self.settings['optimizer'] == "SGD":
-            raise "Using SGD Optimizer has not been implemented yet."
-            #TODO # self.optimizer = torch.optim.SGD(...
-        elif self.settings['optimizer'] == "RMS":
-            self.optimizer = optim.RMSprop(
-                params_to_update,
-                lr=self.settings["learning_rate"],)
-        else:
-            raise "The provided optimizer name may be incorrect or not implemeneted.\
-            Please provide list[train_set, test_set] or list[test_set]"
-
-
-    def prepare_data(
-        self,
-        local_dataset: list[arrow_dataset.Dataset, arrow_dataset.Dataset] |
-                                list[arrow_dataset.Dataset],
-        only_test: bool = False
-    ) -> tuple[torch.utils.data.DataLoader, torch.utils.data.DataLoader]:
-        """Convert training and test data stored on the local client into
-        torch.utils.data.DataLoader.
-        Args:
-        -------------
-            local_dataset (list[...]: local dataset that should be loaded into DataLoader)
-            only_test (bool, default to False): If true, only a test set will be returned
-            Returns
-        -------------
-            Tuple[torch.utils.data.DataLoader, torch.utils.data.DataLoader]: training and test set
-            or
-            Tuple[torch.utils.data.DataLoader]: test set, if only_test == True.
-        """
-        if only_test == False:
-            local_dataset[0] = local_dataset[0].with_transform(self.transform_func)
-            local_dataset[1] = local_dataset[1].with_transform(self.transform_func)
-            batch_size = self.settings["batch_size"]
-            trainloader = torch.utils.data.DataLoader(
-                local_dataset[0],
-                batch_size=batch_size,
-                shuffle=True,
-                num_workers=0,
-            )
-
-            testloader = torch.utils.data.DataLoader(
-                local_dataset[1],
-                batch_size=16,
-                shuffle=False,
-                num_workers=0,
-            )
-            #self.print_data_stats(trainloader) #TODO
-            return trainloader, testloader
-        else:
-            local_dataset[0] = local_dataset[0].with_transform(self.transform_func)
-            testloader = torch.utils.data.DataLoader(
-                local_dataset[0],
-                batch_size=16,
-                shuffle=False,
-                num_workers=0,
-            )
-            return testloader
-
-
-    def print_data_stats(self, trainloader: torch.utils.data.DataLoader) -> None: #TODO
-        """Debug function used to print stats about the loaded datasets.
-        Args:
-            trainloader (torch.utils.data.DataLoader): training set
-        """
-        num_examples = {
-            "trainset": len(self.training_set),
-            "testset": len(self.test_set),
-        }
-        targets = []
-        for _, data in enumerate(trainloader, 0):
-            targets.append(data[1])
-        targets = [item.item() for sublist in targets for item in sublist]
-        model_logger.info(f"{self.node_name}, {Counter(targets)}")
-        model_logger.info(f"{self.node_name}: Training set size: {num_examples['trainset']}")
-        model_logger.info(f"{self.node_name}: Test set size: {num_examples['testset']}")
-
-
-    def get_weights_list(self) -> list[float]:
-        """Get the parameters of the network.
-        Args
-        -------------
-            self
-        Returns
-        -------------
-            List[float]: parameters of the network
-        """
-        return [val.cpu().numpy() for _, val in self.net.state_dict().items()]
-
-
-    def get_weights(self):
-        """Get the weights of the network.
-        Raises
-        -------------
-            Exception: if the model is not initialized it raises an exception
-        Returns
-        -------------
-            _type_: weights of the network
-        """
-        return copy.deepcopy(self.net.state_dict())
-    
-
-    def get_gradients(self):
-        
-        assert self.initial_model != None, "Computing gradients require saving initial model first!"
-        weights_t1 = self.net.state_dict()
-        weights_t2 = self.initial_model.state_dict()
-        
-        self.gradients = OrderedDict.fromkeys(weights_t1.keys(), 0)
-        for key in weights_t1:
-            self.gradients[key] = weights_t2[key] - weights_t1[key]
-        
-        return copy.deepcopy(self.gradients)
-
-
-    def update_weights(self, avg_tensors) -> None:
-        """This function updates the weights of the network.
-        Raises
-        ------
-            Exception: _description_
-        Args:
-            avg_tensors (_type_): tensors that we want to use in the network
-        """
-        self.net.load_state_dict(avg_tensors, strict=True)
-
-
-    def store_model_on_disk(self,
-                            iteration: int,
-                            path: str) -> None: #TODO
-        """This function is used to store the trained model
-        on disk.
-        Raises
-        ------
-            Exception: if the model is not initialized it raises an exception
-        """
-        if self.net:
-            name = f"node_{self.node_name}_iteration_{iteration}.pt"
-            save_path = os.path.join(path, name)
-            torch.save(
-                self.net.state_dict(),
-                save_path,
-            )
-        else:
-            raise NotImplementedError
-
-
-    def preserve_initial_model(self) -> None:
-        """Preserve the initial model provided at the
-        end of the turn (necessary for computing gradients,
-        when using aggregating methods such as FedOpt).
-        Args:
-        -------------
-            self
-        Returns
-        -------------
-            Tuple[float, float]: Loss and accuracy on the training set.
-        """
-        self.initial_model = copy.deepcopy(self.net)
-
-
-    def train(self) -> tuple[float, torch.tensor]:
-        """Train the network and computes loss and accuracy.
-        Args:
-        -------------
-            self
-        Raises
-        ------
-            Exception: Raises an exception when Federated Learning is not initialized
-        Returns
-        -------
-            Tuple[float, float]: Loss and accuracy on the training set.
-        """
-
-        criterion = nn.CrossEntropyLoss()
-        running_loss = 0.0
-        total_correct = 0
-        total = 0
-        #self.net = self.net.to(self.device)
-
-        self.net.train()
-        for _, dic in enumerate(self.trainloader):
-            data = dic['image']
-            target = dic['label']
-
-            self.optimizer.zero_grad()
-
-            if isinstance(data, list):
-                data = data[0]
-            
-            data, target = data.to(self.device), target.to(self.device)
-            # forward pass, backward pass and optimization
-            outputs = self.net(data)
-            _, predicted = torch.max(outputs.data, 1)
-            correct = (predicted == target).float().sum()
-
-            loss = criterion(outputs, target)
-            running_loss += loss.item()
-            total_correct += correct
-            total += target.size(0)
-
-            self.optimizer.zero_grad()
-            self.net.zero_grad()
-            loss.backward()
-            self.optimizer.step()
-            self.optimizer.zero_grad()
-            self.net.zero_grad()
-        
-            if torch.cuda.is_available():
-                torch.cuda.empty_cache()
-
-
-        loss = running_loss / len(self.trainloader)
-        accuracy = total_correct / total
-        model_logger.info(f"Training on {self.node_name} results: loss: {loss}, accuracy: {accuracy}")
-
-        return loss, accuracy
-    
-
-    def evaluate_model(self) -> tuple[float, float, float, float, float, list]:
-        """Validate the network on the local test set.
-        Raises
-        ------
-            Exception: Raises an exception when Federated Learning is not initialized
-        Returns
-        -------
-            Tuple[float, float]: loss and accuracy on the test set.
-        """
-        with torch.no_grad():
-            if self.net:
-                self.net.eval()
-                criterion = nn.CrossEntropyLoss()
-                test_loss = 0
-                correct = 0
-                total = 0
-                y_pred = []
-                y_true = []
-                losses = []
-                with torch.no_grad():
-                    for _, dic in enumerate(self.testloader):
-                        data = dic['image']
-                        target = dic['label']
-                        data, target = data.to(self.device), target.to(self.device)
-                        output = self.net(data)
-                        total += target.size(0)
-                        test_loss = criterion(output, target).item()
-                        losses.append(test_loss)
-                        pred = output.argmax(dim=1, keepdim=True)
-                        correct += pred.eq(target.view_as(pred)).sum().item()
-                        y_pred.append(pred)
-                        y_true.append(target)
-
-                test_loss = np.mean(losses)
-                accuracy = correct / total
-
-                y_true = [item.item() for sublist in y_true for item in sublist]
-                y_pred = [item.item() for sublist in y_pred for item in sublist]
-
-                f1score = f1_score(y_true, y_pred, average="macro")
-                precision = precision_score(y_true, y_pred, average="macro")
-                recall = recall_score(y_true, y_pred, average="macro")
-
-                cm = confusion_matrix(y_true, y_pred)
-                cm = cm.astype("float") / cm.sum(axis=1)[:, np.newaxis]
-                accuracy_per_class = cm.diagonal()
-
-                true_positives = np.diag(cm)
-                num_classes = len(list(set(y_true)))
-
-                false_positives = []
-                for i in range(num_classes):
-                    false_positives.append(sum(cm[:,i]) - cm[i,i])
-
-                false_negatives = []
-                for i in range(num_classes):
-                    false_negatives.append(sum(cm[i,:]) - cm[i,i])
-
-                true_negatives = []
-                for i in range(num_classes):
-                    temp = np.delete(cm, i, 0)   # delete ith row
-                    temp = np.delete(temp, i, 1)  # delete ith column
-                    true_negatives.append(sum(sum(temp)))
-
-                denominator = [sum(x) for x in zip(false_positives, true_negatives)]
-                false_positive_rate = [num/den for num, den in zip(false_positives, denominator)]
-
-                denominator = [sum(x) for x in zip(true_positives, false_negatives)]
-                true_positive_rate = [num/den for num, den in zip(true_positives, denominator)]
-
-                return (
-                    test_loss,
-                    accuracy,
-                    f1score,
-                    precision,
-                    recall,
-                    accuracy_per_class,
-                    true_positive_rate,
-                    false_positive_rate
-                )
-
-
-    def transform_func(self,
-                       data):
-        convert_tensor = transforms.ToTensor()
-        data['image'] = [convert_tensor(img) for img in data['image']]
+# Libraries imports
+import sys, warnings, torch, gc, copy
+import numpy as np
+from datasets import arrow_dataset
+from collections import OrderedDict
+# Modules imports
+from collections import Counter
+from typing import Any, Generic, Mapping, TypeVar, Union
+#from sklearn.metrics import confusion_matrix, f1_score, precision_score, recall_score
+from torch import nn, optim
+from torchvision import transforms
+from sklearn.metrics import f1_score, recall_score, confusion_matrix, precision_score
+import os
+
+from asociita.utils.loggers import Loggers
+
+model_logger = Loggers.model_logger()
+
+class FederatedModel:
+    """This class is used to encapsulate the (PyTorch) federated model that
+    we will train. It accepts only the PyTorch models and 
+    provides a utility functions to initialize the model, 
+    retrieve the weights or perform an indicated number of traning
+    epochs.
+    """
+    def __init__(
+        self,
+        settings: dict,
+        net: nn.Module,
+        local_dataset: list[arrow_dataset.Dataset, arrow_dataset.Dataset] |
+                                list[arrow_dataset.Dataset],
+        node_name: int
+    ) -> None:
+        """Initialize the Federated Model. This model will be attached to a 
+        specific client and will wait for further instructions.
+        -------------
+        Args:
+            settings (dict): Settings for this run.
+            net (nn.Module): Neural Network architecture that we want to use.
+            local_dataset (list[...]): local dataset that will be used with this set.
+            node_name (int): identifier for the node that uses this container.
+            features_name (int): name of key used to retrieve features, e.g. 'image'.
+        -------------
+        Returns:
+            None
+        """
+        self.device = None
+        self.initial_model = None
+        self.optimizer: optim.Optimizer = None
+        
+        # Checks for all the necessary elements:
+        assert settings, "Could not find settings, please ensure that a valid dictionary containing settings was passed in a function call."
+        assert net, "Could not find net object, please ensure that a valid nn.Module was passed in a function call."
+        assert local_dataset, "Could not find local dataset that should be used with that model. Pleasure ensure that local dataset was passed in a function call."
+        
+        self.net = copy.deepcopy(net)
+        self.settings = settings
+        self.node_name = node_name
+
+        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+        self.net.to(self.device)
+        model_logger.info(f"Node {node_name} will use {self.device} as a device.")
+
+        # If both, train and test data were provided
+        if len(local_dataset) == 2:
+            self.trainloader, self.testloader = self.prepare_data(local_dataset)
+        # If only a test dataset was provided.
+        elif len(local_dataset) == 1:
+            self.testloader = self.prepare_data(local_dataset, only_test=True)
+        else:
+            raise "The provided dataset object seem to be wrong. Please provide list[train_set, test_set] or list[test_set]"
+
+        # List containing all the parameters to update
+        params_to_update = []
+        for _, param in self.net.named_parameters():
+            if param.requires_grad is True:
+                params_to_update.append(param)
+
+        # Choosing an optimizer based on settings
+        if self.settings['optimizer'] == "Adam":
+            raise "Using Adam Optimizer has not been implemented yet."
+            # TODO #self.optimizer = torch.optim.Adam(...
+        elif self.settings['optimizer'] == "SGD":
+            raise "Using SGD Optimizer has not been implemented yet."
+            #TODO # self.optimizer = torch.optim.SGD(...
+        elif self.settings['optimizer'] == "RMS":
+            self.optimizer = optim.RMSprop(
+                params_to_update,
+                lr=self.settings["learning_rate"],)
+        else:
+            raise "The provided optimizer name may be incorrect or not implemeneted.\
+            Please provide list[train_set, test_set] or list[test_set]"
+
+
+    def prepare_data(
+        self,
+        local_dataset: list[arrow_dataset.Dataset, arrow_dataset.Dataset] |
+                                list[arrow_dataset.Dataset],
+        only_test: bool = False
+    ) -> tuple[torch.utils.data.DataLoader, torch.utils.data.DataLoader]:
+        """Convert training and test data stored on the local client into
+        torch.utils.data.DataLoader.
+        Args:
+        -------------
+            local_dataset (list[...]: local dataset that should be loaded into DataLoader)
+            only_test (bool, default to False): If true, only a test set will be returned
+            Returns
+        -------------
+            Tuple[torch.utils.data.DataLoader, torch.utils.data.DataLoader]: training and test set
+            or
+            Tuple[torch.utils.data.DataLoader]: test set, if only_test == True.
+        """
+        if only_test == False:
+            local_dataset[0] = local_dataset[0].with_transform(self.transform_func)
+            local_dataset[1] = local_dataset[1].with_transform(self.transform_func)
+            batch_size = self.settings["batch_size"]
+            trainloader = torch.utils.data.DataLoader(
+                local_dataset[0],
+                batch_size=batch_size,
+                shuffle=True,
+                num_workers=0,
+            )
+
+            testloader = torch.utils.data.DataLoader(
+                local_dataset[1],
+                batch_size=16,
+                shuffle=False,
+                num_workers=0,
+            )
+            #self.print_data_stats(trainloader) #TODO
+            return trainloader, testloader
+        else:
+            local_dataset[0] = local_dataset[0].with_transform(self.transform_func)
+            testloader = torch.utils.data.DataLoader(
+                local_dataset[0],
+                batch_size=16,
+                shuffle=False,
+                num_workers=0,
+            )
+            return testloader
+
+
+    def print_data_stats(self, trainloader: torch.utils.data.DataLoader) -> None: #TODO
+        """Debug function used to print stats about the loaded datasets.
+        Args:
+            trainloader (torch.utils.data.DataLoader): training set
+        """
+        num_examples = {
+            "trainset": len(self.training_set),
+            "testset": len(self.test_set),
+        }
+        targets = []
+        for _, data in enumerate(trainloader, 0):
+            targets.append(data[1])
+        targets = [item.item() for sublist in targets for item in sublist]
+        model_logger.info(f"{self.node_name}, {Counter(targets)}")
+        model_logger.info(f"{self.node_name}: Training set size: {num_examples['trainset']}")
+        model_logger.info(f"{self.node_name}: Test set size: {num_examples['testset']}")
+
+
+    def get_weights_list(self) -> list[float]:
+        """Get the parameters of the network.
+        Args
+        -------------
+            self
+        Returns
+        -------------
+            List[float]: parameters of the network
+        """
+        return [val.cpu().numpy() for _, val in self.net.state_dict().items()]
+
+
+    def get_weights(self):
+        """Get the weights of the network.
+        Raises
+        -------------
+            Exception: if the model is not initialized it raises an exception
+        Returns
+        -------------
+            _type_: weights of the network
+        """
+        return copy.deepcopy(self.net.state_dict())
+    
+
+    def get_gradients(self):
+        
+        assert self.initial_model != None, "Computing gradients require saving initial model first!"
+        weights_t1 = self.net.state_dict()
+        weights_t2 = self.initial_model.state_dict()
+        
+        self.gradients = OrderedDict.fromkeys(weights_t1.keys(), 0)
+        for key in weights_t1:
+            self.gradients[key] =  weights_t1[key] - weights_t2[key]
+        
+        return copy.deepcopy(self.gradients)
+
+
+    def update_weights(self, avg_tensors) -> None:
+        """This function updates the weights of the network.
+        Raises
+        ------
+            Exception: _description_
+        Args:
+            avg_tensors (_type_): tensors that we want to use in the network
+        """
+        self.net.load_state_dict(avg_tensors, strict=True)
+
+
+    def store_model_on_disk(self,
+                            iteration: int,
+                            path: str) -> None: #TODO
+        """This function is used to store the trained model
+        on disk.
+        Raises
+        ------
+            Exception: if the model is not initialized it raises an exception
+        """
+        if self.net:
+            name = f"node_{self.node_name}_iteration_{iteration}.pt"
+            save_path = os.path.join(path, name)
+            torch.save(
+                self.net.state_dict(),
+                save_path,
+            )
+        else:
+            raise NotImplementedError
+
+
+    def preserve_initial_model(self) -> None:
+        """Preserve the initial model provided at the
+        end of the turn (necessary for computing gradients,
+        when using aggregating methods such as FedOpt).
+        Args:
+        -------------
+            self
+        Returns
+        -------------
+            Tuple[float, float]: Loss and accuracy on the training set.
+        """
+        self.initial_model = copy.deepcopy(self.net)
+
+
+    def train(self) -> tuple[float, torch.tensor]:
+        """Train the network and computes loss and accuracy.
+        Args:
+        -------------
+            self
+        Raises
+        ------
+            Exception: Raises an exception when Federated Learning is not initialized
+        Returns
+        -------
+            Tuple[float, float]: Loss and accuracy on the training set.
+        """
+
+        criterion = nn.CrossEntropyLoss()
+        running_loss = 0.0
+        total_correct = 0
+        total = 0
+        #self.net = self.net.to(self.device)
+
+        self.net.train()
+        for _, dic in enumerate(self.trainloader):
+            data = dic['image']
+            target = dic['label']
+
+            self.optimizer.zero_grad()
+
+            if isinstance(data, list):
+                data = data[0]
+            
+            data, target = data.to(self.device), target.to(self.device)
+            # forward pass, backward pass and optimization
+            outputs = self.net(data)
+            _, predicted = torch.max(outputs.data, 1)
+            correct = (predicted == target).float().sum()
+
+            loss = criterion(outputs, target)
+            running_loss += loss.item()
+            total_correct += correct
+            total += target.size(0)
+
+            self.optimizer.zero_grad()
+            self.net.zero_grad()
+            loss.backward()
+            self.optimizer.step()
+            self.optimizer.zero_grad()
+            self.net.zero_grad()
+        
+            if torch.cuda.is_available():
+                torch.cuda.empty_cache()
+
+
+        loss = running_loss / len(self.trainloader)
+        accuracy = total_correct / total
+        model_logger.info(f"Training on {self.node_name} results: loss: {loss}, accuracy: {accuracy}")
+
+        return loss, accuracy
+    
+
+    def evaluate_model(self) -> tuple[float, float, float, float, float, list]:
+        """Validate the network on the local test set.
+        Raises
+        ------
+            Exception: Raises an exception when Federated Learning is not initialized
+        Returns
+        -------
+            Tuple[float, float]: loss and accuracy on the test set.
+        """
+        with torch.no_grad():
+            if self.net:
+                self.net.eval()
+                criterion = nn.CrossEntropyLoss()
+                test_loss = 0
+                correct = 0
+                total = 0
+                y_pred = []
+                y_true = []
+                losses = []
+                with torch.no_grad():
+                    for _, dic in enumerate(self.testloader):
+                        data = dic['image']
+                        target = dic['label']
+                        data, target = data.to(self.device), target.to(self.device)
+                        output = self.net(data)
+                        total += target.size(0)
+                        test_loss = criterion(output, target).item()
+                        losses.append(test_loss)
+                        pred = output.argmax(dim=1, keepdim=True)
+                        correct += pred.eq(target.view_as(pred)).sum().item()
+                        y_pred.append(pred)
+                        y_true.append(target)
+
+                test_loss = np.mean(losses)
+                accuracy = correct / total
+
+                y_true = [item.item() for sublist in y_true for item in sublist]
+                y_pred = [item.item() for sublist in y_pred for item in sublist]
+
+                f1score = f1_score(y_true, y_pred, average="macro")
+                precision = precision_score(y_true, y_pred, average="macro")
+                recall = recall_score(y_true, y_pred, average="macro")
+
+                cm = confusion_matrix(y_true, y_pred)
+                cm = cm.astype("float") / cm.sum(axis=1)[:, np.newaxis]
+                accuracy_per_class = cm.diagonal()
+
+                true_positives = np.diag(cm)
+                num_classes = len(list(set(y_true)))
+
+                false_positives = []
+                for i in range(num_classes):
+                    false_positives.append(sum(cm[:,i]) - cm[i,i])
+
+                false_negatives = []
+                for i in range(num_classes):
+                    false_negatives.append(sum(cm[i,:]) - cm[i,i])
+
+                true_negatives = []
+                for i in range(num_classes):
+                    temp = np.delete(cm, i, 0)   # delete ith row
+                    temp = np.delete(temp, i, 1)  # delete ith column
+                    true_negatives.append(sum(sum(temp)))
+
+                denominator = [sum(x) for x in zip(false_positives, true_negatives)]
+                false_positive_rate = [num/den for num, den in zip(false_positives, denominator)]
+
+                denominator = [sum(x) for x in zip(true_positives, false_negatives)]
+                true_positive_rate = [num/den for num, den in zip(true_positives, denominator)]
+
+                return (
+                    test_loss,
+                    accuracy,
+                    f1score,
+                    precision,
+                    recall,
+                    accuracy_per_class,
+                    true_positive_rate,
+                    false_positive_rate
+                )
+
+
+    def transform_func(self,
+                       data):
+        convert_tensor = transforms.ToTensor()
+        data['image'] = [convert_tensor(img) for img in data['image']]
         return data
```

### Comparing `asociita-0.1.6.9/asociita/models/pytorch/mnist.py` & `asociita-0.1.7/asociita/models/pytorch/mnist.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import torch
-import torch.nn.functional as F
-from torch import Tensor, nn
-
-torch.manual_seed(42)
-
-
-class MnistNet(nn.Module):
-    """Mnist network definition."""
-
-    def __init__(self) -> None:
-        """Initialization of the network."""
-        super().__init__()
-        self.fc1 = nn.Linear(28 * 28, 50)
-        self.fc1_drop = nn.Dropout(0.2)
-        self.fc2 = nn.Linear(50, 50)
-        self.fc2_drop = nn.Dropout(0.2)
-        self.fc3 = nn.Linear(50, 10)
-
-    def forward(self, input_data: Tensor) -> Tensor:
-        """Defines the forward pass of the network.
-        Args:
-            input_data (Tensor): Input data
-        Returns
-        -------
-            Tensor: Output data
-        """
-        out = input_data.view(-1, 28 * 28)
-        out = F.relu(self.fc1(out))
-        out = self.fc1_drop(out)
-        out = F.relu(self.fc2(out))
-        out = self.fc2_drop(out)
+import torch
+import torch.nn.functional as F
+from torch import Tensor, nn
+
+torch.manual_seed(42)
+
+
+class MnistNet(nn.Module):
+    """Mnist network definition."""
+
+    def __init__(self) -> None:
+        """Initialization of the network."""
+        super().__init__()
+        self.fc1 = nn.Linear(28 * 28, 50)
+        self.fc1_drop = nn.Dropout(0.2)
+        self.fc2 = nn.Linear(50, 50)
+        self.fc2_drop = nn.Dropout(0.2)
+        self.fc3 = nn.Linear(50, 10)
+
+    def forward(self, input_data: Tensor) -> Tensor:
+        """Defines the forward pass of the network.
+        Args:
+            input_data (Tensor): Input data
+        Returns
+        -------
+            Tensor: Output data
+        """
+        out = input_data.view(-1, 28 * 28)
+        out = F.relu(self.fc1(out))
+        out = self.fc1_drop(out)
+        out = F.relu(self.fc2(out))
+        out = self.fc2_drop(out)
         return F.log_softmax(self.fc3(out), dim=1)
```

### Comparing `asociita-0.1.6.9/asociita/utils/computations.py` & `asociita-0.1.7/asociita/utils/computations.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-from collections import OrderedDict
-from typing import Any, Mapping, TypeVar
-import torch
-import itertools
-from torch import Tensor
-
-class Aggregators:
-    """Defines the Aggregators class."""
-
-    @staticmethod
-    def compute_average(shared_data: dict) -> dict[Any, Any]:
-        """This function computes the average of the weights.
-        Args:
-            shared_data (Dict): weights received from the other nodes of the cluster
-        Returns
-        -------
-            OrderedDict: the average of the weights
-        """
-        models = list(shared_data.values())
-        results: OrderedDict = OrderedDict()
-
-        for model in models:
-            for key in model:
-                if results.get(key) is None:
-                    if torch.cuda.is_available():
-                        model[key] = model[key].to("cuda:0")
-
-                    results[key] = model[key]
-                else:
-                    if torch.cuda.is_available():
-                        model[key] = model[key].to("cuda:0")
-                    results[key] = results[key].add(model[key])
-
-        for key in results:
-            results[key] = torch.div(results[key], len(models))
-        return results
-    
-
-    @staticmethod
-    def add_gradients(model_weights: OrderedDict, gradient: OrderedDict) -> OrderedDict:
-        """Adds gradients to the central weights, concluding one round of Federated Training."""
-        updated_weights = OrderedDict.fromkeys(model_weights.keys(), 0)
-        for key in model_weights:
-            updated_weights[key] = model_weights[key] - gradient[key]
-        return updated_weights
-    
-    
-    @staticmethod
-    def compute_distance_from_mean(shared_data: dict, average_weights: dict) -> dict:
-        """This function takes as input the weights received from all the nodes and
-        the average computed by the server.
-        It computes the distance between the average and
-        the weights received from each node per each layer.
-        Then it computes the mean of the distances per each layers.
-        The function returns a dictionary containing the mean of
-        the distances per each node.
-        Args:
-            shared_data (Dict): the weights received from the other nodes of the cluster
-            average_weights (Dict): the average of the weights
-        Returns
-        -------
-            Dict: a dictionary containing the mean of the distances per each node
-        """
-        distances = {}
-        for node_name, models in shared_data.items():
-            mean = []
-            for layer_name in models:
-
-                mean.append(
-                    torch.mean(
-                        torch.subtract(models[layer_name], average_weights[layer_name]),
-                    ),
-                )
-
-            distances[node_name] = torch.mean(torch.stack(mean))
-
-        return
-    
-
-class Subsets:
-    """Defines the Subsets class - a set of static methods
-    that helps with some set operations."""
-
-    @staticmethod
-    def form_superset(elements: list, 
-                      remove_empty: bool = True,
-                      return_dict: bool = True) -> list[list] | dict[tuple : None]:
-        """Given a list of elements of a length N, forms a superset of a cardinality
-        2^N, containing all the possible combinations of elements in the passed list.
-        
-        -------------
-        Args
-            elements (list): a list containing all the elements from which we want to form a superset.
-            remove_empty (bool): if True, will remove an empty set that is formally also included in the superset.
-            return_dict (bool): if True, will return the superset in a form {tuple: None} rather than [list].
-       -------------
-         Returns
-            list[list] | dict[tuple : None]"""
-        superset = list()
-        for l in range(len(elements) + 1):
-            for subset in itertools.combinations(elements, l):
-                superset.append(list(subset))
-        if remove_empty == True:
-            superset.pop(0)
-        
-        if return_dict == True:
-            superset = {tuple(coalition): None for coalition in superset}
-            return superset
-        else:
-            return superset
-    
-    @staticmethod
-    def form_loo_set(elements: list,
-                     return_dict: bool = True) -> list[list] | dict[list : None]:
-        """Given a list of elements of a length N, forms a set containing all the possible
-        lists of N and N-1 length.
-        -------------
-        Args
-            elements (list): a list containing all the elements from which we want to form a superset.
-            return_dict (bool): if True, will return the superset in a form {tuple: None} rather than [list].
-       -------------
-         Returns
-            list[list] | dict[tuple : None]"""
-        loo_set = list()
-        for l in range(len(elements) - 1, len(elements) + 1):
-            for subset in itertools.combinations(elements, l):
-                loo_set.append(list(subset))
-        
-        if return_dict == True:
-            loo_set = {tuple(coalition) : None for coalition in loo_set}
-            return loo_set
-        else:
-            return loo_set
-
-
-    def select_subsets(coalitions: dict,
-                       searched_node: int) -> dict[tuple : Any]:
-        """Given a list of possible coalitions and a searched node, will return
-        every possible coalition which DO NOT CONTAIN the searche node.
-        -------------
-        Args
-            coalitions (dict): a superset or a set of all possible coalitions, mapping
-                each coalition to some value, e.g. {(1, 2, 3,): None}
-            searched_node (int): an id of the searched node.
-       -------------
-         Returns
-            dict[tuple : Any]"""
-        subsets = {nodes: model for nodes, model in coalitions.items() 
-                  if searched_node not in nodes}
-        return subsets
+from collections import OrderedDict
+from typing import Any, Mapping, TypeVar
+import torch
+import itertools
+from torch import Tensor
+
+class Aggregators:
+    """Defines the Aggregators class."""
+
+    @staticmethod
+    def compute_average(shared_data: dict) -> dict[Any, Any]:
+        """This function computes the average of the weights.
+        Args:
+            shared_data (Dict): weights received from the other nodes of the cluster
+        Returns
+        -------
+            OrderedDict: the average of the weights
+        """
+        models = list(shared_data.values())
+        results: OrderedDict = OrderedDict()
+
+        for model in models:
+            for key in model:
+                if results.get(key) is None:
+                    if torch.cuda.is_available():
+                        model[key] = model[key].to("cuda:0")
+
+                    results[key] = model[key]
+                else:
+                    if torch.cuda.is_available():
+                        model[key] = model[key].to("cuda:0")
+                    results[key] = results[key].add(model[key])
+
+        for key in results:
+            results[key] = torch.div(results[key], len(models))
+        return results
+    
+
+    @staticmethod
+    def add_gradients(model_weights: OrderedDict, gradient: OrderedDict) -> OrderedDict:
+        """Adds gradients to the central weights, concluding one round of Federated Training."""
+        updated_weights = OrderedDict.fromkeys(model_weights.keys(), 0)
+        for key in model_weights:
+            updated_weights[key] = model_weights[key] - gradient[key]
+        return updated_weights
+    
+    
+    @staticmethod
+    def compute_distance_from_mean(shared_data: dict, average_weights: dict) -> dict:
+        """This function takes as input the weights received from all the nodes and
+        the average computed by the server.
+        It computes the distance between the average and
+        the weights received from each node per each layer.
+        Then it computes the mean of the distances per each layers.
+        The function returns a dictionary containing the mean of
+        the distances per each node.
+        Args:
+            shared_data (Dict): the weights received from the other nodes of the cluster
+            average_weights (Dict): the average of the weights
+        Returns
+        -------
+            Dict: a dictionary containing the mean of the distances per each node
+        """
+        distances = {}
+        for node_name, models in shared_data.items():
+            mean = []
+            for layer_name in models:
+
+                mean.append(
+                    torch.mean(
+                        torch.subtract(models[layer_name], average_weights[layer_name]),
+                    ),
+                )
+
+            distances[node_name] = torch.mean(torch.stack(mean))
+
+        return
+    
+
+class Subsets:
+    """Defines the Subsets class - a set of static methods
+    that helps with some set operations."""
+
+    @staticmethod
+    def form_superset(elements: list, 
+                      remove_empty: bool = True,
+                      return_dict: bool = True) -> list[list] | dict[tuple : None]:
+        """Given a list of elements of a length N, forms a superset of a cardinality
+        2^N, containing all the possible combinations of elements in the passed list.
+        
+        -------------
+        Args
+            elements (list): a list containing all the elements from which we want to form a superset.
+            remove_empty (bool): if True, will remove an empty set that is formally also included in the superset.
+            return_dict (bool): if True, will return the superset in a form {tuple: None} rather than [list].
+       -------------
+         Returns
+            list[list] | dict[tuple : None]"""
+        superset = list()
+        for l in range(len(elements) + 1):
+            for subset in itertools.combinations(elements, l):
+                superset.append(list(subset))
+        if remove_empty == True:
+            superset.pop(0)
+        
+        if return_dict == True:
+            superset = {tuple(coalition): None for coalition in superset}
+            return superset
+        else:
+            return superset
+    
+    @staticmethod
+    def form_loo_set(elements: list,
+                     return_dict: bool = True) -> list[list] | dict[list : None]:
+        """Given a list of elements of a length N, forms a set containing all the possible
+        lists of N and N-1 length.
+        -------------
+        Args
+            elements (list): a list containing all the elements from which we want to form a superset.
+            return_dict (bool): if True, will return the superset in a form {tuple: None} rather than [list].
+       -------------
+         Returns
+            list[list] | dict[tuple : None]"""
+        loo_set = list()
+        for l in range(len(elements) - 1, len(elements) + 1):
+            for subset in itertools.combinations(elements, l):
+                loo_set.append(list(subset))
+        
+        if return_dict == True:
+            loo_set = {tuple(coalition) : None for coalition in loo_set}
+            return loo_set
+        else:
+            return loo_set
+
+
+    def select_subsets(coalitions: dict,
+                       searched_node: int) -> dict[tuple : Any]:
+        """Given a list of possible coalitions and a searched node, will return
+        every possible coalition which DO NOT CONTAIN the searche node.
+        -------------
+        Args
+            coalitions (dict): a superset or a set of all possible coalitions, mapping
+                each coalition to some value, e.g. {(1, 2, 3,): None}
+            searched_node (int): an id of the searched node.
+       -------------
+         Returns
+            dict[tuple : Any]"""
+        subsets = {nodes: model for nodes, model in coalitions.items() 
+                  if searched_node not in nodes}
+        return subsets
```

### Comparing `asociita-0.1.6.9/asociita/utils/custom_transformations.py` & `asociita-0.1.7/asociita/utils/custom_transformations.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Any
-import torch.random
-
-
-class AddGaussianNoise(object):
-    def __init__(self, 
-                 mean=0., 
-                 std=1.,
-                 noise_multiplication: float = 0.5) -> None:
-        self.std = std
-        self.mean = mean
-        self.noise_multiplication = noise_multiplication
-    
-
-    def __call__(self, 
-                 tensor) -> Any:
-        return tensor + self.noise_multiplication * (torch.randn(tensor.size()) * self.std + self.mean)
-    
-
-    def __repr__(self) -> str:
+from typing import Any
+import torch.random
+
+
+class AddGaussianNoise(object):
+    def __init__(self, 
+                 mean=0., 
+                 std=1.,
+                 noise_multiplication: float = 0.5) -> None:
+        self.std = std
+        self.mean = mean
+        self.noise_multiplication = noise_multiplication
+    
+
+    def __call__(self, 
+                 tensor) -> Any:
+        return tensor + self.noise_multiplication * (torch.randn(tensor.size()) * self.std + self.mean)
+    
+
+    def __repr__(self) -> str:
         return self.__class__.__name__ + '(mean={0}, std={1})'.format(self.mean, self.std)
```

### Comparing `asociita-0.1.6.9/asociita/utils/handlers.py` & `asociita-0.1.7/asociita/utils/handlers.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-from asociita.components.nodes.federated_node import FederatedNode
-import logging, csv
-from typing import Any
-import os
-
-class Handler:
-    """Common class for various utilities handling the data logs."""
-    @staticmethod
-    def log_model_metrics(iteration: int, 
-                          model: Any,
-                          logger,
-                          ) -> None:
-        """Used to log the model's metrics (on the orchestrator level).
-        
-        Args:
-            iteration (int): Current iteration of the training.
-            node_id (FederatedNode object): Federated Node object that we want to evaluate metrics on.
-        """
-        try:
-            (
-                loss,
-                accuracy,
-                fscore,
-                precision,
-                recall,
-                test_accuracy_per_class,
-                true_positive_rate,
-                false_positive_rate
-            ) = model.evaluate_model()
-            metrics = {"loss":loss, 
-                        "accuracy": accuracy, 
-                        "fscore": fscore, 
-                        "precision": precision,
-                        "recall": recall, 
-                        "test_accuracy_per_class": test_accuracy_per_class, 
-                        "true_positive_rate": true_positive_rate,
-                        "false_positive_rate": false_positive_rate,
-                        "epoch": iteration}
-            logger.info(f"Evaluating model after iteration {iteration} on node {model.node_name}. Results: {metrics}")
-        except Exception as e:
-            logger.warning(f"Unable to compute metrics. {e}")
-    
-
-    @staticmethod
-    def save_model_metrics(iteration: int, 
-                           model: Any,
-                           logger = None,
-                           saving_path: str = None,
-                           file_name: str = 'metrics.csv',
-                           log_to_screen: bool = False) -> None:
-        """Used to save the model metrics.
-        Args:
-            - iteration (int): Current iteration of the training.
-            - node (FederatedNode): FederatedNode Object which metrics we want to save.
-            - participants (list[int]): List of id's of participants
-                that are participating in this simulation. By default,
-                it will be equal to all available nodes -> self.nodes_id
-            - saving_path (str or path-like object): the saving path of the
-                csv file - if none, the file will be saved in the current 
-                working directory.
-            - file_name (str): a desired file name for the metrics, default to
-                'metrics.csv'.
-        Returns:
-            None"""
-        try:
-            (
-                loss,
-                accuracy,
-                fscore,
-                precision,
-                recall,
-                test_accuracy_per_class,
-                true_positive_rate,
-                false_positive_rate
-            ) = model.evaluate_model()
-            metrics = {"epoch": iteration,
-                       "node": model.node_name,
-                        "loss":loss, 
-                        "accuracy": accuracy, 
-                        "fscore": fscore, 
-                        "precision": precision,
-                        "recall": recall, 
-                        "test_accuracy_per_class": test_accuracy_per_class, 
-                        "true_positive_rate": true_positive_rate,
-                        "false_positive_rate": false_positive_rate,
-                        "epoch": iteration}
-            if log_to_screen == True:
-                logger.info(f"Evaluating model after iteration {iteration} on node {model.node_name}. Results: {metrics}")
-        except Exception as e:
-            logger.warning(f"Unable to compute metrics. {e}")
-        path = os.path.join(saving_path, file_name)
-        with open(path, 'a+', newline='') as saved_file:
-                writer = csv.DictWriter(saved_file, list(metrics.keys()))
-                if os.path.getsize(path) == 0:
-                    writer.writeheader()
-                writer.writerow(metrics)
-    
-    
-    @staticmethod
-    def save_csv_file(file,
-                      saving_path: str = None,
-                      file_name: str = 'metrics.csv') -> None:
-        """Used to preserve the content of a csv file."""
-        path = os.path.join(saving_path, file_name)
-        with open(path, 'a+', newline='') as csv_file:
-            writer = csv.DictWriter(csv_file, list(file[0].keys()))
-            writer.writeheader()
-            for row in file:
+from asociita.components.nodes.federated_node import FederatedNode
+import logging, csv
+from typing import Any
+import os
+
+class Handler:
+    """Common class for various utilities handling the data logs."""
+    @staticmethod
+    def log_model_metrics(iteration: int, 
+                          model: Any,
+                          logger,
+                          ) -> None:
+        """Used to log the model's metrics (on the orchestrator level).
+        
+        Args:
+            iteration (int): Current iteration of the training.
+            node_id (FederatedNode object): Federated Node object that we want to evaluate metrics on.
+        """
+        try:
+            (
+                loss,
+                accuracy,
+                fscore,
+                precision,
+                recall,
+                test_accuracy_per_class,
+                true_positive_rate,
+                false_positive_rate
+            ) = model.evaluate_model()
+            metrics = {"loss":loss, 
+                        "accuracy": accuracy, 
+                        "fscore": fscore, 
+                        "precision": precision,
+                        "recall": recall, 
+                        "test_accuracy_per_class": test_accuracy_per_class, 
+                        "true_positive_rate": true_positive_rate,
+                        "false_positive_rate": false_positive_rate,
+                        "epoch": iteration}
+            logger.info(f"Evaluating model after iteration {iteration} on node {model.node_name}. Results: {metrics}")
+        except Exception as e:
+            logger.warning(f"Unable to compute metrics. {e}")
+    
+
+    @staticmethod
+    def save_model_metrics(iteration: int, 
+                           model: Any,
+                           logger = None,
+                           saving_path: str = None,
+                           file_name: str = 'metrics.csv',
+                           log_to_screen: bool = False) -> None:
+        """Used to save the model metrics.
+        Args:
+            - iteration (int): Current iteration of the training.
+            - node (FederatedNode): FederatedNode Object which metrics we want to save.
+            - participants (list[int]): List of id's of participants
+                that are participating in this simulation. By default,
+                it will be equal to all available nodes -> self.nodes_id
+            - saving_path (str or path-like object): the saving path of the
+                csv file - if none, the file will be saved in the current 
+                working directory.
+            - file_name (str): a desired file name for the metrics, default to
+                'metrics.csv'.
+        Returns:
+            None"""
+        try:
+            (
+                loss,
+                accuracy,
+                fscore,
+                precision,
+                recall,
+                test_accuracy_per_class,
+                true_positive_rate,
+                false_positive_rate
+            ) = model.evaluate_model()
+            metrics = {"epoch": iteration,
+                       "node": model.node_name,
+                        "loss":loss, 
+                        "accuracy": accuracy, 
+                        "fscore": fscore, 
+                        "precision": precision,
+                        "recall": recall, 
+                        "test_accuracy_per_class": test_accuracy_per_class, 
+                        "true_positive_rate": true_positive_rate,
+                        "false_positive_rate": false_positive_rate,
+                        "epoch": iteration}
+            if log_to_screen == True:
+                logger.info(f"Evaluating model after iteration {iteration} on node {model.node_name}. Results: {metrics}")
+        except Exception as e:
+            logger.warning(f"Unable to compute metrics. {e}")
+        path = os.path.join(saving_path, file_name)
+        with open(path, 'a+', newline='') as saved_file:
+                writer = csv.DictWriter(saved_file, list(metrics.keys()))
+                if os.path.getsize(path) == 0:
+                    writer.writeheader()
+                writer.writerow(metrics)
+    
+    
+    @staticmethod
+    def save_csv_file(file,
+                      saving_path: str = None,
+                      file_name: str = 'metrics.csv') -> None:
+        """Used to preserve the content of a csv file."""
+        path = os.path.join(saving_path, file_name)
+        with open(path, 'a+', newline='') as csv_file:
+            writer = csv.DictWriter(csv_file, list(file[0].keys()))
+            writer.writeheader()
+            for row in file:
                 writer.writerow(row)
```

### Comparing `asociita-0.1.6.9/asociita/utils/helpers.py` & `asociita-0.1.7/asociita/utils/helpers.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import json
-
-
-class Helpers:
-    @staticmethod
-    def load_from_json(path: 'str', convert_keys: bool = False) -> dict:
-        with open(path, 'r') as json_file:
-            data = json.load(json_file)
-        if convert_keys == True:
-            if data.get('transformations'):
-                data['transformations'] = {int(key): value for key, value in data['transformations'].items()}
-            if data.get('imbalanced_clients'):
-                data['imbalanced_clients'] = {int(key): value for key, value in data['imbalanced_clients'].items()}
+import json
+
+
+class Helpers:
+    @staticmethod
+    def load_from_json(path: 'str', convert_keys: bool = False) -> dict:
+        with open(path, 'r') as json_file:
+            data = json.load(json_file)
+        if convert_keys == True:
+            if data.get('transformations'):
+                data['transformations'] = {int(key): value for key, value in data['transformations'].items()}
+            if data.get('imbalanced_clients'):
+                data['imbalanced_clients'] = {int(key): value for key, value in data['imbalanced_clients'].items()}
         return data
```

### Comparing `asociita-0.1.6.9/asociita/utils/loggers.py` & `asociita-0.1.7/asociita/utils/loggers.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import logging
-
-Orchestrator_logger = logging.getLogger("")
-
-
-# create loggers
-class Loggers:
-    @staticmethod
-    def orchestrator_logger():
-        # Creating a head logger for the orchestrator
-        orchestrator_logger = logging.getLogger("orchestrator_logger")
-        orchestrator_logger.setLevel(logging.DEBUG)
-        formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-        orchestrator_logger.debug("The default level of Orchestrator logger is set to: DEFAULT.")
-        ch = logging.StreamHandler()
-        ch.setLevel(logging.DEBUG)
-        ch.setFormatter(formatter)
-        orchestrator_logger.addHandler(ch)
-        return orchestrator_logger
-    
-
-    @staticmethod
-    def node_logger():
-        # Creating a head logger for the nodes
-        node_logger = logging.getLogger("node_logger")
-        node_logger.setLevel(logging.DEBUG)
-        formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-        node_logger.debug("The default level of Orchestrator logger is set to: DEFAULT.")
-        zh = logging.StreamHandler()
-        zh.setLevel(logging.DEBUG)
-        zh.setFormatter(formatter)
-        node_logger.addHandler(zh)
-        return node_logger
-    
-
-    @staticmethod
-    def model_logger():
-        # Creating a head loger for the models
-        model_logger = logging.getLogger("model_logger")
-        model_logger.setLevel(logging.DEBUG)
-        formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
-        model_logger.debug("The default level of Orchestrator logger is set to: DEFAULT.")
-        sh = logging.StreamHandler()
-        sh.setLevel(logging.DEBUG)
-        sh.setFormatter(formatter)
-        model_logger.addHandler(sh)
-        return model_logger
+import logging
+
+Orchestrator_logger = logging.getLogger("")
+
+
+# create loggers
+class Loggers:
+    @staticmethod
+    def orchestrator_logger():
+        # Creating a head logger for the orchestrator
+        orchestrator_logger = logging.getLogger("orchestrator_logger")
+        orchestrator_logger.setLevel(logging.DEBUG)
+        formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+        orchestrator_logger.debug("The default level of Orchestrator logger is set to: DEFAULT.")
+        ch = logging.StreamHandler()
+        ch.setLevel(logging.DEBUG)
+        ch.setFormatter(formatter)
+        orchestrator_logger.addHandler(ch)
+        return orchestrator_logger
+    
+
+    @staticmethod
+    def node_logger():
+        # Creating a head logger for the nodes
+        node_logger = logging.getLogger("node_logger")
+        node_logger.setLevel(logging.DEBUG)
+        formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+        node_logger.debug("The default level of Orchestrator logger is set to: DEFAULT.")
+        zh = logging.StreamHandler()
+        zh.setLevel(logging.DEBUG)
+        zh.setFormatter(formatter)
+        node_logger.addHandler(zh)
+        return node_logger
+    
+
+    @staticmethod
+    def model_logger():
+        # Creating a head loger for the models
+        model_logger = logging.getLogger("model_logger")
+        model_logger.setLevel(logging.DEBUG)
+        formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+        model_logger.debug("The default level of Orchestrator logger is set to: DEFAULT.")
+        sh = logging.StreamHandler()
+        sh.setLevel(logging.DEBUG)
+        sh.setFormatter(formatter)
+        model_logger.addHandler(sh)
+        return model_logger
```

### Comparing `asociita-0.1.6.9/asociita/utils/orchestrations.py` & `asociita-0.1.7/asociita/utils/orchestrations.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-from typing import Any, Tuple, List, Dict, AnyStr, Union
-from asociita.components.nodes.federated_node import FederatedNode
-from asociita.models.pytorch.federated_model import FederatedModel
-import datasets
-from logging import Logger
-import random
-
-def prepare_nodes(node: FederatedNode, 
-                 model: Any,
-                 dataset: list[datasets.arrow_dataset.Dataset, 
-                               datasets.arrow_dataset.Dataset],
-                query) -> AnyStr:
-    """Used to connect the node and prepare it for training.
-    Updates instances of a FederatedNode object and
-    puts it into communication_queue.
-    
-    -------------
-    Args:
-        node (int): ID of the node that we want to connect.
-        model (Any): Compiled or pre-compiled model to be trained.
-        dataset (list[datasets.arrow_dataset.Dataset, 
-                datasets.arrow_dataset.Dataset]): A dataset in the
-                format ["train_data", "test_data"] that will be used 
-                by the selected node.
-        comunication_queue (multiprocess.Manager.Queue): Communication queue.
-    -------------
-    Returns:
-        message(str): "OK" """
-    node.prepare_node(model=model, data=dataset)
-    query.put(node)
-    return "OK"
-
-
-def create_nodes(node_id: int, 
-                nodes_settings) -> list[FederatedNode]: 
-    """Creates a list of nodes that will be connected to the 
-    orchestrator and contained in a list[FederatedNode] container.
-    -------------
-    Args:
-        node (int): ID of the node that we want to connect.
-    -------------
-    Returns:
-        list[FederatedNode]: List of nodes that were created.
-    """
-    nodes = [FederatedNode(id, nodes_settings) for id in node_id]
-    return nodes
-
-
-def check_health(node: FederatedNode,
-                 orchestrator_logger: Logger) -> bool:
-    """Checks whether node has successfully conducted the transaction
-    and can be moved to the next phase of the training. According to the
-    adopted standard - if node.state == 0, node is ready for the next
-    transaction. On the contrary, if node.state == 1, then node must be 
-    excluded from the simulation (internal error).
-    -------------
-    Args:
-        node (FederatedNode): FederatedNode object
-    -------------
-    Returns:
-        bool(): True if node is healthy, False otherwise."""
-    if node.state == 0:
-        orchestrator_logger.warning(f"Node {node.node_id} was updated successfully.")
-        return True
-    else:
-        orchestrator_logger.warning(f"Node {node.node_id} failed during the update.")
-        return False
-
-
-def sample_nodes(nodes: list[FederatedNode], 
-                 sample_size: int,
-                 orchestrator_logger: Logger) -> list[FederatedNode]:
-    """Sample the nodes given the provided sample size. If sample_size is bigger
-    or equal to the number of av. nodes, the sampler will return the original list.
-     -------------
-    Args:
-        nodes (list[FederatedNode]): original list of nodes to be sampled from
-        sample_size (int): size of the sample.
-    -------------
-    Returns:
-        list[FederatedNode]: List of sampled nodes."""
-    if len(nodes) <= sample_size:
-        orchestrator_logger.warning("Sample size should be smaller than the size of the population, returning the original list")
-        return nodes
-    else:
-        sample = random.sample(nodes, sample_size)
-        return sample
-
-
-def train_nodes(node: FederatedNode, 
-                mode: str = 'weights') -> tuple[int, List[float]]:
-    """Used to command the node to start the local training.
-    Invokes .train_local_model method and returns the results.
-    -------------
-    Args:
-        node (FederatedNode object): Node that we want to train.
-        mode (str): Mode of the training. 
-            Mode = 'weights': Node will return model's weights.
-            Mode = 'gradients': Node will return model's gradients.
-    -------------
-    Returns:
-        tuple(node_id: str, weights)"""
-    node_id, weights = node.train_local_model(mode = mode)
+from typing import Any, Tuple, List, Dict, AnyStr, Union
+from asociita.components.nodes.federated_node import FederatedNode
+from asociita.models.pytorch.federated_model import FederatedModel
+import datasets
+from logging import Logger
+import random
+
+def prepare_nodes(node: FederatedNode, 
+                 model: Any,
+                 dataset: list[datasets.arrow_dataset.Dataset, 
+                               datasets.arrow_dataset.Dataset],
+                query) -> AnyStr:
+    """Used to connect the node and prepare it for training.
+    Updates instances of a FederatedNode object and
+    puts it into communication_queue.
+    
+    -------------
+    Args:
+        node (int): ID of the node that we want to connect.
+        model (Any): Compiled or pre-compiled model to be trained.
+        dataset (list[datasets.arrow_dataset.Dataset, 
+                datasets.arrow_dataset.Dataset]): A dataset in the
+                format ["train_data", "test_data"] that will be used 
+                by the selected node.
+        comunication_queue (multiprocess.Manager.Queue): Communication queue.
+    -------------
+    Returns:
+        message(str): "OK" """
+    node.prepare_node(model=model, data=dataset)
+    query.put(node)
+    return "OK"
+
+
+def create_nodes(node_id: int, 
+                nodes_settings) -> list[FederatedNode]: 
+    """Creates a list of nodes that will be connected to the 
+    orchestrator and contained in a list[FederatedNode] container.
+    -------------
+    Args:
+        node (int): ID of the node that we want to connect.
+    -------------
+    Returns:
+        list[FederatedNode]: List of nodes that were created.
+    """
+    nodes = [FederatedNode(id, nodes_settings) for id in node_id]
+    return nodes
+
+
+def check_health(node: FederatedNode,
+                 orchestrator_logger: Logger) -> bool:
+    """Checks whether node has successfully conducted the transaction
+    and can be moved to the next phase of the training. According to the
+    adopted standard - if node.state == 0, node is ready for the next
+    transaction. On the contrary, if node.state == 1, then node must be 
+    excluded from the simulation (internal error).
+    -------------
+    Args:
+        node (FederatedNode): FederatedNode object
+    -------------
+    Returns:
+        bool(): True if node is healthy, False otherwise."""
+    if node.state == 0:
+        orchestrator_logger.warning(f"Node {node.node_id} was updated successfully.")
+        return True
+    else:
+        orchestrator_logger.warning(f"Node {node.node_id} failed during the update.")
+        return False
+
+
+def sample_nodes(nodes: list[FederatedNode], 
+                 sample_size: int,
+                 orchestrator_logger: Logger) -> list[FederatedNode]:
+    """Sample the nodes given the provided sample size. If sample_size is bigger
+    or equal to the number of av. nodes, the sampler will return the original list.
+     -------------
+    Args:
+        nodes (list[FederatedNode]): original list of nodes to be sampled from
+        sample_size (int): size of the sample.
+    -------------
+    Returns:
+        list[FederatedNode]: List of sampled nodes."""
+    if len(nodes) <= sample_size:
+        orchestrator_logger.warning("Sample size should be smaller than the size of the population, returning the original list")
+        return nodes
+    else:
+        sample = random.sample(nodes, sample_size)
+        return sample
+
+
+def train_nodes(node: FederatedNode, 
+                mode: str = 'weights') -> tuple[int, List[float]]:
+    """Used to command the node to start the local training.
+    Invokes .train_local_model method and returns the results.
+    -------------
+    Args:
+        node (FederatedNode object): Node that we want to train.
+        mode (str): Mode of the training. 
+            Mode = 'weights': Node will return model's weights.
+            Mode = 'gradients': Node will return model's gradients.
+    -------------
+    Returns:
+        tuple(node_id: str, weights)"""
+    node_id, weights = node.train_local_model(mode = mode)
     return (node_id, weights)
```

### Comparing `asociita-0.1.6.9/asociita/utils/showcase.py` & `asociita-0.1.7/asociita/utils/showcase.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import matplotlib.pyplot as plt
-import numpy as np
-from PIL import Image
-import random
-
-
-def show_image(img):
-    img = np.asarray(img)
-    plt.imshow(img)
-
-
-def show_random(imgs_orig, imgs_transformed):
-    fig, ax = plt.subplots(2, 5)
-    for position in range(5):
-        random_pos = random.randint(0, len(imgs_orig) - 1)
-        original_img = np.asarray(imgs_orig[random_pos])
-        transformed_img = np.asarray(imgs_transformed[random_pos])
-        ax[0][position].imshow(original_img)
-        ax[1][position].imshow(transformed_img)
-    plt.show()
-
-
-def save_random(imgs_orig, imgs_transformed, transformation: str):
-    fig, ax = plt.subplots(2, 5)
-    for position in range(5):
-        random_pos = random.randint(0, len(imgs_orig) - 1)
-        original_img = np.asarray(imgs_orig[random_pos])
-        transformed_img = np.asarray(imgs_transformed[random_pos])
-        ax[0][position].imshow(original_img)
-        ax[1][position].imshow(transformed_img)
-    title = transformation + '.pdf'
-    plt.savefig(title)
-
+import matplotlib.pyplot as plt
+import numpy as np
+from PIL import Image
+import random
+
+
+def show_image(img):
+    img = np.asarray(img)
+    plt.imshow(img)
+
+
+def show_random(imgs_orig, imgs_transformed):
+    fig, ax = plt.subplots(2, 5)
+    for position in range(5):
+        random_pos = random.randint(0, len(imgs_orig) - 1)
+        original_img = np.asarray(imgs_orig[random_pos])
+        transformed_img = np.asarray(imgs_transformed[random_pos])
+        ax[0][position].imshow(original_img)
+        ax[1][position].imshow(transformed_img)
+    plt.show()
+
+
+def save_random(imgs_orig, imgs_transformed, transformation: str):
+    fig, ax = plt.subplots(2, 5)
+    for position in range(5):
+        random_pos = random.randint(0, len(imgs_orig) - 1)
+        original_img = np.asarray(imgs_orig[random_pos])
+        transformed_img = np.asarray(imgs_transformed[random_pos])
+        ax[0][position].imshow(original_img)
+        ax[1][position].imshow(transformed_img)
+    title = transformation + '.pdf'
+    plt.savefig(title)
+
```

### Comparing `asociita-0.1.6.9/LICENSE` & `asociita-0.1.7/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Scolpe
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Scolpe
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `asociita-0.1.6.9/README.md` & `asociita-0.1.7/README.md`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-### Setting Configuration
-
-In order to run the simulation, the `Orchestrator` instance must receive a `settings` object that contains all the necessary parameters. It is possible to store those parameters in a `JSON` format and load them as the Python dictionary by using `asociita.utils.helper.load_from_json` function. Below is an exemplary settings object embedded as a `json` file. All the elements are necessary unless stated otherwise.
-
-```
-{
-    "orchestrator":{
-        "iterations": int,
-        "number_of_nodes": int,
-        "local_warm_start": bool,
-        "sample_size": int,
-        "evaluation": "none" | "full"
-        "save_metrics": bool,
-	"save_models": bool,
-	"save_path": str
-	"nodes": [0,
-	1,
-	2]
-    },
-    "nodes":{
-    "local_epochs": int,
-    "model_settings": {
-        "optimizer": "RMS",
-        "batch_size": int,
-        "learning_rate": float}
-        }
-}
-```
-
-The `settings` contains two dictionaries: `orchestrator` and `nodes`.
-
-`orchestrator` contains all the settings necessary details of the training:
-
-* `iterations` is the number of rounds to be performed. Example: `iterations:12`
-* `number_of_nodes` is the number of nodes that will be included in the training. Example: `number_of_nodes: 10`
-* `local_warm_start` allows to distribute various pre-trained weights to different local clients. Not implemeneted yet. Example: `local_warm_start: false`.
-* `sample_size` is the size of the sample that will be taken each round. Example: `sample_size : 4.`
-* `evaluation` allows to control the evaluation procedure across the clients.  Currently, only `none` or `full` are supported. Setting the evaluation to full will perform a full evaluation of every client included in the training. Example: `evaluation: full`
-* `save_metrics` allows to control whether the metrics should be saved in a csv file. Example: `save_metrics: true.`
-* `save_models` allows to control whether the models should be saved. Not implemeneted yet. Example: `save_metrics: false`.
-* `save_path` is the system path that will be used when saving the model. It is possible to define a saving_path in a method call.
-* `nodes` is the list containing the ids of all the nodes participating in the training. Length of `nodes` must be equal `number_of_nodes`.
-
-`nodes` contains all the necessary configuration for nodes.
-
-* `"local_epochs":` the number of local epochs to be performed on the local nodes.
-* `"model_settings"` is a dictionary containing all the parameters for training the model.
-  * `optimizer` is an optimizer that will be used during the training. Example: `optimizer: "RMS"`
-  * `batch_size` is the batch size that will be used during the training. Example: `batch_size: 32`
-  * `learning_rate` is the learning rate that will be used during the training. Example: `learning_rate: 0.001`
+### Setting Configuration
+
+In order to run the simulation, the `Orchestrator` instance must receive a `settings` object that contains all the necessary parameters. It is possible to store those parameters in a `JSON` format and load them as the Python dictionary by using `asociita.utils.helper.load_from_json` function. Below is an exemplary settings object embedded as a `json` file. All the elements are necessary unless stated otherwise.
+
+```
+{
+    "orchestrator":{
+        "iterations": int,
+        "number_of_nodes": int,
+        "local_warm_start": bool,
+        "sample_size": int,
+        "evaluation": "none" | "full"
+        "save_metrics": bool,
+	"save_models": bool,
+	"save_path": str
+	"nodes": [0,
+	1,
+	2]
+    },
+    "nodes":{
+    "local_epochs": int,
+    "model_settings": {
+        "optimizer": "RMS",
+        "batch_size": int,
+        "learning_rate": float}
+        }
+}
+```
+
+The `settings` contains two dictionaries: `orchestrator` and `nodes`.
+
+`orchestrator` contains all the settings necessary details of the training:
+
+* `iterations` is the number of rounds to be performed. Example: `iterations:12`
+* `number_of_nodes` is the number of nodes that will be included in the training. Example: `number_of_nodes: 10`
+* `local_warm_start` allows to distribute various pre-trained weights to different local clients. Not implemeneted yet. Example: `local_warm_start: false`.
+* `sample_size` is the size of the sample that will be taken each round. Example: `sample_size : 4.`
+* `evaluation` allows to control the evaluation procedure across the clients.  Currently, only `none` or `full` are supported. Setting the evaluation to full will perform a full evaluation of every client included in the training. Example: `evaluation: full`
+* `save_metrics` allows to control whether the metrics should be saved in a csv file. Example: `save_metrics: true.`
+* `save_models` allows to control whether the models should be saved. Not implemeneted yet. Example: `save_metrics: false`.
+* `save_path` is the system path that will be used when saving the model. It is possible to define a saving_path in a method call.
+* `nodes` is the list containing the ids of all the nodes participating in the training. Length of `nodes` must be equal `number_of_nodes`.
+
+`nodes` contains all the necessary configuration for nodes.
+
+* `"local_epochs":` the number of local epochs to be performed on the local nodes.
+* `"model_settings"` is a dictionary containing all the parameters for training the model.
+  * `optimizer` is an optimizer that will be used during the training. Example: `optimizer: "RMS"`
+  * `batch_size` is the batch size that will be used during the training. Example: `batch_size: 32`
+  * `learning_rate` is the learning rate that will be used during the training. Example: `learning_rate: 0.001`
```

### Comparing `asociita-0.1.6.9/PKG-INFO` & `asociita-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asociita
-Version: 0.1.6.9
+Version: 0.1.7
 Summary: An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting.
 Home-page: https://github.com/Scolpe/Asociita
 License: MIT
 Author: Maciej Zuziak
 Author-email: maciejkrzysztof.zuziak@isti.cnr.it
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

