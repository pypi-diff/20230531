# Comparing `tmp/SPRT-TANDEM-0.1.3.tar.gz` & `tmp/SPRT-TANDEM-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPRT-TANDEM-0.1.3.tar", last modified: Wed May 31 19:52:26 2023, max compression
+gzip compressed data, was "SPRT-TANDEM-0.1.4.tar", last modified: Wed May 31 20:34:35 2023, max compression
```

## Comparing `SPRT-TANDEM-0.1.3.tar` & `SPRT-TANDEM-0.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 19:52:26.647079 SPRT-TANDEM-0.1.3/
--rw-r--r--   0 afe       (1000) afe       (1000)     1095 2023-05-01 05:13:22.000000 SPRT-TANDEM-0.1.3/LICENSE
--rw-rw-r--   0 afe       (1000) afe       (1000)    14145 2023-05-31 19:52:26.647079 SPRT-TANDEM-0.1.3/PKG-INFO
--rw-r--r--   0 afe       (1000) afe       (1000)    13560 2023-05-31 12:20:47.000000 SPRT-TANDEM-0.1.3/README.md
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 19:52:26.647079 SPRT-TANDEM-0.1.3/SPRT_TANDEM.egg-info/
--rw-rw-r--   0 afe       (1000) afe       (1000)    14145 2023-05-31 19:52:26.000000 SPRT-TANDEM-0.1.3/SPRT_TANDEM.egg-info/PKG-INFO
--rw-rw-r--   0 afe       (1000) afe       (1000)      675 2023-05-31 19:52:26.000000 SPRT-TANDEM-0.1.3/SPRT_TANDEM.egg-info/SOURCES.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)        1 2023-05-31 19:52:26.000000 SPRT-TANDEM-0.1.3/SPRT_TANDEM.egg-info/dependency_links.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)       30 2023-05-31 19:52:26.000000 SPRT-TANDEM-0.1.3/SPRT_TANDEM.egg-info/requires.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)        7 2023-05-31 19:52:26.000000 SPRT-TANDEM-0.1.3/SPRT_TANDEM.egg-info/top_level.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)       38 2023-05-31 19:52:26.647079 SPRT-TANDEM-0.1.3/setup.cfg
--rw-r--r--   0 afe       (1000) afe       (1000)     1077 2023-05-31 19:51:10.000000 SPRT-TANDEM-0.1.3/setup.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 19:52:26.647079 SPRT-TANDEM-0.1.3/tandem/
--rw-r--r--   0 afe       (1000) afe       (1000)      356 2023-05-31 05:14:48.000000 SPRT-TANDEM-0.1.3/tandem/__init__.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 19:52:26.647079 SPRT-TANDEM-0.1.3/tandem/config/
--rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.3/tandem/config/__init__.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)    11169 2023-05-31 19:50:55.000000 SPRT-TANDEM-0.1.3/tandem/config/config_definition.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 19:52:26.647079 SPRT-TANDEM-0.1.3/tandem/data/
--rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.3/tandem/data/__init__.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 19:52:26.647079 SPRT-TANDEM-0.1.3/tandem/models/
--rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.3/tandem/models/__init__.py
--rw-r--r--   0 afe       (1000) afe       (1000)    14111 2023-05-31 05:13:13.000000 SPRT-TANDEM-0.1.3/tandem/models/losses.py
--rwxr--r--   0 afe       (1000) afe       (1000)     1417 2023-05-31 05:14:34.000000 SPRT-TANDEM-0.1.3/tandem/models/optimizers.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)    26287 2023-05-31 05:17:50.000000 SPRT-TANDEM-0.1.3/tandem/models/temporal_integrators.py
--rwxr--r--   0 afe       (1000) afe       (1000)     2822 2023-05-31 05:19:38.000000 SPRT-TANDEM-0.1.3/tandem/sprt_tandem_main.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 19:52:26.647079 SPRT-TANDEM-0.1.3/tandem/utils/
--rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.3/tandem/utils/__init__.py
--rwxr--r--   0 afe       (1000) afe       (1000)     6340 2023-05-31 05:18:03.000000 SPRT-TANDEM-0.1.3/tandem/utils/checkpoint.py
--rw-r--r--   0 afe       (1000) afe       (1000)    22645 2023-05-31 05:22:17.000000 SPRT-TANDEM-0.1.3/tandem/utils/data_processing.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)    26821 2023-05-31 05:18:23.000000 SPRT-TANDEM-0.1.3/tandem/utils/hyperparameter_tuning.py
--rwxr--r--   0 afe       (1000) afe       (1000)    24962 2023-05-31 05:18:36.000000 SPRT-TANDEM-0.1.3/tandem/utils/logging.py
--rwxr--r--   0 afe       (1000) afe       (1000)    19979 2023-05-31 05:21:01.000000 SPRT-TANDEM-0.1.3/tandem/utils/misc.py
--rw-r--r--   0 afe       (1000) afe       (1000)    49570 2023-05-31 05:18:56.000000 SPRT-TANDEM-0.1.3/tandem/utils/performance_metrics.py
--rw-r--r--   0 afe       (1000) afe       (1000)    10207 2023-05-31 05:23:44.000000 SPRT-TANDEM-0.1.3/tandem/utils/training.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:34:35.625424 SPRT-TANDEM-0.1.4/
+-rw-r--r--   0 afe       (1000) afe       (1000)     1095 2023-05-01 05:13:22.000000 SPRT-TANDEM-0.1.4/LICENSE
+-rw-rw-r--   0 afe       (1000) afe       (1000)    14145 2023-05-31 20:34:35.625424 SPRT-TANDEM-0.1.4/PKG-INFO
+-rw-r--r--   0 afe       (1000) afe       (1000)    13560 2023-05-31 12:20:47.000000 SPRT-TANDEM-0.1.4/README.md
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:34:35.621424 SPRT-TANDEM-0.1.4/SPRT_TANDEM.egg-info/
+-rw-rw-r--   0 afe       (1000) afe       (1000)    14145 2023-05-31 20:34:35.000000 SPRT-TANDEM-0.1.4/SPRT_TANDEM.egg-info/PKG-INFO
+-rw-rw-r--   0 afe       (1000) afe       (1000)      675 2023-05-31 20:34:35.000000 SPRT-TANDEM-0.1.4/SPRT_TANDEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)        1 2023-05-31 20:34:35.000000 SPRT-TANDEM-0.1.4/SPRT_TANDEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)       30 2023-05-31 20:34:35.000000 SPRT-TANDEM-0.1.4/SPRT_TANDEM.egg-info/requires.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)        7 2023-05-31 20:34:35.000000 SPRT-TANDEM-0.1.4/SPRT_TANDEM.egg-info/top_level.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)       38 2023-05-31 20:34:35.625424 SPRT-TANDEM-0.1.4/setup.cfg
+-rw-r--r--   0 afe       (1000) afe       (1000)     1167 2023-05-31 20:34:28.000000 SPRT-TANDEM-0.1.4/setup.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:34:35.621424 SPRT-TANDEM-0.1.4/tandem/
+-rw-r--r--   0 afe       (1000) afe       (1000)      356 2023-05-31 05:14:48.000000 SPRT-TANDEM-0.1.4/tandem/__init__.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:34:35.621424 SPRT-TANDEM-0.1.4/tandem/config/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.4/tandem/config/__init__.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    11204 2023-05-31 20:04:18.000000 SPRT-TANDEM-0.1.4/tandem/config/config_definition.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:34:35.621424 SPRT-TANDEM-0.1.4/tandem/data/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.4/tandem/data/__init__.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:34:35.625424 SPRT-TANDEM-0.1.4/tandem/models/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.4/tandem/models/__init__.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    14111 2023-05-31 05:13:13.000000 SPRT-TANDEM-0.1.4/tandem/models/losses.py
+-rwxr--r--   0 afe       (1000) afe       (1000)     1417 2023-05-31 05:14:34.000000 SPRT-TANDEM-0.1.4/tandem/models/optimizers.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    26287 2023-05-31 05:17:50.000000 SPRT-TANDEM-0.1.4/tandem/models/temporal_integrators.py
+-rwxr--r--   0 afe       (1000) afe       (1000)     2822 2023-05-31 05:19:38.000000 SPRT-TANDEM-0.1.4/tandem/sprt_tandem_main.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:34:35.625424 SPRT-TANDEM-0.1.4/tandem/utils/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.4/tandem/utils/__init__.py
+-rwxr--r--   0 afe       (1000) afe       (1000)     6340 2023-05-31 05:18:03.000000 SPRT-TANDEM-0.1.4/tandem/utils/checkpoint.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    22645 2023-05-31 05:22:17.000000 SPRT-TANDEM-0.1.4/tandem/utils/data_processing.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    26821 2023-05-31 05:18:23.000000 SPRT-TANDEM-0.1.4/tandem/utils/hyperparameter_tuning.py
+-rwxr--r--   0 afe       (1000) afe       (1000)    24962 2023-05-31 05:18:36.000000 SPRT-TANDEM-0.1.4/tandem/utils/logging.py
+-rwxr--r--   0 afe       (1000) afe       (1000)    20082 2023-05-31 20:23:06.000000 SPRT-TANDEM-0.1.4/tandem/utils/misc.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    49570 2023-05-31 05:18:56.000000 SPRT-TANDEM-0.1.4/tandem/utils/performance_metrics.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    10223 2023-05-31 20:06:33.000000 SPRT-TANDEM-0.1.4/tandem/utils/training.py
```

### Comparing `SPRT-TANDEM-0.1.3/LICENSE` & `SPRT-TANDEM-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.3/PKG-INFO` & `SPRT-TANDEM-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPRT-TANDEM
-Version: 0.1.3
+Version: 0.1.4
 Summary: SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize both speed and accuracy of early-classification.
 Home-page: https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch
 Author: Akinori F. Ebihara
 Author-email: aebihara@nec.com
 License: MIT
 Keywords: Sequential Probability Ratio Test,likelihood ratio,density ratio estimation,early classification,artificial intelligence,machine learning
 Platform: UNKNOWN
```

### Comparing `SPRT-TANDEM-0.1.3/README.md` & `SPRT-TANDEM-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.3/SPRT_TANDEM.egg-info/PKG-INFO` & `SPRT-TANDEM-0.1.4/SPRT_TANDEM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPRT-TANDEM
-Version: 0.1.3
+Version: 0.1.4
 Summary: SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize both speed and accuracy of early-classification.
 Home-page: https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch
 Author: Akinori F. Ebihara
 Author-email: aebihara@nec.com
 License: MIT
 Keywords: Sequential Probability Ratio Test,likelihood ratio,density ratio estimation,early classification,artificial intelligence,machine learning
 Platform: UNKNOWN
```

### Comparing `SPRT-TANDEM-0.1.3/SPRT_TANDEM.egg-info/SOURCES.txt` & `SPRT-TANDEM-0.1.4/SPRT_TANDEM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.3/setup.py` & `SPRT-TANDEM-0.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,23 +5,26 @@
 with open(
     path.join(path.abspath(path.dirname(__file__)), "README.md"), encoding="utf-8"
 ) as f:
     long_description = f.read()
 
 setup(
     name="SPRT-TANDEM",
-    version="0.1.3",
+    version="0.1.4",
     license="MIT",
     description="SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize both speed and accuracy of early-classification.",
     author="Akinori F. Ebihara",
     author_email="aebihara@nec.com",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
+    package_data={
+        "data": ["SequentialGaussian_2class_offset2.0_dim2/*"],
+    },
     url="https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch",
     keywords=[
         "Sequential Probability Ratio Test",
         "likelihood ratio",
         "density ratio estimation",
         "early classification",
         "artificial intelligence",
```

### Comparing `SPRT-TANDEM-0.1.3/tandem/config/config_definition.py` & `SPRT-TANDEM-0.1.4/tandem/config/config_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,24 @@
 ########################## USER EDITABLE BLOCK STARTS ######################################
 
 # Base info
 CONFIG_PATH = __file__
 LOG_PATH = CONFIG_PATH[: CONFIG_PATH.find("config")] + "logs/"
 
 # Data info
-NUM_CLASSES = 3  # 2
-DATA_SEPARATION = "0.5"
+NUM_CLASSES = 2
+DATA_SEPARATION = "2.0"
+FEAT_DIM = 2
 DATA_PATH = "../data/"
-DATA_FOLDER = f"SequentialGaussian_{NUM_CLASSES}class_offset{DATA_SEPARATION}"
-NUM_TRAIN = 60000  # 300000  # 25000 # 19000
-NUM_VAL = 6000  # 30000  # 4000 # # 990
-NUM_TEST = 6000  # 30000  # 1000 # 10
+DATA_FOLDER = (
+    f"SequentialGaussian_{NUM_CLASSES}class_offset{DATA_SEPARATION}_dim{FEAT_DIM}"
+)
+NUM_TRAIN = 40000  # 300000  # 25000 # 19000
+NUM_VAL = 4000  # 30000  # 4000 # # 990
+NUM_TEST = 4000  # 30000  # 1000 # 10
 TRAIN_DATA = f"{DATA_PATH}{DATA_FOLDER}/train_{NUM_TRAIN}"
 VAL_DATA = f"{DATA_PATH}{DATA_FOLDER}/val_{NUM_VAL}"
 TEST_DATA = f"{DATA_PATH}{DATA_FOLDER}/test_{NUM_TEST}"
 DATA_NAMES = ("data", "label", "llr")
 IS_SHUFFLE = True  # whether to shuffle training data. It may cause significant overhead
 TB_DIRNAME = "TensorBoard_events"
 DB_DIRNAME = "Optuna_databases"
@@ -118,15 +121,15 @@
     "TEST_DATA": TEST_DATA,
     "DATA_NAMES": DATA_NAMES,
     "IS_SHUFFLE": IS_SHUFFLE,
     "NUM_TRAIN": NUM_TRAIN,
     "NUM_VAL": NUM_VAL,
     "NUM_TEST": NUM_TEST,
     "NUM_CLASSES": NUM_CLASSES,
-    "FEAT_DIM": 128,
+    "FEAT_DIM": FEAT_DIM,
     # SPRT-TANDEM parameters
     "ORDER_SPRT": ORDER_SPRT,
     "TIME_STEPS": 50,
     "LLLR_VERSION": LLLR_VERSION,  # LSEL
     "OBLIVIOUS": False,  # Miyagawa & Ebihara, ICML2021
     "PARAM_MULTIPLET_LOSS": PARAM_MULTIPLET_LOSS,
     "PARAM_LLR_LOSS": PARAM_LLR_LOSS,
```

### Comparing `SPRT-TANDEM-0.1.3/tandem/models/losses.py` & `SPRT-TANDEM-0.1.4/tandem/models/losses.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.3/tandem/models/optimizers.py` & `SPRT-TANDEM-0.1.4/tandem/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.3/tandem/models/temporal_integrators.py` & `SPRT-TANDEM-0.1.4/tandem/models/temporal_integrators.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.3/tandem/sprt_tandem_main.py` & `SPRT-TANDEM-0.1.4/tandem/sprt_tandem_main.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.3/tandem/utils/checkpoint.py` & `SPRT-TANDEM-0.1.4/tandem/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.3/tandem/utils/data_processing.py` & `SPRT-TANDEM-0.1.4/tandem/utils/data_processing.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.3/tandem/utils/hyperparameter_tuning.py` & `SPRT-TANDEM-0.1.4/tandem/utils/hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.3/tandem/utils/logging.py` & `SPRT-TANDEM-0.1.4/tandem/utils/logging.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.3/tandem/utils/misc.py` & `SPRT-TANDEM-0.1.4/tandem/utils/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 from types import SimpleNamespace
 import argparse
 from loguru import logger
 import torch
 import torch.nn.functional as F
 
 
+def setup_minimal_example(config: Dict):
+    config["CONFIG_PATH"] = __file__
+    config["NOW"] = ""
+
+
 class PyTorchPhaseManager:
     """
     A context manager for managing the training and evaluation phases of a PyTorch model.
 
     Args:
     - phase (str): The phase to manage ('train' or 'val').
```

### Comparing `SPRT-TANDEM-0.1.3/tandem/utils/performance_metrics.py` & `SPRT-TANDEM-0.1.4/tandem/utils/performance_metrics.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.3/tandem/utils/training.py` & `SPRT-TANDEM-0.1.4/tandem/utils/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         enumerate(data_loaders[phase]),
         mininterval=2,
         total=iter_num,
         desc=colored(f"{phase} in progress...", barcolor),
         colour=barcolor,
         leave=False,
     ):
-        x_batch, y_batch, gt_llrs_batch = move_data_to_device(data, device)
+        x_batch, y_batch, gt_llrs_batch = move_data_to_device(data, device)  # type: ignore
 
         # a periodic validation is inserted between training iterations.
         # This function is recursively called under is_train=True, with phase='eval'.
         if is_train and global_step % config["VALIDATION_STEP"] == 0:
             best, global_step = run_one_epoch(
                 trial,
                 model,
```

