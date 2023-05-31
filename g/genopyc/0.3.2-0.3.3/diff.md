# Comparing `tmp/genopyc-0.3.2-py3-none-any.whl.zip` & `tmp/genopyc-0.3.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 18327 bytes, number of entries: 7
--rwxrwxrwx  2.0 unx      797 b- defN 23-Mar-21 18:10 genopyc/__init__.py
+Zip file size: 18358 bytes, number of entries: 7
+-rwxrwxrwx  2.0 unx      958 b- defN 23-May-31 10:58 genopyc/__init__.py
 -rwxrwxrwx  2.0 unx    23936 b- defN 23-May-31 10:49 genopyc/genopyc.py
--rwxrwxrwx  2.0 unx    34523 b- defN 23-May-31 10:49 genopyc-0.3.2.dist-info/LICENSE.txt
--rwxrwxrwx  2.0 unx      463 b- defN 23-May-31 10:49 genopyc-0.3.2.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-May-31 10:49 genopyc-0.3.2.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        8 b- defN 23-May-31 10:49 genopyc-0.3.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      540 b- defN 23-May-31 10:50 genopyc-0.3.2.dist-info/RECORD
-7 files, 60359 bytes uncompressed, 17373 bytes compressed:  71.2%
+-rwxrwxrwx  2.0 unx    34523 b- defN 23-May-31 10:59 genopyc-0.3.3.dist-info/LICENSE.txt
+-rwxrwxrwx  2.0 unx      463 b- defN 23-May-31 10:59 genopyc-0.3.3.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-May-31 10:59 genopyc-0.3.3.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        8 b- defN 23-May-31 10:59 genopyc-0.3.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      540 b- defN 23-May-31 10:59 genopyc-0.3.3.dist-info/RECORD
+7 files, 60520 bytes uncompressed, 17404 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: genopyc/__init__.py
 Comment: 
 
 Filename: genopyc/genopyc.py
 Comment: 
 
-Filename: genopyc-0.3.2.dist-info/LICENSE.txt
+Filename: genopyc-0.3.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: genopyc-0.3.2.dist-info/METADATA
+Filename: genopyc-0.3.3.dist-info/METADATA
 Comment: 
 
-Filename: genopyc-0.3.2.dist-info/WHEEL
+Filename: genopyc-0.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: genopyc-0.3.2.dist-info/top_level.txt
+Filename: genopyc-0.3.3.dist-info/top_level.txt
 Comment: 
 
-Filename: genopyc-0.3.2.dist-info/RECORD
+Filename: genopyc-0.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## genopyc/__init__.py

```diff
@@ -1,18 +1,22 @@
-from genopyc.genopyc import get_associations
-from genopyc.genopyc import get_gene_position_many
-from genopyc.genopyc import get_variant_position_many
-from genopyc.genopyc import HGVS_VEP
-from genopyc.genopyc import VEP
-from genopyc.genopyc import get_variants_in_LD
-from genopyc.genopyc import get_summary_statistic
-from genopyc.genopyc import get_summary_statistic_list
-from genopyc.genopyc import get_phenotypes
-from genopyc.genopyc import get_ov_region
-from genopyc.genopyc import get_sequence
-from genopyc.genopyc import grch_liftover
-from genopyc.genopyc import get_eqtl_variant
-from genopyc.genopyc import get_variant_info
-from genopyc.genopyc import get_variant_info_many
-from genopyc.genopyc import get_eqtl_df
-from genopyc.genopyc import GetLDMatrix
-from genopyc.genopyc import PairwiseLD
+from genopyc.genopyc import *
+
+# from genopyc.genopyc import get_associations
+# from genopyc.genopyc import get_gene_position_many
+# from genopyc.genopyc import get_variant_position_many
+# from genopyc.genopyc import HGVS_VEP
+# from genopyc.genopyc import VEP
+# from genopyc.genopyc import get_variants_in_LD
+# from genopyc.genopyc import get_summary_statistic
+# from genopyc.genopyc import get_summary_statistic_list
+# from genopyc.genopyc import get_phenotypes
+# from genopyc.genopyc import get_ov_region
+# from genopyc.genopyc import get_sequence
+# from genopyc.genopyc import grch_liftover
+# from genopyc.genopyc import get_eqtl_variant
+# from genopyc.genopyc import get_variant_info
+# from genopyc.genopyc import get_variant_info_many
+# from genopyc.genopyc import get_eqtl_df
+# from genopyc.genopyc import GetLDMatrix
+# from genopyc.genopyc import PairwiseLD
+# from genopyc.genopyc import ConvertVariants
+# from genopyc.genopyc import OTVariantsToGenes
```

## Comparing `genopyc-0.3.2.dist-info/LICENSE.txt` & `genopyc-0.3.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `genopyc-0.3.2.dist-info/RECORD` & `genopyc-0.3.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-genopyc/__init__.py,sha256=SEtaeN_AiqS_SPmJnLBMGWCLJ0sQ2b9ppJoVP9kMa2k,797
+genopyc/__init__.py,sha256=_WPurdLjzzEBech-ijBj1SU5fBCcriP3xwQkqXxvfwA,958
 genopyc/genopyc.py,sha256=4kzcfnkmUc_PWING5b-k-DQ634jcu2cpqwOIry6BOdM,23936
-genopyc-0.3.2.dist-info/LICENSE.txt,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
-genopyc-0.3.2.dist-info/METADATA,sha256=eAzu9DnuCRSkA2CMamwD5UiaCSyJXM6D1mViCmbncVE,463
-genopyc-0.3.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-genopyc-0.3.2.dist-info/top_level.txt,sha256=Wo4uco8QIcmZcoQJmxDYvrDatX_GrmASBAr5wSeBevA,8
-genopyc-0.3.2.dist-info/RECORD,,
+genopyc-0.3.3.dist-info/LICENSE.txt,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
+genopyc-0.3.3.dist-info/METADATA,sha256=hP9Z3XECSGdGkb8R477ziCyHp3oB2nbww0dQp4dBGIU,463
+genopyc-0.3.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+genopyc-0.3.3.dist-info/top_level.txt,sha256=Wo4uco8QIcmZcoQJmxDYvrDatX_GrmASBAr5wSeBevA,8
+genopyc-0.3.3.dist-info/RECORD,,
```

