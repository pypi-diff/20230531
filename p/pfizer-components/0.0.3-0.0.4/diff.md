# Comparing `tmp/pfizer_components-0.0.3-py3-none-any.whl.zip` & `tmp/pfizer_components-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 25306 bytes, number of entries: 15
+Zip file size: 25305 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-24 22:59 pfizer_components.py
 -rw-rw-rw-  2.0 fat     6282 b- defN 23-May-23 08:01 pfizer_components/Button.py
 -rw-rw-rw-  2.0 fat    38851 b- defN 23-May-30 13:49 pfizer_components/Cards.py
 -rw-rw-rw-  2.0 fat      816 b- defN 23-May-30 13:46 pfizer_components/Carousel.py
 -rw-rw-rw-  2.0 fat     4314 b- defN 23-May-23 10:41 pfizer_components/Checkbox.py
 -rw-rw-rw-  2.0 fat     5846 b- defN 23-May-23 15:35 pfizer_components/Dropdown.py
 -rw-rw-rw-  2.0 fat    12287 b- defN 23-May-25 12:09 pfizer_components/Input.py
 -rw-rw-rw-  2.0 fat     2656 b- defN 23-May-24 06:15 pfizer_components/Usage_css.py
 -rw-rw-rw-  2.0 fat     2728 b- defN 23-May-30 13:56 pfizer_components/Usage_python.py
--rw-rw-rw-  2.0 fat      155 b- defN 23-May-30 13:58 pfizer_components/__init__.py
+-rw-rw-rw-  2.0 fat      157 b- defN 23-May-31 12:58 pfizer_components/__init__.py
 -rw-rw-rw-  2.0 fat    29164 b- defN 23-May-25 12:25 pfizer_components/components.py
--rw-rw-rw-  2.0 fat      442 b- defN 23-May-30 13:59 pfizer_components-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 13:59 pfizer_components-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-May-30 13:59 pfizer_components-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1271 b- defN 23-May-30 13:59 pfizer_components-0.0.3.dist-info/RECORD
-15 files, 104922 bytes uncompressed, 23190 bytes compressed:  77.9%
+-rw-rw-rw-  2.0 fat      442 b- defN 23-May-31 13:03 pfizer_components-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-31 13:03 pfizer_components-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-May-31 13:03 pfizer_components-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1271 b- defN 23-May-31 13:03 pfizer_components-0.0.4.dist-info/RECORD
+15 files, 104924 bytes uncompressed, 23189 bytes compressed:  77.9%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: pfizer_components/__init__.py
 Comment: 
 
 Filename: pfizer_components/components.py
 Comment: 
 
-Filename: pfizer_components-0.0.3.dist-info/METADATA
+Filename: pfizer_components-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: pfizer_components-0.0.3.dist-info/WHEEL
+Filename: pfizer_components-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: pfizer_components-0.0.3.dist-info/top_level.txt
+Filename: pfizer_components-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pfizer_components-0.0.3.dist-info/RECORD
+Filename: pfizer_components-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pfizer_components/__init__.py

```diff
@@ -1,3 +1,3 @@
-from pfizer_components.Components import Button, Checkbox, Dropdown, Input
+from pfizer_components.components import Button, Checkbox, Dropdown, Input
 from pfizer_components.Cards import *
-from pfizer_components.Carousel import *
+from pfizer_components.Carousel import *
```

## Comparing `pfizer_components-0.0.3.dist-info/RECORD` & `pfizer_components-0.0.4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 pfizer_components/Cards.py,sha256=nEpIkroRZ9r89yTaR9_YG7I_mP5S5KDgZvY5plrZeIM,38851
 pfizer_components/Carousel.py,sha256=lK-PIP4mrDbVbzmBVKHr7cjPXajhuHi_N-h7fBIe2v8,816
 pfizer_components/Checkbox.py,sha256=nFzX_kjKZwHKhiC0_Aa5gOAmop1l2wvJqTFn4jbPXak,4314
 pfizer_components/Dropdown.py,sha256=Phoa7If8Rrsnfn5xVggavKr6VGYfJMcI0xX563Xettg,5846
 pfizer_components/Input.py,sha256=bcuLpMSgbNqsKq5XhtLVyeEIYWBwexEFqf9hpLbNUnc,12287
 pfizer_components/Usage_css.py,sha256=Zhs8Bs0vzlBqo_GEuujWGUuIzb-ubX_ZNm7WyixOUnY,2656
 pfizer_components/Usage_python.py,sha256=7qY620X3pRX0i3JqIIS3yoOopTYdItLzH-49j1Ujs0s,2728
-pfizer_components/__init__.py,sha256=Pd4_DoogSWRltDmhk276SWX8XnF558tB3iwNfwGATmo,155
+pfizer_components/__init__.py,sha256=-naHq8e64eZDPeUGVyUtTnIU0-sbDl0bhuNgPDxoVTY,157
 pfizer_components/components.py,sha256=vm3RaqWyEd0NLgcwreSPocjpqQMBu1As95nY2XnQin0,29164
-pfizer_components-0.0.3.dist-info/METADATA,sha256=gGPyRTm1VPQ3_gPYlrxYtKtIGIIHYsJVOq8Z48Dx4w0,442
-pfizer_components-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pfizer_components-0.0.3.dist-info/top_level.txt,sha256=gav2t-yrWrH3UFJs7L7V7a2VMnkqN-BfliBdp4mCDHw,18
-pfizer_components-0.0.3.dist-info/RECORD,,
+pfizer_components-0.0.4.dist-info/METADATA,sha256=Z9ENDkC4qHB5Uh27C5AP1lycwEo4dMhZ1GFCDBNUV1w,442
+pfizer_components-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pfizer_components-0.0.4.dist-info/top_level.txt,sha256=gav2t-yrWrH3UFJs7L7V7a2VMnkqN-BfliBdp4mCDHw,18
+pfizer_components-0.0.4.dist-info/RECORD,,
```

