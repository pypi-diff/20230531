# Comparing `tmp/HierarchiaPy-0.2.5.tar.gz` & `tmp/HierarchiaPy-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/HierarchiaPy-0.2.5.tar", last modified: Thu Jul  7 13:33:12 2022, max compression
+gzip compressed data, was "HierarchiaPy-0.2.6.tar", last modified: Wed May 31 11:44:47 2023, max compression
```

## Comparing `HierarchiaPy-0.2.5.tar` & `HierarchiaPy-0.2.6.tar`

### file list

```diff
@@ -1,63 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 13:33:12.000000 HierarchiaPy-0.2.5/
--rw-r--r--   0 root         (0) root         (0)      327 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/.codecov.yml
--rw-r--r--   0 root         (0) root         (0)     1799 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/.gitignore
--rw-r--r--   0 root         (0) root         (0)      609 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/.readthedocs.yml
--rw-r--r--   0 root         (0) root         (0)      273 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/.travis.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 13:33:12.000000 HierarchiaPy-0.2.5/HierarchiaPy/
--rw-r--r--   0 root         (0) root         (0)     6915 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/HierarchiaPy/HierarchiaPy.py
--rw-r--r--   0 root         (0) root         (0)      151 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/HierarchiaPy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 13:33:12.000000 HierarchiaPy-0.2.5/HierarchiaPy/methods/
--rw-r--r--   0 root         (0) root         (0)     8419 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/HierarchiaPy/methods/_ISI98.py
--rw-r--r--   0 root         (0) root         (0)     6069 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/HierarchiaPy/methods/_adagio.py
--rw-r--r--   0 root         (0) root         (0)     2063 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/HierarchiaPy/methods/_average_dominance_index.py
--rw-r--r--   0 root         (0) root         (0)     4091 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/HierarchiaPy/methods/_davids_score.py
--rw-r--r--   0 root         (0) root         (0)     3771 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/HierarchiaPy/methods/_elo.py
--rw-r--r--   0 root         (0) root         (0)     4431 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/HierarchiaPy/methods/_randomized_elo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 13:33:12.000000 HierarchiaPy-0.2.5/HierarchiaPy/metrics/
--rw-r--r--   0 root         (0) root         (0)     1043 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/HierarchiaPy/metrics/_dci.py
--rw-r--r--   0 root         (0) root         (0)     7810 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/HierarchiaPy/metrics/_kendall_k.py
--rw-r--r--   0 root         (0) root         (0)     5483 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/HierarchiaPy/metrics/_landau_h.py
--rw-r--r--   0 root         (0) root         (0)     9546 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/HierarchiaPy/metrics/_steepness.py
--rw-r--r--   0 root         (0) root         (0)     5615 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/HierarchiaPy/metrics/ecdf_dict.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 13:33:12.000000 HierarchiaPy-0.2.5/HierarchiaPy/utilities/
--rw-r--r--   0 root         (0) root         (0)     2725 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/HierarchiaPy/utilities/_network_graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 13:33:12.000000 HierarchiaPy-0.2.5/HierarchiaPy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4782 2022-07-07 13:33:12.000000 HierarchiaPy-0.2.5/HierarchiaPy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1346 2022-07-07 13:33:12.000000 HierarchiaPy-0.2.5/HierarchiaPy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-07 13:33:12.000000 HierarchiaPy-0.2.5/HierarchiaPy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2022-07-07 13:33:12.000000 HierarchiaPy-0.2.5/HierarchiaPy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       78 2022-07-07 13:33:12.000000 HierarchiaPy-0.2.5/HierarchiaPy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1068 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4782 2022-07-07 13:33:12.000000 HierarchiaPy-0.2.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3820 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 13:33:12.000000 HierarchiaPy-0.2.5/docs/
--rw-r--r--   0 root         (0) root         (0)      638 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)      799 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 13:33:12.000000 HierarchiaPy-0.2.5/docs/pictures/
--rw-r--r--   0 root         (0) root         (0)    91240 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/docs/pictures/example_network_graph_2.png
--rw-r--r--   0 root         (0) root         (0)    14928 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/docs/pictures/logo.png
--rw-r--r--   0 root         (0) root         (0)       84 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 13:33:12.000000 HierarchiaPy-0.2.5/docs/source/
--rw-r--r--   0 root         (0) root         (0)      837 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/docs/source/conf.py
--rw-r--r--   0 root         (0) root         (0)     3920 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/docs/source/getting-started.rst
--rw-r--r--   0 root         (0) root         (0)      660 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/docs/source/index.rst
--rw-r--r--   0 root         (0) root         (0)     1400 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/docs/source/intro.rst
--rw-r--r--   0 root         (0) root         (0)     4714 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/docs/source/methods.rst
--rw-r--r--   0 root         (0) root         (0)     4748 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/docs/source/metrics.rst
--rw-r--r--   0 root         (0) root         (0)     2351 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/docs/source/utilities.rst
--rw-r--r--   0 root         (0) root         (0)       67 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       79 2022-07-07 13:33:12.000000 HierarchiaPy-0.2.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1885 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-07 13:33:12.000000 HierarchiaPy-0.2.5/tests/
--rw-r--r--   0 root         (0) root         (0)     1721 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/tests/ISI98_test.py
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2017 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/tests/adagio_test.py
--rw-r--r--   0 root         (0) root         (0)     1231 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/tests/average_dominance_index_test.py
--rw-r--r--   0 root         (0) root         (0)     2094 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/tests/class_test.py
--rw-r--r--   0 root         (0) root         (0)     2882 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/tests/davids_score_test.py
--rw-r--r--   0 root         (0) root         (0)      518 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/tests/dci_test.py
--rw-r--r--   0 root         (0) root         (0)     1383 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/tests/elo_test.py
--rw-r--r--   0 root         (0) root         (0)     1069 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/tests/randomized_elo_test.py
--rw-r--r--   0 root         (0) root         (0)     1458 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/tests/test_linearity.py
--rw-r--r--   0 root         (0) root         (0)      722 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/tests/test_network_vizualization.py
--rw-r--r--   0 root         (0) root         (0)     2078 2022-07-07 13:32:23.000000 HierarchiaPy-0.2.5/tests/test_steepness.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:44:47.241009 HierarchiaPy-0.2.6/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:44:47.236008 HierarchiaPy-0.2.6/HierarchiaPy/
+-rw-r--r--   0 root         (0) root         (0)     6915 2023-05-31 11:44:41.000000 HierarchiaPy-0.2.6/HierarchiaPy/HierarchiaPy.py
+-rw-r--r--   0 root         (0) root         (0)      151 2023-05-31 11:44:41.000000 HierarchiaPy-0.2.6/HierarchiaPy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:44:47.239009 HierarchiaPy-0.2.6/HierarchiaPy/methods/
+-rw-r--r--   0 root         (0) root         (0)     8419 2023-05-31 11:44:41.000000 HierarchiaPy-0.2.6/HierarchiaPy/methods/_ISI98.py
+-rw-r--r--   0 root         (0) root         (0)     6068 2023-05-31 11:44:41.000000 HierarchiaPy-0.2.6/HierarchiaPy/methods/_adagio.py
+-rw-r--r--   0 root         (0) root         (0)     2063 2023-05-31 11:44:41.000000 HierarchiaPy-0.2.6/HierarchiaPy/methods/_average_dominance_index.py
+-rw-r--r--   0 root         (0) root         (0)     4091 2023-05-31 11:44:41.000000 HierarchiaPy-0.2.6/HierarchiaPy/methods/_davids_score.py
+-rw-r--r--   0 root         (0) root         (0)     3771 2023-05-31 11:44:41.000000 HierarchiaPy-0.2.6/HierarchiaPy/methods/_elo.py
+-rw-r--r--   0 root         (0) root         (0)     4431 2023-05-31 11:44:41.000000 HierarchiaPy-0.2.6/HierarchiaPy/methods/_randomized_elo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:44:47.240008 HierarchiaPy-0.2.6/HierarchiaPy/metrics/
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-05-31 11:44:41.000000 HierarchiaPy-0.2.6/HierarchiaPy/metrics/_dci.py
+-rw-r--r--   0 root         (0) root         (0)     7810 2023-05-31 11:44:41.000000 HierarchiaPy-0.2.6/HierarchiaPy/metrics/_kendall_k.py
+-rw-r--r--   0 root         (0) root         (0)     5483 2023-05-31 11:44:41.000000 HierarchiaPy-0.2.6/HierarchiaPy/metrics/_landau_h.py
+-rw-r--r--   0 root         (0) root         (0)     9546 2023-05-31 11:44:41.000000 HierarchiaPy-0.2.6/HierarchiaPy/metrics/_steepness.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:44:47.240008 HierarchiaPy-0.2.6/HierarchiaPy/utilities/
+-rw-r--r--   0 root         (0) root         (0)     2725 2023-05-31 11:44:41.000000 HierarchiaPy-0.2.6/HierarchiaPy/utilities/_network_graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:44:47.237008 HierarchiaPy-0.2.6/HierarchiaPy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4800 2023-05-31 11:44:46.000000 HierarchiaPy-0.2.6/HierarchiaPy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      746 2023-05-31 11:44:47.000000 HierarchiaPy-0.2.6/HierarchiaPy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 11:44:46.000000 HierarchiaPy-0.2.6/HierarchiaPy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-31 11:44:46.000000 HierarchiaPy-0.2.6/HierarchiaPy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2023-05-31 11:44:46.000000 HierarchiaPy-0.2.6/HierarchiaPy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-05-31 11:44:41.000000 HierarchiaPy-0.2.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4800 2023-05-31 11:44:47.241009 HierarchiaPy-0.2.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3858 2023-05-31 11:44:41.000000 HierarchiaPy-0.2.6/README.md
+-rw-r--r--   0 root         (0) root         (0)       79 2023-05-31 11:44:47.241009 HierarchiaPy-0.2.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-05-31 11:44:41.000000 HierarchiaPy-0.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 11:44:47.240008 HierarchiaPy-0.2.6/tests/
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-05-31 11:44:41.000000 HierarchiaPy-0.2.6/tests/test_linearity.py
+-rw-r--r--   0 root         (0) root         (0)      722 2023-05-31 11:44:41.000000 HierarchiaPy-0.2.6/tests/test_network_vizualization.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-05-31 11:44:41.000000 HierarchiaPy-0.2.6/tests/test_steepness.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `HierarchiaPy-0.2.5/HierarchiaPy/HierarchiaPy.py` & `HierarchiaPy-0.2.6/HierarchiaPy/HierarchiaPy.py`

 * *Files identical despite different names*

### Comparing `HierarchiaPy-0.2.5/HierarchiaPy/methods/_ISI98.py` & `HierarchiaPy-0.2.6/HierarchiaPy/methods/_ISI98.py`

 * *Files identical despite different names*

### Comparing `HierarchiaPy-0.2.5/HierarchiaPy/methods/_adagio.py` & `HierarchiaPy-0.2.6/HierarchiaPy/methods/_adagio.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     
     # Preprocessing
     if preprocessing:
         mat = mat - np.transpose(mat)
         mat = np.where(mat < 0, 0, mat)
     
     # Network 
-    network_graph = nx.from_numpy_matrix(mat, create_using=nx.DiGraph(directed=True))
+    network_graph = nx.from_numpy_array(mat, create_using=nx.DiGraph(directed=True))
     
     # Plot network
     if plot_network:
         nx.draw_networkx(network_graph, arrows=True)
         plt.show()
     
     # Calculation of ranks
```

### Comparing `HierarchiaPy-0.2.5/HierarchiaPy/methods/_average_dominance_index.py` & `HierarchiaPy-0.2.6/HierarchiaPy/methods/_average_dominance_index.py`

 * *Files identical despite different names*

### Comparing `HierarchiaPy-0.2.5/HierarchiaPy/methods/_davids_score.py` & `HierarchiaPy-0.2.6/HierarchiaPy/methods/_davids_score.py`

 * *Files identical despite different names*

### Comparing `HierarchiaPy-0.2.5/HierarchiaPy/methods/_elo.py` & `HierarchiaPy-0.2.6/HierarchiaPy/methods/_elo.py`

 * *Files identical despite different names*

### Comparing `HierarchiaPy-0.2.5/HierarchiaPy/methods/_randomized_elo.py` & `HierarchiaPy-0.2.6/HierarchiaPy/methods/_randomized_elo.py`

 * *Files identical despite different names*

### Comparing `HierarchiaPy-0.2.5/HierarchiaPy/metrics/_dci.py` & `HierarchiaPy-0.2.6/HierarchiaPy/metrics/_dci.py`

 * *Files identical despite different names*

### Comparing `HierarchiaPy-0.2.5/HierarchiaPy/metrics/_kendall_k.py` & `HierarchiaPy-0.2.6/HierarchiaPy/metrics/_kendall_k.py`

 * *Files identical despite different names*

### Comparing `HierarchiaPy-0.2.5/HierarchiaPy/metrics/_landau_h.py` & `HierarchiaPy-0.2.6/HierarchiaPy/metrics/_landau_h.py`

 * *Files identical despite different names*

### Comparing `HierarchiaPy-0.2.5/HierarchiaPy/metrics/_steepness.py` & `HierarchiaPy-0.2.6/HierarchiaPy/metrics/_steepness.py`

 * *Files identical despite different names*

### Comparing `HierarchiaPy-0.2.5/HierarchiaPy/utilities/_network_graph.py` & `HierarchiaPy-0.2.6/HierarchiaPy/utilities/_network_graph.py`

 * *Files identical despite different names*

### Comparing `HierarchiaPy-0.2.5/HierarchiaPy.egg-info/PKG-INFO` & `HierarchiaPy-0.2.6/HierarchiaPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: HierarchiaPy
-Version: 0.2.5
+Version: 0.2.6
 Summary: HierarchiaPy: statistical package to derive hiearchy from social interactions
 Home-page: https://github.com/nusretipek/HierarchiaPy
+Download-URL: https://github.com/nusretipek/HierarchiaPy
 Author: Nusret Ipek
 Author-email: Nusret.Ipek@UGent.be
 License: MIT
-Download-URL: https://github.com/nusretipek/HierarchiaPy
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
@@ -116,9 +115,9 @@
 v 0.1.0 - Initial release <br>
 v 0.2.0 - Inclusion of linearity statistics & tests <br>
 v 0.2.1 - Hot-fix for linearity tests <br>
 v 0.2.2 - I&SI 98, performance improvement  <br>
 v 0.2.3 - Landau's h classic improvement  <br>
 v 0.2.4 - Steepness, DCI and network vizualization added <br>
 v 0.2.5 - Performance improvement and vectorization of several modules <br>
-
+v 0.2.6 - Dependency management <br>
```

### Comparing `HierarchiaPy-0.2.5/LICENSE` & `HierarchiaPy-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `HierarchiaPy-0.2.5/PKG-INFO` & `HierarchiaPy-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: HierarchiaPy
-Version: 0.2.5
+Version: 0.2.6
 Summary: HierarchiaPy: statistical package to derive hiearchy from social interactions
 Home-page: https://github.com/nusretipek/HierarchiaPy
+Download-URL: https://github.com/nusretipek/HierarchiaPy
 Author: Nusret Ipek
 Author-email: Nusret.Ipek@UGent.be
 License: MIT
-Download-URL: https://github.com/nusretipek/HierarchiaPy
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
@@ -116,9 +115,9 @@
 v 0.1.0 - Initial release <br>
 v 0.2.0 - Inclusion of linearity statistics & tests <br>
 v 0.2.1 - Hot-fix for linearity tests <br>
 v 0.2.2 - I&SI 98, performance improvement  <br>
 v 0.2.3 - Landau's h classic improvement  <br>
 v 0.2.4 - Steepness, DCI and network vizualization added <br>
 v 0.2.5 - Performance improvement and vectorization of several modules <br>
-
+v 0.2.6 - Dependency management <br>
```

### Comparing `HierarchiaPy-0.2.5/README.md` & `HierarchiaPy-0.2.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -91,7 +91,9 @@
 v 0.1.0 - Initial release <br>
 v 0.2.0 - Inclusion of linearity statistics & tests <br>
 v 0.2.1 - Hot-fix for linearity tests <br>
 v 0.2.2 - I&SI 98, performance improvement  <br>
 v 0.2.3 - Landau's h classic improvement  <br>
 v 0.2.4 - Steepness, DCI and network vizualization added <br>
 v 0.2.5 - Performance improvement and vectorization of several modules <br>
+v 0.2.6 - Dependency management <br>
+
```

### Comparing `HierarchiaPy-0.2.5/setup.py` & `HierarchiaPy-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     _has_setuptools = True
 except ImportError:
     from distutils.core import setup
     
 # Setup parameters
 
 DISTNAME = "HierarchiaPy"
-VERSION = "0.2.5"
+VERSION = "0.2.6"
 AUTHOR = "Nusret Ipek"
 AUTHOR_EMAIL ="Nusret.Ipek@UGent.be"
 
 DESC = "HierarchiaPy: statistical package to derive hiearchy from social interactions"
 with open("README.md", "r") as f:
     LONG_DESC = f.read()
 LONG_DESC_TYPE = "text/markdown"
```

### Comparing `HierarchiaPy-0.2.5/tests/test_linearity.py` & `HierarchiaPy-0.2.6/tests/test_linearity.py`

 * *Files identical despite different names*

### Comparing `HierarchiaPy-0.2.5/tests/test_network_vizualization.py` & `HierarchiaPy-0.2.6/tests/test_network_vizualization.py`

 * *Files identical despite different names*

### Comparing `HierarchiaPy-0.2.5/tests/test_steepness.py` & `HierarchiaPy-0.2.6/tests/test_steepness.py`

 * *Files identical despite different names*

