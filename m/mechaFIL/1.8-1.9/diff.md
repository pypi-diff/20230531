# Comparing `tmp/mechaFIL-1.8.tar.gz` & `tmp/mechaFIL-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mechaFIL-1.8.tar", last modified: Tue Apr 18 13:38:50 2023, max compression
+gzip compressed data, was "mechaFIL-1.9.tar", last modified: Wed May 31 14:14:25 2023, max compression
```

## Comparing `mechaFIL-1.8.tar` & `mechaFIL-1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 kiran      (501) staff       (20)        0 2023-04-18 13:38:50.831648 mechaFIL-1.8/
--rw-r--r--   0 kiran      (501) staff       (20)     1069 2022-11-03 16:37:39.000000 mechaFIL-1.8/LICENSE
--rw-r--r--   0 kiran      (501) staff       (20)     6353 2023-04-18 13:38:50.831502 mechaFIL-1.8/PKG-INFO
--rw-r--r--   0 kiran      (501) staff       (20)     5747 2023-04-18 13:30:28.000000 mechaFIL-1.8/README.md
-drwxr-xr-x   0 kiran      (501) staff       (20)        0 2023-04-18 13:38:50.829161 mechaFIL-1.8/mechaFIL.egg-info/
--rw-r--r--   0 kiran      (501) staff       (20)     6353 2023-04-18 13:38:50.000000 mechaFIL-1.8/mechaFIL.egg-info/PKG-INFO
--rw-r--r--   0 kiran      (501) staff       (20)      409 2023-04-18 13:38:50.000000 mechaFIL-1.8/mechaFIL.egg-info/SOURCES.txt
--rw-r--r--   0 kiran      (501) staff       (20)        1 2023-04-18 13:38:50.000000 mechaFIL-1.8/mechaFIL.egg-info/dependency_links.txt
--rw-r--r--   0 kiran      (501) staff       (20)       39 2023-04-18 13:38:50.000000 mechaFIL-1.8/mechaFIL.egg-info/requires.txt
--rw-r--r--   0 kiran      (501) staff       (20)        9 2023-04-18 13:38:50.000000 mechaFIL-1.8/mechaFIL.egg-info/top_level.txt
-drwxr-xr-x   0 kiran      (501) staff       (20)        0 2023-04-18 13:38:50.831213 mechaFIL-1.8/mechafil/
--rw-r--r--   0 kiran      (501) staff       (20)      316 2023-04-18 13:30:28.000000 mechaFIL-1.8/mechafil/__init__.py
--rw-r--r--   0 kiran      (501) staff       (20)     9057 2023-04-18 13:30:31.000000 mechaFIL-1.8/mechafil/data.py
--rw-r--r--   0 kiran      (501) staff       (20)    13562 2023-04-18 13:30:31.000000 mechaFIL-1.8/mechafil/data_spacescope.py
--rw-r--r--   0 kiran      (501) staff       (20)     8476 2023-04-18 13:30:28.000000 mechaFIL-1.8/mechafil/data_starboard.py
--rw-r--r--   0 kiran      (501) staff       (20)     4547 2023-04-18 13:30:28.000000 mechaFIL-1.8/mechafil/locking.py
--rw-r--r--   0 kiran      (501) staff       (20)     3876 2022-12-21 17:17:26.000000 mechaFIL-1.8/mechafil/minting.py
--rw-r--r--   0 kiran      (501) staff       (20)    11608 2023-04-18 13:30:28.000000 mechaFIL-1.8/mechafil/power.py
--rw-r--r--   0 kiran      (501) staff       (20)     4264 2023-04-18 13:30:31.000000 mechaFIL-1.8/mechafil/sim.py
--rw-r--r--   0 kiran      (501) staff       (20)     6974 2023-04-18 13:30:31.000000 mechaFIL-1.8/mechafil/supply.py
--rw-r--r--   0 kiran      (501) staff       (20)      207 2023-04-18 13:30:28.000000 mechaFIL-1.8/mechafil/utils.py
--rw-r--r--   0 kiran      (501) staff       (20)     3013 2022-12-05 15:42:18.000000 mechaFIL-1.8/mechafil/vesting.py
--rw-r--r--   0 kiran      (501) staff       (20)       38 2023-04-18 13:38:50.831683 mechaFIL-1.8/setup.cfg
--rw-r--r--   0 kiran      (501) staff       (20)      905 2023-04-18 13:30:31.000000 mechaFIL-1.8/setup.py
+drwxr-xr-x   0 kiran      (501) staff       (20)        0 2023-05-31 14:14:25.798367 mechaFIL-1.9/
+-rw-r--r--   0 kiran      (501) staff       (20)     1069 2022-11-03 16:37:39.000000 mechaFIL-1.9/LICENSE
+-rw-r--r--   0 kiran      (501) staff       (20)     6353 2023-05-31 14:14:25.798207 mechaFIL-1.9/PKG-INFO
+-rw-r--r--   0 kiran      (501) staff       (20)     5747 2023-05-24 21:53:20.000000 mechaFIL-1.9/README.md
+drwxr-xr-x   0 kiran      (501) staff       (20)        0 2023-05-31 14:14:25.795487 mechaFIL-1.9/mechaFIL.egg-info/
+-rw-r--r--   0 kiran      (501) staff       (20)     6353 2023-05-31 14:14:25.000000 mechaFIL-1.9/mechaFIL.egg-info/PKG-INFO
+-rw-r--r--   0 kiran      (501) staff       (20)      409 2023-05-31 14:14:25.000000 mechaFIL-1.9/mechaFIL.egg-info/SOURCES.txt
+-rw-r--r--   0 kiran      (501) staff       (20)        1 2023-05-31 14:14:25.000000 mechaFIL-1.9/mechaFIL.egg-info/dependency_links.txt
+-rw-r--r--   0 kiran      (501) staff       (20)       39 2023-05-31 14:14:25.000000 mechaFIL-1.9/mechaFIL.egg-info/requires.txt
+-rw-r--r--   0 kiran      (501) staff       (20)        9 2023-05-31 14:14:25.000000 mechaFIL-1.9/mechaFIL.egg-info/top_level.txt
+drwxr-xr-x   0 kiran      (501) staff       (20)        0 2023-05-31 14:14:25.797886 mechaFIL-1.9/mechafil/
+-rw-r--r--   0 kiran      (501) staff       (20)      316 2023-05-24 21:53:20.000000 mechaFIL-1.9/mechafil/__init__.py
+-rw-r--r--   0 kiran      (501) staff       (20)     9057 2023-05-24 21:53:20.000000 mechaFIL-1.9/mechafil/data.py
+-rw-r--r--   0 kiran      (501) staff       (20)    13562 2023-05-24 21:53:20.000000 mechaFIL-1.9/mechafil/data_spacescope.py
+-rw-r--r--   0 kiran      (501) staff       (20)     8476 2023-05-24 21:53:20.000000 mechaFIL-1.9/mechafil/data_starboard.py
+-rw-r--r--   0 kiran      (501) staff       (20)     4547 2023-05-24 21:53:20.000000 mechaFIL-1.9/mechafil/locking.py
+-rw-r--r--   0 kiran      (501) staff       (20)     3882 2023-05-31 14:13:44.000000 mechaFIL-1.9/mechafil/minting.py
+-rw-r--r--   0 kiran      (501) staff       (20)    11608 2023-05-24 21:53:20.000000 mechaFIL-1.9/mechafil/power.py
+-rw-r--r--   0 kiran      (501) staff       (20)     4264 2023-05-24 21:53:20.000000 mechaFIL-1.9/mechafil/sim.py
+-rw-r--r--   0 kiran      (501) staff       (20)     6974 2023-05-24 21:53:20.000000 mechaFIL-1.9/mechafil/supply.py
+-rw-r--r--   0 kiran      (501) staff       (20)      207 2023-05-24 21:53:20.000000 mechaFIL-1.9/mechafil/utils.py
+-rw-r--r--   0 kiran      (501) staff       (20)     3013 2022-12-05 15:42:18.000000 mechaFIL-1.9/mechafil/vesting.py
+-rw-r--r--   0 kiran      (501) staff       (20)       38 2023-05-31 14:14:25.798407 mechaFIL-1.9/setup.cfg
+-rw-r--r--   0 kiran      (501) staff       (20)      905 2023-05-31 14:13:44.000000 mechaFIL-1.9/setup.py
```

### Comparing `mechaFIL-1.8/LICENSE` & `mechaFIL-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mechaFIL-1.8/PKG-INFO` & `mechaFIL-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mechaFIL
-Version: 1.8
+Version: 1.9
 Summary: Mechanistic model for the Filecoin Economy
 Author: Maria Silva, Tom Mellan, Kiran Karra
 Author-email: misilva73@gmail.com, t.mellan@imperial.ac.uk, kiran.karra@gmail.com
 Project-URL: Documentation, https://github.com/protocol/filecoin-mecha-twin
 Project-URL: Source, https://github.com/protocol/filecoin-mecha-twin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mechaFIL-1.8/README.md` & `mechaFIL-1.9/README.md`

 * *Files identical despite different names*

### Comparing `mechaFIL-1.8/mechaFIL.egg-info/PKG-INFO` & `mechaFIL-1.9/mechaFIL.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mechaFIL
-Version: 1.8
+Version: 1.9
 Summary: Mechanistic model for the Filecoin Economy
 Author: Maria Silva, Tom Mellan, Kiran Karra
 Author-email: misilva73@gmail.com, t.mellan@imperial.ac.uk, kiran.karra@gmail.com
 Project-URL: Documentation, https://github.com/protocol/filecoin-mecha-twin
 Project-URL: Source, https://github.com/protocol/filecoin-mecha-twin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mechaFIL-1.8/mechafil/data.py` & `mechaFIL-1.9/mechafil/data.py`

 * *Files identical despite different names*

### Comparing `mechaFIL-1.8/mechafil/data_spacescope.py` & `mechaFIL-1.9/mechafil/data_spacescope.py`

 * *Files identical despite different names*

### Comparing `mechaFIL-1.8/mechafil/data_starboard.py` & `mechaFIL-1.9/mechafil/data_starboard.py`

 * *Files identical despite different names*

### Comparing `mechaFIL-1.8/mechafil/locking.py` & `mechaFIL-1.9/mechafil/locking.py`

 * *Files identical despite different names*

### Comparing `mechaFIL-1.8/mechafil/minting.py` & `mechaFIL-1.9/mechafil/minting.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,21 +14,20 @@
 STORAGE_MINING = 0.55 * FIL_BASE
 SIMPLE_ALLOC = 0.3 * STORAGE_MINING  # total simple minting allocation
 BASELINE_ALLOC = 0.7 * STORAGE_MINING  # total baseline minting allocation
 GROWTH_RATE = float(
     np.log(2) / 365.0
 )  # daily baseline growth rate (the "g" from https://spec.filecoin.io/#section-systems.filecoin_token)
 BASELINE_STORAGE = (
-    2.88888888
+    2.766213637444971
     * EXBI
     # the b_0 from https://spec.filecoin.io/#section-systems.filecoin_token
 )
 # TODO: understand why the baseline value from startboard differs from the spec!
-# 3189227188947034973 from https://observable-api.starboard.ventures/api/v1/observable/network-storage-capacity/new_baseline_power
-
+# 3189227188947035000 from https://observable-api.starboard.ventures/api/v1/observable/network-storage-capacity/new_baseline_power
 
 def compute_minting_trajectory_df(
     start_date: datetime.date,
     end_date: datetime.date,
     rb_total_power_eib: np.array,
     qa_total_power_eib: np.array,
     qa_day_onboarded_power_pib: np.array,
```

### Comparing `mechaFIL-1.8/mechafil/power.py` & `mechaFIL-1.9/mechafil/power.py`

 * *Files identical despite different names*

### Comparing `mechaFIL-1.8/mechafil/sim.py` & `mechaFIL-1.9/mechafil/sim.py`

 * *Files identical despite different names*

### Comparing `mechaFIL-1.8/mechafil/supply.py` & `mechaFIL-1.9/mechafil/supply.py`

 * *Files identical despite different names*

### Comparing `mechaFIL-1.8/mechafil/vesting.py` & `mechaFIL-1.9/mechafil/vesting.py`

 * *Files identical despite different names*

### Comparing `mechaFIL-1.8/setup.py` & `mechaFIL-1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mechaFIL",
-    version="1.8",
+    version="1.9",
     author="Maria Silva, Tom Mellan, Kiran Karra",
     author_email="misilva73@gmail.com, t.mellan@imperial.ac.uk, kiran.karra@gmail.com",
     description="Mechanistic model for the Filecoin Economy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "Documentation": "https://github.com/protocol/filecoin-mecha-twin",
```

