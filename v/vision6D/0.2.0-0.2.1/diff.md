# Comparing `tmp/vision6D-0.2.0.tar.gz` & `tmp/vision6D-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision6D-0.2.0.tar", last modified: Tue May 30 19:32:55 2023, max compression
+gzip compressed data, was "vision6D-0.2.1.tar", last modified: Wed May 31 20:33:00 2023, max compression
```

## Comparing `vision6D-0.2.0.tar` & `vision6D-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 19:32:55.380729 vision6D-0.2.0/
--rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1545 2023-05-30 19:32:55.381729 vision6D-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      858 2023-05-30 19:21:58.000000 vision6D-0.2.0/README.md
--rw-rw-rw-   0        0        0      406 2023-05-30 19:17:57.000000 vision6D-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0     1923 2023-05-30 19:32:55.387726 vision6D-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      282 2023-05-30 19:29:49.000000 vision6D-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 19:32:55.153591 vision6D-0.2.0/test/
--rw-rw-rw-   0        0        0    21974 2023-05-17 18:41:02.000000 vision6D-0.2.0/test/test_create_dataset.py
--rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.2.0/test/test_projection.py
-drwxrwxrwx   0        0        0        0 2023-05-30 19:32:55.235593 vision6D-0.2.0/vision6D/
--rw-rw-rw-   0        0        0    51597 2023-05-29 23:53:36.000000 vision6D-0.2.0/vision6D/GUI.py
--rw-rw-rw-   0        0        0      913 2023-05-30 19:29:28.000000 vision6D-0.2.0/vision6D/__init__.py
--rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.2.0/vision6D/app.py
--rw-rw-rw-   0        0        0    12369 2023-05-28 01:21:42.000000 vision6D-0.2.0/vision6D/config.py
-drwxrwxrwx   0        0        0        0 2023-05-30 19:32:55.376729 vision6D-0.2.0/vision6D/data/
--rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.2.0/vision6D/data/ossiclesCoordinateMapping.json
--rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.2.0/vision6D/data/ossiclesCoordinateMappingv1.json
--rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.2.0/vision6D/data/style.qss
--rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.2.0/vision6D/interface.py
--rw-rw-rw-   0        0        0    26253 2023-05-29 23:38:16.000000 vision6D-0.2.0/vision6D/interface_gui.py
--rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.2.0/vision6D/mainwindow.py
--rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.2.0/vision6D/run_gui.py
--rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.2.0/vision6D/run_interface.py
--rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.2.0/vision6D/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-30 19:32:55.304720 vision6D-0.2.0/vision6D.egg-info/
--rw-rw-rw-   0        0        0     1545 2023-05-30 19:32:54.000000 vision6D-0.2.0/vision6D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      632 2023-05-30 19:32:55.000000 vision6D-0.2.0/vision6D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 19:32:54.000000 vision6D-0.2.0/vision6D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-30 19:32:54.000000 vision6D-0.2.0/vision6D.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      164 2023-05-30 19:32:54.000000 vision6D-0.2.0/vision6D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 19:32:54.000000 vision6D-0.2.0/vision6D.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 20:33:00.511785 vision6D-0.2.1/
+-rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1545 2023-05-31 20:33:00.512784 vision6D-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      858 2023-05-30 22:42:04.000000 vision6D-0.2.1/README.md
+-rw-rw-rw-   0        0        0      406 2023-05-30 22:42:04.000000 vision6D-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0     2043 2023-05-31 20:33:00.517783 vision6D-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      282 2023-05-30 22:42:04.000000 vision6D-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 20:33:00.301779 vision6D-0.2.1/test/
+-rw-rw-rw-   0        0        0    21817 2023-05-30 22:26:10.000000 vision6D-0.2.1/test/test_create_dataset.py
+-rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.2.1/test/test_projection.py
+drwxrwxrwx   0        0        0        0 2023-05-31 20:33:00.401782 vision6D-0.2.1/vision6D/
+-rw-rw-rw-   0        0        0    51735 2023-05-30 22:49:40.000000 vision6D-0.2.1/vision6D/GUI.py
+-rw-rw-rw-   0        0        0      913 2023-05-30 22:42:04.000000 vision6D-0.2.1/vision6D/__init__.py
+-rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.2.1/vision6D/app.py
+-rw-rw-rw-   0        0        0    12369 2023-05-30 22:42:04.000000 vision6D-0.2.1/vision6D/config.py
+drwxrwxrwx   0        0        0        0 2023-05-31 20:33:00.504783 vision6D-0.2.1/vision6D/data/
+-rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.2.1/vision6D/data/ossiclesCoordinateMapping.json
+-rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.2.1/vision6D/data/ossiclesCoordinateMappingv1.json
+-rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.2.1/vision6D/data/style.qss
+-rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.2.1/vision6D/interface.py
+-rw-rw-rw-   0        0        0    26253 2023-05-30 22:42:04.000000 vision6D-0.2.1/vision6D/interface_gui.py
+-rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.2.1/vision6D/mainwindow.py
+-rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.2.1/vision6D/run_gui.py
+-rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.2.1/vision6D/run_interface.py
+-rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.2.1/vision6D/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-31 20:33:00.450783 vision6D-0.2.1/vision6D.egg-info/
+-rw-rw-rw-   0        0        0     1545 2023-05-31 20:32:59.000000 vision6D-0.2.1/vision6D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      632 2023-05-31 20:33:00.000000 vision6D-0.2.1/vision6D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 20:32:59.000000 vision6D-0.2.1/vision6D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-31 20:32:59.000000 vision6D-0.2.1/vision6D.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      284 2023-05-31 20:32:59.000000 vision6D-0.2.1/vision6D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-31 20:33:00.000000 vision6D-0.2.1/vision6D.egg-info/top_level.txt
```

### Comparing `vision6D-0.2.0/LICENSE` & `vision6D-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.0/PKG-INFO` & `vision6D-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.2.0
+Version: 0.2.1
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: 6D poes estimation,registration,segmentation
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.2.0/README.md` & `vision6D-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.0/setup.cfg` & `vision6D-0.2.1/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6973 696f 6e36 440d 0a76 6572   = vision6D..ver
-00000020: 7369 6f6e 203d 2030 2e32 2e30 0d0a 7572  sion = 0.2.0..ur
+00000020: 7369 6f6e 203d 2030 2e32 2e31 0d0a 7572  sion = 0.2.1..ur
 00000030: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000040: 7562 2e63 6f6d 2f79 6b7a 7a6b 792f 7669  ub.com/ykzzky/vi
 00000050: 7369 6f6e 3644 0d0a 6465 7363 7269 7074  sion6D..descript
 00000060: 696f 6e20 3d20 7669 7369 6f6e 3644 3a20  ion = vision6D: 
 00000070: 4120 746f 6f6c 2066 6f72 2036 4420 706f  A tool for 6D po
 00000080: 7365 2065 7374 696d 6174 696f 6e20 616e  se estimation an
 00000090: 6e6f 7461 7469 6f6e 0d0a 6c6f 6e67 5f64  notation..long_d
@@ -44,78 +44,85 @@
 000002b0: 7461 203d 2074 7275 650d 0a70 7974 686f  ta = true..pytho
 000002c0: 6e5f 7265 7175 6972 6573 203d 203e 3d20  n_requires = >= 
 000002d0: 332e 360d 0a74 6573 745f 7375 6974 6520  3.6..test_suite 
 000002e0: 3d20 7465 7374 730d 0a73 6574 7570 5f72  = tests..setup_r
 000002f0: 6571 7569 7265 7320 3d20 0d0a 0973 6574  equires = ...set
 00000300: 7570 746f 6f6c 730d 0a69 6e73 7461 6c6c  uptools..install
 00000310: 5f72 6571 7569 7265 7320 3d20 0d0a 0970  _requires = ...p
-00000320: 7976 6973 7461 0d0a 096e 756d 7079 0d0a  yvista...numpy..
-00000330: 096d 6174 706c 6f74 6c69 620d 0a09 7472  .matplotlib...tr
-00000340: 696d 6573 680d 0a09 6561 7379 6469 6374  imesh...easydict
-00000350: 0d0a 0970 696c 6c6f 770d 0a09 7363 6970  ...pillow...scip
-00000360: 790d 0a09 7079 7465 7374 0d0a 0970 7974  y...pytest...pyt
-00000370: 6573 742d 6c61 7a79 2d66 6978 7475 7265  est-lazy-fixture
-00000380: 0d0a 0970 7265 2d63 6f6d 6d69 740d 0a09  ...pre-commit...
-00000390: 6f70 656e 6376 2d70 7974 686f 6e2d 6865  opencv-python-he
-000003a0: 6164 6c65 7373 0d0a 0973 6369 6b69 742d  adless...scikit-
-000003b0: 696d 6167 650d 0a09 6368 6172 6465 740d  image...chardet.
-000003c0: 0a09 7079 6765 6f64 6573 6963 0d0a 0950  ..pygeodesic...P
-000003d0: 7951 7435 0d0a 0970 7976 6973 7461 7174  yQt5...pyvistaqt
-000003e0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-000003f0: 6b61 6765 5f64 6174 615d 0d0a 2a20 3d20  kage_data]..* = 
-00000400: 2a2e 706e 672c 202a 2e6a 7067 2c20 2a2e  *.png, *.jpg, *.
-00000410: 716d 6c0d 0a0d 0a5b 6264 6973 745f 7768  qml....[bdist_wh
-00000420: 6565 6c5d 0d0a 756e 6976 6572 7361 6c20  eel]..universal 
-00000430: 3d20 7472 7565 0d0a 0d0a 5b73 6469 7374  = true....[sdist
-00000440: 5d0d 0a66 6f72 6d61 7473 203d 207a 6970  ]..formats = zip
-00000450: 2c20 677a 7461 720d 0a0d 0a5b 636f 7665  , gztar....[cove
-00000460: 7261 6765 3a72 6570 6f72 745d 0d0a 7368  rage:report]..sh
-00000470: 6f77 5f6d 6973 7369 6e67 203d 2074 7275  ow_missing = tru
-00000480: 650d 0a65 7863 6c75 6465 5f6c 696e 6573  e..exclude_lines
-00000490: 203d 200d 0a09 7072 6167 6d61 3a20 6e6f   = ...pragma: no
-000004a0: 2063 6f76 6572 0d0a 0969 6620 4661 6c73   cover...if Fals
-000004b0: 650d 0a0d 0a5b 6772 6565 6e5d 0d0a 6669  e....[green]..fi
-000004c0: 6c65 2d70 6174 7465 726e 203d 2074 6573  le-pattern = tes
-000004d0: 745f 2a2e 7079 0d0a 7665 7262 6f73 6520  t_*.py..verbose 
-000004e0: 3d20 320d 0a6e 6f2d 736b 6970 2d72 6570  = 2..no-skip-rep
-000004f0: 6f72 7420 3d20 7472 7565 0d0a 7175 6965  ort = true..quie
-00000500: 742d 7374 646f 7574 203d 2074 7275 650d  t-stdout = true.
-00000510: 0a72 756e 2d63 6f76 6572 6167 6520 3d20  .run-coverage = 
-00000520: 7472 7565 0d0a 0d0a 5b70 7964 6f63 7374  true....[pydocst
-00000530: 796c 655d 0d0a 6d61 7463 682d 6469 7220  yle]..match-dir 
-00000540: 3d20 283f 2174 6573 7473 2928 3f21 7265  = (?!tests)(?!re
-00000550: 736f 7572 6365 7329 283f 2164 6f63 7329  sources)(?!docs)
-00000560: 5b5e 5c2e 5d2e 2a0d 0a6d 6174 6368 203d  [^\.].*..match =
-00000570: 2028 3f21 7465 7374 2928 3f21 7365 7475   (?!test)(?!setu
-00000580: 7029 5b5e 5c2e 5f5d 2e2a 5c2e 7079 0d0a  p)[^\._].*\.py..
-00000590: 696e 6865 7269 7420 3d20 6661 6c73 650d  inherit = false.
-000005a0: 0a69 676e 6f72 6520 3d20 4432 3030 2c20  .ignore = D200, 
-000005b0: 4432 3033 2c20 4432 3133 2c20 4434 3036  D203, D213, D406
-000005c0: 2c20 4434 3037 0d0a 0d0a 5b66 6c61 6b65  , D407....[flake
-000005d0: 385d 0d0a 6d61 782d 6c69 6e65 2d6c 656e  8]..max-line-len
-000005e0: 6774 6820 3d20 3939 0d0a 646f 6374 6573  gth = 99..doctes
-000005f0: 7473 203d 2054 7275 650d 0a65 7863 6c75  ts = True..exclu
-00000600: 6465 203d 202e 6769 742c 202e 6567 6773  de = .git, .eggs
-00000610: 2c20 5f5f 7079 6361 6368 655f 5f2c 2074  , __pycache__, t
-00000620: 6573 7473 2f2c 2064 6f63 732f 2c20 6275  ests/, docs/, bu
-00000630: 696c 642f 2c20 6469 7374 2f0d 0a0d 0a5b  ild/, dist/....[
-00000640: 6d79 7079 5d0d 0a64 6973 616c 6c6f 775f  mypy]..disallow_
-00000650: 616e 795f 6465 636f 7261 7465 6420 3d20  any_decorated = 
-00000660: 7472 7565 0d0a 6469 7361 6c6c 6f77 5f61  true..disallow_a
-00000670: 6e79 5f67 656e 6572 6963 7320 3d20 7472  ny_generics = tr
-00000680: 7565 0d0a 6469 7361 6c6c 6f77 5f61 6e79  ue..disallow_any
-00000690: 5f75 6e69 6d70 6f72 7465 6420 3d20 6661  _unimported = fa
-000006a0: 6c73 650d 0a64 6973 616c 6c6f 775f 7375  lse..disallow_su
-000006b0: 6263 6c61 7373 696e 675f 616e 7920 3d20  bclassing_any = 
-000006c0: 6661 6c73 650d 0a64 6973 616c 6c6f 775f  false..disallow_
-000006d0: 756e 7479 7065 645f 6361 6c6c 7320 3d20  untyped_calls = 
-000006e0: 7472 7565 0d0a 6469 7361 6c6c 6f77 5f75  true..disallow_u
-000006f0: 6e74 7970 6564 5f64 6566 7320 3d20 7472  ntyped_defs = tr
-00000700: 7565 0d0a 6967 6e6f 7265 5f6d 6973 7369  ue..ignore_missi
-00000710: 6e67 5f69 6d70 6f72 7473 203d 2074 7275  ng_imports = tru
-00000720: 650d 0a77 6172 6e5f 756e 7573 6564 5f69  e..warn_unused_i
-00000730: 676e 6f72 6573 203d 2074 7275 650d 0a77  gnores = true..w
-00000740: 6172 6e5f 7265 7475 726e 5f61 6e79 203d  arn_return_any =
-00000750: 2074 7275 650d 0a0d 0a5b 6567 675f 696e   true....[egg_in
-00000760: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-00000770: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-00000780: 0a0d 0a                                  ...
+00000320: 7976 6973 7461 3e3d 302e 3339 2e31 0d0a  yvista>=0.39.1..
+00000330: 096e 756d 7079 3e3d 312e 3233 2e35 0d0a  .numpy>=1.23.5..
+00000340: 096d 6174 706c 6f74 6c69 623e 3d33 2e35  .matplotlib>=3.5
+00000350: 2e32 0d0a 0974 7269 6d65 7368 3e3d 332e  .2...trimesh>=3.
+00000360: 3134 2e30 0d0a 0965 6173 7964 6963 743e  14.0...easydict>
+00000370: 3d31 2e39 0d0a 0970 696c 6c6f 773e 3d39  =1.9...pillow>=9
+00000380: 2e32 2e30 0d0a 0973 6369 7079 3e3d 312e  .2.0...scipy>=1.
+00000390: 382e 310d 0a09 7079 7465 7374 3e3d 372e  8.1...pytest>=7.
+000003a0: 322e 300d 0a09 7079 7465 7374 2d6c 617a  2.0...pytest-laz
+000003b0: 792d 6669 7874 7572 653e 3d30 2e36 2e33  y-fixture>=0.6.3
+000003c0: 0d0a 0970 7265 2d63 6f6d 6d69 743e 3d32  ...pre-commit>=2
+000003d0: 2e32 312e 300d 0a09 6f70 656e 6376 2d70  .21.0...opencv-p
+000003e0: 7974 686f 6e2d 6865 6164 6c65 7373 3e3d  ython-headless>=
+000003f0: 342e 372e 302e 3638 0d0a 0973 6369 6b69  4.7.0.68...sciki
+00000400: 742d 696d 6167 653e 3d30 2e31 392e 330d  t-image>=0.19.3.
+00000410: 0a09 6368 6172 6465 743e 3d35 2e31 2e30  ..chardet>=5.1.0
+00000420: 0d0a 0970 7967 656f 6465 7369 633e 3d30  ...pygeodesic>=0
+00000430: 2e31 2e38 0d0a 0950 7951 7435 3e3d 352e  .1.8...PyQt5>=5.
+00000440: 3135 2e39 0d0a 0970 7976 6973 7461 7174  15.9...pyvistaqt
+00000450: 3e3d 302e 3130 2e30 0d0a 0d0a 5b6f 7074  >=0.10.0....[opt
+00000460: 696f 6e73 2e70 6163 6b61 6765 5f64 6174  ions.package_dat
+00000470: 615d 0d0a 2a20 3d20 2a2e 706e 672c 202a  a]..* = *.png, *
+00000480: 2e6a 7067 2c20 2a2e 716d 6c0d 0a0d 0a5b  .jpg, *.qml....[
+00000490: 6264 6973 745f 7768 6565 6c5d 0d0a 756e  bdist_wheel]..un
+000004a0: 6976 6572 7361 6c20 3d20 7472 7565 0d0a  iversal = true..
+000004b0: 0d0a 5b73 6469 7374 5d0d 0a66 6f72 6d61  ..[sdist]..forma
+000004c0: 7473 203d 207a 6970 2c20 677a 7461 720d  ts = zip, gztar.
+000004d0: 0a0d 0a5b 636f 7665 7261 6765 3a72 6570  ...[coverage:rep
+000004e0: 6f72 745d 0d0a 7368 6f77 5f6d 6973 7369  ort]..show_missi
+000004f0: 6e67 203d 2074 7275 650d 0a65 7863 6c75  ng = true..exclu
+00000500: 6465 5f6c 696e 6573 203d 200d 0a09 7072  de_lines = ...pr
+00000510: 6167 6d61 3a20 6e6f 2063 6f76 6572 0d0a  agma: no cover..
+00000520: 0969 6620 4661 6c73 650d 0a0d 0a5b 6772  .if False....[gr
+00000530: 6565 6e5d 0d0a 6669 6c65 2d70 6174 7465  een]..file-patte
+00000540: 726e 203d 2074 6573 745f 2a2e 7079 0d0a  rn = test_*.py..
+00000550: 7665 7262 6f73 6520 3d20 320d 0a6e 6f2d  verbose = 2..no-
+00000560: 736b 6970 2d72 6570 6f72 7420 3d20 7472  skip-report = tr
+00000570: 7565 0d0a 7175 6965 742d 7374 646f 7574  ue..quiet-stdout
+00000580: 203d 2074 7275 650d 0a72 756e 2d63 6f76   = true..run-cov
+00000590: 6572 6167 6520 3d20 7472 7565 0d0a 0d0a  erage = true....
+000005a0: 5b70 7964 6f63 7374 796c 655d 0d0a 6d61  [pydocstyle]..ma
+000005b0: 7463 682d 6469 7220 3d20 283f 2174 6573  tch-dir = (?!tes
+000005c0: 7473 2928 3f21 7265 736f 7572 6365 7329  ts)(?!resources)
+000005d0: 283f 2164 6f63 7329 5b5e 5c2e 5d2e 2a0d  (?!docs)[^\.].*.
+000005e0: 0a6d 6174 6368 203d 2028 3f21 7465 7374  .match = (?!test
+000005f0: 2928 3f21 7365 7475 7029 5b5e 5c2e 5f5d  )(?!setup)[^\._]
+00000600: 2e2a 5c2e 7079 0d0a 696e 6865 7269 7420  .*\.py..inherit 
+00000610: 3d20 6661 6c73 650d 0a69 676e 6f72 6520  = false..ignore 
+00000620: 3d20 4432 3030 2c20 4432 3033 2c20 4432  = D200, D203, D2
+00000630: 3133 2c20 4434 3036 2c20 4434 3037 0d0a  13, D406, D407..
+00000640: 0d0a 5b66 6c61 6b65 385d 0d0a 6d61 782d  ..[flake8]..max-
+00000650: 6c69 6e65 2d6c 656e 6774 6820 3d20 3939  line-length = 99
+00000660: 0d0a 646f 6374 6573 7473 203d 2054 7275  ..doctests = Tru
+00000670: 650d 0a65 7863 6c75 6465 203d 202e 6769  e..exclude = .gi
+00000680: 742c 202e 6567 6773 2c20 5f5f 7079 6361  t, .eggs, __pyca
+00000690: 6368 655f 5f2c 2074 6573 7473 2f2c 2064  che__, tests/, d
+000006a0: 6f63 732f 2c20 6275 696c 642f 2c20 6469  ocs/, build/, di
+000006b0: 7374 2f0d 0a0d 0a5b 6d79 7079 5d0d 0a64  st/....[mypy]..d
+000006c0: 6973 616c 6c6f 775f 616e 795f 6465 636f  isallow_any_deco
+000006d0: 7261 7465 6420 3d20 7472 7565 0d0a 6469  rated = true..di
+000006e0: 7361 6c6c 6f77 5f61 6e79 5f67 656e 6572  sallow_any_gener
+000006f0: 6963 7320 3d20 7472 7565 0d0a 6469 7361  ics = true..disa
+00000700: 6c6c 6f77 5f61 6e79 5f75 6e69 6d70 6f72  llow_any_unimpor
+00000710: 7465 6420 3d20 6661 6c73 650d 0a64 6973  ted = false..dis
+00000720: 616c 6c6f 775f 7375 6263 6c61 7373 696e  allow_subclassin
+00000730: 675f 616e 7920 3d20 6661 6c73 650d 0a64  g_any = false..d
+00000740: 6973 616c 6c6f 775f 756e 7479 7065 645f  isallow_untyped_
+00000750: 6361 6c6c 7320 3d20 7472 7565 0d0a 6469  calls = true..di
+00000760: 7361 6c6c 6f77 5f75 6e74 7970 6564 5f64  sallow_untyped_d
+00000770: 6566 7320 3d20 7472 7565 0d0a 6967 6e6f  efs = true..igno
+00000780: 7265 5f6d 6973 7369 6e67 5f69 6d70 6f72  re_missing_impor
+00000790: 7473 203d 2074 7275 650d 0a77 6172 6e5f  ts = true..warn_
+000007a0: 756e 7573 6564 5f69 676e 6f72 6573 203d  unused_ignores =
+000007b0: 2074 7275 650d 0a77 6172 6e5f 7265 7475   true..warn_retu
+000007c0: 726e 5f61 6e79 203d 2074 7275 650d 0a0d  rn_any = true...
+000007d0: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
+000007e0: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
+000007f0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
```

### Comparing `vision6D-0.2.0/test/test_create_dataset.py` & `vision6D-0.2.1/test/test_create_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -387,20 +387,16 @@
         #     if (pt != [0, 0, 0]).all():
         #         lst.append(i)
         #         pts3d.append(pt)
 
         # pts2d = pts2d[lst]
         pts3d = np.array(pts3d).reshape((len(pts3d), 3))
 
-        pts2d = pts2d.astype('float32')
-        pts3d = pts3d.astype('float32')
-        camera_intrinsics = app.camera_intrinsics.astype('float32')
-        
         # use EPNP to predict the pose
-        predicted_pose = vis.utils.solve_epnp_cv2(pts2d, pts3d, camera_intrinsics, app.camera.position)
+        predicted_pose = vis.utils.solve_epnp_cv2(pts2d, pts3d, app.camera_intrinsics, app.camera.position)
         logger.debug(f"\ndifference from predicted pose and RT pose: {np.sum(np.abs(predicted_pose - RT))}")
         assert np.isclose(predicted_pose, RT, atol=20).all()
 
         # use P3P
         # success, rotation_vector, translation_vector = cv2.solvePnP(pts3d, pts2d, camera_intrinsics, distCoeffs=np.zeros((4, 1)), flags=cv2.SOLVEPNP_P3P)
         # if success:
         #     predicted_pose = np.eye(4)
```

### Comparing `vision6D-0.2.0/test/test_projection.py` & `vision6D-0.2.1/test/test_projection.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.0/vision6D/GUI.py` & `vision6D-0.2.1/vision6D/GUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -455,14 +455,16 @@
                     self.add_mesh(actor_name, self.meshdict[actor_name])
         else:
             QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
 
     def add_workspace(self):
         workspace_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.json)")
         if workspace_path != '':
+            # Clear the plot automatically if loading a new workspace
+            self.clear_plot()
             self.hintLabel.hide()
             with open(str(workspace_path), 'r') as f: 
                 workspace = json.load(f)
 
             self.image_path = workspace['image_path']
             self.mask_path = workspace['mask_path']
             self.pose_path = workspace['pose_path']
@@ -642,14 +644,16 @@
         self.used_colors = []
         self.color_button.setText("Color")
 
         self.ignore_slider_value_change = True
         self.opacity_slider.setValue(100)
         self.ignore_slider_value_change = False
 
+        self.clear_output_text()
+
     def render_image(self, actor, camera):
         self.render.clear()
         render_actor = actor.copy(deep=True)
         render_actor.GetProperty().opacity = 1
         self.render.add_actor(render_actor, pickable=False)
         self.render.camera = camera
         self.render.disable()
```

### Comparing `vision6D-0.2.0/vision6D/__init__.py` & `vision6D-0.2.1/vision6D/__init__.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.0/vision6D/app.py` & `vision6D-0.2.1/vision6D/app.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.0/vision6D/config.py` & `vision6D-0.2.1/vision6D/config.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.0/vision6D/data/ossiclesCoordinateMapping.json` & `vision6D-0.2.1/vision6D/data/ossiclesCoordinateMapping.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.0/vision6D/data/ossiclesCoordinateMappingv1.json` & `vision6D-0.2.1/vision6D/data/ossiclesCoordinateMappingv1.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.0/vision6D/data/style.qss` & `vision6D-0.2.1/vision6D/data/style.qss`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.0/vision6D/interface.py` & `vision6D-0.2.1/vision6D/interface.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.0/vision6D/interface_gui.py` & `vision6D-0.2.1/vision6D/interface_gui.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.0/vision6D/mainwindow.py` & `vision6D-0.2.1/vision6D/mainwindow.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.0/vision6D/run_gui.py` & `vision6D-0.2.1/vision6D/run_gui.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.0/vision6D/utils.py` & `vision6D-0.2.1/vision6D/utils.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.0/vision6D.egg-info/PKG-INFO` & `vision6D-0.2.1/vision6D.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.2.0
+Version: 0.2.1
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: 6D poes estimation,registration,segmentation
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.2.0/vision6D.egg-info/SOURCES.txt` & `vision6D-0.2.1/vision6D.egg-info/SOURCES.txt`

 * *Files identical despite different names*

