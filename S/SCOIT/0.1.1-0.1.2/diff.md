# Comparing `tmp/SCOIT-0.1.1.tar.gz` & `tmp/SCOIT-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SCOIT-0.1.1.tar", last modified: Wed Apr 26 03:57:28 2023, max compression
+gzip compressed data, was "dist/SCOIT-0.1.2.tar", last modified: Wed May 31 13:46:54 2023, max compression
```

## Comparing `SCOIT-0.1.1.tar` & `SCOIT-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 wangruohan   (501) staff       (20)        0 2023-04-26 03:57:28.307657 SCOIT-0.1.1/
--rw-r--r--   0 wangruohan   (501) staff       (20)     1070 2022-07-29 09:06:11.000000 SCOIT-0.1.1/LICENSE
--rw-r--r--   0 wangruohan   (501) staff       (20)     6585 2023-04-26 03:57:28.307312 SCOIT-0.1.1/PKG-INFO
--rw-r--r--   0 wangruohan   (501) staff       (20)     6044 2023-04-26 03:46:00.000000 SCOIT-0.1.1/README.md
-drwxr-xr-x   0 wangruohan   (501) staff       (20)        0 2023-04-26 03:57:28.301508 SCOIT-0.1.1/SCOIT.egg-info/
--rw-r--r--   0 wangruohan   (501) staff       (20)     6585 2023-04-26 03:57:28.000000 SCOIT-0.1.1/SCOIT.egg-info/PKG-INFO
--rw-r--r--   0 wangruohan   (501) staff       (20)      313 2023-04-26 03:57:28.000000 SCOIT-0.1.1/SCOIT.egg-info/SOURCES.txt
--rw-r--r--   0 wangruohan   (501) staff       (20)        1 2023-04-26 03:57:28.000000 SCOIT-0.1.1/SCOIT.egg-info/dependency_links.txt
--rw-r--r--   0 wangruohan   (501) staff       (20)       19 2023-04-26 03:57:28.000000 SCOIT-0.1.1/SCOIT.egg-info/requires.txt
--rw-r--r--   0 wangruohan   (501) staff       (20)        6 2023-04-26 03:57:28.000000 SCOIT-0.1.1/SCOIT.egg-info/top_level.txt
-drwxr-xr-x   0 wangruohan   (501) staff       (20)        0 2023-04-26 03:57:28.306290 SCOIT-0.1.1/scoit/
--rw-rw-r--   0 wangruohan   (501) staff       (20)      167 2023-04-25 19:13:00.000000 SCOIT-0.1.1/scoit/__init__.py
--rw-rw-r--   0 wangruohan   (501) staff       (20)     2251 2023-04-25 19:13:00.000000 SCOIT-0.1.1/scoit/cell_analysis.py
--rw-rw-r--   0 wangruohan   (501) staff       (20)     1005 2023-04-26 03:43:07.000000 SCOIT-0.1.1/scoit/gene_analysis.py
--rw-rw-r--   0 wangruohan   (501) staff       (20)    16990 2023-04-25 19:13:00.000000 SCOIT-0.1.1/scoit/multi_omics_model.py
--rw-rw-r--   0 wangruohan   (501) staff       (20)    20854 2023-04-25 19:13:00.000000 SCOIT-0.1.1/scoit/tensorsc_model.py
--rw-rw-r--   0 wangruohan   (501) staff       (20)    18424 2023-04-25 19:13:00.000000 SCOIT-0.1.1/scoit/unionCom_alignment.py
--rw-r--r--   0 wangruohan   (501) staff       (20)       38 2023-04-26 03:57:28.307770 SCOIT-0.1.1/setup.cfg
--rw-rw-r--   0 wangruohan   (501) staff       (20)      820 2023-04-26 03:18:22.000000 SCOIT-0.1.1/setup.py
+drwxr-xr-x   0 wangruohan   (501) staff       (20)        0 2023-05-31 13:46:54.688293 SCOIT-0.1.2/
+-rw-rw-r--   0 wangruohan   (501) staff       (20)     1070 2023-05-31 05:35:00.000000 SCOIT-0.1.2/LICENSE
+-rw-r--r--   0 wangruohan   (501) staff       (20)     6647 2023-05-31 13:46:54.688008 SCOIT-0.1.2/PKG-INFO
+-rw-rw-r--   0 wangruohan   (501) staff       (20)     6106 2023-05-31 05:35:00.000000 SCOIT-0.1.2/README.md
+drwxr-xr-x   0 wangruohan   (501) staff       (20)        0 2023-05-31 13:46:54.681967 SCOIT-0.1.2/SCOIT.egg-info/
+-rw-r--r--   0 wangruohan   (501) staff       (20)     6647 2023-05-31 13:46:54.000000 SCOIT-0.1.2/SCOIT.egg-info/PKG-INFO
+-rw-r--r--   0 wangruohan   (501) staff       (20)      313 2023-05-31 13:46:54.000000 SCOIT-0.1.2/SCOIT.egg-info/SOURCES.txt
+-rw-r--r--   0 wangruohan   (501) staff       (20)        1 2023-05-31 13:46:54.000000 SCOIT-0.1.2/SCOIT.egg-info/dependency_links.txt
+-rw-r--r--   0 wangruohan   (501) staff       (20)       48 2023-05-31 13:46:54.000000 SCOIT-0.1.2/SCOIT.egg-info/requires.txt
+-rw-r--r--   0 wangruohan   (501) staff       (20)        6 2023-05-31 13:46:54.000000 SCOIT-0.1.2/SCOIT.egg-info/top_level.txt
+drwxr-xr-x   0 wangruohan   (501) staff       (20)        0 2023-05-31 13:46:54.686781 SCOIT-0.1.2/scoit/
+-rw-rw-r--   0 wangruohan   (501) staff       (20)      167 2023-05-31 05:35:00.000000 SCOIT-0.1.2/scoit/__init__.py
+-rw-rw-r--   0 wangruohan   (501) staff       (20)     2251 2023-05-31 05:35:00.000000 SCOIT-0.1.2/scoit/cell_analysis.py
+-rw-rw-r--   0 wangruohan   (501) staff       (20)     1005 2023-05-31 05:35:00.000000 SCOIT-0.1.2/scoit/gene_analysis.py
+-rw-rw-r--   0 wangruohan   (501) staff       (20)    16990 2023-05-31 05:35:00.000000 SCOIT-0.1.2/scoit/multi_omics_model.py
+-rw-rw-r--   0 wangruohan   (501) staff       (20)    22401 2023-05-31 05:35:00.000000 SCOIT-0.1.2/scoit/tensorsc_model.py
+-rw-rw-r--   0 wangruohan   (501) staff       (20)    18424 2023-05-31 05:35:00.000000 SCOIT-0.1.2/scoit/unionCom_alignment.py
+-rw-r--r--   0 wangruohan   (501) staff       (20)       38 2023-05-31 13:46:54.688387 SCOIT-0.1.2/setup.cfg
+-rw-rw-r--   0 wangruohan   (501) staff       (20)      855 2023-05-31 05:35:00.000000 SCOIT-0.1.2/setup.py
```

### Comparing `SCOIT-0.1.1/LICENSE` & `SCOIT-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SCOIT-0.1.1/PKG-INFO` & `SCOIT-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SCOIT
-Version: 0.1.1
+Version: 0.1.2
 Summary: SCOIT is an implementation of a probabilistic tensor decomposition framework for single-cell multi-omics data integration.
 Home-page: https://github.com/deepomicslab/SCOIT
 Author: WANG Ruohan
 Author-email: ruohawang2-c@my.cityu.edu.hk
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,18 +18,19 @@
 
 ![image](https://github.com/deepomicslab/SCOIT/blob/main/framework.png)
 
 # Getting started
 
 ## Prerequisite
 + numpy
-+ scipy
++ scipy 1.6.0
 + sklearn
 + communities
 + igraph
++ leidenalg
 + pytorch 1.9.0
 
 ## Install
 ```
 pip install SCOIT
 ```
 
@@ -128,14 +129,15 @@
 Project the feature embedding to cell embeddings and visualize with UMAP.
 > + ```umap_epochs```: The number of UMAP epochs for visualization (default=100).
 > + ```dimension```: The dimension of the embeddings to use (default=30).
 > + ```figure_name```: The saved figure name (default="feature_projections.png").
 
 
 ### Version history
-+ `v0.1.1`: Automatically adjusts the coefficients; Add downstream analyses; Extend to unpaired data;
++ `v0.1.2`: Adjust correlation calculation.
++ `v0.1.1`: Automatically adjusts the coefficients; Add downstream analyses; Extend to unpaired data.
 + `v0.0.1`: Initial version.
 
 ### Maintainer
 WANG Ruohan ruohawang2-c@my.cityu.edu.hk
```

### Comparing `SCOIT-0.1.1/README.md` & `SCOIT-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 
 ![image](https://github.com/deepomicslab/SCOIT/blob/main/framework.png)
 
 # Getting started
 
 ## Prerequisite
 + numpy
-+ scipy
++ scipy 1.6.0
 + sklearn
 + communities
 + igraph
++ leidenalg
 + pytorch 1.9.0
 
 ## Install
 ```
 pip install SCOIT
 ```
 
@@ -113,14 +114,15 @@
 Project the feature embedding to cell embeddings and visualize with UMAP.
 > + ```umap_epochs```: The number of UMAP epochs for visualization (default=100).
 > + ```dimension```: The dimension of the embeddings to use (default=30).
 > + ```figure_name```: The saved figure name (default="feature_projections.png").
 
 
 ### Version history
-+ `v0.1.1`: Automatically adjusts the coefficients; Add downstream analyses; Extend to unpaired data;
++ `v0.1.2`: Adjust correlation calculation.
++ `v0.1.1`: Automatically adjusts the coefficients; Add downstream analyses; Extend to unpaired data.
 + `v0.0.1`: Initial version.
 
 ### Maintainer
 WANG Ruohan ruohawang2-c@my.cityu.edu.hk
```

### Comparing `SCOIT-0.1.1/SCOIT.egg-info/PKG-INFO` & `SCOIT-0.1.2/SCOIT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SCOIT
-Version: 0.1.1
+Version: 0.1.2
 Summary: SCOIT is an implementation of a probabilistic tensor decomposition framework for single-cell multi-omics data integration.
 Home-page: https://github.com/deepomicslab/SCOIT
 Author: WANG Ruohan
 Author-email: ruohawang2-c@my.cityu.edu.hk
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,18 +18,19 @@
 
 ![image](https://github.com/deepomicslab/SCOIT/blob/main/framework.png)
 
 # Getting started
 
 ## Prerequisite
 + numpy
-+ scipy
++ scipy 1.6.0
 + sklearn
 + communities
 + igraph
++ leidenalg
 + pytorch 1.9.0
 
 ## Install
 ```
 pip install SCOIT
 ```
 
@@ -128,14 +129,15 @@
 Project the feature embedding to cell embeddings and visualize with UMAP.
 > + ```umap_epochs```: The number of UMAP epochs for visualization (default=100).
 > + ```dimension```: The dimension of the embeddings to use (default=30).
 > + ```figure_name```: The saved figure name (default="feature_projections.png").
 
 
 ### Version history
-+ `v0.1.1`: Automatically adjusts the coefficients; Add downstream analyses; Extend to unpaired data;
++ `v0.1.2`: Adjust correlation calculation.
++ `v0.1.1`: Automatically adjusts the coefficients; Add downstream analyses; Extend to unpaired data.
 + `v0.0.1`: Initial version.
 
 ### Maintainer
 WANG Ruohan ruohawang2-c@my.cityu.edu.hk
```

### Comparing `SCOIT-0.1.1/scoit/cell_analysis.py` & `SCOIT-0.1.2/scoit/cell_analysis.py`

 * *Files identical despite different names*

### Comparing `SCOIT-0.1.1/scoit/gene_analysis.py` & `SCOIT-0.1.2/scoit/gene_analysis.py`

 * *Files identical despite different names*

### Comparing `SCOIT-0.1.1/scoit/multi_omics_model.py` & `SCOIT-0.1.2/scoit/multi_omics_model.py`

 * *Files identical despite different names*

### Comparing `SCOIT-0.1.1/scoit/tensorsc_model.py` & `SCOIT-0.1.2/scoit/tensorsc_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import pandas as pd
 from sklearn.impute import KNNImputer
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.optim import SGD, Adam
 from torch.utils.data import Dataset, DataLoader, TensorDataset
+from scipy import stats
 from scoit import matrix_model, matrix_model_complete, matrix_list_model, matrix_list_model_complete
 
 def min_max_normalization(data, zero_impute=True):
     contain_na = False
     for omics_data in data:
         if np.isnan(omics_data).any():
             contain_na = True
@@ -37,17 +38,17 @@
         omics_max = []
         for omics_data in data:
             min_ = omics_data.min()
             max_ = omics_data.max()
             omics_data = (omics_data - min_) / (max_ - min_) + 0.1
         
             new_data.append(np.array(omics_data))
-            omics_min.append([min_])
-            omics_max.append([max_])
-
+            omics_min.append(np.array([min_]))
+            omics_max.append(np.array([max_]))
+    
     return new_data, omics_min, omics_max
 
 
 class sc_multi_omics:
     def __init__(self, K1=30, K2=30, K3=30, random_seed=123):
         self.K1 = K1
         self.K2 = K2
@@ -57,20 +58,47 @@
     def cal_corr(self, data):
         if data.shape[0] == 1:
             pearsonr = 0
         else:
             choose_col = (~np.isnan(data[0]).any(axis=0)) & (~np.isnan(data[1]).any(axis=0))
             for i in range(2, data.shape[0]):
                 choose_col = choose_col & (~np.isnan(data[i]).any(axis=0))
+            print("There is %s shared feautures detected in the dataset."%np.sum(choose_col))
             if (np.sum(choose_col)) == 0:
-                print("There is no overlapping genes detected in the dataset.")
+                print("There is no shared feature detected in the dataset.")
                 pearsonr = 0
             else:
-                pearsonr = np.min(np.corrcoef(data[:, :, choose_col].reshape((data.shape[0], -1))))
-        return abs(pearsonr)
+                choose_data = data[:, :, choose_col]
+                pearsonr_list = []
+                for i in range(choose_data.shape[2]):
+                    pearsonr_list.append(np.min(np.corrcoef(choose_data[:, :, i])))
+
+                np.random.seed(self.random_seed)
+                np.random.shuffle(choose_data[0])
+                pearsonr_list_random = []
+                for i in range(choose_data.shape[2]):
+                    pearsonr_list_random.append(np.min(np.corrcoef(choose_data[:, :, i])))
+
+                pearsonr_list_ = []
+                pearsonr_list_random_ = []
+                for i in range(len(pearsonr_list)):
+                    if not (np.isnan(pearsonr_list[i]) or np.isnan(pearsonr_list_random[i])):
+                        pearsonr_list_.append(abs(pearsonr_list[i]))
+                        pearsonr_list_random_.append(abs(pearsonr_list_random[i]))
+
+                if len(pearsonr_list_) != 0:
+                    pearsonr_median = np.median(pearsonr_list_)
+                    pvalue = stats.ttest_ind(pearsonr_list_, pearsonr_list_random_, equal_var=False, alternative='greater').pvalue
+                else:
+                    pearsonr_median = 0
+                    pvalue = 1
+
+        print("The median pearsonr is %s; The P-value is %s." % (pearsonr_median, pvalue))
+
+        return pearsonr_median, pvalue
 
     def KNN_impute(self, matrix):
         data = np.hstack((matrix))
         imputer = KNNImputer()
         KNN_impute_data = imputer.fit_transform(data)
         if data.shape != KNN_impute_data.shape:
             print("Skip KNN preimpute because of the all-zero features.")    
@@ -84,23 +112,24 @@
         
         return matrix
     
     def fit(self, matrix, normalization=True, pre_impute=False, opt="Adam", dist="gaussian", lr=1e-2, n_epochs=1000, lambda_C_regularizer=0, lambda_G_regularizer=0, lambda_O_regularizer=[0, 0], lambda_OC_regularizer=[0, 0], lambda_OG_regularizer=[0, 0], batch_size=256, earlystopping=True, device='cuda' if torch.cuda.is_available() else 'cpu', verbose=True):
         # tune the coefficient
         if (lambda_C_regularizer==0) or (lambda_G_regularizer==0) or (0 in lambda_O_regularizer) or (0 in lambda_OC_regularizer) or (0 in lambda_OG_regularizer):
             print("Automatically tune the coefficients for the penalty terms.")
-            if self.cal_corr(matrix) > 0.4:
-                print("High correlation between the omics detected.")
+            pearsonr_median, pvalue = self.cal_corr(matrix)
+            if pearsonr_median > 0.7 and pvalue < 0.05:
+                print("Correlation between the omics detected.")
                 lambda_C_regularizer = 0.01
                 lambda_G_regularizer = 0.01
                 lambda_O_regularizer = [0.01] * matrix.shape[0]
                 lambda_OC_regularizer = [1] * matrix.shape[0]
                 lambda_OG_regularizer = [1] * matrix.shape[0]
             else:
-                print("Low correlation between the omics detected.")
+                print("No correlation between the omics detected.")
                 lambda_C_regularizer = 0.01
                 lambda_G_regularizer = 1
                 lambda_O_regularizer = [1] * matrix.shape[0]
                 lambda_OC_regularizer = [1] * matrix.shape[0]
                 lambda_OG_regularizer = [0.01] * matrix.shape[0]
         
         # min-max normizaltion 
@@ -176,23 +205,24 @@
         return matrix_hat
     
     
     def fit_complete(self, matrix, normalization=True, pre_impute=True, opt="Adam", dist="gaussian", lr=1e-2, n_epochs=1000, lambda_C_regularizer=0, lambda_G_regularizer=0, lambda_O_regularizer=[0, 0], lambda_OC_regularizer=[0, 0], lambda_OG_regularizer=[0, 0], batch_size=256, earlystopping=True, device='cuda' if torch.cuda.is_available() else 'cpu', verbose=True):
         # tune the coefficent
         if (lambda_C_regularizer==0) or (lambda_G_regularizer==0) or (0 in lambda_O_regularizer) or (0 in lambda_OC_regularizer) or (0 in lambda_OG_regularizer):
             print("Automatically tune the coefficients for the penalty terms.")
-            if np.min(self.cal_corr(matrix)) > 0.4:
-                print("High correlation between the omics detected.")
+            pearsonr_median, pvalue = self.cal_corr(matrix)
+            if pearsonr_median > 0.7 and pvalue < 0.05:
+                print("Correlation between the omics detected.")
                 lambda_C_regularizer = 0.01
                 lambda_G_regularizer = 0.01
                 lambda_O_regularizer = [0.01] * matrix.shape[0]
                 lambda_OC_regularizer = [1] * matrix.shape[0]
                 lambda_OG_regularizer = [1] * matrix.shape[0]
             else:
-                print("Low correlation between the omics detected.")
+                print("No correlation between the omics detected.")
                 lambda_C_regularizer = 0.01
                 lambda_G_regularizer = 1
                 lambda_O_regularizer = [1] * matrix.shape[0]
                 lambda_OC_regularizer = [1] * matrix.shape[0]
                 lambda_OG_regularizer = [0.01] * matrix.shape[0]
         
         # min-max normalization
@@ -318,15 +348,15 @@
         self.O = np.hstack((model.O1.cpu().detach().numpy(), model.O2.cpu().detach().numpy()))
 
         matrix_list_hat = [matrix_list_hat[i].cpu().detach().numpy() for i in range(self.L)]
         if dist == "poisson" or dist == "negative bionomial":
             matrix_list_hat = [np.exp(matrix_list_hat[i]) for i in range(self.L)]
         
         if normalization:
-            matrix_list_hat = matrix_list_hat - 0.1
+            matrix_list_hat = [matrix_list_hat[i] - 0.1 for i in range(self.L)]
             for i in range(len(matrix_list_hat)):
                 if np.isnan(omics_max[i]).any() or np.isnan(omics_min[i]).any():
                     imputer = KNNImputer()
                     omics_max[i] = imputer.fit_transform(np.vstack((matrix_list_hat[i], omics_max[i].reshape((1, -1)))).T)[:, -1]
                     omics_min[i] = imputer.fit_transform(np.vstack((matrix_list_hat[i], omics_min[i].reshape((1, -1)))).T)[:, -1]
                 matrix_list_hat[i] = matrix_list_hat[i] * (omics_max[i] - omics_min[i]) + omics_min[i]
 
@@ -383,15 +413,15 @@
         self.O = np.hstack((model.O1.cpu().detach().numpy(), model.O2.cpu().detach().numpy()))
         
         matrix_list_hat = [matrix_list_hat[i].cpu().detach().numpy() for i in range(self.L)]
         if dist == "poisson" or dist == "negative bionomial":
             matrix_list_hat = [np.exp(matrix_list_hat[i]) for i in range(self.L)]
         
         if normalization:
-            matrix_list_hat = matrix_list_hat - 0.1
+            matrix_list_hat = [matrix_list_hat[i] - 0.1 for i in range(self.L)]
             for i in range(len(matrix_list_hat)):
                 if np.isnan(omics_max[i]).any() or np.isnan(omics_min[i]).any():
                     imputer = KNNImputer()
                     omics_max[i] = imputer.fit_transform(np.vstack((matrix_list_hat[i], omics_max[i].reshape((1, -1)))).T)[:, -1]
                     omics_min[i] = imputer.fit_transform(np.vstack((matrix_list_hat[i], omics_min[i].reshape((1, -1)))).T)[:, -1]
                 matrix_list_hat[i] = matrix_list_hat[i] * (omics_max[i] - omics_min[i]) + omics_min[i]
```

### Comparing `SCOIT-0.1.1/scoit/unionCom_alignment.py` & `SCOIT-0.1.2/scoit/unionCom_alignment.py`

 * *Files identical despite different names*

### Comparing `SCOIT-0.1.1/setup.py` & `SCOIT-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='SCOIT',
-    version='0.1.1',
+    version='0.1.2',
     packages=setuptools.find_packages(),
     url='https://github.com/deepomicslab/SCOIT',
     license='MIT',
 	author='WANG Ruohan',
     author_email='ruohawang2-c@my.cityu.edu.hk',
     description='SCOIT is an implementation of a probabilistic tensor decomposition framework for single-cell multi-omics data integration.',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=['numpy', 'torch==1.9.0'],
+    install_requires=['numpy', 'torch==1.9.0', 'scipy==1.6.0', 'sklearn==0.24.2'],
     classifiers=[
         "Programming Language :: Python :: 3",
 		"License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
     ],
     python_requires='>=3.6',
 )
```

