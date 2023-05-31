# Comparing `tmp/sierras-0.2.1.tar.gz` & `tmp/sierras-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sierras-0.2.1.tar", last modified: Thu May 11 13:20:17 2023, max compression
+gzip compressed data, was "sierras-0.2.2.tar", last modified: Wed May 31 14:48:40 2023, max compression
```

## Comparing `sierras-0.2.1.tar` & `sierras-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:20:17.038415 sierras-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-11 13:19:57.000000 sierras-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-11 13:19:57.000000 sierras-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-11 13:20:17.038415 sierras-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-11 13:19:57.000000 sierras-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-11 13:19:57.000000 sierras-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 13:20:17.038415 sierras-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 13:20:17.038415 sierras-0.2.1/sierras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-11 13:20:17.000000 sierras-0.2.1/sierras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-11 13:20:17.000000 sierras-0.2.1/sierras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 13:20:17.000000 sierras-0.2.1/sierras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-11 13:20:17.000000 sierras-0.2.1/sierras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-11 13:20:17.000000 sierras-0.2.1/sierras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-05-11 13:19:57.000000 sierras-0.2.1/sierras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:40.436269 sierras-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-31 14:48:18.000000 sierras-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-31 14:48:18.000000 sierras-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-31 14:48:40.436269 sierras-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-31 14:48:18.000000 sierras-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-31 14:48:18.000000 sierras-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 14:48:40.436269 sierras-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:40.436269 sierras-0.2.2/sierras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-31 14:48:40.000000 sierras-0.2.2/sierras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-31 14:48:40.000000 sierras-0.2.2/sierras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:48:40.000000 sierras-0.2.2/sierras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-31 14:48:40.000000 sierras-0.2.2/sierras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 14:48:40.000000 sierras-0.2.2/sierras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-31 14:48:18.000000 sierras-0.2.2/sierras.py
```

### Comparing `sierras-0.2.1/LICENSE` & `sierras-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sierras-0.2.1/PKG-INFO` & `sierras-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sierras
-Version: 0.2.1
+Version: 0.2.2
 Summary: A tool for empirical Arrhenius equation fitting for thermally-induced physicochemical processes.
-Author-email: Francisco Fernandez <fernandezfrancisco2195@gmail.com>
+Author-email: Francisco Fernandez <ffernandev@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Francisco Fernandez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -40,18 +40,18 @@
 License-File: LICENSE
 
 # sierras
 
 [![Github Actions CI](https://github.com/fernandezfran/sierras/actions/workflows/sierras_ci.yml/badge.svg)](https://github.com/fernandezfran/sierras/actions/workflows/sierras_ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/sierras/badge/?version=latest)](https://sierras.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/sierras)](https://pypi.org/project/sierras/)
-[![python version](https://img.shields.io/badge/python-3.8%2B-77b7fe)](https://www.python.org/)
-[![mit license](https://img.shields.io/badge/License-MIT-fcf695)](https://github.com/fernandezfran/sierras/blob/main/LICENSE)
-[![diseno_sci_sfw](https://img.shields.io/badge/DiSoftCompCi-FAMAF-ffda00)](https://github.com/leliel12/diseno_sci_sfw)
+[![python version](https://img.shields.io/badge/python-3.8%2B-4584b6)](https://www.python.org/)
+[![mit license](https://img.shields.io/badge/License-MIT-ffde57)](https://github.com/fernandezfran/sierras/blob/main/LICENSE)
 [![downloads](https://static.pepy.tech/badge/sierras)](https://pepy.tech/project/sierras)
+[![diseno_sci_sfw](https://img.shields.io/badge/DiSoftCompCi-FAMAF-ffda00)](https://github.com/leliel12/diseno_sci_sfw)
 
 **sierras** is a tool for empirical Arrhenius equation fitting for 
 thermally-induced physicochemical processes.
 
 
 ## Requirements
 
@@ -94,10 +94,10 @@
 
 
 ## License
 
 [MIT License](https://github.com/fernandezfran/sierras/blob/master/LICENSE)
 
 
-### Contact info
+## Contact info
 
-<fernandezfrancisco2195@gmail.com>
+You can contact me at <ffernandev@gmail.com>
```

### Comparing `sierras-0.2.1/README.md` & `sierras-0.2.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # sierras
 
 [![Github Actions CI](https://github.com/fernandezfran/sierras/actions/workflows/sierras_ci.yml/badge.svg)](https://github.com/fernandezfran/sierras/actions/workflows/sierras_ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/sierras/badge/?version=latest)](https://sierras.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/sierras)](https://pypi.org/project/sierras/)
-[![python version](https://img.shields.io/badge/python-3.8%2B-77b7fe)](https://www.python.org/)
-[![mit license](https://img.shields.io/badge/License-MIT-fcf695)](https://github.com/fernandezfran/sierras/blob/main/LICENSE)
-[![diseno_sci_sfw](https://img.shields.io/badge/DiSoftCompCi-FAMAF-ffda00)](https://github.com/leliel12/diseno_sci_sfw)
+[![python version](https://img.shields.io/badge/python-3.8%2B-4584b6)](https://www.python.org/)
+[![mit license](https://img.shields.io/badge/License-MIT-ffde57)](https://github.com/fernandezfran/sierras/blob/main/LICENSE)
 [![downloads](https://static.pepy.tech/badge/sierras)](https://pepy.tech/project/sierras)
+[![diseno_sci_sfw](https://img.shields.io/badge/DiSoftCompCi-FAMAF-ffda00)](https://github.com/leliel12/diseno_sci_sfw)
 
 **sierras** is a tool for empirical Arrhenius equation fitting for 
 thermally-induced physicochemical processes.
 
 
 ## Requirements
 
@@ -53,10 +53,10 @@
 
 
 ## License
 
 [MIT License](https://github.com/fernandezfran/sierras/blob/master/LICENSE)
 
 
-### Contact info
+## Contact info
 
-<fernandezfrancisco2195@gmail.com>
+You can contact me at <ffernandev@gmail.com>
```

### Comparing `sierras-0.2.1/pyproject.toml` & `sierras-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sierras"
-version = "0.2.1"
-authors = [{name = "Francisco Fernandez", email = "fernandezfrancisco2195@gmail.com"}]
+version = "0.2.2"
+authors = [{name = "Francisco Fernandez", email = "ffernandev@gmail.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 description = "A tool for empirical Arrhenius equation fitting for thermally-induced physicochemical processes."
 keywords = [
     "arrhenius-process",
     "arrhenius-equation",
     "arrhenius-fitting",
```

### Comparing `sierras-0.2.1/sierras.egg-info/PKG-INFO` & `sierras-0.2.2/sierras.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: sierras
-Version: 0.2.1
+Version: 0.2.2
 Summary: A tool for empirical Arrhenius equation fitting for thermally-induced physicochemical processes.
-Author-email: Francisco Fernandez <fernandezfrancisco2195@gmail.com>
+Author-email: Francisco Fernandez <ffernandev@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Francisco Fernandez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -40,18 +40,18 @@
 License-File: LICENSE
 
 # sierras
 
 [![Github Actions CI](https://github.com/fernandezfran/sierras/actions/workflows/sierras_ci.yml/badge.svg)](https://github.com/fernandezfran/sierras/actions/workflows/sierras_ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/sierras/badge/?version=latest)](https://sierras.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/sierras)](https://pypi.org/project/sierras/)
-[![python version](https://img.shields.io/badge/python-3.8%2B-77b7fe)](https://www.python.org/)
-[![mit license](https://img.shields.io/badge/License-MIT-fcf695)](https://github.com/fernandezfran/sierras/blob/main/LICENSE)
-[![diseno_sci_sfw](https://img.shields.io/badge/DiSoftCompCi-FAMAF-ffda00)](https://github.com/leliel12/diseno_sci_sfw)
+[![python version](https://img.shields.io/badge/python-3.8%2B-4584b6)](https://www.python.org/)
+[![mit license](https://img.shields.io/badge/License-MIT-ffde57)](https://github.com/fernandezfran/sierras/blob/main/LICENSE)
 [![downloads](https://static.pepy.tech/badge/sierras)](https://pepy.tech/project/sierras)
+[![diseno_sci_sfw](https://img.shields.io/badge/DiSoftCompCi-FAMAF-ffda00)](https://github.com/leliel12/diseno_sci_sfw)
 
 **sierras** is a tool for empirical Arrhenius equation fitting for 
 thermally-induced physicochemical processes.
 
 
 ## Requirements
 
@@ -94,10 +94,10 @@
 
 
 ## License
 
 [MIT License](https://github.com/fernandezfran/sierras/blob/master/LICENSE)
 
 
-### Contact info
+## Contact info
 
-<fernandezfrancisco2195@gmail.com>
+You can contact me at <ffernandev@gmail.com>
```

### Comparing `sierras-0.2.1/sierras.py` & `sierras-0.2.2/sierras.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,16 +173,16 @@
         -------
         pandas.DataFrame
             A ``pandas.DataFrame`` with the data.
         """
         df = pd.DataFrame(
             {
                 "temperatures": X.ravel(),
-                "reaction_rate": y,
-                "reaction_rate_pred": self.predict(X),
+                "process": y,
+                "process_pred": self.predict(X),
             }
         )
 
         if sample_weight is not None:
             df["weights"] = sample_weight
 
         return df
```

