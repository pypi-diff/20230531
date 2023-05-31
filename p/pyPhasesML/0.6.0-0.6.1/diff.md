# Comparing `tmp/pyPhasesML-0.6.0.tar.gz` & `tmp/pyPhasesML-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesML-0.6.0.tar", last modified: Mon May 22 11:21:10 2023, max compression
+gzip compressed data, was "pyPhasesML-0.6.1.tar", last modified: Wed May 31 11:33:38 2023, max compression
```

## Comparing `pyPhasesML-0.6.0.tar` & `pyPhasesML-0.6.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:21:10.302827 pyPhasesML-0.6.0/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3691 2023-05-22 11:21:10.302827 pyPhasesML-0.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3184 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:21:10.298828 pyPhasesML-0.6.0/pyPhasesML/
--rw-rw-rw-   0 root         (0) root         (0)     2410 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/DataAugmentation.py
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/DataSet.py
--rw-rw-rw-   0 root         (0) root         (0)     3849 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/DataversionManager.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/FeatureExtraction.py
--rw-rw-rw-   0 root         (0) root         (0)     3798 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/Model.py
--rw-rw-rw-   0 root         (0) root         (0)     4491 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/ModelManager.py
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4566 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/SignalPreprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:21:10.300827 pyPhasesML-0.6.0/pyPhasesML/adapter/
--rw-rw-rw-   0 root         (0) root         (0)    10212 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/adapter/ModelKerasAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     7116 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/adapter/ModelTf1Adapter.py
--rw-rw-rw-   0 root         (0) root         (0)    18640 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/adapter/ModelTorchAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/adapter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:21:10.301828 pyPhasesML-0.6.0/pyPhasesML/datapipes/
--rw-rw-rw-   0 root         (0) root         (0)      464 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/datapipes/Augmentor.py
--rw-rw-rw-   0 root         (0) root         (0)      626 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/datapipes/DatasetXY.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/datapipes/FoldMapper.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/datapipes/RecordMap.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/datapipes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:21:10.301828 pyPhasesML-0.6.0/pyPhasesML/exporter/
--rw-rw-rw-   0 root         (0) root         (0)     5385 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/exporter/MemmapRecordExporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/exporter/ModelExporter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/exporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:21:10.302827 pyPhasesML-0.6.0/pyPhasesML/scorer/
--rw-rw-rw-   0 root         (0) root         (0)    18685 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/scorer/Scorer.py
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/scorer/ScorerTF.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/scorer/ScorerTorch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyPhasesML/scorer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:21:10.299827 pyPhasesML-0.6.0/pyPhasesML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3691 2023-05-22 11:21:10.000000 pyPhasesML-0.6.0/pyPhasesML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1041 2023-05-22 11:21:10.000000 pyPhasesML-0.6.0/pyPhasesML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 11:21:10.000000 pyPhasesML-0.6.0/pyPhasesML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-22 11:21:10.000000 pyPhasesML-0.6.0/pyPhasesML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-22 11:21:10.000000 pyPhasesML-0.6.0/pyPhasesML.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-05-22 11:20:45.000000 pyPhasesML-0.6.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 11:21:10.303827 pyPhasesML-0.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-05-22 11:20:47.000000 pyPhasesML-0.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:33:38.941336 pyPhasesML-0.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-05-31 11:33:38.940336 pyPhasesML-0.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3184 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:33:38.937336 pyPhasesML-0.6.1/pyPhasesML/
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/DataAugmentation.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/DataSet.py
+-rw-rw-rw-   0 root         (0) root         (0)     3849 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/DataversionManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/FeatureExtraction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3798 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/Model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4491 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/ModelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4566 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/SignalPreprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:33:38.938336 pyPhasesML-0.6.1/pyPhasesML/adapter/
+-rw-rw-rw-   0 root         (0) root         (0)    10212 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/adapter/ModelKerasAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     7116 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/adapter/ModelTf1Adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)    18468 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/adapter/ModelTorchAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/adapter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:33:38.939336 pyPhasesML-0.6.1/pyPhasesML/datapipes/
+-rw-rw-rw-   0 root         (0) root         (0)      464 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/datapipes/Augmentor.py
+-rw-rw-rw-   0 root         (0) root         (0)      626 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/datapipes/DatasetXY.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/datapipes/FoldMapper.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/datapipes/RecordMap.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/datapipes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:33:38.940336 pyPhasesML-0.6.1/pyPhasesML/exporter/
+-rw-rw-rw-   0 root         (0) root         (0)     5385 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/exporter/MemmapRecordExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/exporter/ModelExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/exporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:33:38.940336 pyPhasesML-0.6.1/pyPhasesML/scorer/
+-rw-rw-rw-   0 root         (0) root         (0)    18685 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/scorer/Scorer.py
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/scorer/ScorerTF.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/scorer/ScorerTorch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyPhasesML/scorer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:33:38.938336 pyPhasesML-0.6.1/pyPhasesML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-05-31 11:33:38.000000 pyPhasesML-0.6.1/pyPhasesML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-05-31 11:33:38.000000 pyPhasesML-0.6.1/pyPhasesML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 11:33:38.000000 pyPhasesML-0.6.1/pyPhasesML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-31 11:33:38.000000 pyPhasesML-0.6.1/pyPhasesML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-31 11:33:38.000000 pyPhasesML-0.6.1/pyPhasesML.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-05-31 11:33:21.000000 pyPhasesML-0.6.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 11:33:38.941336 pyPhasesML-0.6.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-05-31 11:33:22.000000 pyPhasesML-0.6.1/setup.py
```

### Comparing `pyPhasesML-0.6.0/LICENSE` & `pyPhasesML-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.0/PKG-INFO` & `pyPhasesML-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.6.0
+Version: 0.6.1
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.6.0/README.md` & `pyPhasesML-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.0/pyPhasesML/DataAugmentation.py` & `pyPhasesML-0.6.1/pyPhasesML/DataAugmentation.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.0/pyPhasesML/DataSet.py` & `pyPhasesML-0.6.1/pyPhasesML/DataSet.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.0/pyPhasesML/DataversionManager.py` & `pyPhasesML-0.6.1/pyPhasesML/DataversionManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.0/pyPhasesML/FeatureExtraction.py` & `pyPhasesML-0.6.1/pyPhasesML/FeatureExtraction.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.0/pyPhasesML/Model.py` & `pyPhasesML-0.6.1/pyPhasesML/Model.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.0/pyPhasesML/ModelManager.py` & `pyPhasesML-0.6.1/pyPhasesML/ModelManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.0/pyPhasesML/Plugin.py` & `pyPhasesML-0.6.1/pyPhasesML/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.0/pyPhasesML/SignalPreprocessing.py` & `pyPhasesML-0.6.1/pyPhasesML/SignalPreprocessing.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.0/pyPhasesML/adapter/ModelKerasAdapter.py` & `pyPhasesML-0.6.1/pyPhasesML/adapter/ModelKerasAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.0/pyPhasesML/adapter/ModelTf1Adapter.py` & `pyPhasesML-0.6.1/pyPhasesML/adapter/ModelTf1Adapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.0/pyPhasesML/adapter/ModelTorchAdapter.py` & `pyPhasesML-0.6.1/pyPhasesML/adapter/ModelTorchAdapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         else:
             targets = targets.reshape(-1)
 
             if self.ignoreClassIndex is not None:
                 mask = targets != self.ignoreClassIndex
                 targets = targets[mask]
 
-        return targets.float(), mask
+        return targets, mask
 
     def train(self, dataset: TrainingSetLoader):
         self.trigger("trainStart", self)
         if ModelTorchAdapter.useTensorBoard:
             from torch.utils.tensorboard import SummaryWriter
 
             self.summarywriter = SummaryWriter()
@@ -222,17 +222,14 @@
             smoothing = 0.05
         
         model = self.model
         lossCriterion = self.getLossFunction()
         i_epoch = self.startEpoch
         notImprovedSince = 0
         lastImprovdModel = None
-        
-        metricsValues, justPrint = self.evalValidation(dataset.validationData)
-        print(metricsValues)
 
         stopAfterNotImproving = 0 if self.stopAfterNotImproving is None else self.stopAfterNotImproving
 
         while self.maxEpochs is None or i_epoch < self.maxEpochs:
             # Put in train mode
             trainingStartTime = timeit.default_timer()
 
@@ -253,15 +250,15 @@
                 # check if there are any targets left
                 if len(targs) == 0:
                     continue
 
                 # for batchFeat in batchFeats:
                 output = model(batchFeats)
                 output = self.mapOutputForLoss(output, mask)
-                loss = lossCriterion(output, targs.reshape(1, 1))
+                loss = lossCriterion(output, targs)
                 ownStats = hasattr(lossCriterion, "stats")
 
                 if ownStats:
                     processList.set_postfix(ordered_dict=lossCriterion.stats)
                     for stat, value in lossCriterion.stats.items():
                         if stat not in runningStats:
                             runningStats[stat] = value
@@ -318,15 +315,14 @@
             runningStats = {n: v / batchesPerEpoch for n, v in runningStats.items()}
 
             i_epoch += 1
             trainingEndTime = timeit.default_timer()
 
             # Get validation accuracy
             metricsValues, justPrint = self.evalValidation(dataset.validationData)
-            print(metricsValues)
 
             metricStrings = []
             metricDiffStrings = []
             metricValuetrings = []
             improved = False
             modelId = "checkpointModel_%i_" % i_epoch
```

### Comparing `pyPhasesML-0.6.0/pyPhasesML/config.yaml` & `pyPhasesML-0.6.1/pyPhasesML/config.yaml`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.0/pyPhasesML/datapipes/DatasetXY.py` & `pyPhasesML-0.6.1/pyPhasesML/datapipes/DatasetXY.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.0/pyPhasesML/datapipes/FoldMapper.py` & `pyPhasesML-0.6.1/pyPhasesML/datapipes/FoldMapper.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.0/pyPhasesML/exporter/MemmapRecordExporter.py` & `pyPhasesML-0.6.1/pyPhasesML/exporter/MemmapRecordExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.0/pyPhasesML/exporter/ModelExporter.py` & `pyPhasesML-0.6.1/pyPhasesML/exporter/ModelExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.0/pyPhasesML/scorer/Scorer.py` & `pyPhasesML-0.6.1/pyPhasesML/scorer/Scorer.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.0/pyPhasesML.egg-info/PKG-INFO` & `pyPhasesML-0.6.1/pyPhasesML.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.6.0
+Version: 0.6.1
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.6.0/pyPhasesML.egg-info/SOURCES.txt` & `pyPhasesML-0.6.1/pyPhasesML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.6.0/setup.py` & `pyPhasesML-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesML",
-    version="v0.6.0"[1:],
+    version="v0.6.1"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Framework for creating a boilerplate template for ai projects that are ready for MLOps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/",
     packages=setuptools.find_packages(),
```

