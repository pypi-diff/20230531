# Comparing `tmp/ms1searchpy-2.3.6-py3-none-any.whl.zip` & `tmp/ms1searchpy-2.3.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 33769 bytes, number of entries: 14
+Zip file size: 34930 bytes, number of entries: 14
 -rw-r--r--  2.0 unx        0 b- defN 21-Dec-13 13:18 ms1searchpy/__init__.py
--rw-r--r--  2.0 unx     2692 b- defN 21-Dec-13 13:18 ms1searchpy/combine.py
--rw-r--r--  2.0 unx    15709 b- defN 22-Feb-01 14:05 ms1searchpy/directms1quant.py
--rw-r--r--  2.0 unx    72094 b- defN 22-Jan-28 15:04 ms1searchpy/main.py
--rw-r--r--  2.0 unx     7197 b- defN 22-Feb-01 14:06 ms1searchpy/ms1todiffacto.py
--rw-r--r--  2.0 unx     2983 b- defN 22-Jan-28 11:00 ms1searchpy/search.py
--rw-r--r--  2.0 unx    13930 b- defN 22-Jan-28 14:26 ms1searchpy/utils.py
+-rw-r--r--  2.0 unx     2885 b- defN 22-Apr-06 14:56 ms1searchpy/combine.py
+-rw-r--r--  2.0 unx    15507 b- defN 22-Apr-06 14:56 ms1searchpy/directms1quant.py
+-rw-r--r--  2.0 unx    73591 b- defN 22-Apr-07 14:24 ms1searchpy/main.py
+-rw-r--r--  2.0 unx     7413 b- defN 22-Apr-06 14:56 ms1searchpy/ms1todiffacto.py
+-rw-r--r--  2.0 unx     3616 b- defN 22-Apr-06 15:26 ms1searchpy/search.py
+-rw-r--r--  2.0 unx    14223 b- defN 22-Apr-06 14:56 ms1searchpy/utils.py
 -rw-r--r--  2.0 unx    12868 b- defN 22-Jan-28 11:00 ms1searchpy/utils_figures.py
--rwxr-xr-x  2.0 unx      551 b- defN 22-Feb-01 14:12 ms1searchpy-2.3.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     7671 b- defN 22-Feb-01 14:12 ms1searchpy-2.3.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Feb-01 14:12 ms1searchpy-2.3.6.dist-info/WHEEL
--rw-r--r--  2.0 unx      225 b- defN 22-Feb-01 14:12 ms1searchpy-2.3.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 22-Feb-01 14:12 ms1searchpy-2.3.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1152 b- defN 22-Feb-01 14:12 ms1searchpy-2.3.6.dist-info/RECORD
-14 files, 137176 bytes uncompressed, 31857 bytes compressed:  76.8%
+-rwxr-xr-x  2.0 unx      551 b- defN 22-Apr-08 10:53 ms1searchpy-2.3.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6263 b- defN 22-Apr-08 10:53 ms1searchpy-2.3.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Apr-08 10:53 ms1searchpy-2.3.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx      229 b- defN 22-Apr-08 10:53 ms1searchpy-2.3.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 22-Apr-08 10:53 ms1searchpy-2.3.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1152 b- defN 22-Apr-08 10:53 ms1searchpy-2.3.7.dist-info/RECORD
+14 files, 138402 bytes uncompressed, 33018 bytes compressed:  76.1%
```

## zipnote {}

```diff
@@ -18,26 +18,26 @@
 
 Filename: ms1searchpy/utils.py
 Comment: 
 
 Filename: ms1searchpy/utils_figures.py
 Comment: 
 
-Filename: ms1searchpy-2.3.6.dist-info/LICENSE
+Filename: ms1searchpy-2.3.7.dist-info/LICENSE
 Comment: 
 
-Filename: ms1searchpy-2.3.6.dist-info/METADATA
+Filename: ms1searchpy-2.3.7.dist-info/METADATA
 Comment: 
 
-Filename: ms1searchpy-2.3.6.dist-info/WHEEL
+Filename: ms1searchpy-2.3.7.dist-info/WHEEL
 Comment: 
 
-Filename: ms1searchpy-2.3.6.dist-info/entry_points.txt
+Filename: ms1searchpy-2.3.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: ms1searchpy-2.3.6.dist-info/top_level.txt
+Filename: ms1searchpy-2.3.7.dist-info/top_level.txt
 Comment: 
 
-Filename: ms1searchpy-2.3.6.dist-info/RECORD
+Filename: ms1searchpy-2.3.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ms1searchpy/combine.py

```diff
@@ -1,12 +1,14 @@
 from .main import final_iteration
 import pandas as pd
 from collections import defaultdict
 import argparse
+import logging
 
+logger = logging.getLogger(__name__)
 
 def run():
     parser = argparse.ArgumentParser(
         description='Combine DirectMS1 search results',
         epilog='''
 
     Example usage
@@ -17,34 +19,36 @@
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 
     parser.add_argument('file', nargs='+', help='input tsv PFMs_ML files')
     parser.add_argument('-out', help='prefix output file names', default='combined')
     parser.add_argument('-prots_full', help='path to any of *_proteins_full.tsv file. By default this file will be searched in the folder with PFMs_ML files', default='')
     parser.add_argument('-fdr', help='protein fdr filter in %%', default=1.0, type=float)
     parser.add_argument('-prefix', help='decoy prefix', default='DECOY_')
-    parser.add_argument('-nproc',   help='number of processes', default=1, type=int)
+    parser.add_argument('-nproc', help='number of processes', default=1, type=int)
     args = vars(parser.parse_args())
+    logging.basicConfig(format='%(levelname)9s: %(asctime)s %(message)s',
+            datefmt='[%H:%M:%S]', level=logging.INFO)
 
-    df1 = False
+    df1 = None
     for idx, filen in enumerate(args['file']):
         df3 = pd.read_csv(filen, sep='\t')
         df3['ids'] = df3['ids'].apply(lambda x: '%d:%s' % (idx, str(x)))
-        if df1 is False:
+        if df1 is None:
             df1 = df3
             if args['prots_full']:
                 df2 = pd.read_csv(args['prots_full'], sep='\t')
             else:
                 try:
                     df2 = pd.read_csv(filen.replace('_PFMs_ML.tsv', '_proteins_full.tsv'), sep='\t')
                 except:
-                    print('Proteins_full file is missing!')
+                    logging.critical('Proteins_full file is missing!')
                     break
 
         else:
-            df1 = df1.append(df3, ignore_index=True)
+            df1 = pd.concat([df1, df3], ignore_index=True)
 
     pept_prot = defaultdict(set)
     for seq, prots in df1[['seqs', 'proteins']].values:
         for dbname in prots.split(';'):
             pept_prot[seq].add(dbname)
 
     protsN = dict()
```

## ms1searchpy/directms1quant.py

```diff
@@ -1,18 +1,13 @@
 from __future__ import division
 import argparse
-import pkg_resources
 import pandas as pd
-import ast
-import subprocess
 import numpy as np
 from scipy.stats import binom, ttest_ind
-from collections import defaultdict
-import itertools
-from pyteomics import auxiliary as aux
+import logging
 
 def calc_sf_all(v, n, p):
     sf_values = -np.log10(binom.sf(v-1, n, p))
     sf_values[v <= 1] = 0
     sf_values[np.isinf(sf_values)] = 20
     sf_values[n == 0] = 0
     return sf_values
@@ -37,14 +32,18 @@
     parser.add_argument('-fold_change_abs', help='Use absolute log2 scale FC threshold instead of standard deviations', action='store_true')
     parser.add_argument('-qval', help='qvalue threshold', default=0.05, type=float)
     parser.add_argument('-intensity_norm', help='Intensity normalization: 0-none, 1-median', default=1, type=int)
     parser.add_argument('-all_proteins', help='use all proteins instead of FDR controlled', action='store_true')
     parser.add_argument('-all_pfms', help='use all PFMs instead of ML controlled', action='store_true')
     parser.add_argument('-output_peptides', help='Add output table with peptides', action='store_true')
     args = vars(parser.parse_args())
+    logging.basicConfig(format='%(levelname)9s: %(asctime)s %(message)s',
+            datefmt='[%H:%M:%S]', level=logging.INFO)
+    logger = logging.getLogger(__name__)
+
 
     replace_label = '_proteins_full.tsv'
 
     fold_change = float(args['fold_change'])
 
     df_final = False
 
@@ -70,15 +69,15 @@
                 df0 = pd.read_table(z.replace('_proteins_full.tsv', '_PFMs_ML.tsv'))
 
                 if not args['all_pfms']:
 
                     df0 = df0[df0['qpreds'] <= 10]
                 allowed_peptides.update(df0['seqs'])
 
-    print('Total number of TARGET protein GROUPS %d' % (len(allowed_prots)/2, ))
+    logger.info('Total number of TARGET protein GROUPS: %d', len(allowed_prots) / 2)
 
     for i in range(1, 3, 1):
         sample_num = 'S%d' % (i, )
         if args.get(sample_num, 0):
             for z in args[sample_num]:
                 df3 = pd.read_table(z.replace(replace_label, '_PFMs.tsv'))
                 df3 = df3[df3['sequence'].apply(lambda x: x in allowed_peptides)]
@@ -92,15 +91,14 @@
     for i in range(1, 3, 1):
         sample_num = 'S%d' % (i, )
         if args.get(sample_num, 0):
             all_s_lbls[sample_num] = []
             for z in args[sample_num]:
                 label = z.replace(replace_label, '')
                 all_s_lbls[sample_num].append(label)
-                df1 = pd.read_table(z)
                 df3 = pd.read_table(z.replace(replace_label, '_PFMs.tsv'))
 
                 df3 = df3[df3['sequence'].apply(lambda x: x in allowed_peptides)]
 
                 # allowed_prots2 = set()
                 # df3_tmp = df3[df3['proteins'].apply(lambda x: any(z in allowed_prots for z in x.split(';')))]
                 # for dbnames in set(df3_tmp['proteins'].values):
@@ -121,33 +119,32 @@
 
                 df3 = df3.drop_duplicates(subset='sequence')
 
                 df3[label] = df3['Intensity']
                 df3['protein'] = df3['proteins']
                 df3['peptide'] = df3['sequence']
                 df3 = df3[['origseq', 'peptide', 'protein', label]]
-                    
+
                 if df_final is False:
-                    label_basic = label
                     df_final = df3.reset_index(drop=True)
                 else:
                     df_final = df_final.reset_index(drop=True).merge(df3.reset_index(drop=True), on='peptide', how='outer')
                     df_final.protein_x.fillna(value=df_final.protein_y, inplace=True)
                     df_final.origseq_x.fillna(value=df_final.origseq_y, inplace=True)
                     df_final['protein'] = df_final['protein_x']
                     df_final['origseq'] = df_final['origseq_x']
 
                     df_final = df_final.drop(columns=['protein_x', 'protein_y'])
                     df_final = df_final.drop(columns=['origseq_x', 'origseq_y'])
 
 
-    print('Total number of peptide sequences used in quantitation %d' % (len(set(df_final['origseq'])), ))
+    logger.info('Total number of peptide sequences used in quantitation: %d', len(set(df_final['origseq'])))
     # print('Total number of proteins used in quantitation %d' % (len(allowed_prots_all), ))
 
-            
+
     df_final = df_final.assign(protein=df_final['protein'].str.split(';')).explode('protein').reset_index(drop=True)
 
     df_final = df_final.set_index('peptide')
     df_final['proteins'] = df_final['protein']
     df_final = df_final.drop(columns=['protein'])
     # cols = df_final.columns.tolist()
     cols = [z for z in df_final.columns.tolist() if not z.startswith('mz_')]
@@ -155,31 +152,29 @@
     cols.insert(0, 'proteins')
     df_final = df_final[cols]
 
     all_lbls = all_s_lbls['S1'] + all_s_lbls['S2']
 
     df_final_copy = df_final.copy()
 
-    df_res_list = []
-
     custom_min_samples = int(args['min_samples'])
     if custom_min_samples == 0:
         custom_min_samples = int(len(all_lbls)/2)
 
     df_final = df_final_copy.copy()
 
     max_missing = len(all_lbls) - custom_min_samples
 
-    print('Allowed max number of missing values: %d' % (max_missing, ))
+    logger.info('Allowed max number of missing values: %d', max_missing)
 
     df_final['nummissing'] = df_final.isna().sum(axis=1)
     df_final['nonmissing'] = df_final['nummissing'] <= max_missing
 
     df_final = df_final[df_final['nonmissing']]
-    print('Total number of PFMs passed missing values threshold %d' % (len(df_final), ))
+    logger.info('Total number of PFMs passed missing values threshold: %d', len(df_final))
 
 
     df_final['S2_mean'] = df_final[all_s_lbls['S2']].mean(axis=1)
     df_final['S1_mean'] = df_final[all_s_lbls['S1']].mean(axis=1)
     df_final['FC_raw'] = np.log2(df_final['S2_mean']/df_final['S1_mean'])
 
     FC_max = df_final['FC_raw'].max()
@@ -248,22 +243,22 @@
         FC_mean, FC_std, covvalue_cor = calibrate_mass(0.05, -df_final_for_calib['FC'].min(), df_final_for_calib['FC'].max(), df_final_for_calib['FC'])
     except:
         FC_mean, FC_std, covvalue_cor = calibrate_mass(0.1, -df_final_for_calib['FC'].min(), df_final_for_calib['FC'].max(), df_final_for_calib['FC'])
     # print('df_final_FC', FC_mean, FC_std)
 
     # FC_l = FC_mean-fold_change
     # FC_r = FC_mean+fold_change
-    
+
     if not args['fold_change_abs']:
         fold_change = FC_std * fold_change
-    print('absolute FC threshold = %.2f' % (fold_change, ))
+    logger.info('Absolute FC threshold = %.2f', fold_change)
     FC_l = -fold_change
     FC_r = fold_change
 
-    
+
     df_final['up'] = df_final['sign'] * (df_final['FC'] >= FC_r)
     df_final['down'] = df_final['sign'] * (df_final['FC'] <= FC_l)
 
     df_final = df_final.sort_values(by=['nummissing', 'intensity_median'], ascending=(True, False))
     df_final = df_final.drop_duplicates(subset=('origseq', 'proteins'))
 
     up_dict = df_final.groupby('proteins')['up'].sum().to_dict()
@@ -272,37 +267,36 @@
     ####### !!!!!!! #######
     df_final['up'] = df_final.apply(lambda x: x['up'] if up_dict.get(x['proteins'], 0) >= down_dict.get(x['proteins'], 0) else x['down'], axis=1)
     protsN = df_final.groupby('proteins')['up'].count().to_dict()
 
     prots_up = df_final.groupby('proteins')['up'].sum()
 
     N_decoy_total = df_final['decoy'].sum()
-    changed_decoy_total = df_final[(df_final['p-value'] <= p_val_threshold) & (df_final['decoy'])].shape[0]
 
     upreg_decoy_total = df_final[df_final['decoy']]['up'].sum()
 
     p_up = upreg_decoy_total / N_decoy_total
 
     names_arr = np.array(list(protsN.keys()))
 
-    print('Total number of proteins used in quantitation: %d' % (sum(not z.startswith('DECOY_') for z in names_arr), ))
-    print('Total number of peptides: %d' % (len(df_final), ))
-    print('Total number of decoy peptides: %d' % (N_decoy_total, ))
-    print('Total number of significantly changed decoy peptides: %d' % (upreg_decoy_total, ))
-    print('Probability of random peptide to be significantly changed: %.3f' % (p_up, ))
+    logger.info('Total number of proteins used in quantitation: %d', sum(not z.startswith('DECOY_') for z in names_arr))
+    logger.info('Total number of peptides: %d', len(df_final))
+    logger.info('Total number of decoy peptides: %d', N_decoy_total)
+    logger.info('Total number of significantly changed decoy peptides: %d', upreg_decoy_total)
+    logger.info('Probability of random peptide to be significantly changed: %.3f', p_up)
     # print(N_decoy_total, upreg_decoy_total, p_up)
-    
+
     if args['output_peptides']:
         df_final.to_csv(path_or_buf=args['out']+'_quant_peptides.tsv', sep='\t', index=False)
-    
+
     v_arr = np.array(list(prots_up.get(k, 0) for k in names_arr))
     n_arr = np.array(list(protsN.get(k, 0) for k in names_arr))
 
     all_pvals = calc_sf_all(v_arr, n_arr, p_up)
-    
+
     total_set = set()
 
     FC_up_dict_basic = df_final.groupby('proteins')['FC'].median().to_dict()
     FC_up_dict_raw_basic = df_final.groupby('proteins')['FC_raw'].median().to_dict()
 
     df_final = df_final[df_final['up']>0]
 
@@ -351,15 +345,15 @@
 
     df_out_f = df_out[(df_out['BH_pass']) & (df_out['FC_pass'])]
 
     df_out_f.to_csv(path_or_buf=args['out']+'.tsv', sep='\t', index=False)
 
     total_set.update([z.split('|')[1] for z in set(df_out_f['dbname'])])
 
-    print('Total number of significantly changed proteins: %d' % (len(total_set), ))
+    logger.info('Total number of significantly changed proteins: %d', len(total_set))
 
     f1 = open(args['out'] + '_proteins_for_stringdb.txt', 'w')
     for z in total_set:
         f1.write(z + '\n')
     f1.close()
 
 if __name__ == '__main__':
```

## ms1searchpy/main.py

```diff
@@ -1,97 +1,55 @@
 import os
-from . import utils
 import numpy as np
 from scipy.stats import scoreatpercentile
 from scipy.optimize import curve_fit
 from scipy import exp
 import operator
 from copy import copy, deepcopy
-from collections import defaultdict, Counter
-import re
-from pyteomics import parser, mass, fasta, auxiliary as aux, achrom
+from collections import defaultdict, deque, Counter
+from pyteomics import parser, mass, auxiliary as aux, achrom
 try:
     from pyteomics import cmass
 except ImportError:
     cmass = mass
 import subprocess
-from sklearn import linear_model
 import tempfile
 import pandas as pd
 import matplotlib
 matplotlib.use('Agg')
-import matplotlib.pyplot as plt
 from multiprocessing import Queue, Process, cpu_count
-from itertools import chain
 try:
     import seaborn
     seaborn.set(rc={'axes.facecolor':'#ffffff'})
     seaborn.set_style('whitegrid')
 except:
     pass
 
-from .utils import calc_sf_all, recalc_spc
+from . import utils
 from .utils_figures import plot_outfigures
 import lightgbm as lgb
-import pandas as pd
-from sklearn.model_selection import train_test_split
-from scipy.stats import zscore, spearmanr
-import pandas as pd
-from pyteomics import pepxml, achrom, auxiliary as aux, mass, fasta, mzid, parser
 from pyteomics import electrochem
-import numpy as np
 import random
-SEED = 42
-from sklearn.model_selection import train_test_split
-from os import path, mkdir
-from collections import Counter, defaultdict
+SEED = 50
 import warnings
-import pylab as plt
 warnings.formatwarning = lambda msg, *args, **kw: str(msg) + '\n'
 
-import pandas as pd
-from sklearn.model_selection import train_test_split, KFold
-import os
-from collections import Counter, defaultdict
-from scipy.stats import scoreatpercentile
-from sklearn.isotonic import IsotonicRegression
-import warnings
-import numpy as np
-
-import matplotlib
+import logging
 import numpy
 import pandas
-import random
-import sklearn
-import matplotlib.pyplot as plt
-
-from sklearn import (
-    feature_extraction, feature_selection, decomposition, linear_model,
-    model_selection, metrics, svm
-)
-
-import scipy
-from scipy.stats import rankdata
-from copy import deepcopy
+from sklearn import metrics
 import csv
-
-from scipy.stats import rankdata
-import lightgbm as lgb
-import numpy as np
-import pandas as pd
-import matplotlib.pyplot as plt
-from itertools import chain
-import time as timemodule
 import ast
-from sklearn import metrics
+import itertools as it
+import re
 
-SEED = 50
+logger = logging.getLogger(__name__)
 
 def worker_RT(qin, qout, shift, step, RC=False, elude_path=False, ns=False, nr=False, win_sys=False):
-    pepdict = dict()    
+    pepdict = dict()
     if elude_path:
         outtrain_name = os.path.join(tempfile.gettempdir(), os.urandom(24).hex())
         outtrain = open(outtrain_name, 'w')
         outres_name = os.path.join(tempfile.gettempdir(), os.urandom(24).hex())
         for seq, RT in zip(ns, nr):
             outtrain.write(seq + '\t' + str(RT) + '\n')
         outtrain.close()
@@ -130,15 +88,15 @@
 
     p1 = set(resdict['seqs'])
 
     pep_pid = defaultdict(set)
     pid_pep = defaultdict(set)
     banned_dict = dict()
     for pep, pid in zip(resdict['seqs'], resdict['ids']):
-        
+
         pep_pid[pep].add(pid)
         pid_pep[pid].add(pep)
         if pep in banned_dict:
             banned_dict[pep] += 1
         else:
             banned_dict[pep] = 1
 
@@ -162,15 +120,15 @@
                     n_map_dict[v].append(k)
 
                 decoy_set = set()
                 for k in protsN:
                     if isdecoy_key(k):
                         decoy_set.add(k)
                 decoy_set = list(decoy_set)
-                
+
 
                 prots_spc2 = defaultdict(set)
                 for pep, proteins in pept_prot.items():
                     if pep in p1:
                         for protein in proteins:
                             prots_spc2[protein].add(pep)
 
@@ -187,15 +145,14 @@
 
                 tmp_spc_new = dict((k, len(v)) for k, v in prots_spc2.items())
 
 
                 top100decoy_score_tmp = [tmp_spc_new.get(dprot, 0) for dprot in decoy_set]
                 top100decoy_score_tmp_sum = float(sum(top100decoy_score_tmp))
 
-            tmp_spc = tmp_spc_new
             prots_spc = tmp_spc_new
             if not prots_spc_copy:
                 prots_spc_copy = deepcopy(prots_spc)
 
             for idx, v in enumerate(decoy_set):
                 if v in unstable_prots:
                     top100decoy_score_tmp_sum -= top100decoy_score_tmp[idx]
@@ -215,24 +172,24 @@
             v_arr_small = []
             for k, v in best_match_dict.items():
                 n_arr_small.append(k)
                 names_arr_small.append(v)
                 v_arr_small.append(prots_spc[v])
 
             prots_spc_basic = dict()
-            all_pvals = calc_sf_all(np.array(v_arr_small), n_arr_small, p)
+            all_pvals = utils.calc_sf_all(np.array(v_arr_small), n_arr_small, p)
             for idx, k in enumerate(names_arr_small):
                 prots_spc_basic[k] = all_pvals[idx]
 
             if not p0:
                 p0 = float(p)
 
                 prots_spc_tmp = dict()
                 v_arr = np.array([prots_spc[k] for k in names_arr])
-                all_pvals = calc_sf_all(v_arr, n_arr, p)
+                all_pvals = utils.calc_sf_all(v_arr, n_arr, p)
                 for idx, k in enumerate(names_arr):
                     prots_spc_tmp[k] = all_pvals[idx]
 
                 sortedlist_spc = sorted(prots_spc_tmp.items(), key=operator.itemgetter(1))[::-1]
                 with open(base_out_name + '_proteins_full_noexclusion.tsv', 'w') as output:
                     output.write('dbname\tscore\tmatched peptides\ttheoretical peptides\n')
                     for x in sortedlist_spc:
@@ -254,29 +211,29 @@
                         if banned_dict[pep] == 0:
                             for bprot in pept_prot[pep]:
                                 tmp_spc_new[bprot] -= 1
                                 unstable_prots.add(bprot)
             else:
 
                 v_arr = np.array([prots_spc[k] for k in names_arr])
-                all_pvals = calc_sf_all(v_arr, n_arr, p)
+                all_pvals = utils.calc_sf_all(v_arr, n_arr, p)
                 for idx, k in enumerate(names_arr):
                     prots_spc_basic[k] = all_pvals[idx]
 
                 for k, v in prots_spc_basic.items():
                     if k not in prots_spc_final:
                         prots_spc_final[k] = v
 
                 break
 
             prot_fdr = aux.fdr(prots_spc_final.items(), is_decoy=isdecoy)
             if prot_fdr >= 12.5 * fdr:
 
                 v_arr = np.array([prots_spc[k] for k in names_arr])
-                all_pvals = calc_sf_all(v_arr, n_arr, p)
+                all_pvals = utils.calc_sf_all(v_arr, n_arr, p)
                 for idx, k in enumerate(names_arr):
                     prots_spc_basic[k] = all_pvals[idx]
 
                 for k, v in prots_spc_basic.items():
                     if k not in prots_spc_final:
                         prots_spc_final[k] = v
                 break
@@ -285,30 +242,29 @@
         prots_spc_basic2 = copy(prots_spc_final)
     else:
         prots_spc_basic2 = prots_spc_basic2
         for k in prots_spc_final:
             if k not in prots_spc_basic2:
                 prots_spc_basic2[k] = 0
     prots_spc_final = dict()
-    prots_spc_final2 = dict()
 
     if n == 0:
         try:
             n = cpu_count()
         except NotImplementedError:
             n = 1
 
     if n == 1 or os.name == 'nt':
         qin = []
         qout = []
         for mass_koef in range(10):
             rtt_koef = mass_koef
             qin.append((mass_koef, rtt_koef))
         qout = worker(qin, qout, mass_diff, rt_diff, resdict, protsN, pept_prot, isdecoy_key, isdecoy, fdr, prots_spc_basic2, True)
-        
+
         for item, item2 in qout:
             if item2:
                 prots_spc_copy = item2
             for k in protsN:
                 if k not in prots_spc_final:
                     prots_spc_final[k] = [item.get(k, 0.0), ]
                 else:
@@ -370,42 +326,42 @@
     if len(filtered_prots) < 1:
         filtered_prots = aux.filter(prots_spc.items(), fdr=fdr, key=escore, is_decoy=isdecoy, remove_decoy=True, formula=1, full_output=True, correction=0)
     identified_proteins = 0
 
     for x in filtered_prots:
         identified_proteins += 1
 
-    print('TOP 5 identified proteins:')
-    print('dbname\tscore\tmatched peptides\ttheoretical peptides')
+    logger.info('TOP 5 identified proteins:')
+    logger.info('dbname\tscore\tmatched peptides\ttheoretical peptides')
     for x in filtered_prots[:5]:
-        print('\t'.join((str(x[0]), str(x[1]), str(int(prots_spc_copy[x[0]])), str(protsN[x[0]]))))
-    print('\nFinal stage search: identified proteins = %d' % (identified_proteins, ))
-    # print('R=', r)
+        logger.info('\t'.join((str(x[0]), str(x[1]), str(int(prots_spc_copy[x[0]])), str(protsN[x[0]]))))
+    logger.info('Final stage search: identified proteins = %d', identified_proteins)
+
     with open(base_out_name + '_proteins.tsv', 'w') as output:
         output.write('dbname\tscore\tmatched peptides\ttheoretical peptides\tdecoy\n')
         for x in filtered_prots:
             output.write('\t'.join((x[0], str(x[1]), str(prots_spc_copy[x[0]]), str(protsN[x[0]]), str(isdecoy(x)))) + '\n')
 
 
     if fname and identified_proteins > 10:
 
         df0 = pd.read_table(os.path.splitext(fname)[0] + '.tsv')
         df1_peptides = pd.read_table(os.path.splitext(fname)[0] + '_PFMs.tsv')
         df1_peptides['decoy'] = df1_peptides['proteins'].apply(lambda x: any(isdecoy_key(z) for z in x.split(';')))
-        
+
         df1_proteins = pd.read_table(os.path.splitext(fname)[0] + '_proteins_full.tsv')
         df1_proteins_f = pd.read_table(os.path.splitext(fname)[0] + '_proteins.tsv')
         top_proteins = set(df1_proteins_f['dbname'])
         df1_peptides_f = df1_peptides[df1_peptides['proteins'].apply(lambda x: any(z in top_proteins for z in x.split(';')))]
 
         plot_outfigures(df0, df1_peptides, df1_peptides_f,
             base_out_name, df_proteins=df1_proteins,
             df_proteins_f=df1_proteins_f)
 
-    print('The search for file %s is finished.' % (base_out_name, ))
+    logger.info('The search for file %s is finished.', base_out_name)
 
 def noisygaus(x, a, x0, sigma, b):
     return a * exp(-(x - x0) ** 2 / (2 * sigma ** 2)) + b
 
 def calibrate_mass(bwidth, mass_left, mass_right, true_md):
 
     bbins = np.arange(-mass_left, mass_right, bwidth)
@@ -435,16 +391,16 @@
     utils.seen_decoy.clear()
     args = utils.prepare_decoy_db(args)
     for filename in args['files']:
         try:
             args['file'] = filename
             process_peptides(deepcopy(args))
         except Exception as e:
-            print(e)
-            print('Search is failed for file: %s' % (filename, ))
+            logger.error(e)
+            logger.error('Search is failed for file: %s', filename)
     return 1
 
 
 def peptide_processor(peptide, **kwargs):
     seqm = peptide
     results = []
     m = cmass.fast_mass(seqm, aa_mass=kwargs['aa_mass']) + kwargs['aa_mass'].get('Nterm', 0) + kwargs['aa_mass'].get('Cterm', 0)
@@ -454,16 +410,14 @@
     if acc_r == acc_l:
         dm_r = dm_l
     else:
         dm_r = acc_r * m / 1.0e6
     start = nmasses.searchsorted(m - dm_l)
     end = nmasses.searchsorted(m + dm_r)
     for i in range(start, end):
-        peak_id = ids[i]
-        I = Is[i]
         massdiff = (m - nmasses[i]) / m * 1e6
         mods = 0
         results.append((seqm, massdiff, mods, i))
     return results
 
 
 def prepare_peptide_processor(fname, args):
@@ -480,18 +434,18 @@
 
     min_ch = args['cmin']
     max_ch = args['cmax']
 
     min_isotopes = args['i']
     min_scans = args['sc']
 
-    print('\nReading file %s' % (fname, ))
+    logger.info('Reading file %s', fname)
 
     df_features = utils.iterate_spectra(fname, min_ch, max_ch, min_isotopes, min_scans)
-    
+
     # Sort by neutral mass
     df_features = df_features.sort_values(by='massCalib')
 
     nmasses = df_features['massCalib'].values
     rts = df_features['rtApex'].values
     charges = df_features['charge'].values
     ids = df_features['id'].values
@@ -501,15 +455,15 @@
     mzraw = df_features['mz'].values
     avraw = np.zeros(len(df_features))
     if len(set(df_features['FAIMS'])) > 1:
         imraw = df_features['FAIMS'].values
     else:
         imraw = df_features['ion_mobility'].values
 
-    print('Number of peptide isotopic clusters passed filters: %d\n' % (len(nmasses), ))
+    logger.info('Number of peptide isotopic clusters passed filters: %d', len(nmasses))
 
     fmods = args['fmods']
     aa_mass = deepcopy(mass.std_aa_mass)
     if fmods:
         for mod in fmods.split(','):
             m, aa = mod.split('@')
             if aa == '[':
@@ -518,16 +472,14 @@
                 aa_mass['Cterm'] = float(m)
             else:
                 aa_mass[aa] += float(m)
 
     acc_l = args['ptol']
     acc_r = args['ptol']
 
-    # print(df_features.columns)
-
     return {'aa_mass': aa_mass, 'acc_l': acc_l, 'acc_r': acc_r, 'args': args}, df_features
 
 
 def peptide_processor_iter_isoforms(peptide, **kwargs):
     out = []
     out.append(peptide_processor(peptide, **kwargs))
     return out
@@ -585,28 +537,44 @@
 
     elude_path = args['elude']
     elude_path = elude_path.strip()
 
     deeplc_path = args['deeplc']
     deeplc_path = deeplc_path.strip()
 
+    deeplc_model_path = args['deeplc_model_path']
+    deeplc_model_path = deeplc_model_path.strip()
+
+    deeplc_extra_args = []
+    if len(deeplc_model_path) > 0:
+        deeplc_extra_args.append("--file_model")
+        if deeplc_model_path.endswith('.hdf5'):
+            deeplc_extra_args.append(deeplc_model_path)
+            # deeplc_models = deeplc_model_path
+        else:
+            deeplc_extra_args.extend([os.path.join(deeplc_model_path,f) for f in os.listdir(deeplc_model_path) if f.endswith(".hdf5")])
+            # deeplc_models = " ".join([os.path.join(deeplc_model_path,f) for f in os.listdir(deeplc_model_path) if f.endswith(".hdf5")])
+        # deeplc_extra_args.extend(["--file_model", deeplc_models, ])
+    if args['deeplc_library']:
+        deeplc_extra_args.extend(['--use_library', args['deeplc_library'], '--write_library'])
+
     calib_path = args['pl']
     calib_path = calib_path.strip()
 
     if calib_path and args['ts']:
         args['ts'] = 0
-        print('Two-stage RT prediction does not work with list of MS/MS identified peptides...')
+        logger.info('Two-stage RT prediction does not work with list of MS/MS identified peptides...')
 
     args['enzyme'] = utils.get_enzyme(args['e'])
 
     ms1results = []
     peps = utils.peptide_gen(args)
     kwargs, df_features = prepare_peptide_processor(fname_orig, args)
     func = peptide_processor_iter_isoforms
-    print('Running the search ...')
+    logger.info('Running the search ...')
     for y in utils.multimap(1, func, peps, **kwargs):
         for result in y:
             if len(result):
                 ms1results.extend(result)
 
     prefix = args['prefix']
     protsN, pept_prot = utils.get_prot_pept_map(args)
@@ -647,18 +615,18 @@
         names_arr = np.array(list(prots_spc.keys()))
         v_arr = np.array(list(prots_spc.values()))
         n_arr = np.array([protsN[k] for k in prots_spc])
 
         top100decoy_score = [prots_spc.get(dprot, 0) for dprot in protsN if isdecoy_key(dprot)]
         top100decoy_N = [val for key, val in protsN.items() if isdecoy_key(key)]
         p = np.mean(top100decoy_score) / np.mean(top100decoy_N)
-        print('Stage 0 search: probability of random match for theoretical peptide = %.3f' % (np.mean(top100decoy_score) / np.mean(top100decoy_N)))
+        logger.info('Stage 0 search: probability of random match for theoretical peptide = %.3f', (np.mean(top100decoy_score) / np.mean(top100decoy_N)))
 
         prots_spc = dict()
-        all_pvals = calc_sf_all(v_arr, n_arr, p)
+        all_pvals = utils.calc_sf_all(v_arr, n_arr, p)
         for idx, k in enumerate(names_arr):
             prots_spc[k] = all_pvals[idx]
 
         checked = set()
         for k, v in list(prots_spc.items()):
             if k not in checked:
                 if isdecoy_key(k):
@@ -673,17 +641,17 @@
         filtered_prots = aux.filter(prots_spc.items(), fdr=0.05, key=escore, is_decoy=isdecoy, remove_decoy=True, formula=1,
                                     full_output=True)
 
         identified_proteins = 0
 
         for x in filtered_prots:
             identified_proteins += 1
-        print('Stage 0 search: identified proteins = %d\n' % (identified_proteins, ))
+        logger.info('Stage 0 search: identified proteins = %d', identified_proteins)
 
-        print('Running mass recalibration...')
+        logger.info('Running mass recalibration...')
 
         df1 = pd.DataFrame()
         df1['mass diff'] = resdict['md']
         df1['mc'] = resdict['mc']
         df1['iorig'] = resdict['iorig']
         df1['seqs'] = resdict['seqs']
         # df1['orig_md'] = true_md
@@ -693,15 +661,15 @@
         true_prots = set(x[0] for x in filtered_prots)
         for pep, proteins in pept_prot.items():
             if any(protein in true_prots for protein in proteins):
                 true_seqs.add(pep)
 
 
         df1['top_peps'] = (df1['mc'] == 0) & (df1['seqs'].apply(lambda x: x in true_seqs))
-        
+
         df1['mz'] = df1['iorig'].apply(lambda x: mzraw[x])
         df1['nIsotopes'] = df1['iorig'].apply(lambda x: Isotopes[x])
         df1['RT'] = df1['iorig'].apply(lambda x: rts[x])
         df1['Intensity'] = df1['iorig'].apply(lambda x: Is[x])
 
         mass_calib_arg = args['mcalib']
 
@@ -722,15 +690,15 @@
             else:
                 df1['im_qcut'] = pd.qcut(df1['im'], 10, labels=range(10)).astype(str)
                 for im_value in set(df1['im_qcut']):
                     idx1 = df1['im_qcut'] == im_value
                     df1.loc[idx1, 'qpreds'] = str(im_value) + pd.qcut(df1.loc[idx1, 'RT'], 10, labels=range(10)).astype(str)
 
             # df1['qpreds'] = pd.qcut(df1['RT'], 10, labels=range(10))#.astype(int)
-                
+
             cor_dict = df1[df1['top_peps']].groupby('qpreds')['mass diff'].median().to_dict()
 
             rt_q_list = list(range(10))
             for im_value in set(df1['im_qcut']):
                 for rt_q in rt_q_list:
                     lbl_cur = str(im_value) + str(rt_q)
                     if lbl_cur not in cor_dict:
@@ -758,49 +726,44 @@
 
 
 
 
         mass_left = args['ptol']
         mass_right = args['ptol']
 
-        
-
         try:
             mass_shift_cor, mass_sigma_cor, covvalue_cor = calibrate_mass(0.001, mass_left, mass_right, df1[df1['top_peps']]['mass diff corrected'])
         except:
             mass_shift_cor, mass_sigma_cor, covvalue_cor = calibrate_mass(0.01, mass_left, mass_right, df1[df1['top_peps']]['mass diff corrected'])
 
         try:
             mass_shift, mass_sigma, covvalue = calibrate_mass(0.001, mass_left, mass_right, df1[df1['top_peps']]['mass diff'])
         except:
             mass_shift, mass_sigma, covvalue = calibrate_mass(0.01, mass_left, mass_right, df1[df1['top_peps']]['mass diff'])
 
         if mass_calib_arg:
-            print('Uncalibrated mass shift: %.3f ppm' % (mass_shift, ))
-            print('Uncalibrated mass sigma: %.3f ppm' % (mass_sigma, ))
+            logger.info('Uncalibrated mass shift: %.3f ppm', mass_shift)
+            logger.info('Uncalibrated mass sigma: %.3f ppm', mass_sigma)
 
-        print('Estimated mass shift: %.3f ppm' % (mass_shift_cor, ))
-        print('Estimated mass sigma: %.3f ppm' % (mass_sigma_cor, ))
+        logger.info('Estimated mass shift: %.3f ppm', mass_shift_cor)
+        logger.info('Estimated mass sigma: %.3f ppm', mass_sigma_cor)
 
         out_log.write('Estimated mass shift: %s ppm\n' % (mass_shift_cor, ))
         out_log.write('Estimated mass sigma: %s ppm\n' % (mass_sigma_cor, ))
 
         resdict['md'] = df1['mass diff corrected'].values
 
         mass_shift = mass_shift_cor
         mass_sigma = mass_sigma_cor
 
         e_all = abs(resdict['md'] - mass_shift) / (mass_sigma)
         r = 3.0
         e_ind = e_all <= r
         resdict = filter_results(resdict, e_ind)
 
-        zs_all = e_all[e_ind] ** 2
-
-
         e_ind = np.array([Isotopes[iorig] for iorig in resdict['iorig']]) >= min_isotopes_calibration
         resdict2 = filter_results(resdict, e_ind)
 
         e_ind = resdict2['mc'] == 0
         resdict2 = filter_results(resdict2, e_ind)
 
         p1 = set(resdict2['seqs'])
@@ -819,18 +782,18 @@
         names_arr = np.array(list(prots_spc.keys()))
         v_arr = np.array(list(prots_spc.values()))
         n_arr = np.array([protsN[k] for k in prots_spc])
 
         top100decoy_score = [prots_spc.get(dprot, 0) for dprot in protsN if isdecoy_key(dprot)]
         top100decoy_N = [val for key, val in protsN.items() if isdecoy_key(key)]
         p = np.mean(top100decoy_score) / np.mean(top100decoy_N)
-        print('Stage 1 search: probability of random match for theoretical peptide = %.3f' % (np.mean(top100decoy_score) / np.mean(top100decoy_N)))
+        logger.info('Stage 1 search: probability of random match for theoretical peptide = %.3f', (np.mean(top100decoy_score) / np.mean(top100decoy_N)))
 
         prots_spc = dict()
-        all_pvals = calc_sf_all(v_arr, n_arr, p)
+        all_pvals = utils.calc_sf_all(v_arr, n_arr, p)
         for idx, k in enumerate(names_arr):
             prots_spc[k] = all_pvals[idx]
 
         checked = set()
         for k, v in list(prots_spc.items()):
             if k not in checked:
                 if isdecoy_key(k):
@@ -845,19 +808,19 @@
         filtered_prots = aux.filter(prots_spc.items(), fdr=0.05, key=escore, is_decoy=isdecoy, remove_decoy=True, formula=1,
                                     full_output=True)
 
         identified_proteins = 0
 
         for x in filtered_prots:
             identified_proteins += 1
-        print('Stage 1 search: identified proteins = %d\n' % (identified_proteins, ))
+        logger.info('Stage 1 search: identified proteins = %d', identified_proteins)
 
 
 
-        print('Running RT prediction...')
+        logger.info('Running RT prediction...')
 
 
         e_ind = np.array([Isotopes[iorig] for iorig in resdict['iorig']]) >= 1
         resdict2 = filter_results(resdict, e_ind)
 
         e_ind = resdict2['mc'] == 0
         resdict2 = filter_results(resdict2, e_ind)
@@ -911,27 +874,27 @@
             true_rt2 = df1['RT exp'].values
 
         else:
             true_seqs2 = true_seqs
             true_rt2 = true_rt
 
 
-        print('First-stage peptides used for RT prediction: %d' % (len(true_seqs), ))
+        logger.info('First-stage peptides used for RT prediction: %d', len(true_seqs))
 
         if args['ts'] != 2 and deeplc_path:
 
-            
+
             outtrain_name = os.path.join(tempfile.gettempdir(), os.urandom(24).hex())
             outtrain = open(outtrain_name, 'w')
             outcalib_name = os.path.join(tempfile.gettempdir(), os.urandom(24).hex())
             outcalib = open(outcalib_name, 'w')
             outres_name = os.path.join(tempfile.gettempdir(), os.urandom(24).hex())
             ns = true_seqs
             nr = true_rt
-            # print('Peptides used for RT prediction: %d' % (len(ns), ))
+
             ns2 = true_seqs2
             nr2 = true_rt2
 
             outtrain.write('seq,modifications,tr\n')
             for seq, RT in zip(ns2, nr2):
                 mods_tmp = '|'.join([str(idx+1)+'|Carbamidomethyl' for idx, aa in enumerate(seq) if aa == 'C'])
                 outtrain.write(seq + ',' + str(mods_tmp) + ',' + str(RT) + '\n')
@@ -939,27 +902,27 @@
 
             outcalib.write('seq,modifications,tr\n')
             for seq, RT in zip(ns, nr):
                 mods_tmp = '|'.join([str(idx+1)+'|Carbamidomethyl' for idx, aa in enumerate(seq) if aa == 'C'])
                 outcalib.write(seq + ',' + str(mods_tmp) + ',' + str(RT) + '\n')
             outcalib.close()
 
+            subprocess.call([deeplc_path, '--file_pred', outcalib_name, '--file_cal', outtrain_name, '--file_pred_out', outres_name] + deeplc_extra_args, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
 
-            subprocess.call([deeplc_path, '--file_pred', outcalib_name, '--file_cal', outtrain_name, '--file_pred_out', outres_name], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
             pepdict = dict()
             train_RT = []
             train_seq = []
             for x in open(outres_name).readlines()[1:]:
                 _, seq, _, RTexp, RT = x.strip().split(',')
                 pepdict[seq] = float(RT)
                 train_seq.append(seq)
                 train_RT.append(float(RTexp))
 
 
-            train_RT = np.array(train_RT)        
+            train_RT = np.array(train_RT)
             RT_pred = np.array([pepdict[s] for s in train_seq])
 
             rt_diff_tmp = RT_pred - train_RT
             RT_left = -min(rt_diff_tmp)
             RT_right = max(rt_diff_tmp)
 
             try:
@@ -968,32 +931,27 @@
             except:
                 start_width = (scoreatpercentile(rt_diff_tmp, 95) - scoreatpercentile(rt_diff_tmp, 5)) / 50
                 XRT_shift, XRT_sigma, covvalue = calibrate_RT_gaus(start_width, RT_left, RT_right, rt_diff_tmp)
             if np.isinf(covvalue):
                 XRT_shift, XRT_sigma, covvalue = calibrate_RT_gaus(0.1, RT_left, RT_right, rt_diff_tmp)
             if np.isinf(covvalue):
                 XRT_shift, XRT_sigma, covvalue = calibrate_RT_gaus(1.0, RT_left, RT_right, rt_diff_tmp)
-            # print('Calibrated RT shift: ', XRT_shift)
-            # print('Calibrated RT sigma: ', XRT_sigma)
-
-            # aa, bb, RR, ss = aux.linear_regression(RT_pred, train_RT)
 
         else:
             if args['ts'] != 2 and elude_path:
 
 
                 outtrain_name = os.path.join(tempfile.gettempdir(), os.urandom(24).hex())
                 outtrain = open(outtrain_name, 'w')
                 outcalib_name = os.path.join(tempfile.gettempdir(), os.urandom(24).hex())
                 outcalib = open(outcalib_name, 'w')
                 outres_name = os.path.join(tempfile.gettempdir(), os.urandom(24).hex())
 
                 ns = true_seqs
                 nr = true_rt
-                # print('Peptides used for RT prediction: %d' % (len(ns), ))
                 ns2 = true_seqs2
                 nr2 = true_rt2
                 for seq, RT in zip(ns, nr):
                     outtrain.write(seq + '\t' + str(RT) + '\n')
                 outtrain.close()
                 for seq, RT in zip(ns, nr):
                     outcalib.write(seq + '\t' + str(RT) + '\n')
@@ -1016,18 +974,14 @@
 
                 start_width = (scoreatpercentile(rt_diff_tmp, 95) - scoreatpercentile(rt_diff_tmp, 5)) / 50
                 XRT_shift, XRT_sigma, covvalue = calibrate_RT_gaus(start_width, RT_left, RT_right, rt_diff_tmp)
                 if np.isinf(covvalue):
                     XRT_shift, XRT_sigma, covvalue = calibrate_RT_gaus(0.1, RT_left, RT_right, rt_diff_tmp)
                 if np.isinf(covvalue):
                     XRT_shift, XRT_sigma, covvalue = calibrate_RT_gaus(1.0, RT_left, RT_right, rt_diff_tmp)
-                # print('Calibrated RT shift: ', XRT_shift)
-                # print('Calibrated RT sigma: ', XRT_sigma)
-
-                # aa, bb, RR, ss = aux.linear_regression(RT_pred, train_RT)
             else:
                 ns = true_seqs
                 nr = true_rt
                 ns2 = true_seqs2
                 nr2 = true_rt2
                 RC = achrom.get_RCs_vary_lcp(ns2, nr2)
                 RT_pred = np.array([achrom.calculate_RT(s, RC) for s in ns])
@@ -1040,68 +994,53 @@
 
                 start_width = (scoreatpercentile(rt_diff_tmp, 95) - scoreatpercentile(rt_diff_tmp, 5)) / 50
                 XRT_shift, XRT_sigma, covvalue = calibrate_RT_gaus(start_width, RT_left, RT_right, rt_diff_tmp)
                 if np.isinf(covvalue):
                     XRT_shift, XRT_sigma, covvalue = calibrate_RT_gaus(0.1, RT_left, RT_right, rt_diff_tmp)
                 if np.isinf(covvalue):
                     XRT_shift, XRT_sigma, covvalue = calibrate_RT_gaus(1.0, RT_left, RT_right, rt_diff_tmp)
-                # print('Calibrated RT shift: ', XRT_shift)
-                # print('Calibrated RT sigma: ', XRT_sigma)
-
-
-
-
-        print('First-stage calibrated RT shift: %.3f min' % (XRT_shift, ))
-        print('First-stage calibrated RT sigma: %.3f min' % (XRT_sigma, ))
 
 
-        # print(aa, bb, RR, ss)
+        logger.info('First-stage calibrated RT shift: %.3f min', XRT_shift)
+        logger.info('First-stage calibrated RT sigma: %.3f min', XRT_sigma)
 
-
-
-        best_sigma = XRT_sigma
         RT_sigma = XRT_sigma
 
     else:
-        print('No matches found')
+        logger.info('No matches found')
 
     if args['ts']:
-
-        # print('Running second stage RT prediction...')
-
-
         ns = np.array(ns)
         nr = np.array(nr)
         idx = np.abs((rt_diff_tmp) - XRT_shift) <= 3 * XRT_sigma
         ns = ns[idx]
         nr = nr[idx]
-        print('Second-stage peptides used for RT prediction: %d' % (len(ns), ))
+        logger.info('Second-stage peptides used for RT prediction: %d', len(ns))
 
         if deeplc_path:
 
 
 
             outtrain_name = os.path.join(tempfile.gettempdir(), os.urandom(24).hex())
             outtrain = open(outtrain_name, 'w')
             outres_name = os.path.join(tempfile.gettempdir(), os.urandom(24).hex())
 
-            # print('Peptides used for RT prediction: %d' % (len(ns), ))
             ll = len(ns)
             ns = ns[:ll]
             nr = nr[:ll]
 
             outtrain.write('seq,modifications,tr\n')
             for seq, RT in zip(ns, nr):
                 mods_tmp = '|'.join([str(idx+1)+'|Carbamidomethyl' for idx, aa in enumerate(seq) if aa == 'C'])
                 outtrain.write(seq + ',' + str(mods_tmp) + ',' + str(RT) + '\n')
             outtrain.close()
 
-            # [:int(len(ns)/2)] 
+            # [:int(len(ns)/2)]
 
-            subprocess.call([deeplc_path, '--file_pred', outtrain_name, '--file_cal', outtrain_name, '--file_pred_out', outres_name], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+            subprocess.call([deeplc_path, '--file_pred', outtrain_name, '--file_cal', outtrain_name, '--file_pred_out', outres_name] + deeplc_extra_args, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
             pepdict = dict()
             train_RT = []
             train_seq = []
             for x in open(outres_name).readlines()[1:]:
                 _, seq, _, RTexp, RT = x.strip().split(',')
                 pepdict[seq] = float(RT)
                 train_seq.append(seq)
@@ -1121,29 +1060,24 @@
             except:
                 start_width = (scoreatpercentile(rt_diff_tmp, 95) - scoreatpercentile(rt_diff_tmp, 5)) / 50
                 XRT_shift, XRT_sigma, covvalue = calibrate_RT_gaus(start_width, RT_left, RT_right, rt_diff_tmp)
             if np.isinf(covvalue):
                 XRT_shift, XRT_sigma, covvalue = calibrate_RT_gaus(0.1, RT_left, RT_right, rt_diff_tmp)
             if np.isinf(covvalue):
                 XRT_shift, XRT_sigma, covvalue = calibrate_RT_gaus(1.0, RT_left, RT_right, rt_diff_tmp)
-            # print('Calibrated RT shift: ', XRT_shift)
-            # print('Calibrated RT sigma: ', XRT_sigma)
-
-            # aa, bb, RR, ss = aux.linear_regression(RT_pred, train_RT)
 
         else:
 
             if elude_path:
 
-
                 outtrain_name = os.path.join(tempfile.gettempdir(), os.urandom(24).hex())
                 outtrain = open(outtrain_name, 'w')
                 outres_name = os.path.join(tempfile.gettempdir(), os.urandom(24).hex())
 
-                print(len(ns))
+                logger.debug(len(ns))
                 ll = len(ns)
                 ns = ns[:ll]
                 nr = nr[:ll]
                 for seq, RT in zip(ns, nr):
                     outtrain.write(seq + '\t' + str(RT) + '\n')
                 outtrain.close()
 
@@ -1165,18 +1099,14 @@
 
                 start_width = (scoreatpercentile(rt_diff_tmp, 95) - scoreatpercentile(rt_diff_tmp, 5)) / 50
                 XRT_shift, XRT_sigma, covvalue = calibrate_RT_gaus(start_width, RT_left, RT_right, rt_diff_tmp)
                 if np.isinf(covvalue):
                     XRT_shift, XRT_sigma, covvalue = calibrate_RT_gaus(0.1, RT_left, RT_right, rt_diff_tmp)
                 if np.isinf(covvalue):
                     XRT_shift, XRT_sigma, covvalue = calibrate_RT_gaus(1.0, RT_left, RT_right, rt_diff_tmp)
-                # print('Calibrated RT shift: ', XRT_shift)
-                # print('Calibrated RT sigma: ', XRT_sigma)
-
-                # aa, bb, RR, ss = aux.linear_regression(RT_pred, train_RT)
             else:
                 RC = achrom.get_RCs_vary_lcp(ns, nr)
                 RT_pred = np.array([achrom.calculate_RT(s, RC) for s in ns])
                 # aa, bb, RR, ss = aux.linear_regression(RT_pred, nr)
 
                 rt_diff_tmp = RT_pred - nr
                 RT_left = -min(rt_diff_tmp)
@@ -1184,26 +1114,19 @@
 
                 start_width = (scoreatpercentile(rt_diff_tmp, 95) - scoreatpercentile(rt_diff_tmp, 5)) / 50
                 XRT_shift, XRT_sigma, covvalue = calibrate_RT_gaus(start_width, RT_left, RT_right, rt_diff_tmp)
                 if np.isinf(covvalue):
                     XRT_shift, XRT_sigma, covvalue = calibrate_RT_gaus(0.1, RT_left, RT_right, rt_diff_tmp)
                 if np.isinf(covvalue):
                     XRT_shift, XRT_sigma, covvalue = calibrate_RT_gaus(1.0, RT_left, RT_right, rt_diff_tmp)
-                # print('Calibrated RT shift: ', XRT_shift)
-                # print('Calibrated RT sigma: ', XRT_sigma)
-
-        # print(aa, bb, RR, ss)
-
-
 
-        best_sigma = XRT_sigma
         RT_sigma = XRT_sigma
 
-    print('Second-stage calibrated RT shift: %.3f min' % (XRT_shift, ))
-    print('Second-stage calibrated RT sigma: %.3f min' % (XRT_sigma, ))
+    logger.info('Second-stage calibrated RT shift: %.3f min', XRT_shift)
+    logger.info('Second-stage calibrated RT sigma: %.3f min', XRT_sigma)
 
     out_log.write('Calibrated RT shift: %s min\n' % (XRT_shift, ))
     out_log.write('Calibrated RT sigma: %s min\n' % (XRT_sigma, ))
     out_log.close()
 
     p1 = set(resdict['seqs'])
 
@@ -1231,18 +1154,15 @@
 
         outtest.write('seq,modifications\n')
         for seq in p1:
             mods_tmp = '|'.join([str(idx+1)+'|Carbamidomethyl' for idx, aa in enumerate(seq) if aa == 'C'])
             outtest.write(seq + ',' + str(mods_tmp) + '\n')
         outtest.close()
 
-        if args['deeplc_library']:
-            subprocess.call([deeplc_path, '--file_pred', outtest_name, '--file_cal', outtrain_name, '--file_pred_out', outres_name, '--use_library', args['deeplc_library'], '--write_library'], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
-        else:
-            subprocess.call([deeplc_path, '--file_pred', outtest_name, '--file_cal', outtrain_name, '--file_pred_out', outres_name], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+        subprocess.call([deeplc_path, '--file_pred', outtest_name, '--file_cal', outtrain_name, '--file_pred_out', outres_name] + deeplc_extra_args, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
         for x in open(outres_name).readlines()[1:]:
             _, seq, _, RT = x.strip().split(',')
             pepdict[seq] = float(RT)
 
     else:
 
         if n == 1 or os.name == 'nt':
@@ -1285,30 +1205,30 @@
     rt_pred = rt_pred[e_ind]
 
 
     with open(base_out_name + '_protsN.tsv', 'w') as output:
         output.write('dbname\ttheor peptides\n')
         for k, v in protsN.items():
             output.write('\t'.join((k, str(v))) + '\n')
-   
+
     with open(base_out_name + '_PFMs.tsv', 'w') as output:
         output.write('sequence\tmass diff\tRT diff\tpeak_id\tIntensity\tnScans\tnIsotopes\tproteins\tm/z\tRT\taveragineCorr\tcharge\tion_mobility\n')
         # for seq, md, rtd, peak_id, I, nScans, nIsotopes, mzr, rtr, av, ch, im in zip(resdict['seqs'], resdict['md'], rt_diff, resdict['ids'], resdict['Is'], resdict['Scans'], resdict['Isotopes'], resdict['mzraw'], resdict['rt'], resdict['av'], resdict['ch'], resdict['im']):
         for seq, md, rtd, iorig in zip(resdict['seqs'], resdict['md'], rt_diff, resdict['iorig']):
             peak_id = ids[iorig]
             I = Is[iorig]
             nScans = Scans[iorig]
             nIsotopes = Isotopes[iorig]
             mzr = mzraw[iorig]
             rtr = rts[iorig]
             av = avraw[iorig]
             ch = charges[iorig]
             im = imraw[iorig]
             output.write('\t'.join((seq, str(md), str(rtd), str(peak_id), str(I), str(nScans), str(nIsotopes), ';'.join(pept_prot[seq]), str(mzr), str(rtr), str(av), str(ch), str(im))) + '\n')
-            
+
     # e_ind = resdict['mc'] == 0
     # resdict = filter_results(resdict, e_ind)
     # rt_diff = rt_diff[e_ind]
     # rt_pred = rt_pred[e_ind]
 
     mass_diff = (resdict['md'] - mass_shift) / (mass_sigma)
 
@@ -1378,23 +1298,21 @@
                 columns_to_remove.append(feature)
         feature_columns = feature_columns.drop(columns_to_remove)
         return feature_columns
 
     def objective_pfms(df, hyperparameters, iteration, threshold=0):
         """Objective function for grid and random search. Returns
         the cross validation score from a set of hyperparameters."""
-        
+
         all_res = []
-        all_iters = []
 
         groups = df['peptide']
         ix = df.index.values
         unique = np.unique(groups)
         np.random.RandomState(SEED).shuffle(unique)
-        result = []
         for split in np.array_split(unique, 3):
             mask = groups.isin(split)
             train, test = ix[~mask], ix[mask]
             train_df = df.iloc[train]
             test_df = df.iloc[test]
 
             feature_columns = get_features_pfms(df)
@@ -1412,62 +1330,57 @@
             ### 1
             fpr, tpr, thresholds = metrics.roc_curve(get_Y_array_pfms(test_df[~test_df['decoy2']]), test_df[~test_df['decoy2']]['preds'])
             # fpr, tpr, thresholds = metrics.roc_curve(get_Y_array_pfms(test_df), test_df['preds'])
             shr_v = metrics.auc(fpr, tpr)
             # shr_v = len(aux.filter(test_df, fdr=0.25, key='preds', is_decoy='decoy'))
 
             all_res.append(shr_v)
-            # print(shr_v)
 
             if shr_v < threshold:
                 all_res = [0, ]
                 break
 
         shr_v = np.mean(all_res)
         # hyperparameters['n_estimators'] = int(np.max(all_iters))# * 1.5)
-        # print(shr_v)
-        # print('\n')
 
         return np.array([shr_v, hyperparameters, iteration, all_res], dtype=object)
 
     def random_search_pfms(df, param_grid, out_file, max_evals):
-        """Random search for hyperparameter optimization. 
+        """Random search for hyperparameter optimization.
         Writes result of search to csv file every search iteration."""
-        
+
         threshold = 0
-        
+
         # Dataframe for results
         results = pd.DataFrame(columns = ['sharpe', 'params', 'iteration', 'all_res'],
                                     index = list(range(max_evals)))
         for i in range(max_evals):
 
-            # print('%d/%d' % (i+1, max_evals))
-            
             # Choose random hyperparameters
             random_params = {k: random.sample(v, 1)[0] for k, v in param_grid.items()}
 
             # Evaluate randomly selected hyperparameters
             eval_results = objective_pfms(df, random_params, i, threshold)
             results.loc[i, :] = eval_results
 
             threshold = max(threshold, np.mean(eval_results[3]) - 3 * np.std(eval_results[3]))
 
             # open connection (append option) and write results
             of_connection = open(out_file, 'a')
             writer = csv.writer(of_connection)
             writer.writerow(eval_results)
-            
+
             # make sure to close connection
             of_connection.close()
-            
+
         # Sort with best score on top
         results.sort_values('sharpe', ascending = False, inplace = True)
         results.reset_index(inplace = True)
 
-        return results 
+        return results
 
     def get_cat_model_pfms(df, hyperparameters, feature_columns, train, test):
         feature_columns = list(feature_columns)
         dtrain = lgb.Dataset(get_X_array(train, feature_columns), get_Y_array_pfms(train), feature_name=feature_columns, free_raw_data=False)
         dvalid = lgb.Dataset(get_X_array(test, feature_columns), get_Y_array_pfms(test), feature_name=feature_columns, free_raw_data=False)
         np.random.seed(SEED)
         evals_result = {}
@@ -1495,15 +1408,15 @@
     df1['rt'] = df1['iorig'].apply(lambda x: rts[x])
     df1['av'] = df1['iorig'].apply(lambda x: avraw[x])
     df1['ch'] = df1['iorig'].apply(lambda x: charges[x])
     df1['im'] = df1['iorig'].apply(lambda x: imraw[x])
 
     df1['mass_diff'] = mass_diff
     df1['rt_diff'] = rt_diff
-    df1['decoy'] = df1['seqs'].apply(lambda x: all(z.startswith(prefix) for z in pept_prot[x]))    
+    df1['decoy'] = df1['seqs'].apply(lambda x: all(z.startswith(prefix) for z in pept_prot[x]))
 
     df1['peptide'] = df1['seqs']
     mass_dict = {}
     pI_dict = {}
     charge_dict = {}
     for pep in set(df1['peptide']):
         try:
@@ -1542,14 +1455,119 @@
     #         'mz_diff_ppm_2',
     #         'I-0-1',
     #         'I-0-2',
     #     ]:
     #         tmp_dict = df_features.set_index('id').to_dict()[k]
     #         df1[k] = df1['ids'].apply(lambda x: tmp_dict[x])
 
+    # import pickle
+    # df11 = df1.copy()
+    # model2 = pickle.load(open('/home/mark/model2.pickle', 'rb'))
+    # feature_columns2 = pickle.load(open('/home/mark/model2_feature_columns.pickle', 'rb'))
+    # df11['RT'] = df11['rt']
+    # df11['charge'] = df11['ch']
+    # df11['ch'] = df11['charge_theor']
+    # df11['length'] = df11['plen']
+    # df11['m/z'] = df11['mzraw']
+    # df11['RT diff'] = df11['rt_diff']
+    # df11['mass diff'] = df11['mass_diff']
+
+    # from pyteomics import fasta
+    # def custom_cleave(sequence, rule, missed_cleavages=0, min_length=None):
+    #     peptides = []
+    #     ml = missed_cleavages+2
+    #     trange = list(range(ml))
+    #     cleavage_sites = deque([0], maxlen=ml)
+    #     cl = 1
+    #     for i in it.chain([x.end() for x in re.finditer(rule, sequence)],
+    #                 [None]):
+    #         cleavage_sites.append(i)
+    #         if cl < ml:
+    #             cl += 1
+    #         for j in trange[:cl-1]:
+    #             seq = sequence[cleavage_sites[j]:cleavage_sites[-1]]
+    #             if seq:
+    #                 if min_length is None or len(seq) >= min_length:
+    #                     peptides.append((seq, cleavage_sites[j]))
+    #     return peptides
+
+    # best_protein_tmp_dict = {}
+
+    # all_aa_set = set()
+    # prot_pep_cleave_map = defaultdict(dict)
+    # for p in fasta.read(args['d']):
+    #     dbname = p[0].split(' ')[0]
+    #     all_aa_set.update(p[1])
+    #     startposition = 0
+    #     peps_info = custom_cleave(p[1], parser.expasy_rules['trypsin'], 2)
+    #     prot_len = len(p[1])
+    #     for pep, pos in peps_info:
+            
+    #         pep_len = len(pep)
+            
+    #         prev_aa = p[1][max(0, pos-3):pos]
+    #         prev_aa = '-'*(3-len(prev_aa)) + prev_aa
+            
+    #         next_aa = p[1][pos+pep_len:min(pos+pep_len+3, prot_len-1)]
+    #         next_aa = next_aa + '-'*(3-len(next_aa))
+            
+    #         prot_pep_cleave_map[dbname][pep] = [prev_aa, next_aa]
+
+    #         best_protein_tmp_dict[pep] = dbname
+
+    # dbname_default = dbname
+            
+    # aa_map = {'-': 0}
+    # for idx, aa in enumerate(all_aa_set):
+    #     aa_map[aa] = idx+1
+        
+    # for k1 in list(prot_pep_cleave_map.keys()):
+    #     for k2 in list(prot_pep_cleave_map[k1].keys()):
+    #         val = prot_pep_cleave_map[k1][k2]
+    #         prot_pep_cleave_map[k1][k2] = [[aa_map[aa] for aa in val[0]], [aa_map[aa] for aa in val[1]]]
+
+    # df11['bestprotein'] = df11['peptide'].apply(lambda x: best_protein_tmp_dict.get(x, dbname_default))
+
+
+    # df11['prev1'] = df11[['peptide', 'bestprotein']].apply(lambda x: prot_pep_cleave_map[x[1]].get(x[0], [[0, 0, 0], [0, 0, 0]])[0][-1], axis=1)
+    # df11['prev2'] = df11[['peptide', 'bestprotein']].apply(lambda x: prot_pep_cleave_map[x[1]].get(x[0], [[0, 0, 0], [0, 0, 0]])[0][-2], axis=1)
+    # df11['prev3'] = df11[['peptide', 'bestprotein']].apply(lambda x: prot_pep_cleave_map[x[1]].get(x[0], [[0, 0, 0], [0, 0, 0]])[0][-3], axis=1)
+    # df11['next1'] = df11[['peptide', 'bestprotein']].apply(lambda x: prot_pep_cleave_map[x[1]].get(x[0], [[0, 0, 0], [0, 0, 0]])[1][0], axis=1)
+    # df11['next2'] = df11[['peptide', 'bestprotein']].apply(lambda x: prot_pep_cleave_map[x[1]].get(x[0], [[0, 0, 0], [0, 0, 0]])[1][1], axis=1)
+    # df11['next3'] = df11[['peptide', 'bestprotein']].apply(lambda x: prot_pep_cleave_map[x[1]].get(x[0], [[0, 0, 0], [0, 0, 0]])[1][2], axis=1)
+    
+
+    # for cc in ['m/z', 'length', 'RT', 'mass diff', 'RT diff']:
+    #     df11['%s_rank' % (cc, )] = df11.groupby('bestprotein')[cc].rank(pct=True)
+
+    # df11['IntensityNorm_predicted'] = model2.predict(get_X_array(df11, feature_columns2))
+
+    # df11['IntensityNorm'] = df11['Is'].rank(pct=True)
+    # df11['IntensityNorm_predicted'] = df11['IntensityNorm_predicted'].rank(pct=True)
+
+    # # df11['IntensityNorm'] = df11.groupby('bestprotein')['Is'].rank(pct=True)
+    # # df11['IntensityNorm_predicted'] = df11.groupby('bestprotein')['IntensityNorm_predicted'].rank(pct=True)
+
+    # df1['IntensityNorm_predicted'] = df11['IntensityNorm_predicted']
+    # df1['IntensityNorm'] = df11['IntensityNorm']
+    # df1['Idiff'] = df1['IntensityNorm'] - df1['IntensityNorm_predicted']
+
+    # df1['prev1'] = df11['prev1']
+    # df1['prev2'] = df11['prev2']
+    # df1['prev3'] = df11['prev3']
+    # df1['next1'] = df11['next1']
+    # df1['next2'] = df11['next2']
+    # df1['next3'] = df11['next3']
+
+
+
+
+
+
+
 
     p1 = set(resdict['seqs'])
 
     prots_spc2 = defaultdict(set)
     for pep, proteins in pept_prot.items():
         if pep in p1:
             for protein in proteins:
@@ -1563,33 +1581,29 @@
     names_arr = np.array(list(prots_spc.keys()))
     v_arr = np.array(list(prots_spc.values()))
     n_arr = np.array([protsN[k] for k in prots_spc])
 
     top100decoy_score = [prots_spc.get(dprot, 0) for dprot in protsN if isdecoy_key(dprot)]
     top100decoy_N = [val for key, val in protsN.items() if isdecoy_key(key)]
     p = np.mean(top100decoy_score) / np.mean(top100decoy_N)
-    print('Stage 2 search: probability of random match for theoretical peptide = %.3f\n' % (p, ))
+    logger.info('Stage 2 search: probability of random match for theoretical peptide = %.3f', p)
 
     prots_spc = dict()
-    all_pvals = calc_sf_all(v_arr, n_arr, p)
+    all_pvals = utils.calc_sf_all(v_arr, n_arr, p)
     for idx, k in enumerate(names_arr):
         prots_spc[k] = all_pvals[idx]
 
-    sortedlist_spc = sorted(prots_spc.items(), key=operator.itemgetter(1))[::-1]
-    target_prots = [x[0] for x in sortedlist_spc if not x[0].startswith('DECOY_')]
     target_prots_25_fdr = set([x[0] for x in aux.filter(prots_spc.items(), fdr=0.25, key=escore, is_decoy=isdecoy, remove_decoy=False, formula=1, full_output=True, correction=0)])
     df1['proteins'] = df1['seqs'].apply(lambda x: ';'.join(pept_prot[x]))
-    df1['decoy2'] = df1['decoy'] 
+    df1['decoy2'] = df1['decoy']
     df1['decoy'] = df1['proteins'].apply(lambda x: all(z not in target_prots_25_fdr for z in x.split(';')))
 
     if args['ml']:
 
-        print('Start Machine Learning on PFMs...')
-
-        # print('Features used for MachineLearning: ', get_features_pfms(df1))
+        logger.info('Start Machine Learning on PFMs...')
 
         MAX_EVALS = 25
 
         out_file = os.path.join(tempfile.gettempdir(), os.urandom(24).hex())
         of_connection = open(out_file, 'w')
         writer = csv.writer(of_connection)
 
@@ -1599,21 +1613,20 @@
         of_connection.close()
 
         random_results = random_search_pfms(df1, param_grid, out_file, MAX_EVALS)
 
         random_results = pd.read_csv(out_file)
         random_results = random_results[random_results['auc'] != 'auc']
         random_results['params'] = random_results['params'].apply(lambda x: ast.literal_eval(x))
-        convert_dict = {'auc': float, 
-                    } 
-        random_results = random_results.astype(convert_dict) 
+        convert_dict = {'auc': float,
+                    }
+        random_results = random_results.astype(convert_dict)
 
         bestparams = random_results.sort_values(by='auc',ascending=False)['params'].values[0]
         bestparams['num_threads'] = args['nproc']
-        # print(random_results.sort_values(by='auc',ascending=False)['auc'].values[0])
 
         groups = df1['peptide']
         ix = df1.index.values
         unique = np.unique(groups)
         np.random.RandomState(SEED).shuffle(unique)
         result = []
         for split in np.array_split(unique, 3):
@@ -1639,21 +1652,19 @@
     df1u = df1.sort_values(by='preds')
     df1u = df1u.drop_duplicates(subset='seqs')
 
     qval_ok = 0
     for qval_cur in range(50):
         df1ut = df1u[df1u['qpreds'] == qval_cur]
         decoy_ratio = df1ut['decoy'].sum() / len(df1ut)
-        # print(qval_cur, decoy_ratio)
         if decoy_ratio < 0.5:
             qval_ok = qval_cur
         else:
             break
-    print('%d %% of PFMs were removed from protein scoring after Machine Learning' % (100 - (qval_ok+1)*2))
-    # print('qval_ok', qval_ok)
+    logger.info('%d %% of PFMs were removed from protein scoring after Machine Learning', (100 - (qval_ok+1)*2))
 
     df1un = df1u[df1u['qpreds'] <= qval_ok].copy()
     df1un['qpreds'] = pd.qcut(df1un['preds'], 10, labels=range(10))
 
     qdict = df1un.set_index('seqs').to_dict()['qpreds']
 
     df1['qpreds'] = df1['seqs'].apply(lambda x: qdict.get(x, 11))
@@ -1691,19 +1702,19 @@
     names_arr = np.array(list(prots_spc.keys()))
     v_arr = np.array(list(prots_spc.values()))
     n_arr = np.array([protsN[k] for k in prots_spc])
 
     top100decoy_score = [prots_spc.get(dprot, 0) for dprot in protsN if isdecoy_key(dprot)]
     top100decoy_N = [val for key, val in protsN.items() if isdecoy_key(key)]
     p = np.mean(top100decoy_score) / np.mean(top100decoy_N)
-    print('Final stage search: probability of random match for theoretical peptide = %.3f\n' % (p, ))
+    logger.info('Final stage search: probability of random match for theoretical peptide = %.3f', p)
 
 
     prots_spc = dict()
-    all_pvals = calc_sf_all(v_arr, n_arr, p)
+    all_pvals = utils.calc_sf_all(v_arr, n_arr, p)
     for idx, k in enumerate(names_arr):
         prots_spc[k] = all_pvals[idx]
 
     final_iteration(resdict, mass_diff, rt_diff, pept_prot, protsN, base_out_name, prefix, isdecoy, isdecoy_key, escore, fdr, args['nproc'], fname)
 
 
 def worker(qin, qout, mass_diff, rt_diff, resdict, protsN, pept_prot, isdecoy_key, isdecoy, fdr, prots_spc_basic2, win_sys=False):
@@ -1760,15 +1771,15 @@
                         n_map_dict[v].append(k)
 
                     decoy_set = set()
                     for k in protsN:
                         if isdecoy_key(k):
                             decoy_set.add(k)
                     decoy_set = list(decoy_set)
-                    
+
 
                     prots_spc2 = defaultdict(set)
                     for pep, proteins in pept_prot.items():
                         if pep in p1:
                             for protein in proteins:
                                 if protein == features_dict[pep][0]:
                                     prots_spc2[protein].add(pep)
@@ -1786,15 +1797,14 @@
 
                     tmp_spc_new = dict((k, len(v)) for k, v in prots_spc2.items())
 
 
                     top100decoy_score_tmp = [tmp_spc_new.get(dprot, 0) for dprot in decoy_set]
                     top100decoy_score_tmp_sum = float(sum(top100decoy_score_tmp))
 
-                tmp_spc = tmp_spc_new
                 prots_spc = tmp_spc_new
                 if not prots_spc_copy:
                     prots_spc_copy = deepcopy(prots_spc)
 
                 for idx, v in enumerate(decoy_set):
                     if v in unstable_prots:
                         top100decoy_score_tmp_sum -= top100decoy_score_tmp[idx]
@@ -1816,26 +1826,23 @@
                 v_arr_small = []
                 for k, v in best_match_dict.items():
                     n_arr_small.append(k)
                     names_arr_small.append(v)
                     v_arr_small.append(prots_spc[v])
 
                 prots_spc_basic = dict()
-                all_pvals = calc_sf_all(np.array(v_arr_small), n_arr_small, p)
+                all_pvals = utils.calc_sf_all(np.array(v_arr_small), n_arr_small, p)
                 for idx, k in enumerate(names_arr_small):
                     prots_spc_basic[k] = all_pvals[idx]
 
                 best_prot = utils.keywithmaxval(prots_spc_basic)
 
                 best_score = min(prots_spc_basic[best_prot], prev_best_score)
                 prev_best_score = best_score
 
-                # if mass_koef == 0:
-                #     print('best_score', best_score)
-
                 unstable_prots = set()
                 if best_prot not in prots_spc_final:
                     prots_spc_final[best_prot] = best_score
                     banned_pids = set()
                     for pep in prots_spc2[best_prot]:
                         for pid in pep_pid[pep]:
                             banned_pids.add(pid)
@@ -1844,20 +1851,20 @@
                             banned_dict[pep] -= 1
                             if banned_dict[pep] == 0:
                                 best_prot_val = features_dict[pep][0]
                                 for bprot in pept_prot[pep]:
                                     if bprot == best_prot_val:
                                         tmp_spc_new[bprot] -= 1
                                         unstable_prots.add(bprot)
-                        
+
                         banned_pids_total.add(pid)
                 else:
 
                     v_arr = np.array([prots_spc[k] for k in names_arr])
-                    all_pvals = calc_sf_all(v_arr, n_arr, p)
+                    all_pvals = utils.calc_sf_all(v_arr, n_arr, p)
                     for idx, k in enumerate(names_arr):
                         prots_spc_basic[k] = all_pvals[idx]
 
                     for k, v in prots_spc_basic.items():
                         if k not in prots_spc_final:
                             prots_spc_final[k] = v
 
@@ -1866,15 +1873,15 @@
                 try:
                     prot_fdr = aux.fdr(prots_spc_final.items(), is_decoy=isdecoy)
                 except ZeroDivisionError:
                     prot_fdr = 100.0
                 if prot_fdr >= 12.5 * fdr:
 
                     v_arr = np.array([prots_spc[k] for k in names_arr])
-                    all_pvals = calc_sf_all(v_arr, n_arr, p)
+                    all_pvals = utils.calc_sf_all(v_arr, n_arr, p)
                     for idx, k in enumerate(names_arr):
                         prots_spc_basic[k] = all_pvals[idx]
 
                     for k, v in prots_spc_basic.items():
                         if k not in prots_spc_final:
                             prots_spc_final[k] = v
                     break
```

## ms1searchpy/ms1todiffacto.py

```diff
@@ -1,14 +1,12 @@
 from __future__ import division
 import argparse
-import pkg_resources
 import pandas as pd
-import ast
 import subprocess
-import numpy as np
+import logging
 
 def run():
     parser = argparse.ArgumentParser(
         description='run diffacto for ms1searchpy results',
         epilog='''
 
     Example usage
@@ -34,15 +32,19 @@
     parser.add_argument('-peptides', help='name of output peptides file', default='peptides.txt')
     parser.add_argument('-samples', help='name of output samples file', default='sample.txt')
     parser.add_argument('-allowed_prots', help='path to allowed prots', default='')
     parser.add_argument('-out', help='name of diffacto output file', default='diffacto_out.txt')
     parser.add_argument('-norm', help='normalization method. Can be average, median, GMM or None', default='None')
     parser.add_argument('-impute_threshold', help='impute_threshold for missing values fraction', default='0.75')
     parser.add_argument('-min_samples', help='minimum number of samples for peptide usage', default='3')
+    parser.add_argument('-debug', help='Produce debugging output', action='store_true')
     args = vars(parser.parse_args())
+    logging.basicConfig(format='%(levelname)9s: %(asctime)s %(message)s',
+            datefmt='[%H:%M:%S]', level=[logging.INFO, logging.DEBUG][args['debug']])
+    logger = logging.getLogger(__name__)
 
     replace_label = '_proteins.tsv'
 
     df_final = False
 
     allowed_prots = set()
     allowed_peptides = set()
@@ -90,20 +92,19 @@
 
     for i in range(1, 13, 1):
         sample_num = 'S%d' % (i, )
         if args[sample_num]:
             for z in args[sample_num]:
                 label = z.replace(replace_label, '')
                 all_labels.append(label)
-                df1 = pd.read_table(z)
                 df3 = pd.read_table(z.replace(replace_label, '_PFMs.tsv'))
-                print(z)
-                print(z.replace(replace_label, '_PFMs.tsv'))
-                print(df3.shape)
-                print(df3.columns)
+                logger.debug(z)
+                logger.debug(z.replace(replace_label, '_PFMs.tsv'))
+                logger.debug(df3.shape)
+                logger.debug(df3.columns)
 
                 df3 = df3[df3['proteins'].apply(lambda x: any(z in allowed_prots_all for z in x.split(';')))]
                 df3['proteins'] = df3['proteins'].apply(lambda x: ';'.join([z for z in x.split(';') if z in allowed_prots_all]))
 
                 df3['origseq'] = df3['sequence']
                 df3['sequence'] = df3['sequence'] + df3['charge'].astype(int).astype(str) + df3['ion_mobility'].astype(str)
 
@@ -115,34 +116,33 @@
                 df3['protein'] = df3['proteins']
                 df3['peptide'] = df3['sequence']
                 df3 = df3[['origseq', 'peptide', 'protein', label]]
 
 
 
                 if df_final is False:
-                    label_basic = label
                     df_final = df3.reset_index(drop=True)
                 else:
                     df_final = df_final.reset_index(drop=True).merge(df3.reset_index(drop=True), on='peptide', how='outer')
                     df_final.protein_x.fillna(value=df_final.protein_y, inplace=True)
                     df_final.origseq_x.fillna(value=df_final.origseq_y, inplace=True)
                     df_final['protein'] = df_final['protein_x']
                     df_final['origseq'] = df_final['origseq_x']
 
                     df_final = df_final.drop(columns=['protein_x', 'protein_y'])
                     df_final = df_final.drop(columns=['origseq_x', 'origseq_y'])
 
 
     df_final['intensity_median'] = df_final[all_labels].median(axis=1)
     df_final['nummissing'] = df_final[all_labels].isna().sum(axis=1)
-    print(df_final['nummissing'])
+    logger.debug(df_final['nummissing'])
     df_final = df_final.sort_values(by=['nummissing', 'intensity_median'], ascending=(True, False))
     df_final = df_final.drop_duplicates(subset=('origseq', 'protein'))
 
-    print(df_final.columns)
+    logger.debug(df_final.columns)
     df_final = df_final.set_index('peptide')
     df_final['proteins'] = df_final['protein']
     df_final = df_final.drop(columns=['protein'])
     cols = df_final.columns.tolist()
     cols.remove('proteins')
     cols.insert(0, 'proteins')
     df_final = df_final[cols]
```

## ms1searchpy/search.py

```diff
@@ -1,25 +1,25 @@
-from sys import argv
-from . import main, utils
+from . import main
 import argparse
+import logging
 
 def run():
     parser = argparse.ArgumentParser(
         description='Search proteins using LC-MS spectra',
         epilog='''
 
     Example usage
     -------------
     $ search.py input.mzML input2.mzML -d human.fasta -ad 1 -fdr 5.0
     -------------
     ''',
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
 
     parser.add_argument('files', help='input mzML or .tsv files with peptide features', nargs='+')
-    parser.add_argument('-d', help='path to protein fasta file', required=True)
+    parser.add_argument('-d', '-db', help='path to protein fasta file', required=True)
     parser.add_argument('-ptol', help='precursor mass tolerance in ppm', default=10.0, type=float)
     parser.add_argument('-fdr', help='protein fdr filter in %%', default=1.0, type=float)
     parser.add_argument('-i', help='minimum number of isotopes', default=2, type=int)
     parser.add_argument('-ci', help='minimum number of isotopes for mass and RT calibration', default=4, type=int)
     parser.add_argument('-ts', help='Two-stage RT training: 0 - turn off, 1 - turn one, 2 - turn on and use additive model in the first stage (Default)', default=2, type=int)
     parser.add_argument('-sc', help='minimum number of scans for peptide feature', default=2, type=int)
     parser.add_argument('-lmin', help='min length of peptides', default=7, type=int)
@@ -32,16 +32,24 @@
     parser.add_argument('-fmods', help='fixed modifications. in mass1@aminoacid1,mass2@aminoacid2 format', default='57.021464@C')
     parser.add_argument('-ad', help='add decoy', default=0, type=int)
     parser.add_argument('-ml', help='use machine learning for PFMs', default=1, type=int)
     parser.add_argument('-prefix', help='decoy prefix', default='DECOY_')
     parser.add_argument('-nproc',   help='number of processes', default=1, type=int)
     parser.add_argument('-elude', help='path to elude binary file. If empty, the built-in additive model will be used for RT prediction', default='')
     parser.add_argument('-deeplc', help='path to deeplc', default='')
+    parser.add_argument('-deeplc_model_path', help='path to deeplc model or folder with deeplc models', default='')
     parser.add_argument('-deeplc_library', help='path to deeplc library', default='')
     parser.add_argument('-pl', help='path to list of peptides for RT calibration', default='')
-    parser.add_argument('-mcalib',   help='mass calibration: 2 - group by ion mobility and RT, 1 - by RT, 0 - no calibration', default=2, type=int)
+    parser.add_argument('-mcalib', help='mass calibration: 2 - group by ion mobility and RT, 1 - by RT, 0 - no calibration', default=2, type=int)
+    parser.add_argument('-debug', help='Produce debugging output', action='store_true')
     args = vars(parser.parse_args())
-
+    logging.basicConfig(format='%(levelname)9s: %(asctime)s %(message)s',
+            datefmt='[%H:%M:%S]', level=[logging.INFO, logging.DEBUG][args['debug']])
+    logging.getLogger('matplotlib.font_manager').disabled = True
+    logging.getLogger('matplotlib.category').disabled = True
+    logging.getLogger('matplotlib').setLevel(logging.WARNING)
+    logger = logging.getLogger(__name__)
+    logger.debug('Starting with args: %s', args)
     main.process_file(args)
 
 if __name__ == '__main__':
     run()
```

## ms1searchpy/utils.py

```diff
@@ -1,45 +1,67 @@
 from pyteomics import fasta, parser
-from multiprocessing import Queue, Process, cpu_count
 import os
-import csv
-import subprocess
 from scipy.stats import binom
 import numpy as np
 import pandas as pd
 import random
 import itertools
-from collections import Counter
+from biosaur2 import main as bio_main
+import logging
+
+logger = logging.getLogger(__name__)
+
 
 def recalc_spc(banned_dict, unstable_prots, prots_spc2):
     tmp = dict()
     for k in unstable_prots:
         tmp[k] = sum(banned_dict.get(l, 1) > 0 for l in prots_spc2[k])
     return tmp
 
 def iterate_spectra(fname, min_ch, max_ch, min_isotopes, min_scans):
     if os.path.splitext(fname)[-1].lower() == '.mzml':
-        subprocess.call(['biosaur2', fname])
+        args = {
+            'file': fname,
+            'mini': 1,
+            'minmz': 350,
+            'maxmz': 1500,
+            'pasefmini': 100,
+            'htol': 8,
+            'itol': 8,
+            'paseftol': 0.05,
+            'nm': 0,
+            'o': '',
+            'hvf': 1.3,
+            'minlh': 2,
+            'cmin': 1,
+            'cmax': 6,
+            'dia': False,
+            'diahtol': 25,
+            'diaminlh': 1,
+            'mgf': '',
+            'debug': False  # actual debug value is set through logging, not here
+        }
+        bio_main.process_file(args)
         fname = os.path.splitext(fname)[0] + '.features.tsv'
 
     df_features = pd.read_csv(fname, sep='\t')
 
     required_columns = [
         'nIsotopes',
         'nScans',
         'charge',
         'massCalib',
         'rtApex',
-        'mz', 
+        'mz',
         ]
 
     if not all(req_col in df_features.columns for req_col in required_columns):
-        print('input feature file have missing columns: %s' % (';'.join([req_col for req_col in required_columns if req_col not in df_features.columns])))
+        logger.error('input feature file have missing columns: %s', ';'.join([req_col for req_col in required_columns if req_col not in df_features.columns]))
         raise Exception('Exception: wrong columns in feature file')
-    print('Total number of peptide isotopic clusters: %d' % (len(df_features), ))
+    logger.info('Total number of peptide isotopic clusters: %d', len(df_features))
 
     if 'id' not in df_features.columns:
         df_features['id'] = df_features.index
     if 'FAIMS' not in df_features.columns:
         df_features['FAIMS'] = 0
     if 'ion_mobility' not in df_features.columns:
         df_features['ion_mobility'] = 0
@@ -87,31 +109,28 @@
     #         enzyme = convert_tandem_cleave_rule_to_regexp(enzyme)
     #         return enzyme
     #     except:
     #         return enzyme
 
 def prot_gen(args):
     db = args['d']
-    add_decoy = args['ad']
-    prefix = args['prefix']
 
     with fasta.read(db) as f:
         for p in f:
             yield p
 
 def prepare_decoy_db(args):
     add_decoy = args['ad']
     if add_decoy:
 
         prefix = args['prefix']
         db = args['d']
         out1, out2 = os.path.splitext(db)
         out_db = out1 + '_shuffled' + out2
-        print('Creating decoy database: %s' % (out_db, ))
-
+        logger.info('Creating decoy database: %s', out_db)
 
         extra_check = False
         if '{' in args['e']:
             extra_check = True
         if extra_check:
             banned_pairs = set()
             banned_aa = set()
@@ -119,30 +138,30 @@
                 if '{' in enzyme_local:
                     lpart, rpart = enzyme_local.split('|')
                     for aa_left, aa_right in itertools.product(lpart[1:-1], rpart[1:-1]):
                         banned_aa.add(aa_left)
                         banned_aa.add(aa_right)
                         banned_pairs.add(aa_left+aa_right)
 
-            print(banned_aa)
-            print(banned_pairs)
+            logger.debug(banned_aa)
+            logger.debug(banned_pairs)
 
         enzyme = get_enzyme(args['e'])
         cleave_rule_custom = enzyme + '|' + '([BXZUO])'
         # cleave_rule_custom = '([RKBXZUO])'
-        print(cleave_rule_custom)
+        logger.debug(cleave_rule_custom)
 
         shuf_map = dict()
 
         prots = []
 
         for p in fasta.read(db):
             if not p[0].startswith(prefix):
                 target_peptides = [x[1] for x in parser.icleave(p[1], cleave_rule_custom, 0)]
-                
+
                 checked_peptides = set()
                 sample_list = []
                 for idx, pep in enumerate(target_peptides):
 
                     if len(pep) > 2:
                         pep_tmp = pep[1:-1]
                         if extra_check:
@@ -151,21 +170,20 @@
                                     pep_tmp = pep_tmp.replace(bp, '')
                                     checked_peptides.add(idx)
 
 
                         sample_list.extend(pep_tmp)
                 random.shuffle(sample_list)
                 idx_for_shuffle = 0
-                
+
                 decoy_peptides = []
-                len_target_peptides = len(target_peptides)
                 for idx, pep in enumerate(target_peptides):
-                    
+
                     if len(pep) > 2:
-                    
+
                         if pep in shuf_map:
                             tmp_seq = shuf_map[pep]
                         else:
                             if not extra_check or idx not in checked_peptides:
                                 tmp_seq = pep[0]
                                 for pep_aa in pep[1:-1]:
                                     tmp_seq += sample_list[idx_for_shuffle]
@@ -182,26 +200,26 @@
                                         ii += 1
                                     else:
                                         if ii == 0:
                                             tmp_seq += pep[ii]
                                         else:
                                             tmp_seq += sample_list[idx_for_shuffle]
                                             idx_for_shuffle += 1
-                                    
+
                                     ii += 1
                                 tmp_seq += pep[max_l-1]
 
                             shuf_map[pep] = tmp_seq
                     else:
                         tmp_seq = pep
-                    
+
                     decoy_peptides.append(tmp_seq)
 
                 assert len(target_peptides) == len(decoy_peptides)
-                        
+
                 prots.append((p[0], ''.join(target_peptides)))
                 prots.append(('DECOY_' + p[0], ''.join(decoy_peptides)))
 
         fasta.write(prots, open(out_db, 'w')).close()
         args['d'] = out_db
         args['ad'] = 0
     return args
@@ -262,23 +280,24 @@
         if k.startswith(prefix):
             decoy_peps.update(v)
         else:
             target_peps.update(v)
 
         protsN[k] = len(v)
 
-    print('\nDatabase information:')
-    print('Target/Decoy proteins: %d/%d' % (target_prot_count, decoy_prot_count, ))
-    print('Target/Decoy peptides: %d/%d' % (len(target_peps), len(decoy_peps), ))
-    print('Target-Decoy peptide intersection: %.1f %%\n' % (100*len(target_peps.intersection(decoy_peps))/(len(target_peps)+len(decoy_peps)) ))
+    logger.info('Database information:')
+    logger.info('Target/Decoy proteins: %d/%d', target_prot_count, decoy_prot_count)
+    logger.info('Target/Decoy peptides: %d/%d', len(target_peps), len(decoy_peps))
+    logger.info('Target-Decoy peptide intersection: %.1f %%',
+        100 * len(target_peps.intersection(decoy_peps)) / (len(target_peps) + len(decoy_peps)))
     del decoy_peps
     del target_peps
-
     return protsN, pept_prot
 
+
 def convert_tandem_cleave_rule_to_regexp(cleavage_rule):
 
     def get_sense(c_term_rule, n_term_rule):
         if '{' in c_term_rule:
             return 'N'
         elif '{' in n_term_rule:
             return 'C'
@@ -321,16 +340,16 @@
     return '|'.join(out_rules)
 
 def multimap(n, func, it, **kw):
     for s in it:
         yield func(s, **kw)
 
 def keywithmaxval(d):
-     """ a) create a list of the dict's keys and values; 
-         b) return the key with the max value"""  
+     """ a) create a list of the dict's keys and values;
+         b) return the key with the max value"""
      v=list(d.values())
      k=list(d.keys())
      return k[v.index(max(v))]
 
 def calc_sf_all(v, n, p, prev_best_score=False):
     sf_values = -np.log10(binom.sf(v-1, n, p))
     sf_values[np.isnan(sf_values)] = 0
@@ -350,17 +369,17 @@
 #     #         if result:
 #     #             for x in result:
 #     #                 peptide, m, snp_label, res = x
 
 #     #                 for score, spec_t, c, info in res:
 #     #                     if -score <= best_res.get(spec_t, 0):
 #     #                         best_res_raw[spec_t] = [peptide, m, snp_label, score, spec_t, c, info]
-#     #                         best_res[spec_t] = -score   
+#     #                         best_res[spec_t] = -score
 #     #     return best_res_raw, best_res
-      
+
 #     else:
 
 #         qout = Queue()
 #         count = 0
 
 #         while True:
 #             qin = list(islice(it, 5000000))
@@ -382,8 +401,8 @@
 #                             best_res_raw[k] = v
 #                             best_res[k] = -v[3]
 #                     # yield item
 
 #             for p in procs:
 #                 p.join()
 
-#         return best_res_raw, best_res
+#         return best_res_raw, best_res
```

## Comparing `ms1searchpy-2.3.6.dist-info/LICENSE` & `ms1searchpy-2.3.7.dist-info/LICENSE`

 * *Files identical despite different names*

