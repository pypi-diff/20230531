# Comparing `tmp/pdb-toolkit-0.3.1.tar.gz` & `tmp/pdb-toolkit-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdb-toolkit-0.3.1.tar", last modified: Wed Apr 19 14:54:36 2023, max compression
+gzip compressed data, was "pdb-toolkit-0.3.2.tar", last modified: Wed May 31 14:40:01 2023, max compression
```

## Comparing `pdb-toolkit-0.3.1.tar` & `pdb-toolkit-0.3.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:54:36.725484 pdb-toolkit-0.3.1/
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     1064 2023-04-14 08:01:52.000000 pdb-toolkit-0.3.1/LICENSE
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      402 2023-04-19 14:54:36.725484 pdb-toolkit-0.3.1/PKG-INFO
--rw-rw-r--   0 raouf     (1000) raouf     (1000)    11323 2023-04-19 14:01:55.000000 pdb-toolkit-0.3.1/README.md
-drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:54:36.713484 pdb-toolkit-0.3.1/pdb_toolkit/
--rw-rw-r--   0 raouf     (1000) raouf     (1000)        0 2023-04-14 08:01:52.000000 pdb-toolkit-0.3.1/pdb_toolkit/__init__.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     1190 2023-04-14 09:08:12.000000 pdb-toolkit-0.3.1/pdb_toolkit/constants.py
-drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:54:36.717484 pdb-toolkit-0.3.1/pdb_toolkit/editor/
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      241 2023-04-14 08:01:52.000000 pdb-toolkit-0.3.1/pdb_toolkit/editor/__init__.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     1949 2023-04-14 14:54:32.000000 pdb-toolkit-0.3.1/pdb_toolkit/editor/fix_pdb.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      922 2023-04-14 08:01:52.000000 pdb-toolkit-0.3.1/pdb_toolkit/editor/keep_only_atoms.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      944 2023-04-17 13:21:20.000000 pdb-toolkit-0.3.1/pdb_toolkit/editor/protonate_pdb.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     1976 2023-04-14 08:01:52.000000 pdb-toolkit-0.3.1/pdb_toolkit/editor/renumber_pdb.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      857 2023-04-14 08:01:52.000000 pdb-toolkit-0.3.1/pdb_toolkit/editor/sort_atoms.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      742 2023-04-17 09:44:44.000000 pdb-toolkit-0.3.1/pdb_toolkit/editor/unprotonate_pdb.py
-drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:54:36.721484 pdb-toolkit-0.3.1/pdb_toolkit/generic/
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      201 2023-04-17 15:58:54.000000 pdb-toolkit-0.3.1/pdb_toolkit/generic/__init__.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     1452 2023-04-18 14:52:03.000000 pdb-toolkit-0.3.1/pdb_toolkit/generic/align.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      703 2023-04-14 08:01:52.000000 pdb-toolkit-0.3.1/pdb_toolkit/generic/concat_pdbs.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     2602 2023-04-19 08:53:47.000000 pdb-toolkit-0.3.1/pdb_toolkit/generic/download_pdb.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     2557 2023-04-18 12:27:11.000000 pdb-toolkit-0.3.1/pdb_toolkit/generic/extract_chains_from_pdb.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     1096 2023-04-14 08:01:52.000000 pdb-toolkit-0.3.1/pdb_toolkit/generic/split_chains.py
-drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:54:36.725484 pdb-toolkit-0.3.1/pdb_toolkit/parser/
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      282 2023-04-19 10:41:27.000000 pdb-toolkit-0.3.1/pdb_toolkit/parser/__init__.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     1991 2023-04-18 09:20:44.000000 pdb-toolkit-0.3.1/pdb_toolkit/parser/get_atoms_residues.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     1101 2023-04-18 08:36:06.000000 pdb-toolkit-0.3.1/pdb_toolkit/parser/get_pdb_centroid.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     2514 2023-04-14 08:01:52.000000 pdb-toolkit-0.3.1/pdb_toolkit/parser/get_pdb_sequence.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     1661 2023-04-14 09:07:20.000000 pdb-toolkit-0.3.1/pdb_toolkit/parser/split_residues_surface_boundary_core.py
--rw-rw-r--   0 raouf     (1000) raouf     (1000)     2814 2023-04-19 10:41:27.000000 pdb-toolkit-0.3.1/pdb_toolkit/parser/steric_clashes.py
-drwxrwxr-x   0 raouf     (1000) raouf     (1000)        0 2023-04-19 14:54:36.717484 pdb-toolkit-0.3.1/pdb_toolkit.egg-info/
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      402 2023-04-19 14:54:36.000000 pdb-toolkit-0.3.1/pdb_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      951 2023-04-19 14:54:36.000000 pdb-toolkit-0.3.1/pdb_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 raouf     (1000) raouf     (1000)        1 2023-04-19 14:54:36.000000 pdb-toolkit-0.3.1/pdb_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 raouf     (1000) raouf     (1000)        5 2023-04-19 14:54:36.000000 pdb-toolkit-0.3.1/pdb_toolkit.egg-info/requires.txt
--rw-rw-r--   0 raouf     (1000) raouf     (1000)       12 2023-04-19 14:54:36.000000 pdb-toolkit-0.3.1/pdb_toolkit.egg-info/top_level.txt
--rw-rw-r--   0 raouf     (1000) raouf     (1000)       38 2023-04-19 14:54:36.725484 pdb-toolkit-0.3.1/setup.cfg
--rw-rw-r--   0 raouf     (1000) raouf     (1000)      669 2023-04-19 14:48:09.000000 pdb-toolkit-0.3.1/setup.py
+drwxrwxr-x   0 raouf-ks  (1000) raouf-ks  (1000)        0 2023-05-31 14:40:01.643576 pdb-toolkit-0.3.2/
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     1064 2023-05-31 09:48:12.000000 pdb-toolkit-0.3.2/LICENSE
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)    11744 2023-05-31 14:40:01.643576 pdb-toolkit-0.3.2/PKG-INFO
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)    11323 2023-05-31 09:48:12.000000 pdb-toolkit-0.3.2/README.md
+drwxrwxr-x   0 raouf-ks  (1000) raouf-ks  (1000)        0 2023-05-31 14:40:01.643576 pdb-toolkit-0.3.2/pdb_toolkit/
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)        0 2023-05-31 09:48:12.000000 pdb-toolkit-0.3.2/pdb_toolkit/__init__.py
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     1190 2023-05-31 09:48:12.000000 pdb-toolkit-0.3.2/pdb_toolkit/constants.py
+drwxrwxr-x   0 raouf-ks  (1000) raouf-ks  (1000)        0 2023-05-31 14:40:01.643576 pdb-toolkit-0.3.2/pdb_toolkit/editor/
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)      241 2023-05-31 09:48:12.000000 pdb-toolkit-0.3.2/pdb_toolkit/editor/__init__.py
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     1949 2023-05-31 09:48:12.000000 pdb-toolkit-0.3.2/pdb_toolkit/editor/fix_pdb.py
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)      922 2023-05-31 09:48:12.000000 pdb-toolkit-0.3.2/pdb_toolkit/editor/keep_only_atoms.py
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)      944 2023-05-31 09:48:12.000000 pdb-toolkit-0.3.2/pdb_toolkit/editor/protonate_pdb.py
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     1976 2023-05-31 09:48:12.000000 pdb-toolkit-0.3.2/pdb_toolkit/editor/renumber_pdb.py
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)      857 2023-05-31 09:48:12.000000 pdb-toolkit-0.3.2/pdb_toolkit/editor/sort_atoms.py
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)      742 2023-05-31 09:48:12.000000 pdb-toolkit-0.3.2/pdb_toolkit/editor/unprotonate_pdb.py
+drwxrwxr-x   0 raouf-ks  (1000) raouf-ks  (1000)        0 2023-05-31 14:40:01.643576 pdb-toolkit-0.3.2/pdb_toolkit/generic/
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)      201 2023-05-31 09:48:12.000000 pdb-toolkit-0.3.2/pdb_toolkit/generic/__init__.py
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     1452 2023-05-31 09:48:12.000000 pdb-toolkit-0.3.2/pdb_toolkit/generic/align.py
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)      703 2023-05-31 09:48:12.000000 pdb-toolkit-0.3.2/pdb_toolkit/generic/concat_pdbs.py
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     2602 2023-05-31 09:48:12.000000 pdb-toolkit-0.3.2/pdb_toolkit/generic/download_pdb.py
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     2557 2023-05-31 09:48:12.000000 pdb-toolkit-0.3.2/pdb_toolkit/generic/extract_chains_from_pdb.py
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     1096 2023-05-31 09:48:12.000000 pdb-toolkit-0.3.2/pdb_toolkit/generic/split_chains.py
+drwxrwxr-x   0 raouf-ks  (1000) raouf-ks  (1000)        0 2023-05-31 14:40:01.643576 pdb-toolkit-0.3.2/pdb_toolkit/parser/
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)      282 2023-05-31 09:48:12.000000 pdb-toolkit-0.3.2/pdb_toolkit/parser/__init__.py
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     1991 2023-05-31 09:48:12.000000 pdb-toolkit-0.3.2/pdb_toolkit/parser/get_atoms_residues.py
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     1101 2023-05-31 09:48:12.000000 pdb-toolkit-0.3.2/pdb_toolkit/parser/get_pdb_centroid.py
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     2756 2023-05-31 14:07:11.000000 pdb-toolkit-0.3.2/pdb_toolkit/parser/get_pdb_sequence.py
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     1661 2023-05-31 09:48:12.000000 pdb-toolkit-0.3.2/pdb_toolkit/parser/split_residues_surface_boundary_core.py
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)     2814 2023-05-31 09:48:12.000000 pdb-toolkit-0.3.2/pdb_toolkit/parser/steric_clashes.py
+drwxrwxr-x   0 raouf-ks  (1000) raouf-ks  (1000)        0 2023-05-31 14:40:01.643576 pdb-toolkit-0.3.2/pdb_toolkit.egg-info/
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)    11744 2023-05-31 14:40:01.000000 pdb-toolkit-0.3.2/pdb_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)      951 2023-05-31 14:40:01.000000 pdb-toolkit-0.3.2/pdb_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)        1 2023-05-31 14:40:01.000000 pdb-toolkit-0.3.2/pdb_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)        5 2023-05-31 14:40:01.000000 pdb-toolkit-0.3.2/pdb_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)       12 2023-05-31 14:40:01.000000 pdb-toolkit-0.3.2/pdb_toolkit.egg-info/top_level.txt
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)       38 2023-05-31 14:40:01.643576 pdb-toolkit-0.3.2/setup.cfg
+-rw-rw-r--   0 raouf-ks  (1000) raouf-ks  (1000)      722 2023-05-31 14:39:47.000000 pdb-toolkit-0.3.2/setup.py
```

### Comparing `pdb-toolkit-0.3.1/LICENSE` & `pdb-toolkit-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3.1/README.md` & `pdb-toolkit-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3.1/pdb_toolkit/constants.py` & `pdb-toolkit-0.3.2/pdb_toolkit/constants.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3.1/pdb_toolkit/editor/fix_pdb.py` & `pdb-toolkit-0.3.2/pdb_toolkit/editor/fix_pdb.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3.1/pdb_toolkit/editor/keep_only_atoms.py` & `pdb-toolkit-0.3.2/pdb_toolkit/editor/keep_only_atoms.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3.1/pdb_toolkit/editor/protonate_pdb.py` & `pdb-toolkit-0.3.2/pdb_toolkit/editor/protonate_pdb.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3.1/pdb_toolkit/editor/renumber_pdb.py` & `pdb-toolkit-0.3.2/pdb_toolkit/editor/renumber_pdb.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3.1/pdb_toolkit/editor/sort_atoms.py` & `pdb-toolkit-0.3.2/pdb_toolkit/editor/sort_atoms.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3.1/pdb_toolkit/editor/unprotonate_pdb.py` & `pdb-toolkit-0.3.2/pdb_toolkit/editor/unprotonate_pdb.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3.1/pdb_toolkit/generic/align.py` & `pdb-toolkit-0.3.2/pdb_toolkit/generic/align.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3.1/pdb_toolkit/generic/concat_pdbs.py` & `pdb-toolkit-0.3.2/pdb_toolkit/generic/concat_pdbs.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3.1/pdb_toolkit/generic/download_pdb.py` & `pdb-toolkit-0.3.2/pdb_toolkit/generic/download_pdb.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3.1/pdb_toolkit/generic/extract_chains_from_pdb.py` & `pdb-toolkit-0.3.2/pdb_toolkit/generic/extract_chains_from_pdb.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3.1/pdb_toolkit/generic/split_chains.py` & `pdb-toolkit-0.3.2/pdb_toolkit/generic/split_chains.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3.1/pdb_toolkit/parser/get_atoms_residues.py` & `pdb-toolkit-0.3.2/pdb_toolkit/parser/get_atoms_residues.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3.1/pdb_toolkit/parser/get_pdb_centroid.py` & `pdb-toolkit-0.3.2/pdb_toolkit/parser/get_pdb_centroid.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3.1/pdb_toolkit/parser/get_pdb_sequence.py` & `pdb-toolkit-0.3.2/pdb_toolkit/parser/get_pdb_sequence.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 # @Time    : 07/09/2022 15:31
 # @Author  : Raouf KESKES
 # @Email   : raouf.keskes@mabsilico.com
 # @File    : get_pdb_sequence.py
 import os.path
 import tempfile
+import uuid
 
 from Bio.PDB import PDBParser
 from pdb_toolkit.constants import d3to1
 from pdb_toolkit.editor import keep_only_atom_lines
 
 
 def get_pdb_sequence(in_pdb_file, chains=None, ignore_missing=False):
@@ -27,19 +28,25 @@
     """
 
     # init
     res_pos = 0
     sequences = {}
     parser = PDBParser()
 
+
+    # create a temp directory for tmp intermediate pdb file 
+    tmp_path = os.path.join(tempfile.gettempdir(), str(uuid.uuid1()))
+    os.makedirs(tmp_path, exist_ok=True)
+    
     # remove all the noisy lines such as HETATOMS etc.
-    tmp_in_pdb_file = os.path.join(tempfile.gettempdir(), "tmp.pdb")
+    tmp_in_pdb_file = os.path.join(tmp_path, os.path.basename(in_pdb_file))
     keep_only_atom_lines(in_pdb_file, tmp_in_pdb_file)
 
-    structure = parser.get_structure(tmp_in_pdb_file, tmp_in_pdb_file)
+    structure = parser.get_structure(id=tmp_in_pdb_file,
+                                     file=tmp_in_pdb_file)
     if chains:
         chains = set(chains)
     # iterate over structure
 
     for model in structure:
         for chain in model:
             chain_name = chain.get_id()
```

### Comparing `pdb-toolkit-0.3.1/pdb_toolkit/parser/split_residues_surface_boundary_core.py` & `pdb-toolkit-0.3.2/pdb_toolkit/parser/split_residues_surface_boundary_core.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3.1/pdb_toolkit/parser/steric_clashes.py` & `pdb-toolkit-0.3.2/pdb_toolkit/parser/steric_clashes.py`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3.1/pdb_toolkit.egg-info/SOURCES.txt` & `pdb-toolkit-0.3.2/pdb_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdb-toolkit-0.3.1/setup.py` & `pdb-toolkit-0.3.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup, find_packages
 
 
 # Read the contents of your README file
-with open('README.md', encoding='utf-8') as f:
-    description = f.read()
+with open('README.md', 'r') as f:
+    long_description = f.read()
 
 setup(
     name='pdb-toolkit',
-    version='0.3.1',
+    version='0.3.2',
     packages=find_packages(),
     url='https://github.com/raoufkeskes/pdb_toolkit',
     license='MIT Licence',
     author='raouf-ks',
     author_email='raouf.keskes@mabsilico.com',
-    description=description,
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     python_requires='>=3.6',
     install_requires=['wget'],
     classifiers=[
             "Programming Language :: Python :: 3",
             "License :: OSI Approved :: MIT License",
             "Operating System :: OS Independent"
         ],
```

