# Comparing `tmp/protloc_mex_x-0.0.1.tar.gz` & `tmp/protloc_mex_x-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protloc_mex_x-0.0.1.tar", max compression
+gzip compressed data, was "protloc_mex_x-0.0.2.tar", max compression
```

## Comparing `protloc_mex_x-0.0.1.tar` & `protloc_mex_x-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1091 2023-04-25 08:38:35.586641 protloc_mex_x-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0        2 2023-05-09 03:41:02.000000 protloc_mex_x-0.0.1/protloc_mex_X/__init__.py
--rw-r--r--   0        0        0    25940 2023-05-24 13:35:46.000000 protloc_mex_x-0.0.1/protloc_mex_X/ESM2_fr.py
--rw-r--r--   0        0        0     2999 2023-05-08 12:33:04.000000 protloc_mex_x-0.0.1/protloc_mex_X/examples/test1.txt
--rw-r--r--   0        0        0     2749 2023-05-09 03:13:02.000000 protloc_mex_x-0.0.1/protloc_mex_X/feature_corrlation.py
--rw-r--r--   0        0        0      863 2023-05-29 13:07:37.706083 protloc_mex_x-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       35 2023-05-10 08:06:08.458858 protloc_mex_x-0.0.1/README.md
--rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 protloc_mex_x-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-04-25 08:38:35.586641 protloc_mex_x-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0        2 2023-05-09 03:41:02.000000 protloc_mex_x-0.0.2/protloc_mex_X/__init__.py
+-rw-r--r--   0        0        0    36871 2023-05-31 08:20:32.000000 protloc_mex_x-0.0.2/protloc_mex_X/ESM2_fr.py
+-rw-r--r--   0        0        0     2999 2023-05-08 12:33:04.000000 protloc_mex_x-0.0.2/protloc_mex_X/examples/test1.txt
+-rw-r--r--   0        0        0     2749 2023-05-09 03:13:02.000000 protloc_mex_x-0.0.2/protloc_mex_X/feature_corrlation.py
+-rw-r--r--   0        0        0      863 2023-05-31 08:35:47.770448 protloc_mex_x-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-05-10 08:06:08.458858 protloc_mex_x-0.0.2/README.md
+-rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 protloc_mex_x-0.0.2/PKG-INFO
```

### Comparing `protloc_mex_x-0.0.1/LICENSE.txt` & `protloc_mex_x-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `protloc_mex_x-0.0.1/protloc_mex_X/ESM2_fr.py` & `protloc_mex_x-0.0.2/protloc_mex_X/ESM2_fr.py`

 * *Files 12% similar despite different names*

```diff
@@ -82,14 +82,20 @@
             
             del inputs, outputs
             torch.cuda.empty_cache()
             torch.cuda.synchronize()
      
     return X_outcome
 
+
+
+
+
+
+   
 class Esm2LastHiddenFeatureExtractor:
     def __init__(self, tokenizer, model, compute_cls=True, compute_eos=True, compute_mean=True, compute_segments=False):
         self.tokenizer = tokenizer
         self.model = model
         self.compute_cls = compute_cls
         self.compute_eos = compute_eos
         self.compute_mean = compute_mean
@@ -123,14 +129,353 @@
                 segment_mean = torch.zeros(last_hidden_state[:, start:start+1, :].shape, device=last_hidden_state.device)
             
             segment_means.append(segment_mean.squeeze().tolist())
             start = end
 
         return segment_means
     
+    
+    ##计算cls, eos, 氨基酸平均表征, 每1/10段氨基酸平均表征
+    def get_last_hidden_features_combine(self, X_input, sequence_name='sequence', batch_size=32):
+        X_input = X_input.reset_index(drop=True)
+        device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+        self.model.to(device)
+        sequence = X_input[sequence_name].tolist()
+
+        features_length = {}  # save the length of different features
+        columns = None  # initialize the column names
+        all_results = []  # Store all batch results
+        with torch.no_grad():
+            for i in tqdm(range(0, len(sequence), batch_size), desc='batches for inference'):
+                batch_sequences = sequence[i:i+batch_size]
+                inputs = self.tokenizer(batch_sequences, return_tensors="pt", padding=True).to(device)
+                outputs = self.model(**inputs)
+
+                for j in range(len(batch_sequences)):
+                    idx = i + j
+                    tokens = self.tokenizer.convert_ids_to_tokens(inputs['input_ids'][j])
+                    eos_position = tokens.index(self.tokenizer.eos_token) if self.tokenizer.eos_token in tokens else len(tokens) - 1
+                    last_hidden_state = self.get_last_hidden_states(outputs)
+                    last_cls_token = self.get_last_cls_token(last_hidden_state[j:j+1]) if self.compute_cls else None
+                    last_eos_token = self.get_last_eos_token(last_hidden_state[j:j+1], eos_position) if self.compute_eos else None
+                    last_mean_token = self.get_last_mean_token(last_hidden_state[j:j+1], eos_position) if self.compute_mean else None
+                    segment_means = self.get_segment_mean_tokens(last_hidden_state[j:j+1], eos_position) if self.compute_segments else None
+
+                    # extract features and add them to DataFrame directly
+                    features = []
+                    if last_cls_token is not None:
+                        cls_features = last_cls_token.squeeze().tolist()
+                        if 'cls' not in features_length:
+                            features_length['cls'] = len(cls_features)
+                        features.extend(cls_features)
+
+                    if last_eos_token is not None:
+                        eos_features = last_eos_token.squeeze().tolist()
+                        if 'eos' not in features_length:
+                            features_length['eos'] = len(eos_features)
+                        features.extend(eos_features)
+
+                    if last_mean_token is not None:
+                        mean_features = last_mean_token.squeeze().tolist()
+                        if 'mean' not in features_length:
+                            features_length['mean'] = len(mean_features)
+                        features.extend(mean_features)
+
+                    if segment_means is not None:
+                        # In the new version, we keep each segment mean as a separate list
+                        for seg, segment_mean in enumerate(segment_means):
+                            features.extend(segment_mean)
+                            if f'ESM2_segment{seg}_mean' not in features_length:
+                                features_length[f'ESM2_segment{seg}_mean'] = len(segment_mean)
+
+                    # create the column names only for the first item
+                    if columns is None:
+                        columns = []
+                        for feature_type, length in features_length.items():
+                            for k in range(length):
+                                columns.append(f"ESM2_{feature_type}{k}")
+
+                    # Create DataFrame for this batch
+                    result = pd.DataFrame([features], columns=columns, index=[idx])
+                    all_results.append(result)
+
+                del inputs, outputs
+                torch.cuda.empty_cache()
+                torch.cuda.synchronize()
+
+        # Combine all batch results outside the loop
+        X_outcome = pd.concat(all_results, axis=0)
+
+        print(f'Features dimensions: {features_length}')
+
+        # Combine X_input and X_outcome along axis 1
+        combined_result = pd.concat([X_input, X_outcome], axis=1)
+        return combined_result
+    
+
+
+    
+    ##计算磷酸化表征
+    def get_last_hidden_phosphorylation_position_feature(self, X_input, sequence_name='sequence', phosphorylation_positions='phosphorylation_positions', batch_size=32):
+        X_input = X_input.reset_index(drop=True)
+        device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+        self.model.to(device)
+
+        # Group X_input by sequence
+        grouped_X_input = X_input.groupby(sequence_name)
+        sequence_to_indices = grouped_X_input.groups
+
+        # Pre-compute the number of features
+        num_features = self.model.config.hidden_size
+        columns = [f"ESM2_phospho_pos{k}" for k in range(num_features)]
+
+        # Create an empty DataFrame with the column names
+        X_outcome = pd.DataFrame(columns=columns)
+
+        with torch.no_grad():
+            for i in tqdm(range(0, len(grouped_X_input), batch_size), desc='batches for inference'):
+                batch_sequences = list(islice(sequence_to_indices.keys(), i, i + batch_size))
+                batch_grouped_sequences = {seq: X_input.loc[sequence_to_indices[seq]] for seq in batch_sequences}
+
+                # Get the unique sequences in the batch
+                inputs = self.tokenizer(batch_sequences, return_tensors="pt", padding=True).to(device)
+                outputs = self.model(**inputs)
+
+                for j, sequence in enumerate(batch_sequences):
+                    sequence_indices = batch_grouped_sequences[sequence].index
+                    sequence_positions = batch_grouped_sequences[sequence][phosphorylation_positions].tolist()
+                    last_hidden_state = self.get_last_hidden_states(outputs)[j:j+1]
+
+                    for idx, position in zip(sequence_indices, sequence_positions):
+                        position = int(position)  # Make sure position is an integer
+                        position_feature = last_hidden_state[:, position, :]  # Removed +1 since the sequence starts from 1, and consider removing the cls token
+                        features = position_feature.squeeze().tolist()
+
+                        # Add the new row to the DataFrame
+                        X_outcome.loc[idx] = features
+
+                del inputs, outputs
+                torch.cuda.empty_cache()
+                torch.cuda.synchronize()
+
+
+        # Print the dimension of the final phosphorylation features
+        print(f"The dimension of the final phosphorylation features is: {X_outcome.shape[1]}")
+
+        # Combine X_input and X_outcome along axis 1
+        combined_result = pd.concat([X_input, X_outcome], axis=1)
+        return combined_result
+    
+ 
+    def get_amino_acid_representation(self, sequence, amino_acid, position):
+        device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+        self.model.to(device)
+        
+        # Check if the amino acid at the given position matches the input
+        if sequence[position - 1] != amino_acid:
+            raise ValueError(f"The amino acid at position {position} is not {amino_acid}.")
+
+        # Convert the sequence to input tensors
+        inputs = self.tokenizer([sequence], return_tensors="pt", padding=True).to(device)
+        
+        # Get the model outputs
+        with torch.no_grad():
+            outputs = self.model(**inputs)
+        
+        # Get the last hidden state
+        last_hidden_state = self.get_last_hidden_states(outputs)
+        
+        # Get the tokens from the input ids
+        tokens = self.tokenizer.convert_ids_to_tokens(inputs['input_ids'][0])
+        
+        
+        # Get the position of the amino acid token in the tokens list
+        # We add 1 to the position to account for the CLS token at the start
+        token_position =  position if amino_acid == tokens[position] else -1
+        
+        if token_position == -1:
+            raise ValueError(f"The token for amino acid {amino_acid} could not be found in the tokenized sequence.")
+        
+        # Get the feature vector for the amino acid
+        amino_acid_features = last_hidden_state[:, token_position, :].squeeze().tolist()
+        
+        
+        # Get the feature vector for the amino acid
+        amino_acid_features = last_hidden_state[:, token_position, :].squeeze().tolist()
+        
+        # Prepare the DataFrame
+        feature_names = [f"ESM2_{k}" for k in range(len(amino_acid_features))]
+        amino_acid_features_df = pd.DataFrame(amino_acid_features, index=feature_names, columns=[amino_acid]).T
+
+        return amino_acid_features_df
+ 
+    
+ 
+    
+ 
+    
+ 
+def NetPhos_classic_txt_DataFrame(pattern, data):
+    '''
+    This function takes a pattern and data as input and returns a DataFrame containing
+    the parsed information.
+
+    Parameters
+    ----------
+    pattern : str
+        A regular expression pattern used to match lines in the input data.
+    data : str
+        The input data containing the information to be parsed.
+
+    Returns
+    -------
+    df : pandas.DataFrame
+        A DataFrame containing the parsed information.
+
+    Example
+    -------
+    To use this function with the example file provided in the package:
+
+    >>> import os
+    >>> import protloc_mex_X
+    >>> from protloc_mex_X.ESM2_fr import NetPhos_classic_txt_DataFrame
+    ...
+    >>> example_data = os.path.join(protloc_mex_X.__path__[0], "examples", "test1.txt")
+    ...
+    >>> with open(example_data, "r") as f:
+    ...     data = f.read()
+    ... print(data)
+    >>> pattern = r".*YES"
+    >>> result_df = NetPhos_classic_txt_DataFrame(pattern, data)
+
+    '''
+
+    # Extract lines that match the pattern
+    seq_lines = re.findall(pattern, data)
+
+    # Split the extracted lines into lists
+    split_lines = [line.split() for line in seq_lines]
+
+    # Remove '#' character
+    split_lines = [line[1:] for line in split_lines]
+
+    # Check if each list element has a length of 7, if not, skip that line
+    filtered_split_lines = [line for line in split_lines if len(line) == 7]
+
+    # Convert the filtered list to a DataFrame and set column names
+    column_names = ['Sequence', 'position', 'x', 'Context', 'Score', 'Kinase', 'Answer']
+    df = pd.DataFrame(filtered_split_lines, columns=column_names)
+
+    # Convert the 'Score' column to float type
+    df['Score'] = df['Score'].astype(float)
+
+    return df
+
+
+
+def phospho_feature_sim_cosine_weighted_average(dim, df_cls, df_phospho):
+    # Check if all protein_id in df_phospho are in df_cls
+    if not df_phospho.index.isin(df_cls.index).all():
+        raise ValueError("Protein_id in df_phospho is not matched with df_cls.")
+
+    # Merge df_cls and df_phospho on index (protein_id)
+    df = pd.merge(df_cls, df_phospho, how='inner', left_index=True, right_index=True)
+
+    # Calculate cosine similarity for each row in the merged dataframe
+    # 前dim列
+    array_cls = df.iloc[:, :dim].values
+
+    # 接下来的dim列
+    array_phospho = df.iloc[:, dim:2*dim].values
+
+    # 对于全为0的行，添加一个小的正数以避免除零错误
+    epsilon = 1e-10
+    array_cls[np.where(~array_cls.any(axis=1))[0]] += epsilon
+    array_phospho[np.where(~array_phospho.any(axis=1))[0]] += epsilon
+
+    # 计算余弦相似度
+    similarity = np.sum(array_cls * array_phospho, axis=1) / (np.linalg.norm(array_cls, axis=1) * np.linalg.norm(array_phospho, axis=1))
+
+    # 添加到DataFrame
+    df['similarity'] = similarity
+    #Multiply similarity with phospho_feature for each row
+    
+    # 使用NumPy进行运算
+    array_weighted_features= df['similarity'].values[:, None] * array_phospho
+
+    # 将结果转换为 DataFrame 并合并
+    weighted_features_df = pd.DataFrame(array_weighted_features, columns=[f'weighted{i}' for i in range(dim)], index=df.index)
+    df = pd.concat([df, weighted_features_df], axis=1)
+
+    # Calculate total weights (sum of abs similarities) for each protein
+    total_weights = df['similarity'].abs().groupby(df.index).sum()
+    # Calculate sum of weighted features for each protein
+    grouped = df.groupby(df.index).agg({**{f'weighted{i}': 'sum' for i in range(dim)}})
+
+    # Calculate weighted average by dividing sum of weighted features by total weights
+    # for i in range(dim):
+    #     grouped[f'average{i}'] = grouped[f'weighted{i}'] / total_weights
+    average_features = {f'pho_average{i}': grouped[f'weighted{i}'] / total_weights for i in range(dim)}
+    average_df = pd.DataFrame(average_features)
+    grouped = pd.concat([grouped, average_df], axis=1)
+
+    # Merge df_cls and grouped dataframe by protein_id (index)
+    df_cls = pd.merge(df_cls, grouped[[f'pho_average{i}' for i in range(dim)]], how='left', left_index=True, right_index=True)
+
+    # For proteins that do not have phospho_feature, set average_feature to zero
+    # for i in range(dim):
+    #     df_cls[f'average{i}'] = df_cls[f'average{i}'].fillna(0)
+    if df_cls.isnull().any().any():
+        df_cls = df_cls.fillna(0)
+        
+    return df_cls
+
+###后面都是legacy，可用于检验模型是否正确或无用的代码即不在完整工作流中运行，但不允许删除。
+
+class Esm2LastHiddenFeatureExtractor_legacy:
+    def __init__(self, tokenizer, model, compute_cls=True, compute_eos=True, compute_mean=True, compute_segments=False):
+        self.tokenizer = tokenizer
+        self.model = model
+        self.compute_cls = compute_cls
+        self.compute_eos = compute_eos
+        self.compute_mean = compute_mean
+        self.compute_segments = compute_segments
+
+    def get_last_hidden_states(self, outputs):
+        last_hidden_state = outputs.hidden_states[-1]
+        return last_hidden_state
+
+    def get_last_cls_token(self, last_hidden_state):
+        return last_hidden_state[:, 0, :]
+
+    def get_last_eos_token(self, last_hidden_state, eos_position):
+        return last_hidden_state[:, eos_position, :]
+
+    def get_last_mean_token(self, last_hidden_state, eos_position):
+        return last_hidden_state[:, 1:eos_position, :].mean(dim=1)
+
+    def get_segment_mean_tokens(self, last_hidden_state, eos_position, num_segments=10):
+        seq_len = eos_position - 1
+        segment_size, remainder = divmod(seq_len, num_segments)
+        segment_means = []
+
+        start = 1
+        for i in range(num_segments):
+            end = start + segment_size + (1 if i < remainder else 0)
+            
+            if end > start:  # Check if the segment has amino acids
+                segment_mean = last_hidden_state[:, start:end, :].mean(dim=1)
+            else:  # If the segment is empty, create a zero tensor with the same dimensions as the hidden state
+                segment_mean = torch.zeros(last_hidden_state[:, start:start+1, :].shape, device=last_hidden_state.device)
+            
+            segment_means.append(segment_mean.squeeze().tolist())
+            start = end
+
+        return segment_means
+    
     def extract_features(self, cls_token=None, eos_token=None, mean_token=None, segment_means=None):
         features = {}
 
         if cls_token is not None:
             cls_features = cls_token.squeeze().tolist()
             features.update({f"ESM2_cls{k}": feature for k, feature in enumerate(cls_features)})
 
@@ -221,15 +566,15 @@
                 torch.cuda.empty_cache()
                 torch.cuda.synchronize()
 
         # Combine X_input and X_outcome along axis 1
         combined_result = pd.concat([X_input, X_outcome], axis=1)
         return combined_result
 
-    from itertools import islice
+    #from itertools import islice
     
        
     def get_last_hidden_phosphorylation_position_feature(self, X_input, sequence_name='sequence', phosphorylation_positions='phosphorylation_positions', batch_size=32):
         X_input = X_input.reset_index(drop=True)
         X_outcome = pd.DataFrame()
         device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         self.model.to(device)
@@ -357,74 +702,14 @@
         amino_acid_features = last_hidden_state[:, token_position, :].squeeze().tolist()
         
         # Prepare the DataFrame
         feature_names = [f"ESM2_{k}" for k in range(len(amino_acid_features))]
         amino_acid_features_df = pd.DataFrame(amino_acid_features, index=feature_names, columns=[amino_acid]).T
 
         return amino_acid_features_df
-   
-
-  
-def NetPhos_classic_txt_DataFrame(pattern, data):
-    '''
-    This function takes a pattern and data as input and returns a DataFrame containing
-    the parsed information.
-
-    Parameters
-    ----------
-    pattern : str
-        A regular expression pattern used to match lines in the input data.
-    data : str
-        The input data containing the information to be parsed.
-
-    Returns
-    -------
-    df : pandas.DataFrame
-        A DataFrame containing the parsed information.
-
-    Example
-    -------
-    To use this function with the example file provided in the package:
-
-    >>> import os
-    >>> import protloc_mex_X
-    >>> from protloc_mex_X.ESM2_fr import NetPhos_classic_txt_DataFrame
-    ...
-    >>> example_data = os.path.join(protloc_mex_X.__path__[0], "examples", "test1.txt")
-    ...
-    >>> with open(example_data, "r") as f:
-    ...     data = f.read()
-    ... print(data)
-    >>> pattern = r".*YES"
-    >>> result_df = NetPhos_classic_txt_DataFrame(pattern, data)
-
-    '''
-
-    # Extract lines that match the pattern
-    seq_lines = re.findall(pattern, data)
-
-    # Split the extracted lines into lists
-    split_lines = [line.split() for line in seq_lines]
-
-    # Remove '#' character
-    split_lines = [line[1:] for line in split_lines]
-
-    # Check if each list element has a length of 7, if not, skip that line
-    filtered_split_lines = [line for line in split_lines if len(line) == 7]
-
-    # Convert the filtered list to a DataFrame and set column names
-    column_names = ['Sequence', 'position', 'x', 'Context', 'Score', 'Kinase', 'Answer']
-    df = pd.DataFrame(filtered_split_lines, columns=column_names)
-
-    # Convert the 'Score' column to float type
-    df['Score'] = df['Score'].astype(float)
-
-    return df
-
-
 
 def phospho_feature_sim_cosine_mean_legacy(dim, df_cls, df_phospho):
     # Check if all protein_id in df_phospho are in df_cls
     if not df_phospho.index.isin(df_cls.index).all():
         raise ValueError("Protein_id in df_phospho is not matched with df_cls.")
 
     # Merge df_cls and df_phospho on index (protein_id)
@@ -497,63 +782,7 @@
     if df_cls.isnull().any().any():
         df_cls = df_cls.fillna(0)
         
     return df_cls
 
 
 
-def phospho_feature_sim_cosine_weighted_average(dim, df_cls, df_phospho):
-    # Check if all protein_id in df_phospho are in df_cls
-    if not df_phospho.index.isin(df_cls.index).all():
-        raise ValueError("Protein_id in df_phospho is not matched with df_cls.")
-
-    # Merge df_cls and df_phospho on index (protein_id)
-    df = pd.merge(df_cls, df_phospho, how='inner', left_index=True, right_index=True)
-
-    # Calculate cosine similarity for each row in the merged dataframe
-    # 前dim列
-    array_cls = df.iloc[:, :dim].values
-
-    # 接下来的dim列
-    array_phospho = df.iloc[:, dim:2*dim].values
-
-    # 对于全为0的行，添加一个小的正数以避免除零错误
-    epsilon = 1e-10
-    array_cls[np.where(~array_cls.any(axis=1))[0]] += epsilon
-    array_phospho[np.where(~array_phospho.any(axis=1))[0]] += epsilon
-
-    # 计算余弦相似度
-    similarity = np.sum(array_cls * array_phospho, axis=1) / (np.linalg.norm(array_cls, axis=1) * np.linalg.norm(array_phospho, axis=1))
-
-    # 添加到DataFrame
-    df['similarity'] = similarity
-    #Multiply similarity with phospho_feature for each row
-    
-    # 使用NumPy进行运算
-    array_weighted_features= df['similarity'].values[:, None] * array_phospho
-
-    # 将结果转换为 DataFrame 并合并
-    weighted_features_df = pd.DataFrame(array_weighted_features, columns=[f'weighted{i}' for i in range(dim)], index=df.index)
-    df = pd.concat([df, weighted_features_df], axis=1)
-
-    # Calculate total weights (sum of abs similarities) for each protein
-    total_weights = df['similarity'].abs().groupby(df.index).sum()
-    # Calculate sum of weighted features for each protein
-    grouped = df.groupby(df.index).agg({**{f'weighted{i}': 'sum' for i in range(dim)}})
-
-    # Calculate weighted average by dividing sum of weighted features by total weights
-    # for i in range(dim):
-    #     grouped[f'average{i}'] = grouped[f'weighted{i}'] / total_weights
-    average_features = {f'pho_average{i}': grouped[f'weighted{i}'] / total_weights for i in range(dim)}
-    average_df = pd.DataFrame(average_features)
-    grouped = pd.concat([grouped, average_df], axis=1)
-
-    # Merge df_cls and grouped dataframe by protein_id (index)
-    df_cls = pd.merge(df_cls, grouped[[f'pho_average{i}' for i in range(dim)]], how='left', left_index=True, right_index=True)
-
-    # For proteins that do not have phospho_feature, set average_feature to zero
-    # for i in range(dim):
-    #     df_cls[f'average{i}'] = df_cls[f'average{i}'].fillna(0)
-    if df_cls.isnull().any().any():
-        df_cls = df_cls.fillna(0)
-        
-    return df_cls
```

### Comparing `protloc_mex_x-0.0.1/protloc_mex_X/examples/test1.txt` & `protloc_mex_x-0.0.2/protloc_mex_X/examples/test1.txt`

 * *Files identical despite different names*

### Comparing `protloc_mex_x-0.0.1/protloc_mex_X/feature_corrlation.py` & `protloc_mex_x-0.0.2/protloc_mex_X/feature_corrlation.py`

 * *Files identical despite different names*

### Comparing `protloc_mex_x-0.0.1/pyproject.toml` & `protloc_mex_x-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "protloc_mex_X"
-version = "0.0.1"
+version = "0.0.2"
 description = "Internal use kit"
 authors = ["Ze Yu Luo <1024226968@qq.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/yujuan-zhang/ProtLoc-mexl"
 repository = "https://github.com/yujuan-zhang/ProtLoc-mexl"
 documentation = "https://github.com/yujuan-zhang/ProtLoc-mexl/issues"
```

### Comparing `protloc_mex_x-0.0.1/PKG-INFO` & `protloc_mex_x-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protloc-mex-x
-Version: 0.0.1
+Version: 0.0.2
 Summary: Internal use kit
 Home-page: https://github.com/yujuan-zhang/ProtLoc-mexl
 License: MIT
 Author: Ze Yu Luo
 Author-email: 1024226968@qq.com
 Requires-Python: >=3.9
 Classifier: Development Status :: 3 - Alpha
```

