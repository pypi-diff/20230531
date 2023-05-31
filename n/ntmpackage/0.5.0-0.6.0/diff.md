# Comparing `tmp/ntmpackage-0.5.0.tar.gz` & `tmp/ntmpackage-0.6.0.tar.gz`

## Comparing `ntmpackage-0.5.0.tar` & `ntmpackage-0.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ntmpackage-0.5.0/.DS_Store
--rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 ntmpackage-0.5.0/ntmpackage/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ntmpackage-0.5.0/ntmpackage/__init__.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ntmpackage-0.5.0/ntmpackage/pkg_1/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ntmpackage-0.5.0/ntmpackage/pkg_1/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ntmpackage-0.5.0/ntmpackage/pkg_1/opt_fwk/__init__.py
--rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 ntmpackage-0.5.0/ntmpackage/pkg_1/opt_fwk/main1.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ntmpackage-0.5.0/ntmpackage/pkg_2/__init__.py
--rwxr-xr-x   0        0        0      115 2020-02-02 00:00:00.000000 ntmpackage-0.5.0/ntmpackage/pkg_2/main2.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 ntmpackage-0.5.0/LICENSE
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 ntmpackage-0.5.0/README.md
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 ntmpackage-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 ntmpackage-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/.DS_Store
+-rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/ntmpackage/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/ntmpackage/__init__.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/ntmpackage/pkg_1/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/ntmpackage/pkg_1/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/ntmpackage/pkg_1/opt_fwk/__init__.py
+-rwxr-xr-x   0        0        0      209 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/ntmpackage/pkg_1/opt_fwk/main1.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/ntmpackage/pkg_2/__init__.py
+-rwxr-xr-x   0        0        0      116 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/ntmpackage/pkg_2/main2.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/README.md
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 ntmpackage-0.6.0/PKG-INFO
```

### Comparing `ntmpackage-0.5.0/.DS_Store` & `ntmpackage-0.6.0/.DS_Store`

 * *Files 10% similar despite different names*

```diff
@@ -73,21 +73,21 @@
 00000480: 6e64 735b 5368 6f77 5369 6465 6261 7209  nds[ShowSidebar.
 00000490: 0909 095f 1019 7b7b 2d33 382c 2034 3035  ..._..{{-38, 405
 000004a0: 7d2c 207b 3133 3532 2c20 3533 397d 7d09  }, {1352, 539}}.
 000004b0: 0815 232f 3b52 5f6b 6c6d 6e6f 8b00 0000  ..#/;R_klmno....
 000004c0: 0000 0001 0100 0000 0000 0000 0d00 0000  ................
 000004d0: 0000 0000 0000 0000 0000 0000 8c00 0000  ................
 000004e0: 0400 6400 6900 7300 746c 6731 5363 6f6d  ..d.i.s.tlg1Scom
-000004f0: 7000 0000 0000 005d f800 0000 0400 6400  p......]......d.
+000004f0: 7000 0000 0000 0095 3700 0000 0400 6400  p.......7.....d.
 00000500: 6900 7300 746d 6f44 4462 6c6f 6200 0000  i.s.tmoDDblob...
-00000510: 0897 5904 26ba 13c5 4100 0000 0400 6400  ..Y.&...A.....d.
+00000510: 0829 9169 41c0 13c5 4100 0000 0400 6400  .).iA...A.....d.
 00000520: 6900 7300 746d 6f64 4462 6c6f 6200 0000  i.s.tmodDblob...
-00000530: 0897 5904 26ba 13c5 4100 0000 0400 6400  ..Y.&...A.....d.
+00000530: 0829 9169 41c0 13c5 4100 0000 0400 6400  .).iA...A.....d.
 00000540: 6900 7300 7470 6831 5363 6f6d 7000 0000  i.s.tph1Scomp...
-00000550: 0000 0080 0000 0000 0400 6400 6900 7300  ..........d.i.s.
+00000550: 0000 00d0 0000 0000 0400 6400 6900 7300  ..........d.i.s.
 00000560: 7476 5372 6e6c 6f6e 6700 0000 0100 0000  tvSrnlong.......
 00000570: 0a00 6e00 7400 6d00 7000 6100 6300 6b00  ..n.t.m.p.a.c.k.
 00000580: 6100 6700 6562 7773 7062 6c6f 6200 0000  a.g.ebwspblob...
 00000590: b962 706c 6973 7430 30d6 0102 0304 0506  .bplist00.......
 000005a0: 0707 0707 0b07 5d53 686f 7753 7461 7475  ......]ShowStatu
 000005b0: 7342 6172 5b53 686f 7754 6f6f 6c62 6172  sBar[ShowToolbar
 000005c0: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
```

### Comparing `ntmpackage-0.5.0/ntmpackage/.DS_Store` & `ntmpackage-0.6.0/ntmpackage/.DS_Store`

 * *Files identical despite different names*

### Comparing `ntmpackage-0.5.0/ntmpackage/pkg_1/.DS_Store` & `ntmpackage-0.6.0/ntmpackage/pkg_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `ntmpackage-0.5.0/LICENSE` & `ntmpackage-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ntmpackage-0.5.0/README.md` & `ntmpackage-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ntmpackage-0.5.0/pyproject.toml` & `ntmpackage-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ntmpackage"
-version = "0.5.0"
+version = "0.6.0"
 authors = [
   { name="Nara Torres Moreira", email="nara.moreira@astrazeneca.com" },
 ]
 description = "Nara's first package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ntmpackage-0.5.0/PKG-INFO` & `ntmpackage-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntmpackage
-Version: 0.5.0
+Version: 0.6.0
 Summary: Nara's first package
 Project-URL: Homepage, https://github.com/AZ-AI/opt-tools
 Author-email: Nara Torres Moreira <nara.moreira@astrazeneca.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

