# Comparing `tmp/rapids_singlecell-0.7.0.tar.gz` & `tmp/rapids_singlecell-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapids_singlecell-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rapids_singlecell-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rapids_singlecell-0.7.0.tar` & `rapids_singlecell-0.7.1.tar`

### file list

```diff
@@ -1,58 +1,39 @@
--rw-r--r--   0        0        0     1070 2023-05-30 12:25:00.770346 rapids_singlecell-0.7.0/LICENSE
--rw-r--r--   0        0        0     5987 2023-05-30 12:25:00.770346 rapids_singlecell-0.7.0/README.md
--rw-r--r--   0        0        0      998 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/pyproject.toml
--rwxr-xr-x   0        0        0      132 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/__init__.py
--rw-r--r--   0        0        0    25027 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/cunnData/__init__.py
--rw-r--r--   0        0        0      334 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/__init__.py
--rw-r--r--   0        0        0    36773 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_hvg.py
--rw-r--r--   0        0        0    14581 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_normalize.py
--rw-r--r--   0        0        0     4544 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_pca.py
--rw-r--r--   0        0        0     2783 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_plotting.py
--rw-r--r--   0        0        0     4795 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_regress_out.py
--rw-r--r--   0        0        0     1441 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_scale.py
--rw-r--r--   0        0        0    18267 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_simple.py
--rw-r--r--   0        0        0     3351 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_utils.py
--rw-r--r--   0        0        0       29 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/dcg.py
--rw-r--r--   0        0        0       68 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/decoupler_gpu/__init__.py
--rw-r--r--   0        0        0     4609 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/decoupler_gpu/_method_mlm.py
--rw-r--r--   0        0        0     6349 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/decoupler_gpu/_method_wsum.py
--rw-r--r--   0        0        0       27 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/gr.py
--rw-r--r--   0        0        0       91 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/pl.py
--rw-r--r--   0        0        0       30 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/pp.py
--rw-r--r--   0        0        0      340 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/__init__.py
--rw-r--r--   0        0        0     5576 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_clustering.py
--rw-r--r--   0        0        0     3429 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_diffmap.py
--rw-r--r--   0        0        0     4040 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_draw_graph.py
--rw-r--r--   0        0        0     5154 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_embedding_density.py
--rw-r--r--   0        0        0    12177 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py
--rw-r--r--   0        0        0     1729 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_harmony_integrate.py
--rw-r--r--   0        0        0     2425 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_pymde.py
--rw-r--r--   0        0        0     7928 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py
--rw-r--r--   0        0        0     3241 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_tsne.py
--rw-r--r--   0        0        0       68 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/squidpy_gpu/__init__.py
--rw-r--r--   0        0        0     6012 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/squidpy_gpu/_autocorr.py
--rw-r--r--   0        0        0     6467 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/squidpy_gpu/_gearysc.py
--rw-r--r--   0        0        0    29539 2023-05-30 12:25:01.050366 rapids_singlecell-0.7.0/rapids_singlecell/squidpy_gpu/_ligrec.py
--rw-r--r--   0        0        0     6325 2023-05-30 12:25:01.054366 rapids_singlecell-0.7.0/rapids_singlecell/squidpy_gpu/_moransi.py
--rw-r--r--   0        0        0     6227 2023-05-30 12:25:01.054366 rapids_singlecell-0.7.0/rapids_singlecell/squidpy_gpu/_utils.py
--rw-r--r--   0        0        0      571 2023-05-30 12:25:01.054366 rapids_singlecell-0.7.0/rapids_singlecell/tests/README.md
--rw-r--r--   0        0        0   253384 2023-05-30 12:25:01.054366 rapids_singlecell-0.7.0/rapids_singlecell/tests/_data/dummy.h5ad
--rw-r--r--   0        0        0   106788 2023-05-30 12:25:01.054366 rapids_singlecell-0.7.0/rapids_singlecell/tests/_data/paul15_means.pickle
--rw-r--r--   0        0        0   602117 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/_data/test_data.h5ad
--rw-r--r--   0        0        0    50913 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/_scripts/seurat_hvg.csv
--rw-r--r--   0        0        0   397058 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/_scripts/seurat_hvg_v3.csv.gz
--rw-r--r--   0        0        0    62865 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/_scripts/seurat_hvg_v3_batch.csv
--rw-r--r--   0        0        0     1362 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_autocorr.py
--rw-r--r--   0        0        0      461 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_clustering.py
--rw-r--r--   0        0        0    10341 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_cunndata.py
--rw-r--r--   0        0        0     2246 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_decoupler.py
--rw-r--r--   0        0        0      687 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_emdedding_density.py
--rw-r--r--   0        0        0    10622 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_hvg.py
--rw-r--r--   0        0        0    12995 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_ligrec.py
--rw-r--r--   0        0        0     2727 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_normalization.py
--rw-r--r--   0        0        0     3165 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_pca.py
--rw-r--r--   0        0        0      532 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_preprocessing.py
--rw-r--r--   0        0        0     3654 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_qc_metrics.py
--rw-r--r--   0        0        0     1717 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tests/test_rank_genes_groups_logreg.py
--rw-r--r--   0        0        0       26 2023-05-30 12:25:01.058367 rapids_singlecell-0.7.0/rapids_singlecell/tl.py
--rw-r--r--   0        0        0     6794 1970-01-01 00:00:00.000000 rapids_singlecell-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-31 21:28:46.364811 rapids_singlecell-0.7.1/LICENSE
+-rw-r--r--   0        0        0     5987 2023-05-31 21:28:46.364811 rapids_singlecell-0.7.1/README.md
+-rw-r--r--   0        0        0     1062 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/pyproject.toml
+-rwxr-xr-x   0        0        0      132 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/__init__.py
+-rw-r--r--   0        0        0    25027 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/cunnData/__init__.py
+-rw-r--r--   0        0        0      334 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/__init__.py
+-rw-r--r--   0        0        0    36773 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_hvg.py
+-rw-r--r--   0        0        0    14581 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_normalize.py
+-rw-r--r--   0        0        0     4544 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_pca.py
+-rw-r--r--   0        0        0     2783 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_plotting.py
+-rw-r--r--   0        0        0     4795 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_regress_out.py
+-rw-r--r--   0        0        0     1441 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_scale.py
+-rw-r--r--   0        0        0    18267 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_simple.py
+-rw-r--r--   0        0        0     3351 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_utils.py
+-rw-r--r--   0        0        0       29 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/dcg.py
+-rw-r--r--   0        0        0       68 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/decoupler_gpu/__init__.py
+-rw-r--r--   0        0        0     4609 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/decoupler_gpu/_method_mlm.py
+-rw-r--r--   0        0        0     6349 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/decoupler_gpu/_method_wsum.py
+-rw-r--r--   0        0        0       27 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/gr.py
+-rw-r--r--   0        0        0       91 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/pl.py
+-rw-r--r--   0        0        0       30 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/pp.py
+-rw-r--r--   0        0        0      340 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/__init__.py
+-rw-r--r--   0        0        0     5576 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_clustering.py
+-rw-r--r--   0        0        0     3429 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_diffmap.py
+-rw-r--r--   0        0        0     4040 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_draw_graph.py
+-rw-r--r--   0        0        0     5154 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_embedding_density.py
+-rw-r--r--   0        0        0    12177 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py
+-rw-r--r--   0        0        0     1729 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_harmony_integrate.py
+-rw-r--r--   0        0        0     2425 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_pymde.py
+-rw-r--r--   0        0        0     7928 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py
+-rw-r--r--   0        0        0     3241 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_tsne.py
+-rw-r--r--   0        0        0       68 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/squidpy_gpu/__init__.py
+-rw-r--r--   0        0        0     6012 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/squidpy_gpu/_autocorr.py
+-rw-r--r--   0        0        0     6467 2023-05-31 21:28:46.624815 rapids_singlecell-0.7.1/rapids_singlecell/squidpy_gpu/_gearysc.py
+-rw-r--r--   0        0        0    29539 2023-05-31 21:28:46.628815 rapids_singlecell-0.7.1/rapids_singlecell/squidpy_gpu/_ligrec.py
+-rw-r--r--   0        0        0     6325 2023-05-31 21:28:46.628815 rapids_singlecell-0.7.1/rapids_singlecell/squidpy_gpu/_moransi.py
+-rw-r--r--   0        0        0     6227 2023-05-31 21:28:46.628815 rapids_singlecell-0.7.1/rapids_singlecell/squidpy_gpu/_utils.py
+-rw-r--r--   0        0        0       26 2023-05-31 21:28:46.632815 rapids_singlecell-0.7.1/rapids_singlecell/tl.py
+-rw-r--r--   0        0        0     6794 1970-01-01 00:00:00.000000 rapids_singlecell-0.7.1/PKG-INFO
```

### Comparing `rapids_singlecell-0.7.0/LICENSE` & `rapids_singlecell-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/README.md` & `rapids_singlecell-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/pyproject.toml` & `rapids_singlecell-0.7.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -37,7 +37,12 @@
 Documentation = "https://rapids-singlecell.readthedocs.io"
 Source = "https://github.com/Intron7/rapids_singlecell"
 
 [tool.black]
 line-length = 88
 target-version = ['py38']
 include = '^rapids_singlecell/.*\.py$'
+
+[tool.flit.sdist]
+exclude = [
+    "rapids_singlecell/tests",
+]
```

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/cunnData/__init__.py` & `rapids_singlecell-0.7.1/rapids_singlecell/cunnData/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -474,15 +474,15 @@
     def _inplace_subset_obs(self, index):
         """\
         Inplace subsetting along observations dimension.
 
         Same as `adata = adata[index, :]`, but inplace.
         """
         obs_dx, _ = _normalize_indices(
-            index, (slice(None, None, None)), self.obs_names, self.var_names
+            (index, slice(None, None, None)), self.obs_names, self.var_names
         )
         x_dim = _get_dimensions(obs_dx, self.shape[0])
         self._X = self.X[obs_dx, :].reshape(x_dim, self.n_vars)
         self._update_shape()
         self.obs = pd.DataFrame(self.obs.iloc[obs_dx, :])
         if self.layers:
             for key, matrix in self.layers.items():
```

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_hvg.py` & `rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_hvg.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_normalize.py` & `rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_normalize.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_pca.py` & `rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_pca.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_plotting.py` & `rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_plotting.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_regress_out.py` & `rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_regress_out.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_scale.py` & `rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_scale.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_simple.py` & `rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_simple.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/cunnData_funcs/_utils.py` & `rapids_singlecell-0.7.1/rapids_singlecell/cunnData_funcs/_utils.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/decoupler_gpu/_method_mlm.py` & `rapids_singlecell-0.7.1/rapids_singlecell/decoupler_gpu/_method_mlm.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/decoupler_gpu/_method_wsum.py` & `rapids_singlecell-0.7.1/rapids_singlecell/decoupler_gpu/_method_wsum.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_clustering.py` & `rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_clustering.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_diffmap.py` & `rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_diffmap.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_draw_graph.py` & `rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_draw_graph.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_embedding_density.py` & `rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_embedding_density.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py` & `rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_harmonpy_gpu.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_harmony_integrate.py` & `rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_harmony_integrate.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_pymde.py` & `rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_pymde.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py` & `rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_rank_gene_groups.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/scanpy_gpu/_tsne.py` & `rapids_singlecell-0.7.1/rapids_singlecell/scanpy_gpu/_tsne.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/squidpy_gpu/_autocorr.py` & `rapids_singlecell-0.7.1/rapids_singlecell/squidpy_gpu/_autocorr.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/squidpy_gpu/_gearysc.py` & `rapids_singlecell-0.7.1/rapids_singlecell/squidpy_gpu/_gearysc.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/squidpy_gpu/_ligrec.py` & `rapids_singlecell-0.7.1/rapids_singlecell/squidpy_gpu/_ligrec.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/squidpy_gpu/_moransi.py` & `rapids_singlecell-0.7.1/rapids_singlecell/squidpy_gpu/_moransi.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/rapids_singlecell/squidpy_gpu/_utils.py` & `rapids_singlecell-0.7.1/rapids_singlecell/squidpy_gpu/_utils.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.7.0/PKG-INFO` & `rapids_singlecell-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapids_singlecell
-Version: 0.7.0
+Version: 0.7.1
 Summary: running single cell analysis on Nvidia GPUs
 Author: Severin Dicks
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: anndata>=0.7.4
 Requires-Dist: numpy>=1.17.0
 Requires-Dist: decoupler>=1.3.2
```

