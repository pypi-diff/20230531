# Comparing `tmp/pyrepseq-1.0.tar.gz` & `tmp/pyrepseq-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrepseq-1.0.tar", last modified: Sat Dec 10 00:01:07 2022, max compression
+gzip compressed data, was "pyrepseq-1.1.tar", last modified: Wed May 31 19:16:26 2023, max compression
```

## Comparing `pyrepseq-1.0.tar` & `pyrepseq-1.1.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 00:01:07.297493 pyrepseq-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2022-12-10 00:00:56.000000 pyrepseq-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      942 2022-12-10 00:01:07.293493 pyrepseq-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2022-12-10 00:00:56.000000 pyrepseq-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 00:01:07.293493 pyrepseq-1.0/pyrepseq/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2022-12-10 00:00:56.000000 pyrepseq-1.0/pyrepseq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 00:01:07.293493 pyrepseq-1.0/pyrepseq/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2022-12-10 00:00:56.000000 pyrepseq-1.0/pyrepseq/data/pcdelta_pbmc_minervina.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14941 2022-12-10 00:00:56.000000 pyrepseq-1.0/pyrepseq/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2022-12-10 00:00:56.000000 pyrepseq-1.0/pyrepseq/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    16296 2022-12-10 00:00:56.000000 pyrepseq-1.0/pyrepseq/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2022-12-10 00:00:56.000000 pyrepseq-1.0/pyrepseq/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2022-12-10 00:00:56.000000 pyrepseq-1.0/pyrepseq/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-10 00:01:07.293493 pyrepseq-1.0/pyrepseq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      942 2022-12-10 00:01:07.000000 pyrepseq-1.0/pyrepseq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      342 2022-12-10 00:01:07.000000 pyrepseq-1.0/pyrepseq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-10 00:01:07.000000 pyrepseq-1.0/pyrepseq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-10 00:01:07.000000 pyrepseq-1.0/pyrepseq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-10 00:01:07.000000 pyrepseq-1.0/pyrepseq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-10 00:01:07.297493 pyrepseq-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      844 2022-12-10 00:00:56.000000 pyrepseq-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:16:26.855682 pyrepseq-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-31 19:16:15.000000 pyrepseq-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-31 19:16:26.855682 pyrepseq-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-31 19:16:15.000000 pyrepseq-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:16:26.855682 pyrepseq-1.1/pyrepseq/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-31 19:16:15.000000 pyrepseq-1.1/pyrepseq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:16:26.855682 pyrepseq-1.1/pyrepseq/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-31 19:16:15.000000 pyrepseq-1.1/pyrepseq/data/pcdelta_pbmc_minervina.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15614 2023-05-31 19:16:15.000000 pyrepseq-1.1/pyrepseq/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-31 19:16:15.000000 pyrepseq-1.1/pyrepseq/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16500 2023-05-31 19:16:15.000000 pyrepseq-1.1/pyrepseq/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-05-31 19:16:15.000000 pyrepseq-1.1/pyrepseq/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-31 19:16:15.000000 pyrepseq-1.1/pyrepseq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:16:26.855682 pyrepseq-1.1/pyrepseq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-31 19:16:26.000000 pyrepseq-1.1/pyrepseq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-31 19:16:26.000000 pyrepseq-1.1/pyrepseq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:16:26.000000 pyrepseq-1.1/pyrepseq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-31 19:16:26.000000 pyrepseq-1.1/pyrepseq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 19:16:26.000000 pyrepseq-1.1/pyrepseq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 19:16:26.855682 pyrepseq-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-31 19:16:15.000000 pyrepseq-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:16:26.855682 pyrepseq-1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-31 19:16:15.000000 pyrepseq-1.1/tests/test_coincidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-31 19:16:15.000000 pyrepseq-1.1/tests/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-31 19:16:15.000000 pyrepseq-1.1/tests/test_io.py
```

### Comparing `pyrepseq-1.0/LICENSE` & `pyrepseq-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrepseq-1.0/PKG-INFO` & `pyrepseq-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepseq
-Version: 1.0
+Version: 1.1
 Summary: Python library for immune repertoire analyses
 Home-page: http://pyrepseq.readthedocs.io/
 Download-URL: http://github.com/andim/pyrepseq
 Author: Andreas Mayer
 Author-email: andimscience@gmail.com
 Maintainer: Andreas Mayer
 Maintainer-email: andimscience@gmail.com
```

### Comparing `pyrepseq-1.0/README.md` & `pyrepseq-1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 [![License](https://img.shields.io/pypi/l/pyrepseq.svg)](https://github.com/andim/pyrepseq/blob/master/LICENSE)
 [![Latest release](https://img.shields.io/pypi/v/pyrepseq.svg)](https://pypi.python.org/pypi/pyrepseq)
 [![Build Status](https://app.travis-ci.com/andim/pyrepseq.svg?branch=main)](https://app.travis-ci.com/andim/pyrepseq)
 [![Documentation Status](https://readthedocs.org/projects/pyrepseq/badge/?version=latest)](https://pyrepseq.readthedocs.io/en/latest/?badge=latest)
 
-# Pyrepseq: the Swiss army knife of immune repertoire analyses
+# Pyrepseq: analyze your immune repertoire data with ease
 
 Pyrepseq is `scipy` & `seaborn` for studying adaptive immunity: modular implementations of algorithms for fast analyses, and bespoke plotting functions for compelling visualizations.
 
+## Documentation and examples
+
+You can find API documentation on [readthedocs](https://pyrepseq.readthedocs.io/en/latest/?badge=latest)
+
+There are jupyter notebooks illustrating some of the functionality in the 'examples' folder.
+
+You can also find usage examples by looking at the code underlying our recent paper [Mayer Callan PNAS 2023](https://github.com/andim/paper_coincidences).
+
 ## Installation
 
 The quickest way to install Pyrepseq is via pip:
 
 `pip install pyrepseq`
```

### Comparing `pyrepseq-1.0/pyrepseq/data/pcdelta_pbmc_minervina.csv` & `pyrepseq-1.1/pyrepseq/data/pcdelta_pbmc_minervina.csv`

 * *Files identical despite different names*

### Comparing `pyrepseq-1.0/pyrepseq/distance.py` & `pyrepseq-1.1/pyrepseq/distance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .io import aminoacids
+from .stats import pc
 import os.path
 import itertools
 
 import numpy as np
 import pandas as pd
 
 from scipy.spatial.distance import squareform
@@ -115,14 +116,15 @@
     ----------
     seqs: [list of strings | tuple of lists]
         sequences, or (seqs_alpha, seqs_beta)
     seqs2: [list of strings | tuple of lists] (optional)
         second list of sequences for cross-comparisons
     bins: iterable
         bins for the distances Delta. (Default: range(0, 25))
+        bins=0: Calculate exact coincidence probability
     normalize: bool
         whether to return pc (normalized) or raw counts
     pseudocount : float
        for a Bayesian estimation of coincidence frequencies
        e.g. can use Jeffrey's prior value of 0.5 
     maxseqs: int
         maximal number of sequences to keep by random downsampling
@@ -132,14 +134,17 @@
     Returns
     -------
     np.ndarray
         (normalized) histogram of sequence distances
     """
     if bins is None:
         bins = np.arange(0, 25)
+    if isinstance(bins, int) and bins == 0:
+        return pc(seqs, seqs2)
+
     seqs = downsample(seqs, maxseqs)
     if (type(seqs) is tuple) or ((type(seqs) is pd.DataFrame) and seqs.shape[1]==2):
         if type(seqs) is tuple:
             seqs_alpha, seqs_beta = seqs
         if type(seqs) is pd.DataFrame:
             seqs_alpha, seqs_beta = seqs.iloc[:, 0], seqs.iloc[:, 1]
         if seqs2 is None:
@@ -180,28 +185,32 @@
     -------
     pcs : pd.DataFrame
         Returns a DataFrame of pC(delta) for each group
     
     """
     
     def pcDelta_within_group(dfg):
+        index = kwargs.get('bins')
+        index = [index] if isinstance(index, int) else index
         return pd.Series(pcDelta(dfg[seq_columns], **kwargs),
-                         name='Delta', index=kwargs.get('bins'))
+                         name='Delta', index=index)
     return df.groupby(by).apply(pcDelta_within_group)
 
-def pcDelta_grouped_cross(df, by, seq_columns, **kwargs):
+def pcDelta_grouped_cross(df, by, seq_columns, condensed=False, **kwargs):
     """Near-coincidence probabilities conditioned to cross-group comparisons.
     
     Parameters
     ----------
     df : pd.DataFrame
     by : mapping, function, label, or list of labels
       see pd.DataFrame.groupby
     seq_columns : string
        The data frame column on which we want to apply the pcDelta analysis
+    condensed : bool
+        Return a condensed instead of squareform matrix (default: False)
     **kwargs : keyword arguments
         passed on to pcDelta
        
     Returns
     -------
     pcs : pd.DataFrame
         Returns a DataFrame of pC(delta) across pairs of groups
@@ -212,16 +221,23 @@
     data = []
     index = []
     for ((name1, d1)), (name2, d2) in itertools.combinations(groups, 2):
         pcg = pcDelta(d1[seq_columns], d2[seq_columns], **kwargs)
         index.append([name1, name2])
         data.append(pcg)
     data = np.array(data)
-    index = np.array(index)
-    return pd.DataFrame(data, index=index)
+    if condensed:
+        return pd.DataFrame(data,
+        	index=pd.MultiIndex.from_tuples(index,
+        	names=['group1', 'group2']))
+    names = [name for name, dfg in groups]
+    data_square = squareform(data)
+    np.fill_diagonal(data_square,
+                     pcDelta_grouped(df, by, seq_columns=seq_columns, **kwargs))
+    return pd.DataFrame(data_square, index=names, columns=names)
 
 def load_pcDelta_background(return_bins=True):
     """
     Loads pre-computed background pcDelta distributions calculated for PBMC TCRs.
 
     Data: Sample W_F1_2018 from Minervina et al. https://zenodo.org/record/4065547/
```

### Comparing `pyrepseq-1.0/pyrepseq/plotting.py` & `pyrepseq-1.1/pyrepseq/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,28 +197,30 @@
     return plotter.plot(metric=metric, method=method,
                         colorbar_kws=cbar_kws,
                         row_cluster=row_cluster, col_cluster=col_cluster,
                         row_linkage=row_linkage, col_linkage=col_linkage,
                         tree_kws=tree_kws, **kws)
 
 def similarity_clustermap(df, alpha_column='cdr3a', beta_column='cdr3b',
-                           linkage_kws=dict(method='average', optimal_ordering=True),
-                           cluster_kws=dict(t=6, criterion='distance'),
-                           cbar_kws=dict(label='Sequence Distance',
-                               format='%d', orientation='horizontal'),
-                           meta_columns=None,
-                           meta_to_colors=None,
-                           **kws):
+                          norm=None,
+                          linkage_kws=dict(method='average', optimal_ordering=True),
+                          cluster_kws=dict(t=6, criterion='distance'),
+                          cbar_kws=dict(label='Sequence Distance',
+                              format='%d', orientation='horizontal'),
+                          meta_columns=None,
+                          meta_to_colors=None,
+                          **kws):
     """
     Plots a sequence-similarity clustermap.
 
     Parameters
     ----------
     df : pandas DataFrame with data
     alpha_column, beta_column: column name with alpha and beta amino acid information
+    norm: function to normalize distances
     linkage_kws: keyword arguments for linkage algorithm
     cluster_kws: keyword arguments for clustering algorithm
     cbar_kws: keyword arguments for colorbar
     meta_columns: list-like
         metadata to plot alongside the cluster assignment 
     meta_to_colors: list-like
         list of functions mapping metadata labels to colors
@@ -243,16 +245,20 @@
     linkage = hc.linkage(distances, **linkage_kws)
     cluster = hc.fcluster(linkage, **cluster_kws)
 
     cmap = plt.cm.viridis
     cmaplist = [cmap(i) for i in range(cmap.N)]
     cmap = mpl.colors.LinearSegmentedColormap.from_list(
         'Custom cmap', list(reversed(cmaplist)), cmap.N)
-    bounds = np.arange(0, 7, 1) 
-    norm = mpl.colors.BoundaryNorm(bounds, cmap.N)
+
+    if norm is None:
+        bounds = np.arange(0, 7, 1) 
+        norm = mpl.colors.BoundaryNorm(bounds, cmap.N)
+        # plot tick in the middle of the discretized colormap
+        cbar_kws.update(dict(ticks=bounds[:-1]+0.5))
 
     cluster_colors = pd.Series(meta_to_colors[0](cluster, min_count=2),
                                name='Cluster')
     if not meta_columns is None:
         colors_list = [cluster_colors]
         if type(meta_columns) is dict:
             meta_colors = [pd.Series(mapper(df[col]), name=meta_columns[col])
@@ -261,16 +267,14 @@
             meta_colors = [pd.Series(mapper(df[col]), name=col)
                     for col, mapper in zip(meta_columns, meta_to_colors[1:])]
         colors_list.extend(meta_colors)
         colors = pd.concat(colors_list, axis=1)
     else:
         colors = cluster_colors
     
-    # plot tick in the middle of the discretized colormap
-    cbar_kws.update(dict(ticks=bounds[:-1]+0.5))
     
     # default clustermap kws
     clustermap_kws = dict(cbar_kws=cbar_kws,
                           dendrogram_ratio=0.12, colors_ratio=0.04,
                           cbar_pos=(0.38, .99, .4, .02),
                           rasterized=True, figsize=(4.2, 4.2),
                           xticklabels=[], yticklabels=[],
@@ -280,17 +284,18 @@
     cg = clustermap_split(pd.DataFrame(squareform(distances_alpha)),
                           pd.DataFrame(squareform(distances_beta)),
                           row_linkage=linkage, col_linkage=linkage,
                           cmap=cmap, norm=norm,
                           row_colors=colors,
                           **clustermap_kws)
 
-    cbar_labels = [str(b) for b in bounds[:-1]]
-    cbar_labels[-1] = '>' + cbar_labels[-1]
-    cg.cax.set_xticklabels(cbar_labels)
+    if norm is None:
+        cbar_labels = [str(b) for b in bounds[:-1]]
+        cbar_labels[-1] = '>' + cbar_labels[-1]
+        cg.cax.set_xticklabels(cbar_labels)
     cg.ax_heatmap.set_xlabel(r'CDR3$\alpha$ Sequence')
     cg.ax_heatmap.set_ylabel(r'CDR3$\beta$ Sequence')
     cg.ax_col_dendrogram.set_visible(False)
     return cg, linkage, cluster
 
 def label_axes(fig_or_axes, labels=string.ascii_uppercase,
                labelstyle=r'%s',
@@ -352,14 +357,18 @@
     ----------
     seqs: iterable of strings
         sequences to be displayed
     ax: matplotlib.axes
         if None create new figure
     **kwargs: dict
         passed on to logomaker.Logo
+
+    Returns
+    -------
+    axes, counts_matrix
     """
     lengths = np.array([len(s) for s in seqs])
     if(len(np.unique(lengths))>1):
         seqs = align_seqs(seqs)
     counts_mat = lm.alignment_to_matrix(seqs)
     if ax is None:
         fig, ax = plt.subplots(figsize=(0.3*counts_mat.shape[0], 0.4))
@@ -368,15 +377,15 @@
     lm_kwargs.update(kwargs)
     lm.Logo(counts_mat, ax=ax, **lm_kwargs)
     ax.set_xticks([])
     ax.set_yticks([])
     ax.spines['bottom'].set_visible(False)
     if ax is None:
         fig.tight_layout()
-    return ax
+    return ax, counts_mat
    
 def seqlogos_vj(df, cdr3_column, v_column, j_column, axes=None, **kwargs):
     """
     Display a sequence logo with V and J gene information.
 
     Parameters
     ----------
```

### Comparing `pyrepseq-1.0/pyrepseq/version.py` & `pyrepseq-1.1/pyrepseq/version.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from os.path import join as pjoin
 
 # Format expected by setup.py and doc/source/conf.py: string of form "X.Y.Z"
 _version_major = 1
-_version_minor = 0
+_version_minor = 1
 _version_micro = ''  # use '' for first of series, number for 1 and above
 #_version_extra = 'dev'
 _version_extra = ''  # Uncomment this for full releases
 
 # Construct full version string from these.
 _ver = [_version_major, _version_minor]
 if _version_micro:
@@ -46,8 +46,8 @@
 MAJOR = _version_major
 MINOR = _version_minor
 MICRO = _version_micro
 VERSION = __version__
 PACKAGES = ['pyrepseq']
 PACKAGE_DATA = {'' : ['data/*.csv']}
 REQUIRES = ["numpy", "scipy", "pandas", "Levenshtein", "matplotlib",
-            "seaborn", "logomaker", "biopython"]
+            "seaborn", "logomaker", "biopython", "tidytcells>=1.4.0"]
```

### Comparing `pyrepseq-1.0/pyrepseq.egg-info/PKG-INFO` & `pyrepseq-1.1/pyrepseq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepseq
-Version: 1.0
+Version: 1.1
 Summary: Python library for immune repertoire analyses
 Home-page: http://pyrepseq.readthedocs.io/
 Download-URL: http://github.com/andim/pyrepseq
 Author: Andreas Mayer
 Author-email: andimscience@gmail.com
 Maintainer: Andreas Mayer
 Maintainer-email: andimscience@gmail.com
```

### Comparing `pyrepseq-1.0/setup.py` & `pyrepseq-1.1/setup.py`

 * *Files identical despite different names*

