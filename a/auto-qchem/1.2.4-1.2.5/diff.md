# Comparing `tmp/auto_qchem-1.2.4-py3-none-any.whl.zip` & `tmp/auto_qchem-1.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 52173 bytes, number of entries: 20
--rw-r--r--  2.0 unx      211 b- defN 23-May-25 06:45 auto_qchem-1.2.4.data/data/config.yml
+Zip file size: 52357 bytes, number of entries: 20
+-rw-r--r--  2.0 unx      211 b- defN 23-May-25 06:45 auto_qchem-1.2.5.data/data/config.yml
 -rw-r--r--  2.0 unx        0 b- defN 23-May-25 06:45 autoqchem/__init__.py
 -rw-r--r--  2.0 unx    24645 b- defN 23-May-25 06:45 autoqchem/db_functions.py
 -rw-r--r--  2.0 unx     2587 b- defN 22-Oct-06 20:25 autoqchem/descriptor_functions.py
 -rw-r--r--  2.0 unx      981 b- defN 22-Oct-06 20:25 autoqchem/draw_utils.py
 -rw-r--r--  2.0 unx     6445 b- defN 23-May-30 21:03 autoqchem/gaussian_input_generator.py
--rw-r--r--  2.0 unx    19202 b- defN 23-May-25 06:45 autoqchem/gaussian_log_extractor.py
--rw-r--r--  2.0 unx     4775 b- defN 23-May-25 06:45 autoqchem/helper_classes.py
+-rw-r--r--  2.0 unx    19324 b- defN 23-May-30 23:48 autoqchem/gaussian_log_extractor.py
+-rw-r--r--  2.0 unx     5086 b- defN 23-May-31 00:05 autoqchem/helper_classes.py
 -rw-r--r--  2.0 unx     4234 b- defN 23-May-25 06:45 autoqchem/helper_functions.py
 -rw-r--r--  2.0 unx     2536 b- defN 23-May-30 22:10 autoqchem/molecule.py
 -rw-r--r--  2.0 unx     2274 b- defN 23-May-30 22:08 autoqchem/openbabel_utils.py
 -rw-r--r--  2.0 unx    11206 b- defN 23-May-25 06:45 autoqchem/rdkit_utils.py
 -rw-r--r--  2.0 unx    28155 b- defN 23-May-25 06:48 autoqchem/sge_manager.py
 -rw-r--r--  2.0 unx    25908 b- defN 23-May-25 06:46 autoqchem/slurm_manager.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-30 21:01 autoqchem/test.py
--rw-r--r--  2.0 unx    35149 b- defN 23-May-30 23:38 auto_qchem-1.2.4.dist-info/LICENSE.md
--rw-r--r--  2.0 unx      546 b- defN 23-May-30 23:38 auto_qchem-1.2.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-30 23:38 auto_qchem-1.2.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-May-30 23:38 auto_qchem-1.2.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1663 b- defN 23-May-30 23:38 auto_qchem-1.2.4.dist-info/RECORD
-20 files, 170619 bytes uncompressed, 49463 bytes compressed:  71.0%
+-rw-r--r--  2.0 unx    35149 b- defN 23-May-31 00:08 auto_qchem-1.2.5.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx      546 b- defN 23-May-31 00:08 auto_qchem-1.2.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 00:08 auto_qchem-1.2.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-May-31 00:08 auto_qchem-1.2.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1663 b- defN 23-May-31 00:08 auto_qchem-1.2.5.dist-info/RECORD
+20 files, 171052 bytes uncompressed, 49647 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -1,8 +1,8 @@
-Filename: auto_qchem-1.2.4.data/data/config.yml
+Filename: auto_qchem-1.2.5.data/data/config.yml
 Comment: 
 
 Filename: autoqchem/__init__.py
 Comment: 
 
 Filename: autoqchem/db_functions.py
 Comment: 
@@ -39,23 +39,23 @@
 
 Filename: autoqchem/slurm_manager.py
 Comment: 
 
 Filename: autoqchem/test.py
 Comment: 
 
-Filename: auto_qchem-1.2.4.dist-info/LICENSE.md
+Filename: auto_qchem-1.2.5.dist-info/LICENSE.md
 Comment: 
 
-Filename: auto_qchem-1.2.4.dist-info/METADATA
+Filename: auto_qchem-1.2.5.dist-info/METADATA
 Comment: 
 
-Filename: auto_qchem-1.2.4.dist-info/WHEEL
+Filename: auto_qchem-1.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: auto_qchem-1.2.4.dist-info/top_level.txt
+Filename: auto_qchem-1.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: auto_qchem-1.2.4.dist-info/RECORD
+Filename: auto_qchem-1.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## autoqchem/gaussian_log_extractor.py

```diff
@@ -14,14 +14,15 @@
 
         :param log_file_path: local path of the log file
         :type log_file_path: str
         """
 
         with open(log_file_path) as f:
             self.log = f.read()
+        self.log_file_path = log_file_path  # record keeping; used to output log file path in case of exception
 
         # initialize descriptors
         self.descriptors = {}
         self.atom_freq_descriptors = None
         self.atom_td_descriptors = None
         self.atom_descriptors = None
         self.vbur = None
@@ -42,18 +43,18 @@
         except IndexError:
             raise NoGeometryException()
 
         try:
             self._get_frequencies_and_moment_vectors()  # fetch vibration table and vectors
             freqs = [*map(float, self.modes['Frequencies'])]  # extract frequencies
             if [*filter(lambda x: x < 0., freqs)]:  # check for negative frequencies
-                print(self.log.name)
+                print(self.log_file_path)
                 raise NegativeFrequencyException()
         except TypeError:  # no frequencies
-            print(self.log.name)
+            print(self.log_file_path)
             raise OptimizationIncompleteException()
 
     def get_descriptors(self) -> dict:
         """Extract and retrieve all descriptors as a dictionary.
 
         :return: dict
         """
```

## autoqchem/helper_classes.py

```diff
@@ -1,15 +1,30 @@
 import enum
 import os
 import numpy as np
 from dataclasses import dataclass
 
 import yaml
 
-config = yaml.safe_load(open(os.path.join(os.path.dirname(__file__), "..", "config.yml")))
+#config = yaml.safe_load(open(os.path.join(os.path.dirname(__file__), "..", "config.yml")))
+config = {
+    'resources': {
+        'wall_time': "23:59:00",
+        'atoms_per_processor': 6,
+        'max_processors': 20,
+        'ram_per_processor': 2,
+    },
+    'mongoDB':{
+        'host': "autoqchem.org",
+        'port': '27017',
+        'user': "acqWriter",
+        'password': "dftworks",
+    }
+}
+
 k_in_kcal_per_mol_K = 0.0019872041
 Hartree_in_kcal_per_mol = 627.5
 T = 298
 
 
 @enum.unique
 class slurm_status(enum.IntEnum):
```

## Comparing `auto_qchem-1.2.4.dist-info/LICENSE.md` & `auto_qchem-1.2.5.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `auto_qchem-1.2.4.dist-info/METADATA` & `auto_qchem-1.2.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-qchem
-Version: 1.2.4
+Version: 1.2.5
 Summary: auto-qchem
 Home-page: https://github.com/doyle-lab-ucla/auto-qchem
 Author: Andrzej Zuranski, Benjamin Shields, Jason Wang, Winston Gee
 License: GPL
 License-File: LICENSE.md
 Requires-Dist: numpy (==1.21)
 Requires-Dist: pandas (==1.3)
```

## Comparing `auto_qchem-1.2.4.dist-info/RECORD` & `auto_qchem-1.2.5.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-auto_qchem-1.2.4.data/data/config.yml,sha256=CKTQfUKq3utfZs2PvBEDY_sh5A4R1CO5YX8R4tKQ7kY,211
+auto_qchem-1.2.5.data/data/config.yml,sha256=CKTQfUKq3utfZs2PvBEDY_sh5A4R1CO5YX8R4tKQ7kY,211
 autoqchem/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 autoqchem/db_functions.py,sha256=4Tj8EdmsR3tmh48flxvR88WUvw35wiWAVaXPqJGnKC0,24645
 autoqchem/descriptor_functions.py,sha256=-2bBVQvaThDjkQNdUOkGeWM7idouisQU6SnxuXyxvV0,2587
 autoqchem/draw_utils.py,sha256=mKnLnH3EclvKGMeDJ7FXny-4Oq2j8XVg0JiN3Bap-jY,981
 autoqchem/gaussian_input_generator.py,sha256=68hod8d37aY23EjUyCzH8lKC8-MbREuXnGZZ69HsDC4,6445
-autoqchem/gaussian_log_extractor.py,sha256=F7TwTAi8QQQxeI8AeH8zR-QEfcqREE8_pYPiGCOTZiM,19202
-autoqchem/helper_classes.py,sha256=3sYd8n52hAP7OZWa9XIQLBjd0gGuhXbnV7aKd-3zJM0,4775
+autoqchem/gaussian_log_extractor.py,sha256=YRJmQP7dsVJPJLD72ho6emZ00EjqPmM1oHA8sUj7pmc,19324
+autoqchem/helper_classes.py,sha256=Q9ZLs1AbKpX1gtOqN8R1H1Mkuf0jNsmrLHo_BK65b_E,5086
 autoqchem/helper_functions.py,sha256=F1sP-sfW0iBJSc_VqdX0J3kCfgoEb_4ACEZsfNCL918,4234
 autoqchem/molecule.py,sha256=D6SrV2Bfa-W461b0EQ_nJt-GRimAS67ByI5SSaZ6tNs,2536
 autoqchem/openbabel_utils.py,sha256=h4vXa8K07ANKZT1zZkXzAqergQVZIMW7giDtywQhHZg,2274
 autoqchem/rdkit_utils.py,sha256=Hhgza2sNdFlV4HKyHgeEPPfAAJLbd2Ww0DkveO_P_0I,11206
 autoqchem/sge_manager.py,sha256=PSTOLBPz_y_fSo2lleK69RHMTRFr6lrGkmZF40n_oYs,28155
 autoqchem/slurm_manager.py,sha256=MEX_qa6sJZQjtW0f8pHya5aP4mwvbSw-RymASy1TL-U,25908
 autoqchem/test.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-auto_qchem-1.2.4.dist-info/LICENSE.md,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-auto_qchem-1.2.4.dist-info/METADATA,sha256=73NBs_lAzJVr2jaILBRxrmfhzGX-r2dqPt-WdsLs2ZQ,546
-auto_qchem-1.2.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-auto_qchem-1.2.4.dist-info/top_level.txt,sha256=wTV0eKZGGXta2jVcCBo9lzUBZQt7Zmi2RG3sLVJs0UU,10
-auto_qchem-1.2.4.dist-info/RECORD,,
+auto_qchem-1.2.5.dist-info/LICENSE.md,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+auto_qchem-1.2.5.dist-info/METADATA,sha256=FOQi1ZYXrTmTVCZz87fLrb110XTCbduErjhtL5EyAAQ,546
+auto_qchem-1.2.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+auto_qchem-1.2.5.dist-info/top_level.txt,sha256=wTV0eKZGGXta2jVcCBo9lzUBZQt7Zmi2RG3sLVJs0UU,10
+auto_qchem-1.2.5.dist-info/RECORD,,
```

