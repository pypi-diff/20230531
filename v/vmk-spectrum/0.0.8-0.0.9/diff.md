# Comparing `tmp/vmk_spectrum-0.0.8-cp311-cp311-win_amd64.whl.zip` & `tmp/vmk_spectrum-0.0.9-cp311-cp311-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 77386 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat   147968 b- defN 23-May-19 08:53 _pyspectrum.cp311-win_amd64.pyd
--rw-rw-rw-  2.0 fat      159 b- defN 23-May-19 08:50 pyspectrum/__init__.py
--rw-rw-rw-  2.0 fat     5344 b- defN 23-May-19 08:50 pyspectrum/data.py
--rw-rw-rw-  2.0 fat     1257 b- defN 23-May-19 08:50 pyspectrum/device_factory.py
--rw-rw-rw-  2.0 fat      435 b- defN 23-May-19 08:50 pyspectrum/errors.py
--rw-rw-rw-  2.0 fat     4747 b- defN 23-May-19 08:50 pyspectrum/ethernet_device.py
--rw-rw-rw-  2.0 fat     9575 b- defN 23-May-19 08:50 pyspectrum/spectrometer.py
--rw-rw-rw-  2.0 fat      339 b- defN 23-May-19 08:53 vmk_spectrum-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      102 b- defN 23-May-19 08:53 vmk_spectrum-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       25 b- defN 23-May-19 08:53 vmk_spectrum-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      891 b- defN 23-May-19 08:53 vmk_spectrum-0.0.8.dist-info/RECORD
-11 files, 170842 bytes uncompressed, 75884 bytes compressed:  55.6%
+Zip file size: 81054 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat   161280 b- defN 23-May-31 13:36 _pyspectrum.cp311-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      159 b- defN 23-May-31 13:34 pyspectrum/__init__.py
+-rw-rw-rw-  2.0 fat     5344 b- defN 23-May-31 13:34 pyspectrum/data.py
+-rw-rw-rw-  2.0 fat     1257 b- defN 23-May-31 13:34 pyspectrum/device_factory.py
+-rw-rw-rw-  2.0 fat      435 b- defN 23-May-31 13:34 pyspectrum/errors.py
+-rw-rw-rw-  2.0 fat     4747 b- defN 23-May-31 13:34 pyspectrum/ethernet_device.py
+-rw-rw-rw-  2.0 fat     9575 b- defN 23-May-31 13:34 pyspectrum/spectrometer.py
+-rw-rw-rw-  2.0 fat      339 b- defN 23-May-31 13:36 vmk_spectrum-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      102 b- defN 23-May-31 13:36 vmk_spectrum-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       25 b- defN 23-May-31 13:36 vmk_spectrum-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      891 b- defN 23-May-31 13:36 vmk_spectrum-0.0.9.dist-info/RECORD
+11 files, 184154 bytes uncompressed, 79552 bytes compressed:  56.8%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: pyspectrum/ethernet_device.py
 Comment: 
 
 Filename: pyspectrum/spectrometer.py
 Comment: 
 
-Filename: vmk_spectrum-0.0.8.dist-info/METADATA
+Filename: vmk_spectrum-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: vmk_spectrum-0.0.8.dist-info/WHEEL
+Filename: vmk_spectrum-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: vmk_spectrum-0.0.8.dist-info/top_level.txt
+Filename: vmk_spectrum-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: vmk_spectrum-0.0.8.dist-info/RECORD
+Filename: vmk_spectrum-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `vmk_spectrum-0.0.8.dist-info/RECORD` & `vmk_spectrum-0.0.9.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-_pyspectrum.cp311-win_amd64.pyd,sha256=rCXj7xti25fmOfoqKbwjuny3nNHki7G3wTuF1rlihC8,147968
+_pyspectrum.cp311-win_amd64.pyd,sha256=MbDvoCxTRMfu1a56FIzD-SnHvReGr1nSlkQ-7Ld8bLk,161280
 pyspectrum/__init__.py,sha256=mSRAZpwuFOv65WJCeoTzRG7NdnXDmjvGgreEt1ejw6s,159
 pyspectrum/data.py,sha256=HPJHbyaGsWwSQMF6qNlRe48MhYwEHasz3yh_8AfG9H8,5344
 pyspectrum/device_factory.py,sha256=xGVCDVtQC8RkAkcxjg7JiLdkiR4lz9VxQikhyUhSo2c,1257
 pyspectrum/errors.py,sha256=MkI7kErUUpMkkMlwE5MU0kMlp27CcOigYszKmzNXDyY,435
 pyspectrum/ethernet_device.py,sha256=nYPBnjRJmO8TdKuMsMepB0DDiLlvE5zbXr1FWJnk-NA,4747
 pyspectrum/spectrometer.py,sha256=qvori44YiIp7FXwz-NVhGhtM6iQpD-i5t0-GvDUF9oA,9575
-vmk_spectrum-0.0.8.dist-info/METADATA,sha256=hZCtzVHxlBsZvPuD2Ygi3u1crrG3WoRRLnHmADxZ0Bk,339
-vmk_spectrum-0.0.8.dist-info/WHEEL,sha256=9wvhO-5NhjjD8YmmxAvXTPQXMDOZ50W5vklzeoqFtkM,102
-vmk_spectrum-0.0.8.dist-info/top_level.txt,sha256=NT9XfeydHYXZsKuKvLYXhwUnK_kXYb2MHLtB1hRQLY0,25
-vmk_spectrum-0.0.8.dist-info/RECORD,,
+vmk_spectrum-0.0.9.dist-info/METADATA,sha256=ma5BABh0h2sSyZhaGu7JibZ1Do4NuViq4A4uHkf-cyQ,339
+vmk_spectrum-0.0.9.dist-info/WHEEL,sha256=9wvhO-5NhjjD8YmmxAvXTPQXMDOZ50W5vklzeoqFtkM,102
+vmk_spectrum-0.0.9.dist-info/top_level.txt,sha256=NT9XfeydHYXZsKuKvLYXhwUnK_kXYb2MHLtB1hRQLY0,25
+vmk_spectrum-0.0.9.dist-info/RECORD,,
```

