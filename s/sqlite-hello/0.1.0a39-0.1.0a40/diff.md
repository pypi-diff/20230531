# Comparing `tmp/sqlite_hello-0.1.0a39-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip` & `tmp/sqlite_hello-0.1.0a40-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8400 bytes, number of entries: 9
--rwxr-xr-x  2.0 unx    15784 b- defN 23-May-29 06:32 noop.cpython-311-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      305 b- defN 23-May-29 06:32 sqlite_hello/__init__.py
--rwxr-xr-x  2.0 unx    15856 b- defN 23-May-29 06:32 sqlite_hello/hello0.so
--rwxr-xr-x  2.0 unx    15848 b- defN 23-May-29 06:32 sqlite_hello/hola0.so
--rw-r--r--  2.0 unx       80 b- defN 23-May-29 06:32 sqlite_hello/version.py
--rw-r--r--  2.0 unx      507 b- defN 23-May-29 06:32 sqlite_hello-0.1.0a39.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 23-May-29 06:32 sqlite_hello-0.1.0a39.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-May-29 06:32 sqlite_hello-0.1.0a39.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      741 b- defN 23-May-29 06:32 sqlite_hello-0.1.0a39.dist-info/RECORD
-9 files, 49244 bytes uncompressed, 7122 bytes compressed:  85.5%
+Zip file size: 8397 bytes, number of entries: 9
+-rwxr-xr-x  2.0 unx    15784 b- defN 23-May-31 21:22 noop.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      305 b- defN 23-May-31 21:22 sqlite_hello/__init__.py
+-rwxr-xr-x  2.0 unx    15856 b- defN 23-May-31 21:22 sqlite_hello/hello0.so
+-rwxr-xr-x  2.0 unx    15848 b- defN 23-May-31 21:22 sqlite_hello/hola0.so
+-rw-r--r--  2.0 unx       80 b- defN 23-May-31 21:22 sqlite_hello/version.py
+-rw-r--r--  2.0 unx      507 b- defN 23-May-31 21:22 sqlite_hello-0.1.0a40.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 23-May-31 21:22 sqlite_hello-0.1.0a40.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-May-31 21:22 sqlite_hello-0.1.0a40.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      741 b- defN 23-May-31 21:22 sqlite_hello-0.1.0a40.dist-info/RECORD
+9 files, 49244 bytes uncompressed, 7119 bytes compressed:  85.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: sqlite_hello/hola0.so
 Comment: 
 
 Filename: sqlite_hello/version.py
 Comment: 
 
-Filename: sqlite_hello-0.1.0a39.dist-info/METADATA
+Filename: sqlite_hello-0.1.0a40.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_hello-0.1.0a39.dist-info/WHEEL
+Filename: sqlite_hello-0.1.0a40.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_hello-0.1.0a39.dist-info/top_level.txt
+Filename: sqlite_hello-0.1.0a40.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_hello-0.1.0a39.dist-info/RECORD
+Filename: sqlite_hello-0.1.0a40.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_hello/hello0.so

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 460322e04e196fc93071de923096120a2b26fa27
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 36226e10523f46311f69fa1211b779455193d2f3
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
-v0.1.0-alpha.39
+v0.1.0-alpha.40
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
-  [     b]  v0.1.0-alpha.39
+  [     b]  v0.1.0-alpha.40
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
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: cfe41f81a09c55283513a840875cc403c29f09b1
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 0c08bbd1680d4e790c040628b7fc749d9f87e93d
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
-v0.1.0-alpha.39
+v0.1.0-alpha.40
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
-  [     c]  v0.1.0-alpha.39
+  [     c]  v0.1.0-alpha.40
   [    1c]  hola
   [    21]  hola_version
```

## sqlite_hello/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.39"
+__version__ = "0.1.0-alpha.40"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_hello-0.1.0a39.dist-info/RECORD` & `sqlite_hello-0.1.0a40.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 noop.cpython-311-x86_64-linux-gnu.so,sha256=EYkwvM4rO5qdrRrumV09xH-JHgEZiTW5qhXN2rWNjJs,15784
 sqlite_hello/__init__.py,sha256=pcA3IBYCodi0pYnpMRWpFRZcLsiBjMrMdhPM0TLEzUM,305
-sqlite_hello/hello0.so,sha256=vIcKPsnyL1W-KH46MpqAYInvmuaV3ruyrjUBFcg-IDY,15856
-sqlite_hello/hola0.so,sha256=V8O3O8LqfuGBv4B3v5SxfeSaBhlvf2PU4hUnNB6oqxs,15848
-sqlite_hello/version.py,sha256=fq4RaHoS-XTkYimvEcLbbhiVMOX26xtim15eh-xAJCs,80
-sqlite_hello-0.1.0a39.dist-info/METADATA,sha256=vOSDFszzxNO-3-Lk9xcPOS3wYRUH64iKf0ZHgHqY6Wk,507
-sqlite_hello-0.1.0a39.dist-info/WHEEL,sha256=A8X7wachHegSPoWuFmtYiHrJoCGdZ0KzfYp5hU1FoC8,105
-sqlite_hello-0.1.0a39.dist-info/top_level.txt,sha256=KjVnaNCiS11UOKhSHnqZUwUFlrCeCQv89AtVw-JnynI,18
-sqlite_hello-0.1.0a39.dist-info/RECORD,,
+sqlite_hello/hello0.so,sha256=FjlxfLoM4Q-aMBPebJ-4cZnkE43M8RLZBVZ4h-NLCXo,15856
+sqlite_hello/hola0.so,sha256=Vdwyer9DfuS6XQMltkq--fipjs9_KrXi0z5IOhmaB-I,15848
+sqlite_hello/version.py,sha256=n-C-KzIuBBq1QiNrP9fenSYeowhbrCUSBWmNXeY2Too,80
+sqlite_hello-0.1.0a40.dist-info/METADATA,sha256=VrIDZOuSUrOyljZ3BBzvxo7CrBErSqHxpYMyYv8HQPo,507
+sqlite_hello-0.1.0a40.dist-info/WHEEL,sha256=A8X7wachHegSPoWuFmtYiHrJoCGdZ0KzfYp5hU1FoC8,105
+sqlite_hello-0.1.0a40.dist-info/top_level.txt,sha256=KjVnaNCiS11UOKhSHnqZUwUFlrCeCQv89AtVw-JnynI,18
+sqlite_hello-0.1.0a40.dist-info/RECORD,,
```

