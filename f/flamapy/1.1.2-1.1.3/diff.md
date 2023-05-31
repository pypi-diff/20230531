# Comparing `tmp/flamapy-1.1.2.tar.gz` & `tmp/flamapy-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flamapy-1.1.2.tar", last modified: Wed May 31 11:09:34 2023, max compression
+gzip compressed data, was "flamapy-1.1.3.tar", last modified: Wed May 31 12:09:31 2023, max compression
```

## Comparing `flamapy-1.1.2.tar` & `flamapy-1.1.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:34.917863 flamapy-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-31 11:09:34.917863 flamapy-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-31 11:09:20.000000 flamapy-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:34.913864 flamapy-1.1.2/flamapy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:34.913864 flamapy-1.1.2/flamapy/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:34.913864 flamapy-1.1.2/flamapy/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/discover.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:34.913864 flamapy-1.1.2/flamapy/core/models/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/models/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/models/variability_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:34.917863 flamapy-1.1.2/flamapy/core/operations/
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/operations/abstract_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/operations/atomic_sets.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/operations/average_branching_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/operations/commonality.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/operations/core_features.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/operations/count_leafs.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/operations/dead_features.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/operations/error_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/operations/error_diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/operations/estimated_products_number.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/operations/false_optional_features.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/operations/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/operations/products.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/operations/products_number.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/operations/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/operations/valid.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/operations/valid_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/operations/valid_product.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/operations/variability.py
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:34.917863 flamapy-1.1.2/flamapy/core/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/transformations/abstract_transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/transformations/model_to_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/transformations/model_to_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/transformations/text_to_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:34.917863 flamapy-1.1.2/flamapy/endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/endpoint/diverso_lab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:34.913864 flamapy-1.1.2/flamapy/metamodels/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:34.917863 flamapy-1.1.2/flamapy/metamodels/configuration_metamodel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/metamodels/configuration_metamodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:34.917863 flamapy-1.1.2/flamapy/metamodels/configuration_metamodel/models/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/metamodels/configuration_metamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/metamodels/configuration_metamodel/models/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:34.917863 flamapy-1.1.2/flamapy/metamodels/configuration_metamodel/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/metamodels/configuration_metamodel/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-31 11:09:20.000000 flamapy-1.1.2/flamapy/metamodels/configuration_metamodel/transformations/configuration_basic_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:09:34.913864 flamapy-1.1.2/flamapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-31 11:09:34.000000 flamapy-1.1.2/flamapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-31 11:09:34.000000 flamapy-1.1.2/flamapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 11:09:34.000000 flamapy-1.1.2/flamapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 11:09:34.000000 flamapy-1.1.2/flamapy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 11:09:34.000000 flamapy-1.1.2/flamapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 11:09:34.000000 flamapy-1.1.2/flamapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 11:09:34.917863 flamapy-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-31 11:09:20.000000 flamapy-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:09:31.713328 flamapy-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-31 12:09:31.713328 flamapy-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-31 12:09:17.000000 flamapy-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:09:31.701327 flamapy-1.1.3/flamapy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:09:31.705327 flamapy-1.1.3/flamapy/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:09:31.705327 flamapy-1.1.3/flamapy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10385 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/discover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:09:31.705327 flamapy-1.1.3/flamapy/core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/models/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/models/variability_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:09:31.709327 flamapy-1.1.3/flamapy/core/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/operations/abstract_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/operations/atomic_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/operations/average_branching_factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/operations/commonality.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/operations/core_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/operations/count_leafs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/operations/dead_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/operations/error_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/operations/error_diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/operations/estimated_products_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/operations/false_optional_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/operations/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/operations/products.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/operations/products_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/operations/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/operations/valid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/operations/valid_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/operations/valid_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/operations/variability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:09:31.709327 flamapy-1.1.3/flamapy/core/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/transformations/abstract_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/transformations/model_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/transformations/model_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/transformations/text_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:09:31.709327 flamapy-1.1.3/flamapy/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/endpoint/diverso_lab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:09:31.701327 flamapy-1.1.3/flamapy/metamodels/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:09:31.713328 flamapy-1.1.3/flamapy/metamodels/configuration_metamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/metamodels/configuration_metamodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:09:31.713328 flamapy-1.1.3/flamapy/metamodels/configuration_metamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/metamodels/configuration_metamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/metamodels/configuration_metamodel/models/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:09:31.713328 flamapy-1.1.3/flamapy/metamodels/configuration_metamodel/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/metamodels/configuration_metamodel/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-31 12:09:17.000000 flamapy-1.1.3/flamapy/metamodels/configuration_metamodel/transformations/configuration_basic_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:09:31.705327 flamapy-1.1.3/flamapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-31 12:09:31.000000 flamapy-1.1.3/flamapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-31 12:09:31.000000 flamapy-1.1.3/flamapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:09:31.000000 flamapy-1.1.3/flamapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 12:09:31.000000 flamapy-1.1.3/flamapy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 12:09:31.000000 flamapy-1.1.3/flamapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 12:09:31.000000 flamapy-1.1.3/flamapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 12:09:31.713328 flamapy-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-31 12:09:17.000000 flamapy-1.1.3/setup.py
```

### Comparing `flamapy-1.1.2/PKG-INFO` & `flamapy-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy
-Version: 1.1.2
+Version: 1.1.3
 Summary: Flamapy is a Python-based AAFM framework that takes into consideration previous AAFM tool designs and enables multi-solver and multi-metamodel support for the integration of AAFM tooling on the Python ecosystem.
 Home-page: https://github.com/flamapy/core
 Author: Flamapy
 Author-email: flamapy@us.es
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flamapy-1.1.2/README.md` & `flamapy-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `flamapy-1.1.2/flamapy/commands/__init__.py` & `flamapy-1.1.3/flamapy/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `flamapy-1.1.2/flamapy/core/discover.py` & `flamapy-1.1.3/flamapy/core/discover.py`

 * *Files identical despite different names*

### Comparing `flamapy-1.1.2/flamapy/core/models/ast.py` & `flamapy-1.1.3/flamapy/core/models/ast.py`

 * *Files identical despite different names*

### Comparing `flamapy-1.1.2/flamapy/core/operations/__init__.py` & `flamapy-1.1.3/flamapy/core/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `flamapy-1.1.2/flamapy/core/operations/atomic_sets.py` & `flamapy-1.1.3/flamapy/core/operations/atomic_sets.py`

 * *Files identical despite different names*

### Comparing `flamapy-1.1.2/flamapy/core/operations/false_optional_features.py` & `flamapy-1.1.3/flamapy/core/operations/false_optional_features.py`

 * *Files identical despite different names*

### Comparing `flamapy-1.1.2/flamapy/core/operations/sampling.py` & `flamapy-1.1.3/flamapy/core/operations/sampling.py`

 * *Files identical despite different names*

### Comparing `flamapy-1.1.2/flamapy/core/plugins.py` & `flamapy-1.1.3/flamapy/core/plugins.py`

 * *Files identical despite different names*

### Comparing `flamapy-1.1.2/flamapy/endpoint/diverso_lab.py` & `flamapy-1.1.3/flamapy/endpoint/diverso_lab.py`

 * *Files identical despite different names*

### Comparing `flamapy-1.1.2/flamapy/metamodels/configuration_metamodel/models/configuration.py` & `flamapy-1.1.3/flamapy/metamodels/configuration_metamodel/models/configuration.py`

 * *Files identical despite different names*

### Comparing `flamapy-1.1.2/flamapy/metamodels/configuration_metamodel/transformations/configuration_basic_reader.py` & `flamapy-1.1.3/flamapy/metamodels/configuration_metamodel/transformations/configuration_basic_reader.py`

 * *Files identical despite different names*

### Comparing `flamapy-1.1.2/flamapy.egg-info/PKG-INFO` & `flamapy-1.1.3/flamapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy
-Version: 1.1.2
+Version: 1.1.3
 Summary: Flamapy is a Python-based AAFM framework that takes into consideration previous AAFM tool designs and enables multi-solver and multi-metamodel support for the integration of AAFM tooling on the Python ecosystem.
 Home-page: https://github.com/flamapy/core
 Author: Flamapy
 Author-email: flamapy@us.es
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flamapy-1.1.2/flamapy.egg-info/SOURCES.txt` & `flamapy-1.1.3/flamapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flamapy-1.1.2/setup.py` & `flamapy-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="flamapy",
-    version="1.1.2",
+    version="1.1.3",
     author="Flamapy",
     author_email="flamapy@us.es",
     description="Flamapy is a Python-based AAFM framework that takes into consideration previous AAFM tool designs and enables multi-solver and multi-metamodel support for the integration of AAFM tooling on the Python ecosystem.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/flamapy/core",
     packages=setuptools.find_namespace_packages(include=['flamapy.*']),
```

