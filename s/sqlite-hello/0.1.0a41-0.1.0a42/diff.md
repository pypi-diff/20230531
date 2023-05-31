# Comparing `tmp/sqlite_hello-0.1.0a41-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip` & `tmp/sqlite_hello-0.1.0a42-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8401 bytes, number of entries: 9
--rwxr-xr-x  2.0 unx    15784 b- defN 23-May-31 21:26 noop.cpython-311-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      305 b- defN 23-May-31 21:26 sqlite_hello/__init__.py
--rwxr-xr-x  2.0 unx    15856 b- defN 23-May-31 21:26 sqlite_hello/hello0.so
--rwxr-xr-x  2.0 unx    15848 b- defN 23-May-31 21:26 sqlite_hello/hola0.so
--rw-r--r--  2.0 unx       80 b- defN 23-May-31 21:26 sqlite_hello/version.py
--rw-r--r--  2.0 unx      507 b- defN 23-May-31 21:26 sqlite_hello-0.1.0a41.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 23-May-31 21:26 sqlite_hello-0.1.0a41.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-May-31 21:26 sqlite_hello-0.1.0a41.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      741 b- defN 23-May-31 21:26 sqlite_hello-0.1.0a41.dist-info/RECORD
-9 files, 49244 bytes uncompressed, 7123 bytes compressed:  85.5%
+Zip file size: 8404 bytes, number of entries: 9
+-rwxr-xr-x  2.0 unx    15784 b- defN 23-May-31 21:31 noop.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      305 b- defN 23-May-31 21:31 sqlite_hello/__init__.py
+-rwxr-xr-x  2.0 unx    15856 b- defN 23-May-31 21:31 sqlite_hello/hello0.so
+-rwxr-xr-x  2.0 unx    15848 b- defN 23-May-31 21:31 sqlite_hello/hola0.so
+-rw-r--r--  2.0 unx       80 b- defN 23-May-31 21:31 sqlite_hello/version.py
+-rw-r--r--  2.0 unx      507 b- defN 23-May-31 21:31 sqlite_hello-0.1.0a42.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 23-May-31 21:31 sqlite_hello-0.1.0a42.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-May-31 21:31 sqlite_hello-0.1.0a42.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      741 b- defN 23-May-31 21:31 sqlite_hello-0.1.0a42.dist-info/RECORD
+9 files, 49244 bytes uncompressed, 7126 bytes compressed:  85.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: sqlite_hello/hola0.so
 Comment: 
 
 Filename: sqlite_hello/version.py
 Comment: 
 
-Filename: sqlite_hello-0.1.0a41.dist-info/METADATA
+Filename: sqlite_hello-0.1.0a42.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_hello-0.1.0a41.dist-info/WHEEL
+Filename: sqlite_hello-0.1.0a42.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_hello-0.1.0a41.dist-info/top_level.txt
+Filename: sqlite_hello-0.1.0a42.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_hello-0.1.0a41.dist-info/RECORD
+Filename: sqlite_hello-0.1.0a42.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_hello/hello0.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 70d8c1875419fc2202c4a7a74bde9afaae2f221c
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: dd78ecb6d971f9acf4c8ce18551749fe6edd507f
```

### strings --all --bytes=8 {}

```diff
@@ -1,15 +1,15 @@
 __gmon_start__
 _ITM_deregisterTMCloneTable
 _ITM_registerTMCloneTable
 __cxa_finalize
 sqlite3_api
 sqlite3_hello_init
 Hello, %s!
-v0.1.0-alpha.41
+v0.1.0-alpha.42
 hello_version
 GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.1) 9.4.0
 crtstuff.c
 deregister_tm_clones
 __do_global_dtors_aux
 completed.8061
 __do_global_dtors_aux_fini_array_entry
```

### readelf --wide --decompress --string-dump=.rodata {}

```diff
@@ -1,7 +1,7 @@
 
 String dump of section '.rodata':
   [     0]  Hello, %s!
-  [     b]  v0.1.0-alpha.41
+  [     b]  v0.1.0-alpha.42
   [    1b]  hello
   [    21]  hello_version
```

## sqlite_hello/hola0.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: c232ef35a548bd185ed8a0cd271a1eb89cdd3a86
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: bf2ab3e9950ea875081209f7ec6819fd3636a0f5
```

### strings --all --bytes=8 {}

```diff
@@ -1,15 +1,15 @@
 __gmon_start__
 _ITM_deregisterTMCloneTable
 _ITM_registerTMCloneTable
 __cxa_finalize
 sqlite3_api
 sqlite3_hola_init
 Hola, %s!
-v0.1.0-alpha.41
+v0.1.0-alpha.42
 hola_version
 GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.1) 9.4.0
 crtstuff.c
 deregister_tm_clones
 __do_global_dtors_aux
 completed.8061
 __do_global_dtors_aux_fini_array_entry
```

### readelf --wide --decompress --string-dump=.rodata {}

```diff
@@ -1,7 +1,7 @@
 
 String dump of section '.rodata':
   [     2]  Hola, %s!
-  [     c]  v0.1.0-alpha.41
+  [     c]  v0.1.0-alpha.42
   [    1c]  hola
   [    21]  hola_version
```

## sqlite_hello/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.41"
+__version__ = "0.1.0-alpha.42"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_hello-0.1.0a41.dist-info/RECORD` & `sqlite_hello-0.1.0a42.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 noop.cpython-311-x86_64-linux-gnu.so,sha256=EYkwvM4rO5qdrRrumV09xH-JHgEZiTW5qhXN2rWNjJs,15784
 sqlite_hello/__init__.py,sha256=pcA3IBYCodi0pYnpMRWpFRZcLsiBjMrMdhPM0TLEzUM,305
-sqlite_hello/hello0.so,sha256=hRrXunpnoKGx3Tiyl6cO2Dp_TRLZocitgl1uj1GghGc,15856
-sqlite_hello/hola0.so,sha256=hoIxuroL99ZgtxhcqllyVX51pIzXMWMfrENUhpRatuk,15848
-sqlite_hello/version.py,sha256=ibL2gdZDCIseoFnes9IQUQV7UdV4zxsKwgE_mLm2q4Y,80
-sqlite_hello-0.1.0a41.dist-info/METADATA,sha256=GXTEzlZhubgslV91hFxWM2pyIDMmw6k4ALUnajYBWFI,507
-sqlite_hello-0.1.0a41.dist-info/WHEEL,sha256=A8X7wachHegSPoWuFmtYiHrJoCGdZ0KzfYp5hU1FoC8,105
-sqlite_hello-0.1.0a41.dist-info/top_level.txt,sha256=KjVnaNCiS11UOKhSHnqZUwUFlrCeCQv89AtVw-JnynI,18
-sqlite_hello-0.1.0a41.dist-info/RECORD,,
+sqlite_hello/hello0.so,sha256=1PRj4tkcJKOUGRAMw9EH7_D3kIbSHm3YHjTFsAYopw8,15856
+sqlite_hello/hola0.so,sha256=MNL6Flc3wVwjiZDIbhz8ghdAa72xNeifgTS7ZJm8GrY,15848
+sqlite_hello/version.py,sha256=BiQW6BrWJGdZMidQn-2R_EhTQZcYKILeNcKEWiPyGxY,80
+sqlite_hello-0.1.0a42.dist-info/METADATA,sha256=jvfbgKqrqUdd1ShSx03ilkfdE2AT2yJKNG_EZwxcwuk,507
+sqlite_hello-0.1.0a42.dist-info/WHEEL,sha256=A8X7wachHegSPoWuFmtYiHrJoCGdZ0KzfYp5hU1FoC8,105
+sqlite_hello-0.1.0a42.dist-info/top_level.txt,sha256=KjVnaNCiS11UOKhSHnqZUwUFlrCeCQv89AtVw-JnynI,18
+sqlite_hello-0.1.0a42.dist-info/RECORD,,
```

