# Comparing `tmp/tmcutils-0.2.tar.gz` & `tmp/tmcutils-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tmcutils-0.2.tar", last modified: Wed May 24 06:43:23 2023, max compression
+gzip compressed data, was "dist/tmcutils-0.3.tar", last modified: Wed May 31 15:25:13 2023, max compression
```

## Comparing `tmcutils-0.2.tar` & `tmcutils-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 alessandro  (1000) alessandro  (1000)        0 2023-05-24 06:43:23.625724 tmcutils-0.2/
--rw-rw-r--   0 alessandro  (1000) alessandro  (1000)      260 2023-05-24 06:43:23.625724 tmcutils-0.2/PKG-INFO
--rw-rw-r--   0 alessandro  (1000) alessandro  (1000)       34 2023-05-24 06:34:38.000000 tmcutils-0.2/README.rst
--rw-rw-r--   0 alessandro  (1000) alessandro  (1000)      107 2023-05-24 06:43:23.629724 tmcutils-0.2/setup.cfg
--rw-rw-r--   0 alessandro  (1000) alessandro  (1000)      385 2023-05-24 06:43:18.000000 tmcutils-0.2/setup.py
-drwxrwxr-x   0 alessandro  (1000) alessandro  (1000)        0 2023-05-24 06:43:23.625724 tmcutils-0.2/src/
-drwxrwxr-x   0 alessandro  (1000) alessandro  (1000)        0 2023-05-24 06:43:23.625724 tmcutils-0.2/src/tmcutils/
--rw-rw-r--   0 alessandro  (1000) alessandro  (1000)      931 2023-05-24 06:42:45.000000 tmcutils-0.2/src/tmcutils/__init__.py
-drwxrwxr-x   0 alessandro  (1000) alessandro  (1000)        0 2023-05-24 06:43:23.625724 tmcutils-0.2/src/tmcutils.egg-info/
--rw-rw-r--   0 alessandro  (1000) alessandro  (1000)      260 2023-05-24 06:43:23.000000 tmcutils-0.2/src/tmcutils.egg-info/PKG-INFO
--rw-rw-r--   0 alessandro  (1000) alessandro  (1000)      233 2023-05-24 06:43:23.000000 tmcutils-0.2/src/tmcutils.egg-info/SOURCES.txt
--rw-rw-r--   0 alessandro  (1000) alessandro  (1000)        1 2023-05-24 06:43:23.000000 tmcutils-0.2/src/tmcutils.egg-info/dependency_links.txt
--rw-rw-r--   0 alessandro  (1000) alessandro  (1000)        7 2023-05-24 06:43:23.000000 tmcutils-0.2/src/tmcutils.egg-info/requires.txt
--rw-rw-r--   0 alessandro  (1000) alessandro  (1000)        9 2023-05-24 06:43:23.000000 tmcutils-0.2/src/tmcutils.egg-info/top_level.txt
+drwxrwxr-x   0 alessandro  (1000) alessandro  (1000)        0 2023-05-31 15:25:13.300650 tmcutils-0.3/
+-rw-rw-r--   0 alessandro  (1000) alessandro  (1000)      260 2023-05-31 15:25:13.300650 tmcutils-0.3/PKG-INFO
+-rw-rw-r--   0 alessandro  (1000) alessandro  (1000)      133 2023-05-24 06:48:00.000000 tmcutils-0.3/README.rst
+-rw-rw-r--   0 alessandro  (1000) alessandro  (1000)      107 2023-05-31 15:25:13.304650 tmcutils-0.3/setup.cfg
+-rw-rw-r--   0 alessandro  (1000) alessandro  (1000)      385 2023-05-31 15:24:36.000000 tmcutils-0.3/setup.py
+drwxrwxr-x   0 alessandro  (1000) alessandro  (1000)        0 2023-05-31 15:25:13.300650 tmcutils-0.3/src/
+drwxrwxr-x   0 alessandro  (1000) alessandro  (1000)        0 2023-05-31 15:25:13.300650 tmcutils-0.3/src/tmcutils/
+-rw-rw-r--   0 alessandro  (1000) alessandro  (1000)     1641 2023-05-31 15:25:04.000000 tmcutils-0.3/src/tmcutils/__init__.py
+drwxrwxr-x   0 alessandro  (1000) alessandro  (1000)        0 2023-05-31 15:25:13.300650 tmcutils-0.3/src/tmcutils.egg-info/
+-rw-rw-r--   0 alessandro  (1000) alessandro  (1000)      260 2023-05-31 15:25:13.000000 tmcutils-0.3/src/tmcutils.egg-info/PKG-INFO
+-rw-rw-r--   0 alessandro  (1000) alessandro  (1000)      233 2023-05-31 15:25:13.000000 tmcutils-0.3/src/tmcutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 alessandro  (1000) alessandro  (1000)        1 2023-05-31 15:25:13.000000 tmcutils-0.3/src/tmcutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 alessandro  (1000) alessandro  (1000)        7 2023-05-31 15:25:13.000000 tmcutils-0.3/src/tmcutils.egg-info/requires.txt
+-rw-rw-r--   0 alessandro  (1000) alessandro  (1000)        9 2023-05-31 15:25:13.000000 tmcutils-0.3/src/tmcutils.egg-info/top_level.txt
```

### Comparing `tmcutils-0.2/src/tmcutils/__init__.py` & `tmcutils-0.3/src/tmcutils/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import ssl
 import urllib.request
 
 import pandas as pd
 
 
 class Client(object):
     def __init__(self, base):
@@ -20,7 +21,23 @@
         report = pd.DataFrame.from_dict(r['values'])
         report = report[['experiment', 'experiment_id', 'seed', 'epoch'] + [x for x in r['metrics'] if x not in ('experiment', 'epoch')]]
         parameters = r['parameters']
         # parameters = pd.DataFrame.from_dict(parameters)
         parameters = pd.DataFrame.from_dict(parameters, orient='index')
         parameters['experiment_id'] = [int(x) for x in parameters.index]
         return report, parameters
+
+    def save_history(self, experiment: str, seed: int, history, parameters: dict):
+        """
+        curl {BASE}/mlexperiments/register -d '{"experiment":"prova", "metrics":{"ACC":12.3} }'
+        """
+
+
+
+        for epoch in history.epoch:
+            metrics = {metric: history.history[metric][epoch] for metric in history.history.keys()}
+            payload = {"experiment": experiment, "metrics": metrics, "seed": seed, "parameters": parameters}
+            r = urllib.request.urlopen(
+                f"{self.BASE}/analysis/mlexperiments/epochs/seamlexperiments/registerrch",
+                data=json.dumps(payload).encode('utf8'),
+                context=ssl._create_unverified_context())
+
```

