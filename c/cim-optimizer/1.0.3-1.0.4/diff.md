# Comparing `tmp/cim-optimizer-1.0.3.tar.gz` & `tmp/cim-optimizer-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cim-optimizer-1.0.3.tar", last modified: Thu Nov  3 15:27:18 2022, max compression
+gzip compressed data, was "cim-optimizer-1.0.4.tar", last modified: Wed May 31 17:04:32 2023, max compression
```

## Comparing `cim-optimizer-1.0.3.tar` & `cim-optimizer-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2022-11-03 15:27:18.707888 cim-optimizer-1.0.3/
--rw-rw-rw-   0        0        0    19051 2022-11-03 00:36:05.000000 cim-optimizer-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     7244 2022-11-03 15:27:18.706884 cim-optimizer-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     6633 2022-11-03 15:24:35.000000 cim-optimizer-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2022-11-03 15:27:18.680619 cim-optimizer-1.0.3/cim_optimizer/
--rw-rw-rw-   0        0        0     6853 2022-11-03 00:36:04.000000 cim-optimizer-1.0.3/cim_optimizer/AHC.py
--rw-rw-rw-   0        0        0     4882 2022-11-03 00:36:04.000000 cim-optimizer-1.0.3/cim_optimizer/AHC_tuning.py
--rw-rw-rw-   0        0        0     7211 2022-11-03 00:36:04.000000 cim-optimizer-1.0.3/cim_optimizer/CAC.py
--rw-rw-rw-   0        0        0     5895 2022-11-03 00:36:04.000000 cim-optimizer-1.0.3/cim_optimizer/CAC_tuning.py
--rw-rw-rw-   0        0        0     3300 2022-11-03 00:36:04.000000 cim-optimizer-1.0.3/cim_optimizer/CIM_helper.py
--rw-rw-rw-   0        0        0      958 2022-11-03 00:36:04.000000 cim-optimizer-1.0.3/cim_optimizer/__init__.py
--rw-rw-rw-   0        0        0     9073 2022-11-03 00:36:04.000000 cim-optimizer-1.0.3/cim_optimizer/extAHC.py
--rw-rw-rw-   0        0        0     5658 2022-11-03 00:36:04.000000 cim-optimizer-1.0.3/cim_optimizer/extAHC_tuning.py
--rw-rw-rw-   0        0        0     3716 2022-11-03 00:36:04.000000 cim-optimizer-1.0.3/cim_optimizer/optimal_params.py
--rw-rw-rw-   0        0        0      169 2022-11-03 00:57:17.000000 cim-optimizer-1.0.3/cim_optimizer/setup.py
--rw-rw-rw-   0        0        0    33313 2022-11-03 00:36:04.000000 cim-optimizer-1.0.3/cim_optimizer/solve_Ising.py
-drwxrwxrwx   0        0        0        0 2022-11-03 15:27:18.704810 cim-optimizer-1.0.3/cim_optimizer.egg-info/
--rw-rw-rw-   0        0        0     7244 2022-11-03 15:27:18.000000 cim-optimizer-1.0.3/cim_optimizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      505 2022-11-03 15:27:18.000000 cim-optimizer-1.0.3/cim_optimizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-03 15:27:18.000000 cim-optimizer-1.0.3/cim_optimizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2022-11-03 15:27:18.000000 cim-optimizer-1.0.3/cim_optimizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-11-03 15:27:18.000000 cim-optimizer-1.0.3/cim_optimizer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-03 15:27:18.708903 cim-optimizer-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1126 2022-11-03 15:27:13.000000 cim-optimizer-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 17:04:32.428710 cim-optimizer-1.0.4/
+-rw-rw-rw-   0        0        0    19051 2022-11-03 00:36:05.000000 cim-optimizer-1.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     7244 2023-05-31 17:04:32.427712 cim-optimizer-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6633 2022-11-03 15:24:35.000000 cim-optimizer-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 17:04:32.410725 cim-optimizer-1.0.4/cim_optimizer/
+-rw-rw-rw-   0        0        0     6853 2022-11-03 00:36:04.000000 cim-optimizer-1.0.4/cim_optimizer/AHC.py
+-rw-rw-rw-   0        0        0     4882 2022-11-15 17:19:05.000000 cim-optimizer-1.0.4/cim_optimizer/AHC_tuning.py
+-rw-rw-rw-   0        0        0     7211 2022-11-03 00:36:04.000000 cim-optimizer-1.0.4/cim_optimizer/CAC.py
+-rw-rw-rw-   0        0        0     5895 2022-11-03 00:36:04.000000 cim-optimizer-1.0.4/cim_optimizer/CAC_tuning.py
+-rw-rw-rw-   0        0        0     3300 2022-11-03 00:36:04.000000 cim-optimizer-1.0.4/cim_optimizer/CIM_helper.py
+-rw-rw-rw-   0        0        0      958 2022-11-03 00:36:04.000000 cim-optimizer-1.0.4/cim_optimizer/__init__.py
+-rw-rw-rw-   0        0        0     9073 2022-11-03 00:36:04.000000 cim-optimizer-1.0.4/cim_optimizer/extAHC.py
+-rw-rw-rw-   0        0        0     5658 2022-11-03 00:36:04.000000 cim-optimizer-1.0.4/cim_optimizer/extAHC_tuning.py
+-rw-rw-rw-   0        0        0     3716 2022-11-03 00:36:04.000000 cim-optimizer-1.0.4/cim_optimizer/optimal_params.py
+-rw-rw-rw-   0        0        0      169 2022-11-03 00:57:17.000000 cim-optimizer-1.0.4/cim_optimizer/setup.py
+-rw-rw-rw-   0        0        0    39457 2023-05-31 16:48:02.000000 cim-optimizer-1.0.4/cim_optimizer/solve_Ising.py
+drwxrwxrwx   0        0        0        0 2023-05-31 17:04:32.425715 cim-optimizer-1.0.4/cim_optimizer.egg-info/
+-rw-rw-rw-   0        0        0     7244 2023-05-31 17:04:31.000000 cim-optimizer-1.0.4/cim_optimizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      505 2023-05-31 17:04:32.000000 cim-optimizer-1.0.4/cim_optimizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 17:04:31.000000 cim-optimizer-1.0.4/cim_optimizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-31 17:04:31.000000 cim-optimizer-1.0.4/cim_optimizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-31 17:04:31.000000 cim-optimizer-1.0.4/cim_optimizer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 17:04:32.428710 cim-optimizer-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1126 2023-05-31 17:03:05.000000 cim-optimizer-1.0.4/setup.py
```

### Comparing `cim-optimizer-1.0.3/LICENSE.txt` & `cim-optimizer-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cim-optimizer-1.0.3/PKG-INFO` & `cim-optimizer-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cim-optimizer
-Version: 1.0.3
+Version: 1.0.4
 Summary: Simulated Implementation of the Coherent Ising Machine
 Home-page: https://github.com/mcmahon-lab/cim-optimizer
 Author: McMahon Lab
 Author-email: pmcmahon@cornell.edu
 License: CC-BY-4.0 license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `cim-optimizer-1.0.3/README.md` & `cim-optimizer-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cim-optimizer-1.0.3/cim_optimizer/AHC.py` & `cim-optimizer-1.0.4/cim_optimizer/AHC.py`

 * *Files identical despite different names*

### Comparing `cim-optimizer-1.0.3/cim_optimizer/AHC_tuning.py` & `cim-optimizer-1.0.4/cim_optimizer/AHC_tuning.py`

 * *Files identical despite different names*

### Comparing `cim-optimizer-1.0.3/cim_optimizer/CAC.py` & `cim-optimizer-1.0.4/cim_optimizer/CAC.py`

 * *Files identical despite different names*

### Comparing `cim-optimizer-1.0.3/cim_optimizer/CAC_tuning.py` & `cim-optimizer-1.0.4/cim_optimizer/CAC_tuning.py`

 * *Files identical despite different names*

### Comparing `cim-optimizer-1.0.3/cim_optimizer/CIM_helper.py` & `cim-optimizer-1.0.4/cim_optimizer/CIM_helper.py`

 * *Files identical despite different names*

### Comparing `cim-optimizer-1.0.3/cim_optimizer/__init__.py` & `cim-optimizer-1.0.4/cim_optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `cim-optimizer-1.0.3/cim_optimizer/extAHC.py` & `cim-optimizer-1.0.4/cim_optimizer/extAHC.py`

 * *Files identical despite different names*

### Comparing `cim-optimizer-1.0.3/cim_optimizer/extAHC_tuning.py` & `cim-optimizer-1.0.4/cim_optimizer/extAHC_tuning.py`

 * *Files identical despite different names*

### Comparing `cim-optimizer-1.0.3/cim_optimizer/optimal_params.py` & `cim-optimizer-1.0.4/cim_optimizer/optimal_params.py`

 * *Files identical despite different names*

### Comparing `cim-optimizer-1.0.3/cim_optimizer/solve_Ising.py` & `cim-optimizer-1.0.4/cim_optimizer/solve_Ising.py`

 * *Files 18% similar despite different names*

```diff
@@ -209,15 +209,15 @@
         problem : __main__.Ising object
             Ising object corresponding to the given problem. This attribute is
             manually set by when using the nested class from an Ising object:
             >>> Ising(J, h).solve(<args>)
         target_energy : int, optional
             Assumed target/ground energy for the solver to reach, used to stop
             before num_runs runs have been completed.
-        num_runs : int, default=100
+        num_runs : int, default=1
             Maximum number of runs to attempt by the CIM, either running the
             set repeated number of repetitions or stopping if the target energy
             is met.
         num_timesteps_per_run : int, default=1000
             Roundtrip number per run, representing the number of MVM's per run.
         max_wallclock_time_allowed : int, default=10000000
             Seconds passed by the CIM before quitting if num_runs or
@@ -230,18 +230,20 @@
             fields by default.
         custom_feedback_schedule, optional
             Option to specify a custom function or array of length
             num_timesteps_per_run to use as a feedback schedule.
         custom_pump_schedule, optional
             Option to specify a custom function or array of
             length num_timesteps_per_run to use as a pump schedule.
-        hyperparameters_autotune : bool, default=True
+        hyperparameters_autotune : bool, default=False
             If True then: Based on max_wallclock_time_allowed and num_runs,
             dedicate a reasonable amount of time to finding the best
             hyperparameters to use with the CIM.
+        hyperparameters_randomtune : bool, default=True
+            If True then: Run random hyperparameter search based on num_runs.
         ahc_noext_time_step : float, default=0.05
             Time step for each iteration, based on Eq(X) of citation above.
         ahc_noext_r : float, default=0.2
             AHC hyperparameter
         ahc_noext_beta : float, default=0.05
             AHC hyperparameter
         ahc_noext_eps : float, default=0.07
@@ -333,14 +335,15 @@
         amplitude_control_scheme: NoneType = None  # Manual choice of AHC vs. CAC
         custom_feedback_schedule: NoneType = None     # Custom feedback schedule
         custom_pump_schedule: NoneType = None     # Custom pump schedule
         num_parallel_runs : int = 1
         random_number_function = np.random.normal()  # Random Number Generator Function
         # HYPERPARAMETER OPTIMIZATION SCHEME
         hyperparameters_autotune: bool = False
+        hyperparameters_randomtune: bool = True
         # AHC-NO-EXTERNAL-FIELD HYPERPARAMETERS
         ahc_noext_time_step: float = 0.05
         ahc_noext_r: float = 0.2
         ahc_noext_beta: float = 0.05
         ahc_noext_eps: float = 0.07
         ahc_noext_mu: float = 1
         ahc_noext_noise: float = 0
@@ -426,58 +429,135 @@
                 self.chosen_device = torch.device('cpu')
             # Partition number of runs specified into batches.
             num_batches = int(num_runs/self.num_parallel_runs)
             if h is None or (h == np.zeros(N)).all():  # Non-External Field Case
                 h = np.zeros(N)
                 print("No External Field Detected")
                 if self.use_CAC == False:  # AHC Case
-                    if self.hyperparameters_autotune == False: # Case in which Hyperband is not called.
+                    if self.hyperparameters_autotune == False and self.hyperparameters_randomtune == False: # Case in which Hyperband is not called.
                         # Runs the solver in z batches in parallel, and concatenates batches into one flattened run_data list.
                         for z in range(num_batches):
                             curr_batch = self.CIM_AHC_GPU()
                             for y in range(self.num_parallel_runs):
                                 run_data[z*self.num_parallel_runs + y] = [curr_batch[0][y,:], curr_batch[1][y,:,:], curr_batch[2], curr_batch[3][y,:], curr_batch[4][y,:,:]]
                             run_counter += self.num_parallel_runs
+                    elif self.hyperparameters_randomtune == True:
+                        best_rand_scaling = 0
+                        best_ahc_noext_eps = 0
+                        best_energy = 0
+                        for _ in range(10):
+                            rand_scaling = np.random.choice(np.array([0.01, 0.1, 1, 10, 100]))
+                            self.ahc_noext_eps = np.random.choice(np.array([0.0333, 0.1, 0.333, 1, 3, 10]))
+                            cached_J = self.problem.J
+                            self.problem.J = rand_scaling * self.problem.J
+                            test_batch = self.CIM_AHC_GPU()
+                            if np.amin(test_batch[3])/rand_scaling < best_energy:
+                                best_rand_scaling = rand_scaling
+                                best_ahc_noext_eps = self.ahc_noext_eps
+                                best_energy = np.amin(test_batch[3])
+                            self.problem.J = cached_J  # return J matrix back to initial value before looping
+                        print("Best combination of epsilon and scaling constant: epsilon = {}; scaling constant = {}".format(best_ahc_noext_eps, best_rand_scaling))
+                        self.ahc_noext_eps = best_ahc_noext_eps
+                        self.problem.J = rand_scaling * self.problem.J
+                        for z in range(num_batches):
+                            curr_batch = self.CIM_AHC_GPU()
+                            for y in range(self.num_parallel_runs):
+                                run_data[z*self.num_parallel_runs + y] = [curr_batch[0][y,:], curr_batch[1][y,:,:], curr_batch[2], curr_batch[3][y,:], curr_batch[4][y,:,:]]
+                            run_counter += self.num_parallel_runs
+
                     else:
                         tuned_parameters = self.tune_AHC()
                         tuned_parameters.pop('J') # Remove J matrix for OOP call.
                         print(f"Tuned parameters: {tuned_parameters}.")
                         # Runs the solver in z batches in parallel, and concatenates batches into one flattened run_data list.
                         for z in range(num_batches):
                             curr_batch = self.CIM_AHC_GPU(**tuned_parameters)
                             for y in range(self.num_parallel_runs):
                                 run_data[z*self.num_parallel_runs + y] = [curr_batch[0][y,:], curr_batch[1][y,:,:], curr_batch[2], curr_batch[3][y,:], curr_batch[4][y,:,:]]
                             run_counter += self.num_parallel_runs
                 else:
-                    if self.hyperparameters_autotune == False:
+                    if self.hyperparameters_autotune == False and self.hyperparameters_randomtune == False:
                         # Runs the solver in z batches in parallel, and concatenates batches into one flattened run_data list.
                         for z in range(num_batches):
                             curr_batch = self.CIM_CAC_GPU()
                             for y in range(self.num_parallel_runs):
                                 run_data[z*self.num_parallel_runs + y] = [curr_batch[0][y,:], curr_batch[1][y,:,:], curr_batch[2], curr_batch[3][y,:], curr_batch[4][y,:,:]]
                             run_counter += self.num_parallel_runs
+                    elif self.hyperparameters_randomtune == True:
+                        best_rand_scaling = 0
+                        best_cac_gamma = 0
+                        best_energy = 0
+                        for _ in range(10):
+                            rand_scaling = np.random.choice(np.array([0.01, 0.1, 1, 10, 100]))
+                            self.cac_gamma = np.random.choice(np.array([1e-5, 1e-4, 1e-3, 1e-2, 1e-1]))
+                            cached_J = self.problem.J
+                            self.problem.J = rand_scaling * self.problem.J
+                            test_batch = self.CIM_CAC_GPU()
+                            if np.amin(test_batch[3])/rand_scaling < best_energy:
+                                best_rand_scaling = rand_scaling
+                                best_cac_gamma = self.cac_gamma
+                                best_energy = np.amin(test_batch[3])
+                            self.problem.J = cached_J # return J matrix back to initial value before looping
+                        print("Best combination of epsilon and scaling constant: gamma = {}; scaling constant = {}".format(best_cac_gamma, best_rand_scaling))
+                        self.cac_gamma = best_cac_gamma
+                        self.problem.J = rand_scaling * self.problem.J
+                        for z in range(num_batches):
+                            curr_batch = self.CIM_CAC_GPU()
+                            for y in range(self.num_parallel_runs):
+                                run_data[z*self.num_parallel_runs + y] = [curr_batch[0][y,:], curr_batch[1][y,:,:], curr_batch[2], curr_batch[3][y,:], curr_batch[4][y,:,:]]
+                            run_counter += self.num_parallel_runs
                     else:
                         tuned_parameters = self.tune_CAC()
                         tuned_parameters.pop('J') # remove J matrix for OOP call
                         print(f"Tuned parameters: {tuned_parameters}.")
                         # Runs the solver in z batches in parallel, and concatenates batches into one flattened run_data list.
                         for z in range(num_batches):
                             curr_batch = self.CIM_CAC_GPU(**tuned_parameters)
                             for y in range(self.num_parallel_runs):
                                 run_data[z*self.num_parallel_runs + y] = [curr_batch[0][y,:], curr_batch[1][y,:,:], curr_batch[2], curr_batch[3][y,:], curr_batch[4][y,:,:]]
                             run_counter += self.num_parallel_runs
             else:  # External-Field Case
                 print("External Field Detected")
-                if self.hyperparameters_autotune == False:
+                if self.hyperparameters_autotune == False and self.hyperparameters_randomtune == False:
                     # Runs the solver in z batches in parallel, and concatenates batches into one flattened run_data list.
                     for z in range(num_batches):
                         curr_batch = self.CIM_ext_f_AHC_GPU()
                         for y in range(self.num_parallel_runs):
                             run_data[z*self.num_parallel_runs + y] = [curr_batch[0][y,:], curr_batch[1][y,:,:], curr_batch[2], curr_batch[3][y,:], curr_batch[4][y,:,:]]
                         run_counter += self.num_parallel_runs
+                elif self.hyperparameters_randomtune == True:
+                        best_rand_scaling = 0
+                        best_ahc_ext_eps = 0
+                        best_energy = 0
+                        for _ in range(15):
+                            rand_scaling = np.random.choice(np.array([0.01, 0.1, 1, 10, 100]))
+                            self.ahc_ext_eps = np.random.choice(np.array([0.1, 0.333, 1, 3, 10]))
+                            self.ahc_ext_lambd = np.random.choice(np.array([1e-4, 1e-3, 1e-2, 1e-1]))
+                            cached_J = self.problem.J
+                            cached_h = self.problem.h
+                            self.problem.J = rand_scaling * self.problem.J
+                            self.problem.h = rand_scaling * self.problem.h
+                            test_batch = self.CIM_ext_f_AHC_GPU()
+                            if np.amin(test_batch[3])/rand_scaling < best_energy:
+                                best_rand_scaling = rand_scaling
+                                best_ahc_ext_eps = self.ahc_ext_eps
+                                best_ahc_ext_lambd = self.ahc_ext_lambd
+                                best_energy = np.amin(test_batch[3])
+                            self.problem.J = cached_J # return J matrix back to initial value before looping
+                            self.problem.h = cached_h
+                        print("Best combination of epsilon, lambda, and scaling constant: epsilon = {}; lambda = {}; scaling constant = {}".format(best_ahc_ext_eps, best_ahc_ext_lambd, best_rand_scaling))
+                        self.ahc_ext_eps = best_ahc_ext_eps
+                        self.ahc_ext_lambd = best_ahc_ext_lambd
+                        self.problem.J = rand_scaling * self.problem.J
+                        self.problem.h = rand_scaling * self.problem.h
+                        for z in range(num_batches):
+                            curr_batch = self.CIM_ext_f_AHC_GPU()
+                            for y in range(self.num_parallel_runs):
+                                run_data[z*self.num_parallel_runs + y] = [curr_batch[0][y,:], curr_batch[1][y,:,:], curr_batch[2], curr_batch[3][y,:], curr_batch[4][y,:,:]]
+                            run_counter += self.num_parallel_runs
                 else: 
                     tuned_parameters = self.tune_AHC_ext_f()
                     tuned_parameters.pop('J') # Remove J matrix for OOP call.
                     tuned_parameters.pop('h') # Remove h matrix OOP call.
                     print(f"Tuned parameters: {tuned_parameters}.")
                     # Runs the solver in z batches in parallel, and concatenates batches into one flattened run_data list.
                     for z in range(num_batches):
```

### Comparing `cim-optimizer-1.0.3/cim_optimizer.egg-info/PKG-INFO` & `cim-optimizer-1.0.4/cim_optimizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cim-optimizer
-Version: 1.0.3
+Version: 1.0.4
 Summary: Simulated Implementation of the Coherent Ising Machine
 Home-page: https://github.com/mcmahon-lab/cim-optimizer
 Author: McMahon Lab
 Author-email: pmcmahon@cornell.edu
 License: CC-BY-4.0 license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `cim-optimizer-1.0.3/setup.py` & `cim-optimizer-1.0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='cim-optimizer',
-      version=f'1.0.3',
+      version=f'1.0.4',
       description='Simulated Implementation of the Coherent Ising Machine',
       author='McMahon Lab',
       author_email='pmcmahon@cornell.edu',
       license='CC-BY-4.0 license',
       license_files = ('LICENSE.txt',),
       long_description=long_description,
       long_description_content_type='text/markdown',
```

