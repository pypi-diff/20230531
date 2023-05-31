# Comparing `tmp/vocex-0.1.3.tar.gz` & `tmp/vocex-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocex-0.1.3.tar", last modified: Wed May 31 09:57:06 2023, max compression
+gzip compressed data, was "vocex-0.1.4.tar", last modified: Wed May 31 10:00:00 2023, max compression
```

## Comparing `vocex-0.1.3.tar` & `vocex-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        8 2023-05-08 02:42:27.826184 vocex-0.1.3/README.md
--rw-r--r--   0        0        0      398 2023-05-31 09:57:06.412112 vocex-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      507 2023-05-29 13:47:25.541785 vocex-0.1.3/vocex/__init__.py
--rw-r--r--   0        0        0     2025 2023-05-07 15:53:39.423391 vocex-0.1.3/vocex/conformer_layer.py
--rw-r--r--   0        0        0     8803 2023-05-28 21:24:30.563639 vocex-0.1.3/vocex/conformer_model.py
--rw-r--r--   0        0        0     4208 2023-05-27 22:17:11.509445 vocex-0.1.3/vocex/scaler.py
--rw-r--r--   0        0        0     3830 2023-05-24 18:47:16.895683 vocex-0.1.3/vocex/softdtw.py
--rw-r--r--   0        0        0     2460 2023-05-07 15:45:50.981971 vocex-0.1.3/vocex/transformer.py
--rw-r--r--   0        0        0     1756 2023-05-09 04:48:57.299991 vocex-0.1.3/vocex/utils.py
--rw-r--r--   0        0        0      270 1970-01-01 00:00:00.000000 vocex-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        8 2023-05-08 02:42:27.826184 vocex-0.1.4/README.md
+-rw-r--r--   0        0        0      398 2023-05-31 10:00:00.864400 vocex-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      507 2023-05-29 13:47:25.541785 vocex-0.1.4/vocex/__init__.py
+-rw-r--r--   0        0        0     2025 2023-05-07 15:53:39.423391 vocex-0.1.4/vocex/conformer_layer.py
+-rw-r--r--   0        0        0     8759 2023-05-31 09:59:22.905727 vocex-0.1.4/vocex/conformer_model.py
+-rw-r--r--   0        0        0     4208 2023-05-27 22:17:11.509445 vocex-0.1.4/vocex/scaler.py
+-rw-r--r--   0        0        0     3830 2023-05-24 18:47:16.895683 vocex-0.1.4/vocex/softdtw.py
+-rw-r--r--   0        0        0     2460 2023-05-07 15:45:50.981971 vocex-0.1.4/vocex/transformer.py
+-rw-r--r--   0        0        0     1756 2023-05-09 04:48:57.299991 vocex-0.1.4/vocex/utils.py
+-rw-r--r--   0        0        0      270 1970-01-01 00:00:00.000000 vocex-0.1.4/PKG-INFO
```

### Comparing `vocex-0.1.3/vocex/conformer_layer.py` & `vocex-0.1.4/vocex/conformer_layer.py`

 * *Files identical despite different names*

### Comparing `vocex-0.1.3/vocex/conformer_model.py` & `vocex-0.1.4/vocex/conformer_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import torch
 from torch import nn
 from tqdm.auto import tqdm
 from .transformer import TransformerEncoder, PositionalEncoding
 from .conformer_layer import ConformerLayer
 from .scaler import GaussianMinMaxScaler
 from .utils import Transpose, NoamLR
-from .tpu_metrics_delta import MetricsDelta
 from .softdtw import SoftDTW
 
 class VocexModel(nn.Module):
 
     def __init__(
         self,
         measures=["energy", "pitch", "srmr", "snr"],
```

### Comparing `vocex-0.1.3/vocex/scaler.py` & `vocex-0.1.4/vocex/scaler.py`

 * *Files identical despite different names*

### Comparing `vocex-0.1.3/vocex/softdtw.py` & `vocex-0.1.4/vocex/softdtw.py`

 * *Files identical despite different names*

### Comparing `vocex-0.1.3/vocex/transformer.py` & `vocex-0.1.4/vocex/transformer.py`

 * *Files identical despite different names*

### Comparing `vocex-0.1.3/vocex/utils.py` & `vocex-0.1.4/vocex/utils.py`

 * *Files identical despite different names*

