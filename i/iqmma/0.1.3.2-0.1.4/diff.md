# Comparing `tmp/iqmma-0.1.3.2-py3-none-any.whl.zip` & `tmp/iqmma-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 29007 bytes, number of entries: 10
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-26 14:17 iqmma/__init__.py
--rw-r--r--  2.0 unx     1051 b- defN 23-Feb-26 14:17 iqmma/default.ini
--rw-r--r--  2.0 unx    38525 b- defN 23-May-01 09:17 iqmma/iqmma.py
--rw-r--r--  2.0 unx    42493 b- defN 23-Apr-25 13:34 iqmma/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-01 09:22 iqmma-0.1.3.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    12164 b- defN 23-May-01 09:22 iqmma-0.1.3.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-01 09:22 iqmma-0.1.3.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       42 b- defN 23-May-01 09:22 iqmma-0.1.3.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-May-01 09:22 iqmma-0.1.3.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      771 b- defN 23-May-01 09:22 iqmma-0.1.3.2.dist-info/RECORD
-10 files, 106501 bytes uncompressed, 27703 bytes compressed:  74.0%
+Zip file size: 29121 bytes, number of entries: 10
+-rw-r--r--  2.0 unx        0 b- defN 23-May-01 14:29 iqmma/__init__.py
+-rw-r--r--  2.0 unx     1051 b- defN 23-May-01 14:29 iqmma/default.ini
+-rw-r--r--  2.0 unx    39338 b- defN 23-May-31 13:45 iqmma/iqmma.py
+-rw-r--r--  2.0 unx    42523 b- defN 23-May-31 14:09 iqmma/utils.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-31 15:57 iqmma-0.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12199 b- defN 23-May-31 15:57 iqmma-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 15:57 iqmma-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       42 b- defN 23-May-31 15:57 iqmma-0.1.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-May-31 15:57 iqmma-0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      759 b- defN 23-May-31 15:57 iqmma-0.1.4.dist-info/RECORD
+10 files, 107367 bytes uncompressed, 27841 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: iqmma/iqmma.py
 Comment: 
 
 Filename: iqmma/utils.py
 Comment: 
 
-Filename: iqmma-0.1.3.2.dist-info/LICENSE
+Filename: iqmma-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: iqmma-0.1.3.2.dist-info/METADATA
+Filename: iqmma-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: iqmma-0.1.3.2.dist-info/WHEEL
+Filename: iqmma-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: iqmma-0.1.3.2.dist-info/entry_points.txt
+Filename: iqmma-0.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: iqmma-0.1.3.2.dist-info/top_level.txt
+Filename: iqmma-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: iqmma-0.1.3.2.dist-info/RECORD
+Filename: iqmma-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## iqmma/iqmma.py

```diff
@@ -84,15 +84,15 @@
     parser.add_argument('-overwrite_features', nargs='?', help='whether to overwrite existed features files (flag == 1) or use them (flag == 0)', type=int, default=0, const=0, choices=[0, 1])
     parser.add_argument('-overwrite_matching', nargs='?', help='whether to overwrite existed matched files (flag == 1) or use them (flag == 0)', type=int, default=0, const=0, choices=[0, 1])
     parser.add_argument('-overwrite_first_diffacto', nargs='?', help='whether to overwrite existed diffacto files (flag == 1) or use them (flag == 0)', type=int, default=1, const=1, choices=[0, 1])
     parser.add_argument('-mixed', nargs='?', help='whether to reanalyze mixed intensities (1) or not (0)', type=int, default=1, const=1, choices=[0, 1])
     parser.add_argument('-venn', nargs='?', help='whether to plot venn diagrams (1) or not (0)', type=int, default=1, const=1, choices=[0, 1])
     parser.add_argument('-pept_intens', nargs='?', help='max_intens - as intensity for peptide would be taken maximal intens between charge states; summ_intens - as intensity for peptide would be taken sum of intens between charge states; z-attached - each charge state would be treated as independent peptide', type=str, default='z-attached', const='z-attached', choices=['z-attached', 'summ_intens', 'max_intens'])
     parser.add_argument('-choice', nargs='?', help='method how to choose right intensities for peptide. 0 - default order and min Nan values, 1 - min Nan and min of sum CV, 2 - min Nan and min of max CV, 3 - min Nan and min of squared sum CV, 4 - min Nan and min of squared sum of corrected CV', type=int, default=4, const=4, choices=[0, 1, 2, 3, 4,])
-    parser.add_argument('-norm', nargs='?', help='normalization method for intensities. Can be 1 - median or 0 - no normalization', type=int, default=0, const=0, choices=[0, 1])
+    parser.add_argument('-norm', nargs='?', help='normalization method for intensities to remove biases between feature detections. Applied for each file independently. Can be 3 - max, 2 - min, 1 - median or 0 - no normalization. 2 and 3 options are strongly not recommended to use.', type=int, default=1, const=1, choices=[0, 1, 2, 3])
     parser.add_argument('-isotopes', help='monoisotope error', nargs='+', type=int, default=[0,1,-1,2,-2])
     parser.add_argument('-outpept', nargs='?', help='name of output diffacto peptides file (important: .txt)', type=str, default='peptides.txt', const='peptides.txt')
     parser.add_argument('-outsampl', nargs='?', help='name of output diffacto samples file (important: .txt)', type=str, default='sample.txt', const='sample.txt')
     parser.add_argument('-outdiff', nargs='?', help='name of diffacto output file (important: .txt)', type=str, default='diffacto_out.txt', const='diffacto_out.txt')
     parser.add_argument('-min_samples', nargs='?', help='minimum number of samples for peptide usage, -1 means that half of the given number of files would be used', type=int, default=-1, const=-1)
     
     parser.add_argument('-mbr', nargs='?', help='match between runs (1 - on, 0 - off)', type=int, default=0, const=0, choices=[0, 1])
@@ -470,15 +470,16 @@
 
 ### Сопоставление
 
     if args['matching_folder'] :
         if os.path.exists(args['matching_folder']) :
             matching_path = os.path.abspath(os.path.normpath(args['matching_folder']))
         else :
-            pass
+            matching_path = os.path.abspath(os.path.normpath(args['matching_folder']))
+            logger.warning('Path to matching folder does not exists, creating it: {}'.format(matching_path))
     else :
         matching_path = os.path.join(out_directory, 'feats_matched')
         logger.warning('Path to matching folder does not exists, using default one: {}'.format(matching_path))
     os.makedirs(matching_path, exist_ok=True)
 
     logger.info('Start matching features')
     for PSM_path, sample in zip(PSMs_full_paths, samples) :
@@ -494,14 +495,16 @@
                 # temp_df = optimized_search_with_isotope_error_(feats, PSM, mean_rt1=0,sigma_rt1=1e-6,mean_rt2=0,sigma_rt2=1e-6,mean_mz = False,sigma_mz = False,mean_im = False,sigma_im = False, isotopes_array=[0,1,-1,2,-2], logger=logger)[0]
 
                 if args['mbr']:    
                     temp_df = mbr(feats, temp_df, PSMs_full_paths, PSM_path, logger=logger)
 
                 median = temp_df['feature_intensityApex'].median()
                 temp_df['med_norm_feature_intensityApex'] = temp_df['feature_intensityApex']/median
+                temp_df['min_norm_feature_intensityApex'] = temp_df['feature_intensityApex']/temp_df['feature_intensityApex'].min()
+                temp_df['max_norm_feature_intensityApex'] = temp_df['feature_intensityApex']/temp_df['feature_intensityApex'].max()
                 cols = list(temp_df.columns)
                 
                 logger.info(suf + ' features ' + sample + ' DONE')
                 temp_df.to_csv(os.path.join(matching_path, sample + '_' + suf + '.tsv'), sep='\t', columns=cols)
                 logger.info(sample + ' PSMs matched ' + str(temp_df['feature_intensityApex'].notna().sum()) + '/' 
                              + str(len(temp_df)) + ' ' + str(round(temp_df['feature_intensityApex'].notna().sum()/len(temp_df)*100, 2)) + '%')
                 logger.info(suf + ' MATCHED')
@@ -533,17 +536,21 @@
             else :
                 logger.warning('Path to diffacto results does not exists, using default one: {}'.format( os.path.join(out_directory, 'diffacto')))
         else :
             diffacto_folder = os.path.join(out_directory, 'diffacto')
         os.makedirs(diffacto_folder, exist_ok=True)
 
         intens_colomn_name = 'feature_intensityApex'
-        if args['norm'] == 1 :
+        if args['norm'] == 3 :
+            intens_colomn_name = 'max_norm_feature_intensityApex'
+        elif args['norm'] == 2 :
+            intens_colomn_name = 'min_norm_feature_intensityApex'
+        elif args['norm'] == 1 :
             intens_colomn_name = 'med_norm_feature_intensityApex'
-        else :
+        elif args['norm'] == 0 :
             intens_colomn_name = 'feature_intensityApex'
         
         allowed_prots = set()
         if paths['proteins'] :    
             for key in paths['proteins'].keys() :
                 df0 = pd.read_table(paths['proteins'][key], usecols=['dbname'])
                 allowed_prots.update(df0['dbname'])
@@ -573,15 +580,15 @@
                     os.makedirs(charge_faims_intensity_path, exist_ok=True)
                     out_path = os.path.join(diffacto_folder, 'charge_faims_intensity', sample+'_'+suf+'.tsv')
                 else :
                     out_path = None
                     charge_faims_intensity_path = None
                 psms_dict[sample] = charge_states_intensity_processing(paths['feats_matched'][sample][suf],
                                                                         method=args['pept_intens'], 
-                                                                        intens_colomn_name='feature_intensityApex', 
+                                                                        intens_colomn_name=intens_colomn_name, 
                                                                         allowed_peptides=allowed_peptides, # set()
                                                                         allowed_prots=allowed_prots, # set()
                                                                         out_path=out_path,
                                                                         logger=logger
                 )
                 logger.debug('Done %s', sample)
```

## iqmma/utils.py

```diff
@@ -24,15 +24,15 @@
     
     start = int(f.find('['+category+']')) + 2 + len(category)
     end = min(f.find('\n\n', start), len(f))
     
     cfg_string = f[start:end]
     while '#' in cfg_string :
         l = cfg_string.find('#')
-        r = cfg_string.find('\n', l) + 2
+        r = cfg_string.find('\n', l) + 1
         cfg_string = cfg_string[:l] + cfg_string[r:]
 
     lst_of_strings = cfg_string.lstrip().split('\n')
     final = []
     keys = []
     for el in lst_of_strings :
         if el :
@@ -187,15 +187,15 @@
             shift, sigma = popt[1], abs(popt[2])
             right_fc_threshold = shift + 3*sigma
             left_fc_threshold = shift - 3*sigma
             logger.info('Dynamic fold change threshold is applied for {}: {} {}'.format(suf, left_fc_threshold, right_fc_threshold, ))
             table = table[table['P(PECA)'] < bonferroni][['Protein', 'P(PECA)', 'log2_FC']]
             table = table.query('`log2_FC` >= @right_fc_threshold or `log2_FC` <= @left_fc_threshold')
         comp_df = comp_df.merge(table, how='outer', on='Protein', suffixes = (None, '_'+suf))
-    comp_df.rename(columns={'log2_FC': 'log2_FC_'+suffixes[0], 'P(PECA)': 'P(PECA)'+suffixes[0] }, inplace=True )
+    comp_df.rename(columns={'log2_FC': 'log2_FC_'+suffixes[0], 'P(PECA)': 'P(PECA)_'+suffixes[0] }, inplace=True )
     comp_df.dropna(how = 'all', subset=['log2_FC_' + suf for suf in suffixes], inplace=True)
     # comp_df.loc['Total number', :] = df0.notna().sum(axis=0)
     
     total_de_prots = {}
     for suf in suffixes :
         total_de_prots[suf] = comp_df['log2_FC_'+suf].notna().sum()
     
@@ -288,14 +288,15 @@
     final_args = [diffacto_path, 
                   '-i', peptide_path, 
                   '-out', out_path, 
                   '-samples', sample_path, ] + ['-min_samples', min_samples] + other_args
     final_args = list(filter(lambda x: False if x=='' else True, final_args))
     final_args = [str(x) for x in final_args]
     logger.info('Diffacto START')
+    logger.debug(final_args)
     process = subprocess.Popen(final_args, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
     with process.stdout:
         log_subprocess_output(process.stdout, logger=logger)
     exitscore = process.wait()
     logger.debug(exitscore)
     
     if exitscore == 0 :
```

## Comparing `iqmma-0.1.3.2.dist-info/LICENSE` & `iqmma-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `iqmma-0.1.3.2.dist-info/METADATA` & `iqmma-0.1.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqmma
-Version: 0.1.3.2
+Version: 0.1.4
 Summary: A MS1 feature mapping for MS2 spectra identifications.
 Author: Valeriy Postoenko & Leyla Garibova
 Author-email: pyteomics@googlegroups.com
 License: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Education
@@ -28,15 +28,16 @@
 
 ## Installation
 
 Using pip:
 
     pip install iqmma
 
-It will install, if necessary, the minimum set (Biosaur2 and Diffacto) to `iqmma` to function. However, additional feature detections will need to be installed manually according to their manuals (see links below).
+It will install, if necessary, the minimum set (Biosaur2 and Diffacto) to `iqmma` to function. 
+Detailed instruction how to install additional feature detections and some general tooltips are in the [IQMMA_installation_guide.pdf](./IQMMA_installation_guide.pdf).
 
 ## Usage
 
 ### Some explanation and requirements
 
 `iqmma` has two working mods. First of all, it can be quantitation workflow with generating peptide features using multiple tools, matching them on peptides, and two Diffacto quantitation stages (separated and mixed, where the algorithm is choosing the best intensities for each peptide between different feature detections). The second one is stopping after peptide-feature matching to allow user to apply any other quantitation approach on matched intensities.
 
@@ -134,15 +135,15 @@
 
 - Diffacto repo: https://github.com/statisticalbiotechnology/diffacto
 
 - Dinosaur repo: https://github.com/fickludd/dinosaur
 
 - Biosaur2 repo: https://github.com/markmipt/biosaur2
 
-- OpenMS guide: https://abibuilder.cs.uni-tuebingen.de/archive/openms/Documentation/release/latest/html/index.html
+- OpenMS guide: https://openms.readthedocs.io/en/latest/openms-applications-and-tools/installation.html
 
 - Pypi: https://pypi.org/project/iqmma/
 
 - Github: https://github.com/PostoenkoVI/IQMMA
 
 - Mailing list: v.i.postoenko@gmail.com, garibova.02@gmail.com
```

