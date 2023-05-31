# Comparing `tmp/processview-1.1.0.tar.gz` & `tmp/processview-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processview-1.1.0.tar", last modified: Wed Nov 16 15:21:27 2022, max compression
+gzip compressed data, was "processview-1.2.0.tar", last modified: Wed May 31 14:37:04 2023, max compression
```

## Comparing `processview-1.1.0.tar` & `processview-1.2.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-11-16 15:21:27.313486 processview-1.1.0/
--rw-r--r--   0 payno    (81067) soft      (3401)        0 2021-10-26 07:14:42.000000 processview-1.1.0/LICENSE
--rw-r--r--   0 payno    (81067) soft      (3401)     1245 2022-11-16 15:21:27.313486 processview-1.1.0/PKG-INFO
--rw-r--r--   0 payno    (81067) soft      (3401)      306 2021-10-26 07:14:42.000000 processview-1.1.0/README.md
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-11-16 15:21:27.305486 processview-1.1.0/processview/
--rw-r--r--   0 payno    (81067) soft      (3401)        0 2021-10-26 07:14:42.000000 processview-1.1.0/processview/__init__.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-11-16 15:21:27.309486 processview-1.1.0/processview/core/
--rw-r--r--   0 payno    (81067) soft      (3401)        0 2021-10-26 07:14:42.000000 processview-1.1.0/processview/core/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2352 2022-08-22 08:58:53.000000 processview-1.1.0/processview/core/dataset.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2350 2021-10-26 07:14:42.000000 processview-1.1.0/processview/core/helpers.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-11-16 15:21:27.309486 processview-1.1.0/processview/core/manager/
--rw-r--r--   0 payno    (81067) soft      (3401)       23 2021-10-26 07:14:42.000000 processview-1.1.0/processview/core/manager/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)    13677 2022-08-22 08:58:53.000000 processview-1.1.0/processview/core/manager/manager.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-11-16 15:21:27.309486 processview-1.1.0/processview/core/manager/test/
--rw-r--r--   0 payno    (81067) soft      (3401)     1534 2021-10-26 07:14:42.000000 processview-1.1.0/processview/core/manager/test/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)     4815 2022-08-22 08:58:53.000000 processview-1.1.0/processview/core/manager/test/test_manager.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1745 2021-10-26 07:14:42.000000 processview-1.1.0/processview/core/setup.py
--rw-r--r--   0 payno    (81067) soft      (3401)     5128 2021-11-10 14:06:33.000000 processview-1.1.0/processview/core/superviseprocess.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-11-16 15:21:27.309486 processview-1.1.0/processview/core/test/
--rw-r--r--   0 payno    (81067) soft      (3401)     1561 2021-10-26 07:14:42.000000 processview-1.1.0/processview/core/test/__init__.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-11-16 15:21:27.309486 processview-1.1.0/processview/gui/
--rw-r--r--   0 payno    (81067) soft      (3401)        0 2021-10-26 07:14:42.000000 processview-1.1.0/processview/gui/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)    12927 2021-10-26 07:14:42.000000 processview-1.1.0/processview/gui/icons.py
--rw-r--r--   0 payno    (81067) soft      (3401)     2296 2021-10-26 07:14:42.000000 processview-1.1.0/processview/gui/messagebox.py
--rw-r--r--   0 payno    (81067) soft      (3401)    20815 2022-11-16 15:15:49.000000 processview-1.1.0/processview/gui/processmanager.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-11-16 15:21:27.309486 processview-1.1.0/processview/gui/test/
--rw-r--r--   0 payno    (81067) soft      (3401)     1584 2021-10-26 07:14:42.000000 processview-1.1.0/processview/gui/test/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)     3620 2022-08-22 08:58:53.000000 processview-1.1.0/processview/gui/test/test_process_manager.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-11-16 15:21:27.309486 processview-1.1.0/processview/resources/
--rw-r--r--   0 payno    (81067) soft      (3401)    10757 2022-08-22 08:58:53.000000 processview-1.1.0/processview/resources/__init__.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-11-16 15:21:27.305486 processview-1.1.0/processview/resources/gui/
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-11-16 15:21:27.313486 processview-1.1.0/processview/resources/gui/icons/
--rw-r--r--   0 payno    (81067) soft      (3401)      729 2021-10-26 07:14:42.000000 processview-1.1.0/processview/resources/gui/icons/advancement.png
--rw-r--r--   0 payno    (81067) soft      (3401)     5781 2021-10-26 07:14:42.000000 processview-1.1.0/processview/resources/gui/icons/advancement.svg
--rw-r--r--   0 payno    (81067) soft      (3401)      926 2021-10-26 07:14:42.000000 processview-1.1.0/processview/resources/gui/icons/magnifying_glass.png
--rw-r--r--   0 payno    (81067) soft      (3401)     4631 2021-10-26 07:14:42.000000 processview-1.1.0/processview/resources/gui/icons/magnifying_glass.svg
--rw-r--r--   0 payno    (81067) soft      (3401)     1822 2021-10-26 07:14:42.000000 processview-1.1.0/processview/setup.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-11-16 15:21:27.313486 processview-1.1.0/processview/test/
--rw-r--r--   0 payno    (81067) soft      (3401)     1695 2021-10-26 07:14:42.000000 processview-1.1.0/processview/test/__init__.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-11-16 15:21:27.313486 processview-1.1.0/processview/utils/
--rw-r--r--   0 payno    (81067) soft      (3401)     2565 2021-10-26 07:14:42.000000 processview-1.1.0/processview/utils/__init__.py
--rw-r--r--   0 payno    (81067) soft      (3401)     1559 2021-10-26 07:14:42.000000 processview-1.1.0/processview/utils/singleton.py
--rw-r--r--   0 payno    (81067) soft      (3401)     4411 2022-11-16 15:20:51.000000 processview-1.1.0/processview/version.py
-drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2022-11-16 15:21:27.309486 processview-1.1.0/processview.egg-info/
--rw-r--r--   0 payno    (81067) soft      (3401)     1245 2022-11-16 15:21:26.000000 processview-1.1.0/processview.egg-info/PKG-INFO
--rw-r--r--   0 payno    (81067) soft      (3401)     1166 2022-11-16 15:21:27.000000 processview-1.1.0/processview.egg-info/SOURCES.txt
--rw-r--r--   0 payno    (81067) soft      (3401)        1 2022-11-16 15:21:26.000000 processview-1.1.0/processview.egg-info/dependency_links.txt
--rw-r--r--   0 payno    (81067) soft      (3401)        1 2021-10-26 07:15:14.000000 processview-1.1.0/processview.egg-info/not-zip-safe
--rw-r--r--   0 payno    (81067) soft      (3401)       26 2022-11-16 15:21:26.000000 processview-1.1.0/processview.egg-info/requires.txt
--rw-r--r--   0 payno    (81067) soft      (3401)       12 2022-11-16 15:21:26.000000 processview-1.1.0/processview.egg-info/top_level.txt
--rw-r--r--   0 payno    (81067) soft      (3401)       38 2022-11-16 15:21:27.313486 processview-1.1.0/setup.cfg
--rw-r--r--   0 payno    (81067) soft      (3401)    19207 2022-08-22 08:58:53.000000 processview-1.1.0/setup.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.312884 processview-1.2.0/
+-rw-r--r--   0 payno    (81067) soft      (3401)        0 2021-10-26 07:14:42.000000 processview-1.2.0/LICENSE
+-rw-r--r--   0 payno    (81067) soft      (3401)     1043 2023-05-31 14:37:04.312884 processview-1.2.0/PKG-INFO
+-rw-r--r--   0 payno    (81067) soft      (3401)      767 2023-02-02 10:20:46.000000 processview-1.2.0/README.md
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.308884 processview-1.2.0/processview/
+-rw-r--r--   0 payno    (81067) soft      (3401)       91 2023-05-31 13:34:50.000000 processview-1.2.0/processview/__init__.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.308884 processview-1.2.0/processview/core/
+-rw-r--r--   0 payno    (81067) soft      (3401)        0 2021-10-26 07:14:42.000000 processview-1.2.0/processview/core/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     3289 2023-05-31 13:32:57.000000 processview-1.2.0/processview/core/dataset.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2350 2021-10-26 07:14:42.000000 processview-1.2.0/processview/core/helpers.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.308884 processview-1.2.0/processview/core/manager/
+-rw-r--r--   0 payno    (81067) soft      (3401)       23 2021-10-26 07:14:42.000000 processview-1.2.0/processview/core/manager/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    13677 2023-05-25 09:34:28.000000 processview-1.2.0/processview/core/manager/manager.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.308884 processview-1.2.0/processview/core/manager/test/
+-rw-r--r--   0 payno    (81067) soft      (3401)     1534 2021-10-26 07:14:42.000000 processview-1.2.0/processview/core/manager/test/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     4823 2023-05-31 13:34:50.000000 processview-1.2.0/processview/core/manager/test/test_manager.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     1745 2021-10-26 07:14:42.000000 processview-1.2.0/processview/core/setup.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     1067 2023-05-31 12:17:21.000000 processview-1.2.0/processview/core/sorting.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     5128 2021-11-10 14:06:33.000000 processview-1.2.0/processview/core/superviseprocess.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.308884 processview-1.2.0/processview/core/test/
+-rw-r--r--   0 payno    (81067) soft      (3401)     1561 2021-10-26 07:14:42.000000 processview-1.2.0/processview/core/test/__init__.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.312884 processview-1.2.0/processview/gui/
+-rw-r--r--   0 payno    (81067) soft      (3401)        0 2021-10-26 07:14:42.000000 processview-1.2.0/processview/gui/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    12926 2023-03-30 07:14:30.000000 processview-1.2.0/processview/gui/icons.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     2296 2021-10-26 07:14:42.000000 processview-1.2.0/processview/gui/messagebox.py
+-rw-r--r--   0 payno    (81067) soft      (3401)    25054 2023-05-31 14:28:04.000000 processview-1.2.0/processview/gui/processmanager.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.312884 processview-1.2.0/processview/gui/test/
+-rw-r--r--   0 payno    (81067) soft      (3401)     1584 2021-10-26 07:14:42.000000 processview-1.2.0/processview/gui/test/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     3666 2023-05-31 13:36:47.000000 processview-1.2.0/processview/gui/test/test_process_manager.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.312884 processview-1.2.0/processview/resources/
+-rw-r--r--   0 payno    (81067) soft      (3401)    10757 2022-08-22 08:58:53.000000 processview-1.2.0/processview/resources/__init__.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.308884 processview-1.2.0/processview/resources/gui/
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.312884 processview-1.2.0/processview/resources/gui/icons/
+-rw-r--r--   0 payno    (81067) soft      (3401)      729 2021-10-26 07:14:42.000000 processview-1.2.0/processview/resources/gui/icons/advancement.png
+-rw-r--r--   0 payno    (81067) soft      (3401)     5781 2021-10-26 07:14:42.000000 processview-1.2.0/processview/resources/gui/icons/advancement.svg
+-rw-r--r--   0 payno    (81067) soft      (3401)      926 2021-10-26 07:14:42.000000 processview-1.2.0/processview/resources/gui/icons/magnifying_glass.png
+-rw-r--r--   0 payno    (81067) soft      (3401)     4631 2021-10-26 07:14:42.000000 processview-1.2.0/processview/resources/gui/icons/magnifying_glass.svg
+-rw-r--r--   0 payno    (81067) soft      (3401)     1822 2021-10-26 07:14:42.000000 processview-1.2.0/processview/setup.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.312884 processview-1.2.0/processview/test/
+-rw-r--r--   0 payno    (81067) soft      (3401)     1695 2021-10-26 07:14:42.000000 processview-1.2.0/processview/test/__init__.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.312884 processview-1.2.0/processview/utils/
+-rw-r--r--   0 payno    (81067) soft      (3401)     2565 2021-10-26 07:14:42.000000 processview-1.2.0/processview/utils/__init__.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     1559 2021-10-26 07:14:42.000000 processview-1.2.0/processview/utils/singleton.py
+-rw-r--r--   0 payno    (81067) soft      (3401)     4411 2023-05-31 13:34:50.000000 processview-1.2.0/processview/version.py
+drwxr-xr-x   0 payno    (81067) soft      (3401)        0 2023-05-31 14:37:04.308884 processview-1.2.0/processview.egg-info/
+-rw-r--r--   0 payno    (81067) soft      (3401)     1043 2023-05-31 14:37:03.000000 processview-1.2.0/processview.egg-info/PKG-INFO
+-rw-r--r--   0 payno    (81067) soft      (3401)     1200 2023-05-31 14:37:04.000000 processview-1.2.0/processview.egg-info/SOURCES.txt
+-rw-r--r--   0 payno    (81067) soft      (3401)        1 2023-05-31 14:37:03.000000 processview-1.2.0/processview.egg-info/dependency_links.txt
+-rw-r--r--   0 payno    (81067) soft      (3401)       73 2023-05-31 14:37:03.000000 processview-1.2.0/processview.egg-info/requires.txt
+-rw-r--r--   0 payno    (81067) soft      (3401)       12 2023-05-31 14:37:04.000000 processview-1.2.0/processview.egg-info/top_level.txt
+-rw-r--r--   0 payno    (81067) soft      (3401)        1 2023-05-31 12:44:26.000000 processview-1.2.0/processview.egg-info/zip-safe
+-rw-r--r--   0 payno    (81067) soft      (3401)     1089 2023-05-31 14:37:04.312884 processview-1.2.0/setup.cfg
+-rw-r--r--   0 payno    (81067) soft      (3401)       69 2023-05-31 13:34:50.000000 processview-1.2.0/setup.py
```

### Comparing `processview-1.1.0/processview/core/dataset.py` & `processview-1.2.0/processview/core/dataset.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,34 +25,54 @@
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "29/01/2021"
 
 
 from typing import Optional
+from datetime import datetime
 
 
 class DatasetIdentifier:
-    def __init__(self, data_builder):
+    def __init__(self, data_builder, metadata: Optional[dict] = None):
         """
         function that can be called to build data
+
+        :param data_builder: call back to create the Dataset from its identifier
+        :param Optional[dict] metadata: some metadata that could be provided in order to sort identifier between them. For now possible keys are:
+            * `name`: name to be used to sort dataset
+            * `creation_time`: creation of the dataset
+            * `modification_time`: modification of the dataset
         """
         self._dataset_builder = data_builder
+        metadata = metadata or {}
+        self.__creation_time = metadata.get("creation_time", None)
+        self.__modification_time = metadata.get("modification_time", None)
+        self.__name = metadata.get("name", None)
 
     def recreate_dataset(self):
         """Recreate the dataset from the identifier"""
         return self._dataset_builder(self)
 
     def long_description(self) -> str:
         """long description of the identifier"""
         return ""
 
     def short_description(self) -> Optional[str]:
         return None
 
+    def creation_time(self) -> Optional[datetime]:
+        return self.__creation_time
+
+    def modification_time(self) -> Optional[datetime]:
+        return self.__modification_time
+
+    def name(self) -> Optional[str]:
+        return self.__name
+
 
 class Dataset:
     """Base class that class processes should inherit"""
 
     @staticmethod
     def from_identifier(identifier):
         """Return the Dataset from a identifier"""
```

### Comparing `processview-1.1.0/processview/core/helpers.py` & `processview-1.2.0/processview/core/helpers.py`

 * *Files identical despite different names*

### Comparing `processview-1.1.0/processview/core/manager/manager.py` & `processview-1.2.0/processview/core/manager/manager.py`

 * *Files identical despite different names*

### Comparing `processview-1.1.0/processview/core/manager/test/__init__.py` & `processview-1.2.0/processview/core/manager/test/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.1.0/processview/core/manager/test/test_manager.py` & `processview-1.2.0/processview/core/manager/test/test_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,25 +117,24 @@
 
     def get_identifier(self) -> DatasetIdentifier:
         return _DummyIdentifier(self)
 
 
 class _DummyIdentifier(DatasetIdentifier):
     def __init__(self, dataset):
-        super().__init__(dataset)
-        self.name = dataset.name
+        super().__init__(dataset, metadata={"name": dataset.name})
 
     def __str__(self):
-        return self.name
+        return self.name()
 
     def __eq__(self, other):
-        return self.name == other.name
+        return self.name() == other.name()
 
     def __hash__(self):
-        return hash(self.name)
+        return hash(self.name())
 
 
 def suite():
     test_suite = unittest.TestSuite()
     for ui in (TestProcessManager,):
         test_suite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(ui))
     return test_suite
```

### Comparing `processview-1.1.0/processview/core/setup.py` & `processview-1.2.0/processview/core/setup.py`

 * *Files identical despite different names*

### Comparing `processview-1.1.0/processview/core/superviseprocess.py` & `processview-1.2.0/processview/core/superviseprocess.py`

 * *Files identical despite different names*

### Comparing `processview-1.1.0/processview/core/test/__init__.py` & `processview-1.2.0/processview/core/test/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.1.0/processview/gui/icons.py` & `processview-1.2.0/processview/gui/icons.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,14 @@
     :param str name: Name of the icon, in one of the defined icons
                      in this module.
     :return: Corresponding AbstractAnimatedIcon
     :raises: ValueError when name is not known
     """
     key = name + "__anim"
     if key not in _cached_icons:
-
         qtMajorVersion = int(qt.qVersion().split(".")[0])
         icon = None
 
         # ignore mng and gif in Qt5
         if qtMajorVersion != 5:
             try:
                 icon = MovieAnimatedIcon(name)
```

### Comparing `processview-1.1.0/processview/gui/messagebox.py` & `processview-1.2.0/processview/gui/messagebox.py`

 * *Files identical despite different names*

### Comparing `processview-1.1.0/processview/gui/processmanager.py` & `processview-1.2.0/processview/gui/processmanager.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,26 +25,29 @@
 
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "03/11/2020"
 
 
+import fnmatch
+from collections import OrderedDict
 from typing import Union
+import datetime
+
 from silx.gui import qt
-from collections import OrderedDict
+
+from processview.core.dataset import DatasetIdentifier
 from processview.core.manager import DatasetState
 from processview.core.manager import ProcessManager as _ProcessManager
+from processview.core.sorting import SortType, tooltips
 from processview.core.superviseprocess import SuperviseProcess
-from processview.core.dataset import DatasetIdentifier
 from processview.gui import icons as icons
 from processview.gui.messagebox import MessageBox
 from processview.utils import docstring
-import fnmatch
-
 
 _DATASET_STATE_BACKGROUND = {
     DatasetState.ON_GOING: qt.QColor("#839684"),  # light blue
     DatasetState.SUCCEED: qt.QColor("#068c0c"),  # green
     DatasetState.FAILED: qt.QColor("#f52718"),  # red
     DatasetState.PENDING: qt.QColor("#609ab3"),  # blue gray
     DatasetState.SKIPPED: qt.QColor("#f08e0e"),  # light orange
@@ -62,14 +65,18 @@
         self.setWindowFlags(qt.Qt.Widget)
 
         self._centralWidget = ProcessManagerWidget(parent=self)
         self.setCentralWidget(self._centralWidget)
 
 
 class ObservationTable(qt.QTableView):
+    """
+    Redefinition of QTableView for datasets and processes
+    """
+
     def __init__(self, parent):
         qt.QTableView.__init__(self, parent)
         self.verticalHeader().setSectionsClickable(True)
 
         # QMenu for cell from on dataset and one process
         self.menu_dataset_vs_process = qt.QMenu()
         self._reprocessAction = qt.QAction("reprocess")
@@ -85,52 +92,48 @@
         self.copy_menu.addAction(self._copyAction)
 
         # connect signal / slot
         self._copyAction.triggered.connect(self._requestDatasetIdCopy)
         self._reprocessAction.triggered.connect(self._requestReprocessing)
         self._infoAction.triggered.connect(self._requestInfo)
 
-        self.verticalHeader().setContextMenuPolicy(qt.Qt.CustomContextMenu)
-        self.verticalHeader().customContextMenuRequested.connect(
-            self._activeVerticalHeaderMenu
-        )
-
     def _processAt(self, x_pos):
         column = self.columnAt(x_pos)
-        if column >= 0:
+        if column >= 1:
             processes = self.model()._processes
-            if column < len(processes):
-                return processes[list(processes.keys())[column]]
+            process_idx = column - 1
+            if process_idx < len(processes):
+                return processes[list(processes.keys())[process_idx]]
 
     def _datasetAt(self, y_pos):
         row = self.rowAt(y_pos)
         if row >= 0:
             datasets = self.model()._datasets
             if row < len(datasets):
                 return datasets[list(datasets.keys())[row]]
 
-    def _activeVerticalHeaderMenu(self, pos):
-        process = self._processAt(pos.x())
-        dataset = self._datasetAt(pos.y())
-        if dataset is not None:
-            self._target = (None, dataset)
-            self.copy_menu.exec_(self.mapToGlobal(pos))
-
     def contextMenuEvent(self, event):
-        process = self._processAt(event.pos().x())
+        row = self.columnAt(event.pos().x())
         dataset = self._datasetAt(event.pos().y())
-        if (
-            process is not None
-            and dataset is not None
-            and _ProcessManager().met(process=process, dataset=dataset)
-        ):
-            self._target = (process, dataset)
-            self.menu_dataset_vs_process.exec_(event.globalPos())
+        if row == 0:
+            # handle column column
+            self._target = (None, dataset)
+            self.copy_menu.exec_(event.globalPos())
         else:
-            self._target = (None, None)
+            # handle processes column
+            process = self._processAt(event.pos().x())
+            if (
+                process is not None
+                and dataset is not None
+                and _ProcessManager().met(process=process, dataset=dataset)
+            ):
+                self._target = (process, dataset)
+                self.menu_dataset_vs_process.exec_(event.globalPos())
+            else:
+                self._target = (None, None)
         super().contextMenuEvent(event)
 
     def _requestReprocessing(self, *args, **kwargs):
         process, dataset = self._target
         if process is not None and dataset is not None:
             assert isinstance(process, SuperviseProcess)
             assert isinstance(dataset, DatasetIdentifier)
@@ -156,76 +159,89 @@
             extra_info = "{} processing {}".format(process.name, dataset)
             msg.setWindowTitle(extra_info)
             msg.setWindowModality(qt.Qt.NonModal)
             msg.show()
 
 
 class ProcessManagerWidget(qt.QWidget):
+    """
+    Main widget to dispaly dataset vs process metadata
+    """
+
     def __init__(self, parent):
         qt.QWidget.__init__(self, parent)
         self.setLayout(qt.QVBoxLayout())
 
         self._manager = ProcessManager()
 
-        self.filterWidget = _ToggleableFilterWidget(parent=self)
-        self.layout().setContentsMargins(4, 4, 4, 4)
-        self.layout().setSpacing(4)
-        self.filterWidget.layout().setSpacing(4)
-        self.layout().addWidget(self.filterWidget)
+        self._optionsWidget = _ToggleableOptionsWidget(parent=self)
+        self._optionsWidget.setSizePolicy(
+            qt.QSizePolicy.Minimum, qt.QSizePolicy.Minimum
+        )
+        self.setContentsMargins(0, 0, 0, 0)
+        self.layout().setContentsMargins(0, 0, 0, 0)
+        self.layout().setSpacing(2)
+        self.layout().addWidget(self._optionsWidget)
 
         self.observationTable = ObservationTable(self)
+
         self.layout().addWidget(self.observationTable)
         self.observationTable.setModel(
             _DatasetProcessModel(parent=self.observationTable, header=tuple())
         )
         self.observationTable.resizeColumnsToContents()
         self.observationTable.setSortingEnabled(True)
         self.setSizePolicy(qt.QSizePolicy.Expanding, qt.QSizePolicy.Expanding)
 
         # connect signal / slot
         self._manager.sigUpdated.connect(self._updateDatasetStates)
         self._manager.sigNewProcessRegistered.connect(self._updateProcesses)
-        self.filterWidget.filterWidget.sigDatasetPatternEditingFinished.connect(
+        self._optionsWidget.filterWidget.sigDatasetPatternEditingFinished.connect(
             self._filterUpdated
         )
-        self.filterWidget.filterWidget.sigProcessPatternEditingFinished.connect(
+        self._optionsWidget.filterWidget.sigProcessPatternEditingFinished.connect(
             self._filterUpdated
         )
         self._manager.sigProcessUnregistered.connect(self._updateProcesses)
+        self._optionsWidget._orderingWidget.sigSortTypeChanged.connect(
+            self.observationTable.model()._setSorting
+        )
         # update to fit existing processes / datasets
         self._updateProcesses()
         self._updateDatasetStates()
 
     def _updateDatasetStates(self):
         self.observationTable.model().setDatasets(self._manager.get_datasets())
 
     def _updateProcesses(self):
         self.observationTable.model().setProcesses(self._manager.get_processes())
 
     def _filterUpdated(self):
         self.observationTable.model().process_patterns = (
-            self.filterWidget.getProcessPatterns()
+            self._optionsWidget.getProcessPatterns()
         )
         self._updateProcesses()
         self.observationTable.model().dataset_patterns = (
-            self.filterWidget.getDatasetPatterns()
+            self._optionsWidget.getDatasetPatterns()
         )
         self._updateDatasetStates()
 
 
 class _DatasetProcessModel(qt.QAbstractTableModel):
     def __init__(self, parent, header, *args):
         qt.QAbstractTableModel.__init__(self, parent, *args)
         self.header = header
         self._processes = OrderedDict()
-        self._datasets = OrderedDict()
+        self._sorted_datasets = OrderedDict()
+        self._unsorted_datasets = OrderedDict()
         self._processPatterns = tuple()
         # is there some process name pattern to follow ?
         self._datasetPatterns = tuple()
         # is there some dataset id pattern to follow ?
+        self._sort_type = SortType.FIRST_APPEARANCE
 
     def _match_dataset_patterns(self, dataset):
         if len(self._datasetPatterns) == 0:
             return True
         for pattern in self._datasetPatterns:
             if fnmatch.fnmatch(str(dataset), pattern):
                 return True
@@ -271,58 +287,103 @@
         self.endResetModel()
 
     def clear(self):
         self._processes = OrderedDict()
         self.endResetModel()
 
     def rowCount(self, parent=None):
-        return len(self._datasets)
+        return len(self._unsorted_datasets)
 
     def columnCount(self, parent=None):
-        return len(self._processes)
+        return len(self._processes) + 1
 
     def setProcesses(self, processes):
         assert isinstance(processes, (tuple, list))
         self._processes = {}
         processes = list(filter(self._match_process_patterns, processes))
         for i_process, process in enumerate(processes):
             self._processes[i_process] = process
         self.endResetModel()
 
+    @staticmethod
+    def sort_datasets(datasets: list, sort_type):
+        if sort_type is SortType.FIRST_APPEARANCE:
+            pass
+        elif sort_type is SortType.LAST_APPEARANCE:
+            datasets.reverse()
+        elif sort_type in (SortType.ALPHABETICAL, SortType.REVERSE_ALPHABETICAL):
+            datasets = sorted(
+                datasets,
+                key=lambda x: x.name() or "",
+                reverse=sort_type is SortType.REVERSE_ALPHABETICAL,
+            )
+        elif sort_type in (SortType.CREATION_TIME, SortType.REVERSE_CREATION_TIME):
+            datasets = sorted(
+                datasets,
+                key=lambda x: x.creation_time() or datetime.datetime.fromtimestamp(0),
+                reverse=sort_type is SortType.REVERSE_CREATION_TIME,
+            )
+        elif sort_type in (
+            SortType.MODIFICATION_TIME,
+            SortType.REVERSE_MODIFICATION_TIME,
+        ):
+            datasets = sorted(
+                datasets,
+                key=lambda x: x.modification_time()
+                or datetime.datetime.fromtimestamp(0),
+                reverse=sort_type is SortType.REVERSE_MODIFICATION_TIME,
+            )
+        else:
+            raise ValueError("sort type not handled")
+        return datasets
+
     def setDatasets(self, datasets):
         assert isinstance(datasets, (tuple, list))
-        self._datasets = {}
+        self._unsorted_datasets = datasets
+        # filter datasets
         datasets = list(filter(self._match_dataset_patterns, datasets))
+        # sort datasets
+        datasets = self.sort_datasets(datasets=datasets, sort_type=self._sort_type)
+
         for i_dataset, dataset in enumerate(datasets):
-            self._datasets[i_dataset] = dataset
+            self._sorted_datasets[i_dataset] = dataset
         self.endResetModel()
 
     def headerData(self, col, orientation, role):
         if orientation == qt.Qt.Horizontal and role == qt.Qt.DisplayRole:
-            if col < len(self._processes):
-                return self._processes[col].name
-        elif orientation == qt.Qt.Vertical:
-            if col < len(self._datasets):
-                if role == qt.Qt.DisplayRole:
-                    return self._datasets[col].short_description() or str(
-                        self._datasets[col]
-                    )
-                elif role == qt.Qt.ToolTipRole:
-                    return self._datasets[col].long_description()
+            if col == 0:
+                return
+            else:
+                process_idx = col - 1
+            if process_idx < len(self._processes):
+                return self._processes[process_idx].name
         return None
 
     def data(self, index, role):
         if index.isValid() is False:
             return None
 
         if role not in (qt.Qt.DisplayRole, qt.Qt.ToolTipRole, qt.Qt.BackgroundRole):
             return None
 
-        dataset_short_name = self._datasets[index.row()]
-        process_name = self._processes[index.column()]
+        if index.column() == 0:
+            # if dataset name
+            if role == qt.Qt.DisplayRole:
+                return self._sorted_datasets[index.row()].short_description() or str(
+                    self._sorted_datasets[index.row()]
+                )
+            elif role == qt.Qt.ToolTipRole:
+                return self._sorted_datasets[index.row()].long_description()
+            elif role == qt.Qt.BackgroundRole:
+                return qt.QColor("#dedede")
+            else:
+                return
+
+        dataset_short_name = self._sorted_datasets[index.row()]
+        process_name = self._processes[index.column() - 1]
         dataset_process_state = ProcessManager().get_dataset_state(
             dataset=dataset_short_name, process=process_name
         )
         dataset_process_details = ProcessManager().get_dataset_details(
             dataset=dataset_short_name, process=process_name
         )
         if role == qt.Qt.BackgroundRole:
@@ -338,26 +399,44 @@
                 return dataset_process_state.value
         if role == qt.Qt.ToolTipRole:
             if dataset_process_details is None:
                 return ""
             else:
                 return dataset_process_details
 
+    def _setSorting(self, sort_type: SortType):
+        sort_type = SortType.from_value(sort_type)
+        changed = self._sort_type is not sort_type
+        if changed:
+            self._sort_type = sort_type
+            self.setDatasets(datasets=self._unsorted_datasets)
+            self.layoutChanged.emit()
 
-class _ToggleableFilterWidget(qt.QWidget):
 
+class _ToggleableOptionsWidget(qt.QWidget):
     _BUTTON_ICON = qt.QStyle.SP_ToolBarVerticalExtensionButton  # noqa
 
     def __init__(self, parent):
-        qt.QWidget.__init__(self, parent)
+        super().__init__(parent)
         self.setLayout(qt.QGridLayout())
+        # toggable button
         self._toggleButton = qt.QPushButton("", self)
         self.layout().addWidget(self._toggleButton, 0, 0, 1, 1)
+
+        # dataset ordering
+        self._orderingWidget = _OrderingWidget(parent=self)
+        self.layout().setContentsMargins(2, 2, 2, 2)
+        self.layout().setSpacing(0)
+        self.layout().addWidget(self._orderingWidget, 2, 1, 3, 3)
+
+        # filtering
         self._filterWidget = _FilterWidget(parent=self)
-        self.layout().addWidget(self._filterWidget, 0, 1, 4, 4)
+        self.layout().setContentsMargins(2, 2, 2, 2)
+        self.layout().setSpacing(0)
+        self.layout().addWidget(self._filterWidget, 4, 1, 3, 3)
 
         self._toggleButton.setSizePolicy(qt.QSizePolicy.Fixed, qt.QSizePolicy.Fixed)
         self._setButtonIcon(show=True)
 
         # connect signal / slot
         self._toggleButton.clicked.connect(self._toggleFilterWidget)
 
@@ -378,30 +457,33 @@
             icon = qt.QIcon(pixmap)
         self._toggleButton.setIcon(icon)
 
     def _toggleFilterWidget(self):
         visible = not self._filterWidget.isVisible()
         self._setButtonIcon(show=visible)
         self._filterWidget.setVisible(visible)
+        self._orderingWidget.setVisible(visible)
 
 
 class _FilterWidget(qt.QWidget):
     """
     Widget to define some filtering pattern on dataset and / or processes
     """
 
     sigProcessPatternEditingFinished = qt.Signal()
     """signal emit when the process pattern editing finished"""
 
     sigDatasetPatternEditingFinished = qt.Signal()
     """signal emit when the dataset pattern editing finished"""
 
-    def __init__(self, parent=None, name="filter", font_size=12, icon_size=20):
+    def __init__(self, parent=None, name=" filter", font_size=12, icon_size=20):
         qt.QWidget.__init__(self, parent)
         self.setLayout(qt.QGridLayout())
+        self.layout().setSpacing(2)
+        self.layout().setContentsMargins(0, 0, 0, 0)
 
         font = self.font()
         font.setPixelSize(font_size)
         self.setFont(font)
 
         icon = icons.getQIcon("magnifying_glass")
         self._researchLabelIcon = qt.QLabel("", parent=self)
@@ -476,14 +558,48 @@
     def _datasetPatternEditingFinished(self, *args, **kwargs):
         self.sigDatasetPatternEditingFinished.emit()
 
     def _processPatternEditingFinished(self, *args, **kwargs):
         self.sigProcessPatternEditingFinished.emit()
 
 
+class _OrderingWidget(qt.QWidget):
+    """Widget to let the user define the ordering of datasets"""
+
+    sigSortTypeChanged = qt.Signal(str)
+    """emit when sort type changed. Paramater is the name of the new sorting type"""
+
+    def __init__(self, parent=None, *args, **kwargs) -> None:
+        super().__init__(parent, *args, **kwargs)
+        self.setLayout(qt.QFormLayout())
+        self._sortingTypeCB = qt.QComboBox(self)
+        for sort_type in SortType.members():
+            self._sortingTypeCB.addItem(sort_type.value)
+            self._sortingTypeCB.setItemData(
+                self._sortingTypeCB.findText(sort_type.value),
+                tooltips[sort_type],
+                qt.Qt.ToolTipRole,
+            )
+        self.layout().addRow("sorting", self._sortingTypeCB)
+
+        # set up
+        self._sortingTypeCB.setCurrentIndex(
+            self._sortingTypeCB.findText(SortType.FIRST_APPEARANCE.value)
+        )
+
+        # connect signal / slot
+        self._sortingTypeCB.currentIndexChanged.connect(self._changed)
+
+    def _changed(self, *args, **kwargs):
+        self.sigSortTypeChanged.emit(self.getCurrentSort().value)
+
+    def getCurrentSort(self) -> SortType:
+        return SortType.from_value(self._sortingTypeCB.currentText())
+
+
 class ProcessManager(qt.QObject):
     sigUpdated = qt.Signal()
     """Signal emitted when the state of some process / dataset is updated
     """
 
     sigNewProcessRegistered = qt.Signal()
     """Signal emitted when a new process is registered"""
```

### Comparing `processview-1.1.0/processview/gui/test/__init__.py` & `processview-1.2.0/processview/gui/test/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.1.0/processview/gui/test/test_process_manager.py` & `processview-1.2.0/processview/gui/test/test_process_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,30 +79,32 @@
         super().__init__()
         self.name = name
 
     def __str__(self) -> str:
         return self.name
 
     def get_identifier(self) -> DatasetIdentifier:
-        return _DummyIdentifier(self)
+        return _DummyIdentifier(
+            self,
+            metadata={
+                "name": self.name,
+                "modification_time": None,
+            },
+        )
 
 
 class _DummyIdentifier(DatasetIdentifier):
-    def __init__(self, dataset):
-        super().__init__(dataset)
-        self.name = dataset.name
-
     def __str__(self):
-        return self.name
+        return self.name()
 
     def __eq__(self, other):
-        return self.name == other.name
+        return self.name() == other.name()
 
     def __hash__(self):
-        return hash(self.name)
+        return hash(self.name())
 
 
 def suite():
     test_suite = unittest.TestSuite()
     for ui in (TestProcessManager,):
         test_suite.addTest(unittest.defaultTestLoader.loadTestsFromTestCase(ui))
     return test_suite
```

### Comparing `processview-1.1.0/processview/resources/__init__.py` & `processview-1.2.0/processview/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.1.0/processview/resources/gui/icons/advancement.png` & `processview-1.2.0/processview/resources/gui/icons/advancement.png`

 * *Files identical despite different names*

### Comparing `processview-1.1.0/processview/resources/gui/icons/advancement.svg` & `processview-1.2.0/processview/resources/gui/icons/advancement.svg`

 * *Files identical despite different names*

### Comparing `processview-1.1.0/processview/resources/gui/icons/magnifying_glass.png` & `processview-1.2.0/processview/resources/gui/icons/magnifying_glass.png`

 * *Files identical despite different names*

### Comparing `processview-1.1.0/processview/resources/gui/icons/magnifying_glass.svg` & `processview-1.2.0/processview/resources/gui/icons/magnifying_glass.svg`

 * *Files identical despite different names*

### Comparing `processview-1.1.0/processview/setup.py` & `processview-1.2.0/processview/setup.py`

 * *Files identical despite different names*

### Comparing `processview-1.1.0/processview/test/__init__.py` & `processview-1.2.0/processview/test/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.1.0/processview/utils/__init__.py` & `processview-1.2.0/processview/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.1.0/processview/utils/singleton.py` & `processview-1.2.0/processview/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `processview-1.1.0/processview/version.py` & `processview-1.2.0/processview/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     "beta": 11,
     "gamma": 11,
     "rc": 12,
     "final": 15,
 }
 
 MAJOR = 1
-MINOR = 1
+MINOR = 2
 MICRO = 0
 RELEV = "final"  # <16
 SERIAL = 0  # <16
 
 date = __date__
 
 from collections import namedtuple
```

### Comparing `processview-1.1.0/processview.egg-info/SOURCES.txt` & `processview-1.2.0/processview.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 LICENSE
 README.md
+setup.cfg
 setup.py
 processview/__init__.py
 processview/setup.py
 processview/version.py
 processview.egg-info/PKG-INFO
 processview.egg-info/SOURCES.txt
 processview.egg-info/dependency_links.txt
-processview.egg-info/not-zip-safe
 processview.egg-info/requires.txt
 processview.egg-info/top_level.txt
+processview.egg-info/zip-safe
 processview/core/__init__.py
 processview/core/dataset.py
 processview/core/helpers.py
 processview/core/setup.py
+processview/core/sorting.py
 processview/core/superviseprocess.py
 processview/core/manager/__init__.py
 processview/core/manager/manager.py
 processview/core/manager/test/__init__.py
 processview/core/manager/test/test_manager.py
 processview/core/test/__init__.py
 processview/gui/__init__.py
```

