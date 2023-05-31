# Comparing `tmp/pxtextmining-0.5.2.tar.gz` & `tmp/pxtextmining-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pxtextmining-0.5.2.tar", max compression
+gzip compressed data, was "pxtextmining-0.5.3.tar", max compression
```

## Comparing `pxtextmining-0.5.2.tar` & `pxtextmining-0.5.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1068 2022-11-17 15:31:00.811802 pxtextmining-0.5.2/LICENSE
--rw-r--r--   0        0        0      949 2023-04-03 08:21:59.385245 pxtextmining-0.5.2/README.md
--rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.2/pxtextmining/__init__.py
--rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.2/pxtextmining/factories/__init__.py
--rw-r--r--   0        0        0    12184 2023-04-27 10:50:35.275927 pxtextmining-0.5.2/pxtextmining/factories/factory_data_load_and_split.py
--rw-r--r--   0        0        0     7047 2023-04-27 11:01:34.635944 pxtextmining-0.5.2/pxtextmining/factories/factory_model_performance.py
--rw-r--r--   0        0        0    17408 2023-04-27 14:20:24.575856 pxtextmining-0.5.2/pxtextmining/factories/factory_pipeline.py
--rw-r--r--   0        0        0    10996 2023-04-27 11:01:34.635944 pxtextmining-0.5.2/pxtextmining/factories/factory_predict_unlabelled_text.py
--rw-r--r--   0        0        0     3529 2023-04-27 11:01:34.635944 pxtextmining-0.5.2/pxtextmining/factories/factory_write_results.py
--rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.2/pxtextmining/helpers/__init__.py
--rw-r--r--   0        0        0      945 2023-04-03 08:21:49.655245 pxtextmining-0.5.2/pxtextmining/helpers/text_preprocessor.py
--rw-r--r--   0        0        0      688 2023-04-03 08:21:49.655245 pxtextmining-0.5.2/pxtextmining/helpers/tokenization.py
--rw-r--r--   0        0        0     6918 2023-04-27 10:50:35.275927 pxtextmining-0.5.2/pxtextmining/params.py
--rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.2/pxtextmining/pipelines/__init__.py
--rw-r--r--   0        0        0    11542 2023-04-27 11:01:34.635944 pxtextmining-0.5.2/pxtextmining/pipelines/multilabel_pipeline.py
--rw-r--r--   0        0        0     1082 2023-04-27 14:30:31.355856 pxtextmining-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1966 1970-01-01 00:00:00.000000 pxtextmining-0.5.2/setup.py
--rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 pxtextmining-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-11-17 15:31:00.811802 pxtextmining-0.5.3/LICENSE
+-rw-r--r--   0        0        0      949 2023-04-03 08:21:59.385245 pxtextmining-0.5.3/README.md
+-rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.3/pxtextmining/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.3/pxtextmining/factories/__init__.py
+-rw-r--r--   0        0        0    11885 2023-05-31 08:46:58.592917 pxtextmining-0.5.3/pxtextmining/factories/factory_data_load_and_split.py
+-rw-r--r--   0        0        0     9562 2023-05-31 08:46:58.592917 pxtextmining-0.5.3/pxtextmining/factories/factory_model_performance.py
+-rw-r--r--   0        0        0    22115 2023-05-31 08:46:58.592917 pxtextmining-0.5.3/pxtextmining/factories/factory_pipeline.py
+-rw-r--r--   0        0        0    12046 2023-05-31 08:46:58.592917 pxtextmining-0.5.3/pxtextmining/factories/factory_predict_unlabelled_text.py
+-rw-r--r--   0        0        0     4509 2023-05-31 08:46:58.592917 pxtextmining-0.5.3/pxtextmining/factories/factory_write_results.py
+-rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.3/pxtextmining/helpers/__init__.py
+-rw-r--r--   0        0        0      945 2023-04-03 08:21:49.655245 pxtextmining-0.5.3/pxtextmining/helpers/text_preprocessor.py
+-rw-r--r--   0        0        0      625 2023-05-31 08:46:58.592917 pxtextmining-0.5.3/pxtextmining/helpers/tokenization.py
+-rw-r--r--   0        0        0     6727 2023-05-31 08:46:58.592917 pxtextmining-0.5.3/pxtextmining/params.py
+-rw-r--r--   0        0        0        0 2022-11-17 15:31:00.861802 pxtextmining-0.5.3/pxtextmining/pipelines/__init__.py
+-rw-r--r--   0        0        0    11682 2023-05-31 08:46:58.592917 pxtextmining-0.5.3/pxtextmining/pipelines/multilabel_pipeline.py
+-rw-r--r--   0        0        0     5531 2023-05-31 08:46:58.592917 pxtextmining-0.5.3/pxtextmining/pipelines/sentiment_pipeline.py
+-rw-r--r--   0        0        0     1167 2023-05-31 08:46:58.592917 pxtextmining-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1992 1970-01-01 00:00:00.000000 pxtextmining-0.5.3/setup.py
+-rw-r--r--   0        0        0     2101 1970-01-01 00:00:00.000000 pxtextmining-0.5.3/PKG-INFO
```

### Comparing `pxtextmining-0.5.2/LICENSE` & `pxtextmining-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pxtextmining-0.5.2/README.md` & `pxtextmining-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pxtextmining-0.5.2/pxtextmining/factories/factory_data_load_and_split.py` & `pxtextmining-0.5.3/pxtextmining/factories/factory_data_load_and_split.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,22 @@
 import numpy as np
 import pandas as pd
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import OneHotEncoder
 from tensorflow.data import Dataset
 from transformers import AutoTokenizer
 
-from pxtextmining.params import minor_cats,  dataset, major_cat_dict, merged_minor_cats
+from pxtextmining.params import (
+    minor_cats,
+    dataset,
+    major_cat_dict,
+    merged_minor_cats,
+    q_map,
+)
+
 
 def merge_categories(df, new_cat, cats_to_merge):
     """Merges categories together in a dataset. Assumes all categories are all in the right format, one hot encoded with int values.
 
     Args:
         df (pd.DataFrame): DataFrame with labelled data.
         new_cat (str): Name for new column of merged data.
@@ -20,17 +27,17 @@
 
     Returns:
         (pd.DataFrame): DataFrame with new columns
     """
     df[new_cat] = np.NaN
     for cat in cats_to_merge:
         print(f"Number of {cat} labels: {df[cat].sum()}")
-        df[new_cat] = df[new_cat].mask(df[cat] == 1, other = 1)
+        df[new_cat] = df[new_cat].mask(df[cat] == 1, other=1)
     print(f"Number of new label {new_cat}: {df[new_cat].sum()}")
-    df = df.drop(columns = cats_to_merge)
+    df = df.drop(columns=cats_to_merge)
     return df
 
 
 def bert_data_to_dataset(
     X,
     Y=None,
     max_length=150,
@@ -50,23 +57,35 @@
         additional_features (bool, optional): Whether additional features are to be included, currently this is only question type
             in 'FFT_q_standardised' column. Defaults to False.
 
     Returns:
         (tf.data.Dataset OR dict): `tf.data.Dataset` if Y is provided, `dict` otherwise.
     """
     tokenizer = AutoTokenizer.from_pretrained(model_name)
-    data_encoded = dict(
-        tokenizer(
-            list(X["FFT answer"]),
-            truncation=True,
-            padding=True,
-            max_length=max_length,
-            return_tensors="tf",
+    try:
+        data_encoded = dict(
+            tokenizer(
+                list(X["FFT answer"]),
+                truncation=True,
+                padding=True,
+                max_length=max_length,
+                return_tensors="tf",
+            )
         )
-    )
+    except:
+        data_encoded = dict(
+            tokenizer(
+                list(X),
+                truncation=True,
+                padding=True,
+                max_length=max_length,
+                return_tensors="tf",
+            )
+        )
+    data_encoded.pop("attention_mask", None)
     if additional_features == True:
         onehotted = onehot(X, "FFT_q_standardised")
         data_encoded["input_cat"] = onehotted.astype(np.float32)
     if Y is not None:
         data_encoded = Dataset.from_tensor_slices((data_encoded, Y))
     return data_encoded
 
@@ -91,42 +110,31 @@
     print(f"Shape of raw data is {raw_data.shape}")
     raw_data.columns = raw_data.columns.str.strip()
     raw_data = raw_data.set_index("Comment ID").copy()
     features = ["FFT categorical answer", "FFT question", "FFT answer"]
     # For now the labels are hardcoded, these are subject to change as framework is in progress
     if target in ["minor_categories", "major_categories"]:
         cols = minor_cats
-    if target == 'test':
+    if target == "test":
         cols = merged_minor_cats
     elif target == "sentiment":
         cols = ["Comment sentiment"]
     # Sort out the features first
     features_df = raw_data.loc[:, features].copy()
     features_df = clean_empty_features(features_df)
     # Standardize FFT qs
-    q_map = {
-        "Please tell us why": "nonspecific",
-        "Please tells us why you gave this answer?": "nonspecific",
-        "FFT Why?": "nonspecific",
-        "What was good?": "what_good",
-        "Is there anything we could have done better?": "could_improve",
-        "How could we improve?": "could_improve",
-        "What could we do better?": "could_improve",
-        "Please can you tell us why you gave your answer and what we could have done better?": "nonspecific",
-        "Please describe any things about the 111 service that\r\nyou were particularly satisfied and/or dissatisfied with": "nonspecific",
-        "Please describe any things about the 111 service that\nyou were particularly satisfied and/or dissatisfied with": 'nonspecific',
-        "Nonspecific": 'nonspecific'
-    }
     features_df.loc[:, "FFT_q_standardised"] = (
         features_df.loc[:, "FFT question"].map(q_map).copy()
     )
     if features_df["FFT_q_standardised"].count() != features_df.shape[0]:
-        raise ValueError(f'Check q_map is correct. features_df.shape[0] is {features_df.shape[0]}. \n \
+        raise ValueError(
+            f'Check q_map is correct. features_df.shape[0] is {features_df.shape[0]}. \n \
                          features_df["FFT_q_standardised"].count()  is {features_df["FFT_q_standardised"].count()}. \n\n\
-                         Questions are: {features_df["FFT question"].value_counts()}')
+                         Questions are: {features_df["FFT question"].value_counts()}'
+        )
     features_df.loc[:, "text_length"] = features_df.loc[:, "FFT answer"].apply(
         lambda x: len([word for word in str(x).split(" ") if word != ""])
     )
     # Sort out the targets
     targets_df = raw_data.loc[:, cols].copy()
     targets_df = targets_df.replace("1", 1)
     targets_df = targets_df.fillna(value=0)
@@ -137,15 +145,15 @@
     targets_df.loc[:, "num_labels"] = targets_df.loc[:, cols].sum(axis=1)
     targets_df = targets_df[targets_df["num_labels"] != 0]
     targets_df = targets_df.fillna(value=0)
     # merge two together
     combined_df = pd.merge(features_df, targets_df, left_index=True, right_index=True)
     combined_df = combined_df.reset_index()
     combined_df = combined_df.drop_duplicates()
-    combined_df = combined_df.set_index('Comment ID')
+    combined_df = combined_df.set_index("Comment ID")
     print(f"Shape of cleaned data is {combined_df.shape}")
     return combined_df
 
 
 def clean_empty_features(text_dataframe):
     """Replaces all empty whitespaces in a dataframe with np.NaN.
 
@@ -171,17 +179,15 @@
         (pd.DataFrame): One-hot encoded data
     """
     encoder = OneHotEncoder(sparse=False)
     col_encoded = encoder.fit_transform(df[[col_to_onehot]])
     return col_encoded
 
 
-def process_multilabel_data(
-    df, target, preprocess_text=True, additional_features=False
-):
+def process_data(df, target, preprocess_text=True, additional_features=False):
     """Utilises remove_punc_and_nums and clean_empty_features functions to clean the text data and
     drop any rows that are only whitespace after cleaning. Also fills one-hot encoded columns with
     0s rather than NaNs so that Y target is not sparse.
 
     Args:
         df (pd.DataFrame): DataFrame containing text data, any additional features, and targets
         target (list): List of column names of targets
@@ -189,35 +195,41 @@
             an sklearn model then should be True. If utilising transformer-based BERT model then should be set to False.
             Defaults to True.
         additional_features (bool, optional): Whether or not 'question type' feature should be included. Defaults to False.
 
     Returns:
         (tuple): Tuple containing two pd.DataFrames. The first contains the X features (text, with or without question type depending on additional_features), the second contains the one-hot encoded Y targets
     """
-    Y = df[target].fillna(value=0)
+
     if preprocess_text == True:
         X = df["FFT answer"].astype(str).apply(remove_punc_and_nums)
         X = clean_empty_features(X)
         print(f"After preprocessing, shape of X is {X.shape}")
     if preprocess_text == False:
         X = df["FFT answer"].astype(str)
     if additional_features == True:
-        X = pd.merge(X, df[['FFT_q_standardised']], left_index = True, right_index = True)
+        X = pd.merge(X, df[["FFT_q_standardised"]], left_index=True, right_index=True)
         X = X.reset_index()
         X = X.drop_duplicates()
-        X = X.set_index('Comment ID')
+        X = X.set_index("Comment ID")
+    if target == "sentiment":
+        Y = df["Comment sentiment"].astype(int) - 1
+    else:
+        Y = df[target].fillna(value=0)
     Y = Y.loc[X.index]
     Y = Y.reset_index()
     Y = Y.drop_duplicates()
-    Y = Y.set_index('Comment ID')
+    Y = Y.set_index("Comment ID")
+    if target == "sentiment":
+        Y = Y["Comment sentiment"]
     Y = np.array(Y).astype(int)
     return X, Y
 
 
-def process_and_split_multilabel_data(
+def process_and_split_data(
     df,
     target,
     preprocess_text=True,
     additional_features=False,
     random_state=42,
 ):
     """Combines the process_multilabel_data and train_test_split functions into one function
@@ -230,15 +242,15 @@
             Defaults to True.
         additional_features (bool, optional): Whether or not 'question type' feature should be included. Defaults to False.
         random_state (int, optional): Controls the shuffling applied to the data before applying the split. Enables reproducible output across multiple function calls. Defaults to 42.
 
     Returns:
         (list): List containing train-test split of preprocessed X features and Y targets.
     """
-    X, Y = process_multilabel_data(
+    X, Y = process_data(
         df,
         target,
         preprocess_text=preprocess_text,
         additional_features=additional_features,
     )
     X_train, X_test, Y_train, Y_test = train_test_split(
         X, Y, test_size=0.2, random_state=random_state
@@ -271,13 +283,13 @@
     for word in text_split:
         text_lower.append(word.lower())
     cleaned_sentence = " ".join(word for word in text_lower)
     cleaned_sentence = cleaned_sentence.strip()
     return cleaned_sentence
 
 
-if __name__ == '__main__':
-    df = load_multilabel_data(dataset, target = 'major_categories')
+if __name__ == "__main__":
+    df = load_multilabel_data(dataset, target="major_categories")
     print(df.shape)
     print(df.head())
     for i in df.columns:
         print(f"{i}: {df[i].dtype}")
```

### Comparing `pxtextmining-0.5.2/pxtextmining/factories/factory_model_performance.py` & `pxtextmining-0.5.3/pxtextmining/factories/factory_model_performance.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import numpy as np
 import pandas as pd
 from sklearn import metrics
 from sklearn.dummy import DummyClassifier
 from sklearn.metrics import confusion_matrix
+from tensorflow.keras.models import Model
+from sklearn.base import is_classifier
 
 from pxtextmining.factories.factory_predict_unlabelled_text import (
     fix_no_labels,
     predict_with_bert,
     turn_probs_into_binary,
-    predict_with_probs,
+    predict_multiclass_bert,
     predict_multilabel_sklearn
 )
 
 
 def get_dummy_model(x_train, y_train):
     """Creates dummy model that randomly predicts labels, fitted on the training data.
 
@@ -23,14 +25,61 @@
     Returns:
         (sklearn.dummy.DummyClassifier): Trained dummy classifier.
     """
     model = DummyClassifier(strategy="uniform")
     model.fit(x_train, y_train)
     return model
 
+
+def get_multiclass_metrics(x_test, y_test, labels, random_state, model, additional_features, training_time = None):
+    """Creates a string detailing various performance metrics for a multiclass model, which can then be written to
+    a text file.
+
+    Args:
+        x_test (pd.DataFrame): DataFrame containing test dataset features
+        y_test (pd.DataFrame): DataFrame containing test dataset true target values
+        labels (list): List containing the target labels
+        random_state (int): Seed used to control the shuffling of the data, to enable reproducible results.
+        model (tf.keras or sklearn model): Trained estimator.
+        additional_features (bool, optional): Whether or not additional features (e.g. question type) have been included in training the model. Defaults to False.
+        training_time (str, optional): Amount of time taken for model to train. Defaults to None.
+
+    Raises:
+        ValueError: Only models built with sklearn or tensorflow are allowed.
+
+    Returns:
+        (str): String containing the model architecture/hyperparameters, random state used for the train test split, and classification report.
+    """
+    metrics_string = "\n *****************"
+    metrics_string += (
+        f"\n Random state seed for train test split is: {random_state} \n\n"
+    )
+    # TF Keras models output probabilities with model.predict, whilst sklearn models output binary outcomes
+    # Get them both to output the same (binary outcomes) and take max prob as label if no labels predicted at all
+    if isinstance(model, Model) == True:
+        stringlist = []
+        model.summary(print_fn=lambda x: stringlist.append(x))
+        model_summary = "\n".join(stringlist)
+        metrics_string += f"\n{model_summary}\n"
+        y_pred = predict_multiclass_bert(x_test, model, additional_features = additional_features, already_encoded = False)
+    elif is_classifier(model) == True:
+        metrics_string += f"\n{model}\n"
+        y_pred = model.predict(x_test)
+    else:
+        raise ValueError('Model type not recognised')
+    # Calculate various metrics
+    metrics_string += f"\n\nTraining time: {training_time}\n"
+    # Classification report
+    metrics_string += "\n\n Classification report:\n"
+    c_report_str = metrics.classification_report(
+        y_test, y_pred, target_names=labels, zero_division=0
+    )
+    metrics_string += c_report_str
+    return metrics_string
+
 def get_multilabel_metrics(
     x_test,
     y_test,
     labels,
     random_state,
     model_type,
     model,
@@ -109,19 +158,21 @@
     metrics_string += c_report_str
     return metrics_string
 
 
 def get_accuracy_per_class(y_test, pred):
     """Function to produce accuracy per class for the predicted categories, compared against real values.
 
-    :param pd.Series y_test: Test data (real target values).
-    :param pd.Series pred: Predicted target values.
+    Args:
+        y_test (pd.Series): Test data (real target values).
+        pred (pd.Series): Predicted target values.
+
+    Returns:
+        (pd.DataFrame): The computed accuracy per class metrics for the model.
 
-    :return: The computed accuracy per class metrics for the model.
-    :rtype: pd.DataFrame
     """
     cm = confusion_matrix(y_test, pred)
     accuracy_per_class = cm.astype("float") / cm.sum(axis=1)[:, np.newaxis]
     accuracy_per_class = pd.DataFrame(accuracy_per_class.diagonal())
     accuracy_per_class.columns = ["accuracy"]
     unique, frequency = np.unique(y_test, return_counts=True)
     accuracy_per_class["class"], accuracy_per_class["counts"] = unique, frequency
```

### Comparing `pxtextmining-0.5.2/pxtextmining/factories/factory_pipeline.py` & `pxtextmining-0.5.3/pxtextmining/factories/factory_pipeline.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,71 +15,179 @@
 from sklearn.svm import SVC
 from sklearn.utils.class_weight import compute_class_weight
 from sklearn.model_selection import cross_validate
 from tensorflow.keras import Sequential, layers
 from tensorflow.keras.callbacks import EarlyStopping
 from tensorflow.keras.initializers import TruncatedNormal
 from tensorflow.keras.layers import Dense, Dropout, Input, concatenate
-from tensorflow.keras.losses import BinaryCrossentropy
+from tensorflow.keras.losses import BinaryCrossentropy, CategoricalCrossentropy
 from tensorflow.keras.models import Model
 from tensorflow.keras.optimizers import Adam
 from transformers import DistilBertConfig, TFDistilBertForSequenceClassification
+import xgboost as xgb
 
 from pxtextmining.helpers.tokenization import spacy_tokenizer
 from pxtextmining.params import model_name
 
 model_name = model_name
 
-def create_bert_model(Y_train, model_name=model_name, max_length=150):
+
+def create_sklearn_pipeline_sentiment(
+    model_type, num_classes, tokenizer=None, additional_features=False
+):
+    """Creates sklearn pipeline and hyperparameter grid for searching, for a multiclass target.
+
+    Args:
+        model_type (str): Allows for selection of different estimators. Permitted values are "svm" (Support Vector Classifier), or "xgb" (XGBoost).
+        num_classes (int): Number of target classes.
+        tokenizer (str, optional): Allows for selection of "spacy" tokenizer. Defaults to None, which is the default sklearn tokenizer
+        additional_features (bool, optional): Whether or not additional features (question type, text length) are to be included in the features fed into the model. Defaults to True.
+
+    Returns:
+        (tuple): Tuple containing the `sklearn.pipeline.Pipeline` with the selected estimator, and a `dict` containing the hyperparameters to be tuned.
+
+    """
+    if additional_features == True:
+        cat_transformer = OneHotEncoder(handle_unknown="ignore")
+        vectorizer = create_sklearn_vectorizer(tokenizer=None)
+        preproc = make_column_transformer(
+            (cat_transformer, ["FFT_q_standardised"]),
+            (vectorizer, "FFT answer"),
+        )
+        params = {
+            "columntransformer__tfidfvectorizer__ngram_range": ((1, 1), (1, 2), (2, 2)),
+            "columntransformer__tfidfvectorizer__max_df": [
+                0.85,
+                0.86,
+                0.87,
+                0.88,
+                0.89,
+                0.9,
+                0.91,
+                0.92,
+                0.93,
+                0.94,
+                0.95,
+                0.96,
+                0.97,
+                0.98,
+                0.99,
+            ],
+            "columntransformer__tfidfvectorizer__min_df": stats.uniform(0, 0.1),
+        }
+    else:
+        preproc = create_sklearn_vectorizer(tokenizer=tokenizer)
+        params = {
+            "tfidfvectorizer__ngram_range": ((1, 1), (1, 2), (2, 2)),
+            "tfidfvectorizer__max_df": [
+                0.85,
+                0.86,
+                0.87,
+                0.88,
+                0.89,
+                0.9,
+                0.91,
+                0.92,
+                0.93,
+                0.94,
+                0.95,
+                0.96,
+                0.97,
+                0.98,
+                0.99,
+            ],
+            "tfidfvectorizer__min_df": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
+        }
+    if model_type == "svm":
+        pipe = make_pipeline(
+            preproc,
+            SVC(
+                probability=True,
+                class_weight="balanced",
+                max_iter=1000,
+                cache_size=1000,
+            ),
+        )
+        params["svc__C"] = stats.uniform(0.1, 20)
+        params["svc__kernel"] = [
+            "linear",
+            "rbf",
+            "sigmoid",
+        ]
+    if model_type == "xgb":
+        pipe = make_pipeline(
+            preproc,
+            xgb.XGBClassifier(
+                num_class=num_classes, objective="multi:softmax", n_estimators=500
+            ),
+        )
+        params["xgbclassifier__max_depth"] = [4, 5, 6, 7, 8]
+        params["xgbclassifier__min_child_weight"] = [0.5, 1, 2, 5]
+        params["xgbclassifier__gamma"] = [0, 0.1, 0.2, 0.3, 0.4, 0.5]
+    return pipe, params
+
+
+def create_bert_model(Y_train, model_name=model_name, max_length=150, multilabel=True):
     """Creates Transformer based model trained on text data, with last layer added on
     for multilabel classification task. Number of neurons in last layer depends on number of labels in Y target.
 
     Args:
         Y_train (pd.DataFrame): DataFrame containing one-hot encoded targets
         model_name (str, optional): Type of pretrained transformer model to load. Defaults to `model_name` set in `pxtextmining.params`
         max_length (int, optional): Maximum length of text to be passed through transformer model. Defaults to 150.
+        multilabel (Bool, optional): Whether the target is multilabel or not. If set to False, target is multiclass. Defaults to True.
 
     Returns:
         (tensorflow.keras.models.Model): Compiled Tensforflow Keras model with pretrained transformer layers and last layer suited for multilabel classification task
     """
     config = DistilBertConfig.from_pretrained(model_name)
     transformer_model = TFDistilBertForSequenceClassification.from_pretrained(
         model_name, output_hidden_states=False
     )
     bert = transformer_model.layers[0]
     input_ids = Input(shape=(max_length,), name="input_ids", dtype="int32")
     inputs = {"input_ids": input_ids}
     bert_model = bert(inputs)[0][:, 0, :]
     dropout = Dropout(config.dropout, name="pooled_output")
     pooled_output = dropout(bert_model, training=False)
-    output = Dense(
-        units=Y_train.shape[1],
-        kernel_initializer=TruncatedNormal(stddev=config.initializer_range),
-        activation="sigmoid",
-        name="output",
-    )(pooled_output)
-    model = Model(inputs=inputs, outputs=output, name="BERT_MultiLabel")
+    if multilabel == True:
+        output = Dense(
+            units=Y_train.shape[1],
+            kernel_initializer=TruncatedNormal(stddev=config.initializer_range),
+            activation="sigmoid",
+            name="output",
+        )(pooled_output)
+        loss = BinaryCrossentropy()
+    else:
+        output = Dense(
+            units=Y_train.shape[1],
+            kernel_initializer=TruncatedNormal(stddev=config.initializer_range),
+            activation="softmax",
+            name="output",
+        )(pooled_output)
+        loss = CategoricalCrossentropy()
+    model = Model(inputs=inputs, outputs=output, name="DistilBERT")
     # compile model
-    loss = BinaryCrossentropy()
     optimizer = Adam(5e-5)
     metrics = ["CategoricalAccuracy"]
     model.compile(optimizer=optimizer, loss=loss, metrics=metrics)
     return model
 
 
 def create_bert_model_additional_features(
-    Y_train, model_name=model_name, max_length=150
+    Y_train, model_name=model_name, max_length=150, multilabel=True
 ):
     """Creates Transformer based model trained on text data, concatenated with an additional Dense layer taking additional inputs, with last layer added on
     for multilabel classification task. Number of neurons in last layer depends on number of labels in Y target.
 
     Args:
         Y_train (pd.DataFrame): DataFrame containing one-hot encoded targets
         model_name (str, optional): Type of pretrained transformer model to load. Defaults to `model_name` set in `pxtextmining.params`
         max_length (int, optional): Maximum length of text to be passed through transformer model. Defaults to 150.
+        multilabel (Bool, optional): Whether the target is multilabel or not. If set to False, target is multiclass. Defaults to True.
 
     Returns:
         (tensorflow.keras.models.Model): Compiled Tensforflow Keras model with pretrained transformer layers, three question_type inputs passed through a Dense layer, and last layer suited for multilabel classification task
 
     """
     config = DistilBertConfig.from_pretrained(model_name)
     transformer_model = TFDistilBertForSequenceClassification.from_pretrained(
@@ -93,22 +201,31 @@
     bert_output = dropout(bert_model, training=False)
     # Get onehotencoded categories in (3 categories)
     input_cat = Input(shape=(3,), name="input_cat")
     cat_dense = Dense(units=10, activation="relu")
     cat_dense = cat_dense(input_cat)
     # concatenate both together
     concat_layer = concatenate([bert_output, cat_dense])
-    output = Dense(
-        units=Y_train.shape[1],
-        kernel_initializer=TruncatedNormal(stddev=config.initializer_range),
-        activation="sigmoid",
-        name="output",
-    )(concat_layer)
-    model = Model(inputs=[input_ids, input_cat], outputs=output, name="BERT_MultiLabel")
-    loss = BinaryCrossentropy()
+    if multilabel == True:
+        output = Dense(
+            units=Y_train.shape[1],
+            kernel_initializer=TruncatedNormal(stddev=config.initializer_range),
+            activation="sigmoid",
+            name="output",
+        )(concat_layer)
+        loss = BinaryCrossentropy()
+    else:
+        output = Dense(
+            units=Y_train.shape[1],
+            kernel_initializer=TruncatedNormal(stddev=config.initializer_range),
+            activation="softmax",
+            name="output",
+        )(concat_layer)
+        loss = CategoricalCrossentropy()
+    model = Model(inputs=[input_ids, input_cat], outputs=output)
     optimizer = Adam(5e-5)
     metrics = ["CategoricalAccuracy"]
     model.compile(optimizer=optimizer, loss=loss, metrics=metrics)
     return model
 
 
 def train_bert_model(
@@ -251,15 +368,31 @@
         preproc = make_column_transformer(
             (cat_transformer, ["FFT_q_standardised"]),
             (vectorizer, "FFT answer"),
             # (num_transformer, ["text_length"]),
         )
         params = {
             "columntransformer__tfidfvectorizer__ngram_range": ((1, 1), (1, 2), (2, 2)),
-            "columntransformer__tfidfvectorizer__max_df": [0.85,0.86,0.87,0.88,0.89,0.9,0.91,0.92,0.93,0.94,0.95,0.96,0.97,0.98,0.99],
+            "columntransformer__tfidfvectorizer__max_df": [
+                0.85,
+                0.86,
+                0.87,
+                0.88,
+                0.89,
+                0.9,
+                0.91,
+                0.92,
+                0.93,
+                0.94,
+                0.95,
+                0.96,
+                0.97,
+                0.98,
+                0.99,
+            ],
             "columntransformer__tfidfvectorizer__min_df": stats.uniform(0, 0.1),
         }
     else:
         preproc = create_sklearn_vectorizer(tokenizer=tokenizer)
         params = {
             "tfidfvectorizer__ngram_range": ((1, 1), (1, 2), (2, 2)),
             "tfidfvectorizer__max_df": stats.uniform(0.8, 1),
@@ -298,21 +431,23 @@
         params["randomforestclassifier__class_weight"] = [
             "balanced",
             "balanced_subsample",
             None,
         ]
         params["randomforestclassifier__min_samples_leaf"] = stats.randint(1, 10)
         params["randomforestclassifier__max_features"] = ["sqrt", "log2", None, 0.3]
-    if model_type == 'xgb':
+    if model_type == "xgb":
         pipe = make_pipeline(preproc, xgb.XGBClassifier(tree_method="hist"))
 
     return pipe, params
 
 
-def search_sklearn_pipelines(X_train, Y_train, models_to_try, additional_features=True):
+def search_sklearn_pipelines(
+    X_train, Y_train, models_to_try, target=None, additional_features=True
+):
     """Iterates through selected estimators, instantiating the relevant sklearn pipelines and searching for the optimum hyperparameters.
 
     Args:
         X_train (pd.DataFrame): DataFrame containing the features to be fed into the estimator
         Y_train (pd.DataFrame): DataFrame containing the targets
         models_to_try (list): List containing the estimator types to be tried. Permitted values are "mnb" (Multinomial Naive Bayes), "knn" (K Nearest Neighbours), "svm" (Support Vector Classifier), or "rfc" (Random Forest Classifier).
         additional_features (bool, optional): Whether or not additional features (question type, text length) are to be included in the features fed into the model. Defaults to True.
@@ -327,26 +462,35 @@
     training_times = []
     for model_type in models_to_try:
         if model_type not in ["mnb", "knn", "svm", "rfc", "xgb"]:
             raise ValueError(
                 "Please choose valid model_type. Options are mnb, knn, svm, xgb or rfc"
             )
         else:
-            if additional_features == False:
-                pipe, params = create_sklearn_pipeline(
-                    model_type, additional_features=False
+            if target == "sentiment":
+                num_classes = len(np.unique(Y_train))
+                pipe, params = create_sklearn_pipeline_sentiment(
+                    model_type,
+                    num_classes=num_classes,
+                    tokenizer=None,
+                    additional_features=additional_features,
                 )
-            elif additional_features == True:
+            else:
                 pipe, params = create_sklearn_pipeline(
-                    model_type, additional_features=True
+                    model_type, additional_features=additional_features
                 )
             start_time = time.time()
-            print(f"****SEARCHING {pipe.steps[-1][-1]}")
             search = RandomizedSearchCV(
-                pipe, params, scoring="f1_macro", n_iter=50, cv=4, n_jobs=-2, refit=True
+                pipe,
+                params,
+                scoring="f1_macro",
+                n_iter=100,
+                cv=4,
+                n_jobs=-2,
+                refit=True,
             )
             search.fit(X_train, Y_train)
             models.append(search.best_estimator_)
             training_time = round(time.time() - start_time, 0)
             training_times.append(str(datetime.timedelta(seconds=training_time)))
     return models, training_times
 
@@ -358,28 +502,29 @@
         X_train (pd.DataFrame): DataFrame containing the features to be fed into the estimator
         Y_train (pd.DataFrame): DataFrame containing the targets
 
     Returns:
         (tuple): Tuple containing: a fitted `pipeline` with a MultiOutputClassifier utilising a Support Vector Classifier estimator, and a `str` of the training time taken for the fitting of the pipeline.
     """
     cat_transformer = OneHotEncoder(handle_unknown="ignore")
-    vectorizer = TfidfVectorizer(max_df = 0.9, min_df = 0, ngram_range=(1, 2))
+    vectorizer = TfidfVectorizer(max_df=0.9, min_df=0, ngram_range=(1, 2))
     preproc = make_column_transformer(
-                (cat_transformer, ["FFT_q_standardised"]),
-                (vectorizer, "FFT answer"),
-            )
+        (cat_transformer, ["FFT_q_standardised"]),
+        (vectorizer, "FFT answer"),
+    )
     pipe = make_pipeline(
-                preproc,
-                MultiOutputClassifier(
-                    SVC(C = 15,
-                        probability=True,
-                        class_weight="balanced",
-                        max_iter=1000,
-                        cache_size=1000,
-                    ),
-                ),
-            )
+        preproc,
+        MultiOutputClassifier(
+            SVC(
+                C=15,
+                probability=True,
+                class_weight="balanced",
+                max_iter=1000,
+                cache_size=1000,
+            ),
+        ),
+    )
     start_time = time.time()
     pipe.fit(X_train, Y_train)
     training_time = round(time.time() - start_time, 0)
     training_time = str(datetime.timedelta(seconds=training_time))
     return pipe, training_time
```

### Comparing `pxtextmining-0.5.2/pxtextmining/factories/factory_predict_unlabelled_text.py` & `pxtextmining-0.5.3/pxtextmining/factories/factory_predict_unlabelled_text.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,33 @@
                 prob_of_label = pred_probs[label_index, row, 1]
                 if prob_of_label > 0.5:
                     predictions[row][label_index] = 1
     preds_df = pd.DataFrame(predictions, index=processed_text.index, columns=labels)
     preds_df["labels"] = preds_df.apply(get_labels, args=(labels,), axis=1)
     return preds_df
 
+def predict_multiclass_bert(x, model, additional_features, already_encoded):
+    """Makes multiclass predictions using a transformer-based model. Can encode the data if not already encoded.
+
+    Args:
+        x (pd.DataFrame): DataFrame containing features to be passed through model.
+        model (tf.keras.models.Model): Pretrained transformer based model in tensorflow keras.
+        additional_features (bool, optional): Whether or not additional features (e.g. question type) are included. Defaults to False.
+        already_encoded (bool, optional): Whether or not the input data needs to be encoded. Defaults to False.
+
+    Returns:
+        (np.array): Predicted labels in one-hot encoded format.
+    """
+    y_probs = predict_with_bert(x, model, additional_features = additional_features,
+                           already_encoded = already_encoded)
+    y_binary = turn_probs_into_binary(y_probs)
+    y_binary_fixed = fix_no_labels(y_binary, y_probs, model_type = 'bert')
+    y_preds = np.argmax(y_binary_fixed, axis=1)
+    return y_preds
+
 def predict_with_probs(x, model, labels):
     """Given a trained model and some features, makes predictions based on the model's outputted probabilities using the model.predict_proba function.
     Any label with a predicted probability over 0.5 is taken as the predicted label. If no labels are over 0.5 probability then the
     label with the highest probability is taken.
     Converts into one-hot encoded format (similar to what model.predict would output).
     Currently only works with sklearn models.
```

### Comparing `pxtextmining-0.5.2/pxtextmining/factories/factory_write_results.py` & `pxtextmining-0.5.3/pxtextmining/factories/factory_write_results.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pickle
 import os
 import numpy as np
 import pandas as pd
 
 from pxtextmining.factories.factory_predict_unlabelled_text import get_labels, predict_multilabel_sklearn, predict_with_probs, get_probabilities
 from tensorflow.keras import Model, Sequential
+from pxtextmining.factories.factory_model_performance import parse_metrics_file
 
 
 def write_multilabel_models_and_metrics(models, model_metrics, path):
     """Saves models and their associated performance metrics into a specified folder
 
     Args:
         models (list): List containing the trained tf.keras or sklearn models to be saved.
@@ -61,7 +62,23 @@
     probs_predicted = get_probabilities(predicted_labels, labels, probabilities, model_type = 'sklearn')
     df = df.merge(actual_labels, left_index = True, right_index = True)
     df = df.merge(predicted_labels, left_index = True, right_index = True)
     df = df.merge(probs_actual, left_index = True, right_index = True)
     df = df.merge(probs_predicted, left_index = True, right_index = True)
     df.to_excel(path, index = False)
     print(f'Successfully completed, written to {path}')
+
+def write_model_analysis(model_name, labels, dataset, path):
+    """Writes an Excel file with the performance metrics of each label, as well as the counts of samples for each label.
+
+    Args:
+        model_name (str): Model name used in the performance metrics file
+        labels (list): List of labels for the categories to be predicted.
+        dataset (pd.DataFrame): Original dataset before train test split
+        path (str): Filepath where model and performance metrics file are saved.
+    """
+    metrics_df = parse_metrics_file(f"{path}/{model_name}.txt", labels=labels)
+    label_counts = pd.DataFrame(dataset[labels].sum())
+    label_counts = label_counts.reset_index()
+    label_counts = label_counts.rename(columns={"index": "label", 0: "label_count"})
+    metrics_df = metrics_df.merge(label_counts, on="label")
+    metrics_df.to_excel(f"{path}/{model_name}_perf.xlsx", index=False)
```

### Comparing `pxtextmining-0.5.2/pxtextmining/helpers/text_preprocessor.py` & `pxtextmining-0.5.3/pxtextmining/helpers/text_preprocessor.py`

 * *Files identical despite different names*

### Comparing `pxtextmining-0.5.2/pxtextmining/pipelines/multilabel_pipeline.py` & `pxtextmining-0.5.3/pxtextmining/pipelines/multilabel_pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pandas as pd
 
 from sklearn.model_selection import train_test_split
 
 from pxtextmining.factories.factory_data_load_and_split import (
     bert_data_to_dataset,
     load_multilabel_data,
-    process_and_split_multilabel_data,
+    process_and_split_data,
 )
 from pxtextmining.factories.factory_model_performance import (
     get_multilabel_metrics,
     parse_metrics_file,
 )
 from pxtextmining.factories.factory_pipeline import (
     calculating_class_weights,
@@ -21,24 +21,26 @@
     search_sklearn_pipelines,
     train_bert_model,
     train_tf_model,
 )
 from pxtextmining.factories.factory_write_results import (
     write_multilabel_models_and_metrics,
     write_model_preds,
+    write_model_analysis
 )
 from pxtextmining.helpers.text_preprocessor import tf_preprocessing
 from pxtextmining.params import major_cats, minor_cats, dataset, merged_minor_cats
 
 
 def run_sklearn_pipeline(
     additional_features=False,
     target=major_cats,
     models_to_try=["mnb", "knn", "svm", "rfc"],
     path="test_multilabel",
+    include_analysis = False
 ):
     """Runs all the functions required to load multilabel data, preprocess it, and split it into training and test sets.
     Creates sklearn pipelines and hyperparameters to search, using specified estimators.
     For each estimator type selected, performs a randomized search across the hyperparameters to identify the parameters providing the best
     results on the holdout data within the randomized search.
     Evaluates the performance of the refitted estimator with the best hyperparameters on the test set, and saves the model
     and the performance metrics to a specified folder.
@@ -51,42 +53,50 @@
     """
     random_state = random.randint(1, 999)
     if target == major_cats:
         target_name = "major_categories"
     if target == minor_cats:
         target_name = "minor_categories"
     df = load_multilabel_data(filename=dataset, target=target_name)
-    X_train, X_test, Y_train, Y_test = process_and_split_multilabel_data(
+    X_train, X_test, Y_train, Y_test = process_and_split_data(
         df,
         target=target,
         additional_features=additional_features,
         random_state=random_state,
     )
     models, training_times = search_sklearn_pipelines(
         X_train,
         Y_train,
         models_to_try=models_to_try,
-        additional_features=additional_features,
+        additional_features=additional_features
     )
     model_metrics = []
     for i in range(len(models)):
         m = models[i]
         t = training_times[i]
         model_metrics.append(
             get_multilabel_metrics(
                 X_test,
                 Y_test,
                 random_state=random_state,
                 labels=target,
                 model_type="sklearn",
                 model=m,
                 training_time=t,
+                additional_features=additional_features
             )
         )
     write_multilabel_models_and_metrics(models, model_metrics, path=path)
+    if include_analysis == True:
+        for i in range(len(models)):
+            model_name = f'model_{i}'
+            write_model_preds(X_test, Y_test, models[i], labels=target,
+                              additional_features=additional_features, path=f"{path}/{model_name}_labels.xlsx")
+            write_model_analysis(model_name, labels=target, dataset=df, path=path)
+    print("Pipeline complete")
 
 
 def run_svc_pipeline(
     additional_features=False,
     target=major_cats,
     path="test_multilabel",
     include_analysis=False,
@@ -107,15 +117,15 @@
     if target == major_cats:
         target_name = "major_categories"
     if target == minor_cats:
         target_name = "minor_categories"
     if target == merged_minor_cats:
         target_name = "test"
     df = load_multilabel_data(filename=dataset, target=target_name)
-    X_train, X_test, Y_train, Y_test = process_and_split_multilabel_data(
+    X_train, X_test, Y_train, Y_test = process_and_split_data(
         df,
         target=target,
         additional_features=additional_features,
         random_state=random_state,
     )
     model, training_time = create_and_train_svc_model(X_train, Y_train)
     model_metrics = get_multilabel_metrics(
@@ -134,21 +144,16 @@
             X_test,
             Y_test,
             model,
             labels=target,
             additional_features=additional_features,
             path=f"{path}/labels.xlsx"
         )
-        metrics_df = parse_metrics_file(f"{path}/model_0.txt", labels=target)
-        label_counts = pd.DataFrame(df[target].sum())
-        label_counts = label_counts.reset_index()
-        label_counts = label_counts.rename(columns={"index": "label", 0: "label_count"})
-        metrics_df = metrics_df.merge(label_counts, on="label")
-        metrics_df.to_excel(f"{path}/perf.xlsx", index=False)
-
+        write_model_analysis(model_name='model_0', labels=target, dataset = df, path = path)
+    print("Pipeline complete!")
 
 def run_tf_pipeline(target=major_cats, path="test_multilabel/tf"):
     """Runs all the functions required to load multilabel data, preprocess it, and split it into training and test sets.
     Creates tf.keras LSTM model and trains it on the train set.
     Evaluates the performance of trained model with the best hyperparameters on the test set, and saves the model
     and the performance metrics to a specified folder.
     Cannot currently take additional features, is only designed for text data alone.
@@ -158,15 +163,15 @@
         target (list, optional): The target labels, which should be columns in the dataset DataFrame. Defaults to major_cats.
         path (str, optional): Path where the models are to be saved. If path does not exist, it will be created. Defaults to 'test_multilabel'.
     """
     random_state = random.randint(1, 999)
     df = load_multilabel_data(
         filename="datasets/multilabeldata_2.csv", target="major_categories"
     )
-    X_train, X_test, Y_train, Y_test = process_and_split_multilabel_data(
+    X_train, X_test, Y_train, Y_test = process_and_split_data(
         df, target=target, random_state=random_state
     )
     X_train_pad, vocab_size = tf_preprocessing(X_train)
     X_test_pad, _ = tf_preprocessing(X_test)
     class_weights_dict = calculating_class_weights(Y_train)
     model = create_tf_model(vocab_size)
     model_trained, training_time = train_tf_model(
@@ -199,15 +204,15 @@
     random_state = random.randint(1, 999)
     print(f"random_state is: {random_state}")
     if target == major_cats:
         target_name = "major_categories"
     if target == minor_cats:
         target_name = "minor_categories"
     df = load_multilabel_data(filename=dataset, target=target_name)
-    X_train_val, X_test, Y_train_val, Y_test = process_and_split_multilabel_data(
+    X_train_val, X_test, Y_train_val, Y_test = process_and_split_data(
         df,
         target=target,
         preprocess_text=False,
         additional_features=additional_features,
         random_state=random_state,
     )
     X_train, X_val, Y_train, Y_val = train_test_split(
@@ -246,14 +251,14 @@
         already_encoded=True,
     )
     write_multilabel_models_and_metrics([model_trained], [model_metrics], path=path)
 
 
 if __name__ == "__main__":
     # run_bert_pipeline(additional_features = True, path = 'test_multilabel/bert_minorcats', target = minor_cats)
-    # run_sklearn_pipeline(additional_features = True, target= minor_cats, models_to_try = ["knn", "svm", "rfc"], path = 'test_multilabel/minorcats_sklearn')
+    # run_sklearn_pipeline(additional_features = True, target= minor_cats, models_to_try = ["svm"], path = 'test_multilabel/230522-b')
     run_svc_pipeline(
         additional_features=True,
-        target=merged_minor_cats,
-        path="test_multilabel/minorcats_merged_230420",
+        target=minor_cats,
+        path="test_multilabel/230522",
         include_analysis=True
     )
```

### Comparing `pxtextmining-0.5.2/pyproject.toml` & `pxtextmining-0.5.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pxtextmining"
-version = "0.5.2"
+version = "0.5.3"
 description = "Multilabel text classification of patient experience feedback."
 authors = ['CDU Data Science <cdudatascience@nottshc.nhs.uk>',
 'YiWen Hon <yiwen.hon@nottshc.nhs.uk>']
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/CDU-data-science-team/pxtextmining"
 documentation = "https://cdu-data-science-team.github.io/pxtextmining"
@@ -16,25 +16,29 @@
 matplotlib = "^3.3.2"
 numpy = ">=1.22"
 pandas = "^1.4.0"
 scikit-learn = "1.0.2"
 tensorflow = "^2.11.0"
 transformers = "^4.26.1"
 scipy = "^1.10.1"
+xgboost = "^1.7.5"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 uvicorn = "^0.20.0"
-requests = "2.25.1"
 pydantic = "^1.10.4"
 pytest = "^7.2.2"
 fastapi = "^0.94.1"
 httpx = "^0.23.3"
+pytest-cov = "^4.0.0"
+pytest-mock = "^3.10.0"
+requests = "^2.31.0"
+jupyter = "^1.0.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
 mkdocstrings-python = "^0.8.2"
```

### Comparing `pxtextmining-0.5.2/setup.py` & `pxtextmining-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,20 @@
  'matplotlib>=3.3.2,<4.0.0',
  'numpy>=1.22',
  'pandas>=1.4.0,<2.0.0',
  'scikit-learn==1.0.2',
  'scipy>=1.10.1,<2.0.0',
  'spacy>=3.4.4,<4.0.0',
  'tensorflow>=2.11.0,<3.0.0',
- 'transformers>=4.26.1,<5.0.0']
+ 'transformers>=4.26.1,<5.0.0',
+ 'xgboost>=1.7.5,<2.0.0']
 
 setup_kwargs = {
     'name': 'pxtextmining',
-    'version': '0.5.2',
+    'version': '0.5.3',
     'description': 'Multilabel text classification of patient experience feedback.',
     'long_description': '# pxtextmining: Text Classification of Patient Experience feedback\n\n## Project description\n**pxtextmining** is a Python package for classifying patient feedback comments collected via the [NHS England Friends and Family Test](https://www.england.nhs.uk/fft/) (FFT). It is part of the [Patient Experience Qualitative Data Categorisation project](https://cdu-data-science-team.github.io/PatientExperience-QDC/), funded by NHS England and hosted by Nottinghamshire Healthcare NHS Foundation Trust.\n\n__We are working openly by [open-sourcing](https://github.com/CDU-data-science-team/pxtextmining/blob/main/LICENSE) the analysis code and data where possible to promote replication, reproducibility and further developments. Pull requests are more than welcome.__\n\n## Documentation and installation\n\nFull documentation, including installation instructions, is available on our [documentation page](https://cdu-data-science-team.github.io/pxtextmining/).\n',
     'author': 'CDU Data Science',
     'author_email': 'cdudatascience@nottshc.nhs.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/CDU-data-science-team/pxtextmining',
```

### Comparing `pxtextmining-0.5.2/PKG-INFO` & `pxtextmining-0.5.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pxtextmining
-Version: 0.5.2
+Version: 0.5.3
 Summary: Multilabel text classification of patient experience feedback.
 Home-page: https://github.com/CDU-data-science-team/pxtextmining
 License: MIT
 Author: CDU Data Science
 Author-email: cdudatascience@nottshc.nhs.uk
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,15 @@
 Requires-Dist: numpy (>=1.22)
 Requires-Dist: pandas (>=1.4.0,<2.0.0)
 Requires-Dist: scikit-learn (==1.0.2)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: spacy (>=3.4.4,<4.0.0)
 Requires-Dist: tensorflow (>=2.11.0,<3.0.0)
 Requires-Dist: transformers (>=4.26.1,<5.0.0)
+Requires-Dist: xgboost (>=1.7.5,<2.0.0)
 Project-URL: Documentation, https://cdu-data-science-team.github.io/pxtextmining
 Project-URL: Repository, https://github.com/CDU-data-science-team/pxtextmining
 Description-Content-Type: text/markdown
 
 # pxtextmining: Text Classification of Patient Experience feedback
 
 ## Project description
```

