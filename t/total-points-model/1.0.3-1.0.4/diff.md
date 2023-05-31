# Comparing `tmp/total-points-model-1.0.3.tar.gz` & `tmp/total-points-model-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "total-points-model-1.0.3.tar", last modified: Wed May 31 06:54:34 2023, max compression
+gzip compressed data, was "total-points-model-1.0.4.tar", last modified: Wed May 31 06:54:47 2023, max compression
```

## Comparing `total-points-model-1.0.3.tar` & `total-points-model-1.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-05-31 06:54:34.134180 total-points-model-1.0.3/
--rw-r--r--   0 ciaran     (501) staff       (20)     1068 2023-05-31 06:13:49.000000 total-points-model-1.0.3/LICENSE
--rw-r--r--   0 ciaran     (501) staff       (20)     2360 2023-05-31 06:54:34.134024 total-points-model-1.0.3/PKG-INFO
--rw-r--r--   0 ciaran     (501) staff       (20)      779 2023-05-31 06:41:17.000000 total-points-model-1.0.3/README.md
--rw-r--r--   0 ciaran     (501) staff       (20)      889 2023-05-31 06:13:49.000000 total-points-model-1.0.3/pyproject.toml
--rw-r--r--   0 ciaran     (501) staff       (20)       38 2023-05-31 06:54:34.134227 total-points-model-1.0.3/setup.cfg
-drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-05-31 06:54:34.128970 total-points-model-1.0.3/total_points_model/
--rw-r--r--   0 ciaran     (501) staff       (20)        0 2023-05-31 06:13:49.000000 total-points-model-1.0.3/total_points_model/__init__.py
--rw-r--r--   0 ciaran     (501) staff       (20)       45 2023-05-31 06:21:51.000000 total-points-model-1.0.3/total_points_model/config.py
-drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-05-31 06:54:34.130421 total-points-model-1.0.3/total_points_model/domain/
--rw-r--r--   0 ciaran     (501) staff       (20)        0 2023-05-31 06:13:49.000000 total-points-model-1.0.3/total_points_model/domain/__init__.py
-drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-05-31 06:54:34.131559 total-points-model-1.0.3/total_points_model/domain/contracts/
--rw-r--r--   0 ciaran     (501) staff       (20)        0 2023-05-31 06:13:49.000000 total-points-model-1.0.3/total_points_model/domain/contracts/__init__.py
--rw-r--r--   0 ciaran     (501) staff       (20)    26290 2023-05-31 06:13:49.000000 total-points-model-1.0.3/total_points_model/domain/contracts/mappings.py
--rw-r--r--   0 ciaran     (501) staff       (20)     1390 2023-05-31 06:13:49.000000 total-points-model-1.0.3/total_points_model/domain/contracts/modelling_data_contract.py
--rw-r--r--   0 ciaran     (501) staff       (20)      469 2023-05-31 06:13:49.000000 total-points-model-1.0.3/total_points_model/domain/contracts/rolling_columns.py
-drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-05-31 06:54:34.132889 total-points-model-1.0.3/total_points_model/domain/modelling/
--rw-r--r--   0 ciaran     (501) staff       (20)        0 2023-05-31 06:13:49.000000 total-points-model-1.0.3/total_points_model/domain/modelling/__init__.py
--rw-r--r--   0 ciaran     (501) staff       (20)     7604 2023-05-31 06:13:49.000000 total-points-model-1.0.3/total_points_model/domain/modelling/hyperparameter_tuning.py
--rw-r--r--   0 ciaran     (501) staff       (20)    10870 2023-05-31 06:13:49.000000 total-points-model-1.0.3/total_points_model/domain/modelling/model_evaluation.py
--rw-r--r--   0 ciaran     (501) staff       (20)      873 2023-05-31 06:13:49.000000 total-points-model-1.0.3/total_points_model/domain/modelling/optuna_xgb_param_grid.py
--rw-r--r--   0 ciaran     (501) staff       (20)     3911 2023-05-31 06:13:49.000000 total-points-model-1.0.3/total_points_model/domain/modelling/supermodel.py
-drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-05-31 06:54:34.133747 total-points-model-1.0.3/total_points_model/domain/preprocessing/
--rw-r--r--   0 ciaran     (501) staff       (20)        0 2023-05-31 06:13:49.000000 total-points-model-1.0.3/total_points_model/domain/preprocessing/__init__.py
--rw-r--r--   0 ciaran     (501) staff       (20)     8480 2023-05-31 06:13:49.000000 total-points-model-1.0.3/total_points_model/domain/preprocessing/data_preprocessor.py
--rw-r--r--   0 ciaran     (501) staff       (20)     4087 2023-05-31 06:13:49.000000 total-points-model-1.0.3/total_points_model/domain/preprocessing/elo_calculator.py
--rw-r--r--   0 ciaran     (501) staff       (20)     9527 2023-05-31 06:13:49.000000 total-points-model-1.0.3/total_points_model/domain/preprocessing/preprocessing_functions.py
-drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-05-31 06:54:34.130227 total-points-model-1.0.3/total_points_model.egg-info/
--rw-r--r--   0 ciaran     (501) staff       (20)     2360 2023-05-31 06:54:34.000000 total-points-model-1.0.3/total_points_model.egg-info/PKG-INFO
--rw-r--r--   0 ciaran     (501) staff       (20)     1067 2023-05-31 06:54:34.000000 total-points-model-1.0.3/total_points_model.egg-info/SOURCES.txt
--rw-r--r--   0 ciaran     (501) staff       (20)        1 2023-05-31 06:54:34.000000 total-points-model-1.0.3/total_points_model.egg-info/dependency_links.txt
--rw-r--r--   0 ciaran     (501) staff       (20)      263 2023-05-31 06:54:34.000000 total-points-model-1.0.3/total_points_model.egg-info/requires.txt
--rw-r--r--   0 ciaran     (501) staff       (20)       19 2023-05-31 06:54:34.000000 total-points-model-1.0.3/total_points_model.egg-info/top_level.txt
+drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-05-31 06:54:47.457358 total-points-model-1.0.4/
+-rw-r--r--   0 ciaran     (501) staff       (20)     1068 2023-05-31 06:13:49.000000 total-points-model-1.0.4/LICENSE
+-rw-r--r--   0 ciaran     (501) staff       (20)     2360 2023-05-31 06:54:47.457214 total-points-model-1.0.4/PKG-INFO
+-rw-r--r--   0 ciaran     (501) staff       (20)      779 2023-05-31 06:41:17.000000 total-points-model-1.0.4/README.md
+-rw-r--r--   0 ciaran     (501) staff       (20)      889 2023-05-31 06:54:36.000000 total-points-model-1.0.4/pyproject.toml
+-rw-r--r--   0 ciaran     (501) staff       (20)       38 2023-05-31 06:54:47.457422 total-points-model-1.0.4/setup.cfg
+drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-05-31 06:54:47.452446 total-points-model-1.0.4/total_points_model/
+-rw-r--r--   0 ciaran     (501) staff       (20)        0 2023-05-31 06:13:49.000000 total-points-model-1.0.4/total_points_model/__init__.py
+-rw-r--r--   0 ciaran     (501) staff       (20)       45 2023-05-31 06:21:51.000000 total-points-model-1.0.4/total_points_model/config.py
+drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-05-31 06:54:47.453811 total-points-model-1.0.4/total_points_model/domain/
+-rw-r--r--   0 ciaran     (501) staff       (20)        0 2023-05-31 06:13:49.000000 total-points-model-1.0.4/total_points_model/domain/__init__.py
+drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-05-31 06:54:47.454906 total-points-model-1.0.4/total_points_model/domain/contracts/
+-rw-r--r--   0 ciaran     (501) staff       (20)        0 2023-05-31 06:13:49.000000 total-points-model-1.0.4/total_points_model/domain/contracts/__init__.py
+-rw-r--r--   0 ciaran     (501) staff       (20)    26290 2023-05-31 06:13:49.000000 total-points-model-1.0.4/total_points_model/domain/contracts/mappings.py
+-rw-r--r--   0 ciaran     (501) staff       (20)     1390 2023-05-31 06:13:49.000000 total-points-model-1.0.4/total_points_model/domain/contracts/modelling_data_contract.py
+-rw-r--r--   0 ciaran     (501) staff       (20)      469 2023-05-31 06:13:49.000000 total-points-model-1.0.4/total_points_model/domain/contracts/rolling_columns.py
+drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-05-31 06:54:47.456223 total-points-model-1.0.4/total_points_model/domain/modelling/
+-rw-r--r--   0 ciaran     (501) staff       (20)        0 2023-05-31 06:13:49.000000 total-points-model-1.0.4/total_points_model/domain/modelling/__init__.py
+-rw-r--r--   0 ciaran     (501) staff       (20)     7604 2023-05-31 06:13:49.000000 total-points-model-1.0.4/total_points_model/domain/modelling/hyperparameter_tuning.py
+-rw-r--r--   0 ciaran     (501) staff       (20)    10870 2023-05-31 06:13:49.000000 total-points-model-1.0.4/total_points_model/domain/modelling/model_evaluation.py
+-rw-r--r--   0 ciaran     (501) staff       (20)      873 2023-05-31 06:13:49.000000 total-points-model-1.0.4/total_points_model/domain/modelling/optuna_xgb_param_grid.py
+-rw-r--r--   0 ciaran     (501) staff       (20)     3911 2023-05-31 06:13:49.000000 total-points-model-1.0.4/total_points_model/domain/modelling/supermodel.py
+drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-05-31 06:54:47.456949 total-points-model-1.0.4/total_points_model/domain/preprocessing/
+-rw-r--r--   0 ciaran     (501) staff       (20)        0 2023-05-31 06:13:49.000000 total-points-model-1.0.4/total_points_model/domain/preprocessing/__init__.py
+-rw-r--r--   0 ciaran     (501) staff       (20)     8480 2023-05-31 06:13:49.000000 total-points-model-1.0.4/total_points_model/domain/preprocessing/data_preprocessor.py
+-rw-r--r--   0 ciaran     (501) staff       (20)     4087 2023-05-31 06:13:49.000000 total-points-model-1.0.4/total_points_model/domain/preprocessing/elo_calculator.py
+-rw-r--r--   0 ciaran     (501) staff       (20)     9527 2023-05-31 06:13:49.000000 total-points-model-1.0.4/total_points_model/domain/preprocessing/preprocessing_functions.py
+drwxr-xr-x   0 ciaran     (501) staff       (20)        0 2023-05-31 06:54:47.453567 total-points-model-1.0.4/total_points_model.egg-info/
+-rw-r--r--   0 ciaran     (501) staff       (20)     2360 2023-05-31 06:54:47.000000 total-points-model-1.0.4/total_points_model.egg-info/PKG-INFO
+-rw-r--r--   0 ciaran     (501) staff       (20)     1067 2023-05-31 06:54:47.000000 total-points-model-1.0.4/total_points_model.egg-info/SOURCES.txt
+-rw-r--r--   0 ciaran     (501) staff       (20)        1 2023-05-31 06:54:47.000000 total-points-model-1.0.4/total_points_model.egg-info/dependency_links.txt
+-rw-r--r--   0 ciaran     (501) staff       (20)      263 2023-05-31 06:54:47.000000 total-points-model-1.0.4/total_points_model.egg-info/requires.txt
+-rw-r--r--   0 ciaran     (501) staff       (20)       19 2023-05-31 06:54:47.000000 total-points-model-1.0.4/total_points_model.egg-info/top_level.txt
```

### Comparing `total-points-model-1.0.3/LICENSE` & `total-points-model-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `total-points-model-1.0.3/PKG-INFO` & `total-points-model-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: total-points-model
-Version: 1.0.3
+Version: 1.0.4
 Summary: Train an AFL Total Points model
 Author-email: Ciaran Grant <ciaran.grant@hotmail.co.uk>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `total-points-model-1.0.3/README.md` & `total-points-model-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `total-points-model-1.0.3/pyproject.toml` & `total-points-model-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "total-points-model"
-version = "1.0.3"
+version = "1.0.4"
 description = "Train an AFL Total Points model"
 readme = "README.md"
 authors = [{name = "Ciaran Grant", email = "ciaran.grant@hotmail.co.uk"}]
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
 dependencies = [
     "pandas == 1.5.3",
```

### Comparing `total-points-model-1.0.3/total_points_model/domain/contracts/mappings.py` & `total-points-model-1.0.4/total_points_model/domain/contracts/mappings.py`

 * *Files identical despite different names*

### Comparing `total-points-model-1.0.3/total_points_model/domain/contracts/modelling_data_contract.py` & `total-points-model-1.0.4/total_points_model/domain/contracts/modelling_data_contract.py`

 * *Files identical despite different names*

### Comparing `total-points-model-1.0.3/total_points_model/domain/modelling/hyperparameter_tuning.py` & `total-points-model-1.0.4/total_points_model/domain/modelling/hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `total-points-model-1.0.3/total_points_model/domain/modelling/model_evaluation.py` & `total-points-model-1.0.4/total_points_model/domain/modelling/model_evaluation.py`

 * *Files identical despite different names*

### Comparing `total-points-model-1.0.3/total_points_model/domain/modelling/optuna_xgb_param_grid.py` & `total-points-model-1.0.4/total_points_model/domain/modelling/optuna_xgb_param_grid.py`

 * *Files identical despite different names*

### Comparing `total-points-model-1.0.3/total_points_model/domain/modelling/supermodel.py` & `total-points-model-1.0.4/total_points_model/domain/modelling/supermodel.py`

 * *Files identical despite different names*

### Comparing `total-points-model-1.0.3/total_points_model/domain/preprocessing/data_preprocessor.py` & `total-points-model-1.0.4/total_points_model/domain/preprocessing/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `total-points-model-1.0.3/total_points_model/domain/preprocessing/elo_calculator.py` & `total-points-model-1.0.4/total_points_model/domain/preprocessing/elo_calculator.py`

 * *Files identical despite different names*

### Comparing `total-points-model-1.0.3/total_points_model/domain/preprocessing/preprocessing_functions.py` & `total-points-model-1.0.4/total_points_model/domain/preprocessing/preprocessing_functions.py`

 * *Files identical despite different names*

### Comparing `total-points-model-1.0.3/total_points_model.egg-info/PKG-INFO` & `total-points-model-1.0.4/total_points_model.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: total-points-model
-Version: 1.0.3
+Version: 1.0.4
 Summary: Train an AFL Total Points model
 Author-email: Ciaran Grant <ciaran.grant@hotmail.co.uk>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `total-points-model-1.0.3/total_points_model.egg-info/SOURCES.txt` & `total-points-model-1.0.4/total_points_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

