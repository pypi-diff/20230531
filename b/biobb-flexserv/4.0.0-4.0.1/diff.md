# Comparing `tmp/biobb_flexserv-4.0.0.tar.gz` & `tmp/biobb_flexserv-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biobb_flexserv-4.0.0.tar", last modified: Tue Apr 11 15:02:18 2023, max compression
+gzip compressed data, was "dist/biobb_flexserv-4.0.1.tar", last modified: Wed May 31 08:26:13 2023, max compression
```

## Comparing `biobb_flexserv-4.0.0.tar` & `biobb_flexserv-4.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11357 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/LICENSE
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      982 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5872 2023-04-11 15:01:07.000000 biobb_flexserv-4.0.0/README.md
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/biobb_flexserv/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       79 2023-04-11 15:00:50.000000 biobb_flexserv-4.0.0/biobb_flexserv/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/biobb_flexserv/flexserv/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       61 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/flexserv/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7225 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/flexserv/bd_run.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7731 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/flexserv/dmd_run.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7304 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/flexserv/nma_run.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      193 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6161 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_animate.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7558 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_bfactor.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6870 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_collectivity.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7235 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_evecs.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11403 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_hinges.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7907 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_info.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6805 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_lindemann.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    16439 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_similarity.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7511 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_stiffness.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6157 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_unzip.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7450 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_zip.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/biobb_flexserv.egg-info/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      982 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/biobb_flexserv.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      888 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/biobb_flexserv.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/biobb_flexserv.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      762 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/biobb_flexserv.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/biobb_flexserv.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       15 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/biobb_flexserv.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-04-11 15:02:18.000000 biobb_flexserv-4.0.0/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2331 2023-04-11 14:59:22.000000 biobb_flexserv-4.0.0/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11357 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.1/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1082 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5896 2023-05-31 08:24:53.000000 biobb_flexserv-4.0.1/README.md
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/biobb_flexserv/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       81 2023-05-31 08:23:56.000000 biobb_flexserv-4.0.1/biobb_flexserv/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/biobb_flexserv/flexserv/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       61 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.1/biobb_flexserv/flexserv/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7209 2023-04-13 07:06:13.000000 biobb_flexserv-4.0.1/biobb_flexserv/flexserv/bd_run.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7677 2023-04-13 07:06:13.000000 biobb_flexserv-4.0.1/biobb_flexserv/flexserv/dmd_run.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7432 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/flexserv/nma_run.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      194 2023-04-13 07:06:13.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7497 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_animate.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9623 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_bfactor.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8126 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_collectivity.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8444 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_evecs.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    12583 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_hinges.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9331 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_info.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8036 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_lindemann.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    18293 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_similarity.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8807 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_stiffness.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7450 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_unzip.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8897 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_zip.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/biobb_flexserv.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1082 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/biobb_flexserv.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      888 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/biobb_flexserv.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/biobb_flexserv.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      762 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/biobb_flexserv.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/biobb_flexserv.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       15 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/biobb_flexserv.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2429 2023-05-31 08:23:38.000000 biobb_flexserv-4.0.1/setup.py
```

### Comparing `biobb_flexserv-4.0.0/LICENSE` & `biobb_flexserv-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.0/PKG-INFO` & `biobb_flexserv-4.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: biobb_flexserv
-Version: 4.0.0
+Version: 4.0.1
 Summary: biobb_flexserv is a BioBB category for biomolecular flexibility studies on protein 3D structures.
 Home-page: https://github.com/bioexcel/biobb_flexserv
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
 Project-URL: Documentation, http://biobb_flexserv.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `biobb_flexserv-4.0.0/README.md` & `biobb_flexserv-4.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_flexserv?label=Version)](https://GitHub.com/bioexcel/biobb_flexserv/tags/)
 [![](https://img.shields.io/pypi/v/biobb-flexserv.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-flexserv/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_flexserv?label=Conda)](https://anaconda.org/bioconda/biobb_flexserv)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_flexserv?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_flexserv)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_flexserv?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_flexserv:4.0.0--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_flexserv:4.0.1--pypl5321hdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_flexserv)
 [![](https://img.shields.io/pypi/pyversions/biobb-flexserv.svg?label=Python%20Versions)](https://pypi.org/project/biobb-flexserv/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_flexserv)
 
 [![](https://readthedocs.org/projects/biobb-flexserv/badge/?version=latest&label=Docs)](https://biobb-flexserv.readthedocs.io/en/latest/?badge=latest)
@@ -31,60 +31,60 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb_flexserv.readthedocs.io/en/latest/).
 
 ### Version
-v4.0.0 2023.1
+v4.0.1 2023.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
 
-        pip install "biobb_flexserv>=4.0.0"
+        pip install "biobb_flexserv>=4.0.1"
 
 
 * Usage: [Python API documentation](https://biobb-flexserv.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_flexserv>=4.0.0"
+        conda install -c bioconda "biobb_flexserv>=4.0.1"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-flexserv.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-flexserv.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_flexserv:4.0.0--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_flexserv:4.0.1--pypl5321hdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_flexserv:4.0.0--pyhdfd78af_0
+        docker run quay.io/biocontainers/biobb_flexserv:4.0.1--pypl5321hdfd78af_0
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_flexserv.sif https://depot.galaxyproject.org/singularity/biobb_flexserv:4.0.0--pyhdfd78af_0
+        singularity pull --name biobb_flexserv.sif https://depot.galaxyproject.org/singularity/biobb_flexserv:4.0.1--pypl5321hdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_flexserv.sif <command>
```

### Comparing `biobb_flexserv-4.0.0/biobb_flexserv/flexserv/bd_run.py` & `biobb_flexserv-4.0.1/biobb_flexserv/flexserv/bd_run.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python3
 
 """Module containing the bd_run class and the command line interface."""
 import argparse
-from pathlib import Path, PurePath
+from pathlib import Path
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
+
 class BDRun(BiobbObject):
     """
     | biobb_flexserv BDRun
     | Wrapper of the Browian Dynamics tool from the FlexServ module.
     | Generates protein conformational structures using the Brownian Dynamics (BD) method.
 
     Args:
@@ -44,28 +45,27 @@
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
     def __init__(self, input_pdb_path: str, output_log_path: str,
-    output_crd_path: str, properties: dict = None, **kwargs) -> None:
+                 output_crd_path: str, properties: dict = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_pdb_path': input_pdb_path },
-            'out': {    'output_log_path': output_log_path,
-                        'output_crd_path': output_crd_path
-            }
+            'in': {'input_pdb_path': input_pdb_path},
+            'out': {'output_log_path': output_log_path,
+                    'output_crd_path': output_crd_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.binary_path = properties.get('binary_path', 'bd')
         self.time = properties.get('time', 1000000)
         self.dt = properties.get('dt', 1e-15)
@@ -76,15 +76,16 @@
         self.check_arguments()
 
     @launchlogger
     def launch(self):
         """Launches the execution of the FlexServ BDRun module."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # Internal file paths
         try:
             # Using rel paths to shorten the amount of characters due to fortran path length limitations
             input_pdb = str(Path(self.stage_io_dict["in"]["input_pdb_path"]).relative_to(Path.cwd()))
             output_crd = str(Path(self.stage_io_dict["out"]["output_crd_path"]).relative_to(Path.cwd()))
@@ -95,23 +96,23 @@
             output_crd = self.stage_io_dict["out"]["output_crd_path"]
             output_log = self.stage_io_dict["out"]["output_log_path"]
 
         # Command line
         # bd structure.ca.pdb 1000000 1e-15 1000 40 3.8 traj.crd > bd.log
         # itempsmax, dt, itsnap, const, r0
         self.cmd = [self.binary_path,
-                input_pdb,
-                str(self.time),
-                str(self.dt),
-                str(self.wfreq),
-                "40", # Hardcoded "Const", see https://mmb.irbbarcelona.org/gitlab/adam/FlexServ/blob/master/bd/bd2.f#L51 
-                "3.8", # Hardcoded "r0", see https://mmb.irbbarcelona.org/gitlab/adam/FlexServ/blob/master/bd/bd2.f#L52
-                output_crd,
-                '>',output_log
-               ]
+                    input_pdb,
+                    str(self.time),
+                    str(self.dt),
+                    str(self.wfreq),
+                    "40",  # Hardcoded "Const", see https://mmb.irbbarcelona.org/gitlab/adam/FlexServ/blob/master/bd/bd2.f#L51
+                    "3.8",  # Hardcoded "r0", see https://mmb.irbbarcelona.org/gitlab/adam/FlexServ/blob/master/bd/bd2.f#L52
+                    output_crd,
+                    '>', output_log
+                    ]
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
@@ -121,24 +122,26 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def bd_run(input_pdb_path: str,
-            output_log_path: str, output_crd_path: str,
-            properties: dict = None, **kwargs) -> int:
+           output_log_path: str, output_crd_path: str,
+           properties: dict = None, **kwargs) -> int:
     """Create :class:`BDRun <flexserv.bd_run.BDRun>`flexserv.bd_run.BDRun class and
     execute :meth:`launch() <flexserv.bd_run.BDRun.launch>` method"""
 
-    return BDRun(   input_pdb_path=input_pdb_path,
-                    output_log_path=output_log_path,
-                    output_crd_path=output_crd_path,
-                    properties=properties).launch()
+    return BDRun(input_pdb_path=input_pdb_path,
+                 output_log_path=output_log_path,
+                 output_crd_path=output_crd_path,
+                 properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Generates protein conformational structures using the Brownian Dynamics method.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -147,14 +150,15 @@
     required_args.add_argument('--output_crd_path', required=True, help='Output ensemble file. Accepted formats: crd, mdcrd, inpcrd.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call
-    bd_run(         input_pdb_path=args.input_pdb_path,
-                    output_log_path=args.output_log_path,
-                    output_crd_path=args.output_crd_path,
-                    properties=properties)
+    bd_run(input_pdb_path=args.input_pdb_path,
+           output_log_path=args.output_log_path,
+           output_crd_path=args.output_crd_path,
+           properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_flexserv-4.0.0/biobb_flexserv/flexserv/dmd_run.py` & `biobb_flexserv-4.0.1/biobb_flexserv/flexserv/dmd_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python3
 
 """Module containing the dmd_run class and the command line interface."""
 import argparse
-import shutil
 from pathlib import Path
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
+
 class DMDRun(BiobbObject):
     """
     | biobb_flexserv DMDRun
     | Wrapper of the Discrete Molecular Dynamics tool from the FlexServ module.
     | Generates protein conformational structures using the Discrete Molecular Dynamics (DMD) method.
 
     Args:
@@ -45,63 +45,63 @@
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
     def __init__(self, input_pdb_path: str, output_log_path: str,
-    output_crd_path: str, properties: dict = None, **kwargs) -> None:
+                 output_crd_path: str, properties: dict = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_pdb_path': input_pdb_path },
-            'out': {    'output_log_path': output_log_path,
-                        'output_crd_path': output_crd_path
-            }
+            'in': {'input_pdb_path': input_pdb_path},
+            'out': {'output_log_path': output_log_path,
+                    'output_crd_path': output_crd_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.binary_path = properties.get('binary_path', 'dmdgoopt')
-        #self.dt = properties.get('dt', 1.D-12)
+        # self.dt = properties.get('dt', 1.D-12)
         self.dt = properties.get('dt', 1e-12)
         self.temperature = properties.get('temperature', 300)
         self.frames = properties.get('frames', 1000)
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     @launchlogger
     def launch(self):
         """Launches the execution of the FlexServ BDRun module."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # Internal file paths
         try:
             # Using rel paths to shorten the amount of characters due to fortran path length limitations
             input_pdb = str(Path(self.stage_io_dict["in"]["input_pdb_path"]).relative_to(Path.cwd()))
             output_crd = str(Path(self.stage_io_dict["out"]["output_crd_path"]).relative_to(Path.cwd()))
             output_log = str(Path(self.stage_io_dict["out"]["output_log_path"]).relative_to(Path.cwd()))
         except ValueError:
             # Container or remote case
             input_pdb = self.stage_io_dict["in"]["input_pdb_path"]
             output_crd = self.stage_io_dict["out"]["output_crd_path"]
             output_log = self.stage_io_dict["out"]["output_log_path"]
 
-        # Config file
+        # Config file
         instructions_file = str(Path(self.stage_io_dict.get("unique_dir")).joinpath("dmd.in"))
         with open(instructions_file, 'w') as dmdin:
 
             dmdin.write("&INPUT\n")
             dmdin.write("  FILE9='{}',\n".format(input_pdb))
             dmdin.write("  FILE21='{}',\n".format(output_crd))
             dmdin.write("  TSNAP={},\n".format(self.dt))
@@ -112,19 +112,18 @@
             dmdin.write("  SIGMA=0.05,\n")
             dmdin.write("  SIGMAGO=0.1,\n")
             dmdin.write("  KKK=2839\n")
             dmdin.write("&END\n")
 
         # Command line
         # dmdgoopt < dmd.in > dmd.log
-        self.cmd = [ 
-                self.binary_path,
-                '<', instructions_file,
-                '>', output_log
-               ]
+        self.cmd = [self.binary_path,
+                    '<', instructions_file,
+                    '>', output_log
+                    ]
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
@@ -134,24 +133,26 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def dmd_run(input_pdb_path: str,
             output_log_path: str, output_crd_path: str,
             properties: dict = None, **kwargs) -> int:
     """Create :class:`DMDRun <flexserv.dmd_run.DMDRun>`flexserv.dmd_run.DMDRun class and
     execute :meth:`launch() <flexserv.dmd_run.DMDRun.launch>` method"""
 
-    return DMDRun(  input_pdb_path=input_pdb_path,
-                    output_log_path=output_log_path,
-                    output_crd_path=output_crd_path,
-                    properties=properties).launch()
+    return DMDRun(input_pdb_path=input_pdb_path,
+                  output_log_path=output_log_path,
+                  output_crd_path=output_crd_path,
+                  properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Generates protein conformational structures using the Discrete Molecular Dynamics method.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -160,14 +161,15 @@
     required_args.add_argument('--output_crd_path', required=True, help='Output ensemble file. Accepted formats: crd, mdcrd, inpcrd.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call
-    dmd_run(        input_pdb_path=args.input_pdb_path,
-                    output_log_path=args.output_log_path,
-                    output_crd_path=args.output_crd_path,
-                    properties=properties)
+    dmd_run(input_pdb_path=args.input_pdb_path,
+            output_log_path=args.output_log_path,
+            output_crd_path=args.output_crd_path,
+            properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `biobb_flexserv-4.0.0/biobb_flexserv/flexserv/nma_run.py` & `biobb_flexserv-4.0.1/biobb_flexserv/flexserv/nma_run.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 #!/usr/bin/env python3
 
 """Module containing the nma_run class and the command line interface."""
 import argparse
+import os
 from pathlib import Path
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
+
 class NMARun(BiobbObject):
     """
     | biobb_flexserv NMARun
     | Wrapper of the Normal Mode Analysis tool from the FlexServ module.
     | Generates protein conformational structures using the Normal Mode Analysis (NMA) method.
 
     Args:
         input_pdb_path (str): Input PDB file. File type: input. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/data/flexserv/structure.ca.pdb>`_. Accepted formats: pdb (edam:format_1476).
         output_log_path (str): Output log file. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/reference/flexserv/nma_run_out.log>`_. Accepted formats: log (edam:format_2330), out (edam:format_2330), txt (edam:format_2330), o (edam:format_2330).
         output_crd_path (str): Output ensemble. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/reference/flexserv/nma_run_out.crd>`_. Accepted formats: crd (edam:format_3878), mdcrd (edam:format_3878), inpcrd (edam:format_3878).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
-            * **binary_path** (*str*) - ("bd") BD binary path to be used.
+            * **binary_path** (*str*) - ("diaghess") NMA binary path to be used.
             * **frames** (*int*) - (1000) Number of frames in the final ensemble
             * **nvecs** (*int*) - (50) Number of vectors to take into account for the ensemble generation
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
 
     Examples:
         This is a use example of how to use the building block from Python::
@@ -43,28 +45,27 @@
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
     def __init__(self, input_pdb_path: str, output_log_path: str,
-    output_crd_path: str, properties: dict = None, **kwargs) -> None:
+                 output_crd_path: str, properties: dict = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 'input_pdb_path': input_pdb_path },
-            'out': {    'output_log_path': output_log_path,
-                        'output_crd_path': output_crd_path
-            }
+            'in': {'input_pdb_path': input_pdb_path},
+            'out': {'output_log_path': output_log_path,
+                    'output_crd_path': output_crd_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.binary_path = properties.get('binary_path', 'diaghess')
         self.frames = properties.get('frames', 1000)
         self.nvecs = properties.get('nvecs', 50)
@@ -74,15 +75,16 @@
         self.check_arguments()
 
     @launchlogger
     def launch(self):
         """Launches the execution of the FlexServ NMARun module."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
+        if self.check_restart():
+            return 0
         self.stage_files()
 
         # Internal file paths
         try:
             # Using rel paths to shorten the amount of characters due to fortran path length limitations
             input_pdb = str(Path(self.stage_io_dict["in"]["input_pdb_path"]).relative_to(Path.cwd()))
             output_crd = str(Path(self.stage_io_dict["out"]["output_crd_path"]).relative_to(Path.cwd()))
@@ -90,31 +92,33 @@
         except ValueError:
             # Container or remote case
             input_pdb = self.stage_io_dict["in"]["input_pdb_path"]
             output_crd = self.stage_io_dict["out"]["output_crd_path"]
             output_log = self.stage_io_dict["out"]["output_log_path"]
 
         # Command line
-        #nmanu.pl structure.ca.pdb hessian.dat 1 0 40
-        #diaghess
-        #mc-eigen.pl eigenvec.dat > file.proj
-        #pca_anim_mc.pl -pdb structure.ca.pdb -evec eigenvec.dat -i file.proj -n 50 -pout traj.crd
-        self.cmd = [ 
-                "nmanu.pl ",
-                input_pdb,
-                "hessian.dat 1 0 40;",
-                self.binary_path,
-                "; mc-eigen-mdweb.pl eigenvec.dat ", str(self.frames), " > file.proj",
-                "; pca_anim_mc.pl -pdb",
-                input_pdb,
-                " -evec eigenvec.dat -i file.proj -n ",
-                str(self.nvecs),
-                " -pout",  output_crd,
-                '>', output_log
-               ]
+        # nmanu.pl structure.ca.pdb hessian.dat 1 0 40
+        # diaghess
+        # mc-eigen.pl eigenvec.dat > file.proj
+        # pca_anim_mc.pl -pdb structure.ca.pdb -evec eigenvec.dat -i file.proj -n 50 -pout traj.crd
+        conda_path = os.getenv("CONDA_PREFIX")
+        nmanu = conda_path + "/bin/nmanu.pl"
+        self.cmd = ["perl ",
+                    nmanu,
+                    input_pdb,
+                    "hessian.dat 1 0 40;",
+                    self.binary_path,
+                    "; mc-eigen-mdweb.pl eigenvec.dat ", str(self.frames), " > file.proj",
+                    "; pca_anim_mc.pl -pdb",
+                    input_pdb,
+                    " -evec eigenvec.dat -i file.proj -n ",
+                    str(self.nvecs),
+                    " -pout", output_crd,
+                    '>', output_log
+                    ]
 
         # Run Biobb block
         self.run_biobb()
 
         # Copy files to host
         self.copy_to_host()
 
@@ -124,24 +128,26 @@
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def nma_run(input_pdb_path: str,
             output_log_path: str, output_crd_path: str,
             properties: dict = None, **kwargs) -> int:
     """Create :class:`NMARun <flexserv.nma_run.NMARun>`flexserv.nma_run.NMARun class and
     execute :meth:`launch() <flexserv.nma_run.NMARun.launch>` method"""
 
-    return NMARun( input_pdb_path=input_pdb_path,
-                    output_log_path=output_log_path,
-                    output_crd_path=output_crd_path,
-                    properties=properties).launch()
+    return NMARun(input_pdb_path=input_pdb_path,
+                  output_log_path=output_log_path,
+                  output_crd_path=output_crd_path,
+                  properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Generates protein conformational structures using the Normal Mode Analysis method.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -150,14 +156,15 @@
     required_args.add_argument('--output_crd_path', required=True, help='Output ensemble file. Accepted formats: crd, mdcrd, inpcrd.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call
-    nma_run(        input_pdb_path=args.input_pdb_path,
-                    output_log_path=args.output_log_path,
-                    output_crd_path=args.output_crd_path,
-                    properties=properties)
+    nma_run(input_pdb_path=args.input_pdb_path,
+            output_log_path=args.output_log_path,
+            output_crd_path=args.output_crd_path,
+            properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_animate.py` & `biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_animate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 #!/usr/bin/env python3
 
 """Module containing the PCZanimate class and the command line interface."""
 import argparse
 import shutil
-from pathlib import Path
+from pathlib import PurePath
+from biobb_common.tools import file_utils as fu
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
+
 class PCZanimate(BiobbObject):
     """
     | biobb_flexserv PCZanimate
     | Extract PCA animations from a compressed PCZ file.
     | Wrapper of the pczdump tool from the PCAsuite FlexServ module.
 
     Args:
@@ -42,31 +44,27 @@
             * version: >=1.0
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
-    def __init__(self, input_pcz_path: str, 
-    output_crd_path: str, properties: dict = None, **kwargs) -> None:
+    def __init__(self, input_pcz_path: str,
+                 output_crd_path: str, properties: dict = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 
-                'input_pcz_path': input_pcz_path
-             },
-            'out': {    
-                'output_crd_path': output_crd_path
-            }
+            'in': {'input_pcz_path': input_pcz_path},
+            'out': {'output_crd_path': output_crd_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.binary_path = properties.get('binary_path', 'pczdump')
         self.eigenvector = properties.get('eigenvector', 1)
         self.pdb = properties.get('pdb', False)
@@ -76,63 +74,88 @@
         self.check_arguments()
 
     @launchlogger
     def launch(self):
         """Launches the execution of the FlexServ pcz_animate module."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
-        self.stage_files()
+        if self.check_restart():
+            return 0
+        # self.stage_files()
+
+        # # Internal file paths
+        # try:
+        #     # Using rel paths to shorten the amount of characters due to fortran path length limitations
+        #     input_pcz = str(Path(self.stage_io_dict["in"]["input_pcz_path"]).relative_to(Path.cwd()))
+        #     output_crd = str(Path(self.stage_io_dict["out"]["output_crd_path"]).relative_to(Path.cwd()))
+        # except ValueError:
+        #     # Container or remote case
+        #     input_pcz = self.stage_io_dict["in"]["input_pcz_path"]
+        #     output_crd = self.stage_io_dict["out"]["output_crd_path"]
+
+        # Manually creating a Sandbox to avoid issues with input parameters buffer overflow:
+        #   Long strings defining a file path makes Fortran or C compiled programs crash if the string
+        #   declared is shorter than the input parameter path (string) length.
+        #   Generating a temporary folder and working inside this folder (sandbox) fixes this problem.
+        #   The problem was found in Galaxy executions, launching Singularity containers (May 2023).
+
+        # Creating temporary folder
+        self.tmp_folder = fu.create_unique_dir()
+        fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
 
-        # Internal file paths
-        try:
-            # Using rel paths to shorten the amount of characters due to fortran path length limitations
-            input_pcz = str(Path(self.stage_io_dict["in"]["input_pcz_path"]).relative_to(Path.cwd()))
-            output_crd = str(Path(self.stage_io_dict["out"]["output_crd_path"]).relative_to(Path.cwd()))
-        except ValueError:
-            # Container or remote case
-            input_pcz = self.stage_io_dict["in"]["input_pcz_path"]
-            output_crd = self.stage_io_dict["out"]["output_crd_path"]
+        shutil.copy2(self.io_dict["in"]["input_pcz_path"], self.tmp_folder)
 
         # Command line
         # pczdump -i structure.ca.std.pcz --anim=1 --pdb -o anim_1.pdb
-        self.cmd = [self.binary_path,
-                "-i", input_pcz,
-                "-o", output_crd,
-                "--anim={}".format(self.eigenvector)
-               ]
- 
+        # self.cmd = [self.binary_path,
+        #             "-i", input_pcz,
+        #             "-o", output_crd,
+        #             "--anim={}".format(self.eigenvector)
+        #             ]
+
+        self.cmd = ['cd', self.tmp_folder, ';',
+                    self.binary_path,
+                    '-i', PurePath(self.io_dict["in"]["input_pcz_path"]).name,
+                    '-o', PurePath(self.io_dict["out"]["output_crd_path"]).name,
+                    "--anim={}".format(self.eigenvector)
+                    ]
+
         if self.pdb:
             self.cmd.append('--pdb')
 
         # Run Biobb block
         self.run_biobb()
 
+        # Copy outputs from temporary folder to output path
+        shutil.copy2(PurePath(self.tmp_folder).joinpath(PurePath(self.io_dict["out"]["output_crd_path"]).name), PurePath(self.io_dict["out"]["output_crd_path"]))
+
         # Copy files to host
-        self.copy_to_host()
+        # self.copy_to_host()
 
         # remove temporary folder(s)
         self.tmp_files.extend([
-            self.stage_io_dict.get("unique_dir")
+            # self.stage_io_dict.get("unique_dir"),
+            self.tmp_folder
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def pcz_animate(input_pcz_path: str, output_crd_path: str,
-            properties: dict = None, **kwargs) -> int:
+                properties: dict = None, **kwargs) -> int:
     """Create :class:`PCZanimate <flexserv.pcasuite.pcz_animate>`flexserv.pcasuite.PCZanimate class and
     execute :meth:`launch() <flexserv.pcasuite.pcz_animate.launch>` method"""
 
-    return PCZanimate(  
-                    input_pcz_path=input_pcz_path,
-                    output_crd_path=output_crd_path,
-                    properties=properties).launch()
+    return PCZanimate(input_pcz_path=input_pcz_path,
+                      output_crd_path=output_crd_path,
+                      properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Extract PCA animations from a compressed PCZ file.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -140,13 +163,14 @@
     required_args.add_argument('--output_crd_path', required=True, help='Output animated trajectory file. Accepted formats: crd, mdcrd, inpcrd, pdb.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call
-    pcz_animate(    input_pcz_path=args.input_pcz_path,
-                    output_crd_path=args.output_crd_path,
-                    properties=properties)
+    pcz_animate(input_pcz_path=args.input_pcz_path,
+                output_crd_path=args.output_crd_path,
+                properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_bfactor.py` & `biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_zip.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,171 +1,201 @@
 #!/usr/bin/env python3
 
-"""Module containing the PCZbfactor class and the command line interface."""
+"""Module containing the PCAzip class and the command line interface."""
 import argparse
-from pathlib import Path
+import shutil
+from pathlib import PurePath
+from biobb_common.tools import file_utils as fu
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
-class PCZbfactor(BiobbObject):
+
+class PCZzip(BiobbObject):
     """
-    | biobb_flexserv PCZbfactor
-    | Extract residue bfactors x PCA mode from a compressed PCZ file.
-    | Wrapper of the pczdump tool from the PCAsuite FlexServ module.
+    | biobb_flexserv PCZzip
+    | Wrapper of the pcazip tool from the PCAsuite FlexServ module.
+    | Compress Molecular Dynamics (MD) trajectories using Principal Component Analysis (PCA) algorithms.
 
     Args:
-        input_pcz_path (str): Input compressed trajectory file. File type: input. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/data/pcasuite/pcazip.pcz>`_. Accepted formats: pcz (edam:format_3874).
-        output_dat_path (str): Output Bfactor x residue x PCA mode file. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/reference/pcasuite/bfactors.dat>`_. Accepted formats: dat (edam:format_1637), txt (edam:format_2330), csv (edam:format_3752).
-        output_pdb_path (str) (Optional): Output PDB with Bfactor x residue x PCA mode file. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/reference/pcasuite/bfactors.pdb>`_. Accepted formats: pdb (edam:format_1476).
+        input_pdb_path (str): Input PDB file. File type: input. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/data/pcasuite/structure.ca.pdb>`_. Accepted formats: pdb (edam:format_1476).
+        input_crd_path (str): Input Trajectory file. File type: input. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/data/pcasuite/traj.crd>`_. Accepted formats: crd (edam:format_3878), mdcrd (edam:format_3878), inpcrd (edam:format_3878).
+        output_pcz_path (str): Output compressed trajectory. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/reference/pcasuite/pcazip.pcz>`_. Accepted formats: pcz (edam:format_3874).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
-            * **binary_path** (*str*) - ("pczdump") pczdump binary path to be used.
-            * **eigenvector** (*int*) - (0) PCA mode (eigenvector) from which to extract bfactor values per residue (0 means average over all modes).
-            * **pdb** (*bool*) - (False) Generate a PDB file with the computed bfactors (to be easily represented with colour scale) 
+            * **binary_path** (*str*) - ("pcazip") pcazip binary path to be used.
+            * **neigenv** (*int*) - (0) Number of generated eigenvectors
+            * **variance** (*int*) - (90) Percentage of variance captured by the final set of eigenvectors
+            * **verbose** (*bool*) - (False) Make output verbose
+            * **gauss_rmsd** (*bool*) - (False) Use a gaussian RMSd for fitting
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
-            from biobb_flexserv.pcasuite.pcz_bfactor import pcz_bfactor
+            from biobb_flexserv.pcasuite.pcz_zip import pcz_zip
             prop = {
-                'eigenvector': 1,
-                'pdb': True
+                'variance': 90
             }
-            pcz_bfactor( input_pcz_path='/path/to/pcazip_input.pcz',
-                    output_dat_path='/path/to/bfactors_mode1.dat',
-                    output_pdb_path='/path/to/bfactors_mode1.pdb',
+            pcz_zip( input_pdb_path='/path/to/pcazip_input.pdb',
+                    input_crd_path='/path/to/pcazip_input.crd',
+                    output_pcz_path='/path/to/pcazip_traj.pcz',
                     properties=prop)
 
     Info:
         * wrapped_software:
             * name: FlexServ PCAsuite
             * version: >=1.0
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
-    def __init__(self, input_pcz_path: str, output_dat_path: str,
-    output_pdb_path: str, properties: dict = None, **kwargs) -> None:
+    def __init__(self, input_pdb_path: str, input_crd_path: str,
+                 output_pcz_path: str, properties: dict = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 
-                'input_pcz_path': input_pcz_path
-             },
-            'out': {    
-                'output_dat_path': output_dat_path,
-                'output_pdb_path': output_pdb_path
-            }
+            'in': {'input_pdb_path': input_pdb_path,
+                   'input_crd_path': input_crd_path},
+            'out': {'output_pcz_path': output_pcz_path}
         }
 
         # Properties specific for BB
         self.properties = properties
-        self.binary_path = properties.get('binary_path', 'pczdump')
-        self.eigenvector = properties.get('eigenvector', 1)
-        self.pdb = properties.get('pdb', False)
+        self.binary_path = properties.get('binary_path', 'pcazip')
+        self.neigenv = properties.get('neigenv', 0)
+        # self.variance = properties.get('variance', 90)
+        self.variance = properties.get('variance')
+        self.verbose = properties.get('verbose', False)
+        self.gauss_rmsd = properties.get('gauss_rmsd', False)
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     @launchlogger
     def launch(self):
-        """Launches the execution of the FlexServ pcz_bfactor module."""
+        """Launches the execution of the FlexServ pcazip module."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
-        self.stage_files()
+        if self.check_restart():
+            return 0
+        # self.stage_files()
+
+        # try:
+        #     # Using rel paths to shorten the amount of characters due to fortran path length limitations
+        #     input_pdb = str(Path(self.stage_io_dict["in"]["input_pdb_path"]).relative_to(Path.cwd()))
+        #     input_crd = str(Path(self.stage_io_dict["in"]["input_crd_path"]).relative_to(Path.cwd()))
+        #     output_pcz = str(Path(self.stage_io_dict["out"]["output_pcz_path"]).relative_to(Path.cwd()))
+        # except ValueError:
+        #     # Container or remote case
+        #     input_pdb = self.stage_io_dict["in"]["input_pdb_path"]
+        #     input_crd = self.stage_io_dict["in"]["input_crd_path"]
+        #     output_pcz = self.stage_io_dict["out"]["output_pcz_path"]
+
+        # Manually creating a Sandbox to avoid issues with input parameters buffer overflow:
+        #   Long strings defining a file path makes Fortran or C compiled programs crash if the string
+        #   declared is shorter than the input parameter path (string) length.
+        #   Generating a temporary folder and working inside this folder (sandbox) fixes this problem.
+        #   The problem was found in Galaxy executions, launching Singularity containers (May 2023).
+
+        # Creating temporary folder
+        self.tmp_folder = fu.create_unique_dir()
+        fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
+
+        shutil.copy2(self.io_dict["in"]["input_pdb_path"], self.tmp_folder)
+        shutil.copy2(self.io_dict["in"]["input_crd_path"], self.tmp_folder)
+
+        # Command line
+        # pcazip -i infile -o outfile -n natoms
+        # [-v] [--mask maskfile] [-e nev] [-q qual] [--pdb pdbfile]
+        # self.cmd = [self.binary_path,
+        #             "-p", input_pdb,
+        #             "-i", input_crd,
+        #             "-o", output_pcz
+        #             ]
+
+        self.cmd = ['cd', self.tmp_folder, ';',
+                    self.binary_path,
+                    "-p", PurePath(self.io_dict["in"]["input_pdb_path"]).name,
+                    "-i", PurePath(self.io_dict["in"]["input_crd_path"]).name,
+                    "-o", PurePath(self.io_dict["out"]["output_pcz_path"]).name
+                    ]
+
+        if self.verbose:
+            self.cmd.append('-v')
+
+        if self.gauss_rmsd:
+            self.cmd.append('-g')
+
+        if self.neigenv:
+            self.cmd.append('-e')
+            self.cmd.append(str(self.neigenv))
+
+        if self.variance:
+            self.cmd.append('-q')
+            self.cmd.append(str(self.variance))
 
-        # Internal file paths
-        try:
-            # Using rel paths to shorten the amount of characters due to fortran path length limitations
-            input_pcz = str(Path(self.stage_io_dict["in"]["input_pcz_path"]).relative_to(Path.cwd()))
-            output_pdb = str(Path(self.stage_io_dict["out"]["output_pdb_path"]).relative_to(Path.cwd()))
-            output_dat = str(Path(self.stage_io_dict["out"]["output_dat_path"]).relative_to(Path.cwd()))
-        except ValueError:
-            # Container or remote case
-            input_pcz = self.stage_io_dict["in"]["input_pcz_path"]
-            output_pdb = self.stage_io_dict["out"]["output_pdb_path"]
-            output_dat = self.stage_io_dict["out"]["output_dat_path"]
-
-        # Command line (1: dat file)
-        # pczdump -i structure.ca.std.pcz --fluc=1 -o bfactor_1.dat
-        self.cmd = [self.binary_path,
-                "-i", input_pcz,
-                "-o", output_dat,
-                "--bfactor",
-                "--fluc={}".format(self.eigenvector)
-               ]
-  
         # Run Biobb block
         self.run_biobb()
 
-        if self.pdb:
-            # Command line (2: pdb file)
-            # pczdump -i structure.ca.std.pcz --fluc=1 --pdb -o bfactor_1.pdb
-            self.cmd = [self.binary_path,
-                "-i", input_pcz,
-                "-o", output_pdb,
-                "--bfactor",
-                "--fluc={}".format(self.eigenvector),
-                "--pdb"
-               ]
-
-            # Run Biobb block
-            self.run_biobb()
+        # Copy outputs from temporary folder to output path
+        shutil.copy2(PurePath(self.tmp_folder).joinpath(PurePath(self.io_dict["out"]["output_pcz_path"]).name), PurePath(self.io_dict["out"]["output_pcz_path"]))
 
         # Copy files to host
-        self.copy_to_host()
+        # self.copy_to_host()
 
         # remove temporary folder(s)
         self.tmp_files.extend([
-            self.stage_io_dict.get("unique_dir")
+            # self.stage_io_dict.get("unique_dir"),
+            self.tmp_folder
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
-def pcz_bfactor(input_pcz_path: str, output_dat_path: str, output_pdb_path: str,
+
+def pcz_zip(input_pdb_path: str, input_crd_path: str,
+            output_pcz_path: str,
             properties: dict = None, **kwargs) -> int:
-    """Create :class:`PCZbfactor <flexserv.pcasuite.pcz_bfactor>`flexserv.pcasuite.PCZbfactor class and
-    execute :meth:`launch() <flexserv.pcasuite.pcz_bfactor.launch>` method"""
+    """Create :class:`PCZzip <flexserv.pcasuite.PCZzip>`flexserv.pcasuite.PCZzip class and
+    execute :meth:`launch() <flexserv.pcasuite.PCZzip.launch>` method"""
+
+    return PCZzip(input_pdb_path=input_pdb_path,
+                  input_crd_path=input_crd_path,
+                  output_pcz_path=output_pcz_path,
+                  properties=properties).launch()
 
-    return PCZbfactor(  
-                    input_pcz_path=input_pcz_path,
-                    output_dat_path=output_dat_path,
-                    output_pdb_path=output_pdb_path,
-                    properties=properties).launch()
 
 def main():
-    parser = argparse.ArgumentParser(description='Extract residue bfactors x PCA mode from a compressed PCZ file.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
+    parser = argparse.ArgumentParser(description='Compress Molecular Dynamics (MD) trajectories using Principal Component Analysis (PCA) algorithms.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
-    required_args.add_argument('--input_pcz_path', required=True, help='Input compressed trajectory file. Accepted formats: pcz.')
-    required_args.add_argument('--output_dat_path', required=True, help='Output Bfactor x residue x PCA mode file. Accepted formats: dat, txt, csv.')
-    required_args.add_argument('--output_pdb_path', required=False, help='Output PDB with Bfactor x residue x PCA mode file. Accepted formats: pdb.')
+    required_args.add_argument('--input_pdb_path', required=True, help='Input PDB file. Accepted formats: pdb.')
+    required_args.add_argument('--input_crd_path', required=True, help='Input trajectory file. Accepted formats: crd, mdcrd, inpcrd.')
+    required_args.add_argument('--output_pcz_path', required=True, help='Output compressed trajectory file. Accepted formats: pcz.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call
-    pcz_bfactor(    input_pcz_path=args.input_pcz_path,
-                    output_dat_path=args.output_dat_path,
-                    output_pdb_path=args.output_pdb_path,
-                    properties=properties)
+    pcz_zip(input_pdb_path=args.input_pdb_path,
+            input_crd_path=args.input_crd_path,
+            output_pcz_path=args.output_pcz_path,
+            properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_collectivity.py` & `biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_collectivity.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 #!/usr/bin/env python3
 
 """Module containing the PCZcollectivity class and the command line interface."""
 import argparse
+import shutil
+from pathlib import PurePath
+from biobb_common.tools import file_utils as fu
 import json
-from pathlib import Path
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
+
 class PCZcollectivity(BiobbObject):
     """
     | biobb_flexserv PCZcollectivity
     | Extract PCA collectivity (numerical measure of how many atoms are affected by a given mode) from a compressed PCZ file.
     | Wrapper of the pczdump tool from the PCAsuite FlexServ module.
 
     Args:
@@ -42,31 +45,27 @@
             * version: >=1.0
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
-    def __init__(self, input_pcz_path: str, 
-    output_json_path: str, properties: dict = None, **kwargs) -> None:
+    def __init__(self, input_pcz_path: str,
+                 output_json_path: str, properties: dict = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 
-                'input_pcz_path': input_pcz_path
-             },
-            'out': {    
-                'output_json_path': output_json_path
-            }
+            'in': {'input_pcz_path': input_pcz_path},
+            'out': {'output_json_path': output_json_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.binary_path = properties.get('binary_path', 'pczdump')
         self.eigenvector = properties.get('eigenvector', 0)
 
@@ -75,83 +74,104 @@
         self.check_arguments()
 
     @launchlogger
     def launch(self):
         """Launches the execution of the FlexServ pcz_collectivity module."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
-        self.stage_files()
+        if self.check_restart():
+            return 0
+        # self.stage_files()
 
         # Internal file paths
-        try:
-            # Using rel paths to shorten the amount of characters due to fortran path length limitations
-            input_pcz = str(Path(self.stage_io_dict["in"]["input_pcz_path"]).relative_to(Path.cwd()))
-            output_json = str(Path(self.stage_io_dict["out"]["output_json_path"]).relative_to(Path.cwd()))
-        except ValueError:
-            # Container or remote case
-            input_pcz = self.stage_io_dict["in"]["input_pcz_path"]
-            output_json = self.stage_io_dict["out"]["output_json_path"]
+        # try:
+        #     # Using rel paths to shorten the amount of characters due to fortran path length limitations
+        #     input_pcz = str(Path(self.stage_io_dict["in"]["input_pcz_path"]).relative_to(Path.cwd()))
+        #     output_json = str(Path(self.stage_io_dict["out"]["output_json_path"]).relative_to(Path.cwd()))
+        # except ValueError:
+        #     # Container or remote case
+        #     input_pcz = self.stage_io_dict["in"]["input_pcz_path"]
+        #     output_json = self.stage_io_dict["out"]["output_json_path"]
+
+        # Manually creating a Sandbox to avoid issues with input parameters buffer overflow:
+        #   Long strings defining a file path makes Fortran or C compiled programs crash if the string
+        #   declared is shorter than the input parameter path (string) length.
+        #   Generating a temporary folder and working inside this folder (sandbox) fixes this problem.
+        #   The problem was found in Galaxy executions, launching Singularity containers (May 2023).
+
+        # Creating temporary folder
+        self.tmp_folder = fu.create_unique_dir()
+        fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
+
+        shutil.copy2(self.io_dict["in"]["input_pcz_path"], self.tmp_folder)
 
         # Temporary output
-        temp_out = str(Path(self.stage_io_dict.get("unique_dir")).joinpath("output.dat"))
+        # temp_out = str(Path(self.stage_io_dict.get("unique_dir")).joinpath("output.dat"))
+        temp_out = "output.dat"
+        temp_json = "output.json"
 
         # Command line
         # pczdump -i structure.ca.std.pcz --collectivity -o pcz.collectivity
-        self.cmd = [self.binary_path,
-                "-i", input_pcz,
-                "-o", temp_out,
-                "--collectivity={}".format(self.eigenvector)
-               ]
- 
+        # self.cmd = [self.binary_path,
+        #             "-i", input_pcz,
+        #             "-o", temp_out,
+        #             "--collectivity={}".format(self.eigenvector)
+        #             ]
+
+        self.cmd = ['cd', self.tmp_folder, ';',
+                    self.binary_path,
+                    '-i', PurePath(self.io_dict["in"]["input_pcz_path"]).name,
+                    '-o', temp_out,
+                    "--collectivity={}".format(self.eigenvector)
+                    ]
+
         # Run Biobb block
         self.run_biobb()
 
         # Parse output collectivity
-           #  0.132891
-           #  0.165089
-           #  0.147202
+        #  0.132891
+        #  0.165089
+        #  0.147202
         info_dict = {}
         info_dict['collectivity'] = []
-        with open (temp_out,'r') as file:
+        with open(PurePath(self.tmp_folder).joinpath(temp_out), 'r') as file:
             for line in file:
                 info = float(line.strip())
                 info_dict['collectivity'].append(info)
-       
-        # convert into JSON:
-        y = json.dumps(info_dict)
-
-        ## the result is a JSON string:
-        print(json.dumps(info_dict, indent=4))
 
-        with open (output_json,'w') as out_file:
+        with open(PurePath(self.tmp_folder).joinpath(temp_json), 'w') as out_file:
             out_file.write(json.dumps(info_dict, indent=4))
 
+        # Copy outputs from temporary folder to output path
+        shutil.copy2(PurePath(self.tmp_folder).joinpath(temp_json), PurePath(self.io_dict["out"]["output_json_path"]))
+
         # Copy files to host
-        self.copy_to_host()
+        # self.copy_to_host()
 
         # remove temporary folder(s)
         self.tmp_files.extend([
-            self.stage_io_dict.get("unique_dir")
+            # self.stage_io_dict.get("unique_dir"),
+            self.tmp_folder
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def pcz_collectivity(input_pcz_path: str, output_json_path: str,
-            properties: dict = None, **kwargs) -> int:
+                     properties: dict = None, **kwargs) -> int:
     """Create :class:`PCZcollectivity <flexserv.pcasuite.pcz_collectivity>`flexserv.pcasuite.PCZcollectivity class and
     execute :meth:`launch() <flexserv.pcasuite.pcz_collectivity.launch>` method"""
 
-    return PCZcollectivity(  
-                    input_pcz_path=input_pcz_path,
-                    output_json_path=output_json_path,
-                    properties=properties).launch()
+    return PCZcollectivity(input_pcz_path=input_pcz_path,
+                           output_json_path=output_json_path,
+                           properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Extract PCA collectivity (numerical measure of how many atoms are affected by a given mode) from a compressed PCZ file.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -159,13 +179,14 @@
     required_args.add_argument('--output_json_path', required=True, help='Output json file with PCA collectivity. Accepted formats: json.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call
-    pcz_collectivity(   input_pcz_path=args.input_pcz_path,
-                        output_json_path=args.output_json_path,
-                        properties=properties)
+    pcz_collectivity(input_pcz_path=args.input_pcz_path,
+                     output_json_path=args.output_json_path,
+                     properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_evecs.py` & `biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_lindemann.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,188 +1,190 @@
 #!/usr/bin/env python3
 
-"""Module containing the PCZevecs class and the command line interface."""
+"""Module containing the PCZlindemann class and the command line interface."""
 import argparse
-import json, math
-from pathlib import Path
+import shutil
+import json
+from pathlib import PurePath
+from biobb_common.tools import file_utils as fu
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
-class PCZevecs(BiobbObject):
+
+class PCZlindemann(BiobbObject):
     """
-    | biobb_flexserv PCZevecs
-    | Extract PCA Eigen Vectors from a compressed PCZ file.
+    | biobb_flexserv PCZlindemann
+    | Extract Lindemann coefficient (an estimate of the solid-liquid behaviour of a protein) from a compressed PCZ file.
     | Wrapper of the pczdump tool from the PCAsuite FlexServ module.
 
     Args:
         input_pcz_path (str): Input compressed trajectory file. File type: input. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/data/pcasuite/pcazip.pcz>`_. Accepted formats: pcz (edam:format_3874).
-        output_json_path (str): Output json file with PCA Eigen Vectors. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/reference/pcasuite/pcz_evecs.json>`_. Accepted formats: json (edam:format_3464).
+        output_json_path (str): Output json file with PCA Eigen Vectors. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/reference/pcasuite/pcz_lindemann.json>`_. Accepted formats: json (edam:format_3464).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
             * **binary_path** (*str*) - ("pczdump") pczdump binary path to be used.
-            * **eigenvector** (*int*) - (1) PCA mode (eigenvector) from which to extract eigen vectors.
+            * **mask** (*str*) - ("all atoms") Residue mask, in the format ":resnum1, resnum2, resnum3" (e.g. ":10,21,33"). See https://mmb.irbbarcelona.org/software/pcasuite/ for the complete format specification.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
-            from biobb_flexserv.pcasuite.pcz_evecs import pcz_evecs
-
+            from biobb_flexserv.pcasuite.pcz_lindemann import pcz_lindemann
             prop = {
-                'eigenvector': 1
+                'mask': ':10,12,15'
             }
-
-            pcz_evecs( input_pcz_path='/path/to/pcazip_input.pcz',
-                    output_json_path='/path/to/pcz_evecs.json',
+            pcz_lindemann( input_pcz_path='/path/to/pcazip_input.pcz',
+                    output_json_path='/path/to/lindemann_report.json',
                     properties=prop)
 
     Info:
         * wrapped_software:
             * name: FlexServ PCAsuite
             * version: >=1.0
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
-    def __init__(self, input_pcz_path: str, 
-    output_json_path: str, properties: dict = None, **kwargs) -> None:
+    def __init__(self, input_pcz_path: str,
+                 output_json_path: str, properties: dict = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 
-                'input_pcz_path': input_pcz_path
-             },
-            'out': {    
-                'output_json_path': output_json_path
-            }
+            'in': {'input_pcz_path': input_pcz_path},
+            'out': {'output_json_path': output_json_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.binary_path = properties.get('binary_path', 'pczdump')
-        self.eigenvector = properties.get('eigenvector', 1)
+        self.mask = properties.get('mask', '')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     @launchlogger
     def launch(self):
-        """Launches the execution of the FlexServ pcz_evecs module."""
+        """Launches the execution of the FlexServ pcz_lindemann module."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
-        self.stage_files()
+        if self.check_restart():
+            return 0
+        # self.stage_files()
 
         # Internal file paths
-        try:
-            # Using rel paths to shorten the amount of characters due to fortran path length limitations
-            input_pcz = str(Path(self.stage_io_dict["in"]["input_pcz_path"]).relative_to(Path.cwd()))
-            output_json = str(Path(self.stage_io_dict["out"]["output_json_path"]).relative_to(Path.cwd()))
-        except ValueError:
-            # Container or remote case
-            input_pcz = self.stage_io_dict["in"]["input_pcz_path"]
-            output_json = self.stage_io_dict["out"]["output_json_path"]
+        # try:
+        #     # Using rel paths to shorten the amount of characters due to fortran path length limitations
+        #     input_pcz = str(Path(self.stage_io_dict["in"]["input_pcz_path"]).relative_to(Path.cwd()))
+        #     output_json = str(Path(self.stage_io_dict["out"]["output_json_path"]).relative_to(Path.cwd()))
+        # except ValueError:
+        #     # Container or remote case
+        #     input_pcz = self.stage_io_dict["in"]["input_pcz_path"]
+        #     output_json = self.stage_io_dict["out"]["output_json_path"]
+
+        # Manually creating a Sandbox to avoid issues with input parameters buffer overflow:
+        #   Long strings defining a file path makes Fortran or C compiled programs crash if the string
+        #   declared is shorter than the input parameter path (string) length.
+        #   Generating a temporary folder and working inside this folder (sandbox) fixes this problem.
+        #   The problem was found in Galaxy executions, launching Singularity containers (May 2023).
+
+        # Creating temporary folder
+        self.tmp_folder = fu.create_unique_dir()
+        fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
+
+        shutil.copy2(self.io_dict["in"]["input_pcz_path"], self.tmp_folder)
 
         # Temporary output
-        temp_out = str(Path(self.stage_io_dict.get("unique_dir")).joinpath("output.dat"))
+        # temp_out = str(Path(self.stage_io_dict.get("unique_dir")).joinpath("output.dat"))
+        temp_out = "output.dat"
+        temp_json = "output.json"
 
         # Command line
-        # pczdump -i structure.ca.std.pcz --evecs -o pcz.evecs
-        self.cmd = [self.binary_path,
-                "-i", input_pcz,
-                "-o", temp_out,
-                "--evec={}".format(self.eigenvector)
-               ]
- 
+        # pczdump -i structure.ca.std.pcz --lindemann -M ":2-86" -o lindemann_report.txt
+        # self.cmd = [self.binary_path,
+        #             "-i", input_pcz,
+        #             "-o", temp_out,
+        #             "--lindemann"
+        #             ]
+
+        self.cmd = ['cd', self.tmp_folder, ';',
+                    self.binary_path,
+                    "-i", PurePath(self.io_dict["in"]["input_pcz_path"]).name,
+                    "-o", temp_out,
+                    "--lindemann"
+                    ]
+
+        if self.mask:
+            self.cmd.append("-M {}".format(self.mask))
+
         # Run Biobb block
         self.run_biobb()
 
-        # Parse output evecs
-           #  0.180  -0.069   0.168   0.204  -0.054   0.235   0.145  -0.001   0.260   0.183
-           # -0.041   0.231   0.174  -0.077   0.144   0.097  -0.022   0.143   0.069   0.008
-
+        # Parse output Lindemann
+        #  0.132891
         info_dict = {}
-        info_dict['evecs'] = []
-        with open (temp_out,'r') as file:
+        with open(PurePath(self.tmp_folder).joinpath(temp_out), 'r') as file:
             for line in file:
-                info = line.strip().split(' ')
-                for nums in info:
-                    if nums:
-                        info_dict['evecs'].append(nums)
-
-        # Computing Projections
-        info_dict['projs'] = []
-        module = 1
-        proj = 0
-        for num in info_dict['evecs']:
-            val = float(num) * float(num)
-            proj = proj + val                
-            if module % 3 == 0:
-                proj = math.sqrt(proj)
-                module = 1
-                info_dict['projs'].append(float("{:.4f}".format(proj))) 
-                proj = 0
-            else:
-                module = module + 1
-       
-        # convert into JSON:
-        y = json.dumps(info_dict)
-
-        ## the result is a JSON string:
-        print(json.dumps(info_dict, indent=4))
+                info = float(line.strip())
+                info_dict['lindemann'] = info
 
-        with open (output_json, 'w') as out_file:
+        with open(PurePath(self.tmp_folder).joinpath(temp_json), 'w') as out_file:
             out_file.write(json.dumps(info_dict, indent=4))
 
+        # Copy outputs from temporary folder to output path
+        shutil.copy2(PurePath(self.tmp_folder).joinpath(temp_json), PurePath(self.io_dict["out"]["output_json_path"]))
+
         # Copy files to host
-        self.copy_to_host()
+        # self.copy_to_host()
 
         # remove temporary folder(s)
         self.tmp_files.extend([
-            self.stage_io_dict.get("unique_dir")
+            # self.stage_io_dict.get("unique_dir"),
+            self.tmp_folder
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
-def pcz_evecs(input_pcz_path: str, output_json_path: str,
-            properties: dict = None, **kwargs) -> int:
-    """Create :class:`PCZevecs <flexserv.pcasuite.pcz_evecs>`flexserv.pcasuite.PCZevecs class and
-    execute :meth:`launch() <flexserv.pcasuite.pcz_evecs.launch>` method"""
-
-    return PCZevecs(  
-                    input_pcz_path=input_pcz_path,
-                    output_json_path=output_json_path,
-                    properties=properties).launch()
+
+def pcz_lindemann(input_pcz_path: str, output_json_path: str,
+                  properties: dict = None, **kwargs) -> int:
+    """Create :class:`PCZlindemann <flexserv.pcasuite.pcz_lindemann>`flexserv.pcasuite.PCZlindemann class and
+    execute :meth:`launch() <flexserv.pcasuite.pcz_lindemann.launch>` method"""
+
+    return PCZlindemann(input_pcz_path=input_pcz_path,
+                        output_json_path=output_json_path,
+                        properties=properties).launch()
+
 
 def main():
-    parser = argparse.ArgumentParser(description='Extract PCA Eigen Vectors from a compressed PCZ file.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
+    parser = argparse.ArgumentParser(description='Extract Lindemann coefficients from a compressed PCZ file.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
     required_args.add_argument('--input_pcz_path', required=True, help='Input compressed trajectory file. Accepted formats: pcz.')
-    required_args.add_argument('--output_json_path', required=True, help='Output json file with PCA evecs. Accepted formats: json.')
+    required_args.add_argument('--output_json_path', required=True, help='Output json file with Lindemann coefficient report. Accepted formats: json.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call
-    pcz_evecs(      input_pcz_path=args.input_pcz_path,
-                    output_json_path=args.output_json_path,
-                    properties=properties)
+    pcz_lindemann(input_pcz_path=args.input_pcz_path,
+                  output_json_path=args.output_json_path,
+                  properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_hinges.py` & `biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_hinges.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 #!/usr/bin/env python3
 
 """Module containing the PCZhinges class and the command line interface."""
 import argparse
-import json, re
-from pathlib import Path
+import shutil
+import json
+import re
+from pathlib import PurePath
+from biobb_common.tools import file_utils as fu
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
+
 class PCZhinges(BiobbObject):
     """
     | biobb_flexserv PCZhinges
     | Compute possible hinge regions (residues around which large protein movements are organized) of a molecule from a compressed PCZ file.
     | Wrapper of the pczdump tool from the PCAsuite FlexServ module.
 
     Args:
         input_pcz_path (str): Input compressed trajectory file. File type: input. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/data/pcasuite/pcazip.pcz>`_. Accepted formats: pcz (edam:format_3874).
         output_json_path (str): Output hinge regions x PCA mode file. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/reference/pcasuite/hinges.json>`_. Accepted formats: json (edam:format_3464).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
             * **binary_path** (*str*) - ("pczdump") pczdump binary path to be used.
             * **eigenvector** (*int*) - (0) PCA mode (eigenvector) from which to extract bfactor values per residue (0 means average over all modes).
-            * **method** (*str*) - ("Dynamic_domain") Method to compute the hinge regions (Options: Bfactor_slope, Force_constant, Dynamic_domain) 
+            * **method** (*str*) - ("Dynamic_domain") Method to compute the hinge regions (Options: Bfactor_slope, Force_constant, Dynamic_domain)
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
             from biobb_flexserv.pcasuite.pcz_hinges import pcz_hinges
@@ -43,196 +47,213 @@
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
     def __init__(self, input_pcz_path: str, output_json_path: str,
-    properties: dict = None, **kwargs) -> None:
+                 properties: dict = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 
-                'input_pcz_path': input_pcz_path
-             },
-            'out': {    
-                'output_json_path': output_json_path
-            }
+            'in': {'input_pcz_path': input_pcz_path},
+            'out': {'output_json_path': output_json_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.binary_path = properties.get('binary_path', 'pczdump')
         self.eigenvector = properties.get('eigenvector', 1)
         self.method = properties.get('method', "Bfactor_slope")
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
-    def parse_output(self,output_file):
+    def parse_output(self, output_file):
         """ Parses FlexServ hinges methods output file report """
 
         method = ''
         if self.method == "Bfactor_slope":
             method = "#### Distance variation method"
         elif self.method == "Force_constant":
             method = "#### Force constant"
         elif self.method == "Dynamic_domain":
             method = "#### Lavery method"
         else:
             print("Method not recognised ({}), please check it and try again. ".format(self.method))
 
         start = False
         out_data = ''
-        with open (output_file,'r') as file:
+        with open(output_file, 'r') as file:
             for line in file:
-                if method in line: 
+                if method in line:
                     start = True
                 elif "####" in line:
                     start = False
                 if start:
                     out_data += line
 
         dict_out = {}
         dict_out["method"] = self.method
         if self.method == "Force_constant":
             dict_out["values_per_residue"] = []
             for line in out_data.split("\n"):
-                print ("Force_constant: -" + str(line) + "-")
                 if line and "#" not in line:
                     dict_out["values_per_residue"].append(float(line.strip()))
-                if "possible hinge" in line: # Peak constant (possible hinge): residue 64 (16.740)
+                if "possible hinge" in line:  # Peak constant (possible hinge): residue 64 (16.740)
                     residue = int(line.split(' ')[6])
                     dict_out["hinge_residues"] = residue
         elif self.method == "Bfactor_slope":
             dict_out["hinge_residues"] = []
             for line in out_data.split("\n"):
-                print ("Bfactor_slope: -" + str(line) + "-")
                 if "Window" in line:  # Window 28: residue  54 seems a downhill hinge point
-                    residue = int(re.split(r'\s+',line)[3])
+                    residue = int(re.split(r'\s+', line)[3])
                     dict_out["hinge_residues"].append(residue)
-                if "Consensus" in line: # Consensus Downhill hinge point :  23.7 (  64.965)
+                if "Consensus" in line:  # Consensus Downhill hinge point :  23.7 (  64.965)
                     hinge_point = float(line.split(':')[1].split('(')[0])
                     dict_out["consensus_hinge"] = hinge_point
         elif self.method == "Dynamic_domain":
             start = 0
             dict_out["clusters"] = []
             for line in out_data.split("\n"):
-                print ("Dynamic_domain: -" + str(line) + "-")
-                if not "threshold" in line and "nClusters" in line:  # nClusters: 2
+                if "threshold" not in line and "nClusters" in line:  # nClusters: 2
                     nclusters = int(line.split(':')[1])
                     dict_out["nClusters"] = nclusters
                 if "Threshold" in line:  # *** Threshold defined: 0.300000
                     threshold = float(line.split(':')[1])
                     dict_out["threshold"] = threshold
                 if "Min. drij" in line:  # *** Min. drij: 0.000322
                     minValue = float(line.split(':')[1])
                     dict_out["minValue"] = minValue
                 if "Max. drij" in line:  # *** Max. drij: 6.385425
                     maxValue = float(line.split(':')[1])
                     dict_out["maxValue"] = maxValue
                 if "threshold" in line:  # nClusters: 2 threshold: 3.192873
                     final_threshold = float(line.split(':')[2])
                     dict_out["final_threshold"] = final_threshold
-                if "Cluster" in line and "elements" in line: # Cluster 0 (74 elements)
+                if "Cluster" in line and "elements" in line:  # Cluster 0 (74 elements)
                     clusterLine = line.split()
                     clusterNum = int(clusterLine[1])
-                    clusterElems = int(clusterLine[2].replace('(',''))
-                    cluster = {"clusterNum" : clusterNum, "clusterElems" : clusterElems}
+                    clusterElems = int(clusterLine[2].replace('(', ''))
+                    cluster = {"clusterNum": clusterNum, "clusterElems": clusterElems}
                     dict_out["clusters"].append(cluster)
                     start = start + 1
                 if start and "[" in line:
-                    #dict_out["clusters"][start-1]["residues"] = list(map(int,list(line.replace(", ]", "").replace("  [","").split(', '))))
+                    # dict_out["clusters"][start-1]["residues"] = list(map(int,list(line.replace(", ]", "").replace("  [","").split(', '))))
                     dict_out["clusters"][start-1]["residues"] = eval(line)
-                #Interacting regions: 13 14 30 31 69 70 84 85 112 113 114 115 116 166 167 199 200
+                # Interacting regions: 13 14 30 31 69 70 84 85 112 113 114 115 116 166 167 199 200
                 if "Interacting regions" in line:
                     nums = line.split(':')[1]
-                    dict_out["interacting_regions"] = list(map(int,nums.split()))
-                #Hinge residues: 13 14 30 31 69 70 84 85 112 113 114 115 116 166 167 199 200
-                if "Hinge residues" in line:  
+                    dict_out["interacting_regions"] = list(map(int, nums.split()))
+                # Hinge residues: 13 14 30 31 69 70 84 85 112 113 114 115 116 166 167 199 200
+                if "Hinge residues" in line:
                     nums = line.split(':')[1]
-                    dict_out["hinge_residues"] = list(map(int,nums.split()))
+                    dict_out["hinge_residues"] = list(map(int, nums.split()))
 
         return dict_out
 
     @launchlogger
     def launch(self):
         """Launches the execution of the FlexServ pcz_hinges module."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
-        self.stage_files()
+        if self.check_restart():
+            return 0
+        # self.stage_files()
 
         # Internal file paths
-        try:
-            # Using rel paths to shorten the amount of characters due to fortran path length limitations
-            input_pcz = str(Path(self.stage_io_dict["in"]["input_pcz_path"]).relative_to(Path.cwd()))
-            output_json = str(Path(self.stage_io_dict["out"]["output_json_path"]).relative_to(Path.cwd()))
-        except ValueError:
-            # Container or remote case
-            input_pcz = self.stage_io_dict["in"]["input_pcz_path"]
-            output_json = self.stage_io_dict["out"]["output_json_path"]
+        # try:
+        #     # Using rel paths to shorten the amount of characters due to fortran path length limitations
+        #     input_pcz = str(Path(self.stage_io_dict["in"]["input_pcz_path"]).relative_to(Path.cwd()))
+        #     output_json = str(Path(self.stage_io_dict["out"]["output_json_path"]).relative_to(Path.cwd()))
+        # except ValueError:
+        #     # Container or remote case
+        #     input_pcz = self.stage_io_dict["in"]["input_pcz_path"]
+        #     output_json = self.stage_io_dict["out"]["output_json_path"]
+
+        # Manually creating a Sandbox to avoid issues with input parameters buffer overflow:
+        #   Long strings defining a file path makes Fortran or C compiled programs crash if the string
+        #   declared is shorter than the input parameter path (string) length.
+        #   Generating a temporary folder and working inside this folder (sandbox) fixes this problem.
+        #   The problem was found in Galaxy executions, launching Singularity containers (May 2023).
+
+        # Creating temporary folder
+        self.tmp_folder = fu.create_unique_dir()
+        fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
+
+        shutil.copy2(self.io_dict["in"]["input_pcz_path"], self.tmp_folder)
 
         # Temporary output
-        temp_out = str(Path(self.stage_io_dict.get("unique_dir")).joinpath("output.dat"))
+        # temp_out = str(Path(self.stage_io_dict.get("unique_dir")).joinpath("output.dat"))
+        temp_out = "output.dat"
+        temp_log = "output.log"
+        temp_json = "output.json"
 
         # Command line (1: dat file)
         # pczdump -i structure.ca.std.pcz --fluc=1 -o bfactor_1.dat
-        self.cmd = [self.binary_path,
-                "-i", input_pcz,
-                "-o", temp_out,
-                "-t", "0.3",
-                "--hinge={}".format(self.eigenvector),
-                ">&", "pcz_dump.hinges.log"
-               ]
-  
+        # self.cmd = [self.binary_path,
+        #             "-i", input_pcz,
+        #             "-o", temp_out,
+        #             "-t", "0.3",
+        #             "--hinge={}".format(self.eigenvector),
+        #             ">&", "pcz_dump.hinges.log"
+        #             ]
+
+        self.cmd = ['cd', self.tmp_folder, ';',
+                    self.binary_path,
+                    '-i', PurePath(self.io_dict["in"]["input_pcz_path"]).name,
+                    '-o', temp_out,
+                    "-t", "0.3",
+                    "--hinge={}".format(self.eigenvector),
+                    ">&", temp_log
+                    ]
+
         # Run Biobb block
         self.run_biobb()
 
-        # Parsing output file and extracting results for the given method 
-        dict_out = self.parse_output(temp_out)
-
-        # convert into JSON:
-        y = json.dumps(dict_out)
+        # Parsing output file and extracting results for the given method
+        dict_out = self.parse_output(PurePath(self.tmp_folder).joinpath(temp_out))
 
-        ## the result is a JSON string:
-        print(json.dumps(dict_out, indent=4))
-
-        with open (output_json, 'w') as out_file:
+        with open(PurePath(self.tmp_folder).joinpath(temp_json), 'w') as out_file:
             out_file.write(json.dumps(dict_out, indent=4))
 
+        # Copy outputs from temporary folder to output path
+        shutil.copy2(PurePath(self.tmp_folder).joinpath(temp_json), PurePath(self.io_dict["out"]["output_json_path"]))
+
         # Copy files to host
-        self.copy_to_host()
+        # self.copy_to_host()
 
         # remove temporary folder(s)
         self.tmp_files.extend([
-            self.stage_io_dict.get("unique_dir")
+            # self.stage_io_dict.get("unique_dir"),
+            self.tmp_folder
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def pcz_hinges(input_pcz_path: str, output_json_path: str,
-            properties: dict = None, **kwargs) -> int:
+               properties: dict = None, **kwargs) -> int:
     """Create :class:`PCZhinges <flexserv.pcasuite.pcz_hinges>`flexserv.pcasuite.PCZhinges class and
     execute :meth:`launch() <flexserv.pcasuite.pcz_hinges.launch>` method"""
 
-    return PCZhinges(  
-                    input_pcz_path=input_pcz_path,
-                    output_json_path=output_json_path,
-                    properties=properties).launch()
+    return PCZhinges(input_pcz_path=input_pcz_path,
+                     output_json_path=output_json_path,
+                     properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Compute possible hinge regions (residues around which large protein movements are organized) of a molecule from a compressed PCZ file.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -240,13 +261,14 @@
     required_args.add_argument('--output_json_path', required=True, help='Output hinge regions x PCA mode file. Accepted formats: json.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call
-    pcz_hinges(     input_pcz_path=args.input_pcz_path,
-                    output_json_path=args.output_json_path,
-                    properties=properties)
+    pcz_hinges(input_pcz_path=args.input_pcz_path,
+               output_json_path=args.output_json_path,
+               properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_info.py` & `biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_stiffness.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,196 +1,210 @@
 #!/usr/bin/env python3
 
-"""Module containing the PCZinfo class and the command line interface."""
+"""Module containing the PCZstiffness class and the command line interface."""
 import argparse
+import shutil
 import json
-from pathlib import Path
+import math
+from pathlib import PurePath
+from biobb_common.tools import file_utils as fu
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
-class PCZinfo(BiobbObject):
+
+class PCZstiffness(BiobbObject):
     """
-    | biobb_flexserv PCZinfo
-    | Extract PCA info (variance, Dimensionality) from a compressed PCZ file.
+    | biobb_flexserv PCZstiffness
+    | Extract PCA stiffness from a compressed PCZ file.
     | Wrapper of the pczdump tool from the PCAsuite FlexServ module.
 
     Args:
         input_pcz_path (str): Input compressed trajectory file. File type: input. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/data/pcasuite/pcazip.pcz>`_. Accepted formats: pcz (edam:format_3874).
-        output_json_path (str): Output json file with PCA info such as number of components, variance and dimensionality. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/reference/pcasuite/pcz_info.json>`_. Accepted formats: json (edam:format_3464).
+        output_json_path (str): Output json file with PCA Stiffness. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/reference/pcasuite/pcz_stiffness.json>`_. Accepted formats: json (edam:format_3464).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
             * **binary_path** (*str*) - ("pczdump") pczdump binary path to be used.
+            * **eigenvector** (*int*) - (0) PCA mode (eigenvector) from which to extract stiffness.
+            * **temperature** (*int*) - (300) Temperature with which compute the apparent stiffness.
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
-            from biobb_flexserv.pcasuite.pcz_info import pcz_info
+            from biobb_flexserv.pcasuite.pcz_stiffness import pcz_stiffness
+
+            prop = {
+                'eigenvector': 1
+            }
 
-            pcz_info( input_pcz_path='/path/to/pcazip_input.pcz',
-                    output_json_path='/path/to/pcz_info.json')
+            pcz_stiffness( input_pcz_path='/path/to/pcazip_input.pcz',
+                    output_json_path='/path/to/pcz_stiffness.json',
+                    properties=prop)
 
     Info:
         * wrapped_software:
             * name: FlexServ PCAsuite
             * version: >=1.0
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
-    def __init__(self, input_pcz_path: str, 
-    output_json_path: str, properties: dict = None, **kwargs) -> None:
+    def __init__(self, input_pcz_path: str,
+                 output_json_path: str, properties: dict = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 
-                'input_pcz_path': input_pcz_path
-             },
-            'out': {    
-                'output_json_path': output_json_path
-            }
+            'in': {'input_pcz_path': input_pcz_path},
+            'out': {'output_json_path': output_json_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.binary_path = properties.get('binary_path', 'pczdump')
+        self.eigenvector = properties.get('eigenvector', 0)
+        self.temperature = properties.get('temperature', 300)
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     @launchlogger
     def launch(self):
-        """Launches the execution of the FlexServ pcz_info module."""
+        """Launches the execution of the FlexServ pcz_stiffness module."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
-        self.stage_files()
+        if self.check_restart():
+            return 0
+        # self.stage_files()
 
         # Internal file paths
-        try:
-            # Using rel paths to shorten the amount of characters due to fortran path length limitations
-            input_pcz = str(Path(self.stage_io_dict["in"]["input_pcz_path"]).relative_to(Path.cwd()))
-            output_json = str(Path(self.stage_io_dict["out"]["output_json_path"]).relative_to(Path.cwd()))
-        except ValueError:
-            # Container or remote case
-            input_pcz = self.stage_io_dict["in"]["input_pcz_path"]
-            output_json = self.stage_io_dict["out"]["output_json_path"]
+        # try:
+        #     # Using rel paths to shorten the amount of characters due to fortran path length limitations
+        #     input_pcz = str(Path(self.stage_io_dict["in"]["input_pcz_path"]).relative_to(Path.cwd()))
+        #     output_json = str(Path(self.stage_io_dict["out"]["output_json_path"]).relative_to(Path.cwd()))
+        # except ValueError:
+        #     # Container or remote case
+        #     input_pcz = self.stage_io_dict["in"]["input_pcz_path"]
+        #     output_json = self.stage_io_dict["out"]["output_json_path"]
+
+        # Manually creating a Sandbox to avoid issues with input parameters buffer overflow:
+        #   Long strings defining a file path makes Fortran or C compiled programs crash if the string
+        #   declared is shorter than the input parameter path (string) length.
+        #   Generating a temporary folder and working inside this folder (sandbox) fixes this problem.
+        #   The problem was found in Galaxy executions, launching Singularity containers (May 2023).
+
+        # Creating temporary folder
+        self.tmp_folder = fu.create_unique_dir()
+        fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
+
+        shutil.copy2(self.io_dict["in"]["input_pcz_path"], self.tmp_folder)
 
         # Temporary output
-        temp_out_1 = str(Path(self.stage_io_dict.get("unique_dir")).joinpath("output1.dat"))
-        temp_out_2 = str(Path(self.stage_io_dict.get("unique_dir")).joinpath("output2.dat"))
+        # temp_out = str(Path(self.stage_io_dict.get("unique_dir")).joinpath("output.dat"))
+        temp_out = "output.dat"
+        temp_json = "output.json"
 
         # Command line
-        # pczdump -i structure.ca.std.pcz --info -o pcz.info
-        self.cmd = [self.binary_path,
-                "-i", input_pcz,
-                "-o", temp_out_1,
-                "--info", ';',
-                self.binary_path,
-                "-i", input_pcz,
-                "-o", temp_out_2,
-                "--evals"
-               ]
- 
+        # pczdump -i structure.ca.std.pcz --stiffness -o pcz.stiffness
+        # self.cmd = [self.binary_path,
+        #             "-i", input_pcz,
+        #             "-o", temp_out,
+        #             "--stiff={}".format(self.eigenvector),
+        #             "--temperature={}".format(self.temperature)
+        #             ]
+
+        self.cmd = ['cd', self.tmp_folder, ';',
+                    self.binary_path,
+                    "-i", PurePath(self.io_dict["in"]["input_pcz_path"]).name,
+                    "-o", temp_out,
+                    "--stiff={}".format(self.eigenvector),
+                    "--temperature={}".format(self.temperature)
+                    ]
+
         # Run Biobb block
         self.run_biobb()
 
-        # Parse output info
-            # Title             : MC generated trajectory
-            # Atoms             :       85
-            # Vectors           :        4
-            # Frames            :     1000
-            # Total variance    :  1137.20
-            # Explained variance:  1043.32
-            # Quality           :    91.74%
-            # Dimensionality    :       21
-            # RMSd type         : Standard RMSd
-            # Have atom names   : True
+        # Parse output stiffness
         info_dict = {}
-        with open (temp_out_1,'r') as file:
+        info_dict['stiffness'] = []
+        info_dict['stiffness_log'] = []
+        row = 0
+        with open(PurePath(self.tmp_folder).joinpath(temp_out), 'r') as file:
             for line in file:
-                info = line.split(':')
-                info_dict[info[0].strip().replace(' ','_')] = info[1].strip()
+                info = line.strip().split(',')
+                line_array = []
+                line_array_log = []
+                for nums in info:
+                    if nums:
+                        line_array.append(float(nums))
+                        if float(nums) != 0:
+                            line_array_log.append(math.log10(float(nums)))
+                        else:
+                            line_array_log.append(float(nums))
+
+                info_dict['stiffness'].append(line_array)
+                info_dict['stiffness'][row][row] = float('inf')
+                info_dict['stiffness_log'].append(line_array_log)
+                info_dict['stiffness_log'][row][row] = float('inf')
+                row += 1
 
-        # Parse output evals
-            # 744.201782
-            # 170.061981
-            # 89.214905
-            # 39.836308
-        info_dict['Eigen_Values'] = []  
-        info_dict['Eigen_Values_dimensionality_vs_total'] = []  
-        info_dict['Eigen_Values_dimensionality_vs_explained'] = []  
-        accum_tot = 0
-        accum_exp = 0
-        with open (temp_out_2,'r') as file:
-            for line in file:
-                eval = float(line.strip())
-                eval_var = (eval / float(info_dict['Total_variance']))*100
-                accum_tot = accum_tot + eval_var
-                eval_dim = (eval / float(info_dict['Explained_variance']))*100
-                accum_exp = accum_exp + eval_dim
-                info_dict['Eigen_Values'].append(eval)
-                info_dict['Eigen_Values_dimensionality_vs_total'].append(accum_tot)
-                info_dict['Eigen_Values_dimensionality_vs_explained'].append(accum_exp)
-       
-        # convert into JSON:
-        y = json.dumps(info_dict)
-
-        ## the result is a JSON string:
-        print(json.dumps(info_dict, indent=4))
-
-        with open (output_json, 'w') as out_file:
+        with open(PurePath(self.tmp_folder).joinpath(temp_json), 'w') as out_file:
             out_file.write(json.dumps(info_dict, indent=4))
 
+        # Copy outputs from temporary folder to output path
+        shutil.copy2(PurePath(self.tmp_folder).joinpath(temp_json), PurePath(self.io_dict["out"]["output_json_path"]))
+
         # Copy files to host
-        self.copy_to_host()
+        # self.copy_to_host()
 
         # remove temporary folder(s)
         self.tmp_files.extend([
-            self.stage_io_dict.get("unique_dir")
+            # self.stage_io_dict.get("unique_dir"),
+            self.tmp_folder
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
-def pcz_info(input_pcz_path: str, output_json_path: str,
-            properties: dict = None, **kwargs) -> int:
-    """Create :class:`PCZinfo <flexserv.pcasuite.pcz_info>`flexserv.pcasuite.PCZinfo class and
-    execute :meth:`launch() <flexserv.pcasuite.pcz_info.launch>` method"""
-
-    return PCZinfo(  
-                    input_pcz_path=input_pcz_path,
-                    output_json_path=output_json_path,
-                    properties=properties).launch()
+
+def pcz_stiffness(input_pcz_path: str, output_json_path: str,
+                  properties: dict = None, **kwargs) -> int:
+    """Create :class:`PCZstiffness <flexserv.pcasuite.pcz_stiffness>`flexserv.pcasuite.PCZstiffness class and
+    execute :meth:`launch() <flexserv.pcasuite.pcz_stiffness.launch>` method"""
+
+    return PCZstiffness(input_pcz_path=input_pcz_path,
+                        output_json_path=output_json_path,
+                        properties=properties).launch()
+
 
 def main():
-    parser = argparse.ArgumentParser(description='Extract PCA info from a compressed PCZ file.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
+    parser = argparse.ArgumentParser(description='Extract PCA Stiffness from a compressed PCZ file.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
     required_args.add_argument('--input_pcz_path', required=True, help='Input compressed trajectory file. Accepted formats: pcz.')
-    required_args.add_argument('--output_json_path', required=True, help='Output json file with PCA info such as number of components, variance and dimensionality. Accepted formats: json.')
+    required_args.add_argument('--output_json_path', required=True, help='Output json file with PCA stiffness. Accepted formats: json.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call
-    pcz_info(       input_pcz_path=args.input_pcz_path,
-                    output_json_path=args.output_json_path,
-                    properties=properties)
+    pcz_stiffness(input_pcz_path=args.input_pcz_path,
+                  output_json_path=args.output_json_path,
+                  properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_lindemann.py` & `biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_unzip.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,169 +1,177 @@
 #!/usr/bin/env python3
 
-"""Module containing the PCZlindemann class and the command line interface."""
+"""Module containing the PCZunzip class and the command line interface."""
 import argparse
-import json
-from pathlib import Path
+import shutil
+from pathlib import PurePath
+from biobb_common.tools import file_utils as fu
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
-class PCZlindemann(BiobbObject):
+
+class PCZunzip(BiobbObject):
     """
-    | biobb_flexserv PCZlindemann
-    | Extract Lindemann coefficient (an estimate of the solid-liquid behaviour of a protein) from a compressed PCZ file.
-    | Wrapper of the pczdump tool from the PCAsuite FlexServ module.
+    | biobb_flexserv PCZunzip
+    | Wrapper of the pcaunzip tool from the PCAsuite FlexServ module.
+    | Uncompress Molecular Dynamics (MD) trajectories compressed using Principal Component Analysis (PCA) algorithms.
 
     Args:
-        input_pcz_path (str): Input compressed trajectory file. File type: input. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/data/pcasuite/pcazip.pcz>`_. Accepted formats: pcz (edam:format_3874).
-        output_json_path (str): Output json file with PCA Eigen Vectors. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/reference/pcasuite/pcz_lindemann.json>`_. Accepted formats: json (edam:format_3464).
+        input_pcz_path (str): Input compressed trajectory. File type: input. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/data/pcasuite/pcazip.pcz>`_. Accepted formats: pcz (edam:format_3874).
+        output_crd_path (str): Output uncompressed trajectory. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/reference/pcasuite/traj.crd>`_. Accepted formats: crd (edam:format_3878), mdcrd (edam:format_3878), inpcrd (edam:format_3878), pdb (edam:format_1476).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
-            * **binary_path** (*str*) - ("pczdump") pczdump binary path to be used.
-            * **mask** (*str*) - ("all atoms") Residue mask, in the format ":resnum1, resnum2, resnum3" (e.g. ":10,21,33"). See https://mmb.irbbarcelona.org/software/pcasuite/ for the complete format specification.
+            * **binary_path** (*str*) - ("pcaunzip") pcaunzip binary path to be used.
+            * **verbose** (*bool*) - (False) Make output verbose
+            * **pdb** (*bool*) - (False) Use PDB format for output trajectory
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
-            from biobb_flexserv.pcasuite.pcz_lindemann import pcz_lindemann
+            from biobb_flexserv.pcasuite.pcz_unzip import pcz_unzip
             prop = {
-                'mask': ':10,12,15'
+                'pdb': False
             }
-            pcz_lindemann( input_pcz_path='/path/to/pcazip_input.pcz',
-                    output_json_path='/path/to/lindemann_report.json',
+            pcz_unzip( input_pcz_path='/path/to/pcazip_input.pcz',
+                    output_crd_path='/path/to/pcazip_traj.crd',
                     properties=prop)
 
     Info:
         * wrapped_software:
             * name: FlexServ PCAsuite
             * version: >=1.0
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
-    def __init__(self, input_pcz_path: str, 
-    output_json_path: str, properties: dict = None, **kwargs) -> None:
+    def __init__(self, input_pcz_path: str,
+                 output_crd_path: str, properties: dict = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 
-                'input_pcz_path': input_pcz_path
-             },
-            'out': {    
-                'output_json_path': output_json_path
-            }
+            'in': {'input_pcz_path': input_pcz_path},
+            'out': {'output_crd_path': output_crd_path}
         }
 
         # Properties specific for BB
         self.properties = properties
-        self.binary_path = properties.get('binary_path', 'pczdump')
-        self.mask = properties.get('mask', '')
+        self.binary_path = properties.get('binary_path', 'pcaunzip')
+        self.verbose = properties.get('verbose', False)
+        self.pdb = properties.get('pdb', False)
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     @launchlogger
     def launch(self):
-        """Launches the execution of the FlexServ pcz_lindemann module."""
+        """Launches the execution of the FlexServ pcaunzip module."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
-        self.stage_files()
+        if self.check_restart():
+            return 0
+        # self.stage_files()
 
         # Internal file paths
-        try:
-            # Using rel paths to shorten the amount of characters due to fortran path length limitations
-            input_pcz = str(Path(self.stage_io_dict["in"]["input_pcz_path"]).relative_to(Path.cwd()))
-            output_json = str(Path(self.stage_io_dict["out"]["output_json_path"]).relative_to(Path.cwd()))
-        except ValueError:
-            # Container or remote case
-            input_pcz = self.stage_io_dict["in"]["input_pcz_path"]
-            output_json = self.stage_io_dict["out"]["output_json_path"]
+        # try:
+        #     # Using rel paths to shorten the amount of characters due to fortran path length limitations
+        #     input_pcz = str(Path(self.stage_io_dict["in"]["input_pcz_path"]).relative_to(Path.cwd()))
+        #     output_crd = str(Path(self.stage_io_dict["out"]["output_crd_path"]).relative_to(Path.cwd()))
+        # except ValueError:
+        #     # Container or remote case
+        #     input_pcz = self.stage_io_dict["in"]["input_pcz_path"]
+        #     output_crd = self.stage_io_dict["out"]["output_crd_path"]
+
+        # Manually creating a Sandbox to avoid issues with input parameters buffer overflow:
+        #   Long strings defining a file path makes Fortran or C compiled programs crash if the string
+        #   declared is shorter than the input parameter path (string) length.
+        #   Generating a temporary folder and working inside this folder (sandbox) fixes this problem.
+        #   The problem was found in Galaxy executions, launching Singularity containers (May 2023).
+
+        # Creating temporary folder
+        self.tmp_folder = fu.create_unique_dir()
+        fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
 
-        # Temporary output
-        temp_out = str(Path(self.stage_io_dict.get("unique_dir")).joinpath("output.dat"))
+        shutil.copy2(self.io_dict["in"]["input_pcz_path"], self.tmp_folder)
 
         # Command line
-        # pczdump -i structure.ca.std.pcz --lindemann -M ":2-86" -o lindemann_report.txt
-        self.cmd = [self.binary_path,
-                "-i", input_pcz,
-                "-o", temp_out,
-                "--lindemann"
-               ]
- 
-        if self.mask:
-            self.cmd.append("-M {}".format(self.mask))
-
-        # Run Biobb block
-        self.run_biobb()
+        # pcaunzip -i infile [-o outfile] [--pdb] [--verbose] [--help]
+        # self.cmd = [self.binary_path,
+        #             "-i", input_pcz,
+        #             "-o", output_crd
+        #             ]
+
+        self.cmd = ['cd', self.tmp_folder, ';',
+                    self.binary_path,
+                    "-i", PurePath(self.io_dict["in"]["input_pcz_path"]).name,
+                    "-o", PurePath(self.io_dict["out"]["output_crd_path"]).name
+                    ]
 
-        # Parse output Lindemann
-           #  0.132891
-        info_dict = {}
-        with open (temp_out,'r') as file:
-            for line in file:
-                info = float(line.strip())
-                info_dict['lindemann'] = info
+        if self.verbose:
+            self.cmd.append('-v')
 
-        # convert into JSON:
-        y = json.dumps(info_dict)
+        if self.pdb:
+            self.cmd.append('--pdb')
 
-        ## the result is a JSON string:
-        print(json.dumps(info_dict, indent=4))
+        # Run Biobb block
+        self.run_biobb()
 
-        with open (output_json, 'w') as out_file:
-            out_file.write(json.dumps(info_dict, indent=4))
+        # Copy outputs from temporary folder to output path
+        shutil.copy2(PurePath(self.tmp_folder).joinpath(PurePath(self.io_dict["out"]["output_crd_path"]).name), PurePath(self.io_dict["out"]["output_crd_path"]))
 
         # Copy files to host
-        self.copy_to_host()
+        # self.copy_to_host()
 
         # remove temporary folder(s)
         self.tmp_files.extend([
-            self.stage_io_dict.get("unique_dir")
+            # self.stage_io_dict.get("unique_dir"),
+            self.tmp_folder
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
-def pcz_lindemann(input_pcz_path: str, output_json_path: str,
-            properties: dict = None, **kwargs) -> int:
-    """Create :class:`PCZlindemann <flexserv.pcasuite.pcz_lindemann>`flexserv.pcasuite.PCZlindemann class and
-    execute :meth:`launch() <flexserv.pcasuite.pcz_lindemann.launch>` method"""
-
-    return PCZlindemann(  
-                    input_pcz_path=input_pcz_path,
-                    output_json_path=output_json_path,
+
+def pcz_unzip(input_pcz_path: str,
+              output_crd_path: str,
+              properties: dict = None, **kwargs) -> int:
+    """Create :class:`PCZunzip <flexserv.pcasuite.PCZunzip>`flexserv.pcasuite.PCZunzip class and
+    execute :meth:`launch() <flexserv.pcasuite.PCZunzip.launch>` method"""
+
+    return PCZunzip(input_pcz_path=input_pcz_path,
+                    output_crd_path=output_crd_path,
                     properties=properties).launch()
 
+
 def main():
-    parser = argparse.ArgumentParser(description='Extract Lindemann coefficients from a compressed PCZ file.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
+    parser = argparse.ArgumentParser(description='Uncompress Molecular Dynamics (MD) compressed trajectories using Principal Component Analysis (PCA) algorithms.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
     required_args.add_argument('--input_pcz_path', required=True, help='Input compressed trajectory file. Accepted formats: pcz.')
-    required_args.add_argument('--output_json_path', required=True, help='Output json file with Lindemann coefficient report. Accepted formats: json.')
+    required_args.add_argument('--output_crd_path', required=True, help='Output trajectory file. Accepted formats: crd, mdcrd, inpcrd, pdb.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call
-    pcz_lindemann(  input_pcz_path=args.input_pcz_path,
-                    output_json_path=args.output_json_path,
-                    properties=properties)
+    pcz_unzip(input_pcz_path=args.input_pcz_path,
+              output_crd_path=args.output_crd_path,
+              properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_similarity.py` & `biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_similarity.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 #!/usr/bin/env python3
 
 """Module containing the PCZsimilarity class and the command line interface."""
 import argparse
 import json
 import numpy as np
-from pathlib import Path
+import shutil
+from pathlib import PurePath
+from biobb_common.tools import file_utils as fu
 from math import exp
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
+
 class PCZsimilarity(BiobbObject):
     """
     | biobb_flexserv PCZsimilarity
     | Compute PCA similarity between two given compressed PCZ files.
     | Wrapper of the pczdump tool from the PCAsuite FlexServ module.
 
     Args:
@@ -41,97 +44,93 @@
             * version: >=1.0
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
-    def __init__(self, input_pcz_path1: str, input_pcz_path2: str, 
-    output_json_path: str, properties: dict = None, **kwargs) -> None:
+    def __init__(self, input_pcz_path1: str, input_pcz_path2: str,
+                 output_json_path: str, properties: dict = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 
-                'input_pcz_path1': input_pcz_path1,
-                'input_pcz_path2': input_pcz_path2
-             },
-            'out': {    
-                'output_json_path': output_json_path
-            }
+            'in': {'input_pcz_path1': input_pcz_path1,
+                   'input_pcz_path2': input_pcz_path2},
+            'out': {'output_json_path': output_json_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.binary_path = properties.get('binary_path', 'pczdump')
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     # Check two eigenvectors to be compatible for dot product
     # i.e. same number of vectors and values per vector
-    def are_compatible (self,eigenvectors_1, eigenvectors_2): 
+    def are_compatible(self, eigenvectors_1, eigenvectors_2):
         # Check the number of eigenvectors and the number of values in both eigenvectors to match
         if len(eigenvectors_1) != len(eigenvectors_2):
             print('WARNING: Number of eigenvectors does not match')
             return False
         if len(eigenvectors_1[0]) != len(eigenvectors_2[0]):
             print('WARNING: Number of values in eigenvectors does not match')
             return False
         return True
 
     # Get the weighted cross product between eigenvectors
     # This is meant to compare PCA results for molecular dynamics structural conformations
     # The number of eigenvectors to be compared may be specified. All (0) by default
     # DISCLAIMER: This code has been translated from a perl script signed by Alberto Perez (13/09/04)
-    def get_similarity_index (self, 
-        eigenvalues_1, eigenvectors_1, 
-        eigenvalues_2, eigenvectors_2):
+    def get_similarity_index(self,
+                             eigenvalues_1, eigenvectors_1,
+                             eigenvalues_2, eigenvectors_2):
 
         amplifying_factor = 0
 
         # Check the number of eigenvectors and the number of values in both eigenvectors to match
         if not self.are_compatible(eigenvectors_1, eigenvectors_2):
             raise SystemExit('Eigenvectors are not compatible')
-        
+
         # Find out the total number of eigenvectors
         # Set the number of eigenvectors to be analyzed in case it is not set or it exceeds the total
-        eigenvectors_number = min(len(eigenvectors_1),len(eigenvectors_2))
+        eigenvectors_number = min(len(eigenvectors_1), len(eigenvectors_2))
 
         # Find out the number of atoms in the structure
         # Eigenvectors are atom coordinates and each atom has 3 coordinates (x, y, z)
         if len(eigenvectors_1[0]) % 3 != 0:
             raise SystemExit('Something is wrong with eigenvectors since number of values is not divisor of 3')
-        atom_number = int( len(eigenvectors_1[0]) / 3 )
+        atom_number = int(len(eigenvectors_1[0]) / 3)
 
         # Get the denominator
         cte1 = part1 = cte2 = part2 = 0
         for eigenvalue in eigenvalues_1:
             cte1 += exp(-1 / eigenvalue * amplifying_factor)
             part1 += exp(-2 / eigenvalue * amplifying_factor) ** 2
         for eigenvalue in eigenvalues_2:
             cte2 += exp(-1 / eigenvalue * amplifying_factor)
             part2 += exp(-2 / eigenvalue * amplifying_factor) ** 2
         denominator = part1 * cte2 * cte2 / cte1 / cte1 + part2 * cte1 * cte1 / cte2 / cte2
 
         # Get all eigenvector values together
-        eigenvector_values_1 = [ v for ev in eigenvectors_1 for v in ev ]
-        eigenvector_values_2 = [ v for ev in eigenvectors_2 for v in ev ]
+        eigenvector_values_1 = [v for ev in eigenvectors_1 for v in ev]
+        eigenvector_values_2 = [v for ev in eigenvectors_2 for v in ev]
 
         # IDK what it is doing now
         total_summatory = 0
         for i in range(eigenvectors_number):
             for j in range(eigenvectors_number):
-                #Array has vectors in increasing order of vap, get last one first
+                # Array has vectors in increasing order of vap, get last one first
                 a = (eigenvectors_number - 1 - i) * atom_number * 3
                 b = (eigenvectors_number - i) * atom_number * 3 - 1
                 c = (eigenvectors_number - 1 - j) * atom_number * 3
                 d = (eigenvectors_number - j) * atom_number * 3 - 1
                 temp1 = eigenvector_values_1[a:b]
                 temp2 = eigenvector_values_2[c:d]
                 if len(temp1) != len(temp2):
@@ -140,218 +139,244 @@
                 add = 0
                 for k, value_1 in enumerate(temp1):
                     value_2 = temp2[k]
                     add += value_1 * value_2
                 add = add * exp(-1 / eigenvalues_1[i] * amplifying_factor - 1 / eigenvalues_2[j] * amplifying_factor)
                 add2 = add ** 2
                 total_summatory += add2
-        
+
         similarity_index = total_summatory * 2 / denominator
         return similarity_index
 
     # Get the dot product matrix of two eigenvectors
-    def dot_product (self, eigenvectors_1, eigenvectors_2):
+    def dot_product(self, eigenvectors_1, eigenvectors_2):
         # Check the number of eigenvectors and the number of values in both eigenvectors to match
         if not self.are_compatible(eigenvectors_1, eigenvectors_2):
             raise SystemExit('Eigenvectors are not compatible')
-        # Get the number of eigenvectors
-        n_components = len(eigenvectors_1)
         # Get the dot product
         dpm = np.dot(eigenvectors_1, np.transpose(eigenvectors_2))
         return dpm
 
     # Get the subspace overlap
     # DANI: Es como el similarity index pero sin utilizar los eigenvalues y sin toda la parte de los weights, creo
-    def get_subspace_overlap (self, eigenvectors_1, eigenvectors_2):
+    def get_subspace_overlap(self, eigenvectors_1, eigenvectors_2):
         # Get the number of eigenvectors
         n_components = len(eigenvectors_1)
         # Get the dot product
         dpm = self.dot_product(eigenvectors_1, eigenvectors_2)
         print(dpm)
         sso = np.sqrt((dpm * dpm).sum() / n_components)
-        #sso = (dpm * dpm).sum() / n_components
+        # sso = (dpm * dpm).sum() / n_components
         return sso
 
-    def get_rwsip (self, 
-        eigenvalues_1, eigenvectors_1, 
-        eigenvalues_2, eigenvectors_2):
+    def get_rwsip(self,
+                  eigenvalues_1, eigenvectors_1,
+                  eigenvalues_2, eigenvectors_2):
 
         # Get the number of eigenvectors
         n_components = len(eigenvectors_1)
 
         accum = 0
         norm = 0
-        for pc in range(0,n_components):
+        for pc in range(0, n_components):
             dpm = np.dot(eigenvectors_1[pc], np.transpose(eigenvectors_2[pc]))
             val = dpm * dpm * eigenvalues_1[pc] * eigenvalues_2[pc]
             norm = norm + eigenvalues_1[pc] * eigenvalues_2[pc]
             accum = accum + val
 
         sso = np.sqrt(accum / norm)
-        #sso = (dpm * dpm).sum() / n_components
+        # sso = (dpm * dpm).sum() / n_components
         return sso
 
-
     @launchlogger
     def launch(self):
         """Launches the execution of the FlexServ pcz_similarity module."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
-        self.stage_files()
+        if self.check_restart():
+            return 0
+        # self.stage_files()
 
         # Internal file paths
-        try:
-            # Using rel paths to shorten the amount of characters due to fortran path length limitations
-            input_pcz_1 = str(Path(self.stage_io_dict["in"]["input_pcz_path1"]).relative_to(Path.cwd()))
-            input_pcz_2 = str(Path(self.stage_io_dict["in"]["input_pcz_path2"]).relative_to(Path.cwd()))
-            output_json = str(Path(self.stage_io_dict["out"]["output_json_path"]).relative_to(Path.cwd()))
-        except ValueError:
-            # Container or remote case
-            input_pcz = self.stage_io_dict["in"]["input_pcz_path"]
-            output_json = self.stage_io_dict["out"]["output_json_path"]
+        # try:
+        #     # Using rel paths to shorten the amount of characters due to fortran path length limitations
+        #     input_pcz_1 = str(Path(self.stage_io_dict["in"]["input_pcz_path1"]).relative_to(Path.cwd()))
+        #     input_pcz_2 = str(Path(self.stage_io_dict["in"]["input_pcz_path2"]).relative_to(Path.cwd()))
+        #     output_json = str(Path(self.stage_io_dict["out"]["output_json_path"]).relative_to(Path.cwd()))
+        # except ValueError:
+        #     # Container or remote case
+        #     output_json = self.stage_io_dict["out"]["output_json_path"]
+
+        # Manually creating a Sandbox to avoid issues with input parameters buffer overflow:
+        #   Long strings defining a file path makes Fortran or C compiled programs crash if the string
+        #   declared is shorter than the input parameter path (string) length.
+        #   Generating a temporary folder and working inside this folder (sandbox) fixes this problem.
+        #   The problem was found in Galaxy executions, launching Singularity containers (May 2023).
+
+        # Creating temporary folder
+        self.tmp_folder = fu.create_unique_dir()
+        fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
+
+        shutil.copy2(self.io_dict["in"]["input_pcz_path1"], self.tmp_folder)
+        shutil.copy2(self.io_dict["in"]["input_pcz_path2"], self.tmp_folder)
 
         # Temporary output
-        temp_out_1 = str(Path(self.stage_io_dict.get("unique_dir")).joinpath("output_1.dat"))
-        temp_out_2 = str(Path(self.stage_io_dict.get("unique_dir")).joinpath("output_2.dat"))
+        temp_json = "output.json"
+        temp_out_1 = "output1.dat"
+        temp_out_2 = "output2.dat"
 
         # Command line 1
         # pczdump -i structure.ca.std.pcz --evals -o evals.txt
-        self.cmd = [
-                # Evals pcz 1 
-                self.binary_path,
-                "-i", input_pcz_1,
-                "-o", temp_out_1,
-                "--evals", ';',
-                # Evals pcz 2
-                self.binary_path,
-                "-i", input_pcz_2,
-                "-o", temp_out_2,
-                "--evals"
-        ]
- 
+        # self.cmd = [self.binary_path,   # Evals pcz 1
+        #             "-i", input_pcz_1,
+        #             "-o", temp_out_1,
+        #             "--evals", ';',
+        #             self.binary_path,   # Evals pcz 2
+        #             "-i", input_pcz_2,
+        #             "-o", temp_out_2,
+        #             "--evals"
+        #             ]
+
+        self.cmd = ['cd', self.tmp_folder, ';',
+                    self.binary_path,    # Evals pcz 1
+                    "-i", PurePath(self.io_dict["in"]["input_pcz_path1"]).name,
+                    "-o", temp_out_1,
+                    "--evals", ';',
+                    self.binary_path,    # Evals pcz 2
+                    "-i", PurePath(self.io_dict["in"]["input_pcz_path2"]).name,
+                    "-o", temp_out_2,
+                    "--evals"
+                    ]
+
         # Run Biobb block 1
         self.run_biobb()
 
         # Parse output evals
         info_dict = {}
         info_dict['evals_1'] = []
         info_dict['evals_2'] = []
 
-        row = 0
-        with open (temp_out_1,'r') as file:
+        with open(PurePath(self.tmp_folder).joinpath(temp_out_1), 'r') as file:
             for line in file:
                 info = float(line.strip())
                 info_dict['evals_1'].append(info)
 
-        with open (temp_out_2,'r') as file:
+        with open(PurePath(self.tmp_folder).joinpath(temp_out_2), 'r') as file:
             for line in file:
                 info = float(line.strip())
-                info_dict['evals_2'].append(info)       
-       
+                info_dict['evals_2'].append(info)
+
         num_evals_1 = len(info_dict['evals_1'])
         num_evals_2 = len(info_dict['evals_2'])
-        num_evals_min = min(num_evals_1,num_evals_2)
+        num_evals_min = min(num_evals_1, num_evals_2)
         info_dict['num_evals_min'] = num_evals_min
 
         # Command line 2
         # pczdump -i structure.ca.std.pcz --evals -o evals.txt
         self.cmd = []
-        for pc in (range(1,num_evals_min+1)):
-            # Evecs pcz 1 
+        self.cmd.append('cd')
+        self.cmd.append(self.tmp_folder)
+        self.cmd.append(';')
+        for pc in (range(1, num_evals_min+1)):
+            # Evecs pcz 1
             self.cmd.append(self.binary_path)
             self.cmd.append("-i")
-            self.cmd.append(input_pcz_1)
-            #self.cmd.append("-o evecs_1_pc{}".format(pc))
+            # self.cmd.append(input_pcz_1)
+            self.cmd.append(PurePath(self.io_dict["in"]["input_pcz_path1"]).name)
+            # self.cmd.append("-o evecs_1_pc{}".format(pc))
             self.cmd.append("-o")
-            self.cmd.append(str(Path(self.stage_io_dict.get("unique_dir")).joinpath("evecs_1_pc{}".format(pc))))
+            # self.cmd.append(str(Path(self.stage_io_dict.get("unique_dir")).joinpath("evecs_1_pc{}".format(pc))))
+            self.cmd.append("evecs_1_pc{}".format(pc))
             self.cmd.append("--evec={}".format(pc))
             self.cmd.append(";")
             # Evals pcz 2
             self.cmd.append(self.binary_path)
             self.cmd.append("-i")
-            self.cmd.append(input_pcz_2)
-            #self.cmd.append("-o evecs_2_pc{}".format(pc))
+            # self.cmd.append(input_pcz_2)
+            self.cmd.append(PurePath(self.io_dict["in"]["input_pcz_path2"]).name)
+            # self.cmd.append("-o evecs_2_pc{}".format(pc))
             self.cmd.append("-o")
-            self.cmd.append(str(Path(self.stage_io_dict.get("unique_dir")).joinpath("evecs_2_pc{}".format(pc))))
+            # self.cmd.append(str(Path(self.stage_io_dict.get("unique_dir")).joinpath("evecs_2_pc{}".format(pc))))
+            self.cmd.append("evecs_2_pc{}".format(pc))
             self.cmd.append("--evec={}".format(pc))
             self.cmd.append(";")
 
         # Run Biobb block 2
         self.run_biobb()
 
         # Parse output evecs
         info_dict['evecs_1'] = {}
         info_dict['evecs_2'] = {}
         eigenvectors_1 = []
         eigenvectors_2 = []
-        for pc in (range(1,num_evals_min+1)):
+        for pc in (range(1, num_evals_min+1)):
             pc_id = "pc{}".format(pc)
             info_dict['evecs_1'][pc_id] = []
             info_dict['evecs_2'][pc_id] = []
-            with open (str(Path(self.stage_io_dict.get("unique_dir")).joinpath("evecs_1_pc{}".format(pc))),'r') as file:
+            # with open(str(Path(self.stage_io_dict.get("unique_dir")).joinpath("evecs_1_pc{}".format(pc))), 'r') as file:
+            with open(PurePath(self.tmp_folder).joinpath("evecs_1_pc{}".format(pc)), 'r') as file:
                 list_evecs = []
                 for line in file:
                     info = line.strip().split(' ')
                     for nums in info:
                         if nums:
                             list_evecs.append(float(nums))
                 info_dict['evecs_1'][pc_id] = list_evecs
                 eigenvectors_1.append(list_evecs)
 
-            with open (str(Path(self.stage_io_dict.get("unique_dir")).joinpath("evecs_2_pc{}".format(pc))),'r') as file:
+            # with open(str(Path(self.stage_io_dict.get("unique_dir")).joinpath("evecs_2_pc{}".format(pc))), 'r') as file:
+            with open(PurePath(self.tmp_folder).joinpath("evecs_2_pc{}".format(pc)), 'r') as file:
                 list_evecs = []
                 for line in file:
                     info = line.strip().split(' ')
                     for nums in info:
                         if nums:
                             list_evecs.append(float(nums))
                 info_dict['evecs_2'][pc_id] = list_evecs
                 eigenvectors_2.append(list_evecs)
-        
+
         simIndex = self.get_similarity_index(info_dict['evals_1'], eigenvectors_1, info_dict['evals_2'], eigenvectors_2)
         info_dict['similarityIndex'] = float("{:.3f}".format(simIndex))
         dotProduct = self.get_subspace_overlap(eigenvectors_1, eigenvectors_2)
-        #info_dict['similarityIndex_dotProduct'] = float("{:.3f}".format(dotProduct))
+        # info_dict['similarityIndex_dotProduct'] = float("{:.3f}".format(dotProduct))
         info_dict['similarityIndex_rmsip'] = float("{:.3f}".format(dotProduct))
         rwsip = self.get_rwsip(info_dict['evals_1'], eigenvectors_1, info_dict['evals_2'], eigenvectors_2)
         info_dict['similarityIndex_rwsip'] = float("{:.3f}".format(rwsip))
 
-        # convert into JSON:
-        y = json.dumps(info_dict)
-
-        ## the result is a JSON string:
-        print(json.dumps(info_dict, indent=4))
-
-        with open (output_json, 'w') as out_file:
+        with open(PurePath(self.tmp_folder).joinpath(temp_json), 'w') as out_file:
             out_file.write(json.dumps(info_dict, indent=4))
 
+        # Copy outputs from temporary folder to output path
+        shutil.copy2(PurePath(self.tmp_folder).joinpath(temp_json), PurePath(self.io_dict["out"]["output_json_path"]))
+
         # Copy files to host
-        self.copy_to_host()
+        # self.copy_to_host()
 
         # remove temporary folder(s)
         self.tmp_files.extend([
-            self.stage_io_dict.get("unique_dir")
+            # self.stage_io_dict.get("unique_dir"),
+            self.tmp_folder
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
+
 def pcz_similarity(input_pcz_path1: str, input_pcz_path2: str, output_json_path: str,
-            properties: dict = None, **kwargs) -> int:
+                   properties: dict = None, **kwargs) -> int:
     """Create :class:`PCZsimilarity <flexserv.pcasuite.pcz_similarity>`flexserv.pcasuite.PCZsimilarity class and
     execute :meth:`launch() <flexserv.pcasuite.pcz_similarity.launch>` method"""
 
-    return PCZsimilarity(  
-                    input_pcz_path1=input_pcz_path1,
-                    input_pcz_path2=input_pcz_path2,
-                    output_json_path=output_json_path,
-                    properties=properties).launch()
+    return PCZsimilarity(input_pcz_path1=input_pcz_path1,
+                         input_pcz_path2=input_pcz_path2,
+                         output_json_path=output_json_path,
+                         properties=properties).launch()
+
 
 def main():
     parser = argparse.ArgumentParser(description='Compute PCA Similarity from a given pair of compressed PCZ files.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
@@ -360,14 +385,15 @@
     required_args.add_argument('--output_json_path', required=True, help='Output json file with PCA similarity. Accepted formats: json.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call
-    pcz_similarity( input_pcz_path1=args.input_pcz_path1,
-                    input_pcz_path2=args.input_pcz_path2,
-                    output_json_path=args.output_json_path,
-                    properties=properties)
+    pcz_similarity(input_pcz_path1=args.input_pcz_path1,
+                   input_pcz_path2=args.input_pcz_path2,
+                   output_json_path=args.output_json_path,
+                   properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_flexserv-4.0.0/biobb_flexserv/pcasuite/pcz_stiffness.py` & `biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_bfactor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,187 +1,209 @@
 #!/usr/bin/env python3
 
-"""Module containing the PCZstiffness class and the command line interface."""
+"""Module containing the PCZbfactor class and the command line interface."""
 import argparse
-import json, math
-from pathlib import Path
+import shutil
+from pathlib import PurePath
+from biobb_common.tools import file_utils as fu
 from biobb_common.generic.biobb_object import BiobbObject
-from biobb_common.configuration import  settings
+from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
-class PCZstiffness(BiobbObject):
+
+class PCZbfactor(BiobbObject):
     """
-    | biobb_flexserv PCZstiffness
-    | Extract PCA stiffness from a compressed PCZ file.
+    | biobb_flexserv PCZbfactor
+    | Extract residue bfactors x PCA mode from a compressed PCZ file.
     | Wrapper of the pczdump tool from the PCAsuite FlexServ module.
 
     Args:
         input_pcz_path (str): Input compressed trajectory file. File type: input. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/data/pcasuite/pcazip.pcz>`_. Accepted formats: pcz (edam:format_3874).
-        output_json_path (str): Output json file with PCA Stiffness. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/reference/pcasuite/pcz_stiffness.json>`_. Accepted formats: json (edam:format_3464).
+        output_dat_path (str): Output Bfactor x residue x PCA mode file. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/reference/pcasuite/bfactors.dat>`_. Accepted formats: dat (edam:format_1637), txt (edam:format_2330), csv (edam:format_3752).
+        output_pdb_path (str) (Optional): Output PDB with Bfactor x residue x PCA mode file. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexserv/raw/master/biobb_flexserv/test/reference/pcasuite/bfactors.pdb>`_. Accepted formats: pdb (edam:format_1476).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
             * **binary_path** (*str*) - ("pczdump") pczdump binary path to be used.
-            * **eigenvector** (*int*) - (0) PCA mode (eigenvector) from which to extract stiffness.
-            * **temperature** (*int*) - (300) Temperature with which compute the apparent stiffness.
+            * **eigenvector** (*int*) - (0) PCA mode (eigenvector) from which to extract bfactor values per residue (0 means average over all modes).
+            * **pdb** (*bool*) - (False) Generate a PDB file with the computed bfactors (to be easily represented with colour scale)
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
-            from biobb_flexserv.pcasuite.pcz_stiffness import pcz_stiffness
-
+            from biobb_flexserv.pcasuite.pcz_bfactor import pcz_bfactor
             prop = {
-                'eigenvector': 1
+                'eigenvector': 1,
+                'pdb': True
             }
-
-            pcz_stiffness( input_pcz_path='/path/to/pcazip_input.pcz',
-                    output_json_path='/path/to/pcz_stiffness.json',
+            pcz_bfactor( input_pcz_path='/path/to/pcazip_input.pcz',
+                    output_dat_path='/path/to/bfactors_mode1.dat',
+                    output_pdb_path='/path/to/bfactors_mode1.pdb',
                     properties=prop)
 
     Info:
         * wrapped_software:
             * name: FlexServ PCAsuite
             * version: >=1.0
             * license: Apache-2.0
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
-    def __init__(self, input_pcz_path: str, 
-    output_json_path: str, properties: dict = None, **kwargs) -> None:
+    def __init__(self, input_pcz_path: str, output_dat_path: str,
+                 output_pdb_path: str, properties: dict = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': { 
-                'input_pcz_path': input_pcz_path
-             },
-            'out': {    
-                'output_json_path': output_json_path
-            }
+            'in': {'input_pcz_path': input_pcz_path},
+            'out': {'output_dat_path': output_dat_path,
+                    'output_pdb_path': output_pdb_path}
         }
 
         # Properties specific for BB
         self.properties = properties
         self.binary_path = properties.get('binary_path', 'pczdump')
-        self.eigenvector = properties.get('eigenvector', 0)
-        self.temperature = properties.get('temperature', 300)
+        self.eigenvector = properties.get('eigenvector', 1)
+        self.pdb = properties.get('pdb', False)
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     @launchlogger
     def launch(self):
-        """Launches the execution of the FlexServ pcz_stiffness module."""
+        """Launches the execution of the FlexServ pcz_bfactor module."""
 
         # Setup Biobb
-        if self.check_restart(): return 0
-        self.stage_files()
+        if self.check_restart():
+            return 0
+        # self.stage_files()
+
+        # # Internal file paths
+        # try:
+        #     # Using rel paths to shorten the amount of characters due to fortran path length limitations
+        #     input_pcz = str(Path(self.stage_io_dict["in"]["input_pcz_path"]).relative_to(Path.cwd()))
+        #     output_pdb = str(Path(self.stage_io_dict["out"]["output_pdb_path"]).relative_to(Path.cwd()))
+        #     output_dat = str(Path(self.stage_io_dict["out"]["output_dat_path"]).relative_to(Path.cwd()))
+        # except ValueError:
+        #     # Container or remote case
+        #     input_pcz = self.stage_io_dict["in"]["input_pcz_path"]
+        #     output_pdb = self.stage_io_dict["out"]["output_pdb_path"]
+        #     output_dat = self.stage_io_dict["out"]["output_dat_path"]
+
+        # Manually creating a Sandbox to avoid issues with input parameters buffer overflow:
+        #   Long strings defining a file path makes Fortran or C compiled programs crash if the string
+        #   declared is shorter than the input parameter path (string) length.
+        #   Generating a temporary folder and working inside this folder (sandbox) fixes this problem.
+        #   The problem was found in Galaxy executions, launching Singularity containers (May 2023).
+
+        # Creating temporary folder
+        self.tmp_folder = fu.create_unique_dir()
+        fu.log('Creating %s temporary folder' % self.tmp_folder, self.out_log)
+
+        shutil.copy2(self.io_dict["in"]["input_pcz_path"], self.tmp_folder)
+
+        # Command line (1: dat file)
+        # pczdump -i structure.ca.std.pcz --fluc=1 -o bfactor_1.dat
+        # self.cmd = [self.binary_path,
+        #             "-i", input_pcz,
+        #             "-o", output_dat,
+        #             "--bfactor",
+        #             "--fluc={}".format(self.eigenvector)
+        #             ]
+
+        self.cmd = ['cd', self.tmp_folder, ';',
+                    self.binary_path,
+                    '-i', PurePath(self.io_dict["in"]["input_pcz_path"]).name,
+                    '-o', PurePath(self.io_dict["out"]["output_dat_path"]).name,
+                    "--bfactor",
+                    "--fluc={}".format(self.eigenvector)
+                    ]
 
-        # Internal file paths
-        try:
-            # Using rel paths to shorten the amount of characters due to fortran path length limitations
-            input_pcz = str(Path(self.stage_io_dict["in"]["input_pcz_path"]).relative_to(Path.cwd()))
-            output_json = str(Path(self.stage_io_dict["out"]["output_json_path"]).relative_to(Path.cwd()))
-        except ValueError:
-            # Container or remote case
-            input_pcz = self.stage_io_dict["in"]["input_pcz_path"]
-            output_json = self.stage_io_dict["out"]["output_json_path"]
-
-        # Temporary output
-        temp_out = str(Path(self.stage_io_dict.get("unique_dir")).joinpath("output.dat"))
-
-        # Command line
-        # pczdump -i structure.ca.std.pcz --stiffness -o pcz.stiffness
-        self.cmd = [self.binary_path,
-                "-i", input_pcz,
-                "-o", temp_out,
-                "--stiff={}".format(self.eigenvector),
-                "--temperature={}".format(self.temperature)
-               ]
- 
         # Run Biobb block
         self.run_biobb()
 
-        # Parse output stiffness
-        info_dict = {}
-        info_dict['stiffness'] = []
-        info_dict['stiffness_log'] = []
-        row = 0
-        with open (temp_out,'r') as file:
-            for line in file:
-                info = line.strip().split(',')
-                line_array = []
-                line_array_log = []
-                for nums in info:
-                    if nums:
-                        line_array.append(float(nums))
-                        if float(nums) != 0:
-                            line_array_log.append(math.log10(float(nums)))
-                        else:
-                            line_array_log.append(float(nums))
-                                
-                info_dict['stiffness'].append(line_array)
-                info_dict['stiffness'][row][row] = float('inf')
-                info_dict['stiffness_log'].append(line_array_log)
-                info_dict['stiffness_log'][row][row] = float('inf')
-                row += 1
-       
-        # convert into JSON:
-        y = json.dumps(info_dict)
+        if self.pdb:
+            # Command line (2: pdb file)
+            # pczdump -i structure.ca.std.pcz --fluc=1 --pdb -o bfactor_1.pdb
+            # self.cmd = [self.binary_path,
+            #             "-i", input_pcz,
+            #             "-o", output_pdb,
+            #             "--bfactor",
+            #             "--fluc={}".format(self.eigenvector),
+            #             "--pdb"
+            #             ]
+
+            self.cmd = ['cd', self.tmp_folder, ';',
+                        self.binary_path,
+                        '-i', PurePath(self.io_dict["in"]["input_pcz_path"]).name,
+                        '-o', PurePath(self.io_dict["out"]["output_pdb_path"]).name,
+                        "--bfactor",
+                        "--fluc={}".format(self.eigenvector),
+                        "--pdb"
+                        ]
 
-        ## the result is a JSON string:
-        print(json.dumps(info_dict, indent=4))
+            # Run Biobb block
+            self.run_biobb()
 
-        with open (output_json, 'w') as out_file:
-            out_file.write(json.dumps(info_dict, indent=4))
+        # Copy outputs from temporary folder to output path
+        shutil.copy2(PurePath(self.tmp_folder).joinpath(PurePath(self.io_dict["out"]["output_dat_path"]).name), PurePath(self.io_dict["out"]["output_dat_path"]))
+
+        if self.pdb:
+            shutil.copy2(PurePath(self.tmp_folder).joinpath(PurePath(self.io_dict["out"]["output_pdb_path"]).name), PurePath(self.io_dict["out"]["output_pdb_path"]))
 
         # Copy files to host
-        self.copy_to_host()
+        # self.copy_to_host()
 
         # remove temporary folder(s)
         self.tmp_files.extend([
-            self.stage_io_dict.get("unique_dir")
+            # self.stage_io_dict.get("unique_dir"),
+            self.tmp_folder
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
-def pcz_stiffness(input_pcz_path: str, output_json_path: str,
-            properties: dict = None, **kwargs) -> int:
-    """Create :class:`PCZstiffness <flexserv.pcasuite.pcz_stiffness>`flexserv.pcasuite.PCZstiffness class and
-    execute :meth:`launch() <flexserv.pcasuite.pcz_stiffness.launch>` method"""
-
-    return PCZstiffness(  
-                    input_pcz_path=input_pcz_path,
-                    output_json_path=output_json_path,
-                    properties=properties).launch()
+
+def pcz_bfactor(input_pcz_path: str, output_dat_path: str, output_pdb_path: str,
+                properties: dict = None, **kwargs) -> int:
+    """Create :class:`PCZbfactor <flexserv.pcasuite.pcz_bfactor>`flexserv.pcasuite.PCZbfactor class and
+    execute :meth:`launch() <flexserv.pcasuite.pcz_bfactor.launch>` method"""
+
+    return PCZbfactor(input_pcz_path=input_pcz_path,
+                      output_dat_path=output_dat_path,
+                      output_pdb_path=output_pdb_path,
+                      properties=properties).launch()
+
 
 def main():
-    parser = argparse.ArgumentParser(description='Extract PCA Stiffness from a compressed PCZ file.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
+    parser = argparse.ArgumentParser(description='Extract residue bfactors x PCA mode from a compressed PCZ file.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
     required_args.add_argument('--input_pcz_path', required=True, help='Input compressed trajectory file. Accepted formats: pcz.')
-    required_args.add_argument('--output_json_path', required=True, help='Output json file with PCA stiffness. Accepted formats: json.')
+    required_args.add_argument('--output_dat_path', required=True, help='Output Bfactor x residue x PCA mode file. Accepted formats: dat, txt, csv.')
+    required_args.add_argument('--output_pdb_path', required=False, help='Output PDB with Bfactor x residue x PCA mode file. Accepted formats: pdb.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call
-    pcz_stiffness(  input_pcz_path=args.input_pcz_path,
-                    output_json_path=args.output_json_path,
-                    properties=properties)
+    pcz_bfactor(input_pcz_path=args.input_pcz_path,
+                output_dat_path=args.output_dat_path,
+                output_pdb_path=args.output_pdb_path,
+                properties=properties)
+
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_flexserv-4.0.0/biobb_flexserv.egg-info/PKG-INFO` & `biobb_flexserv-4.0.1/biobb_flexserv.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: biobb-flexserv
-Version: 4.0.0
+Version: 4.0.1
 Summary: biobb_flexserv is a BioBB category for biomolecular flexibility studies on protein 3D structures.
 Home-page: https://github.com/bioexcel/biobb_flexserv
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
 Project-URL: Documentation, http://biobb_flexserv.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `biobb_flexserv-4.0.0/biobb_flexserv.egg-info/SOURCES.txt` & `biobb_flexserv-4.0.1/biobb_flexserv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.0/biobb_flexserv.egg-info/entry_points.txt` & `biobb_flexserv-4.0.1/biobb_flexserv.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.0/setup.py` & `biobb_flexserv-4.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_flexserv",
-    version="4.0.0",
+    version="4.0.1",
     author="Biobb developers",
     author_email="adam.hospital@irbbarcelona.org",
     description="biobb_flexserv is a BioBB category for biomolecular flexibility studies on protein 3D structures.",
     long_description="biobb_flexserv allows the generation of protein conformational ensembles from 3D structures and the analysis of its molecular flexibility.",
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure",
     url="https://github.com/bioexcel/biobb_flexserv",
@@ -38,12 +38,14 @@
             "pcz_stiffness = biobb_flexserv.pcasuite.pcz_stiffness:main",
             "pcz_similarity = biobb_flexserv.pcasuite.pcz_similarity:main"
         ]
     },
     classifiers=(
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX",
     ),
 )
```

