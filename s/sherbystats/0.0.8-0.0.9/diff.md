# Comparing `tmp/sherbystats-0.0.8.tar.gz` & `tmp/sherbystats-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherbystats-0.0.8.tar", last modified: Mon Apr 17 14:57:35 2023, max compression
+gzip compressed data, was "sherbystats-0.0.9.tar", last modified: Wed May 31 17:10:57 2023, max compression
```

## Comparing `sherbystats-0.0.8.tar` & `sherbystats-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ryangosselin   (501) staff       (20)        0 2023-04-17 14:57:35.055189 sherbystats-0.0.8/
--rw-r--r--   0 ryangosselin   (501) staff       (20)      508 2023-04-17 14:57:35.054962 sherbystats-0.0.8/PKG-INFO
--rw-r--r--   0 ryangosselin   (501) staff       (20)       38 2023-04-17 14:57:35.055290 sherbystats-0.0.8/setup.cfg
--rwxrwxrwx   0 ryangosselin   (501) staff       (20)      663 2023-04-17 14:57:11.000000 sherbystats-0.0.8/setup.py
-drwxr-xr-x   0 ryangosselin   (501) staff       (20)        0 2023-04-17 14:57:35.053338 sherbystats-0.0.8/sherbystats/
--rwxrwxrwx   0 ryangosselin   (501) staff       (20)      173 2023-04-14 13:30:30.000000 sherbystats-0.0.8/sherbystats/__init__.py
--rwxr-xr-x   0 ryangosselin   (501) staff       (20)     4755 2022-12-02 18:57:23.000000 sherbystats-0.0.8/sherbystats/anova.py
--rw-r--r--   0 ryangosselin   (501) staff       (20)    12256 2022-11-28 21:45:55.000000 sherbystats-0.0.8/sherbystats/doe.py
--rwxr-xr-x   0 ryangosselin   (501) staff       (20)      993 2022-11-28 21:46:07.000000 sherbystats-0.0.8/sherbystats/mlr.py
--rwxrwxrwx   0 ryangosselin   (501) staff       (20)     1846 2023-04-17 14:48:55.000000 sherbystats-0.0.8/sherbystats/normplot.py
--rwxrwxrwx   0 ryangosselin   (501) staff       (20)      700 2022-11-28 21:46:48.000000 sherbystats-0.0.8/sherbystats/xlsread.py
-drwxr-xr-x   0 ryangosselin   (501) staff       (20)        0 2023-04-17 14:57:35.054608 sherbystats-0.0.8/sherbystats.egg-info/
--rw-r--r--   0 ryangosselin   (501) staff       (20)      508 2023-04-17 14:57:34.000000 sherbystats-0.0.8/sherbystats.egg-info/PKG-INFO
--rw-r--r--   0 ryangosselin   (501) staff       (20)      278 2023-04-17 14:57:34.000000 sherbystats-0.0.8/sherbystats.egg-info/SOURCES.txt
--rw-r--r--   0 ryangosselin   (501) staff       (20)        1 2023-04-17 14:57:34.000000 sherbystats-0.0.8/sherbystats.egg-info/dependency_links.txt
--rw-r--r--   0 ryangosselin   (501) staff       (20)       12 2023-04-17 14:57:34.000000 sherbystats-0.0.8/sherbystats.egg-info/top_level.txt
+drwxr-xr-x   0 ryangosselin   (501) staff       (20)        0 2023-05-31 17:10:57.636484 sherbystats-0.0.9/
+-rw-r--r--   0 ryangosselin   (501) staff       (20)      508 2023-05-31 17:10:57.636203 sherbystats-0.0.9/PKG-INFO
+-rw-r--r--   0 ryangosselin   (501) staff       (20)       38 2023-05-31 17:10:57.636585 sherbystats-0.0.9/setup.cfg
+-rwxrwxrwx   0 ryangosselin   (501) staff       (20)      663 2023-05-31 17:05:51.000000 sherbystats-0.0.9/setup.py
+drwxr-xr-x   0 ryangosselin   (501) staff       (20)        0 2023-05-31 17:10:57.633974 sherbystats-0.0.9/sherbystats/
+-rwxrwxrwx   0 ryangosselin   (501) staff       (20)      173 2023-04-14 13:30:30.000000 sherbystats-0.0.9/sherbystats/__init__.py
+-rwxr-xr-x   0 ryangosselin   (501) staff       (20)     4561 2023-05-31 16:57:27.000000 sherbystats-0.0.9/sherbystats/anova.py
+-rw-r--r--   0 ryangosselin   (501) staff       (20)    12256 2022-11-28 21:45:55.000000 sherbystats-0.0.9/sherbystats/doe.py
+-rwxr-xr-x   0 ryangosselin   (501) staff       (20)      993 2022-11-28 21:46:07.000000 sherbystats-0.0.9/sherbystats/mlr.py
+-rwxrwxrwx   0 ryangosselin   (501) staff       (20)     1846 2023-04-17 14:48:55.000000 sherbystats-0.0.9/sherbystats/normplot.py
+-rwxrwxrwx   0 ryangosselin   (501) staff       (20)      700 2022-11-28 21:46:48.000000 sherbystats-0.0.9/sherbystats/xlsread.py
+drwxr-xr-x   0 ryangosselin   (501) staff       (20)        0 2023-05-31 17:10:57.635778 sherbystats-0.0.9/sherbystats.egg-info/
+-rw-r--r--   0 ryangosselin   (501) staff       (20)      508 2023-05-31 17:10:57.000000 sherbystats-0.0.9/sherbystats.egg-info/PKG-INFO
+-rw-r--r--   0 ryangosselin   (501) staff       (20)      278 2023-05-31 17:10:57.000000 sherbystats-0.0.9/sherbystats.egg-info/SOURCES.txt
+-rw-r--r--   0 ryangosselin   (501) staff       (20)        1 2023-05-31 17:10:57.000000 sherbystats-0.0.9/sherbystats.egg-info/dependency_links.txt
+-rw-r--r--   0 ryangosselin   (501) staff       (20)       12 2023-05-31 17:10:57.000000 sherbystats-0.0.9/sherbystats.egg-info/top_level.txt
```

### Comparing `sherbystats-0.0.8/setup.py` & `sherbystats-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name="sherbystats",
-    version="0.0.8",
+    version="0.0.9",
     author="Ryan Gosselin",
     author_email="ryan.gosselin@usherbrooke.ca",
     url="https://www.usherbrooke.ca/gchimiquebiotech/departement/professeurs/ryan-gosselin/",
     packages=["sherbystats"],
     description="Ryan @ UdeS",
     long_description="Python for GCB140 and GCH711:\
     \n\
```

### Comparing `sherbystats-0.0.8/sherbystats/anova.py` & `sherbystats-0.0.9/sherbystats/anova.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # ANOVA 
 # Ryan Gosselin
 # Version 2023
 
 import statsmodels.api as sm
 from statsmodels.formula.api import ols
 import numpy as np
+import pandas as pd
 
 
 
 def get_index_positions(list_of_elems, element):
     ''' Returns the indexes of all occurrences of give element in
     the list- listOfElements '''
     index_pos_list = []
@@ -128,21 +129,18 @@
     
     # Check for confounding
     # Summed within the table
     #SSsum = table['SS'].sum() 
     dfsum = table['df'].sum()
     
     
-    # Create a Python dictionary object with all the column values
-    d_row = {'SS':SST,'df':dfT,'MS':'-','F':'-','p':'-'}
+    # Include row for totals
+    d_row = [SST,dfT,'-','-','-']
+    table.loc[len(table)] = d_row
     
-    # Append the above Python dictionary object as a row to the existing pandas DataFrame
-    # Using the DataFrame.append() function
-    table = table.append(d_row,ignore_index=True)
-
     table.index = WORDS
     
     # Get rid of NaN
     table.at['Erreur', 'F'] = ('-')
     table.at['Erreur', 'p'] = ('-')
     
     freedom = dfsum > dfT
```

### Comparing `sherbystats-0.0.8/sherbystats/doe.py` & `sherbystats-0.0.9/sherbystats/doe.py`

 * *Files identical despite different names*

### Comparing `sherbystats-0.0.8/sherbystats/mlr.py` & `sherbystats-0.0.9/sherbystats/mlr.py`

 * *Files identical despite different names*

### Comparing `sherbystats-0.0.8/sherbystats/normplot.py` & `sherbystats-0.0.9/sherbystats/normplot.py`

 * *Files identical despite different names*

### Comparing `sherbystats-0.0.8/sherbystats/xlsread.py` & `sherbystats-0.0.9/sherbystats/xlsread.py`

 * *Files identical despite different names*

