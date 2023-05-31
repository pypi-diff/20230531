# Comparing `tmp/genda_lens-0.0.2.tar.gz` & `tmp/genda_lens-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genda_lens-0.0.2.tar", max compression
+gzip compressed data, was "genda_lens-0.0.3.tar", max compression
```

## Comparing `genda_lens-0.0.2.tar` & `genda_lens-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1065 2023-05-16 07:25:58.546949 genda_lens-0.0.2/LICENSE
--rw-r--r--   0        0        0     4094 2023-05-27 22:01:31.208109 genda_lens-0.0.2/README.md
--rw-r--r--   0        0        0       48 2023-05-29 19:40:52.621288 genda_lens-0.0.2/genda_lens/__init__.py
--rw-r--r--   0        0        0     8236 2023-05-27 21:28:14.357211 genda_lens-0.0.2/genda_lens/coref_tasks/abc_utils.py
--rw-r--r--   0        0        0    12485 2023-05-18 12:02:26.903295 genda_lens-0.0.2/genda_lens/coref_tasks/wino_utils.py
--rw-r--r--   0        0        0    57119 2023-03-21 08:24:08.746101 genda_lens-0.0.2/genda_lens/data/DaWinoBias_anti_stereotyped_evalda.txt
--rw-r--r--   0        0        0    57118 2023-03-09 16:12:47.834912 genda_lens-0.0.2/genda_lens/data/DaWinoBias_pro_stereotyped_evalda.txt
--rw-r--r--   0        0        0   336571 2023-04-26 15:47:17.498741 genda_lens-0.0.2/genda_lens/data/abc_fem_sents.txt
--rw-r--r--   0        0        0   324943 2023-04-26 15:47:29.017834 genda_lens-0.0.2/genda_lens/data/abc_male_sents.txt
--rw-r--r--   0        0        0   706895 2023-05-03 17:07:48.000948 genda_lens-0.0.2/genda_lens/data/name_aug_csv_files/first_names_2023_men.csv
--rw-r--r--   0        0        0   891168 2023-05-03 17:07:48.029137 genda_lens-0.0.2/genda_lens/data/name_aug_csv_files/first_names_2023_women.csv
--rw-r--r--   0        0        0  4094899 2023-05-03 17:07:48.124266 genda_lens-0.0.2/genda_lens/data/name_aug_csv_files/last_names_2023.csv
--rw-r--r--   0        0        0     1114 2023-05-03 17:07:48.132607 genda_lens-0.0.2/genda_lens/data/name_aug_csv_files/overlapping_names.csv
--rw-r--r--   0        0        0    11901 2023-05-03 17:07:48.133913 genda_lens-0.0.2/genda_lens/data/name_aug_csv_files/unisex_names.csv
--rw-r--r--   0        0        0    18439 2023-05-29 19:40:07.994862 genda_lens-0.0.2/genda_lens/genda_lens.py
--rw-r--r--   0        0        0    10287 2023-05-27 21:13:32.580660 genda_lens-0.0.2/genda_lens/lm_tasks/abc_utils.py
--rw-r--r--   0        0        0      256 2023-05-18 12:02:26.951826 genda_lens-0.0.2/genda_lens/lm_tasks/load_model.py
--rw-r--r--   0        0        0     6957 2023-05-18 12:02:26.953592 genda_lens-0.0.2/genda_lens/lm_tasks/wino_utils.py
--rw-r--r--   0        0        0     1550 2023-05-18 12:02:26.954488 genda_lens-0.0.2/genda_lens/ner_tasks/augmentation.py
--rw-r--r--   0        0        0     5755 2023-05-18 12:02:26.955388 genda_lens-0.0.2/genda_lens/ner_tasks/performance.py
--rw-r--r--   0        0        0     2687 2023-05-18 12:02:26.956243 genda_lens-0.0.2/genda_lens/ner_tasks/process_names.py
--rw-r--r--   0        0        0      764 2023-05-29 19:41:00.042448 genda_lens-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5201 1970-01-01 00:00:00.000000 genda_lens-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-16 07:25:58.546949 genda_lens-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4094 2023-05-27 22:01:31.208109 genda_lens-0.0.3/README.md
+-rw-r--r--   0        0        0       48 2023-05-29 20:46:47.326614 genda_lens-0.0.3/genda_lens/__init__.py
+-rw-r--r--   0        0        0     8316 2023-05-31 07:00:51.115657 genda_lens-0.0.3/genda_lens/coref_tasks/abc_utils.py
+-rw-r--r--   0        0        0    12485 2023-05-18 12:02:26.903295 genda_lens-0.0.3/genda_lens/coref_tasks/wino_utils.py
+-rw-r--r--   0        0        0    57119 2023-03-21 08:24:08.746101 genda_lens-0.0.3/genda_lens/data/DaWinoBias_anti_stereotyped_evalda.txt
+-rw-r--r--   0        0        0    57118 2023-03-09 16:12:47.834912 genda_lens-0.0.3/genda_lens/data/DaWinoBias_pro_stereotyped_evalda.txt
+-rw-r--r--   0        0        0   336571 2023-04-26 15:47:17.498741 genda_lens-0.0.3/genda_lens/data/abc_fem_sents.txt
+-rw-r--r--   0        0        0   324943 2023-04-26 15:47:29.017834 genda_lens-0.0.3/genda_lens/data/abc_male_sents.txt
+-rw-r--r--   0        0        0   706895 2023-05-03 17:07:48.000948 genda_lens-0.0.3/genda_lens/data/name_aug_csv_files/first_names_2023_men.csv
+-rw-r--r--   0        0        0   891168 2023-05-03 17:07:48.029137 genda_lens-0.0.3/genda_lens/data/name_aug_csv_files/first_names_2023_women.csv
+-rw-r--r--   0        0        0  4094899 2023-05-03 17:07:48.124266 genda_lens-0.0.3/genda_lens/data/name_aug_csv_files/last_names_2023.csv
+-rw-r--r--   0        0        0     1114 2023-05-03 17:07:48.132607 genda_lens-0.0.3/genda_lens/data/name_aug_csv_files/overlapping_names.csv
+-rw-r--r--   0        0        0    11901 2023-05-03 17:07:48.133913 genda_lens-0.0.3/genda_lens/data/name_aug_csv_files/unisex_names.csv
+-rw-r--r--   0        0        0    18111 2023-05-31 07:00:56.498026 genda_lens-0.0.3/genda_lens/genda_lens.py
+-rw-r--r--   0        0        0    10893 2023-05-31 20:20:54.950384 genda_lens-0.0.3/genda_lens/lm_tasks/abc_utils.py
+-rw-r--r--   0        0        0      256 2023-05-18 12:02:26.951826 genda_lens-0.0.3/genda_lens/lm_tasks/load_model.py
+-rw-r--r--   0        0        0     7101 2023-05-31 07:00:53.006029 genda_lens-0.0.3/genda_lens/lm_tasks/wino_utils.py
+-rw-r--r--   0        0        0     1550 2023-05-18 12:02:26.954488 genda_lens-0.0.3/genda_lens/ner_tasks/augmentation.py
+-rw-r--r--   0        0        0     6038 2023-05-31 06:54:23.704953 genda_lens-0.0.3/genda_lens/ner_tasks/performance.py
+-rw-r--r--   0        0        0     2687 2023-05-18 12:02:26.956243 genda_lens-0.0.3/genda_lens/ner_tasks/process_names.py
+-rw-r--r--   0        0        0      762 2023-05-29 20:48:01.837794 genda_lens-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5199 1970-01-01 00:00:00.000000 genda_lens-0.0.3/PKG-INFO
```

### Comparing `genda_lens-0.0.2/LICENSE` & `genda_lens-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.2/README.md` & `genda_lens-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.2/genda_lens/coref_tasks/abc_utils.py` & `genda_lens-0.0.3/genda_lens/coref_tasks/abc_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 """
 Utility functions for running the ABC coreference task.
 
 Builds on the codebase developed for the following paper: 
 
 Title: “Type B reflexivization as an unambiguous testbed for multilingual multi-task gender bias.”
 Authors: González, A. V., Barrett, M., Hvingelby, R., Webster, K., & Søgaard, A.
@@ -21,215 +20,241 @@
 import pandas as pd
 import spacy
 import torch
 from sklearn.metrics import classification_report, f1_score
 
 
 def run_abc_coref(coref_model):
-    ''' 
+    """
     Run the coreference model on the ABC dataset and return predictions. (Duration approx. 20 min.)
-    '''
+    """
     # load stereotypically male occupation sentences
-    with open(os.path.join(Path(__file__).parents[1], "data", "abc_male_sents.txt"), "r") as f:
+    with open(
+        os.path.join(Path(__file__).parents[1], "data", "abc_male_sents.txt"), "r"
+    ) as f:
         male_abc = f.readlines()
     # load stereotypically female occupation sentences
-    with open(os.path.join(Path(__file__).parents[1], "data", "abc_fem_sents.txt"), "r") as f:
+    with open(
+        os.path.join(Path(__file__).parents[1], "data", "abc_fem_sents.txt"), "r"
+    ) as f:
         fem_abc = f.readlines()
 
     all_preds = []
-    for gendered_data in [fem_abc, male_abc]:  
-        data_ = [line_ for line_ in gendered_data if line_ != '---\n']
+    for gendered_data in [fem_abc, male_abc]:
+        data_ = [line_ for line_ in gendered_data if line_ != "---\n"]
         i = 0
         preds = []
 
-        #PROGRESS BAR
+        # PROGRESS BAR
         abc_bar = progressbar.ProgressBar(maxval=len(data_)).start()
-        
+
         # run the model on the data with the predict method and save the predictions
-        for idx, i in enumerate(data_): 
+        for idx, i in enumerate(data_):
             line = [i.split()]
             try:
-            # get preds  
+                # get preds
                 predicted_clusters = coref_model.predict(line)
-            except: 
+            except:
                 print(line)
             preds.append(predicted_clusters)
             abc_bar.update(idx)
         abc_bar.finish()
-        
+
         all_preds.append(preds)
     fem_preds = all_preds[0]
     male_preds = all_preds[1]
 
     return fem_preds, male_preds
-        
+
+
 def chunks(lst, n):
     """Yield successive n-sized chunks from lst."""
     for i in range(0, len(lst), n):
-        yield lst[i:i + n]
+        yield lst[i : i + n]
+
 
 def get_coref_predictions(chunk_preds):
     """Get the coreference predictions for the reflexive case and the anti-reflexive cases.
-    
+
     Args:
         - chunk_preds: list of predictions
         - coref_output_file: the name of the file where the predictions are stored
-    
+
     Returns:
         - fem
         - male
         - reflexive
     """
-    
+
     ref, male, fem = [], [], []
-    
+
     # the truth labels for the reflexive case, i.e. all 1s
     labels_ref = list(np.repeat(1, len(chunk_preds)))
     # the truth labels for the anti-reflexive cases, i.e. all 0s
     labels_anti_ref = list(np.repeat(0, len(chunk_preds)))
-    
+
     for p in chunk_preds:
-        #assert if %3 == 0
-        
-        ref_pred, male_pred,fem_pred = p[0], p[1], p[2]
-        
-        predicted_clusters = "clusters" # could be an input argument to the function to ensure that the correct key is used in case of tesitng pther models
+        # assert if %3 == 0
+
+        ref_pred, male_pred, fem_pred = p[0], p[1], p[2]
 
-        cluster_ref = ref_pred[predicted_clusters] 
+        predicted_clusters = "clusters"  # could be an input argument to the function to ensure that the correct key is used in case of tesitng pther models
+
+        cluster_ref = ref_pred[predicted_clusters]
         cluster_male = male_pred[predicted_clusters]
-        cluster_fem = fem_pred[predicted_clusters] 
-        clusters = [cluster_ref, cluster_male, cluster_fem]   
+        cluster_fem = fem_pred[predicted_clusters]
+        clusters = [cluster_ref, cluster_male, cluster_fem]
 
         for i, cluster in enumerate(clusters):
             if i == 0:
                 if cluster != []:
                     ref.append(1)
                 else:
                     ref.append(0)
-            elif i==1:
+            elif i == 1:
                 if cluster != []:
                     male.append(1)
                 else:
                     male.append(0)
-            elif i==2:
+            elif i == 2:
                 if cluster != []:
                     fem.append(1)
                 else:
                     fem.append(0)
     return ref, fem, male, labels_ref, labels_anti_ref
 
+
 def get_positive_preds(chunk_preds):
-    '''Get False Posivie Rates for the reflexive case and the anti-reflexive cases and print output tables.'''
-    
+    """Get False Posivie Rates for the reflexive case and the anti-reflexive cases and print output tables."""
+
     ref, fem, male, labels_ref, labels_anti_ref = get_coref_predictions(chunk_preds)
-    labels_preds_ = zip([labels_ref,labels_anti_ref,labels_anti_ref], [ref,fem,male])                
+    labels_preds_ = zip(
+        [labels_ref, labels_anti_ref, labels_anti_ref], [ref, fem, male]
+    )
     # the tags for the classification reports
-    tags = ["reflexive", "anti_reflexive_female", "anti_reflexive_male"] 
+    tags = ["reflexive", "anti_reflexive_female", "anti_reflexive_male"]
     res = {}
     for idx, (label, pred) in enumerate(labels_preds_):
-        
         if label == labels_ref:
             # get the true positive rate for the current label and prediction
             res[f"tpr_{tags[idx]}"] = flm.true_positive_rate(label, pred, pos_label=1)
-        
+
         elif label == labels_anti_ref:
             # get the false positive rate for the current label and prediction
             res[f"fpr_{tags[idx]}"] = flm.false_positive_rate(label, pred, pos_label=1)
-    print(f"""
-    Total positive prediction of coreference clusters: 
-    
-    Female: {np.sum(fem)}
-    Male: {np.sum(male)}
-    Reflexive: {np.sum(ref)}
-    Total predictions:  {len(fem)} {len(male)} {len(ref)}""")
+
+    # print(f"""
+    # Total positive prediction of coreference clusters:
+
+    # Female: {np.sum(fem)}
+    # Male: {np.sum(male)}
+    # Reflexive: {np.sum(ref)}
+    # Total predictions:  {len(fem)} {len(male)} {len(ref)}""")
 
     return res
 
-def evaluate_coref_abc(fem_preds, male_preds): 
-    
-    for gender in ["fem", "male", "all_sents"]: #and for all 
-        
+
+def evaluate_coref_abc(fem_preds, male_preds):
+    for gender in ["fem", "male", "all_sents"]:  # and for all
         if gender == "fem":
             preds = fem_preds
         elif gender == "male":
             preds = male_preds
         elif gender == "all_sents":
-            preds = fem_preds +male_preds # merge the two lists
-        
+            preds = fem_preds + male_preds  # merge the two lists
+
         # split the predictions into chunks of 3
-        chunk_preds = list(chunks(preds, 3)) #danish
+        chunk_preds = list(chunks(preds, 3))  # danish
 
         # get the false positive rates for the reflexive and anti-reflexive cases
         results = get_positive_preds(chunk_preds)
 
         # save the results in a dataframe
         if gender == "fem":
             df_fem = results
         elif gender == "male":
             df_male = results
         elif gender == "all_sents":
             df_all_sents = results
-    
-    return df_fem, df_male, df_all_sents #dicts 
 
-def logratio(x:float ,y:float):
-    return round(math.log2(x/ y), 2)
+    return df_fem, df_male, df_all_sents  # dicts
+
+
+def logratio(x: float, y: float):
+    return round(math.log2(x / y), 2)
+
+
+def eval_results(fem: dict, male: dict, all: dict, model_name: str):
+    """Evaluate the results of the coreference model on the ABC data."""
+
+    data = [
+        fem["tpr_reflexive"],
+        fem["fpr_anti_reflexive_female"],
+        fem["fpr_anti_reflexive_male"],
+        male["tpr_reflexive"],
+        male["fpr_anti_reflexive_female"],
+        male["fpr_anti_reflexive_male"],
+        all["tpr_reflexive"],
+        all["fpr_anti_reflexive_female"],
+        all["fpr_anti_reflexive_male"],
+    ]
+
+    mean_refl = np.mean([fem["tpr_reflexive"], male["tpr_reflexive"]])
+    mean_fem = np.mean(
+        [fem["fpr_anti_reflexive_female"], male["fpr_anti_reflexive_female"]]
+    )
+    mean_male = np.mean(
+        [fem["fpr_anti_reflexive_male"], male["fpr_anti_reflexive_male"]]
+    )
 
-def eval_results(fem:dict, male:dict, all:dict, model_name:str):
-    '''Evaluate the results of the coreference model on the ABC data.'''    
-    
-    data = [fem['tpr_reflexive'],
-           fem['fpr_anti_reflexive_female'], 
-           fem['fpr_anti_reflexive_male'], 
-
-           male['tpr_reflexive'], 
-           male['fpr_anti_reflexive_female'],
-           male['fpr_anti_reflexive_male'],
-           
-           all['tpr_reflexive'],
-           all['fpr_anti_reflexive_female'],
-           all['fpr_anti_reflexive_male']
-           ]
-    
-    mean_refl = np.mean([fem['tpr_reflexive'], male['tpr_reflexive']])
-    mean_fem = np.mean([fem['fpr_anti_reflexive_female'], male['fpr_anti_reflexive_female']])
-    mean_male = np.mean([fem['fpr_anti_reflexive_male'], male['fpr_anti_reflexive_male']])
-    
     gender_effect_size = logratio(mean_male, mean_fem)
 
-    data = [[round(data_,2) for data_ in data]]
-    
+    data = [[round(data_, 2) for data_ in data]]
+
     simlpe_data = {
-        f'Simple Output for {model_name}': ['', 'ABC', ''],
-        'Gender Effect Size': ['', gender_effect_size, ''],
-        'Pronoun': ['Female', 'Male', 'Reflexive'],
-        'Mean Rate of Detected Clusters': [mean_fem, mean_male, mean_refl]
+        f"Simple Output for {model_name}": ["", "ABC", ""],
+        "Gender Effect Size": ["", gender_effect_size, ""],
+        "Pronoun": ["Female", "Male", "Reflexive"],
+        "Mean Rate of Detected Clusters": [mean_fem, mean_male, mean_refl],
     }
 
     simlpe_data = pd.DataFrame(simlpe_data).T
 
     # Set the first row as the column names
     simlpe_data.columns = simlpe_data.iloc[0]
 
     # Drop the first row
     simple_df = simlpe_data.iloc[1:]
 
     detailed_data = {
-        f'Detailed Output for {model_name}': ['', '', 'ABC', '', '', '' ],
-        'Gender Effect Size': ['', '', gender_effect_size, '', '', ''],
-        'Pronoun': ['', 'Female', '', 'Male', '', 'Reflexive'],
-        'Mean Rate of Detected Clusters': ['', mean_fem, '', mean_male, '', mean_refl],
-        'Stereotypical Occupation': ['Female', 'Male', 'Female', 'Male', 'Female', 'Male'],
-        'Rate of Detected Clusters': [fem['fpr_anti_reflexive_female'], male['fpr_anti_reflexive_female'], fem['fpr_anti_reflexive_male'], male['fpr_anti_reflexive_male'], fem['tpr_reflexive'], male['tpr_reflexive']]
-        
+        f"Detailed Output for {model_name}": ["", "", "ABC", "", "", ""],
+        "Gender Effect Size": ["", "", gender_effect_size, "", "", ""],
+        "Pronoun": ["", "Female", "", "Male", "", "Reflexive"],
+        "Mean Rate of Detected Clusters": ["", mean_fem, "", mean_male, "", mean_refl],
+        "Stereotypical Occupation": [
+            "Female",
+            "Male",
+            "Female",
+            "Male",
+            "Female",
+            "Male",
+        ],
+        "Rate of Detected Clusters": [
+            fem["fpr_anti_reflexive_female"],
+            male["fpr_anti_reflexive_female"],
+            fem["fpr_anti_reflexive_male"],
+            male["fpr_anti_reflexive_male"],
+            fem["tpr_reflexive"],
+            male["tpr_reflexive"],
+        ],
     }
 
     detailed_data = pd.DataFrame(detailed_data).T
 
     # Set the first row as the column names
     detailed_data.columns = detailed_data.iloc[0]
 
     # Drop the first row
     detailed_df = detailed_data.iloc[1:]
     results = [simple_df, detailed_df]
 
-    return results
+    return results
```

### Comparing `genda_lens-0.0.2/genda_lens/coref_tasks/wino_utils.py` & `genda_lens-0.0.3/genda_lens/coref_tasks/wino_utils.py`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.2/genda_lens/data/DaWinoBias_anti_stereotyped_evalda.txt` & `genda_lens-0.0.3/genda_lens/data/DaWinoBias_anti_stereotyped_evalda.txt`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.2/genda_lens/data/DaWinoBias_pro_stereotyped_evalda.txt` & `genda_lens-0.0.3/genda_lens/data/DaWinoBias_pro_stereotyped_evalda.txt`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.2/genda_lens/data/abc_fem_sents.txt` & `genda_lens-0.0.3/genda_lens/data/abc_fem_sents.txt`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.2/genda_lens/data/abc_male_sents.txt` & `genda_lens-0.0.3/genda_lens/data/abc_male_sents.txt`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.2/genda_lens/data/name_aug_csv_files/first_names_2023_men.csv` & `genda_lens-0.0.3/genda_lens/data/name_aug_csv_files/first_names_2023_men.csv`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.2/genda_lens/data/name_aug_csv_files/first_names_2023_women.csv` & `genda_lens-0.0.3/genda_lens/data/name_aug_csv_files/first_names_2023_women.csv`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.2/genda_lens/data/name_aug_csv_files/last_names_2023.csv` & `genda_lens-0.0.3/genda_lens/data/name_aug_csv_files/last_names_2023.csv`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.2/genda_lens/data/name_aug_csv_files/overlapping_names.csv` & `genda_lens-0.0.3/genda_lens/data/name_aug_csv_files/overlapping_names.csv`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.2/genda_lens/data/name_aug_csv_files/unisex_names.csv` & `genda_lens-0.0.3/genda_lens/data/name_aug_csv_files/unisex_names.csv`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.2/genda_lens/genda_lens.py` & `genda_lens-0.0.3/genda_lens/genda_lens.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import warnings
+
 warnings.simplefilter("ignore", FutureWarning)
 
 
 class Evaluator:
     """Module for detecting gender bias in Danish language models."""
 
     def __init__(self, model_name):
         self.model_name = model_name
         print(
             f"[INFO] You can test {self.model_name} by running Evaluator.evaluate_<model type>()"
         )
 
-
     def evaluate_pretrained(
         self, test, mask_token=None, start_token=None, sep_token=None
     ):
         """Evaluate gender bias in a pre-trained model trained with masked language modeling.
 
         This function can be used for running two different tests:
         The Dawinobias Language Modeling Task and the ABC Language Modeling Task.
@@ -115,20 +115,17 @@
 
             results = evaluate_lm_winobias(
                 clf_rep_anti, clf_rep_pro, model_name=self.model_name
             )
 
         else:
             raise ValueError("Not a valid test. Choose between 'abc' and 'dawinobias'")
-        print(
-            "[INFO] output(list) generated. Access condensed output with output[0], and detailed output with with output[1]."
-        )
+        print("[INFO] Output generated.")
         return results
 
-
     def evaluate_ner(self, n):
         """Evaluate gender bias in a NER model.
         This function can be used for running the DaNe dataset test.
         Read more about the specifics of these test in the User Guide.
 
         Args:
             n (int): Number of repetitions to run the augmentation pipeline. To ensure robustness we recommend a value of n => 20.
@@ -181,17 +178,15 @@
             (muslim_m_aug, "Minority male names", n),
         ]
 
         # run model
         output = eval_model_augmentation(
             model, self.model_name, str(n), augmenters, testdata
         )
-        print(
-            "[INFO] output(list) generated. Access condensed output with output[0], and detailed output with with output[1]."
-        )
+        print("[INFO] Output generated.")
         return output
 
     def evaluate_coref(self, test, model):
         """Evaluate gender bias in a coreference model.
 
         This function can be used for running two different tests:
         The Dawinobias Language Coreference Task and the ABC Coreference Task.
@@ -279,17 +274,15 @@
             )
 
             results = eval_results(
                 df_fem, df_male, all_sents, model_name=self.model_name
             )
         else:
             raise ValueError("Not a valid test. Choose between 'abc' and 'dawinobias'")
-        print(
-            "[INFO] output(list) generated. Access condensed output with output[0], and detailed output with with output[1]."
-        )
+        print("[INFO] Output generated.")
         return results
 
 
 class Visualizer:
     """Module for visualizing results from the bias evaluation."""
 
     def __init__(self):
```

### Comparing `genda_lens-0.0.2/genda_lens/lm_tasks/wino_utils.py` & `genda_lens-0.0.3/genda_lens/lm_tasks/wino_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 """
 Utility functions for running the DaWinobias language modeling task.
 
 Builds on the codebase developed for the following project: 
 
 Title: “DaWinoBias: Assessing Occupational Gender Stereotypes in Danish NLP Models”
 Authors: Koppelgaard, K., Brødbæk, S. K.
@@ -19,181 +18,219 @@
 import spacy
 import torch
 from sklearn.metrics import classification_report
 from tqdm import tqdm
 
 
 def load_texts(filepath):
-    """load DaWinoBias texts - and shuffle data 
-    """    
+    """load DaWinoBias texts - and shuffle data"""
     with open(filepath) as file:
         text = file.read().splitlines()
     lines = [line.strip() for line in text]
     random.shuffle(lines)
     return lines
 
-def remove_sq_br(tokens):  
-    #input tokens to remove '[]' 
-    return [[token for token in tokens if token != '[' and token != ']']]
+
+def remove_sq_br(tokens):
+    # input tokens to remove '[]'
+    return [[token for token in tokens if token != "[" and token != "]"]]
+
 
 def idx_pron(tokens):
-    """Get index of pronoun in sentence
-    """    
-    #define pronouns
-    pronouns = ['hans', 'hendes', 'han', 'hun', 'ham', 'hende','▁hun', '▁hendes', '▁hende', '▁han', '▁hans', '▁ham']
-    # find idx of pronouns 
+    """Get index of pronoun in sentence"""
+    # define pronouns
+    pronouns = [
+        "hans",
+        "hendes",
+        "han",
+        "hun",
+        "ham",
+        "hende",
+        "▁hun",
+        "▁hendes",
+        "▁hende",
+        "▁han",
+        "▁hans",
+        "▁ham",
+    ]
+    # find idx of pronouns
     prons_idx = [tokens.index(i) for i in pronouns if i in tokens][0]
     return prons_idx
 
-def predict_masked(lines, condition, nlp, tokenizer, mask_token, model_name): 
+
+def predict_masked(lines, condition, nlp, tokenizer, mask_token, model_name):
     labels, preds = [], []
 
     print(f"[INFO] Running test on condition: {condition} sentences.")
     for idx, line in enumerate(tqdm(lines)):
         # tokenize and lowercase
         line_tokenized = tokenizer(line)
         tokens = [token.text.lower() for token in line_tokenized]
-        
+
         # remove square brackets from tokens
         tokens = remove_sq_br(tokens)[0]
 
         # find index of pronoun
         prons_idx = idx_pron(tokens)
 
-        #save correct pronoun
+        # save correct pronoun
         correct_pronoun = tokens[prons_idx]
-        
+
         # MASK pronouns
         tokens[prons_idx] = mask_token
-                 
-        # join sentence into one string 
-        if mask_token == '<mask>' and model_name == "vesteinn/DanskBert": 
-            sentence = ' '.join(tokens).replace(" <mask>", "<mask>")
-        else: 
-            sentence = ' '.join(tokens)
-        
+
+        # join sentence into one string
+        if mask_token == "<mask>" and model_name == "vesteinn/DanskBert":
+            sentence = " ".join(tokens).replace(" <mask>", "<mask>")
+        else:
+            sentence = " ".join(tokens)
+
         # compute fill-mask prediction
-        pred = nlp(sentence)[0]['token_str']
-        
+        pred = nlp(sentence)[0]["token_str"]
+
         # save labels and predictions
         labels.append(correct_pronoun)
         preds.append(pred)
-        
+
     return labels, preds
 
-def group_pronouns(pronouns): 
-    '''group labels in female and male pronouns'''
 
-    #define groups of pronouns
-    female_pronouns = ['hun', 'hendes', 'hende', '▁hun', '▁hendes', '▁hende']
-    male_pronouns = ['han', 'hans', 'ham', '▁han', '▁hans', '▁ham']
-
-    #initialize lists
-    group_pronoun= []
-
-    #group labels
-    for pronoun in pronouns: 
-        if pronoun in female_pronouns: 
-            group_pronoun.append('hun/hendes')
-        elif pronoun in male_pronouns: 
-            group_pronoun.append('han/hans')
+def group_pronouns(pronouns):
+    """group labels in female and male pronouns"""
+
+    # define groups of pronouns
+    female_pronouns = ["hun", "hendes", "hende", "▁hun", "▁hendes", "▁hende"]
+    male_pronouns = ["han", "hans", "ham", "▁han", "▁hans", "▁ham"]
+
+    # initialize lists
+    group_pronoun = []
+
+    # group labels
+    for pronoun in pronouns:
+        if pronoun in female_pronouns:
+            group_pronoun.append("hun/hendes")
+        elif pronoun in male_pronouns:
+            group_pronoun.append("han/hans")
         else:
-            group_pronoun.append('UNK')
+            group_pronoun.append("UNK")
     return group_pronoun
 
-def evaluate_model(labels, predictions): #, filename, model_name):
+
+def evaluate_model(labels, predictions):  # , filename, model_name):
     """Create and save classification report
-    Args: 
-        labels: labels 
+    Args:
+        labels: labels
         predictions: model predictions
     Returns:
         clf_report: classification report in pandas df format
     """
     # create df for storing metrics
-    df = pd.DataFrame(classification_report(labels,predictions,output_dict = True, zero_division=1)).round(decimals=2)
-    return df 
+    df = pd.DataFrame(
+        classification_report(labels, predictions, output_dict=True, zero_division=1)
+    ).round(decimals=2)
+    return df
 
 
-def run_winobias(tokenizer, nlp, mask_token, model_name): 
+def run_winobias(tokenizer, nlp, mask_token, model_name):
     # data paths
-    inpath_pro = os.path.join(Path(__file__).parents[1],"data","DaWinoBias_pro_stereotyped_evalda.txt")
-    inpath_anti = os.path.join(Path(__file__).parents[1],"data","DaWinoBias_anti_stereotyped_evalda.txt")
+    inpath_pro = os.path.join(
+        Path(__file__).parents[1], "data", "DaWinoBias_pro_stereotyped_evalda.txt"
+    )
+    inpath_anti = os.path.join(
+        Path(__file__).parents[1], "data", "DaWinoBias_anti_stereotyped_evalda.txt"
+    )
 
     # load data
     anti_sents = load_texts(inpath_anti)
     pro_sents = load_texts(inpath_pro)
 
     # mask and predict pronoun
-    anti_labels_, anti_preds_ = predict_masked(lines = anti_sents, condition = "anti-stereotypical", nlp = nlp, tokenizer = tokenizer, mask_token = mask_token, model_name = model_name)
-    pro_labels_, pro_preds_ = predict_masked(lines = pro_sents, condition = "pro-stereotypical", nlp = nlp, tokenizer = tokenizer, mask_token = mask_token, model_name = model_name)
+    anti_labels_, anti_preds_ = predict_masked(
+        lines=anti_sents,
+        condition="anti-stereotypical",
+        nlp=nlp,
+        tokenizer=tokenizer,
+        mask_token=mask_token,
+        model_name=model_name,
+    )
+    pro_labels_, pro_preds_ = predict_masked(
+        lines=pro_sents,
+        condition="pro-stereotypical",
+        nlp=nlp,
+        tokenizer=tokenizer,
+        mask_token=mask_token,
+        model_name=model_name,
+    )
+
+    # group pronouns into male/female category
+    anti_labels, anti_preds = group_pronouns(anti_labels_), group_pronouns(anti_preds_)
+    pro_labels, pro_preds = group_pronouns(pro_labels_), group_pronouns(pro_preds_)
+
+    # print( "[INFO] Raw predictions for model:", model_name)
+    # print("[INFO] Number of female pron. predictions:", len([i for i in anti_preds if i =='hun/hendes']))
+    # print("[INFO] Number of male pron. predictions:", len([i for i in anti_preds if i =='han/hans']))
+    # print("[INFO] Number of 'UNKNOWN' predictions:", len([i for i in anti_preds if i =='UNK']))
 
-    # group pronouns into male/female category 
-    anti_labels, anti_preds = group_pronouns(anti_labels_),group_pronouns(anti_preds_) 
-    pro_labels, pro_preds = group_pronouns(pro_labels_),group_pronouns(pro_preds_) 
-    print( "[INFO] Raw predictions for model:", model_name)
-    
-    print("[INFO] Number of female pron. predictions:", len([i for i in anti_preds if i =='hun/hendes']))
-    print("[INFO] Number of male pron. predictions:", len([i for i in anti_preds if i =='han/hans']))
-    print("[INFO] Number of 'UNKNOWN' predictions:", len([i for i in anti_preds if i =='UNK']))
-    
     # evaluate performance
     clf_rep_anti = evaluate_model(anti_labels, anti_preds)
     clf_rep_pro = evaluate_model(pro_labels, pro_preds)
-    
+
     return clf_rep_anti, clf_rep_pro
 
-def logratio(x:float ,y:float):
-    return round(math.log2(x/ y), 2)
+
+def logratio(x: float, y: float):
+    return round(math.log2(x / y), 2)
+
 
 def evaluate_lm_winobias(anti_res, pro_res, model_name):
     """Evaluate winobias coref experiment
     Args:
         anti_res: results for anti-stereotypical condition
         pro_res: results for pro-stereotypical condition
-        
+
     """
     # Gender Effect Size calculation
     anti_acc = anti_res["accuracy"].values[0]
     pro_acc = pro_res["accuracy"].values[0]
     gender_effect_size = logratio(pro_acc, anti_acc)
 
     anti_f1_fem_pron = anti_res["hun/hendes"].values[2]
     anti_f1_male_pron = anti_res["han/hans"].values[2]
 
     pro_f1_fem_pron = pro_res["hun/hendes"].values[2]
     pro_f1_male_pron = pro_res["han/hans"].values[2]
 
     simlpe_data = {
-        f'Simple Output for {model_name}': ['', 'DaWinoBias'],
-        'Gender Effect Size': ['', gender_effect_size],
-        'Condition': ['Anti-stereotypical','Pro-stereotypical'],
-        'Accuracy': [anti_acc, pro_acc]
-        }
+        f"Simple Output for {model_name}": ["", "DaWinoBias"],
+        "Gender Effect Size": ["", gender_effect_size],
+        "Condition": ["Anti-stereotypical", "Pro-stereotypical"],
+        "Accuracy": [anti_acc, pro_acc],
+    }
 
     simlpe_data = pd.DataFrame(simlpe_data).T
 
     # Set the first row as the column names
     simlpe_data.columns = simlpe_data.iloc[0]
 
     # Drop the first row
     simple_df = simlpe_data.iloc[1:]
-    
+
     detailed_data = {
-        f'Detailed Output for {model_name}': ['', 'DaWinoBias', '',''],
-        'Gender Effect Size': ['', gender_effect_size, '',''],
-        'Condition': ['Anti-stereotypical','', 'Pro-stereotypical', ''],
-        'Accuracy': [anti_acc, '', pro_acc, ''],
-        'Pronouns': ['Female', 'Male', 'Female', 'Male'],
-        'F1': [anti_f1_fem_pron, anti_f1_male_pron, pro_f1_fem_pron, pro_f1_male_pron]
-        }
+        f"Detailed Output for {model_name}": ["", "DaWinoBias", "", ""],
+        "Gender Effect Size": ["", gender_effect_size, "", ""],
+        "Condition": ["Anti-stereotypical", "", "Pro-stereotypical", ""],
+        "Accuracy": [anti_acc, "", pro_acc, ""],
+        "Pronouns": ["Female", "Male", "Female", "Male"],
+        "F1": [anti_f1_fem_pron, anti_f1_male_pron, pro_f1_fem_pron, pro_f1_male_pron],
+    }
 
     detailed_data = pd.DataFrame(detailed_data).T
 
     # Set the first row as the column names
     detailed_data.columns = detailed_data.iloc[0]
 
     # Drop the first row
     detailed_df = detailed_data.iloc[1:]
 
     results = [simple_df, detailed_df]
 
-    return results
+    return results
```

### Comparing `genda_lens-0.0.2/genda_lens/ner_tasks/augmentation.py` & `genda_lens-0.0.3/genda_lens/ner_tasks/augmentation.py`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.2/genda_lens/ner_tasks/performance.py` & `genda_lens-0.0.3/genda_lens/ner_tasks/performance.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,64 +12,71 @@
 import math
 import os
 
 import pandas as pd
 import spacy
 from dacy.score import score
 
+
 def load_mdl(model_name):
-    """Loading pre-trained model using DaCy or from Hugging Face via spacy_wrap 
+    """Loading pre-trained model using DaCy or from Hugging Face via spacy_wrap
 
     Args:
-        model_name (str): name of model in DaCy or on Hugging Face 
+        model_name (str): name of model in DaCy or on Hugging Face
 
     Raises:
         ValueError: raise error if HF model cannot be loaded from Hugging Face
-        ValueError: raise error if model type not supported in package 
+        ValueError: raise error if model type not supported in package
 
     Returns:
-        model: NER model  
-    """    
+        model: NER model
+    """
     import dacy
+
     if model_name in dacy.models():
         print(f"[INFO] Loading model {model_name} with DaCy.")
         import dacy
 
-        #model = dacy.load("da_dacy_large_trf-0.2.0")
+        # model = dacy.load("da_dacy_large_trf-0.2.0")
         model = dacy.load(model_name)
     elif model_name not in dacy.models():
         print(f"[INFO] Loading model {model_name} from Hugging Face with spaCy-wrap.")
         try:
-            #import spacy
+            # import spacy
             import spacy_wrap
+
             model = spacy.blank("da")
-            # config for loading 
-            config = {"model": {"name": model_name}, 
-                        "predictions_to": ["ents"]} 
+            # config for loading
+            config = {"model": {"name": model_name}, "predictions_to": ["ents"]}
             model.add_pipe("token_classification_transformer", config=config)
         except OSError:
-            raise ValueError("Cannot load model from Hugging Face. Please specify the full name of the model i.e. 'name/model-name' ")     
+            raise ValueError(
+                "Cannot load model from Hugging Face. Please specify the full name of the model i.e. 'name/model-name' "
+            )
     else:
-        raise ValueError("Cannot load model. This package only supports models from DaCy and Hugging Face.")
+        raise ValueError(
+            "Cannot load model. This package only supports models from DaCy and Hugging Face."
+        )
     return model
 
+
 def eval_model_augmentation(mdl, model_name, n, augmenters, dataset):
     """Compute NER performance on the DaNe test set using DaCy's score function
 
     Args:
-        mdl (model): NER model  
+        mdl (model): NER model
         model_name (str): model name
-        n (int): number of repetitions to run 
-        augmenters (generator): dictionary with name augmentaions to test 
-        dataset (corpus): the DaNe test set 
+        n (int): number of repetitions to run
+        augmenters (generator): dictionary with name augmentaions to test
+        dataset (corpus): the DaNe test set
 
     Returns:
-        list: list with two df's: output condensed and output detailed  
-    """    
-    # loop over all models in model_dict 
+        list: list with two df's: output condensed and output detailed
+    """
+    # loop over all models in model_dict
     scores = []
     i = 0
     for aug, nam, k in augmenters:
         print(f"\t [INFO] Running augmenter: {nam} with {k} repetitions.")
         scores_ = score(corpus=dataset, apply_fn=mdl, augmenters=aug, k=k)
         scores_["model"] = model_name
         scores_["augmenter"] = nam
@@ -84,73 +91,98 @@
     # compute simple and detailed output
     out_detailed = eval_ner_detailed(scores_summed, l_ratio, model_name)
 
     out_simple = eval_ner_simple(scores_summed, l_ratio, model_name)
 
     return [out_simple, out_detailed]
 
-def logratio(x:float ,y:float):
-    return round(math.log2(x/ y), 2)
+
+def logratio(x: float, y: float):
+    return round(math.log2(x / y), 2)
+
 
 def get_means_sds(df):
-    '''
+    """
     Compute mean F1 and SD for each augmenter of a single model.
 
     input:
-     - df with model performance of a single model. 
+     - df with model performance of a single model.
 
-    output: 
-    -  
-    '''
-    print(df.head())
-    df["f1"] = df["ents_excl_MISC_ents_f"] #*100
-    df = df[df["augmenter"].isin(["Majority female names", "Majority male names", "Minority male names", "Minority female names"])]
-    augs, means, sds = [],[],[]
+    output:
+    -
+    """
+    df["f1"] = df["ents_excl_MISC_ents_f"]  # *100
+    df = df[
+        df["augmenter"].isin(
+            [
+                "Majority female names",
+                "Majority male names",
+                "Minority male names",
+                "Minority female names",
+            ]
+        )
+    ]
+    augs, means, sds = [], [], []
     for aug in set(df["augmenter"]):
         augs.append(aug)
-        sub = df[df["augmenter"]==aug]
-        means.append(round(sub["f1"].mean(),4))
-        sds.append(round(sub["f1"].std(),2))
+        sub = df[df["augmenter"] == aug]
+        means.append(round(sub["f1"].mean(), 4))
+        sds.append(round(sub["f1"].std(), 2))
     # create df
     out_df = pd.DataFrame({"Group": augs, "F1": means, "SD": sds})
     # create df with mean and SD in one column
-    combinations = [str(str(a)+" ("+str(b)+")") for (a,b) in zip(means,sds)]
+    combinations = [str(str(a) + " (" + str(b) + ")") for (a, b) in zip(means, sds)]
     out_df_condensed = pd.DataFrame({"Group": augs, "F1 (SD)": combinations})
 
     # Compute log-ratio
-    f = out_df[out_df["Group"]=="Majority female names"].iloc[0,1]
-    m = out_df[out_df["Group"]=="Majority male names"].iloc[0,1]
-    ratio = logratio(m,f)  
+    f = out_df[out_df["Group"] == "Majority female names"].iloc[0, 1]
+    m = out_df[out_df["Group"] == "Majority male names"].iloc[0, 1]
+    ratio = logratio(m, f)
 
     return out_df_condensed, ratio
 
 
 def eval_ner_simple(df, l_ratio, model_name):
     data = {
-        f'Simple Output {model_name}': ['', 'Augmented DaNe', ''],
-        'Gender Effect Size': ['', l_ratio,''],
-        'Name Augmentation': ['Female', '', 'Male'],
-        'Macro F1 (SD)': [df[df["Group"]=="Majority female names"].iloc[0,1], '', 
-                     df[df["Group"]=="Majority male names"].iloc[0,1]],
+        f"Simple Output {model_name}": ["", "Augmented DaNe", ""],
+        "Gender Effect Size": ["", l_ratio, ""],
+        "Name Augmentation": ["Female", "", "Male"],
+        "Macro F1 (SD)": [
+            df[df["Group"] == "Majority female names"].iloc[0, 1],
+            "",
+            df[df["Group"] == "Majority male names"].iloc[0, 1],
+        ],
     }
     df_out = pd.DataFrame(data).T
     df_out.columns = df_out.iloc[0]
     df_out = df_out.iloc[1:]
     return df_out
 
+
 def eval_ner_detailed(df, l_ratio, model_name):
     data = {
-        f'Detailed Output for {model_name}': ['', 'Augmented DaNe', '', ''],
-        'Gender Effect Size': ['', l_ratio,'', ''],
-        'Name Augmentation': ['Female', '', 'Male', ''],
-        'Macro F1 (SD)': [df[df["Group"]=="Majority female names"].iloc[0,1],'', df[df["Group"]=="Majority male names"].iloc[0,1],''],
-        'Name Augmentation ': ['Majority Female', 'Minority Female', 'Majority Male', 'Minority Male'],
-        'Macro F1 (SD) ': [df[df["Group"]=="Majority female names"].iloc[0,1], 
-                      df[df["Group"]=="Minority female names"].iloc[0,1], 
-                      df[df["Group"]=="Majority male names"].iloc[0,1], 
-                      df[df["Group"]=="Minority male names"].iloc[0,1]]
+        f"Detailed Output for {model_name}": ["", "Augmented DaNe", "", ""],
+        "Gender Effect Size": ["", l_ratio, "", ""],
+        "Name Augmentation": ["Female", "", "Male", ""],
+        "Macro F1 (SD)": [
+            df[df["Group"] == "Majority female names"].iloc[0, 1],
+            "",
+            df[df["Group"] == "Majority male names"].iloc[0, 1],
+            "",
+        ],
+        "Name Augmentation ": [
+            "Majority Female",
+            "Minority Female",
+            "Majority Male",
+            "Minority Male",
+        ],
+        "Macro F1 (SD) ": [
+            df[df["Group"] == "Majority female names"].iloc[0, 1],
+            df[df["Group"] == "Minority female names"].iloc[0, 1],
+            df[df["Group"] == "Majority male names"].iloc[0, 1],
+            df[df["Group"] == "Minority male names"].iloc[0, 1],
+        ],
     }
     out_df = pd.DataFrame(data).T
     out_df.columns = out_df.iloc[0]
     out_df = out_df.iloc[1:]
     return out_df
-
```

### Comparing `genda_lens-0.0.2/genda_lens/ner_tasks/process_names.py` & `genda_lens-0.0.3/genda_lens/ner_tasks/process_names.py`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.2/PKG-INFO` & `genda_lens-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: genda-lens
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for quantifying bias in Danish language models.
 Home-page: https://github.com/DaDebias/genda-lens
 License: MIT
-Author: Rybner, Astrid. Rolskov, Thea
+Author: Astrid Rybner, Thea Rolskov
 Author-email: astrid.rybner@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: genda-lens Version: 0.0.2 Summary: A package for
+Metadata-Version: 2.1 Name: genda-lens Version: 0.0.3 Summary: A package for
 quantifying bias in Danish language models. Home-page: https://github.com/
-DaDebias/genda-lens License: MIT Author: Rybner, Astrid. Rolskov, Thea Author-
+DaDebias/genda-lens License: MIT Author: Astrid Rybner, Thea Rolskov Author-
 email: astrid.rybner@hotmail.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: augmenty (>=1.3.7,<1.4) Requires-Dist: dacy
 (>=2.7.1,<2.8) Requires-Dist: fairlearn (>=0.8.0,<0.9.0) Requires-Dist:
 matplotlib (>=3.7,<3.8) Requires-Dist: numpy (>=1.24,<1.25) Requires-Dist:
```

