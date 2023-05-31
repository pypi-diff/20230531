# Comparing `tmp/easytorch-3.8.1.tar.gz` & `tmp/easytorch-3.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytorch-3.8.1.tar", last modified: Sun May 28 12:52:49 2023, max compression
+gzip compressed data, was "easytorch-3.8.2.tar", last modified: Wed May 31 16:06:20 2023, max compression
```

## Comparing `easytorch-3.8.1.tar` & `easytorch-3.8.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:52:49.000995 easytorch-3.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-28 12:52:29.000000 easytorch-3.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-28 12:52:49.000995 easytorch-3.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-28 12:52:29.000000 easytorch-3.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:52:48.992995 easytorch-3.8.1/easytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-28 12:52:29.000000 easytorch-3.8.1/easytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:52:48.996995 easytorch-3.8.1/easytorch/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-28 12:52:29.000000 easytorch-3.8.1/easytorch/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-28 12:52:29.000000 easytorch-3.8.1/easytorch/config/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:52:48.996995 easytorch-3.8.1/easytorch/data/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-28 12:52:29.000000 easytorch-3.8.1/easytorch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-05-28 12:52:29.000000 easytorch-3.8.1/easytorch/data/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-28 12:52:29.000000 easytorch-3.8.1/easytorch/data/datautils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-28 12:52:29.000000 easytorch-3.8.1/easytorch/data/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13268 2023-05-28 12:52:29.000000 easytorch-3.8.1/easytorch/easytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:52:48.996995 easytorch-3.8.1/easytorch/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-28 12:52:29.000000 easytorch-3.8.1/easytorch/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-28 12:52:29.000000 easytorch-3.8.1/easytorch/metrics/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-05-28 12:52:29.000000 easytorch-3.8.1/easytorch/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19093 2023-05-28 12:52:29.000000 easytorch-3.8.1/easytorch/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:52:48.996995 easytorch-3.8.1/easytorch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-28 12:52:29.000000 easytorch-3.8.1/easytorch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-28 12:52:29.000000 easytorch-3.8.1/easytorch/utils/ddp_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-28 12:52:29.000000 easytorch-3.8.1/easytorch/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-28 12:52:29.000000 easytorch-3.8.1/easytorch/utils/tensorutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:52:49.000995 easytorch-3.8.1/easytorch/vision/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-28 12:52:29.000000 easytorch-3.8.1/easytorch/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-05-28 12:52:29.000000 easytorch-3.8.1/easytorch/vision/imageutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-28 12:52:29.000000 easytorch-3.8.1/easytorch/vision/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-28 12:52:29.000000 easytorch-3.8.1/easytorch/vision/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 12:52:48.992995 easytorch-3.8.1/easytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-28 12:52:48.000000 easytorch-3.8.1/easytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-28 12:52:48.000000 easytorch-3.8.1/easytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 12:52:48.000000 easytorch-3.8.1/easytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-28 12:52:48.000000 easytorch-3.8.1/easytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-28 12:52:48.000000 easytorch-3.8.1/easytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 12:52:49.000995 easytorch-3.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-28 12:52:29.000000 easytorch-3.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:06:20.810397 easytorch-3.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-31 16:06:08.000000 easytorch-3.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-31 16:06:20.810397 easytorch-3.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-31 16:06:08.000000 easytorch-3.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:06:20.810397 easytorch-3.8.2/easytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-31 16:06:08.000000 easytorch-3.8.2/easytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:06:20.810397 easytorch-3.8.2/easytorch/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-31 16:06:08.000000 easytorch-3.8.2/easytorch/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-31 16:06:08.000000 easytorch-3.8.2/easytorch/config/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:06:20.810397 easytorch-3.8.2/easytorch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-31 16:06:08.000000 easytorch-3.8.2/easytorch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-05-31 16:06:08.000000 easytorch-3.8.2/easytorch/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-31 16:06:08.000000 easytorch-3.8.2/easytorch/data/datautils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-31 16:06:08.000000 easytorch-3.8.2/easytorch/data/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13268 2023-05-31 16:06:08.000000 easytorch-3.8.2/easytorch/easytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:06:20.810397 easytorch-3.8.2/easytorch/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-31 16:06:08.000000 easytorch-3.8.2/easytorch/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-31 16:06:08.000000 easytorch-3.8.2/easytorch/metrics/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-05-31 16:06:08.000000 easytorch-3.8.2/easytorch/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19088 2023-05-31 16:06:08.000000 easytorch-3.8.2/easytorch/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:06:20.810397 easytorch-3.8.2/easytorch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-31 16:06:08.000000 easytorch-3.8.2/easytorch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-31 16:06:08.000000 easytorch-3.8.2/easytorch/utils/ddp_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-31 16:06:08.000000 easytorch-3.8.2/easytorch/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-31 16:06:08.000000 easytorch-3.8.2/easytorch/utils/tensorutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:06:20.810397 easytorch-3.8.2/easytorch/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-31 16:06:08.000000 easytorch-3.8.2/easytorch/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-05-31 16:06:08.000000 easytorch-3.8.2/easytorch/vision/imageutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-31 16:06:08.000000 easytorch-3.8.2/easytorch/vision/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-31 16:06:08.000000 easytorch-3.8.2/easytorch/vision/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 16:06:20.810397 easytorch-3.8.2/easytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-31 16:06:20.000000 easytorch-3.8.2/easytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-31 16:06:20.000000 easytorch-3.8.2/easytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 16:06:20.000000 easytorch-3.8.2/easytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-31 16:06:20.000000 easytorch-3.8.2/easytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 16:06:20.000000 easytorch-3.8.2/easytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 16:06:20.810397 easytorch-3.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-31 16:06:08.000000 easytorch-3.8.2/setup.py
```

### Comparing `easytorch-3.8.1/LICENSE` & `easytorch-3.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easytorch-3.8.1/PKG-INFO` & `easytorch-3.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytorch
-Version: 3.8.1
+Version: 3.8.2
 Summary: Easy Neural Network Experiments with pytorch
 Home-page: https://github.com/sraashis/easytorch
 Author: Aashis Khana1
 Author-email: sraashis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `easytorch-3.8.1/README.md` & `easytorch-3.8.2/README.md`

 * *Files identical despite different names*

### Comparing `easytorch-3.8.1/easytorch/config/__init__.py` & `easytorch-3.8.2/easytorch/config/__init__.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.8.1/easytorch/config/state.py` & `easytorch-3.8.2/easytorch/config/state.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.8.1/easytorch/data/data.py` & `easytorch-3.8.2/easytorch/data/data.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.8.1/easytorch/data/datautils.py` & `easytorch-3.8.2/easytorch/data/datautils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.8.1/easytorch/data/multiproc.py` & `easytorch-3.8.2/easytorch/data/multiproc.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.8.1/easytorch/easytorch.py` & `easytorch-3.8.2/easytorch/easytorch.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.8.1/easytorch/metrics/loss.py` & `easytorch-3.8.2/easytorch/metrics/loss.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.8.1/easytorch/metrics/metrics.py` & `easytorch-3.8.2/easytorch/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.8.1/easytorch/runner.py` & `easytorch-3.8.2/easytorch/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,15 +388,15 @@
         for i, batch in enumerate(dataloader, 1):
             self.batch_index = i
             it = self.iteration(batch)
             self.save_predictions(dataloader.dataset, it, writer=results_writer)
             info(f"{self.conf['name']}, batch {i}/{len(dataloader)} done", self.conf['verbose'])
 
         success(f"{self.conf['name']}, Inference results saved in:"
-                f"\n\t{self.cache['output_csv']}", self.conf['verbose'])
+                f"\n\t{results_writer.name}", self.conf['verbose'])
 
     def train(self, train_loader, validation_loader) -> None:
         ep = 0
         for ep in range(1, self.conf['epochs'] + 1):
             self.mode = Phase.TRAIN
             self.epoch = ep
```

### Comparing `easytorch-3.8.1/easytorch/utils/__init__.py` & `easytorch-3.8.2/easytorch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.8.1/easytorch/utils/ddp_check.py` & `easytorch-3.8.2/easytorch/utils/ddp_check.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.8.1/easytorch/utils/tensorutils.py` & `easytorch-3.8.2/easytorch/utils/tensorutils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.8.1/easytorch/vision/imageutils.py` & `easytorch-3.8.2/easytorch/vision/imageutils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.8.1/easytorch/vision/plotter.py` & `easytorch-3.8.2/easytorch/vision/plotter.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.8.1/easytorch/vision/transforms.py` & `easytorch-3.8.2/easytorch/vision/transforms.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.8.1/easytorch.egg-info/PKG-INFO` & `easytorch-3.8.2/easytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytorch
-Version: 3.8.1
+Version: 3.8.2
 Summary: Easy Neural Network Experiments with pytorch
 Home-page: https://github.com/sraashis/easytorch
 Author: Aashis Khana1
 Author-email: sraashis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `easytorch-3.8.1/easytorch.egg-info/SOURCES.txt` & `easytorch-3.8.2/easytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easytorch-3.8.1/setup.py` & `easytorch-3.8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     import cv2
 except:
     _requires.append('opencv-contrib-python-headless')
 
 # This call to setup() does all the work
 setup(
     name="easytorch",
-    version="3.8.1",
+    version="3.8.2",
     description="Easy Neural Network Experiments with pytorch",
     long_description=_README,
     long_description_content_type="text/markdown",
     url="https://github.com/sraashis/easytorch",
     author="Aashis Khana1",
     author_email="sraashis@gmail.com",
     license="MIT",
```

