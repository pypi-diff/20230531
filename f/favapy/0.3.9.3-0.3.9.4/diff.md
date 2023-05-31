# Comparing `tmp/favapy-0.3.9.3.tar.gz` & `tmp/favapy-0.3.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "favapy-0.3.9.3.tar", last modified: Fri May 19 14:16:27 2023, max compression
+gzip compressed data, was "favapy-0.3.9.4.tar", last modified: Wed May 31 14:18:16 2023, max compression
```

## Comparing `favapy-0.3.9.3.tar` & `favapy-0.3.9.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tgn531     (501) staff       (20)        0 2023-05-19 14:16:27.519131 favapy-0.3.9.3/
--rw-r--r--   0 tgn531     (501) staff       (20)     1065 2022-03-14 10:14:48.000000 favapy-0.3.9.3/LICENSE
--rw-r--r--   0 tgn531     (501) staff       (20)     4067 2023-05-19 14:16:27.519429 favapy-0.3.9.3/PKG-INFO
--rw-r--r--   0 tgn531     (501) staff       (20)     3360 2023-05-19 14:13:30.000000 favapy-0.3.9.3/README.md
--rw-r--r--   0 tgn531     (501) staff       (20)       85 2022-03-16 16:20:29.000000 favapy-0.3.9.3/pyproject.toml
--rw-r--r--   0 tgn531     (501) staff       (20)      948 2023-05-19 14:16:27.695779 favapy-0.3.9.3/setup.cfg
--rw-r--r--   0 tgn531     (501) staff       (20)     1080 2023-05-19 14:09:41.000000 favapy-0.3.9.3/setup.py
-drwxr-xr-x   0 tgn531     (501) staff       (20)        0 2023-05-19 14:16:27.252994 favapy-0.3.9.3/src/
-drwxr-xr-x   0 tgn531     (501) staff       (20)        0 2023-05-19 14:16:27.464150 favapy-0.3.9.3/src/favapy/
--rw-r--r--   0 tgn531     (501) staff       (20)        0 2022-03-16 11:55:28.000000 favapy-0.3.9.3/src/favapy/__init__.py
--rw-r--r--   0 tgn531     (501) staff       (20)    10296 2023-05-19 14:08:39.000000 favapy-0.3.9.3/src/favapy/fava.py
-drwxr-xr-x   0 tgn531     (501) staff       (20)        0 2023-05-19 14:16:27.517946 favapy-0.3.9.3/src/favapy.egg-info/
--rw-r--r--   0 tgn531     (501) staff       (20)     4067 2023-05-19 14:16:26.000000 favapy-0.3.9.3/src/favapy.egg-info/PKG-INFO
--rw-r--r--   0 tgn531     (501) staff       (20)      299 2023-05-19 14:16:26.000000 favapy-0.3.9.3/src/favapy.egg-info/SOURCES.txt
--rw-r--r--   0 tgn531     (501) staff       (20)        1 2023-05-19 14:16:26.000000 favapy-0.3.9.3/src/favapy.egg-info/dependency_links.txt
--rw-r--r--   0 tgn531     (501) staff       (20)       44 2023-05-19 14:16:26.000000 favapy-0.3.9.3/src/favapy.egg-info/entry_points.txt
--rw-r--r--   0 tgn531     (501) staff       (20)       38 2023-05-19 14:16:26.000000 favapy-0.3.9.3/src/favapy.egg-info/requires.txt
--rw-r--r--   0 tgn531     (501) staff       (20)        7 2023-05-19 14:16:26.000000 favapy-0.3.9.3/src/favapy.egg-info/top_level.txt
+drwxr-xr-x   0 tgn531     (501) staff       (20)        0 2023-05-31 14:18:16.171148 favapy-0.3.9.4/
+-rw-r--r--   0 tgn531     (501) staff       (20)     1065 2022-03-14 10:14:48.000000 favapy-0.3.9.4/LICENSE
+-rw-r--r--   0 tgn531     (501) staff       (20)     4067 2023-05-31 14:18:16.171333 favapy-0.3.9.4/PKG-INFO
+-rw-r--r--   0 tgn531     (501) staff       (20)     3360 2023-05-19 14:13:30.000000 favapy-0.3.9.4/README.md
+-rw-r--r--   0 tgn531     (501) staff       (20)       85 2022-03-16 16:20:29.000000 favapy-0.3.9.4/pyproject.toml
+-rw-r--r--   0 tgn531     (501) staff       (20)      948 2023-05-31 14:18:16.173479 favapy-0.3.9.4/setup.cfg
+-rw-r--r--   0 tgn531     (501) staff       (20)     1080 2023-05-31 14:16:30.000000 favapy-0.3.9.4/setup.py
+drwxr-xr-x   0 tgn531     (501) staff       (20)        0 2023-05-31 14:18:16.154758 favapy-0.3.9.4/src/
+drwxr-xr-x   0 tgn531     (501) staff       (20)        0 2023-05-31 14:18:16.165232 favapy-0.3.9.4/src/favapy/
+-rw-r--r--   0 tgn531     (501) staff       (20)        0 2022-03-16 11:55:28.000000 favapy-0.3.9.4/src/favapy/__init__.py
+-rw-r--r--   0 tgn531     (501) staff       (20)    10386 2023-05-31 14:15:12.000000 favapy-0.3.9.4/src/favapy/fava.py
+drwxr-xr-x   0 tgn531     (501) staff       (20)        0 2023-05-31 14:18:16.170364 favapy-0.3.9.4/src/favapy.egg-info/
+-rw-r--r--   0 tgn531     (501) staff       (20)     4067 2023-05-31 14:18:15.000000 favapy-0.3.9.4/src/favapy.egg-info/PKG-INFO
+-rw-r--r--   0 tgn531     (501) staff       (20)      299 2023-05-31 14:18:15.000000 favapy-0.3.9.4/src/favapy.egg-info/SOURCES.txt
+-rw-r--r--   0 tgn531     (501) staff       (20)        1 2023-05-31 14:18:15.000000 favapy-0.3.9.4/src/favapy.egg-info/dependency_links.txt
+-rw-r--r--   0 tgn531     (501) staff       (20)       44 2023-05-31 14:18:15.000000 favapy-0.3.9.4/src/favapy.egg-info/entry_points.txt
+-rw-r--r--   0 tgn531     (501) staff       (20)       38 2023-05-31 14:18:15.000000 favapy-0.3.9.4/src/favapy.egg-info/requires.txt
+-rw-r--r--   0 tgn531     (501) staff       (20)        7 2023-05-31 14:18:15.000000 favapy-0.3.9.4/src/favapy.egg-info/top_level.txt
```

### Comparing `favapy-0.3.9.3/LICENSE` & `favapy-0.3.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `favapy-0.3.9.3/PKG-INFO` & `favapy-0.3.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: favapy
-Version: 0.3.9.3
+Version: 0.3.9.4
 Summary: Infer Functional Associations using Variational Autoencoders on -Omics data.
 Home-page: https://github.com/mikelkou/VAE_Functional_associations
 Author: Mikaela Koutrouli
 Author-email: mikaela.koutrouli@cpr.ku.dk
 Project-URL: Bug Tracker, https://github.com/mikelkou/VAE_Functional_associations/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `favapy-0.3.9.3/README.md` & `favapy-0.3.9.4/README.md`

 * *Files identical despite different names*

### Comparing `favapy-0.3.9.3/setup.cfg` & `favapy-0.3.9.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = favapy
-version = 0.3.9.3
+version = 0.3.9.4
 author = Mikaela Koutrouli
 author_email = mikaela.koutrouli@cpr.ku.dk
 description = Infer Functional Associations using Variational Autoencoders on -Omics data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mikelkou/VAE_Functional_associations
 project_urls =
```

### Comparing `favapy-0.3.9.3/setup.py` & `favapy-0.3.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="favapy",
-    version="0.3.9.3",
+    version="0.3.9.4",
     author="Mikaela Koutrouli",
     author_email="mikaela.koutrouli@cpr.ku.dk",
     description="Infer Functional Associations using Variational Autoencoders on -Omics data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mikelkou/VAE_Functional_associations",
     project_urls={
```

### Comparing `favapy-0.3.9.3/src/favapy/fava.py` & `favapy-0.3.9.4/src/favapy/fava.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 
 
 def pairs_after_cutoff(correlation, interaction_count=100000, PCC_cutoff=None):
     if PCC_cutoff is not None and isinstance(PCC_cutoff, (int, float)):
         logging.info(" A cut-off of " + str(PCC_cutoff) + " is applied.")
         correlation_df_new = correlation.loc[(correlation['Score'] >= PCC_cutoff)]
     else:
-        correlation_df_new = correlation.head(interaction_count+1)
+        correlation_df_new = correlation.iloc[:interaction_count,:]
         logging.warn(" The number of interactions in the output file is " + str(interaction_count) + " in which both directions are included: proteinA - proteinB and proteinB - proteinA.")
     return correlation_df_new
 
 def cook(data,
 	log2_normalization = True,
 	hidden_layer = None,
         latent_dim = None,
@@ -204,17 +204,17 @@
             latent_dim = 5
 
     opt = tf.keras.optimizers.Adam(learning_rate=0.001, clipnorm=0.001)
     x_train = x_test = np.array(x) 
     vae = VAE(opt, x_train, x_test, batch_size, original_dim, hidden_layer, latent_dim, epochs)
     x_test_encoded = np.array(vae.encoder.predict(x_test, batch_size=batch_size))
     correlation = create_protein_pairs(x_test_encoded, row_names)
-    final_pairs =  pairs_after_cutoff(correlation, interaction_count=interaction_count, PCC_cutoff=PCC_cutoff)
-    final_pairs = final_pairs[final_pairs.iloc[:,0] != final_pairs.iloc[:,1]]
+    final_pairs = correlation[correlation.iloc[:,0] != correlation.iloc[:,1]]
     final_pairs = final_pairs.sort_values(by=['Score'], ascending=False)
+    final_pairs =  pairs_after_cutoff(correlation=final_pairs, interaction_count=interaction_count, PCC_cutoff=PCC_cutoff)
     return final_pairs
 
 
 def main():
     args = argument_parser()
 
     x, row_names = load_data(args.input_file,args.data_type)
@@ -238,21 +238,22 @@
 
     opt = tf.keras.optimizers.Adam(learning_rate=0.001, clipnorm=0.001)
     x_train = x_test = np.array(x) 
     vae = VAE(opt, x_train, x_test, args.batch_size, original_dim, args.hidden_layer, args.latent_dim, args.epochs)
     x_test_encoded = np.array(vae.encoder.predict(x_test, batch_size=args.batch_size))
     
     logging.info(" Calculating Pearson correlation scores.")
-
     correlation = create_protein_pairs(x_test_encoded, row_names)    
-    final_pairs =  pairs_after_cutoff(correlation, interaction_count=args.interaction_count, PCC_cutoff=args.PCC_cutoff)
-    logging.warn(" If it is not the desired cut-off, please check again the value assigned to the related parameter (-n or interaction_count | -c or PCC_cutoff).")
 
-    final_pairs = final_pairs[final_pairs.iloc[:,0] != final_pairs.iloc[:,1]]
+    final_pairs = correlation[correlation.iloc[:,0] != correlation.iloc[:,1]]
     final_pairs = final_pairs.sort_values(by=['Score'], ascending=False)
+    final_pairs =  pairs_after_cutoff(correlation=final_pairs, interaction_count=args.interaction_count, PCC_cutoff=args.PCC_cutoff)
+    final_pairs.Score = final_pairs.Score.astype(float).round(5)
+    logging.warn(" If it is not the desired cut-off, please check again the value assigned to the related parameter (-n or interaction_count | -c or PCC_cutoff).")
+
     logging.info(" Saving the file with the interactions in the chosen directory ...")
 
     # Save the file
     np.savetxt(args.output_file, final_pairs, fmt='%s')
     logging.info(" Congratulations! A file is waitiing for you here: " + args.output_file)
```

### Comparing `favapy-0.3.9.3/src/favapy.egg-info/PKG-INFO` & `favapy-0.3.9.4/src/favapy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: favapy
-Version: 0.3.9.3
+Version: 0.3.9.4
 Summary: Infer Functional Associations using Variational Autoencoders on -Omics data.
 Home-page: https://github.com/mikelkou/VAE_Functional_associations
 Author: Mikaela Koutrouli
 Author-email: mikaela.koutrouli@cpr.ku.dk
 Project-URL: Bug Tracker, https://github.com/mikelkou/VAE_Functional_associations/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

