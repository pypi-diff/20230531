# Comparing `tmp/synctoolbox-1.3.0.tar.gz` & `tmp/synctoolbox-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/synctoolbox-1.3.0.tar", last modified: Wed Nov 16 12:43:46 2022, max compression
+gzip compressed data, was "dist/synctoolbox-1.3.1.tar", last modified: Wed May 31 13:36:14 2023, max compression
```

## Comparing `synctoolbox-1.3.0.tar` & `synctoolbox-1.3.1.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxrwxr-x   0 yiitozer  (1001) yiitozer  (1001)        0 2022-11-16 12:43:46.000000 synctoolbox-1.3.0/
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     1529 2021-10-12 15:07:17.000000 synctoolbox-1.3.0/LICENCE
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     8193 2022-11-16 12:43:46.000000 synctoolbox-1.3.0/PKG-INFO
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     7327 2021-10-20 08:41:59.000000 synctoolbox-1.3.0/README.md
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)       38 2022-11-16 12:43:46.000000 synctoolbox-1.3.0/setup.cfg
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     1781 2022-11-16 12:42:49.000000 synctoolbox-1.3.0/setup.py
-drwxrwxr-x   0 yiitozer  (1001) yiitozer  (1001)        0 2022-11-16 12:43:46.000000 synctoolbox-1.3.0/synctoolbox/
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)        0 2021-10-12 15:07:17.000000 synctoolbox-1.3.0/synctoolbox/__init__.py
-drwxrwxr-x   0 yiitozer  (1001) yiitozer  (1001)        0 2022-11-16 12:43:46.000000 synctoolbox-1.3.0/synctoolbox/dtw/
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)        0 2021-10-12 15:07:17.000000 synctoolbox-1.3.0/synctoolbox/dtw/__init__.py
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     5201 2022-07-25 15:24:31.000000 synctoolbox-1.3.0/synctoolbox/dtw/anchor.py
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     6187 2021-10-12 15:07:17.000000 synctoolbox-1.3.0/synctoolbox/dtw/core.py
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     3082 2022-11-16 12:42:49.000000 synctoolbox-1.3.0/synctoolbox/dtw/cost.py
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)    28654 2022-11-16 12:42:49.000000 synctoolbox-1.3.0/synctoolbox/dtw/mrmsdtw.py
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)    11536 2022-11-16 12:42:49.000000 synctoolbox-1.3.0/synctoolbox/dtw/utils.py
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     7039 2022-11-16 12:42:49.000000 synctoolbox-1.3.0/synctoolbox/dtw/visualization.py
-drwxrwxr-x   0 yiitozer  (1001) yiitozer  (1001)        0 2022-11-16 12:43:46.000000 synctoolbox-1.3.0/synctoolbox/feature/
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)        0 2021-10-12 15:07:17.000000 synctoolbox-1.3.0/synctoolbox/feature/__init__.py
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     7854 2021-10-12 15:07:17.000000 synctoolbox-1.3.0/synctoolbox/feature/chroma.py
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)    19931 2022-11-16 12:42:49.000000 synctoolbox-1.3.0/synctoolbox/feature/csv_tools.py
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     6396 2021-11-26 14:43:05.000000 synctoolbox-1.3.0/synctoolbox/feature/dlnco.py
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     3584 2021-10-20 08:41:56.000000 synctoolbox-1.3.0/synctoolbox/feature/filterbank.py
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     2363 2022-11-16 12:42:49.000000 synctoolbox-1.3.0/synctoolbox/feature/novelty.py
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     6574 2021-11-24 09:54:11.000000 synctoolbox-1.3.0/synctoolbox/feature/pitch.py
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)    13098 2021-11-24 09:54:22.000000 synctoolbox-1.3.0/synctoolbox/feature/pitch_onset.py
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     4788 2022-11-16 12:42:49.000000 synctoolbox-1.3.0/synctoolbox/feature/utils.py
-drwxrwxr-x   0 yiitozer  (1001) yiitozer  (1001)        0 2022-11-16 12:43:46.000000 synctoolbox-1.3.0/synctoolbox.egg-info/
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     8193 2022-11-16 12:43:46.000000 synctoolbox-1.3.0/synctoolbox.egg-info/PKG-INFO
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)      693 2022-11-16 12:43:46.000000 synctoolbox-1.3.0/synctoolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)        1 2022-11-16 12:43:46.000000 synctoolbox-1.3.0/synctoolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)      317 2022-11-16 12:43:46.000000 synctoolbox-1.3.0/synctoolbox.egg-info/requires.txt
--rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)       12 2022-11-16 12:43:46.000000 synctoolbox-1.3.0/synctoolbox.egg-info/top_level.txt
+drwxrwxr-x   0 yiitozer  (1001) yiitozer  (1001)        0 2023-05-31 13:36:14.000000 synctoolbox-1.3.1/
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     1529 2023-05-31 13:10:14.000000 synctoolbox-1.3.1/LICENCE
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     8175 2023-05-31 13:36:14.000000 synctoolbox-1.3.1/PKG-INFO
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     7309 2023-05-31 13:10:14.000000 synctoolbox-1.3.1/README.md
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)       38 2023-05-31 13:36:14.000000 synctoolbox-1.3.1/setup.cfg
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     1781 2023-05-31 13:36:00.000000 synctoolbox-1.3.1/setup.py
+drwxrwxr-x   0 yiitozer  (1001) yiitozer  (1001)        0 2023-05-31 13:36:14.000000 synctoolbox-1.3.1/synctoolbox/
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)        0 2023-05-31 13:10:14.000000 synctoolbox-1.3.1/synctoolbox/__init__.py
+drwxrwxr-x   0 yiitozer  (1001) yiitozer  (1001)        0 2023-05-31 13:36:14.000000 synctoolbox-1.3.1/synctoolbox/dtw/
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)        0 2023-05-31 13:10:14.000000 synctoolbox-1.3.1/synctoolbox/dtw/__init__.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     5201 2023-05-31 13:10:14.000000 synctoolbox-1.3.1/synctoolbox/dtw/anchor.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     6187 2023-05-31 13:10:14.000000 synctoolbox-1.3.1/synctoolbox/dtw/core.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     3037 2023-05-31 13:36:00.000000 synctoolbox-1.3.1/synctoolbox/dtw/cost.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)    28654 2023-05-31 13:10:14.000000 synctoolbox-1.3.1/synctoolbox/dtw/mrmsdtw.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)    11536 2023-05-31 13:10:14.000000 synctoolbox-1.3.1/synctoolbox/dtw/utils.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     7039 2023-05-31 13:10:14.000000 synctoolbox-1.3.1/synctoolbox/dtw/visualization.py
+drwxrwxr-x   0 yiitozer  (1001) yiitozer  (1001)        0 2023-05-31 13:36:14.000000 synctoolbox-1.3.1/synctoolbox/feature/
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)        0 2023-05-31 13:10:14.000000 synctoolbox-1.3.1/synctoolbox/feature/__init__.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     7854 2023-05-31 13:10:14.000000 synctoolbox-1.3.1/synctoolbox/feature/chroma.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)    19931 2023-05-31 13:10:14.000000 synctoolbox-1.3.1/synctoolbox/feature/csv_tools.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     6396 2023-05-31 13:10:14.000000 synctoolbox-1.3.1/synctoolbox/feature/dlnco.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     3584 2023-05-31 13:10:14.000000 synctoolbox-1.3.1/synctoolbox/feature/filterbank.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     2363 2023-05-31 13:10:14.000000 synctoolbox-1.3.1/synctoolbox/feature/novelty.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     6574 2023-05-31 13:10:14.000000 synctoolbox-1.3.1/synctoolbox/feature/pitch.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)    13098 2023-05-31 13:10:14.000000 synctoolbox-1.3.1/synctoolbox/feature/pitch_onset.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     4788 2023-05-31 13:10:14.000000 synctoolbox-1.3.1/synctoolbox/feature/utils.py
+drwxrwxr-x   0 yiitozer  (1001) yiitozer  (1001)        0 2023-05-31 13:36:14.000000 synctoolbox-1.3.1/synctoolbox.egg-info/
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     8175 2023-05-31 13:36:14.000000 synctoolbox-1.3.1/synctoolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)      734 2023-05-31 13:36:14.000000 synctoolbox-1.3.1/synctoolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)        1 2023-05-31 13:36:14.000000 synctoolbox-1.3.1/synctoolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)      317 2023-05-31 13:36:14.000000 synctoolbox-1.3.1/synctoolbox.egg-info/requires.txt
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)       12 2023-05-31 13:36:14.000000 synctoolbox-1.3.1/synctoolbox.egg-info/top_level.txt
+drwxrwxr-x   0 yiitozer  (1001) yiitozer  (1001)        0 2023-05-31 13:36:14.000000 synctoolbox-1.3.1/tests/
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     2461 2023-05-31 13:10:14.000000 synctoolbox-1.3.1/tests/test_dtw.py
+-rw-rw-r--   0 yiitozer  (1001) yiitozer  (1001)     6816 2023-05-31 13:36:00.000000 synctoolbox-1.3.1/tests/test_features.py
```

### Comparing `synctoolbox-1.3.0/LICENCE` & `synctoolbox-1.3.1/LICENCE`

 * *Files identical despite different names*

### Comparing `synctoolbox-1.3.0/PKG-INFO` & `synctoolbox-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synctoolbox
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python Package for Efficient, Robust, and Accurate Music Synchronization (SyncToolbox)
 Home-page: https://github.com/meinardmueller/synctoolbox
 Download-URL: https://github.com/meinardmueller/synctoolbox
 Author: Meinard Müller, Yigitcan Özer, Michael Krause, Thomas Prätzlich and Jonathan Driedger
 Author-email: meinard.mueller@audiolabs-erlangen.de
 License: MIT
 Keywords: audio music sound synchronization dtw mrmsdtw
@@ -29,16 +29,15 @@
 
 Using suitable feature representations and cost measures, the toolbox's core technology is based on dynamic time warping (DTW), which brings the feature sequences into temporal correspondence. To account for efficiency, robustness and, accuracy, our toolbox integrates and combines techniques such as [multiscale DTW (MsDTW)](https://www.audiolabs-erlangen.de/fau/professor/mueller/publications/2006_MuellerMattesKurth_MultiscaleAudioSynchronization_ISMIR.pdf), [memory-restricted MsDTW (MrMsDTW)](https://www.audiolabs-erlangen.de/fau/professor/mueller/publications/2016_PraetzlichDriedgerMueller_MrMsDTW_ICASSP.pdf), and [high-resolution music synchronization](https://www.audiolabs-erlangen.de/fau/professor/mueller/publications/2009_EwertMuellerGrosche_HighResAudioSync_ICASSP.pdf). 
 
 If you use the Sync Toolbox in your research, please consider the following references.
 
 ## References
 
-Meinard Müller, Yigitcan Özer, Michael Krause, Thomas Prätzlich, and Jonathan Driedger.
-and Frank Zalkow. [Sync Toolbox: A Python Package for Efficient, Robust, and Accurate Music Synchronization.](https://joss.theoj.org/papers/10.21105/joss.03434) Journal of Open Source Software (JOSS), 6(64), 2021.
+Meinard Müller, Yigitcan Özer, Michael Krause, Thomas Prätzlich, and Jonathan Driedger. [Sync Toolbox: A Python Package for Efficient, Robust, and Accurate Music Synchronization.](https://joss.theoj.org/papers/10.21105/joss.03434) Journal of Open Source Software (JOSS), 6(64), 2021.
 
 Meinard Müller, Henning Mattes, and Frank Kurth.
 [An Efficient Multiscale Approach to Audio Synchronization](https://www.audiolabs-erlangen.de/fau/professor/mueller/publications/2006_MuellerMattesKurth_MultiscaleAudioSynchronization_ISMIR.pdf).
 In Proceedings of the International Society for Music Information Retrieval Conference (ISMIR): 192–197, 2006.
 
 Sebastian Ewert, Meinard Müller, and Peter Grosche.
 [High Resolution Audio Synchronization Using Chroma Onset Features](https://www.audiolabs-erlangen.de/fau/professor/mueller/publications/2009_EwertMuellerGrosche_HighResAudioSync_ICASSP.pdf).
```

### Comparing `synctoolbox-1.3.0/README.md` & `synctoolbox-1.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 
 Using suitable feature representations and cost measures, the toolbox's core technology is based on dynamic time warping (DTW), which brings the feature sequences into temporal correspondence. To account for efficiency, robustness and, accuracy, our toolbox integrates and combines techniques such as [multiscale DTW (MsDTW)](https://www.audiolabs-erlangen.de/fau/professor/mueller/publications/2006_MuellerMattesKurth_MultiscaleAudioSynchronization_ISMIR.pdf), [memory-restricted MsDTW (MrMsDTW)](https://www.audiolabs-erlangen.de/fau/professor/mueller/publications/2016_PraetzlichDriedgerMueller_MrMsDTW_ICASSP.pdf), and [high-resolution music synchronization](https://www.audiolabs-erlangen.de/fau/professor/mueller/publications/2009_EwertMuellerGrosche_HighResAudioSync_ICASSP.pdf). 
 
 If you use the Sync Toolbox in your research, please consider the following references.
 
 ## References
 
-Meinard Müller, Yigitcan Özer, Michael Krause, Thomas Prätzlich, and Jonathan Driedger.
-and Frank Zalkow. [Sync Toolbox: A Python Package for Efficient, Robust, and Accurate Music Synchronization.](https://joss.theoj.org/papers/10.21105/joss.03434) Journal of Open Source Software (JOSS), 6(64), 2021.
+Meinard Müller, Yigitcan Özer, Michael Krause, Thomas Prätzlich, and Jonathan Driedger. [Sync Toolbox: A Python Package for Efficient, Robust, and Accurate Music Synchronization.](https://joss.theoj.org/papers/10.21105/joss.03434) Journal of Open Source Software (JOSS), 6(64), 2021.
 
 Meinard Müller, Henning Mattes, and Frank Kurth.
 [An Efficient Multiscale Approach to Audio Synchronization](https://www.audiolabs-erlangen.de/fau/professor/mueller/publications/2006_MuellerMattesKurth_MultiscaleAudioSynchronization_ISMIR.pdf).
 In Proceedings of the International Society for Music Information Retrieval Conference (ISMIR): 192–197, 2006.
 
 Sebastian Ewert, Meinard Müller, and Peter Grosche.
 [High Resolution Audio Synchronization Using Chroma Onset Features](https://www.audiolabs-erlangen.de/fau/professor/mueller/publications/2009_EwertMuellerGrosche_HighResAudioSync_ICASSP.pdf).
```

### Comparing `synctoolbox-1.3.0/setup.py` & `synctoolbox-1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r') as fdesc:
     long_description = fdesc.read()
 
 setup(
     name='synctoolbox',
-    version='1.3.0',
+    version='1.3.1',
     description='Python Package for Efficient, Robust, and Accurate Music Synchronization (SyncToolbox)',
     author='Meinard Müller, Yigitcan Özer, Michael Krause, Thomas Prätzlich and Jonathan Driedger',
     author_email='meinard.mueller@audiolabs-erlangen.de',
     url='https://github.com/meinardmueller/synctoolbox',
     download_url='https://github.com/meinardmueller/synctoolbox',
     packages=find_packages(),
     long_description=long_description,
```

### Comparing `synctoolbox-1.3.0/synctoolbox/dtw/anchor.py` & `synctoolbox-1.3.1/synctoolbox/dtw/anchor.py`

 * *Files identical despite different names*

### Comparing `synctoolbox-1.3.0/synctoolbox/dtw/core.py` & `synctoolbox-1.3.1/synctoolbox/dtw/core.py`

 * *Files identical despite different names*

### Comparing `synctoolbox-1.3.0/synctoolbox/dtw/cost.py` & `synctoolbox-1.3.1/synctoolbox/dtw/cost.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from numba import jit
 import numpy as np
+from sklearn.metrics.pairwise import euclidean_distances
 
 
 #@jit(nopython=True)
 def cosine_distance(f1, f2, cos_meas_max=2.0, cos_meas_min=1.0):
     """For all pairs of vectors f1' and f2' in f1 and f2, computes 1 - (f1.f2),
     where '.' is the dot product, and rescales the results to lie in the
     range [cos_meas_min, cos_meas_max].
     Corresponds to regular cosine distance if f1' and f2' are normalized and
     cos_meas_min==0.0 and cos_meas_max==1.0."""
     return (1 - f1.T @ f2) * (cos_meas_max - cos_meas_min) + cos_meas_min
 
 
-@jit(nopython=True)
+
+#@jit(nopython=True)
 def euclidean_distance(f1, f2, l2_meas_max=1.0, l2_meas_min=0.0):
     """Computes euclidean distances between the vectors in f1 and f2, and
     rescales the results to lie in the range [cos_meas_min, cos_meas_max]."""
-    S1 = np.zeros((f1.shape[1], f2.shape[1]))
-    for n in range(f2.shape[1]):
-        S1[:, n] = np.sqrt(np.sum((f1.T - f2[:, n]) ** 2, axis=1))
+
+    S1 = euclidean_distances(f1.T, f2.T)
 
     return S1 * (l2_meas_max - l2_meas_min) + l2_meas_min
 
 
 def compute_high_res_cost_matrix(f_chroma1: np.ndarray,
                                  f_chroma2: np.ndarray,
                                  f_onset1: np.ndarray,
```

### Comparing `synctoolbox-1.3.0/synctoolbox/dtw/mrmsdtw.py` & `synctoolbox-1.3.1/synctoolbox/dtw/mrmsdtw.py`

 * *Files identical despite different names*

### Comparing `synctoolbox-1.3.0/synctoolbox/dtw/utils.py` & `synctoolbox-1.3.1/synctoolbox/dtw/utils.py`

 * *Files identical despite different names*

### Comparing `synctoolbox-1.3.0/synctoolbox/dtw/visualization.py` & `synctoolbox-1.3.1/synctoolbox/dtw/visualization.py`

 * *Files identical despite different names*

### Comparing `synctoolbox-1.3.0/synctoolbox/feature/chroma.py` & `synctoolbox-1.3.1/synctoolbox/feature/chroma.py`

 * *Files identical despite different names*

### Comparing `synctoolbox-1.3.0/synctoolbox/feature/csv_tools.py` & `synctoolbox-1.3.1/synctoolbox/feature/csv_tools.py`

 * *Files identical despite different names*

### Comparing `synctoolbox-1.3.0/synctoolbox/feature/dlnco.py` & `synctoolbox-1.3.1/synctoolbox/feature/dlnco.py`

 * *Files identical despite different names*

### Comparing `synctoolbox-1.3.0/synctoolbox/feature/filterbank.py` & `synctoolbox-1.3.1/synctoolbox/feature/filterbank.py`

 * *Files identical despite different names*

### Comparing `synctoolbox-1.3.0/synctoolbox/feature/novelty.py` & `synctoolbox-1.3.1/synctoolbox/feature/novelty.py`

 * *Files identical despite different names*

### Comparing `synctoolbox-1.3.0/synctoolbox/feature/pitch.py` & `synctoolbox-1.3.1/synctoolbox/feature/pitch.py`

 * *Files identical despite different names*

### Comparing `synctoolbox-1.3.0/synctoolbox/feature/pitch_onset.py` & `synctoolbox-1.3.1/synctoolbox/feature/pitch_onset.py`

 * *Files identical despite different names*

### Comparing `synctoolbox-1.3.0/synctoolbox/feature/utils.py` & `synctoolbox-1.3.1/synctoolbox/feature/utils.py`

 * *Files identical despite different names*

### Comparing `synctoolbox-1.3.0/synctoolbox.egg-info/PKG-INFO` & `synctoolbox-1.3.1/synctoolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synctoolbox
-Version: 1.3.0
+Version: 1.3.1
 Summary: Python Package for Efficient, Robust, and Accurate Music Synchronization (SyncToolbox)
 Home-page: https://github.com/meinardmueller/synctoolbox
 Download-URL: https://github.com/meinardmueller/synctoolbox
 Author: Meinard Müller, Yigitcan Özer, Michael Krause, Thomas Prätzlich and Jonathan Driedger
 Author-email: meinard.mueller@audiolabs-erlangen.de
 License: MIT
 Keywords: audio music sound synchronization dtw mrmsdtw
@@ -29,16 +29,15 @@
 
 Using suitable feature representations and cost measures, the toolbox's core technology is based on dynamic time warping (DTW), which brings the feature sequences into temporal correspondence. To account for efficiency, robustness and, accuracy, our toolbox integrates and combines techniques such as [multiscale DTW (MsDTW)](https://www.audiolabs-erlangen.de/fau/professor/mueller/publications/2006_MuellerMattesKurth_MultiscaleAudioSynchronization_ISMIR.pdf), [memory-restricted MsDTW (MrMsDTW)](https://www.audiolabs-erlangen.de/fau/professor/mueller/publications/2016_PraetzlichDriedgerMueller_MrMsDTW_ICASSP.pdf), and [high-resolution music synchronization](https://www.audiolabs-erlangen.de/fau/professor/mueller/publications/2009_EwertMuellerGrosche_HighResAudioSync_ICASSP.pdf). 
 
 If you use the Sync Toolbox in your research, please consider the following references.
 
 ## References
 
-Meinard Müller, Yigitcan Özer, Michael Krause, Thomas Prätzlich, and Jonathan Driedger.
-and Frank Zalkow. [Sync Toolbox: A Python Package for Efficient, Robust, and Accurate Music Synchronization.](https://joss.theoj.org/papers/10.21105/joss.03434) Journal of Open Source Software (JOSS), 6(64), 2021.
+Meinard Müller, Yigitcan Özer, Michael Krause, Thomas Prätzlich, and Jonathan Driedger. [Sync Toolbox: A Python Package for Efficient, Robust, and Accurate Music Synchronization.](https://joss.theoj.org/papers/10.21105/joss.03434) Journal of Open Source Software (JOSS), 6(64), 2021.
 
 Meinard Müller, Henning Mattes, and Frank Kurth.
 [An Efficient Multiscale Approach to Audio Synchronization](https://www.audiolabs-erlangen.de/fau/professor/mueller/publications/2006_MuellerMattesKurth_MultiscaleAudioSynchronization_ISMIR.pdf).
 In Proceedings of the International Society for Music Information Retrieval Conference (ISMIR): 192–197, 2006.
 
 Sebastian Ewert, Meinard Müller, and Peter Grosche.
 [High Resolution Audio Synchronization Using Chroma Onset Features](https://www.audiolabs-erlangen.de/fau/professor/mueller/publications/2009_EwertMuellerGrosche_HighResAudioSync_ICASSP.pdf).
```

### Comparing `synctoolbox-1.3.0/synctoolbox.egg-info/SOURCES.txt` & `synctoolbox-1.3.1/synctoolbox.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -18,8 +18,10 @@
 synctoolbox/feature/chroma.py
 synctoolbox/feature/csv_tools.py
 synctoolbox/feature/dlnco.py
 synctoolbox/feature/filterbank.py
 synctoolbox/feature/novelty.py
 synctoolbox/feature/pitch.py
 synctoolbox/feature/pitch_onset.py
-synctoolbox/feature/utils.py
+synctoolbox/feature/utils.py
+tests/test_dtw.py
+tests/test_features.py
```

