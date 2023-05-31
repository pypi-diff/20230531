# Comparing `tmp/unravel-python-1.2.8.tar.gz` & `tmp/unravel-python-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unravel-python-1.2.8.tar", last modified: Tue May 23 14:46:37 2023, max compression
+gzip compressed data, was "unravel-python-1.2.9.tar", last modified: Wed May 31 09:21:56 2023, max compression
```

## Comparing `unravel-python-1.2.8.tar` & `unravel-python-1.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 14:46:37.590000 unravel-python-1.2.8/
--rw-rw-rw-   0        0        0    35823 2023-03-09 15:58:46.000000 unravel-python-1.2.8/LICENSE
--rw-rw-rw-   0        0        0     3950 2023-05-23 14:46:38.000000 unravel-python-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     3442 2023-04-28 07:26:38.000000 unravel-python-1.2.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-23 14:46:38.000000 unravel-python-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1146 2023-04-28 13:02:26.000000 unravel-python-1.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 14:46:37.590000 unravel-python-1.2.8/unravel/
--rw-rw-rw-   0        0        0      358 2023-05-23 14:46:26.000000 unravel-python-1.2.8/unravel/__init__.py
--rw-rw-rw-   0        0        0    50689 2023-05-23 14:32:28.000000 unravel-python-1.2.8/unravel/core.py
--rw-rw-rw-   0        0        0     4558 2023-05-03 18:24:34.000000 unravel-python-1.2.8/unravel/example.py
--rw-rw-rw-   0        0        0    14624 2023-04-24 14:10:10.000000 unravel-python-1.2.8/unravel/utils.py
--rw-rw-rw-   0        0        0    10275 2023-05-23 14:42:30.000000 unravel-python-1.2.8/unravel/viz.py
-drwxrwxrwx   0        0        0        0 2023-05-23 14:46:37.600000 unravel-python-1.2.8/unravel_python.egg-info/
--rw-rw-rw-   0        0        0     3950 2023-05-23 14:46:38.000000 unravel-python-1.2.8/unravel_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-05-23 14:46:38.000000 unravel-python-1.2.8/unravel_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 14:46:38.000000 unravel-python-1.2.8/unravel_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-23 14:46:38.000000 unravel-python-1.2.8/unravel_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-23 14:46:38.000000 unravel-python-1.2.8/unravel_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 09:21:56.070000 unravel-python-1.2.9/
+-rw-rw-rw-   0        0        0    35823 2023-03-09 15:58:46.000000 unravel-python-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0     3950 2023-05-31 09:21:58.000000 unravel-python-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3442 2023-04-28 07:26:38.000000 unravel-python-1.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-31 09:21:58.000000 unravel-python-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1146 2023-04-28 13:02:26.000000 unravel-python-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 09:21:56.080000 unravel-python-1.2.9/unravel/
+-rw-rw-rw-   0        0        0      358 2023-05-31 09:21:44.000000 unravel-python-1.2.9/unravel/__init__.py
+-rw-rw-rw-   0        0        0    51658 2023-05-31 09:20:30.000000 unravel-python-1.2.9/unravel/core.py
+-rw-rw-rw-   0        0        0     4558 2023-05-03 18:24:34.000000 unravel-python-1.2.9/unravel/example.py
+-rw-rw-rw-   0        0        0    14624 2023-04-24 14:10:10.000000 unravel-python-1.2.9/unravel/utils.py
+-rw-rw-rw-   0        0        0    10275 2023-05-23 14:42:30.000000 unravel-python-1.2.9/unravel/viz.py
+drwxrwxrwx   0        0        0        0 2023-05-31 09:21:56.090000 unravel-python-1.2.9/unravel_python.egg-info/
+-rw-rw-rw-   0        0        0     3950 2023-05-31 09:21:56.000000 unravel-python-1.2.9/unravel_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-05-31 09:21:56.000000 unravel-python-1.2.9/unravel_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 09:21:56.000000 unravel-python-1.2.9/unravel_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-31 09:21:56.000000 unravel-python-1.2.9/unravel_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-31 09:21:56.000000 unravel-python-1.2.9/unravel_python.egg-info/top_level.txt
```

### Comparing `unravel-python-1.2.8/LICENSE` & `unravel-python-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.8/PKG-INFO` & `unravel-python-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unravel-python
-Version: 1.2.8
+Version: 1.2.9
 Summary: Implementation of UNRAVEL
 Home-page: https://github.com/DelinteNicolas/UNRAVEL
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `unravel-python-1.2.8/README.md` & `unravel-python-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.8/setup.py` & `unravel-python-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.8/unravel/core.py` & `unravel-python-1.2.9/unravel/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,28 +289,30 @@
 
     if ang > 90 and not direction:
         ang = 180-ang
 
     return ang
 
 
-def relative_angular_weighting(vs, vList: list, nList: list):
+def relative_angular_weighting(vs, vList: list, nList: list, legacy: bool = False):
     '''
     Computes the relative contributions of the segments in vList to vs using
     relative angular weighting, which attributes less weight to fixel
     perpendicular to the streamline segment.
 
     Parameters
     ----------
     vs : 1-D array
         Segment vector
     vList : list
         List of the k vectors corresponding to each fiber population
     nList : list
         List of the null k vectors
+    legacy : bool
+        If True uses the definition of the UNRAVEL paper. Default is False.
 
     Returns
     -------
     ang_coef : list
         List of the k coefficients
 
     '''
@@ -334,37 +336,50 @@
     sum_diff = np.sum(angle_diffList)
 
     ang_coef = []
 
     for i, angle_diff in enumerate(angle_diffList):
         if nList[i]:
             ang_coef.append(0)
-        elif sum_diff == K*90:    # Else divides by 0
-            ang_coef.append(1/K)
+        elif legacy:
+            if sum_diff == K*90:    # Else divides by 0
+                ang_coef.append(1/K)
+            else:
+                coef = (min(90, sum_diff)-angle_diff)/(min(90, sum_diff)
+                                                       * (K-sum(nList))-sum_diff)
+                ang_coef.append(coef)
         else:
-            coef = (min(90, sum_diff)-angle_diff)/(min(90, sum_diff)
-                                                   * (K-sum(nList))-sum_diff)
+            lis = angle_diffList.copy()
+            lis.remove(angle_diff)
+            coef = np.prod(lis) * (90-angle_diff)/(90 * (K-sum(nList))-sum_diff)
             ang_coef.append(coef)
 
+    if not legacy:
+        ang_coef = np.array(ang_coef)
+        ang_coef = ang_coef/np.sum(ang_coef)
+        return list(ang_coef)
+
     return ang_coef
 
 
-def angular_weighting(vs, vList: list, nList: list):
+def angular_weighting(vs, vList: list, nList: list, legacy: bool = False):
     '''
     Computes the relative contributions of the segments in vList to vs using
     angular weighting.
 
     Parameters
     ----------
     vs : 1-D array
         Segment vector
     vList : list
         List of the k vectors corresponding to each fiber population
     nList : list
         List of the null k vectors
+    legacy : bool
+        If True uses the definition of the UNRAVEL paper. Default is False.
 
     Returns
     -------
     ang_coef : list
         List of the k coefficients
 
     '''
@@ -388,21 +403,32 @@
     sum_diff = np.sum(angle_diffList)
 
     ang_coef = []
 
     for i, angle_diff in enumerate(angle_diffList):
         if nList[i]:
             ang_coef.append(0)
-        elif sum_diff == K*90:    # Else divides by 0
-            ang_coef.append(1/K)
+        elif legacy:
+            if sum_diff == K*90:    # Else divides by 0
+                ang_coef.append(1/K)
+            else:
+                coef = 1-angle_diff/sum_diff
+                coef = coef/(K-1-sum(nList))
+                ang_coef.append(coef)
         else:
-            coef = 1-angle_diff/sum_diff
-            coef = coef/(K-1-sum(nList))
+            lis = angle_diffList.copy()
+            lis.remove(angle_diff)
+            coef = np.prod(lis)
             ang_coef.append(coef)
 
+    if not legacy:
+        ang_coef = np.array(ang_coef)
+        ang_coef = ang_coef/np.sum(ang_coef)
+        return list(ang_coef)
+
     return ang_coef
 
 
 def closest_fixel_only(vs, vList: list, nList: list):
     '''
     Computes the relative contributions of the segments in vList to vs using
     closest fixel only approach.
```

### Comparing `unravel-python-1.2.8/unravel/example.py` & `unravel-python-1.2.9/unravel/example.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.8/unravel/utils.py` & `unravel-python-1.2.9/unravel/utils.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.8/unravel/viz.py` & `unravel-python-1.2.9/unravel/viz.py`

 * *Files identical despite different names*

### Comparing `unravel-python-1.2.8/unravel_python.egg-info/PKG-INFO` & `unravel-python-1.2.9/unravel_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unravel-python
-Version: 1.2.8
+Version: 1.2.9
 Summary: Implementation of UNRAVEL
 Home-page: https://github.com/DelinteNicolas/UNRAVEL
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

