# Comparing `tmp/biobb_flexdyn-4.0.2.tar.gz` & `tmp/biobb_flexdyn-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biobb_flexdyn-4.0.2.tar", last modified: Fri May 26 08:20:26 2023, max compression
+gzip compressed data, was "dist/biobb_flexdyn-4.0.3.tar", last modified: Wed May 31 08:52:51 2023, max compression
```

## Comparing `biobb_flexdyn-4.0.2.tar` & `biobb_flexdyn-4.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/
--rw-r--r--   0 gbayarri (1147421021) 1791188573    11357 2023-03-31 13:41:20.000000 biobb_flexdyn-4.0.2/LICENSE
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1104 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573     5623 2023-05-26 08:18:31.000000 biobb_flexdyn-4.0.2/README.md
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/biobb_flexdyn/
--rw-r--r--   0 gbayarri (1147421021) 1791188573       67 2023-05-26 08:18:18.000000 biobb_flexdyn-4.0.2/biobb_flexdyn/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/
--rw-r--r--   0 gbayarri (1147421021) 1791188573      128 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    15447 2023-05-26 08:00:28.000000 biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/concoord_disco.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573    11996 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/concoord_dist.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6914 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/imod_imc.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     5537 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/imod_imode.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6228 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/imod_imove.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6927 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/nolb_nma.py
--rwxr-xr-x   0 gbayarri (1147421021) 1791188573     6114 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/prody_anm.py
-drwxr-xr-x   0 gbayarri (1147421021) 1791188573        0 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/biobb_flexdyn.egg-info/
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1104 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/biobb_flexdyn.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) 1791188573      564 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/biobb_flexdyn.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573        1 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/biobb_flexdyn.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573      379 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/biobb_flexdyn.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       20 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/biobb_flexdyn.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       14 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/biobb_flexdyn.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) 1791188573       38 2023-05-26 08:20:26.000000 biobb_flexdyn-4.0.2/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) 1791188573     1963 2023-05-26 08:18:05.000000 biobb_flexdyn-4.0.2/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 08:52:51.000000 biobb_flexdyn-4.0.3/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11357 2023-03-31 13:41:20.000000 biobb_flexdyn-4.0.3/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1104 2023-05-31 08:52:51.000000 biobb_flexdyn-4.0.3/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5623 2023-05-31 08:52:09.000000 biobb_flexdyn-4.0.3/README.md
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 08:52:51.000000 biobb_flexdyn-4.0.3/biobb_flexdyn/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       67 2023-05-31 08:51:22.000000 biobb_flexdyn-4.0.3/biobb_flexdyn/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 08:52:51.000000 biobb_flexdyn-4.0.3/biobb_flexdyn/flexdyn/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      128 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.3/biobb_flexdyn/flexdyn/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    15447 2023-05-26 08:00:28.000000 biobb_flexdyn-4.0.3/biobb_flexdyn/flexdyn/concoord_disco.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11996 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.3/biobb_flexdyn/flexdyn/concoord_dist.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8421 2023-05-31 08:34:22.000000 biobb_flexdyn-4.0.3/biobb_flexdyn/flexdyn/imod_imc.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6938 2023-05-31 08:34:22.000000 biobb_flexdyn-4.0.3/biobb_flexdyn/flexdyn/imod_imode.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7724 2023-05-31 08:34:22.000000 biobb_flexdyn-4.0.3/biobb_flexdyn/flexdyn/imod_imove.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6927 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.3/biobb_flexdyn/flexdyn/nolb_nma.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     6114 2023-04-12 15:32:08.000000 biobb_flexdyn-4.0.3/biobb_flexdyn/flexdyn/prody_anm.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 08:52:51.000000 biobb_flexdyn-4.0.3/biobb_flexdyn.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1104 2023-05-31 08:52:51.000000 biobb_flexdyn-4.0.3/biobb_flexdyn.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      564 2023-05-31 08:52:51.000000 biobb_flexdyn-4.0.3/biobb_flexdyn.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-05-31 08:52:51.000000 biobb_flexdyn-4.0.3/biobb_flexdyn.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      379 2023-05-31 08:52:51.000000 biobb_flexdyn-4.0.3/biobb_flexdyn.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2023-05-31 08:52:51.000000 biobb_flexdyn-4.0.3/biobb_flexdyn.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       14 2023-05-31 08:52:51.000000 biobb_flexdyn-4.0.3/biobb_flexdyn.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-05-31 08:52:51.000000 biobb_flexdyn-4.0.3/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1963 2023-05-31 08:51:12.000000 biobb_flexdyn-4.0.3/setup.py
```

### Comparing `biobb_flexdyn-4.0.2/LICENSE` & `biobb_flexdyn-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.0.2/PKG-INFO` & `biobb_flexdyn-4.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobb_flexdyn
-Version: 4.0.2
+Version: 4.0.3
 Summary: biobb_flexdyn is a BioBB category for studies on the conformational landscape of native proteins.
 Home-page: https://github.com/bioexcel/biobb_flexdyn
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
 Project-URL: Documentation, http://biobb_flexdyn.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: 3D-Bioinfo ELIXIR FlexDyn Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure
```

### Comparing `biobb_flexdyn-4.0.2/README.md` & `biobb_flexdyn-4.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_flexdyn?label=Version)](https://GitHub.com/bioexcel/biobb_flexdyn/tags/)
 [![](https://img.shields.io/pypi/v/biobb-flexdyn.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-flexdyn/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_flexdyn?label=Conda)](https://anaconda.org/bioconda/biobb_flexdyn)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_flexdyn?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_flexdyn)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_flexdyn?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_flexdyn:4.0.2--pyhdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_flexdyn:4.0.3--pyhdfd78af_0)
 
 [![](https://img.shields.io/badge/OS-Unix%20%7C%20MacOS-blue)](https://github.com/bioexcel/biobb_flexdyn)
 [![](https://img.shields.io/pypi/pyversions/biobb-flexdyn.svg?label=Python%20Versions)](https://pypi.org/project/biobb-flexdyn/)
 [![](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![](https://img.shields.io/badge/Open%20Source%3f-Yes!-blue)](https://github.com/bioexcel/biobb_flexdyn)
 
 [![](https://readthedocs.org/projects/biobb-flexdyn/badge/?version=latest&label=Docs)](https://biobb-flexdyn.readthedocs.io/en/latest/?badge=latest)
@@ -30,60 +30,60 @@
 Biobb (BioExcel building blocks) packages are Python building blocks that
 create new layer of compatibility and interoperability over popular
 bioinformatics tools.
 The latest documentation of this package can be found in our readthedocs site:
 [latest API documentation](http://biobb_flexdyn.readthedocs.io/en/latest/).
 
 ### Version
-v4.0.2 2023.1
+v4.0.3 2023.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
 
-        pip install "biobb_flexdyn>=4.0.2"
+        pip install "biobb_flexdyn>=4.0.3"
 
 
 * Usage: [Python API documentation](https://biobb-flexdyn.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_flexdyn>=4.0.2"
+        conda install -c bioconda "biobb_flexdyn>=4.0.3"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-flexdyn.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-flexdyn.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_flexdyn:4.0.2--pyhdfd78af_0
+        docker pull quay.io/biocontainers/biobb_flexdyn:4.0.3--pyhdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_flexdyn:4.0.2--pyhdfd78af_0
+        docker run quay.io/biocontainers/biobb_flexdyn:4.0.3--pyhdfd78af_0
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_flexdyn.sif https://depot.galaxyproject.org/singularity/biobb_flexdyn:4.0.2--pyhdfd78af_0
+        singularity pull --name biobb_flexdyn.sif https://depot.galaxyproject.org/singularity/biobb_flexdyn:4.0.3--pyhdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_flexdyn.sif <command>
```

### Comparing `biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/concoord_disco.py` & `biobb_flexdyn-4.0.3/biobb_flexdyn/flexdyn/concoord_disco.py`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/concoord_dist.py` & `biobb_flexdyn-4.0.3/biobb_flexdyn/flexdyn/concoord_dist.py`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/imod_imc.py` & `biobb_flexdyn-4.0.3/biobb_flexdyn/flexdyn/imod_imode.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,165 +1,169 @@
 #!/usr/bin/env python3
 
 """Module containing the imode class and the command line interface."""
 import argparse
 import shutil
-from pathlib import Path
+from pathlib import PurePath
+from biobb_common.tools import file_utils as fu
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
 
-class ImodImc(BiobbObject):
+class ImodImode(BiobbObject):
     """
-    | biobb_flexdyn imod_imc
-    | Wrapper of the imc tool
-    | Compute a Monte-Carlo IC-NMA based conformational ensemble using the imc tool from the iMODS package.
+    | biobb_flexdyn imod_imode
+    | Wrapper of the imode tool
+    | Compute the normal modes of a macromolecule using the imode tool from the iMODS package.
 
     Args:
-        input_pdb_path (str): Input PDB file. File type: input. `Sample file <https://github.com/bioexcel/biobb_flexdyn/raw/master/biobb_flexdyn/test/data/flexdyn/structure_cleaned.pdb>`_. Accepted formats: pdb (edam:format_1476).
-        input_dat_path (str): Input dat with normal modes. File type: input. `Sample file <https://github.com/bioexcel/biobb_flexdyn/raw/master/biobb_flexdyn/test/data/flexdyn/imod_imode_evecs.dat>`_. Accepted formats: dat (edam:format_1637), txt (edam:format_2330).
-        output_traj_path (str): Output multi-model PDB file with the generated ensemble. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexdyn/raw/master/biobb_flexdyn/test/reference/flexdyn/imod_imc_output.pdb>`_. Accepted formats: pdb (edam:format_1476).
+        input_pdb_path (str): Input PDB file. File type: input. `Sample file <https://github.com/bioexcel/biobb_flexdyn/raw/master/biobb_flexdyn/test/data/flexdyn/structure.pdb>`_. Accepted formats: pdb (edam:format_1476).
+        output_dat_path (str): Output dat with normal modes. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexdyn/raw/master/biobb_flexdyn/test/reference/flexdyn/imod_imode_evecs.dat>`_. Accepted formats: dat (edam:format_1637), txt (edam:format_2330).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
-            * **num_structs** (*int*) - (500) Number of structures to be generated
-            * **num_modes** (*int*) - (5) Number of eigenvectors to be employed
-            * **amplitude** (*int*) - (1) Amplitude linear factor to scale motion
+            * **cg** (*int*) - (2) Coarse-Grained model. Values: 0 (CA), 1 (C5), 2 (Heavy atoms).
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
-            from biobb_flexdyn.flexdyn.imod_imc import imod_imc
+            from biobb_flexdyn.flexdyn.imod_imode import imod_imode
             prop = {
-                'num_structs' : 500
+                'cg' : 2
             }
-            imod_imc(   input_pdb_path='/path/to/structure.pdb',
-                          input_dat_path='/path/to/input_evecs.dat',
-                          output_traj_path='/path/to/output_ensemble.pdb',
-                          properties=prop)
+            imod_imode(   input_pdb_path='/path/to/structure.pdb',
+                    output_dat_path='/path/to/output_evecs.dat',
+                    properties=prop)
 
     Info:
         * wrapped_software:
             * name: iMODS
             * version: >=1.0.4
             * license: other
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
-    def __init__(self, input_pdb_path: str, input_dat_path: str, output_traj_path: str,
+    def __init__(self, input_pdb_path: str, output_dat_path: str,
                  properties: dict = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': {'input_pdb_path': input_pdb_path, 'input_dat_path': input_dat_path},
-            'out': {'output_traj_path': output_traj_path}
+            'in': {'input_pdb_path': input_pdb_path},
+            'out': {'output_dat_path': output_dat_path}
         }
 
         # Properties specific for BB
         self.properties = properties
-        self.binary_path = properties.get('binary_path', 'imc')
+        self.binary_path = properties.get('binary_path', 'imode_gcc')
 
-        self.num_structs = properties.get('num_structs', 500)
-        self.num_modes = properties.get('num_modes', 5)
-        self.amplitude = properties.get('amplitude', 1.0)
+        self.cg = properties.get('cg', 2)
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     @launchlogger
     def launch(self):
-        """Launches the execution of the FlexDyn iMOD imc module."""
+        """Launches the execution of the FlexDyn iMOD imode module."""
 
         # Setup Biobb
         if self.check_restart():
             return 0
-        self.stage_files()
+        # self.stage_files()
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
 
         # Output temporary file
-        out_file_prefix = Path(self.stage_io_dict.get("unique_dir")).joinpath("imod_ensemble")
-        out_file = Path(self.stage_io_dict.get("unique_dir")).joinpath("imod_ensemble.pdb")
+        # out_file_prefix = Path(self.stage_io_dict.get("unique_dir")).joinpath("imods_evecs")
+        # out_file = Path(self.stage_io_dict.get("unique_dir")).joinpath("imods_evecs_ic.evec")
+        out_file_prefix = "imods_evecs"  # Needed as imod is appending the _ic.evec extension
+        out_file = "imods_evecs_ic.evec"
 
         # Command line
-        # imc 1ake_backbone.pdb  1ake_backbone_evecs.dat -o 1ake_backbone.ensemble.pdb -c 500
-        self.cmd = [self.binary_path,
-                    str(Path(self.stage_io_dict["in"]["input_pdb_path"]).relative_to(Path.cwd())),
-                    str(Path(self.stage_io_dict["in"]["input_dat_path"]).relative_to(Path.cwd())),
-                    "-o", str(out_file_prefix)
+        # imode_gcc  1ake_backbone.pdb -m 0 -o patata.evec
+        # self.cmd = [self.binary_path,
+        #             str(Path(self.stage_io_dict["in"]["input_pdb_path"]).relative_to(Path.cwd())),
+        #             "-o", str(out_file_prefix),
+        #             "-m", str(self.cg)
+        #             ]
+
+        self.cmd = ['cd', self.tmp_folder, ';',
+                    self.binary_path,
+                    PurePath(self.io_dict["in"]["input_pdb_path"]).name,
+                    '-o', out_file_prefix,
+                    '-m', str(self.cg)
                     ]
 
-        # Properties
-        if self.num_structs:
-            self.cmd.append('-c')
-            self.cmd.append(str(self.num_structs))
-
-        if self.num_modes:
-            self.cmd.append('-n')
-            self.cmd.append(str(self.num_modes))
-
-        if self.amplitude:
-            self.cmd.append('-a')
-            self.cmd.append(str(self.amplitude))
-
         # Run Biobb block
         self.run_biobb()
 
         # Copying generated output file to the final (user-given) file name
-        shutil.copy2(out_file, self.stage_io_dict["out"]["output_traj_path"])
+        # shutil.copy2(out_file, self.stage_io_dict["out"]["output_dat_path"])
+
+        # Copy outputs from temporary folder to output path
+        shutil.copy2(PurePath(self.tmp_folder).joinpath(out_file), PurePath(self.io_dict["out"]["output_dat_path"]))
 
         # Copy files to host
-        self.copy_to_host()
+        # self.copy_to_host()
 
         # remove temporary folder(s)
         self.tmp_files.extend([
-            self.stage_io_dict.get("unique_dir")
+            # self.stage_io_dict.get("unique_dir")
+            self.tmp_folder
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
 
-def imod_imc(input_pdb_path: str, input_dat_path: str, output_traj_path: str,
-             properties: dict = None, **kwargs) -> int:
-    """Create :class:`ImodImc <flexdyn.imod_imc.ImodImc>`flexdyn.imod_imc.ImodImc class and
-    execute :meth:`launch() <flexdyn.imod_imc.ImodImc.launch>` method"""
-
-    return ImodImc(input_pdb_path=input_pdb_path,
-                   input_dat_path=input_dat_path,
-                   output_traj_path=output_traj_path,
-                   properties=properties).launch()
+def imod_imode(input_pdb_path: str, output_dat_path: str,
+               properties: dict = None, **kwargs) -> int:
+    """Create :class:`ImodImode <flexdyn.imod_imode.ImodImode>`flexdyn.imod_imode.ImodImode class and
+    execute :meth:`launch() <flexdyn.imod_imode.ImodImode.launch>` method"""
+
+    return ImodImode(input_pdb_path=input_pdb_path,
+                     output_dat_path=output_dat_path,
+                     properties=properties).launch()
 
 
 def main():
-    parser = argparse.ArgumentParser(description='Compute a Monte-Carlo IC-NMA based conformational ensemble using the imc tool from the iMODS package.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
+    parser = argparse.ArgumentParser(description='Compute the normal modes of a macromolecule using the imode tool from the iMODS package.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
     required_args.add_argument('--input_pdb_path', required=True, help='Input structure file. Accepted formats: pdb')
-    required_args.add_argument('--input_dat_path', required=True, help='Input evecs file. Accepted formats: dat')
-    required_args.add_argument('--output_traj_path', required=True, help='Output traj file. Accepted formats: pdb.')
+    required_args.add_argument('--output_dat_path', required=True, help='Output evecs dat file. Accepted formats: dat.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call
-    imod_imc(input_pdb_path=args.input_pdb_path,
-             input_dat_path=args.input_dat_path,
-             output_traj_path=args.output_traj_path,
-             properties=properties)
+    imod_imode(input_pdb_path=args.input_pdb_path,
+               output_dat_path=args.output_dat_path,
+               properties=properties)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/imod_imode.py` & `biobb_flexdyn-4.0.3/biobb_flexdyn/flexdyn/imod_imove.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,143 +1,175 @@
 #!/usr/bin/env python3
 
 """Module containing the imode class and the command line interface."""
 import argparse
 import shutil
-from pathlib import Path
+from pathlib import PurePath
+from biobb_common.tools import file_utils as fu
 from biobb_common.generic.biobb_object import BiobbObject
 from biobb_common.configuration import settings
 from biobb_common.tools.file_utils import launchlogger
 
 
-class ImodImode(BiobbObject):
+class ImodImove(BiobbObject):
     """
-    | biobb_flexdyn imod_imode
-    | Wrapper of the imode tool
-    | Compute the normal modes of a macromolecule using the imode tool from the iMODS package.
+    | biobb_flexdyn imod_imove
+    | Wrapper of the imove tool
+    | Compute the normal modes of a macromolecule using the imove tool from the iMODS package.
 
     Args:
-        input_pdb_path (str): Input PDB file. File type: input. `Sample file <https://github.com/bioexcel/biobb_flexdyn/raw/master/biobb_flexdyn/test/data/flexdyn/structure.pdb>`_. Accepted formats: pdb (edam:format_1476).
-        output_dat_path (str): Output dat with normal modes. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexdyn/raw/master/biobb_flexdyn/test/reference/flexdyn/imod_imode_evecs.dat>`_. Accepted formats: dat (edam:format_1637), txt (edam:format_2330).
+        input_pdb_path (str): Input PDB file. File type: input. `Sample file <https://github.com/bioexcel/biobb_flexdyn/raw/master/biobb_flexdyn/test/data/flexdyn/structure_cleaned.pdb>`_. Accepted formats: pdb (edam:format_1476).
+        input_dat_path (str): Input dat with normal modes. File type: input. `Sample file <https://github.com/bioexcel/biobb_flexdyn/raw/master/biobb_flexdyn/test/data/flexdyn/imod_imode_evecs.dat>`_. Accepted formats: dat (edam:format_1637), txt (edam:format_2330).
+        output_pdb_path (str): Output multi-model PDB file with the generated animation by Principal Component. File type: output. `Sample file <https://github.com/bioexcel/biobb_flexdyn/raw/master/biobb_flexdyn/test/reference/flexdyn/imod_imove_output.pdb>`_. Accepted formats: pdb (edam:format_1476).
         properties (dict - Python dictionary object containing the tool parameters, not input/output files):
-            * **cg** (*int*) - (2) Coarse-Grained model. Values: 0 (CA), 1 (C5), 2 (Heavy atoms).
+            * **pc** (*int*) - (1) Principal Component.
+            * **num_frames** (*int*) - (11) Number of frames to be generated
             * **remove_tmp** (*bool*) - (True) [WF property] Remove temporal files.
             * **restart** (*bool*) - (False) [WF property] Do not execute if output files exist.
 
     Examples:
         This is a use example of how to use the building block from Python::
 
-            from biobb_flexdyn.flexdyn.imod_imode import imod_imode
+            from biobb_flexdyn.flexdyn.imod_imove import imod_imove
             prop = {
-                'cg' : 2
+                'pc' : 1
             }
-            imod_imode(   input_pdb_path='/path/to/structure.pdb',
-                    output_dat_path='/path/to/output_evecs.dat',
-                    properties=prop)
+            imod_imove(   input_pdb_path='/path/to/structure.pdb',
+                          input_dat_path='/path/to/input_evecs.dat',
+                          output_pdb_path='/path/to/output_anim.pdb',
+                          properties=prop)
 
     Info:
         * wrapped_software:
             * name: iMODS
             * version: >=1.0.4
             * license: other
         * ontology:
             * name: EDAM
             * schema: http://edamontology.org/EDAM.owl
 
     """
-    def __init__(self, input_pdb_path: str, output_dat_path: str,
+    def __init__(self, input_pdb_path: str, input_dat_path: str, output_pdb_path: str,
                  properties: dict = None, **kwargs) -> None:
 
         properties = properties or {}
 
         # Call parent class constructor
         super().__init__(properties)
         self.locals_var_dict = locals().copy()
 
         # Input/Output files
         self.io_dict = {
-            'in': {'input_pdb_path': input_pdb_path},
-            'out': {'output_dat_path': output_dat_path}
+            'in': {'input_pdb_path': input_pdb_path, 'input_dat_path': input_dat_path},
+            'out': {'output_pdb_path': output_pdb_path}
         }
 
         # Properties specific for BB
         self.properties = properties
-        self.binary_path = properties.get('binary_path', 'imode_gcc')
+        self.binary_path = properties.get('binary_path', 'imove')
 
-        self.cg = properties.get('cg', 2)
+        self.pc = properties.get('pc', 1)
+        self.num_frames = properties.get('num_frames', 11)
 
         # Check the properties
         self.check_properties(properties)
         self.check_arguments()
 
     @launchlogger
     def launch(self):
-        """Launches the execution of the FlexDyn iMOD imode module."""
+        """Launches the execution of the FlexDyn iMOD imove module."""
 
         # Setup Biobb
         if self.check_restart():
             return 0
-        self.stage_files()
+        # self.stage_files()
 
-        # Output temporary file
-        out_file_prefix = Path(self.stage_io_dict.get("unique_dir")).joinpath("imods_evecs")
-        out_file = Path(self.stage_io_dict.get("unique_dir")).joinpath("imods_evecs_ic.evec")
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
+        shutil.copy2(self.io_dict["in"]["input_dat_path"], self.tmp_folder)
 
         # Command line
-        # imode_gcc  1ake_backbone.pdb -m 0 -o patata.evec
-        self.cmd = [self.binary_path,
-                    str(Path(self.stage_io_dict["in"]["input_pdb_path"]).relative_to(Path.cwd())),
-                    "-o", str(out_file_prefix),
-                    "-m", str(self.cg)
+        # imove 1ake_backbone.pdb  1ake_backbone_evecs.dat -o 1ake_backbone.ensemble.pdb 1 -c 500
+        # self.cmd = [self.binary_path,
+        #             str(Path(self.stage_io_dict["in"]["input_pdb_path"]).relative_to(Path.cwd())),
+        #             str(Path(self.stage_io_dict["in"]["input_dat_path"]).relative_to(Path.cwd())),
+        #             str(Path(self.stage_io_dict["out"]["output_pdb_path"]).relative_to(Path.cwd())),
+        #             str(self.pc)
+        #             ]
+
+        self.cmd = ['cd', self.tmp_folder, ';',
+                    self.binary_path,
+                    PurePath(self.io_dict["in"]["input_pdb_path"]).name,
+                    PurePath(self.io_dict["in"]["input_dat_path"]).name,
+                    PurePath(self.io_dict["out"]["output_pdb_path"]).name,
+                    str(self.pc)
                     ]
 
+        # Properties
+        if self.num_frames:
+            self.cmd.append('-c')
+            self.cmd.append(str(self.num_frames))
+
         # Run Biobb block
         self.run_biobb()
 
-        # Copying generated output file to the final (user-given) file name
-        shutil.copy2(out_file, self.stage_io_dict["out"]["output_dat_path"])
+        # Copy outputs from temporary folder to output path
+        shutil.copy2(PurePath(self.tmp_folder).joinpath(PurePath(self.io_dict["out"]["output_pdb_path"]).name), PurePath(self.io_dict["out"]["output_pdb_path"]))
 
         # Copy files to host
-        self.copy_to_host()
+        # self.copy_to_host()
 
         # remove temporary folder(s)
         self.tmp_files.extend([
-            self.stage_io_dict.get("unique_dir")
+            # self.stage_io_dict.get("unique_dir")
+            self.tmp_folder
         ])
         self.remove_tmp_files()
 
         self.check_arguments(output_files_created=True, raise_exception=False)
 
         return self.return_code
 
 
-def imod_imode(input_pdb_path: str, output_dat_path: str,
+def imod_imove(input_pdb_path: str, input_dat_path: str, output_pdb_path: str,
                properties: dict = None, **kwargs) -> int:
-    """Create :class:`ImodImode <flexdyn.imod_imode.ImodImode>`flexdyn.imod_imode.ImodImode class and
-    execute :meth:`launch() <flexdyn.imod_imode.ImodImode.launch>` method"""
+    """Create :class:`ImodImove <flexdyn.imod_imove.ImodImove>`flexdyn.imod_imove.ImodImove class and
+    execute :meth:`launch() <flexdyn.imod_imove.ImodImove.launch>` method"""
 
-    return ImodImode(input_pdb_path=input_pdb_path,
-                     output_dat_path=output_dat_path,
+    return ImodImove(input_pdb_path=input_pdb_path,
+                     input_dat_path=input_dat_path,
+                     output_pdb_path=output_pdb_path,
                      properties=properties).launch()
 
 
 def main():
-    parser = argparse.ArgumentParser(description='Compute the normal modes of a macromolecule using the imode tool from the iMODS package.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
+    parser = argparse.ArgumentParser(description='Animate the normal modes of a macromolecule using the imove tool from the iMODS package.', formatter_class=lambda prog: argparse.RawTextHelpFormatter(prog, width=99999))
     parser.add_argument('--config', required=False, help='Configuration file')
 
     # Specific args
     required_args = parser.add_argument_group('required arguments')
     required_args.add_argument('--input_pdb_path', required=True, help='Input structure file. Accepted formats: pdb')
-    required_args.add_argument('--output_dat_path', required=True, help='Output evecs dat file. Accepted formats: dat.')
+    required_args.add_argument('--input_dat_path', required=True, help='Input evecs file. Accepted formats: dat')
+    required_args.add_argument('--output_pdb_path', required=True, help='Output pdb file. Accepted formats: pdb.')
 
     args = parser.parse_args()
     args.config = args.config or "{}"
     properties = settings.ConfReader(config=args.config).get_prop_dic()
 
     # Specific call
-    imod_imode(input_pdb_path=args.input_pdb_path,
-               output_dat_path=args.output_dat_path,
+    imod_imove(input_pdb_path=args.input_pdb_path,
+               input_dat_path=args.input_dat_path,
+               output_pdb_path=args.output_pdb_path,
                properties=properties)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/nolb_nma.py` & `biobb_flexdyn-4.0.3/biobb_flexdyn/flexdyn/nolb_nma.py`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.0.2/biobb_flexdyn/flexdyn/prody_anm.py` & `biobb_flexdyn-4.0.3/biobb_flexdyn/flexdyn/prody_anm.py`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.0.2/biobb_flexdyn.egg-info/PKG-INFO` & `biobb_flexdyn-4.0.3/biobb_flexdyn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobb-flexdyn
-Version: 4.0.2
+Version: 4.0.3
 Summary: biobb_flexdyn is a BioBB category for studies on the conformational landscape of native proteins.
 Home-page: https://github.com/bioexcel/biobb_flexdyn
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
 Project-URL: Documentation, http://biobb_flexdyn.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: 3D-Bioinfo ELIXIR FlexDyn Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure
```

### Comparing `biobb_flexdyn-4.0.2/biobb_flexdyn.egg-info/SOURCES.txt` & `biobb_flexdyn-4.0.3/biobb_flexdyn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_flexdyn-4.0.2/setup.py` & `biobb_flexdyn-4.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_flexdyn",
-    version="4.0.2",
+    version="4.0.3",
     author="Biobb developers",
     author_email="adam.hospital@irbbarcelona.org",
     description="biobb_flexdyn is a BioBB category for studies on the conformational landscape of native proteins.",
     long_description="biobb_flexdyn allows the generation of protein conformational ensembles from 3D structures and the analysis of its molecular flexibility.",
     long_description_content_type="text/markdown",
     keywords="3D-Bioinfo ELIXIR FlexDyn Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure",
     url="https://github.com/bioexcel/biobb_flexdyn",
```

