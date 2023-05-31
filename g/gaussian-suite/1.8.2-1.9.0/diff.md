# Comparing `tmp/gaussian_suite-1.8.2.tar.gz` & `tmp/gaussian_suite-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaussian_suite-1.8.2.tar", last modified: Thu Sep 15 12:01:27 2022, max compression
+gzip compressed data, was "gaussian_suite-1.9.0.tar", last modified: Thu Sep 15 15:55:08 2022, max compression
```

## Comparing `gaussian_suite-1.8.2.tar` & `gaussian_suite-1.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 12:01:27.449830 gaussian_suite-1.8.2/
--rw-rw-rw-   0 root         (0) root         (0)    35072 2022-09-15 12:01:03.000000 gaussian_suite-1.8.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3392 2022-09-15 12:01:27.449830 gaussian_suite-1.8.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2721 2022-09-15 12:01:03.000000 gaussian_suite-1.8.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 12:01:27.446834 gaussian_suite-1.8.2/gaussian_suite/
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-09-15 12:01:03.000000 gaussian_suite-1.8.2/gaussian_suite/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2022-09-15 12:01:24.000000 gaussian_suite-1.8.2/gaussian_suite/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)     2170 2022-09-15 12:01:03.000000 gaussian_suite-1.8.2/gaussian_suite/cd_extractor.py
--rw-rw-rw-   0 root         (0) root         (0)    22135 2022-09-15 12:01:03.000000 gaussian_suite-1.8.2/gaussian_suite/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     9265 2022-09-15 12:01:03.000000 gaussian_suite-1.8.2/gaussian_suite/extractor.py
--rw-rw-rw-   0 root         (0) root         (0)     9950 2022-09-15 12:01:03.000000 gaussian_suite-1.8.2/gaussian_suite/freq_extractor.py
--rw-rw-rw-   0 root         (0) root         (0)    22064 2022-09-15 12:01:03.000000 gaussian_suite-1.8.2/gaussian_suite/gen_input.py
--rw-rw-rw-   0 root         (0) root         (0)     2261 2022-09-15 12:01:03.000000 gaussian_suite-1.8.2/gaussian_suite/gen_job.py
--rw-rw-rw-   0 root         (0) root         (0)    10631 2022-09-15 12:01:03.000000 gaussian_suite-1.8.2/gaussian_suite/opt_extractor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 12:01:27.449830 gaussian_suite-1.8.2/gaussian_suite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3392 2022-09-15 12:01:27.000000 gaussian_suite-1.8.2/gaussian_suite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      528 2022-09-15 12:01:27.000000 gaussian_suite-1.8.2/gaussian_suite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-15 12:01:27.000000 gaussian_suite-1.8.2/gaussian_suite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2022-09-15 12:01:27.000000 gaussian_suite-1.8.2/gaussian_suite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       64 2022-09-15 12:01:27.000000 gaussian_suite-1.8.2/gaussian_suite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-09-15 12:01:27.000000 gaussian_suite-1.8.2/gaussian_suite.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      226 2022-09-15 12:01:03.000000 gaussian_suite-1.8.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-09-15 12:01:27.449830 gaussian_suite-1.8.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1440 2022-09-15 12:01:24.000000 gaussian_suite-1.8.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 15:55:08.643665 gaussian_suite-1.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35072 2022-09-15 15:54:36.000000 gaussian_suite-1.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3392 2022-09-15 15:55:08.642665 gaussian_suite-1.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2721 2022-09-15 15:54:36.000000 gaussian_suite-1.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 15:55:08.640665 gaussian_suite-1.9.0/gaussian_suite/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-09-15 15:54:36.000000 gaussian_suite-1.9.0/gaussian_suite/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2022-09-15 15:55:05.000000 gaussian_suite-1.9.0/gaussian_suite/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2170 2022-09-15 15:54:36.000000 gaussian_suite-1.9.0/gaussian_suite/cd_extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)    22312 2022-09-15 15:54:36.000000 gaussian_suite-1.9.0/gaussian_suite/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     9265 2022-09-15 15:54:36.000000 gaussian_suite-1.9.0/gaussian_suite/extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)     9950 2022-09-15 15:54:36.000000 gaussian_suite-1.9.0/gaussian_suite/freq_extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)    22064 2022-09-15 15:54:36.000000 gaussian_suite-1.9.0/gaussian_suite/gen_input.py
+-rw-rw-rw-   0 root         (0) root         (0)     2320 2022-09-15 15:54:36.000000 gaussian_suite-1.9.0/gaussian_suite/gen_job.py
+-rw-rw-rw-   0 root         (0) root         (0)    10631 2022-09-15 15:54:36.000000 gaussian_suite-1.9.0/gaussian_suite/opt_extractor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-15 15:55:08.642665 gaussian_suite-1.9.0/gaussian_suite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3392 2022-09-15 15:55:08.000000 gaussian_suite-1.9.0/gaussian_suite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      528 2022-09-15 15:55:08.000000 gaussian_suite-1.9.0/gaussian_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-15 15:55:08.000000 gaussian_suite-1.9.0/gaussian_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2022-09-15 15:55:08.000000 gaussian_suite-1.9.0/gaussian_suite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2022-09-15 15:55:08.000000 gaussian_suite-1.9.0/gaussian_suite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2022-09-15 15:55:08.000000 gaussian_suite-1.9.0/gaussian_suite.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      226 2022-09-15 15:54:36.000000 gaussian_suite-1.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-09-15 15:55:08.643665 gaussian_suite-1.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1440 2022-09-15 15:55:05.000000 gaussian_suite-1.9.0/setup.py
```

### Comparing `gaussian_suite-1.8.2/LICENSE` & `gaussian_suite-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gaussian_suite-1.8.2/PKG-INFO` & `gaussian_suite-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaussian_suite
-Version: 1.8.2
+Version: 1.9.0
 Summary: A package for working with Gaussian input and output files
 Home-page: https://gitlab.com/chilton-group/gaussian_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/gaussian_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/gaussian_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gaussian_suite-1.8.2/README.md` & `gaussian_suite-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `gaussian_suite-1.8.2/gaussian_suite/cd_extractor.py` & `gaussian_suite-1.9.0/gaussian_suite/cd_extractor.py`

 * *Files identical despite different names*

### Comparing `gaussian_suite-1.8.2/gaussian_suite/cli.py` & `gaussian_suite-1.9.0/gaussian_suite/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     ext = os.path.splitext(file_name)[1]
     if ext != extension:
         sys.exit("Incorrect file format provided!")
 
     return
 
 
-def generate_input_func(user_args, hpc_args):
+def generate_input_func(user_args):
     """
     Wrapper function for CLI gen_input call
 
     Parameters
     ----------
     user_args : argparser object
         User arguments
@@ -157,28 +157,28 @@
 
     Returns
     -------
     None
 
     """
 
+    # Get current machine name
     hpc_args = hpc.read_args(['generate_job'] + unknown_args)
-
     if hpc_args.profile == 'read_hostname':
         machine = parse_hostname()
     else:
         machine = hpc_args.profile
 
     supported_machines = [
         "csf3",
         "csf4"
     ]
 
     if machine not in supported_machines:
-        sys.exit("Error: Unsupported machine")
+        sys.exit("Error: Unsupported machine, perhaps try --profile")
 
     default_mod = {
         "csf3": "apps/binapps/gaussian/g16c01_em64t",
         "csf4": "gaussian/g16c01_em64t_detectcpu"
     }
 
     default_scratch = {
@@ -198,25 +198,31 @@
 
     # GB per core
     mem_multiplier = {
         "csf3": 4,
         "csf4": 4
     }
 
+    if hpc_args.node_type == "high_mem":
+        mem_multiplier = {
+            "csf3": 16,
+            "csf4": 16
+        }
+
     # Create submission script
     gen_job.create_submission_script(
         "{}.DATA".format(user_args.com_file_name[:-4]),
         user_args.n_cores,
         user_args.n_cores * mem_multiplier[machine],
-        machine,
         default_mod[machine],
         default_scratch[machine],
         default_chk[machine],
         default_version[machine],
         gen_fchk=not user_args.no_gen_fchk,
+        hpc_extra=unknown_args
     )
 
     return
 
 
 def coord_extractor_func(user_args):
     """
@@ -444,15 +450,15 @@
 
         # output array of charges, dip_x, dip_y, dip_z
         out_array = np.vstack([charges, np.array(dipoles).T]).T
 
         np.savetxt(
             out_name,
             out_array,
-            header="Charges (e), dipole_x (A e), dipole_y (A e), dipole_z (A e)",
+            header="Charges (e), dipole_x (A e), dipole_y (A e), dipole_z (A e)", # noqa
             fmt="% 7.5e"
         )
 
         print("Charges and dipoles are written to")
         print("{}".format(out_name))
 
     else:
@@ -884,15 +890,15 @@
     # which is assigned to help function
     parser.set_defaults(func=lambda user_args: parser.print_help())
 
     # read sub-parser
     _args, _ = parser.parse_known_args(arg_list)
 
     # select parsing option based on sub-parser
-    if _args.prog in ['extractor', 'gen_job', 'gen_input']:
+    if _args.prog in ['extractor', 'gen_job']:
         args, hpc_args = parser.parse_known_args(arg_list)
         args.func(args, hpc_args)
     else:
         args = parser.parse_args(arg_list)
         args.func(args)
     return
```

### Comparing `gaussian_suite-1.8.2/gaussian_suite/extractor.py` & `gaussian_suite-1.9.0/gaussian_suite/extractor.py`

 * *Files identical despite different names*

### Comparing `gaussian_suite-1.8.2/gaussian_suite/freq_extractor.py` & `gaussian_suite-1.9.0/gaussian_suite/freq_extractor.py`

 * *Files identical despite different names*

### Comparing `gaussian_suite-1.8.2/gaussian_suite/gen_input.py` & `gaussian_suite-1.9.0/gaussian_suite/gen_input.py`

 * *Files identical despite different names*

### Comparing `gaussian_suite-1.8.2/gaussian_suite/gen_job.py` & `gaussian_suite-1.9.0/gaussian_suite/gen_job.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,52 +3,51 @@
 for running Gaussian calculations
 """
 
 import os
 import hpc_suite as hpc
 
 
-def create_submission_script(f_name, n_cores, memory, machine, gaussian_module,
+def create_submission_script(f_name, n_cores, memory, gaussian_module,
                              gaussian_scratch, gaussian_chk, gaussian_version,
-                             gen_fchk=True):
+                             gen_fchk=True, hpc_extra=[""]):
     """
     Creates Gaussian submission script for HPC systems
 
     Parameters
     ----------
         f_name : str
             File name of .data file generated by create_data_file function
         n_cores : int
             Number of cores (threads) to request
         memory : int
             Total memory in gigabytes
-        machine : str {"SLURM", "SGE"}
-            Type of HPC system
         gaussian_module : str
             Path to Gaussian module for module load command
         gaussian_scratch : str
             Path to Gaussian scratch folder
         gaussian_chk : str
             Filename (with path to $CurrDir for CSF3) of checkpoint file
-        gaussian_version : str
+        gaussian_version : str {"$g16root/g16/g16", "$g9root/g9/g9"}
             version of Gaussian
         gen_fchk : bool, default True
             If true, generates formatted checkpoint file using `formchk`
             utility
+        hpc_extra : list[str], optional
+            String arguments to hpc_suite generate_job cli
 
     Returns
     -------
         None
     """
 
     f_head = os.path.splitext(f_name)[0]
 
-    args = hpc.read_args(['generate_job'])
+    args = hpc.read_args(['generate_job'] + hpc_extra)
 
-    args.profile = machine
     args.omp = n_cores
 
     # Set environmental variables
     args.env_vars["CurrDir"] = "$(pwd -P)"
     args.env_vars["JNAME"] = f_head
     args.env_vars["GAUSS_SCRDIR"] = gaussian_scratch
     args.env_vars["GAUSS_MDEF"] = "{:d}GB".format(memory)
```

### Comparing `gaussian_suite-1.8.2/gaussian_suite/opt_extractor.py` & `gaussian_suite-1.9.0/gaussian_suite/opt_extractor.py`

 * *Files identical despite different names*

### Comparing `gaussian_suite-1.8.2/gaussian_suite.egg-info/PKG-INFO` & `gaussian_suite-1.9.0/gaussian_suite.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaussian-suite
-Version: 1.8.2
+Version: 1.9.0
 Summary: A package for working with Gaussian input and output files
 Home-page: https://gitlab.com/chilton-group/gaussian_suite
 Author: Chilton Group
 Author-email: nicholas.chilton@manchester.ac.uk
 Project-URL: Bug Tracker, https://gitlab.com/chilton-group/gaussian_suite/-/issues
 Project-URL: Documentation, https://chilton-group.gitlab.io/gaussian_suite
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gaussian_suite-1.8.2/gaussian_suite.egg-info/SOURCES.txt` & `gaussian_suite-1.9.0/gaussian_suite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaussian_suite-1.8.2/setup.py` & `gaussian_suite-1.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 # DO NOT EDIT THIS NUMBER!
 # IT IS AUTOMATICALLY CHANGED BY python-semantic-release
-__version__ = "1.8.2"
+__version__ = "1.9.0"
 
 setuptools.setup(
     name='gaussian_suite',
     version=__version__,
     author='Chilton Group',
     author_email='nicholas.chilton@manchester.ac.uk',
     description='A package for working with Gaussian input and output files',
@@ -32,15 +32,15 @@
     packages=setuptools.find_packages(),
     python_requires='>=3.9',
     install_requires=[
         'numpy',
         'scipy',
         'xyz_py>=5.0.0',
         'requests',
-        'hpc_suite>=1.3.3',
+        'hpc_suite>=1.7.0',
         'deprecation'
         ],
     entry_points={
         'console_scripts': [
             'gaussian_suite = gaussian_suite.cli:main'
             ]
         }
```

