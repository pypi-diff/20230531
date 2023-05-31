# Comparing `tmp/modisco-lite-2.1.1.tar.gz` & `tmp/modisco-lite-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modisco-lite-2.1.1.tar", last modified: Wed May 24 20:58:38 2023, max compression
+gzip compressed data, was "modisco-lite-2.2.0.tar", last modified: Wed May 31 17:04:50 2023, max compression
```

## Comparing `modisco-lite-2.1.1.tar` & `modisco-lite-2.2.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2023-05-24 20:58:38.206776 modisco-lite-2.1.1/
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     1068 2022-08-09 18:54:36.000000 modisco-lite-2.1.1/LICENSE
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      197 2022-08-09 18:54:36.000000 modisco-lite-2.1.1/MANIFEST.in
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      321 2023-05-24 20:58:38.202776 modisco-lite-2.1.1/PKG-INFO
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6537 2023-05-24 17:21:53.000000 modisco-lite-2.1.1/README.md
--rwxr-xr-x   0 jmschr    (1222) kundaje  (65541)     5755 2023-05-24 17:21:53.000000 modisco-lite-2.1.1/modisco
-drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2023-05-24 20:58:38.050776 modisco-lite-2.1.1/modisco_lite.egg-info/
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      321 2023-05-24 20:58:37.000000 modisco-lite-2.1.1/modisco_lite.egg-info/PKG-INFO
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      521 2023-05-24 20:58:37.000000 modisco-lite-2.1.1/modisco_lite.egg-info/SOURCES.txt
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)        1 2023-05-24 20:58:37.000000 modisco-lite-2.1.1/modisco_lite.egg-info/dependency_links.txt
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      159 2023-05-24 20:58:37.000000 modisco-lite-2.1.1/modisco_lite.egg-info/requires.txt
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)       12 2023-05-24 20:58:37.000000 modisco-lite-2.1.1/modisco_lite.egg-info/top_level.txt
-drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2023-05-24 20:58:38.186776 modisco-lite-2.1.1/modiscolite/
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      251 2023-05-24 20:57:15.000000 modisco-lite-2.1.1/modiscolite/__init__.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     8038 2022-09-28 01:28:38.000000 modisco-lite-2.1.1/modiscolite/affinitymat.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    17392 2022-10-11 23:03:15.000000 modisco-lite-2.1.1/modiscolite/aggregator.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     1185 2022-09-28 03:19:15.000000 modisco-lite-2.1.1/modiscolite/cluster.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     7359 2022-09-29 01:59:01.000000 modisco-lite-2.1.1/modiscolite/core.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6733 2022-09-28 18:48:23.000000 modisco-lite-2.1.1/modiscolite/extract_seqlets.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     3745 2022-09-28 18:49:11.000000 modisco-lite-2.1.1/modiscolite/gapped_kmer.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    12407 2023-01-14 03:05:25.000000 modisco-lite-2.1.1/modiscolite/io.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    11309 2022-09-28 06:45:23.000000 modisco-lite-2.1.1/modiscolite/old_large_modisco.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     9463 2023-05-24 20:51:27.000000 modisco-lite-2.1.1/modiscolite/report.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    13367 2022-09-30 17:56:33.000000 modisco-lite-2.1.1/modiscolite/tfmodisco.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     3384 2022-09-30 21:12:20.000000 modisco-lite-2.1.1/modiscolite/util.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)       38 2023-05-24 20:58:38.206776 modisco-lite-2.1.1/setup.cfg
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      644 2023-05-24 20:57:27.000000 modisco-lite-2.1.1/setup.py
+drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2023-05-31 17:04:50.626234 modisco-lite-2.2.0/
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     1068 2023-05-31 17:03:51.000000 modisco-lite-2.2.0/LICENSE
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      321 2023-05-31 17:04:50.626234 modisco-lite-2.2.0/PKG-INFO
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6537 2023-05-31 17:03:51.000000 modisco-lite-2.2.0/README.md
+-rwxr-xr-x   0 jmschr    (1222) kundaje  (65541)     6974 2023-05-31 17:03:51.000000 modisco-lite-2.2.0/modisco
+drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2023-05-31 17:04:50.598235 modisco-lite-2.2.0/modisco_lite.egg-info/
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      321 2023-05-31 17:04:50.000000 modisco-lite-2.2.0/modisco_lite.egg-info/PKG-INFO
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      503 2023-05-31 17:04:50.000000 modisco-lite-2.2.0/modisco_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)        1 2023-05-31 17:04:50.000000 modisco-lite-2.2.0/modisco_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      159 2023-05-31 17:04:50.000000 modisco-lite-2.2.0/modisco_lite.egg-info/requires.txt
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)       12 2023-05-31 17:04:50.000000 modisco-lite-2.2.0/modisco_lite.egg-info/top_level.txt
+drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2023-05-31 17:04:50.622234 modisco-lite-2.2.0/modiscolite/
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      278 2023-05-31 17:04:23.000000 modisco-lite-2.2.0/modiscolite/__init__.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     8038 2023-05-31 17:03:51.000000 modisco-lite-2.2.0/modiscolite/affinitymat.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    17392 2023-05-31 17:03:51.000000 modisco-lite-2.2.0/modiscolite/aggregator.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     1185 2023-05-31 17:03:51.000000 modisco-lite-2.2.0/modiscolite/cluster.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     7359 2023-05-31 17:03:51.000000 modisco-lite-2.2.0/modiscolite/core.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6733 2023-05-31 17:03:51.000000 modisco-lite-2.2.0/modiscolite/extract_seqlets.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     3745 2023-05-31 17:03:51.000000 modisco-lite-2.2.0/modiscolite/gapped_kmer.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    14407 2023-05-31 17:03:51.000000 modisco-lite-2.2.0/modiscolite/io.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     4676 2023-05-31 17:03:51.000000 modisco-lite-2.2.0/modiscolite/meme_writer.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     9463 2023-05-31 17:03:51.000000 modisco-lite-2.2.0/modiscolite/report.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    13367 2023-05-31 17:03:51.000000 modisco-lite-2.2.0/modiscolite/tfmodisco.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     3601 2023-05-31 17:03:51.000000 modisco-lite-2.2.0/modiscolite/util.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)       38 2023-05-31 17:04:50.626234 modisco-lite-2.2.0/setup.cfg
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      644 2023-05-31 17:04:28.000000 modisco-lite-2.2.0/setup.py
```

### Comparing `modisco-lite-2.1.1/LICENSE` & `modisco-lite-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modisco-lite-2.1.1/README.md` & `modisco-lite-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `modisco-lite-2.1.1/modisco` & `modisco-lite-2.2.0/modisco`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 #!/usr/bin/env python
 # tf-modisco command-line tool
-# Author: Jacob Schreiber <jmschreiber91@gmail.com>
+# Author: Jacob Schreiber <jmschreiber91@gmail.com>, Ivy Raine <ivy.ember.raine@gmail.com>
 
 import h5py
 import hdf5plugin
 import argparse
 import modiscolite
 
 import numpy as np
 
+
 desc = """TF-MoDISco is a motif detection algorithm that takes in nucleotide
 	sequence and the attributions from a neural network model and return motifs
 	that are repeatedly enriched for attriution score across the examples.
 	This tool will take in one-hot encoded sequence, the corresponding
 	attribution scores, and a few other parameters, and return the motifs."""
 
 # Read in the arguments
 parser = argparse.ArgumentParser(description=desc)
-subparsers = parser.add_subparsers(help="Must be either 'motifs', 'report', or 'convert'.", required=True, dest='cmd')
+subparsers = parser.add_subparsers(help="Must be either 'motifs', 'report', 'convert', 'convert-backward', or 'meme'.", required=True, dest='cmd')
 
 motifs_parser = subparsers.add_parser("motifs", help="Run TF-MoDISco and extract the motifs.")
 motifs_parser.add_argument("-s", "--sequences", type=str,
 	help="A .npy or .npz file containing the one-hot encoded sequences.")
 motifs_parser.add_argument("-a", "--attributions", type=str,
 	help="A .npy or .npz file containing the hypothetical attributions, i.e., the attributions for all nucleotides at all positions.")
 motifs_parser.add_argument("-i", "--h5py", type=str,
@@ -57,14 +58,29 @@
 
 convertback_parser = subparsers.add_parser("convert-backward", help="Convert a new h5py to the old format.")
 convertback_parser.add_argument("-i", "--h5py", type=str, required=True,
 	help="An HDF5 file formatted in the new way.")
 convertback_parser.add_argument("-o", "--output", type=str, required=True,
 	help="An HDF5 file formatted in the old way.")
 
+meme_parser = subparsers.add_parser("meme", help="Create a MEME file from a modisco results file.", formatter_class=argparse.RawTextHelpFormatter)
+meme_parser.add_argument("-i", "--h5py", type=str, required=True,
+	help="An HDF5 file containing the output from modiscolite.")
+meme_parser.add_argument("-t", "--datatype", type=modiscolite.util.MemeDataType, choices=list(modiscolite.util.MemeDataType), required=True,
+	help="""A case-sensitive string specifying the desired data of the output file.,
+The options are as follows:
+- 'PFM':      The position-frequency matrix.
+- 'CWM':      The contribution-weight matrix.
+- 'hCWM':     The hypothetical contribution-weight matrix; hypothetical
+              contribution scores are the contributions of nucleotides not encoded
+              by the one-hot encoding sequence. 
+- 'CWM-PFM':  The softmax of the contribution-weight matrix.
+- 'hCWM-PFM': The softmax of the hypothetical contribution-weight matrix."""
+)
+meme_parser.add_argument("-o", "--output", type=str, help="The path to the output file.")
 
 # Pull the arguments
 args = parser.parse_args()
 
 if args.cmd == "motifs":
 	if args.h5py is not None:
 		# Load the scores
@@ -120,14 +136,17 @@
 		flank_size=5,
 		target_seqlet_fdr=0.05,
 		n_leiden_runs=args.n_leiden,
 		verbose=args.verbose)
 
 	modiscolite.io.save_hdf5(args.output, pos_patterns, neg_patterns)
 
+elif args.cmd == 'meme':
+	modiscolite.io.write_meme_from_h5(args.h5py, args.datatype, args.output)
+
 elif args.cmd == 'report':
 	modiscolite.report.report_motifs(args.h5py, args.output, img_path_suffix=args.suffix, meme_motif_db=args.meme_db, 
 		top_n_matches=args.n_matches)
 
 elif args.cmd == 'convert':
 	modiscolite.io.convert(args.h5py, args.output)
```

### Comparing `modisco-lite-2.1.1/modiscolite/affinitymat.py` & `modisco-lite-2.2.0/modiscolite/affinitymat.py`

 * *Files identical despite different names*

### Comparing `modisco-lite-2.1.1/modiscolite/aggregator.py` & `modisco-lite-2.2.0/modiscolite/aggregator.py`

 * *Files identical despite different names*

### Comparing `modisco-lite-2.1.1/modiscolite/cluster.py` & `modisco-lite-2.2.0/modiscolite/cluster.py`

 * *Files identical despite different names*

### Comparing `modisco-lite-2.1.1/modiscolite/core.py` & `modisco-lite-2.2.0/modiscolite/core.py`

 * *Files identical despite different names*

### Comparing `modisco-lite-2.1.1/modiscolite/extract_seqlets.py` & `modisco-lite-2.2.0/modiscolite/extract_seqlets.py`

 * *Files identical despite different names*

### Comparing `modisco-lite-2.1.1/modiscolite/gapped_kmer.py` & `modisco-lite-2.2.0/modiscolite/gapped_kmer.py`

 * *Files identical despite different names*

### Comparing `modisco-lite-2.1.1/modiscolite/io.py` & `modisco-lite-2.2.0/modiscolite/io.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # io.py
-# Authors: Jacob Schreiber <jmschreiber91@gmail.com>
+# Authors: Jacob Schreiber <jmschreiber91@gmail.com>, Ivy Raine <ivy.ember.raine@gmail.com>
+
+import os
 
 import h5py
 import hdf5plugin
 
 import numpy as np
+import scipy
+
+from . import util
+from . import meme_writer
 
 def convert(old_filename, filename):
 	old_grp = h5py.File(old_filename, "r")['metacluster_idx_to_submetacluster_results']
 	new_grp = h5py.File(filename, "w")
 
 	if 'metacluster_0' in old_grp.keys():
 		pos_patterns_grp = new_grp.create_group("pos_patterns")
@@ -154,14 +160,69 @@
 	if neg_patterns is not None:
 		neg_group = grp.create_group("neg_patterns")
 		for idx, pattern in enumerate(neg_patterns):
 			neg_pattern = neg_group.create_group("pattern_"+str(idx))
 			save_pattern(pattern, neg_pattern)
 
 
+def write_meme_from_h5(filename: os.PathLike, datatype: util.MemeDataType, output_filename: os.PathLike) -> None:
+	"""Write a MEME file from an h5 file output from TF-MoDISco. Based on the given datatype.
+
+	Parameters
+	----------
+	filename: str
+		The name of the h5 file to read.
+	datatype: MemeDataType
+		The datatype to use for the MEME file.
+	output_filename: str
+		The name of the MEME file to write.
+	"""
+
+	alphabet = 'ACGT'
+	writer = meme_writer.MEMEWriter(
+		memesuite_version='5',
+		alphabet=alphabet,
+		background_frequencies='A 0.25 C 0.25 G 0.25 T 0.25'
+	)
+
+	with h5py.File(filename, 'r') as grp:
+		for (name, datasets) in grp['pos_patterns'].items():
+
+			probability_matrix = None
+			if datatype == util.MemeDataType.PFM:
+				probability_matrix = datasets['sequence'][:] / np.sum(datasets['sequence'][:], axis=1, keepdims=True)
+			elif datatype == util.MemeDataType.CWM:
+				probability_matrix = datasets['contrib_scores'][:]
+			elif datatype == util.MemeDataType.hCWM:
+				probability_matrix = datasets['hypothetical_contribs'][:]
+			elif datatype == util.MemeDataType.CWM_PFM:
+				# Softmax version of CWM.
+				probability_matrix = scipy.special.softmax(datasets['contrib_scores'][:], axis=1)
+			elif datatype == util.MemeDataType.hCWM_PFM:
+				# Softmax version of hCWM.
+				probability_matrix = scipy.special.softmax(datasets['hypothetical_contribs'][:], axis=1)
+			else:
+				raise ValueError("Unknown datatype: {}".format(datatype))
+
+			motif = meme_writer.MEMEWriterMotif(
+						name=name,
+						probability_matrix=probability_matrix,
+						source_sites=1,
+						alphabet=alphabet,
+						alphabet_length=4)
+
+			writer.add_motif(motif)
+	
+	new_output_filename = output_filename
+	if output_filename is None:
+		file_without_extension = os.path.splitext(filename)[0]
+		new_output_filename = f'{file_without_extension}.{datatype.name}.meme'
+	writer.write(new_output_filename)
+
+
 def convert_new_to_old(new_format_filename, old_format_filename):
 	'''This function does the opposite of the convert function.
 	Given the filepath to a tfmodisco-lite-formatted file (arg 1),
 	it writes the same information in the original tfmodisco format
 	to file (arg 2).
 	
 	This function assumes that metacluster0 should be the positive
@@ -282,8 +343,8 @@
                     
 				old_patterns_subgrp.create_dataset("all_pattern_names", data=pattern_names)
 
 			# required to avoid error: a collection of seqlets for the entire metacluster
 			old_metacluster_grp.create_dataset("seqlets", data=metacluster_seqlet_strings)
 
 	old_f.close()
-	new_f.close()
+	new_f.close()
```

### Comparing `modisco-lite-2.1.1/modiscolite/report.py` & `modisco-lite-2.2.0/modiscolite/report.py`

 * *Files identical despite different names*

### Comparing `modisco-lite-2.1.1/modiscolite/tfmodisco.py` & `modisco-lite-2.2.0/modiscolite/tfmodisco.py`

 * *Files identical despite different names*

### Comparing `modisco-lite-2.1.1/modiscolite/util.py` & `modisco-lite-2.2.0/modiscolite/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 # util.py
-# Authors: Jacob Schreiber <jmschreiber91@gmail.com>
+# Authors: Jacob Schreiber <jmschreiber91@gmail.com>, Ivy Raine <ivy.ember.raine@gmail.com>
 # adapted from code written by Avanti Shrikumar 
 
+from enum import Enum
 import numpy as np
 from numba import njit
 
+
+class MemeDataType(Enum):
+	PFM = "PFM"
+	CWM = "CWM"
+	hCWM = "hCWM"
+	CWM_PFM = "CWM-PFM"
+	hCWM_PFM = "hCWM-PFM"
+
+	def __str__(self):
+		return self.value
+
+
+
 def cpu_sliding_window_sum(arr, window_size):
 	to_return = np.zeros(len(arr)-window_size+1)
 	current_sum = np.sum(arr[0:window_size])
 	to_return[0] = current_sum
 	idx_to_include = window_size
 	idx_to_exclude = 0
 	while idx_to_include < len(arr):
```

### Comparing `modisco-lite-2.1.1/setup.py` & `modisco-lite-2.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
 	name='modisco-lite',
-	version='2.1.1',
+	version='2.2.0',
 	author='Jacob Schreiber',
 	author_email='jmschreiber91@gmail.com',
 	packages=['modiscolite'],
 	python_requires='>=3.7, <3.11',
 	scripts=['modisco'],
 	url='https://github.com/jmschrei/tfmodisco-lite',
 	license='LICENSE.txt',
```

