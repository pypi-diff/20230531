# Comparing `tmp/mct-quantizers-nightly-1.0.0.29052023.post1013.tar.gz` & `tmp/mct-quantizers-nightly-1.0.0.30052023.post958.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-quantizers-nightly-1.0.0.29052023.post1013.tar", last modified: Mon May 29 00:10:15 2023, max compression
+gzip compressed data, was "mct-quantizers-nightly-1.0.0.30052023.post958.tar", last modified: Tue May 30 00:09:59 2023, max compression
```

## Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013.tar` & `mct-quantizers-nightly-1.0.0.30052023.post958.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:10:15.404254 mct-quantizers-nightly-1.0.0.29052023.post1013/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-29 00:10:15.404254 mct-quantizers-nightly-1.0.0.29052023.post1013/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:10:15.396254 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:10:15.400254 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/common/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/common/base_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/common/get_all_subclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/common/quant_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/common/quant_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:10:15.400254 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:10:15.400254 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:10:15.400254 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:10:15.400254 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/validation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:10:15.400254 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:10:15.400254 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:10:15.404254 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:10:15.404254 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-29 00:09:53.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:10:15.404254 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-29 00:10:15.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-05-29 00:10:15.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 00:10:15.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 00:10:15.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-29 00:10:15.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-29 00:10:15.404254 mct-quantizers-nightly-1.0.0.29052023.post1013/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-29 00:10:13.000000 mct-quantizers-nightly-1.0.0.29052023.post1013/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:09:59.339436 mct-quantizers-nightly-1.0.0.30052023.post958/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-30 00:09:59.339436 mct-quantizers-nightly-1.0.0.30052023.post958/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:09:59.331436 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:09:59.331436 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/common/base_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/common/get_all_subclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/common/quant_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/common/quant_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:09:59.335435 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14484 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:09:59.335435 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:09:59.335435 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:09:59.335435 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/validation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:09:59.335435 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:09:59.335435 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:09:59.335435 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:09:59.339436 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-30 00:09:45.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:09:59.339436 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-30 00:09:59.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-05-30 00:09:59.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 00:09:59.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 00:09:59.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 00:09:59.000000 mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-30 00:09:59.339436 mct-quantizers-nightly-1.0.0.30052023.post958/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-30 00:09:58.000000 mct-quantizers-nightly-1.0.0.30052023.post958/setup.py
```

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/LICENSE.md` & `mct-quantizers-nightly-1.0.0.30052023.post958/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/PKG-INFO` & `mct-quantizers-nightly-1.0.0.30052023.post958/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers-nightly
-Version: 1.0.0.29052023.post1013
+Version: 1.0.0.30052023.post958
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/common/__init__.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/common/base_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/common/base_inferable_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from enum import Enum
 from typing import Any, Dict, List
 
 from mct_quantizers.common.quant_info import QuantizationMethod
+from mct_quantizers.logger import Logger
 
 
 class QuantizationTarget(Enum):
     Activation = "Activation"
     Weights = "Weights"
```

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/common/constants.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/common/get_all_subclasses.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/common/get_all_subclasses.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/common/get_quantizers.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/common/get_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/common/quant_info.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/common/quant_info.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/common/quant_utils.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/__init__.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/activation_quantization_holder.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/activation_quantization_holder.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,15 +131,17 @@
         def convert_to_inferable_quantizers(self):
             """
             Convert layer's quantizer to inferable quantizer.
 
             Returns:
                 None
             """
-            self.activation_holder_quantizer = self.activation_holder_quantizer.convert2inferable()
+            if hasattr(self.activation_holder_quantizer, 'convert2inferable') and callable(
+                    self.activation_holder_quantizer.convert2inferable):  # pragma: no cover
+                self.activation_holder_quantizer = self.activation_holder_quantizer.convert2inferable()
 
 
 else:
     class KerasActivationQuantizationHolder:  # pragma: no cover
         def __init__(self, *args, **kwargs):
             Logger.error('Installing tensorflow and tensorflow_model_optimization is mandatory '
                          'when using ActivationQuantizationHolder. '
```

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/load_model.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantize_wrapper.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantize_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,23 +284,25 @@
             Returns:
                 None
             """
             # Activations quantizers
             inferable_activation_quantizers = []
             if self.is_activation_quantization:
                 for quantizer in self.activation_quantizers:
-                    inferable_activation_quantizers.append(quantizer.convert2inferable())
+                    if hasattr(quantizer, 'convert2inferable') and callable(quantizer.convert2inferable):
+                        inferable_activation_quantizers.append(quantizer.convert2inferable())
                 self.activation_quantizers = inferable_activation_quantizers
                 self._set_activations_vars()
 
             # Weight quantizers
             inferable_weight_quantizers = {}
             if self.is_weights_quantization:
                 for name, quantizer in self.weights_quantizers.items():
-                    inferable_weight_quantizers.update({name: quantizer.convert2inferable()})
+                    if hasattr(quantizer, 'convert2inferable') and callable(quantizer.convert2inferable):
+                        inferable_weight_quantizers.update({name: quantizer.convert2inferable()})
                 self.weights_quantizers = inferable_weight_quantizers
                 self._set_weights_vars(False)
 
         def get_weights_vars(self) -> List[Tuple[str, Any, BaseInferableQuantizer]]:
             """
             A getter of the layer's weights variables.
```

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizer_utils.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/keras/validation_functions.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/keras/validation_functions.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/logger.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/logger.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/__init__.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/activation_quantization_holder.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/activation_quantization_holder.py`

 * *Files 13% similar despite different names*

```diff
@@ -54,15 +54,17 @@
 
         def convert_to_inferable_quantizers(self):
             """
             Convert a layer's quantizer to an inferable quantizer.
             Returns:
                 None
             """
-            self.activation_holder_quantizer = self.activation_holder_quantizer.convert2inferable()
+            if hasattr(self.activation_holder_quantizer, 'convert2inferable') and callable(
+                    self.activation_holder_quantizer.convert2inferable):  # pragma: no cover
+                self.activation_holder_quantizer = self.activation_holder_quantizer.convert2inferable()
 
 else:
     class PytorchActivationQuantizationHolder:  # pragma: no cover
         def __init__(self, *args, **kwargs):
             Logger.critical('Installing Pytorch is mandatory '
                             'when using PytorchActivationQuantizationHolder. '
                             'Could not find the torch package.')  # pragma: no cover
```

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/load_model.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantize_wrapper.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantize_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,23 +101,25 @@
             Convert the wrapper quantizers with inferable quantizers
 
             """
             # Activation quantizers
             if self.is_activation_quantization:
                 inferable_activation_quantizers = []
                 for quantizer in self.activation_quantizers:
-                    inferable_activation_quantizers.append(quantizer.convert2inferable())
+                    if hasattr(quantizer, 'convert2inferable') and callable(quantizer.convert2inferable):
+                        inferable_activation_quantizers.append(quantizer.convert2inferable())
                 self.activation_quantizers = inferable_activation_quantizers
                 self._set_activation_vars()
 
             # Weight quantizers
             if self.is_weights_quantization:
                 inferable_weight_quantizers = {}
                 for name, quantizer in self.weights_quantizers.items():
-                    inferable_weight_quantizers.update({name: quantizer.convert2inferable()})
+                    if hasattr(quantizer, 'convert2inferable') and callable(quantizer.convert2inferable):
+                        inferable_weight_quantizers.update({name: quantizer.convert2inferable()})
                 self.weights_quantizers = inferable_weight_quantizers
                 self._set_weights_vars(False)
 
         def _set_weights_vars(self, is_training: bool = True):
             """
             Initialize learnable weights as parameters in the wrapper, and their quantizers
```

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizer_utils.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers_nightly.egg-info/PKG-INFO` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers_nightly.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers-nightly
-Version: 1.0.0.29052023.post1013
+Version: 1.0.0.30052023.post958
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/mct_quantizers_nightly.egg-info/SOURCES.txt` & `mct-quantizers-nightly-1.0.0.30052023.post958/mct_quantizers_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.0.0.29052023.post1013/setup.py` & `mct-quantizers-nightly-1.0.0.30052023.post958/setup.py`

 * *Files identical despite different names*

