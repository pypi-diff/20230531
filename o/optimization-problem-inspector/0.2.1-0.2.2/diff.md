# Comparing `tmp/optimization_problem_inspector-0.2.1-py3-none-any.whl.zip` & `tmp/optimization_problem_inspector-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 30926 bytes, number of entries: 20
+Zip file size: 30961 bytes, number of entries: 20
 -rw-r--r--  2.0 unx       53 b- defN 20-Feb-02 00:00 optimization_problem_inspector/__about__.py
 -rw-r--r--  2.0 unx       31 b- defN 20-Feb-02 00:00 optimization_problem_inspector/__init__.py
--rw-r--r--  2.0 unx    36190 b- defN 20-Feb-02 00:00 optimization_problem_inspector/app.py
+-rw-r--r--  2.0 unx    36279 b- defN 20-Feb-02 00:00 optimization_problem_inspector/app.py
 -rw-r--r--  2.0 unx     1934 b- defN 20-Feb-02 00:00 optimization_problem_inspector/app_strings.py
 -rw-r--r--  2.0 unx     9974 b- defN 20-Feb-02 00:00 optimization_problem_inspector/coco_interface.py
 -rw-r--r--  2.0 unx     1608 b- defN 20-Feb-02 00:00 optimization_problem_inspector/config.py
 -rw-r--r--  2.0 unx      116 b- defN 20-Feb-02 00:00 optimization_problem_inspector/errors.py
 -rw-r--r--  2.0 unx    15342 b- defN 20-Feb-02 00:00 optimization_problem_inspector/features.py
 -rw-r--r--  2.0 unx      259 b- defN 20-Feb-02 00:00 optimization_problem_inspector/logger.py
 -rw-r--r--  2.0 unx     4836 b- defN 20-Feb-02 00:00 optimization_problem_inspector/models.py
 -rw-r--r--  2.0 unx    19332 b- defN 20-Feb-02 00:00 optimization_problem_inspector/problem.py
 -rw-r--r--  2.0 unx     9459 b- defN 20-Feb-02 00:00 optimization_problem_inspector/sampling.py
 -rw-r--r--  2.0 unx     4925 b- defN 20-Feb-02 00:00 optimization_problem_inspector/serialization.py
 -rw-r--r--  2.0 unx       86 b- defN 20-Feb-02 00:00 optimization_problem_inspector/assets/gui-help.md
 -rw-r--r--  2.0 unx      578 b- defN 20-Feb-02 00:00 optimization_problem_inspector/assets/typography.css
-?rw-r--r--  2.0 unx     3794 b- defN 20-Feb-02 00:00 optimization_problem_inspector-0.2.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 optimization_problem_inspector-0.2.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx       68 b- defN 20-Feb-02 00:00 optimization_problem_inspector-0.2.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1157 b- defN 20-Feb-02 00:00 optimization_problem_inspector-0.2.1.dist-info/licenses/LICENSE.txt
-?rw-r--r--  2.0 unx     2014 b- defN 20-Feb-02 00:00 optimization_problem_inspector-0.2.1.dist-info/RECORD
-20 files, 111843 bytes uncompressed, 27508 bytes compressed:  75.4%
+?rw-r--r--  2.0 unx     3794 b- defN 20-Feb-02 00:00 optimization_problem_inspector-0.2.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 optimization_problem_inspector-0.2.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx       68 b- defN 20-Feb-02 00:00 optimization_problem_inspector-0.2.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1157 b- defN 20-Feb-02 00:00 optimization_problem_inspector-0.2.2.dist-info/licenses/LICENSE.txt
+?rw-r--r--  2.0 unx     2014 b- defN 20-Feb-02 00:00 optimization_problem_inspector-0.2.2.dist-info/RECORD
+20 files, 111932 bytes uncompressed, 27543 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: optimization_problem_inspector/assets/gui-help.md
 Comment: 
 
 Filename: optimization_problem_inspector/assets/typography.css
 Comment: 
 
-Filename: optimization_problem_inspector-0.2.1.dist-info/METADATA
+Filename: optimization_problem_inspector-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: optimization_problem_inspector-0.2.1.dist-info/WHEEL
+Filename: optimization_problem_inspector-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: optimization_problem_inspector-0.2.1.dist-info/entry_points.txt
+Filename: optimization_problem_inspector-0.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: optimization_problem_inspector-0.2.1.dist-info/licenses/LICENSE.txt
+Filename: optimization_problem_inspector-0.2.2.dist-info/licenses/LICENSE.txt
 Comment: 
 
-Filename: optimization_problem_inspector-0.2.1.dist-info/RECORD
+Filename: optimization_problem_inspector-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## optimization_problem_inspector/__about__.py

```diff
@@ -1,2 +1,2 @@
 # SPDX-License-Identifier: MIT
-__version__ = '0.2.1'
+__version__ = '0.2.2'
```

## optimization_problem_inspector/app.py

```diff
@@ -1090,8 +1090,12 @@
     app.run_server(
         host="0.0.0.0",
         debug=True,
     )
 
 
 if __name__ == "__main__":
-    main()
+    while True:
+        try:
+            main()
+        except KeyboardInterrupt:
+            raise
```

## Comparing `optimization_problem_inspector-0.2.1.dist-info/METADATA` & `optimization_problem_inspector-0.2.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimization-problem-inspector
-Version: 0.2.1
+Version: 0.2.2
 Summary: A tool for analysis of industrial optimization problems and their solutions
 Project-URL: Documentation, https://github.com/unknown/optimization-problem-inspector#readme
 Project-URL: Issues, https://github.com/unknown/optimization-problem-inspector/issues
 Project-URL: Source, https://github.com/unknown/optimization-problem-inspector
 Author-email: Jernej Zupančič <88.jernej@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

## Comparing `optimization_problem_inspector-0.2.1.dist-info/licenses/LICENSE.txt` & `optimization_problem_inspector-0.2.2.dist-info/licenses/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `optimization_problem_inspector-0.2.1.dist-info/RECORD` & `optimization_problem_inspector-0.2.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-optimization_problem_inspector/__about__.py,sha256=HCrMGMmDNXAw1c5nKre3J9VhwWU-_h5nfoyDyX1on9w,53
+optimization_problem_inspector/__about__.py,sha256=OBnVFcuULFdtq1LErwhb9gczRYehsXt0hqtRB1WRdx8,53
 optimization_problem_inspector/__init__.py,sha256=W-Iw-hOna0MxXOaE4ehJxxBNt6owr2n32RFEtLZl4tM,31
-optimization_problem_inspector/app.py,sha256=dAfxTHOTBFDawcY6w9V2rPTkRL4gYRurbdn2WT5Wu4U,36190
+optimization_problem_inspector/app.py,sha256=kYXqojGQYP2lU0vx37UJaVSBY8daHdEWaJJaWe-iuuc,36279
 optimization_problem_inspector/app_strings.py,sha256=fgwDkjJb1uPxQCg8kv3-Cv6xnmtzudHNQ7--clfT340,1934
 optimization_problem_inspector/coco_interface.py,sha256=pJHWPDoPYBUQWhyrJYmI5I_QsTlpz3byViqFebJ1PQU,9974
 optimization_problem_inspector/config.py,sha256=dSQ99a4en6xDZELCDsa8_ewlVqQQuuilwfa-dqxzC00,1608
 optimization_problem_inspector/errors.py,sha256=r2RHeO9B5edBo8LHUMohLdB_HE_jNjAAvfkRcXE_KAw,116
 optimization_problem_inspector/features.py,sha256=-lOlZIMhh0ridtVwcFStZHf37Okow7_1iKCZi1f9cPg,15342
 optimization_problem_inspector/logger.py,sha256=Sp4yYifCT9YLdJIPn8lFaDmZoIbGFo45b21cLsNI4Lw,259
 optimization_problem_inspector/models.py,sha256=zJesjXbpYxw4nT0lsUPpXzXXwqFlDy1kXAUmraCmk3k,4836
 optimization_problem_inspector/problem.py,sha256=Bno_xSKpfEi4TesDO_VJ5pZpfnnRhTaOWk-13LW0i9E,19332
 optimization_problem_inspector/sampling.py,sha256=NfLfh1EHuTYBQVEK4IRiFvDQh-spnZTG2QKltYEG4yI,9459
 optimization_problem_inspector/serialization.py,sha256=QUraACAkt2HPpVoDQuoiaDfFDLlHhlEWozVRgaldMwI,4925
 optimization_problem_inspector/assets/gui-help.md,sha256=V1e1bEYqx48qhYnlxnqtMpAfKPLGxMty_Yye5KXCCnQ,86
 optimization_problem_inspector/assets/typography.css,sha256=JIrxZjJIZl8VySS-ao-HdCcZDpfeU9H1j87zQh6Moyw,578
-optimization_problem_inspector-0.2.1.dist-info/METADATA,sha256=CJAbSMTelHfTx7KDudGFVwInrxxnA7sAGSzydlQ-CtY,3794
-optimization_problem_inspector-0.2.1.dist-info/WHEEL,sha256=y1bSCq4r5i4nMmpXeUJMqs3ipKvkZObrIXSvJHm1qCI,87
-optimization_problem_inspector-0.2.1.dist-info/entry_points.txt,sha256=CBKAxN7Me5VbviWhbuzvvxNQVo6YB_7mitq8A5m3GMY,68
-optimization_problem_inspector-0.2.1.dist-info/licenses/LICENSE.txt,sha256=o_AcDderANEapBiEJuuDouZOWs9IH3_c2SUyfEcTVPk,1157
-optimization_problem_inspector-0.2.1.dist-info/RECORD,,
+optimization_problem_inspector-0.2.2.dist-info/METADATA,sha256=WV_K2rBelJAESCpC5CMNjz3isPASpKGB-FvDNL6TiAA,3794
+optimization_problem_inspector-0.2.2.dist-info/WHEEL,sha256=y1bSCq4r5i4nMmpXeUJMqs3ipKvkZObrIXSvJHm1qCI,87
+optimization_problem_inspector-0.2.2.dist-info/entry_points.txt,sha256=CBKAxN7Me5VbviWhbuzvvxNQVo6YB_7mitq8A5m3GMY,68
+optimization_problem_inspector-0.2.2.dist-info/licenses/LICENSE.txt,sha256=o_AcDderANEapBiEJuuDouZOWs9IH3_c2SUyfEcTVPk,1157
+optimization_problem_inspector-0.2.2.dist-info/RECORD,,
```

