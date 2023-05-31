# Comparing `tmp/biobb_flexserv-4.0.1.tar.gz` & `tmp/biobb_flexserv-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/biobb_flexserv-4.0.1.tar", last modified: Wed May 31 08:26:13 2023, max compression
+gzip compressed data, was "dist/biobb_flexserv-4.0.2.tar", last modified: Wed May 31 10:41:43 2023, max compression
```

## Comparing `biobb_flexserv-4.0.1.tar` & `biobb_flexserv-4.0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11357 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.1/LICENSE
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1082 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5896 2023-05-31 08:24:53.000000 biobb_flexserv-4.0.1/README.md
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/biobb_flexserv/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       81 2023-05-31 08:23:56.000000 biobb_flexserv-4.0.1/biobb_flexserv/__init__.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/biobb_flexserv/flexserv/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       61 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.1/biobb_flexserv/flexserv/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7209 2023-04-13 07:06:13.000000 biobb_flexserv-4.0.1/biobb_flexserv/flexserv/bd_run.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7677 2023-04-13 07:06:13.000000 biobb_flexserv-4.0.1/biobb_flexserv/flexserv/dmd_run.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7432 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/flexserv/nma_run.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      194 2023-04-13 07:06:13.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/__init__.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7497 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_animate.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9623 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_bfactor.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8126 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_collectivity.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8444 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_evecs.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    12583 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_hinges.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9331 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_info.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8036 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_lindemann.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    18293 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_similarity.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8807 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_stiffness.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7450 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_unzip.py
--rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8897 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_zip.py
-drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/biobb_flexserv.egg-info/
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1082 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/biobb_flexserv.egg-info/PKG-INFO
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      888 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/biobb_flexserv.egg-info/SOURCES.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/biobb_flexserv.egg-info/dependency_links.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      762 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/biobb_flexserv.egg-info/entry_points.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/biobb_flexserv.egg-info/requires.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       15 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/biobb_flexserv.egg-info/top_level.txt
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-05-31 08:26:13.000000 biobb_flexserv-4.0.1/setup.cfg
--rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2429 2023-05-31 08:23:38.000000 biobb_flexserv-4.0.1/setup.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    11357 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.2/LICENSE
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1082 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     5896 2023-05-31 10:41:05.000000 biobb_flexserv-4.0.2/README.md
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/biobb_flexserv/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       81 2023-05-31 10:40:45.000000 biobb_flexserv-4.0.2/biobb_flexserv/__init__.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/biobb_flexserv/flexserv/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       61 2023-03-31 13:36:44.000000 biobb_flexserv-4.0.2/biobb_flexserv/flexserv/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7209 2023-04-13 07:06:13.000000 biobb_flexserv-4.0.2/biobb_flexserv/flexserv/bd_run.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7677 2023-04-13 07:06:13.000000 biobb_flexserv-4.0.2/biobb_flexserv/flexserv/dmd_run.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7628 2023-05-31 10:38:32.000000 biobb_flexserv-4.0.2/biobb_flexserv/flexserv/nma_run.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      194 2023-04-13 07:06:13.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/__init__.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7497 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_animate.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9623 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_bfactor.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8126 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_collectivity.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8444 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_evecs.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    12583 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_hinges.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     9331 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_info.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8036 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_lindemann.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)    18293 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_similarity.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8807 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_stiffness.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     7450 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_unzip.py
+-rwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     8897 2023-05-31 08:02:59.000000 biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_zip.py
+drwxr-xr-x   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        0 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/biobb_flexserv.egg-info/
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     1082 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/biobb_flexserv.egg-info/PKG-INFO
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      888 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/biobb_flexserv.egg-info/SOURCES.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)        1 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/biobb_flexserv.egg-info/dependency_links.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)      762 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/biobb_flexserv.egg-info/entry_points.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       20 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/biobb_flexserv.egg-info/requires.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       15 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/biobb_flexserv.egg-info/top_level.txt
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)       38 2023-05-31 10:41:43.000000 biobb_flexserv-4.0.2/setup.cfg
+-rw-r--r--   0 gbayarri (1147421021) IRBBARCELONA\Domain Users (1791188573)     2429 2023-05-31 10:40:40.000000 biobb_flexserv-4.0.2/setup.py
```

### Comparing `biobb_flexserv-4.0.1/LICENSE` & `biobb_flexserv-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.1/PKG-INFO` & `biobb_flexserv-4.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobb_flexserv
-Version: 4.0.1
+Version: 4.0.2
 Summary: biobb_flexserv is a BioBB category for biomolecular flexibility studies on protein 3D structures.
 Home-page: https://github.com/bioexcel/biobb_flexserv
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
 Project-URL: Documentation, http://biobb_flexserv.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure
```

### Comparing `biobb_flexserv-4.0.1/README.md` & `biobb_flexserv-4.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![](https://img.shields.io/github/v/tag/bioexcel/biobb_flexserv?label=Version)](https://GitHub.com/bioexcel/biobb_flexserv/tags/)
 [![](https://img.shields.io/pypi/v/biobb-flexserv.svg?label=Pypi)](https://pypi.python.org/pypi/biobb-flexserv/)
 [![](https://img.shields.io/conda/vn/bioconda/biobb_flexserv?label=Conda)](https://anaconda.org/bioconda/biobb_flexserv)
 [![](https://img.shields.io/conda/dn/bioconda/biobb_flexserv?label=Conda%20Downloads)](https://anaconda.org/bioconda/biobb_flexserv)
 [![](https://img.shields.io/badge/Docker-Quay.io-blue)](https://quay.io/repository/biocontainers/biobb_flexserv?tab=tags)
-[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_flexserv:4.0.1--pypl5321hdfd78af_0)
+[![](https://img.shields.io/badge/Singularity-GalaxyProject-blue)](https://depot.galaxyproject.org/singularity/biobb_flexserv:4.0.2--pypl5321hdfd78af_0)
 
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
-v4.0.1 2023.1
+v4.0.2 2023.1
 
 ### Installation
 Using PIP:
 
 > **Important:** PIP only installs the package. All the dependencies must be installed separately. To perform a complete installation, please use ANACONDA or DOCKER.
 
 * Installation:
 
 
-        pip install "biobb_flexserv>=4.0.1"
+        pip install "biobb_flexserv>=4.0.2"
 
 
 * Usage: [Python API documentation](https://biobb-flexserv.readthedocs.io/en/latest/modules.html)
 
 Using ANACONDA:
 
 * Installation:
 
 
-        conda install -c bioconda "biobb_flexserv>=4.0.1"
+        conda install -c bioconda "biobb_flexserv>=4.0.2"
 
 
 * Usage: With conda installation BioBBs can be used with the [Python API documentation](https://biobb-flexserv.readthedocs.io/en/latest/modules.html) and the [Command Line documentation](https://biobb-flexserv.readthedocs.io/en/latest/command_line.html)
 
 Using DOCKER:
 
 * Installation:
 
 
-        docker pull quay.io/biocontainers/biobb_flexserv:4.0.1--pypl5321hdfd78af_0
+        docker pull quay.io/biocontainers/biobb_flexserv:4.0.2--pypl5321hdfd78af_0
 
 
 * Usage:
 
 
-        docker run quay.io/biocontainers/biobb_flexserv:4.0.1--pypl5321hdfd78af_0
+        docker run quay.io/biocontainers/biobb_flexserv:4.0.2--pypl5321hdfd78af_0
 
 Using SINGULARITY:
 
 **MacOS users**: it's strongly recommended to avoid Singularity and use **Docker** as containerization system.
 
 * Installation:
 
 
-        singularity pull --name biobb_flexserv.sif https://depot.galaxyproject.org/singularity/biobb_flexserv:4.0.1--pypl5321hdfd78af_0
+        singularity pull --name biobb_flexserv.sif https://depot.galaxyproject.org/singularity/biobb_flexserv:4.0.2--pypl5321hdfd78af_0
 
 
 * Usage:
 
 
         singularity exec biobb_flexserv.sif <command>
```

### Comparing `biobb_flexserv-4.0.1/biobb_flexserv/flexserv/bd_run.py` & `biobb_flexserv-4.0.2/biobb_flexserv/flexserv/bd_run.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.1/biobb_flexserv/flexserv/dmd_run.py` & `biobb_flexserv-4.0.2/biobb_flexserv/flexserv/dmd_run.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.1/biobb_flexserv/flexserv/nma_run.py` & `biobb_flexserv-4.0.2/biobb_flexserv/flexserv/nma_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,21 +98,27 @@
         # Command line
         # nmanu.pl structure.ca.pdb hessian.dat 1 0 40
         # diaghess
         # mc-eigen.pl eigenvec.dat > file.proj
         # pca_anim_mc.pl -pdb structure.ca.pdb -evec eigenvec.dat -i file.proj -n 50 -pout traj.crd
         conda_path = os.getenv("CONDA_PREFIX")
         nmanu = conda_path + "/bin/nmanu.pl"
+        nma_eigen = conda_path + "/bin/mc-eigen-mdweb.pl"
+        pca_anim = conda_path + "/bin/pca_anim_mc.pl"
         self.cmd = ["perl ",
                     nmanu,
                     input_pdb,
                     "hessian.dat 1 0 40;",
                     self.binary_path,
-                    "; mc-eigen-mdweb.pl eigenvec.dat ", str(self.frames), " > file.proj",
-                    "; pca_anim_mc.pl -pdb",
+                    "; perl",
+                    nma_eigen,
+                    "eigenvec.dat ", str(self.frames), " > file.proj",
+                    "; perl",
+                    pca_anim,
+                    "-pdb",
                     input_pdb,
                     " -evec eigenvec.dat -i file.proj -n ",
                     str(self.nvecs),
                     " -pout", output_crd,
                     '>', output_log
                     ]
```

### Comparing `biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_animate.py` & `biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_animate.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_bfactor.py` & `biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_bfactor.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_collectivity.py` & `biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_collectivity.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_evecs.py` & `biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_evecs.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_hinges.py` & `biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_hinges.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_info.py` & `biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_info.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_lindemann.py` & `biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_lindemann.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_similarity.py` & `biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_similarity.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_stiffness.py` & `biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_stiffness.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_unzip.py` & `biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_unzip.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.1/biobb_flexserv/pcasuite/pcz_zip.py` & `biobb_flexserv-4.0.2/biobb_flexserv/pcasuite/pcz_zip.py`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.1/biobb_flexserv.egg-info/PKG-INFO` & `biobb_flexserv-4.0.2/biobb_flexserv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biobb-flexserv
-Version: 4.0.1
+Version: 4.0.2
 Summary: biobb_flexserv is a BioBB category for biomolecular flexibility studies on protein 3D structures.
 Home-page: https://github.com/bioexcel/biobb_flexserv
 Author: Biobb developers
 Author-email: adam.hospital@irbbarcelona.org
 Project-URL: Documentation, http://biobb_flexserv.readthedocs.io/en/latest/
 Project-URL: Bioexcel, https://bioexcel.eu/
 Keywords: Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure
```

### Comparing `biobb_flexserv-4.0.1/biobb_flexserv.egg-info/SOURCES.txt` & `biobb_flexserv-4.0.2/biobb_flexserv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.1/biobb_flexserv.egg-info/entry_points.txt` & `biobb_flexserv-4.0.2/biobb_flexserv.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `biobb_flexserv-4.0.1/setup.py` & `biobb_flexserv-4.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="biobb_flexserv",
-    version="4.0.1",
+    version="4.0.2",
     author="Biobb developers",
     author_email="adam.hospital@irbbarcelona.org",
     description="biobb_flexserv is a BioBB category for biomolecular flexibility studies on protein 3D structures.",
     long_description="biobb_flexserv allows the generation of protein conformational ensembles from 3D structures and the analysis of its molecular flexibility.",
     long_description_content_type="text/markdown",
     keywords="Bioinformatics Workflows BioExcel Compatibility Flexibility Ensembles Protein Structure",
     url="https://github.com/bioexcel/biobb_flexserv",
```

