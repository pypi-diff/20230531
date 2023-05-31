# Comparing `tmp/gulagcleaner-0.4.8.tar.gz` & `tmp/gulagcleaner-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gulagcleaner-0.4.8.tar", last modified: Sun Feb 12 17:52:21 2023, max compression
+gzip compressed data, was "gulagcleaner-0.5.0.tar", last modified: Wed May 31 21:34:32 2023, max compression
```

## Comparing `gulagcleaner-0.4.8.tar` & `gulagcleaner-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-02-12 17:52:21.257393 gulagcleaner-0.4.8/
--rw-rw-rw-   0        0        0    71644 2023-02-12 15:01:11.000000 gulagcleaner-0.4.8/LICENSE
--rw-rw-rw-   0        0        0     1419 2023-02-12 17:52:21.257393 gulagcleaner-0.4.8/PKG-INFO
--rw-rw-rw-   0        0        0      806 2023-02-12 15:26:20.000000 gulagcleaner-0.4.8/README.md
-drwxrwxrwx   0        0        0        0 2023-02-12 17:52:21.226142 gulagcleaner-0.4.8/gulagcleaner/
--rw-rw-rw-   0        0        0        0 2023-02-12 15:01:11.000000 gulagcleaner-0.4.8/gulagcleaner/__init__.py
--rw-rw-rw-   0        0        0     2423 2023-02-12 17:49:52.000000 gulagcleaner-0.4.8/gulagcleaner/command_line.py
--rw-rw-rw-   0        0        0     3595 2023-02-12 17:47:32.000000 gulagcleaner-0.4.8/gulagcleaner/gulagcleaner_extract.py
-drwxrwxrwx   0        0        0        0 2023-02-12 17:52:21.257393 gulagcleaner-0.4.8/gulagcleaner.egg-info/
--rw-rw-rw-   0        0        0     1419 2023-02-12 17:52:21.000000 gulagcleaner-0.4.8/gulagcleaner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-02-12 17:52:21.000000 gulagcleaner-0.4.8/gulagcleaner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-12 17:52:21.000000 gulagcleaner-0.4.8/gulagcleaner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-02-12 17:52:21.000000 gulagcleaner-0.4.8/gulagcleaner.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2023-02-12 17:52:21.000000 gulagcleaner-0.4.8/gulagcleaner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-02-12 17:52:21.000000 gulagcleaner-0.4.8/gulagcleaner.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-02-12 15:01:11.000000 gulagcleaner-0.4.8/pyproject.toml
--rw-rw-rw-   0        0        0      905 2023-02-12 17:52:21.257393 gulagcleaner-0.4.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-31 21:34:32.593029 gulagcleaner-0.5.0/
+-rw-rw-rw-   0        0        0    71644 2023-02-12 15:01:11.000000 gulagcleaner-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     2437 2023-05-31 21:34:32.593091 gulagcleaner-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1870 2023-05-31 21:24:37.000000 gulagcleaner-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 21:34:32.564420 gulagcleaner-0.5.0/gulagcleaner/
+-rw-rw-rw-   0        0        0        0 2023-02-12 15:01:11.000000 gulagcleaner-0.5.0/gulagcleaner/__init__.py
+-rw-rw-rw-   0        0        0     2757 2023-05-31 21:16:23.000000 gulagcleaner-0.5.0/gulagcleaner/command_line.py
+-rw-rw-rw-   0        0        0     5886 2023-05-31 21:17:33.000000 gulagcleaner-0.5.0/gulagcleaner/gulagcleaner_extract.py
+drwxrwxrwx   0        0        0        0 2023-05-31 21:34:32.590421 gulagcleaner-0.5.0/gulagcleaner.egg-info/
+-rw-rw-rw-   0        0        0     2437 2023-05-31 21:34:32.000000 gulagcleaner-0.5.0/gulagcleaner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-05-31 21:34:32.000000 gulagcleaner-0.5.0/gulagcleaner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 21:34:32.000000 gulagcleaner-0.5.0/gulagcleaner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-05-31 21:34:32.000000 gulagcleaner-0.5.0/gulagcleaner.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2023-05-31 21:34:32.000000 gulagcleaner-0.5.0/gulagcleaner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-31 21:34:32.000000 gulagcleaner-0.5.0/gulagcleaner.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-02-12 15:01:11.000000 gulagcleaner-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0      857 2023-05-31 21:34:32.600419 gulagcleaner-0.5.0/setup.cfg
```

### Comparing `gulagcleaner-0.4.8/LICENSE` & `gulagcleaner-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gulagcleaner-0.4.8/gulagcleaner/command_line.py` & `gulagcleaner-0.5.0/gulagcleaner/command_line.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,55 +6,64 @@
     Main function for the "gulagcleaner" CLI command.
 
     The "gulagcleaner" command takes an argument for the path of a PDF file and tries to deembed the pages inside it. The pages are saved in a new PDF in the same folder.
     
     Available CLI arguments:
     -h : displays help information
     -r : replaces the original file with the deembedded file
+    -o : uses the old deembeding method (for files older than 18/05/2023)
     -v : displays the version of the program
+
     '''
     import sys
     import os.path
 
     # Check for the -h argument
     if '-h' in sys.argv:
-        print("Usage: gulagcleaner [-h] [-r] [-v] <filename>")
+        print("Usage: gulagcleaner [-h] [-r] [-o] [-v] <filename>")
         print("")
-        print("Deembeds pages from a PDF file")
+        print("Deembeds pages from a PDF file.")
         print("")
         print("Positional arguments:")
-        print("  filename      the PDF file to deembed pages from")
+        print("  filename      the PDF file to deembed pages from.")
         print("")
         print("Optional arguments:")
-        print("  -h            show this help message and exit")
-        print("  -r            replaces the original file with the deembedded file")
-        print("  -v            shows the version of the program")
+        print("  -h            show this help message and exit.")
+        print("  -r            replaces the original file with the deembedded file.")
+        print("  -o            uses the old deembeding method (for files older than 18/05/2023).")
+        print("  -v            shows the version of the program.")
         return
 
     # Check for the -v argument
     if '-v' in sys.argv:
-        print("actual version: 0.4.8")
+        print("actual version: 0.5.0")
         return
 
     # Get the filename argument
     if len(sys.argv) < 2:
-        print('Usage: gulagcleaner [-h] [-r] [-v] <filename>')
+        print('Usage: gulagcleaner [-h] [-r] [-o] [-v] <filename>')
         return
     filename = sys.argv[-1]
 
     # Check if the file exists
     if not os.path.exists(filename):
         print("File not found.")
         return
 
     # Check if the -r argument is present
     replace = '-r' in sys.argv
 
+     # Check if the -o argument is present
+    if '-o' in sys.argv:
+        method = "old"
+    else:
+        method = "new"
+    
     # Call the deembed function
-    return_msg = gulagcleaner_extract.deembed(filename, replace)
+    return_msg = gulagcleaner_extract.deembed(filename, replace,method)
     if return_msg["Success"]:
         print("Deembedding successful. File saved in", return_msg["return_path"])
         print("Metadata:")
         print("Archivo: " + return_msg["Meta"]["Archivo"])
         print("Autor: " + return_msg["Meta"]["Autor"])
         print("Asignatura: " + return_msg["Meta"]["Asignatura"])
         print("Curso y Grado: " + return_msg["Meta"]["Curso y Grado"])
```

### Comparing `gulagcleaner-0.4.8/setup.cfg` & `gulagcleaner-0.5.0/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,54 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 756c 6167 636c 6561 6e65 720d   = gulagcleaner.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e34 2e38  .version = 0.4.8
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e35 2e30  .version = 0.5.0
 00000030: 0d0a 6175 7468 6f72 203d 2059 4d31 3632  ..author = YM162
 00000040: 2c4b 6f73 6d69 634b 6174 5856 2c70 6761  ,KosmicKatXV,pga
 00000050: 6c69 6e61 6e65 730d 0a61 7574 686f 725f  linanes..author_
 00000060: 656d 6169 6c20 3d20 6461 7669 642e 666f  email = david.fo
-00000070: 6e74 616e 6564 6140 6573 7475 6469 616e  ntaneda@estudian
-00000080: 7465 2e75 616d 2e65 730d 0a64 6573 6372  te.uam.es..descr
-00000090: 6970 7469 6f6e 203d 2048 6572 7261 6d69  iption = Herrami
-000000a0: 656e 7461 2064 6520 656c 696d 696e 6163  enta de eliminac
-000000b0: 69c3 b36e 2064 6520 616e 756e 6369 6f73  i..n de anuncios
-000000c0: 2070 6172 6120 5044 4673 2067 656e 6572   para PDFs gener
-000000d0: 6164 6f73 2070 6f72 206c 6120 706c 6174  ados por la plat
-000000e0: 6166 6f72 6d61 2057 756f 6c61 682e 0d0a  aforma Wuolah...
-000000f0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-00000100: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
-00000110: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
-00000120: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
-00000130: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
-00000140: 6e0d 0a75 726c 203d 2068 7474 7073 3a2f  n..url = https:/
-00000150: 2f67 6974 6875 622e 636f 6d2f 594d 3136  /github.com/YM16
-00000160: 322f 6775 6c61 672d 636c 6561 6e65 722d  2/gulag-cleaner-
-00000170: 636c 690d 0a70 726f 6a65 6374 5f75 726c  cli..project_url
-00000180: 7320 3d20 0d0a 0942 7567 2054 7261 636b  s = ...Bug Track
-00000190: 6572 203d 2068 7474 7073 3a2f 2f67 6974  er = https://git
-000001a0: 6875 622e 636f 6d2f 594d 3136 322f 6775  hub.com/YM162/gu
-000001b0: 6c61 672d 636c 6561 6e65 722d 636c 692f  lag-cleaner-cli/
-000001c0: 6973 7375 6573 0d0a 636c 6173 7369 6669  issues..classifi
-000001d0: 6572 7320 3d20 0d0a 0950 726f 6772 616d  ers = ...Program
-000001e0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000001f0: 2050 7974 686f 6e20 3a3a 2033 0d0a 094c   Python :: 3...L
-00000200: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
-00000210: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
-00000220: 6365 6e73 650d 0a09 4f70 6572 6174 696e  cense...Operatin
-00000230: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
-00000240: 6e64 6570 656e 6465 6e74 0d0a 0d0a 5b6f  ndependent....[o
-00000250: 7074 696f 6e73 5d0d 0a69 6e73 7461 6c6c  ptions]..install
-00000260: 5f72 6571 7569 7265 7320 3d20 0d0a 0970  _requires = ...p
-00000270: 6466 7277 3e3d 302e 340d 0a09 7069 6b65  dfrw>=0.4...pike
-00000280: 7064 663e 3d35 2e31 2e32 0d0a 0970 6466  pdf>=5.1.2...pdf
-00000290: 6d69 6e65 722e 7369 783e 3d32 3032 3230  miner.six>=20220
-000002a0: 3532 340d 0a70 6163 6b61 6765 7320 3d20  524..packages = 
-000002b0: 6669 6e64 3a0d 0a70 7974 686f 6e5f 7265  find:..python_re
-000002c0: 7175 6972 6573 203d 203e 3d33 2e36 0d0a  quires = >=3.6..
-000002d0: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
-000002e0: 6765 732e 6669 6e64 5d0d 0a65 7863 6c75  ges.find]..exclu
-000002f0: 6465 203d 200d 0a09 7465 7374 730d 0a0d  de = ...tests...
-00000300: 0a5b 6f70 7469 6f6e 732e 656e 7472 795f  .[options.entry_
-00000310: 706f 696e 7473 5d0d 0a63 6f6e 736f 6c65  points]..console
-00000320: 5f73 6372 6970 7473 203d 200d 0a09 6775  _scripts = ...gu
-00000330: 6c61 6763 6c65 616e 6572 203d 2067 756c  lagcleaner = gul
-00000340: 6167 636c 6561 6e65 722e 636f 6d6d 616e  agcleaner.comman
-00000350: 645f 6c69 6e65 3a6d 6169 6e0d 0a0d 0a5b  d_line:main....[
-00000360: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-00000370: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-00000380: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000070: 6e74 616e 6564 6131 3640 676d 6169 6c2e  ntaneda16@gmail.
+00000080: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
+00000090: 203d 2041 6420 7265 6d6f 7661 6c20 746f   = Ad removal to
+000000a0: 6f6c 2066 6f72 2050 4446 7320 7772 6974  ol for PDFs writ
+000000b0: 7465 6e20 696e 2070 7974 686f 6e2e 0d0a  ten in python...
+000000c0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000d0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
+000000e0: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
+000000f0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
+00000100: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
+00000110: 6e0d 0a75 726c 203d 2068 7474 7073 3a2f  n..url = https:/
+00000120: 2f67 6974 6875 622e 636f 6d2f 594d 3136  /github.com/YM16
+00000130: 322f 6775 6c61 672d 636c 6561 6e65 722d  2/gulag-cleaner-
+00000140: 636c 690d 0a70 726f 6a65 6374 5f75 726c  cli..project_url
+00000150: 7320 3d20 0d0a 0942 7567 2054 7261 636b  s = ...Bug Track
+00000160: 6572 203d 2068 7474 7073 3a2f 2f67 6974  er = https://git
+00000170: 6875 622e 636f 6d2f 594d 3136 322f 6775  hub.com/YM162/gu
+00000180: 6c61 672d 636c 6561 6e65 722d 636c 692f  lag-cleaner-cli/
+00000190: 6973 7375 6573 0d0a 636c 6173 7369 6669  issues..classifi
+000001a0: 6572 7320 3d20 0d0a 0950 726f 6772 616d  ers = ...Program
+000001b0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000001c0: 2050 7974 686f 6e20 3a3a 2033 0d0a 094c   Python :: 3...L
+000001d0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+000001e0: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
+000001f0: 6365 6e73 650d 0a09 4f70 6572 6174 696e  cense...Operatin
+00000200: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
+00000210: 6e64 6570 656e 6465 6e74 0d0a 0d0a 5b6f  ndependent....[o
+00000220: 7074 696f 6e73 5d0d 0a69 6e73 7461 6c6c  ptions]..install
+00000230: 5f72 6571 7569 7265 7320 3d20 0d0a 0970  _requires = ...p
+00000240: 6466 7277 3e3d 302e 340d 0a09 7069 6b65  dfrw>=0.4...pike
+00000250: 7064 663e 3d35 2e31 2e32 0d0a 0970 6466  pdf>=5.1.2...pdf
+00000260: 6d69 6e65 722e 7369 783e 3d32 3032 3230  miner.six>=20220
+00000270: 3532 340d 0a70 6163 6b61 6765 7320 3d20  524..packages = 
+00000280: 6669 6e64 3a0d 0a70 7974 686f 6e5f 7265  find:..python_re
+00000290: 7175 6972 6573 203d 203e 3d33 2e36 0d0a  quires = >=3.6..
+000002a0: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
+000002b0: 6765 732e 6669 6e64 5d0d 0a65 7863 6c75  ges.find]..exclu
+000002c0: 6465 203d 200d 0a09 7465 7374 730d 0a0d  de = ...tests...
+000002d0: 0a5b 6f70 7469 6f6e 732e 656e 7472 795f  .[options.entry_
+000002e0: 706f 696e 7473 5d0d 0a63 6f6e 736f 6c65  points]..console
+000002f0: 5f73 6372 6970 7473 203d 200d 0a09 6775  _scripts = ...gu
+00000300: 6c61 6763 6c65 616e 6572 203d 2067 756c  lagcleaner = gul
+00000310: 6167 636c 6561 6e65 722e 636f 6d6d 616e  agcleaner.comman
+00000320: 645f 6c69 6e65 3a6d 6169 6e0d 0a0d 0a5b  d_line:main....[
+00000330: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+00000340: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+00000350: 6520 3d20 300d 0a0d 0a                   e = 0....
```

