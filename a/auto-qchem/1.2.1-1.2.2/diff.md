# Comparing `tmp/auto_qchem-1.2.1-py3-none-any.whl.zip` & `tmp/auto_qchem-1.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
 Zip file size: 52184 bytes, number of entries: 20
--rw-r--r--  2.0 unx      211 b- defN 23-May-25 06:45 auto_qchem-1.2.1.data/data/config.yml
+-rw-r--r--  2.0 unx      211 b- defN 23-May-25 06:45 auto_qchem-1.2.2.data/data/config.yml
 -rw-r--r--  2.0 unx        0 b- defN 23-May-25 06:45 autoqchem/__init__.py
 -rw-r--r--  2.0 unx    24645 b- defN 23-May-25 06:45 autoqchem/db_functions.py
 -rw-r--r--  2.0 unx     2587 b- defN 22-Oct-06 20:25 autoqchem/descriptor_functions.py
 -rw-r--r--  2.0 unx      981 b- defN 22-Oct-06 20:25 autoqchem/draw_utils.py
 -rw-r--r--  2.0 unx     6445 b- defN 23-May-30 21:03 autoqchem/gaussian_input_generator.py
 -rw-r--r--  2.0 unx    19202 b- defN 23-May-25 06:45 autoqchem/gaussian_log_extractor.py
 -rw-r--r--  2.0 unx     4775 b- defN 23-May-25 06:45 autoqchem/helper_classes.py
 -rw-r--r--  2.0 unx     4234 b- defN 23-May-25 06:45 autoqchem/helper_functions.py
 -rw-r--r--  2.0 unx     2536 b- defN 23-May-30 22:10 autoqchem/molecule.py
 -rw-r--r--  2.0 unx     2274 b- defN 23-May-30 22:08 autoqchem/openbabel_utils.py
 -rw-r--r--  2.0 unx    11206 b- defN 23-May-25 06:45 autoqchem/rdkit_utils.py
 -rw-r--r--  2.0 unx    28155 b- defN 23-May-25 06:48 autoqchem/sge_manager.py
 -rw-r--r--  2.0 unx    25908 b- defN 23-May-25 06:46 autoqchem/slurm_manager.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-30 21:01 autoqchem/test.py
--rw-r--r--  2.0 unx    35149 b- defN 23-May-30 23:23 auto_qchem-1.2.1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx      591 b- defN 23-May-30 23:23 auto_qchem-1.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-30 23:23 auto_qchem-1.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-May-30 23:23 auto_qchem-1.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1663 b- defN 23-May-30 23:23 auto_qchem-1.2.1.dist-info/RECORD
-20 files, 170664 bytes uncompressed, 49474 bytes compressed:  71.0%
+-rw-r--r--  2.0 unx    35149 b- defN 23-May-30 23:32 auto_qchem-1.2.2.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx      592 b- defN 23-May-30 23:32 auto_qchem-1.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-30 23:32 auto_qchem-1.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-May-30 23:32 auto_qchem-1.2.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1663 b- defN 23-May-30 23:32 auto_qchem-1.2.2.dist-info/RECORD
+20 files, 170665 bytes uncompressed, 49474 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -1,8 +1,8 @@
-Filename: auto_qchem-1.2.1.data/data/config.yml
+Filename: auto_qchem-1.2.2.data/data/config.yml
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
 
-Filename: auto_qchem-1.2.1.dist-info/LICENSE.md
+Filename: auto_qchem-1.2.2.dist-info/LICENSE.md
 Comment: 
 
-Filename: auto_qchem-1.2.1.dist-info/METADATA
+Filename: auto_qchem-1.2.2.dist-info/METADATA
 Comment: 
 
-Filename: auto_qchem-1.2.1.dist-info/WHEEL
+Filename: auto_qchem-1.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: auto_qchem-1.2.1.dist-info/top_level.txt
+Filename: auto_qchem-1.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: auto_qchem-1.2.1.dist-info/RECORD
+Filename: auto_qchem-1.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `auto_qchem-1.2.1.dist-info/LICENSE.md` & `auto_qchem-1.2.2.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `auto_qchem-1.2.1.dist-info/METADATA` & `auto_qchem-1.2.2.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: auto-qchem
-Version: 1.2.1
+Version: 1.2.2
 Summary: auto-qchem
 Home-page: https://github.com/doyle-lab-ucla/auto-qchem
 Author: Andrzej Zuranski, Benjamin Shields, Jason Wang, Winston Gee
 License: GPL
 License-File: LICENSE.md
 Requires-Dist: numpy (==1.21)
 Requires-Dist: pandas (==1.3)
 Requires-Dist: pyyaml (==6.0)
 Requires-Dist: scipy (==1.7)
 Requires-Dist: fabric (==2.6)
 Requires-Dist: paramiko (==3.1)
-Requires-Dist: pymongo (==4.3)
+Requires-Dist: pymongo (==3.10)
 Requires-Dist: appdirs (==1.4)
 Requires-Dist: ipywidgets (==8.0)
 Requires-Dist: py3Dmol (==1.8)
 Requires-Dist: rdkit
 Requires-Dist: openbabel
```

## Comparing `auto_qchem-1.2.1.dist-info/RECORD` & `auto_qchem-1.2.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-auto_qchem-1.2.1.data/data/config.yml,sha256=CKTQfUKq3utfZs2PvBEDY_sh5A4R1CO5YX8R4tKQ7kY,211
+auto_qchem-1.2.2.data/data/config.yml,sha256=CKTQfUKq3utfZs2PvBEDY_sh5A4R1CO5YX8R4tKQ7kY,211
 autoqchem/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 autoqchem/db_functions.py,sha256=4Tj8EdmsR3tmh48flxvR88WUvw35wiWAVaXPqJGnKC0,24645
 autoqchem/descriptor_functions.py,sha256=-2bBVQvaThDjkQNdUOkGeWM7idouisQU6SnxuXyxvV0,2587
 autoqchem/draw_utils.py,sha256=mKnLnH3EclvKGMeDJ7FXny-4Oq2j8XVg0JiN3Bap-jY,981
 autoqchem/gaussian_input_generator.py,sha256=68hod8d37aY23EjUyCzH8lKC8-MbREuXnGZZ69HsDC4,6445
 autoqchem/gaussian_log_extractor.py,sha256=F7TwTAi8QQQxeI8AeH8zR-QEfcqREE8_pYPiGCOTZiM,19202
 autoqchem/helper_classes.py,sha256=3sYd8n52hAP7OZWa9XIQLBjd0gGuhXbnV7aKd-3zJM0,4775
 autoqchem/helper_functions.py,sha256=F1sP-sfW0iBJSc_VqdX0J3kCfgoEb_4ACEZsfNCL918,4234
 autoqchem/molecule.py,sha256=D6SrV2Bfa-W461b0EQ_nJt-GRimAS67ByI5SSaZ6tNs,2536
 autoqchem/openbabel_utils.py,sha256=h4vXa8K07ANKZT1zZkXzAqergQVZIMW7giDtywQhHZg,2274
 autoqchem/rdkit_utils.py,sha256=Hhgza2sNdFlV4HKyHgeEPPfAAJLbd2Ww0DkveO_P_0I,11206
 autoqchem/sge_manager.py,sha256=PSTOLBPz_y_fSo2lleK69RHMTRFr6lrGkmZF40n_oYs,28155
 autoqchem/slurm_manager.py,sha256=MEX_qa6sJZQjtW0f8pHya5aP4mwvbSw-RymASy1TL-U,25908
 autoqchem/test.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-auto_qchem-1.2.1.dist-info/LICENSE.md,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-auto_qchem-1.2.1.dist-info/METADATA,sha256=pCXWVqz6bQbr7bJbG3jkI5mpWAg4aa6U4loRx-tPqHo,591
-auto_qchem-1.2.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-auto_qchem-1.2.1.dist-info/top_level.txt,sha256=wTV0eKZGGXta2jVcCBo9lzUBZQt7Zmi2RG3sLVJs0UU,10
-auto_qchem-1.2.1.dist-info/RECORD,,
+auto_qchem-1.2.2.dist-info/LICENSE.md,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+auto_qchem-1.2.2.dist-info/METADATA,sha256=sEHjvh8DQ1I6F2IndwVD8QbhHjvQt5EyvO_dF1MFdik,592
+auto_qchem-1.2.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+auto_qchem-1.2.2.dist-info/top_level.txt,sha256=wTV0eKZGGXta2jVcCBo9lzUBZQt7Zmi2RG3sLVJs0UU,10
+auto_qchem-1.2.2.dist-info/RECORD,,
```

