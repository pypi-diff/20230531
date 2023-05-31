# Comparing `tmp/SC2Spa-1.1.8.tar.gz` & `tmp/SC2Spa-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SC2Spa-1.1.8.tar", last modified: Tue May 16 15:37:48 2023, max compression
+gzip compressed data, was "SC2Spa-1.1.9.tar", last modified: Wed May 31 14:12:29 2023, max compression
```

## Comparing `SC2Spa-1.1.8.tar` & `SC2Spa-1.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 15:37:48.425156 SC2Spa-1.1.8/
--rwxrwxrwx   0 root         (0) root         (0)     1525 2022-11-18 16:54:51.000000 SC2Spa-1.1.8/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     1359 2023-05-16 15:37:48.424332 SC2Spa-1.1.8/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      806 2023-01-09 13:31:30.000000 SC2Spa-1.1.8/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 15:37:48.418051 SC2Spa-1.1.8/SC2Spa/
--rwxrwxrwx   0 root         (0) root         (0)    12963 2023-02-13 15:19:44.000000 SC2Spa-1.1.8/SC2Spa/BM.py
--rwxrwxrwx   0 root         (0) root         (0)     8248 2022-12-06 20:19:48.000000 SC2Spa-1.1.8/SC2Spa/ME.py
--rwxrwxrwx   0 root         (0) root         (0)     3062 2022-07-12 15:41:45.000000 SC2Spa-1.1.8/SC2Spa/PP.py
--rwxrwxrwx   0 root         (0) root         (0)    50180 2023-05-16 15:34:39.000000 SC2Spa-1.1.8/SC2Spa/SI.py
--rwxrwxrwx   0 root         (0) root         (0)     4381 2023-01-08 16:28:45.000000 SC2Spa-1.1.8/SC2Spa/SVA.py
--rwxrwxrwx   0 root         (0) root         (0)    21673 2023-05-15 15:40:00.000000 SC2Spa-1.1.8/SC2Spa/Vis.py
--rwxrwxrwx   0 root         (0) root         (0)      211 2023-03-14 16:25:06.000000 SC2Spa-1.1.8/SC2Spa/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      460 2023-03-14 16:25:06.000000 SC2Spa-1.1.8/SC2Spa/__metadata__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 15:37:48.422930 SC2Spa-1.1.8/SC2Spa.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     1359 2023-05-16 15:37:48.000000 SC2Spa-1.1.8/SC2Spa.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      274 2023-05-16 15:37:48.000000 SC2Spa-1.1.8/SC2Spa.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-16 15:37:48.000000 SC2Spa-1.1.8/SC2Spa.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        7 2023-05-16 15:37:48.000000 SC2Spa-1.1.8/SC2Spa.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      691 2023-05-16 15:37:34.000000 SC2Spa-1.1.8/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-16 15:37:48.425436 SC2Spa-1.1.8/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 14:12:29.716720 SC2Spa-1.1.9/
+-rwxrwxrwx   0 root         (0) root         (0)     1525 2022-11-18 16:54:51.000000 SC2Spa-1.1.9/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     1359 2023-05-31 14:12:29.716263 SC2Spa-1.1.9/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      806 2023-01-09 13:31:30.000000 SC2Spa-1.1.9/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 14:12:29.712256 SC2Spa-1.1.9/SC2Spa/
+-rwxrwxrwx   0 root         (0) root         (0)    12963 2023-02-13 15:19:44.000000 SC2Spa-1.1.9/SC2Spa/BM.py
+-rwxrwxrwx   0 root         (0) root         (0)     8248 2022-12-06 20:19:48.000000 SC2Spa-1.1.9/SC2Spa/ME.py
+-rwxrwxrwx   0 root         (0) root         (0)     3062 2022-07-12 15:41:45.000000 SC2Spa-1.1.9/SC2Spa/PP.py
+-rwxrwxrwx   0 root         (0) root         (0)    50542 2023-05-31 14:09:58.000000 SC2Spa-1.1.9/SC2Spa/SI.py
+-rwxrwxrwx   0 root         (0) root         (0)     4381 2023-01-08 16:28:45.000000 SC2Spa-1.1.9/SC2Spa/SVA.py
+-rwxrwxrwx   0 root         (0) root         (0)    21739 2023-05-30 12:11:12.000000 SC2Spa-1.1.9/SC2Spa/Vis.py
+-rwxrwxrwx   0 root         (0) root         (0)      211 2023-03-14 16:25:06.000000 SC2Spa-1.1.9/SC2Spa/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      460 2023-03-14 16:25:06.000000 SC2Spa-1.1.9/SC2Spa/__metadata__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-31 14:12:29.715349 SC2Spa-1.1.9/SC2Spa.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1359 2023-05-31 14:12:29.000000 SC2Spa-1.1.9/SC2Spa.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      274 2023-05-31 14:12:29.000000 SC2Spa-1.1.9/SC2Spa.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-05-31 14:12:29.000000 SC2Spa-1.1.9/SC2Spa.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)        7 2023-05-31 14:12:29.000000 SC2Spa-1.1.9/SC2Spa.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      691 2023-05-31 14:12:04.000000 SC2Spa-1.1.9/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-05-31 14:12:29.716895 SC2Spa-1.1.9/setup.cfg
```

### Comparing `SC2Spa-1.1.8/LICENSE` & `SC2Spa-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.1.8/PKG-INFO` & `SC2Spa-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SC2Spa
-Version: 1.1.8
+Version: 1.1.9
 Summary: SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution
 Author-email: "Linbu Liao, Won Lab" <linbu.liao@gmail.com>
 Project-URL: Homepage, https://github.com/linbuliao/SC2Spa
 Project-URL: Bug Tracker, https://github.com/pypa/SC2Spa/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `SC2Spa-1.1.8/README.md` & `SC2Spa-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.1.8/SC2Spa/BM.py` & `SC2Spa-1.1.9/SC2Spa/BM.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.1.8/SC2Spa/ME.py` & `SC2Spa-1.1.9/SC2Spa/ME.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.1.8/SC2Spa/PP.py` & `SC2Spa-1.1.9/SC2Spa/PP.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.1.8/SC2Spa/SI.py` & `SC2Spa-1.1.9/SC2Spa/SI.py`

 * *Files 1% similar despite different names*

```diff
@@ -691,16 +691,16 @@
     # Calculate cells' distance to the closest ST bead
     dis_sc[neighbors_sc >= n_ST] = 1e6
     dis_sc[:, 0] = 1e6
     adata_query.obs['Dis2ClosestBead'] = dis_sc.min(axis=1)
 
     #Label closest ST beads of single cells
     adata_query.obs['ClosestBead_order'] = neighbors_sc[range(neighbors_sc.shape[0]),
-    dis_sc.argmin(axis=1)]
-    adata_query.obs['ClosestBead_name'] = adata_ref.obs_names[adata_query.obs['ClosestBead_order']]
+                                                        dis_sc.argmin(axis=1)]
+    adata_query.obs['ClosestBead_name'] = adata_query.obs['ClosestBead_order'].apply(lambda x: adata_ref.obs_names[x] if x < n_ST else 'NA')
 
     #Label closest single cells of ST beads
     # ClosestSC_list = adata_query.groupby('ClosestBead_name', as_index = False)['Dis2ClosestBead'].idxmin()['Dis2ClosestBead'].tolist()
     ClosestSC_list = adata_query.obs.reset_index().groupby('ClosestBead_name', as_index=False).agg(
         {'Dis2ClosestBead': 'min', 'index': 'first'})['index'].tolist()
     adata_query.obs['ClosestSC'] = False
     adata_query.obs.loc[ClosestSC_list, 'ClosestSC'] = True
@@ -907,15 +907,16 @@
         Reference anndata object. Gene expression matrix should be the shape of (cell, gene).
         Predicted locations should be stored in adata_ref.obs[['x_transfer', 'y_transfer']]
     adata_query
         Query anndata object. Gene expression matrix should be the shape of (cell, gene).
         Cell type annotation should be stored in adata_query.obs[ct_name]
         Predicted locations should be stored in adata_query.obs[['x_transfer', 'y_transfer']]
     weight_constant
-        A constant added up to the distance.
+        A constant added up to the distance between a cell and a ST voxel when calculating
+        the weight of the cell to the ST voxel.
 
     Returns
     -------
     df_neighbor
         A dataframe that contains the cell type information and normalized reciprocal distance
          of mapped ST beads and single cells
 
@@ -935,15 +936,16 @@
     df_neighbor['SCT'] = adata_query.obs.iloc[df_neighbor['neighbor'] - n_ST][ct_name].tolist()
 
     df_neighbor['weight'] = 1 / (df_neighbor['dis'] + weight_constant)
 
     return df_neighbor
 
 
-def NRD_CT(neighbors, dis, adata_ref, adata_query, ct_name='simp_name', weight_constant = 1, exclude_CTs=['nan']):
+def NRD_CT(neighbors, dis, adata_ref, adata_query, ct_name='simp_name', weight_constant = 1,
+           exclude_CTs=['nan']):
 
     '''
     Normalized Reciprocal Distance
     Calculate the proportion of cell types for ST beads based on the NRD_weight output
     Predicted cell type proportion will be saved in adata_ref.obs.
 
     Parameters
@@ -959,14 +961,17 @@
         Query anndata object. Gene expression matrix should be the shape of (cell, gene).
         Cell type annotation should be stored in adata_query.obs[ct_name]
         Predicted locations should be stored in adata_query.obs[['x_transfer', 'y_transfer']]
     dis_min
         Distance cutoff that determines if a ST bead and a single cell is paired
     exclude_CTs
         A list that contains cell types to be excluded
+    weight_constant
+        A constant added up to the distance between a cell and a ST voxel when calculating
+        the weight of the cell to the ST voxel.
 
     Returns
     -------
     None
 
     '''
```

### Comparing `SC2Spa-1.1.8/SC2Spa/SVA.py` & `SC2Spa-1.1.9/SC2Spa/SVA.py`

 * *Files identical despite different names*

### Comparing `SC2Spa-1.1.8/SC2Spa/Vis.py` & `SC2Spa-1.1.9/SC2Spa/Vis.py`

 * *Files 2% similar despite different names*

```diff
@@ -439,16 +439,16 @@
     adata
         anndata file.
         Cell type information should be stored in `adata.obs[c_name]
         Fine mapping result should be stored in `adata.obs['FM']` if `FM==True`
         Coordinate Information should be stored in `adata.obsm[coords_name]`
         Reconstruction info should be stored in adata.obs['Recon_scST']
     CT_list
-        A list that contains the cell types to be shown. the cell types must
-        exist in `adata.obs[c_name]`
+        A list that contains the cell types to be shown. The cell types must
+        be in `adata.obs[c_name]`
     c_name
         Name of cell type column in adata.obs
     s
         size of beads in the figure
     legend
         Draw legend in the figure if True
 
@@ -485,28 +485,32 @@
     plt.grid(False)
     plt.axis('off')
 
     if (legend):
         plt.legend(handles=scatter.legend_elements()[0],
                    labels=cts)
 
-    if ((save != None)):
+    if (save != None):
 
         if not os.path.exists(root):
             os.makedirs(root)
         plt.savefig(root + save + '.png',
                     dpi=128, bbox_inches='tight')
     plt.show()
 
     ##Extract handles
     handles = scatter.legend_elements()[0]
 
     plt.legend(handles=scatter.legend_elements()[0],
                labels=cts)
-    plt.savefig(root + save + '_legend.png', bbox_inches='tight')
+    plt.grid(False)
+    plt.axis('off')
+
+    if(save != None):
+        plt.savefig(root + save + '_legend.png', bbox_inches='tight')
 
     plt.show()
 
 
 def Superimpose(adata:anndata.AnnData, coords_name='spatial', G1='APOE', G2='NRGN',
                 s = 2, C1 = 'Reds', C2 = 'Blues', figsize = (10, 10),
                 alpha1=0.5, alpha2=0.7, save_root = 'figures/BME/', save=True):
```

### Comparing `SC2Spa-1.1.8/SC2Spa.egg-info/PKG-INFO` & `SC2Spa-1.1.9/SC2Spa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SC2Spa
-Version: 1.1.8
+Version: 1.1.9
 Summary: SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution
 Author-email: "Linbu Liao, Won Lab" <linbu.liao@gmail.com>
 Project-URL: Homepage, https://github.com/linbuliao/SC2Spa
 Project-URL: Bug Tracker, https://github.com/pypa/SC2Spa/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `SC2Spa-1.1.8/pyproject.toml` & `SC2Spa-1.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SC2Spa"
-version = "1.1.8"
+version = "1.1.9"
 authors = [
   { name="Linbu Liao, Won Lab", email="linbu.liao@gmail.com" },
 ]
 description = "SC2Spa: a deep learning based approach to map transcriptome to spatial origins at cellular resolution"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

