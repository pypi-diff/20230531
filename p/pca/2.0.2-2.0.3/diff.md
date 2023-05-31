# Comparing `tmp/pca-2.0.2.tar.gz` & `tmp/pca-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pca-2.0.2.tar", last modified: Sun May 28 21:20:52 2023, max compression
+gzip compressed data, was "pca-2.0.3.tar", last modified: Wed May 31 20:47:32 2023, max compression
```

## Comparing `pca-2.0.2.tar` & `pca-2.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 21:20:52.944193 pca-2.0.2/
--rw-rw-rw-   0        0        0     1094 2022-05-07 12:53:27.000000 pca-2.0.2/LICENSE
--rw-rw-rw-   0        0        0      100 2022-05-07 12:53:27.000000 pca-2.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0    10335 2023-05-28 21:20:52.942703 pca-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     9811 2023-05-28 19:59:46.000000 pca-2.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 21:20:52.901265 pca-2.0.2/pca/
--rw-rw-rw-   0        0        0     1272 2023-05-28 21:20:40.000000 pca-2.0.2/pca/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 21:20:52.940201 pca-2.0.2/pca/data/
--rw-rw-rw-   0        0        0        0 2022-05-07 12:53:27.000000 pca-2.0.2/pca/data/__init__.py
--rw-rw-rw-   0        0        0    33480 2023-04-28 11:42:55.000000 pca-2.0.2/pca/examples.py
--rw-rw-rw-   0        0        0    78132 2023-05-28 14:18:17.000000 pca-2.0.2/pca/pca.py
-drwxrwxrwx   0        0        0        0 2023-05-28 21:20:52.941706 pca-2.0.2/pca/tests/
--rw-rw-rw-   0        0        0        0 2022-05-07 12:53:27.000000 pca-2.0.2/pca/tests/__init__.py
--rw-rw-rw-   0        0        0    10683 2023-04-23 10:01:48.000000 pca-2.0.2/pca/tests/test_pca.py
-drwxrwxrwx   0        0        0        0 2023-05-28 21:20:52.937430 pca-2.0.2/pca.egg-info/
--rw-rw-rw-   0        0        0    10335 2023-05-28 21:20:52.000000 pca-2.0.2/pca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-05-28 21:20:52.000000 pca-2.0.2/pca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 21:20:52.000000 pca-2.0.2/pca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2023-05-28 21:20:52.000000 pca-2.0.2/pca.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-28 21:20:52.000000 pca-2.0.2/pca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 21:20:52.944193 pca-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1459 2023-04-23 09:54:09.000000 pca-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 20:47:32.001826 pca-2.0.3/
+-rw-rw-rw-   0        0        0     1094 2022-05-07 12:53:27.000000 pca-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0      100 2022-05-07 12:53:27.000000 pca-2.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    10335 2023-05-31 20:47:31.995837 pca-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9811 2023-05-28 19:59:46.000000 pca-2.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 20:47:31.921043 pca-2.0.3/pca/
+-rw-rw-rw-   0        0        0     1272 2023-05-31 20:46:18.000000 pca-2.0.3/pca/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 20:47:31.990049 pca-2.0.3/pca/data/
+-rw-rw-rw-   0        0        0        0 2022-05-07 12:53:27.000000 pca-2.0.3/pca/data/__init__.py
+-rw-rw-rw-   0        0        0    33480 2023-04-28 11:42:55.000000 pca-2.0.3/pca/examples.py
+-rw-rw-rw-   0        0        0    75101 2023-05-31 20:43:53.000000 pca-2.0.3/pca/pca.py
+drwxrwxrwx   0        0        0        0 2023-05-31 20:47:31.993843 pca-2.0.3/pca/tests/
+-rw-rw-rw-   0        0        0        0 2022-05-07 12:53:27.000000 pca-2.0.3/pca/tests/__init__.py
+-rw-rw-rw-   0        0        0    10683 2023-05-31 19:00:16.000000 pca-2.0.3/pca/tests/test_pca.py
+drwxrwxrwx   0        0        0        0 2023-05-31 20:47:31.987856 pca-2.0.3/pca.egg-info/
+-rw-rw-rw-   0        0        0    10335 2023-05-31 20:47:31.000000 pca-2.0.3/pca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-05-31 20:47:31.000000 pca-2.0.3/pca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 20:47:31.000000 pca-2.0.3/pca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-05-31 20:47:31.000000 pca-2.0.3/pca.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-31 20:47:31.000000 pca-2.0.3/pca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 20:47:32.002044 pca-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1700 2023-05-31 20:38:42.000000 pca-2.0.3/setup.py
```

### Comparing `pca-2.0.2/LICENSE` & `pca-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pca-2.0.2/PKG-INFO` & `pca-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pca
-Version: 2.0.2
+Version: 2.0.3
 Summary: pca: A Python Package for Principal Component Analysis.
 Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/2.0.2.tar.gz
+Download-URL: https://github.com/erdogant/pca/archive/2.0.3.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pca Version: 2.0.2 Summary: pca: A Python Package
+Metadata-Version: 2.1 Name: pca Version: 2.0.3 Summary: pca: A Python Package
 for Principal Component Analysis. Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/2.0.2.tar.gz Author:
+Download-URL: https://github.com/erdogant/pca/archive/2.0.3.tar.gz Author:
 Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3
 Description-Content-Type: text/markdown License-File: LICENSE
    [https://github.com/erdogant/pca/blob/master/docs/figs/iris_density.png]
 [![Python](https://img.shields.io/pypi/pyversions/pca)](https://img.shields.io/
 pypi/pyversions/pca) [![Pypi](https://img.shields.io/pypi/v/pca)](https://
```

### Comparing `pca-2.0.2/README.md` & `pca-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pca-2.0.2/pca/__init__.py` & `pca-2.0.3/pca/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     hotellingsT2,
     spe_dmodx,
     )
 
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '2.0.2'
+__version__ = '2.0.3'
 
 # module level doc-string
 __doc__ = """
 pca
 =====================================================================
 
 Description
```

### Comparing `pca-2.0.2/pca/examples.py` & `pca-2.0.3/pca/examples.py`

 * *Files identical despite different names*

### Comparing `pca-2.0.2/pca/pca.py` & `pca-2.0.3/pca/pca.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 """pca: A Python Package for Principal Component Analysis."""
 
-# %% Libraries
-import requests
-from urllib.parse import urlparse
-from tqdm import tqdm
+import datazets as dz
 from scatterd import scatterd
 from sklearn.decomposition import PCA, SparsePCA, TruncatedSVD  # MiniBatchSparsePCA
 from sklearn.preprocessing import StandardScaler
 from sklearn.metrics.pairwise import euclidean_distances
 from scipy import stats
 from matplotlib.patches import Ellipse
 import scipy.sparse as sp
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
-import os
 from adjustText import adjust_text
 import statsmodels.stats.multitest as multitest
-from typing import List, Union, Tuple
+from typing import Union
 
 
 # %% Association learning across all variables
 class pca:
     """pca module.
 
     Parameters
@@ -72,27 +68,27 @@
     References
     ----------
     * Blog: https://towardsdatascience.com/what-are-pca-loadings-and-biplots-9a7897f2e559
     * Github: https://github.com/erdogant/pca
     * Documentation: https://erdogant.github.io/pca/
 
     """
+
     def __init__(self,
                  n_components=0.95,
                  n_feat=25,
                  method='pca',
                  alpha=0.05,
                  multipletests='fdr_bh',
                  n_std=3,
                  onehot=False,
                  normalize=False,
                  detect_outliers=['ht2', 'spe'],
                  random_state=None,
                  verbose=3):
-
         """Initialize pca with user-defined parameters."""
         if isinstance(detect_outliers, str): detect_outliers = [detect_outliers]
         if detect_outliers is not None: detect_outliers=list(map(str.lower, detect_outliers))
 
         if onehot:
             if verbose>=3: print('[pca] >Method is set to: [sparse_pca] because onehot=True.')
             method = 'sparse_pca'
@@ -426,15 +422,15 @@
             self.n_components = X.shape[1] - 1
             if verbose>=3: print('[pca] >n_components is set to %d' %(self.n_components))
 
         self.n_feat = np.min([self.n_feat, X.shape[1]])
 
         if (not self.onehot) and (not self.normalize) and isinstance(X, pd.DataFrame) and (str(X.values.dtype)=='bool'):
             if verbose>=2: print('[pca] >[WARNING]: Sparse or one-hot boolean input data is detected, it is highly recommended to set onehot=True or alternatively, normalize=True')
-        
+
         # Set col labels
         if isinstance(X, pd.DataFrame) and col_labels is None:
             if verbose>=3: print('[pca] >Extracting column labels from dataframe.')
             col_labels = X.columns.values
         if col_labels is None or len(col_labels)==0 or len(col_labels)!=X.shape[1]:
             if verbose>=3: print('[pca] >Column labels are auto-completed.')
             col_labels = np.arange(1, X.shape[1] + 1).astype(str)
@@ -447,15 +443,14 @@
             row_labels = X.index.values
         if row_labels is None or len(row_labels)!=X.shape[0]:
             # row_labels = np.ones(X.shape[0]).astype(int)
             row_labels = np.arange(0, X.shape[0]).astype(int)
             if verbose>=3: print('[pca] >Row labels are auto-completed.')
         # if isinstance(row_labels, list):
         row_labels=np.array(row_labels)
-        
 
         if isinstance(X, pd.DataFrame):
             X = X.values
 
         if sp.issparse(X) and self.normalize:
             if verbose>=3: print('[pca] >[WARNING]: Can not normalize a sparse matrix. Normalize is set to [False]')
             self.normalize=False
@@ -527,27 +522,27 @@
             raise Exception('[pca] >Error: No PCs are found with explained variance.')
 
         return labels, topfeat, n_feat
 
     # Scatter plot
     def scatter(self,
                 labels=None,
-                c=[0,0.1,0.4],
+                c=[0, 0.1, 0.4],
                 s=150,
                 marker='o',
                 edgecolor='#000000',
                 SPE=False,
                 HT2=False,
                 jitter=None,
                 PC=None,
                 alpha=0.8,
                 gradient=None,
                 density=False,
                 density_on_top=False,
-                fontcolor=[0,0,0],
+                fontcolor=[0, 0, 0],
                 fontsize=18,
                 fontweight='normal',
                 cmap='tab20c',
                 title=None,
                 legend=None,
                 figsize=(25, 15),
                 dpi=100,
@@ -640,14 +635,17 @@
 
         """
         if verbose is None: verbose = self.verbose
         _show_deprecated_warning(label, y, verbose)
         if not hasattr(self, 'results'):
             if verbose>=2: print('[pca]> No results to plot. Hint: model.fit(X) <return>.')
             return None, None
+        if (PC is not None) and self.results['PC'].shape[1]<len(PC):
+            if verbose>=1: print('[pca]> 3D plot requires 3 PCs <return>.')
+            return None, None
 
         # Set parameters based on intuition
         if c is None: s=0
         if cmap is None: s=0
         if alpha is None: alpha=0.8
         if PC is None: PC=[0, 1]
         d3 = True if len(PC)==3 else False
@@ -692,28 +690,28 @@
         # Add figure properties
         fig, ax = _add_plot_properties(self, PC, d3, title, legend, labels, fig, ax, fontsize, verbose)
         # Return
         return (fig, ax)
 
     def biplot(self,
                labels=None,
-               c=[0,0.1,0.4],
+               c=[0, 0.1, 0.4],
                s=150,
                marker='o',
                edgecolor='#000000',
                jitter=None,
                n_feat=None,
                PC=None,
                SPE=None,
                HT2=None,
                alpha=0.8,
                gradient=None,
                density=False,
                density_on_top=False,
-               fontcolor=[0,0,0],
+               fontcolor=[0, 0, 0],
                fontsize=18,
                fontweight='normal',
                color_arrow=None,
                arrowdict={'fontsize': None, 'color_text': None, 'weight': None, 'alpha': None, 'color_strong': '#880808', 'color_weak': '#002a77', 'scale_factor': None},
                cmap='tab20c',
                title=None,
                legend=None,
@@ -854,15 +852,15 @@
         # Pre-processing
         labels, topfeat, n_feat = self._fig_preprocessing(labels, n_feat, d3)
         # Scatterplot
         fig, ax = self.scatter(labels=labels, legend=legend, PC=PC, SPE=SPE, HT2=HT2, cmap=cmap, visible=visible, figsize=figsize, alpha=alpha, title=title, gradient=gradient, fig=fig, ax=ax, c=c, s=s, jitter=jitter, marker=marker, fontcolor=fontcolor, fontweight=fontweight, fontsize=fontsize, edgecolor=edgecolor, density=density, density_on_top=density_on_top, dpi=dpi, grid=grid, verbose=verbose)
         # Add the loadings with arrow to the plot
         fig, ax = _plot_loadings(self, topfeat, n_feat, PC, d3, arrowdict, fig, ax, verbose)
         # Plot
-        if visible: plt.show()
+        # if visible: plt.show()
         # Return
         return fig, ax
 
     def scatter3d(self, PC=[0, 1, 2], **args):
         """Scatter 3d plot.
 
         Parameters
@@ -938,17 +936,16 @@
         if fig is None and ax is None:
             # Create entire new figure.
             fig, ax = plt.subplots(figsize=figsize, edgecolor='k')
         elif fig is not None and ax is None:
             ax = fig.axes[0]
 
         # Set visibility and plot
-        if fig is not None:
-            fig.set_visible(visible)
-        plt.plot(xtick_idx, explvarCum, 'o-', color='k', linewidth=1, label='Cumulative explained variance')
+        if fig is not None: fig.set_visible(visible)
+        plt.plot(xtick_idx, explvarCum, 'o-', color='k', linewidth=1, label='Cumulative explained variance', visible=visible)
 
         # Set xticks if less then 100 datapoints
         if len(explvar)<100:
             ax.set_xticks(xtick_idx)
             xticklabel=xtick_idx.astype(str)
             if xsteps is not None:
                 xticklabel[np.arange(1, len(xticklabel), xsteps)] = ''
@@ -965,17 +962,17 @@
 
         # Plot vertical line To stress the cut-off point
         ax.axvline(self.n_components, linewidth=0.8, color='r')
         ax.axhline(y=self.results['pcp'], xmin=0, xmax=1, linewidth=0.8, color='r')
         if len(xtick_idx)<100:
             plt.bar(xtick_idx, explvar, color='#3182bd', alpha=0.8, label='Explained variance')
 
-        if visible:
-            plt.show()
-            plt.draw()
+        # if visible:
+        #     plt.draw()
+        #     plt.show()
         # Return
         return (fig, ax)
 
     # Top scoring components
     def norm(self, X, n_components=None, pcexclude=[1]):
         """Normalize out PCs.
 
@@ -1047,15 +1044,15 @@
 
         Returns
         -------
         pd.DataFrame()
             Dataset containing mixed features.
 
         """
-        return import_example(data=data, url=url, sep=sep)
+        return import_example(data=data, url=url, sep=sep, verbose=0)
 
 
 # %%
 def _get_coordinates(PCs, PC):
     xs = PCs.iloc[:, PC[0]].values
     ys = np.zeros(len(xs))
     zs = None
@@ -1365,58 +1362,15 @@
 
     Returns
     -------
     pd.DataFrame()
         Dataset containing mixed features.
 
     """
-    if url is None:
-        if data=='sprinkler':
-            url='https://erdogant.github.io/datasets/sprinkler.zip'
-        elif data=='titanic':
-            url='https://erdogant.github.io/datasets/titanic_train.zip'
-        elif data=='student':
-            url='https://erdogant.github.io/datasets/student_train.zip'
-        elif data=='cancer':
-            url='https://erdogant.github.io/datasets/cancer_dataset.zip'
-        elif data=='fifa':
-            url='https://erdogant.github.io/datasets/FIFA_2018.zip'
-        elif data=='waterpump':
-            url='https://erdogant.github.io/datasets/waterpump/waterpump_test.zip'
-        elif data=='retail':
-            url='https://erdogant.github.io/datasets/marketing_data_online_retail_small.zip'
-        elif data=='iris':
-            from sklearn.datasets import load_iris
-            label = load_iris().feature_names
-            y = load_iris().target
-            X = pd.DataFrame(data=load_iris().data, columns=label, index=y)
-            return X
-        else:
-            data = wget.filename_from_url(url)
-
-    if url is None:
-        if verbose>=3: print('Nothing to download.')
-        return None
-
-    curpath = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data')
-    filename = os.path.basename(urlparse(url).path)
-    PATH_TO_DATA = os.path.join(curpath, filename)
-    if not os.path.isdir(curpath):
-        os.makedirs(curpath, exist_ok=True)
-
-    # Check file exists.
-    if not os.path.isfile(PATH_TO_DATA):
-        if verbose>=3: print('Downloading [%s] dataset from github source..' %(data))
-        wget.download(url, PATH_TO_DATA)
-
-    # Import local dataset
-    if verbose>=3: print('Import dataset [%s]' %(data))
-    df = pd.read_csv(PATH_TO_DATA, sep=sep)
-    # Return
-    return df
+    return dz.get(data, url=url, sep=sep, verbose=0)
 
 
 # %%
 def _get_explained_variance(X, components):
     """Get the explained variance.
 
     Get the explained variance from the principal components of the
@@ -1455,15 +1409,15 @@
     # Algorithm, as we compute the adjustd variance for each component, we
     # subtract the variance from components in the direction of previous axes
     proj_corrected_vecs = np.zeros_like(components)
     for i in range(n_components):
         vec = components[i].copy()
         # subtract the previous projections
         for j in range(i):
-            vec -= np.dot(unit_vecs[j], vec)*unit_vecs[j]
+            vec -= np.dot(unit_vecs[j], vec) * unit_vecs[j]
 
         proj_corrected_vecs[i] = vec
 
     # get estimated variance of Y which is matrix product of feature vector
     # and the adjusted components
     Y = np.tensordot(X, proj_corrected_vecs.T, axes=(1, 0))
     YYT = np.tensordot(Y.T, Y, axes=(1, 0))
@@ -1492,88 +1446,36 @@
     # Return
     return arrowdict, cmap, PC, d3, s
 
 
 def _set_arrowdict(arrowdict, color_arrow=None, fontsize=18, fontweight='normal'):
     # color_arrow = None if (color_arrow is None) else color_arrow
     arrowdict = {**{'color_arrow': color_arrow, 'color_text': None, 'fontsize': 18 if fontsize==0 else fontsize, 'weight': fontweight, 'alpha': None, 'ha': 'center', 'va': 'center', 'color_strong': '#880808', 'color_weak': '#002a77', 'scale_factor': None}, **arrowdict}
-    # if arrowdict.get('color_text') is None and (color_arrow is not None):
-        # arrowdict['color_text'] = color_arrow
     if arrowdict.get('fontsize') is None:
         arrowdict['fontsize'] = 18 if fontsize==0 else fontsize
     if arrowdict.get('weight') is None:
         arrowdict['weight'] = fontweight
     return arrowdict
 
 
-# %% Retrieve files files.
-class wget:
-    """Retrieve file from url."""
-
-    def filename_from_url(url):
-        """Return filename."""
-        return os.path.basename(url)
-
-    def download(url, writepath):
-        """Download.
-
-        Parameters
-        ----------
-        url : str.
-            Internet source.
-        writepath : str.
-            Directory to write the file.
-
-        Returns
-        -------
-        None.
-
-        """
-        r = requests.get(url, stream=True)
-        with open(writepath, "wb") as fd:
-            for chunk in r.iter_content(chunk_size=1024):
-                fd.write(chunk)
-
-
-def _setup_figure(fig, ax, d3, visible, figsize, dpi):
-    if fig is None and ax is None:
-        # Create new figure.
-        fig = plt.figure(figsize=figsize, dpi=dpi)
-
-        # Add d3 projection
-        if d3:
-            ax = fig.add_subplot(projection='3d')
-            # ax = Axes3D(fig, rect=[0, 0, .95, 1], elev=48, azim=134)
-        else:
-            ax = fig.add_subplot()
-    elif fig is not None and ax is None:
-        # Extract axes from fig.
-        ax = fig.axes[0]
-
-    if fig is not None:
-        fig.set_visible(visible)
-
-    return fig, ax
-
-
 def _plot_loadings(self, topfeat, n_feat, PC, d3, arrowdict, fig, ax, verbose):
     topfeat = pd.concat([topfeat.iloc[PC, :], topfeat.loc[~topfeat.index.isin(PC), :]])
     topfeat.reset_index(inplace=True)
     # Collect coefficients
     coeff = self.results['loadings'].iloc[PC, :]
 
     # Use the PCs only for scaling purposes
     mean_x = np.mean(self.results['PC'].iloc[:, PC[0]].values)
     mean_y = np.mean(self.results['PC'].iloc[:, PC[1]].values)
     if d3: mean_z = np.mean(self.results['PC'].iloc[:, PC[2]].values)
 
     # Plot and scale values for arrows and text by taking the absolute minimum range of the x-axis and y-axis.
     max_axis = np.max(np.abs(self.results['PC'].iloc[:, PC]).min(axis=1))
     max_arrow = np.abs(coeff).max().max()
-    if arrowdict['scale_factor'] is None: 
+    if arrowdict['scale_factor'] is None:
         scale_factor = 1.8 if d3 else 1.1
     else:
         scale_factor = arrowdict['scale_factor']
     # Scale the arrows using the scale factor
     scale = (np.max([1, np.round(max_axis / max_arrow, 2)])) * scale_factor
 
     # For vizualization purposes we will keep only the unique feature-names
@@ -1582,30 +1484,30 @@
         n_feat = topfeat.shape[0]
         if verbose>=2: print('[pca] >[WARNING]: n_feat can not be reached because of the limitation of n_components (=%d). n_feat is reduced to %d.' %(self.n_components, n_feat))
 
     # Plot arrows and text
     arrow_line_color = arrowdict['color_arrow']
     arrow_text_color = arrowdict['color_text']
     arrow_alpha = arrowdict['alpha']
-    alpha_scaled = normalize_size(topfeat['loading'].abs().values.reshape(-1,1), minscale=0.35, maxscale=0.95, scaler='minmax')
+    alpha_scaled = normalize_size(topfeat['loading'].abs().values.reshape(-1, 1), minscale=0.35, maxscale=0.95, scaler='minmax')
     texts = []
     for i in range(0, n_feat):
         getfeat = topfeat['feature'].iloc[i]
         label = getfeat + ' (' + ('%.3g' %topfeat['loading'].iloc[i]) + ')'
         getcoef = coeff[getfeat].values
         # Set first PC vs second PC direction. Note that these are not neccarily the best loading.
         xarrow = getcoef[0] * scale  # First PC in the x-axis direction
         yarrow = getcoef[1] * scale  # Second PC in the y-axis direction
         # Set the arrow and arrow-text colors
         # Update arrow color if None
         loading_color = arrowdict['color_weak'] if topfeat['type'].iloc[i] == 'weak' else arrowdict['color_strong']
         # Update colors if None
         if arrowdict['color_arrow'] is None: arrow_line_color = loading_color
         if arrowdict['color_text'] is None: arrow_text_color = loading_color
-        if arrowdict['alpha'] is None: arrow_alpha =  alpha_scaled[i]
+        if arrowdict['alpha'] is None: arrow_alpha = alpha_scaled[i]
 
         if d3:
             zarrow = getcoef[2] * scale
             ax.quiver(mean_x, mean_y, mean_z, xarrow - mean_x, yarrow - mean_y, zarrow - mean_z, color=arrow_line_color, alpha=arrow_alpha, lw=2)
             texts.append(ax.text(xarrow, yarrow, zarrow, label, fontsize=arrowdict['fontsize'], c=arrow_text_color, weight=arrowdict['weight'], ha=arrowdict['ha'], va=arrowdict['va'], zorder=25))
         else:
             head_width = 0.1
@@ -1708,15 +1610,15 @@
     -------
     getsizes : array-like
         scaled values between min-max.
 
     """
     # Instead of Min-Max scaling, that shrinks any distribution in the [0, 1] interval, scaling the variables to
     # Z-scores is better. Min-Max Scaling is too sensitive to outlier observations and generates unseen problems,
-    
+
     # Set sizes to 0 if not available
     getsizes[np.isinf(getsizes)]=0
     getsizes[np.isnan(getsizes)]=0
 
     # out-of-scale datapoints.
     if scaler == 'zscore' and len(np.unique(getsizes)) > 3:
         getsizes = (getsizes.flatten() - np.mean(getsizes)) / np.std(getsizes)
```

### Comparing `pca-2.0.2/pca/tests/test_pca.py` & `pca-2.0.3/pca/tests/test_pca.py`

 * *Files identical despite different names*

### Comparing `pca-2.0.2/pca.egg-info/PKG-INFO` & `pca-2.0.3/pca.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pca
-Version: 2.0.2
+Version: 2.0.3
 Summary: pca: A Python Package for Principal Component Analysis.
 Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/2.0.2.tar.gz
+Download-URL: https://github.com/erdogant/pca/archive/2.0.3.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: pca Version: 2.0.2 Summary: pca: A Python Package
+Metadata-Version: 2.1 Name: pca Version: 2.0.3 Summary: pca: A Python Package
 for Principal Component Analysis. Home-page: https://erdogant.github.io/pca
-Download-URL: https://github.com/erdogant/pca/archive/2.0.2.tar.gz Author:
+Download-URL: https://github.com/erdogant/pca/archive/2.0.3.tar.gz Author:
 Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3
 Description-Content-Type: text/markdown License-File: LICENSE
    [https://github.com/erdogant/pca/blob/master/docs/figs/iris_density.png]
 [![Python](https://img.shields.io/pypi/pyversions/pca)](https://img.shields.io/
 pypi/pyversions/pca) [![Pypi](https://img.shields.io/pypi/v/pca)](https://
```

### Comparing `pca-2.0.2/setup.py` & `pca-2.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,25 @@
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 # Setup ------------
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
-     install_requires=['requests', 'statsmodels', 'matplotlib','numpy','scikit-learn','scipy','colourmap>=1.1.11','pandas','tqdm','scatterd>=1.3.1', 'adjusttext'],
+     install_requires=['datazets',
+                       'statsmodels',
+                       'matplotlib',
+                       'numpy',
+                       'scikit-learn',
+                       'scipy',
+                       'colourmap>=1.1.14',
+                       'pandas',
+                       'scatterd>=1.3.1',
+                       'adjusttext',
+                       ],
      python_requires='>=3',
      name='pca',
      version=new_version,
      author="Erdogan Taskesen",
      author_email="erdogant@gmail.com",
      description="pca: A Python Package for Principal Component Analysis.",
      long_description=long_description,
```

