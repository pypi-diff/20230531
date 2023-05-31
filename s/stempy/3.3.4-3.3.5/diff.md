# Comparing `tmp/stempy-3.3.4-cp39-cp39-win_amd64.whl.zip` & `tmp/stempy-3.3.5-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 2006125 bytes, number of entries: 16
--rw-rw-rw-  2.0 fat      101 b- defN 23-Apr-28 18:49 stempy/__init__.py
--rw-rw-rw-  2.0 fat   265216 b- defN 23-Apr-28 18:59 stempy/_image.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   219648 b- defN 23-Apr-28 18:59 stempy/_io.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat  4203520 b- defN 23-Apr-28 18:59 stempy/stem.dll
--rw-rw-rw-  2.0 fat 17225502 b- defN 23-Apr-28 18:59 stempy/stem.lib
--rw-rw-rw-  2.0 fat      556 b- defN 23-Apr-28 18:49 stempy/utils.py
--rw-rw-rw-  2.0 fat    32699 b- defN 23-Apr-28 18:49 stempy/image/__init__.py
--rw-rw-rw-  2.0 fat    10673 b- defN 23-Apr-28 18:49 stempy/io/__init__.py
--rw-rw-rw-  2.0 fat     3716 b- defN 23-Apr-28 18:49 stempy/io/compatibility.py
--rw-rw-rw-  2.0 fat    40225 b- defN 23-Apr-28 18:49 stempy/io/sparse_array.py
--rw-rw-rw-  2.0 fat     1496 b- defN 23-Apr-28 18:49 stempy/pipeline/__init__.py
--rw-rw-rw-  2.0 fat     1531 b- defN 23-Apr-28 18:59 stempy-3.3.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      492 b- defN 23-Apr-28 18:59 stempy-3.3.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       94 b- defN 23-Apr-28 18:59 stempy-3.3.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-28 18:59 stempy-3.3.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1265 b- defN 23-Apr-28 18:59 stempy-3.3.4.dist-info/RECORD
-16 files, 22006741 bytes uncompressed, 2004085 bytes compressed:  90.9%
+Zip file size: 2006130 bytes, number of entries: 16
+-rw-rw-rw-  2.0 fat      101 b- defN 23-May-31 12:59 stempy/__init__.py
+-rw-rw-rw-  2.0 fat   265216 b- defN 23-May-31 13:09 stempy/_image.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   219648 b- defN 23-May-31 13:09 stempy/_io.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat  4203520 b- defN 23-May-31 13:09 stempy/stem.dll
+-rw-rw-rw-  2.0 fat 17225502 b- defN 23-May-31 13:09 stempy/stem.lib
+-rw-rw-rw-  2.0 fat      556 b- defN 23-May-31 12:59 stempy/utils.py
+-rw-rw-rw-  2.0 fat    32699 b- defN 23-May-31 12:59 stempy/image/__init__.py
+-rw-rw-rw-  2.0 fat    10673 b- defN 23-May-31 12:59 stempy/io/__init__.py
+-rw-rw-rw-  2.0 fat     3716 b- defN 23-May-31 12:59 stempy/io/compatibility.py
+-rw-rw-rw-  2.0 fat    40225 b- defN 23-May-31 12:59 stempy/io/sparse_array.py
+-rw-rw-rw-  2.0 fat     1496 b- defN 23-May-31 12:59 stempy/pipeline/__init__.py
+-rw-rw-rw-  2.0 fat     1531 b- defN 23-May-31 13:09 stempy-3.3.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      492 b- defN 23-May-31 13:09 stempy-3.3.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       94 b- defN 23-May-31 13:09 stempy-3.3.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-May-31 13:09 stempy-3.3.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1265 b- defN 23-May-31 13:09 stempy-3.3.5.dist-info/RECORD
+16 files, 22006741 bytes uncompressed, 2004090 bytes compressed:  90.9%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: stempy/io/sparse_array.py
 Comment: 
 
 Filename: stempy/pipeline/__init__.py
 Comment: 
 
-Filename: stempy-3.3.4.dist-info/LICENSE
+Filename: stempy-3.3.5.dist-info/LICENSE
 Comment: 
 
-Filename: stempy-3.3.4.dist-info/METADATA
+Filename: stempy-3.3.5.dist-info/METADATA
 Comment: 
 
-Filename: stempy-3.3.4.dist-info/WHEEL
+Filename: stempy-3.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: stempy-3.3.4.dist-info/top_level.txt
+Filename: stempy-3.3.5.dist-info/top_level.txt
 Comment: 
 
-Filename: stempy-3.3.4.dist-info/RECORD
+Filename: stempy-3.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## stempy/stem.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800b7568
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri Apr 28 18:59:23 2023
+Time/Date		Wed May 31 13:09:01 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000000bb000
 SizeOfInitializedData	0000000000347000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000b7568
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		00407000
 SizeOfHeaders		00000400
-CheckSum		0040dd61
+CheckSum		00403c7c
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -488346,17 +488346,17 @@
    1800bfa40:	movabs 0x4000000001803f9d,%al
    1800bfa49:	sahf
    1800bfa4a:	(bad)
    1800bfa4b:	addb   $0x0,(%rcx)
    1800bfa4e:	add    %al,(%rax)
    1800bfa50:	add    %al,(%rax)
    1800bfa52:	add    %al,(%rax)
-   1800bfa54:	mov    (%rdi),%edx
-   1800bfa56:	rex.WR
-   1800bfa57:	add    %al,%fs:(%rax)
+   1800bfa54:	in     (%dx),%eax
+   1800bfa55:	rex.RX ja 0x1800bfabc
+   1800bfa58:	add    %al,(%rax)
    1800bfa5a:	add    %al,(%rax)
    1800bfa5c:	or     $0x3c000000,%eax
    1800bfa61:	add    (%rax),%eax
    1800bfa63:	add    %cl,(%rax)
    1800bfa65:	push   %rsp
    1800bfa66:	or     $0x0,%al
    1800bfa68:	or     %cl,0xc(%rax)
```

## Comparing `stempy-3.3.4.dist-info/LICENSE` & `stempy-3.3.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `stempy-3.3.4.dist-info/RECORD` & `stempy-3.3.5.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 stempy/__init__.py,sha256=_VjjuLPcMTN6QGnmO5lVHmjnso2xEangtTmAKf8c_Rk,101
-stempy/_image.cp39-win_amd64.pyd,sha256=EOt8LNHinVrsYU4iLTIEbxAggfD7P71KdCTqeqWdR74,265216
-stempy/_io.cp39-win_amd64.pyd,sha256=HcjwL1R89Aqyxw0zdt16IMI-Tp2umftV4NOvfJw_iGU,219648
-stempy/stem.dll,sha256=X4YkV2jgMGDnkKe5_JN4_8KLTJ1fZaHewqMnKysxUmo,4203520
+stempy/_image.cp39-win_amd64.pyd,sha256=wYAYXGx4APKWaB50POaQXb1bJjZflfy8xPsc-NqLwDk,265216
+stempy/_io.cp39-win_amd64.pyd,sha256=Tg1dw6PxlV8s42eobqxQprzKz6EU_VqOBRHzao5s71A,219648
+stempy/stem.dll,sha256=CSLCDbSA-hO6ZLAMvC_PKRwSbjbKml8reV4ts2ESzb0,4203520
 stempy/stem.lib,sha256=GM8D_bAFnblfvzIfIgl5U3xygcOQs1w0jZPAyFEFaNc,17225502
 stempy/utils.py,sha256=RA5c-GK8ha52ndNkqAuVb0Tlc5Wz1I4nPDl4L9kyXig,556
 stempy/image/__init__.py,sha256=SXmbboh6LhNnMtpibe4arNRLTqYMNkH9dF3k6lF_bmE,32699
 stempy/io/__init__.py,sha256=_SE1IX9YiG_Kcexn_YM0sdl8neQaa5WgBa5s8zEKA-A,10673
 stempy/io/compatibility.py,sha256=RGJi0mF_spY7UHqiLppNOsU7ZGDyezECsca0qt8DJ5k,3716
 stempy/io/sparse_array.py,sha256=OTZDCvLn8YzLb1SsKR-xsbu7K6pjgNxaii8KrfbhMNk,40225
 stempy/pipeline/__init__.py,sha256=w2GQTRx3uaHvI71Njq4LEej0O6NGERBAtpzxpovBLLU,1496
-stempy-3.3.4.dist-info/LICENSE,sha256=BcHyi7a5Tl01bzZ40boX0eUcrCSvk0ATYAs9P1C099E,1531
-stempy-3.3.4.dist-info/METADATA,sha256=BFymIoaXbI1z2gjoEuL1hryx8VQMHzJzuqHqv627oWw,492
-stempy-3.3.4.dist-info/WHEEL,sha256=w7c8R8EBcsIfULD7fwodEARLixQaQPkGy-B0R6IiyK8,94
-stempy-3.3.4.dist-info/top_level.txt,sha256=y781UigXVGwQbPQglCuxXrzVV_KW3zCDzfYZg-Fk_wE,7
-stempy-3.3.4.dist-info/RECORD,,
+stempy-3.3.5.dist-info/LICENSE,sha256=BcHyi7a5Tl01bzZ40boX0eUcrCSvk0ATYAs9P1C099E,1531
+stempy-3.3.5.dist-info/METADATA,sha256=XmF12ggbZc5qINkYJ9nyGrYS8iv7IMpiYFnBzTjuRV4,492
+stempy-3.3.5.dist-info/WHEEL,sha256=w7c8R8EBcsIfULD7fwodEARLixQaQPkGy-B0R6IiyK8,94
+stempy-3.3.5.dist-info/top_level.txt,sha256=y781UigXVGwQbPQglCuxXrzVV_KW3zCDzfYZg-Fk_wE,7
+stempy-3.3.5.dist-info/RECORD,,
```

