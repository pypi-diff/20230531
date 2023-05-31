# Comparing `tmp/PyWGCNA-1.5.0.tar.gz` & `tmp/PyWGCNA-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyWGCNA-1.5.0.tar", last modified: Tue Nov  1 00:05:30 2022, max compression
+gzip compressed data, was "PyWGCNA-1.8.0.tar", last modified: Mon Nov  7 17:15:16 2022, max compression
```

## Comparing `PyWGCNA-1.5.0.tar` & `PyWGCNA-1.8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2022-11-01 00:05:30.362079 PyWGCNA-1.5.0/
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     1067 2022-01-27 20:57:46.000000 PyWGCNA-1.5.0/LICENSE.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      735 2022-11-01 00:05:30.362144 PyWGCNA-1.5.0/PKG-INFO
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2022-11-01 00:05:30.361203 PyWGCNA-1.5.0/PyWGCNA/
--rw-rw-r--   0 nargesrezaie   (501) staff       (20)      119 2022-06-20 20:33:26.000000 PyWGCNA-1.5.0/PyWGCNA/__init__.py
--rw-rw-r--   0 nargesrezaie   (501) staff       (20)     9680 2022-10-31 23:50:53.000000 PyWGCNA-1.5.0/PyWGCNA/comparison.py
--rw-rw-r--   0 nargesrezaie   (501) staff       (20)     5160 2022-10-19 22:38:51.000000 PyWGCNA-1.5.0/PyWGCNA/geneExp.py
--rw-rw-r--   0 nargesrezaie   (501) staff       (20)     5233 2022-10-31 23:12:41.000000 PyWGCNA-1.5.0/PyWGCNA/utils.py
--rw-rw-r--   0 nargesrezaie   (501) staff       (20)   180359 2022-10-31 23:24:18.000000 PyWGCNA-1.5.0/PyWGCNA/wgcna.py
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2022-11-01 00:05:30.361966 PyWGCNA-1.5.0/PyWGCNA.egg-info/
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      735 2022-11-01 00:05:30.000000 PyWGCNA-1.5.0/PyWGCNA.egg-info/PKG-INFO
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      289 2022-11-01 00:05:30.000000 PyWGCNA-1.5.0/PyWGCNA.egg-info/SOURCES.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)        1 2022-11-01 00:05:30.000000 PyWGCNA-1.5.0/PyWGCNA.egg-info/dependency_links.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      243 2022-11-01 00:05:30.000000 PyWGCNA-1.5.0/PyWGCNA.egg-info/requires.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)        8 2022-11-01 00:05:30.000000 PyWGCNA-1.5.0/PyWGCNA.egg-info/top_level.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     2012 2022-09-08 19:42:04.000000 PyWGCNA-1.5.0/README.md
--rw-r--r--   0 nargesrezaie   (501) staff       (20)       79 2022-11-01 00:05:30.362398 PyWGCNA-1.5.0/setup.cfg
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     1689 2022-11-01 00:04:58.000000 PyWGCNA-1.5.0/setup.py
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2022-11-07 17:15:16.446302 PyWGCNA-1.8.0/
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     1067 2022-01-27 20:57:46.000000 PyWGCNA-1.8.0/LICENSE.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      733 2022-11-07 17:15:16.446446 PyWGCNA-1.8.0/PKG-INFO
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2022-11-07 17:15:16.444121 PyWGCNA-1.8.0/PyWGCNA/
+-rw-rw-r--   0 nargesrezaie   (501) staff       (20)      119 2022-06-20 20:33:26.000000 PyWGCNA-1.8.0/PyWGCNA/__init__.py
+-rw-rw-r--   0 nargesrezaie   (501) staff       (20)     9680 2022-10-31 23:50:53.000000 PyWGCNA-1.8.0/PyWGCNA/comparison.py
+-rw-rw-r--   0 nargesrezaie   (501) staff       (20)     5618 2022-11-01 23:03:43.000000 PyWGCNA-1.8.0/PyWGCNA/geneExp.py
+-rw-rw-r--   0 nargesrezaie   (501) staff       (20)     5571 2022-11-01 23:44:36.000000 PyWGCNA-1.8.0/PyWGCNA/utils.py
+-rw-rw-r--   0 nargesrezaie   (501) staff       (20)   186903 2022-11-07 16:54:49.000000 PyWGCNA-1.8.0/PyWGCNA/wgcna.py
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2022-11-07 17:15:16.446134 PyWGCNA-1.8.0/PyWGCNA.egg-info/
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      733 2022-11-07 17:15:16.000000 PyWGCNA-1.8.0/PyWGCNA.egg-info/PKG-INFO
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      289 2022-11-07 17:15:16.000000 PyWGCNA-1.8.0/PyWGCNA.egg-info/SOURCES.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)        1 2022-11-07 17:15:16.000000 PyWGCNA-1.8.0/PyWGCNA.egg-info/dependency_links.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      250 2022-11-07 17:15:16.000000 PyWGCNA-1.8.0/PyWGCNA.egg-info/requires.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)        8 2022-11-07 17:15:16.000000 PyWGCNA-1.8.0/PyWGCNA.egg-info/top_level.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     2012 2022-09-08 19:42:04.000000 PyWGCNA-1.8.0/README.md
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)       79 2022-11-07 17:15:16.446881 PyWGCNA-1.8.0/setup.cfg
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     1694 2022-11-07 17:14:48.000000 PyWGCNA-1.8.0/setup.py
```

### Comparing `PyWGCNA-1.5.0/LICENSE.txt` & `PyWGCNA-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyWGCNA-1.5.0/PKG-INFO` & `PyWGCNA-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PyWGCNA
-Version: 1.5.0
+Version: 1.8.0
 Summary: PyWGCNA is a Python package designed to do Weighted correlation network analysis (WGCNA)
 Home-page: https://github.com/mortazavilab/PyWGCNA
 Author: Narges Rezaie
 Author-email: nargesrezaie80@gmail.com
 License: MIT
-Download-URL: https://github.com/mortazavilab/PyWGCNA/archive/refs/tags/v1.0.0.tar.gz
+Download-URL: https://github.com/mortazavilab/PyWGCNA/archive/refs/tags/V1.8.tar.gz
 Keywords: PyWGCNA,WGCNA,bulk,gene clustering,network analysis
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research 
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `PyWGCNA-1.5.0/PyWGCNA/comparison.py` & `PyWGCNA-1.8.0/PyWGCNA/comparison.py`

 * *Files identical despite different names*

### Comparing `PyWGCNA-1.5.0/PyWGCNA/geneExp.py` & `PyWGCNA-1.8.0/PyWGCNA/geneExp.py`

 * *Files 20% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                  sampleInfo=None):
         self.species = species
         self.level = level
         if geneExpPath is not None:
             if not os.path.isfile(geneExpPath):
                 raise ValueError("file does not exist!")
             else:
-                expressionList = pd.read_csv(geneExpPath, sep=sep)
+                expressionList = pd.read_csv(geneExpPath, sep=sep, index_col=0)
         elif geneExp is not None:
             if isinstance(geneExp, pd.DataFrame):
                 expressionList = geneExp
             else:
                 raise ValueError("geneExp is not data frame!")
         elif anndata is not None:
             if isinstance(anndata, ad.AnnData):
@@ -57,67 +57,79 @@
                 return
             else:
                 raise ValueError("geneExp is not data frame!")
         else:
             raise ValueError("all type of input can not be empty at the same time!")
 
         if geneInfo is None:
-            geneInfo = pd.DataFrame(index=expressionList.columns[1:])
+            geneInfo = pd.DataFrame(index=expressionList.columns)
 
         if sampleInfo is None:
-            sampleInfo = pd.DataFrame(index=expressionList.iloc[:, 0])
-
-        expressionList.index = expressionList.iloc[:, 0]  # sample_id
-        # drop sample id columns
-        expressionList = expressionList.drop([expressionList.columns[0]], axis=1)
+            sampleInfo = pd.DataFrame(index=expressionList.index)
 
         self.geneExpr = ad.AnnData(X=expressionList, obs=sampleInfo, var=geneInfo)
 
-    def updateGeneInfo(self, geneInfo=None, path=None, sep=','):
+    @staticmethod
+    def updateGeneInfo(geneExpr, geneInfo=None, path=None, sep=','):
         """
         add/update genes info in expr anndata
 
+        :param geneExpr: gene expression data along with sample and genes/transcript information
+        :type geneExpr: anndata
         :param geneInfo: gene information table you want to add to your data
         :type geneInfo: pandas dataframe
         :param path: path of geneInfo
         :type path: str
         :param sep: separation symbol to use for reading data in path properly (default: ',')
         :type sep: str
+
+        :return: updated gene expression data along with sample and genes/transcript information
+        :rtype: anndata
         """
         if path is not None:
             if not os.path.isfile(path):
                 raise ValueError("path does not exist!")
-            geneInfo = pd.read_csv(path, sep=sep)
+            geneInfo = pd.read_csv(path, sep=sep, index_col=0)
         elif geneInfo is not None:
             if not isinstance(geneInfo, pd.DataFrame):
                 raise ValueError("geneInfo is not pandas dataframe!")
         else:
             raise ValueError("path and geneInfo can not be empty at the same time!")
 
-        same_columns = self.geneExpr.var.columns.intersection(geneInfo.index)
-        self.geneExpr.var.drop(same_columns, axis=1, inplace=True)
-        self.geneExpr.var = pd.concat([self.geneExpr.var, geneInfo], axis=1)
+        same_columns = geneExpr.var.columns.intersection(geneInfo.columns)
+        geneExpr.var.drop(same_columns, axis=1, inplace=True)
+        geneExpr.var = pd.concat([geneExpr.var, geneInfo], axis=1).loc[geneExpr.var.index, :]
+
+        return geneExpr
 
-    def updateSampleInfo(self, sampleInfo=None, path=None, sep=','):
+    @staticmethod
+    def updateSampleInfo(geneExpr, sampleInfo=None, path=None, sep=','):
         """
         add/update metadata in expr anndata
 
+        :param geneExpr: gene expression data along with sample and genes/transcript information
+        :type geneExpr: anndata
         :param sampleInfo: Sample information table you want to add to your data
         :type sampleInfo: pandas dataframe
         :param path: path of metaData
         :type path: str
         :param sep: separation symbol to use for reading data in path properly (default: ',')
         :type sep: str
+
+        :return: updated gene expression data along with sample and genes/transcript information
+        :rtype: anndata
         """
         if path is not None:
             if not os.path.isfile(path):
                 raise ValueError("path does not exist!")
-            sampleInfo = pd.read_csv(path, sep=sep)
+            sampleInfo = pd.read_csv(path, sep=sep, index_col=0)
         elif sampleInfo is not None:
             if not isinstance(sampleInfo, pd.DataFrame):
                 raise ValueError("meta data is not pandas dataframe!")
         else:
             raise ValueError("path and metaData can not be empty at the same time!")
 
-        same_columns = self.geneExpr.obs.columns.intersection(sampleInfo.index)
-        self.geneExpr.obs.drop(same_columns, axis=1, inplace=True)
-        self.geneExpr.obs = pd.concat([self.geneExpr.var, sampleInfo], axis=1)
+        same_columns = geneExpr.obs.columns.intersection(sampleInfo.columns)
+        geneExpr.obs.drop(same_columns, axis=1, inplace=True)
+        geneExpr.obs = pd.concat([geneExpr.obs, sampleInfo], axis=1).loc[geneExpr.obs.index, :]
+
+        return geneExpr
```

### Comparing `PyWGCNA-1.5.0/PyWGCNA/utils.py` & `PyWGCNA-1.8.0/PyWGCNA/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,23 +75,26 @@
                          geneMarker=sc, sc=True)
     compare.compareNetworks()
 
     return compare
 
 
 def getGeneList(dataset='mmusculus_gene_ensembl',
-                attributes=['ensembl_gene_id', 'external_gene_name', 'gene_biotype']):
+                attributes=['ensembl_gene_id', 'external_gene_name', 'gene_biotype'],
+                maps=['gene_id', 'gene_name', 'go_id']):
     """
     get table that map gene ensembl id to gene name from biomart
 
     :param dataset: name of the dataset we used from biomart; mouse: mmusculus_gene_ensembl and human: hsapiens_gene_ensembl
         you can find more information here: https://bioconductor.riken.jp/packages/3.4/bioc/vignettes/biomaRt/inst/doc/biomaRt.html#selecting-a-biomart-database-and-dataset
     :type dataset: string
     :param attributes: List the types of data we want
     :type attributes: list
+    :param maps: mapping between attributes and column names of gene information you want to show
+    :type maps: list
     
     :return: table extracted from biomart related to the datasets including information from attributes
     :rtype: pandas dataframe
     """
 
     server = biomart.BiomartServer('http://uswest.ensembl.org/biomart')
     mart = server.datasets[dataset]
@@ -105,14 +108,20 @@
     for line in data.splitlines():
         line = line.split('\t')
         dict = {}
         for i in range(len(attributes)):
             dict[attributes[i]] = line[i]
         geneInfo = geneInfo.append(dict, ignore_index=True)
 
+    geneInfo.index = geneInfo[attributes[0]]
+    geneInfo.drop(attributes[0], axis=1, inplace=True)
+
+    if maps is not None:
+        geneInfo.columns = maps[1:]
+
     return geneInfo
 
 
 def getGeneListGOid(dataset='mmusculus_gene_ensembl',
                     attributes=['ensembl_gene_id', 'external_gene_name', 'go_id'],
                     Goid='GO:0003700'):
     """
```

### Comparing `PyWGCNA-1.5.0/PyWGCNA/wgcna.py` & `PyWGCNA-1.8.0/PyWGCNA/wgcna.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import math
+import requests
+from time import sleep
 import numpy as np
 import pandas as pd
 import scipy.stats as stats
 import statistics
 import sys
 import warnings
 from scipy.spatial.distance import pdist, squareform
@@ -257,17 +259,22 @@
 
         fig.tight_layout()
         if self.save:
             fig.savefig(f"{self.outputPath}/figures/summary_power.{self.figureType}")
 
         # Set Power
         self.adjacency = WGCNA.adjacency(self.datExpr.to_df(), power=self.power, adjacencyType=self.networkType)
+        self.adjacency = pd.DataFrame(self.adjacency,
+                                      columns=self.datExpr.to_df().columns,
+                                      index=self.datExpr.to_df().columns)
 
         # Turn adjacency into topological overlap
-        self.TOM = WGCNA.TOMsimilarity(self.adjacency, TOMType=self.TOMType)
+        self.TOM = WGCNA.TOMsimilarity(self.adjacency.to_numpy(), TOMType=self.TOMType)
+        self.TOM.columns = self.datExpr.to_df().columns
+        self.TOM.index = self.datExpr.to_df().columns
         dissTOM = 1 - self.TOM
         dissTOM = dissTOM.round(decimals=8)
 
         a = squareform(dissTOM.values, checks=False)
         # Call the hierarchical clustering function
         self.geneTree = linkage(a, method="average")
 
@@ -343,24 +350,29 @@
         :type show: bool
         """
         print(f"{BOLD}{OKBLUE}Analysing WGCNA...{ENDC}")
 
         datTraits = self.getDatTraits()
 
         print(f"{OKCYAN}Calculating module trait relationship ...{ENDC}")
-        # Define numbers of genes and samples
-        nGenes = self.datExpr.to_df().shape[1]
-        nSamples = self.datExpr.to_df().shape[0]
-        names = np.concatenate((self.MEs.columns, datTraits.columns))
-        self.moduleTraitCor = pd.DataFrame(np.corrcoef(self.MEs.T, datTraits.T),
-                                           index=names, columns=names)
-        self.moduleTraitCor = self.moduleTraitCor.iloc[0:self.MEs.shape[1], self.MEs.shape[1]:]
-        self.moduleTraitPvalue = WGCNA.corPvalue(self.moduleTraitCor, nSamples)
 
-        fig, ax = plt.subplots(figsize=(max(20, self.moduleTraitPvalue.shape[0] * 1.5),
+        self.moduleTraitCor = pd.DataFrame(index=self.MEs.columns,
+                                           columns=datTraits.columns,
+                                           dtype="float")
+        self.moduleTraitPvalue = pd.DataFrame(index=self.MEs.columns,
+                                              columns=datTraits.columns,
+                                              dtype="float")
+
+        for i in self.MEs.columns:
+            for j in datTraits.columns:
+                tmp = stats.pearsonr(self.MEs[i], datTraits[j], alternative='greater')
+                self.moduleTraitCor.loc[i, j] = tmp[0]
+                self.moduleTraitPvalue.loc[i, j] = tmp[1]
+
+        fig, ax = plt.subplots(figsize=(max(20, int(self.moduleTraitPvalue.shape[0] * 1.5)),
                                         self.moduleTraitPvalue.shape[1] * 1.5), facecolor='white')
         # names
         xlabels = []
         for label in self.MEs.columns:
             xlabels.append(label[2:].capitalize() + '(' + str(sum(self.datExpr.var['moduleColors'] == label[2:])) + ')')
         ylabels = datTraits.columns
 
@@ -391,52 +403,40 @@
 
         print(f"{OKCYAN}Adding (signed) eigengene-based connectivity (module membership) ...{ENDC}")
         self.CalculateSignedKME()
         print("\tDone..\n")
 
         if geneList is not None:
             print(f"{OKCYAN}Updating gene information based on given gene list ...{ENDC}")
-            self.updateGeneInfo(geneInfo=geneList, order=False, level=self.level)
+            self.updateGeneInfo(geneInfo=geneList)
             print("\tDone..\n")
 
+        # Select module probes
+        modules = np.unique(self.datExpr.var['moduleColors']).tolist()
+        metadata = self.datExpr.obs.columns.tolist()
+        if order is not None:
+            if all(item in metadata for item in order):
+                metadata = order
+            else:
+                sys.exit("Given order is not valid!")
+
         if self.save:
             print(f"{OKCYAN}plotting module heatmap eigengene...{ENDC}")
-            # Select module probes
-            modules = np.unique(self.datExpr.var['moduleColors']).tolist()
-            metadata = self.datExpr.obs.columns.tolist()
-            if order is None:
-                metadata.remove('sample_id')
-            else:
-                if all(item in metadata for item in order):
-                    metadata = order
-                else:
-                    sys.exit("Given order is not valid!")
             for module in modules:
                 self.plotModuleEigenGene(module, metadata, show=False)
             print("\tDone..\n")
 
         if self.save:
             print(f"{OKCYAN}plotting module barplot eigengene...{ENDC}")
-            # Select module probes
-            modules = np.unique(self.datExpr.var['moduleColors']).tolist()
-            metadata = self.datExpr.obs.columns.tolist()
-            if order is None:
-                metadata.remove('sample_id')
-            else:
-                if all(item in order for item in metadata):
-                    metadata = order
-                else:
-                    sys.exit("Given order is not valid!")
             for module in modules:
                 self.barplotModuleEigenGene(module, metadata, colorBar=metadata[-1], show=True)
             print("\tDone..\n")
 
         if self.save:
             print(f"{OKCYAN}doing Enrichr GO analysis for each module...{ENDC}")
-            modules = np.unique(self.datExpr.var['moduleColors']).tolist()
             if 'gene_name' not in self.datExpr.var.columns:
                 print(
                     f"{WARNING}\tgene name didn't found in gene information!\n\t Go term analysis can not be done{ENDC}")
             else:
                 for module in modules:
                     self.functional_enrichment_analysis(type="GO",
                                                         moduleName=module)
@@ -1092,15 +1092,15 @@
             sys.exit(("some entries are not between", min, "and", max))
 
     @staticmethod
     def TomSimilarityFromAdj(adjMat, TOMDenom, TOMType):
         # Prepare adjacency
         np.fill_diagonal(adjMat, 0)
         # Compute TOM
-        L = np.matmul(adjMat, adjMat)
+        L = adjMat @ adjMat
         ki = adjMat.sum(axis=1)
         kj = adjMat.sum(axis=0)
         if TOMDenom == 0:  # min
             MINK = np.array([np.minimum(ki_, kj) for ki_ in ki])
         else:  # mean
             MINK = np.array([((ki_ + kj) / 2) for ki_ in ki])
         if TOMType == 0:  # unsigned
@@ -1777,21 +1777,21 @@
         Sizes = pd.DataFrame(NumLabs).value_counts().sort_index()
         OrdNumLabs = pd.DataFrame({"Name": NumLabs, "Value": np.repeat(1, len(NumLabs))})
 
         if UnlabeledExist:
             if len(Sizes) > 1:
                 SizeRank = np.insert(stats.rankdata(-1 * Sizes[1:len(Sizes)], method='ordinal') + 1, 0, 1)
             else:
-                SizeRank = 1
+                SizeRank = [1]
             for i in range(len(NumLabs)):
-                OrdNumLabs.Value[i] = SizeRank[NumLabs[i]]
+                OrdNumLabs.Value[i] = SizeRank[NumLabs[i] - 1]
         else:
-            SizeRank = stats.rankdata(-1 * Sizes[0:len(Sizes)], method='ordinal')
+            SizeRank = stats.rankdata(-1 * Sizes, method='ordinal')
             for i in range(len(NumLabs)):
-                OrdNumLabs.Value[i] = SizeRank[NumLabs[i]]
+                OrdNumLabs.Value[i] = SizeRank[NumLabs[i]-1]
 
         print("\tDone..\n")
 
         OrdNumLabs.Value = OrdNumLabs.Value - UnlabeledExist
         return OrdNumLabs
 
     @staticmethod
@@ -2672,19 +2672,14 @@
                 f"{WARNING}mergeCloseModules: merging of modules failed --> returning unmerged modules and *no* "
                 f"eigengenes.\n{ENDC}")
             return {"colors": origColors, "allOK": False}
         else:
             return {"colors": MergedNewColors, "dendro": Tree, "oldDendro": oldTree, "cutHeight": cutHeight,
                     "oldMEs": oldMEs['data'], "newMEs": newMEs['data'], "allOK": True}
 
-    @staticmethod
-    def corPvalue(cor, nSamples):
-        T = np.sqrt(nSamples - 2) * (cor / np.sqrt(1 - (cor ** 2)))
-        pt = 1 - pd.DataFrame(t.cdf(np.abs(T), nSamples - 2), index=T.index, columns=T.columns)
-        return 2 * pt
 
     def saveWGCNA(self):
         """
         Saves the current WGCNA in pickle format with the .p extension
         """
         print(f"{BOLD}{OKBLUE}Saving WGCNA as {self.name}.p{ENDC}")
 
@@ -2695,29 +2690,28 @@
     def getDatTraits(self):
         """
         get data trait module base on samples information
 
         :return: a dataframe contains information in suitable format for plotting module trait relationship heatmap
         :rtype: pandas dataframe
         """
-        tmp = self.datExpr.obs.copy()
-        datTraits = pd.DataFrame(tmp.sample_id)
-        tmp.drop(['sample_id'], axis=1, inplace=True)
-        for i in range(tmp.shape[1]):
-            tmp.iloc[:, i] = tmp.iloc[:, i].astype(str)
-            if len(np.unique(tmp.iloc[:, i])) == 2:
-                datTraits[tmp.columns[i]] = tmp.iloc[:, i]
-                org = np.unique(tmp.iloc[:, i]).tolist()
+        data = self.datExpr.obs.copy()
+        datTraits = pd.DataFrame(index=data.index)
+        for i in range(data.shape[1]):
+            data.iloc[:, i] = data.iloc[:, i].astype(str)
+            if len(np.unique(data.iloc[:, i])) == 2:
+                datTraits[data.columns[i]] = data.iloc[:, i]
+                org = np.unique(data.iloc[:, i]).tolist()
                 rep = list(range(len(org)))
                 datTraits.replace(to_replace=org, value=rep,
-                                       inplace=True)
-            elif len(np.unique(tmp.iloc[:, i])) > 2:
-                for name in np.unique(tmp.iloc[:, i]):
-                    datTraits[name] = tmp.iloc[:, i]
-                    org = np.unique(tmp.iloc[:, i])
+                                  inplace=True)
+            elif len(np.unique(data.iloc[:, i])) > 2:
+                for name in np.unique(data.iloc[:, i]):
+                    datTraits[name] = data.iloc[:, i]
+                    org = np.unique(data.iloc[:, i])
                     rep = np.repeat(0, len(org))
                     rep[np.where(org == name)] = 1
                     org = org.tolist()
                     rep = rep.tolist()
                     datTraits.replace(to_replace=org, value=rep, inplace=True)
 
         return datTraits
@@ -2808,15 +2802,15 @@
 
         modules = np.unique(self.datExpr.var['moduleColors']).tolist()
         if np.all(moduleName not in modules):
             print(f"{WARNING}Module name does not exist in {ENDC}")
             return None
         else:
             heatmap = self.datExpr[:, self.datExpr.var['moduleColors'] == moduleName].to_df()
-            heatmap = (heatmap-heatmap.min(axis=0))/(heatmap.max(axis=0)-heatmap.min(axis=0))
+            heatmap = (heatmap - heatmap.min(axis=0)) / (heatmap.max(axis=0) - heatmap.min(axis=0))
             heatmap = heatmap.T
             a = pdist(heatmap)
             np.nan_to_num(a, copy=False)
             Z = WGCNA.hclust(a, method="average")
             # Clusterize the data
             labels = fcluster(Z, t=0.8, criterion='distance')
             # Keep the indices to sort labels
@@ -2866,15 +2860,15 @@
             cmap = sns.color_palette("dark:red", as_cmap=True)
             sns.heatmap(heatmap, cmap=cmap,
                         cbar=False,  # cbar_ax=axs[2,1],
                         yticklabels=False, xticklabels=False,
                         ax=axs[2, 0])
             if not show:
                 plt.close(fig)
-            fig.savefig(f"{self.outputPath}figures/module_heatmap_eigengene_{moduleName}.{self.figureType}")
+            fig.savefig(f"{self.outputPath}/figures/module_heatmap_eigengene_{moduleName}.{self.figureType}")
 
         return None
 
     def barplotModuleEigenGene(self, moduleName, metadata, combine=True, colorBar=None, show=True):
         """
         bar plot of module eigen gene figure in given module
 
@@ -2973,15 +2967,15 @@
                 axs[1, 0].errorbar(ind, ybar, yerr=ebar, fmt="o", color="r")
                 axs[1, 0].scatter(xdot, ydot, c='black', alpha=0.5)
                 axs[1, 0].set_xticks(np.arange(len(ind)))
                 axs[1, 0].set_xticklabels(label, rotation=90)
                 axs[1, 0].set_ylabel('eigengeneExp')
                 axs[1, 0].set_facecolor('white')
                 fig.subplots_adjust(bottom=0.3)
-                fig.savefig(f"{self.outputPath}figures/module_barplot_eigengene_{moduleName}.{self.figureType}")
+                fig.savefig(f"{self.outputPath}/figures/module_barplot_eigengene_{moduleName}.{self.figureType}")
                 if not show:
                     plt.close(fig)
 
             else:
                 fig, axs = plt.subplots(nrows=1, ncols=len(metadata), figsize=(5 * len(metadata), 5))
 
                 for i in range(len(metadata)):
@@ -2989,34 +2983,39 @@
                     df[metadata[i]] = sampleInfo[metadata[i]].values
                     palette = self.metadataColors[metadata[i]]
                     bar = sns.barplot(x=metadata[i], y="eigengeneExp", data=df, palette=palette, ci='sd', capsize=0.1,
                                       ax=axs[i])
                     if i != 0:
                         bar.set(ylabel=None)
 
-                fig.savefig(f"{self.outputPath}figures/module_barplot_eigengene_{moduleName}.{self.figureType}")
+                fig.savefig(f"{self.outputPath}/figures/module_barplot_eigengene_{moduleName}.{self.figureType}")
                 if not show:
                     plt.close(fig)
 
-    def functional_enrichment_analysis(self, type, moduleName, sets=None, p_value=0.05):
+    def functional_enrichment_analysis(self, type, moduleName, sets=None, p_value=0.05, file_name=None):
         """
         Doing functional enrichment analysis including GO, KEGG and REACTOME
 
         :param type: indicate the type of databases which it should be one of "GO", "KEGG", "REACTOME"
         :type type: str
         :param moduleName: module name
         :type moduleName: str
         :param sets: str, list, tuple of Enrichr Library name(s). or custom defined gene_sets (dict, or gmt file) (you can add any Enrichr Libraries from here: https://maayanlab.cloud/Enrichr/#stats) only need to fill if the type is GO or KEGG
         :type sets: str, list, tuple
         :param p_value: Defines the pValue threshold. (default: 0.05)
         :type p_value: float
+        :param file_name: name of the file you want to use to save plot (default is moduleName)
+        :type file_name: str
         """
         if type not in ["GO", "KEGG", "REACTOME"]:
             sys.exit("Type is not valid! it should be one of them GO, KEGG, REACTOME")
 
+        if file_name is None:
+            file_name = moduleName
+
         modules = np.unique(self.datExpr.var['moduleColors']).tolist()
         if np.all(moduleName not in modules):
             print(f"{WARNING}Module name does not exist in {ENDC}")
             return
 
         if not os.path.exists(f"{self.outputPath}/figures/{type}"):
             print(f"{WARNING}{type} directory does not exist!\nCreating {type} directory!{ENDC}")
@@ -3030,68 +3029,71 @@
         geneModule = self.datExpr.var.gene_name[self.datExpr.var.moduleColors == moduleName]
         geneModule = geneModule.fillna("").values.tolist()
         if type in ["GO", "KEGG"]:
             enr = gp.enrichr(gene_list=geneModule,
                              gene_sets=sets,
                              organism=self.species,
                              description='',
-                             outdir=f"{self.outputPath}/figures/{type}/{moduleName}",
+                             outdir=f"{self.outputPath}/figures/{type}/{file_name}",
                              cutoff=p_value)
             dotplot(enr.res2d,
                     title=f"Gene ontology in {moduleName} module with {sum(self.datExpr.var['moduleColors'] == moduleName)} genes",
                     cmap='viridis_r',
                     cutoff=p_value,
-                    ofname=f"{self.outputPath}/figures/{type}/{moduleName}.{self.figureType}")
+                    ofname=f"{self.outputPath}/figures/{type}/{file_name}.{self.figureType}")
         else:
+            numGeneModule = len(geneModule)
             geneModule = ",".join(geneModule)
             result = analysis.identifiers(ids=geneModule,
                                           species=self.species,
-                                          p_value=p_value)
+                                          p_value=str(p_value))
             token = result['summary']['token']
             analysis.report(token,
-                            path=f"{self.outputPath}/figures/{type}",
-                            file=f"{moduleName}.{self.figureType}",
+                            path=f"{self.outputPath}/figures/{type}/",
+                            file=f"{file_name}.{self.figureType}",
                             number='50',
                             species=self.species)
+            token_result = analysis.token(token,
+                                          species=self.species,
+                                          p_value=str(p_value))
+
+            print(f"{numGeneModule - token_result['identifiersNotFound']} out of {numGeneModule} identifiers in the sample were found in Reactome.")
+            print(f"{token_result['resourceSummary'][0]['pathways']} pathways were hit by at least one of them, which {len(token_result['pathways'])} of them have p-value more than {p_value}.")
+            print(f"Report was saved {self.outputPath}/figures/{type}/{file_name}.{self.figureType}!")
+            print(f"For more information please visit https://reactome.org/PathwayBrowser/#/DTAB=AN&ANALYSIS={token}")
 
-    def updateGeneInfo(self, geneInfo=None, path=None, sep=' ', order=True, level='gene'):
+    def updateGeneInfo(self, geneInfo=None, path=None, sep=','):
         """
         add/update genes info in datExpr and geneExpr anndata
 
         :param geneInfo: gene information table you want to add to your data
         :type geneInfo: pandas dataframe
         :param path: path of geneInfo
         :type path: str
-        :param sep: separation symbol to use for reading data in path properly
+        :param sep: separation symbol to use for reading data in path properly (default: ",")
         :type sep: str
-        :param order: if you want to update/add gene information by keeping the order as the same as data. if you want to add gene infor from biomart you should set this to be false. (default: TRUE)
-        :type order: bool
-        :param level: indicated the expression data is at gene level or transcript level
-        :type level: str
         """
 
-        self.geneExpr = GeneExp.updateGeneInfo(self.geneExpr, geneInfo, path, sep, order, level)
-        self.datExpr = GeneExp.updateGeneInfo(self.datExpr, geneInfo, path, sep, order, level)
+        self.geneExpr = GeneExp.updateGeneInfo(self.geneExpr, geneInfo, path, sep)
+        self.datExpr = GeneExp.updateGeneInfo(self.datExpr, geneInfo, path, sep)
 
-    def updateMetadata(self, metaData=None, path=None, sep=' ', order=True):
+    def updateSampleInfo(self, sampleInfo=None, path=None, sep=','):
         """
         add/update metadata in datExpr and geneExpr anndata
 
-        :param metaData: Sample information table you want to add to your data
-        :type metaData: pandas dataframe
+        :param sampleInfo: Sample information table you want to add to your data
+        :type sampleInfo: pandas dataframe
         :param path: path of metaData
         :type path: str
-        :param sep: separation symbol to use for reading data in path properly
+        :param sep: separation symbol to use for reading data in path properly (default: ",")
         :type sep: str
-        :param order: if you want to update/add gene information by keeping the order as the same as data. if you want to add gene infor from biomart you should set this to be false. (default: TRUE)
-        :type order: bool
         """
 
-        self.geneExpr = GeneExp.updateMetadata(self.geneExpr, metaData, path, sep, order)
-        self.datExpr = GeneExp.updateMetadata(self.datExpr, metaData, path, sep, order)
+        self.geneExpr = GeneExp.updateSampleInfo(self.geneExpr, sampleInfo, path, sep)
+        self.datExpr = GeneExp.updateSampleInfo(self.datExpr, sampleInfo, path, sep)
 
     @staticmethod
     def softConnectivity(datExpr, corOptions=pd.DataFrame(), weights=None, type="unsigned", power=6, blockSize=1500,
                          minNSamples=None):
         """
         Given expression data or a similarity, the function constructs the adjacency matrix and for each node calculates its connectivity, that is the sum of the adjacency to the other nodes.
 
@@ -3236,81 +3238,241 @@
 
         output = np.corrcoef(datExpr.T, datME.T)
         tmp = len(datME.columns)
         col = ["k" + datME.columns[i] for i in range(tmp)]
         self.signedKME = pd.DataFrame(output[0:datExpr.shape[1], datExpr.shape[1]:],
                                       index=datExpr.columns, columns=col)
 
-    def CoexpressionModulePlot(self, module, numGenes=10, numConnections=100, minTOM=0, filters=None):
+    def CoexpressionModulePlot(self, modules, numGenes=10, numConnections=100, minTOM=0, filters=None, file_name=None):
         """
         plot Coexpression for given module
 
-        :param module: name of modules you like to plot
-        :type module: str
-        :param numGenes: number of genes you want to show
+        :param modules: name of modules you like to plot
+        :type modules: list of str
+        :param numGenes: number of genes you want to show for each module
         :type numGenes: int
-        :param numConnections: number of connection you want to show
+        :param numConnections: number of connection you want to show for each module
         :type numConnections: int
         :param minTOM: minimum TOM to keep connections
         :type minTOM: float
         :param filters: Dictionary which keys are columns names of datExpr.var that you want to filter the genes based on it and values are determining which rows you want to keep
         :type filters: dict
+        :param file_name: name of the html output file (default: module names or network if there is more than 3 modules for input)
+        :type file_name: str
 
         :return: save a html file with name of modules in figures directory
         """
         if self.signedKME is None:
-            print("signedKME is empty! call signedKME() to calcuate it")
+            print("signedKME is empty! call signedKME() to calculate it")
 
-        if not os.path.exists(self.outputPath + '/figures/network/'):
+        if not os.path.exists(f"{self.outputPath}/figures/network/"):
             print(f"{WARNING}Network directory does not exist!\nCreating network directory!{ENDC}")
-            os.makedirs(self.outputPath + '/figures/network/')
+            os.makedirs(f"{self.outputPath}/figures/network/")
 
-        name = 'gene_id'
-        name_biotype = 'gene_biotype'
-        if self.level == 'transcript':
-            name = 'transcript_id'
-            name_biotype = 'transcript_biotype'
-        gene_id = self.datExpr.var.loc[self.datExpr.var.moduleColors == module, :]
+        gene_id = self.datExpr.var.loc[self.datExpr.var.moduleColors.isin(modules), :]
+        if gene_id.shape[0] == 0:
+            sys.exit(f"There is no gene assign to {','.join(modules)} module(s)!")
         if filters is not None:
             for key in filters.keys():
                 gene_id = gene_id.loc[gene_id[key].isin(filters[key]), :]
-        gene_id[name] = gene_id[name].str.split('\\.', expand=True)[0]
-        gene_id = gene_id[name]
-        if len(gene_id) < numGenes:
-            numGenes = len(gene_id)
+        if gene_id.shape[0] < numGenes:
+            numGenes = gene_id.shape[0]
             numConnections = numGenes * (numGenes - 1)
+        genes = []
+        for module in modules:
+            mat = self.signedKME.loc[gene_id.index].sort_values(["kME" + module], ascending=False)
+            mat = mat.iloc[:numGenes, :]
+            genes = genes + mat.index.tolist()
 
-        self.signedKME.index.name = None
-        index = self.signedKME.reset_index(inplace=False)
-        index = index['index'].str.split('\\.', expand=True)[0]
-        self.signedKME.index = index
-        self.signedKME.index.name = None
-
-        mat = self.signedKME.loc[gene_id].sort_values(["kME" + module], ascending=False)
-        mat = mat.iloc[:numGenes, :]
-
-        self.TOM.columns = self.datExpr.to_df().columns
-        self.TOM.index = self.datExpr.to_df().columns
-        adj = self.TOM.loc[mat.index, mat.index]
+        adj = self.TOM.loc[genes, genes]
         adj[adj < minTOM] = 0
         adj = adj.where(np.triu(np.ones(adj.shape)).astype(np.bool))
         adj = adj.where(adj.values != np.diag(adj), 0,
                         adj.where(adj.values != np.flipud(adj).diagonal(0), 0, inplace=True))
         adj = adj.stack().nlargest(numConnections)
 
         net = Network()
         gene_id = list(adj.index.get_level_values(0)) + list(adj.index.get_level_values(1))
         gene_id = np.unique(gene_id)
-        nodes = self.datExpr.var.loc[gene_id,]
-        title = name + ":" + nodes[name] + "\n" + name_biotype + ":" + nodes[name_biotype]
-        net.add_nodes(list(nodes[name]),
+        nodes = self.datExpr.var.loc[gene_id, :]
+        node_color = nodes["moduleColors"].tolist()
+        nodes.drop(["dynamicColors", "moduleColors", "moduleLabels"], axis=1, inplace=True)
+        title = nodes.index.tolist()
+        for i in range(nodes.shape[0]):
+            for j in range(nodes.shape[1]):
+                if not pd.isna(nodes.iloc[i, j]):
+                    title[i] = title[i] + "\n" + str(nodes.columns[j]) + ": " + str(nodes.iloc[i, j])
+
+        net.add_nodes(nodes.index.tolist(),
                       title=title,
-                      label=list(nodes.gene_name),
-                      color=[module] * numGenes)
+                      label=nodes.index.tolist(),
+                      color=node_color)
 
         for i in range(len(adj)):
             if adj[i] != 0:
                 net.add_edge(adj.index.get_level_values(0)[i],
                              adj.index.get_level_values(1)[i],
                              weight=adj[i])
 
-        net.show(self.outputPath + '/figures/network/' + module + '.html')
+        if file_name is None:
+            if len(modules) <= 3:
+                file_name = '_'.join(modules)
+            else:
+                file_name = "network"
+        net.show(f"{self.outputPath}/figures/network/{file_name}.html")
+
+    def PPI_network(self, species, moduleName=None, geneList=None, output_format="image"):
+        """
+        retrieve an image of a STRING network of a neighborhood surrounding one or more proteins or ask STRING to show only the network of interactions between your input proteins.
+
+        :param species: NCBI taxon identifiers (e.g. Human is 9606, see: https://string-db.org/cgi/input.pl?input_page_active_form=organisms).
+        :type species: int
+        :param moduleName: name of module you want to find PPI
+        :type moduleName: str
+        :param geneList: list of genes you want to find PPI
+        :type geneList: list
+        :param output_format: format of output which can be "image", "highres_image", "svg" (default: "image")
+        :type output_format: str
+
+        :return: dataframe contains genes along with interaction with their scores
+        :rtype: pandas dataframe
+        """
+
+        if moduleName is not None:
+            genes = self.datExpr.var[self.datExpr.var.moduleColors == moduleName]
+            geneList = genes.index.astype(str).tolist()
+        elif geneList is None:
+            sys.exit("geneList or moduleName should be empty at the same time!")
+
+        if not os.path.exists(f"{self.outputPath}/figures/PPI/"):
+            print(f"{WARNING}PPI directory does not exist!\nCreating PPI directory!{ENDC}")
+            os.makedirs(f"{self.outputPath}/figures/PPI/")
+
+        res = WGCNA.request_PPI(genes=geneList, species=species)
+        res.sort_values(by=["gene1"], axis=0, inplace=True)
+
+        string_api_url = "https://version-11-5.string-db.org/api"
+        method = "network"
+
+        request_url = "/".join([string_api_url, output_format, method])
+
+        for gene in res.gene1.unique():
+            tmp = res[res.gene1 == gene]
+            genes = tmp.gene2.tolist()
+            genes.append(tmp.gene1.tolist()[0])
+            params = {
+                "identifiers": "\r".join(genes),  # your protein
+                "species": species,  # species NCBI identifier
+                "add_white_nodes": 15,  # add 15 white nodes to my protein
+                "network_flavor": "confidence",  # show confidence links
+                "caller_identity": "www.awesome_app.org"  # your app name
+
+            }
+            WGCNA.request_PPI_image(params=params,
+                                    genes=genes,
+                                    file_name=f"{self.outputPath}/figures/PPI/{tmp.gene1.tolist()[0]}_PPI.png",
+                                    request_url=request_url)
+        return res
+
+    @staticmethod
+    def request_PPI_subset(params,
+                           request_url='https://version-11-5.string-db.org/api/tsv-no-header/interaction_partners'):
+        """
+        request STRING to find genes interact with our gene list base
+
+        :param request_url: suitable url for using STRING API
+        :type request_url: str
+        :param params: parameters for requesting
+        :type params: dict
+
+        :return: dataframe contains genes interact with each other
+        :rtype: pandas dataframe
+        """
+        response = requests.post(request_url, data=params)
+
+        res = pd.DataFrame(columns=["gene1", "gene2", "score"])
+        if response.status_code == 200:
+            for line in response.text.strip().split("\n"):
+                l = line.strip().split("\t")
+
+                res = res.append({'gene1': l[2], 'gene2': l[3], 'score': l[5]},
+                                 ignore_index=True)
+
+        sleep(1)
+
+        return res
+
+    @staticmethod
+    def request_PPI(genes,
+                    species):
+        """
+        Getting all the STRING interaction partners of the protein set
+
+        :param genes: list of genes you want to find interaction for
+        :type genes: list
+        :param species: NCBI taxon identifiers (e.g. Human is 9606, see: https://string-db.org/cgi/input.pl?input_page_active_form=organisms).
+        :type species: int
+
+        :return: dataframe contains genes interact with each other
+        :rtype: pandas dataframe
+        """
+
+        string_api_url = "https://version-11-5.string-db.org/api"
+        output_format = "tsv-no-header"
+        method = "interaction_partners"
+
+        request_url = "/".join([string_api_url, output_format, method])
+
+        count = 0
+        res = pd.DataFrame(columns=["gene1", "gene2", "score"])
+        while count < len(genes):
+
+            if count + 2000 > len(genes):
+                my_genes = genes[count:]
+            else:
+                my_genes = genes[count:count + 2000]
+
+            params = {
+                "identifiers": "%0d".join(my_genes),  # your protein
+                "species": species,  # species NCBI identifier
+                "limit": 5,
+                "caller_identity": "www.awesome_app.org"  # your app name
+            }
+
+            tmp = WGCNA.request_PPI_subset(params, request_url)
+            count = count + 2000
+            res = pd.concat([res, tmp], ignore_index=True)
+
+        print(f"{len(res.gene1.unique().tolist())} genes out of {len(genes)} genes have PPI.")
+        return res
+
+    @staticmethod
+    def request_PPI_image(params,
+                          genes,
+                          file_name,
+                          request_url='https://version-11-5.string-db.org/api/image/network'):
+        """
+        plot PPI interaction along with link that direct you to the STRING webpage
+
+        :param params: parameters for requesting
+        :type params: dict
+        :param genes: list of genes you want to find interaction for
+        :type genes: list
+        :param file_name: name of the output file
+        :type file_name: str
+        :param request_url: suitable url for using STRING API
+        :type request_url: str
+
+        """
+        response = requests.post(request_url, data=params)
+
+        if response.status_code == 200:
+            print("Saving interaction network to %s" % file_name)
+
+            with open(file_name, 'wb') as fh:
+                fh.write(response.content)
+
+            print("For having interactive network, click line below:")
+            tmp = "%0d".join(genes)
+            print(f"https://string-db.org/api/tsv/get_link?identifiers={tmp}&species={params['species']}")
+
+        sleep(1)
```

### Comparing `PyWGCNA-1.5.0/PyWGCNA.egg-info/PKG-INFO` & `PyWGCNA-1.8.0/PyWGCNA.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PyWGCNA
-Version: 1.5.0
+Version: 1.8.0
 Summary: PyWGCNA is a Python package designed to do Weighted correlation network analysis (WGCNA)
 Home-page: https://github.com/mortazavilab/PyWGCNA
 Author: Narges Rezaie
 Author-email: nargesrezaie80@gmail.com
 License: MIT
-Download-URL: https://github.com/mortazavilab/PyWGCNA/archive/refs/tags/v1.0.0.tar.gz
+Download-URL: https://github.com/mortazavilab/PyWGCNA/archive/refs/tags/V1.8.tar.gz
 Keywords: PyWGCNA,WGCNA,bulk,gene clustering,network analysis
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research 
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `PyWGCNA-1.5.0/README.md` & `PyWGCNA-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `PyWGCNA-1.5.0/setup.py` & `PyWGCNA-1.8.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from setuptools import setup
 
 setup(
     name='PyWGCNA',  # the name of your package
     packages=['PyWGCNA'],  # same as above
-    version='v1.5.0',  # version number
+    version='v1.8.0',  # version number
     license='MIT',  # license type
     description='PyWGCNA is a Python package designed to do Weighted correlation network analysis (WGCNA)',
     # short description
     author='Narges Rezaie',  # your name
     author_email='nargesrezaie80@gmail.com',  # your email
     url='https://github.com/mortazavilab/PyWGCNA',  # url to your git repo
-    download_url='https://github.com/mortazavilab/PyWGCNA/archive/refs/tags/v1.0.0.tar.gz',  # link to the tar.gz file associated with this release
+    download_url='https://github.com/mortazavilab/PyWGCNA/archive/refs/tags/V1.8.tar.gz',  # link to the tar.gz file associated with this release
     keywords=['PyWGCNA', 'WGCNA', 'bulk', 'gene clustering', 'network analysis'],  #
     install_requires=[  # these can also include >, <, == to enforce version compatibility
-        'pandas>=1.5.0',  # make sure the packages you put here are those NOT included in the
+        'pandas>=1.3.5',  # make sure the packages you put here are those NOT included in the
         'numpy>=1.21.2',  # base python distribution
-        'scipy>=1.9.1',
-        'scikit-learn>=1.1.2',
+        'scipy>=1.9.3',
+        'scikit-learn>=1.1.3',
         'statsmodels>=0.12.2',
         'matplotlib>=3.4.2',
         'seaborn>=0.11.1',
         'biomart>=0.9.2',
         'gseapy>=0.10.5',
         'pytest',
         'pyvis>=0.1.9',
-        'setuptools>=58.0.4',
-        'biomart',
+        'setuptools>=59.8.0',
+        'biomart>=0.9.2',
         'reactome2py>=3.0.0',
         'anndata>=0.8.0',
-        'resources>=0.0.1',
+        'requests>=2.28.1',
     ],
     classifiers=[  # choose from here: https://pypi.org/classifiers/
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research ',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
```

