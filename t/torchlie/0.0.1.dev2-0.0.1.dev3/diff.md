# Comparing `tmp/torchlie-0.0.1.dev2.tar.gz` & `tmp/torchlie-0.0.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchlie-0.0.1.dev2.tar", last modified: Mon May 29 21:01:01 2023, max compression
+gzip compressed data, was "torchlie-0.0.1.dev3.tar", last modified: Wed May 31 14:07:33 2023, max compression
```

## Comparing `torchlie-0.0.1.dev2.tar` & `torchlie-0.0.1.dev3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-05-29 21:01:01.281989 torchlie-0.0.1.dev2/
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      526 2023-05-29 21:01:01.280410 torchlie-0.0.1.dev2/PKG-INFO
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        0 2023-05-29 19:37:31.000000 torchlie-0.0.1.dev2/README.md
-drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-05-29 21:01:01.229689 torchlie-0.0.1.dev2/lie/
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      521 2023-05-29 21:00:42.000000 torchlie-0.0.1.dev2/lie/__init__.py
-drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-05-29 21:01:01.259070 torchlie-0.0.1.dev2/lie/functional/
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      289 2023-05-05 15:22:31.000000 torchlie-0.0.1.dev2/lie/functional/__init__.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1282 2023-05-05 15:22:31.000000 torchlie-0.0.1.dev2/lie/functional/check_contexts.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1818 2023-05-08 21:17:15.000000 torchlie-0.0.1.dev2/lie/functional/constants.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    10767 2023-05-29 12:55:12.000000 torchlie-0.0.1.dev2/lie/functional/lie_group.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    32553 2023-05-29 12:55:12.000000 torchlie-0.0.1.dev2/lie/functional/se3_impl.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    35868 2023-05-29 14:04:19.000000 torchlie-0.0.1.dev2/lie/functional/so3_impl.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1259 2023-05-11 17:14:52.000000 torchlie-0.0.1.dev2/lie/functional/utils.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    20259 2023-05-29 20:03:35.000000 torchlie-0.0.1.dev2/lie/lie_tensor.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     3094 2023-05-29 20:03:09.000000 torchlie-0.0.1.dev2/lie/types.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)       38 2023-05-29 21:01:01.283016 torchlie-0.0.1.dev2/setup.cfg
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1184 2023-05-29 19:54:08.000000 torchlie-0.0.1.dev2/setup.py
-drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-05-29 21:01:01.275626 torchlie-0.0.1.dev2/torchlie.egg-info/
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      526 2023-05-29 21:01:01.000000 torchlie-0.0.1.dev2/torchlie.egg-info/PKG-INFO
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      387 2023-05-29 21:01:01.000000 torchlie-0.0.1.dev2/torchlie.egg-info/SOURCES.txt
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        1 2023-05-29 21:01:01.000000 torchlie-0.0.1.dev2/torchlie.egg-info/dependency_links.txt
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        4 2023-05-29 21:01:01.000000 torchlie-0.0.1.dev2/torchlie.egg-info/top_level.txt
+drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-05-31 14:07:33.661072 torchlie-0.0.1.dev3/
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      526 2023-05-31 14:07:33.659020 torchlie-0.0.1.dev3/PKG-INFO
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        0 2023-05-30 20:56:05.000000 torchlie-0.0.1.dev3/README.md
+drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-05-31 14:07:33.606418 torchlie-0.0.1.dev3/lie/
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      521 2023-05-31 14:05:55.000000 torchlie-0.0.1.dev3/lie/__init__.py
+drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-05-31 14:07:33.637227 torchlie-0.0.1.dev3/lie/functional/
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      289 2023-05-30 20:56:06.000000 torchlie-0.0.1.dev3/lie/functional/__init__.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1282 2023-05-30 20:56:06.000000 torchlie-0.0.1.dev3/lie/functional/check_contexts.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1818 2023-05-30 20:56:06.000000 torchlie-0.0.1.dev3/lie/functional/constants.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    10767 2023-05-30 20:56:06.000000 torchlie-0.0.1.dev3/lie/functional/lie_group.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    32596 2023-05-30 20:56:06.000000 torchlie-0.0.1.dev3/lie/functional/se3_impl.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    35868 2023-05-30 20:56:06.000000 torchlie-0.0.1.dev3/lie/functional/so3_impl.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1259 2023-05-30 20:56:06.000000 torchlie-0.0.1.dev3/lie/functional/utils.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    20259 2023-05-30 20:56:06.000000 torchlie-0.0.1.dev3/lie/lie_tensor.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     3094 2023-05-30 20:56:06.000000 torchlie-0.0.1.dev3/lie/types.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)       38 2023-05-31 14:07:33.662222 torchlie-0.0.1.dev3/setup.cfg
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1184 2023-05-30 20:56:06.000000 torchlie-0.0.1.dev3/setup.py
+drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-05-31 14:07:33.654709 torchlie-0.0.1.dev3/torchlie.egg-info/
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      526 2023-05-31 14:07:33.000000 torchlie-0.0.1.dev3/torchlie.egg-info/PKG-INFO
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      387 2023-05-31 14:07:33.000000 torchlie-0.0.1.dev3/torchlie.egg-info/SOURCES.txt
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        1 2023-05-31 14:07:33.000000 torchlie-0.0.1.dev3/torchlie.egg-info/dependency_links.txt
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        4 2023-05-31 14:07:33.000000 torchlie-0.0.1.dev3/torchlie.egg-info/top_level.txt
```

### Comparing `torchlie-0.0.1.dev2/PKG-INFO` & `torchlie-0.0.1.dev3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlie
-Version: 0.0.1.dev2
+Version: 0.0.1.dev3
 Summary: Torch extension for differentiable Lie groups.
 Home-page: https://github.com/facebookresearch/theseus/lie
 Author: Meta Research
 Keywords: lie groups,differentiable optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `torchlie-0.0.1.dev2/lie/__init__.py` & `torchlie-0.0.1.dev3/lie/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
-__version__ = "0.0.1.dev2"
+__version__ = "0.0.1.dev3"
 
 from .types import ltype, SE3, SO3
 from .lie_tensor import (  # usort: skip
     LieTensor,
     adj,
     as_euclidean,
     as_lietensor,
```

### Comparing `torchlie-0.0.1.dev2/lie/functional/check_contexts.py` & `torchlie-0.0.1.dev3/lie/functional/check_contexts.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev2/lie/functional/constants.py` & `torchlie-0.0.1.dev3/lie/functional/constants.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev2/lie/functional/lie_group.py` & `torchlie-0.0.1.dev3/lie/functional/lie_group.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev2/lie/functional/se3_impl.py` & `torchlie-0.0.1.dev3/lie/functional/se3_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -428,15 +428,17 @@
         / (theta4_nz * two_cosine_minus_two_nz),
     )
     d = torch.where(
         near_zero,
         -1 / 6.0 - theta2 / 180.0,
         (theta - sine) / (theta_nz * two_cosine_minus_two_nz),
     )
-    e = (ret_ang.view(*size, 1, 3) @ ret_lin.view(*size, 3, 1)).view(*size)
+
+    e = ret_ang.view(*size, 1, 3) @ ret_lin.view(*size, 3, 1)
+    e = e.view(*size) if len(size) > 0 else e.squeeze()
 
     ce_ret_ang = (c * e).view(*size, 1) * ret_ang
     jac[..., :3, 3:] = ce_ret_ang.view(*size, 3, 1) * ret_ang.view(*size, 1, 3)
     jac[..., :3, 3:] += b_ret_ang.view(*size, 3, 1) * ret_lin.view(
         *size, 1, 3
     ) + ret_lin.view(*size, 3, 1) * b_ret_ang.view(*size, 1, 3)
     diag_jac_t = torch.diagonal(jac[..., :3, 3:], dim1=-1, dim2=-2)
```

### Comparing `torchlie-0.0.1.dev2/lie/functional/so3_impl.py` & `torchlie-0.0.1.dev3/lie/functional/so3_impl.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev2/lie/functional/utils.py` & `torchlie-0.0.1.dev3/lie/functional/utils.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev2/lie/lie_tensor.py` & `torchlie-0.0.1.dev3/lie/lie_tensor.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev2/lie/types.py` & `torchlie-0.0.1.dev3/lie/types.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev2/setup.py` & `torchlie-0.0.1.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1.dev2/torchlie.egg-info/PKG-INFO` & `torchlie-0.0.1.dev3/torchlie.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlie
-Version: 0.0.1.dev2
+Version: 0.0.1.dev3
 Summary: Torch extension for differentiable Lie groups.
 Home-page: https://github.com/facebookresearch/theseus/lie
 Author: Meta Research
 Keywords: lie groups,differentiable optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

