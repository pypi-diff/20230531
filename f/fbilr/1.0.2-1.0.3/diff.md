# Comparing `tmp/fbilr-1.0.2.tar.gz` & `tmp/fbilr-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/date/chenzonggui/software/fbilr/dist/tmp6qnitt_f/fbilr-1.0.2.tar", last modified: Thu Apr 21 16:18:03 2022, max compression
+gzip compressed data, was "/home/chenzonggui/software/fbilr/dist/tmpncmqfwug/fbilr-1.0.3.tar", last modified: Wed May 31 02:40:23 2023, max compression
```

## Comparing `fbilr-1.0.2.tar` & `fbilr-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 chenzonggui  (1014) tanglab   (1000)        0 2022-04-21 16:17:47.000000 fbilr-1.0.2/
-drwxr-xr-x   0 chenzonggui  (1014) tanglab   (1000)        0 2022-04-21 16:17:47.000000 fbilr-1.0.2/src/
-drwxr-xr-x   0 chenzonggui  (1014) tanglab   (1000)        0 2022-04-21 16:17:47.000000 fbilr-1.0.2/src/fbilr/
--rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)        0 2022-04-08 06:15:28.000000 fbilr-1.0.2/src/fbilr/__init__.py
-drwxr-xr-x   0 chenzonggui  (1014) tanglab   (1000)        0 2022-04-21 16:17:47.000000 fbilr-1.0.2/src/fbilr.egg-info/
--rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)     4101 2022-04-21 16:17:47.000000 fbilr-1.0.2/src/fbilr.egg-info/PKG-INFO
--rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)      290 2022-04-21 16:17:47.000000 fbilr-1.0.2/src/fbilr.egg-info/SOURCES.txt
--rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)        1 2022-04-21 16:17:47.000000 fbilr-1.0.2/src/fbilr.egg-info/dependency_links.txt
--rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)       38 2022-04-21 16:17:47.000000 fbilr-1.0.2/src/fbilr.egg-info/requires.txt
--rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)        6 2022-04-21 16:17:47.000000 fbilr-1.0.2/src/fbilr.egg-info/top_level.txt
-drwxr-xr-x   0 chenzonggui  (1014) tanglab   (1000)        0 2022-04-21 16:17:47.000000 fbilr-1.0.2/src/scripts/
--rwxr-xr-x   0 chenzonggui  (1014) tanglab   (1000)     7117 2022-04-21 09:23:35.000000 fbilr-1.0.2/src/scripts/find_barcode.py
--rwxr-xr-x   0 chenzonggui  (1014) tanglab   (1000)     6980 2022-04-21 16:07:49.000000 fbilr-1.0.2/src/scripts/plot_barcode_detail.py
--rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)     1068 2022-04-01 02:20:21.000000 fbilr-1.0.2/LICENSE
--rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)     3654 2022-04-21 15:40:11.000000 fbilr-1.0.2/README.md
--rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)       84 2022-04-08 05:53:51.000000 fbilr-1.0.2/pyproject.toml
--rwxr-xr-x   0 chenzonggui  (1014) tanglab   (1000)      893 2022-04-21 16:16:51.000000 fbilr-1.0.2/setup.py
--rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)     4101 2022-04-21 16:17:47.000000 fbilr-1.0.2/PKG-INFO
--rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)       38 2022-04-21 16:17:47.000000 fbilr-1.0.2/setup.cfg
+drwxr-xr-x   0 chenzonggui  (1014) tanglab   (1000)        0 2023-05-31 02:40:23.000000 fbilr-1.0.3/
+-rwxr-xr-x   0 chenzonggui  (1014) tanglab   (1000)      889 2023-05-31 02:39:35.000000 fbilr-1.0.3/setup.py
+-rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)     3853 2023-05-31 02:40:23.000000 fbilr-1.0.3/PKG-INFO
+-rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)     3410 2023-05-31 02:28:52.000000 fbilr-1.0.3/README.md
+drwxr-xr-x   0 chenzonggui  (1014) tanglab   (1000)        0 2023-05-31 02:40:23.000000 fbilr-1.0.3/src/
+drwxr-xr-x   0 chenzonggui  (1014) tanglab   (1000)        0 2023-05-31 02:40:23.000000 fbilr-1.0.3/src/fbilr.egg-info/
+-rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)      348 2023-05-31 02:40:23.000000 fbilr-1.0.3/src/fbilr.egg-info/SOURCES.txt
+-rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)     3853 2023-05-31 02:40:23.000000 fbilr-1.0.3/src/fbilr.egg-info/PKG-INFO
+-rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)        1 2023-05-31 02:40:23.000000 fbilr-1.0.3/src/fbilr.egg-info/dependency_links.txt
+-rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)       38 2023-05-31 02:40:23.000000 fbilr-1.0.3/src/fbilr.egg-info/requires.txt
+-rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)        6 2023-05-31 02:40:23.000000 fbilr-1.0.3/src/fbilr.egg-info/top_level.txt
+drwxr-xr-x   0 chenzonggui  (1014) tanglab   (1000)        0 2023-05-31 02:40:23.000000 fbilr-1.0.3/src/fbilr/
+-rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)     1547 2023-05-30 13:14:09.000000 fbilr-1.0.3/src/fbilr/utils.py
+-rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)    13243 2023-05-31 02:18:56.000000 fbilr-1.0.3/src/fbilr/finders.py
+-rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)        0 2022-04-08 06:15:28.000000 fbilr-1.0.3/src/fbilr/__init__.py
+-rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)     1016 2023-05-30 09:37:26.000000 fbilr-1.0.3/src/fbilr/find.py
+drwxr-xr-x   0 chenzonggui  (1014) tanglab   (1000)        0 2023-05-31 02:40:23.000000 fbilr-1.0.3/src/scripts/
+-rwxr-xr-x   0 chenzonggui  (1014) tanglab   (1000)     6980 2022-04-30 09:57:14.000000 fbilr-1.0.3/src/scripts/plot_barcode_detail.py
+-rwxr-xr-x   0 chenzonggui  (1014) tanglab   (1000)     2369 2023-05-31 01:41:54.000000 fbilr-1.0.3/src/scripts/find_barcode.py
+-rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)       38 2023-05-31 02:40:23.000000 fbilr-1.0.3/setup.cfg
+-rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)     1068 2022-04-01 02:20:21.000000 fbilr-1.0.3/LICENSE
+-rw-r--r--   0 chenzonggui  (1014) tanglab   (1000)       84 2022-04-08 05:53:51.000000 fbilr-1.0.3/pyproject.toml
```

### Comparing `fbilr-1.0.2/src/fbilr.egg-info/PKG-INFO` & `fbilr-1.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: fbilr
-Version: 1.0.2
+Version: 1.0.3
 Summary: Find barcode in long reads
-Home-page: https://gitee.com/chenzonggui/fbilr
+Home-page: https://github.com/Ckenen/fbilr
 Author: Zonggui Chen
 Author-email: ggchenzonggui@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
@@ -20,29 +20,25 @@
 
 FBILR is designed to find the best-matched barcode on reads and report detailed information (orientation, location, and edit distance). Since the barcode is likely to be located at one of the ends of the read (head or tail), and the read length is longer than 1,000 bp, FBILR restricts the search range to within 200bp of both ends to reduce the amount of computation and save time. Besides, FBILR is able to run in parallel and the order of output is accordant to input.
 
 ## Usage
 
 The usage of FBILR is shown below:
 
-    find_barcodes.py -t 8 -w 200 -m metrics.txt -s stats.txt barcodes.fasta reads.fastq.gz
-    # or
-    find_barcodes.py -t 8 -w 200 -s stats.txt barcodes.fasta reads.fastq.gz | gzip -c > metrics.txt.gz
-    # or 
-    pigz -p 4 -d -c reads.fastq.gz | find_barcodes.py -t 8 -w 200 -s stats.txt barcodes.fasta - | pigz -p 4 -c > metrics.txt.gz
+    find_barcodes.py -t 8 -w 200 -m matrix.txt -s summary.txt barcodes.fasta reads.fastq.gz    
 
 After that, you can visualize the result with the following command:
 
-    plot_barcode_detail.py -m metrics.txt -p outdir/out
+    plot_barcode_detail.py -m matrix.txt -p outdir/out
 
 ## Output files
 
-The find_barcode.py script will output 2 files (`metrics.txt` and `stats.txt`).
+The find_barcode.py script will output 2 files (`matrix.txt` and `summary.txt`).
 
-The `metrics.txt` is a tab-delimited file that consists of 8 columns (shown as follows). In this file, one row corresponds to one read in the input FASTQ file. Each read can find an optimal barcode, even though the edit distance is large (edit distance represents the difference between barcode sequence and reference sequence, including mismatch, insertion, and deletion of bases).
+The `matrix.txt` is a tab-delimited file that consists of 8 columns (shown as follows). In this file, one row corresponds to one read in the input FASTQ file. Each read can find an optimal barcode, even though the edit distance is large (edit distance represents the difference between barcode sequence and reference sequence, including mismatch, insertion, and deletion of bases).
 
     column 1: read name
     column 2: read length
     column 3: barcode name
     column 4: barcode orientation (F or R)
     column 5: barcode location (H, M or T)
     column 6: start in read (0-base, included)
@@ -54,15 +50,15 @@
     ed320d59-77c6-41ba-895d-f4fdba5855f2    249     Bar2    F       H       29      53      0
     9aa445f6-63b9-44e5-9b9c-43feea216b7a    492     Bar3    F       H       36      60      0
     3087cbe0-7b00-40ff-837c-4cc59cf7e7ff    280     Bar4    R       T       239     263     0
     15c53c45-ff43-4374-8716-049495d113aa    345     Bar4    F       H       27      50      3
     21c0fe8d-1725-42ba-b490-eec2cd6f76b3    408     Bar2    F       H       27      51      0
     90af744f-1367-493d-84e2-ca2375413e2d    551     Bar8    F       H       47      71      0
 
-The `stats.txt` is a tab-delimited file that consists of 2 columns (shown ad follows). Whether a barcode exists on a read is determined by edit distance (similarity). If the edit distance is small enough (-e option), we can confidently judge that the barcode exists, otherwise does not exist (unclassified). This file statistics the count of each barcode.
+The `summary.txt` is a tab-delimited file that consists of 2 columns (shown ad follows). Whether a barcode exists on a read is determined by edit distance (similarity). If the edit distance is small enough (-e option), we can confidently judge that the barcode exists, otherwise does not exist (unclassified). This file statistics the count of each barcode.
 
     column 1: barcode name
     column 2: count
 
     # Example: 
     Bar1	783154
     Bar2	236937
```

### Comparing `fbilr-1.0.2/src/scripts/plot_barcode_detail.py` & `fbilr-1.0.3/src/scripts/plot_barcode_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,54 +172,54 @@
         if orient == "F":
             counter_f_h[dis1] += 1
             counter_f_t[dis2] += 1
         else:
             counter_r_h[dis1] += 1
             counter_r_t[dis2] += 1
 
-    fig, axs = plt.subplots(2, 2, figsize=(10, 6))
+    fig, axs = plt.subplots(2, 2, figsize=(16, 6))
 
     plt.sca(axs[0][0])
     plt.title("Barcodes in forward")
-    xs = np.arange(0, 101)
+    xs = np.arange(0, 151)
     ys = [counter_f_h[x] for x in xs]
     t = sum(counter_f_h.values())
     ys = np.array(ys) * 100 / t
     plt.bar(xs, ys, width=1)
     plt.xlim(min(xs) - 1, max(xs) + 1)
     plt.ylabel("Percentage (%)")
     plt.xlabel("Distance to head end")
     plt.tight_layout()
 
     plt.sca(axs[0][1])
-    plt.title("Barcodes in reverse")
-    xs = np.arange(-100, 1)
+    plt.title("Barcodes in forward")
+    xs = np.arange(-150, 1)
     ys = [counter_f_t[-x] for x in xs]
     t = sum(counter_f_t.values())
     ys = np.array(ys) * 100 / t
     plt.bar(xs, ys, width=1)
     plt.xlim(min(xs) - 1, max(xs) + 1)
     plt.xlabel("Distance to tail end")
     plt.tight_layout()
 
     plt.sca(axs[1][0])
-    plt.title("Barcodes in forward")
-    xs = np.arange(0, 101)
+    plt.title("Barcodes in reverse")
+    xs = np.arange(0, 151)
     ys = [counter_r_h[x] for x in xs]
     t = sum(counter_r_h.values())
     ys = np.array(ys) * 100 / t
     plt.bar(xs, ys, width=1)
     plt.xlim(min(xs) - 1, max(xs) + 1)
     plt.ylabel("Percentage (%)")
     plt.xlabel("Distance to head end")
     plt.tight_layout()
 
     plt.sca(axs[1][1])
     plt.title("Barcodes in reverse")
-    xs = np.arange(-100, 1)
+    xs = np.arange(-150, 1)
     ys = [counter_r_t[-x] for x in xs]
     t = sum(counter_r_t.values())
     ys = np.array(ys) * 100 / t
     plt.bar(xs, ys, width=1)
     plt.xlim(min(xs) - 1, max(xs) + 1)
     plt.xlabel("Distance to tail end")
     plt.tight_layout()
```

### Comparing `fbilr-1.0.2/LICENSE` & `fbilr-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fbilr-1.0.2/README.md` & `fbilr-1.0.3/src/fbilr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,44 @@
+Metadata-Version: 2.1
+Name: fbilr
+Version: 1.0.3
+Summary: Find barcode in long reads
+Home-page: https://github.com/Ckenen/fbilr
+Author: Zonggui Chen
+Author-email: ggchenzonggui@qq.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Unix
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # FBILR: Find Barcode In Long Reads
 
 ## Description
 
 FBILR is designed to find the best-matched barcode on reads and report detailed information (orientation, location, and edit distance). Since the barcode is likely to be located at one of the ends of the read (head or tail), and the read length is longer than 1,000 bp, FBILR restricts the search range to within 200bp of both ends to reduce the amount of computation and save time. Besides, FBILR is able to run in parallel and the order of output is accordant to input.
 
 ## Usage
 
 The usage of FBILR is shown below:
 
-    find_barcodes.py -t 8 -w 200 -m metrics.txt -s stats.txt barcodes.fasta reads.fastq.gz
-    # or
-    find_barcodes.py -t 8 -w 200 -s stats.txt barcodes.fasta reads.fastq.gz | gzip -c > metrics.txt.gz
-    # or 
-    pigz -p 4 -d -c reads.fastq.gz | find_barcodes.py -t 8 -w 200 -s stats.txt barcodes.fasta - | pigz -p 4 -c > metrics.txt.gz
+    find_barcodes.py -t 8 -w 200 -m matrix.txt -s summary.txt barcodes.fasta reads.fastq.gz    
 
 After that, you can visualize the result with the following command:
 
-    plot_barcode_detail.py -m metrics.txt -p outdir/out
+    plot_barcode_detail.py -m matrix.txt -p outdir/out
 
 ## Output files
 
-The find_barcode.py script will output 2 files (`metrics.txt` and `stats.txt`).
+The find_barcode.py script will output 2 files (`matrix.txt` and `summary.txt`).
 
-The `metrics.txt` is a tab-delimited file that consists of 8 columns (shown as follows). In this file, one row corresponds to one read in the input FASTQ file. Each read can find an optimal barcode, even though the edit distance is large (edit distance represents the difference between barcode sequence and reference sequence, including mismatch, insertion, and deletion of bases).
+The `matrix.txt` is a tab-delimited file that consists of 8 columns (shown as follows). In this file, one row corresponds to one read in the input FASTQ file. Each read can find an optimal barcode, even though the edit distance is large (edit distance represents the difference between barcode sequence and reference sequence, including mismatch, insertion, and deletion of bases).
 
     column 1: read name
     column 2: read length
     column 3: barcode name
     column 4: barcode orientation (F or R)
     column 5: barcode location (H, M or T)
     column 6: start in read (0-base, included)
@@ -38,15 +50,15 @@
     ed320d59-77c6-41ba-895d-f4fdba5855f2    249     Bar2    F       H       29      53      0
     9aa445f6-63b9-44e5-9b9c-43feea216b7a    492     Bar3    F       H       36      60      0
     3087cbe0-7b00-40ff-837c-4cc59cf7e7ff    280     Bar4    R       T       239     263     0
     15c53c45-ff43-4374-8716-049495d113aa    345     Bar4    F       H       27      50      3
     21c0fe8d-1725-42ba-b490-eec2cd6f76b3    408     Bar2    F       H       27      51      0
     90af744f-1367-493d-84e2-ca2375413e2d    551     Bar8    F       H       47      71      0
 
-The `stats.txt` is a tab-delimited file that consists of 2 columns (shown ad follows). Whether a barcode exists on a read is determined by edit distance (similarity). If the edit distance is small enough (-e option), we can confidently judge that the barcode exists, otherwise does not exist (unclassified). This file statistics the count of each barcode.
+The `summary.txt` is a tab-delimited file that consists of 2 columns (shown ad follows). Whether a barcode exists on a read is determined by edit distance (similarity). If the edit distance is small enough (-e option), we can confidently judge that the barcode exists, otherwise does not exist (unclassified). This file statistics the count of each barcode.
 
     column 1: barcode name
     column 2: count
 
     # Example: 
     Bar1	783154
     Bar2	236937
@@ -75,7 +87,9 @@
 Finally, the bar1 is the best-matched barcode in this read.
 
 ## Packaging and distributing
 
     python -m build
     python3 -m twine upload --repository pypi dist/*
 
+
+
```

### Comparing `fbilr-1.0.2/setup.py` & `fbilr-1.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,21 +7,21 @@
     scripts.append(s)
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fbilr",
-    version="1.0.2",
+    version="1.0.3",
     author="Zonggui Chen",
     author_email="ggchenzonggui@qq.com",
     description="Find barcode in long reads",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://gitee.com/chenzonggui/fbilr",
+    url="https://github.com/Ckenen/fbilr",
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: Unix"
     ],
```

